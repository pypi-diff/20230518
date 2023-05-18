# Comparing `tmp/miquido_spawn_gitlab_job-1.0.4.tar.gz` & `tmp/miquido_spawn_gitlab_job-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miquido_spawn_gitlab_job-1.0.4.tar", last modified: Wed May 17 13:42:34 2023, max compression
+gzip compressed data, was "miquido_spawn_gitlab_job-1.0.5.tar", last modified: Thu May 18 05:12:17 2023, max compression
```

## Comparing `miquido_spawn_gitlab_job-1.0.4.tar` & `miquido_spawn_gitlab_job-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:42:34.362109 miquido_spawn_gitlab_job-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-17 13:42:34.362109 miquido_spawn_gitlab_job-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 13:42:34.362109 miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-17 13:42:20.761028 miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-17 13:42:20.761028 miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2023-05-17 13:42:20.761028 miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/spawner.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-17 13:42:34.214097 miquido_spawn_gitlab_job-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:12:17.759268 miquido_spawn_gitlab_job-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-05-18 05:12:17.759268 miquido_spawn_gitlab_job-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 05:12:17.759268 miquido_spawn_gitlab_job-1.0.5/gitlab_env_spawner/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-17 13:41:45.059298 miquido_spawn_gitlab_job-1.0.5/gitlab_env_spawner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-17 13:41:45.059298 miquido_spawn_gitlab_job-1.0.5/gitlab_env_spawner/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2023-05-18 05:12:07.090422 miquido_spawn_gitlab_job-1.0.5/gitlab_env_spawner/spawner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-18 05:12:17.627258 miquido_spawn_gitlab_job-1.0.5/setup.py
```

### Comparing `miquido_spawn_gitlab_job-1.0.4/PKG-INFO` & `miquido_spawn_gitlab_job-1.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: miquido_spawn_gitlab_job
-Version: 1.0.4
+Version: 1.0.5
 Summary: Launches dynamic environment on AWS ECS
 Home-page: UNKNOWN
 Author: Marek
 Author-email: marek.moscichowski@miquido.com
 License: MIT
 Description: UNKNOWN
 Keywords: GITLAB
```

### Comparing `miquido_spawn_gitlab_job-1.0.4/gitlab_env_spawner/spawner.py` & `miquido_spawn_gitlab_job-1.0.5/gitlab_env_spawner/spawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 def __map_container_files(s):
     with open(s[1], 'r') as f:
         return f.read()
 
 
 def spawn():
+    print(f'pwd = {os.getcwd()}')
+
     lb = boto3.client('lambda')
     additional_containers = list(filter(lambda x: x[0][0:11] == 'DD_SERVICE_', os.environ.items()))
     additional_containers = list(map(__map_container_files, additional_containers))
 
     environment_variables = list(filter(lambda x: x[0][0:3] == 'DD_', os.environ.items()))
     environment_variables = list(map(lambda x: (x[0][3:], x[1]), environment_variables))
     environment_variables = reduce(lambda res, x: {**res, **{x[0]: x[1]}}, environment_variables, {})
```

### Comparing `miquido_spawn_gitlab_job-1.0.4/setup.py` & `miquido_spawn_gitlab_job-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='miquido_spawn_gitlab_job',  # How you named your package folder (MyLib)
     packages=['gitlab_env_spawner'],  # Chose the same as "name"
-    version='1.0.4',
+    version='1.0.5',
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Launches dynamic environment on AWS ECS',
     # Give a short description about your library
     author='Marek',  # Type in your name
     author_email='marek.moscichowski@miquido.com',  # Type in your E-Mail
     keywords=['GITLAB'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
```

