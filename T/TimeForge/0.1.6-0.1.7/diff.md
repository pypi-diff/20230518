# Comparing `tmp/TimeForge-0.1.6.tar.gz` & `tmp/TimeForge-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeForge-0.1.6.tar", last modified: Tue May  9 20:24:27 2023, max compression
+gzip compressed data, was "TimeForge-0.1.7.tar", last modified: Thu May 18 14:54:53 2023, max compression
```

## Comparing `TimeForge-0.1.6.tar` & `TimeForge-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 20:24:27.025466 TimeForge-0.1.6/
--rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.6/LICENSE.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-09 20:24:27.025466 TimeForge-0.1.6/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      559 2023-05-08 08:20:49.000000 TimeForge-0.1.6/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-05-09 20:24:18.000000 TimeForge-0.1.6/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-09 20:24:27.025466 TimeForge-0.1.6/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 20:24:27.022133 TimeForge-0.1.6/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 20:24:27.022133 TimeForge-0.1.6/src/TimeForge.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-05-09 20:24:27.000000 TimeForge-0.1.6/src/TimeForge.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 20:24:27.025466 TimeForge-0.1.6/src/timeforge/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.6/src/timeforge/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6817 2023-05-09 20:24:02.000000 TimeForge-0.1.6/src/timeforge/__main__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-18 14:54:53.953662 TimeForge-0.1.7/
+-rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.7/LICENSE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-18 14:54:53.953662 TimeForge-0.1.7/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      559 2023-05-08 08:20:49.000000 TimeForge-0.1.7/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      989 2023-05-18 14:54:47.000000 TimeForge-0.1.7/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-18 14:54:53.953662 TimeForge-0.1.7/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-18 14:54:53.950328 TimeForge-0.1.7/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-18 14:54:53.950328 TimeForge-0.1.7/src/TimeForge.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1232 2023-05-18 14:54:53.000000 TimeForge-0.1.7/src/TimeForge.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-05-18 14:54:53.000000 TimeForge-0.1.7/src/TimeForge.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-18 14:54:53.000000 TimeForge-0.1.7/src/TimeForge.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-05-18 14:54:53.000000 TimeForge-0.1.7/src/TimeForge.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-05-18 14:54:53.000000 TimeForge-0.1.7/src/TimeForge.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-18 14:54:53.950328 TimeForge-0.1.7/src/timeforge/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.7/src/timeforge/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6817 2023-05-09 20:24:02.000000 TimeForge-0.1.7/src/timeforge/__main__.py
```

### Comparing `TimeForge-0.1.6/LICENSE.md` & `TimeForge-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.1.6/PKG-INFO` & `TimeForge-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.6
+Version: 0.1.7
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.6/README.md` & `TimeForge-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.1.6/pyproject.toml` & `TimeForge-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TimeForge"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = "Create realistic looking but fake time documentation for your student job at KIT"
 readme = "README.md"
 requires-python= ">=3.7"
 classifiers = [
@@ -26,9 +26,10 @@
 	"wcwidth >= 0.2.6",
 	"deutschland >= 0.3.1",
 	"de-feiertage >= 1.0.1",
 	"pypdf >= 3.8.0",
 ]
 
 [projects.urls]
-"Homepage" = "https://github.com/MitchiLaser/timeforge"
+Homepage = "https://github.com/MitchiLaser/timeforge"
+repository = "https://github.com/MitchiLaser/timeforge"
```

### Comparing `TimeForge-0.1.6/src/TimeForge.egg-info/PKG-INFO` & `TimeForge-0.1.7/src/TimeForge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.6
+Version: 0.1.7
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.6/src/timeforge/__main__.py` & `TimeForge-0.1.7/src/timeforge/__main__.py`

 * *Files identical despite different names*

