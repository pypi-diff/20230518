# Comparing `tmp/mat_enm-0.0.2.tar.gz` & `tmp/mat_enm-0.0.3.tar.gz`

## Comparing `mat_enm-0.0.2.tar` & `mat_enm-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mat_enm-0.0.2/calc.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mat_enm-0.0.2/consts/__init__.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mat_enm-0.0.2/LICENSE
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mat_enm-0.0.2/README.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 mat_enm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 mat_enm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mat_enm-0.0.3/calc.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mat_enm-0.0.3/consts/__init__.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mat_enm-0.0.3/LICENSE
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mat_enm-0.0.3/README.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 mat_enm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 mat_enm-0.0.3/PKG-INFO
```

### Comparing `mat_enm-0.0.2/LICENSE` & `mat_enm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.2/pyproject.toml` & `mat_enm-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "mat-enm"
-version = "0.0.2"
+name = "mat_enm"
+version = "0.0.3"
 authors = [
     { name="lucas", email="lucas.larroque@iquall.net" },
 ]
 description = "Paquete para el manejo de enm por medio de mat"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `mat_enm-0.0.2/PKG-INFO` & `mat_enm-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mat-enm
-Version: 0.0.2
+Name: mat_enm
+Version: 0.0.3
 Summary: Paquete para el manejo de enm por medio de mat
 Project-URL: Homepage, https://gitlab.com/lucas.larroque/mat-enm
 Project-URL: Bug Tracker, https://gitlab.com/lucas.larroque/mat-enm/issues
 Author-email: lucas <lucas.larroque@iquall.net>
 License: MIT License
         
         Copyright (c) 2023 lucas larroque
```

