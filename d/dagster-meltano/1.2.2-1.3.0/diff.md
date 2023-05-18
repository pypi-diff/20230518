# Comparing `tmp/dagster_meltano-1.2.2.tar.gz` & `tmp/dagster_meltano-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_meltano-1.2.2.tar", max compression
+gzip compressed data, was "dagster_meltano-1.3.0.tar", max compression
```

## Comparing `dagster_meltano-1.2.2.tar` & `dagster_meltano-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/LICENSE
--rw-r--r--   0        0        0     2103 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/README.md
--rw-r--r--   0        0        0      313 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/__init__.py
--rw-r--r--   0        0        0       47 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/exceptions.py
--rw-r--r--   0        0        0     2187 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/generation.py
--rw-r--r--   0        0        0     1723 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/job.py
--rw-r--r--   0        0        0      592 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/logging.yaml
--rw-r--r--   0        0        0     5301 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/meltano_resource.py
--rw-r--r--   0        0        0     4040 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/ops.py
--rw-r--r--   0        0        0      859 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/schedule.py
--rw-r--r--   0        0        0     1011 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/dagster_meltano/utils.py
--rw-r--r--   0        0        0      646 2023-05-17 07:48:07.026474 dagster_meltano-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 dagster_meltano-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2103 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/README.md
+-rw-r--r--   0        0        0      313 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/exceptions.py
+-rw-r--r--   0        0        0     2348 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/generation.py
+-rw-r--r--   0        0        0     1856 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/job.py
+-rw-r--r--   0        0        0      592 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/logging.yaml
+-rw-r--r--   0        0        0     5855 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/meltano_resource.py
+-rw-r--r--   0        0        0     4040 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/ops.py
+-rw-r--r--   0        0        0      859 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/schedule.py
+-rw-r--r--   0        0        0     1011 2023-05-18 19:35:04.212015 dagster_meltano-1.3.0/dagster_meltano/utils.py
+-rw-r--r--   0        0        0      686 2023-05-18 19:35:04.216015 dagster_meltano-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 dagster_meltano-1.3.0/PKG-INFO
```

### Comparing `dagster_meltano-1.2.2/LICENSE` & `dagster_meltano-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.2/README.md` & `dagster_meltano-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.2/dagster_meltano/generation.py` & `dagster_meltano-1.3.0/dagster_meltano/generation.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 
 from dagster_meltano.meltano_resource import MeltanoResource
 from dagster_meltano.utils import generate_dbt_group_name
 
 
 def load_jobs_from_meltano_project(
     meltano_project_dir: Optional[str],
+    retries: int = 0,
 ) -> List[Union[JobDefinition, ScheduleDefinition]]:
     """This function generates dagster jobs for all jobs defined in the Meltano project. If there are schedules connected
     to the jobs, it also returns those.
 
     Args:
         project_dir (Optional[str], optional): The location of the Meltano project. Defaults to os.getenv("MELTANO_PROJECT_ROOT").
+        retries (int, optional): The number of retries to attempt if the Meltano CLI fails to run. Defaults to 0.
 
     Returns:
         List[Union[JobDefinition, ScheduleDefinition]]: Returns a list of either Dagster JobDefinitions or ScheduleDefinitions
     """
     meltano_resource = MeltanoResource(
         project_dir=meltano_project_dir,
         meltano_bin="meltano",
+        retries=retries,
     )
 
     meltano_jobs = meltano_resource.jobs
 
     return list(meltano_jobs)
```

### Comparing `dagster_meltano-1.2.2/dagster_meltano/job.py` & `dagster_meltano-1.3.0/dagster_meltano/job.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,26 @@
     JobDefinition,
     Nothing,
     OpDefinition,
     OpExecutionContext,
     get_dagster_logger,
     job,
     op,
+    RetryPolicy,
 )
 
 from dagster_meltano.ops import meltano_run_op as meltano_run_op_factory
 from dagster_meltano.utils import generate_dagster_name
 
 
 class Job:
-    def __init__(self, meltano_job: dict) -> None:
+    def __init__(self, meltano_job: dict, retries: int = 0) -> None:
         self.name = meltano_job["job_name"]
         self.tasks = meltano_job["tasks"]
+        self.retries = retries
 
     @property
     def dagster_name(self) -> str:
         return generate_dagster_name(self.name)
 
     def task_contains_tap(self, task: str) -> bool:
         """Check whether the supplied task contains a tap."""
@@ -36,14 +38,15 @@
         # We need to import the `meltano_resource` here to prevent circular imports.
         from dagster_meltano.meltano_resource import meltano_resource
 
         @job(
             name=self.dagster_name,
             description=f"Runs the `{self.name}` job from Meltano.",
             resource_defs={"meltano": meltano_resource},
+            op_retry_policy=RetryPolicy(max_retries=self.retries),
         )
         def dagster_job():
             op_layers = [[], []]
             previous_task_contains_tap = None
             for task in self.tasks:
                 meltano_run_op = meltano_run_op_factory(task)
                 current_task_contains_tap = self.task_contains_tap(task)
