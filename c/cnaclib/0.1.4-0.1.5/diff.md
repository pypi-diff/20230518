# Comparing `tmp/cnaclib-0.1.4.tar.gz` & `tmp/cnaclib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnaclib-0.1.4.tar", last modified: Thu May 18 13:28:14 2023, max compression
+gzip compressed data, was "cnaclib-0.1.5.tar", last modified: Thu May 18 14:07:28 2023, max compression
```

## Comparing `cnaclib-0.1.4.tar` & `cnaclib-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 13:28:14.727321 cnaclib-0.1.4/
--rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      392 2023-05-18 13:28:14.726321 cnaclib-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2023-05-18 11:56:52.000000 cnaclib-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 13:28:14.703321 cnaclib-0.1.4/cnaclib/
--rw-rw-rw-   0        0        0       16 2023-05-10 11:58:44.000000 cnaclib-0.1.4/cnaclib/__init__.py
--rw-rw-rw-   0        0        0    21717 2023-05-18 09:49:05.000000 cnaclib-0.1.4/cnaclib/rac.py
--rw-rw-rw-   0        0        0    21757 2023-05-11 15:43:48.000000 cnaclib-0.1.4/cnaclib/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-18 13:28:14.722321 cnaclib-0.1.4/cnaclib.egg-info/
--rw-rw-rw-   0        0        0      392 2023-05-18 13:28:14.000000 cnaclib-0.1.4/cnaclib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-18 13:28:14.000000 cnaclib-0.1.4/cnaclib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 13:28:14.000000 cnaclib-0.1.4/cnaclib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-05-18 13:28:14.000000 cnaclib-0.1.4/cnaclib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 13:28:14.000000 cnaclib-0.1.4/cnaclib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 13:28:14.728321 cnaclib-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1012 2023-05-18 13:26:43.000000 cnaclib-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:07:28.516067 cnaclib-0.1.5/
+-rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      392 2023-05-18 14:07:28.514067 cnaclib-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1826 2023-05-18 14:06:31.000000 cnaclib-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 14:07:28.433059 cnaclib-0.1.5/cnaclib/
+-rw-rw-rw-   0        0        0       16 2023-05-10 11:58:44.000000 cnaclib-0.1.5/cnaclib/__init__.py
+-rw-rw-rw-   0        0        0    21717 2023-05-18 09:49:05.000000 cnaclib-0.1.5/cnaclib/rac.py
+-rw-rw-rw-   0        0        0    21757 2023-05-11 15:43:48.000000 cnaclib-0.1.5/cnaclib/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:07:28.510067 cnaclib-0.1.5/cnaclib.egg-info/
+-rw-rw-rw-   0        0        0      392 2023-05-18 14:07:27.000000 cnaclib-0.1.5/cnaclib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-18 14:07:27.000000 cnaclib-0.1.5/cnaclib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 14:07:27.000000 cnaclib-0.1.5/cnaclib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-05-18 14:07:27.000000 cnaclib-0.1.5/cnaclib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 14:07:27.000000 cnaclib-0.1.5/cnaclib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 14:07:28.541070 cnaclib-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2023-05-18 14:06:50.000000 cnaclib-0.1.5/setup.py
```

### Comparing `cnaclib-0.1.4/LICENSE.txt` & `cnaclib-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.4/README.md` & `cnaclib-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# cnaclib : Librairie Python développée pour les usagers et les employés de la CNAC. 
+# cnaclib : Librairie Python développée la CNAC. 
 
 ## About cnaclib
 
 **cnaclib** C’est un package `Python` dédié aux usagers et aux employés de la CNAC.
 
-## Pourquoi utiliser cnaclib ?
+## Pourquoi utiliser cnaclib?
 
 * Il dispose de plusieurs modules et fonctions `Python` pour : 
     * Faire une simulation de calculs pour le bénéfice du régime d’assurance chômage (RAC)
     * Faire une simulation de calculs pour le bénéfice des mesures d’encouragement à l’emploi (loi 06-21)
     * Générer la liste des codes de wilaya de 01 à 58
     * Avoir le nom de la wilaya en arabe ou en français en fonction de son code 
     * Avoir le code de la wilaya en fonction de son nom en arabe ou en français
```

### Comparing `cnaclib-0.1.4/cnaclib/rac.py` & `cnaclib-0.1.5/cnaclib/rac.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.4/cnaclib/tools.py` & `cnaclib-0.1.5/cnaclib/tools.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.4/setup.py` & `cnaclib-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name = 'cnaclib',
-    version = '0.1.4',
+    version = '0.1.5',
     author= 'BENHAMADA Nadir',
     author_email="aistatendz@gmail.com",
     description='Simulateur RAC',
     packages=setuptools.find_packages(),
     install_requires=["certifi>=2023.5.7",
                       "charset-normalizer>=3.1.0",
                        "cnaclib>=0.1",
```

