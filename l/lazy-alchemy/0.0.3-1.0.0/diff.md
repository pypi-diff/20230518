# Comparing `tmp/lazy_alchemy-0.0.3.tar.gz` & `tmp/lazy_alchemy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_alchemy-0.0.3.tar", last modified: Thu May 18 09:09:09 2023, max compression
+gzip compressed data, was "lazy_alchemy-1.0.0.tar", last modified: Fri Jul  1 10:36:14 2022, max compression
```

## Comparing `lazy_alchemy-0.0.3.tar` & `lazy_alchemy-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 satyamsoni   (501) staff       (20)        0 2023-05-18 09:09:09.633925 lazy_alchemy-0.0.3/
--rw-r--r--   0 satyamsoni   (501) staff       (20)     1061 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/LICENSE
--rw-r--r--   0 satyamsoni   (501) staff       (20)       28 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/MANIFEST.in
--rw-r--r--   0 satyamsoni   (501) staff       (20)     4000 2023-05-18 09:09:09.633991 lazy_alchemy-0.0.3/PKG-INFO
--rw-r--r--   0 satyamsoni   (501) staff       (20)     2692 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/README.md
-drwxr-xr-x   0 satyamsoni   (501) staff       (20)        0 2023-05-18 09:09:09.632800 lazy_alchemy-0.0.3/lazy_alchemy/
--rw-r--r--   0 satyamsoni   (501) staff       (20)        5 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/lazy_alchemy/VERSION
--rw-r--r--   0 satyamsoni   (501) staff       (20)      268 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/lazy_alchemy/__init__.py
--rw-r--r--   0 satyamsoni   (501) staff       (20)     1730 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/lazy_alchemy/lazy_alchemy.py
-drwxr-xr-x   0 satyamsoni   (501) staff       (20)        0 2023-05-18 09:09:09.633426 lazy_alchemy-0.0.3/lazy_alchemy.egg-info/
--rw-r--r--   0 satyamsoni   (501) staff       (20)     4000 2023-05-18 09:09:09.000000 lazy_alchemy-0.0.3/lazy_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 satyamsoni   (501) staff       (20)      360 2023-05-18 09:09:09.000000 lazy_alchemy-0.0.3/lazy_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 satyamsoni   (501) staff       (20)        1 2023-05-18 09:09:09.000000 lazy_alchemy-0.0.3/lazy_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 satyamsoni   (501) staff       (20)       42 2023-05-18 09:09:09.000000 lazy_alchemy-0.0.3/lazy_alchemy.egg-info/requires.txt
--rw-r--r--   0 satyamsoni   (501) staff       (20)       19 2023-05-18 09:09:09.000000 lazy_alchemy-0.0.3/lazy_alchemy.egg-info/top_level.txt
--rw-r--r--   0 satyamsoni   (501) staff       (20)      232 2023-05-18 09:09:09.634219 lazy_alchemy-0.0.3/setup.cfg
--rw-r--r--   0 satyamsoni   (501) staff       (20)     1886 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/setup.py
-drwxr-xr-x   0 satyamsoni   (501) staff       (20)        0 2023-05-18 09:09:09.633812 lazy_alchemy-0.0.3/tests/
--rw-r--r--   0 satyamsoni   (501) staff       (20)        0 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/tests/__init__.py
--rw-r--r--   0 satyamsoni   (501) staff       (20)      599 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/tests/seed_db.py
--rw-r--r--   0 satyamsoni   (501) staff       (20)     1941 2023-05-18 09:05:55.000000 lazy_alchemy-0.0.3/tests/test_lazy_orm.py
+drwxr-xr-x   0 satyamsoni   (501) staff       (20)        0 2022-07-01 10:36:14.109818 lazy_alchemy-1.0.0/
+-rw-r--r--   0 satyamsoni   (501) staff       (20)     1061 2022-07-01 09:29:13.000000 lazy_alchemy-1.0.0/LICENSE
+-rw-r--r--   0 satyamsoni   (501) staff       (20)       15 2022-07-01 09:29:13.000000 lazy_alchemy-1.0.0/MANIFEST.in
+-rw-r--r--   0 satyamsoni   (501) staff       (20)     4000 2022-07-01 10:36:14.109883 lazy_alchemy-1.0.0/PKG-INFO
+-rw-r--r--   0 satyamsoni   (501) staff       (20)     2692 2022-07-01 10:25:25.000000 lazy_alchemy-1.0.0/README.md
+drwxr-xr-x   0 satyamsoni   (501) staff       (20)        0 2022-07-01 10:36:14.108910 lazy_alchemy-1.0.0/lazy_alchemy/
+-rw-r--r--   0 satyamsoni   (501) staff       (20)      268 2022-07-01 09:29:13.000000 lazy_alchemy-1.0.0/lazy_alchemy/__init__.py
+-rw-r--r--   0 satyamsoni   (501) staff       (20)     1730 2022-07-01 09:29:13.000000 lazy_alchemy-1.0.0/lazy_alchemy/lazy_alchemy.py
+drwxr-xr-x   0 satyamsoni   (501) staff       (20)        0 2022-07-01 10:36:14.109437 lazy_alchemy-1.0.0/lazy_alchemy.egg-info/
+-rw-r--r--   0 satyamsoni   (501) staff       (20)     4000 2022-07-01 10:36:13.000000 lazy_alchemy-1.0.0/lazy_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 satyamsoni   (501) staff       (20)      339 2022-07-01 10:36:14.000000 lazy_alchemy-1.0.0/lazy_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 satyamsoni   (501) staff       (20)        1 2022-07-01 10:36:13.000000 lazy_alchemy-1.0.0/lazy_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 satyamsoni   (501) staff       (20)       38 2022-07-01 10:36:14.000000 lazy_alchemy-1.0.0/lazy_alchemy.egg-info/requires.txt
+-rw-r--r--   0 satyamsoni   (501) staff       (20)       19 2022-07-01 10:36:14.000000 lazy_alchemy-1.0.0/lazy_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 satyamsoni   (501) staff       (20)      232 2022-07-01 10:36:14.110276 lazy_alchemy-1.0.0/setup.cfg
+-rw-r--r--   0 satyamsoni   (501) staff       (20)     1850 2022-07-01 09:29:13.000000 lazy_alchemy-1.0.0/setup.py
+drwxr-xr-x   0 satyamsoni   (501) staff       (20)        0 2022-07-01 10:36:14.109732 lazy_alchemy-1.0.0/tests/
+-rw-r--r--   0 satyamsoni   (501) staff       (20)        0 2022-07-01 09:29:13.000000 lazy_alchemy-1.0.0/tests/__init__.py
+-rw-r--r--   0 satyamsoni   (501) staff       (20)      599 2022-07-01 09:29:13.000000 lazy_alchemy-1.0.0/tests/seed_db.py
+-rw-r--r--   0 satyamsoni   (501) staff       (20)     1941 2022-07-01 09:29:13.000000 lazy_alchemy-1.0.0/tests/test_lazy_orm.py
```

### Comparing `lazy_alchemy-0.0.3/LICENSE` & `lazy_alchemy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lazy_alchemy-0.0.3/PKG-INFO` & `lazy_alchemy-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy_alchemy
-Version: 0.0.3
+Version: 1.0.0
 Summary: Lazy-Alchemy is a Python package that loads the DB models lazily.
 Home-page: https://github.com/satyamsoni2211/lazy_alchemy
 Author: Satyam Soni
 Author-email: satyamsoni@hotmail.co.uk
 License: MIT
 Keywords: sqlalchemy,alchemy,mysql,postgres,mssql,sql,sqlite,lazy,performance,orm,mapper,performance,database,lazy,relational,classes,oops,metaclass
 Platform: any
