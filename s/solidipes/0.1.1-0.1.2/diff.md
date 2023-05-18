# Comparing `tmp/solidipes-0.1.1.tar.gz` & `tmp/solidipes-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipes-0.1.1.tar", max compression
+gzip compressed data, was "solidipes-0.1.2.tar", max compression
```

## Comparing `solidipes-0.1.1.tar` & `solidipes-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0     1165 2023-04-26 11:46:24.627178 solidipes-0.1.1/README.md
--rw-r--r--   0        0        0     2126 2023-05-12 13:22:06.748835 solidipes-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      163 2023-05-12 13:22:06.748835 solidipes-0.1.1/solidipes/__init__.py
--rw-r--r--   0        0        0      505 2023-05-12 09:53:39.243433 solidipes-0.1.1/solidipes/config.py
--rw-r--r--   0        0        0      446 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/__init__.py
--rw-r--r--   0        0        0      559 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/binary.py
--rw-r--r--   0        0        0      384 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/code_snippet.py
--rw-r--r--   0        0        0     4220 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/data_container.py
--rw-r--r--   0        0        0     2419 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/file.py
--rw-r--r--   0        0        0      386 2023-04-26 08:42:13.550032 solidipes-0.1.1/solidipes/loaders/geof_mesh.py
--rw-r--r--   0        0        0      829 2023-04-28 15:23:01.795502 solidipes-0.1.1/solidipes/loaders/image.py
--rw-r--r--   0        0        0      337 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/meshio.py
--rw-r--r--   0        0        0    75141 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/mime_types.py
--rw-r--r--   0        0        0     6583 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/parse_inp.py
--rw-r--r--   0        0        0     5175 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/pyvista_mesh.py
--rw-r--r--   0        0        0     1660 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/table.py
--rw-r--r--   0        0        0      791 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/text.py
--rw-r--r--   0        0        0        0 2023-05-12 13:21:56.464581 solidipes-0.1.1/solidipes/reports/__init__.py
--rw-r--r--   0        0        0     2559 2023-04-26 09:27:37.848878 solidipes-0.1.1/solidipes/reports/curation.py
--rw-r--r--   0        0        0     6516 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/reports/jtcam.py
--rw-r--r--   0        0        0     8405 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/reports/jtcam_small_logo.png
--rw-r--r--   0        0        0    28449 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/reports/jupyter_logo.png
--rw-r--r--   0        0        0    29716 2023-05-08 14:15:43.996185 solidipes-0.1.1/solidipes/reports/web_report.py
--rw-r--r--   0        0        0     2529 2023-05-08 14:15:43.996185 solidipes-0.1.1/solidipes/scanners/scanner.py
--rw-r--r--   0        0        0        0 2023-05-12 13:21:56.464581 solidipes-0.1.1/solidipes/scripts/__init__.py
--rw-r--r--   0        0        0     2736 2023-05-04 13:43:57.392612 solidipes-0.1.1/solidipes/scripts/download.py
--rw-r--r--   0        0        0     1275 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/scripts/generate_report.py
--rw-r--r--   0        0        0     3145 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/scripts/init.py
--rw-r--r--   0        0        0      990 2023-05-12 09:53:39.243433 solidipes-0.1.1/solidipes/scripts/main.py
--rw-r--r--   0        0        0      817 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/scripts/quick_view.py
--rw-r--r--   0        0        0     8659 2023-05-04 13:43:57.396612 solidipes-0.1.1/solidipes/scripts/upload.py
--rw-r--r--   0        0        0     4858 2023-05-12 09:53:39.243433 solidipes-0.1.1/solidipes/utils.py
--rw-r--r--   0        0        0     1532 2023-04-28 10:53:18.883696 solidipes-0.1.1/solidipes/viewer_backends.py
--rw-r--r--   0        0        0      355 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/__init__.py
--rw-r--r--   0        0        0     1256 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/binary.py
--rw-r--r--   0        0        0      916 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/code_snippet.py
--rw-r--r--   0        0        0      830 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/image.py
--rw-r--r--   0        0        0     3819 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/pyvista_plotter.py
--rw-r--r--   0        0        0     3090 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/table.py
--rw-r--r--   0        0        0     1670 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/text.py
--rw-r--r--   0        0        0     2223 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/viewer.py
--rw-r--r--   0        0        0     7545 2023-05-04 13:43:57.396612 solidipes-0.1.1/solidipes/zenodo_utils.py
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 solidipes-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1165 2023-04-26 11:46:24.627178 solidipes-0.1.2/README.md
+-rw-r--r--   0        0        0     2106 2023-05-18 12:58:39.095447 solidipes-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-05-18 12:58:39.099447 solidipes-0.1.2/solidipes/__init__.py
+-rw-r--r--   0        0        0      505 2023-05-12 09:53:39.243433 solidipes-0.1.2/solidipes/config.py
+-rw-r--r--   0        0        0      484 2023-05-18 12:58:13.802829 solidipes-0.1.2/solidipes/loaders/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/binary.py
+-rw-r--r--   0        0        0      384 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/code_snippet.py
+-rw-r--r--   0        0        0     4220 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/data_container.py
+-rw-r--r--   0        0        0     2419 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/file.py
+-rw-r--r--   0        0        0      386 2023-04-26 08:42:13.550032 solidipes-0.1.2/solidipes/loaders/geof_mesh.py
+-rw-r--r--   0        0        0      940 2023-05-17 11:01:16.491974 solidipes-0.1.2/solidipes/loaders/image.py
+-rw-r--r--   0        0        0      337 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/meshio.py
+-rw-r--r--   0        0        0    75141 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/mime_types.py
+-rw-r--r--   0        0        0     6583 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/parse_inp.py
+-rw-r--r--   0        0        0     5175 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/pyvista_mesh.py
+-rw-r--r--   0        0        0     1660 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/table.py
+-rw-r--r--   0        0        0      791 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/loaders/text.py
+-rw-r--r--   0        0        0      378 2023-05-18 12:58:13.802829 solidipes-0.1.2/solidipes/loaders/video.py
+-rw-r--r--   0        0        0        0 2023-05-18 12:58:28.795196 solidipes-0.1.2/solidipes/reports/__init__.py
+-rw-r--r--   0        0        0     2559 2023-04-26 09:27:37.848878 solidipes-0.1.2/solidipes/reports/curation.py
+-rw-r--r--   0        0        0     6516 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/reports/jtcam.py
+-rw-r--r--   0        0        0     8405 2023-04-26 08:20:35.886224 solidipes-0.1.2/solidipes/reports/jtcam_small_logo.png
+-rw-r--r--   0        0        0    28449 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/reports/jupyter_logo.png
+-rw-r--r--   0        0        0    29716 2023-05-17 11:03:42.931594 solidipes-0.1.2/solidipes/reports/web_report.py
+-rw-r--r--   0        0        0     2529 2023-05-17 11:03:42.931594 solidipes-0.1.2/solidipes/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2023-05-18 12:58:28.795196 solidipes-0.1.2/solidipes/scripts/__init__.py
+-rw-r--r--   0        0        0     2736 2023-05-04 13:43:57.392612 solidipes-0.1.2/solidipes/scripts/download.py
+-rw-r--r--   0        0        0     1275 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/scripts/generate_report.py
+-rw-r--r--   0        0        0     3145 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/scripts/init.py
+-rw-r--r--   0        0        0      990 2023-05-12 09:53:39.243433 solidipes-0.1.2/solidipes/scripts/main.py
+-rw-r--r--   0        0        0      817 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/scripts/quick_view.py
+-rw-r--r--   0        0        0     8659 2023-05-04 13:43:57.396612 solidipes-0.1.2/solidipes/scripts/upload.py
+-rw-r--r--   0        0        0     4910 2023-05-18 12:58:13.802829 solidipes-0.1.2/solidipes/utils.py
+-rw-r--r--   0        0        0     1532 2023-04-28 10:53:18.883696 solidipes-0.1.2/solidipes/viewer_backends.py
+-rw-r--r--   0        0        0      393 2023-05-18 12:58:13.802829 solidipes-0.1.2/solidipes/viewers/__init__.py
+-rw-r--r--   0        0        0     1256 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/viewers/binary.py
+-rw-r--r--   0        0        0      916 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/viewers/code_snippet.py
+-rw-r--r--   0        0        0     1230 2023-05-17 11:01:16.495975 solidipes-0.1.2/solidipes/viewers/image.py
+-rw-r--r--   0        0        0     3819 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/viewers/pyvista_plotter.py
+-rw-r--r--   0        0        0     3090 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/viewers/table.py
+-rw-r--r--   0        0        0     1670 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/viewers/text.py
+-rw-r--r--   0        0        0      830 2023-05-18 12:58:13.802829 solidipes-0.1.2/solidipes/viewers/video.py
+-rw-r--r--   0        0        0     2223 2023-04-26 08:20:35.890224 solidipes-0.1.2/solidipes/viewers/viewer.py
+-rw-r--r--   0        0        0     7545 2023-05-04 13:43:57.396612 solidipes-0.1.2/solidipes/zenodo_utils.py
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 solidipes-0.1.2/PKG-INFO
```

### Comparing `solidipes-0.1.1/README.md` & `solidipes-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/pyproject.toml` & `solidipes-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solidipes"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python package for the DCSM project"
 authors = [
 	"Son Pham-Ba <son.phamba@epfl.ch>",
 	"Guillaume Anciaux <guillaume.anciaux@epfl.ch>"
 ]
 license = ""
 readme = "README.md"
