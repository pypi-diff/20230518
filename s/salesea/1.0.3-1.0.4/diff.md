# Comparing `tmp/salesea-1.0.3.tar.gz` & `tmp/salesea-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesea-1.0.3.tar", last modified: Thu May 18 09:49:49 2023, max compression
+gzip compressed data, was "salesea-1.0.4.tar", last modified: Thu May 18 10:22:24 2023, max compression
```

## Comparing `salesea-1.0.3.tar` & `salesea-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 09:49:49.822657 salesea-1.0.3/
--rw-rw-rw-   0        0        0     2072 2023-05-18 09:49:49.822657 salesea-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1431 2023-05-18 09:19:56.000000 salesea-1.0.3/README.md
--rw-rw-rw-   0        0        0      111 2023-05-18 09:49:49.822657 salesea-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1484 2023-05-18 09:49:42.000000 salesea-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:49:49.803628 salesea-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 09:49:49.815659 salesea-1.0.3/src/salesea/
--rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.3/src/salesea/__init__.py
--rw-rw-rw-   0        0        0     1916 2023-05-18 08:27:21.000000 salesea-1.0.3/src/salesea/__main__.py
--rw-rw-rw-   0        0        0     7607 2023-05-18 09:43:08.000000 salesea-1.0.3/src/salesea/app.py
--rw-rw-rw-   0        0        0     3509 2023-05-18 08:19:26.000000 salesea-1.0.3/src/salesea/config.py
--rw-rw-rw-   0        0        0      715 2023-05-18 08:26:30.000000 salesea-1.0.3/src/salesea/log.py
--rw-rw-rw-   0        0        0     7418 2023-05-18 09:49:15.000000 salesea-1.0.3/src/salesea/nginx.py
--rw-rw-rw-   0        0        0      936 2023-05-18 09:22:59.000000 salesea-1.0.3/src/salesea/solution.py
--rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.3/src/salesea/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-18 09:49:49.821627 salesea-1.0.3/src/salesea.egg-info/
--rw-rw-rw-   0        0        0     2072 2023-05-18 09:49:49.000000 salesea-1.0.3/src/salesea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-18 09:49:49.000000 salesea-1.0.3/src/salesea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 09:49:49.000000 salesea-1.0.3/src/salesea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-18 09:49:49.000000 salesea-1.0.3/src/salesea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-18 09:49:49.000000 salesea-1.0.3/src/salesea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 09:49:49.000000 salesea-1.0.3/src/salesea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 10:22:24.680713 salesea-1.0.4/
+-rw-rw-rw-   0        0        0     2047 2023-05-18 10:22:24.680713 salesea-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1431 2023-05-18 09:19:56.000000 salesea-1.0.4/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-18 10:22:24.681712 salesea-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1844 2023-05-18 10:22:20.000000 salesea-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:22:24.655715 salesea-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 10:22:24.673713 salesea-1.0.4/src/salesea/
+-rw-rw-rw-   0        0        0       25 2023-05-18 07:08:55.000000 salesea-1.0.4/src/salesea/__init__.py
+-rw-rw-rw-   0        0        0     1916 2023-05-18 08:27:21.000000 salesea-1.0.4/src/salesea/__main__.py
+-rw-rw-rw-   0        0        0     7607 2023-05-18 09:43:08.000000 salesea-1.0.4/src/salesea/app.py
+-rw-rw-rw-   0        0        0     3509 2023-05-18 08:19:26.000000 salesea-1.0.4/src/salesea/config.py
+-rw-rw-rw-   0        0        0      715 2023-05-18 08:26:30.000000 salesea-1.0.4/src/salesea/log.py
+-rw-rw-rw-   0        0        0     7418 2023-05-18 09:49:15.000000 salesea-1.0.4/src/salesea/nginx.py
+-rw-rw-rw-   0        0        0      936 2023-05-18 09:22:59.000000 salesea-1.0.4/src/salesea/solution.py
+-rw-rw-rw-   0        0        0      134 2023-05-18 07:39:33.000000 salesea-1.0.4/src/salesea/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:22:24.679714 salesea-1.0.4/src/salesea.egg-info/
+-rw-rw-rw-   0        0        0     2047 2023-05-18 10:22:24.000000 salesea-1.0.4/src/salesea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-05-18 10:22:24.000000 salesea-1.0.4/src/salesea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 10:22:24.000000 salesea-1.0.4/src/salesea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-18 10:22:24.000000 salesea-1.0.4/src/salesea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      150 2023-05-18 10:22:24.000000 salesea-1.0.4/src/salesea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 10:22:24.000000 salesea-1.0.4/src/salesea.egg-info/top_level.txt
```

### Comparing `salesea-1.0.3/PKG-INFO` & `salesea-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # salesea@nginx-log-parser
 
 ## 开始使用
 
 > 网络姻缘一线牵 珍惜这段缘
```

### Comparing `salesea-1.0.3/README.md` & `salesea-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `salesea-1.0.3/src/salesea/__main__.py` & `salesea-1.0.4/src/salesea/__main__.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.3/src/salesea/app.py` & `salesea-1.0.4/src/salesea/app.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.3/src/salesea/config.py` & `salesea-1.0.4/src/salesea/config.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.3/src/salesea/log.py` & `salesea-1.0.4/src/salesea/log.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.3/src/salesea/nginx.py` & `salesea-1.0.4/src/salesea/nginx.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.3/src/salesea/solution.py` & `salesea-1.0.4/src/salesea/solution.py`

 * *Files identical despite different names*

### Comparing `salesea-1.0.3/src/salesea.egg-info/PKG-INFO` & `salesea-1.0.4/src/salesea.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: salesea
-Version: 1.0.3
+Version: 1.0.4
 Summary: This is an Nginx log collection tool.
 Author: howard
 Author-email: 18071131140telephone@gmail.com
 Keywords: nginx,logs,collection
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # salesea@nginx-log-parser
 
 ## 开始使用
 
 > 网络姻缘一线牵 珍惜这段缘
```

