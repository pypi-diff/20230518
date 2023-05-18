# Comparing `tmp/visionai-data-format-1.0.1.tar.gz` & `tmp/visionai-data-format-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-1.0.1.tar", last modified: Thu May 11 07:26:20 2023, max compression
+gzip compressed data, was "visionai-data-format-1.0.2.tar", last modified: Thu May 18 04:05:31 2023, max compression
```

## Comparing `visionai-data-format-1.0.1.tar` & `visionai-data-format-1.0.2.tar`

### file list

```diff
@@ -1,73 +1,39 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.974892 visionai-data-format-1.0.1/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.543804 visionai-data-format-1.0.1/.github/
--rw-r--r--   0 christian   (501) staff       (20)      472 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 christian   (501) staff       (20)      288 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.github/labels.yml
--rw-r--r--   0 christian   (501) staff       (20)       16 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.github/semantic.yml
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.545948 visionai-data-format-1.0.1/.github/workflows/
--rw-r--r--   0 christian   (501) staff       (20)      699 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.github/workflows/test.yml
--rw-r--r--   0 christian   (501) staff       (20)     3080 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.gitignore
--rw-r--r--   0 christian   (501) staff       (20)     1741 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 christian   (501) staff       (20)     1507 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/Makefile
--rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-11 07:26:19.969912 visionai-data-format-1.0.1/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)       69 2022-11-09 05:29:43.000000 visionai-data-format-1.0.1/README.md
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.564077 visionai-data-format-1.0.1/ci/
--rw-r--r--   0 christian   (501) staff       (20)      965 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/ci/.commitlint.yaml
--rw-r--r--   0 christian   (501) staff       (20)     1465 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/ci/COMMIT_MESSAGE_TEMPLATE
--rw-r--r--   0 christian   (501) staff       (20)       63 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/ci/dev.txt
--rw-r--r--   0 christian   (501) staff       (20)      312 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/ci/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)     3658 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/conftest.py
--rw-r--r--   0 christian   (501) staff       (20)       38 2023-05-11 07:26:19.991616 visionai-data-format-1.0.1/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)      577 2023-05-11 06:46:16.000000 visionai-data-format-1.0.1/setup.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.568459 visionai-data-format-1.0.1/tests/
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.603258 visionai-data-format-1.0.1/tests/test_data/
--rw-r--r--   0 christian   (501) staff       (20)     2549 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_contexts_data.json
--rw-r--r--   0 christian   (501) staff       (20)     7424 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data.json
--rw-r--r--   0 christian   (501) staff       (20)     5852 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar.json
--rw-r--r--   0 christian   (501) staff       (20)     5850 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_class.json
--rw-r--r--   0 christian   (501) staff       (20)    10870 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_objects_frame_intervals.json
--rw-r--r--   0 christian   (501) staff       (20)    10870 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_single_lidar_wrong_visionai_frame_intervals.json
--rw-r--r--   0 christian   (501) staff       (20)     5852 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_wrong_frame_properties_sensor.json
--rw-r--r--   0 christian   (501) staff       (20)      454 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_data_wrong_visionai_streams_sensor.json
--rw-r--r--   0 christian   (501) staff       (20)    26678 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation.json
--rw-r--r--   0 christian   (501) staff       (20)    25431 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation_without_tags.json
--rw-r--r--   0 christian   (501) staff       (20)    26676 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_objects_semantic_segmentation_wrong_tags_classes.json
--rw-r--r--   0 christian   (501) staff       (20)     4796 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_raw_data.json
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_visionai_classification_ontology.json
--rw-r--r--   0 christian   (501) staff       (20)     5885 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_visionai_ontology.json
--rw-r--r--   0 christian   (501) staff       (20)      454 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/fake_visionai_semantic_ontology.json
--rw-r--r--   0 christian   (501) staff       (20)     7052 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/generated_objects_data.json
--rw-r--r--   0 christian   (501) staff       (20)     4424 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_data/generated_raw_data.json
--rw-r--r--   0 christian   (501) staff       (20)     2177 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/tests/test_schemas.py
--rw-r--r--   0 christian   (501) staff       (20)     4739 2023-05-11 06:47:55.000000 visionai-data-format-1.0.1/tests/test_validators.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.619617 visionai-data-format-1.0.1/visionai_data_format/
--rw-r--r--   0 christian   (501) staff       (20)     1609 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/Readme.md
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     1400 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/bdd_to_vai.py
--rw-r--r--   0 christian   (501) staff       (20)     7697 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/coco_to_vai.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.708067 visionai-data-format-1.0.1/visionai_data_format/schemas/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-11 06:22:30.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     2142 2023-05-11 06:22:30.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-11 06:22:30.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 christian   (501) staff       (20)     1657 2023-05-11 06:46:16.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/common.py
--rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-11 07:02:55.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.754114 visionai-data-format-1.0.1/visionai_data_format/schemas/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-11 06:22:30.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)    39369 2023-05-11 06:46:16.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 christian   (501) staff       (20)    27999 2023-05-11 06:46:16.000000 visionai-data-format-1.0.1/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.915197 visionai-data-format-1.0.1/visionai_data_format/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)      495 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/calculation.py
--rw-r--r--   0 christian   (501) staff       (20)    10506 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/checker.py
--rw-r--r--   0 christian   (501) staff       (20)      761 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/classes.py
--rw-r--r--   0 christian   (501) staff       (20)      335 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/common.py
--rw-r--r--   0 christian   (501) staff       (20)     6877 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/converter.py
--rw-r--r--   0 christian   (501) staff       (20)     4059 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/resize.py
--rw-r--r--   0 christian   (501) staff       (20)     1992 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/utils/validator.py
--rw-r--r--   0 christian   (501) staff       (20)     2274 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 christian   (501) staff       (20)     6237 2023-05-11 04:50:19.000000 visionai-data-format-1.0.1/visionai_data_format/vai_to_coco.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-11 07:26:19.629978 visionai-data-format-1.0.1/visionai_data_format.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     2353 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       40 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)       21 2023-05-11 07:26:19.000000 visionai-data-format-1.0.1/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.398867 visionai-data-format-1.0.2/
+-rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-18 04:05:31.398720 visionai-data-format-1.0.2/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)       69 2023-05-12 07:07:09.000000 visionai-data-format-1.0.2/README.md
+-rw-r--r--   0 christian   (501) staff       (20)       38 2023-05-18 04:05:31.399041 visionai-data-format-1.0.2/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      577 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.386900 visionai-data-format-1.0.2/tests/
+-rw-r--r--   0 christian   (501) staff       (20)     2176 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/tests/test_schemas.py
+-rw-r--r--   0 christian   (501) staff       (20)     4731 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/tests/test_validators.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.389034 visionai-data-format-1.0.2/visionai_data_format/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     1400 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/bdd_to_vai.py
+-rw-r--r--   0 christian   (501) staff       (20)     7696 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/coco_to_vai.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.394590 visionai-data-format-1.0.2/visionai_data_format/schemas/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2551 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)     1657 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/common.py
+-rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.394933 visionai-data-format-1.0.2/visionai_data_format/schemas/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)    39355 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 christian   (501) staff       (20)    27992 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.397991 visionai-data-format-1.0.2/visionai_data_format/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)      494 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 christian   (501) staff       (20)    10506 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/checker.py
+-rw-r--r--   0 christian   (501) staff       (20)      761 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/classes.py
+-rw-r--r--   0 christian   (501) staff       (20)      335 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/common.py
+-rw-r--r--   0 christian   (501) staff       (20)     6877 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/converter.py
+-rw-r--r--   0 christian   (501) staff       (20)     4059 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/utils/resize.py
+-rw-r--r--   0 christian   (501) staff       (20)     1991 2023-05-18 02:48:45.000000 visionai-data-format-1.0.2/visionai_data_format/utils/validator.py
+-rw-r--r--   0 christian   (501) staff       (20)     2274 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 christian   (501) staff       (20)     6237 2023-05-18 02:48:43.000000 visionai-data-format-1.0.2/visionai_data_format/vai_to_coco.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-05-18 04:05:31.392839 visionai-data-format-1.0.2/visionai_data_format.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)      189 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     1122 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       40 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)       21 2023-05-18 04:05:31.000000 visionai-data-format-1.0.2/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-1.0.1/setup.py` & `visionai-data-format-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.0.1"
+PACKAGE_VERSION = "1.0.2"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai-data-format-1.0.1/tests/test_schemas.py` & `visionai-data-format-1.0.2/tests/test_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 
 def test_visionai(
     fake_raw_visionai_data,
     fake_generated_raw_visionai_data,
     fake_objects_visionai_data,
     fake_generated_objects_visionai_data,
 ):
