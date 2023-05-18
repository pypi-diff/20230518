# Comparing `tmp/openmc_plot-0.2.2.tar.gz` & `tmp/openmc_plot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmc_plot-0.2.2.tar", last modified: Wed Feb 22 19:53:27 2023, max compression
+gzip compressed data, was "openmc_plot-0.3.0.tar", last modified: Fri Feb 24 23:42:45 2023, max compression
```

## Comparing `openmc_plot-0.2.2.tar` & `openmc_plot-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.247342 openmc_plot-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-02-22 19:53:27.247342 openmc_plot-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/examples/dagmc_geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/dagmc_geometry/create_geometry_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/examples/default_source/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/default_source/settings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/examples/pincell/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/pincell/geometry.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/examples/regularmesh_plot/
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/regularmesh_plot/create_statepoint_with_regularmesh_tally.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/examples/ring_source/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/ring_source/make_ring_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/ring_source/make_two_ring_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/ring_source/settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/ring_source/settings_multiple_sources.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/examples/tokamak/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/create_geometry_xml_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/geometry_no_materials.xml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/geometry_some_materials.xml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/geometry_unordered_mat_ids.xml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/materials.xml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/settings_multiple_sources.xml
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/tokamak/summary.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/examples/weightwindows/
--rw-r--r--   0 runner    (1001) docker     (123)  1411929 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/examples/weightwindows/settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 19:53:27.247342 openmc_plot-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.243342 openmc_plot-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.247342 openmc_plot-0.2.2/src/openmc_plot/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-22 19:53:27.000000 openmc_plot-0.2.2/src/openmc_plot/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/cross_sections.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/dagmcslice_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/geometry_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/header.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/regularmesh_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/source_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-02-22 19:53:11.000000 openmc_plot-0.2.2/src/openmc_plot/weightwindows_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:53:27.247342 openmc_plot-0.2.2/src/openmc_plot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-02-22 19:53:27.000000 openmc_plot-0.2.2/src/openmc_plot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-22 19:53:27.000000 openmc_plot-0.2.2/src/openmc_plot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 19:53:27.000000 openmc_plot-0.2.2/src/openmc_plot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-22 19:53:27.000000 openmc_plot-0.2.2/src/openmc_plot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-22 19:53:27.000000 openmc_plot-0.2.2/src/openmc_plot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 19:53:27.000000 openmc_plot-0.2.2/src/openmc_plot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.904693 openmc_plot-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-02-24 23:42:45.904693 openmc_plot-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/examples/dagmc_geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/dagmc_geometry/create_geometry_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/examples/default_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/default_source/settings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/examples/pincell/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/pincell/geometry.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/examples/regularmesh_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/regularmesh_plot/create_statepoint_with_regularmesh_tally.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.896692 openmc_plot-0.3.0/examples/ring_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/ring_source/make_ring_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/ring_source/make_two_ring_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/ring_source/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/ring_source/settings_multiple_sources.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.896692 openmc_plot-0.3.0/examples/tokamak/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/create_geometry_xml_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/geometry_no_materials.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/geometry_some_materials.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/geometry_unordered_mat_ids.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/materials.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/settings_multiple_sources.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/tokamak/summary.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.896692 openmc_plot-0.3.0/examples/weightwindows/
+-rw-r--r--   0 runner    (1001) docker     (123)  1411929 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/examples/weightwindows/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 23:42:45.904693 openmc_plot-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.892692 openmc_plot-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.896692 openmc_plot-0.3.0/src/openmc_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-24 23:42:45.000000 openmc_plot-0.3.0/src/openmc_plot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/cross_sections.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.900692 openmc_plot-0.3.0/src/openmc_plot/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/pages/1_🖼_Geometry_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/pages/2_🧊_Regular_mesh_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/pages/3_✴️_Source_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/pages/4_🪟_Weight_window_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/pages/5_🍕_DAGMC_slice_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4077544 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/pages/dagmc.h5m
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-24 23:42:30.000000 openmc_plot-0.3.0/src/openmc_plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 23:42:45.900692 openmc_plot-0.3.0/src/openmc_plot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-02-24 23:42:45.000000 openmc_plot-0.3.0/src/openmc_plot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-02-24 23:42:45.000000 openmc_plot-0.3.0/src/openmc_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 23:42:45.000000 openmc_plot-0.3.0/src/openmc_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-24 23:42:45.000000 openmc_plot-0.3.0/src/openmc_plot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-24 23:42:45.000000 openmc_plot-0.3.0/src/openmc_plot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-24 23:42:45.000000 openmc_plot-0.3.0/src/openmc_plot.egg-info/top_level.txt
```

### Comparing `openmc_plot-0.2.2/.github/workflows/python-publish.yml` & `openmc_plot-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/.gitignore` & `openmc_plot-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/LICENSE` & `openmc_plot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/PKG-INFO` & `openmc_plot-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_plot
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Python package containing a collection of scripts for producing and downloading data for OpenMC
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2022 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,17 +32,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
-A Python app for plotting OpenMC geometry.
+A Python app for plotting OpenMC.
 
