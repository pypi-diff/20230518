# Comparing `tmp/mat_enm-0.0.8.tar.gz` & `tmp/mat_enm-0.0.9.tar.gz`

## Comparing `mat_enm-0.0.8.tar` & `mat_enm-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.8/src/mat_enm/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mat_enm-0.0.8/src/mat_enm/calc.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mat_enm-0.0.8/src/mat_enm/consts/__init__.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mat_enm-0.0.8/LICENSE
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mat_enm-0.0.8/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 mat_enm-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 mat_enm-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mat_enm-0.0.9/src/mat_enm/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mat_enm-0.0.9/src/mat_enm/calc.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mat_enm-0.0.9/src/mat_enm/consts/__init__.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mat_enm-0.0.9/LICENSE
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mat_enm-0.0.9/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 mat_enm-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 mat_enm-0.0.9/PKG-INFO
```

### Comparing `mat_enm-0.0.8/LICENSE` & `mat_enm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.8/pyproject.toml` & `mat_enm-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mat_enm"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name="lucas", email="lucas.larroque@iquall.net" },
 ]
 description = "Paquete para el manejo de enm por medio de mat"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `mat_enm-0.0.8/PKG-INFO` & `mat_enm-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat_enm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Paquete para el manejo de enm por medio de mat
 Project-URL: Homepage, https://gitlab.com/lucas.larroque/mat-enm
 Project-URL: Bug Tracker, https://gitlab.com/lucas.larroque/mat-enm/-/issues
 Author-email: lucas <lucas.larroque@iquall.net>
 License: MIT License
         
         Copyright (c) 2023 lucas larroque
```

