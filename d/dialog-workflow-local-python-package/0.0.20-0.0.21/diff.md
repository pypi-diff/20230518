# Comparing `tmp/dialog-workflow-local-python-package-0.0.20.tar.gz` & `tmp/dialog-workflow-local-python-package-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-python-package-0.0.20.tar", last modified: Sun May 14 15:00:09 2023, max compression
+gzip compressed data, was "dialog-workflow-local-python-package-0.0.21.tar", last modified: Thu May 18 18:29:08 2023, max compression
```

## Comparing `dialog-workflow-local-python-package-0.0.20.tar` & `dialog-workflow-local-python-package-0.0.21.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:09.787144 dialog-workflow-local-python-package-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-14 15:00:09.787144 dialog-workflow-local-python-package-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:09.787144 dialog-workflow-local-python-package-0.0.20/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:00:09.787144 dialog-workflow-local-python-package-0.0.20/dialog_workflow_local_python_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-14 15:00:09.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow_local_python_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-14 15:00:09.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow_local_python_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:00:09.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow_local_python_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 15:00:09.000000 dialog-workflow-local-python-package-0.0.20/dialog_workflow_local_python_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:00:09.787144 dialog-workflow-local-python-package-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-14 14:59:52.000000 dialog-workflow-local-python-package-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-18 18:29:08.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-18 18:29:08.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:29:08.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 18:29:08.000000 dialog-workflow-local-python-package-0.0.21/dialog_workflow_local_python_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:29:08.686162 dialog-workflow-local-python-package-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 18:28:56.000000 dialog-workflow-local-python-package-0.0.21/setup.py
```

### Comparing `dialog-workflow-local-python-package-0.0.20/dialog_workflow/Act.py` & `dialog-workflow-local-python-package-0.0.21/dialog_workflow/Act.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.20/dialog_workflow/Constants.py` & `dialog-workflow-local-python-package-0.0.21/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.20/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-python-package-0.0.21/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.20/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-python-package-0.0.21/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.20/dialog_workflow/test.py` & `dialog-workflow-local-python-package-0.0.21/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.20/dialog_workflow/utils.py` & `dialog-workflow-local-python-package-0.0.21/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-python-package-0.0.20/setup.py` & `dialog-workflow-local-python-package-0.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local-python-package',  
-     version='0.0.20',
+     version='0.0.21',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

