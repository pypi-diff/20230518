# Comparing `tmp/integrate-ai-0.0.42.tar.gz` & `tmp/integrate-ai-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integrate_ai-0.0.42.tar", max compression
+gzip compressed data, was "integrate-ai-9.5.0.tar", last modified: Wed May 17 20:51:48 2023, max compression
```

## Comparing `integrate-ai-0.0.42.tar` & `integrate-ai-9.5.0.tar`

### file list

```diff
@@ -1,18 +1,29 @@
--rw-r--r--   0        0        0       58 2023-02-10 16:24:07.727183 integrate_ai-0.0.42/LICENSE
--rw-r--r--   0        0        0      794 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/README.md
--rw-r--r--   0        0        0      762 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/__init__.py
--rw-r--r--   0        0        0      657 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/cli.py
--rw-r--r--   0        0        0    20244 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/client.py
--rw-r--r--   0        0        0     1081 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/main.py
--rw-r--r--   0        0        0     2693 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/sdk.py
--rw-r--r--   0        0        0     5651 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/server.py
--rw-r--r--   0        0        0        0 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/utils/__init__.py
--rw-r--r--   0        0        0     8301 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/utils/docker_client.py
--rw-r--r--   0        0        0     1138 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/utils/error_handling.py
--rw-r--r--   0        0        0      664 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/utils/logger.py
--rw-r--r--   0        0        0      859 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/utils/path_utils.py
--rw-r--r--   0        0        0     6025 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/utils/rest_client.py
--rw-r--r--   0        0        0     2840 2023-02-10 16:24:07.731183 integrate_ai-0.0.42/src/integrate_ai/utils/typer_utils.py
--rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 integrate_ai-0.0.42/setup.py
--rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 integrate_ai-0.0.42/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/backend_shim.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:48.920935 integrate-ai-9.5.0/integrate_ai/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20910 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/sdk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/integrate_ai/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8291 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/docker_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/error_handling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/path_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6025 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/rest_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2840 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/typer_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/integrate_ai.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1753 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/setup.py
```

### Comparing `integrate_ai-0.0.42/README.md` & `integrate-ai-9.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: integrate-ai
+Version: 9.5.0
+Summary: integrate.ai
+Author: integrate.ai
+License: Copyright (C) 2022 integrate.ai, Inc. All rights reserved.
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7.5
+Description-Content-Type: text/markdown
+
 # integrate.ai Command Line Interface
 
 A CLI that enables users to interact with integrate.ai's software.
 
 This tool allows users to manage client and sdk packages. Use the integate.ai sdk to seamlessly integrate federated learning and analytics workflows directly into your product.
 
 ## Installation
```

### Comparing `integrate_ai-0.0.42/src/integrate_ai/cli.py` & `integrate-ai-9.5.0/integrate_ai/cli.py`

 * *Files identical despite different names*

### Comparing `integrate_ai-0.0.42/src/integrate_ai/client.py` & `integrate-ai-9.5.0/integrate_ai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,20 +103,22 @@
             rprint("`No` response received. Exiting...")
             raise typer.Exit(0)
 
     # login and pull docker image
     with Progress(SpinnerColumn(), TextColumn("[progress.description]{task.description}")) as progress:
         p = progress.add_task(description="Logging into docker repo...", total=1)
         login_result = docker_client.login()
+        assert login_result
         progress.update(task_id=p, completed=True)
         p = progress.add_task(
             description=f"Pulling docker image {version_to_pull}. This will take a few minutes...",
             total=1,
         )
         pull_result = docker_client.pull(repo=docker_client.get_repo_name(), tag=version_to_pull)
