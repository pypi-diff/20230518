# Comparing `tmp/kotan-0.1.3.tar.gz` & `tmp/kotan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kotan-0.1.3.tar", max compression
+gzip compressed data, was "kotan-0.1.4.tar", max compression
```

## Comparing `kotan-0.1.3.tar` & `kotan-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-16 05:09:07.710676 kotan-0.1.3/README.md
--rw-r--r--   0        0        0       41 2023-05-16 05:09:07.710676 kotan-0.1.3/kotan/__init__.py
--rw-r--r--   0        0        0      299 2023-05-16 05:09:07.710676 kotan-0.1.3/kotan/const.py
--rw-r--r--   0        0        0     2123 2023-05-16 05:09:07.710676 kotan-0.1.3/kotan/job.py
--rw-r--r--   0        0        0      112 2023-05-16 05:09:07.710676 kotan-0.1.3/kotan/tasks/__init__.py
--rw-r--r--   0        0        0     3252 2023-05-16 05:25:51.904962 kotan-0.1.3/kotan/tasks/data_augmentation.py
--rw-r--r--   0        0        0     2590 2023-05-16 05:25:58.316875 kotan-0.1.3/kotan/tasks/machine_translation.py
--rw-r--r--   0        0        0      327 2023-05-16 05:26:06.280766 kotan-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 kotan-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-16 05:09:07.710676 kotan-0.1.4/README.md
+-rw-r--r--   0        0        0       45 2023-05-17 23:24:18.924115 kotan-0.1.4/kotan/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-16 05:09:07.710676 kotan-0.1.4/kotan/const.py
+-rw-r--r--   0        0        0     2122 2023-05-17 23:24:17.844189 kotan-0.1.4/kotan/job.py
+-rw-r--r--   0        0        0      112 2023-05-16 05:09:07.710676 kotan-0.1.4/kotan/tasks/__init__.py
+-rw-r--r--   0        0        0     3251 2023-05-16 06:06:15.311045 kotan-0.1.4/kotan/tasks/data_augmentation.py
+-rw-r--r--   0        0        0     2590 2023-05-16 05:25:58.316875 kotan-0.1.4/kotan/tasks/machine_translation.py
+-rw-r--r--   0        0        0      327 2023-05-17 23:24:23.783782 kotan-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 kotan-0.1.4/PKG-INFO
```

### Comparing `kotan-0.1.3/kotan/job.py` & `kotan-0.1.4/kotan/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 # Task list
 SUPPORTED_TASKS = {
     "mt": KoTANTranslationFactory,
     "translation": KoTANTranslationFactory,
     "aug": KoTANAugmentationFactory,
-    "augumentation": KoTANAugmentationFactory
+    "augmentation": KoTANAugmentationFactory
 }
 
 
 class KoTAN:
     def __new__(
             cls,
             task,
```

### Comparing `kotan-0.1.3/kotan/tasks/data_augmentation.py` & `kotan-0.1.4/kotan/tasks/data_augmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Args:
         src (str): source language
         
     Returns:
         class: KoTANAugmentation class
 
     Examples:
-        >>> mt = KoTAN(task="augumentation", level="fine")
+        >>> mt = KoTAN(task="augmentation", level="fine")
     """
 
     def __init__(self, 
                  task, 
                  tgt, 
                  LANG_ALIASES,
                  level):
```

### Comparing `kotan-0.1.3/kotan/tasks/machine_translation.py` & `kotan-0.1.4/kotan/tasks/machine_translation.py`

 * *Files identical despite different names*

### Comparing `kotan-0.1.3/PKG-INFO` & `kotan-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kotan
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: jisukim
 Author-email: jisukim8873@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

