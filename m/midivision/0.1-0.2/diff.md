# Comparing `tmp/midivision-0.1.tar.gz` & `tmp/midivision-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midivision-0.1.tar", last modified: Wed May 17 16:12:20 2023, max compression
+gzip compressed data, was "midivision-0.2.tar", last modified: Thu May 18 18:38:27 2023, max compression
```

## Comparing `midivision-0.1.tar` & `midivision-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:12:20.409849 midivision-0.1/
--rw-rw-rw-   0        0        0     1134 2023-05-16 14:58:24.000000 midivision-0.1/LICENSE
--rw-rw-rw-   0        0        0     2188 2023-05-17 16:12:20.408849 midivision-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1675 2023-05-16 14:58:20.000000 midivision-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 16:12:20.397844 midivision-0.1/midivision/
--rw-rw-rw-   0        0        0      500 2023-05-16 14:58:44.000000 midivision-0.1/midivision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 16:12:20.407849 midivision-0.1/midivision.egg-info/
--rw-rw-rw-   0        0        0     2188 2023-05-17 16:12:20.000000 midivision-0.1/midivision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-17 16:12:20.000000 midivision-0.1/midivision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:12:20.000000 midivision-0.1/midivision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-17 16:12:20.000000 midivision-0.1/midivision.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-05-17 16:12:20.000000 midivision-0.1/midivision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-17 16:12:20.000000 midivision-0.1/midivision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2023-05-16 14:58:32.000000 midivision-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 16:12:20.409849 midivision-0.1/setup.cfg
--rw-rw-rw-   0        0        0     2186 2023-05-16 18:47:57.000000 midivision-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:38:27.260375 midivision-0.2/
+-rw-rw-rw-   0        0        0     1134 2023-05-16 14:58:24.000000 midivision-0.2/LICENSE
+-rw-rw-rw-   0        0        0     2429 2023-05-18 18:38:27.260375 midivision-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1901 2023-05-18 18:37:38.000000 midivision-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 18:38:27.211142 midivision-0.2/midivision/
+-rw-rw-rw-   0        0        0      934 2023-05-18 18:19:52.000000 midivision-0.2/midivision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:38:27.260375 midivision-0.2/midivision.egg-info/
+-rw-rw-rw-   0        0        0     2429 2023-05-18 18:38:26.000000 midivision-0.2/midivision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-18 18:38:26.000000 midivision-0.2/midivision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:38:26.000000 midivision-0.2/midivision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-18 18:38:26.000000 midivision-0.2/midivision.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 18:38:26.000000 midivision-0.2/midivision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 18:38:26.000000 midivision-0.2/midivision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-05-16 14:58:32.000000 midivision-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 18:38:27.266916 midivision-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2151 2023-05-18 18:20:08.000000 midivision-0.2/setup.py
```

### Comparing `midivision-0.1/LICENSE` & `midivision-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `midivision-0.1/setup.py` & `midivision-0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     # ######################################################################
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        ],
-    version='0.1',
+    ],
+    version='0.2',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
-    
+
     # ######################################################################
     # ENTRY POINTS
     # ######################################################################
     entry_points={
         'console_scripts': ['install=midivision.install:main'],
     },
 
@@ -45,15 +45,15 @@
     # ######################################################################
     test_suite='nose.collector',
     tests_require=['nose'],
 
     # ######################################################################
     # DEPENDENCIES
     # ######################################################################
-    install_requires=['scipy','ipython','matplotlib','tqdm'],
+    install_requires=['ipython',],
 
     # ######################################################################
     # OPTIONS
     # ######################################################################
     include_package_data=True,
     package_data={'': ['data/*.*', 'tests/*.*']},
 )
```

