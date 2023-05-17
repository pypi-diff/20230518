# Comparing `tmp/dynbps-0.0.4.tar.gz` & `tmp/dynbps-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynbps-0.0.4.tar", last modified: Wed May 17 12:34:58 2023, max compression
+gzip compressed data, was "dist/dynbps-0.0.5.tar", last modified: Wed May 17 22:36:32 2023, max compression
```

## Comparing `dynbps-0.0.4.tar` & `dynbps-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 12:34:58.282989 dynbps-0.0.4/
--rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.4/LICENSE
--rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.4/MANIFEST.in
--rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-17 12:34:58.281868 dynbps-0.0.4/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      284 2023-05-17 12:25:45.000000 dynbps-0.0.4/README.md
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 12:34:58.269639 dynbps-0.0.4/dynbps/
--rw-r--r--   0 josephrilling   (501) staff       (20)     9023 2023-05-17 12:25:54.000000 dynbps-0.0.4/dynbps/BPS.py
--rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-17 12:25:54.000000 dynbps-0.0.4/dynbps/__init__.py
--rw-r--r--   0 josephrilling   (501) staff       (20)      646 2023-05-17 12:25:54.000000 dynbps-0.0.4/dynbps/_modidx.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 12:34:58.279010 dynbps-0.0.4/dynbps.egg-info/
--rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      313 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/SOURCES.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/dependency_links.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/entry_points.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.4/dynbps.egg-info/not-zip-safe
--rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/requires.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-17 12:34:58.000000 dynbps-0.0.4/dynbps.egg-info/top_level.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-17 12:25:30.000000 dynbps-0.0.4/settings.ini
--rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-17 12:34:58.283156 dynbps-0.0.4/setup.cfg
--rw-rw-r--   0 josephrilling   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 dynbps-0.0.4/setup.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 22:36:32.599564 dynbps-0.0.5/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.5/LICENSE
+-rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.5/MANIFEST.in
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-17 22:36:32.598995 dynbps-0.0.5/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      284 2023-05-17 22:26:24.000000 dynbps-0.0.5/README.md
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 22:36:32.586451 dynbps-0.0.5/dynbps/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     9023 2023-05-17 22:36:20.000000 dynbps-0.0.5/dynbps/BPS.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-17 22:36:20.000000 dynbps-0.0.5/dynbps/__init__.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)      681 2023-05-17 22:36:20.000000 dynbps-0.0.5/dynbps/_modidx.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 22:36:32.597244 dynbps-0.0.5/dynbps/datasets/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    41999 2023-05-17 22:21:27.000000 dynbps-0.0.5/dynbps/datasets/data.xlsx
+-rw-r--r--   0 josephrilling   (501) staff       (20)      189 2023-05-17 22:36:20.000000 dynbps-0.0.5/dynbps/loadData.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-17 22:36:32.596489 dynbps-0.0.5/dynbps.egg-info/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1051 2023-05-17 22:36:32.000000 dynbps-0.0.5/dynbps.egg-info/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      358 2023-05-17 22:36:32.000000 dynbps-0.0.5/dynbps.egg-info/SOURCES.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-17 22:36:32.000000 dynbps-0.0.5/dynbps.egg-info/dependency_links.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-17 22:36:32.000000 dynbps-0.0.5/dynbps.egg-info/entry_points.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.5/dynbps.egg-info/not-zip-safe
+-rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-17 22:36:32.000000 dynbps-0.0.5/dynbps.egg-info/requires.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-17 22:36:32.000000 dynbps-0.0.5/dynbps.egg-info/top_level.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-17 22:36:20.000000 dynbps-0.0.5/settings.ini
+-rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-17 22:36:32.599725 dynbps-0.0.5/setup.cfg
+-rw-rw-r--   0 josephrilling   (501) staff       (20)     2640 2023-05-17 22:24:08.000000 dynbps-0.0.5/setup.py
```

### Comparing `dynbps-0.0.4/LICENSE` & `dynbps-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.4/PKG-INFO` & `dynbps-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.4/dynbps/BPS.py` & `dynbps-0.0.5/dynbps/BPS.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.4/dynbps/_modidx.py` & `dynbps-0.0.5/dynbps/_modidx.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,8 +4,9 @@
                 'doc_baseurl': '/dynbps',
                 'doc_host': 'https://josephrilling.github.io',
                 'git_url': 'https://github.com/josephrilling/dynbps',
                 'lib_path': 'dynbps'},
   'syms': { 'dynbps.BPS': { 'dynbps.BPS.BPS': ('bps.html#bps', 'dynbps/BPS.py'),
                             'dynbps.BPS.BPS.__init__': ('bps.html#bps.__init__', 'dynbps/BPS.py'),
                             'dynbps.BPS.BPS.fit': ('bps.html#bps.fit', 'dynbps/BPS.py'),
-                            'dynbps.BPS.BPS.predict': ('bps.html#bps.predict', 'dynbps/BPS.py')}}}
+                            'dynbps.BPS.BPS.predict': ('bps.html#bps.predict', 'dynbps/BPS.py')},
+            'dynbps.loadData': {}}}
```

### Comparing `dynbps-0.0.4/dynbps.egg-info/PKG-INFO` & `dynbps-0.0.5/dynbps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.4/settings.ini` & `dynbps-0.0.5/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dynbps
 lib_name = dynbps
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dynbps
 nbs_path = nbs
 recursive = True
```

### Comparing `dynbps-0.0.4/setup.py` & `dynbps-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         'Development Status :: ' + statuses[int(cfg['status'])],
         'Intended Audience :: ' + cfg['audience'].title(),
         'Natural Language :: ' + cfg['language'].title(),
     ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
+    package_data={'': ['datasets/*.xlsx']},
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
     long_description = open('README.md', encoding='utf-8').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
```

