# Comparing `tmp/kedro-prefect-oliver-0.1.5.tar.gz` & `tmp/kedro-prefect-oliver-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-prefect-oliver-0.1.5.tar", last modified: Wed May 17 16:07:03 2023, max compression
+gzip compressed data, was "kedro-prefect-oliver-0.1.6.tar", last modified: Thu May 18 00:18:26 2023, max compression
```

## Comparing `kedro-prefect-oliver-0.1.5.tar` & `kedro-prefect-oliver-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4582 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/README
--rw-rw-rw-   0 root         (0) root         (0)     5684 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/infrastructure.py
--rw-rw-rw-   0 root         (0) root         (0)    13691 2023-05-17 16:06:43.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/register.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 16:07:03.007270 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-17 16:07:02.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-17 16:07:03.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-17 16:07:02.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-05-17 16:07:02.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-17 16:07:02.000000 kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-18 00:18:26.061203 kedro-prefect-oliver-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-18 00:18:07.000000 kedro-prefect-oliver-0.1.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-18 00:18:26.057203 kedro-prefect-oliver-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4582 2023-05-18 00:18:07.000000 kedro-prefect-oliver-0.1.6/README
+-rw-rw-rw-   0 root         (0) root         (0)     5684 2023-05-18 00:18:07.000000 kedro-prefect-oliver-0.1.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-18 00:18:26.061203 kedro-prefect-oliver-0.1.6/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-18 00:18:26.057203 kedro-prefect-oliver-0.1.6/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-18 00:18:26.057203 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-05-18 00:18:07.000000 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2023-05-18 00:18:07.000000 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver/infrastructure.py
+-rw-rw-rw-   0 root         (0) root         (0)    14380 2023-05-18 00:18:07.000000 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver/register.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-18 00:18:26.057203 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-18 00:18:26.000000 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-18 00:18:26.000000 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-18 00:18:26.000000 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-05-18 00:18:26.000000 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-18 00:18:26.000000 kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver.egg-info/top_level.txt
```

### Comparing `kedro-prefect-oliver-0.1.5/LICENSE` & `kedro-prefect-oliver-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.5/PKG-INFO` & `kedro-prefect-oliver-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.5
+Version: 0.1.6
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kedro-prefect-oliver-0.1.5/README` & `kedro-prefect-oliver-0.1.6/README`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.5/pyproject.toml` & `kedro-prefect-oliver-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name =  "kedro-prefect-oliver"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     {name = "Oliver OTL", email = "dev@olivetreeholdings.com"},
 ]
 description = "Kedro-Prefect integration library"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/infrastructure.py` & `kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver/infrastructure.py`

 * *Files identical despite different names*

### Comparing `kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver/register.py` & `kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver/register.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,15 +180,17 @@
         name="init_task",
     )
 
     return {"init_task": init_task, "tasks": tasks}
 
 
 @flow(task_runner=SequentialTaskRunner(), validate_parameters=False, log_prints=False)
-def create_pipeline(pipeline_name: str, env: str) -> None:
+def create_pipeline(
+    pipeline_name: str, env: str, task_retries: int, task_retry_delay: int
+) -> None:
     """Create a Prefect flow from a Kedro pipeline."""
 
     kedro_tasks = init_kedro_nodes(pipeline_name, env)
     init_task = kedro_tasks["init_task"]
     tasks = kedro_tasks["tasks"]
 
     run_kedro_init_task = run_kedro_task.with_options(name=init_task.name)
@@ -202,15 +204,19 @@
         ready = {
             node
             for node in todo_nodes
             if set(task_dependencies[node]) <= submitted_tasks.keys()
         }
         todo_nodes -= ready
         for node in ready:
-            run_kedro_node_task = run_kedro_task.with_options(name=node.name)
+            run_kedro_node_task = run_kedro_task.with_options(
+                name=node.name,
+                retries=task_retries,
+                retry_delay_seconds=task_retry_delay,
+            )
             future = run_kedro_node_task.submit(
                 node,
                 task_dict,
                 wait_for=[submitted_tasks[t] for t in task_dependencies[node]],
             )
             submitted_tasks[node] = future
 
@@ -286,14 +292,16 @@
     dev: bool = False,
     interval: float = None,
     anchor_date: str = None,
     rrule_string: str = None,
     cron_string: str = None,
     day_or: bool = True,
     timezone: str = "America/New_York",
+    task_retries: int = 0,
+    task_retry_delay: int = 0,
 ) -> None:
     """Deploy a Kedro pipeline as a Prefect flow."""
 
     kedro_pipeline = kedro_pipeline or "__default__"
     # get the dependencies and installs
     requires = None
     if dev:
@@ -316,15 +324,20 @@
     gcs_block_name = gcs_path.replace("/", "-")
     gcs_block = GCS(bucket_path=bucket + "/" + gcs_path, project=project)
     gcs_block.save(gcs_block_name, overwrite=True)
 
     job_name = f"{kedro_package.replace('_', '-')}-kubernetes-job"
     kubernetes_job = KubernetesJob.load(job_name)
 
-    parameters = {"pipeline_name": kedro_pipeline, "env": env}
+    parameters = {
+        "pipeline_name": kedro_pipeline,
+        "env": env,
+        "task_retries": task_retries,
+        "task_retry_delay": task_retry_delay,
+    }
 
     deployment = Deployment.build_from_flow(
         entrypoint=entrypoint,
         flow=create_pipeline.with_options(
             name=f"{kedro_package}.{kedro_pipeline}", version=version
         ),
         name="kubernetes-job",
@@ -391,14 +404,26 @@
 )
 @click.option(
     "--timezone",
     type=str,
     default="America/New_York",
     help="Deployment schedule timezone",
 )
+@click.option(
+    "--task_retries",
+    type=int,
+    default=0,
+    help="Number of times to retry a task if it fails",
+)
+@click.option(
+    "--task_retry_delay",
+    type=int,
+    default=0,
+    help="Number of seconds to wait between task retries",
+)
 def deploy_prefect_flow(
     project: str,
     entrypoint: str,
     bucket: str,
     kedro_package: str,
     kedro_pipeline: str,
     tags: List[str],
@@ -406,14 +431,16 @@
     dev: bool,
     interval: float,
     anchor_date: str,
     rrule: str,
     cron: str,
     day_or: bool,
     timezone: str,
+    task_retries: int,
+    task_retry_delay: int,
 ) -> None:
     deploy_flow(
         project,
         entrypoint,
         bucket,
         kedro_package,
         kedro_pipeline,
@@ -422,14 +449,16 @@
         dev,
         interval,
         anchor_date,
         rrule,
         cron,
         day_or,
         timezone,
+        task_retries,
+        task_retry_delay,
     )
 
 
 if __name__ == "__main__":
     print("Deploying Prefect flow...")
     # Standalone mode is false to make the function callable from other scripts
     # Standalone mode is a click parameter
```

### Comparing `kedro-prefect-oliver-0.1.5/src/kedro_prefect_oliver.egg-info/PKG-INFO` & `kedro-prefect-oliver-0.1.6/src/kedro_prefect_oliver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-prefect-oliver
-Version: 0.1.5
+Version: 0.1.6
 Summary: Kedro-Prefect integration library
 Author-email: Oliver OTL <dev@olivetreeholdings.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