```

### Comparing `dagster_meltano-1.2.2/dagster_meltano/logging.yaml` & `dagster_meltano-1.3.0/dagster_meltano/logging.yaml`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.2/dagster_meltano/meltano_resource.py` & `dagster_meltano-1.3.0/dagster_meltano/meltano_resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,17 +14,23 @@
 from dagster_meltano.utils import Singleton
 from dagster_shell import execute_shell_command
 
 STDOUT = 1
 
 
 class MeltanoResource(metaclass=Singleton):
-    def __init__(self, project_dir: str = None, meltano_bin: Optional[str] = "meltano"):
+    def __init__(
+        self,
+        project_dir: str = None,
+        meltano_bin: Optional[str] = "meltano",
+        retries: int = 0,
+    ):
         self.project_dir = str(project_dir)
         self.meltano_bin = meltano_bin
+        self.retries = retries
 
     @property
     def default_env(self) -> Dict[str, str]:
         """The default environment to use when running Meltano commands.
 
         Returns:
             Dict[str, str]: The environment variables.
@@ -61,16 +67,14 @@
         )
 
         if exit_code != 0:
             raise MeltanoCommandError(
                 f"Command '{command}' failed with exit code {exit_code}"
             )
 
-        print(output)
-
         return output
 
     async def load_json_from_cli(self, command: List[str]) -> dict:
         """Use the Meltano CLI to load JSON data.
         Use asyncio to run multiple commands concurrently.
 
         Args:
@@ -114,15 +118,21 @@
         """
         jobs, schedules = asyncio.run(self.gather_meltano_yaml_information())
         return {"jobs": jobs["jobs"], "schedules": schedules["schedules"]}
 
     @cached_property
     def meltano_jobs(self) -> List[Job]:
         meltano_job_list = self.meltano_yaml["jobs"]
-        return [Job(meltano_job) for meltano_job in meltano_job_list]
+        return [
+            Job(
+                meltano_job=meltano_job,
+                retries=self.retries,
+            )
+            for meltano_job in meltano_job_list
+        ]
 
     @cached_property
     def meltano_schedules(self) -> List[Schedule]:
         meltano_schedule_list = self.meltano_yaml["schedules"]["job"]
         schedule_list = [
             Schedule(meltano_schedule) for meltano_schedule in meltano_schedule_list
         ]
@@ -142,21 +152,33 @@
 
 
 @resource(
     description="A resource that corresponds to a Meltano project.",
     config_schema={
         "project_dir": Field(
             str,
+            description="The path to the Meltano project.",
             default_value=os.getenv("MELTANO_PROJECT_ROOT", os.getcwd()),
             is_required=False,
-        )
+        ),
+        "retries": Field(
+            int,
+            description="The number of times to retry a failed job.",
+            default_value=0,
+            is_required=False,
+        ),
     },
 )
 def meltano_resource(init_context):
     project_dir = init_context.resource_config["project_dir"]
-    return MeltanoResource(project_dir)
+    retries = init_context.resource_config["retries"]
+
+    return MeltanoResource(
+        project_dir=project_dir,
+        retries=retries,
+    )
 
 
 if __name__ == "__main__":
     meltano_resource = MeltanoResource("/workspace/meltano")
     print(list(meltano_resource.jobs))
     print(meltano_resource.jobs)
```

### Comparing `dagster_meltano-1.2.2/dagster_meltano/ops.py` & `dagster_meltano-1.3.0/dagster_meltano/ops.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.2/dagster_meltano/schedule.py` & `dagster_meltano-1.3.0/dagster_meltano/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.2/dagster_meltano/utils.py` & `dagster_meltano-1.3.0/dagster_meltano/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.2/pyproject.toml` & `dagster_meltano-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "dagster-meltano"
-version = "1.2.2"
+version = "1.3.0"
 description = "A dagster plugin that allows you to run your Meltano project inside Dagster."
 authors = ["Jules Huisman"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "dagster_meltano" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-dagster = ">=1.0,<2"
+dagster = ">=1.3,<2"
 dagster-shell = ">=0,<1"
+sqlalchemy = "<2.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.15.9"
 pytest = "^7.2.0"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
 Homepage = "https://github.com/quantile-development/dagster-meltano"
```

### Comparing `dagster_meltano-1.2.2/PKG-INFO` & `dagster_meltano-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dagster-meltano
-Version: 1.2.2
+Version: 1.3.0
 Summary: A dagster plugin that allows you to run your Meltano project inside Dagster.
 License: Apache 2.0
 Author: Jules Huisman
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dagster (>=1.0,<2)
+Requires-Dist: dagster (>=1.3,<2)
 Requires-Dist: dagster-shell (>=0,<1)
+Requires-Dist: sqlalchemy (<2.0)
 Description-Content-Type: text/markdown
 
 # Dagster-meltano
 
 A dagster plugin that allows you to run Meltano using Dagster.
 
 [![Downloads](https://pepy.tech/badge/dagster-meltano/month)](https://pepy.tech/project/dagster-meltano)
```

