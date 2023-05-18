# Comparing `tmp/frat_brain-1.5.1.tar.gz` & `tmp/frat_brain-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frat_brain-1.5.1.tar", max compression
+gzip compressed data, was "frat_brain-1.5.2.tar", max compression
```

## Comparing `frat_brain-1.5.1.tar` & `frat_brain-1.5.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.5.1/LICENSE
--rw-r--r--   0        0        0     3354 2023-05-16 15:38:37.400002 frat_brain-1.5.1/README.md
--rw-r--r--   0        0        0     8196 2023-05-04 14:03:22.213584 frat_brain-1.5.1/fRAT/.DS_Store
--rw-r--r--   0        0        0      228 2023-05-10 16:07:10.854878 frat_brain-1.5.1/fRAT/HOUSE/__init__.py
--rw-r--r--   0        0        0      539 2023-05-17 16:08:32.624385 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6154 2023-05-10 13:02:37.995811 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc
--rw-r--r--   0        0        0     1732 2023-05-09 12:00:42.782332 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc
--rw-r--r--   0        0        0     3402 2023-05-17 16:08:32.709491 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc
--rw-r--r--   0        0        0     2339 2023-05-10 14:23:49.376966 frat_brain-1.5.1/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc
--rw-r--r--   0        0        0     6580 2023-05-10 16:07:10.855691 frat_brain-1.5.1/fRAT/HOUSE/add_motion.py
--rw-r--r--   0        0        0     1836 2023-05-10 16:07:10.856488 frat_brain-1.5.1/fRAT/HOUSE/add_noise.py
--rw-r--r--   0        0        0     4510 2023-05-10 16:07:10.857305 frat_brain-1.5.1/fRAT/HOUSE/handler.py
--rw-r--r--   0        0        0     2047 2023-05-10 16:07:10.858140 frat_brain-1.5.1/fRAT/HOUSE/separate_noise_volumes.py
--rw-r--r--   0        0        0    53981 2023-05-10 16:07:10.859431 frat_brain-1.5.1/fRAT/__main__.py
--rw-r--r--   0        0        0      211 2023-05-17 16:36:50.786298 frat_brain-1.5.1/fRAT/_version.py
--rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.5.1/fRAT/configuration_profiles/latest_settings.toml
--rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.860695 frat_brain-1.5.1/fRAT/configuration_profiles/maps/default_config.toml
--rw-r--r--   0        0        0     4473 2023-05-17 16:16:24.744843 frat_brain-1.5.1/fRAT/configuration_profiles/maps/statmap_config.toml
--rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.862965 frat_brain-1.5.1/fRAT/configuration_profiles/maps/test_config.toml
--rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.864159 frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/default_config.toml
--rw-r--r--   0        0        0    17991 2023-05-17 16:21:31.060646 frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
--rw-r--r--   0        0        0    17405 2023-05-10 16:07:10.866968 frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/test_config.toml
--rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.5.1/fRAT/images/fRAT.gif
--rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.5.1/fRAT/nogui.py
--rw-r--r--   0        0        0     6148 2023-05-04 14:03:22.211954 frat_brain-1.5.1/fRAT/utils/.DS_Store
--rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.5.1/fRAT/utils/__init__.py
--rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.5.1/fRAT/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.5.1/fRAT/utils/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.5.1/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.5.1/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
--rw-r--r--   0        0        0    17651 2023-05-17 16:08:16.861001 frat_brain-1.5.1/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.5.1/fRAT/utils/__pycache__/figures.cpython-310.pyc
--rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.5.1/fRAT/utils/__pycache__/html_report.cpython-310.pyc
--rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.5.1/fRAT/utils/__pycache__/printResults.cpython-310.pyc
--rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.5.1/fRAT/utils/__pycache__/statistics.cpython-310.pyc
--rw-r--r--   0        0        0     9315 2023-05-17 16:16:18.839737 frat_brain-1.5.1/fRAT/utils/__pycache__/statmap.cpython-310.pyc
--rw-r--r--   0        0        0     5726 2023-05-17 16:08:29.826539 frat_brain-1.5.1/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    15234 2023-05-17 16:08:16.669826 frat_brain-1.5.1/fRAT/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.5.1/fRAT/utils/analysis.py
--rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.5.1/fRAT/utils/bootstrap.css
--rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.5.1/fRAT/utils/dash_report.py
--rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.5.1/fRAT/utils/directory_comparison.py
--rw-r--r--   0        0        0    34597 2023-05-10 16:07:10.868291 frat_brain-1.5.1/fRAT/utils/fRAT_config_setup.py
--rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.5.1/fRAT/utils/figures.py
--rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.5.1/fRAT/utils/html_report.py
--rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.5.1/fRAT/utils/printResults.py
--rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.5.1/fRAT/utils/script.js
--rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.5.1/fRAT/utils/statistics.py
--rw-r--r--   0        0        0    13137 2023-05-17 16:16:14.911516 frat_brain-1.5.1/fRAT/utils/statmap.py
--rw-r--r--   0        0        0     9345 2023-05-10 16:07:10.871233 frat_brain-1.5.1/fRAT/utils/statmap_config_setup.py
--rw-r--r--   0        0        0    19156 2023-05-10 16:07:10.917697 frat_brain-1.5.1/fRAT/utils/utils.py
--rw-r--r--   0        0        0     2390 2023-05-17 17:03:36.479842 frat_brain-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     6306 1970-01-01 00:00:00.000000 frat_brain-1.5.1/setup.py
--rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 frat_brain-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.5.2/LICENSE
+-rw-r--r--   0        0        0     3354 2023-05-16 15:38:37.400002 frat_brain-1.5.2/README.md
+-rw-r--r--   0        0        0     8196 2023-05-04 14:03:22.213584 frat_brain-1.5.2/fRAT/.DS_Store
+-rw-r--r--   0        0        0      228 2023-05-10 16:07:10.854878 frat_brain-1.5.2/fRAT/HOUSE/__init__.py
+-rw-r--r--   0        0        0      539 2023-05-17 16:08:32.624385 frat_brain-1.5.2/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6154 2023-05-18 10:54:31.552312 frat_brain-1.5.2/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc
+-rw-r--r--   0        0        0     1732 2023-05-18 10:54:31.593176 frat_brain-1.5.2/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc
+-rw-r--r--   0        0        0     3402 2023-05-17 16:08:32.709491 frat_brain-1.5.2/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc
+-rw-r--r--   0        0        0     2339 2023-05-18 10:54:31.598566 frat_brain-1.5.2/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc
+-rw-r--r--   0        0        0     6580 2023-05-10 16:07:10.855691 frat_brain-1.5.2/fRAT/HOUSE/add_motion.py
+-rw-r--r--   0        0        0     1836 2023-05-10 16:07:10.856488 frat_brain-1.5.2/fRAT/HOUSE/add_noise.py
+-rw-r--r--   0        0        0     4510 2023-05-10 16:07:10.857305 frat_brain-1.5.2/fRAT/HOUSE/handler.py
+-rw-r--r--   0        0        0     2047 2023-05-10 16:07:10.858140 frat_brain-1.5.2/fRAT/HOUSE/separate_noise_volumes.py
+-rw-r--r--   0        0        0    53981 2023-05-10 16:07:10.859431 frat_brain-1.5.2/fRAT/__main__.py
+-rw-r--r--   0        0        0      211 2023-05-17 16:36:50.786298 frat_brain-1.5.2/fRAT/_version.py
+-rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.5.2/fRAT/configuration_profiles/latest_settings.toml
+-rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.860695 frat_brain-1.5.2/fRAT/configuration_profiles/maps/default_config.toml
+-rw-r--r--   0        0        0     4473 2023-05-18 10:54:31.497541 frat_brain-1.5.2/fRAT/configuration_profiles/maps/statmap_config.toml
+-rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.862965 frat_brain-1.5.2/fRAT/configuration_profiles/maps/test_config.toml
+-rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.864159 frat_brain-1.5.2/fRAT/configuration_profiles/roi_analysis/default_config.toml
+-rw-r--r--   0        0        0    17991 2023-05-18 10:46:57.820697 frat_brain-1.5.2/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
+-rw-r--r--   0        0        0    17405 2023-05-10 16:07:10.866968 frat_brain-1.5.2/fRAT/configuration_profiles/roi_analysis/test_config.toml
+-rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.5.2/fRAT/images/fRAT.gif
+-rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.5.2/fRAT/nogui.py
+-rw-r--r--   0        0        0     6148 2023-05-04 14:03:22.211954 frat_brain-1.5.2/fRAT/utils/.DS_Store
+-rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.5.2/fRAT/utils/__init__.py
+-rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.5.2/fRAT/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.5.2/fRAT/utils/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.5.2/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.5.2/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
+-rw-r--r--   0        0        0    17651 2023-05-17 16:08:16.861001 frat_brain-1.5.2/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.5.2/fRAT/utils/__pycache__/figures.cpython-310.pyc
+-rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.5.2/fRAT/utils/__pycache__/html_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.5.2/fRAT/utils/__pycache__/printResults.cpython-310.pyc
+-rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.5.2/fRAT/utils/__pycache__/statistics.cpython-310.pyc
+-rw-r--r--   0        0        0     9315 2023-05-17 16:16:18.839737 frat_brain-1.5.2/fRAT/utils/__pycache__/statmap.cpython-310.pyc
+-rw-r--r--   0        0        0     5726 2023-05-17 16:08:29.826539 frat_brain-1.5.2/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    15290 2023-05-18 10:45:31.348301 frat_brain-1.5.2/fRAT/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.5.2/fRAT/utils/analysis.py
+-rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.5.2/fRAT/utils/bootstrap.css
+-rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.5.2/fRAT/utils/dash_report.py
+-rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.5.2/fRAT/utils/directory_comparison.py
+-rw-r--r--   0        0        0    34597 2023-05-10 16:07:10.868291 frat_brain-1.5.2/fRAT/utils/fRAT_config_setup.py
+-rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.5.2/fRAT/utils/figures.py
+-rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.5.2/fRAT/utils/html_report.py
+-rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.5.2/fRAT/utils/printResults.py
+-rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.5.2/fRAT/utils/script.js
+-rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.5.2/fRAT/utils/statistics.py
+-rw-r--r--   0        0        0    13137 2023-05-17 16:16:14.911516 frat_brain-1.5.2/fRAT/utils/statmap.py
+-rw-r--r--   0        0        0     9345 2023-05-10 16:07:10.871233 frat_brain-1.5.2/fRAT/utils/statmap_config_setup.py
+-rw-r--r--   0        0        0    19312 2023-05-18 10:45:29.419506 frat_brain-1.5.2/fRAT/utils/utils.py
+-rw-r--r--   0        0        0     2390 2023-05-18 10:58:01.856145 frat_brain-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6306 1970-01-01 00:00:00.000000 frat_brain-1.5.2/setup.py
+-rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 frat_brain-1.5.2/PKG-INFO
```

### Comparing `frat_brain-1.5.1/LICENSE` & `frat_brain-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/README.md` & `frat_brain-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/.DS_Store` & `frat_brain-1.5.2/fRAT/.DS_Store`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 12:46:05 2023 UTC, .py size: 6580 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0d92 5b64 b419 0000  o.........[d....
+00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 b419 0000  o.........[d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6402 6c05 5a06 6400 6402 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 5a08 6400 6403 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6404 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 12:00:33 2023 UTC, .py size: 1836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e135 5a64 2c07 0000  o........5Zd,...
+00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 2c07 0000  o.........[d,...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c04 6d05 5a05 0100 6403 5a06 6404  d.l.m.Z...d.Z.d.
 00000050: 5a07 6405 6406 8400 5a08 4700 6407 6408  Z.d.d...Z.G.d.d.
 00000060: 8400 6408 8302 5a09 6401 5300 2909 e900  ..d...Z.d.S.)...
 00000070: 0000 004e 2901 da05 5574 696c 737a 1241  ...N)...Utilsz.A
@@ -67,43 +67,43 @@
 00000420: 6556 616c 7565 732e 6373 76da 0b50 6172  eValues.csv..Par
 00000430: 7469 6369 7061 6e74 7a0f 4e6f 6973 6520  ticipantz.Noise 
 00000440: 6f76 6572 2074 696d 655a 0c5f 6e6f 6973  over timeZ._nois
 00000450: 656c 6576 656c 30fa 012f 2904 da03 6578  elevel0../)...ex
 00000460: 7472 1100 0000 7215 0000 0072 1800 0000  tr....r....r....
 00000470: 6700 0000 0000 0000 0029 03da 036c 6f63  g........)...loc
 00000480: da05 7363 616c 65da 0473 697a 6572 0100  ..scale..sizer..
-00000490: 0000 da0b 5f6e 6f69 7365 6c65 7665 6c29  ...._noiselevel)
+00000490: 0000 5a0b 5f6e 6f69 7365 6c65 7665 6c29  ..Z._noiselevel)
 000004a0: 13da 0270 64da 0872 6561 645f 6373 7672  ...pd..read_csvr
 000004b0: 1200 0000 da05 666c 6f61 7472 1300 0000  ......floatr....
 000004c0: 7202 0000 00da 0a73 6176 655f 6272 6169  r......save_brai
 000004d0: 6e72 1700 0000 7211 0000 0072 1400 0000  nr....r....r....
 000004e0: 7215 0000 0072 1800 0000 720f 0000 00da  r....r....r.....
 000004f0: 116e 6f69 7365 5f6d 756c 7469 706c 6965  .noise_multiplie
 00000500: 7273 da02 6e70 da06 7261 6e64 6f6d da0b  rs..np..random..
 00000510: 6465 6661 756c 745f 726e 67da 066e 6f72  default_rng..nor
 00000520: 6d61 6cda 0573 6861 7065 2906 721a 0000  mal..shape).r...
 00000530: 00da 0f6e 6f69 7365 5f76 616c 7565 5f63  ...noise_value_c
 00000540: 7376 5a17 7061 7274 6963 6970 616e 745f  svZ.participant_
 00000550: 6e6f 6973 655f 6c65 7665 6cda 0a6d 756c  noise_level..mul
 00000560: 7469 706c 6965 725a 0e67 6175 7373 6961  tiplierZ.gaussia
-00000570: 6e5f 6e6f 6973 65da 0a6e 6f69 7379 5f64  n_noise..noisy_d
+00000570: 6e5f 6e6f 6973 655a 0a6e 6f69 7379 5f64  n_noiseZ.noisy_d
 00000580: 6174 6172 0600 0000 7206 0000 0072 0700  atar....r....r..
 00000590: 0000 7219 0000 001b 0000 0073 2400 0000  ..r........s$...
 000005a0: 1202 0201 1401 04ff 0e04 1401 06ff 0c04  ................
 000005b0: 0c01 0601 0601 06fe 0a04 0c01 1202 1401  ................
 000005c0: 08ff 04f8 7a1a 4164 644e 6f69 7365 2e61  ....z.AddNoise.a
 000005d0: 6464 5f6e 6f69 7365 5f74 6f5f 6669 6c65  dd_noise_to_file
 000005e0: 4e29 05da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
 000005f0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 00000600: 6c6e 616d 655f 5f72 1b00 0000 7219 0000  lname__r....r...
 00000610: 0072 0600 0000 7206 0000 0072 0600 0000  .r....r....r....
 00000620: 7207 0000 0072 0300 0000 0e00 0000 7306  r....r........s.
 00000630: 0000 0008 0008 010c 0c72 0300 0000 290a  .........r....).
-00000640: da05 6e75 6d70 7972 2800 0000 da06 7061  ..numpyr(.....pa
-00000650: 6e64 6173 7223 0000 00da 0a66 5241 542e  ndasr#.....fRAT.
+00000640: da05 6e75 6d70 7972 2700 0000 da06 7061  ..numpyr'.....pa
+00000650: 6e64 6173 7222 0000 00da 0a66 5241 542e  ndasr".....fRAT.
 00000660: 7574 696c 7372 0200 0000 da0c 5554 494c  utilsr......UTIL
 00000670: 4954 595f 4e41 4d45 da0b 464f 4c44 4552  ITY_NAME..FOLDER
 00000680: 5f4e 414d 4572 0800 0000 7203 0000 0072  _NAMEr....r....r
 00000690: 0600 0000 7206 0000 0072 0600 0000 7207  ....r....r....r.
 000006a0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
 000006b0: 0073 0e00 0000 0800 0801 0c02 0402 0401  .s..............
 000006c0: 0803 1204                                ....
```

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 14:08:08 2023 UTC, .py size: 2047 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48a5 5b64 ff07 0000  o.......H.[d....
+00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 ff07 0000  o.........[d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6400 6403 6c04 6d05 5a05 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6405 5a08 6406  d.l.m.Z...d.Z.d.
 00000060: 6407 6702 5a09 6408 6409 8400 5a0a 4700  d.g.Z.d.d...Z.G.
 00000070: 640a 640b 8400 640b 8302 5a0b 6402 5300  d.d...d...Z.d.S.
```

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/add_motion.py` & `frat_brain-1.5.2/fRAT/HOUSE/add_motion.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/add_noise.py` & `frat_brain-1.5.2/fRAT/HOUSE/add_noise.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/handler.py` & `frat_brain-1.5.2/fRAT/HOUSE/handler.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/HOUSE/separate_noise_volumes.py` & `frat_brain-1.5.2/fRAT/HOUSE/separate_noise_volumes.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/__main__.py` & `frat_brain-1.5.2/fRAT/__main__.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/configuration_profiles/maps/default_config.toml` & `frat_brain-1.5.2/fRAT/configuration_profiles/maps/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/configuration_profiles/maps/statmap_config.toml` & `frat_brain-1.5.2/fRAT/configuration_profiles/maps/statmap_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/configuration_profiles/maps/test_config.toml` & `frat_brain-1.5.2/fRAT/configuration_profiles/maps/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/default_config.toml` & `frat_brain-1.5.2/fRAT/configuration_profiles/roi_analysis/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml` & `frat_brain-1.5.2/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/configuration_profiles/roi_analysis/test_config.toml` & `frat_brain-1.5.2/fRAT/configuration_profiles/roi_analysis/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/images/fRAT.gif` & `frat_brain-1.5.2/fRAT/images/fRAT.gif`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/nogui.py` & `frat_brain-1.5.2/fRAT/nogui.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/.DS_Store` & `frat_brain-1.5.2/fRAT/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/analysis.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/analysis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/dash_report.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/dash_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/figures.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/html_report.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/html_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/printResults.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/printResults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/statistics.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/statistics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/statmap.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/statmap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/__pycache__/utils.cpython-310.pyc` & `frat_brain-1.5.2/fRAT/utils/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 16:07:10 2023 UTC, .py size: 19156 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2ec1 5b64 d44a 0000  o.........[d.J..
+00000000: 6f0d 0d0a 0000 0000 c901 6664 704b 0000  o.........fdpK..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -236,718 +236,721 @@
 00000eb0: 00da 046c 696e 6572 1400 0000 7214 0000  ...liner....r...
 00000ec0: 0072 1500 0000 da0e 7072 696e 745f 616e  .r......print_an
 00000ed0: 645f 7361 7665 8100 0000 730a 0000 0008  d_save....s.....
 00000ee0: 0204 0108 0114 0104 fd7a 1455 7469 6c73  .........z.Utils
 00000ef0: 2e70 7269 6e74 5f61 6e64 5f73 6176 654e  .print_and_saveN
 00000f00: da03 616c 6cda 0a63 6f6e 6669 675f 6c6f  ..all..config_lo
 00000f10: 6763 0600 0000 0000 0000 0000 0000 0a00  gc..............
-00000f20: 0000 0900 0000 4300 0000 7320 0100 0074  ......C...s ...t
+00000f20: 0000 0900 0000 4300 0000 733e 0100 0074  ......C...s>...t
 00000f30: 007c 009b 0064 017c 059b 0064 029d 0464  .|...d.|...d...d
-00000f40: 0383 028f 7b7d 0674 007c 019b 0064 017c  ....{}.t.|...d.|
-00000f50: 029b 009d 0364 0483 028f 587d 077c 06a0  .....d....X}.|..
+00000f40: 0383 028f 8a7d 0674 007c 019b 0064 017c  .....}.t.|...d.|
+00000f50: 029b 009d 0364 0483 028f 677d 077c 06a0  .....d....g}.|..
 00000f60: 0164 0574 029b 0064 067c 029b 0064 079d  .d.t...d.|...d..
 00000f70: 05a1 0101 007c 0372 347c 0344 005d 077d  .....|.r4|.D.].}
 00000f80: 087c 06a0 017c 08a1 0101 0071 277c 06a0  .|...|.....q'|..
 00000f90: 0164 08a1 0101 007c 06a0 0164 08a1 0101  .d.....|...d....
