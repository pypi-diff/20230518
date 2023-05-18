# Comparing `tmp/asimov-gwdata-0.1.4.tar.gz` & `tmp/asimov-gwdata-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asimov-gwdata-0.1.4.tar", last modified: Fri May 12 08:23:42 2023, max compression
+gzip compressed data, was "asimov-gwdata-0.1.5.tar", last modified: Thu May 18 13:06:28 2023, max compression
```

## Comparing `asimov-gwdata-0.1.4.tar` & `asimov-gwdata-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1065 2023-05-12 08:22:13.000000 asimov-gwdata-0.1.4/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)      677 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      677 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      460 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/blueprints/asimov-analysis.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/datafind/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.4/datafind/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6093 2023-05-11 13:58:29.000000 asimov-gwdata-0.1.4/datafind/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/datafind/datafind_template.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/datafind/main.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/pyproject.toml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/scripts/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/scripts/asimov-test-script.sh
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/scripts/test-calibration-dump.yaml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/test_settings.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 13:06:28.123248 asimov-gwdata-0.1.5/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1065 2023-05-12 08:22:13.000000 asimov-gwdata-0.1.5/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1402 2023-05-18 13:06:28.123248 asimov-gwdata-0.1.5/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      873 2023-05-12 13:33:40.000000 asimov-gwdata-0.1.5/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 13:06:28.113248 asimov-gwdata-0.1.5/asimov_gwdata.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1402 2023-05-18 13:06:28.000000 asimov-gwdata-0.1.5/asimov_gwdata.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      460 2023-05-18 13:06:28.000000 asimov-gwdata-0.1.5/asimov_gwdata.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-18 13:06:28.000000 asimov-gwdata-0.1.5/asimov_gwdata.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-05-18 13:06:28.000000 asimov-gwdata-0.1.5/asimov_gwdata.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       55 2023-05-18 13:06:28.000000 asimov-gwdata-0.1.5/asimov_gwdata.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-05-18 13:06:28.000000 asimov-gwdata-0.1.5/asimov_gwdata.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 13:06:28.113248 asimov-gwdata-0.1.5/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.5/blueprints/asimov-analysis.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 13:06:28.123248 asimov-gwdata-0.1.5/datafind/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.5/datafind/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6260 2023-05-18 10:43:44.000000 asimov-gwdata-0.1.5/datafind/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.5/datafind/datafind_template.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3506 2023-05-18 10:54:49.000000 asimov-gwdata-0.1.5/datafind/main.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1051 2023-05-12 13:02:39.000000 asimov-gwdata-0.1.5/pyproject.toml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-18 13:06:28.123248 asimov-gwdata-0.1.5/scripts/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.5/scripts/asimov-test-script.sh
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.5/scripts/test-calibration-dump.yaml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-18 13:06:28.123248 asimov-gwdata-0.1.5/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.5/test_settings.yaml
```

### Comparing `asimov-gwdata-0.1.4/LICENSE` & `asimov-gwdata-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.4/datafind/asimov.py` & `asimov-gwdata-0.1.5/datafind/asimov.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,15 +68,19 @@
         }
 
         job = htcondor.Submit(description)
         os.makedirs(self.production.rundir, exist_ok=True)
         with set_directory(self.production.rundir):
             with open(f"{name}.sub", "w") as subfile:
                 subfile.write(job.__str__())