+        assert pull_result
         progress.update(task_id=p, completed=True)
         rprint(f"Image {version_to_pull} is now available.")
         raise typer.Exit(0)
 
 
 @app.command()
 def version(
@@ -335,14 +337,44 @@
 
     container = docker_client.get_container(container_name)
     environment = get_aws_env(dataset_path)
 
     excute_command_and_close_docker(container, cmd, environment, local_log_path, remove_after_complete, verbose)
 
 
+def _get_image_name(docker_client):
+    """
+    Get image name used to spin up fl-client.
+    If `IAI_ALT_DOCKER_IMAGE_NAME` is set, use the given image name, otherwise read the latest version exist in fl-client repo.
+    Args:
+        docker_client (DockerClient): A DockerClient object
+    Returns:
+        image_name (str): image name for fl-client
+
+    """
+    image_name = os.environ.get("IAI_ALT_DOCKER_IMAGE_NAME")
+    if image_name:
+        rich.print(f"Using image {image_name}")
+        return image_name
+
+    current_images = docker_client.get_local_versions(docker_client.get_repo_name())
+    latest_version = docker_client.get_latest_version_of_image(current_images)
+
+    if len(current_images) == 0:
+        rich.print("No client image found on system.")
+        rich.print("Exiting...")
+        raise typer.Exit(0)
+
+    image_name = f"{docker_client.get_repo_name()}"
+    if latest_version:
+        image_name += ":" + latest_version
+
+    return image_name
+
+
 def mount_and_start_docker(docker_client: DockerClient, container_name: str, session: str, command: str, **kwargs):
     """Mount data paths to docker and start docker container
 
     Args:
         docker_client (DockerClient): A DockerClient object
         container_name (str): Name of the container
         session (str): Session id
@@ -352,29 +384,18 @@
             test_path (Dict): Testing data path for train command
             dataset_path (Dict): Data path for eda command
 
     Returns:
         mounted_data_path (Dict): Mounted data path
         local_log_path (str): Full path to the client log file
     """
-    current_images = docker_client.get_local_versions(docker_client.get_repo_name())
-    latest_version = docker_client.get_latest_version_of_image(current_images)
-
     mount_path = "/root/"
+    image_name = _get_image_name(docker_client)
 
-    if len(current_images) == 0:
-        rich.print("No client image found on system.")
-        rich.print("Exiting...")
-        raise typer.Exit(0)
-
-    image_name = f"{docker_client.get_repo_name()}"
-    if latest_version:
-        image_name += ":" + latest_version
-
-    ## Adding a conatiner path for logging, this is mounted later
+    # Adding a container path for logging, this is mounted later
 
     session_log_folder, local_log_path = get_log_paths(client_name=container_name, session=session)
     container_log_path = mount_path + f"iai/logs/{container_name}.log"
 
     # Create full path to log file if it does not exist
     os.makedirs(session_log_folder, exist_ok=True)
     # Creates an empty file
@@ -397,14 +418,15 @@
                     "tty": True,
                     "name": container_name,
                     "volumes": volumes,
                     "environment": {"IAI_LOG_SAVE_PATH": container_log_path},
                     "extra_hosts": {"localhost": "host-gateway"},
                 },
             )
+            assert response
         except Exception as e:
             progress.console.print(e, style="red")
             raise typer.Exit(0)
 
         progress.update(task_id=start_container_task, completed=True)
         progress.console.print(f"Container {container_name} is started.", style="green")
     return mounted_data_path, local_log_path
@@ -491,15 +513,15 @@
         remove_after_complete: Remove the container after complete when equals True
         verbose: Log verbose for container
 
     """
     set_env_var(environment, "IAI_DEBUG_LOCAL_GATEWAY")
     set_env_var(environment, "IAI_FLOUR_LOG_LEVEL")
     with Progress(SpinnerColumn(), TextColumn("[progress.description]{task.description}")) as progress:
-        task = progress.add_task(description=f"Processing...", total=1)
+        task = progress.add_task(description="Processing...", total=1)
         response = container.exec_run(
             cmd,
             stdout=verbose,
             stream=True,
             demux=True,
             environment=environment,
         )
@@ -508,19 +530,19 @@
                 if error:
                     progress.console.print(error.decode("utf-8"))
                 else:
                     progress.console.print(output.decode("utf-8"))
 
         progress.update(task_id=task, completed=True)
 
-    progress.console.print(f"Finished processing.", style="green")
-    progress.console.print(f"Logs are saved in {local_log_path} and can be found with iai client log", style="blue")
+    progress.console.print("Finished processing.", style="green")
+    progress.console.print("Logs are saved in {local_log_path} and can be found with iai client log", style="blue")
 
     with Progress(SpinnerColumn(), TextColumn("[progress.description]{task.description}")) as progress:
-        closing_task = progress.add_task(description=f"Closing container...", total=1)
+        closing_task = progress.add_task(description="Closing container...", total=1)
         container.stop()
         if remove_after_complete:
             container.remove()
         progress.update(task_id=closing_task, completed=True)
 
         raise typer.Exit(0)
```

### Comparing `integrate_ai-0.0.42/src/integrate_ai/main.py` & `integrate-ai-9.5.0/integrate_ai/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Module containing top-level Typer app functionality."""
 
