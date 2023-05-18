# Comparing `tmp/kannon-0.1.3.tar.gz` & `tmp/kannon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kannon-0.1.3.tar", max compression
+gzip compressed data, was "kannon-0.1.4.tar", max compression
```

## Comparing `kannon-0.1.3.tar` & `kannon-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-04-17 06:07:59.924958 kannon-0.1.3/LICENSE
--rw-r--r--   0        0        0     6109 2023-04-17 06:07:59.924958 kannon-0.1.3/README.md
--rw-r--r--   0        0        0       70 2023-04-17 06:07:59.924958 kannon-0.1.3/kannon/__init__.py
--rw-r--r--   0        0        0     1229 2023-04-17 06:07:59.924958 kannon-0.1.3/kannon/kube_util.py
--rw-r--r--   0        0        0     6858 2023-04-17 06:07:59.924958 kannon-0.1.3/kannon/master.py
--rw-r--r--   0        0        0       64 2023-04-17 06:07:59.924958 kannon-0.1.3/kannon/task.py
--rw-r--r--   0        0        0     1264 2023-04-17 06:08:14.869369 kannon-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6947 1970-01-01 00:00:00.000000 kannon-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-18 05:22:38.243355 kannon-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6109 2023-05-18 05:22:38.243355 kannon-0.1.4/README.md
+-rw-r--r--   0        0        0       70 2023-05-18 05:22:38.243355 kannon-0.1.4/kannon/__init__.py
+-rw-r--r--   0        0        0     1229 2023-05-18 05:22:38.243355 kannon-0.1.4/kannon/kube_util.py
+-rw-r--r--   0        0        0     7118 2023-05-18 05:22:38.243355 kannon-0.1.4/kannon/master.py
+-rw-r--r--   0        0        0       64 2023-05-18 05:22:38.243355 kannon-0.1.4/kannon/task.py
+-rw-r--r--   0        0        0     1248 2023-05-18 05:22:52.291572 kannon-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 kannon-0.1.4/PKG-INFO
```

### Comparing `kannon-0.1.3/LICENSE` & `kannon-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kannon-0.1.3/README.md` & `kannon-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kannon-0.1.3/kannon/kube_util.py` & `kannon-0.1.4/kannon/kube_util.py`

 * *Files identical despite different names*

### Comparing `kannon-0.1.3/kannon/master.py` & `kannon-0.1.4/kannon/master.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from collections import deque
 from copy import deepcopy
 from time import sleep
 from typing import Deque, Dict, List, Optional, Set
 
 import gokart
+from gokart.target import make_target
 from kubernetes import client
 from luigi.task import flatten
 
 from .kube_util import JobStatus, create_job, gen_job_name, get_job_status
 from .task import TaskOnBullet
 
 logger = logging.getLogger(__name__)
@@ -103,33 +104,35 @@
         # Run on master job
         try:
             gokart.build(task)
         except Exception:
             raise RuntimeError(f"Task {self._gen_task_info(task)} on job master has failed.")
 
     def _exec_bullet_task(self, task: TaskOnBullet) -> None:
+        # Save task instance as pickle object
+        pkl_path = self._gen_pkl_path(task)
+        make_target(pkl_path).dump(task)
         # Run on child job
-        serialized_task = gokart.TaskInstanceParameter().serialize(task)
         job_name = gen_job_name(f"{self.job_prefix}-{task.get_task_family()}")
         job = self._create_child_job_object(
             job_name=job_name,
-            serialized_task=serialized_task,
+            task_pkl_path=pkl_path,
         )
         create_job(self.api_instance, job, self.namespace)
         logger.info(f"Created child job {job_name} with task {self._gen_task_info(task)}")
         task_unique_id = task.make_unique_id()
         self.task_id_to_job_name[task_unique_id] = job_name
 
-    def _create_child_job_object(self, job_name: str, serialized_task: str) -> client.V1Job:
+    def _create_child_job_object(self, job_name: str, task_pkl_path: str) -> client.V1Job:
         # TODO: use python -c to avoid dependency to execute_task.py
         cmd = [
             "python",
             self.path_child_script,
-            "--serialized-task",
-            f"'{serialized_task}'",
+            "--task-pkl-path",
+            f"'{task_pkl_path}'",
         ]
         job = deepcopy(self.template_job)
         # replace command
         assert job.spec.template.spec.containers[0].command is None, \
             "command will be replaced by kannon, so you shouldn't set any command and args"
         job.spec.template.spec.containers[0].command = cmd
         # replace env
@@ -146,14 +149,18 @@
 
         return job
 
     @staticmethod
     def _gen_task_info(task: gokart.TaskOnKart) -> str:
         return f"{task.get_task_family()}_{task.make_unique_id()}"
 
+    @staticmethod
+    def _gen_pkl_path(task: gokart.TaskOnKart) -> str:
+        return os.path.join(task.workspace_directory, 'kannon', f'task_obj_{task.make_unique_id()}.pkl')
+
     def _is_executable(self, task: gokart.TaskOnKart) -> bool:
         children = flatten(task.requires())
 
         for child in children:
             if not child.complete():
                 return False
             if child.make_unique_id() not in self.task_id_to_job_name:
```

### Comparing `kannon-0.1.3/pyproject.toml` & `kannon-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kannon"
-version = "0.1.3"
+version = "0.1.4"
 description = "Kannon is a wrapper for the gokart library that allows gokart tasks to be easily executed in a distributed and parallel manner on multiple kubernetes jobs."
 authors = ["M3, inc."]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/m3dev/kannon"
 repository = "https://github.com/m3dev/kannon"
 
@@ -14,15 +14,14 @@
 style = "pep440"
 pattern = "^(?P<base>\\d+\\.\\d+\\.\\d+)"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 gokart = "^1.2.2"
 kubernetes = "^26.1.0"
-fire = "^0.5.0"
 
 [tool.poetry.group.dev.dependencies]
 pyproject-flake8 = "5.0.4"
 tox = "*"
 coverage = "*"
 isort = "^5.7"
 yapf = ">=0.32"
```

### Comparing `kannon-0.1.3/PKG-INFO` & `kannon-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: kannon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Kannon is a wrapper for the gokart library that allows gokart tasks to be easily executed in a distributed and parallel manner on multiple kubernetes jobs.
 Home-page: https://github.com/m3dev/kannon
 License: MIT
 Author: M3, inc.
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gokart (>=1.2.2,<2.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0)
 Project-URL: Repository, https://github.com/m3dev/kannon
 Description-Content-Type: text/markdown
 
 # kannon
```

