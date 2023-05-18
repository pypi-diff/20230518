# Comparing `tmp/mat_enm-0.0.4.tar.gz` & `tmp/mat_enm-0.0.5.tar.gz`

## Comparing `mat_enm-0.0.4.tar` & `mat_enm-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mat_enm-0.0.4/mat_enm.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mat_enm-0.0.4/consts/__init__.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mat_enm-0.0.4/LICENSE
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mat_enm-0.0.4/README.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 mat_enm-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 mat_enm-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mat_enm-0.0.5/mat_enm.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 mat_enm-0.0.5/consts/__init__.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mat_enm-0.0.5/LICENSE
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mat_enm-0.0.5/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 mat_enm-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 mat_enm-0.0.5/PKG-INFO
```

### Comparing `mat_enm-0.0.4/LICENSE` & `mat_enm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_enm-0.0.4/pyproject.toml` & `mat_enm-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mat_enm"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="lucas", email="lucas.larroque@iquall.net" },
 ]
 description = "Paquete para el manejo de enm por medio de mat"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
@@ -16,8 +16,8 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/lucas.larroque/mat-enm"
-"Bug Tracker" = "https://gitlab.com/lucas.larroque/mat-enm/issues"
+"Bug Tracker" = "https://gitlab.com/lucas.larroque/mat-enm/-/issues"
```

### Comparing `mat_enm-0.0.4/PKG-INFO` & `mat_enm-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mat_enm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Paquete para el manejo de enm por medio de mat
 Project-URL: Homepage, https://gitlab.com/lucas.larroque/mat-enm
-Project-URL: Bug Tracker, https://gitlab.com/lucas.larroque/mat-enm/issues
+Project-URL: Bug Tracker, https://gitlab.com/lucas.larroque/mat-enm/-/issues
 Author-email: lucas <lucas.larroque@iquall.net>
 License: MIT License
         
         Copyright (c) 2023 lucas larroque
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

