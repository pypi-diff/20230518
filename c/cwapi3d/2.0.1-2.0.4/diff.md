# Comparing `tmp/cwapi3d-2.0.1.tar.gz` & `tmp/cwapi3d-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwapi3d-2.0.1.tar", last modified: Tue May 16 15:47:06 2023, max compression
+gzip compressed data, was "cwapi3d-2.0.4.tar", last modified: Thu May 18 14:18:54 2023, max compression
```

## Comparing `cwapi3d-2.0.1.tar` & `cwapi3d-2.0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.831681 cwapi3d-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/attribute_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/attribute_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/bim_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/bim_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/cadwork/
--rw-r--r--   0 runner    (1001) docker     (123)    86279 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/cadwork/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/connector_axis_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/connector_axis_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/cwapi3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-16 15:47:06.000000 cwapi3d-2.0.1/src/cwapi3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-16 15:47:06.000000 cwapi3d-2.0.1/src/cwapi3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:47:06.000000 cwapi3d-2.0.1/src/cwapi3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 15:47:06.000000 cwapi3d-2.0.1/src/cwapi3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/element_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    33675 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/element_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/endtype_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/endtype_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/file_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/file_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/geometry_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/geometry_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/list_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/list_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/machine_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/machine_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/material_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/material_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/menu_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/menu_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/roof_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/roof_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/scene_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/scene_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/shop_drawing_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/shop_drawing_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/utility_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/utility_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/visualization_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/visualization_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/attribute_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/attribute_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/bim_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/bim_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/cadwork/
+-rw-r--r--   0 runner    (1001) docker     (123)    86279 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/cadwork/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/connector_axis_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/connector_axis_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/cwapi3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-18 14:18:53.000000 cwapi3d-2.0.4/src/cwapi3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-18 14:18:53.000000 cwapi3d-2.0.4/src/cwapi3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:18:53.000000 cwapi3d-2.0.4/src/cwapi3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-18 14:18:53.000000 cwapi3d-2.0.4/src/cwapi3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/element_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    33675 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/element_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/endtype_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/endtype_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/file_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/file_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/geometry_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/geometry_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/list_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/list_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/machine_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/machine_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/material_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/material_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/menu_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/menu_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/roof_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/roof_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/scene_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/scene_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/shop_drawing_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/shop_drawing_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/utility_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/utility_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/visualization_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/visualization_controller/__init__.pyi
```

### Comparing `cwapi3d-2.0.1/LICENSE` & `cwapi3d-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/PKG-INFO` & `cwapi3d-2.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 2.0.1
+Version: 2.0.4
 Summary: Python bindings for CwAPI3D
 Home-page: https://github.com/cwapi3d/cwapi3dpython
 Author: Cadwork
 Author-email: it@cadwork.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `cwapi3d-2.0.1/README.md` & `cwapi3d-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/setup.py` & `cwapi3d-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='cwapi3d',
-    version='2.0.1',
+    version='2.0.4',
     author='Cadwork',
     author_email='it@cadwork.ca',
     description='Python bindings for CwAPI3D',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cwapi3d/cwapi3dpython',
     classifiers=[
```

### Comparing `cwapi3d-2.0.1/src/attribute_controller/__init__.pyi` & `cwapi3d-2.0.4/src/attribute_controller/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -570,28 +570,29 @@
 
     [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
-        bool: element material name
+        str: element material name
     """
 
 
 def get_prefab_layer(element: int) -> str:
     """Gets the element prefab layer
 
     [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
-        bool: element prefab layer
+        str: element prefab layer
+
     """
 
 
 def get_machine_calculation_set(element: int) -> str:
     """Gets the element machine calculation set
 
     [:information_source: Available for script filled attributes](#){.mark-text}
```

### Comparing `cwapi3d-2.0.1/src/bim_controller/__init__.pyi` & `cwapi3d-2.0.4/src/bim_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/cadwork/__init__.pyi` & `cwapi3d-2.0.4/src/cadwork/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/connector_axis_controller/__init__.pyi` & `cwapi3d-2.0.4/src/connector_axis_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/cwapi3d.egg-info/PKG-INFO` & `cwapi3d-2.0.4/src/cwapi3d.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 2.0.1
+Version: 2.0.4
 Summary: Python bindings for CwAPI3D
 Home-page: https://github.com/cwapi3d/cwapi3dpython
 Author: Cadwork
 Author-email: it@cadwork.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `cwapi3d-2.0.1/src/cwapi3d.egg-info/SOURCES.txt` & `cwapi3d-2.0.4/src/cwapi3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/element_controller/__init__.pyi` & `cwapi3d-2.0.4/src/element_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/endtype_controller/__init__.pyi` & `cwapi3d-2.0.4/src/endtype_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/file_controller/__init__.pyi` & `cwapi3d-2.0.4/src/file_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/geometry_controller/__init__.pyi` & `cwapi3d-2.0.4/src/geometry_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/list_controller/__init__.pyi` & `cwapi3d-2.0.4/src/list_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/machine_controller/__init__.pyi` & `cwapi3d-2.0.4/src/machine_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/material_controller/__init__.pyi` & `cwapi3d-2.0.4/src/material_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/scene_controller/__init__.pyi` & `cwapi3d-2.0.4/src/scene_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/shop_drawing_controller/__init__.pyi` & `cwapi3d-2.0.4/src/shop_drawing_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/utility_controller/__init__.pyi` & `cwapi3d-2.0.4/src/utility_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.1/src/visualization_controller/__init__.pyi` & `cwapi3d-2.0.4/src/visualization_controller/__init__.pyi`

 * *Files identical despite different names*

