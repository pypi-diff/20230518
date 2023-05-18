# Comparing `tmp/nvosscript-1.3.0.tar.gz` & `tmp/nvosscript-1.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.0.tar", last modified: Mon May 15 02:50:32 2023, max compression
+gzip compressed data, was "nvosscript-1.3.0.1.tar", last modified: Thu May 18 06:50:24 2023, max compression
```

## Comparing `nvosscript-1.3.0.tar` & `nvosscript-1.3.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.761165 nvosscript-1.3.0/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.0/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-05-15 02:50:32.760947 nvosscript-1.3.0/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.0/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.757087 nvosscript-1.3.0/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.0/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    13051 2023-05-12 07:47:19.000000 nvosscript-1.3.0/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.3.0/nvos/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-12 07:47:19.000000 nvosscript-1.3.0/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     6172 2023-05-11 08:47:40.000000 nvosscript-1.3.0/nvos/run.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.3.0/nvos/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.758389 nvosscript-1.3.0/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-15 02:50:32.000000 nvosscript-1.3.0/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-15 02:50:32.761226 nvosscript-1.3.0/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-05-12 07:47:19.000000 nvosscript-1.3.0/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.759223 nvosscript-1.3.0/skyeye/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.0/skyeye/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.3.0/skyeye/datahandler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.3.0/skyeye/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.3.0/skyeye/skyeyecommand.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.759947 nvosscript-1.3.0/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.0/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.3.0/start/commonUtil.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4525 2023-05-12 07:47:19.000000 nvosscript-1.3.0/start/main.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.752771 nvosscript-1.3.0/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.760269 nvosscript-1.3.0/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.0/venv/bin/activate_this.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-15 02:50:32.760612 nvosscript-1.3.0/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.0/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 06:50:24.490702 nvosscript-1.3.0.1/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.0.1/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-18 06:50:24.490552 nvosscript-1.3.0.1/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.0.1/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 06:50:24.487513 nvosscript-1.3.0.1/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.0.1/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    13219 2023-05-18 06:41:49.000000 nvosscript-1.3.0.1/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.3.0.1/nvos/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-12 07:47:19.000000 nvosscript-1.3.0.1/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     6172 2023-05-11 08:47:40.000000 nvosscript-1.3.0.1/nvos/run.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.3.0.1/nvos/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 06:50:24.488458 nvosscript-1.3.0.1/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-18 06:50:24.000000 nvosscript-1.3.0.1/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-18 06:50:24.000000 nvosscript-1.3.0.1/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-18 06:50:24.000000 nvosscript-1.3.0.1/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-18 06:50:24.000000 nvosscript-1.3.0.1/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-18 06:50:24.000000 nvosscript-1.3.0.1/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-18 06:50:24.000000 nvosscript-1.3.0.1/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-18 06:50:24.490744 nvosscript-1.3.0.1/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      807 2023-05-18 06:50:03.000000 nvosscript-1.3.0.1/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 06:50:24.489188 nvosscript-1.3.0.1/skyeye/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.0.1/skyeye/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.3.0.1/skyeye/datahandler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.3.0.1/skyeye/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.3.0.1/skyeye/skyeyecommand.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 06:50:24.489608 nvosscript-1.3.0.1/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.0.1/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.3.0.1/start/commonUtil.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4527 2023-05-18 06:50:03.000000 nvosscript-1.3.0.1/start/main.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 06:50:24.485190 nvosscript-1.3.0.1/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 06:50:24.489856 nvosscript-1.3.0.1/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.0.1/venv/bin/activate_this.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 06:50:24.490223 nvosscript-1.3.0.1/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.0.1/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.0/LICENSE` & `nvosscript-1.3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0/nvos/file.py` & `nvosscript-1.3.0.1/nvos/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,23 +206,28 @@
     return project_space_list
 
 
 def get_current_git_branch(workspace_path):
     git_path = os.path.join(workspace_path, ".git")
     if not os.path.exists(git_path):
         return ""
-    completed_process = subprocess.run(['git', 'branch'], stdout=subprocess.PIPE)
-    git_branch_val = completed_process.stdout.decode().splitlines()
-    if len(git_branch_val) == 0:
+
+    try:
+        completed_process = subprocess.run(['git', 'branch'], stdout=subprocess.PIPE)
+        git_branch_val = completed_process.stdout.decode().splitlines()
+        if len(git_branch_val) == 0:
+            return ""
+        git_branch_data = ""
+        for line in git_branch_val:
+            if "*" in line:
+                git_branch_data = line.split("*")[1].strip()
+        return git_branch_data
+    except Exception as e:
+        print(f"Error: {os.path.join(os.getcwd(), '.ndtc')} : {e.strerror}")
         return ""
-    git_branch_data = ""
-    for line in git_branch_val:
-        if "*" in line:
-            git_branch_data = line.split("*")[1].strip()
-    return git_branch_data
 
 
 # 获取项目的空间
 def find_project_space(workspace_path, result_list):
     for file_path in os.listdir(workspace_path):
         if file_path == ".idea" or file_path == ".repo" or file_path == ".ndtc" or file_path == ".DS_Store":
             continue
```

### Comparing `nvosscript-1.3.0/nvos/login.py` & `nvosscript-1.3.0.1/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0/nvos/remote.py` & `nvosscript-1.3.0.1/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0/nvos/run.py` & `nvosscript-1.3.0.1/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0/nvos/utils.py` & `nvosscript-1.3.0.1/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0/setup.py` & `nvosscript-1.3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.0',
+    version='1.3.0.1',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.0/skyeye/datahandler.py` & `nvosscript-1.3.0.1/skyeye/datahandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0/skyeye/remote.py` & `nvosscript-1.3.0.1/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0/start/main.py` & `nvosscript-1.3.0.1/start/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.0")
+        print("1.3.0.1")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.0/venv/bin/activate_this.py` & `nvosscript-1.3.0.1/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0/win/win_auto_script.py` & `nvosscript-1.3.0.1/win/win_auto_script.py`

 * *Files identical despite different names*

