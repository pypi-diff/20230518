# Comparing `tmp/bioumlsim-0.2.0.tar.gz` & `tmp/bioumlsim-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.2.0.tar", last modified: Wed May 17 19:01:07 2023, max compression
+gzip compressed data, was "bioumlsim-0.2.1.tar", last modified: Thu May 18 18:10:00 2023, max compression
```

## Comparing `bioumlsim-0.2.0.tar` & `bioumlsim-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 19:01:07.951435 bioumlsim-0.2.0/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      771 2023-05-17 19:01:07.952405 bioumlsim-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.2.0/README.md
--rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      790 2023-05-17 19:01:07.953402 bioumlsim-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 19:01:07.929402 bioumlsim-0.2.0/src/
--rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.2.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:01:07.951435 bioumlsim-0.2.0/src/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-17 19:01:07.000000 bioumlsim-0.2.0/src/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2351 2023-05-17 18:45:43.000000 bioumlsim-0.2.0/src/bioumlsim.py
--rw-rw-rw-   0        0        0      377 2023-05-17 18:41:47.000000 bioumlsim-0.2.0/src/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:10:00.191411 bioumlsim-0.2.1/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-05-18 18:10:00.191411 bioumlsim-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.2.1/README.md
+-rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      798 2023-05-18 18:10:00.194918 bioumlsim-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 18:10:00.149430 bioumlsim-0.2.1/src/
+-rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:10:00.189411 bioumlsim-0.2.1/src/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-05-18 18:10:00.000000 bioumlsim-0.2.1/src/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-18 18:10:00.000000 bioumlsim-0.2.1/src/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:10:00.000000 bioumlsim-0.2.1/src/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.2.1/src/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-18 18:10:00.000000 bioumlsim-0.2.1/src/bioumlsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-18 18:10:00.000000 bioumlsim-0.2.1/src/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3210 2023-05-18 18:05:17.000000 bioumlsim-0.2.1/src/bioumlsim.py
+-rw-rw-rw-   0        0        0      345 2023-05-18 18:05:55.000000 bioumlsim-0.2.1/src/test.py
```

### Comparing `bioumlsim-0.2.0/LICENSE` & `bioumlsim-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.0/PKG-INFO` & `bioumlsim-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.2.0/setup.cfg` & `bioumlsim-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696f 756d 6c73 696d 0d0a 7665   = bioumlsim..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 300d 0a61  rsion = 0.2.0..a
+00000020: 7273 696f 6e20 3d20 302e 322e 310d 0a61  rsion = 0.2.1..a
 00000030: 7574 686f 7220 3d20 496c 7961 204b 6973  uthor = Ilya Kis
 00000040: 656c 6576 2c20 4269 6f73 6f66 742e 7275  elev, Biosoft.ru
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2034 7833 6375 7430 7240 676d 6169 6c2e   4x3cut0r@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2050 7974 686f 6e20 696e 7465 7266   = Python interf
 00000090: 6163 6520 666f 7220 7369 6d75 6c61 7469  ace for simulati
@@ -40,11 +40,11 @@
 00000270: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
 00000280: 4d61 7468 656d 6174 6963 730d 0a0d 0a5b  Mathematics....[
 00000290: 6f70 7469 6f6e 735d 0d0a 7079 7468 6f6e  options]..python
 000002a0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
 000002b0: 380d 0a7a 6970 5f73 6166 6520 3d20 4661  8..zip_safe = Fa
 000002c0: 6c73 650d 0a69 6e73 7461 6c6c 5f72 6571  lse..install_req
 000002d0: 7569 7265 7320 3d20 0d0a 094a 5079 7065  uires = ...JPype
-000002e0: 313d 3d31 2e34 2e31 0d0a 0d0a 5b65 6767  1==1.4.1....[egg
-000002f0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000300: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000310: 2030 0d0a 0d0a                            0....
+000002e0: 313d 3d31 2e34 2e31 0d0a 096e 756d 7079  1==1.4.1...numpy
+000002f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000300: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000310: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `bioumlsim-0.2.0/src/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.2.1/src/bioumlsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.2.0/src/bioumlsim.py` & `bioumlsim-0.2.1/src/bioumlsim.py`

 * *Files 17% similar despite different names*

```diff
@@ -59,8 +59,36 @@
             numpoints: number of time points
         Returns:
             simulation results
         """
         print(f"Simulating model: {self.engine.getDiagram().getName()}.")
         self.engine.setCompletionTime(tend)
         self.engine.setTimeIncrement(tend / numpoints)
-        return self.engine.simulateSimple(self.model) 
+        return Result(self.engine.simulateSimple(self.model), self.engine) 
+    
+class Result:
+    
+    def __init__(self, sr, engine):
+        self.sr = sr
+        self.engine = engine
+        species = engine.getFloatingSpecies()
+        self.values = numpy.array(sr.getValuesTransposed(species))
+        self.names = numpy.array(species)
+        self.times = numpy.array(sr.getTimes());
+        
+    def toFile(self, file):
+        jpype.JClass("biouml.standard.simulation.SimulationResultUtils").write(self.sr, self.names, file)
+    
+    def __str__(self):
+        return str(self.values)
+    
+    def getTimes(self):
+        return self.times
+    
+    def getNames(self):
+        return self.names
+        
+    def getValues(self, variable=None):
+        if (variable!=None):
+            return numpy.array(self.sr.getValues(variable))
+        else:
+            return self.values
```

