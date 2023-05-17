# Comparing `tmp/brainlit-0.3.4.tar.gz` & `tmp/brainlit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainlit-0.3.4.tar", last modified: Tue May  9 16:47:48 2023, max compression
+gzip compressed data, was "/Users/thomasathey/Documents/mimlab/mouselight/brainlit_parent/brainlit/dist/.tmp-fs6lmyuz/brainlit-0.3.5.tar", last modified: Wed May 17 23:42:14 2023, max compression
```

## Comparing `brainlit-0.3.4.tar` & `brainlit-0.3.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.905185 brainlit-0.3.4/
--rw-r--r--   0 thomasathey   (501) staff       (20)    11358 2020-10-26 19:40:08.000000 brainlit-0.3.4/LICENSE
--rw-r--r--   0 thomasathey   (501) staff       (20)     3056 2023-05-09 16:47:48.904580 brainlit-0.3.4/PKG-INFO
--rw-r--r--   0 thomasathey   (501) staff       (20)     2262 2023-05-09 16:45:44.000000 brainlit-0.3.4/README.md
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.878351 brainlit-0.3.4/brainlit/
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.883953 brainlit-0.3.4/brainlit/BrainLine/
--rw-r--r--   0 thomasathey   (501) staff       (20)      346 2023-04-26 12:32:15.000000 brainlit-0.3.4/brainlit/BrainLine/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    44207 2023-05-09 16:45:47.000000 brainlit-0.3.4/brainlit/BrainLine/analyze_results.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    28417 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/BrainLine/apply_ilastik.py
--rw-r--r--   0 thomasathey   (501) staff       (20)      394 2023-04-12 15:04:36.000000 brainlit-0.3.4/brainlit/BrainLine/imports.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     3778 2023-04-12 15:04:36.000000 brainlit-0.3.4/brainlit/BrainLine/parse_ara.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    10975 2023-05-02 20:53:23.000000 brainlit-0.3.4/brainlit/BrainLine/util.py
--rw-r--r--   0 thomasathey   (501) staff       (20)      385 2023-05-09 16:46:16.000000 brainlit-0.3.4/brainlit/__init__.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.884356 brainlit-0.3.4/brainlit/algorithms/
--rw-r--r--   0 thomasathey   (501) staff       (20)      394 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/algorithms/__init__.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.885889 brainlit-0.3.4/brainlit/algorithms/connect_fragments/
--rw-r--r--   0 thomasathey   (501) staff       (20)      231 2022-03-16 13:30:15.000000 brainlit-0.3.4/brainlit/algorithms/connect_fragments/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     2239 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/algorithms/connect_fragments/trace_evaluation.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    18206 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/algorithms/connect_fragments/viterbrain.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.887230 brainlit-0.3.4/brainlit/algorithms/detect_somas/
--rw-r--r--   0 thomasathey   (501) staff       (20)       54 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/algorithms/detect_somas/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     5191 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/algorithms/detect_somas/detect.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.888954 brainlit-0.3.4/brainlit/algorithms/generate_fragments/
--rwxr-xr-x   0 thomasathey   (501) staff       (20)      132 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/algorithms/generate_fragments/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    31716 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/algorithms/generate_fragments/state_generation.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     6158 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/algorithms/generate_fragments/tube_seg.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.890488 brainlit-0.3.4/brainlit/algorithms/trace_analysis/
--rwxr-xr-x   0 thomasathey   (501) staff       (20)      121 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/algorithms/trace_analysis/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    17453 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/algorithms/trace_analysis/fit_spline.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    11686 2022-03-16 13:30:15.000000 brainlit-0.3.4/brainlit/algorithms/trace_analysis/spline_fxns.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.892177 brainlit-0.3.4/brainlit/feature_extraction/
--rw-r--r--   0 thomasathey   (501) staff       (20)       55 2020-10-26 19:40:08.000000 brainlit-0.3.4/brainlit/feature_extraction/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    12440 2023-04-03 18:41:18.000000 brainlit-0.3.4/brainlit/feature_extraction/base.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     3332 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/feature_extraction/neighborhood.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.893273 brainlit-0.3.4/brainlit/map_neurons/
--rw-r--r--   0 thomasathey   (501) staff       (20)       92 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/map_neurons/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    19224 2023-05-05 16:56:46.000000 brainlit-0.3.4/brainlit/map_neurons/map_neurons.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.894038 brainlit-0.3.4/brainlit/napari_viterbrain/
--rw-r--r--   0 thomasathey   (501) staff       (20)     2049 2023-04-03 21:17:17.000000 brainlit-0.3.4/brainlit/napari_viterbrain/viterbrain_plugin.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.896267 brainlit-0.3.4/brainlit/preprocessing/
--rw-r--r--   0 thomasathey   (501) staff       (20)       99 2020-10-26 19:40:08.000000 brainlit-0.3.4/brainlit/preprocessing/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    22539 2023-04-07 13:39:56.000000 brainlit-0.3.4/brainlit/preprocessing/image_process.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     8614 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/preprocessing/preprocess.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.902051 brainlit-0.3.4/brainlit/utils/
--rwxr-xr-x   0 thomasathey   (501) staff       (20)    42070 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/utils/Neuron_trace.py
--rw-r--r--   0 thomasathey   (501) staff       (20)      232 2023-03-01 16:17:04.000000 brainlit-0.3.4/brainlit/utils/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     3021 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/utils/benchmarking_params.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    15886 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/utils/session.py
--rw-r--r--   0 thomasathey   (501) staff       (20)    20173 2023-04-03 21:17:17.000000 brainlit-0.3.4/brainlit/utils/upload.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     2514 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/utils/util.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     7017 2023-05-09 16:45:44.000000 brainlit-0.3.4/brainlit/utils/write.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.903686 brainlit-0.3.4/brainlit/viz/
--rw-r--r--   0 thomasathey   (501) staff       (20)       37 2022-01-31 22:42:20.000000 brainlit-0.3.4/brainlit/viz/__init__.py
--rw-r--r--   0 thomasathey   (501) staff       (20)     7752 2023-01-02 19:42:55.000000 brainlit-0.3.4/brainlit/viz/swc2voxel.py
-drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-09 16:47:48.881456 brainlit-0.3.4/brainlit.egg-info/
--rw-r--r--   0 thomasathey   (501) staff       (20)     3056 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/PKG-INFO
--rw-r--r--   0 thomasathey   (501) staff       (20)     1616 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/SOURCES.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)        1 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/dependency_links.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)       68 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/entry_points.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)      325 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/requires.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)        9 2023-05-09 16:47:48.000000 brainlit-0.3.4/brainlit.egg-info/top_level.txt
--rw-r--r--   0 thomasathey   (501) staff       (20)       38 2023-05-09 16:47:48.905373 brainlit-0.3.4/setup.cfg
--rw-r--r--   0 thomasathey   (501) staff       (20)     2699 2023-05-02 20:53:23.000000 brainlit-0.3.4/setup.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.535737 brainlit-0.3.5/
+-rw-r--r--   0 thomasathey   (501) staff       (20)    11358 2020-10-26 19:40:08.000000 brainlit-0.3.5/LICENSE
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3056 2023-05-17 23:42:14.535140 brainlit-0.3.5/PKG-INFO
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2262 2023-05-17 15:41:43.000000 brainlit-0.3.5/README.md
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.501025 brainlit-0.3.5/brainlit/
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.510645 brainlit-0.3.5/brainlit/BrainLine/
+-rw-r--r--   0 thomasathey   (501) staff       (20)      346 2023-04-26 12:32:15.000000 brainlit-0.3.5/brainlit/BrainLine/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    44707 2023-05-17 15:41:43.000000 brainlit-0.3.5/brainlit/BrainLine/analyze_results.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    30859 2023-05-17 18:40:37.000000 brainlit-0.3.5/brainlit/BrainLine/apply_ilastik.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)      394 2023-04-12 15:04:36.000000 brainlit-0.3.5/brainlit/BrainLine/imports.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3778 2023-04-12 15:04:36.000000 brainlit-0.3.5/brainlit/BrainLine/parse_ara.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    10939 2023-05-17 15:41:43.000000 brainlit-0.3.5/brainlit/BrainLine/util.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)      385 2023-05-17 23:42:05.000000 brainlit-0.3.5/brainlit/__init__.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.511409 brainlit-0.3.5/brainlit/algorithms/
+-rw-r--r--   0 thomasathey   (501) staff       (20)      394 2022-01-31 22:42:20.000000 brainlit-0.3.5/brainlit/algorithms/__init__.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.513905 brainlit-0.3.5/brainlit/algorithms/connect_fragments/
+-rw-r--r--   0 thomasathey   (501) staff       (20)      231 2022-03-16 13:30:15.000000 brainlit-0.3.5/brainlit/algorithms/connect_fragments/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2239 2023-01-02 19:42:55.000000 brainlit-0.3.5/brainlit/algorithms/connect_fragments/trace_evaluation.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    18206 2023-05-17 22:04:25.000000 brainlit-0.3.5/brainlit/algorithms/connect_fragments/viterbrain.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.515393 brainlit-0.3.5/brainlit/algorithms/detect_somas/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       54 2022-01-31 22:42:20.000000 brainlit-0.3.5/brainlit/algorithms/detect_somas/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     5191 2022-01-31 22:42:20.000000 brainlit-0.3.5/brainlit/algorithms/detect_somas/detect.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.517914 brainlit-0.3.5/brainlit/algorithms/generate_fragments/
+-rwxr-xr-x   0 thomasathey   (501) staff       (20)      132 2023-01-02 19:42:55.000000 brainlit-0.3.5/brainlit/algorithms/generate_fragments/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    31716 2023-05-17 22:04:25.000000 brainlit-0.3.5/brainlit/algorithms/generate_fragments/state_generation.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     6158 2023-01-02 19:42:55.000000 brainlit-0.3.5/brainlit/algorithms/generate_fragments/tube_seg.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.520281 brainlit-0.3.5/brainlit/algorithms/trace_analysis/
+-rwxr-xr-x   0 thomasathey   (501) staff       (20)      121 2022-01-31 22:42:20.000000 brainlit-0.3.5/brainlit/algorithms/trace_analysis/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    17453 2023-05-11 21:46:11.000000 brainlit-0.3.5/brainlit/algorithms/trace_analysis/fit_spline.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    11686 2022-03-16 13:30:15.000000 brainlit-0.3.5/brainlit/algorithms/trace_analysis/spline_fxns.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.522634 brainlit-0.3.5/brainlit/feature_extraction/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       55 2020-10-26 19:40:08.000000 brainlit-0.3.5/brainlit/feature_extraction/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    12440 2023-04-03 18:41:18.000000 brainlit-0.3.5/brainlit/feature_extraction/base.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3332 2022-01-31 22:42:20.000000 brainlit-0.3.5/brainlit/feature_extraction/neighborhood.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.524176 brainlit-0.3.5/brainlit/map_neurons/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       92 2023-05-16 14:07:12.000000 brainlit-0.3.5/brainlit/map_neurons/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    19224 2023-05-17 15:12:50.000000 brainlit-0.3.5/brainlit/map_neurons/map_neurons.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.525109 brainlit-0.3.5/brainlit/napari_viterbrain/
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2049 2023-05-17 22:04:24.000000 brainlit-0.3.5/brainlit/napari_viterbrain/viterbrain_plugin.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.527606 brainlit-0.3.5/brainlit/preprocessing/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       99 2020-10-26 19:40:08.000000 brainlit-0.3.5/brainlit/preprocessing/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    22539 2023-04-07 13:39:56.000000 brainlit-0.3.5/brainlit/preprocessing/image_process.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     8614 2023-01-02 19:42:55.000000 brainlit-0.3.5/brainlit/preprocessing/preprocess.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.532821 brainlit-0.3.5/brainlit/utils/
+-rwxr-xr-x   0 thomasathey   (501) staff       (20)    42070 2023-05-16 14:07:12.000000 brainlit-0.3.5/brainlit/utils/Neuron_trace.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)      232 2023-03-01 16:17:04.000000 brainlit-0.3.5/brainlit/utils/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3021 2022-01-31 22:42:20.000000 brainlit-0.3.5/brainlit/utils/benchmarking_params.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    15886 2023-05-17 15:41:43.000000 brainlit-0.3.5/brainlit/utils/session.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)    20173 2023-05-17 22:04:25.000000 brainlit-0.3.5/brainlit/utils/upload.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2514 2023-01-02 19:42:55.000000 brainlit-0.3.5/brainlit/utils/util.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     7017 2023-05-17 15:41:43.000000 brainlit-0.3.5/brainlit/utils/write.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.534276 brainlit-0.3.5/brainlit/viz/
+-rw-r--r--   0 thomasathey   (501) staff       (20)       37 2022-01-31 22:42:20.000000 brainlit-0.3.5/brainlit/viz/__init__.py
+-rw-r--r--   0 thomasathey   (501) staff       (20)     7752 2023-01-02 19:42:55.000000 brainlit-0.3.5/brainlit/viz/swc2voxel.py
+drwxr-xr-x   0 thomasathey   (501) staff       (20)        0 2023-05-17 23:42:14.505834 brainlit-0.3.5/brainlit.egg-info/
+-rw-r--r--   0 thomasathey   (501) staff       (20)     3056 2023-05-17 23:42:14.000000 brainlit-0.3.5/brainlit.egg-info/PKG-INFO
+-rw-r--r--   0 thomasathey   (501) staff       (20)     1616 2023-05-17 23:42:14.000000 brainlit-0.3.5/brainlit.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)        1 2023-05-17 23:42:14.000000 brainlit-0.3.5/brainlit.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)       68 2023-05-17 23:42:14.000000 brainlit-0.3.5/brainlit.egg-info/entry_points.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)      357 2023-05-17 23:42:14.000000 brainlit-0.3.5/brainlit.egg-info/requires.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)        9 2023-05-17 23:42:14.000000 brainlit-0.3.5/brainlit.egg-info/top_level.txt
+-rw-r--r--   0 thomasathey   (501) staff       (20)       38 2023-05-17 23:42:14.535921 brainlit-0.3.5/setup.cfg
+-rw-r--r--   0 thomasathey   (501) staff       (20)     2745 2023-05-17 22:45:31.000000 brainlit-0.3.5/setup.py
```

### Comparing `brainlit-0.3.4/LICENSE` & `brainlit-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/PKG-INFO` & `brainlit-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainlit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Code to process and analyze brainlit data
 Home-page: https://github.com/neurodata/brainlit
 Author: ('Thomas Athey, Bijan Varjivand, Ryan Lu, Matt Figdore, Alex Fiallos, Stanley Wang, Victor Wang',)
 Author-email: tathey1@jhu.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `brainlit-0.3.4/README.md` & `brainlit-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/BrainLine/analyze_results.py` & `brainlit-0.3.5/brainlit/BrainLine/analyze_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from statannotations.stats.StatTest import StatTest
 from statannotations import stats
 import pandas as pd
 import matplotlib.pyplot as plt
 import os
 from joblib import Parallel, delayed
 import pickle
+import brainrender
 from brainrender import Scene
 from brainrender.actors import Points, Volume
 import json
 from cloudvolume.exceptions import OutOfBoundsError
 
 
 class BrainDistribution:
@@ -278,14 +279,15 @@
         Args:
             subtype_colors (_type_): Mapping of subtypes (in soma_data.py file) to colors for soma plotting.
             brain_region (str, optional): Brain region to display with the detections (e.g. dorsal raphe nucleus). Defaults to "DR".
         """
         brain_ids = self.brain_ids
         brain2paths = self.brain2paths
 
+        brainrender.settings.WHOLE_SCREEN = False
         scene = Scene(atlas_name="allen_mouse_50um", title="Input Somas")
         scene.add_brain_region(brain_region, alpha=0.15)
 
         for brain_id in brain_ids:
             viz_link = brain2paths[brain_id]["somas_atlas_url"]
             viz_link = NGLink(viz_link.split("json_url=")[-1])
             ngl_json = viz_link._json
@@ -585,17 +587,26 @@
     group_data1_log = np.log(group_data1)
     group_data2_log = np.log(group_data2)
 
     return ttest_ind(group_data1_log, group_data2_log, **stats_params)
 
 
 def _get_corners_collection(
-    vol_mask, vol_reg, block_size, max_coords: list = [-1, -1, -1]
+    vol_mask,
+    vol_reg,
+    block_size,
+    max_coords: list = [-1, -1, -1],
+    min_coords: list = [-1, -1, -1],
 ):
-    corners = _get_corners(vol_mask.shape, chunk_size=block_size, max_coords=max_coords)
+    corners = _get_corners(
+        vol_mask.shape,
+        chunk_size=block_size,
+        max_coords=max_coords,
+        min_coords=min_coords,
+    )
 
     new_corners = []
     for corner in corners:
         x = corner[0][0]
         x2 = corner[1][0]
         x_reg = int(x / 8)
         x2_reg = np.amin([int(x2 / 8), vol_reg.shape[0]])
@@ -677,24 +688,26 @@
 
 
 def collect_regional_segmentation(
     brain_id: str,
     data_file: str,
     outdir: str,
     ncpu: int = 1,
+    min_coords: list = [-1, -1, -1],
     max_coords: list = [-1, -1, -1],
 ):
     """Combine segmentation and registration to generate counts of axon voxels across brain regions. Note this scripts writes a file for every chunk, which might be many.
 
     Args:
         brain_id (str): Brain ID to process, from axon_data.py
         data_file (str): path to json file with data information.
         outdir (str): Path to directory to write files.
         ncpu (int, optional): Number of cpus to use for parallel processing. Defaults to 1.
-        max_coords (list, optional): Upper limits of brain to complete processing, -1 will lead to processing the whole axis. Defaults to [-1, -1, -1].
+        min_coords (list, optional): Lower limits of brain to complete processing, -1 will lead to processing from the beginning of the axis. Defaults to [-1, -1, -1].
+        max_coords (list, optional): Upper limits of brain to complete processing, -1 will lead to processing to the end of the axis. Defaults to [-1, -1, -1].
     """
     with open(data_file) as f:
         data = json.load(f)
     brain2paths = data["brain2paths"]
     dir_base = brain2paths[brain_id]["base"]
 
     dir = os.path.join(dir_base, "axon_mask")
@@ -702,15 +715,19 @@
     print(f"Mask shape: {vol_mask.shape}")
 
     dir = os.path.join(dir_base, "atlas_to_target")
     vol_reg = CloudVolume(dir, parallel=1, mip=0, fill_missing=True)
     print(f"Atlas shape: {vol_reg.shape}")
 
     corners = _get_corners_collection(
-        vol_mask, vol_reg, block_size=[256, 256, 256], max_coords=max_coords
+        vol_mask,
+        vol_reg,
+        block_size=[100, 100, 100],
+        max_coords=max_coords,
+        min_coords=min_coords,
     )
     Parallel(n_jobs=ncpu)(
         delayed(_compute_composition_corner)(corner, outdir, dir_base)
         for corner in tqdm(corners, desc="Finding labels")
     )
 
     volumes = _combine_regional_segmentations(outdir)
@@ -882,14 +899,15 @@
 
         Args:
             subtype_colors (dict): Mapping of subtype to color to be used in visualization.
         """
         brain_ids = self.brain_ids
         brain2paths = self.brain2paths
 
+        brainrender.settings.WHOLE_SCREEN = False
         scene = Scene(atlas_name="allen_mouse_50um", title="Input Somas")
         scene.add_brain_region(brain_region, alpha=0.15)
 
         for subtype in subtype_colors.keys():
             im_total = None
             for i, brain_id in enumerate(brain_ids):
                 if brain2paths[brain_id]["subtype"] == subtype:
```