-00000fa0: 0064 007d 097c 0744 005d 297d 087c 08a0  .d.}.|.D.])}.|..
+00000fa0: 0064 007d 097c 0744 005d 387d 087c 08a0  .d.}.|.D.]8}.|..
 00000fb0: 0364 09a1 0172 537c 08a0 0364 0aa1 0173  .d...rS|...d...s
 00000fc0: 537c 08a0 0464 0964 0ba1 0264 0c64 0d85  S|...d.d...d.d..
-00000fd0: 0219 007d 097c 0464 0e6b 0272 5d7c 06a0  ...}.|.d.k.r]|..
-00000fe0: 017c 08a1 0101 0071 3d7c 097c 0476 0072  .|.....q=|.|.v.r
-00000ff0: 667c 06a0 017c 08a1 0101 0071 3d57 0064  f|...|.....q=W.d
-00001000: 0004 0004 0083 0301 006e 1031 0073 7177  .........n.1.sqw
-00001010: 0101 0001 0001 0059 0001 0057 0064 0004  .......Y...W.d..
-00001020: 0004 0083 0301 0064 0053 0057 0064 0004  .......d.S.W.d..
-00001030: 0004 0083 0301 0064 0053 0031 0073 8977  .......d.S.1.s.w
-00001040: 0101 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
-00001050: 0f4e fa01 2f7a 052e 746f 6d6c da01 77da  .N../z..toml..w.
-00001060: 0172 7a20 2320 4765 6e65 7261 6c20 696e  .rz # General in
-00001070: 666f 726d 6174 696f 6e0a 7665 7273 696f  formation.versio
-00001080: 6e20 3d20 7a15 0a63 6f6e 6669 675f 6669  n = z..config_fi
-00001090: 6c65 5f75 7365 6420 3d20 277a 0227 0a72  le_used = 'z.'.r
-000010a0: 5b00 0000 fa01 237a 0223 2372 2300 0000  [.....#z.##r#...
-000010b0: 721e 0000 00e9 ffff ffff 7261 0000 0029  r.........ra...)
-000010c0: 05da 046f 7065 6e72 5c00 0000 da07 7665  ...openr\.....ve
-000010d0: 7273 696f 6eda 0a73 7461 7274 7377 6974  rsion..startswit
-000010e0: 6872 2a00 0000 290a 5a06 6e65 7764 6972  hr*...).Z.newdir
-000010f0: da0b 636f 6e66 6967 5f70 6174 68da 0f63  ..config_path..c
-00001100: 6f6e 6669 675f 6669 6c65 6e61 6d65 5a0f  onfig_filenameZ.
-00001110: 6164 6469 7469 6f6e 616c 5f69 6e66 6fda  additional_info.
-00001120: 1172 656c 6576 616e 745f 7365 6374 696f  .relevant_sectio
-00001130: 6e73 da0f 6e65 775f 636f 6e66 6967 5f6e  ns..new_config_n
-00001140: 616d 6572 3800 0000 7265 0000 0072 5f00  amer8...re...r_.
-00001150: 0000 5a0f 6375 7272 656e 745f 7365 6374  ..Z.current_sect
-00001160: 696f 6e72 1400 0000 7214 0000 0072 1500  ionr....r....r..
-00001170: 0000 da0b 7361 7665 5f63 6f6e 6669 6788  ....save_config.
-00001180: 0000 0073 2c00 0000 2e02 0601 0201 04ff  ...s,...........
-00001190: 0202 0afe 0404 0801 0c01 0a02 0a02 0402  ................
-000011a0: 0801 1401 1401 0802 0c01 0801 0a01 0280  ................
-000011b0: 02f9 50f2 7a11 5574 696c 732e 7361 7665  ..P.z.Utils.save
-000011c0: 5f63 6f6e 6669 6754 6306 0000 0000 0000  _configTc.......
-000011d0: 0000 0000 0007 0000 0006 0000 0043 0000  .............C..
-000011e0: 0073 9c00 0000 7c01 a000 6401 a101 7309  .s....|...d...s.
-000011f0: 7c01 6401 3700 7d01 7c02 a000 6401 a101  |.d.7.}.|...d...
-00001200: 7312 7c02 6401 3700 7d02 7c05 7217 6402  s.|.d.7.}.|.r.d.
-00001210: 7d06 6e02 7c00 7d06 7c03 723e 7c04 722e  }.n.|.}.|.r>|.r.
-00001220: 7401 a002 7c01 9b00 7c00 9b00 9d02 7c02  t...|...|.....|.
-00001230: 9b00 6403 7c06 9b00 9d03 a102 0100 6400  ..d.|.........d.
-00001240: 5300 7401 a002 7c01 9b00 7c00 9b00 9d02  S.t...|...|.....
-00001250: 7c02 9b00 7c06 9b00 9d02 a102 0100 6400  |...|.........d.
-00001260: 5300 7403 a004 7c01 9b00 7c00 9b00 9d02  S.t...|...|.....
-00001270: 7c02 9b00 7c06 9b00 9d02 a102 0100 6400  |...|.........d.
-00001280: 5300 2904 4e72 6300 0000 7a0f 7061 7261  S.).Nrc...z.para
-00001290: 6d56 616c 7565 732e 6373 765a 0563 6f70  mValues.csvZ.cop
-000012a0: 795f 2905 da08 656e 6473 7769 7468 da06  y_)...endswith..
-000012b0: 7368 7574 696c da04 636f 7079 7234 0000  shutil..copyr4..
-000012c0: 00da 0672 656e 616d 6529 07da 086f 6c64  ...rename)...old
-000012d0: 5f6e 616d 655a 0c6f 7269 6769 6e61 6c5f  _nameZ.original_
-000012e0: 6469 725a 076e 6577 5f64 6972 7272 0000  dirZ.new_dirrr..
-000012f0: 00da 0b72 656e 616d 655f 636f 7079 da0e  ...rename_copy..
-00001300: 7061 7261 6d65 7465 725f 6669 6c65 da08  parameter_file..
-00001310: 6e65 775f 6e61 6d65 7214 0000 0072 1400  new_namer....r..
-00001320: 0000 7215 0000 00da 096d 6f76 655f 6669  ..r......move_fi
-00001330: 6c65 a100 0000 7318 0000 000a 0208 010a  le....s.........
-00001340: 0208 0104 0206 0104 0204 0204 0122 0120  .............". 
-00001350: 0220 027a 0f55 7469 6c73 2e6d 6f76 655f  . .z.Utils.move_
-00001360: 6669 6c65 6302 0000 0000 0000 0000 0000  filec...........
-00001370: 0002 0000 0003 0000 0043 0000 0073 4600  .........C...sF.
-00001380: 0000 7c01 7214 7400 6a01 a002 7c00 a101  ..|.r.t.j...|...
-00001390: 7214 7403 a004 7c00 a101 0100 7405 a006  r.t...|.....t...
-000013a0: 7c00 a101 0100 6400 5300 7400 6a01 a002  |.....d.S.t.j...
-000013b0: 7c00 a101 7321 7405 a006 7c00 a101 0100  |...s!t...|.....
-000013c0: 6400 5300 6400 5300 7241 0000 0029 0772  d.S.d.S.rA...).r
-000013d0: 3400 0000 7235 0000 00da 0665 7869 7374  4...r5.....exist
-000013e0: 7372 7100 0000 da06 726d 7472 6565 7208  srq.....rmtreer.
-000013f0: 0000 00da 066d 6b5f 6469 7229 0272 3500  .....mk_dir).r5.
-00001400: 0000 da0a 6465 6c65 7465 5f6f 6c64 7214  ....delete_oldr.
-00001410: 0000 0072 1400 0000 7215 0000 00da 1263  ...r....r......c
-00001420: 6865 636b 5f61 6e64 5f6d 616b 655f 6469  heck_and_make_di
-00001430: 72b6 0000 0073 0c00 0000 1002 0a01 0e01  r....s..........
-00001440: 0c02 0e01 04ff 7a18 5574 696c 732e 6368  ......z.Utils.ch
-00001450: 6563 6b5f 616e 645f 6d61 6b65 5f64 6972  eck_and_make_dir
-00001460: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
-00001470: 0008 0000 0003 0000 0073 4201 0000 7c02  .........sB...|.
-00001480: 6401 6b02 7269 6700 7d03 7400 6402 8301  d.k.rig.}.t.d...
-00001490: 0100 7401 8800 8301 4400 5d0d 5c02 7d04  ..t.....D.].\.}.
-000014a0: 7d05 7400 6403 6a02 7c04 7c05 6404 8d02  }.t.d.j.|.|.d...
-000014b0: 8301 0100 710e 7c03 7368 7400 6405 7c01  ....q.|.sht.d.|.
-000014c0: 9b00 6406 9d03 8301 0100 7403 6407 8301  ..d.......t.d...
-000014d0: 7d06 7c06 a004 a100 6408 6b02 723a 7405  }.|.....d.k.r:t.
-000014e0: 7406 6409 7407 8800 8301 8302 8301 7d03  t.d.t.........}.
-000014f0: 6e2c 7407 7c06 8301 6409 6b04 7263 640a  n,t.|...d.k.rcd.
-00001500: 640b 8400 7c06 a008 640c a101 4400 8301  d...|...d...D...
-00001510: 7d03 7a09 7405 7409 740a 7c03 8302 8301  }.z.t.t.t.|.....
-00001520: 7d03 5700 6e12 0400 740b 7962 0100 0100  }.W.n...t.yb....
-00001530: 0100 7400 640d 8301 0100 6700 7d03 5900  ..t.d.....g.}.Y.
-00001540: 6e04 7700 6700 7d03 7196 7c03 721e 6e2d  n.w.g.}.q.|.r.n-
-00001550: 740c 7c02 7405 8302 7287 740c 7c02 6409  t.|.t...r.t.|.d.
-00001560: 1900 740d 8302 7287 7c02 6409 1900 a004  ..t...r.|.d.....
-00001570: a100 6408 6b02 7287 7405 7406 6409 7407  ..d.k.r.t.t.d.t.
-00001580: 8800 8301 8302 8301 7d03 6e0f 7c02 7d03  ........}.n.|.}.
-00001590: 740c 7c03 740a 8302 7292 7c03 6701 7d03  t.|.t...r.|.g.}.
-000015a0: 6e04 7405 7c03 8301 7d03 8700 6601 640e  n.t.|...}...f.d.
-000015b0: 640b 8408 7c03 4400 8301 7d03 7c03 5300  d...|.D...}.|.S.
-000015c0: 290f 4eda 0752 756e 7469 6d65 725b 0000  ).N..Runtimer[..
-000015d0: 007a 107b 726f 695f 6e75 6d7d 3a20 7b72  .z.{roi_num}: {r
-000015e0: 6f69 7d29 02da 0772 6f69 5f6e 756d da03  oi})...roi_num..
-000015f0: 726f 697a 050a 2d2d 2d20 7a0d 2063 7265  roiz..--- z. cre
-00001600: 6174 696f 6e20 2d2d 2d7a b854 7970 6520  ation ---z.Type 
-00001610: 6120 636f 6d6d 612d 7365 7061 7261 7465  a comma-separate
-00001620: 6420 6c69 7374 206f 6620 7468 6520 524f  d list of the RO
-00001630: 4973 2028 6c69 7374 6564 2061 626f 7665  Is (listed above
-00001640: 2920 796f 7520 7761 6e74 2074 6f20 7072  ) you want to pr
-00001650: 6f64 7563 6520 6120 6669 6775 7265 2066  oduce a figure f
-00001660: 6f72 2c20 2765 2e67 2e20 322c 2031 352c  or, 'e.g. 2, 15,
-00001670: 2037 2c20 3233 2720 6f72 2027 616c 6c27   7, 23' or 'all'
-00001680: 2066 6f72 2061 6c6c 2072 6f69 732e 200a   for all rois. .
-00001690: 416c 7465 726e 6174 6976 656c 7920 7072  Alternatively pr
-000016a0: 6573 7320 656e 7465 7220 7477 6963 6520  ess enter twice 
-000016b0: 746f 2073 6b69 7020 7468 6973 2073 7465  to skip this ste
-000016c0: 703a 2072 6100 0000 7201 0000 0063 0100  p: ra...r....c..
-000016d0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000016e0: 0000 5300 0000 f314 0000 0067 007c 005d  ..S........g.|.]
-000016f0: 067d 017c 01a0 00a1 0091 0271 0253 0072  .}.|.......q.S.r
-00001700: 1400 0000 2901 da05 7374 7269 70a9 0272  ....)...strip..r
-00001710: 3700 0000 7213 0000 0072 1400 0000 7214  7...r....r....r.
-00001720: 0000 0072 1500 0000 7239 0000 00d2 0000  ...r....r9......
-00001730: 00f3 0200 0000 1400 7a2a 5574 696c 732e  ........z*Utils.
-00001740: 6669 6e64 5f63 686f 7365 6e5f 726f 6973  find_chosen_rois
-00001750: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00001760: 6f6d 703e fa01 2c7a 2c43 6f6d 6d61 2d73  omp>..,z,Comma-s
-00001770: 6570 6172 6174 6564 206c 6973 7420 636f  eparated list co
-00001780: 6e74 6169 6e73 206e 6f6e 2069 6e74 6567  ntains non integ
-00001790: 6572 732e 0a63 0100 0000 0000 0000 0000  ers..c..........
-000017a0: 0000 0200 0000 0400 0000 1300 0000 7314  ..............s.
-000017b0: 0000 0067 007c 005d 067d 0188 007c 0119  ...g.|.].}...|..
-000017c0: 0091 0271 0253 0072 1400 0000 7214 0000  ...q.S.r....r...
-000017d0: 0029 0272 3700 0000 5a0a 726f 695f 6e75  .).r7...Z.roi_nu
-000017e0: 6d62 6572 a901 da08 616c 6c5f 726f 6973  mber....all_rois
-000017f0: 7214 0000 0072 1500 0000 7239 0000 00ea  r....r....r9....
-00001800: 0000 0072 8400 0000 290e 7258 0000 00da  ...r....).rX....
-00001810: 0965 6e75 6d65 7261 7465 da06 666f 726d  .enumerate..form
-00001820: 6174 da05 696e 7075 74da 056c 6f77 6572  at..input..lower
-00001830: 7210 0000 00da 0572 616e 6765 da03 6c65  r......range..le
-00001840: 6eda 0573 706c 6974 da03 6d61 70da 0369  n..split..map..i
-00001850: 6e74 7211 0000 0072 0e00 0000 725d 0000  ntr....r....r]..
-00001860: 0029 0772 8700 0000 da09 6675 6e63 5f6e  .).r......func_n
-00001870: 616d 655a 1163 6f6e 6669 675f 7265 6769  ameZ.config_regi
-00001880: 6f6e 5f76 6172 5a0b 6368 6f73 656e 5f72  on_varZ.chosen_r
-00001890: 6f69 7372 7f00 0000 7280 0000 005a 0772  oisr....r....Z.r
-000018a0: 6f69 5f61 6e73 7214 0000 0072 8600 0000  oi_ansr....r....
-000018b0: 7215 0000 00da 1066 696e 645f 6368 6f73  r......find_chos
-000018c0: 656e 5f72 6f69 73bf 0000 0073 4400 0000  en_rois....sD...
-000018d0: 0802 0401 0801 1002 1401 0402 1001 0201  ................
-000018e0: 0201 04ff 0c04 1401 0c02 1401 0202 1201  ................
-000018f0: 0c01 0801 0801 02fe 0405 0201 04ec 0280  ................
-00001900: 1817 0e01 02ff 1402 0402 0a02 0801 0802  ................
-00001910: 1202 0402 7a16 5574 696c 732e 6669 6e64  ....z.Utils.find
-00001920: 5f63 686f 7365 6e5f 726f 6973 6302 0000  _chosen_roisc...
-00001930: 0000 0000 0000 0000 0004 0000 0008 0000  ................
-00001940: 0043 0000 0073 7e00 0000 7400 a001 a100  .C...s~...t.....
-00001950: 7d02 6401 7d03 7a1f 7c01 6402 6b02 7216  }.d.}.z.|.d.k.r.
-00001960: 7c00 9b00 6403 9d02 7d03 7400 a002 7c03  |...d...}.t...|.
-00001970: a101 7d02 6e0e 7c01 6404 6b02 7224 7c00  ..}.n.|.d.k.r$|.
-00001980: 9b00 6405 9d02 7d03 7400 a002 7c03 a101  ..d...}.t...|...
-00001990: 7d02 5700 6e10 0400 7403 7935 0100 0100  }.W.n...t.y5....
-000019a0: 0100 7404 6406 7405 6a06 9b00 6407 9d03  ..t.d.t.j...d...
-000019b0: 8301 8201 7700 7c02 a007 6408 a101 7d02  ....w.|...d...}.
-000019c0: 7c02 7c03 6602 5300 2909 4e72 2300 0000  |.|.f.S.).Nr#...
-000019d0: fa10 5365 7373 696f 6e20 6176 6572 6167  ..Session averag
-000019e0: 6564 7a4a 2f4f 7665 7261 6c6c 2f53 756d  edzJ/Overall/Sum
-000019f0: 6d61 7269 7365 645f 7265 7375 6c74 732f  marised_results/
-00001a00: 5365 7373 696f 6e5f 6176 6572 6167 6564  Session_averaged
-00001a10: 5f72 6573 756c 7473 2f63 6f6d 6269 6e65  _results/combine
-00001a20: 645f 7265 7375 6c74 732e 6a73 6f6e fa14  d_results.json..
-00001a30: 5061 7274 6963 6970 616e 7420 6176 6572  Participant aver
-00001a40: 6167 6564 7a4e 2f4f 7665 7261 6c6c 2f53  agedzN/Overall/S
-00001a50: 756d 6d61 7269 7365 645f 7265 7375 6c74  ummarised_result
-00001a60: 732f 5061 7274 6963 6970 616e 745f 6176  s/Participant_av
-00001a70: 6572 6167 6564 5f72 6573 756c 7473 2f63  eraged_results/c
-00001a80: 6f6d 6269 6e65 645f 7265 7375 6c74 732e  ombined_results.
-00001a90: 6a73 6f6e 7a23 636f 6d62 696e 6564 5f72  jsonz#combined_r
-00001aa0: 6573 756c 7473 2e6a 736f 6e20 6e6f 7420  esults.json not 
-00001ab0: 666f 756e 6420 696e 207a 0820 666f 6c64  found in z. fold
-00001ac0: 6572 2e72 4a00 0000 2908 724c 0000 0072  er.rJ...).rL...r
-00001ad0: 4d00 0000 da09 7265 6164 5f6a 736f 6e72  M.....read_jsonr
-00001ae0: 1100 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
-00001af0: 5600 0000 da0e 6176 6572 6167 696e 675f  V.....averaging_
-00001b00: 7479 7065 da0b 736f 7274 5f76 616c 7565  type..sort_value
-00001b10: 7329 04da 0666 6f6c 6465 7272 9700 0000  s)...folderr....
-00001b20: da02 6466 7235 0000 0072 1400 0000 7214  ..dfr5...r....r.
-00001b30: 0000 0072 1500 0000 da15 7265 6164 5f63  ...r......read_c
-00001b40: 6f6d 6269 6e65 645f 7265 7375 6c74 73ee  ombined_results.
-00001b50: 0000 0073 1e00 0000 0802 0401 0202 0801  ...s............
-00001b60: 0a01 0c01 0802 0a01 0a01 0480 0c02 1201  ................
-00001b70: 02ff 0a03 0802 7a1b 5574 696c 732e 7265  ......z.Utils.re
-00001b80: 6164 5f63 6f6d 6269 6e65 645f 7265 7375  ad_combined_resu
-00001b90: 6c74 7363 0100 0000 0000 0000 0000 0000  ltsc............
-00001ba0: 0500 0000 0900 0000 0300 0000 73c2 0000  ............s...
-00001bb0: 0064 0164 0284 007c 006a 0044 0083 017c  .d.d...|.j.D...|
-00001bc0: 005f 0074 0164 0364 0484 0074 027c 006a  ._.t.d.d...t.|.j
-00001bd0: 0083 0144 0083 0164 0583 027d 0174 0164  ...D...d...}.t.d
-00001be0: 0664 0484 0074 027c 006a 0083 0144 0083  .d...t.|.j...D..
-00001bf0: 0164 0583 027d 027c 0273 2e74 0364 0774  .d...}.|.s.t.d.t
-00001c00: 046a 059b 0064 089d 0383 0182 0167 007d  .j...d.......g.}
-00001c10: 0374 046a 0644 005d 2889 0074 0187 0066  .t.j.D.](..t...f
-00001c20: 0164 0964 0484 0874 027c 006a 0083 0144  .d.d...t.|.j...D
-00001c30: 0083 0164 0583 027d 047c 0472 4c7c 03a0  ...d...}.|.rL|..
-00001c40: 077c 04a1 0101 0071 3374 0864 0a88 009b  .|.....q3t.d....
-00001c50: 0064 0b74 046a 059b 0064 0c74 046a 059b  .d.t.j...d.t.j..
-00001c60: 0064 0d9d 0783 0182 017c 017c 037c 0266  .d.......|.|.|.f
-00001c70: 0353 0029 0e4e 6301 0000 0000 0000 0000  .S.).Nc.........
-00001c80: 0000 0002 0000 0004 0000 0053 0000 0072  ...........S...r
-00001c90: 8100 0000 7214 0000 00a9 0172 8b00 0000  ....r......r....
-00001ca0: 7283 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-00001cb0: 1500 0000 7239 0000 0005 0100 0072 8400  ....r9.......r..
-00001cc0: 0000 7a2a 5574 696c 732e 6669 6e64 5f63  ..z*Utils.find_c
-00001cd0: 6f6c 756d 6e5f 6c6f 6373 2e3c 6c6f 6361  olumn_locs.<loca
-00001ce0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
-00001cf0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00001d00: 0000 0073 0000 00f3 2000 0000 8100 7c00  ...s.... .....|.
-00001d10: 5d0b 5c02 7d01 7d02 6400 7c02 7600 7202  ].\.}.}.d.|.v.r.
-00001d20: 7c01 5600 0100 7102 6401 5300 2902 7a0b  |.V...q.d.S.).z.
-00001d30: 6967 6e6f 7265 2066 696c 654e 7214 0000  ignore fileNr...
-00001d40: 00a9 0372 3700 0000 da07 636f 756e 7465  ...r7.....counte
-00001d50: 7272 4800 0000 7214 0000 0072 1400 0000  rrH...r....r....
-00001d60: 7215 0000 00da 093c 6765 6e65 7870 723e  r......<genexpr>
-00001d70: 0701 0000 7304 0000 0002 801e 007a 2955  ....s........z)U
-00001d80: 7469 6c73 2e66 696e 645f 636f 6c75 6d6e  tils.find_column
-00001d90: 5f6c 6f63 732e 3c6c 6f63 616c 733e 2e3c  _locs.<locals>.<
-00001da0: 6765 6e65 7870 723e 4663 0100 0000 0000  genexpr>Fc......
-00001db0: 0000 0000 0000 0300 0000 0300 0000 7300  ..............s.
-00001dc0: 0000 729d 0000 0029 02da 0862 6173 656c  ..r....)...basel
-00001dd0: 696e 654e 7214 0000 0072 9e00 0000 7214  ineNr....r....r.
-00001de0: 0000 0072 1400 0000 7215 0000 0072 a000  ...r....r....r..
-00001df0: 0000 0a01 0000 7308 0000 0002 800a 0006  ......s.........
-00001e00: 010e ff7a 1c4e 6f20 6261 7365 6c69 6e65  ...z.No baseline
-00001e10: 2063 6f6c 756d 6e20 666f 756e 6420 696e   column found in
-00001e20: 2072 3300 0000 6301 0000 0000 0000 0000   r3...c.........
-00001e30: 0000 0003 0000 0003 0000 0033 0000 0073  ...........3...s
-00001e40: 2400 0000 8100 7c00 5d0d 5c02 7d01 7d02  $.....|.].\.}.}.
-00001e50: 8800 a000 a100 7c02 6b02 7202 7c01 5600  ......|.k.r.|.V.
-00001e60: 0100 7102 6400 5300 7241 0000 0072 9c00  ..q.d.S.rA...r..
-00001e70: 0000 729e 0000 00a9 01da 036b 6579 7214  ..r........keyr.
-00001e80: 0000 0072 1500 0000 72a0 0000 0011 0100  ...r....r.......
-00001e90: 0073 0400 0000 0280 2200 7a05 4b65 7920  .s......".z.Key 
-00001ea0: 227a 0f22 206e 6f74 2066 6f75 6e64 2069  "z." not found i
-00001eb0: 6e20 7a76 2e20 4368 6563 6b20 7468 6520  n zv. Check the 
-00001ec0: 4372 6974 6963 616c 2050 6172 616d 6574  Critical Paramet
-00001ed0: 6572 7320 6f70 7469 6f6e 2069 6e20 7468  ers option in th
-00001ee0: 6520 5061 7273 696e 6720 6d65 6e75 2028  e Parsing menu (
-00001ef0: 7061 7261 6d65 7465 725f 6469 6374 3120  parameter_dict1 
-00001f00: 6966 206e 6f74 2075 7369 6e67 2074 6865  if not using the
-00001f10: 2047 5549 2920 636f 7272 6563 746c 7920   GUI) correctly 
-00001f20: 6d61 7463 6820 7468 6520 7a09 2068 6561  match the z. hea
-00001f30: 6465 7273 2e29 0972 4200 0000 da04 6e65  ders.).rB.....ne
-00001f40: 7874 7288 0000 00da 094e 616d 6545 7272  xtr......NameErr
-00001f50: 6f72 7256 0000 0072 7600 0000 da0e 7061  orrV...rv.....pa
-00001f60: 7261 6d65 7465 725f 6469 6374 da06 6170  rameter_dict..ap
-00001f70: 7065 6e64 7296 0000 0029 05da 0574 6162  pendr....)...tab
-00001f80: 6c65 da11 6967 6e6f 7265 5f63 6f6c 756d  le..ignore_colum
-00001f90: 6e5f 6c6f 635a 1362 6173 656c 696e 655f  n_locZ.baseline_
-00001fa0: 636f 6c75 6d6e 5f6c 6f63 da14 6372 6974  column_loc..crit
-00001fb0: 6963 616c 5f63 6f6c 756d 6e5f 6c6f 6373  ical_column_locs
-00001fc0: 5a0a 636f 6c75 6d6e 5f6c 6f63 7214 0000  Z.column_locr...
-00001fd0: 0072 a200 0000 7215 0000 00da 1066 696e  .r....r......fin
-00001fe0: 645f 636f 6c75 6d6e 5f6c 6f63 7303 0100  d_column_locs...
-00001ff0: 0073 2400 0000 1202 1402 0201 04ff 1403  .s$.............
-00002000: 0201 04ff 0402 1201 0402 0a01 1e01 0402  ................
-00002010: 0c01 1202 0402 0afe 0a04 7a16 5574 696c  ..........z.Util
-00002020: 732e 6669 6e64 5f63 6f6c 756d 6e5f 6c6f  s.find_column_lo
-00002030: 6373 6301 0000 0000 0000 0000 0000 0004  csc.............
-00002040: 0000 0008 0000 0043 0000 0073 8200 0000  .......C...s....
-00002050: 7c00 7205 7c00 7d01 6e04 7400 a001 a100  |.r.|.}.n.t.....
-00002060: 7d01 7400 6a02 a003 7c01 9b00 6401 7404  }.t.j...|...d.t.
-00002070: 6a05 9b00 9d03 a101 7226 7406 a007 7c01  j.......r&t...|.
-00002080: 9b00 6401 7404 6a05 9b00 9d03 a101 7d02  ..d.t.j.......}.
-00002090: 6402 7d03 7c02 7c03 6602 5300 7a0f 7406  d.}.|.|.f.S.z.t.
-000020a0: a007 7c01 9b00 6403 9d02 a101 7d02 6404  ..|...d.....}.d.
-000020b0: 7d03 5700 7c02 7c03 6602 5300 0400 7408  }.W.|.|.f.S...t.
-000020c0: 7940 0100 0100 0100 7409 6405 8301 8201  y@......t.d.....
-000020d0: 7700 2906 4e72 6300 0000 da0b 6261 7365  w.).Nrc.....base
-000020e0: 5f66 6f6c 6465 727a 152f 636f 7079 5f70  _folderz./copy_p
-000020f0: 6172 616d 5661 6c75 6573 2e63 7376 da0d  aramValues.csv..
-00002100: 7265 706f 7274 5f66 6f6c 6465 727a b34d  report_folderz.M
-00002110: 616b 6520 7375 7265 2061 2063 6f70 7920  ake sure a copy 
-00002120: 6f66 2070 6172 616d 5661 6c75 6573 2e63  of paramValues.c
-00002130: 7376 2069 7320 696e 2074 6865 2063 686f  sv is in the cho
-00002140: 7365 6e20 666f 6c64 6572 2e20 0a41 6c73  sen folder. .Als
-00002150: 6f20 6d61 6b65 2073 7572 6520 7468 6520  o make sure the 
-00002160: 7365 6c65 6374 6564 2066 6f6c 6465 7220  selected folder 
-00002170: 636f 6e74 6169 6e73 2061 6c6c 2074 6865  contains all the
-00002180: 2070 6172 7469 6369 7061 6e74 2064 6972   participant dir
-00002190: 6563 746f 7269 6573 2069 6e20 7468 6520  ectories in the 
-000021a0: 6e65 6365 7373 6172 7920 4249 4453 2066  necessary BIDS f
-000021b0: 6f72 6d61 7420 652e 672e 2073 7562 2d30  ormat e.g. sub-0
-000021c0: 312e 290a 7234 0000 00da 0667 6574 6377  1.).r4.....getcw
-000021d0: 6472 3500 0000 da06 6973 6669 6c65 7256  dr5.....isfilerV
-000021e0: 0000 0072 7600 0000 724c 0000 00da 0872  ...rv...rL.....r
-000021f0: 6561 645f 6373 7672 5400 0000 7296 0000  ead_csvrT...r...
-00002200: 0029 0472 3c00 0000 7299 0000 0072 a800  .).r<...r....r..
-00002210: 0000 da0b 666f 6c64 6572 5f74 7970 6572  ....folder_typer
-00002220: 1400 0000 7214 0000 0072 1500 0000 da15  ....r....r......
-00002230: 6c6f 6164 5f70 6172 616d 5661 6c75 6573  load_paramValues
-00002240: 5f66 696c 651c 0100 0073 1c00 0000 0402  _file....s......
-00002250: 0601 0802 1802 1601 0401 080c 02f7 1001  ................
-00002260: 0601 0807 0cfb 0801 02ff 7a1b 5574 696c  ..........z.Util
-00002270: 732e 6c6f 6164 5f70 6172 616d 5661 6c75  s.load_paramValu
-00002280: 6573 5f66 696c 6563 0100 0000 0000 0000  es_filec........
-00002290: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
-000022a0: 7326 0000 007a 0874 00a0 017c 00a1 0101  s&...z.t...|....
-000022b0: 0057 0064 0053 0004 0074 0279 1201 0001  .W.d.S...t.y....
-000022c0: 0001 0059 0064 0053 0077 0072 4100 0000  ...Y.d.S.w.rA...
-000022d0: 2903 7234 0000 00da 056d 6b64 6972 da0f  ).r4.....mkdir..
-000022e0: 4669 6c65 4578 6973 7473 4572 726f 7229  FileExistsError)
-000022f0: 0172 3500 0000 7214 0000 0072 1400 0000  .r5...r....r....
-00002300: 7215 0000 0072 7b00 0000 3301 0000 730a  r....r{...3...s.
-00002310: 0000 0002 0210 010c 0106 0102 ff7a 0c55  .............z.U
-00002320: 7469 6c73 2e6d 6b5f 6469 7263 0000 0000  tils.mk_dirc....
-00002330: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00002340: 4700 0000 731e 0000 0074 007c 0064 0119  G...s....t.|.d..
-00002350: 007c 0064 0219 0083 027c 0064 0364 0085  .|.d.....|.d.d..
-00002360: 0219 008e 0053 0029 044e 7201 0000 0072  .....S.).Nr....r
-00002370: 1e00 0000 e902 0000 0029 01da 0767 6574  .........)...get
-00002380: 6174 7472 a901 da04 6172 6776 7214 0000  attr....argvr...
-00002390: 0072 1400 0000 7215 0000 00da 1769 6e73  .r....r......ins
-000023a0: 7461 6e63 655f 6d65 7468 6f64 5f68 616e  tance_method_han
-000023b0: 646c 6572 3a01 0000 7302 0000 001e 027a  dler:...s......z
-000023c0: 1d55 7469 6c73 2e69 6e73 7461 6e63 655f  .Utils.instance_
-000023d0: 6d65 7468 6f64 5f68 616e 646c 6572 6300  method_handlerc.
-000023e0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000023f0: 0000 0047 0000 0073 1400 0000 7c00 6401  ...G...s....|.d.
-00002400: 1900 7c00 6402 6400 8502 1900 8e00 5300  ..|.d.d.......S.
-00002410: 2903 4e72 0100 0000 721e 0000 0072 1400  ).Nr....r....r..
-00002420: 0000 72b7 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00002430: 0072 1500 0000 da14 636c 6173 735f 6d65  .r......class_me
-00002440: 7468 6f64 5f68 616e 646c 6572 3e01 0000  thod_handler>...
-00002450: 7251 0000 007a 1a55 7469 6c73 2e63 6c61  rQ...z.Utils.cla
-00002460: 7373 5f6d 6574 686f 645f 6861 6e64 6c65  ss_method_handle
-00002470: 7263 0100 0000 0000 0000 0000 0000 0300  rc..............
-00002480: 0000 0400 0000 4300 0000 734e 0000 0074  ......C...sN...t
-00002490: 006a 0164 016b 0272 0a74 02a0 03a1 007d  .j.d.k.r.t.....}
-000024a0: 016e 0574 0474 006a 0183 017d 0174 02a0  .n.t.t.j...}.t..
-000024b0: 0564 02a1 017d 0274 006a 0672 217c 0073  .d...}.t.j.r!|.s
-000024c0: 2174 0764 037c 019b 0064 049d 0383 0101  !t.d.|...d......
-000024d0: 007c 026a 087c 0164 058d 0153 0029 064e  .|.j.|.d...S.).N
-000024e0: da03 6d61 78da 0a66 6f72 6b73 6572 7665  ..max..forkserve
-000024f0: 727a 200a 5374 6172 7469 6e67 2070 726f  rz .Starting pro
-00002500: 6365 7373 696e 6720 706f 6f6c 2075 7369  cessing pool usi
-00002510: 6e67 207a 0720 636f 7265 732e 2901 da09  ng z. cores.)...
-00002520: 7072 6f63 6573 7365 7329 0972 5600 0000  processes).rV...
-00002530: 5a0e 6d61 785f 636f 7265 5f75 7361 6765  Z.max_core_usage
-00002540: da02 6d70 da09 6370 755f 636f 756e 7472  ..mp..cpu_countr
-00002550: 9000 0000 da0b 6765 745f 636f 6e74 6578  ......get_contex
-00002560: 7472 5700 0000 7258 0000 00da 0450 6f6f  trW...rX.....Poo
-00002570: 6c29 03da 0772 6573 7461 7274 da07 776f  l)...restart..wo
-00002580: 726b 6572 73da 0363 7478 7214 0000 0072  rkers..ctxr....r
-00002590: 1400 0000 7215 0000 00da 1573 7461 7274  ....r......start
-000025a0: 5f70 726f 6365 7373 696e 675f 706f 6f6c  _processing_pool
-000025b0: 4201 0000 730e 0000 000a 020a 010a 020a  B...s...........
-000025c0: 020a 0210 010c 027a 1b55 7469 6c73 2e73  .......z.Utils.s
-000025d0: 7461 7274 5f70 726f 6365 7373 696e 675f  tart_processing_
-000025e0: 706f 6f6c 6302 0000 0000 0000 0000 0000  poolc...........
-000025f0: 0002 0000 0003 0000 0043 0000 0073 2400  .........C...s$.
-00002600: 0000 7c00 a000 a100 0100 7c00 a001 a100  ..|.......|.....
-00002610: 0100 7c01 7210 7402 6a03 6401 6402 8d01  ..|.r.t.j.d.d...
-00002620: 7d00 7c00 5300 2903 4e54 2901 72c2 0000  }.|.S.).NT).r...
-00002630: 0029 04da 0563 6c6f 7365 da04 6a6f 696e  .)...close..join
-00002640: 7208 0000 0072 c500 0000 2902 da04 706f  r....r....)...po
-00002650: 6f6c 72c2 0000 0072 1400 0000 7214 0000  olr....r....r...
-00002660: 0072 1500 0000 da14 6a6f 696e 5f70 726f  .r......join_pro
-00002670: 6365 7373 696e 675f 706f 6f6c 5001 0000  cessing_poolP...
-00002680: 730a 0000 0008 0208 0104 020c 0104 027a  s..............z
-00002690: 1a55 7469 6c73 2e6a 6f69 6e5f 7072 6f63  .Utils.join_proc
-000026a0: 6573 7369 6e67 5f70 6f6f 6c63 0500 0000  essing_poolc....
-000026b0: 0000 0000 0000 0000 0800 0000 0a00 0000  ................
-000026c0: 4300 0000 7318 0100 0074 007c 019b 0064  C...s....t.|...d
-000026d0: 017c 029b 009d 0364 0283 028f 787d 057a  .|.....d....x}.z
-000026e0: 677c 05a0 01a1 007d 0674 02a0 0364 03a0  g|.....}.t...d..
-000026f0: 047c 06a1 01a1 017d 067c 0644 005d 0c7d  .|.....}.|.D.].}
-00002700: 077c 067c 0719 0064 046b 0272 2664 007c  .|.|...d.k.r&d.|
-00002710: 067c 073c 0071 1a7c 0372 2974 0564 1069  .|.<.q.|.r)t.d.i
-00002720: 007c 06a4 018e 0161 0674 076a 08a0 097c  .|.....a.t.j...|
-00002730: 01a1 0164 0519 0064 066b 0272 5667 0064  ...d...d.k.rVg.d
-00002740: 07a2 0167 0064 08a2 0164 099c 0274 065f  ...g.d...d...t._
-00002750: 0a64 0a64 0b84 0074 0b74 0c74 066a 0d83  .d.d...t.t.t.j..
-00002760: 0183 0144 0083 0174 065f 0e74 0fa0 1074  ...D...t._.t...t
-00002770: 06a1 0101 007c 0264 0c6b 0272 697c 0474  .....|.d.k.ri|.t
-00002780: 065f 117c 0474 065f 1264 0d74 065f 1364  ._.|.t._.d.t._.d
-00002790: 0e74 065f 1464 0e74 065f 1574 0657 0057  .t._.d.t._.t.W.W
-000027a0: 0002 0064 0004 0004 0083 0301 0053 0004  ...d.........S..
-000027b0: 0074 026a 166a 1774 1866 0279 8101 0001  .t.j.j.t.f.y....
-000027c0: 0001 0074 1964 0f83 0182 0177 0031 0073  ...t.d.....w.1.s
-000027d0: 8577 0101 0001 0001 0059 0001 0064 0053  .w.......Y...d.S
-000027e0: 0029 114e 7263 0000 0072 6500 0000 7223  .).Nrc...re...r#
-000027f0: 0000 00da 044e 6f6e 6572 6700 0000 5a0c  .....Nonerg...Z.
-00002800: 726f 695f 616e 616c 7973 6973 290b 7a0c  roi_analysis).z.
-00002810: 546f 7461 6c20 766f 7865 6c73 7a0f 4578  Total voxelsz.Ex
-00002820: 636c 7564 6564 2076 6f78 656c 737a 1a41  cluded voxelsz.A
-00002830: 7665 7261 6765 2076 6f78 656c 7320 7065  verage voxels pe
-00002840: 7220 7365 7373 696f 6eda 044d 6561 6eda  r session..Mean.
-00002850: 0753 7464 5f64 6576 da13 436f 6e66 6964  .Std_dev..Confid
-00002860: 656e 6365 5f69 6e74 6572 7661 6cda 064d  ence_interval..M
-00002870: 6564 6961 6eda 074d 696e 696d 756d da07  edian..Minimum..
-00002880: 4d61 7869 6d75 6dda 0c50 6172 7469 6369  Maximum..Partici
-00002890: 7061 6e74 73da 0853 6573 7369 6f6e 7329  pants..Sessions)
-000028a0: 0a5a 0c56 6f78 656c 5f61 6d6f 756e 74da  .Z.Voxel_amount.
-000028b0: 1645 7863 6c75 6465 645f 766f 7865 6c73  .Excluded_voxels
-000028c0: 5f61 6d6f 756e 745a 0e41 7665 7261 6765  _amountZ.Average
-000028d0: 5f76 6f78 656c 7372 cb00 0000 5a12 5374  _voxelsr....Z.St
-000028e0: 616e 6461 7264 5f64 6576 6961 7469 6f6e  andard_deviation
-000028f0: 72cd 0000 0072 ce00 0000 72cf 0000 0072  r....r....r....r
-00002900: d000 0000 72d2 0000 0029 0272 9400 0000  ....r....).r....
-00002910: 7293 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00002920: 0000 0200 0000 0500 0000 5300 0000 731e  ..........S...s.
-00002930: 0000 0069 007c 005d 0b7d 0174 006a 017c  ...i.|.].}.t.j.|
-00002940: 0119 0074 006a 027c 0119 0093 0271 0253  ...t.j.|.....q.S
-00002950: 0072 1400 0000 2903 7256 0000 00da 0f70  .r....).rV.....p
-00002960: 6172 616d 6574 6572 5f64 6963 7431 da0f  arameter_dict1..
-00002970: 7061 7261 6d65 7465 725f 6469 6374 3229  parameter_dict2)
-00002980: 0272 3700 0000 da01 6972 1400 0000 7214  .r7.....ir....r.
-00002990: 0000 0072 1500 0000 da0a 3c64 6963 7463  ...r......<dictc
-000029a0: 6f6d 703e 8401 0000 730a 0000 0006 0002  omp>....s.......
-000029b0: 0108 ff08 0106 ff7a 2555 7469 6c73 2e6c  .......z%Utils.l
-000029c0: 6f61 645f 636f 6e66 6967 2e3c 6c6f 6361  oad_config.<loca
-000029d0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7a10  ls>.<dictcomp>z.
-000029e0: 7465 7374 5f63 6f6e 6669 672e 746f 6d6c  test_config.toml
-000029f0: 5a0f 7465 7374 5f52 4f49 5f72 6570 6f72  Z.test_ROI_repor
-00002a00: 745a 0974 6573 745f 6d61 7073 7a35 436f  tZ.test_mapsz5Co
-00002a10: 6e66 6967 2066 696c 6520 6e6f 7420 696e  nfig file not in
-00002a20: 2063 6f72 7265 6374 2066 6f72 6d61 7420   correct format 
-00002a30: 6f72 206d 6973 7369 6e67 2065 6e74 7269  or missing entri
-00002a40: 6573 2e72 1400 0000 291a 7268 0000 00da  es.r....).rh....
-00002a50: 0972 6561 646c 696e 6573 da04 746f 6d6c  .readlines..toml
-00002a60: da05 6c6f 6164 7372 c700 0000 7206 0000  ..loadsr....r...
-00002a70: 0072 5600 0000 7234 0000 0072 3500 0000  .rV...r4...r5...
-00002a80: 728e 0000 00da 1173 7461 7469 7374 6963  r......statistic
-00002a90: 5f6f 7074 696f 6e73 728c 0000 0072 8d00  _optionsr....r..
-00002aa0: 0000 72d4 0000 0072 a600 0000 7208 0000  ..r....r....r...
-00002ab0: 00da 1463 6c65 616e 5f63 6f6e 6669 675f  ...clean_config_
-00002ac0: 6f70 7469 6f6e 73da 0e62 7261 696e 5f66  options..brain_f
-00002ad0: 696c 655f 6c6f 6372 ac00 0000 da0d 6f75  ile_locr......ou
-00002ae0: 7470 7574 5f66 6f6c 6465 725a 126f 7574  tput_folderZ.out
-00002af0: 7075 745f 666f 6c64 6572 5f6e 616d 65da  put_folder_name.
-00002b00: 0f73 7461 745f 6d61 705f 666f 6c64 6572  .stat_map_folder
-00002b10: da07 6465 636f 6465 72da 0f54 6f6d 6c44  ..decoder..TomlD
-00002b20: 6563 6f64 6545 7272 6f72 da0e 4174 7472  ecodeError..Attr
-00002b30: 6962 7574 6545 7272 6f72 7296 0000 0029  ibuteErrorr....)
-00002b40: 08da 0363 6c73 726b 0000 00da 0866 696c  ...clsrk.....fil
-00002b50: 656e 616d 65da 0473 6176 6572 3500 0000  ename..saver5...
-00002b60: da08 746f 6d6c 6669 6c65 da05 7061 7273  ..tomlfile..pars
-00002b70: 6572 a300 0000 7214 0000 0072 1400 0000  er....r....r....
-00002b80: 7215 0000 00da 0b6c 6f61 645f 636f 6e66  r......load_conf
-00002b90: 6967 5a01 0000 733c 0000 0016 0202 0108  igZ...s<........
-00002ba0: 0110 0108 020c 0108 0102 8004 020e 0314  ................
-00002bb0: 0206 0206 0c08 f306 190c 0108 ff0a 0308  ................
-00002bc0: 0206 0206 0106 0106 0106 0104 0210 cb14  ................
-00002bd0: 3708 0102 ff14 c97a 1155 7469 6c73 2e6c  7......z.Utils.l
-00002be0: 6f61 645f 636f 6e66 6967 6301 0000 0000  oad_configc.....
-00002bf0: 0000 0000 0000 0003 0000 0007 0000 0043  ...............C
-00002c00: 0000 0073 6e00 0000 6700 6401 a201 7d01  ...sn...g.d...}.
-00002c10: 7400 7c00 6a01 8301 7402 7501 7212 7c01  t.|.j...t.u.r.|.
-00002c20: a003 7c00 6a01 a101 7c00 5f01 6700 6402  ..|.j...|._.g.d.
-00002c30: a201 7d02 7400 7c00 6a04 8301 7402 7501  ..}.t.|.j...t.u.
-00002c40: 7235 6403 7405 6404 7406 a007 6405 7c00  r5d.t.d.t...d.|.
-00002c50: 6a04 a102 6406 1900 9b00 9d02 8301 1800  j...d...........
-00002c60: 7c00 5f08 7c02 a003 7c00 6a04 a101 7c00  |._.|...|.j...|.
-00002c70: 5f04 7c00 5300 2907 4e29 0d7a 1343 6572  _.|.S.).N).z.Cer
-00002c80: 6562 656c 6c75 6d2d 4d4e 4966 6c69 7274  ebellum-MNIflirt
-00002c90: 7a13 4365 7265 6265 6c6c 756d 2d4d 4e49  z.Cerebellum-MNI
-00002ca0: 666e 6972 747a 1248 6172 7661 7264 4f78  fnirtz.HarvardOx
-00002cb0: 666f 7264 2d63 6f72 747a 1148 6172 7661  ford-cortz.Harva
-00002cc0: 7264 4f78 666f 7264 2d73 7562 7a0f 4a48  rdOxford-subz.JH
-00002cd0: 552d 4943 424d 2d6c 6162 656c 737a 0f4a  U-ICBM-labelsz.J
-00002ce0: 4855 2d49 4342 4d2d 7472 6163 7473 5a07  HU-ICBM-tractsZ.
-00002cf0: 6a75 656c 6963 68da 034d 4e49 7a0c 534d  juelich..MNIz.SM
-00002d00: 4154 542d 6c61 6265 6c73 da03 5354 4e7a  ATT-labels..STNz
-00002d10: 1373 7472 6961 7475 6d2d 7374 7275 6374  .striatum-struct
-00002d20: 7572 616c 7a10 5461 6c61 6972 6163 682d  uralz.Talairach-
-00002d30: 6c61 6265 6c73 da08 5468 616c 616d 7573  labels..Thalamus
-00002d40: 2906 7a09 3830 252c 2031 2e32 387a 0938  ).z.80%, 1.28z.8
-00002d50: 3525 2c20 312e 3434 7a09 3930 252c 2031  5%, 1.44z.90%, 1
-00002d60: 2e36 347a 0939 3525 2c20 312e 3936 7a09  .64z.95%, 1.96z.
-00002d70: 3938 252c 2032 2e33 337a 0939 3925 2c20  98%, 2.33z.99%, 
-00002d80: 322e 3538 721e 0000 007a 0230 2e72 2200  2.58r....z.0.r".
-00002d90: 0000 7201 0000 0029 0972 1f00 0000 da0c  ..r....).r......
-00002da0: 6174 6c61 735f 6e75 6d62 6572 7290 0000  atlas_numberr...
-00002db0: 0072 4a00 0000 da11 636f 6e66 5f6c 6576  .rJ.....conf_lev
-00002dc0: 656c 5f6e 756d 6265 72da 0566 6c6f 6174  el_number..float
-00002dd0: da02 7265 728e 0000 00da 0f62 6f6f 7473  ..rer......boots
-00002de0: 7472 6170 5f61 6c70 6861 2903 7256 0000  trap_alpha).rV..
-00002df0: 00da 0d61 746c 6173 5f6f 7074 696f 6e73  ...atlas_options
-00002e00: 5a12 636f 6e66 5f6c 6576 656c 5f6f 7074  Z.conf_level_opt
-00002e10: 696f 6e73 7214 0000 0072 1400 0000 7215  ionsr....r....r.
-00002e20: 0000 0072 dc00 0000 9601 0000 7310 0000  ...r........s...
-00002e30: 0008 020e 050e 0108 020e 0222 010e 0104  ..........."....
-00002e40: 027a 1a55 7469 6c73 2e63 6c65 616e 5f63  .z.Utils.clean_c
-00002e50: 6f6e 6669 675f 6f70 7469 6f6e 7363 0100  onfig_optionsc..
-00002e60: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00002e70: 0000 4300 0000 7320 0000 0074 00a0 017c  ..C...s ...t...|
-00002e80: 00a1 017d 017c 016a 027d 027c 01a0 03a1  ...}.|.j.}.|....
-00002e90: 007d 017c 017c 0266 0253 0072 4100 0000  .}.|.|.f.S.rA...
-00002ea0: 2904 da03 6e69 62da 046c 6f61 64da 0668  )...nib..load..h
-00002eb0: 6561 6465 72da 0967 6574 5f66 6461 7461  eader..get_fdata
-00002ec0: 2903 da09 6669 6c65 5f70 6174 68da 0464  )...file_path..d
-00002ed0: 6174 6172 f400 0000 7214 0000 0072 1400  atar....r....r..
-00002ee0: 0000 7215 0000 00da 0a6c 6f61 645f 6272  ..r......load_br
-00002ef0: 6169 6ea8 0100 0073 0800 0000 0a02 0602  ain....s........
-00002f00: 0801 0802 7a10 5574 696c 732e 6c6f 6164  ....z.Utils.load
-00002f10: 5f62 7261 696e 6301 0000 0000 0000 0000  _brainc.........
-00002f20: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-00002f30: 2200 0000 6700 6401 a201 7d01 7c01 4400  "...g.d...}.|.D.
-00002f40: 5d08 7d02 7c00 a000 7c02 6402 a102 7d00  ].}.|...|.d...}.
-00002f50: 7106 7c00 5300 2903 4e29 04fa 072e 6e69  q.|.S.).N)....ni
-00002f60: 692e 677a 7a04 2e6e 6969 7a04 2e68 6472  i.gzz..niiz..hdr
-00002f70: 7a05 2e6a 736f 6e72 2300 0000 2901 722a  z..jsonr#...).r*
-00002f80: 0000 0029 0372 3500 0000 723d 0000 0072  ...).r5...r=...r
-00002f90: 3f00 0000 7214 0000 0072 1400 0000 7215  ?...r....r....r.
-00002fa0: 0000 00da 0973 7472 6970 5f65 7874 b101  .....strip_ext..
-00002fb0: 0000 7308 0000 0008 0208 020e 0104 027a  ..s............z
-00002fc0: 0f55 7469 6c73 2e73 7472 6970 5f65 7874  .Utils.strip_ext
-00002fd0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00002fe0: 0004 0000 0043 0000 0073 5c00 0000 6401  .....C...s\...d.
-00002ff0: 6402 8400 7400 7c00 9b00 6403 9d02 8301  d...t.|...d.....
-00003000: 4400 8301 7d01 6404 6402 8400 7c01 4400  D...}.d.d...|.D.
-00003010: 8301 7d02 7401 7c01 8301 6405 6b02 721d  ..}.t.|...d.k.r.
-00003020: 7402 6406 8301 8201 7403 6a04 722a 7405  t.d.....t.j.r*t.
-00003030: 6407 7401 7c01 8301 9b00 6408 9d03 8301  d.t.|.....d.....
-00003040: 0100 7c01 7c02 6602 5300 2909 4e63 0100  ..|.|.f.S.).Nc..
-00003050: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00003060: 0000 5300 0000 731c 0000 0067 007c 005d  ..S...s....g.|.]
-00003070: 0a7d 0174 00a0 0164 007c 01a1 0272 027c  .}.t...d.|...r.|
-00003080: 0191 0271 0253 0029 017a 0b73 7562 2d5b  ...q.S.).z.sub-[
-00003090: 302d 395d 2b24 2902 72ef 0000 00da 0673  0-9]+$).r......s
-000030a0: 6561 7263 6829 0272 3700 0000 da05 6469  earch).r7.....di
-000030b0: 7265 6372 1400 0000 7214 0000 0072 1500  recr....r....r..
-000030c0: 0000 7239 0000 00bd 0100 0073 0200 0000  ..r9.......s....
-000030d0: 1c00 7a2f 5574 696c 732e 6669 6e64 5f70  ..z/Utils.find_p
-000030e0: 6172 7469 6369 7061 6e74 5f64 6972 732e  articipant_dirs.
-000030f0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00003100: 6d70 3e7a 022f 2a63 0100 0000 0000 0000  mp>z./*c........
-00003110: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-00003120: 731a 0000 0067 007c 005d 097d 017c 01a0  s....g.|.].}.|..
-00003130: 0064 00a1 0164 0119 0091 0271 0253 0029  .d...d.....q.S.)
-00003140: 0272 6300 0000 7267 0000 0029 0172 8e00  .rc...rg...).r..
-00003150: 0000 2902 7237 0000 00da 0b70 6172 7469  ..).r7.....parti
-00003160: 6369 7061 6e74 7214 0000 0072 1400 0000  cipantr....r....
-00003170: 7215 0000 0072 3900 0000 be01 0000 7302  r....r9.......s.
-00003180: 0000 001a 0072 0100 0000 7a9e 5061 7274  .....r....z.Part
-00003190: 6963 6970 616e 7420 6469 7265 6374 6f72  icipant director
-000031a0: 6965 7320 6e6f 7420 666f 756e 642e 0a4d  ies not found..M
-000031b0: 616b 6520 7375 7265 2070 6172 7469 6369  ake sure partici
-000031c0: 7061 6e74 2064 6972 6563 746f 7269 6573  pant directories
-000031d0: 2061 7265 206c 6162 656c 6c65 6420 652e   are labelled e.
-000031e0: 672e 2073 7562 2d30 3120 616e 6420 7468  g. sub-01 and th
-000031f0: 6520 7365 6c65 6374 6564 2064 6972 6563  e selected direc
-00003200: 746f 7279 2063 6f6e 7461 696e 7320 616c  tory contains al
-00003210: 6c20 7061 7274 6963 6970 616e 7420 6469  l participant di
-00003220: 7265 6374 6f72 6965 732e 7a06 466f 756e  rectories.z.Foun
-00003230: 6420 7a15 2070 6172 7469 6369 7061 6e74  d z. participant
-00003240: 2066 6f6c 6465 7273 2e29 0672 0200 0000   folders.).r....
-00003250: 728d 0000 0072 5400 0000 7256 0000 0072  r....rT...rV...r
-00003260: 5700 0000 7258 0000 0029 0372 3c00 0000  W...rX...).r<...
-00003270: 5a11 7061 7274 6963 6970 616e 745f 7061  Z.participant_pa
-00003280: 7468 73da 1170 6172 7469 6369 7061 6e74  ths..participant
-00003290: 5f6e 616d 6573 7214 0000 0072 1400 0000  _namesr....r....
-000032a0: 7215 0000 00da 1566 696e 645f 7061 7274  r......find_part
-000032b0: 6963 6970 616e 745f 6469 7273 ba01 0000  icipant_dirs....
-000032c0: 730e 0000 0018 030e 010c 0208 0106 0314  s...............
-000032d0: 0108 027a 1b55 7469 6c73 2e66 696e 645f  ...z.Utils.find_
-000032e0: 7061 7274 6963 6970 616e 745f 6469 7273  participant_dirs
-000032f0: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-00003300: 0008 0000 0043 0000 0073 a400 0000 7c00  .....C...s....|.
-00003310: 6100 6401 7d01 6402 7d02 7401 6403 7c00  a.d.}.d.}.t.d.|.
-00003320: 9b00 6404 7402 7c01 8301 9b00 6405 7402  ..d.t.|.....d.t.
-00003330: 7c02 8301 9b00 6406 9d07 8301 0100 7403  |.....d.......t.
-00003340: 6a04 6400 6407 8502 1900 7c01 7c02 6602  j.d.d.....|.|.f.
-00003350: 6b03 7250 7402 7403 6a04 6408 1900 8301  k.rPt.t.j.d.....
-00003360: 9b00 6405 7402 7403 6a04 6409 1900 8301  ..d.t.t.j.d.....
-00003370: 9b00 6405 7402 7403 6a04 6407 1900 8301  ..d.t.t.j.d.....
-00003380: 9b00 9d05 7d03 7401 640a 7c03 9b00 640b  ....}.t.d.|...d.
-00003390: 7402 7c01 8301 9b00 6405 7402 7c02 8301  t.|.....d.t.|...
-000033a0: 9b00 640c 9d07 8301 0100 6400 5300 6400  ..d.......d.S.d.
-000033b0: 5300 290d 4ee9 0300 0000 e90a 0000 007a  S.).N..........z
-000033c0: 060a 6652 4154 207a 2520 6973 2064 6576  ..fRAT z% is dev
-000033d0: 656c 6f70 6564 2061 6e64 2074 6573 7465  eloped and teste
-000033e0: 6420 7769 7468 2050 7974 686f 6e20 7233  d with Python r3
-000033f0: 0000 007a 022e 0a72 b500 0000 7201 0000  ...z...r....r...
-00003400: 0072 1e00 0000 7a15 494e 464f 3a20 5079  .r....z.INFO: Py
-00003410: 7468 6f6e 2076 6572 7369 6f6e 207a 2b20  thon version z+ 
-00003420: 6973 2075 6e74 6573 7465 642e 2043 6f6e  is untested. Con
-00003430: 7369 6465 7220 6368 616e 6769 6e67 2074  sider changing t
-00003440: 6f20 7665 7273 696f 6e20 7a22 2069 6620  o version z" if 
-00003450: 7468 6572 6520 6172 6520 6572 726f 7273  there are errors
-00003460: 2072 756e 6e69 6e67 2066 5241 542e 2905   running fRAT.).
-00003470: 7269 0000 0072 5800 0000 725d 0000 00da  ri...rX...r]....
-00003480: 0373 7973 da0c 7665 7273 696f 6e5f 696e  .sys..version_in
-00003490: 666f 2904 5a0c 6672 6174 5f76 6572 7369  fo).Z.frat_versi
-000034a0: 6f6e 5a0c 6578 7065 6374 5f6d 616a 6f72  onZ.expect_major
-000034b0: 5a0c 6578 7065 6374 5f6d 696e 6f72 5a0f  Z.expect_minorZ.
-000034c0: 6375 7272 656e 745f 7665 7273 696f 6e72  current_versionr
-000034d0: 1400 0000 7214 0000 0072 1500 0000 da0c  ....r....r......
-000034e0: 6368 6563 6b76 6572 7369 6f6e c901 0000  checkversion....
-000034f0: 7318 0000 0004 0304 0304 0124 0216 0132  s..........$...2
-00003500: 010a 0106 0104 ff06 010e ff04 fe7a 1255  .............z.U
-00003510: 7469 6c73 2e63 6865 636b 7665 7273 696f  tils.checkversio
-00003520: 6e63 0200 0000 0000 0000 0000 0000 0400  nc..............
-00003530: 0000 0800 0000 4300 0000 73ae 0000 007c  ......C...s....|
-00003540: 0064 016b 0272 097c 016a 0072 0964 0053  .d.k.r.|.j.r.d.S
-00003550: 007c 016a 0172 2364 0264 036c 026d 037d  .|.j.r#d.d.l.m.}
-00003560: 0201 0074 04a0 05a1 009b 0064 047c 026a  ...t.......d.|.j
-00003570: 069b 009d 037d 0374 04a0 077c 03a1 0101  .....}.t...|....
-00003580: 007c 0353 007c 016a 0864 0576 0072 3574  .|.S.|.j.d.v.r5t
-00003590: 0964 0683 0101 0074 0a6a 0b64 0764 0864  .d.....t.j.d.d.d
-000035a0: 098d 027d 037c 0353 007c 016a 087d 037a  ...}.|.S.|.j.}.z
-000035b0: 0774 04a0 077c 03a1 0101 0057 006e 0b04  .t...|.....W.n..
-000035c0: 0074 0c79 4a01 0001 0001 0074 0c64 0a83  .t.yJ......t.d..
-000035d0: 0182 0177 007c 016a 0d72 5574 0964 0b7c  ...w.|.j.rUt.d.|
-000035e0: 039b 009d 0283 0101 007c 0353 0029 0c4e  .........|.S.).N
-000035f0: da0a 5374 6174 6973 7469 6373 721e 0000  ..Statisticsr...
-00003600: 0029 01da 1145 6e76 6972 6f6e 6d65 6e74  .)...Environment
-00003610: 5f53 6574 7570 7263 0000 0029 0272 2300  _Setuprc...).r#.
-00003620: 0000 fa01 207a 2853 656c 6563 7420 7468  .... z(Select th
-00003630: 6520 6469 7265 6374 6f72 7920 6f75 7470  e directory outp
-00003640: 7574 2062 7920 7468 6520 6652 4154 2e7a  ut by the fRAT.z
-00003650: 2753 656c 6563 7420 7468 6520 6469 7265  'Select the dire
-00003660: 6374 6f72 7920 6f75 7470 7574 2062 7920  ctory output by 
-00003670: 7468 6520 6652 4154 5429 0272 0b00 0000  the fRATT).r....
-00003680: 7255 0000 007a 4e4f 7574 7075 7420 666f  rU...zNOutput fo
-00003690: 6c64 6572 206c 6f63 6174 696f 6e20 2866  lder location (f
-000036a0: 5241 5420 6f75 7470 7574 2066 6f6c 6465  RAT output folde
-000036b0: 7220 6c6f 6361 7469 6f6e 2920 6973 206e  r location) is n
-000036c0: 6f74 2061 2076 616c 6964 2064 6972 6563  ot a valid direc
-000036d0: 746f 7279 2e7a 194f 7574 7075 7420 666f  tory.z.Output fo
-000036e0: 6c64 6572 2073 656c 6563 7469 6f6e 3a20  lder selection: 
-000036f0: 290e da0c 7275 6e5f 706c 6f74 7469 6e67  )...run_plotting
-00003700: da0c 7275 6e5f 616e 616c 7973 6973 da08  ..run_analysis..
-00003710: 616e 616c 7973 6973 7206 0100 0072 3400  analysisr....r4.
-00003720: 0000 72ae 0000 00da 0d73 6176 655f 6c6f  ..r......save_lo
-00003730: 6361 7469 6f6e 7255 0000 005a 1472 6570  cationrU...Z.rep
-00003740: 6f72 745f 6f75 7470 7574 5f66 6f6c 6465  ort_output_folde
-00003750: 7272 5800 0000 7208 0000 0072 5a00 0000  rrX...r....rZ...
-00003760: 7254 0000 0072 5700 0000 2904 5a0c 6375  rT...rW...).Z.cu
-00003770: 7272 656e 745f 7374 6570 7256 0000 0072  rrent_steprV...r
-00003780: 0601 0000 5a0e 6a73 6f6e 5f64 6972 6563  ....Z.json_direc
-00003790: 746f 7279 7214 0000 0072 1400 0000 7215  toryr....r....r.
-000037a0: 0000 00da 1963 6864 6972 5f74 6f5f 6f75  .....chdir_to_ou
-000037b0: 7470 7574 5f64 6972 6563 746f 7279 d801  tput_directory..
-000037c0: 0000 732c 0000 000e 0204 0106 020c 0114  ..s,............
-000037d0: 010a 0204 120a f008 010e 0104 0e06 f502  ................
-000037e0: 020e 010c 0102 0102 0104 ff02 ff06 040e  ................
-000037f0: 0104 027a 1f55 7469 6c73 2e63 6864 6972  ...z.Utils.chdir
-00003800: 5f74 6f5f 6f75 7470 7574 5f64 6972 6563  _to_output_direc
-00003810: 746f 7279 6305 0000 0000 0000 0000 0000  toryc...........
-00003820: 0006 0000 0008 0000 0043 0000 0073 3e00  .........C...s>.
-00003830: 0000 7400 a001 7c00 6400 7c04 a103 7d05  ..t...|.d.|...}.
-00003840: 7400 a002 7c05 7c03 9b00 6401 7c02 9b00  t...|.|...d.|...
-00003850: 7c01 9b00 6402 9d05 a102 0100 7c03 9b00  |...d.......|...
-00003860: 6401 7c02 9b00 7c01 9b00 6402 9d05 5300  d.|...|...d...S.
-00003870: 2903 4e72 6300 0000 72f9 0000 0029 0372  ).Nrc...r....).r
-00003880: f200 0000 da0a 4e69 6674 6931 5061 6972  ......Nifti1Pair
-00003890: 72e5 0000 0029 0672 f700 0000 da03 6578  r....).r......ex
-000038a0: 745a 0b6e 6f5f 6578 745f 6669 6c65 72de  tZ.no_ext_filer.
-000038b0: 0000 0072 f400 0000 da05 6272 6169 6e72  ...r......brainr
-000038c0: 1400 0000 7214 0000 0072 1500 0000 da0a  ....r....r......
-000038d0: 7361 7665 5f62 7261 696e f501 0000 7306  save_brain....s.
-000038e0: 0000 000e 021c 0114 027a 1055 7469 6c73  .........z.Utils
-000038f0: 2e73 6176 655f 6272 6169 6e29 0272 2300  .save_brain).r#.
-00003900: 0000 4629 034e 7261 0000 0072 6200 0000  ..F).Nra...rb...
-00003910: 2903 4654 4629 0146 2901 7223 0000 0029  ).FTF).F).r#...)
-00003920: 0254 4e72 4100 0000 2920 da08 5f5f 6e61  .TNrA...) ..__na
-00003930: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00003940: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
-00003950: 7374 6174 6963 6d65 7468 6f64 7216 0000  staticmethodr...
-00003960: 0072 3200 0000 7240 0000 0072 4900 0000  .r2...r@...rI...
-00003970: 7250 0000 0072 5a00 0000 7260 0000 0072  rP...rZ...r`...r
-00003980: 6f00 0000 7278 0000 0072 7d00 0000 7292  o...rx...r}...r.
-00003990: 0000 0072 9b00 0000 72ab 0000 0072 b200  ...r....r....r..
-000039a0: 0000 727b 0000 0072 b900 0000 72ba 0000  ..r{...r....r...
-000039b0: 0072 c500 0000 72c9 0000 00da 0b63 6c61  .r....r......cla
-000039c0: 7373 6d65 7468 6f64 72e8 0000 0072 dc00  ssmethodr....r..
-000039d0: 0000 72f8 0000 0072 fa00 0000 72ff 0000  ..r....r....r...
-000039e0: 0072 0401 0000 720c 0100 0072 1001 0000  .r....r....r....
-000039f0: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
-00003a00: 1500 0000 7208 0000 0017 0000 0073 6e00  ....r........sn.
-00003a10: 0000 0800 0201 0a01 020f 0a01 022a 0a01  .............*..
-00003a20: 020d 0a01 0207 0a01 0203 0c01 0213 0a01  ................
-00003a30: 0206 0c01 0218 0c01 0214 0c01 0208 0a01  ................
-00003a40: 022e 0a01 0214 0a01 0218 0c01 0216 0a01  ................
-00003a50: 0206 0a01 0203 0a01 0203 0c01 020d 0a01  ................
-00003a60: 0209 0c01 023b 0a01 0211 0a01 0208 0a01  .....;..........
-00003a70: 0208 0a01 020e 0a01 020e 0a01 021c 1001  ................
-00003a80: 7208 0000 0029 1972 2500 0000 720c 0000  r....).r%...r...
-00003a90: 0072 3400 0000 72ef 0000 0072 7100 0000  .r4...r....rq...
-00003aa0: 7202 0100 0072 0200 0000 da07 7061 7468  r....r......path
-00003ab0: 6c69 6272 0300 0000 da07 746b 696e 7465  libr......tkinte
-00003ac0: 7272 0400 0000 7205 0000 00da 0574 7970  rr....r......typ
-00003ad0: 6573 7206 0000 005a 0c6d 756c 7469 7072  esr....Z.multipr
-00003ae0: 6f63 6573 7372 be00 0000 da07 6e69 6261  ocessr......niba
-00003af0: 6265 6c72 f200 0000 da06 7061 6e64 6173  belr......pandas
-00003b00: 724c 0000 0072 d900 0000 da1c 6652 4154  rL...r......fRAT
-00003b10: 2e75 7469 6c73 2e66 5241 545f 636f 6e66  .utils.fRAT_conf
-00003b20: 6967 5f73 6574 7570 7256 0000 0072 6900  ig_setuprV...ri.
-00003b30: 0000 7208 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00003b40: 0072 1400 0000 7215 0000 00da 083c 6d6f  .r....r......<mo
-00003b50: 6475 6c65 3e01 0000 0073 2400 0000 0800  dule>....s$.....
-00003b60: 0801 0801 0801 0801 0801 0c01 0c01 1001  ................
-00003b70: 0c01 0802 0801 0801 0801 0802 0402 0401  ................
-00003b80: 1203                                     ..
+00000fd0: 0219 007d 097c 08a0 0364 0ea1 0173 627c  ...}.|...d...sb|
+00000fe0: 08a0 0564 09a1 0164 0f19 009b 0064 089d  ...d...d.....d..
+00000ff0: 027d 087c 0464 106b 0272 6c7c 06a0 017c  .}.|.d.k.rl|...|
+00001000: 08a1 0101 0071 3d7c 097c 0476 0072 757c  .....q=|.|.v.ru|
+00001010: 06a0 017c 08a1 0101 0071 3d57 0064 0004  ...|.....q=W.d..
+00001020: 0004 0083 0301 006e 1031 0073 8077 0101  .......n.1.s.w..
+00001030: 0001 0001 0059 0001 0057 0064 0004 0004  .....Y...W.d....
+00001040: 0083 0301 0064 0053 0057 0064 0004 0004  .....d.S.W.d....
+00001050: 0083 0301 0064 0053 0031 0073 9877 0101  .....d.S.1.s.w..
+00001060: 0001 0001 0059 0001 0064 0053 0029 114e  .....Y...d.S.).N
+00001070: fa01 2f7a 052e 746f 6d6c da01 77da 0172  ../z..toml..w..r
+00001080: 7a20 2320 4765 6e65 7261 6c20 696e 666f  z # General info
+00001090: 726d 6174 696f 6e0a 7665 7273 696f 6e20  rmation.version 
+000010a0: 3d20 7a15 0a63 6f6e 6669 675f 6669 6c65  = z..config_file
+000010b0: 5f75 7365 6420 3d20 277a 0227 0a72 5b00  _used = 'z.'.r[.
+000010c0: 0000 fa01 237a 0223 2372 2300 0000 721e  ....#z.##r#...r.
+000010d0: 0000 00e9 ffff ffff 2902 7266 0000 0072  ........).rf...r
+000010e0: 5b00 0000 7201 0000 0072 6100 0000 2906  [...r....ra...).
+000010f0: da04 6f70 656e 725c 0000 00da 0776 6572  ..openr\.....ver
+00001100: 7369 6f6e da0a 7374 6172 7473 7769 7468  sion..startswith
+00001110: 722a 0000 00da 0573 706c 6974 290a 5a06  r*.....split).Z.
+00001120: 6e65 7764 6972 da0b 636f 6e66 6967 5f70  newdir..config_p
+00001130: 6174 68da 0f63 6f6e 6669 675f 6669 6c65  ath..config_file
+00001140: 6e61 6d65 5a0f 6164 6469 7469 6f6e 616c  nameZ.additional
+00001150: 5f69 6e66 6fda 1172 656c 6576 616e 745f  _info..relevant_
+00001160: 7365 6374 696f 6e73 da0f 6e65 775f 636f  sections..new_co
+00001170: 6e66 6967 5f6e 616d 6572 3800 0000 7265  nfig_namer8...re
+00001180: 0000 0072 5f00 0000 5a0f 6375 7272 656e  ...r_...Z.curren
+00001190: 745f 7365 6374 696f 6e72 1400 0000 7214  t_sectionr....r.
+000011a0: 0000 0072 1500 0000 da0b 7361 7665 5f63  ...r......save_c
+000011b0: 6f6e 6669 6788 0000 0073 3000 0000 2e02  onfig....s0.....
+000011c0: 0601 0201 04ff 0202 0afe 0404 0801 0c01  ................
+000011d0: 0a02 0a02 0402 0801 1401 1401 0a02 1402  ................
+000011e0: 0802 0c01 0801 0a01 0280 02f5 50f2 7a11  ............P.z.
+000011f0: 5574 696c 732e 7361 7665 5f63 6f6e 6669  Utils.save_confi
+00001200: 6754 6306 0000 0000 0000 0000 0000 0007  gTc.............
+00001210: 0000 0006 0000 0043 0000 0073 9c00 0000  .......C...s....
+00001220: 7c01 a000 6401 a101 7309 7c01 6401 3700  |...d...s.|.d.7.
+00001230: 7d01 7c02 a000 6401 a101 7312 7c02 6401  }.|...d...s.|.d.
+00001240: 3700 7d02 7c05 7217 6402 7d06 6e02 7c00  7.}.|.r.d.}.n.|.
+00001250: 7d06 7c03 723e 7c04 722e 7401 a002 7c01  }.|.r>|.r.t...|.
+00001260: 9b00 7c00 9b00 9d02 7c02 9b00 6403 7c06  ..|.....|...d.|.
+00001270: 9b00 9d03 a102 0100 6400 5300 7401 a002  ........d.S.t...
+00001280: 7c01 9b00 7c00 9b00 9d02 7c02 9b00 7c06  |...|.....|...|.
+00001290: 9b00 9d02 a102 0100 6400 5300 7403 a004  ........d.S.t...
+000012a0: 7c01 9b00 7c00 9b00 9d02 7c02 9b00 7c06  |...|.....|...|.
+000012b0: 9b00 9d02 a102 0100 6400 5300 2904 4e72  ........d.S.).Nr
+000012c0: 6300 0000 7a0f 7061 7261 6d56 616c 7565  c...z.paramValue
+000012d0: 732e 6373 765a 0563 6f70 795f 2905 da08  s.csvZ.copy_)...
+000012e0: 656e 6473 7769 7468 da06 7368 7574 696c  endswith..shutil
+000012f0: da04 636f 7079 7234 0000 00da 0672 656e  ..copyr4.....ren
+00001300: 616d 6529 07da 086f 6c64 5f6e 616d 655a  ame)...old_nameZ
+00001310: 0c6f 7269 6769 6e61 6c5f 6469 725a 076e  .original_dirZ.n
+00001320: 6577 5f64 6972 7273 0000 00da 0b72 656e  ew_dirrs.....ren
+00001330: 616d 655f 636f 7079 da0e 7061 7261 6d65  ame_copy..parame
+00001340: 7465 725f 6669 6c65 da08 6e65 775f 6e61  ter_file..new_na
+00001350: 6d65 7214 0000 0072 1400 0000 7215 0000  mer....r....r...
+00001360: 00da 096d 6f76 655f 6669 6c65 a500 0000  ...move_file....
+00001370: 7318 0000 000a 0208 010a 0208 0104 0206  s...............
+00001380: 0104 0204 0204 0122 0120 0220 027a 0f55  .......". . .z.U
+00001390: 7469 6c73 2e6d 6f76 655f 6669 6c65 6302  tils.move_filec.
+000013a0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000013b0: 0000 0043 0000 0073 4600 0000 7c01 7214  ...C...sF...|.r.
+000013c0: 7400 6a01 a002 7c00 a101 7214 7403 a004  t.j...|...r.t...
+000013d0: 7c00 a101 0100 7405 a006 7c00 a101 0100  |.....t...|.....
+000013e0: 6400 5300 7400 6a01 a002 7c00 a101 7321  d.S.t.j...|...s!
+000013f0: 7405 a006 7c00 a101 0100 6400 5300 6400  t...|.....d.S.d.
+00001400: 5300 7241 0000 0029 0772 3400 0000 7235  S.rA...).r4...r5
+00001410: 0000 00da 0665 7869 7374 7372 7200 0000  .....existsrr...
+00001420: da06 726d 7472 6565 7208 0000 00da 066d  ..rmtreer......m
+00001430: 6b5f 6469 7229 0272 3500 0000 da0a 6465  k_dir).r5.....de
+00001440: 6c65 7465 5f6f 6c64 7214 0000 0072 1400  lete_oldr....r..
+00001450: 0000 7215 0000 00da 1263 6865 636b 5f61  ..r......check_a
+00001460: 6e64 5f6d 616b 655f 6469 72ba 0000 0073  nd_make_dir....s
+00001470: 0c00 0000 1002 0a01 0e01 0c02 0e01 04ff  ................
+00001480: 7a18 5574 696c 732e 6368 6563 6b5f 616e  z.Utils.check_an
+00001490: 645f 6d61 6b65 5f64 6972 6303 0000 0000  d_make_dirc.....
+000014a0: 0000 0000 0000 0007 0000 0008 0000 0003  ................
+000014b0: 0000 0073 4201 0000 7c02 6401 6b02 7269  ...sB...|.d.k.ri
+000014c0: 6700 7d03 7400 6402 8301 0100 7401 8800  g.}.t.d.....t...
+000014d0: 8301 4400 5d0d 5c02 7d04 7d05 7400 6403  ..D.].\.}.}.t.d.
+000014e0: 6a02 7c04 7c05 6404 8d02 8301 0100 710e  j.|.|.d.......q.
+000014f0: 7c03 7368 7400 6405 7c01 9b00 6406 9d03  |.sht.d.|...d...
+00001500: 8301 0100 7403 6407 8301 7d06 7c06 a004  ....t.d...}.|...
+00001510: a100 6408 6b02 723a 7405 7406 6409 7407  ..d.k.r:t.t.d.t.
+00001520: 8800 8301 8302 8301 7d03 6e2c 7407 7c06  ........}.n,t.|.
+00001530: 8301 6409 6b04 7263 640a 640b 8400 7c06  ..d.k.rcd.d...|.
+00001540: a008 640c a101 4400 8301 7d03 7a09 7405  ..d...D...}.z.t.
+00001550: 7409 740a 7c03 8302 8301 7d03 5700 6e12  t.t.|.....}.W.n.
+00001560: 0400 740b 7962 0100 0100 0100 7400 640d  ..t.yb......t.d.
+00001570: 8301 0100 6700 7d03 5900 6e04 7700 6700  ....g.}.Y.n.w.g.
+00001580: 7d03 7196 7c03 721e 6e2d 740c 7c02 7405  }.q.|.r.n-t.|.t.
+00001590: 8302 7287 740c 7c02 6409 1900 740d 8302  ..r.t.|.d...t...
+000015a0: 7287 7c02 6409 1900 a004 a100 6408 6b02  r.|.d.......d.k.
+000015b0: 7287 7405 7406 6409 7407 8800 8301 8302  r.t.t.d.t.......
+000015c0: 8301 7d03 6e0f 7c02 7d03 740c 7c03 740a  ..}.n.|.}.t.|.t.
+000015d0: 8302 7292 7c03 6701 7d03 6e04 7405 7c03  ..r.|.g.}.n.t.|.
+000015e0: 8301 7d03 8700 6601 640e 640b 8408 7c03  ..}...f.d.d...|.
+000015f0: 4400 8301 7d03 7c03 5300 290f 4eda 0752  D...}.|.S.).N..R
+00001600: 756e 7469 6d65 725b 0000 007a 107b 726f  untimer[...z.{ro
+00001610: 695f 6e75 6d7d 3a20 7b72 6f69 7d29 02da  i_num}: {roi})..
+00001620: 0772 6f69 5f6e 756d da03 726f 697a 050a  .roi_num..roiz..
+00001630: 2d2d 2d20 7a0d 2063 7265 6174 696f 6e20  --- z. creation 
+00001640: 2d2d 2d7a b854 7970 6520 6120 636f 6d6d  ---z.Type a comm
+00001650: 612d 7365 7061 7261 7465 6420 6c69 7374  a-separated list
+00001660: 206f 6620 7468 6520 524f 4973 2028 6c69   of the ROIs (li
+00001670: 7374 6564 2061 626f 7665 2920 796f 7520  sted above) you 
+00001680: 7761 6e74 2074 6f20 7072 6f64 7563 6520  want to produce 
+00001690: 6120 6669 6775 7265 2066 6f72 2c20 2765  a figure for, 'e
+000016a0: 2e67 2e20 322c 2031 352c 2037 2c20 3233  .g. 2, 15, 7, 23
+000016b0: 2720 6f72 2027 616c 6c27 2066 6f72 2061  ' or 'all' for a
+000016c0: 6c6c 2072 6f69 732e 200a 416c 7465 726e  ll rois. .Altern
+000016d0: 6174 6976 656c 7920 7072 6573 7320 656e  atively press en
+000016e0: 7465 7220 7477 6963 6520 746f 2073 6b69  ter twice to ski
+000016f0: 7020 7468 6973 2073 7465 703a 2072 6100  p this step: ra.
+00001700: 0000 7201 0000 0063 0100 0000 0000 0000  ..r....c........
+00001710: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00001720: f314 0000 0067 007c 005d 067d 017c 01a0  .....g.|.].}.|..
+00001730: 00a1 0091 0271 0253 0072 1400 0000 2901  .....q.S.r....).
+00001740: da05 7374 7269 70a9 0272 3700 0000 7213  ..strip..r7...r.
+00001750: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00001760: 0000 7239 0000 00d6 0000 00f3 0200 0000  ..r9............
+00001770: 1400 7a2a 5574 696c 732e 6669 6e64 5f63  ..z*Utils.find_c
+00001780: 686f 7365 6e5f 726f 6973 2e3c 6c6f 6361  hosen_rois.<loca
+00001790: 6c73 3e2e 3c6c 6973 7463 6f6d 703e fa01  ls>.<listcomp>..
+000017a0: 2c7a 2c43 6f6d 6d61 2d73 6570 6172 6174  ,z,Comma-separat
+000017b0: 6564 206c 6973 7420 636f 6e74 6169 6e73  ed list contains
+000017c0: 206e 6f6e 2069 6e74 6567 6572 732e 0a63   non integers..c
+000017d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000017e0: 0400 0000 1300 0000 7314 0000 0067 007c  ........s....g.|
+000017f0: 005d 067d 0188 007c 0119 0091 0271 0253  .].}...|.....q.S
+00001800: 0072 1400 0000 7214 0000 0029 0272 3700  .r....r....).r7.
+00001810: 0000 5a0a 726f 695f 6e75 6d62 6572 a901  ..Z.roi_number..
+00001820: da08 616c 6c5f 726f 6973 7214 0000 0072  ..all_roisr....r
+00001830: 1500 0000 7239 0000 00ee 0000 0072 8500  ....r9.......r..
+00001840: 0000 290e 7258 0000 00da 0965 6e75 6d65  ..).rX.....enume
+00001850: 7261 7465 da06 666f 726d 6174 da05 696e  rate..format..in
+00001860: 7075 74da 056c 6f77 6572 7210 0000 00da  put..lowerr.....
+00001870: 0572 616e 6765 da03 6c65 6e72 6b00 0000  .range..lenrk...
+00001880: da03 6d61 70da 0369 6e74 7211 0000 0072  ..map..intr....r
+00001890: 0e00 0000 725d 0000 0029 0772 8800 0000  ....r]...).r....
+000018a0: da09 6675 6e63 5f6e 616d 655a 1163 6f6e  ..func_nameZ.con
+000018b0: 6669 675f 7265 6769 6f6e 5f76 6172 5a0b  fig_region_varZ.
+000018c0: 6368 6f73 656e 5f72 6f69 7372 8000 0000  chosen_roisr....
+000018d0: 7281 0000 005a 0772 6f69 5f61 6e73 7214  r....Z.roi_ansr.
+000018e0: 0000 0072 8700 0000 7215 0000 00da 1066  ...r....r......f
+000018f0: 696e 645f 6368 6f73 656e 5f72 6f69 73c3  ind_chosen_rois.
+00001900: 0000 0073 4400 0000 0802 0401 0801 1002  ...sD...........
+00001910: 1401 0402 1001 0201 0201 04ff 0c04 1401  ................
+00001920: 0c02 1401 0202 1201 0c01 0801 0801 02fe  ................
+00001930: 0405 0201 04ec 0280 1817 0e01 02ff 1402  ................
+00001940: 0402 0a02 0801 0802 1202 0402 7a16 5574  ............z.Ut
+00001950: 696c 732e 6669 6e64 5f63 686f 7365 6e5f  ils.find_chosen_
+00001960: 726f 6973 6302 0000 0000 0000 0000 0000  roisc...........
+00001970: 0004 0000 0008 0000 0043 0000 0073 7e00  .........C...s~.
+00001980: 0000 7400 a001 a100 7d02 6401 7d03 7a1f  ..t.....}.d.}.z.
+00001990: 7c01 6402 6b02 7216 7c00 9b00 6403 9d02  |.d.k.r.|...d...
+000019a0: 7d03 7400 a002 7c03 a101 7d02 6e0e 7c01  }.t...|...}.n.|.
+000019b0: 6404 6b02 7224 7c00 9b00 6405 9d02 7d03  d.k.r$|...d...}.
+000019c0: 7400 a002 7c03 a101 7d02 5700 6e10 0400  t...|...}.W.n...
+000019d0: 7403 7935 0100 0100 0100 7404 6406 7405  t.y5......t.d.t.
+000019e0: 6a06 9b00 6407 9d03 8301 8201 7700 7c02  j...d.......w.|.
+000019f0: a007 6408 a101 7d02 7c02 7c03 6602 5300  ..d...}.|.|.f.S.
+00001a00: 2909 4e72 2300 0000 fa10 5365 7373 696f  ).Nr#.....Sessio
+00001a10: 6e20 6176 6572 6167 6564 7a4a 2f4f 7665  n averagedzJ/Ove
+00001a20: 7261 6c6c 2f53 756d 6d61 7269 7365 645f  rall/Summarised_
+00001a30: 7265 7375 6c74 732f 5365 7373 696f 6e5f  results/Session_
+00001a40: 6176 6572 6167 6564 5f72 6573 756c 7473  averaged_results
+00001a50: 2f63 6f6d 6269 6e65 645f 7265 7375 6c74  /combined_result
+00001a60: 732e 6a73 6f6e fa14 5061 7274 6963 6970  s.json..Particip
+00001a70: 616e 7420 6176 6572 6167 6564 7a4e 2f4f  ant averagedzN/O
+00001a80: 7665 7261 6c6c 2f53 756d 6d61 7269 7365  verall/Summarise
+00001a90: 645f 7265 7375 6c74 732f 5061 7274 6963  d_results/Partic
+00001aa0: 6970 616e 745f 6176 6572 6167 6564 5f72  ipant_averaged_r
+00001ab0: 6573 756c 7473 2f63 6f6d 6269 6e65 645f  esults/combined_
+00001ac0: 7265 7375 6c74 732e 6a73 6f6e 7a23 636f  results.jsonz#co
+00001ad0: 6d62 696e 6564 5f72 6573 756c 7473 2e6a  mbined_results.j
+00001ae0: 736f 6e20 6e6f 7420 666f 756e 6420 696e  son not found in
+00001af0: 207a 0820 666f 6c64 6572 2e72 4a00 0000   z. folder.rJ...
+00001b00: 2908 724c 0000 0072 4d00 0000 da09 7265  ).rL...rM.....re
+00001b10: 6164 5f6a 736f 6e72 1100 0000 da09 4578  ad_jsonr......Ex
+00001b20: 6365 7074 696f 6e72 5600 0000 da0e 6176  ceptionrV.....av
+00001b30: 6572 6167 696e 675f 7479 7065 da0b 736f  eraging_type..so
+00001b40: 7274 5f76 616c 7565 7329 04da 0666 6f6c  rt_values)...fol
+00001b50: 6465 7272 9700 0000 da02 6466 7235 0000  derr......dfr5..
+00001b60: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00001b70: da15 7265 6164 5f63 6f6d 6269 6e65 645f  ..read_combined_
+00001b80: 7265 7375 6c74 73f2 0000 0073 1e00 0000  results....s....
+00001b90: 0802 0401 0202 0801 0a01 0c01 0802 0a01  ................
+00001ba0: 0a01 0480 0c02 1201 02ff 0a03 0802 7a1b  ..............z.
+00001bb0: 5574 696c 732e 7265 6164 5f63 6f6d 6269  Utils.read_combi
+00001bc0: 6e65 645f 7265 7375 6c74 7363 0100 0000  ned_resultsc....
+00001bd0: 0000 0000 0000 0000 0500 0000 0900 0000  ................
+00001be0: 0300 0000 73c2 0000 0064 0164 0284 007c  ....s....d.d...|
+00001bf0: 006a 0044 0083 017c 005f 0074 0164 0364  .j.D...|._.t.d.d
+00001c00: 0484 0074 027c 006a 0083 0144 0083 0164  ...t.|.j...D...d
+00001c10: 0583 027d 0174 0164 0664 0484 0074 027c  ...}.t.d.d...t.|
+00001c20: 006a 0083 0144 0083 0164 0583 027d 027c  .j...D...d...}.|
+00001c30: 0273 2e74 0364 0774 046a 059b 0064 089d  .s.t.d.t.j...d..
+00001c40: 0383 0182 0167 007d 0374 046a 0644 005d  .....g.}.t.j.D.]
+00001c50: 2889 0074 0187 0066 0164 0964 0484 0874  (..t...f.d.d...t
+00001c60: 027c 006a 0083 0144 0083 0164 0583 027d  .|.j...D...d...}
+00001c70: 047c 0472 4c7c 03a0 077c 04a1 0101 0071  .|.rL|...|.....q
+00001c80: 3374 0864 0a88 009b 0064 0b74 046a 059b  3t.d.....d.t.j..
+00001c90: 0064 0c74 046a 059b 0064 0d9d 0783 0182  .d.t.j...d......
+00001ca0: 017c 017c 037c 0266 0353 0029 0e4e 6301  .|.|.|.f.S.).Nc.
+00001cb0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001cc0: 0000 0053 0000 0072 8200 0000 7214 0000  ...S...r....r...
+00001cd0: 00a9 0172 8c00 0000 7284 0000 0072 1400  ...r....r....r..
+00001ce0: 0000 7214 0000 0072 1500 0000 7239 0000  ..r....r....r9..
+00001cf0: 0009 0100 0072 8500 0000 7a2a 5574 696c  .....r....z*Util
+00001d00: 732e 6669 6e64 5f63 6f6c 756d 6e5f 6c6f  s.find_column_lo
+00001d10: 6373 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  cs.<locals>.<lis
+00001d20: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
+00001d30: 0000 0003 0000 0003 0000 0073 0000 00f3  ...........s....
+00001d40: 2000 0000 8100 7c00 5d0b 5c02 7d01 7d02   .....|.].\.}.}.
+00001d50: 6400 7c02 7600 7202 7c01 5600 0100 7102  d.|.v.r.|.V...q.
+00001d60: 6401 5300 2902 7a0b 6967 6e6f 7265 2066  d.S.).z.ignore f
+00001d70: 696c 654e 7214 0000 00a9 0372 3700 0000  ileNr......r7...
+00001d80: da07 636f 756e 7465 7272 4800 0000 7214  ..counterrH...r.
+00001d90: 0000 0072 1400 0000 7215 0000 00da 093c  ...r....r......<
+00001da0: 6765 6e65 7870 723e 0b01 0000 7304 0000  genexpr>....s...
+00001db0: 0002 801e 007a 2955 7469 6c73 2e66 696e  .....z)Utils.fin
+00001dc0: 645f 636f 6c75 6d6e 5f6c 6f63 732e 3c6c  d_column_locs.<l
+00001dd0: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+00001de0: 4663 0100 0000 0000 0000 0000 0000 0300  Fc..............
+00001df0: 0000 0300 0000 7300 0000 729d 0000 0029  ......s...r....)
+00001e00: 02da 0862 6173 656c 696e 654e 7214 0000  ...baselineNr...
+00001e10: 0072 9e00 0000 7214 0000 0072 1400 0000  .r....r....r....
+00001e20: 7215 0000 0072 a000 0000 0e01 0000 7308  r....r........s.
+00001e30: 0000 0002 800a 0006 010e ff7a 1c4e 6f20  ...........z.No 
+00001e40: 6261 7365 6c69 6e65 2063 6f6c 756d 6e20  baseline column 
+00001e50: 666f 756e 6420 696e 2072 3300 0000 6301  found in r3...c.
+00001e60: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00001e70: 0000 0033 0000 0073 2400 0000 8100 7c00  ...3...s$.....|.
+00001e80: 5d0d 5c02 7d01 7d02 8800 a000 a100 7c02  ].\.}.}.......|.
+00001e90: 6b02 7202 7c01 5600 0100 7102 6400 5300  k.r.|.V...q.d.S.
+00001ea0: 7241 0000 0072 9c00 0000 729e 0000 00a9  rA...r....r.....
+00001eb0: 01da 036b 6579 7214 0000 0072 1500 0000  ...keyr....r....
+00001ec0: 72a0 0000 0015 0100 0073 0400 0000 0280  r........s......
+00001ed0: 2200 7a05 4b65 7920 227a 0f22 206e 6f74  ".z.Key "z." not
+00001ee0: 2066 6f75 6e64 2069 6e20 7a76 2e20 4368   found in zv. Ch
+00001ef0: 6563 6b20 7468 6520 4372 6974 6963 616c  eck the Critical
+00001f00: 2050 6172 616d 6574 6572 7320 6f70 7469   Parameters opti
+00001f10: 6f6e 2069 6e20 7468 6520 5061 7273 696e  on in the Parsin
+00001f20: 6720 6d65 6e75 2028 7061 7261 6d65 7465  g menu (paramete
+00001f30: 725f 6469 6374 3120 6966 206e 6f74 2075  r_dict1 if not u
+00001f40: 7369 6e67 2074 6865 2047 5549 2920 636f  sing the GUI) co
+00001f50: 7272 6563 746c 7920 6d61 7463 6820 7468  rrectly match th
+00001f60: 6520 7a09 2068 6561 6465 7273 2e29 0972  e z. headers.).r
+00001f70: 4200 0000 da04 6e65 7874 7289 0000 00da  B.....nextr.....
+00001f80: 094e 616d 6545 7272 6f72 7256 0000 0072  .NameErrorrV...r
+00001f90: 7700 0000 da0e 7061 7261 6d65 7465 725f  w.....parameter_
+00001fa0: 6469 6374 da06 6170 7065 6e64 7296 0000  dict..appendr...
+00001fb0: 0029 05da 0574 6162 6c65 da11 6967 6e6f  .)...table..igno
+00001fc0: 7265 5f63 6f6c 756d 6e5f 6c6f 635a 1362  re_column_locZ.b
+00001fd0: 6173 656c 696e 655f 636f 6c75 6d6e 5f6c  aseline_column_l
+00001fe0: 6f63 da14 6372 6974 6963 616c 5f63 6f6c  oc..critical_col
+00001ff0: 756d 6e5f 6c6f 6373 5a0a 636f 6c75 6d6e  umn_locsZ.column
+00002000: 5f6c 6f63 7214 0000 0072 a200 0000 7215  _locr....r....r.
+00002010: 0000 00da 1066 696e 645f 636f 6c75 6d6e  .....find_column
+00002020: 5f6c 6f63 7307 0100 0073 2400 0000 1202  _locs....s$.....
+00002030: 1402 0201 04ff 1403 0201 04ff 0402 1201  ................
+00002040: 0402 0a01 1e01 0402 0c01 1202 0402 0afe  ................
+00002050: 0a04 7a16 5574 696c 732e 6669 6e64 5f63  ..z.Utils.find_c
+00002060: 6f6c 756d 6e5f 6c6f 6373 6301 0000 0000  olumn_locsc.....
+00002070: 0000 0000 0000 0004 0000 0008 0000 0043  ...............C
+00002080: 0000 0073 8200 0000 7c00 7205 7c00 7d01  ...s....|.r.|.}.
+00002090: 6e04 7400 a001 a100 7d01 7400 6a02 a003  n.t.....}.t.j...
+000020a0: 7c01 9b00 6401 7404 6a05 9b00 9d03 a101  |...d.t.j.......
+000020b0: 7226 7406 a007 7c01 9b00 6401 7404 6a05  r&t...|...d.t.j.
+000020c0: 9b00 9d03 a101 7d02 6402 7d03 7c02 7c03  ......}.d.}.|.|.
+000020d0: 6602 5300 7a0f 7406 a007 7c01 9b00 6403  f.S.z.t...|...d.
+000020e0: 9d02 a101 7d02 6404 7d03 5700 7c02 7c03  ....}.d.}.W.|.|.
+000020f0: 6602 5300 0400 7408 7940 0100 0100 0100  f.S...t.y@......
+00002100: 7409 6405 8301 8201 7700 2906 4e72 6300  t.d.....w.).Nrc.
+00002110: 0000 da0b 6261 7365 5f66 6f6c 6465 727a  ....base_folderz
+00002120: 152f 636f 7079 5f70 6172 616d 5661 6c75  ./copy_paramValu
+00002130: 6573 2e63 7376 da0d 7265 706f 7274 5f66  es.csv..report_f
+00002140: 6f6c 6465 727a b34d 616b 6520 7375 7265  olderz.Make sure
+00002150: 2061 2063 6f70 7920 6f66 2070 6172 616d   a copy of param
+00002160: 5661 6c75 6573 2e63 7376 2069 7320 696e  Values.csv is in
+00002170: 2074 6865 2063 686f 7365 6e20 666f 6c64   the chosen fold
+00002180: 6572 2e20 0a41 6c73 6f20 6d61 6b65 2073  er. .Also make s
+00002190: 7572 6520 7468 6520 7365 6c65 6374 6564  ure the selected
+000021a0: 2066 6f6c 6465 7220 636f 6e74 6169 6e73   folder contains
+000021b0: 2061 6c6c 2074 6865 2070 6172 7469 6369   all the partici
+000021c0: 7061 6e74 2064 6972 6563 746f 7269 6573  pant directories
+000021d0: 2069 6e20 7468 6520 6e65 6365 7373 6172   in the necessar
+000021e0: 7920 4249 4453 2066 6f72 6d61 7420 652e  y BIDS format e.
+000021f0: 672e 2073 7562 2d30 312e 290a 7234 0000  g. sub-01.).r4..
+00002200: 00da 0667 6574 6377 6472 3500 0000 da06  ...getcwdr5.....
+00002210: 6973 6669 6c65 7256 0000 0072 7700 0000  isfilerV...rw...
+00002220: 724c 0000 00da 0872 6561 645f 6373 7672  rL.....read_csvr
+00002230: 5400 0000 7296 0000 0029 0472 3c00 0000  T...r....).r<...
+00002240: 7299 0000 0072 a800 0000 da0b 666f 6c64  r....r......fold
+00002250: 6572 5f74 7970 6572 1400 0000 7214 0000  er_typer....r...
+00002260: 0072 1500 0000 da15 6c6f 6164 5f70 6172  .r......load_par
+00002270: 616d 5661 6c75 6573 5f66 696c 6520 0100  amValues_file ..
+00002280: 0073 1c00 0000 0402 0601 0802 1802 1601  .s..............
+00002290: 0401 080c 02f7 1001 0601 0807 0cfb 0801  ................
+000022a0: 02ff 7a1b 5574 696c 732e 6c6f 6164 5f70  ..z.Utils.load_p
+000022b0: 6172 616d 5661 6c75 6573 5f66 696c 6563  aramValues_filec
+000022c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000022d0: 0800 0000 4300 0000 7326 0000 007a 0874  ....C...s&...z.t
+000022e0: 00a0 017c 00a1 0101 0057 0064 0053 0004  ...|.....W.d.S..
+000022f0: 0074 0279 1201 0001 0001 0059 0064 0053  .t.y.......Y.d.S
+00002300: 0077 0072 4100 0000 2903 7234 0000 00da  .w.rA...).r4....
+00002310: 056d 6b64 6972 da0f 4669 6c65 4578 6973  .mkdir..FileExis
+00002320: 7473 4572 726f 7229 0172 3500 0000 7214  tsError).r5...r.
+00002330: 0000 0072 1400 0000 7215 0000 0072 7c00  ...r....r....r|.
+00002340: 0000 3701 0000 730a 0000 0002 0210 010c  ..7...s.........
+00002350: 0106 0102 ff7a 0c55 7469 6c73 2e6d 6b5f  .....z.Utils.mk_
+00002360: 6469 7263 0000 0000 0000 0000 0000 0000  dirc............
+00002370: 0100 0000 0400 0000 4700 0000 731e 0000  ........G...s...
+00002380: 0074 007c 0064 0119 007c 0064 0219 0083  .t.|.d...|.d....
+00002390: 027c 0064 0364 0085 0219 008e 0053 0029  .|.d.d.......S.)
+000023a0: 044e 7201 0000 0072 1e00 0000 e902 0000  .Nr....r........
+000023b0: 0029 01da 0767 6574 6174 7472 a901 da04  .)...getattr....
+000023c0: 6172 6776 7214 0000 0072 1400 0000 7215  argvr....r....r.
+000023d0: 0000 00da 1769 6e73 7461 6e63 655f 6d65  .....instance_me
+000023e0: 7468 6f64 5f68 616e 646c 6572 3e01 0000  thod_handler>...
+000023f0: 7302 0000 001e 027a 1d55 7469 6c73 2e69  s......z.Utils.i
+00002400: 6e73 7461 6e63 655f 6d65 7468 6f64 5f68  nstance_method_h
+00002410: 616e 646c 6572 6300 0000 0000 0000 0000  andlerc.........
+00002420: 0000 0001 0000 0004 0000 0047 0000 0073  ...........G...s
+00002430: 1400 0000 7c00 6401 1900 7c00 6402 6400  ....|.d...|.d.d.
+00002440: 8502 1900 8e00 5300 2903 4e72 0100 0000  ......S.).Nr....
+00002450: 721e 0000 0072 1400 0000 72b7 0000 0072  r....r....r....r
+00002460: 1400 0000 7214 0000 0072 1500 0000 da14  ....r....r......
+00002470: 636c 6173 735f 6d65 7468 6f64 5f68 616e  class_method_han
+00002480: 646c 6572 4201 0000 7251 0000 007a 1a55  dlerB...rQ...z.U
+00002490: 7469 6c73 2e63 6c61 7373 5f6d 6574 686f  tils.class_metho
+000024a0: 645f 6861 6e64 6c65 7263 0100 0000 0000  d_handlerc......
+000024b0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+000024c0: 0000 734e 0000 0074 006a 0164 016b 0272  ..sN...t.j.d.k.r
+000024d0: 0a74 02a0 03a1 007d 016e 0574 0474 006a  .t.....}.n.t.t.j
+000024e0: 0183 017d 0174 02a0 0564 02a1 017d 0274  ...}.t...d...}.t
+000024f0: 006a 0672 217c 0073 2174 0764 037c 019b  .j.r!|.s!t.d.|..
+00002500: 0064 049d 0383 0101 007c 026a 087c 0164  .d.......|.j.|.d
+00002510: 058d 0153 0029 064e da03 6d61 78da 0a66  ...S.).N..max..f
+00002520: 6f72 6b73 6572 7665 727a 200a 5374 6172  orkserverz .Star
+00002530: 7469 6e67 2070 726f 6365 7373 696e 6720  ting processing 
+00002540: 706f 6f6c 2075 7369 6e67 207a 0720 636f  pool using z. co
+00002550: 7265 732e 2901 da09 7072 6f63 6573 7365  res.)...processe
+00002560: 7329 0972 5600 0000 5a0e 6d61 785f 636f  s).rV...Z.max_co
+00002570: 7265 5f75 7361 6765 da02 6d70 da09 6370  re_usage..mp..cp
+00002580: 755f 636f 756e 7472 9000 0000 da0b 6765  u_countr......ge
+00002590: 745f 636f 6e74 6578 7472 5700 0000 7258  t_contextrW...rX
+000025a0: 0000 00da 0450 6f6f 6c29 03da 0772 6573  .....Pool)...res
+000025b0: 7461 7274 da07 776f 726b 6572 73da 0363  tart..workers..c
+000025c0: 7478 7214 0000 0072 1400 0000 7215 0000  txr....r....r...
+000025d0: 00da 1573 7461 7274 5f70 726f 6365 7373  ...start_process
+000025e0: 696e 675f 706f 6f6c 4601 0000 730e 0000  ing_poolF...s...
+000025f0: 000a 020a 010a 020a 020a 0210 010c 027a  ...............z
+00002600: 1b55 7469 6c73 2e73 7461 7274 5f70 726f  .Utils.start_pro
+00002610: 6365 7373 696e 675f 706f 6f6c 6302 0000  cessing_poolc...
+00002620: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00002630: 0043 0000 0073 2400 0000 7c00 a000 a100  .C...s$...|.....
+00002640: 0100 7c00 a001 a100 0100 7c01 7210 7402  ..|.......|.r.t.
+00002650: 6a03 6401 6402 8d01 7d00 7c00 5300 2903  j.d.d...}.|.S.).
+00002660: 4e54 2901 72c2 0000 0029 04da 0563 6c6f  NT).r....)...clo
+00002670: 7365 da04 6a6f 696e 7208 0000 0072 c500  se..joinr....r..
+00002680: 0000 2902 da04 706f 6f6c 72c2 0000 0072  ..)...poolr....r
+00002690: 1400 0000 7214 0000 0072 1500 0000 da14  ....r....r......
+000026a0: 6a6f 696e 5f70 726f 6365 7373 696e 675f  join_processing_
+000026b0: 706f 6f6c 5401 0000 730a 0000 0008 0208  poolT...s.......
+000026c0: 0104 020c 0104 027a 1a55 7469 6c73 2e6a  .......z.Utils.j
+000026d0: 6f69 6e5f 7072 6f63 6573 7369 6e67 5f70  oin_processing_p
+000026e0: 6f6f 6c63 0500 0000 0000 0000 0000 0000  oolc............
+000026f0: 0800 0000 0a00 0000 4300 0000 7318 0100  ........C...s...
+00002700: 0074 007c 019b 0064 017c 029b 009d 0364  .t.|...d.|.....d
+00002710: 0283 028f 787d 057a 677c 05a0 01a1 007d  ....x}.zg|.....}
+00002720: 0674 02a0 0364 03a0 047c 06a1 01a1 017d  .t...d...|.....}
+00002730: 067c 0644 005d 0c7d 077c 067c 0719 0064  .|.D.].}.|.|...d
+00002740: 046b 0272 2664 007c 067c 073c 0071 1a7c  .k.r&d.|.|.<.q.|
+00002750: 0372 2974 0564 1069 007c 06a4 018e 0161  .r)t.d.i.|.....a
+00002760: 0674 076a 08a0 097c 01a1 0164 0519 0064  .t.j...|...d...d
+00002770: 066b 0272 5667 0064 07a2 0167 0064 08a2  .k.rVg.d...g.d..
+00002780: 0164 099c 0274 065f 0a64 0a64 0b84 0074  .d...t._.d.d...t
+00002790: 0b74 0c74 066a 0d83 0183 0144 0083 0174  .t.t.j.....D...t
+000027a0: 065f 0e74 0fa0 1074 06a1 0101 007c 0264  ._.t...t.....|.d
+000027b0: 0c6b 0272 697c 0474 065f 117c 0474 065f  .k.ri|.t._.|.t._
+000027c0: 1264 0d74 065f 1364 0e74 065f 1464 0e74  .d.t._.d.t._.d.t
+000027d0: 065f 1574 0657 0057 0002 0064 0004 0004  ._.t.W.W...d....
+000027e0: 0083 0301 0053 0004 0074 026a 166a 1774  .....S...t.j.j.t
+000027f0: 1866 0279 8101 0001 0001 0074 1964 0f83  .f.y.......t.d..
+00002800: 0182 0177 0031 0073 8577 0101 0001 0001  ...w.1.s.w......
+00002810: 0059 0001 0064 0053 0029 114e 7263 0000  .Y...d.S.).Nrc..
+00002820: 0072 6500 0000 7223 0000 00da 044e 6f6e  .re...r#.....Non
+00002830: 6572 6700 0000 5a0c 726f 695f 616e 616c  erg...Z.roi_anal
+00002840: 7973 6973 290b 7a0c 546f 7461 6c20 766f  ysis).z.Total vo
+00002850: 7865 6c73 7a0f 4578 636c 7564 6564 2076  xelsz.Excluded v
+00002860: 6f78 656c 737a 1a41 7665 7261 6765 2076  oxelsz.Average v
+00002870: 6f78 656c 7320 7065 7220 7365 7373 696f  oxels per sessio
+00002880: 6eda 044d 6561 6eda 0753 7464 5f64 6576  n..Mean..Std_dev
+00002890: da13 436f 6e66 6964 656e 6365 5f69 6e74  ..Confidence_int
+000028a0: 6572 7661 6cda 064d 6564 6961 6eda 074d  erval..Median..M
+000028b0: 696e 696d 756d da07 4d61 7869 6d75 6dda  inimum..Maximum.
+000028c0: 0c50 6172 7469 6369 7061 6e74 73da 0853  .Participants..S
+000028d0: 6573 7369 6f6e 7329 0a5a 0c56 6f78 656c  essions).Z.Voxel
+000028e0: 5f61 6d6f 756e 74da 1645 7863 6c75 6465  _amount..Exclude
+000028f0: 645f 766f 7865 6c73 5f61 6d6f 756e 745a  d_voxels_amountZ
+00002900: 0e41 7665 7261 6765 5f76 6f78 656c 7372  .Average_voxelsr
+00002910: cb00 0000 5a12 5374 616e 6461 7264 5f64  ....Z.Standard_d
+00002920: 6576 6961 7469 6f6e 72cd 0000 0072 ce00  eviationr....r..
+00002930: 0000 72cf 0000 0072 d000 0000 72d2 0000  ..r....r....r...
+00002940: 0029 0272 9400 0000 7293 0000 0063 0100  .).r....r....c..
+00002950: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00002960: 0000 5300 0000 731e 0000 0069 007c 005d  ..S...s....i.|.]
+00002970: 0b7d 0174 006a 017c 0119 0074 006a 027c  .}.t.j.|...t.j.|
+00002980: 0119 0093 0271 0253 0072 1400 0000 2903  .....q.S.r....).
+00002990: 7256 0000 00da 0f70 6172 616d 6574 6572  rV.....parameter
+000029a0: 5f64 6963 7431 da0f 7061 7261 6d65 7465  _dict1..paramete
+000029b0: 725f 6469 6374 3229 0272 3700 0000 da01  r_dict2).r7.....
+000029c0: 6972 1400 0000 7214 0000 0072 1500 0000  ir....r....r....
+000029d0: da0a 3c64 6963 7463 6f6d 703e 8801 0000  ..<dictcomp>....
+000029e0: 730a 0000 0006 0002 0108 ff08 0106 ff7a  s..............z
+000029f0: 2555 7469 6c73 2e6c 6f61 645f 636f 6e66  %Utils.load_conf
+00002a00: 6967 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  ig.<locals>.<dic
+00002a10: 7463 6f6d 703e 7a10 7465 7374 5f63 6f6e  tcomp>z.test_con
+00002a20: 6669 672e 746f 6d6c 5a0f 7465 7374 5f52  fig.tomlZ.test_R
+00002a30: 4f49 5f72 6570 6f72 745a 0974 6573 745f  OI_reportZ.test_
+00002a40: 6d61 7073 7a35 436f 6e66 6967 2066 696c  mapsz5Config fil
+00002a50: 6520 6e6f 7420 696e 2063 6f72 7265 6374  e not in correct
+00002a60: 2066 6f72 6d61 7420 6f72 206d 6973 7369   format or missi
+00002a70: 6e67 2065 6e74 7269 6573 2e72 1400 0000  ng entries.r....
+00002a80: 291a 7268 0000 00da 0972 6561 646c 696e  ).rh.....readlin
+00002a90: 6573 da04 746f 6d6c da05 6c6f 6164 7372  es..toml..loadsr
+00002aa0: c700 0000 7206 0000 0072 5600 0000 7234  ....r....rV...r4
+00002ab0: 0000 0072 3500 0000 726b 0000 00da 1173  ...r5...rk.....s
+00002ac0: 7461 7469 7374 6963 5f6f 7074 696f 6e73  tatistic_options
+00002ad0: 728d 0000 0072 8e00 0000 72d4 0000 0072  r....r....r....r
+00002ae0: a600 0000 7208 0000 00da 1463 6c65 616e  ....r......clean
+00002af0: 5f63 6f6e 6669 675f 6f70 7469 6f6e 73da  _config_options.
+00002b00: 0e62 7261 696e 5f66 696c 655f 6c6f 6372  .brain_file_locr
+00002b10: ac00 0000 da0d 6f75 7470 7574 5f66 6f6c  ......output_fol
+00002b20: 6465 725a 126f 7574 7075 745f 666f 6c64  derZ.output_fold
+00002b30: 6572 5f6e 616d 65da 0f73 7461 745f 6d61  er_name..stat_ma
+00002b40: 705f 666f 6c64 6572 da07 6465 636f 6465  p_folder..decode
+00002b50: 72da 0f54 6f6d 6c44 6563 6f64 6545 7272  r..TomlDecodeErr
+00002b60: 6f72 da0e 4174 7472 6962 7574 6545 7272  or..AttributeErr
+00002b70: 6f72 7296 0000 0029 08da 0363 6c73 726c  orr....)...clsrl
+00002b80: 0000 00da 0866 696c 656e 616d 65da 0473  .....filename..s
+00002b90: 6176 6572 3500 0000 da08 746f 6d6c 6669  aver5.....tomlfi
+00002ba0: 6c65 da05 7061 7273 6572 a300 0000 7214  le..parser....r.
+00002bb0: 0000 0072 1400 0000 7215 0000 00da 0b6c  ...r....r......l
+00002bc0: 6f61 645f 636f 6e66 6967 5e01 0000 733c  oad_config^...s<
+00002bd0: 0000 0016 0202 0108 0110 0108 020c 0108  ................
+00002be0: 0102 8004 020e 0314 0206 0206 0c08 f306  ................
+00002bf0: 190c 0108 ff0a 0308 0206 0206 0106 0106  ................
+00002c00: 0106 0104 0210 cb14 3708 0102 ff14 c97a  ........7......z
+00002c10: 1155 7469 6c73 2e6c 6f61 645f 636f 6e66  .Utils.load_conf
+00002c20: 6967 6301 0000 0000 0000 0000 0000 0003  igc.............
+00002c30: 0000 0007 0000 0043 0000 0073 6e00 0000  .......C...sn...
+00002c40: 6700 6401 a201 7d01 7400 7c00 6a01 8301  g.d...}.t.|.j...
+00002c50: 7402 7501 7212 7c01 a003 7c00 6a01 a101  t.u.r.|...|.j...
+00002c60: 7c00 5f01 6700 6402 a201 7d02 7400 7c00  |._.g.d...}.t.|.
+00002c70: 6a04 8301 7402 7501 7235 6403 7405 6404  j...t.u.r5d.t.d.
+00002c80: 7406 a007 6405 7c00 6a04 a102 6406 1900  t...d.|.j...d...
+00002c90: 9b00 9d02 8301 1800 7c00 5f08 7c02 a003  ........|._.|...
+00002ca0: 7c00 6a04 a101 7c00 5f04 7c00 5300 2907  |.j...|._.|.S.).
+00002cb0: 4e29 0d7a 1343 6572 6562 656c 6c75 6d2d  N).z.Cerebellum-
+00002cc0: 4d4e 4966 6c69 7274 7a13 4365 7265 6265  MNIflirtz.Cerebe
+00002cd0: 6c6c 756d 2d4d 4e49 666e 6972 747a 1248  llum-MNIfnirtz.H
+00002ce0: 6172 7661 7264 4f78 666f 7264 2d63 6f72  arvardOxford-cor
+00002cf0: 747a 1148 6172 7661 7264 4f78 666f 7264  tz.HarvardOxford
+00002d00: 2d73 7562 7a0f 4a48 552d 4943 424d 2d6c  -subz.JHU-ICBM-l
+00002d10: 6162 656c 737a 0f4a 4855 2d49 4342 4d2d  abelsz.JHU-ICBM-
+00002d20: 7472 6163 7473 5a07 6a75 656c 6963 68da  tractsZ.juelich.
+00002d30: 034d 4e49 7a0c 534d 4154 542d 6c61 6265  .MNIz.SMATT-labe
+00002d40: 6c73 da03 5354 4e7a 1373 7472 6961 7475  ls..STNz.striatu
+00002d50: 6d2d 7374 7275 6374 7572 616c 7a10 5461  m-structuralz.Ta
+00002d60: 6c61 6972 6163 682d 6c61 6265 6c73 da08  lairach-labels..
+00002d70: 5468 616c 616d 7573 2906 7a09 3830 252c  Thalamus).z.80%,
+00002d80: 2031 2e32 387a 0938 3525 2c20 312e 3434   1.28z.85%, 1.44
+00002d90: 7a09 3930 252c 2031 2e36 347a 0939 3525  z.90%, 1.64z.95%
+00002da0: 2c20 312e 3936 7a09 3938 252c 2032 2e33  , 1.96z.98%, 2.3
+00002db0: 337a 0939 3925 2c20 322e 3538 721e 0000  3z.99%, 2.58r...
+00002dc0: 007a 0230 2e72 2200 0000 7201 0000 0029  .z.0.r"...r....)
+00002dd0: 0972 1f00 0000 da0c 6174 6c61 735f 6e75  .r......atlas_nu
+00002de0: 6d62 6572 7290 0000 0072 4a00 0000 da11  mberr....rJ.....
+00002df0: 636f 6e66 5f6c 6576 656c 5f6e 756d 6265  conf_level_numbe
+00002e00: 72da 0566 6c6f 6174 da02 7265 726b 0000  r..float..rerk..
+00002e10: 00da 0f62 6f6f 7473 7472 6170 5f61 6c70  ...bootstrap_alp
+00002e20: 6861 2903 7256 0000 00da 0d61 746c 6173  ha).rV.....atlas
+00002e30: 5f6f 7074 696f 6e73 5a12 636f 6e66 5f6c  _optionsZ.conf_l
+00002e40: 6576 656c 5f6f 7074 696f 6e73 7214 0000  evel_optionsr...
+00002e50: 0072 1400 0000 7215 0000 0072 dc00 0000  .r....r....r....
+00002e60: 9a01 0000 7310 0000 0008 020e 050e 0108  ....s...........
+00002e70: 020e 0222 010e 0104 027a 1a55 7469 6c73  ...".....z.Utils
+00002e80: 2e63 6c65 616e 5f63 6f6e 6669 675f 6f70  .clean_config_op
+00002e90: 7469 6f6e 7363 0100 0000 0000 0000 0000  tionsc..........
+00002ea0: 0000 0300 0000 0300 0000 4300 0000 7320  ..........C...s 
+00002eb0: 0000 0074 00a0 017c 00a1 017d 017c 016a  ...t...|...}.|.j
+00002ec0: 027d 027c 01a0 03a1 007d 017c 017c 0266  .}.|.....}.|.|.f
+00002ed0: 0253 0072 4100 0000 2904 da03 6e69 62da  .S.rA...)...nib.
+00002ee0: 046c 6f61 64da 0668 6561 6465 72da 0967  .load..header..g
+00002ef0: 6574 5f66 6461 7461 2903 da09 6669 6c65  et_fdata)...file
+00002f00: 5f70 6174 68da 0464 6174 6172 f400 0000  _path..datar....
+00002f10: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00002f20: 0a6c 6f61 645f 6272 6169 6eac 0100 0073  .load_brain....s
+00002f30: 0800 0000 0a02 0602 0801 0802 7a10 5574  ............z.Ut
+00002f40: 696c 732e 6c6f 6164 5f62 7261 696e 6301  ils.load_brainc.
+00002f50: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+00002f60: 0000 0043 0000 0073 2200 0000 6700 6401  ...C...s"...g.d.
+00002f70: a201 7d01 7c01 4400 5d08 7d02 7c00 a000  ..}.|.D.].}.|...
+00002f80: 7c02 6402 a102 7d00 7106 7c00 5300 2903  |.d...}.q.|.S.).
+00002f90: 4e29 04fa 072e 6e69 692e 677a 7a04 2e6e  N)....nii.gzz..n
+00002fa0: 6969 7a04 2e68 6472 7a05 2e6a 736f 6e72  iiz..hdrz..jsonr
+00002fb0: 2300 0000 2901 722a 0000 0029 0372 3500  #...).r*...).r5.
+00002fc0: 0000 723d 0000 0072 3f00 0000 7214 0000  ..r=...r?...r...
+00002fd0: 0072 1400 0000 7215 0000 00da 0973 7472  .r....r......str
+00002fe0: 6970 5f65 7874 b501 0000 7308 0000 0008  ip_ext....s.....
+00002ff0: 0208 020e 0104 027a 0f55 7469 6c73 2e73  .......z.Utils.s
+00003000: 7472 6970 5f65 7874 6301 0000 0000 0000  trip_extc.......
+00003010: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00003020: 0073 5c00 0000 6401 6402 8400 7400 7c00  .s\...d.d...t.|.
+00003030: 9b00 6403 9d02 8301 4400 8301 7d01 6404  ..d.....D...}.d.
+00003040: 6402 8400 7c01 4400 8301 7d02 7401 7c01  d...|.D...}.t.|.
+00003050: 8301 6405 6b02 721d 7402 6406 8301 8201  ..d.k.r.t.d.....
+00003060: 7403 6a04 722a 7405 6407 7401 7c01 8301  t.j.r*t.d.t.|...
+00003070: 9b00 6408 9d03 8301 0100 7c01 7c02 6602  ..d.......|.|.f.
+00003080: 5300 2909 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00003090: 0000 0200 0000 0600 0000 5300 0000 731c  ..........S...s.
+000030a0: 0000 0067 007c 005d 0a7d 0174 00a0 0164  ...g.|.].}.t...d
+000030b0: 007c 01a1 0272 027c 0191 0271 0253 0029  .|...r.|...q.S.)
+000030c0: 017a 0b73 7562 2d5b 302d 395d 2b24 2902  .z.sub-[0-9]+$).
+000030d0: 72ef 0000 00da 0673 6561 7263 6829 0272  r......search).r
+000030e0: 3700 0000 da05 6469 7265 6372 1400 0000  7.....direcr....
+000030f0: 7214 0000 0072 1500 0000 7239 0000 00c1  r....r....r9....
+00003100: 0100 0073 0200 0000 1c00 7a2f 5574 696c  ...s......z/Util
+00003110: 732e 6669 6e64 5f70 6172 7469 6369 7061  s.find_participa
+00003120: 6e74 5f64 6972 732e 3c6c 6f63 616c 733e  nt_dirs.<locals>
+00003130: 2e3c 6c69 7374 636f 6d70 3e7a 022f 2a63  .<listcomp>z./*c
+00003140: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003150: 0500 0000 5300 0000 731a 0000 0067 007c  ....S...s....g.|
+00003160: 005d 097d 017c 01a0 0064 00a1 0164 0119  .].}.|...d...d..
+00003170: 0091 0271 0253 0029 0272 6300 0000 7267  ...q.S.).rc...rg
+00003180: 0000 0029 0172 6b00 0000 2902 7237 0000  ...).rk...).r7..
+00003190: 00da 0b70 6172 7469 6369 7061 6e74 7214  ...participantr.
+000031a0: 0000 0072 1400 0000 7215 0000 0072 3900  ...r....r....r9.
+000031b0: 0000 c201 0000 7302 0000 001a 0072 0100  ......s......r..
+000031c0: 0000 7a9e 5061 7274 6963 6970 616e 7420  ..z.Participant 
+000031d0: 6469 7265 6374 6f72 6965 7320 6e6f 7420  directories not 
+000031e0: 666f 756e 642e 0a4d 616b 6520 7375 7265  found..Make sure
+000031f0: 2070 6172 7469 6369 7061 6e74 2064 6972   participant dir
+00003200: 6563 746f 7269 6573 2061 7265 206c 6162  ectories are lab
+00003210: 656c 6c65 6420 652e 672e 2073 7562 2d30  elled e.g. sub-0
+00003220: 3120 616e 6420 7468 6520 7365 6c65 6374  1 and the select
+00003230: 6564 2064 6972 6563 746f 7279 2063 6f6e  ed directory con
+00003240: 7461 696e 7320 616c 6c20 7061 7274 6963  tains all partic
+00003250: 6970 616e 7420 6469 7265 6374 6f72 6965  ipant directorie
+00003260: 732e 7a06 466f 756e 6420 7a15 2070 6172  s.z.Found z. par
+00003270: 7469 6369 7061 6e74 2066 6f6c 6465 7273  ticipant folders
+00003280: 2e29 0672 0200 0000 728e 0000 0072 5400  .).r....r....rT.
+00003290: 0000 7256 0000 0072 5700 0000 7258 0000  ..rV...rW...rX..
+000032a0: 0029 0372 3c00 0000 5a11 7061 7274 6963  .).r<...Z.partic
+000032b0: 6970 616e 745f 7061 7468 73da 1170 6172  ipant_paths..par
+000032c0: 7469 6369 7061 6e74 5f6e 616d 6573 7214  ticipant_namesr.
+000032d0: 0000 0072 1400 0000 7215 0000 00da 1566  ...r....r......f
+000032e0: 696e 645f 7061 7274 6963 6970 616e 745f  ind_participant_
+000032f0: 6469 7273 be01 0000 730e 0000 0018 030e  dirs....s.......
+00003300: 010c 0208 0106 0314 0108 027a 1b55 7469  ...........z.Uti
+00003310: 6c73 2e66 696e 645f 7061 7274 6963 6970  ls.find_particip
+00003320: 616e 745f 6469 7273 6301 0000 0000 0000  ant_dirsc.......
+00003330: 0000 0000 0004 0000 0008 0000 0043 0000  .............C..
+00003340: 0073 a400 0000 7c00 6100 6401 7d01 6402  .s....|.a.d.}.d.
+00003350: 7d02 7401 6403 7c00 9b00 6404 7402 7c01  }.t.d.|...d.t.|.
+00003360: 8301 9b00 6405 7402 7c02 8301 9b00 6406  ....d.t.|.....d.
+00003370: 9d07 8301 0100 7403 6a04 6400 6407 8502  ......t.j.d.d...
+00003380: 1900 7c01 7c02 6602 6b03 7250 7402 7403  ..|.|.f.k.rPt.t.
+00003390: 6a04 6408 1900 8301 9b00 6405 7402 7403  j.d.......d.t.t.
+000033a0: 6a04 6409 1900 8301 9b00 6405 7402 7403  j.d.......d.t.t.
+000033b0: 6a04 6407 1900 8301 9b00 9d05 7d03 7401  j.d.........}.t.
+000033c0: 640a 7c03 9b00 640b 7402 7c01 8301 9b00  d.|...d.t.|.....
+000033d0: 6405 7402 7c02 8301 9b00 640c 9d07 8301  d.t.|.....d.....
+000033e0: 0100 6400 5300 6400 5300 290d 4ee9 0300  ..d.S.d.S.).N...
+000033f0: 0000 e90a 0000 007a 060a 6652 4154 207a  .......z..fRAT z
+00003400: 2520 6973 2064 6576 656c 6f70 6564 2061  % is developed a
+00003410: 6e64 2074 6573 7465 6420 7769 7468 2050  nd tested with P
+00003420: 7974 686f 6e20 7233 0000 007a 022e 0a72  ython r3...z...r
+00003430: b500 0000 7201 0000 0072 1e00 0000 7a15  ....r....r....z.
+00003440: 494e 464f 3a20 5079 7468 6f6e 2076 6572  INFO: Python ver
+00003450: 7369 6f6e 207a 2b20 6973 2075 6e74 6573  sion z+ is untes
+00003460: 7465 642e 2043 6f6e 7369 6465 7220 6368  ted. Consider ch
+00003470: 616e 6769 6e67 2074 6f20 7665 7273 696f  anging to versio
+00003480: 6e20 7a22 2069 6620 7468 6572 6520 6172  n z" if there ar
+00003490: 6520 6572 726f 7273 2072 756e 6e69 6e67  e errors running
+000034a0: 2066 5241 542e 2905 7269 0000 0072 5800   fRAT.).ri...rX.
+000034b0: 0000 725d 0000 00da 0373 7973 da0c 7665  ..r].....sys..ve
+000034c0: 7273 696f 6e5f 696e 666f 2904 5a0c 6672  rsion_info).Z.fr
+000034d0: 6174 5f76 6572 7369 6f6e 5a0c 6578 7065  at_versionZ.expe
+000034e0: 6374 5f6d 616a 6f72 5a0c 6578 7065 6374  ct_majorZ.expect
+000034f0: 5f6d 696e 6f72 5a0f 6375 7272 656e 745f  _minorZ.current_
+00003500: 7665 7273 696f 6e72 1400 0000 7214 0000  versionr....r...
+00003510: 0072 1500 0000 da0c 6368 6563 6b76 6572  .r......checkver
+00003520: 7369 6f6e cd01 0000 7318 0000 0004 0304  sion....s.......
+00003530: 0304 0124 0216 0132 010a 0106 0104 ff06  ...$...2........
+00003540: 010e ff04 fe7a 1255 7469 6c73 2e63 6865  .....z.Utils.che
+00003550: 636b 7665 7273 696f 6e63 0200 0000 0000  ckversionc......
+00003560: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
+00003570: 0000 73ae 0000 007c 0064 016b 0272 097c  ..s....|.d.k.r.|
+00003580: 016a 0072 0964 0053 007c 016a 0172 2364  .j.r.d.S.|.j.r#d
+00003590: 0264 036c 026d 037d 0201 0074 04a0 05a1  .d.l.m.}...t....
+000035a0: 009b 0064 047c 026a 069b 009d 037d 0374  ...d.|.j.....}.t
+000035b0: 04a0 077c 03a1 0101 007c 0353 007c 016a  ...|.....|.S.|.j
+000035c0: 0864 0576 0072 3574 0964 0683 0101 0074  .d.v.r5t.d.....t
+000035d0: 0a6a 0b64 0764 0864 098d 027d 037c 0353  .j.d.d.d...}.|.S
+000035e0: 007c 016a 087d 037a 0774 04a0 077c 03a1  .|.j.}.z.t...|..
+000035f0: 0101 0057 006e 0b04 0074 0c79 4a01 0001  ...W.n...t.yJ...
+00003600: 0001 0074 0c64 0a83 0182 0177 007c 016a  ...t.d.....w.|.j
+00003610: 0d72 5574 0964 0b7c 039b 009d 0283 0101  .rUt.d.|........
+00003620: 007c 0353 0029 0c4e da0a 5374 6174 6973  .|.S.).N..Statis
+00003630: 7469 6373 721e 0000 0029 01da 1145 6e76  ticsr....)...Env
+00003640: 6972 6f6e 6d65 6e74 5f53 6574 7570 7263  ironment_Setuprc
+00003650: 0000 0029 0272 2300 0000 fa01 207a 2853  ...).r#..... z(S
+00003660: 656c 6563 7420 7468 6520 6469 7265 6374  elect the direct
+00003670: 6f72 7920 6f75 7470 7574 2062 7920 7468  ory output by th
+00003680: 6520 6652 4154 2e7a 2753 656c 6563 7420  e fRAT.z'Select 
+00003690: 7468 6520 6469 7265 6374 6f72 7920 6f75  the directory ou
+000036a0: 7470 7574 2062 7920 7468 6520 6652 4154  tput by the fRAT
+000036b0: 5429 0272 0b00 0000 7255 0000 007a 4e4f  T).r....rU...zNO
+000036c0: 7574 7075 7420 666f 6c64 6572 206c 6f63  utput folder loc
+000036d0: 6174 696f 6e20 2866 5241 5420 6f75 7470  ation (fRAT outp
+000036e0: 7574 2066 6f6c 6465 7220 6c6f 6361 7469  ut folder locati
+000036f0: 6f6e 2920 6973 206e 6f74 2061 2076 616c  on) is not a val
+00003700: 6964 2064 6972 6563 746f 7279 2e7a 194f  id directory.z.O
+00003710: 7574 7075 7420 666f 6c64 6572 2073 656c  utput folder sel
+00003720: 6563 7469 6f6e 3a20 290e da0c 7275 6e5f  ection: )...run_
+00003730: 706c 6f74 7469 6e67 da0c 7275 6e5f 616e  plotting..run_an
+00003740: 616c 7973 6973 da08 616e 616c 7973 6973  alysis..analysis
+00003750: 7206 0100 0072 3400 0000 72ae 0000 00da  r....r4...r.....
+00003760: 0d73 6176 655f 6c6f 6361 7469 6f6e 7255  .save_locationrU
+00003770: 0000 005a 1472 6570 6f72 745f 6f75 7470  ...Z.report_outp
+00003780: 7574 5f66 6f6c 6465 7272 5800 0000 7208  ut_folderrX...r.
+00003790: 0000 0072 5a00 0000 7254 0000 0072 5700  ...rZ...rT...rW.
+000037a0: 0000 2904 5a0c 6375 7272 656e 745f 7374  ..).Z.current_st
+000037b0: 6570 7256 0000 0072 0601 0000 5a0e 6a73  eprV...r....Z.js
+000037c0: 6f6e 5f64 6972 6563 746f 7279 7214 0000  on_directoryr...
+000037d0: 0072 1400 0000 7215 0000 00da 1963 6864  .r....r......chd
+000037e0: 6972 5f74 6f5f 6f75 7470 7574 5f64 6972  ir_to_output_dir
+000037f0: 6563 746f 7279 dc01 0000 732c 0000 000e  ectory....s,....
+00003800: 0204 0106 020c 0114 010a 0204 120a f008  ................
+00003810: 010e 0104 0e06 f502 020e 010c 0102 0102  ................
+00003820: 0104 ff02 ff06 040e 0104 027a 1f55 7469  ...........z.Uti
+00003830: 6c73 2e63 6864 6972 5f74 6f5f 6f75 7470  ls.chdir_to_outp
+00003840: 7574 5f64 6972 6563 746f 7279 6305 0000  ut_directoryc...
+00003850: 0000 0000 0000 0000 0006 0000 0008 0000  ................
+00003860: 0043 0000 0073 3e00 0000 7400 a001 7c00  .C...s>...t...|.
+00003870: 6400 7c04 a103 7d05 7400 a002 7c05 7c03  d.|...}.t...|.|.
+00003880: 9b00 6401 7c02 9b00 7c01 9b00 6402 9d05  ..d.|...|...d...
+00003890: a102 0100 7c03 9b00 6401 7c02 9b00 7c01  ....|...d.|...|.
+000038a0: 9b00 6402 9d05 5300 2903 4e72 6300 0000  ..d...S.).Nrc...
+000038b0: 72f9 0000 0029 0372 f200 0000 da0a 4e69  r....).r......Ni
+000038c0: 6674 6931 5061 6972 72e5 0000 0029 0672  fti1Pairr....).r
+000038d0: f700 0000 da03 6578 745a 0b6e 6f5f 6578  ......extZ.no_ex
+000038e0: 745f 6669 6c65 72de 0000 0072 f400 0000  t_filer....r....
+000038f0: da05 6272 6169 6e72 1400 0000 7214 0000  ..brainr....r...
+00003900: 0072 1500 0000 da0a 7361 7665 5f62 7261  .r......save_bra
+00003910: 696e f901 0000 7306 0000 000e 021c 0114  in....s.........
+00003920: 027a 1055 7469 6c73 2e73 6176 655f 6272  .z.Utils.save_br
+00003930: 6169 6e29 0272 2300 0000 4629 034e 7261  ain).r#...F).Nra
+00003940: 0000 0072 6200 0000 2903 4654 4629 0146  ...rb...).FTF).F
+00003950: 2901 7223 0000 0029 0254 4e72 4100 0000  ).r#...).TNrA...
+00003960: 2920 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  ) ..__name__..__
+00003970: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00003980: 6e61 6d65 5f5f da0c 7374 6174 6963 6d65  name__..staticme
+00003990: 7468 6f64 7216 0000 0072 3200 0000 7240  thodr....r2...r@
+000039a0: 0000 0072 4900 0000 7250 0000 0072 5a00  ...rI...rP...rZ.
+000039b0: 0000 7260 0000 0072 7000 0000 7279 0000  ..r`...rp...ry..
+000039c0: 0072 7e00 0000 7292 0000 0072 9b00 0000  .r~...r....r....
+000039d0: 72ab 0000 0072 b200 0000 727c 0000 0072  r....r....r|...r
+000039e0: b900 0000 72ba 0000 0072 c500 0000 72c9  ....r....r....r.
+000039f0: 0000 00da 0b63 6c61 7373 6d65 7468 6f64  .....classmethod
+00003a00: 72e8 0000 0072 dc00 0000 72f8 0000 0072  r....r....r....r
+00003a10: fa00 0000 72ff 0000 0072 0401 0000 720c  ....r....r....r.
+00003a20: 0100 0072 1001 0000 7214 0000 0072 1400  ...r....r....r..
+00003a30: 0000 7214 0000 0072 1500 0000 7208 0000  ..r....r....r...
+00003a40: 0017 0000 0073 6e00 0000 0800 0201 0a01  .....sn.........
+00003a50: 020f 0a01 022a 0a01 020d 0a01 0207 0a01  .....*..........
+00003a60: 0203 0c01 0213 0a01 0206 0c01 021c 0c01  ................
+00003a70: 0214 0c01 0208 0a01 022e 0a01 0214 0a01  ................
+00003a80: 0218 0c01 0216 0a01 0206 0a01 0203 0a01  ................
+00003a90: 0203 0c01 020d 0a01 0209 0c01 023b 0a01  .............;..
+00003aa0: 0211 0a01 0208 0a01 0208 0a01 020e 0a01  ................
+00003ab0: 020e 0a01 021c 1001 7208 0000 0029 1972  ........r....).r
+00003ac0: 2500 0000 720c 0000 0072 3400 0000 72ef  %...r....r4...r.
+00003ad0: 0000 0072 7200 0000 7202 0100 0072 0200  ...rr...r....r..
+00003ae0: 0000 da07 7061 7468 6c69 6272 0300 0000  ....pathlibr....
+00003af0: da07 746b 696e 7465 7272 0400 0000 7205  ..tkinterr....r.
+00003b00: 0000 00da 0574 7970 6573 7206 0000 005a  .....typesr....Z
+00003b10: 0c6d 756c 7469 7072 6f63 6573 7372 be00  .multiprocessr..
+00003b20: 0000 da07 6e69 6261 6265 6c72 f200 0000  ....nibabelr....
+00003b30: da06 7061 6e64 6173 724c 0000 0072 d900  ..pandasrL...r..
+00003b40: 0000 da1c 6652 4154 2e75 7469 6c73 2e66  ....fRAT.utils.f
+00003b50: 5241 545f 636f 6e66 6967 5f73 6574 7570  RAT_config_setup
+00003b60: 7256 0000 0072 6900 0000 7208 0000 0072  rV...ri...r....r
+00003b70: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
+00003b80: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00003b90: 0073 2400 0000 0800 0801 0801 0801 0801  .s$.............
+00003ba0: 0801 0c01 0c01 1001 0c01 0802 0801 0801  ................
+00003bb0: 0801 0802 0402 0401 1203                 ..........
```

### Comparing `frat_brain-1.5.1/fRAT/utils/analysis.py` & `frat_brain-1.5.2/fRAT/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/bootstrap.css` & `frat_brain-1.5.2/fRAT/utils/bootstrap.css`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/dash_report.py` & `frat_brain-1.5.2/fRAT/utils/dash_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/directory_comparison.py` & `frat_brain-1.5.2/fRAT/utils/directory_comparison.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/fRAT_config_setup.py` & `frat_brain-1.5.2/fRAT/utils/fRAT_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/figures.py` & `frat_brain-1.5.2/fRAT/utils/figures.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/html_report.py` & `frat_brain-1.5.2/fRAT/utils/html_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/printResults.py` & `frat_brain-1.5.2/fRAT/utils/printResults.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/statistics.py` & `frat_brain-1.5.2/fRAT/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/statmap.py` & `frat_brain-1.5.2/fRAT/utils/statmap.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/statmap_config_setup.py` & `frat_brain-1.5.2/fRAT/utils/statmap_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.5.1/fRAT/utils/utils.py` & `frat_brain-1.5.2/fRAT/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,18 @@
             f.write('\n')
 
             current_section = None
             for line in r:
                 if line.startswith('#') and not line.startswith('##'):
                     current_section = line.replace('#', '')[1:-1]
 
+                if not line.startswith(('#', '\n')):
+                    # Remove parameter help text
+                    line = f"{line.split('#')[0]}\n"
+
                 if relevant_sections == 'all':
                     f.write(line)
                 elif current_section in relevant_sections:
                     f.write(line)
 
     @staticmethod
     def move_file(old_name, original_dir, new_dir, copy=False, rename_copy=True, parameter_file=False):
```

### Comparing `frat_brain-1.5.1/pyproject.toml` & `frat_brain-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frat-brain"
-version = "1.5.1"
+version = "1.5.2"
 description = "Application for ROI fMRI data analysis."
 authors = ["Elliot Howley <elliohow@hotmail.com>"]
 readme = "README.md"
 homepage = "https://fmri-roi-analysis-tool.readthedocs.io/en/latest/"
 repository = "https://github.com/elliohow/fMRI_ROI_Analysis_Tool"
 packages = [{include = "fRAT"}]
```

### Comparing `frat_brain-1.5.1/setup.py` & `frat_brain-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
  'zope-interface==5.2.0']
 
 entry_points = \
 {'console_scripts': ['fRAT = fRAT.__main__:start_gui']}
 
 setup_kwargs = {
     'name': 'frat-brain',
-    'version': '1.5.1',
+    'version': '1.5.2',
     'description': 'Application for ROI fMRI data analysis.',
     'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Citation\n\n**When using fRAT, please include the following citation:**\n\nHowley, E., Francis, S., & Schluppeck, D. (2023). fRAT: an interactive, Python-based tool for region-of-interest summaries of functional imaging data. Journal of Open Source Software, 8(85), 5200. https://doi.org/10.21105/joss.05200\n\n## Reporting bugs\n\nTo report a bug or suggest a new feature, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing to the project\n\nIf you\'d like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n',
     'author': 'Elliot Howley',
     'author_email': 'elliohow@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fmri-roi-analysis-tool.readthedocs.io/en/latest/',
```

### Comparing `frat_brain-1.5.1/PKG-INFO` & `frat_brain-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frat-brain
-Version: 1.5.1
+Version: 1.5.2
 Summary: Application for ROI fMRI data analysis.
 Home-page: https://fmri-roi-analysis-tool.readthedocs.io/en/latest/
 Author: Elliot Howley
 Author-email: elliohow@hotmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