-
     assert (
         VisionAIModel(**fake_raw_visionai_data).dict(exclude_unset=True)
         == fake_generated_raw_visionai_data
     )
 
     assert (
         VisionAIModel(**fake_objects_visionai_data).dict(exclude_unset=True)
```

### Comparing `visionai-data-format-1.0.1/tests/test_validators.py` & `visionai-data-format-1.0.2/tests/test_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,114 +1,106 @@
 import pytest
 
 from visionai_data_format.schemas.ontology import Ontology
 from visionai_data_format.schemas.visionai_schema import VisionAIModel
 
 
 def test_validate_bbox(fake_visionai_ontology, fake_objects_data_single_lidar):
-
     ontology = Ontology(**fake_visionai_ontology).dict(exclude_unset=True)
 
     errors = VisionAIModel(**fake_objects_data_single_lidar).validate_with_ontology(
         ontology=ontology,
     )
 
     assert errors == []
 
 
 def test_validate_bbox_wrong_frame_properties_sensor_name(
     fake_visionai_ontology, fake_objects_data_wrong_frame_properties_sensor
 ):
-
     ontology = Ontology(**fake_visionai_ontology).dict(exclude_unset=True)
 
     errors = VisionAIModel(
         **fake_objects_data_wrong_frame_properties_sensor
     ).validate_with_ontology(
         ontology=ontology,
     )
 
     assert errors == ["Frame properties contains extra sensor(s) : {'camera2'}"]
 
 
 def test_validate_bbox_wrong_streams_under_visionai(
     fake_visionai_ontology, fake_objects_data_wrong_frame_properties_sensor
 ):
-
     ontology = Ontology(**fake_visionai_ontology).dict(exclude_unset=True)
 
     errors = VisionAIModel(
         **fake_objects_data_wrong_frame_properties_sensor
     ).validate_with_ontology(
         ontology=ontology,
     )
 
     assert errors == ["Frame properties contains extra sensor(s) : {'camera2'}"]
 
 
 def test_validate_bbox_wrong_class_under_visionai(
     fake_visionai_ontology, fake_objects_data_single_lidar_wrong_class
 ):
-
     ontology = Ontology(**fake_visionai_ontology).dict(exclude_unset=True)
 
     errors = VisionAIModel(
         **fake_objects_data_single_lidar_wrong_class
     ).validate_with_ontology(
         ontology=ontology,
     )
 
     assert errors == ["Attribute objects with classes {'children'} doesn't accepted"]
 
 
 def test_validate_semantic_segmentation(
     fake_visionai_semantic_ontology, fake_objects_semantic_segmentation
 ):
-
     ontology = Ontology(**fake_visionai_semantic_ontology).dict(exclude_unset=True)
 
     errors = VisionAIModel(**fake_objects_semantic_segmentation).validate_with_ontology(
         ontology=ontology,
     )
 
     assert errors == []
 
 
 def test_validate_semantic_segmentation_visionai_without_tags(
     fake_visionai_semantic_ontology, fake_objects_semantic_segmentation_without_tags
 ):
-
     ontology = Ontology(**fake_visionai_semantic_ontology).dict(exclude_unset=True)
     with pytest.raises(Exception):
         errors = VisionAIModel(
             **fake_objects_semantic_segmentation_without_tags
         ).validate_with_ontology(
             ontology=ontology,
         )
         assert errors == []
 
 
 def test_validate_semantic_segmentation_visionai_wrong_tags_classes(
     fake_visionai_semantic_ontology,
     fake_objects_semantic_segmentation_wrong_tags_classes,
 ):
-
     ontology = Ontology(**fake_visionai_semantic_ontology).dict(exclude_unset=True)
     errors = VisionAIModel(
         **fake_objects_semantic_segmentation_wrong_tags_classes
     ).validate_with_ontology(
         ontology=ontology,
     )
     assert errors == ["Tag label with classes {'road'} doesn't accepted"]
 
 
 def test_validate_classification(
     fake_visionai_classification_ontology, fake_contexts_data
 ):
-
     ontology = Ontology(**fake_visionai_classification_ontology).dict(
         exclude_unset=True
     )
     errors = VisionAIModel(**fake_contexts_data).validate_with_ontology(
         ontology=ontology,
     )
     assert errors == []
```

### Comparing `visionai-data-format-1.0.1/visionai_data_format/bdd_to_vai.py` & `visionai-data-format-1.0.2/visionai_data_format/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/coco_to_vai.py` & `visionai-data-format-1.0.2/visionai_data_format/coco_to_vai.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,14 @@
             uri=uri,
             type=StreamType.camera,
             description="Frontal camera",
         )
     }
     # to vision_ai:
     for image_name, frame_obj in frames.items():
