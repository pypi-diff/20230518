# Comparing `tmp/serialization_tool-0.5.tar.gz` & `tmp/serialization_tool-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialization_tool-0.5.tar", last modified: Thu May 18 08:34:29 2023, max compression
+gzip compressed data, was "serialization_tool-1.0.tar", last modified: Thu May 18 09:42:10 2023, max compression
```

## Comparing `serialization_tool-0.5.tar` & `serialization_tool-1.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.145834 serialization_tool-0.5/
--rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      313 2023-05-18 08:34:29.145834 serialization_tool-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-0.5/README.md
--rw-rw-rw-   0        0        0      115 2023-05-18 08:34:29.161846 serialization_tool-0.5/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-05-18 08:33:47.000000 serialization_tool-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:34:28.993830 serialization_tool-0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.037846 serialization_tool-0.5/src/serialization_tool/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.5/src/serialization_tool/__init__.py
--rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-0.5/src/serialization_tool/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.109830 serialization_tool-0.5/src/serialization_tool/serialization/
--rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-0.5/src/serialization_tool/serialization/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-05-03 17:44:51.000000 serialization_tool-0.5/src/serialization_tool/serialization/constants.py
--rw-rw-rw-   0        0        0     9770 2023-05-18 08:09:13.000000 serialization_tool-0.5/src/serialization_tool/serialization/serializer.py
--rw-rw-rw-   0        0        0      465 2023-05-03 20:36:54.000000 serialization_tool-0.5/src/serialization_tool/serialization_factory.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.117870 serialization_tool-0.5/src/serialization_tool/types/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.5/src/serialization_tool/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.129829 serialization_tool-0.5/src/serialization_tool/types/json/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.5/src/serialization_tool/types/json/__init__.py
--rw-rw-rw-   0        0        0      138 2023-04-28 13:23:00.000000 serialization_tool-0.5/src/serialization_tool/types/json/constants.py
--rw-rw-rw-   0        0        0      578 2023-05-17 19:50:20.000000 serialization_tool-0.5/src/serialization_tool/types/json/json.py
--rw-rw-rw-   0        0        0     6666 2023-05-11 06:39:24.000000 serialization_tool-0.5/src/serialization_tool/types/json/utilities.py
--rw-rw-rw-   0        0        0      468 2023-05-01 04:12:05.000000 serialization_tool-0.5/src/serialization_tool/types/serialization.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.141834 serialization_tool-0.5/src/serialization_tool/types/xml/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.5/src/serialization_tool/types/xml/__init__.py
--rw-rw-rw-   0        0        0      132 2023-05-11 08:00:16.000000 serialization_tool-0.5/src/serialization_tool/types/xml/constants.py
--rw-rw-rw-   0        0        0     5111 2023-05-18 08:07:49.000000 serialization_tool-0.5/src/serialization_tool/types/xml/utilities.py
--rw-rw-rw-   0        0        0      857 2023-05-17 19:38:24.000000 serialization_tool-0.5/src/serialization_tool/types/xml/xml.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.097847 serialization_tool-0.5/src/serialization_tool.egg-info/
--rw-rw-rw-   0        0        0      313 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      984 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 09:42:10.585728 serialization_tool-1.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      313 2023-05-18 09:42:10.586727 serialization_tool-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-1.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-18 09:42:10.599750 serialization_tool-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      426 2023-05-18 09:42:08.000000 serialization_tool-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:42:10.493192 serialization_tool-1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 09:42:10.505206 serialization_tool-1.0/src/serialization_tool/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.0/src/serialization_tool/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-1.0/src/serialization_tool/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:42:10.563761 serialization_tool-1.0/src/serialization_tool/serialization/
+-rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-1.0/src/serialization_tool/serialization/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-05-03 17:44:51.000000 serialization_tool-1.0/src/serialization_tool/serialization/constants.py
+-rw-rw-rw-   0        0        0     9770 2023-05-18 08:09:13.000000 serialization_tool-1.0/src/serialization_tool/serialization/serializer.py
+-rw-rw-rw-   0        0        0      465 2023-05-03 20:36:54.000000 serialization_tool-1.0/src/serialization_tool/serialization_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:42:10.568747 serialization_tool-1.0/src/serialization_tool/types/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.0/src/serialization_tool/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:42:10.576747 serialization_tool-1.0/src/serialization_tool/types/json/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.0/src/serialization_tool/types/json/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-28 13:23:00.000000 serialization_tool-1.0/src/serialization_tool/types/json/constants.py
+-rw-rw-rw-   0        0        0      578 2023-05-17 19:50:20.000000 serialization_tool-1.0/src/serialization_tool/types/json/json.py
+-rw-rw-rw-   0        0        0     6666 2023-05-18 09:38:10.000000 serialization_tool-1.0/src/serialization_tool/types/json/utilities.py
+-rw-rw-rw-   0        0        0      468 2023-05-01 04:12:05.000000 serialization_tool-1.0/src/serialization_tool/types/serialization.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:42:10.584741 serialization_tool-1.0/src/serialization_tool/types/xml/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-1.0/src/serialization_tool/types/xml/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-05-11 08:00:16.000000 serialization_tool-1.0/src/serialization_tool/types/xml/constants.py
+-rw-rw-rw-   0        0        0     2246 2023-05-18 09:36:12.000000 serialization_tool-1.0/src/serialization_tool/types/xml/utilities.py
+-rw-rw-rw-   0        0        0      857 2023-05-18 09:35:59.000000 serialization_tool-1.0/src/serialization_tool/types/xml/xml.py
+drwxrwxrwx   0        0        0        0 2023-05-18 09:42:10.555722 serialization_tool-1.0/src/serialization_tool.egg-info/
+-rw-rw-rw-   0        0        0      313 2023-05-18 09:42:10.000000 serialization_tool-1.0/src/serialization_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-05-18 09:42:10.000000 serialization_tool-1.0/src/serialization_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 09:42:10.000000 serialization_tool-1.0/src/serialization_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-18 09:42:10.000000 serialization_tool-1.0/src/serialization_tool.egg-info/top_level.txt
```

### Comparing `serialization_tool-0.5/LICENSE.txt` & `serialization_tool-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `serialization_tool-0.5/src/serialization_tool/serialization/constants.py` & `serialization_tool-1.0/src/serialization_tool/serialization/constants.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-0.5/src/serialization_tool/serialization/serializer.py` & `serialization_tool-1.0/src/serialization_tool/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-0.5/src/serialization_tool/types/json/json.py` & `serialization_tool-1.0/src/serialization_tool/types/json/json.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-0.5/src/serialization_tool/types/json/utilities.py` & `serialization_tool-1.0/src/serialization_tool/types/json/utilities.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-0.5/src/serialization_tool/types/xml/xml.py` & `serialization_tool-1.0/src/serialization_tool/types/xml/xml.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-0.5/src/serialization_tool.egg-info/SOURCES.txt` & `serialization_tool-1.0/src/serialization_tool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.py
 src/serialization_tool/__init__.py
 src/serialization_tool/constants.py
 src/serialization_tool/serialization_factory.py
 src/serialization_tool.egg-info/PKG-INFO
 src/serialization_tool.egg-info/SOURCES.txt
 src/serialization_tool.egg-info/dependency_links.txt
-src/serialization_tool.egg-info/requires.txt
 src/serialization_tool.egg-info/top_level.txt
 src/serialization_tool/serialization/__init__.py
 src/serialization_tool/serialization/constants.py
 src/serialization_tool/serialization/serializer.py
 src/serialization_tool/types/__init__.py
 src/serialization_tool/types/serialization.py
 src/serialization_tool/types/json/__init__.py
```

