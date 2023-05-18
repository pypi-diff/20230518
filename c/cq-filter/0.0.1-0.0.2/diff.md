# Comparing `tmp/cq-filter-0.0.1.tar.gz` & `tmp/cq-filter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq-filter-0.0.1.tar", last modified: Wed May 17 18:41:18 2023, max compression
+gzip compressed data, was "cq-filter-0.0.2.tar", last modified: Thu May 18 20:57:57 2023, max compression
```

## Comparing `cq-filter-0.0.1.tar` & `cq-filter-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:18.951014 cq-filter-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:18.947014 cq-filter-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 18:41:02.000000 cq-filter-0.0.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:18.947014 cq-filter-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-17 18:41:02.000000 cq-filter-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-17 18:41:02.000000 cq-filter-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-17 18:41:02.000000 cq-filter-0.0.1/.github/workflows/test-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 18:41:02.000000 cq-filter-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-17 18:41:02.000000 cq-filter-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-17 18:41:18.951014 cq-filter-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-17 18:41:02.000000 cq-filter-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-17 18:41:02.000000 cq-filter-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-17 18:41:02.000000 cq-filter-0.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 18:41:02.000000 cq-filter-0.0.1/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 18:41:02.000000 cq-filter-0.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:41:18.951014 cq-filter-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:18.947014 cq-filter-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:18.947014 cq-filter-0.0.1/src/cq_filter/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 18:41:02.000000 cq-filter-0.0.1/src/cq_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-17 18:41:02.000000 cq-filter-0.0.1/src/cq_filter/cq_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:18.947014 cq-filter-0.0.1/src/cq_filter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:02.000000 cq-filter-0.0.1/src/cq_filter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-17 18:41:02.000000 cq-filter-0.0.1/src/cq_filter/tests/test_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:41:18.947014 cq-filter-0.0.1/src/cq_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-17 18:41:18.000000 cq-filter-0.0.1/src/cq_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-17 18:41:18.000000 cq-filter-0.0.1/src/cq_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:41:18.000000 cq-filter-0.0.1/src/cq_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 18:41:18.000000 cq-filter-0.0.1/src/cq_filter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:57:57.342524 cq-filter-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:57:57.342524 cq-filter-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 20:57:32.000000 cq-filter-0.0.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:57:57.342524 cq-filter-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-18 20:57:32.000000 cq-filter-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-18 20:57:32.000000 cq-filter-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-18 20:57:32.000000 cq-filter-0.0.2/.github/workflows/test-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 20:57:32.000000 cq-filter-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-18 20:57:32.000000 cq-filter-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-18 20:57:57.342524 cq-filter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-18 20:57:32.000000 cq-filter-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-18 20:57:32.000000 cq-filter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 20:57:32.000000 cq-filter-0.0.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 20:57:32.000000 cq-filter-0.0.2/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-18 20:57:32.000000 cq-filter-0.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 20:57:57.342524 cq-filter-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:57:57.338524 cq-filter-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:57:57.342524 cq-filter-0.0.2/src/cq_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 20:57:32.000000 cq-filter-0.0.2/src/cq_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-18 20:57:32.000000 cq-filter-0.0.2/src/cq_filter/cq_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:57:57.342524 cq-filter-0.0.2/src/cq_filter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 20:57:32.000000 cq-filter-0.0.2/src/cq_filter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-18 20:57:32.000000 cq-filter-0.0.2/src/cq_filter/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-18 20:57:32.000000 cq-filter-0.0.2/src/cq_filter/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-18 20:57:32.000000 cq-filter-0.0.2/src/cq_filter/tests/test_last.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:57:57.342524 cq-filter-0.0.2/src/cq_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-18 20:57:57.000000 cq-filter-0.0.2/src/cq_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-18 20:57:57.000000 cq-filter-0.0.2/src/cq_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:57:57.000000 cq-filter-0.0.2/src/cq_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 20:57:57.000000 cq-filter-0.0.2/src/cq_filter.egg-info/top_level.txt
```

### Comparing `cq-filter-0.0.1/.github/workflows/ci.yml` & `cq-filter-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cq-filter-0.0.1/.github/workflows/release.yml` & `cq-filter-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `cq-filter-0.0.1/.github/workflows/test-release.yml` & `cq-filter-0.0.2/.github/workflows/test-release.yml`

 * *Files identical despite different names*

### Comparing `cq-filter-0.0.1/LICENSE` & `cq-filter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cq-filter-0.0.1/PKG-INFO` & `cq-filter-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq-filter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cadquery object filtering framework
 Author-email: Matti Eiden <snaipperi@gmail.com>
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/voneiden/cq-filter/issues/
 Project-URL: Documentation, https://github.com/voneiden/cq-filter/
 Project-URL: Source Code, https://github.com/voneiden/cq-filter/
 Keywords: cadquery,filter
@@ -21,14 +21,15 @@
 
 cq-filter adds a few new workplane methods that take a function argument
 of type `f: Callable[[CQObject], bool]`:
 
 * `filter(f)`: filters Workplane objects
 * `sort(f)`: orders Workplane objects
 * `group(f)`: groups Workplane objects
+* `last`: selects newly created faces
 
 Additionally, it adds subscription support to the Workplane, allowing 
 selection of objects quickly.
 
 ## Rationale
 
 Manipulating object selections in cadquery isn't currently possible without breaking out of the fluent API.
@@ -80,15 +81,46 @@
 Selection should be done immediatelly after the grouping. Grouping data will be erased by 
 next manipulation of workplane.
 
 * selecting a range of groups (`[0:2]`) works as expected
 
 * Cluster() defaults to a tolerance of `1e-4`
 