-
         objects_per_image = {
             object_id: objects[object_id] for object_id in frame_obj.objects
         }
 
         new_image_name = f"{int(image_name):012d}"
         vision_ai_data_dict[new_image_name] = VisionAIModel(
             visionai=VisionAI(
```

### Comparing `visionai-data-format-1.0.1/visionai_data_format/schemas/coco_schema.py` & `visionai-data-format-1.0.2/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/schemas/common.py` & `visionai-data-format-1.0.2/visionai_data_format/schemas/common.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/schemas/ontology.py` & `visionai-data-format-1.0.2/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/schemas/utils/validators.py` & `visionai-data-format-1.0.2/visionai_data_format/schemas/utils/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 
 def validate_classes(
     visionai: Dict,
     root_key: str,
     sub_root_key: str,
     ontology_classes: Set[str],
 ) -> Tuple[Set[str], Dict[str, Dict[str, Set]]]:
-
     if not visionai:
         return set()
 
     classes_attributes_map: Dict[str, Dict[str, Set]] = parse_visionai_child_type(
         child_data=visionai.get(root_key, {}),
         data_key=sub_root_key,
     )
@@ -158,28 +157,26 @@
     if extra_classes:
         return (f"Tag label with classes {extra_classes} doesn't accepted", -1)
 
     return ("", len(classes_set))
 
 
 def validate_tags(visionai: Dict, tags: Dict, *args, **kwargs) -> Tuple[str, int]:
-
     ontology_classes: Set[str] = set(tags.keys())
 
     return validate_tags_classes(
         tags=visionai["tags"], ontology_classes=ontology_classes
     )
 
 
 def validate_attributes(
     classes_attributes_map: Dict[str, Dict[str, Set]],
     attributes: Dict,
     excluded_attributes: Optional[Set] = None,
 ) -> Tuple[bool, Optional[Tuple]]:
-
     for label_class, label_attrs_data in classes_attributes_map.items():
         # already valid the class in previous step
         ontology_attr_name_type_dict: Dict[str, Set] = attributes.get(label_class, {})
         ontology_attr_name_type_set: Set[str] = set(ontology_attr_name_type_dict.keys())
         label_name_type_set: Set[str] = set(label_attrs_data.keys())
 
         extra_attr = label_name_type_set - ontology_attr_name_type_set
@@ -219,15 +216,14 @@
     data_root_key: str,
     data_child_key: str,
     frames: Dict,
     has_lidar_sensor: bool,
     has_multi_sensor: bool,
     sensor_name_set: Set[str],
 ) -> Optional[str]:
-
     for frame_obj in frames.values():
         cur_obj_data_type = set()
         cur_obj_stream_sensor = set()
         cur_obj_coor_sensor = set()
         obj_data_dict = frame_obj.get(data_root_key)
         if not obj_data_dict:
             continue
@@ -325,15 +321,14 @@
         )
     return classes_attributes_map
 
 
 def parse_data_pointers(
     data_under_vai: Dict, pointer_type: str
 ) -> Tuple[Dict[Tuple[str, str], Dict], Dict[str, Dict]]:
