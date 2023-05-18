# Comparing `tmp/pe-configurator-0.1.8.tar.gz` & `tmp/pe-configurator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-configurator-0.1.8.tar", last modified: Thu May 18 14:58:38 2023, max compression
+gzip compressed data, was "pe-configurator-0.1.9.tar", last modified: Thu May 18 15:06:56 2023, max compression
```

## Comparing `pe-configurator-0.1.8.tar` & `pe-configurator-0.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.381465 pe-configurator-0.1.8/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1100 2023-05-12 08:39:45.000000 pe-configurator-0.1.8/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-18 14:58:38.381465 pe-configurator-0.1.8/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.8/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.371465 pe-configurator-0.1.8/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.8/blueprints/test.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.371465 pe-configurator-0.1.8/data/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.8/data/calibration_files.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.371465 pe-configurator-0.1.8/examples/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.8/examples/.DS_Store
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.371465 pe-configurator-0.1.8/examples/test_GW190412/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.8/examples/test_GW190412/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.8/examples/test_GW190412/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.8/examples/test_GW190412/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.371465 pe-configurator-0.1.8/examples/test_GW190521/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW190521/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW190521/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW190521/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.371465 pe-configurator-0.1.8/examples/test_GW190814/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW190814/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW190814/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW190814/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.381465 pe-configurator-0.1.8/examples/test_GW191109/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW191109/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW191109/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/examples/test_GW191109/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.381465 pe-configurator-0.1.8/pe_configurator.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-18 14:58:38.000000 pe-configurator-0.1.8/pe_configurator.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1087 2023-05-18 14:58:38.000000 pe-configurator-0.1.8/pe_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-18 14:58:38.000000 pe-configurator-0.1.8/pe_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-05-18 14:58:38.000000 pe-configurator-0.1.8/pe_configurator.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-05-18 14:58:38.000000 pe-configurator-0.1.8/pe_configurator.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-05-18 14:58:38.000000 pe-configurator-0.1.8/pe_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.381465 pe-configurator-0.1.8/peconfigurator/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8458 2023-05-18 14:57:57.000000 pe-configurator-0.1.8/peconfigurator/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/peconfigurator/asimov_template.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.381465 pe-configurator-0.1.8/peconfigurator/auxiliary/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/peconfigurator/auxiliary/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10580 2023-05-18 11:46:09.000000 pe-configurator-0.1.8/peconfigurator/auxiliary/make_report.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17933 2023-05-18 11:46:09.000000 pe-configurator-0.1.8/peconfigurator/auxiliary/produce_fake_posteriors.ipynb
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7197 2023-05-18 11:46:09.000000 pe-configurator-0.1.8/peconfigurator/auxiliary/run_analyzer.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/peconfigurator/get_settings.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    18402 2023-05-18 14:33:02.000000 pe-configurator-0.1.8/peconfigurator/proc_samples.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/peconfigurator/run_on_many_events.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-18 14:58:38.381465 pe-configurator-0.1.8/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 14:58:38.381465 pe-configurator-0.1.8/tests/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.8/tests/test_get_settings.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.341339 pe-configurator-0.1.9/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1100 2023-05-12 08:39:45.000000 pe-configurator-0.1.9/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-18 15:06:56.341339 pe-configurator-0.1.9/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.9/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.331339 pe-configurator-0.1.9/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.9/blueprints/test.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.331339 pe-configurator-0.1.9/data/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.9/data/calibration_files.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.331339 pe-configurator-0.1.9/examples/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.9/examples/.DS_Store
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.331339 pe-configurator-0.1.9/examples/test_GW190412/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.9/examples/test_GW190412/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.9/examples/test_GW190412/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.9/examples/test_GW190412/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.331339 pe-configurator-0.1.9/examples/test_GW190521/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW190521/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW190521/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW190521/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.331339 pe-configurator-0.1.9/examples/test_GW190814/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW190814/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW190814/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW190814/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.331339 pe-configurator-0.1.9/examples/test_GW191109/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW191109/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW191109/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/examples/test_GW191109/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.341339 pe-configurator-0.1.9/pe_configurator.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-18 15:06:56.000000 pe-configurator-0.1.9/pe_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1087 2023-05-18 15:06:56.000000 pe-configurator-0.1.9/pe_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-18 15:06:56.000000 pe-configurator-0.1.9/pe_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-05-18 15:06:56.000000 pe-configurator-0.1.9/pe_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-05-18 15:06:56.000000 pe-configurator-0.1.9/pe_configurator.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-05-18 15:06:56.000000 pe-configurator-0.1.9/pe_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.341339 pe-configurator-0.1.9/peconfigurator/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8513 2023-05-18 15:05:57.000000 pe-configurator-0.1.9/peconfigurator/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/peconfigurator/asimov_template.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.341339 pe-configurator-0.1.9/peconfigurator/auxiliary/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/peconfigurator/auxiliary/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10580 2023-05-18 11:46:09.000000 pe-configurator-0.1.9/peconfigurator/auxiliary/make_report.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    17933 2023-05-18 11:46:09.000000 pe-configurator-0.1.9/peconfigurator/auxiliary/produce_fake_posteriors.ipynb
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7197 2023-05-18 11:46:09.000000 pe-configurator-0.1.9/peconfigurator/auxiliary/run_analyzer.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/peconfigurator/get_settings.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    18402 2023-05-18 14:33:02.000000 pe-configurator-0.1.9/peconfigurator/proc_samples.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/peconfigurator/run_on_many_events.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-18 15:06:56.341339 pe-configurator-0.1.9/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 15:06:56.341339 pe-configurator-0.1.9/tests/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.9/tests/test_get_settings.py
```

### Comparing `pe-configurator-0.1.8/LICENSE` & `pe-configurator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/PKG-INFO` & `pe-configurator-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-0.1.8/README.md` & `pe-configurator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/data/calibration_files.txt` & `pe-configurator-0.1.9/data/calibration_files.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/.DS_Store` & `pe-configurator-0.1.9/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190412/test.html` & `pe-configurator-0.1.9/examples/test_GW190412/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190412/test.json` & `pe-configurator-0.1.9/examples/test_GW190412/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190412/test.pdf` & `pe-configurator-0.1.9/examples/test_GW190412/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190521/test.html` & `pe-configurator-0.1.9/examples/test_GW190521/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190521/test.json` & `pe-configurator-0.1.9/examples/test_GW190521/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190521/test.pdf` & `pe-configurator-0.1.9/examples/test_GW190521/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190814/test.html` & `pe-configurator-0.1.9/examples/test_GW190814/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190814/test.json` & `pe-configurator-0.1.9/examples/test_GW190814/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW190814/test.pdf` & `pe-configurator-0.1.9/examples/test_GW190814/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW191109/test.html` & `pe-configurator-0.1.9/examples/test_GW191109/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW191109/test.json` & `pe-configurator-0.1.9/examples/test_GW191109/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/examples/test_GW191109/test.pdf` & `pe-configurator-0.1.9/examples/test_GW191109/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/pe_configurator.egg-info/PKG-INFO` & `pe-configurator-0.1.9/pe_configurator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-0.1.8/pe_configurator.egg-info/SOURCES.txt` & `pe-configurator-0.1.9/pe_configurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/peconfigurator/asimov.py` & `pe-configurator-0.1.9/peconfigurator/asimov.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
         Add the recommendations to the ledger.
         """
         with open(self.collect_assets()['recommendations'], "r") as datafile:
             data = json.load(datafile)
 
         # Copy the report file to the pages directory.
         pages_dir = os.path.join(config.get("general", "webroot"), self.production.event.name, self.production.name)
+        
         shutil.copy(self.collect_assets()['report'], os.path.join(pages_dir, "index.html"))
         
         meta = self.production.event.meta
 
         if "waveform" not in meta:
             meta['waveform'] = {}
         if "likelihood" not in meta:
@@ -194,13 +195,14 @@
         self.production.event.update_data()
         self.production.status = "uploaded"
 
     def html(self):
         """Return the HTML representation of this pipeline."""
         out = ""
         pages_dir = os.path.join(self.production.event.name, self.production.name)
+        os.makedirs(pages_dir, exist_ok=True)
         if self.production.status in {"finished", "uploaded"}:
             out += """<div class="asimov-pipeline">"""
             out += f"""<a href="{pages_dir}/index.html">Report</a>"""
             out += """</div>"""
 
         return out
```

### Comparing `pe-configurator-0.1.8/peconfigurator/auxiliary/make_report.py` & `pe-configurator-0.1.9/peconfigurator/auxiliary/make_report.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/peconfigurator/auxiliary/produce_fake_posteriors.ipynb` & `pe-configurator-0.1.9/peconfigurator/auxiliary/produce_fake_posteriors.ipynb`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/peconfigurator/auxiliary/run_analyzer.py` & `pe-configurator-0.1.9/peconfigurator/auxiliary/run_analyzer.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/peconfigurator/get_settings.py` & `pe-configurator-0.1.9/peconfigurator/get_settings.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/peconfigurator/proc_samples.py` & `pe-configurator-0.1.9/peconfigurator/proc_samples.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/peconfigurator/run_on_many_events.py` & `pe-configurator-0.1.9/peconfigurator/run_on_many_events.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/pyproject.toml` & `pe-configurator-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.8/tests/test_get_settings.py` & `pe-configurator-0.1.9/tests/test_get_settings.py`

 * *Files identical despite different names*

