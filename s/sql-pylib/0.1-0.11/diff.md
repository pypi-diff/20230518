# Comparing `tmp/sql-pylib-0.1.tar.gz` & `tmp/sql-pylib-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql-pylib-0.1.tar", last modified: Thu May 18 07:48:38 2023, max compression
+gzip compressed data, was "sql-pylib-0.11.tar", last modified: Thu May 18 08:16:26 2023, max compression
```

## Comparing `sql-pylib-0.1.tar` & `sql-pylib-0.11.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 07:48:38.333621 sql-pylib-0.1/
--rw-r--r--   0 docquity_prince   (501) staff       (20)     1035 2023-05-18 07:48:38.333420 sql-pylib-0.1/PKG-INFO
--rw-r--r--   0 docquity_prince   (501) staff       (20)      577 2023-05-18 07:48:29.000000 sql-pylib-0.1/README.md
--rw-r--r--   0 docquity_prince   (501) staff       (20)       38 2023-05-18 07:48:38.333684 sql-pylib-0.1/setup.cfg
--rw-r--r--   0 docquity_prince   (501) staff       (20)      813 2023-05-18 07:47:14.000000 sql-pylib-0.1/setup.py
-drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 07:48:38.331391 sql-pylib-0.1/sql_pylib/
--rw-r--r--   0 docquity_prince   (501) staff       (20)        0 2022-10-27 02:59:22.000000 sql-pylib-0.1/sql_pylib/__init__.py
--rw-r--r--   0 docquity_prince   (501) staff       (20)     3863 2022-10-27 02:59:22.000000 sql-pylib-0.1/sql_pylib/database_download_upload.py
--rw-r--r--   0 docquity_prince   (501) staff       (20)     1538 2022-10-27 02:59:22.000000 sql-pylib-0.1/sql_pylib/load_from_redshift_to_pandas.py
--rw-r--r--   0 docquity_prince   (501) staff       (20)    33155 2023-05-18 07:21:12.000000 sql-pylib-0.1/sql_pylib/sql_builder.py
-drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 07:48:38.333160 sql-pylib-0.1/sql_pylib.egg-info/
--rw-r--r--   0 docquity_prince   (501) staff       (20)     1035 2023-05-18 07:48:38.000000 sql-pylib-0.1/sql_pylib.egg-info/PKG-INFO
--rw-r--r--   0 docquity_prince   (501) staff       (20)      309 2023-05-18 07:48:38.000000 sql-pylib-0.1/sql_pylib.egg-info/SOURCES.txt
--rw-r--r--   0 docquity_prince   (501) staff       (20)        1 2023-05-18 07:48:38.000000 sql-pylib-0.1/sql_pylib.egg-info/dependency_links.txt
--rw-r--r--   0 docquity_prince   (501) staff       (20)       90 2023-05-18 07:48:38.000000 sql-pylib-0.1/sql_pylib.egg-info/requires.txt
--rw-r--r--   0 docquity_prince   (501) staff       (20)       10 2023-05-18 07:48:38.000000 sql-pylib-0.1/sql_pylib.egg-info/top_level.txt
+drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 08:16:26.337106 sql-pylib-0.11/
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     1036 2023-05-18 08:16:26.336907 sql-pylib-0.11/PKG-INFO
+-rw-r--r--   0 docquity_prince   (501) staff       (20)      577 2023-05-18 07:48:29.000000 sql-pylib-0.11/README.md
+-rw-r--r--   0 docquity_prince   (501) staff       (20)       38 2023-05-18 08:16:26.337159 sql-pylib-0.11/setup.cfg
+-rw-r--r--   0 docquity_prince   (501) staff       (20)      814 2023-05-18 08:15:32.000000 sql-pylib-0.11/setup.py
+drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 08:16:26.332332 sql-pylib-0.11/sql_pylib/
+-rw-r--r--   0 docquity_prince   (501) staff       (20)        0 2022-10-27 02:59:22.000000 sql-pylib-0.11/sql_pylib/__init__.py
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     3863 2022-10-27 02:59:22.000000 sql-pylib-0.11/sql_pylib/database_download_upload.py
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     1538 2022-10-27 02:59:22.000000 sql-pylib-0.11/sql_pylib/load_from_redshift_to_pandas.py
+-rw-r--r--   0 docquity_prince   (501) staff       (20)    33155 2023-05-18 07:21:12.000000 sql-pylib-0.11/sql_pylib/sql_builder.py
+drwxr-xr-x   0 docquity_prince   (501) staff       (20)        0 2023-05-18 08:16:26.336664 sql-pylib-0.11/sql_pylib.egg-info/
+-rw-r--r--   0 docquity_prince   (501) staff       (20)     1036 2023-05-18 08:16:26.000000 sql-pylib-0.11/sql_pylib.egg-info/PKG-INFO
+-rw-r--r--   0 docquity_prince   (501) staff       (20)      309 2023-05-18 08:16:26.000000 sql-pylib-0.11/sql_pylib.egg-info/SOURCES.txt
+-rw-r--r--   0 docquity_prince   (501) staff       (20)        1 2023-05-18 08:16:26.000000 sql-pylib-0.11/sql_pylib.egg-info/dependency_links.txt
+-rw-r--r--   0 docquity_prince   (501) staff       (20)       90 2023-05-18 08:16:26.000000 sql-pylib-0.11/sql_pylib.egg-info/requires.txt
+-rw-r--r--   0 docquity_prince   (501) staff       (20)       10 2023-05-18 08:16:26.000000 sql-pylib-0.11/sql_pylib.egg-info/top_level.txt
```

### Comparing `sql-pylib-0.1/PKG-INFO` & `sql-pylib-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-pylib
-Version: 0.1
+Version: 0.11
 Summary: Custom Python library for standard SQL tasks
 Home-page: https://github.com/PrinceJavier/sql_pylib
 Author: Prince Javier
 Author-email: othepjavier@gmail.com
 License: MIT
 Keywords: sql python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sql-pylib-0.1/README.md` & `sql-pylib-0.11/README.md`

 * *Files identical despite different names*

### Comparing `sql-pylib-0.1/setup.py` & `sql-pylib-0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sql-pylib',
-    version='0.1',
+    version='0.11',
     packages=find_packages(),
     description='Custom Python library for standard SQL tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Prince Javier',
     author_email='othepjavier@gmail.com',
     url='https://github.com/PrinceJavier/sql_pylib',
     install_requires=[
 		'pandas',
 		'numpy',
 		'python-decouple',
 		'tqdm',
-		'pymysql>=1.0.2',
-		'sqlalchemy>=1.4.0',
-		'psycopg2-binary>=2.9.1',
+		'pymysql==1.0.2',
+		'sqlalchemy==1.4.0',
+		'psycopg2-binary==2.9.1',
     		  ],  
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
```

### Comparing `sql-pylib-0.1/sql_pylib/database_download_upload.py` & `sql-pylib-0.11/sql_pylib/database_download_upload.py`

 * *Files identical despite different names*

### Comparing `sql-pylib-0.1/sql_pylib/load_from_redshift_to_pandas.py` & `sql-pylib-0.11/sql_pylib/load_from_redshift_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sql-pylib-0.1/sql_pylib/sql_builder.py` & `sql-pylib-0.11/sql_pylib/sql_builder.py`

 * *Files identical despite different names*

### Comparing `sql-pylib-0.1/sql_pylib.egg-info/PKG-INFO` & `sql-pylib-0.11/sql_pylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-pylib
-Version: 0.1
+Version: 0.11
 Summary: Custom Python library for standard SQL tasks
 Home-page: https://github.com/PrinceJavier/sql_pylib
 Author: Prince Javier
 Author-email: othepjavier@gmail.com
 License: MIT
 Keywords: sql python
 Classifier: Development Status :: 3 - Alpha
```

