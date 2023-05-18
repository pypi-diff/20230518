# Comparing `tmp/esp-idf-size-0.3.0.tar.gz` & `tmp/esp-idf-size-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-size/esp-idf-size/dist/.tmp-b5p4_6_x/esp-idf-size-0.3.0.tar", last modified: Mon Mar 27 17:23:03 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-size/esp-idf-size/dist/.tmp-zosoa97p/esp-idf-size-0.3.1.tar", last modified: Thu May 18 09:54:53 2023, max compression
```

## Comparing `esp-idf-size-0.3.0.tar` & `esp-idf-size-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/esp_idf_size/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32h4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32s3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    56335 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/esp_idf_size/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/esp_idf_size.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/esp_idf_size.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/esp_idf_size.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/esp_idf_size.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/esp_idf_size.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/esp_idf_size.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:23:03.000000 esp-idf-size-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-27 17:22:48.000000 esp-idf-size-0.3.0/test/test_idf_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32c2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32c6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32h2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32h4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32s2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32s3.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56338 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/esp_idf_size/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/esp_idf_size.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:54:53.000000 esp-idf-size-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-18 09:54:30.000000 esp-idf-size-0.3.1/test/test_idf_size.py
```

### Comparing `esp-idf-size-0.3.0/LICENSE` & `esp-idf-size-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.0/PKG-INFO` & `esp-idf-size-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-size
-Version: 0.3.0
+Version: 0.3.1
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/espressif/esp-idf-size
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32.yaml` & `esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32s2.yaml` & `esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32s2.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.0/esp_idf_size/chip_info/esp32s3.yaml` & `esp-idf-size-0.3.1/esp_idf_size/chip_info/esp32s3.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.0/esp_idf_size/core.py` & `esp-idf-size-0.3.1/esp_idf_size/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     ''' Detect target chip based on the target archive name in the linker script part of the MAP file '''
     scan_to_header(map_file, 'Linker script and memory map')
 
     RE_TARGET = re.compile(r'IDF_TARGET_(\S*) =')
     # For back-compatible with cmake in idf version before 5.0
     RE_TARGET_CMAKEv4x = re.compile(r'project_elf_src_(\S*)\.c.obj')
     # For back-compatible with make
-    RE_TARGET_MAKE = re.compile(r'^LOAD .*?/xtensa-([^-]+)-elf/')
+    RE_TARGET_MAKE = re.compile(r'^LOAD .*?/xtensa-(esp[^-]+)-elf/')
 
     for line in map_file:
         match_target = RE_TARGET.search(line)
         if match_target:
             return match_target.group(1).lower()
 
         match_target = RE_TARGET_CMAKEv4x.search(line)
```

### Comparing `esp-idf-size-0.3.0/esp_idf_size.egg-info/PKG-INFO` & `esp-idf-size-0.3.1/esp_idf_size.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-size
-Version: 0.3.0
+Version: 0.3.1
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/espressif/esp-idf-size
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-size-0.3.0/esp_idf_size.egg-info/SOURCES.txt` & `esp-idf-size-0.3.1/esp_idf_size.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.0/setup.py` & `esp-idf-size-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-0.3.0/test/test_idf_size.py` & `esp-idf-size-0.3.1/test/test_idf_size.py`

 * *Files identical despite different names*

