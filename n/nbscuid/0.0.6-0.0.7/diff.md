# Comparing `tmp/nbscuid-0.0.6.tar.gz` & `tmp/nbscuid-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbscuid-0.0.6.tar", last modified: Wed May 17 21:45:30 2023, max compression
+gzip compressed data, was "nbscuid-0.0.7.tar", last modified: Wed May 17 21:58:29 2023, max compression
```

## Comparing `nbscuid-0.0.6.tar` & `nbscuid-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:45:30.135256 nbscuid-0.0.6/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      332 2023-05-03 23:21:30.000000 nbscuid-0.0.6/.gitignore
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      715 2023-05-04 22:27:17.000000 nbscuid-0.0.6/.readthedocs.yml
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1073 2023-02-24 23:26:03.000000 nbscuid-0.0.6/LICENSE
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     3214 2023-05-17 21:45:30.134755 nbscuid-0.0.6/PKG-INFO
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1504 2023-05-15 17:28:53.000000 nbscuid-0.0.6/README.md
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:45:30.047731 nbscuid-0.0.6/docs/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      638 2023-05-03 20:38:18.000000 nbscuid-0.0.6/docs/Makefile
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      804 2023-05-03 20:38:18.000000 nbscuid-0.0.6/docs/make.bat
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       32 2023-05-04 22:11:40.000000 nbscuid-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:45:30.063776 nbscuid-0.0.6/docs/source/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1915 2023-05-04 15:24:38.000000 nbscuid-0.0.6/docs/source/conf.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       35 2023-05-17 16:40:58.000000 nbscuid-0.0.6/docs/source/gettingstarted.md
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      497 2023-05-17 15:13:04.000000 nbscuid-0.0.6/docs/source/index.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       58 2023-05-03 20:44:35.000000 nbscuid-0.0.6/docs/source/modules.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      795 2023-05-03 20:44:35.000000 nbscuid-0.0.6/docs/source/nbscuid.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     2027 2023-05-17 15:12:29.000000 nbscuid-0.0.6/docs/source/tutorialsetup.md
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:45:30.094005 nbscuid-0.0.6/nbscuid/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-02-24 23:33:45.000000 nbscuid-0.0.6/nbscuid/__init__.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1671 2023-05-16 17:45:54.000000 nbscuid-0.0.6/nbscuid/_jupyter-book-config-defaults.yml
--rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     1053 2023-04-24 23:15:21.000000 nbscuid-0.0.6/nbscuid/build.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     7640 2023-02-24 23:27:28.000000 nbscuid-0.0.6/nbscuid/cache.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-05-04 07:46:51.000000 nbscuid-0.0.6/nbscuid/quickstart.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1048 2023-03-08 00:11:40.000000 nbscuid-0.0.6/nbscuid/read.py
--rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     7289 2023-05-15 17:02:44.000000 nbscuid-0.0.6/nbscuid/run.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     9661 2023-05-03 23:11:22.000000 nbscuid-0.0.6/nbscuid/util.py
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:45:30.130714 nbscuid-0.0.6/nbscuid.egg-info/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     3214 2023-05-17 21:45:29.000000 nbscuid-0.0.6/nbscuid.egg-info/PKG-INFO
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      612 2023-05-17 21:45:29.000000 nbscuid-0.0.6/nbscuid.egg-info/SOURCES.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        1 2023-05-17 21:45:29.000000 nbscuid-0.0.6/nbscuid.egg-info/dependency_links.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       84 2023-05-17 21:45:29.000000 nbscuid-0.0.6/nbscuid.egg-info/entry_points.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       94 2023-05-17 21:45:29.000000 nbscuid-0.0.6/nbscuid.egg-info/requires.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        8 2023-05-17 21:45:29.000000 nbscuid-0.0.6/nbscuid.egg-info/top_level.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1020 2023-05-17 21:44:51.000000 nbscuid-0.0.6/pyproject.toml
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       38 2023-05-17 21:45:30.138125 nbscuid-0.0.6/setup.cfg
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.306395 nbscuid-0.0.7/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      332 2023-05-03 23:21:30.000000 nbscuid-0.0.7/.gitignore
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      715 2023-05-04 22:27:17.000000 nbscuid-0.0.7/.readthedocs.yml
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1073 2023-02-24 23:26:03.000000 nbscuid-0.0.7/LICENSE
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     3115 2023-05-17 21:58:29.305905 nbscuid-0.0.7/PKG-INFO
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1405 2023-05-17 21:52:45.000000 nbscuid-0.0.7/README.md
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.240841 nbscuid-0.0.7/docs/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      638 2023-05-03 20:38:18.000000 nbscuid-0.0.7/docs/Makefile
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      804 2023-05-03 20:38:18.000000 nbscuid-0.0.7/docs/make.bat
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       32 2023-05-04 22:11:40.000000 nbscuid-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.267614 nbscuid-0.0.7/docs/source/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1915 2023-05-04 15:24:38.000000 nbscuid-0.0.7/docs/source/conf.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       35 2023-05-17 16:40:58.000000 nbscuid-0.0.7/docs/source/gettingstarted.md
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      497 2023-05-17 15:13:04.000000 nbscuid-0.0.7/docs/source/index.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       58 2023-05-03 20:44:35.000000 nbscuid-0.0.7/docs/source/modules.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      795 2023-05-03 20:44:35.000000 nbscuid-0.0.7/docs/source/nbscuid.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     2023 2023-05-17 21:54:08.000000 nbscuid-0.0.7/docs/source/tutorialsetup.md
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.289735 nbscuid-0.0.7/nbscuid/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-02-24 23:33:45.000000 nbscuid-0.0.7/nbscuid/__init__.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1671 2023-05-16 17:45:54.000000 nbscuid-0.0.7/nbscuid/_jupyter-book-config-defaults.yml
+-rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     1053 2023-04-24 23:15:21.000000 nbscuid-0.0.7/nbscuid/build.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     7640 2023-02-24 23:27:28.000000 nbscuid-0.0.7/nbscuid/cache.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-05-04 07:46:51.000000 nbscuid-0.0.7/nbscuid/quickstart.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1048 2023-03-08 00:11:40.000000 nbscuid-0.0.7/nbscuid/read.py
+-rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     7289 2023-05-15 17:02:44.000000 nbscuid-0.0.7/nbscuid/run.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     9661 2023-05-03 23:11:22.000000 nbscuid-0.0.7/nbscuid/util.py
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.302905 nbscuid-0.0.7/nbscuid.egg-info/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     3115 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/PKG-INFO
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      612 2023-05-17 21:58:29.295826 nbscuid-0.0.7/nbscuid.egg-info/SOURCES.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        1 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/dependency_links.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       84 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/entry_points.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       94 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/requires.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        8 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/top_level.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1020 2023-05-17 21:58:04.000000 nbscuid-0.0.7/pyproject.toml
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       38 2023-05-17 21:58:29.306626 nbscuid-0.0.7/setup.cfg
```

### Comparing `nbscuid-0.0.6/.readthedocs.yml` & `nbscuid-0.0.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/LICENSE` & `nbscuid-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/PKG-INFO` & `nbscuid-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbscuid
-Version: 0.0.6
+Version: 0.0.7
 Summary: Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 Author-email: Elena Romashkova <eromashkova@ucar.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -46,24 +46,24 @@
 - Run different notebooks in different environments
 - Cache intermediate data products
 - Quickly build a Jupyter book with results
 
 
 ## Installation
 