-
     """mapping data pointers under visionai with
     object uuid and its name as key
 
     Parameters
     ----------
     data_under_vai : Dict
         data under visionai, such as `objects` or `contexts` data
@@ -349,15 +344,14 @@
     """
 
     if not data_under_vai:
         return {}, {}
     data_pointers: Dict[Tuple[str, str], Dict] = defaultdict(dict)
     data_obj_under_vai_intervals: Dict[str, List] = defaultdict(list)
     for uuid, data in data_under_vai.items():
-
         for attr_name, attr_ptr_data in data[pointer_type].items():
             data_pointers[(uuid, attr_name)] = {
                 "type": attr_ptr_data["type"],
                 "frame_intervals": attr_ptr_data["frame_intervals"],
             }
         data_obj_under_vai_intervals[uuid] = []
         for interval in data["frame_intervals"]:
@@ -544,15 +538,14 @@
 
 
 def vai_data_data_pointers_intervals(
     root_key: str,
     data_pointers: Dict[Tuple[str, str], Dict],
     data_obj_under_vai_intervals: Dict[str, List],
 ) -> Tuple[bool, Union[Dict[Tuple[str, str], List[Tuple[int, int]]], str]]:
-
     """validate intervals between data pointer and its object frame intervals
 
     Parameters
     ----------
     root_key : str
         visionai object key, such as `contexts` or `objects`
     data_pointers : Dict[tuple[str, str], dict]
@@ -699,15 +692,14 @@
     Tuple[bool,str]
         return a tuple of boolean status and its error message
     """
 
     msg: str = ""
     for frame_data in dynamic_attrs.values():
         for frame_num, attr_info in frame_data.items():
