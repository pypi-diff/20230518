# Comparing `tmp/baba-0.1.8b0.tar.gz` & `tmp/baba-0.1.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baba-0.1.8b0.tar", last modified: Thu May 18 03:28:06 2023, max compression
+gzip compressed data, was "baba-0.1.9b0.tar", last modified: Thu May 18 03:52:56 2023, max compression
```

## Comparing `baba-0.1.8b0.tar` & `baba-0.1.9b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:06.601644 baba-0.1.8b0/
--rw-rw-rw-   0        0        0     9234 2023-05-18 03:03:13.000000 baba-0.1.8b0/LICENSE.txt
--rw-rw-rw-   0        0        0     1842 2023-05-18 03:28:06.600621 baba-0.1.8b0/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2023-05-18 03:25:16.000000 baba-0.1.8b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:06.587657 baba-0.1.8b0/baba/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:52:03.000000 baba-0.1.8b0/baba/__init__.py
--rw-rw-rw-   0        0        0     2084 2023-05-18 03:06:44.000000 baba-0.1.8b0/baba/taskbase.py
--rw-rw-rw-   0        0        0      475 2023-05-17 12:38:08.000000 baba-0.1.8b0/baba/test.py
-drwxrwxrwx   0        0        0        0 2023-05-18 03:28:06.598658 baba-0.1.8b0/baba.egg-info/
--rw-rw-rw-   0        0        0     1842 2023-05-18 03:28:06.000000 baba-0.1.8b0/baba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-05-18 03:28:06.000000 baba-0.1.8b0/baba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 03:28:06.000000 baba-0.1.8b0/baba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-18 03:28:06.000000 baba-0.1.8b0/baba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 03:28:06.602641 baba-0.1.8b0/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-18 03:27:28.000000 baba-0.1.8b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 03:52:56.478274 baba-0.1.9b0/
+-rw-rw-rw-   0        0        0     9234 2023-05-18 03:03:13.000000 baba-0.1.9b0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1842 2023-05-18 03:52:56.477272 baba-0.1.9b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2023-05-18 03:25:16.000000 baba-0.1.9b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 03:52:56.462784 baba-0.1.9b0/baba/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:52:03.000000 baba-0.1.9b0/baba/__init__.py
+-rw-rw-rw-   0        0        0     2084 2023-05-18 03:06:44.000000 baba-0.1.9b0/baba/taskbase.py
+-rw-rw-rw-   0        0        0      475 2023-05-17 12:38:08.000000 baba-0.1.9b0/baba/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 03:52:56.472950 baba-0.1.9b0/baba.egg-info/
+-rw-rw-rw-   0        0        0     1842 2023-05-18 03:52:56.000000 baba-0.1.9b0/baba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-18 03:52:56.000000 baba-0.1.9b0/baba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 03:52:56.000000 baba-0.1.9b0/baba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-18 03:52:56.000000 baba-0.1.9b0/baba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 03:52:56.479271 baba-0.1.9b0/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2023-05-18 03:49:43.000000 baba-0.1.9b0/setup.py
```

### Comparing `baba-0.1.8b0/LICENSE.txt` & `baba-0.1.9b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baba-0.1.8b0/PKG-INFO` & `baba-0.1.9b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baba
-Version: 0.1.8b0
+Version: 0.1.9b0
 Summary: 好爸爸的每个类都是被用来继承的。作为顶层设计，它为通用行为实现了最基础的标准实践。比如自动埋点、权限控制、性能分析、任务流转、异常处理、单元测试等。
 Home-page: https://pypi.org/project/baba/
 Author: jie.kim
 Author-email: ubbs@163.com
 License: Apache
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `baba-0.1.8b0/README.md` & `baba-0.1.9b0/README.md`

 * *Files identical despite different names*

### Comparing `baba-0.1.8b0/baba/taskbase.py` & `baba-0.1.9b0/baba/taskbase.py`

 * *Files identical despite different names*

### Comparing `baba-0.1.8b0/baba.egg-info/PKG-INFO` & `baba-0.1.9b0/baba.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baba
-Version: 0.1.8b0
+Version: 0.1.9b0
 Summary: 好爸爸的每个类都是被用来继承的。作为顶层设计，它为通用行为实现了最基础的标准实践。比如自动埋点、权限控制、性能分析、任务流转、异常处理、单元测试等。
 Home-page: https://pypi.org/project/baba/
 Author: jie.kim
 Author-email: ubbs@163.com
 License: Apache
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

