# Comparing `tmp/nextaddatamodule-0.0.1.tar.gz` & `tmp/nextaddatamodule-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextaddatamodule-0.0.1.tar", last modified: Thu May 18 07:35:39 2023, max compression
+gzip compressed data, was "nextaddatamodule-0.0.2.tar", last modified: Thu May 18 07:44:08 2023, max compression
```

## Comparing `nextaddatamodule-0.0.1.tar` & `nextaddatamodule-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:35:39.869593 nextaddatamodule-0.0.1/
--rw-r--r--   0 likaiyun   (501) staff       (20)      520 2023-05-18 07:35:39.869213 nextaddatamodule-0.0.1/PKG-INFO
-drwxr-xr-x   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:35:39.859115 nextaddatamodule-0.0.1/nextaddatamodule/
--rw-r--r--   0 likaiyun   (501) staff       (20)       19 2023-05-18 07:18:02.000000 nextaddatamodule-0.0.1/nextaddatamodule/__init__.py
--rw-r--r--   0 likaiyun   (501) staff       (20)       31 2023-05-18 07:17:50.000000 nextaddatamodule-0.0.1/nextaddatamodule/add.py
-drwxr-xr-x   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:35:39.868597 nextaddatamodule-0.0.1/nextaddatamodule/dataapi/
--rw-r--r--   0 likaiyun   (501) staff       (20)       24 2023-05-18 07:17:25.000000 nextaddatamodule-0.0.1/nextaddatamodule/dataapi/__init__.py
--rw-r--r--   0 likaiyun   (501) staff       (20)       31 2023-05-18 07:17:09.000000 nextaddatamodule-0.0.1/nextaddatamodule/dataapi/multiply.py
-drwxr-xr-x   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:35:39.866489 nextaddatamodule-0.0.1/nextaddatamodule.egg-info/
--rw-r--r--   0 likaiyun   (501) staff       (20)      520 2023-05-18 07:35:39.000000 nextaddatamodule-0.0.1/nextaddatamodule.egg-info/PKG-INFO
--rw-r--r--   0 likaiyun   (501) staff       (20)      295 2023-05-18 07:35:39.000000 nextaddatamodule-0.0.1/nextaddatamodule.egg-info/SOURCES.txt
--rw-r--r--   0 likaiyun   (501) staff       (20)        1 2023-05-18 07:35:39.000000 nextaddatamodule-0.0.1/nextaddatamodule.egg-info/dependency_links.txt
--rw-r--r--   0 likaiyun   (501) staff       (20)       17 2023-05-18 07:35:39.000000 nextaddatamodule-0.0.1/nextaddatamodule.egg-info/top_level.txt
--rw-r--r--   0 likaiyun   (501) staff       (20)       38 2023-05-18 07:35:39.869731 nextaddatamodule-0.0.1/setup.cfg
--rw-r--r--   0 likaiyun   (501) staff       (20)     1013 2023-05-18 07:35:23.000000 nextaddatamodule-0.0.1/setup.py
+drwxr-xr-x   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:44:08.160991 nextaddatamodule-0.0.2/
+-rw-r--r--   0 likaiyun   (501) staff       (20)      520 2023-05-18 07:44:08.160611 nextaddatamodule-0.0.2/PKG-INFO
+drwxr-xr-x   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:44:08.151148 nextaddatamodule-0.0.2/nextaddatamodule/
+-rw-r--r--   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:43:35.000000 nextaddatamodule-0.0.2/nextaddatamodule/__init__.py
+-rw-r--r--   0 likaiyun   (501) staff       (20)       31 2023-05-18 07:17:50.000000 nextaddatamodule-0.0.2/nextaddatamodule/add.py
+drwxr-xr-x   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:44:08.159444 nextaddatamodule-0.0.2/nextaddatamodule/dataapi/
+-rw-r--r--   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:43:44.000000 nextaddatamodule-0.0.2/nextaddatamodule/dataapi/__init__.py
+-rw-r--r--   0 likaiyun   (501) staff       (20)       31 2023-05-18 07:17:09.000000 nextaddatamodule-0.0.2/nextaddatamodule/dataapi/multiply.py
+drwxr-xr-x   0 likaiyun   (501) staff       (20)        0 2023-05-18 07:44:08.157044 nextaddatamodule-0.0.2/nextaddatamodule.egg-info/
+-rw-r--r--   0 likaiyun   (501) staff       (20)      520 2023-05-18 07:44:08.000000 nextaddatamodule-0.0.2/nextaddatamodule.egg-info/PKG-INFO
+-rw-r--r--   0 likaiyun   (501) staff       (20)      295 2023-05-18 07:44:08.000000 nextaddatamodule-0.0.2/nextaddatamodule.egg-info/SOURCES.txt
+-rw-r--r--   0 likaiyun   (501) staff       (20)        1 2023-05-18 07:44:08.000000 nextaddatamodule-0.0.2/nextaddatamodule.egg-info/dependency_links.txt
+-rw-r--r--   0 likaiyun   (501) staff       (20)       17 2023-05-18 07:44:08.000000 nextaddatamodule-0.0.2/nextaddatamodule.egg-info/top_level.txt
+-rw-r--r--   0 likaiyun   (501) staff       (20)       38 2023-05-18 07:44:08.161124 nextaddatamodule-0.0.2/setup.cfg
+-rw-r--r--   0 likaiyun   (501) staff       (20)     1013 2023-05-18 07:44:01.000000 nextaddatamodule-0.0.2/setup.py
```

### Comparing `nextaddatamodule-0.0.1/PKG-INFO` & `nextaddatamodule-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextaddatamodule
-Version: 0.0.1
+Version: 0.0.2
 Summary: My first Python package
 Author: karrylee
 Author-email: zylky8023@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `nextaddatamodule-0.0.1/nextaddatamodule.egg-info/PKG-INFO` & `nextaddatamodule-0.0.2/nextaddatamodule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextaddatamodule
-Version: 0.0.1
+Version: 0.0.2
 Summary: My first Python package
 Author: karrylee
 Author-email: zylky8023@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `nextaddatamodule-0.0.1/setup.py` & `nextaddatamodule-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # 配置
 setup(
        # 名称必须匹配文件名 'verysimplemodule'
         name="nextaddatamodule",
```