### Comparing `brainlit-0.3.4/brainlit/BrainLine/apply_ilastik.py` & `brainlit-0.3.5/brainlit/BrainLine/apply_ilastik.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 import shutil
 from tqdm import tqdm
 import subprocess
 from joblib import Parallel, delayed
 import multiprocessing
 from brainlit.BrainLine.util import _find_sample_names, _get_corners
 from datetime import date
-from cloudvolume import CloudVolume, exceptions
+from cloudvolume import CloudVolume, exceptions, Bbox
 import numpy as np
 import h5py
 from skimage import io, measure
 from pathlib import Path
 from os.path import isfile, join
 from os import listdir
 import random
 from cloudreg.scripts.transform_points import NGLink
 from cloudreg.scripts.visualization import create_viz_link_from_json
 import pandas as pd
 from brainlit.BrainLine.imports import *
 import json
 from typing import Union
+import igneous.task_creation as tc
+from taskqueue import LocalTaskQueue
 
 
 class ApplyIlastik:
     """Applies ilastik to subvolumes for the purpose of validating machine learning algorithms.
 
     Arguments:
         ilastk_path (str): Path to ilastik executable.
@@ -56,24 +58,27 @@
                     f"--project={self.project_path}",
                     fname,
                 ],
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
             )
 
-    def process_subvols(self):
-        """Apply ilastik to all validation subvolumes of the specified brain ids in the specified directory"""
+    def process_subvols(self, ncpu: int = 6):
+        """Apply ilastik to all validation subvolumes of the specified brain ids in the specified directory
+
+        Args:
+            ncpu (int, optional): Number of cpus to use for segmentation. Defaults to 6.
+        """
         items_total = []
         for brain in tqdm(self.brains, desc="Gathering brains..."):
             path = f"{self.brains_path}brain{brain}/val/"
 
             items_total += _find_sample_names(path, dset="", add_dir=True)
 
-        # run all files
-        Parallel(n_jobs=8)(
+        Parallel(n_jobs=ncpu)(
             delayed(self._apply_ilastik)(item)
             for item in tqdm(items_total, desc="running ilastik...")
         )
 
     def move_results(self):
         """Move results from process_subvols to a new subfolder."""
         for brain in tqdm(self.brains, desc="Moving results"):
@@ -439,27 +444,27 @@
     def apply_ilastik_parallel(
         self,
         brain_id: str,
         layer_names: list,
         threshold: float,
         data_dir: str,
         chunk_size: list,
-        max_coords: list = [-1, -1, -1],
         min_coords: list = [-1, -1, -1],
+        max_coords: list = [-1, -1, -1],
     ):
         """Apply ilastik to large brain, in parallel.
 
         Args:
             brain_id (str): Brain ID (key in brain2paths in _data.py file).
             layer_names (list): Precomputed layer names to be appended to the base path.
             threshold (float): Threshold for the ilastik predictor.
             data_dir (str or Path): Path to directory where downloaded data will be temporarily stored.
             chunk_size (list): Size of chunks to be used for parallel application of ilastik.
