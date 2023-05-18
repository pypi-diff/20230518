# Comparing `tmp/midiferenciacion-0.4.tar.gz` & `tmp/midiferenciacion-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midiferenciacion-0.4.tar", last modified: Thu May 18 17:39:11 2023, max compression
+gzip compressed data, was "midiferenciacion-0.41.tar", last modified: Thu May 18 18:46:28 2023, max compression
```

## Comparing `midiferenciacion-0.4.tar` & `midiferenciacion-0.41.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 17:39:11.277097 midiferenciacion-0.4/
--rw-r--r--   0 sarboledab   (501) staff       (20)     1134 2023-05-16 14:58:24.000000 midiferenciacion-0.4/LICENSE
--rw-r--r--   0 sarboledab   (501) staff       (20)      521 2023-05-18 17:39:11.276676 midiferenciacion-0.4/PKG-INFO
--rw-r--r--   0 sarboledab   (501) staff       (20)     1675 2023-05-16 14:58:20.000000 midiferenciacion-0.4/README.md
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 17:39:11.276129 midiferenciacion-0.4/midiferenciacion.egg-info/
--rw-r--r--   0 sarboledab   (501) staff       (20)      521 2023-05-18 17:39:11.000000 midiferenciacion-0.4/midiferenciacion.egg-info/PKG-INFO
--rw-r--r--   0 sarboledab   (501) staff       (20)      304 2023-05-18 17:39:11.000000 midiferenciacion-0.4/midiferenciacion.egg-info/SOURCES.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)        1 2023-05-18 17:39:11.000000 midiferenciacion-0.4/midiferenciacion.egg-info/dependency_links.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)       48 2023-05-18 17:39:11.000000 midiferenciacion-0.4/midiferenciacion.egg-info/entry_points.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)       11 2023-05-18 17:39:11.000000 midiferenciacion-0.4/midiferenciacion.egg-info/requires.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)        7 2023-05-18 17:39:11.000000 midiferenciacion-0.4/midiferenciacion.egg-info/top_level.txt
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 17:39:11.271456 midiferenciacion-0.4/midiff/
--rw-r--r--   0 sarboledab   (501) staff       (20)      500 2023-05-16 14:58:43.000000 midiferenciacion-0.4/midiff/__init__.py
--rw-r--r--   0 sarboledab   (501) staff       (20)      131 2023-05-16 14:58:32.000000 midiferenciacion-0.4/pyproject.toml
--rw-r--r--   0 sarboledab   (501) staff       (20)       38 2023-05-18 17:39:11.277298 midiferenciacion-0.4/setup.cfg
--rw-r--r--   0 sarboledab   (501) staff       (20)     2238 2023-05-18 17:39:08.000000 midiferenciacion-0.4/setup.py
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 18:46:28.781356 midiferenciacion-0.41/
+-rw-r--r--   0 sarboledab   (501) staff       (20)     1134 2023-05-16 14:58:24.000000 midiferenciacion-0.41/LICENSE
+-rw-r--r--   0 sarboledab   (501) staff       (20)      522 2023-05-18 18:46:28.780700 midiferenciacion-0.41/PKG-INFO
+-rw-r--r--   0 sarboledab   (501) staff       (20)     1585 2023-05-18 18:45:10.000000 midiferenciacion-0.41/README.md
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 18:46:28.774412 midiferenciacion-0.41/midiferenciacion/
+-rw-r--r--   0 sarboledab   (501) staff       (20)      158 2023-05-18 18:43:35.000000 midiferenciacion-0.41/midiferenciacion/__init__.py
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-18 18:46:28.779762 midiferenciacion-0.41/midiferenciacion.egg-info/
+-rw-r--r--   0 sarboledab   (501) staff       (20)      522 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/PKG-INFO
+-rw-r--r--   0 sarboledab   (501) staff       (20)      314 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/SOURCES.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)        1 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/dependency_links.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       48 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/entry_points.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       11 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/requires.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       17 2023-05-18 18:46:28.000000 midiferenciacion-0.41/midiferenciacion.egg-info/top_level.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)      131 2023-05-16 14:58:32.000000 midiferenciacion-0.41/pyproject.toml
+-rw-r--r--   0 sarboledab   (501) staff       (20)       38 2023-05-18 18:46:28.781556 midiferenciacion-0.41/setup.cfg
+-rw-r--r--   0 sarboledab   (501) staff       (20)     2239 2023-05-18 18:46:12.000000 midiferenciacion-0.41/setup.py
```

### Comparing `midiferenciacion-0.4/LICENSE` & `midiferenciacion-0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `midiferenciacion-0.4/PKG-INFO` & `midiferenciacion-0.41/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midiferenciacion
-Version: 0.4
+Version: 0.41
 Summary: Make a diferentiation of a given function
 Home-page: https://pypi.org/project/midiferenciacion
 Author: Sofia Arboleda-Bolivar
 Author-email: sofia.arboledab@udea.edu.co
 License: MIT
 Keywords: Dif math
 Classifier: Programming Language :: Python :: 3
```

### Comparing `midiferenciacion-0.4/midiferenciacion.egg-info/PKG-INFO` & `midiferenciacion-0.41/midiferenciacion.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midiferenciacion
-Version: 0.4
+Version: 0.41
 Summary: Make a diferentiation of a given function
 Home-page: https://pypi.org/project/midiferenciacion
 Author: Sofia Arboleda-Bolivar
 Author-email: sofia.arboledab@udea.edu.co
 License: MIT
 Keywords: Dif math
 Classifier: Programming Language :: Python :: 3
```

### Comparing `midiferenciacion-0.4/setup.py` & `midiferenciacion-0.41/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.4',
+    version='0.41',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

