# Comparing `tmp/pe-configurator-0.1.6.tar.gz` & `tmp/pe-configurator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-configurator-0.1.6.tar", last modified: Fri May 12 08:43:04 2023, max compression
+gzip compressed data, was "pe-configurator-0.1.7.tar", last modified: Thu May 18 14:35:43 2023, max compression
```

## Comparing `pe-configurator-0.1.6.tar` & `pe-configurator-0.1.7.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.530877 pe-configurator-0.1.6/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1100 2023-05-12 08:39:45.000000 pe-configurator-0.1.6/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-12 08:43:04.530877 pe-configurator-0.1.6/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.490877 pe-configurator-0.1.6/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/blueprints/test.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.490877 pe-configurator-0.1.6/data/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.6/data/calibration_files.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.500877 pe-configurator-0.1.6/examples/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/examples/.DS_Store
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.510877 pe-configurator-0.1.6/examples/test_GW190412/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/examples/test_GW190412/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/examples/test_GW190412/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/examples/test_GW190412/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.510877 pe-configurator-0.1.6/examples/test_GW190521/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190521/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190521/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190521/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/examples/test_GW190814/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190814/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190814/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190814/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/examples/test_GW191109/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW191109/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW191109/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW191109/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/pe_configurator.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1032 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/peconfigurator/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6877 2023-04-28 13:12:38.000000 pe-configurator-0.1.6/peconfigurator/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/asimov_template.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/peconfigurator/auxiliary/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/auxiliary/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10401 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/auxiliary/make_report.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/auxiliary/run_analyzer.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/get_settings.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15907 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/proc_samples.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/run_on_many_events.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-12 08:43:04.530877 pe-configurator-0.1.6/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/tests/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/tests/test_get_settings.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.631834 pe-configurator-0.1.7/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1100 2023-05-12 08:39:45.000000 pe-configurator-0.1.7/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-18 14:35:43.621834 pe-configurator-0.1.7/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.7/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.591834 pe-configurator-0.1.7/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.7/blueprints/test.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.591834 pe-configurator-0.1.7/data/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.7/data/calibration_files.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.601834 pe-configurator-0.1.7/examples/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.7/examples/.DS_Store
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.601834 pe-configurator-0.1.7/examples/test_GW190412/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.7/examples/test_GW190412/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.7/examples/test_GW190412/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.7/examples/test_GW190412/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.611834 pe-configurator-0.1.7/examples/test_GW190521/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW190521/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW190521/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW190521/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.611834 pe-configurator-0.1.7/examples/test_GW190814/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW190814/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW190814/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW190814/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.621834 pe-configurator-0.1.7/examples/test_GW191109/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW191109/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW191109/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/examples/test_GW191109/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.621834 pe-configurator-0.1.7/pe_configurator.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-18 14:35:43.000000 pe-configurator-0.1.7/pe_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1087 2023-05-18 14:35:43.000000 pe-configurator-0.1.7/pe_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-18 14:35:43.000000 pe-configurator-0.1.7/pe_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-05-18 14:35:43.000000 pe-configurator-0.1.7/pe_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-05-18 14:35:43.000000 pe-configurator-0.1.7/pe_configurator.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-05-18 14:35:43.000000 pe-configurator-0.1.7/pe_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.621834 pe-configurator-0.1.7/peconfigurator/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8456 2023-05-18 14:32:55.000000 pe-configurator-0.1.7/peconfigurator/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/peconfigurator/asimov_template.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.621834 pe-configurator-0.1.7/peconfigurator/auxiliary/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/peconfigurator/auxiliary/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10580 2023-05-18 11:46:09.000000 pe-configurator-0.1.7/peconfigurator/auxiliary/make_report.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    17933 2023-05-18 11:46:09.000000 pe-configurator-0.1.7/peconfigurator/auxiliary/produce_fake_posteriors.ipynb
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7197 2023-05-18 11:46:09.000000 pe-configurator-0.1.7/peconfigurator/auxiliary/run_analyzer.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/peconfigurator/get_settings.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    18402 2023-05-18 14:33:02.000000 pe-configurator-0.1.7/peconfigurator/proc_samples.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/peconfigurator/run_on_many_events.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-18 14:35:43.631834 pe-configurator-0.1.7/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:35:43.621834 pe-configurator-0.1.7/tests/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.7/tests/test_get_settings.py
```

### Comparing `pe-configurator-0.1.6/LICENSE` & `pe-configurator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/PKG-INFO` & `pe-configurator-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-0.1.6/README.md` & `pe-configurator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/data/calibration_files.txt` & `pe-configurator-0.1.7/data/calibration_files.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/.DS_Store` & `pe-configurator-0.1.7/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190412/test.html` & `pe-configurator-0.1.7/examples/test_GW190412/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190412/test.json` & `pe-configurator-0.1.7/examples/test_GW190412/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190412/test.pdf` & `pe-configurator-0.1.7/examples/test_GW190412/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190521/test.html` & `pe-configurator-0.1.7/examples/test_GW190521/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190521/test.json` & `pe-configurator-0.1.7/examples/test_GW190521/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190521/test.pdf` & `pe-configurator-0.1.7/examples/test_GW190521/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190814/test.html` & `pe-configurator-0.1.7/examples/test_GW190814/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190814/test.json` & `pe-configurator-0.1.7/examples/test_GW190814/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW190814/test.pdf` & `pe-configurator-0.1.7/examples/test_GW190814/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW191109/test.html` & `pe-configurator-0.1.7/examples/test_GW191109/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW191109/test.json` & `pe-configurator-0.1.7/examples/test_GW191109/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/examples/test_GW191109/test.pdf` & `pe-configurator-0.1.7/examples/test_GW191109/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/pe_configurator.egg-info/PKG-INFO` & `pe-configurator-0.1.7/pe_configurator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-0.1.6/pe_configurator.egg-info/SOURCES.txt` & `pe-configurator-0.1.7/pe_configurator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,10 @@
 peconfigurator/asimov.py
 peconfigurator/asimov_template.yaml
 peconfigurator/get_settings.py
 peconfigurator/proc_samples.py
 peconfigurator/run_on_many_events.py
 peconfigurator/auxiliary/__init__.py
 peconfigurator/auxiliary/make_report.py