+## Using `last` to select newly created faces
+
+A call to `.last(everything=False)` attempts to select newly created faces. When `everything = False` it will only
+select faces that have a normal parallel to the current workplane. Presumably this default behaviour is what you'd
+want to use to select the face(s) created by a call to `extrude` or `cutBlind`. Supplying `everything = True` will 
+select all faces that are new.
+
+```python
+from cq_filter import Workplane
+
+wp = (
+    Workplane()
+    .rect(5, 5)
+    .extrude(2)
+    .last()
+    .workplane()
+)
+```
+
+* ⚠️ `last` will not select faces that were modified
+* ⚠️ `last` is probably not very handy for selecting the end face of something like `revolve`  
+
+
 ## Usage 
 
-You'll probably want to create your own workplane class
+You may want to create your own workplane class if you have multiple mixins
 
 ```python 
+from cq_filter import CQFilterMixin
+
 class Workplane(CQFilterMixin, cq.Workplane):
    pass
 ```
+
+If you don't have multiple mixins, then the above class can also be directly imported 
+
+```python 
+from cq_filter import Workplane
+```
```

### Comparing `cq-filter-0.0.1/README.md` & `cq-filter-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 cq-filter adds a few new workplane methods that take a function argument
 of type `f: Callable[[CQObject], bool]`:
 
 * `filter(f)`: filters Workplane objects
 * `sort(f)`: orders Workplane objects
 * `group(f)`: groups Workplane objects
+* `last`: selects newly created faces
 
 Additionally, it adds subscription support to the Workplane, allowing 
 selection of objects quickly.
 
 ## Rationale
 
 Manipulating object selections in cadquery isn't currently possible without breaking out of the fluent API.
@@ -62,15 +63,46 @@
 Selection should be done immediatelly after the grouping. Grouping data will be erased by 
 next manipulation of workplane.
 
 * selecting a range of groups (`[0:2]`) works as expected
 
 * Cluster() defaults to a tolerance of `1e-4`
 
+## Using `last` to select newly created faces
+
+A call to `.last(everything=False)` attempts to select newly created faces. When `everything = False` it will only
+select faces that have a normal parallel to the current workplane. Presumably this default behaviour is what you'd
+want to use to select the face(s) created by a call to `extrude` or `cutBlind`. Supplying `everything = True` will 
+select all faces that are new.
+
+```python
+from cq_filter import Workplane
+
+wp = (
+    Workplane()
+    .rect(5, 5)
+    .extrude(2)
+    .last()
+    .workplane()
+)
+```
+
+* ⚠️ `last` will not select faces that were modified
+* ⚠️ `last` is probably not very handy for selecting the end face of something like `revolve`  
+
+
 ## Usage 
 
-You'll probably want to create your own workplane class
+You may want to create your own workplane class if you have multiple mixins
 
 ```python 
+from cq_filter import CQFilterMixin
+
 class Workplane(CQFilterMixin, cq.Workplane):
    pass
 ```
+
+If you don't have multiple mixins, then the above class can also be directly imported 
+
+```python 
+from cq_filter import Workplane
+```
```

### Comparing `cq-filter-0.0.1/pyproject.toml` & `cq-filter-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cq-filter-0.0.1/requirements-dev.txt` & `cq-filter-0.0.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `cq-filter-0.0.1/src/cq_filter/tests/test_filter.py` & `cq-filter-0.0.2/src/cq_filter/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `cq-filter-0.0.1/src/cq_filter.egg-info/PKG-INFO` & `cq-filter-0.0.2/src/cq_filter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq-filter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cadquery object filtering framework
 Author-email: Matti Eiden <snaipperi@gmail.com>
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/voneiden/cq-filter/issues/
 Project-URL: Documentation, https://github.com/voneiden/cq-filter/
 Project-URL: Source Code, https://github.com/voneiden/cq-filter/
 Keywords: cadquery,filter
@@ -21,14 +21,15 @@
 
 cq-filter adds a few new workplane methods that take a function argument
 of type `f: Callable[[CQObject], bool]`:
 
 * `filter(f)`: filters Workplane objects
 * `sort(f)`: orders Workplane objects
 * `group(f)`: groups Workplane objects
+* `last`: selects newly created faces
 
 Additionally, it adds subscription support to the Workplane, allowing 
 selection of objects quickly.
 
 ## Rationale
 
 Manipulating object selections in cadquery isn't currently possible without breaking out of the fluent API.
@@ -80,15 +81,46 @@
 Selection should be done immediatelly after the grouping. Grouping data will be erased by 
 next manipulation of workplane.
 
 * selecting a range of groups (`[0:2]`) works as expected
 
 * Cluster() defaults to a tolerance of `1e-4`
 
+## Using `last` to select newly created faces
+
+A call to `.last(everything=False)` attempts to select newly created faces. When `everything = False` it will only
+select faces that have a normal parallel to the current workplane. Presumably this default behaviour is what you'd
+want to use to select the face(s) created by a call to `extrude` or `cutBlind`. Supplying `everything = True` will 
+select all faces that are new.
+
+```python
+from cq_filter import Workplane
+
+wp = (
+    Workplane()
+    .rect(5, 5)
+    .extrude(2)
+    .last()
+    .workplane()
+)
+```
+
+* ⚠️ `last` will not select faces that were modified
+* ⚠️ `last` is probably not very handy for selecting the end face of something like `revolve`  
+
+
 ## Usage 
 
-You'll probably want to create your own workplane class
+You may want to create your own workplane class if you have multiple mixins
 
 ```python 
+from cq_filter import CQFilterMixin
+
 class Workplane(CQFilterMixin, cq.Workplane):
    pass
 ```
+
+If you don't have multiple mixins, then the above class can also be directly imported 
+
+```python 
+from cq_filter import Workplane
+```
```

