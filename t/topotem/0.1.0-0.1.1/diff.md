# Comparing `tmp/topotem-0.1.0.tar.gz` & `tmp/topotem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topotem-0.1.0.tar", max compression
+gzip compressed data, was "topotem-0.1.1.tar", max compression
```

## Comparing `topotem-0.1.0.tar` & `topotem-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1091 2023-05-17 21:45:29.232665 topotem-0.1.0/LICENSE
--rw-r--r--   0        0        0      499 2023-05-18 10:34:19.470329 topotem-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      187 2023-05-17 15:14:46.665553 topotem-0.1.0/README.md
--rw-r--r--   0        0        0      731 2023-05-04 10:32:50.956746 topotem-0.1.0/topotem/__init__.py
--rw-r--r--   0        0        0    18068 2023-05-17 16:05:42.597293 topotem-0.1.0/topotem/dummy_data.py
--rw-r--r--   0        0        0     5018 2023-05-17 15:53:58.625584 topotem-0.1.0/topotem/fft_mapping.py
--rw-r--r--   0        0        0     7434 2023-05-04 10:32:50.957746 topotem-0.1.0/topotem/lattice_structure_tools.py
--rw-r--r--   0        0        0    90403 2023-05-17 17:07:22.372575 topotem-0.1.0/topotem/polarisation.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 topotem-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-05-18 12:26:26.424114 topotem-0.1.1/LICENSE
+-rw-r--r--   0        0        0      540 2023-05-18 13:22:19.373339 topotem-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-05-18 12:26:26.428278 topotem-0.1.1/README.md
+-rw-r--r--   0        0        0      733 2023-05-18 13:17:48.219614 topotem-0.1.1/topotem/__init__.py
+-rw-r--r--   0        0        0    18068 2023-05-18 12:26:26.570324 topotem-0.1.1/topotem/dummy_data.py
+-rw-r--r--   0        0        0     5018 2023-05-18 12:26:26.570324 topotem-0.1.1/topotem/fft_mapping.py
+-rw-r--r--   0        0        0     7434 2023-05-18 12:26:26.579244 topotem-0.1.1/topotem/lattice_structure_tools.py
+-rw-r--r--   0        0        0    90403 2023-05-18 12:26:26.580239 topotem-0.1.1/topotem/polarisation.py
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 topotem-0.1.1/PKG-INFO
```

### Comparing `topotem-0.1.0/LICENSE` & `topotem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `topotem-0.1.0/topotem/__init__.py` & `topotem-0.1.1/topotem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     find_polarisation_vectors, correct_off_tilt_vectors,
     plot_polarisation_vectors, atom_deviation_from_straight_line_fit,
     get_divide_into, get_average_polarisation_in_regions,
     get_average_polarisation_in_regions_square,
     get_strain_map, rotation_of_atom_planes, ratio_of_lattice_spacings,
     get_angles_from_uv, get_vector_magnitudes,
     plot_atom_deviation_from_all_zone_axes,
-    get_polar_2d_colorwheel_color_list,
+    # get_polar_2d_colorwheel_color_list,
     combine_atom_deviations_from_zone_axes)
 
 from .lattice_structure_tools import (
     calculate_atom_plane_curvature,
 )
```

### Comparing `topotem-0.1.0/topotem/dummy_data.py` & `topotem-0.1.1/topotem/dummy_data.py`

 * *Files identical despite different names*

### Comparing `topotem-0.1.0/topotem/fft_mapping.py` & `topotem-0.1.1/topotem/fft_mapping.py`

 * *Files identical despite different names*

### Comparing `topotem-0.1.0/topotem/lattice_structure_tools.py` & `topotem-0.1.1/topotem/lattice_structure_tools.py`

 * *Files identical despite different names*

### Comparing `topotem-0.1.0/topotem/polarisation.py` & `topotem-0.1.1/topotem/polarisation.py`

 * *Files identical despite different names*

### Comparing `topotem-0.1.0/PKG-INFO` & `topotem-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: topotem
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: GeriTopore
 Author-email: g.topore22@imperial.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: atomap (>=0.3.3,<0.4.0)
+Requires-Dist: chardet (>=5.1.0,<6.0.0)
+Requires-Dist: colorcet (>=3.0.1,<4.0.0)
 Requires-Dist: hyperspy (>=1.7.5,<2.0.0)
 Requires-Dist: matplotlib-scalebar (>=0.8.1,<0.9.0)
 Description-Content-Type: text/markdown
 
 # TopoTEM
 TopoTEM is a Python tool for analysing, quantifying and visualising atomic displacements and polarisation in atomic-resolution Scanning Transmission Microscopy (STEM) images.
```