-This repository contains part of the source code for the OpenMC geometry plotting app which is part of the website [xsplot.com](http://xsplot.com)
+This repository contains the source code for the OpenMC plot.
+
+Try the web app at [http://openmc-plot.xsplot.com](http://openmc-plot.xsplot.com)
 
 This repository contains:
 - A Python [Streamlit](https://streamlit.io) based GUI 🐍
 - A Dockerfile that provides the hosting environment for the web app 🐳
 
 # Plot geometry
 ![openmc plot geometry](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/d/d7bcce794d51d34381371fc991c0e1ff2a65df08.gif)
@@ -54,15 +56,17 @@
 ![openmc plot mesh](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/2/24a9db7bc9cc227908dbaf13a54d1245a4d16f20.gif)
 
 # Plot weight windows
 ![openmc plot mesh](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/1/114aeb91172c7577e9231ffe30edf141678d26f6.gif)
 
 # Install
 
-OpenMC_plot can be install directly from the Python package index (PyPi) using pip.
+First you will need to [install OpenMC](https://docs.openmc.org/en/stable/quickinstall.html)
+
+OpenMC_plot can then be install directly from the Python package index (PyPi) using pip.
 
 ```
 pip install openmc_plot
 ```
 
 # Usage
 
@@ -74,16 +78,14 @@
 
 Your default web browser should then load with the GUI.
 
 You will also need to have [OpenMC installed](https://docs.openmc.org/en/stable/quickinstall.html).
 
 # Run web app locally (developers)
 
-You can view the hosted version of this repository here [xsplot.com](http://xsplot.com). However you might want to host your own version locally.
-
 To host your own local version of [xsplot.com](http://xsplot.com) you will need [Docker](https://www.docker.com/) installed and then can build and run the Dockerfile
 with the following commands.
 
 First clone the repository
 ```bash
 git clone https://github.com/fusion-energy/openmc_plot
 ```
```

### Comparing `openmc_plot-0.2.2/README.md` & `openmc_plot-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-A Python app for plotting OpenMC geometry.
+A Python app for plotting OpenMC.
 
-This repository contains part of the source code for the OpenMC geometry plotting app which is part of the website [xsplot.com](http://xsplot.com)
+This repository contains the source code for the OpenMC plot.
+
+Try the web app at [http://openmc-plot.xsplot.com](http://openmc-plot.xsplot.com)
 
 This repository contains:
 - A Python [Streamlit](https://streamlit.io) based GUI 🐍
 - A Dockerfile that provides the hosting environment for the web app 🐳
 
 # Plot geometry
 ![openmc plot geometry](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/d/d7bcce794d51d34381371fc991c0e1ff2a65df08.gif)
@@ -16,15 +18,17 @@
 ![openmc plot mesh](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/2/24a9db7bc9cc227908dbaf13a54d1245a4d16f20.gif)
 
 # Plot weight windows
 ![openmc plot mesh](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/1/114aeb91172c7577e9231ffe30edf141678d26f6.gif)
 
 # Install
 
-OpenMC_plot can be install directly from the Python package index (PyPi) using pip.
+First you will need to [install OpenMC](https://docs.openmc.org/en/stable/quickinstall.html)
+
+OpenMC_plot can then be install directly from the Python package index (PyPi) using pip.
 
 ```
 pip install openmc_plot
 ```
 
 # Usage
 
@@ -36,16 +40,14 @@
 
 Your default web browser should then load with the GUI.
 
 You will also need to have [OpenMC installed](https://docs.openmc.org/en/stable/quickinstall.html).
 
 # Run web app locally (developers)
 
-You can view the hosted version of this repository here [xsplot.com](http://xsplot.com). However you might want to host your own version locally.
-
 To host your own local version of [xsplot.com](http://xsplot.com) you will need [Docker](https://www.docker.com/) installed and then can build and run the Dockerfile
 with the following commands.
 
 First clone the repository
 ```bash
 git clone https://github.com/fusion-energy/openmc_plot
 ```
```

### Comparing `openmc_plot-0.2.2/examples/pincell/geometry.xml` & `openmc_plot-0.3.0/examples/pincell/geometry.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/regularmesh_plot/create_statepoint_with_regularmesh_tally.py` & `openmc_plot-0.3.0/examples/regularmesh_plot/create_statepoint_with_regularmesh_tally.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # dt_plasma_material = openmc.Material()
 # dt_plasma_material.set_density("g/cm3", 1e-7)
 # dt_plasma_material.add_nuclide("H2", 0.5)
 # dt_plasma_material.add_nuclide("H3", 0.5)
 
 mats = openmc.Materials(
-    [breeder_material, eurofer_material, copper_material]#, dt_plasma_material]
+    [breeder_material, eurofer_material, copper_material]  # , dt_plasma_material]
 )
 
 
 # GEOMETRY
 
 # surfaces
 central_sol_surface = openmc.ZCylinder(r=100)
@@ -38,15 +38,17 @@
 port_hole = openmc.Sphere(r=60, x0=500)
 upper_port_hole = openmc.Sphere(r=100, z0=500)
 vessel_inner_surface = openmc.Sphere(r=500)
 first_wall_outer_surface = openmc.Sphere(r=510)
 breeder_blanket_outer_surface = openmc.Sphere(r=610, boundary_type="vacuum")
 
 # cells
-central_sol_region = -central_sol_surface & -breeder_blanket_outer_surface & +upper_port_hole
+central_sol_region = (
+    -central_sol_surface & -breeder_blanket_outer_surface & +upper_port_hole
+)
 central_sol_cell = openmc.Cell(region=central_sol_region)
 central_sol_cell.fill = copper_material
 
 central_shield_region = (
     +central_sol_surface
     & -central_shield_outer_surface
     & -breeder_blanket_outer_surface
@@ -56,30 +58,35 @@
 central_shield_cell.fill = eurofer_material
 
 # plasma_cell_region = -plasma_surface
 # plasma_cell_cell = openmc.Cell(region=plasma_cell_region)
 # plasma_cell_cell.fill = dt_plasma_material
 
 inner_vessel_region = (
-    -vessel_inner_surface & +central_shield_outer_surface  & +port_hole & +upper_port_hole
-    #& +plasma_surface
+    -vessel_inner_surface
+    & +central_shield_outer_surface
+    & +port_hole
+    & +upper_port_hole
+    # & +plasma_surface
 )
 inner_vessel_cell = openmc.Cell(region=inner_vessel_region)
 # inner_vessel_cell.fill = eurofer_material
 # no material set as default is vacuum
 
 upper_port_hole_region = -upper_port_hole
 upper_port_hole_cell = openmc.Cell(region=upper_port_hole_region)
 
 port_hole_region = -port_hole
 port_hole_cell = openmc.Cell(region=port_hole_region)
 # port_hole_cell.fill = eurofer_material
 # no material set as default is vacuum
 
-first_wall_region = -first_wall_outer_surface & +vessel_inner_surface & +port_hole &+upper_port_hole
+first_wall_region = (
+    -first_wall_outer_surface & +vessel_inner_surface & +port_hole & +upper_port_hole
+)
 first_wall_cell = openmc.Cell(region=first_wall_region)
 first_wall_cell.fill = eurofer_material
 
 breeder_blanket_region = (
     +first_wall_outer_surface
     & -breeder_blanket_outer_surface
     & +central_shield_outer_surface
@@ -160,15 +167,15 @@
 mesh_tally_1 = openmc.Tally(name="heating_on_mesh")
 mesh_tally_1.filters = [mesh_filter]
 mesh_tally_1.scores = ["heating"]
 tallies.append(mesh_tally_1)
 
 model = openmc.model.Model(my_geometry, mats, sett, tallies)
 sp_filename = model.run()
-sp_filename = f'statepoint.{sett.batches}.h5'
+sp_filename = f"statepoint.{sett.batches}.h5"
 
 # loads up the output file from the simulation
 statepoint = openmc.StatePoint(sp_filename)
 
 # extracts the mesh tally by name
 my_tbr_tally = statepoint.get_tally(name="heating_on_mesh")
 
@@ -192,15 +199,15 @@
 bottom = mesh.lower_left[0]
 top = mesh.upper_right[0]
 extent = (left, right, bottom, top)
 slice_value = int(len(ffx) / 2)
 plt.imshow(X=ffx[slice_value], extent=extent)
 plt.show()
 
-ffy = ff2#.transpose(2, 1, 0)
+ffy = ff2  # .transpose(2, 1, 0)
 left = mesh.lower_left[1]
 right = mesh.upper_right[1]
 bottom = mesh.lower_left[1]
 top = mesh.upper_right[1]
 extent = (left, right, bottom, top)
 slice_value = int(len(ffy) / 2)
 plt.imshow(X=ffy[slice_value], extent=extent)
```

### Comparing `openmc_plot-0.2.2/examples/ring_source/make_ring_source.py` & `openmc_plot-0.3.0/examples/ring_source/make_ring_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 # the distribution of radius is just a single value
 radius = openmc.stats.Discrete([10], [1])
 
 # the distribution of source z values is just a single value
 z_values = openmc.stats.Discrete([0], [1])
 
 # the distribution of source azimuthal angles values is a uniform distribution between 0 and 2 Pi
-angle = openmc.stats.Uniform(a=0., b=2* 3.14159265359)
+angle = openmc.stats.Uniform(a=0.0, b=2 * 3.14159265359)
 
 # this makes the ring source using the three distributions and a radius
-my_source.space = openmc.stats.CylindricalIndependent(r=radius, phi=angle, z=z_values, origin=(0.0, 0.0, 0.0))
+my_source.space = openmc.stats.CylindricalIndependent(
+    r=radius, phi=angle, z=z_values, origin=(0.0, 0.0, 0.0)
+)
 
 # sets the direction to isotropic
 my_source.angle = openmc.stats.Isotropic()
 
 # sets the energy distribution to a Muir distribution neutrons
 my_source.energy = openmc.stats.Muir(e0=14080000.0, m_rat=5.0, kt=20000.0)
 
 my_settings = openmc.Settings()
 
 my_settings.source = my_source
 
-my_settings.export_to_xml()
+my_settings.export_to_xml()
```

### Comparing `openmc_plot-0.2.2/examples/ring_source/make_two_ring_source.py` & `openmc_plot-0.3.0/examples/ring_source/make_two_ring_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,46 +6,49 @@
 # the distribution of radius is just a single value
 radius = openmc.stats.Discrete([10], [1])
 
 # the distribution of source z values is just a single value
 z_values = openmc.stats.Discrete([0], [1])
 
 # the distribution of source azimuthal angles values is a uniform distribution between 0 and 2 Pi
-angle = openmc.stats.Uniform(a=0., b=2* 3.14159265359)
+angle = openmc.stats.Uniform(a=0.0, b=2 * 3.14159265359)
 
 # this makes the ring source using the three distributions and a radius
-my_source1.space = openmc.stats.CylindricalIndependent(r=radius, phi=angle, z=z_values, origin=(0.0, 0.0, 0.0))
+my_source1.space = openmc.stats.CylindricalIndependent(
+    r=radius, phi=angle, z=z_values, origin=(0.0, 0.0, 0.0)
+)
 
 # sets the direction to isotropic
 my_source1.angle = openmc.stats.Isotropic()
 
 # sets the energy distribution to a Muir distribution neutrons
 my_source1.energy = openmc.stats.Muir(e0=14080000.0, m_rat=5.0, kt=20000.0)
 
 
-
 # initialises a new source object
 my_source2 = openmc.Source()
 
 # the distribution of radius is just a single value
 radius = openmc.stats.Discrete([9], [1])
 
 # the distribution of source z values is just a single value
 z_values = openmc.stats.Discrete([0], [1])
 
 # the distribution of source azimuthal angles values is a uniform distribution between 0 and 2 Pi
-angle = openmc.stats.Uniform(a=0., b=2* 3.14159265359)
+angle = openmc.stats.Uniform(a=0.0, b=2 * 3.14159265359)
 
 # this makes the ring source using the three distributions and a radius
-my_source2.space = openmc.stats.CylindricalIndependent(r=radius, phi=angle, z=z_values, origin=(0.0, 0.0, 0.0))
+my_source2.space = openmc.stats.CylindricalIndependent(
+    r=radius, phi=angle, z=z_values, origin=(0.0, 0.0, 0.0)
+)
 
 # sets the direction to isotropic
 my_source2.angle = openmc.stats.Isotropic()
 
 # sets the energy distribution to a Muir distribution neutrons
 my_source2.energy = openmc.stats.Muir(e0=2000000.0, m_rat=4.0, kt=20000.0)
 
 my_settings = openmc.Settings()
 
 my_settings.source = [my_source1, my_source2]
 
-my_settings.export_to_xml('settings_multiple_sources.xml')
+my_settings.export_to_xml("settings_multiple_sources.xml")
```

### Comparing `openmc_plot-0.2.2/examples/ring_source/settings.xml` & `openmc_plot-0.3.0/examples/ring_source/settings.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/ring_source/settings_multiple_sources.xml` & `openmc_plot-0.3.0/examples/ring_source/settings_multiple_sources.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/tokamak/create_geometry_xml_files.py` & `openmc_plot-0.3.0/examples/tokamak/create_geometry_xml_files.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,80 @@
-
-
 import openmc
 import matplotlib.pyplot as plt
 
 # surfaces
-central_column_surface = openmc.ZCylinder(r=100) # note the new surface type
+central_column_surface = openmc.ZCylinder(r=100)  # note the new surface type
 inner_sphere_surface = openmc.Sphere(r=480)
-middle_sphere_surface = openmc.Sphere(r=500) 
-outer_sphere_surface = openmc.Sphere(r=600, boundary_type='vacuum')
+middle_sphere_surface = openmc.Sphere(r=500)
+outer_sphere_surface = openmc.Sphere(r=600, boundary_type="vacuum")
 
 # regions
 # the center column region is cut at the top and bottom using the -outer_sphere_surface
 central_column_region = -central_column_surface & -outer_sphere_surface
-firstwall_region = -middle_sphere_surface & +inner_sphere_surface & +central_column_surface
-blanket_region = +middle_sphere_surface & -outer_sphere_surface & +central_column_surface
+firstwall_region = (
+    -middle_sphere_surface & +inner_sphere_surface & +central_column_surface
+)
+blanket_region = (
+    +middle_sphere_surface & -outer_sphere_surface & +central_column_surface
+)
 inner_vessel_region = +central_column_surface & -inner_sphere_surface
 
 # cells
 firstwall_cell = openmc.Cell(region=firstwall_region)
 central_column_cell = openmc.Cell(region=central_column_region)
 blanket_cell = openmc.Cell(region=blanket_region)
 inner_vessel_cell = openmc.Cell(region=inner_vessel_region)
 
-universe = openmc.Universe(cells=[central_column_cell, firstwall_cell,
-                                  blanket_cell, inner_vessel_cell])
+universe = openmc.Universe(
+    cells=[central_column_cell, firstwall_cell, blanket_cell, inner_vessel_cell]
+)
 
 my_geometry = openmc.Geometry(universe)
 
-my_geometry.export_to_xml('geometry_no_materials.xml')
+my_geometry.export_to_xml("geometry_no_materials.xml")
 
 mat_1 = openmc.Material()
 mat_1.id = 1
-mat_1.add_element('Na', 1)
-mat_1.set_density('g/cm3', 1)
+mat_1.add_element("Na", 1)
+mat_1.set_density("g/cm3", 1)
 blanket_cell.fill = mat_1
 
-universe = openmc.Universe(cells=[central_column_cell, firstwall_cell,
-                                  blanket_cell, inner_vessel_cell])
+universe = openmc.Universe(
+    cells=[central_column_cell, firstwall_cell, blanket_cell, inner_vessel_cell]
+)
 
 my_geometry = openmc.Geometry(universe)
 
-my_geometry.export_to_xml('geometry_some_materials.xml')
+my_geometry.export_to_xml("geometry_some_materials.xml")
 
 
 mat_1 = openmc.Material()
 mat_1.id = 1
-mat_1.add_element('Na', 1)
-mat_1.set_density('g/cm3', 1)
+mat_1.add_element("Na", 1)
+mat_1.set_density("g/cm3", 1)
 central_column_cell.fill = mat_1
 
 mat_2 = openmc.Material()
 mat_2.id = 2
-mat_2.add_element('Na', 1)
-mat_2.set_density('g/cm3', 1)
+mat_2.add_element("Na", 1)
+mat_2.set_density("g/cm3", 1)
 firstwall_cell.fill = mat_2
 
 mat_3 = openmc.Material()
 mat_3.id = 4
-mat_3.add_element('Na', 1)
-mat_3.set_density('g/cm3', 1)
+mat_3.add_element("Na", 1)
+mat_3.set_density("g/cm3", 1)
 blanket_cell.fill = mat_3
 
 mat_4 = openmc.Material()
 mat_4.id = 9
-mat_4.add_element('Na', 1)
-mat_4.set_density('g/cm3', 1)
+mat_4.add_element("Na", 1)
+mat_4.set_density("g/cm3", 1)
 inner_vessel_cell.fill = mat_4
 
-universe = openmc.Universe(cells=[central_column_cell, firstwall_cell,
-                                  blanket_cell, inner_vessel_cell])
+universe = openmc.Universe(
+    cells=[central_column_cell, firstwall_cell, blanket_cell, inner_vessel_cell]
+)
 
 my_geometry = openmc.Geometry(universe)
 
-my_geometry.export_to_xml('geometry.xml')
+my_geometry.export_to_xml("geometry.xml")
```

### Comparing `openmc_plot-0.2.2/examples/tokamak/geometry.xml` & `openmc_plot-0.3.0/examples/tokamak/geometry.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/tokamak/geometry_no_materials.xml` & `openmc_plot-0.3.0/examples/tokamak/geometry_no_materials.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/tokamak/geometry_some_materials.xml` & `openmc_plot-0.3.0/examples/tokamak/geometry_some_materials.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/tokamak/geometry_unordered_mat_ids.xml` & `openmc_plot-0.3.0/examples/tokamak/geometry_unordered_mat_ids.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/tokamak/settings_multiple_sources.xml` & `openmc_plot-0.3.0/examples/tokamak/settings_multiple_sources.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/tokamak/summary.h5` & `openmc_plot-0.3.0/examples/tokamak/summary.h5`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/examples/weightwindows/settings.xml` & `openmc_plot-0.3.0/examples/weightwindows/settings.xml`

 * *Files identical despite different names*

### Comparing `openmc_plot-0.2.2/pyproject.toml` & `openmc_plot-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "streamlit",
     "openmc_source_plotter>=0.6.2",
     "dagmc_geometry_slice_plotter>=0.3.0",
     "openmc_geometry_plot>=0.3.3",
+    "regular_mesh_plotter>=0.5.3",
 ]
 dynamic = ["version"]
 
 
 [tool.setuptools_scm]
 write_to = "src/openmc_plot/_version.py"
```

### Comparing `openmc_plot-0.2.2/src/openmc_plot/geometry_tab.py` & `openmc_plot-0.3.0/src/openmc_plot/pages/1_🖼_Geometry_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,506 +9,501 @@
 import streamlit as st
 from matplotlib import colors
 from pylab import cm, colormaps
 
 from utils import save_uploadedfile
 
 
-def create_geometry_tab():
+st.write(
+    """
+        This tab makes use of the 🐍 Python package ```openmc_geometry_plot``` which is available on [GitHub](https://github.com/fusion-energy/openmc_geometry_plot).
+    """
+)
+file_label_col1, file_label_col2 = st.columns([1, 1])
+file_col1, file_col2 = st.columns([1, 1])
+file_col1.write(
+    """
+        👉 Create your ```openmc.Geometry()``` and export the geometry xml file using ```export_to_xml()```.
+    """
+)
+file_col2.write(
+    """
+        👉 Create your DAGMC h5m file using tools like [CAD-to-h5m](https://github.com/fusion-energy/cad_to_dagmc), [STL-to_h5m](https://github.com/fusion-energy/stl_to_h5m) [vertices-to-h5m](https://github.com/fusion-energy/vertices_to_h5m), [Brep-to-h5m](https://github.com/fusion-energy/brep_to_h5m) or the [Cubit](https://coreform.com/products/coreform-cubit/) [Plugin](https://github.com/svalinn/Cubit-plugin)
+    """
+)
+
+geometry_xml_file = file_col1.file_uploader(
+    "Upload your geometry.xml", type=["xml"]
+)
+dagmc_file = file_col2.file_uploader("Upload your DAGMC h5m", type=["h5m"])
+
+my_geometry = None
+
+if dagmc_file is None and geometry_xml_file is None:
+    new_title = '<center><p style="font-family:sans-serif; color:Red; font-size: 30px;">Upload your geometry.xml or DAGMC h5m file</p></center>'
+    st.markdown(new_title, unsafe_allow_html=True)
 
     st.write(
         """
-            This tab makes use of the 🐍 Python package ```openmc_geometry_plot``` which is available on [GitHub](https://github.com/fusion-energy/openmc_geometry_plot).
+            Not got a geometry.xml file handy, right mouse 🖱️ click and save these links 
+            [ example 1 ](https://fusion-energy.github.io/openmc_geometry_plot/examples/csg_tokamak/geometry.xml),
+            [ example 2 ](https://fusion-energy.github.io/openmc_geometry_plot/examples/csg_cylinder_box/geometry.xml)
         """
     )
-    file_label_col1, file_label_col2 = st.columns([1, 1])
-    file_col1, file_col2 = st.columns([1, 1])
-    file_col1.write(
-        """
-            👉 Create your ```openmc.Geometry()``` and export the geometry xml file using ```export_to_xml()```.
-        """
-    )
-    file_col2.write(
+    st.write(
         """
-            👉 Create your DAGMC h5m file using tools like [CAD-to-h5m](https://github.com/fusion-energy/cad_to_dagmc), [STL-to_h5m](https://github.com/fusion-energy/stl_to_h5m) [vertices-to-h5m](https://github.com/fusion-energy/vertices_to_h5m), [Brep-to-h5m](https://github.com/fusion-energy/brep_to_h5m) or the [Cubit](https://coreform.com/products/coreform-cubit/) [Plugin](https://github.com/svalinn/Cubit-plugin)
+            Not got a DAGMC h5m file handy, right mouse 🖱️ click and save these links 
+            [ example 1 ](https://fusion-energy.github.io/openmc_geometry_plot/examples/dagmc_tokamak/dagmc_180_tokamak.h5m)
         """
     )
-            
-    geometry_xml_file = file_col1.file_uploader(
-        "Upload your geometry.xml", type=["xml"]
-    )
-    dagmc_file = file_col2.file_uploader("Upload your DAGMC h5m", type=["h5m"])
-
-    my_geometry = None
-
-    if dagmc_file is None and geometry_xml_file is None:
-        new_title = '<center><p style="font-family:sans-serif; color:Red; font-size: 30px;">Upload your geometry.xml or DAGMC h5m file</p></center>'
-        st.markdown(new_title, unsafe_allow_html=True)
-
-        st.write(
-            """
-                Not got a geometry.xml file handy, right mouse 🖱️ click and save these links 
-                [ example 1 ](https://fusion-energy.github.io/openmc_geometry_plot/examples/csg_tokamak/geometry.xml),
-                [ example 2 ](https://fusion-energy.github.io/openmc_geometry_plot/examples/csg_cylinder_box/geometry.xml)
-            """
-        )
-        st.write(
-            """
-                Not got a DAGMC h5m file handy, right mouse 🖱️ click and save these links 
-                [ example 1 ](https://fusion-energy.github.io/openmc_geometry_plot/examples/dagmc_tokamak/dagmc_180_tokamak.h5m)
-            """
-        )
-    # DAGMC route
-    elif dagmc_file is not None and geometry_xml_file is not None:
-
-        save_uploadedfile(dagmc_file)
-        save_uploadedfile(geometry_xml_file)
-
-        bound_dag_univ = openmc.DAGMCUniverse(
-            filename=dagmc_file.name
-        ).bounded_universe()
-        my_geometry = openmc.Geometry(root=bound_dag_univ)
-
-        dag_universe = my_geometry.get_dagmc_universe()
-
-        mat_ids = range(0, len(dag_universe.material_names) + 1)
-        # mat_names = dag_universe.material_names
-
-        if len(mat_ids) >= 1:
-            set_mat_ids = set(mat_ids)
-        else:
-            set_mat_ids = ()
-
-        # set_cell_ids = set(di.get_volumes_from_h5m(dagmc_file.name))
-        set_cell_ids = list(range(1, dag_universe.n_cells + 1))
-        set_mat_names = set(dag_universe.material_names)
-        all_cell_names = set_cell_ids
-        set_cell_names = set(all_cell_names)
-
-    elif dagmc_file is not None and geometry_xml_file is None:
-
-        save_uploadedfile(dagmc_file)
-
-        # make a basic openmc geometry
-        bound_dag_univ = openmc.DAGMCUniverse(
-            filename=dagmc_file.name
-        ).bounded_universe()
-        my_geometry = openmc.Geometry(root=bound_dag_univ)
+# DAGMC route
+elif dagmc_file is not None and geometry_xml_file is not None:
 
-        dag_universe = my_geometry.get_dagmc_universe()
+    save_uploadedfile(dagmc_file)
+    save_uploadedfile(geometry_xml_file)
 
-        # find all material names
-        mat_ids = range(0, len(dag_universe.material_names) + 1)
-
-        if len(mat_ids) >= 1:
-            set_mat_ids = set(mat_ids)
-        else:
-            set_mat_ids = ()
-
-        # set_cell_ids = set(di.get_volumes_from_h5m(dagmc_file.name))
-        set_cell_ids = list(range(1, dag_universe.n_cells + 1))
-        set_mat_names = set(dag_universe.material_names)
-        all_cell_names = set_cell_ids
-        set_cell_names = set(all_cell_names)
-
-    # CSG route
-    elif dagmc_file is None and geometry_xml_file is not None:
-        save_uploadedfile(geometry_xml_file)
-
-        tree = ET.parse(geometry_xml_file.name)
-
-        root = tree.getroot()
-        all_cells = root.findall("cell")
-        mat_ids = []
-
-        for cell in all_cells:
-            if "material" in cell.keys():
-                if cell.get("material") == "void":
-                    mat_ids.append(0)
-                    print(f"material for cell {cell} is void")
-                else:
-                    mat_ids.append(int(cell.get("material")))
-
-        if len(mat_ids) >= 1:
-            set_mat_ids = set(mat_ids)
-        else:
-            set_mat_ids = ()
-
-        set_mat_names = set_mat_ids  # can't find material names in CSG with just the geometry xml as we don't have material names
+    bound_dag_univ = openmc.DAGMCUniverse(
+        filename=dagmc_file.name
+    ).bounded_universe()
+    my_geometry = openmc.Geometry(root=bound_dag_univ)
+
+    dag_universe = my_geometry.get_dagmc_universe()
+
+    mat_ids = range(0, len(dag_universe.material_names) + 1)
+    # mat_names = dag_universe.material_names
+
+    if len(mat_ids) >= 1:
+        set_mat_ids = set(mat_ids)
+    else:
+        set_mat_ids = ()
+
+    # set_cell_ids = set(di.get_volumes_from_h5m(dagmc_file.name))
+    set_cell_ids = list(range(1, dag_universe.n_cells + 1))
+    set_mat_names = set(dag_universe.material_names)
+    all_cell_names = set_cell_ids
+    set_cell_names = set(all_cell_names)
+
+elif dagmc_file is not None and geometry_xml_file is None:
+
+    save_uploadedfile(dagmc_file)
+
+    # make a basic openmc geometry
+    bound_dag_univ = openmc.DAGMCUniverse(
+        filename=dagmc_file.name
+    ).bounded_universe()
+    my_geometry = openmc.Geometry(root=bound_dag_univ)
+
+    dag_universe = my_geometry.get_dagmc_universe()
+
+    # find all material names
+    mat_ids = range(0, len(dag_universe.material_names) + 1)
+
+    if len(mat_ids) >= 1:
+        set_mat_ids = set(mat_ids)
+    else:
+        set_mat_ids = ()
+
+    # set_cell_ids = set(di.get_volumes_from_h5m(dagmc_file.name))
+    set_cell_ids = list(range(1, dag_universe.n_cells + 1))
+    set_mat_names = set(dag_universe.material_names)
+    all_cell_names = set_cell_ids
+    set_cell_names = set(all_cell_names)
+
+# CSG route
+elif dagmc_file is None and geometry_xml_file is not None:
+    save_uploadedfile(geometry_xml_file)
+
+    tree = ET.parse(geometry_xml_file.name)
+
+    root = tree.getroot()
+    all_cells = root.findall("cell")
+    mat_ids = []
+
+    for cell in all_cells:
+        if "material" in cell.keys():
+            if cell.get("material") == "void":
+                mat_ids.append(0)
+                print(f"material for cell {cell} is void")
+            else:
+                mat_ids.append(int(cell.get("material")))
 
-        my_mats = openmc.Materials()
-        for mat_id in set_mat_ids:
-            new_mat = openmc.Material()
-            new_mat.id = mat_id
-            new_mat.add_nuclide("He4", 1)
-            # adds a single nuclide that is in minimal cross section xml to avoid material failing
-            my_mats.append(new_mat)
+    if len(mat_ids) >= 1:
+        set_mat_ids = set(mat_ids)
+    else:
+        set_mat_ids = ()
+
+    set_mat_names = set_mat_ids  # can't find material names in CSG with just the geometry xml as we don't have material names
+
+    my_mats = openmc.Materials()
+    for mat_id in set_mat_ids:
+        new_mat = openmc.Material()
+        new_mat.id = mat_id
+        new_mat.add_nuclide("He4", 1)
+        # adds a single nuclide that is in minimal cross section xml to avoid material failing
+        my_mats.append(new_mat)
 
-        my_geometry = openmc.Geometry.from_xml(
-            path=geometry_xml_file.name, materials=my_mats
-        )
-        all_cell_ids = []
-        all_cell_names = []
-        all_cells = my_geometry.get_all_cells()
-        for cell_id, cell in all_cells.items():
-            all_cell_ids.append(cell.id)
-            all_cell_names.append(cell.name)
-        set_cell_ids = set(all_cell_ids)
-        set_cell_names = set(all_cell_names)
-
-    if my_geometry:
-        print("geometry is set to something so attempting to plot")
-        bb = my_geometry.bounding_box
-
-        col1, col2 = st.columns([1, 3])
-
-        view_direction = col1.selectbox(
-            label="View direction",
-            options=("z", "x", "y"),
-            index=0,
-            key="geometry_view_direction",
-            help="Setting the direction of view automatically sets the horizontal and vertical axis used for the plot.",
-        )
-        backend = col1.selectbox(
-            label="Ploting backend",
-            options=("matplotlib", "plotly"),
-            index=0,
-            key="geometry_ploting_backend",
-            help="Create png images with MatPlotLib or HTML plots with Plotly",
+    my_geometry = openmc.Geometry.from_xml(
+        path=geometry_xml_file.name, materials=my_mats
+    )
+    all_cell_ids = []
+    all_cell_names = []
+    all_cells = my_geometry.get_all_cells()
+    for cell_id, cell in all_cells.items():
+        all_cell_ids.append(cell.id)
+        all_cell_names.append(cell.name)
+    set_cell_ids = set(all_cell_ids)
+    set_cell_names = set(all_cell_names)
+
+if my_geometry:
+    print("geometry is set to something so attempting to plot")
+    bb = my_geometry.bounding_box
+
+    view_direction = st.sidebar.selectbox(
+        label="View direction",
+        options=("z", "x", "y"),
+        index=0,
+        key="geometry_view_direction",
+        help="Setting the direction of view automatically sets the horizontal and vertical axis used for the plot.",
+    )
+    backend = st.sidebar.selectbox(
+        label="Ploting backend",
+        options=("matplotlib", "plotly"),
+        index=0,
+        key="geometry_ploting_backend",
+        help="Create png images with MatPlotLib or HTML plots with Plotly",
+    )
+    outline = st.sidebar.selectbox(
+        label="Outline",
+        options=("materials", "cells", None),
+        index=0,
+        key="outline",
+        help="Allows an outline to be drawn around the cells or materials, select None for no outline",
+    )
+    color_by = st.sidebar.selectbox(
+        label="Color by",
+        options=("materials", "cells"),
+        index=0,
+        key="color_by",
+        help="Should the plot be colored by material or by cell",
+    )
+    plot_left, plot_right = None, None
+    plot_bottom, plot_top = None, None
+    x_min, x_max = None, None
+    y_min, y_max = None, None
+
+    x_index = {"z": 0, "y": 0, "x": 1}[view_direction]
+    y_index = {"z": 1, "y": 2, "x": 2}[view_direction]
+    slice_index = {"z": 2, "y": 1, "x": 0}[view_direction]
+
+    if np.isinf(bb[0][x_index]) or np.isinf(bb[1][x_index]):
+        x_min = st.sidebar.number_input(label="minimum vertical axis value", key="x_min")
+        x_max = st.sidebar.number_input(label="maximum vertical axis value", key="x_max")
+    else:
+        x_min = float(bb[0][x_index])
+        x_max = float(bb[1][x_index])
+
+    # y axis is y values
+    if np.isinf(bb[0][y_index]) or np.isinf(bb[1][y_index]):
+        y_min = st.sidebar.number_input(label="minimum vertical axis value", key="y_min")
+        y_max = st.sidebar.number_input(label="maximum vertical axis value", key="y_max")
+    else:
+        y_min = float(bb[0][y_index])
+        y_max = float(bb[1][y_index])
+
+    # slice axis is z
+    if np.isinf(bb[0][slice_index]) or np.isinf(bb[1][slice_index]):
+        slice_min = st.sidebar.number_input(label="minimum slice value", key="slice_min")
+        slice_max = st.sidebar.number_input(label="maximum slice value", key="slice_max")
+    else:
+        slice_min = float(bb[0][slice_index])
+        slice_max = float(bb[1][slice_index])
+
+    if isinstance(x_min, float) and isinstance(x_max, float):
+        plot_right, plot_left = st.sidebar.slider(
+            label="Left and right values for the horizontal axis",
+            min_value=x_min,
+            max_value=x_max,
+            value=(x_min, x_max),
+            key="left_right_slider",
+            help="Set the lowest visible value and highest visible value on the horizontal axis",
         )
-        outline = col1.selectbox(
-            label="Outline",
-            options=("materials", "cells", None),
-            index=0,
-            key="outline",
-            help="Allows an outline to be drawn around the cells or materials, select None for no outline",
+
+    if isinstance(y_min, float) and isinstance(y_max, float):
+        plot_bottom, plot_top = st.sidebar.slider(
+            label="Bottom and top values for the vertical axis",
+            min_value=y_min,
+            max_value=y_max,
+            value=(y_min, y_max),
+            key="bottom_top_slider",
+            help="Set the lowest visible value and highest visible value on the vertical axis",
         )
-        color_by = col1.selectbox(
-            label="Color by",
-            options=("materials", "cells"),
-            index=0,
-            key="color_by",
-            help="Should the plot be colored by material or by cell",
+    if isinstance(slice_min, float) and isinstance(slice_max, float):
+        slice_value = st.sidebar.slider(
+            label="Slice value",
+            min_value=slice_min,
+            max_value=slice_max,
+            value=(slice_min + slice_max) / 2,
+            key="slice_slider",
+            help="Set the value of the slice axis",
         )
-        plot_left, plot_right = None, None
-        plot_bottom, plot_top = None, None
-        x_min, x_max = None, None
-        y_min, y_max = None, None
-
-        x_index = {"z": 0, "y": 0, "x": 1}[view_direction]
-        y_index = {"z": 1, "y": 2, "x": 2}[view_direction]
-        slice_index = {"z": 2, "y": 1, "x": 0}[view_direction]
-
-        if np.isinf(bb[0][x_index]) or np.isinf(bb[1][x_index]):
-            x_min = col1.number_input(label="minimum vertical axis value", key="x_min")
-            x_max = col1.number_input(label="maximum vertical axis value", key="x_max")
-        else:
-            x_min = float(bb[0][x_index])
-            x_max = float(bb[1][x_index])
 
-        # y axis is y values
-        if np.isinf(bb[0][y_index]) or np.isinf(bb[1][y_index]):
-            y_min = col1.number_input(label="minimum vertical axis value", key="y_min")
-            y_max = col1.number_input(label="maximum vertical axis value", key="y_max")
-        else:
-            y_min = float(bb[0][y_index])
-            y_max = float(bb[1][y_index])
-
-        # slice axis is z
-        if np.isinf(bb[0][slice_index]) or np.isinf(bb[1][slice_index]):
-            slice_min = col1.number_input(label="minimum slice value", key="slice_min")
-            slice_max = col1.number_input(label="maximum slice value", key="slice_max")
-        else:
-            slice_min = float(bb[0][slice_index])
-            slice_max = float(bb[1][slice_index])
+    pixels_across = st.sidebar.number_input(
+        label="Number of horizontal pixels",
+        value=500,
+        help="Increasing this value increases the image resolution but also requires longer to create the image",
+    )
 
-        if isinstance(x_min, float) and isinstance(x_max, float):
-            plot_right, plot_left = col1.slider(
-                label="Left and right values for the horizontal axis",
-                min_value=x_min,
-                max_value=x_max,
-                value=(x_min, x_max),
-                key="left_right_slider",
-                help="Set the lowest visible value and highest visible value on the horizontal axis",
+    selected_color_map = st.sidebar.selectbox(
+        label="Color map", options=colormaps(), index=82
+    )  # index 82 is tab20c
+
+    if color_by == "materials":
+
+        cmap = cm.get_cmap(selected_color_map, len(set_mat_ids))
+        initial_hex_color = []
+        for i in range(cmap.N):
+            rgba = cmap(i)
+            # rgb2hex accepts rgb or rgba
+            initial_hex_color.append(colors.rgb2hex(rgba))
+
+        for c, id in enumerate(set_mat_ids):
+            # todo add
+            st.sidebar.color_picker(
+                f"Color of material with id {id}",
+                key=f"mat_{id}",
+                value=initial_hex_color[c],
             )
 
-        if isinstance(y_min, float) and isinstance(y_max, float):
-            plot_bottom, plot_top = col1.slider(
-                label="Bottom and top values for the vertical axis",
-                min_value=y_min,
-                max_value=y_max,
-                value=(y_min, y_max),
-                key="bottom_top_slider",
-                help="Set the lowest visible value and highest visible value on the vertical axis",
-            )
-        if isinstance(slice_min, float) and isinstance(slice_max, float):
-            slice_value = col1.slider(
-                label="Slice value",
-                min_value=slice_min,
-                max_value=slice_max,
-                value=(slice_min + slice_max) / 2,
-                key="slice_slider",
-                help="Set the value of the slice axis",
+        my_colors = {}
+        for id in set_mat_ids:
+            hex_color = st.session_state[f"mat_{id}"].lstrip("#")
+            RGB = tuple(int(hex_color[i : i + 2], 16) / 255 for i in (0, 2, 4))
+            my_colors[id] = RGB
+
+    elif color_by == "cells":
+        cmap = cm.get_cmap(selected_color_map, len(set_cell_ids))
+        initial_hex_color = []
+        for i in range(cmap.N):
+            rgba = cmap(i)
+            # rgb2hex accepts rgb or rgba
+            initial_hex_color.append(colors.rgb2hex(rgba))
+
+        for c, (cell_id, cell_name) in enumerate(zip(set_cell_ids, all_cell_names)):
+            if cell_name in ["", None]:
+                cell_name = "not set"
+            st.color_picker(
+                f"Color of cell id {cell_id}, cell name {cell_name}",
+                key=f"cell_{cell_id}",
+                value=initial_hex_color[c],
             )
 
-        pixels_across = col1.number_input(
-            label="Number of horizontal pixels",
-            value=500,
-            help="Increasing this value increases the image resolution but also requires longer to create the image",
-        )
-
-        selected_color_map = col1.selectbox(
-            label="Color map", options=colormaps(), index=82
-        )  # index 82 is tab20c
-
-        if color_by == "materials":
-
-            cmap = cm.get_cmap(selected_color_map, len(set_mat_ids))
-            initial_hex_color = []
-            for i in range(cmap.N):
-                rgba = cmap(i)
-                # rgb2hex accepts rgb or rgba
-                initial_hex_color.append(colors.rgb2hex(rgba))
-
-            for c, id in enumerate(set_mat_ids):
-                # todo add
-                st.color_picker(
-                    f"Color of material with id {id}",
-                    key=f"mat_{id}",
-                    value=initial_hex_color[c],
-                )
+        my_colors = {0: (1, 1, 1)}  # adding entry for void cells
+        for id in set_cell_ids:
+            hex_color = st.session_state[f"cell_{id}"].lstrip("#")
+            RGB = tuple(int(hex_color[i : i + 2], 16) / 255 for i in (0, 2, 4))
+            my_colors[id] = RGB
+
+    title = st.sidebar.text_input(
+        "Plot title",
+        help="Optionally set your own title for the plot",
+        value=f"Slice through OpenMC geometry with view direction {view_direction}",
+    )
 
-            my_colors = {}
-            for id in set_mat_ids:
-                hex_color = st.session_state[f"mat_{id}"].lstrip("#")
-                RGB = tuple(int(hex_color[i : i + 2], 16) / 255 for i in (0, 2, 4))
-                my_colors[id] = RGB
-
-        elif color_by == "cells":
-            cmap = cm.get_cmap(selected_color_map, len(set_cell_ids))
-            initial_hex_color = []
-            for i in range(cmap.N):
-                rgba = cmap(i)
-                # rgb2hex accepts rgb or rgba
-                initial_hex_color.append(colors.rgb2hex(rgba))
-
-            for c, (cell_id, cell_name) in enumerate(zip(set_cell_ids, all_cell_names)):
-                if cell_name in ["", None]:
-                    cell_name = "not set"
-                st.color_picker(
-                    f"Color of cell id {cell_id}, cell name {cell_name}",
-                    key=f"cell_{cell_id}",
-                    value=initial_hex_color[c],
-                )
+    if (
+        isinstance(plot_left, float)
+        and isinstance(plot_right, float)
+        and isinstance(plot_top, float)
+        and isinstance(plot_bottom, float)
+    ):
+        if color_by == "cells":
+            color_data_slice = my_geometry.get_slice_of_cell_ids(
+                view_direction=view_direction,
+                plot_left=plot_left,
+                plot_right=plot_right,
+                plot_top=plot_top,
+                plot_bottom=plot_bottom,
+                pixels_across=pixels_across,
+                slice_value=slice_value,
+            )
+        elif color_by == "materials":
+            color_data_slice = my_geometry.get_slice_of_material_ids(
+                view_direction=view_direction,
+                plot_left=plot_left,
+                plot_right=plot_right,
+                plot_top=plot_top,
+                plot_bottom=plot_bottom,
+                pixels_across=pixels_across,
+                slice_value=slice_value,
+            )
 
-            my_colors = {0: (1, 1, 1)}  # adding entry for void cells
-            for id in set_cell_ids:
-                hex_color = st.session_state[f"cell_{id}"].lstrip("#")
-                RGB = tuple(int(hex_color[i : i + 2], 16) / 255 for i in (0, 2, 4))
-                my_colors[id] = RGB
-
-        title = col1.text_input(
-            "Plot title",
-            help="Optionally set your own title for the plot",
-            value=f"Slice through OpenMC geometry with view direction {view_direction}",
+        (xlabel, ylabel) = my_geometry.get_axis_labels(
+            view_direction=view_direction
         )
-
-        if (
-            isinstance(plot_left, float)
-            and isinstance(plot_right, float)
-            and isinstance(plot_top, float)
-            and isinstance(plot_bottom, float)
-        ):
-            if color_by == "cells":
-                color_data_slice = my_geometry.get_slice_of_cell_ids(
+        if outline is not None:
+            # gets unique levels for outlines contour plot
+            # this can be avoided if outline is the same as the color data
+            if outline == color_by:
+                outline_data_slice = color_data_slice
+            elif outline == "cells":
+                outline_data_slice = my_geometry.get_slice_of_cell_ids(
                     view_direction=view_direction,
                     plot_left=plot_left,
                     plot_right=plot_right,
                     plot_top=plot_top,
                     plot_bottom=plot_bottom,
                     pixels_across=pixels_across,
                     slice_value=slice_value,
                 )
-            elif color_by == "materials":
-                color_data_slice = my_geometry.get_slice_of_material_ids(
+            elif outline == "materials":
+                outline_data_slice = my_geometry.get_slice_of_material_ids(
                     view_direction=view_direction,
                     plot_left=plot_left,
                     plot_right=plot_right,
                     plot_top=plot_top,
                     plot_bottom=plot_bottom,
                     pixels_across=pixels_across,
                     slice_value=slice_value,
                 )
+            else:
+                raise ValueError(
+                    f"outline can only be cells or materials, not {outline}"
+                )
+
+        if backend == "matplotlib":
 
-            (xlabel, ylabel) = my_geometry.get_axis_labels(
-                view_direction=view_direction
+            extent = my_geometry.get_plot_extent(
+                plot_left,
+                plot_right,
+                plot_bottom,
+                plot_top,
+                slice_value,
+                bb,
+                view_direction,
+            )[
+                :-1
+            ]  # slice value is returned in the function so removing with -1
+
+            bounds = list(my_colors.keys())
+            color_values = list(my_colors.values())
+
+            mat_cmap = colors.ListedColormap(color_values)
+            # our material ids are set to be 1 and 2. void space is 0
+            # this +1 is needed as the bounds must be larger that the value to include the values
+            bounds.append(bounds[-1] + 1)
+
+            mat_norm = colors.BoundaryNorm(bounds, mat_cmap.N)
+
+            plt.imshow(
+                color_data_slice,
+                extent=extent,
+                interpolation="none",
+                norm=mat_norm,  # needed for colors
+                cmap=mat_cmap,  # needed for colors
             )
-            if outline is not None:
-                # gets unique levels for outlines contour plot
-                # this can be avoided if outline is the same as the color data
-                if outline == color_by:
-                    outline_data_slice = color_data_slice
-                elif outline == "cells":
-                    outline_data_slice = my_geometry.get_slice_of_cell_ids(
-                        view_direction=view_direction,
-                        plot_left=plot_left,
-                        plot_right=plot_right,
-                        plot_top=plot_top,
-                        plot_bottom=plot_bottom,
-                        pixels_across=pixels_across,
-                        slice_value=slice_value,
-                    )
-                elif outline == "materials":
-                    outline_data_slice = my_geometry.get_slice_of_material_ids(
-                        view_direction=view_direction,
-                        plot_left=plot_left,
-                        plot_right=plot_right,
-                        plot_top=plot_top,
-                        plot_bottom=plot_bottom,
-                        pixels_across=pixels_across,
-                        slice_value=slice_value,
-                    )
-                else:
-                    raise ValueError(
-                        f"outline can only be cells or materials, not {outline}"
-                    )
 
-            if backend == "matplotlib":
+            plt.xlabel(xlabel)
+            plt.ylabel(ylabel)
+            plt.title(title)
 
-                extent = my_geometry.get_plot_extent(
-                    plot_left,
-                    plot_right,
-                    plot_bottom,
-                    plot_top,
-                    slice_value,
-                    bb,
-                    view_direction,
-                )[
-                    :-1
-                ]  # slice value is returned in the function so removing with -1
-
-                bounds = list(my_colors.keys())
-                color_values = list(my_colors.values())
-
-                mat_cmap = colors.ListedColormap(color_values)
-                # our material ids are set to be 1 and 2. void space is 0
-                # this +1 is needed as the bounds must be larger that the value to include the values
-                bounds.append(bounds[-1] + 1)
+            if outline is not None:
+                levels = np.unique(
+                    [item for sublist in outline_data_slice for item in sublist]
+                )
+                plt.contour(
+                    outline_data_slice,
+                    origin="upper",
+                    colors="k",
+                    linestyles="solid",
+                    levels=levels,
+                    linewidths=0.5,
+                    extent=extent,
+                )
 
-                mat_norm = colors.BoundaryNorm(bounds, mat_cmap.N)
+            plt.savefig("openmc_plot_geometry_image.png")
+            st.pyplot(plt)
 
-                plt.imshow(
-                    color_data_slice,
-                    extent=extent,
-                    interpolation="none",
-                    norm=mat_norm,  # needed for colors
-                    cmap=mat_cmap,  # needed for colors
+            with open("openmc_plot_geometry_image.png", "rb") as file:
+                st.sidebar.download_button(
+                    label="Download image",
+                    data=file,
+                    file_name="openmc_plot_geometry_image.png",
+                    mime="image/png",
                 )
+        else:
 
-                plt.xlabel(xlabel)
-                plt.ylabel(ylabel)
-                plt.title(title)
-
-                if outline is not None:
-                    levels = np.unique(
-                        [item for sublist in outline_data_slice for item in sublist]
-                    )
-                    plt.contour(
-                        outline_data_slice,
-                        origin="upper",
-                        colors="k",
-                        linestyles="solid",
-                        levels=levels,
-                        linewidths=0.5,
-                        extent=extent,
-                    )
+            data = [
+                go.Heatmap(
+                    z=color_data_slice,
+                    showscale=False,
+                    colorscale="viridis",
+                    x0=plot_left,
+                    dx=abs(plot_left - plot_right) / (len(color_data_slice[0]) - 1),
+                    y0=plot_bottom,
+                    dy=abs(plot_bottom - plot_top) / (len(color_data_slice) - 1),
+                    # colorbar=dict(title=dict(side="right", text=cbar_label)),
+                    # text = material_ids,
+                    # hovertemplate=
+                    # # 'material ID = %{z}<br>'+
+                    # "Cell ID = %{z}<br>" +
+                    # # '<br>%{text}<br>'+
+                    # xlabel[:2].title()
+                    # + ": %{x} cm<br>"
+                    # + ylabel[:2].title()
+                    # + ": %{y} cm<br>",
+                )
+            ]
 
-                plt.savefig("openmc_plot_geometry_image.png")
-                col2.pyplot(plt)
-                # col2.image("openmc_plot_geometry_image.png", use_column_width="always")
-
-                with open("openmc_plot_geometry_image.png", "rb") as file:
-                    col1.download_button(
-                        label="Download image",
-                        data=file,
-                        file_name="openmc_plot_geometry_image.png",
-                        mime="image/png",
-                    )
-            else:
+            if outline is not None:
 
-                data = [
-                    go.Heatmap(
-                        z=color_data_slice,
-                        showscale=False,
-                        colorscale="viridis",
+                data.append(
+                    go.Contour(
+                        z=outline_data_slice,
                         x0=plot_left,
-                        dx=abs(plot_left - plot_right) / (len(color_data_slice[0]) - 1),
+                        dx=abs(plot_left - plot_right)
+                        / (len(outline_data_slice[0]) - 1),
                         y0=plot_bottom,
-                        dy=abs(plot_bottom - plot_top) / (len(color_data_slice) - 1),
-                        # colorbar=dict(title=dict(side="right", text=cbar_label)),
-                        # text = material_ids,
-                        # hovertemplate=
-                        # # 'material ID = %{z}<br>'+
-                        # "Cell ID = %{z}<br>" +
-                        # # '<br>%{text}<br>'+
-                        # xlabel[:2].title()
-                        # + ": %{x} cm<br>"
-                        # + ylabel[:2].title()
-                        # + ": %{y} cm<br>",
+                        dy=abs(plot_bottom - plot_top)
+                        / (len(outline_data_slice) - 1),
+                        contours_coloring="lines",
+                        line_width=1,
+                        colorscale=[[0, "rgb(0, 0, 0)"], [1.0, "rgb(0, 0, 0)"]],
+                        showscale=False,
                     )
-                ]
+                )
 
-                if outline is not None:
+            plot = go.Figure(data=data)
 
-                    data.append(
-                        go.Contour(
-                            z=outline_data_slice,
-                            x0=plot_left,
-                            dx=abs(plot_left - plot_right)
-                            / (len(outline_data_slice[0]) - 1),
-                            y0=plot_bottom,
-                            dy=abs(plot_bottom - plot_top)
-                            / (len(outline_data_slice) - 1),
-                            contours_coloring="lines",
-                            line_width=1,
-                            colorscale=[[0, "rgb(0, 0, 0)"], [1.0, "rgb(0, 0, 0)"]],
-                            showscale=False,
-                        )
-                    )
+            plot.update_layout(
+                xaxis={"title": xlabel},
+                # reversed autorange is required to avoid image needing rotation/flipping in plotly
+                yaxis={"title": ylabel, "autorange": "reversed"},
+                title=title,
+                autosize=False,
+                height=800,
+            )
+            plot.update_yaxes(
+                scaleanchor="x",
+                scaleratio=1,
+            )
 
-                plot = go.Figure(data=data)
+            plot.write_html("openmc_plot_geometry_image.html")
 
-                plot.update_layout(
-                    xaxis={"title": xlabel},
-                    # reversed autorange is required to avoid image needing rotation/flipping in plotly
-                    yaxis={"title": ylabel, "autorange": "reversed"},
-                    title=title,
-                    autosize=False,
-                    height=800,
+            with open("openmc_plot_geometry_image.html", "rb") as file:
+                st.sidebar.download_button(
+                    label="Download image",
+                    data=file,
+                    file_name="openmc_plot_geometry_image.html",
+                    mime=None,
                 )
-                plot.update_yaxes(
-                    scaleanchor="x",
-                    scaleratio=1,
-                )
-
-                plot.write_html("openmc_plot_geometry_image.html")
+            st.plotly_chart(plot, use_container_width=True)
 
-                with open("openmc_plot_geometry_image.html", "rb") as file:
-                    col1.download_button(
-                        label="Download image",
-                        data=file,
-                        file_name="openmc_plot_geometry_image.html",
-                        mime=None,
-                    )
-                col2.plotly_chart(plot, use_container_width=True)
-
-            col2.write("Model info")
-            col2.write(f"Material IDS found {set_mat_ids}")
-            col2.write(f"Material names found {set_mat_names}")
-            col2.write(f"Cell IDS found {set_cell_ids}")
-            col2.write(f"Cell names found {set_cell_names}")
-            col2.write(
-                f"Bounding box lower left x={bb[0][0]} y={bb[0][1]} z={bb[0][2]}"
-            )
-            col2.write(
-                f"Bounding box upper right x={bb[1][0]} y={bb[1][1]} z={bb[1][2]}"
-            )
+        st.write("Model info")
+        st.write(f"Material IDS found {set_mat_ids}")
+        st.write(f"Material names found {set_mat_names}")
+        st.write(f"Cell IDS found {set_cell_ids}")
+        st.write(f"Cell names found {set_cell_names}")
+        st.write(
+            f"Bounding box lower left x={bb[0][0]} y={bb[0][1]} z={bb[0][2]}"
+        )
+        st.write(
+            f"Bounding box upper right x={bb[1][0]} y={bb[1][1]} z={bb[1][2]}"
+        )
```

### Comparing `openmc_plot-0.2.2/src/openmc_plot/source_tab.py` & `openmc_plot-0.3.0/src/openmc_plot/pages/3_✴️_Source_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,74 @@
 import streamlit as st
 from utils import save_uploadedfile
 import openmc
 import openmc_source_plotter
 
 
-def create_source_tab():
+st.write(
+    """
+        This tab makes use of the 🐍 Python package ```openmc_source_plotter``` which is available on [GitHub](https://github.com/fusion-energy/openmc_source_plotter/).
+
+        👉 Create your ```openmc.Settings()``` assign the Source and export the settings xml file using ```export_to_xml()```.
+    """
+)
+settings_xml_file = st.file_uploader(
+    "Upload your settings.xml", type=["xml"], key="settings_uploader"
+)
+
+if settings_xml_file == None:
+    new_title = '<p style="font-family:sans-serif; color:Red; font-size: 30px;">Upload your settings.xml</p>'
+    st.markdown(new_title, unsafe_allow_html=True)
 
-    st.write(
+    st.markdown(
         """
-            This tab makes use of the 🐍 Python package ```openmc_source_plotter``` which is available on [GitHub](https://github.com/fusion-energy/openmc_source_plotter/).
-
-            👉 Create your ```openmc.Settings()``` assign the Source and export the settings xml file using ```export_to_xml()```.
+        Not got a settings xml file handy, right mouse 🖱️ click and save this link
+        [example 1](https://fusion-energy.github.io/openmc_plot/examples/ring_source/settings.xml)
         """
     )
-    settings_xml_file = st.file_uploader(
-        "Upload your settings.xml", type=["xml"], key="settings_uploader"
-    )
 
-    if settings_xml_file == None:
-        new_title = '<p style="font-family:sans-serif; color:Red; font-size: 30px;">Upload your settings.xml</p>'
-        st.markdown(new_title, unsafe_allow_html=True)
-
-        st.markdown(
-            """
-            Not got a settings xml file handy, right mouse 🖱️ click and save this link
-            [example 1](https://fusion-energy.github.io/openmc_plot/examples/ring_source/settings.xml)
-            """
-        )
+else:
 
-    else:
+    save_uploadedfile(settings_xml_file)
 
-        save_uploadedfile(settings_xml_file)
+    my_settings = openmc.Settings.from_xml(settings_xml_file.name)
 
-        my_settings = openmc.Settings.from_xml(settings_xml_file.name)
+    type_of_source_plot = st.sidebar.radio(
+        "Select type of plot", options=["Energy", "Space", "Angle"]
+    )
 
-        col1, col2 = st.columns([1, 3])
+    n_samples = st.sidebar.number_input(
+        label="number of samples",
+        min_value=1,
+        step=1,
+        value=1000,
+    )
 
-        type_of_source_plot = col1.radio(
-            "Select type of plot", options=["Energy", "Space", "Angle"]
-        )
+    fig = None
 
-        n_samples = col1.number_input(
-            label="number of samples",
-            min_value=1,
-            step=1,
-            value=1000,
+    for old_source in my_settings.source:
+        new_source = openmc.Source()
+        if old_source.angle is not None:
+            new_source.angle = old_source.angle
+        if old_source.space is not None:
+            new_source.space = old_source.space
+        if old_source.energy is not None:
+            new_source.energy = old_source.energy
+
+        if type_of_source_plot == "Energy":
+            fig = new_source.plot_source_energy(figure=fig, n_samples=n_samples)
+        if type_of_source_plot == "Angle":
+            fig = new_source.plot_source_direction(figure=fig, n_samples=n_samples)
+        if type_of_source_plot == "Space":
+            fig = new_source.plot_source_position(figure=fig, n_samples=n_samples)
+
+    st.plotly_chart(fig)
+
+    fig.write_html("openmc_plot_source_image.html")
+
+    with open("openmc_plot_source_image.html", "rb") as file:
+        st.sidebar.download_button(
+            label="Download image",
+            data=file,
+            file_name="openmc_plot_source_image.html",
+            mime=None,
         )
-
-        fig = None
-
-        for old_source in my_settings.source:
-            new_source = openmc.Source()
-            if old_source.angle is not None:
-                new_source.angle = old_source.angle
-            if old_source.space is not None:
-                new_source.space = old_source.space
-            if old_source.energy is not None:
-                new_source.energy = old_source.energy
-
-            if type_of_source_plot == "Energy":
-                fig = new_source.plot_source_energy(figure=fig, n_samples=n_samples)
-            if type_of_source_plot == "Angle":
-                fig = new_source.plot_source_direction(figure=fig, n_samples=n_samples)
-            if type_of_source_plot == "Space":
-                fig = new_source.plot_source_position(figure=fig, n_samples=n_samples)
-
-        col2.plotly_chart(fig)
-
-        fig.write_html('openmc_plot_source_image.html')
-
-        with open("openmc_plot_source_image.html", "rb") as file:
-            col1.download_button(
-                label="Download image",
-                data=file,
-                file_name="openmc_plot_source_image.html",
-                mime=None
-            )
```

### Comparing `openmc_plot-0.2.2/src/openmc_plot/weightwindows_tab.py` & `openmc_plot-0.3.0/src/openmc_plot/pages/4_🪟_Weight_window_plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,183 +4,191 @@
 import openmc
 import matplotlib.pyplot as plt
 from pylab import *
 import xml.etree.ElementTree as ET
 from matplotlib.colors import LogNorm
 
 
-def create_weightwindow_tab():
+
+st.write(
+    """
+        👉 Create your ```openmc.WeightWindows()``` and export the settings xml file using ```export_to_xml()```.
+
+        Weight windows on RegularMesh and CylindricalMesh are supported
+    """
+)
+settings_xml_file = st.file_uploader("Upload your settings.xml", type=["xml"])
+
+if settings_xml_file == None:
+    new_title = '<p style="font-family:sans-serif; color:Red; font-size: 30px;">Upload your settings.xml</p>'
+    st.markdown(new_title, unsafe_allow_html=True)
 
     st.write(
         """
-            👉 Create your ```openmc.WeightWindows()``` and export the settings xml file using ```export_to_xml()```.
-
-            Weight windows on RegularMesh and CylindricalMesh are supported
+            Not got a settings xml file handy, right mouse 🖱️ click and save these links 
+            [ example 1 ](https://fusion-energy.github.io/openmc_plot/examples/weightwindows/settings.xml)
         """
     )
-    settings_xml_file = st.file_uploader("Upload your settings.xml", type=["xml"])
+else:
 
-    if settings_xml_file == None:
-        new_title = '<p style="font-family:sans-serif; color:Red; font-size: 30px;">Upload your settings.xml</p>'
-        st.markdown(new_title, unsafe_allow_html=True)
+    save_uploadedfile(settings_xml_file)
 
-        st.write(
-            """
-                Not got a settings xml file handy, right mouse 🖱️ click and save these links 
-                [ example 1 ](https://fusion-energy.github.io/openmc_plot/examples/weightwindows/settings.xml)
-            """
-        )
-    else:
+    my_settings = openmc.Settings.from_xml(settings_xml_file.name)
 
-        save_uploadedfile(settings_xml_file)
+    weight_windows = my_settings.weight_windows
 
-        my_settings = openmc.Settings.from_xml(settings_xml_file.name)
+    if weight_windows == []:
 
-        weight_windows = my_settings.weight_windows
+        msg = f"{settings_xml_file.name} does not contain weight windows"
+        new_title = f'<p style="font-family:sans-serif; color:Red; font-size: 30px;">{msg}</p>'
+        st.markdown(new_title, unsafe_allow_html=True)
 
-        if weight_windows == []:
+    else:
 
-            msg = f'{settings_xml_file.name} does not contain weight windows'
-            new_title = f'<p style="font-family:sans-serif; color:Red; font-size: 30px;">{msg}</p>'
-            st.markdown(new_title, unsafe_allow_html=True)
+        weight_window_by_id = {}
+        for weight_window in weight_windows:
+            weight_window_by_id[weight_window.id] = weight_window
+
+        if len(weight_window_by_id.keys()) > 1:
+            weight_window_selector = st.sidebar.selectbox(
+                label="Weight window ID to plot",
+                options=weight_window_by_id.keys(),
+                index=0,
+            )
+        else:
+            weight_window_selector = list(weight_window_by_id.keys())[0]
 
+        selected_weight_window = weight_window_by_id[weight_window_selector]
+
+        upper_or_lower = st.sidebar.radio(
+            "upper or lower bounds", options=["upper bounds", "lower bounds"]
+        )
+        if upper_or_lower == "upper bounds":
+            plotted_part_of_weight_window = (
+                selected_weight_window.upper_ww_bounds.flatten()
+            )
         else:
+            plotted_part_of_weight_window = (
+                selected_weight_window.lower_ww_bounds.flatten()
+            )
 
-            weight_window_by_id = {}
-            for weight_window in weight_windows:
-                weight_window_by_id[weight_window.id] = weight_window
-
-            col1, col2 = st.columns([1, 3])
-
-            if len(weight_window_by_id.keys()) > 1:
-                weight_window_selector = col1.selectbox(
-                    label="Weight window ID to plot", options=weight_window_by_id.keys(), index=0
-                )
-            else:
-                weight_window_selector = list(weight_window_by_id.keys())[0]
+        mesh = selected_weight_window.mesh
 
-            selected_weight_window = weight_window_by_id[weight_window_selector]
+        if isinstance(mesh, openmc.CylindricalMesh):
 
-            upper_or_lower = col1.radio(
-                "upper or lower bounds", options=["upper bounds", "lower bounds"]
+            reshaped_tally = plotted_part_of_weight_window.reshape(
+                mesh.dimension, order="F"
             )
-            if upper_or_lower == "upper bounds":
-                plotted_part_of_weight_window = selected_weight_window.upper_ww_bounds.flatten()
-            else:
-                plotted_part_of_weight_window = selected_weight_window.lower_ww_bounds.flatten()
 
-            mesh = selected_weight_window.mesh
+            # TODO add XY top down slice
+            # axis_to_slice = st.sidebar.selectbox(
+            #     label="Slice plane", options=("RZ", "XY"), index=0, key='ww_axis_to_slice'
+            # )
+            axis_to_slice = "RZ"
 
-            if isinstance(mesh, openmc.CylindricalMesh):
+            reshaped_tally = plotted_part_of_weight_window.reshape(
+                (mesh.dimension[2], mesh.dimension[1], mesh.dimension[0]), order="F"
+            )
 
-                reshaped_tally = plotted_part_of_weight_window.reshape(mesh.dimension, order="F")
+            tally_aligned = reshaped_tally.transpose(2, 0, 1)
+            x_label = "R [cm]"
+            y_label = "Z [cm]"
+
+            left = mesh.r_grid[0]
+            right = mesh.r_grid[-1]
+            bottom = mesh.z_grid[0]
+            top = mesh.z_grid[-1]
+
+            slice_value = st.sidebar.slider(
+                label="slice index",
+                min_value=0,
+                max_value=len(mesh.phi_grid) - 1,
+                value=int(len(mesh.phi_grid) / 2),
+            )
 
-                # TODO add XY top down slice
-                # axis_to_slice = col1.selectbox(
-                #     label="Slice plane", options=("RZ", "XY"), index=0, key='ww_axis_to_slice'
-                # )
-                axis_to_slice = 'RZ'
+        elif isinstance(mesh, openmc.RegularMesh):
 
-                reshaped_tally = plotted_part_of_weight_window.reshape((mesh.dimension[2], mesh.dimension[1], mesh.dimension[0]), order="F")
+            reshaped_tally = plotted_part_of_weight_window.reshape(
+                mesh.dimension, order="F"
+            )
 
-                tally_aligned = reshaped_tally.transpose(2, 0, 1)
-                x_label = "R [cm]"
-                y_label = "Z [cm]"
+            axis_to_slice = st.sidebar.selectbox(
+                label="Slice plane",
+                options=("X", "Y", "Z"),
+                index=0,
+                key="ww_axis_to_slice",
+            )
 
-                left = mesh.r_grid[0]
-                right = mesh.r_grid[-1]
-                bottom = mesh.z_grid[0]
-                top = mesh.z_grid[-1]
-
-                slice_value = col1.slider(
-                    label="slice index",
-                    min_value=0,
-                    max_value=len(mesh.phi_grid) - 1,
-                    value=int(len(mesh.phi_grid) / 2),
-                )
+            if axis_to_slice == "X":
+                tally_aligned = reshaped_tally.transpose(1, 2, 0)
+                bb_index = 0
+                x_label = "Y [cm]"
+                y_label = "Z [cm]"
+            elif axis_to_slice == "Y":
+                tally_aligned = reshaped_tally.transpose(0, 1, 2)
+                bb_index = 1
+                x_label = "X [cm]"
+                y_label = "Z [cm]"
+            else:  # axis_to_slice == 'Z':
+                tally_aligned = reshaped_tally.transpose(2, 0, 1)
+                bb_index = 2
+                x_label = "X [cm]"
+                y_label = "Y [cm]"
+
+            left = mesh.lower_left[bb_index]
+            right = mesh.upper_right[bb_index]
+            bottom = mesh.lower_left[bb_index]
+            top = mesh.upper_right[bb_index]
+
+            slice_value = st.sidebar.slider(
+                label="slice index",
+                min_value=0,
+                max_value=len(tally_aligned) - 1,
+                value=int(len(tally_aligned) / 2),
+            )
 
-            elif isinstance(mesh, openmc.RegularMesh):
+        log_lin_scale = st.sidebar.radio(
+            "Normalization", options=["log", "linear"], key="ww_log_lin_scale"
+        )
+        if log_lin_scale == "linear":
+            norm = None
+        else:
+            norm = LogNorm()
 
-                reshaped_tally = plotted_part_of_weight_window.reshape(mesh.dimension, order="F")
+        image_slice = tally_aligned[slice_value]
 
-                axis_to_slice = col1.selectbox(
-                    label="Slice plane", options=("X", "Y", "Z"), index=0, key='ww_axis_to_slice'
-                )
+        if axis_to_slice == "Y":
+            image_slice = np.rot90(image_slice)
+        if axis_to_slice == "Z":
+            image_slice = np.rot90(image_slice)
+        if axis_to_slice == "X":
+            image_slice = np.flipud(image_slice)
+        # if axis_to_slice == "RZ":
+        #     image_slice = np.flipud(image_slice)
 
-                if axis_to_slice == "X":
-                    tally_aligned = reshaped_tally.transpose(1, 2, 0)
-                    bb_index = 0
-                    x_label = "Y [cm]"
-                    y_label = "Z [cm]"
-                elif axis_to_slice == "Y":
-                    tally_aligned = reshaped_tally.transpose(
-                        0, 1, 2
-                    )
-                    bb_index = 1
-                    x_label = "X [cm]"
-                    y_label = "Z [cm]"
-                else:  # axis_to_slice == 'Z':
-                    tally_aligned = reshaped_tally.transpose(2, 0, 1)
-                    bb_index = 2
-                    x_label = "X [cm]"
-                    y_label = "Y [cm]"
-
-                left = mesh.lower_left[bb_index]
-                right = mesh.upper_right[bb_index]
-                bottom = mesh.lower_left[bb_index]
-                top = mesh.upper_right[bb_index]
-
-                slice_value = col1.slider(
-                    label="slice index",
-                    min_value=0,
-                    max_value=len(tally_aligned) - 1,
-                    value=int(len(tally_aligned) / 2),
-                )
+        plt.cla()
+        plt.clf()
 
-            log_lin_scale = col1.radio(
-                "Normalization", options=["log", "linear"],
-                key='ww_log_lin_scale')
-            if log_lin_scale == "linear":
-                norm = None
-            else:
-                norm = LogNorm()
-
-            image_slice = tally_aligned[slice_value]
-
-            if axis_to_slice == "Y":
-                image_slice = np.rot90(image_slice)
-            if axis_to_slice == "Z":
-                image_slice = np.rot90(image_slice)
-            if axis_to_slice == "X":
-                image_slice = np.flipud(image_slice)
-            # if axis_to_slice == "RZ":
-            #     image_slice = np.flipud(image_slice)
-
-            plt.cla()
-            plt.clf()
-
-            plt.axes(title=f"Weight window {upper_or_lower}", xlabel=x_label, ylabel=y_label)
-            # could be assigned like this
-            # plt.xlabel(x_label)
-            # plt.ylabel(y_label)
-            # plt.title('Tally value')
-            if np.amax(image_slice) == np.amin(image_slice) and norm is not None:
-                msg = "slice contains the uniform values, can't be plotted on log scale"
-                format = f'<p style="font-family:sans-serif; color:Red; font-size: 30px;">{msg}</p>'
-                col2.markdown(format, unsafe_allow_html=True)
-            else:
-                plt.imshow(
-                    X=image_slice,
-                    extent=(left, right, bottom, top),
-                    norm=norm
+        plt.axes(
+            title=f"Weight window {upper_or_lower}", xlabel=x_label, ylabel=y_label
+        )
+        # could be assigned like this
+        # plt.xlabel(x_label)
+        # plt.ylabel(y_label)
+        # plt.title('Tally value')
+        if np.amax(image_slice) == np.amin(image_slice) and norm is not None:
+            msg = "slice contains the uniform values, can't be plotted on log scale"
+            format = f'<p style="font-family:sans-serif; color:Red; font-size: 30px;">{msg}</p>'
+            st.markdown(format, unsafe_allow_html=True)
+        else:
+            plt.imshow(X=image_slice, extent=(left, right, bottom, top), norm=norm)
+            plt.colorbar(label=upper_or_lower)
+            st.pyplot(plt)
+            plt.savefig("openmc_plot_weightwindow_image.png")
+
+            with open("openmc_plot_weightwindow_image.png", "rb") as file:
+                st.sidebar.download_button(
+                    label="Download image",
+                    data=file,
+                    file_name="openmc_plot_weightwindow_image.png",
+                    mime="image/png",
                 )
-                plt.colorbar(label=upper_or_lower)
-                col2.pyplot(plt)
-                plt.savefig("openmc_plot_weightwindow_image.png")
-
-                with open("openmc_plot_weightwindow_image.png", "rb") as file:
-                    col1.download_button(
-                        label="Download image",
-                        data=file,
-                        file_name="openmc_plot_weightwindow_image.png",
-                        mime="image/png"
-                    )
```

### Comparing `openmc_plot-0.2.2/src/openmc_plot.egg-info/PKG-INFO` & `openmc_plot-0.3.0/src/openmc_plot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc-plot
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Python package containing a collection of scripts for producing and downloading data for OpenMC
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 License: MIT License
         
         Copyright (c) 2022 Fusion Energy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,17 +32,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
-A Python app for plotting OpenMC geometry.
+A Python app for plotting OpenMC.
 
-This repository contains part of the source code for the OpenMC geometry plotting app which is part of the website [xsplot.com](http://xsplot.com)
+This repository contains the source code for the OpenMC plot.
+
+Try the web app at [http://openmc-plot.xsplot.com](http://openmc-plot.xsplot.com)
 
 This repository contains:
 - A Python [Streamlit](https://streamlit.io) based GUI 🐍
 - A Dockerfile that provides the hosting environment for the web app 🐳
 
 # Plot geometry
 ![openmc plot geometry](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/d/d7bcce794d51d34381371fc991c0e1ff2a65df08.gif)
@@ -54,15 +56,17 @@
 ![openmc plot mesh](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/2/24a9db7bc9cc227908dbaf13a54d1245a4d16f20.gif)
 
 # Plot weight windows
 ![openmc plot mesh](https://canada1.discourse-cdn.com/free1/uploads/openmc/original/2X/1/114aeb91172c7577e9231ffe30edf141678d26f6.gif)
 
 # Install
 
-OpenMC_plot can be install directly from the Python package index (PyPi) using pip.
+First you will need to [install OpenMC](https://docs.openmc.org/en/stable/quickinstall.html)
+
+OpenMC_plot can then be install directly from the Python package index (PyPi) using pip.
 
 ```
 pip install openmc_plot
 ```
 
 # Usage
 
@@ -74,16 +78,14 @@
 
 Your default web browser should then load with the GUI.
 
 You will also need to have [OpenMC installed](https://docs.openmc.org/en/stable/quickinstall.html).
 
 # Run web app locally (developers)
 
-You can view the hosted version of this repository here [xsplot.com](http://xsplot.com). However you might want to host your own version locally.
-
 To host your own local version of [xsplot.com](http://xsplot.com) you will need [Docker](https://www.docker.com/) installed and then can build and run the Dockerfile
 with the following commands.
 
 First clone the repository
 ```bash
 git clone https://github.com/fusion-energy/openmc_plot
 ```
```

### Comparing `openmc_plot-0.2.2/src/openmc_plot.egg-info/SOURCES.txt` & `openmc_plot-0.3.0/src/openmc_plot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 examples/tokamak/settings_multiple_sources.xml
 examples/tokamak/summary.h5
 examples/weightwindows/settings.xml
 src/openmc_plot/__init__.py
 src/openmc_plot/_version.py
 src/openmc_plot/app.py
 src/openmc_plot/cross_sections.xml
-src/openmc_plot/dagmcslice_tab.py
-src/openmc_plot/geometry_tab.py
-src/openmc_plot/header.py
 src/openmc_plot/launch.py
-src/openmc_plot/regularmesh_tab.py
-src/openmc_plot/source_tab.py
 src/openmc_plot/utils.py
-src/openmc_plot/weightwindows_tab.py
 src/openmc_plot.egg-info/PKG-INFO
 src/openmc_plot.egg-info/SOURCES.txt
 src/openmc_plot.egg-info/dependency_links.txt
 src/openmc_plot.egg-info/entry_points.txt
 src/openmc_plot.egg-info/requires.txt
-src/openmc_plot.egg-info/top_level.txt
+src/openmc_plot.egg-info/top_level.txt
+src/openmc_plot/pages/1_🖼_Geometry_plot.py
+src/openmc_plot/pages/2_🧊_Regular_mesh_plot.py
+src/openmc_plot/pages/3_✴️_Source_plot.py
+src/openmc_plot/pages/4_🪟_Weight_window_plot.py
+src/openmc_plot/pages/5_🍕_DAGMC_slice_plot.py
+src/openmc_plot/pages/dagmc.h5m
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