-
             if attr_info["type"] != "binary":
                 continue
             mask_rle: str = attr_info["val"]
 
             # retrieve classes from #pixelnumVclass
             # TODO: move this to visionai-data-format
             pixel_list: List[str] = [data for data in mask_rle.split("#") if data]
@@ -745,15 +737,14 @@
     data_under_vai: Dict,
     frames: Dict[str, Dict],
     root_key: str = "contexts",
     sub_root_key: str = "context_data",
     pointer_type: str = "context_data_pointers",
     tags_count: int = -1,
 ) -> Tuple[bool, str]:
-
     parsed_data_pointers: Tuple[
         Dict[Tuple[str, str], Dict], Dict[str, List]
     ] = parse_data_pointers(
         data_under_vai,
         pointer_type,
     )
     data_pointers, data_obj_under_vai_intervals = parsed_data_pointers
@@ -787,15 +778,14 @@
     data_pointers_keys: Set[Tuple[str, str]] = (
         set() if not data_pointers else set(data_pointers.keys())
     )
 
     # validate if combinations of static and dynamic equals to data pointers
     combination_attrs = static_attrs_keys | dynamic_attrs_keys
     if combination_attrs ^ data_pointers_keys:
-
         extra_attributes_name: Set[str] = combination_attrs - data_pointers_keys
         missing_attributes_name: Set[str] = data_pointers_keys - combination_attrs
         msg = ""
         if extra_attributes_name:
             msg += f"Extra attributes from data pointers : {extra_attributes_name} \n"
 
         if missing_attributes_name:
@@ -863,15 +853,14 @@
     has_lidar_sensor: bool,
     has_multi_sensor: bool,
     ontology_attributes_map: Optional[Dict[str, Dict[str, Set]]] = None,
     tags_count: int = -1,
     *args,
     **kwargs,
 ) -> Optional[str]:
-
     if not ontology_attributes_map:
         ontology_attributes_map = {}
     ontology_classes = set(ontology_data.keys())
     visionai_frames = visionai.get("frames", {})
     visionai_objects = visionai.get(root_key, {})
     extra_classes, classes_attributes_map = validate_classes(
         visionai=visionai,
@@ -1010,15 +999,14 @@
             return False
     return True
 
 
 def validate_coor_system_obj(
     coord_systems_data: Dict[str, Dict], ontology_sensors_name_set: Set[str]
 ) -> str:
-
     if not coord_systems_data:
         return False
     data_sensors = {
         sensor_name
         for sensor_name, sensor_info in coord_systems_data.items()
         if sensor_info["type"] != "local_cs"
     }
@@ -1032,15 +1020,14 @@
     visionai: Dict,
     sensor_info: Dict[str, str],
     has_multi_sensor: bool,
     has_lidar_sensor: bool,
     *args,
     **kwargs,
 ) -> Tuple[str, Dict[str, str]]:
