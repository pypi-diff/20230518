# Comparing `tmp/fw_gear_dcm2niix-2.0.0-py3-none-any.whl.zip` & `tmp/fw_gear_dcm2niix-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 25276 bytes, number of entries: 15
+Zip file size: 25338 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/__init__.py
 -rw-r--r--  2.0 unx    14361 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/arrange.py
 -rw-r--r--  2.0 unx     7642 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/dcm2niix_run.py
 -rw-r--r--  2.0 unx     5646 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/dcm2niix_utils.py
 -rw-r--r--  2.0 unx     3528 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/interfaces.py
 -rw-r--r--  2.0 unx     1240 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/prepare.py
 -rw-r--r--  2.0 unx       24 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/__init__.py
 -rw-r--r--  2.0 unx    15016 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/metadata.py
 -rw-r--r--  2.0 unx     7078 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/parse_config.py
 -rw-r--r--  2.0 unx     6904 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/resolve.py
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13561 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1354 b- defN 16-Jan-01 00:00 fw_gear_dcm2niix-2.0.0.dist-info/RECORD
-15 files, 77753 bytes uncompressed, 23000 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13774 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1354 b- defN 16-Jan-01 00:00 fw_gear_dcm2niix-2.0.1.dist-info/RECORD
+15 files, 77966 bytes uncompressed, 23062 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: fw_gear_dcm2niix/utils/parse_config.py
 Comment: 
 
 Filename: fw_gear_dcm2niix/utils/resolve.py
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.0.dist-info/LICENSE
+Filename: fw_gear_dcm2niix-2.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.0.dist-info/METADATA
+Filename: fw_gear_dcm2niix-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.0.dist-info/WHEEL
+Filename: fw_gear_dcm2niix-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.0.dist-info/RECORD
+Filename: fw_gear_dcm2niix-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fw_gear_dcm2niix-2.0.0.dist-info/LICENSE` & `fw_gear_dcm2niix-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_gear_dcm2niix-2.0.0.dist-info/METADATA` & `fw_gear_dcm2niix-2.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-gear-dcm2niix
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Flywheel Gear for implementing Chris Rorden's dcm2niix for converting DICOM (or PAR/REC) to NIfTI (or NRRD).
 Home-page: https://gitlab.com/flywheel-io/scientific-solutions/gears/dcm2niix/
 License: Other
 Keywords: Flywheel,Gears
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.9,<4.0
@@ -45,15 +45,15 @@
 dcm2niix doi: 10.1016/j.jneumeth.2016.03.001
 
 ### License 
 
 License: Other
 
 [Chris Rorden's dcm2niix](https://github.com/rordenlab/dcm2niix) is provided through
-its [license](https://github.com/rordenlab/dcm2niix/blob/v1.0.20220720/license.txt). 
+its [license](https://github.com/rordenlab/dcm2niix/blob/v1.0.20230411/license.txt). 
 
 ### Classification
 
 Category: converter
 
 Gear Level:
 
@@ -190,14 +190,19 @@
   - __Description__: Single file mode, do not convert other images in the folder. Options: true, false (default).
   - __Default__: False
 - tag
   - __Name__: tag
   - __Type__: string
   - __Description__: The tag to be added to one output file upon run completion.
   - __Default__: ""
+- tag_on_failure
+  - __Name__: tag_on_failure
+  - __Type__: Boolean
+  - __Description__: If `True`, tag the input file with "dcm2nii-failure" if the gear fails to generate any nifti images.
+  - __Default__: False
 - text_notes_private
   - __Name__: text_notes_private
   - __Type__: Boolean
   - __Description__: Text notes include private patient details. Options: true, false (default).
   - __Default__: False
```

## Comparing `fw_gear_dcm2niix-2.0.0.dist-info/RECORD` & `fw_gear_dcm2niix-2.0.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 fw_gear_dcm2niix/dcm2niix/dcm2niix_utils.py,sha256=Bi7FVy2B4qeUJr_57FAM9OjizTRYeDDuLIvzoVEDpf8,5646
 fw_gear_dcm2niix/dcm2niix/interfaces.py,sha256=f-cFwE-W9WAbvXaVptrapXmMgnpXgI0yk7J92d_hUwM,3528
 fw_gear_dcm2niix/dcm2niix/prepare.py,sha256=SXB0Hglz6Y8L0yJ1h61YBFtAZMVtht1c59Iltz3O4II,1240
 fw_gear_dcm2niix/utils/__init__.py,sha256=JqFj1MIfZbijg-OcS_ho5QzMfpHEy2G-Pn95dFTlioM,24
 fw_gear_dcm2niix/utils/metadata.py,sha256=ipjsjmZke3xubty-AT73RmaeCOEnIPTTumA-epeBE7k,15016
 fw_gear_dcm2niix/utils/parse_config.py,sha256=Q1AJcBS0rE0FouFVtfun6l627uBUPAI5EQOL2lXdBS4,7078
 fw_gear_dcm2niix/utils/resolve.py,sha256=geyQqxyA_U2LFK1pvZj-l5-g0E0WZrnOH9NBH4ywMNA,6904
-fw_gear_dcm2niix-2.0.0.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
-fw_gear_dcm2niix-2.0.0.dist-info/METADATA,sha256=RigPsXWnYwaOhTgnoS1QUizJVFmcE6U243-bUE7E-eQ,13561
-fw_gear_dcm2niix-2.0.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-fw_gear_dcm2niix-2.0.0.dist-info/RECORD,,
+fw_gear_dcm2niix-2.0.1.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
+fw_gear_dcm2niix-2.0.1.dist-info/METADATA,sha256=WP5zrLhFW1XmxANnyi0LsEuoK9DEDuRYtWwdKStWRS4,13774
+fw_gear_dcm2niix-2.0.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+fw_gear_dcm2niix-2.0.1.dist-info/RECORD,,
```