-1. Clone this repo
-
-2. Activate the environment you want to install `nbscuid` in. Within the cloned `nbscuid` directory, run:
+- Run:
     ```
-    pip install .
+    pip install nbscuid
     ```
-    Alternatively, to install the commands `nbscuid-run` and `nbscuid-build` without installing all of `nbscuid`'s dependencies, first install `pipx` with `pip install pipx`, then run:
+    
+    Alternatively, to install the commands `nbscuid-run` and `nbscuid-build` without installing all of `nbscuid`'s dependencies, first install pipx with `pip install pipx`, then run:
     ```
-    pipx install .
+    pipx install nbscuid
     ```
+    
 
 ## Running a notebook collection
 
 Create a new folder that contains a `config.yml` file. (A guide to what goes in a `config.yml` file is coming soon!) This will be the run directory for your collection of notebooks, where all the computed notebooks will appear.
 
 To run all the notebooks you've specified, execute:
```

### Comparing `nbscuid-0.0.6/README.md` & `nbscuid-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 - Run different notebooks in different environments
 - Cache intermediate data products
 - Quickly build a Jupyter book with results
 
 
 ## Installation
 
-1. Clone this repo
-
-2. Activate the environment you want to install `nbscuid` in. Within the cloned `nbscuid` directory, run:
+- Run:
     ```
-    pip install .
+    pip install nbscuid
     ```
-    Alternatively, to install the commands `nbscuid-run` and `nbscuid-build` without installing all of `nbscuid`'s dependencies, first install `pipx` with `pip install pipx`, then run:
+    
+    Alternatively, to install the commands `nbscuid-run` and `nbscuid-build` without installing all of `nbscuid`'s dependencies, first install pipx with `pip install pipx`, then run:
     ```
-    pipx install .
+    pipx install nbscuid
     ```