-import subprocess
+import subprocess  # noqa: F401 - needed for unittest patch
 import typer
 import integrate_ai.sdk as sdk
 import integrate_ai.client as client
 import integrate_ai.server as server
 from integrate_ai.utils.typer_utils import show_package_version
 
-from rich import print as rprint
 
 app = typer.Typer(no_args_is_help=True)
 
 app.add_typer(sdk.app, name="sdk")
 app.add_typer(client.app, name="client")
 app.add_typer(server.app, name="server")
 
@@ -23,15 +22,14 @@
     no_prompt: bool = typer.Option(False, "--no-prompt", help="Disable prompts. Confirmations will default to `Y`.")
 ):
     """
     The CLI interface to manage integrate.ai operations.
 
     Your IAI token will be required in many commmands. For convenience, you can set this in the `IAI_TOKEN` environment variable to avoid repeated prompts.
     """
-    pass
 
 
 @app.command()
 def version():
     """
     The currently installed version of the cli.
     """
```

### Comparing `integrate_ai-0.0.42/src/integrate_ai/sdk.py` & `integrate-ai-9.5.0/integrate_ai/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         raise IntegrateAIException(f" Not installing the right package {pip_install_command}")
 
     # pip will output the version number and give an error if the version is not found
     if version == "":
         rprint(f"Trying to install latest {package}.")
     else:
         rprint(f"Trying to install {package}=={version}.")
-
     subprocess.run(pip_install_command, check=True, shell=True)
 
 
 @app.command()
 def version():
     """
     The currently installed version of the sdk.
```

### Comparing `integrate_ai-0.0.42/src/integrate_ai/server.py` & `integrate-ai-9.5.0/integrate_ai/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         docker_client.login()
         progress.update(task_id=p, completed=True)
         p = progress.add_task(
             description=f"Pulling docker image {version_to_pull}. This will take a few minutes...",
             total=1,
         )
         pull_result = docker_client.pull(repo=docker_client.get_repo_name(), tag=version_to_pull)
+        assert pull_result
         progress.update(task_id=p, completed=True)
         rprint(f"Image {version_to_pull} is now available.")
         raise typer.Exit(0)
 
 
 @app.command()
 def version(
```

### Comparing `integrate_ai-0.0.42/src/integrate_ai/utils/docker_client.py` & `integrate-ai-9.5.0/integrate_ai/utils/docker_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import docker  # type: ignore
 from docker.models.images import Image  # type: ignore
 from integrate_ai.utils.rest_client import RestClient
 from integrate_ai.utils.error_handling import DockerException
 from typing import Optional, Dict, List
 from distutils.version import LooseVersion
-import os
 from typing import Any
 
 
 class DockerClient:
     """Class to interact with docker client.
 
     This class performs various docker operations such as login, pull, rmi, etc.
```

### Comparing `integrate_ai-0.0.42/src/integrate_ai/utils/error_handling.py` & `integrate-ai-9.5.0/integrate_ai/utils/error_handling.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """Module containing exception-related functionality."""
 
 from requests import Response  # type: ignore
-import typer
-import os
 
 
 class IntegrateAIException(Exception):
     """The general exception for request and response errors."""
 
-    pass
-
 
 class DockerException(Exception):
     """The general exception for docker-related errors."""
 
-    pass
-
 
-def check_for_IntegrateAIException(response):
+def check_for_IntegrateAIException(response: Response):
     """Raises an IntegrateAIException from a response.
 
     If response has an error status code, raises a custom IntegrateAIException instead
       of the original Exception.
 
     Args:
         response (Response): HTTP response to check for error status and raise custom
```

### Comparing `integrate_ai-0.0.42/src/integrate_ai/utils/logger.py` & `integrate-ai-9.5.0/integrate_ai/utils/logger.py`

 * *Files identical despite different names*

### Comparing `integrate_ai-0.0.42/src/integrate_ai/utils/path_utils.py` & `integrate-ai-9.5.0/integrate_ai/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `integrate_ai-0.0.42/src/integrate_ai/utils/rest_client.py` & `integrate-ai-9.5.0/integrate_ai/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `integrate_ai-0.0.42/src/integrate_ai/utils/typer_utils.py` & `integrate-ai-9.5.0/integrate_ai/utils/typer_utils.py`

 * *Files identical despite different names*