```

### Comparing `lazy_alchemy-0.0.3/README.md` & `lazy_alchemy-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lazy_alchemy-0.0.3/lazy_alchemy/lazy_alchemy.py` & `lazy_alchemy-1.0.0/lazy_alchemy/lazy_alchemy.py`

 * *Files identical despite different names*

### Comparing `lazy_alchemy-0.0.3/lazy_alchemy.egg-info/PKG-INFO` & `lazy_alchemy-1.0.0/lazy_alchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-alchemy
-Version: 0.0.3
+Version: 1.0.0
 Summary: Lazy-Alchemy is a Python package that loads the DB models lazily.
 Home-page: https://github.com/satyamsoni2211/lazy_alchemy
 Author: Satyam Soni
 Author-email: satyamsoni@hotmail.co.uk
 License: MIT
 Keywords: sqlalchemy,alchemy,mysql,postgres,mssql,sql,sqlite,lazy,performance,orm,mapper,performance,database,lazy,relational,classes,oops,metaclass
 Platform: any
```

### Comparing `lazy_alchemy-0.0.3/setup.py` & `lazy_alchemy-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 PACKAGE_NAME = "lazy_alchemy"
 
 setup(
     name=PACKAGE_NAME,
     version=version,
     license="MIT",
     packages=find_packages(exclude=["test"]),
-    include_package_data=True,
     description="Lazy-Alchemy is a Python package that loads the DB models lazily.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Satyam Soni",
     author_email="satyamsoni@hotmail.co.uk",
     url="https://github.com/satyamsoni2211/lazy_alchemy",
     keywords=["sqlalchemy", "alchemy", "mysql", "postgres",
               "mssql", "sql", "sqlite", "lazy", "performance",
               "orm", "mapper", "performance", "database", "lazy",
               "relational", "classes", "oops", "metaclass"],
     install_requires=[
-        "sqlalchemy <2.0",
+        "sqlalchemy",
     ],
     classifiers=[
         # See https://pypi.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
```

### Comparing `lazy_alchemy-0.0.3/tests/seed_db.py` & `lazy_alchemy-1.0.0/tests/seed_db.py`

 * *Files identical despite different names*

### Comparing `lazy_alchemy-0.0.3/tests/test_lazy_orm.py` & `lazy_alchemy-1.0.0/tests/test_lazy_orm.py`

 * *Files identical despite different names*

