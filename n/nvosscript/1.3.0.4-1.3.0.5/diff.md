# Comparing `tmp/nvosscript-1.3.0.4.tar.gz` & `tmp/nvosscript-1.3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.0.4.tar", last modified: Thu May 18 08:55:39 2023, max compression
+gzip compressed data, was "nvosscript-1.3.0.5.tar", last modified: Thu May 18 09:23:56 2023, max compression
```

## Comparing `nvosscript-1.3.0.4.tar` & `nvosscript-1.3.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 08:55:39.629818 nvosscript-1.3.0.4/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.0.4/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-18 08:55:39.629671 nvosscript-1.3.0.4/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.0.4/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 08:55:39.626973 nvosscript-1.3.0.4/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.0.4/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    13483 2023-05-18 08:55:16.000000 nvosscript-1.3.0.4/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.3.0.4/nvos/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-12 07:47:19.000000 nvosscript-1.3.0.4/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     6172 2023-05-11 08:47:40.000000 nvosscript-1.3.0.4/nvos/run.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.3.0.4/nvos/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 08:55:39.627784 nvosscript-1.3.0.4/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-18 08:55:39.000000 nvosscript-1.3.0.4/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-18 08:55:39.000000 nvosscript-1.3.0.4/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-18 08:55:39.000000 nvosscript-1.3.0.4/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-18 08:55:39.000000 nvosscript-1.3.0.4/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-18 08:55:39.000000 nvosscript-1.3.0.4/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-18 08:55:39.000000 nvosscript-1.3.0.4/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-18 08:55:39.629858 nvosscript-1.3.0.4/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      807 2023-05-18 08:55:38.000000 nvosscript-1.3.0.4/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 08:55:39.628490 nvosscript-1.3.0.4/skyeye/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.0.4/skyeye/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.3.0.4/skyeye/datahandler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.3.0.4/skyeye/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.3.0.4/skyeye/skyeyecommand.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 08:55:39.628960 nvosscript-1.3.0.4/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.0.4/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.3.0.4/start/commonUtil.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4527 2023-05-18 08:55:38.000000 nvosscript-1.3.0.4/start/main.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 08:55:39.624829 nvosscript-1.3.0.4/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 08:55:39.629112 nvosscript-1.3.0.4/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.0.4/venv/bin/activate_this.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 08:55:39.629378 nvosscript-1.3.0.4/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.0.4/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:23:56.948537 nvosscript-1.3.0.5/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.0.5/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-18 09:23:56.948383 nvosscript-1.3.0.5/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.0.5/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:23:56.945519 nvosscript-1.3.0.5/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.0.5/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    13494 2023-05-18 09:22:50.000000 nvosscript-1.3.0.5/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.3.0.5/nvos/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-12 07:47:19.000000 nvosscript-1.3.0.5/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     6172 2023-05-11 08:47:40.000000 nvosscript-1.3.0.5/nvos/run.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.3.0.5/nvos/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:23:56.946525 nvosscript-1.3.0.5/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-05-18 09:23:56.000000 nvosscript-1.3.0.5/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-18 09:23:56.000000 nvosscript-1.3.0.5/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-18 09:23:56.000000 nvosscript-1.3.0.5/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-18 09:23:56.000000 nvosscript-1.3.0.5/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-18 09:23:56.000000 nvosscript-1.3.0.5/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-18 09:23:56.000000 nvosscript-1.3.0.5/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-18 09:23:56.948581 nvosscript-1.3.0.5/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      807 2023-05-18 09:23:55.000000 nvosscript-1.3.0.5/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:23:56.947240 nvosscript-1.3.0.5/skyeye/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.0.5/skyeye/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.3.0.5/skyeye/datahandler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.3.0.5/skyeye/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.3.0.5/skyeye/skyeyecommand.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:23:56.947694 nvosscript-1.3.0.5/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.0.5/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.3.0.5/start/commonUtil.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4527 2023-05-18 09:23:55.000000 nvosscript-1.3.0.5/start/main.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:23:56.943123 nvosscript-1.3.0.5/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:23:56.947831 nvosscript-1.3.0.5/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.0.5/venv/bin/activate_this.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-18 09:23:56.948084 nvosscript-1.3.0.5/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.0.5/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.0.4/LICENSE` & `nvosscript-1.3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.4/nvos/file.py` & `nvosscript-1.3.0.5/nvos/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         git_branch_data = ""
         for line in git_branch_val:
             if "*" in line:
                 git_branch_data = line.split("*")[1].strip()
         return git_branch_data
     except Exception as e:
         print(f"Error: {os.path.join(os.getcwd(), '.ndtc')} : {e.strerror}")
-        return ""
+        return "(no branch)"
 
 
 # 获取项目的空间
 def find_project_space(workspace_path, result_list):
     for file_path in os.listdir(workspace_path):
         if file_path == ".idea" or file_path == ".repo" or file_path == ".ndtc" or file_path == ".DS_Store":
             continue
```

### Comparing `nvosscript-1.3.0.4/nvos/login.py` & `nvosscript-1.3.0.5/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.4/nvos/remote.py` & `nvosscript-1.3.0.5/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.4/nvos/run.py` & `nvosscript-1.3.0.5/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.4/nvos/utils.py` & `nvosscript-1.3.0.5/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.4/setup.py` & `nvosscript-1.3.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.0.4',
+    version='1.3.0.5',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.0.4/skyeye/datahandler.py` & `nvosscript-1.3.0.5/skyeye/datahandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.4/skyeye/remote.py` & `nvosscript-1.3.0.5/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.4/start/main.py` & `nvosscript-1.3.0.5/start/main.py`

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
-        print("1.3.0.4")
+        print("1.3.0.5")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.0.4/venv/bin/activate_this.py` & `nvosscript-1.3.0.5/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.0.4/win/win_auto_script.py` & `nvosscript-1.3.0.5/win/win_auto_script.py`

 * *Files identical despite different names*