+            min_coords (list, optional): Lower bound of bounding box on which to apply ilastk (i.e. does not apply ilastik before these bounds). Defaults to [-1, -1, -1].
             max_coords (list, optional): Upper bound of bounding box on which to apply ilastk (i.e. does not apply ilastik beyond these bounds). Defaults to [-1, -1, -1].
-            min_coords (list, optional): Lower bound of bounding box on which to apply ilastk (i.e. does not apply ilastik beyond these bounds). Defaults to [-1, -1, -1].
         """
         results_dir = self.results_dir
         volume_base_dir = self.brain2paths[brain_id]["base"]
         sample_path = volume_base_dir + layer_names[0]
         vol = CloudVolume(sample_path, parallel=True, mip=0, fill_missing=True)
         shape = vol.shape
         print(f"Processing: {sample_path} with shape {shape} at threshold {threshold}")
@@ -483,21 +488,20 @@
             else:
                 print(f"Downloaded data will be stored in {results_dir}")
         elif self.object_type == "axon":
             mask_dir = volume_base_dir + "axon_mask"
             try:
                 CloudVolume(mask_dir)
             except:
-                self._make_mask_info(mask_dir, vol)
+                self._make_mask_info(mask_dir, vol, chunk_size)
 
         corners = _get_corners(
             shape, chunk_size, max_coords=max_coords, min_coords=min_coords
         )
         corners_chunks = [corners[i : i + 100] for i in range(0, len(corners), 100)]
-
         for corners_chunk in tqdm(corners_chunks, desc="corner chunks"):
             Parallel(n_jobs=self.ncpu)(
                 delayed(self._process_chunk)(
                     corner[0],
                     corner[1],
                     volume_base_dir,
                     layer_names,
@@ -507,26 +511,26 @@
                     results_dir,
                 )
                 for corner in tqdm(corners_chunk, leave=False)
             )
             for f in os.listdir(data_dir):
                 os.remove(os.path.join(data_dir, f))
 
-    def _make_mask_info(self, mask_dir: str, vol: CloudVolume):
+    def _make_mask_info(self, mask_dir: str, vol: CloudVolume, chunk_size: list):
         info = CloudVolume.create_new_info(
             num_channels=1,
             layer_type="segmentation",
             data_type="uint64",  # Channel images might be 'uint8'
             encoding="raw",  # raw, jpeg, compressed_segmentation, fpzip, kempressed
             resolution=vol.resolution,  # Voxel scaling, units are in nanometers
             voxel_offset=vol.voxel_offset,  # x,y,z offset in voxels from the origin
             # mesh            = 'mesh',
             # Pick a convenient size for your underlying chunk representation
             # Powers of two are recommended, doesn't need to cover image exactly
-            chunk_size=(128, 128, 2),  # units are voxels
+            chunk_size=chunk_size,  # units are voxels
             volume_size=vol.volume_size,  # e.g. a cubic millimeter dataset
         )
         vol_mask = CloudVolume(mask_dir, info=info, compress=False)
         vol_mask.commit_info()
 
     def _process_chunk(
         self,
@@ -622,14 +626,15 @@
         results_dir = self.results_dir
         onlyfiles = [
             join(results_dir, f)
             for f in listdir(results_dir)
             if isfile(join(results_dir, f))
         ]
         onlyfiles = [f for f in onlyfiles if ".txt" in f]
+        onlyfiles = [f for f in onlyfiles if "all_somas" not in f]
         div_factor = [8, 8, 1]
         for file in tqdm(onlyfiles, desc="reading files"):
             print(file)
             file1 = open(file, "r")
             lines = file1.readlines()
 
             for line in tqdm(lines, desc="parsing coordinates", leave=False):
@@ -707,7 +712,54 @@
                 )
                 break
         print(ngl_json)
         viz_link = create_viz_link_from_json(
             ngl_json, neuroglancer_link="https://viz.neurodata.io/?json_url="
         )
         print(f"Viz link with segmentation: {viz_link}")
+
+
+def downsample_mask(brain, data_file, ncpu: int = 1, bounds: list = None):
+    """Use Igneous pipeline to downsample new axon_mask segmentation. Necessary to transform the mask into atlas space.
+
+    Args:
+        brain (str): ID key whose axon_mask will be downsampled.
+        data_file (str): Path to data JSON.
+        ncpu (int, optional): Number of cores to use for downsampling. Defaults to 1.
+        bounds (list, optional): List of two lists of length 3 specifying corners of bounding box to restrict downsampling to. Defaults to None.
+
+    Raises:
+        ValueError: _description_
+    """
+    with open(data_file) as f:
+        data = json.load(f)
+    object_type = data["object_type"]
+    brain2paths = data["brain2paths"]
+    if object_type != "axon":
+        raise ValueError(f"Entered non-axon data file")
+    dir_base = brain2paths[brain]["base"]
+    layer_path = dir_base + "axon_mask"
+
+    tq = LocalTaskQueue(parallel=ncpu)
+
+    if bounds != None:
+        bounds = Bbox(bounds[0], bounds[1])
+
+    tasks = tc.create_downsampling_tasks(
+        layer_path,  # e.g. 'gs://bucket/dataset/layer'
+        mip=0,  # Start downsampling from this mip level (writes to next level up)
+        fill_missing=True,  # Ignore missing chunks and fill them with black
+        axis="z",
+        num_mips=2,  # number of downsamples to produce. Downloaded shape is chunk_size * 2^num_mip
+        chunk_size=None,  # manually set chunk size of next scales, overrides preserve_chunk_size
+        preserve_chunk_size=True,  # use existing chunk size, don't halve to get more downsamples
+        sparse=False,  # for sparse segmentation, allow inflation of pixels against background
+        bounds=bounds,  # mip 0 bounding box to downsample
+        encoding=None,  # e.g. 'raw', 'compressed_segmentation', etc
+        delete_black_uploads=True,  # issue a delete instead of uploading files containing all background
+        background_color=0,  # Designates the background color
+        compress="gzip",  # None, 'gzip', and 'br' (brotli) are options
+        factor=(2, 2, 2),  # common options are (2,2,1) and (2,2,2)
+    )
+
+    tq.insert(tasks)
+    tq.execute()
```

### Comparing `brainlit-0.3.4/brainlit/BrainLine/parse_ara.py` & `brainlit-0.3.5/brainlit/BrainLine/parse_ara.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/BrainLine/util.py` & `brainlit-0.3.5/brainlit/BrainLine/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import json
 import numpy as np
 import os
 import networkx as nx
 from pathlib import Path
 from brainlit.BrainLine.parse_ara import build_tree
 from tqdm import tqdm
-from brainlit.BrainLine import data
 from brainlit.BrainLine.imports import *
 import json
 
 
 def download_subvolumes(
     data_dir: str,
     brain_id: str,
@@ -112,15 +111,15 @@
                 / f"{int(center[0])}_{int(center[1])}_{int(center[2])}{suffix}.h5"
             )
             with h5py.File(fname, "w") as f:
                 dset = f.create_dataset("image_3channel", data=image)
 
 
 def _get_corners(
-    shape, chunk_size, max_coords: list = [-1, -1, -1], min_coords: list = [-1, -1, -1]
+    shape, chunk_size, min_coords: list = [-1, -1, -1], max_coords: list = [-1, -1, -1]
 ):
     corners = []
     for i in tqdm(range(0, shape[0], chunk_size[0])):
         for j in tqdm(range(0, shape[1], chunk_size[1]), leave=False):
             for k in range(0, shape[2], chunk_size[2]):
                 c1 = [i, j, k]
                 c2 = [
```

### Comparing `brainlit-0.3.4/brainlit/algorithms/connect_fragments/trace_evaluation.py` & `brainlit-0.3.5/brainlit/algorithms/connect_fragments/trace_evaluation.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/algorithms/connect_fragments/viterbrain.py` & `brainlit-0.3.5/brainlit/algorithms/connect_fragments/viterbrain.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/algorithms/detect_somas/detect.py` & `brainlit-0.3.5/brainlit/algorithms/detect_somas/detect.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/algorithms/generate_fragments/state_generation.py` & `brainlit-0.3.5/brainlit/algorithms/generate_fragments/state_generation.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/algorithms/generate_fragments/tube_seg.py` & `brainlit-0.3.5/brainlit/algorithms/generate_fragments/tube_seg.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/algorithms/trace_analysis/fit_spline.py` & `brainlit-0.3.5/brainlit/algorithms/trace_analysis/fit_spline.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/algorithms/trace_analysis/spline_fxns.py` & `brainlit-0.3.5/brainlit/algorithms/trace_analysis/spline_fxns.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/feature_extraction/base.py` & `brainlit-0.3.5/brainlit/feature_extraction/base.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/feature_extraction/neighborhood.py` & `brainlit-0.3.5/brainlit/feature_extraction/neighborhood.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/map_neurons/map_neurons.py` & `brainlit-0.3.5/brainlit/map_neurons/map_neurons.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/napari_viterbrain/viterbrain_plugin.py` & `brainlit-0.3.5/brainlit/napari_viterbrain/viterbrain_plugin.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/preprocessing/image_process.py` & `brainlit-0.3.5/brainlit/preprocessing/image_process.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/preprocessing/preprocess.py` & `brainlit-0.3.5/brainlit/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/utils/Neuron_trace.py` & `brainlit-0.3.5/brainlit/utils/Neuron_trace.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/utils/benchmarking_params.py` & `brainlit-0.3.5/brainlit/utils/benchmarking_params.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/utils/session.py` & `brainlit-0.3.5/brainlit/utils/session.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/utils/upload.py` & `brainlit-0.3.5/brainlit/utils/upload.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/utils/util.py` & `brainlit-0.3.5/brainlit/utils/util.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/utils/write.py` & `brainlit-0.3.5/brainlit/utils/write.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit/viz/swc2voxel.py` & `brainlit-0.3.5/brainlit/viz/swc2voxel.py`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/brainlit.egg-info/PKG-INFO` & `brainlit-0.3.5/brainlit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainlit
-Version: 0.3.4
+Version: 0.3.5
 Summary: Code to process and analyze brainlit data
 Home-page: https://github.com/neurodata/brainlit
 Author: ('Thomas Athey, Bijan Varjivand, Ryan Lu, Matt Figdore, Alex Fiallos, Stanley Wang, Victor Wang',)
 Author-email: tathey1@jhu.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `brainlit-0.3.4/brainlit.egg-info/SOURCES.txt` & `brainlit-0.3.5/brainlit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainlit-0.3.4/setup.py` & `brainlit-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 AUTHOR = (
     "Thomas Athey, Bijan Varjivand, Ryan Lu, Matt Figdore, Alex Fiallos, Stanley Wang, Victor Wang",
 )
 AUTHOR_EMAIL = "tathey1@jhu.edu"
 URL = "https://github.com/neurodata/brainlit"
 MINIMUM_PYTHON_VERSION = 3, 7  # Minimum of Python 3.7
 REQUIRED_PACKAGES = [
+    "numpy==1.23.2",
     "CloudReg",
     "aicspylibczi>=3.0.5",
     "brainrender",
     "numpy>=1.8.1",
     "scikit-image>=0.16.2",
     "networkx>=2.1",
     "scikit-learn==1.1.2",  # issues with pairwise_distances_argmin_min (e.g. used in NeuronTrace) on other versions
     "scipy>=1.1.0",
-    "seaborn>=0.9.0",
+    "seaborn>=0.12.2",
     "tifffile>=2020.7.17",
     "napari[pyqt5]>=0.2.11",
     "PyQt5<=5.15.7",  # bc there was an error with 5.15.8, can remove once that's resolved
     "cloud-volume>=4.2.0",
     "feather-format==0.4.1",
     "ome-zarr>=0.6.0",
     "zarr>=2.10.2",
     "h5py>=3.3.0",
     # "pcurvepy @ git+https://git@github.com/CaseyWeiner/pcurvepy@master#egg=pcurvepy",
     "similaritymeasures>=0.4.4",
     "statannotations>=0.4.4",
+    "igneous-pipeline",
 ]
 
 # Find savanna version.
 PROJECT_PATH = os.path.dirname(os.path.abspath(__file__))
 for line in open(os.path.join(PROJECT_PATH, "brainlit", "__init__.py")):
     if line.startswith("__version__ = "):
         VERSION = line.strip().split()[2][1:-1]
```

