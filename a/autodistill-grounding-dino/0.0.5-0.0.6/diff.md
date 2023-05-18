# Comparing `tmp/autodistill_grounding_dino-0.0.5.tar.gz` & `tmp/autodistill_grounding_dino-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill_grounding_dino-0.0.5.tar", last modified: Wed May 17 23:00:04 2023, max compression
+gzip compressed data, was "autodistill_grounding_dino-0.0.6.tar", last modified: Thu May 18 16:07:25 2023, max compression
```

## Comparing `autodistill_grounding_dino-0.0.5.tar` & `autodistill_grounding_dino-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:00:04.443704 autodistill_grounding_dino-0.0.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-05-17 23:00:04.443704 autodistill_grounding_dino-0.0.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3157 2023-05-16 16:46:34.000000 autodistill_grounding_dino-0.0.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:00:04.443704 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2023-05-16 17:10:44.000000 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3113 2023-05-17 21:28:46.000000 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino/grounding_dino.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7778 2023-05-17 21:28:46.000000 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino/helpers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:00:04.443704 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-05-17 23:00:04.000000 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      408 2023-05-17 23:00:04.000000 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 23:00:04.000000 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-05-17 23:00:04.000000 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2023-05-17 23:00:04.000000 autodistill_grounding_dino-0.0.5/autodistill_grounding_dino.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 23:00:04.443704 autodistill_grounding_dino-0.0.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-05-17 23:00:02.000000 autodistill_grounding_dino-0.0.5/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 23:00:04.443704 autodistill_grounding_dino-0.0.5/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-05-17 21:20:53.000000 autodistill_grounding_dino-0.0.5/test/test_hello.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 16:07:25.921839 autodistill_grounding_dino-0.0.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-05-18 16:07:25.921839 autodistill_grounding_dino-0.0.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3157 2023-05-16 16:46:34.000000 autodistill_grounding_dino-0.0.6/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 16:07:25.921839 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2023-05-18 16:05:48.000000 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3113 2023-05-17 21:28:46.000000 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino/grounding_dino.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8224 2023-05-18 16:04:21.000000 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino/helpers.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 16:07:25.921839 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-05-18 16:07:25.000000 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      408 2023-05-18 16:07:25.000000 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-18 16:07:25.000000 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-05-18 16:07:25.000000 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2023-05-18 16:07:25.000000 autodistill_grounding_dino-0.0.6/autodistill_grounding_dino.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-18 16:07:25.921839 autodistill_grounding_dino-0.0.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1323 2023-05-17 23:00:02.000000 autodistill_grounding_dino-0.0.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 16:07:25.921839 autodistill_grounding_dino-0.0.6/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-05-17 21:20:53.000000 autodistill_grounding_dino-0.0.6/test/test_hello.py
```

### Comparing `autodistill_grounding_dino-0.0.5/PKG-INFO` & `autodistill_grounding_dino-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill_grounding_dino
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: Automatically distill large foundational models into smaller, in-domain models for deployment
 Platform: UNKNOWN
```

### Comparing `autodistill_grounding_dino-0.0.5/README.md` & `autodistill_grounding_dino-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `autodistill_grounding_dino-0.0.5/autodistill_grounding_dino/grounding_dino.py` & `autodistill_grounding_dino-0.0.6/autodistill_grounding_dino/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `autodistill_grounding_dino-0.0.5/autodistill_grounding_dino/helpers.py` & `autodistill_grounding_dino-0.0.6/autodistill_grounding_dino/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,26 +118,37 @@
             # Install the package in editable mode
             subprocess.run(
                 ["pip", "install", "-q", "-e", "."],
                 cwd=REPO_DIR,
                 stdout=devnull,
                 stderr=devnull,
             )
+            
+            #re-upgrade supervision
+            subprocess.run(
+                ["pip", "install", "-q", "--upgrade", "supervision"],
+                cwd=REPO_DIR,
+                stdout=devnull,
+                stderr=devnull,
+            )
 
         if not os.path.exists(CHECKPOINT_DIR):
             os.makedirs(CHECKPOINT_DIR)
         GROUNDING_DINO_CHECKPOINT_PATH = os.path.join(
             CHECKPOINT_DIR, "groundingdino_swint_ogc.pth"
         )
         if not os.path.exists(GROUNDING_DINO_CHECKPOINT_PATH):
             url = "https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth"
             urllib.request.urlretrieve(url, GROUNDING_DINO_CHECKPOINT_PATH)
 
-        import groundingdino
-        from groundingdino.util.inference import Model
+        try:
+            import groundingdino
+            from groundingdino.util.inference import Model
+        except:
+            raise("Failed to import groundingdino after installation. If you are in Google Colab, you must restart the runtime and run this cell again.")
 
         grounding_dino_model = Model(
             model_config_path=GROUNDING_DINO_CONFIG_PATH,
             model_checkpoint_path=GROUNDING_DINO_CHECKPOINT_PATH,
         )
 
         grounding_dino_model.to(DEVICE)
```

### Comparing `autodistill_grounding_dino-0.0.5/autodistill_grounding_dino.egg-info/PKG-INFO` & `autodistill_grounding_dino-0.0.6/autodistill_grounding_dino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-grounding-dino
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: Automatically distill large foundational models into smaller, in-domain models for deployment
 Platform: UNKNOWN
```

### Comparing `autodistill_grounding_dino-0.0.5/setup.py` & `autodistill_grounding_dino-0.0.6/setup.py`

 * *Files identical despite different names*

