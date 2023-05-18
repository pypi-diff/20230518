# Comparing `tmp/jwtools-0.1.2.tar.gz` & `tmp/jwtools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtools-0.1.2.tar", last modified: Thu May 18 02:17:01 2023, max compression
+gzip compressed data, was "jwtools-0.1.3.tar", last modified: Thu May 18 02:27:57 2023, max compression
```

## Comparing `jwtools-0.1.2.tar` & `jwtools-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 02:17:01.616776 jwtools-0.1.2/
--rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      907 2023-05-18 02:17:01.615776 jwtools-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-05-18 02:11:32.000000 jwtools-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 02:17:01.606777 jwtools-0.1.2/jwtools/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.2/jwtools/__init__.py
--rw-rw-rw-   0        0        0     1303 2023-05-18 02:16:45.000000 jwtools-0.1.2/jwtools/func.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:17:01.612781 jwtools-0.1.2/jwtools.egg-info/
--rw-rw-rw-   0        0        0      907 2023-05-18 02:17:01.000000 jwtools-0.1.2/jwtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-18 02:17:01.000000 jwtools-0.1.2/jwtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 02:17:01.000000 jwtools-0.1.2/jwtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-18 02:17:01.000000 jwtools-0.1.2/jwtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 02:17:01.616776 jwtools-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-05-18 02:08:17.000000 jwtools-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:17:01.614776 jwtools-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      210 2023-05-18 02:01:21.000000 jwtools-0.1.2/tests/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:27:57.899724 jwtools-0.1.3/
+-rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      851 2023-05-18 02:27:57.899724 jwtools-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-18 02:26:11.000000 jwtools-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 02:27:57.893721 jwtools-0.1.3/jwtools/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.3/jwtools/__init__.py
+-rw-rw-rw-   0        0        0     1303 2023-05-18 02:16:45.000000 jwtools-0.1.3/jwtools/func.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:27:57.896723 jwtools-0.1.3/jwtools.egg-info/
+-rw-rw-rw-   0        0        0      851 2023-05-18 02:27:57.000000 jwtools-0.1.3/jwtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-18 02:27:57.000000 jwtools-0.1.3/jwtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:27:57.000000 jwtools-0.1.3/jwtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-18 02:27:57.000000 jwtools-0.1.3/jwtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:27:57.899724 jwtools-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-05-18 02:27:05.000000 jwtools-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:27:57.898723 jwtools-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-05-18 02:01:21.000000 jwtools-0.1.3/tests/test1.py
```

### Comparing `jwtools-0.1.2/LICENSE` & `jwtools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.2/jwtools/func.py` & `jwtools-0.1.3/jwtools/func.py`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.2/setup.py` & `jwtools-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jwtools',
-    version='0.1.2',
+    version='0.1.3',
     description="It is a micro-toolbox that includes various common operations and will continue to be improved in the future.",
     long_description=open('README.md', encoding='utf-8').read(),
     include_package_data=True,
     author='jinghewang',
     author_email='jinghewang@163.com',
     license='MIT License',
     url='https://github.com/jinghewang/python-jwtools.git',
```