-                
+
+            full_command = f"""#! /bin/bash
+{ full_command }
+"""
+
             with open(f"{name}.sh", "w") as bashfile:
                 bashfile.write(str(full_command))
 
         with set_directory(self.production.rundir):
             try:
                 schedulers = htcondor.Collector().locate(
                     htcondor.DaemonTypes.Schedd, config.get("condor", "scheduler")
@@ -94,16 +98,16 @@
     def submit_dag(self, dryrun=False):
         self.production.status = "running"
         self.production.job_id = int(self.clusterid)
         return self.clusterid
 
     def detect_completion(self):
         self.logger.info("Checking for completion.")
-        frames = self.collect_assets()
-        if len(list(frames.keys())) > 0:
+        assets = self.collect_assets()
+        if len(list(assets.keys())) > 0:
             self.logger.info("Outputs detected, job complete.")
             return True
         else:
             self.logger.info("Datafind job completion was not detected.")
             return False
 
     def after_completion(self):
@@ -111,53 +115,53 @@
         self.production.event.update_data()
 
     def collect_assets(self):
         """
         Collect the assets for this job.
         """
         outputs = {}
-        if os.path.exists(f"{self.production.rundir}/frames/"):
-            results_dir = glob.glob(f"{self.production.rundir}/frames/*")
+        if os.path.exists(os.path.join(self.production.rundir, "frames")):
+            results_dir = glob.glob(os.path.join(self.production.rundir, "frames", "*"))
             frames = {}
 
             for frame in results_dir:
                 ifo = frame.split("/")[-1].split("_")[0].split("-")[1]
                 frames[ifo] = frame
 
             outputs["frames"] = frames
 
             self.production.event.meta['data']['data files'] = frames
 
-        if os.path.exists(f"{self.production.rundir}/psds/"):
-            results_dir = glob.glob(f"{self.production.rundir}/psds/*")
+        if os.path.exists(os.path.join(self.production.rundir, "psds")):
+            results_dir = glob.glob(os.path.join(self.production.rundir, "psds", "*"))
             psds = {}
 
             for psd in results_dir:
-                ifo = psds.split(".")[0]
+                ifo = os.path.splitext(psds)[0]
                 psds[ifo] = psd
 
             outputs["psds"] = psds
 
         # TODO: Need to have this check the sample rate before it saves to ledger
         # self.production.event.meta['data']['data files'] = frames
 
-        if os.path.exists(f"{self.production.rundir}/calibration/"):
-            results_dir = glob.glob(f"{self.production.rundir}/calibration/*")
+        if os.path.exists(os.path.join(self.production.rundir, "calibration")):
+            results_dir = glob.glob(os.path.join(self.production.rundir, "calibration", "*"))
             calibration = {}
 
             for cal in results_dir:
-                ifo = cal.split(".")[0]
+                ifo = os.path.splitext(cal)[0]
                 calibration[ifo] = cal
 
             outputs["calibration"] = calibration
 
             self.production.event.meta['data']['calibration'] = calibration
 
-        if os.path.exists(f"{self.production.rundir}/posterior/"):
-            results = glob.glob(f"{self.production.rundir}/posterior/*")
+        if os.path.exists(os.path.join(self.production.rundir, "posterior")):
+            results = glob.glob(os.path.join(self.production.rundir, "posterior", "*")
 
             outputs["samples"] = results[0]
 
         return outputs
 
     def html(self):
         """Return the HTML representation of this pipeline."""
```

### Comparing `asimov-gwdata-0.1.4/datafind/datafind_template.yml` & `asimov-gwdata-0.1.5/datafind/datafind_template.yml`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.4/datafind/main.py` & `asimov-gwdata-0.1.5/datafind/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,17 +37,21 @@
     """
 
     # First find the metafile
     if "source" in settings:
         if settings['source']['type'] == "pesummary":
             location = settings['source']['location']
             location = glob.glob(location)[0]
-    
+    else:
+        raise ValueError("No metafile location found")
     data = read(location, package="gw")
-    analysis = settings['source']['analysis']
+    try:
+        analysis = settings['source']['analysis']
+    except KeyError:
+        raise ValueError("No source analysis found in config")
 
     for component in components:
     
         if component == "calibration":
             calibration_data = data.priors["calibration"][analysis]
             os.makedirs("calibration", exist_ok=True)
             for ifo, calibration in calibration_data.items():
```

### Comparing `asimov-gwdata-0.1.4/pyproject.toml` & `asimov-gwdata-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent"
 ]
 requires-python = ">=3.7"
 dependencies = [
         "gwosc",
 	"asimov>=0.4.0",
+	"pesummary",
 ]
 
 [project.optional-dependencies]
 docs = [
 	"sphinx",
 	"kentigern",
 ]
```

