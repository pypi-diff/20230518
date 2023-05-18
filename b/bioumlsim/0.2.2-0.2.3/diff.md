# Comparing `tmp/bioumlsim-0.2.2.tar.gz` & `tmp/bioumlsim-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.2.2.tar", last modified: Thu May 18 18:26:43 2023, max compression
+gzip compressed data, was "bioumlsim-0.2.3.tar", last modified: Thu May 18 18:58:02 2023, max compression
```

## Comparing `bioumlsim-0.2.2.tar` & `bioumlsim-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 18:26:43.011386 bioumlsim-0.2.2/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      771 2023-05-18 18:26:43.012387 bioumlsim-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.2.2/README.md
--rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      798 2023-05-18 18:26:43.015393 bioumlsim-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 18:26:42.987387 bioumlsim-0.2.2/src/
--rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.2.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 18:26:43.010391 bioumlsim-0.2.2/src/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-05-18 18:26:42.000000 bioumlsim-0.2.2/src/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-18 18:26:42.000000 bioumlsim-0.2.2/src/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 18:26:42.000000 bioumlsim-0.2.2/src/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.2.2/src/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-18 18:26:42.000000 bioumlsim-0.2.2/src/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-18 18:26:42.000000 bioumlsim-0.2.2/src/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3245 2023-05-18 18:26:09.000000 bioumlsim-0.2.2/src/bioumlsim.py
--rw-rw-rw-   0        0        0      330 2023-05-18 18:24:46.000000 bioumlsim-0.2.2/src/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:58:02.903016 bioumlsim-0.2.3/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-05-18 18:58:02.904016 bioumlsim-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.2.3/README.md
+-rw-rw-rw-   0        0        0      185 2023-05-17 10:21:02.000000 bioumlsim-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      798 2023-05-18 18:58:02.910015 bioumlsim-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 18:58:02.855019 bioumlsim-0.2.3/src/
+-rw-rw-rw-   0        0        0        0 2023-05-17 07:30:52.000000 bioumlsim-0.2.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:58:02.902015 bioumlsim-0.2.3/src/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 10:19:31.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-18 18:58:02.000000 bioumlsim-0.2.3/src/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3469 2023-05-18 18:55:37.000000 bioumlsim-0.2.3/src/bioumlsim.py
+-rw-rw-rw-   0        0        0      388 2023-05-18 18:51:14.000000 bioumlsim-0.2.3/src/test.py
```

### Comparing `bioumlsim-0.2.2/LICENSE` & `bioumlsim-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.2.2/PKG-INFO` & `bioumlsim-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.2.2/setup.cfg` & `bioumlsim-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696f 756d 6c73 696d 0d0a 7665   = bioumlsim..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 320d 0a61  rsion = 0.2.2..a
+00000020: 7273 696f 6e20 3d20 302e 322e 330d 0a61  rsion = 0.2.3..a
 00000030: 7574 686f 7220 3d20 496c 7961 204b 6973  uthor = Ilya Kis
 00000040: 656c 6576 2c20 4269 6f73 6f66 742e 7275  elev, Biosoft.ru
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2034 7833 6375 7430 7240 676d 6169 6c2e   4x3cut0r@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2050 7974 686f 6e20 696e 7465 7266   = Python interf
 00000090: 6163 6520 666f 7220 7369 6d75 6c61 7469  ace for simulati
```

### Comparing `bioumlsim-0.2.2/src/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.2.3/src/bioumlsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.2.2/src/bioumlsim.py` & `bioumlsim-0.2.3/src/bioumlsim.py`

 * *Files 26% similar despite different names*

```diff
@@ -72,16 +72,22 @@
         self.sr = sr
         self.engine = engine
         species = engine.getFloatingSpecies()
         self.values = numpy.array(sr.getValuesTransposed(species))
         self.names = numpy.array(species)
         self.times = numpy.array(sr.getTimes());
         
-    def toFile(self, file):
-        jpype.JClass("biouml.standard.simulation.SimulationResultUtils").write(self.sr, self.names, file)
+    def toFile(self, file, precision=3, separator ='\t'):
+        f = open(file, 'w')
+        f.write(numpy.array2string(self.names, separator=separator)[1:-1])
+        f.write('\n')
+        for row in self.values:
+            f.write(numpy.array2string(row, precision=precision, separator=separator)[1:-1])
+            f.write('\n')
+        f.close()
     
     def __str__(self):
         return str(self.values)
     
     def getTimes(self):
         return self.times
```