@@ -35,16 +35,15 @@
 streamlit-option-menu = "^0.3.2"
 requests-toolbelt = "^0.10.1"
 argcomplete = "^3.0.5"
 streamlit-ace = "^0.1.1"
 markdown = "^3.4.3"
 python-gitlab = "^3.14.0"
 matplotlib = ">=3.7.1"
-svglib = "^1.5.1"
-reportlab = "^3.6.13"
+cairosvg = "^2.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.4"
 build = "^0.10.0"
 pytest = "^7.2.1"
 jupyter = "^1.0.0"
 jupyterlab = "^3.6.1"
```

### Comparing `solidipes-0.1.1/solidipes/loaders/binary.py` & `solidipes-0.1.2/solidipes/loaders/binary.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/loaders/data_container.py` & `solidipes-0.1.2/solidipes/loaders/data_container.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/loaders/file.py` & `solidipes-0.1.2/solidipes/loaders/file.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/loaders/mime_types.py` & `solidipes-0.1.2/solidipes/loaders/mime_types.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/loaders/parse_inp.py` & `solidipes-0.1.2/solidipes/loaders/parse_inp.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/loaders/pyvista_mesh.py` & `solidipes-0.1.2/solidipes/loaders/pyvista_mesh.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/loaders/table.py` & `solidipes-0.1.2/solidipes/loaders/table.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/loaders/text.py` & `solidipes-0.1.2/solidipes/loaders/text.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/reports/curation.py` & `solidipes-0.1.2/solidipes/reports/curation.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/reports/jtcam.py` & `solidipes-0.1.2/solidipes/reports/jtcam.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/reports/jtcam_small_logo.png` & `solidipes-0.1.2/solidipes/reports/jtcam_small_logo.png`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/reports/jupyter_logo.png` & `solidipes-0.1.2/solidipes/reports/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/reports/web_report.py` & `solidipes-0.1.2/solidipes/reports/web_report.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/scanners/scanner.py` & `solidipes-0.1.2/solidipes/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/scripts/download.py` & `solidipes-0.1.2/solidipes/scripts/download.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/scripts/generate_report.py` & `solidipes-0.1.2/solidipes/scripts/generate_report.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/scripts/init.py` & `solidipes-0.1.2/solidipes/scripts/init.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/scripts/main.py` & `solidipes-0.1.2/solidipes/scripts/main.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/scripts/quick_view.py` & `solidipes-0.1.2/solidipes/scripts/quick_view.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/scripts/upload.py` & `solidipes-0.1.2/solidipes/scripts/upload.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/utils.py` & `solidipes-0.1.2/solidipes/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,26 @@
     from .loaders.binary import Binary
     from .loaders.code_snippet import CodeSnippet
     from .loaders.geof_mesh import GeofMesh
     from .loaders.image import Image
     from .loaders.pyvista_mesh import PyvistaMesh
     from .loaders.table import Table
     from .loaders.text import Markdown, Text
+    from .loaders.video import Video
 
     # Note: the first matching type is used
     loader_list = [
         Table,
         PyvistaMesh,
         Image,
         Markdown,
         Text,
         CodeSnippet,
         GeofMesh,
+        Video,
     ]
 
     if not os.path.isfile(path):
         raise FileNotFoundError(f'File "{path}" does not exist')
 
     for loader in loader_list:
         if loader.check_file_support(path):
```