-
     if not visionai.get("streams"):
         return ("VisionAI missing streams data", {})
 
     # verify the streams based on sensors
     streams_data = visionai.get("streams")
     if not validate_streams_obj(
         streams_data=streams_data,
@@ -1091,15 +1078,14 @@
 
     attribute_data_name_type_set = {
         (attr_name, attr_info["type"])
         for attr_name, attr_info in attribute_data.items()
     }
 
     for data_uuid, data_info in data_under_vai.items():
-
         data_pointer = data_info.get(pointer_type)
         if not data_pointer:
             return False, f"UUID {data_uuid} doesn't contains data key {pointer_type}"
 
         data_pointer_name_set = set(data_pointer.keys())
 
         extras = data_pointer_name_set - attribute_data_name_set
```

### Comparing `visionai-data-format-1.0.1/visionai_data_format/schemas/visionai_schema.py` & `visionai-data-format-1.0.2/visionai_data_format/schemas/visionai_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
 
     schema_version: SchemaVersion = Field(
         description="Version number of the VisionAI schema this annotation JSON object follows.",
     )
 
 
 class StaticBoolean(ExcludedNoneBaseModel):
-
     attributes: Optional[Attributes] = None
     name: StrictStr = Field(
         ...,
         description="This is a string encoding the name of this object data."
         + " It is used as index inside the corresponding object data pointers.",
     )
     type: Optional[Type] = Field(
@@ -304,15 +303,14 @@
         None,
         description="The confidence score of model prediction of this object."
         + " Ground truth does not have this attribute.",
     )
 
 
 class BaseStaticElementData(ExcludedNoneBaseModel):
-
     boolean: Optional[List[StaticBoolean]] = Field(
         None, description='List of "boolean" that describe this object.'
     )
     num: Optional[List[StaticNum]] = Field(
         None, description='List of "number" that describe this object.'
     )
     text: Optional[List[StaticText]] = Field(
@@ -320,15 +318,14 @@
     )
     vec: Optional[List[StaticVec]] = Field(
         None, description='List of "vec" that describe this object.'
     )
 
 
 class BaseDynamicElementData(ExcludedNoneBaseModel):
-
     boolean: Optional[List[DynamicBoolean]] = Field(
         None, description='List of "boolean" that describe this object.'
     )
     num: Optional[List[DynamicNum]] = Field(
         None, description='List of "number" that describe this object.'
     )
     text: Optional[List[DynamicText]] = Field(
@@ -336,15 +333,14 @@
     )
     vec: Optional[List[DynamicVec]] = Field(
         None, description='List of "vec" that describe this object.'
     )
 
 
 class ElementDataPointer(ExcludedNoneBaseModel):
-
     attributes: Optional[Dict[StrictStr, AttributeType]] = Field(
         None,
         description="This is a JSON object which contains pointers to the attributes of"
         + ' the element data pointed by this pointer. The attributes pointer keys shall be the "name" of the'
         + " attribute of the element data this pointer points to.",
     )
     frame_intervals: Optional[List[FrameInterval]] = Field(
@@ -613,15 +609,14 @@
         descriptions="A relative or absolute time reference that specifies "
         + "the time instant this frame corresponds to",
     )
     streams: Dict[StrictStr, FramePropertyStream]
 
 
 class ObjectDataElement(ExcludedNoneBaseModel):
-
     attributes: Optional[Attributes] = None
     name: StrictStr = Field(
         description="This is a string encoding the name of this object data."
         + " It is used as index inside the corresponding object data pointers.",
     )
     stream: StrictStr = Field(
         description="Name of the stream in respect of which this object data is expressed.",
@@ -832,27 +827,25 @@
         default=None,
         description="This is the JSON object of tags. Object keys are strings."
         + " Values are dictionary containing information of current sequence.",
     )
 
     @validator("tags")
     def validate_tags(cls, value):
-
         assert value, f" Value {value} is not allowed"
         return value
 
 
 class VisionAIModel(ExcludedNoneBaseModel):
     class Config:
         extra = Extra.forbid
 
     visionai: VisionAI
 
     def validate_with_ontology(self, ontology: Type[Ontology]) -> List[str]:
-
         validator_map = {
             "contexts": validate_contexts,
             "objects": validate_objects,
         }
 
         errors: List[str] = []
```

### Comparing `visionai-data-format-1.0.1/visionai_data_format/utils/checker.py` & `visionai-data-format-1.0.2/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/utils/classes.py` & `visionai-data-format-1.0.2/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/utils/converter.py` & `visionai-data-format-1.0.2/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/utils/resize.py` & `visionai-data-format-1.0.2/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/utils/validator.py` & `visionai-data-format-1.0.2/visionai_data_format/utils/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         logger.error("[validate_bdd] Validation failed : " + str(e))
         return None
 
 
 def attribute_generator(
     category: str, attribute: Dict, ontology_class_attrs: Dict
 ) -> Dict:
-
     if not attribute:
         return dict()
 
     new_attribute = dict()
     category = category.upper()
     for attr_name, attr_value in attribute.items():
         logger.info(f"attr_name : {attr_name}")
```

### Comparing `visionai-data-format-1.0.1/visionai_data_format/vai_to_bdd.py` & `visionai-data-format-1.0.2/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.1/visionai_data_format/vai_to_coco.py` & `visionai-data-format-1.0.2/visionai_data_format/vai_to_coco.py`

 * *Files identical despite different names*