+peconfigurator/auxiliary/produce_fake_posteriors.ipynb
 peconfigurator/auxiliary/run_analyzer.py
 tests/test_get_settings.py
```

### Comparing `pe-configurator-0.1.6/peconfigurator/asimov.py` & `pe-configurator-0.1.7/peconfigurator/asimov.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import importlib
 import os
 import configparser
 import json
+import shutil
 
 import h5py
 from asimov.pipeline import Pipeline
 from asimov import config
 import htcondor
 import yaml
 from asimov.utils import set_directory
 
 class AsimovPipeline(Pipeline):
     """
-    An asimov pipeline for heron.
+    An asimov pipeline for PE Configurator.
     """
     name = "peconfigurator"
     config_template = os.path.join(os.path.dirname(__file__), "asimov_template.yaml")
     #importlib.resources.path(__package__, "asimov_template.yaml")
     _pipeline_command = "peconfigurator"
 
 
@@ -39,15 +40,15 @@
                             keys.remove('version')
                             keys.remove('history')
                             self.production.meta['dataset'] = keys[0]
                         return posterior_file
                 except Exception:
                     pass
         else:
-            self.logger.error("Could not find an analysis providing the posterior to analyse.")
+            self.logger.error("Could not find an analysis providing posterior samples to analyse.")
     
     def build_dag(self, dryrun=False):
         """
         Create a condor submission description.
         """
         name = self.production.name
         ini = self.production.event.repository.find_prods(name,
@@ -56,36 +57,36 @@
         meta = self.production.meta
         posterior = self._find_posterior()
 
         executable = f"{os.path.join(config.get('pipelines', 'environment'), 'bin', self._pipeline_command)}"
         command = ["--dataset", f"{meta['dataset']}",
                    "--output_dir", "results",
                    "--json_file", "recommendations.json",
+                   "--report_file", "report.html",
 	           "--q-min", f"{meta['minimum mass ratio']}",
                    ]
         if "higher modes" in meta['checks']:
             command += ["--HM"]
         if "luminosity distance" in meta['checks']:
             command += ["--include_dL_recommendations"]
         if "no safety" in meta['checks']:
             command += ["--override_safeties"]
         command += [posterior]
-        # To do: Add remaining settings once you've decided where they should go
+
         full_command = executable + " " + " ".join(command)
         self.logger.info(full_command)
         
         description = {
             "executable": executable,
             "arguments": " ".join(command),
             "output": f"{name}.out",
             "error": f"{name}.err",
             "log": f"{name}.log",
             "getenv": "True",
             "request_memory": "4096 MB",
-            "request_disk": "100 MB",
             "batch_name": f"{self.name}/{self.production.event.name}/{name}",
             "accounting_group_user": config.get('condor', 'user'),
             "accounting_group": self.production.meta['scheduler']["accounting group"],
             "request_disk": "8192MB",
             "+flock_local": "True",
             "+DESIRED_Sites": htcondor.classad.quote("nogrid"),
         }
@@ -117,33 +118,38 @@
         self.production.job_id = int(self.clusterid)
         return self.clusterid
 
     def collect_assets(self):
         output = {}
         if os.path.exists(os.path.join(self.production.rundir, "results")):
             output['recommendations'] = os.path.join(self.production.rundir, "results", "recommendations.json")
+            output['report'] = os.path.join(self.production.rundir, "results", "report.html")
         return output
     
     def detect_completion(self):
-        self.logger.info("Checking for completion.")
+        self.logger.info("Checking for job completion.")
         results = self.collect_assets()
         if len(list(results.keys())) > 0:
             self.logger.info("Outputs detected, job complete.")
             return True
         else:
-            self.logger.info("Datafind job completion was not detected.")
+            self.logger.info("PE Configurator job completion was not detected.")
             return False
 
     def after_completion(self):
         """
         Add the recommendations to the ledger.
         """
         with open(self.collect_assets()['recommendations'], "r") as datafile:
             data = json.load(datafile)
 
+        # Copy the report file to the pages directory.
+        pages_dir = os.path.join(config.get("general", "webroot"), self.production.event.name, self.production.name)
+        shutil.copy(self.collect_assets()['report'], os.path.join(pages_dir, index.html))
+        
         meta = self.production.event.meta
 
         if "waveform" not in meta:
             meta['waveform'] = {}
         if "likelihood" not in meta:
             meta['likelihood'] = {}
         
@@ -164,9 +170,37 @@
             meta['likelihood']['psd length'] = meta['data']['segment length']
 
         if "chirpmass_min" in data:
             if not "chirp mass" in meta['priors']:
                 meta['priors']['chirp mass'] = {}
             meta['priors']['chirp mass']['minimum'] = data['chirpmass_min']
             meta['priors']['chirp mass']['maximum'] = data['chirpmass_max']
+
+        if "q_min" in data:
+            if not "mass ratio" in meta['priors']:
+                meta['priors']['mass ratio'] = {}
+                meta['priors']['mass ratio']['minimum'] = data["q_min"]
+            else:
+                if meta['priors']['mass ratio']['minimum'] > data["q_min"]:
+                    meta['priors']['mass ratio']['minimum'] = data["q_min"]
+        
+        if "dL_max" in data:
+            if not "luminosity distance" in meta['priors']:
+                meta['priors']['luminosity distance'] = {}
+                meta['priors']['luminosity distance']['maximum'] = data["dL_max"]
+            else:
+                if meta['priors']['luminosity distance']['maximum'] < data["dL_max"]:
+                    meta['priors']['luminosity distance']['maximum'] = data["dL_max"]
+                
         self.production.event.update_data()
         self.production.status = "uploaded"
+
+    def html(self):
+        """Return the HTML representation of this pipeline."""
+        out = ""
+        pages_dir = os.path.join(self.production.event.name, self.production.name)
+        if self.production.status in {"finished", "uploaded"}:
+            out += """<div class="asimov-pipeline">"""
+            out += f"""<a href="{pages_dir}/index.html">Report</a>"""
+            out += """</div>"""
+
+        return out
```

### Comparing `pe-configurator-0.1.6/peconfigurator/auxiliary/make_report.py` & `pe-configurator-0.1.7/peconfigurator/auxiliary/make_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,19 +43,19 @@
 def markdown_writer_heuristics(samples):
     """Write the rules-based analysis out
 
     Args:
         samples ([array-like]): the samples
     """
     msgs = []
-    msgs.append(distance_checks(samples))
-    msgs.append(NS_check(samples))
-    msgs.append(mass_ratio_checks(samples))
-    msgs.append(SNR_threshold(samples))
-    msgs.append(spin_checks(samples))
+    msgs.extend(distance_checks(samples))
+    msgs.extend(NS_check(samples))
+    msgs.extend(mass_ratio_checks(samples))
+    msgs.extend(SNR_threshold(samples))
+    msgs.extend(spin_checks(samples))
     result = ""
     for msg in msgs:
         if msg:
             result += f"""
 * **{msg}**\n
 """
     return result
@@ -161,14 +161,16 @@
     Parameters
     ----------
     """
     chirpmass_min = recommended_settings["chirpmass_min"]
     chirpmass_max = recommended_settings["chirpmass_max"]
     checks_passed = all(checks.values())
 
+    q_min = recommended_settings.get("q_min", None)
+
     nb = NoteBook()
     f = read(pesummary_file)
     if analysis is None:
         analysis = f.labels[0]
     elif analysis not in f.labels:
         raise ValueError(
             "The analysis '{}' does not exist in '{}'. The available analyses "
@@ -280,18 +282,21 @@
 else:
     n = np.floor(N/3)+1
 
 plt.rcParams['axes.titlesize'] =  'xx-large'   
 plt.rcParams['font.size'] = 18
 plt.rcParams['text.usetex'] = False
 axes=df.hist(figsize=(12,8),bins=50,layout=(n,3),histtype="step",density=True)
-if checks_passed:
-    axes[j,k].axvline(x={chirpmass_min}, ls="--", color="r")
-    axes[j,k].axvline(x={chirpmass_max}, ls="--", color="r")
-    _ = axes[j,k].set_xlim(0.95 * {chirpmass_min},1.05 * {chirpmass_max})
+#if checks_passed:
+axes[j,k].axvline(x={chirpmass_min}, ls="--", color="r")
+axes[j,k].axvline(x={chirpmass_max}, ls="--", color="r")
+_ = axes[j,k].set_xlim(0.95 * {chirpmass_min},1.05 * {chirpmass_max})
+if {q_min} is not None:
+    axes[0,2].axvline(x={q_min}, ls="--", color="r")
+    _ = axes[0,2].set_xlim(0.95 * {q_min},df[r"$q$"].max())
 """
     text = f"Plot of selected posterior parameters. **All masses are in the detector frame**.  The red dashed lines show the proposed $\\mathcal{{M}}$ bounds,[{np.round(chirpmass_min,4)},{np.round(chirpmass_max,4)}]"
 
     nb.add_cell(text, markdown=True)
     nb.add_cell(cell, code=True)
 
     # MECO frequency check
```

### Comparing `pe-configurator-0.1.6/peconfigurator/auxiliary/run_analyzer.py` & `pe-configurator-0.1.7/peconfigurator/auxiliary/run_analyzer.py`

 * *Files 15% similar despite different names*

```diff
@@ -76,48 +76,48 @@
     """
     m1 = samples["mass_1"]
     m2 = samples["mass_2"]
     m1_low = np.percentile(m1, 5)
     m2_low = np.percentile(m2, 5)
     m1_med = np.percentile(m1, 50)
     m2_med = np.percentile(m2, 50)
-    message = ""
+    message = []
     if m1_low < 3 and m1_med > 3:
-        message += "Mass 1 has minor support for mass < 3 $M_{\\odot}$\n"
+        message.append("Mass 1 has minor support for mass < 3 $M_{\\odot}$\n")
     elif m1_med < 3:
-        message += "Mass 1 has strong support for mass < 3  $M_{\\odot}$\n"
+        message.append("Mass 1 has strong support for mass < 3  $M_{\\odot}$\n")
 
     if m2_low < 3 and m2_med > 3:
         if message is not None:
-            message += "Mass 2 has minor support for mass < 3 $M_{\\odot}$"
+            message.append("Mass 2 has minor support for mass < 3 $M_{\\odot}$")
         else:
-            message += "Mass 2 has minor support for mass < 3 $M_{\\odot}$"
+            message.append("Mass 2 has minor support for mass < 3 $M_{\\odot}$")
     elif m2_med < 3:
         if message is not None:
-            message += "Mass 2 has strong support for mass < 3 $M_{\\odot}$"
+            message.append("Mass 2 has strong support for mass < 3 $M_{\\odot}$")
         else:
-            message += "Mass 2 has strong support for mass < 3 $M_{\\odot}$"
+            message.append("Mass 2 has strong support for mass < 3 $M_{\\odot}$")
     return message
 
 
 def SNR_threshold(samples, th_low=8.0, th_high=25.0):
     """Check if the network SNR is lower than some threshold.
     This is intended for very special cases where we somehow
     miss the signal.
 
     Args:
         samples (array-like): The samples
     """
     snr = samples["network_matched_filter_snr"]
     median_snr = np.median(snr)
-    message = ""
+    message = []
     if median_snr < th_low:
-        message += f"The median network matched filter SNR is below {th_low}. Is the signal being found?"
+        message.append(f"The median network matched filter SNR is below {th_low}. Is the signal being found?")
     if median_snr > th_high:
-        message += (
+        message.append(
             f"The median network matched filter SNR is above {th_high}! Very loud event?"
         )
     return message
 
 
 def spin_checks(samples):
     """Perform several checks on the spin parameters
@@ -136,25 +136,25 @@
     a1_width = a1_high-a1_low
     a2_low = np.percentile(a2,5)
     a2_high = np.percentile(a2,95)
     a2_width = a2_high-a2_low
     
     chi_eff_med = np.median(chi_eff)
     chi_p_med = np.median(chi_p)
-    message=""
+    message=[]
     if a1_width<0.4:
-        message+=r"$a_{1}$ is well constrained!\n"
+        message.append(r"$a_{1}$ is well constrained!")
     if a2_width<0.4:
-        message+=r"$a_{2}$ is well constrained!\n"
+        message.append("$a_{2}$ is well constrained!")
     if chi_eff_med < -0.1:
-        message+="The median $\\chi_{\rm eff}<0.1$!\n"
+        message.append("The median $\chi_{\rm eff}<-0.1$!")
     elif chi_eff_med > 0.3:
-        message+="The median $\\chi_{\rm eff}>0.3$!\n"
+        message.append("The median $\chi_{\rm eff}>0.3$!")
     if chi_p_med > 0.6:
-        message+="The median $\\chi_{p}>0.6$, highly precessing event?"
+        message.append(r"The median $\chi_{p}>0.6$, highly precessing event?")
     
     return message
 
 def mass_ratio_checks(samples):
     """Perform various checks on mass ratio
 
     Args:
@@ -162,36 +162,36 @@
     """
     mass_ratio = samples["mass_ratio"]
 
     # Checks on the 90% confidence
     low = np.percentile(mass_ratio, 5)
     high = np.percentile(mass_ratio, 95)
     med = np.percentile(mass_ratio,50)
-    message=""
+    message=[]
     if high < 0.9:
-        message = "Equal masses are excluded at high confidence for this event!\n"
+        message.append("Equal masses are excluded at high confidence for this event!")
     if med<1./3:
-        message+= "Median mass ratio is below 1/3, highly unequal mass event!"
+        message.append("Median mass ratio is below 1/3, highly unequal mass event!")
     return message
 
 def distance_checks(samples, th_low=150, th_high=5000):
     """Perform various checks on the distance. In particular, is the distance
     is very small or very large
 
     Args:
         samples (array-like): The samples
     """
     # Distance in Mpc
     dist = samples["luminosity_distance"]
     median_dist = np.median(dist)
-    message = ""
+    message = []
     if median_dist < th_low:
-        message += f"The median luminosity distance is below {th_low} Mpc!"
+        message.append(f"The median luminosity distance is below {th_low} Mpc!")
     elif median_dist > th_high:
-        message += f"The median luminosity distance is above {th_high} Mpc!"
+        message.append(f"The median luminosity distance is above {th_high} Mpc!")
     return message
 
 
 def theta_JN_checks(samples):
     """Perform check on inclination. In particular, highlight if the inclination
     is close to edge-on
```

### Comparing `pe-configurator-0.1.6/peconfigurator/get_settings.py` & `pe-configurator-0.1.7/peconfigurator/get_settings.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/peconfigurator/proc_samples.py` & `pe-configurator-0.1.7/peconfigurator/proc_samples.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 def mt_from_eta_mc(eta, mc):
     """Compute total mass from symmetric mass ratio and chirp mass"""
     return mc / eta ** (3.0 / 5)
 
 
 def check_railing(samples, label, nbins, tolerance, checks, recommendations=None):
-
-    rail_low, rail_high, recommendation,bounds = railing_check(
+    rail_low, rail_high, recommendation, bounds = railing_check(
         samples, nbins, tolerance, label
     )
     if rail_low or rail_high:
         click.echo(
             f"Checking for railing in {label}: " + click.style("FAILED", fg="red")
         )
         click.secho(
@@ -51,14 +50,15 @@
         click.echo(
             f"Checking for railing in {label}: " + click.style("PASSED", fg="green")
         )
         checks[label] = True
         recommendations[label] = ""
     return bounds
 
+
 def create_json_output(recommended_settings, output_name, args):
     """Write the results to a json file to allow for easy injections"""
     metadata = dict(date=str(datetime.datetime.now()), command_line_args=str(args))
     dc = deepcopy(recommended_settings)
     dc.update(metadata=metadata)
 
     with open(f"{args.output_dir}/{output_name}", "w") as json_file:
@@ -104,14 +104,20 @@
     parser.add_argument(
         "--q-min",
         default=None,
         type=float,
         help="The lower bound of the q-prior to be used for production",
     )
     parser.add_argument(
+        "--dL-max",
+        default=None,
+        type=float,
+        help="The upper bound of the dL-prior to be used for production",
+    )
+    parser.add_argument(
         "--ell-max", help="The ell to use for HM Nyquist check for EOB", default=3
     )
     parser.add_argument(
         "--tolerance",
         type=float,
         help="Tolerance used when checking for railing",
         default=2.0,
@@ -147,15 +153,25 @@
     )
     parser.add_argument(
         "--override_safeties",
         action="store_true",
         help="Disregard all warnings and generate json file anyway. USE AT OWN RISK!",
     )
     parser.add_argument("--debug", action="store_true", help="For debugging")
-    parser.add_argument("--include_dL_recommendations",action="store_true",help="Including recommendations for distance in output")
+    parser.add_argument(
+        "--include_dL_recommendations",
+        action="store_true",
+        help="Including recommendations for distance in output",
+    )
+    parser.add_argument(
+        "--override_fstart",
+        type=float,
+        help="Overrides the recommended f_start with the value provided by the user",
+        default=-1,
+    )
     args = parser.parse_args()
 
     pesum = get_preferred_result(args.samples_file)
 
     try:
         samples = pesum.samples_dict[args.dataset]
     except KeyError:
@@ -198,19 +214,50 @@
 
     if chirpmass_width > 30.0:
         chirpmass_min_bound = (1 - args.bounds_tol) * chirpmass_min
         chirpmass_max_bound = (1 + args.bounds_tol) * chirpmass_max
     else:
         chirpmass_min_bound = chirpmass_min - args.bounds_tol * chirpmass_width
         chirpmass_max_bound = chirpmass_max + args.bounds_tol * chirpmass_width
+    
+    # If chirp mass is railing, update the bounds with recommendation
+    checks = {}
+    recs = {}
+    mchirp_railing_high = False
+    new_mchirp_bounds = check_railing(
+        chirp_mass,
+        "chirp_mass",
+        args.nbins,
+        args.tolerance,
+        checks,
+        recommendations=recs,
+    )
+    if new_mchirp_bounds[0] is not None:
+        click.echo(f"Estimating chirp mass lower bound to be {new_mchirp_bounds[0]}$M_{{\odot}}$. Please inspect visually if the recommendation is sensible.")
+        chirpmass_min_bound = new_mchirp_bounds[0]
+    if new_mchirp_bounds[1] is not None:
+        click.echo(f"Estimating chirp mass upper bound to be {new_mchirp_bounds[1]}$M_{{\odot}}$. Please inspect visually if the recommendation is sensible.")
+        chirpmass_max_bound = new_mchirp_bounds[1]
+        mchirp_railing_high = True
+
+
+    # Check if mass-ratio is railing
+    bounds_massratio = check_railing(
+        q, "mass_ratio", args.nbins, args.tolerance, checks, recommendations=recs
+    )
 
+    massratio_railing = False
     q_min = float(q.min())
-    if args.q_min is not None:
-        if args.q_min > q_min:
-            q_min = args.q_min
+    if bounds_massratio[0] is not None:
+        massratio_railing = True
+        if q_min > bounds_massratio[0]:
+            q_min = bounds_massratio[0]
+    #if args.q_min is not None:
+    #    if args.q_min > q_min:
+    #        q_min = args.q_min
 
     eta_min = q_min / (1 + q_min) ** 2
 
     click.echo("Processing....")
     click.echo("Estimating seglen based on posterior samples")
 
     # seglen section
@@ -313,94 +360,100 @@
         f_start = f_start_adj
         seobp_amporder = seobp_amporder_adj
         click.echo(
             "The start frequency had to be adjusted to accomodate the changed chirp mass"
         )
     else:
         click.echo("No adjustment necessary!")
+
     # f_start section ends
 
     click.echo("Done processing")
     click.echo()
     click.echo("#" * 30 + " SUMMARY " + 30 * "#")
     click.echo("Posterior parameters")
     click.echo("--" * 20)
     print(df.describe())
     click.echo("--" * 20)
     click.echo("Sanity checks")
 
     checks_passed = True
-    checks = {}
-    recs = {}
 
     # Railing checks
-    check_railing(
-        chirp_mass,
-        "chirp_mass",
-        args.nbins,
-        args.tolerance,
-        checks,
-        recommendations=recs,
-    )
     bounds_distance = check_railing(
         dist, "distance", args.nbins, args.tolerance, checks, recommendations=recs
     )
-    check_railing(
-        q, "mass_ratio", args.nbins, args.tolerance, checks, recommendations=recs
-    )
     # End railing checks
 
     # MECO check section
     new_checks = checks.copy()
     f_ref = args.f_ref
+    f_ref_buffer = 0.97
 
     f_MECOs = np.array(
         [
             MECO_freq(mt, 1 / qp, s1z, s2z)
             for mt, qp, s1z, s2z in list(zip(mtot, q, chi1z, chi2z))
         ]
     )
 
     f_MECO_min = np.min(f_MECOs)
     if f_ref >= 0.97 * f_MECO_min:
         click.echo(
             "Checking that f_ref is not above f_MECO: "
             + click.style("FAILED", fg="red")
         )
+        checks["f_ref"] = False
+        f_ref = np.floor(f_ref_buffer * f_MECO_min)
+        new_checks["f_ref"] = True
         click.secho(
-            f"WARNNING: the reference frequency {f_ref}>=0.97*min(f_MECO), f_MECO = {f_MECO_min}, overwritting reference frequency to f_ref=0.95*min(f_MECO)",
+            f"WARNING: the reference frequency is too close to the MECO frequency, f_MECO = {f_MECO_min}, overwritting reference frequency to f_ref={f_ref}",
             fg="red",
         )
-        checks["f_ref"] = False
-        f_ref = 0.95 * f_MECO_min
-        new_checks["f_ref"] = True
 
     else:
         click.echo(
             "Checking that f_ref is not above f_MECO: "
             + click.style("PASSED", fg="green")
         )
         checks["f_ref"] = True
         new_checks["f_ref"] = True
 
-    # Do we pass the MECO check with the expanded chirp mass?
-    idx_min = np.argmin(f_MECOs)
-    q_min = q[idx_min]
-    eta_min = eta_from_q(q_min)
-    mtot_min_adj = mt_from_eta_mc(eta_min, chirpmass_max_bound)
-    f_meco = MECO_freq(mtot_min_adj, 1 / q_min, chi1z[idx_min], chi2z[idx_min])
-    if f_ref >= 0.97 * f_meco:
-        click.secho(
-            f"The reference frequency ({f_ref}) is too close to the new MECO frequency, {f_meco} Hz, overwritting reference frequency to f_ref=0.95*f_MECO",
-            fg="red",
+    # Do we pass the MECO check with the expanded chirp mass? Yes, if there is railing in the upper bound of the chirp mass posterior
+    if mchirp_railing_high:
+        idx_min = np.argmin(f_MECOs)
+        q_min = q[idx_min]
+        eta_min = eta_from_q(q_min)
+        mtot_min_adj = mt_from_eta_mc(eta_min, chirpmass_max_bound)
+        f_meco = MECO_freq(mtot_min_adj, 1 / q_min, chi1z[idx_min], chi2z[idx_min])
+        click.echo(
+            "Checking that f_ref is not above f_MECO for the recommended chirp mass prior range."
         )
-        checks["f_ref"] = False
-        f_ref = 0.95 * f_meco
-        new_checks["f_ref"] = True
+        if f_ref >= f_ref_buffer * f_meco:
+            checks["f_ref"] = False
+            f_ref = np.floor(f_ref_buffer * f_meco)
+            new_checks["f_ref"] = True
+            click.secho(
+                f"The reference frequency is too close to the new MECO frequency, {f_meco} Hz, overwritting reference frequency to f_ref={f_ref}",
+                fg="red",
+            )
 
+    # Try to override f_start is requested by the user
+    # Process will fail if the MECO test is not satisfied for the new f_start
+    if args.override_fstart > 0:
+        if args.override_fstart <= f_ref:
+            f_start = args.override_fstart
+            click.secho(
+                f"WARNING: Overriding f_start to the request value of {f_start}Hz. Notice that some power may be lost in the higher harmonics!",
+                fg="red",
+            )
+        else:
+            raise ValueError(
+                f"Requested f_start of {args.override_fstart}Hz is greater than 0.97*f_MECO={f_ref_buffer*f_meco} Hz. This can produce pathological waveform generation. Please consider to request a lower value."
+            )
     if f_ref < f_start:
         click.secho(
             f"The reference frequency ({f_ref}) is lower than the starting waveform generation frequency, {f_start} Hz, overwritting reference frequency to f_start.",
             fg="red",
         )
         checks["f_ref"] = False
         f_ref = f_start
@@ -447,14 +500,18 @@
             f_MECO_adj=f_meco,
         )
     if args.include_dL_recommendations:
         if bounds_distance[0] is not None:
             recommended_settings.update(dL_min=bounds_distance[0])
         if bounds_distance[1] is not None:
             recommended_settings.update(dL_max=bounds_distance[1])
+    
+    # Include mass-ratio recommendations
+    if massratio_railing:
+        recommended_settings.update(q_min=bounds_massratio[0])
 
     # np.savetxt("liberal_seglens.dat",fulllens)
     # Did all the checks pass?
     checks_passed = all(new_checks.values())
     click.echo(80 * "+")
     click.echo()
 
@@ -477,14 +534,14 @@
             checks=checks,
             recommendations=recs,
             analysis=args.dataset,
             filename=args.report_file,
             outdir=args.output_dir,
         )
         sp.call(
-            f"jupyter nbconvert --output-dir={args.output_dir} --no-input --to html  --execute --ExecutePreprocessor.timeout=120 {args.output_dir}/{args.report_file}",
+            f"jupyter nbconvert --output-dir={args.output_dir} --no-input --to html  --execute --ExecutePreprocessor.timeout=600 {args.output_dir}/{args.report_file}",
             shell=True,
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pe-configurator-0.1.6/peconfigurator/run_on_many_events.py` & `pe-configurator-0.1.7/peconfigurator/run_on_many_events.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/pyproject.toml` & `pe-configurator-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.6/tests/test_get_settings.py` & `pe-configurator-0.1.7/tests/test_get_settings.py`

 * *Files identical despite different names*