### Comparing `solidipes-0.1.1/solidipes/viewer_backends.py` & `solidipes-0.1.2/solidipes/viewer_backends.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/viewers/binary.py` & `solidipes-0.1.2/solidipes/viewers/binary.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/viewers/code_snippet.py` & `solidipes-0.1.2/solidipes/viewers/code_snippet.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/viewers/image.py` & `solidipes-0.1.2/solidipes/viewers/video.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import streamlit as st
 from IPython.display import display
 
 from .. import loaders, viewer_backends
 from .viewer import Viewer
 
 
-class Image(Viewer):
-    """Viewer for images"""
+class Video(Viewer):
+    """Viewer for videos"""
 
     def __init__(self, data=None):
-        self.compatible_data_types = [loaders.Image]
+        self.compatible_data_types = [loaders.Video]
         #: Image to display
-        self.image = None
+        self.video = None
         super().__init__(data)
 
     def add(self, data_container):
         """Replace the viewer's image"""
         self.check_data_compatibility(data_container)
-        self.image = data_container.image
+        self.video = data_container.video
 
     def show(self):
         if viewer_backends.current_backend == "jupyter notebook":
             display(self.image)
 
         elif viewer_backends.current_backend == "streamlit":
             with st.container():
-                st.image(self.image)
+                st.video(self.video)
         else:  # python
             self.image.show()