+    
 
 ## Running a notebook collection
 
 Create a new folder that contains a `config.yml` file. (A guide to what goes in a `config.yml` file is coming soon!) This will be the run directory for your collection of notebooks, where all the computed notebooks will appear.
 
 To run all the notebooks you've specified, execute:
```

### Comparing `nbscuid-0.0.6/docs/Makefile` & `nbscuid-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/docs/make.bat` & `nbscuid-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/docs/source/conf.py` & `nbscuid-0.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/docs/source/nbscuid.rst` & `nbscuid-0.0.7/docs/source/nbscuid.rst`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/docs/source/tutorialsetup.md` & `nbscuid-0.0.7/docs/source/tutorialsetup.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 4. Using your text editor of choice, open the file `nbscuid-examples/tutorial/config.yml`. This file runs the whole notebook collection, and there are many ways to customize it. We'll be editing a few paths to make it work on your machine.
 5. In this file, under `data_sources`, edit `run_dir` to be the full path to wherever your copy of `nbscuid-examples/tutorial` is located. Then edit `nb_path_root` to be the path to the `nblibrary` folder within `tutorial`. Usually, below this, you would also want to update `default_kernel_name` to be the environment installed on your machine that you want to run your notebooks in. However, since you just installed the environment `nbscuid-tutorial1`, this is already set correctly.
 6. Open a terminal. In this terminal, activate whatever envionment you installed `nbscuid` in.
 7. `cd` into the `nbscuid-examples/tutorial` folder.
 8. Run 
             
-            nbscuid-run config.yml 
+        nbscuid-run config.yml 
 
     This will run a few simple notebooks showcasing some of `nbscuid`'s capabilities. The executed notebooks get copied to a directory called `computed_notebooks/placeholder-title` created in your `run_dir`.
 9. Next, run 
 
         nbscuid-build config.yml
         
      This will build the Jupyter Book based on the table of contents specified in the `config.yml` file, under Jupyter Book Table of Contents. The html files that make up the Jupyter Book will be created under `computed_notebooks/placeholder-title/_build/html`.
```

### Comparing `nbscuid-0.0.6/nbscuid/_jupyter-book-config-defaults.yml` & `nbscuid-0.0.7/nbscuid/_jupyter-book-config-defaults.yml`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/nbscuid/build.py` & `nbscuid-0.0.7/nbscuid/build.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/nbscuid/cache.py` & `nbscuid-0.0.7/nbscuid/cache.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/nbscuid/read.py` & `nbscuid-0.0.7/nbscuid/read.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/nbscuid/run.py` & `nbscuid-0.0.7/nbscuid/run.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/nbscuid/util.py` & `nbscuid-0.0.7/nbscuid/util.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/nbscuid.egg-info/PKG-INFO` & `nbscuid-0.0.7/nbscuid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbscuid
-Version: 0.0.6
+Version: 0.0.7
 Summary: Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 Author-email: Elena Romashkova <eromashkova@ucar.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -46,24 +46,24 @@
 - Run different notebooks in different environments
 - Cache intermediate data products
 - Quickly build a Jupyter book with results
 
 
 ## Installation
 
-1. Clone this repo
-
-2. Activate the environment you want to install `nbscuid` in. Within the cloned `nbscuid` directory, run:
+- Run:
     ```
-    pip install .
+    pip install nbscuid
     ```
-    Alternatively, to install the commands `nbscuid-run` and `nbscuid-build` without installing all of `nbscuid`'s dependencies, first install `pipx` with `pip install pipx`, then run:
+    
+    Alternatively, to install the commands `nbscuid-run` and `nbscuid-build` without installing all of `nbscuid`'s dependencies, first install pipx with `pip install pipx`, then run:
     ```
-    pipx install .
+    pipx install nbscuid
     ```
+    
 
 ## Running a notebook collection
 
 Create a new folder that contains a `config.yml` file. (A guide to what goes in a `config.yml` file is coming soon!) This will be the run directory for your collection of notebooks, where all the computed notebooks will appear.
 
 To run all the notebooks you've specified, execute:
```

### Comparing `nbscuid-0.0.6/nbscuid.egg-info/SOURCES.txt` & `nbscuid-0.0.7/nbscuid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.6/pyproject.toml` & `nbscuid-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 #[tool.setuptools.package-data]
 #mypkg = ["*.yml"]
 
 
 [project]
 name = "nbscuid"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Elena Romashkova", email="eromashkova@ucar.edu" },
 ]
 description = "Notebook-Based, Super CUstomizable Infrastructure for Diagnostics"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