```

### Comparing `solidipes-0.1.1/solidipes/viewers/pyvista_plotter.py` & `solidipes-0.1.2/solidipes/viewers/pyvista_plotter.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/viewers/table.py` & `solidipes-0.1.2/solidipes/viewers/table.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/viewers/text.py` & `solidipes-0.1.2/solidipes/viewers/text.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/viewers/viewer.py` & `solidipes-0.1.2/solidipes/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/solidipes/zenodo_utils.py` & `solidipes-0.1.2/solidipes/zenodo_utils.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.1/PKG-INFO` & `solidipes-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: solidipes
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for the DCSM project
 Home-page: https://gitlab.com/groups/dcsm
 Author: Son Pham-Ba
 Author-email: son.phamba@epfl.ch
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argcomplete (>=3.0.5,<4.0.0)
+Requires-Dist: cairosvg (>=2.7.0,<3.0.0)
 Requires-Dist: datasize (>=1.0.0,<2.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: ipydatawidgets (==4.3.2)
 Requires-Dist: markdown (>=3.4.3,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: meshio[all] (>=5.3.4,<6.0.0)
 Requires-Dist: openpyxl (>=3.1.1,<4.0.0)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: python-gitlab (>=3.14.0,<4.0.0)
 Requires-Dist: pyvista (>=0.38.1,<0.39.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: reportlab (>=3.6.13,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
 Requires-Dist: scipy (>=1.10.1)
 Requires-Dist: stpyvista (>=0.0.6,<0.0.7)
 Requires-Dist: streamlit (>=1.17.0,<2.0.0)
 Requires-Dist: streamlit-ace (>=0.1.1,<0.2.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-option-menu (>=0.3.2,<0.4.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
-Requires-Dist: svglib (>=1.5.1,<2.0.0)
 Requires-Dist: sympy (>=1.11.1)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: trame (>=2.2.6,<3.0.0)
 Project-URL: Documentation, https://solidipes.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.com/dcsm/solidipes
 Description-Content-Type: text/markdown
```

