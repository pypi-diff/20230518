# Comparing `tmp/bidsschematools-0.5.1.tar.gz` & `tmp/bidsschematools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bidsschematools-0.5.1.tar", last modified: Wed Sep 21 21:05:01 2022, max compression
+gzip compressed data, was "bidsschematools-0.6.0.tar", last modified: Sat Oct 29 13:01:11 2022, max compression
```

## Comparing `bidsschematools-0.5.1.tar` & `bidsschematools-0.6.0.tar`

### file list

```diff
@@ -1,429 +1,446 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.064840 bidsschematools-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-09-21 21:05:01.064840 bidsschematools-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/data/schema/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/BIDS_VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/SCHEMA_VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/data/schema/meta/
--rw-r--r--   0 runner    (1001) docker     (121)     8697 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/meta/context.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.036840 bidsschematools-0.5.1/bidsschematools/data/schema/objects/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/associated_data.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    18513 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/columns.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8091 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/common_principles.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/datatypes.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16592 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/entities.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    11132 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/formats.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   111890 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/modalities.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    27795 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/suffixes.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/objects/top_level_files.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.036840 bidsschematools-0.5.1/bidsschematools/data/schema/rules/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/associated_data.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.036840 bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/
--rw-r--r--   0 runner    (1001) docker     (121)    12116 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/asl.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/dwi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/events.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/fmap.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/func.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/hints.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/mri.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/common_derivatives_validation.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/common_principles.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/dataset_metadata.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.036840 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/anat.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/beh.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.036840 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/derivatives/
--rw-r--r--   0 runner    (1001) docker     (121)     9804 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/derivatives/common_derivatives.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/derivatives/common_imaging_derivatives.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/dwi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/eeg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/fmap.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/func.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/ieeg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/meg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/micr.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/perf.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/pet.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/entities.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6378 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/errors.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/modalities.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/anat.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6566 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/asl.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/beh.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/continuous.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/derivatives/
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/dwi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/eeg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/entity_rules.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/events.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/fmap.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/func.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/ieeg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8049 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/meg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/micr.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    10024 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/mri.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8075 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/pet.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/derivatives/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/derivatives/common_derivatives.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/eeg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/ieeg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/meg.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/perf.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/pet.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/physio.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/task.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/data/schema/rules/top_level_files.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    40078 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/render.py
--rw-r--r--   0 runner    (1001) docker     (121)     8897 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/tests/data/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-09-21 21:04:51.000000 bidsschematools-0.5.1/bidsschematools/tests/data/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/README
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.024840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.040840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.044840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
--rw-r--r--   0 runner    (1001) docker     (121)   411101 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   411101 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_headshape.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.044840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/README
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/participants.json
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/participants.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.024840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.024840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.044840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/
--rwxr-xr-x   0 runner    (1001) docker     (121)   118231 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii
--rwxr-xr-x   0 runner    (1001) docker     (121)     1190 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-02_ses-01_T1w.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.044840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1941 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.json
--rw-r--r--   0 runner    (1001) docker     (121)    84350 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz
--rwxr-xr-x   0 runner    (1001) docker     (121)      413 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.json
--rw-r--r--   0 runner    (1001) docker     (121)    15131 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.tsv
--rwxr-xr-x   0 runner    (1001) docker     (121)     1061 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-09-21 21:04:53.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.044840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    22820 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.044840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/README
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.028840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.044840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.044840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
--rw-r--r--   0 runner    (1001) docker     (121)   411101 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/bidsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/README
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/participants.json
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/participants.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/sub-cbm001_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/sub-cbm002_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/sub-cbm003_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/sub-cbm004_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/sub-cbm005_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/sub-cbm006_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/sub-cbm007_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/sub-cbm008_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/sub-cbm009_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.048840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/sub-cbm010_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/sub-cbm011_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/sub-cbm012_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/sub-cbm013_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/sub-cbm014_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/sub-cbm015_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/sub-cbm016_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/sub-cbm017_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.052840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/sub-cbm018_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/sub-cbm019_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_channels.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_eeg.edf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_eeg.json
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_events.tsv
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/sub-cbm020_scans.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.028840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T1w.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T1w.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T2w.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T2w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_magnitude1.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_magnitude2.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_phasediff.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_phasediff.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/README
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.json
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.tsv
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/samples.json
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/samples.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.028840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SEM.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SEM.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/0/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/sub-01_ses-02_sample-A_SEM.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/sub-01_ses-02_sample-A_SEM.png
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/sub-01_sessions.json
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/sub-01_sessions.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.056840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/README
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/participants.json
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/participants.tsv
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/samples.json
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/samples.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_photo.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_photo.png
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.json
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.ome.tif
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.json
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.ome.tif
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.json
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.ome.tif
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.json
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.ome.tif
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_photo.json
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_photo.png
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.json
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.ome.tif
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.json
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.ome.tif
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.json
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.ome.tif
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.json
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.ome.tif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/
--rwxr-xr-x   0 runner    (1001) docker     (121)      390 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/README
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/participants.json
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/participants.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/anat/
--rwxr-xr-x   0 runner    (1001) docker     (121)        1 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1804 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.json
--rwxr-xr-x   0 runner    (1001) docker     (121)   112710 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz
--rwxr-xr-x   0 runner    (1001) docker     (121)      774 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json
--rwxr-xr-x   0 runner    (1001) docker     (121)      771 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/README
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-anat_TB1TFL.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-anat_TB1TFL.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-famp_TB1TFL.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-famp_TB1TFL.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/README
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/README
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.060840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.064840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.064840 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-09-21 21:04:52.000000 bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/data/broken_dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/data/expected_bids_validator_xs_write.log
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/test_make_testdata.py
--rw-r--r--   0 runner    (1001) docker     (121)     9536 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)    10581 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14685 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/tests/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10563 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    33770 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/bidsschematools/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:05:01.032840 bidsschematools-0.5.1/bidsschematools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-09-21 21:05:00.000000 bidsschematools-0.5.1/bidsschematools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    25245 2022-09-21 21:05:01.000000 bidsschematools-0.5.1/bidsschematools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:05:00.000000 bidsschematools-0.5.1/bidsschematools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-21 21:05:00.000000 bidsschematools-0.5.1/bidsschematools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:05:00.000000 bidsschematools-0.5.1/bidsschematools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-21 21:05:00.000000 bidsschematools-0.5.1/bidsschematools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-21 21:05:00.000000 bidsschematools-0.5.1/bidsschematools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-09-21 21:04:31.000000 bidsschematools-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-09-21 21:05:01.064840 bidsschematools-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.778874 bidsschematools-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-10-29 13:01:11.778874 bidsschematools-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/data/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/BIDS_VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/SCHEMA_VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.742873 bidsschematools-0.6.0/bidsschematools/data/schema/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)     9280 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/meta/context.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/meta/expression_tests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.742873 bidsschematools-0.6.0/bidsschematools/data/schema/objects/
+-rw-r--r--   0 runner    (1001) docker     (121)    24034 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/columns.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8140 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/common_principles.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/datatypes.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16624 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    11348 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/files.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4897 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/formats.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   116632 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/modalities.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    28142 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/objects/suffixes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.742873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.742873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/
+-rw-r--r--   0 runner    (1001) docker     (121)    12116 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/asl.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/common_derivatives.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/dwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/fmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/func.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/hints.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/mri.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/nirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/common_principles.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/dataset_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6378 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/errors.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.730872 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.742873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/common/core.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/common/tables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.742873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/deriv/
+-rw-r--r--   0 runner    (1001) docker     (121)     4654 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/deriv/imaging.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5277 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/deriv/preprocessed_data.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.746873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/
+-rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/anat.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/beh.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/channels.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/dwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/eeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/fmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/func.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/ieeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/meg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/micr.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/nirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/perf.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/pet.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/photo.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/task.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/modalities.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.746873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/anat.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6566 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/asl.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/beh.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/continuous.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.746873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (121)     2799 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/dwi.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/eeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/entity_rules.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/fmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3514 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/func.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/ieeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8049 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/meg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/micr.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10024 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/mri.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5060 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/nirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8927 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/pet.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.746873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.746873 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/derivatives/common_derivatives.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/eeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/ieeg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/meg.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/modality_agnostic.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/nirs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/perf.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/pet.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/physio.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/task.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.750873 bidsschematools-0.6.0/bidsschematools/render/
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21614 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/render/tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17628 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/render/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11403 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/render/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6025 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.750873 bidsschematools-0.6.0/bidsschematools/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.750873 bidsschematools-0.6.0/bidsschematools/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.750873 bidsschematools-0.6.0/bidsschematools/tests/data/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-29 13:01:00.000000 bidsschematools-0.6.0/bidsschematools/tests/data/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.750873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-10-29 13:01:02.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-10-29 13:01:02.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.750873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/README
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.734872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.750873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.754873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)   411101 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   411101 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_headshape.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.754873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/README
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/participants.json
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.734872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.734872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.754873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/
+-rwxr-xr-x   0 runner    (1001) docker     (121)   118231 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1190 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-02_ses-01_T1w.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.754873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1941 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.json
+-rw-r--r--   0 runner    (1001) docker     (121)    84350 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz
+-rwxr-xr-x   0 runner    (1001) docker     (121)      413 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.json
+-rw-r--r--   0 runner    (1001) docker     (121)    15131 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.tsv
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1061 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-10-29 13:01:03.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.754873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    22817 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.754873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/README
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.734872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.754873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/anat/sub-Sub1_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.754873 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_aslcontext.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)   411101 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/bidsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/README
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/participants.json
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/sub-cbm001_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/sub-cbm002_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/sub-cbm003_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/sub-cbm004_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/sub-cbm005_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/sub-cbm006_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.758874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/sub-cbm007_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/sub-cbm008_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/sub-cbm009_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/sub-cbm010_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/sub-cbm011_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)      876 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/sub-cbm012_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/sub-cbm013_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.762874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/sub-cbm014_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/sub-cbm015_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/sub-cbm016_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/sub-cbm017_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/sub-cbm018_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/sub-cbm019_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/
+-rw-r--r--   0 runner    (1001) docker     (121)     1990 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_channels.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_eeg.edf
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_eeg.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/sub-cbm020_scans.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.766874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T1w.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T1w.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T2w.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/anat/sub-100307_T2w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.770874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_magnitude1.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_magnitude2.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_phasediff.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/hcp_example_bids/sub-100307/fmap/sub-100307_acq-forT1w_phasediff.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.770874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/README
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.json
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/samples.json
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/samples.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.770874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.770874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SEM.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SEM.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.770874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/0/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-01/micr/sub-01_ses-01_sample-A_SPIM.ome.zarr/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.770874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/sub-01_ses-02_sample-A_SEM.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/ses-02/micr/sub-01_ses-02_sample-A_SEM.png
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/sub-01_sessions.json
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/sub-01/sub-01_sessions.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.770874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/README
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/participants.json
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/participants.tsv
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/samples.json
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/samples.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_photo.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_photo.png
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_photo.json
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_photo.png
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.ome.tif
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.ome.tif
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      390 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/README
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/participants.json
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/anat/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1804 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)   112710 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz
+-rwxr-xr-x   0 runner    (1001) docker     (121)      774 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)      771 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/README
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-anat_TB1TFL.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-anat_TB1TFL.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-famp_TB1TFL.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_tb1tfl/sub-01/fmap/sub-01_acq-famp_TB1TFL.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/README
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/README
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.774874 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2022-10-29 13:01:01.000000 bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/data/broken_dataset_description.json
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/data/expected_bids_validator_xs_write.log
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/test_make_testdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5353 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/test_render_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4838 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/test_render_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/test_render_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4943 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10543 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10107 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.778874 bidsschematools-0.6.0/bidsschematools/types/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7288 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/types/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28424 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/bidsschematools/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 13:01:11.738872 bidsschematools-0.6.0/bidsschematools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-10-29 13:01:11.000000 bidsschematools-0.6.0/bidsschematools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    25821 2022-10-29 13:01:11.000000 bidsschematools-0.6.0/bidsschematools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:11.000000 bidsschematools-0.6.0/bidsschematools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-29 13:01:11.000000 bidsschematools-0.6.0/bidsschematools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 13:01:11.000000 bidsschematools-0.6.0/bidsschematools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-29 13:01:11.000000 bidsschematools-0.6.0/bidsschematools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-29 13:01:11.000000 bidsschematools-0.6.0/bidsschematools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-10-29 13:00:39.000000 bidsschematools-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-10-29 13:01:11.778874 bidsschematools-0.6.0/setup.cfg
```

### Comparing `bidsschematools-0.5.1/LICENSE` & `bidsschematools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/PKG-INFO` & `bidsschematools-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bidsschematools
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python tools for working with the BIDS schema.
 Home-page: https://github.com/bids-standard/bids-specification
 Author: bids-standard developers
 Author-email: bids.maintenance@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bidsschematools-0.5.1/bidsschematools/__main__.py` & `bidsschematools-0.6.0/bidsschematools/__main__.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/meta/context.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/meta/context.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -183,15 +183,33 @@
           properties:
             path:
               description: 'Path to associated bvec file'
               type: string
             n_cols:
               description: 'Number of columns in bvec file'
               type: integer
-
+        channels:
+          description: 'Channels file'
+          type: object
+          properties:
+            path:
+              description: 'Path to associated channels file'
+              type: string
+            type:
+              description: 'Contents of the type column'
+              type: array
+              items:
+                type: string
+        coordsystem:
+          description: 'Coordinate system file'
+          type: object
+          properties:
+            path:
+              description: 'Path to associated coordsystem file'
+              type: string
     # The following properties are populated if the current file is of an appropriate type
     columns:
       description: 'TSV columns, indexed by column header, values are arrays with column contents'
       type: object
       additionalProperties:
         type: array
     json:
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/columns.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/columns.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -48,28 +48,52 @@
 color:
   name: color
   display_name: Color label
   description: |
     Hexadecimal. Label color for visualization.
   type: string
   unit: hexadecimal
+detector__channels:
+  name: detector
+  display_name: Detector Name
+  description: |
+    Name of the detector as specified in the `*_optodes.tsv` file.
+    `n/a` for channels that do not contain NIRS signals (for example, acceleration).
+  anyOf:
+    - type: string
+    - type: string
+      enum:
+        - n/a
+detector_type:
+  name: detector_type
+  display_name: Detector Type
+  description: |
+    The type of detector. Only to be used if the field `DetectorType` in `*_nirs.json` is set to `mixed`.
+  anyOf:
+    - type: string
 derived_from:
   name: derived_from
   display_name: Derived from
   description: |
     `sample-<label>` entity from which a sample is derived,
     for example a slice of tissue (`sample-02`) derived from a block of tissue (`sample-01`).
   type: string
   pattern: ^sample-[0-9a-zA-Z]+$
 description:
   name: description
   display_name: Description
   description: |
     Brief free-text description of the channel, or other information of interest.
   type: string
+description__optode:
+  name: description
+  display_name: Description
+  description: |
+    Free-form text description of the optode, or other information of interest.
+  type: string
 dimension:
   name: dimension
   display_name: Dimension
   description: |
     Size of the group (grid/strip/probe) that this electrode belongs to.
     Must be of form `[AxB]` with the smallest dimension first (for example, `[1x8]`).
   type: string
@@ -236,14 +260,20 @@
 # name column for electrodes.tsv files
 name__electrodes:
   name: name
   display_name: Electrode name
   description: |
     Name of the electrode contact point.
   type: string
+name__optodes:
+  name: name
+  display_name: Optode name
+  description: |
+    Name of the optode, must be unique.
+  type: string
 # name column for dseg.tsv files
 name__segmentations:
   name: name
   display_name: Label name
   description: |
     The unique label name.
   type: string
@@ -274,14 +304,24 @@
 
     If any data points have been discarded before forming the data file
     (for example, "dummy volumes" in BOLD fMRI),
     a time of 0 corresponds to the first stored data point and not the first
     acquired data point.
   type: number
   unit: s
+orientation_component:
+  name: orientation_component
+  display_name: Orientation Component
+  description: |
+    Description of the orientation of the channel.
+  type: string
+  enum:
+    - x
+    - y
+    - z
 pathology:
   name: pathology
   display_name: Pathology
   description: |
     String value describing the pathology of the sample or type of control.
     When different from `healthy`, pathology SHOULD be specified.
     The pathology may be specified in either `samples.tsv` or
@@ -416,14 +456,22 @@
     - Female
     - other
     - o
     - O
     - OTHER
     - Other
     - n/a
+short_channel:
+  name: short_channel
+  display_name: Short Channel
+  description: |
+    Is the channel designated as short.
+    The total number of channels listed as short channels
+    SHOULD be stored in `ShortChannelCount` in `*_nirs.json`.
+  type: boolean
 size:
   name: size
   display_name: Electrode size
   description: |
     Surface area of the electrode, units MUST be in `mm^2`.
   type: number
   unit: 'mm^2'
@@ -436,14 +484,32 @@
     Note that parameters should be defined in the general MEG sidecar .json file.
     Indicate `n/a` in the absence of software filters applied.
   anyOf:
     - type: string
     - type: string
       enum:
         - n/a
+source__channels:
+  name: source
+  display_name: Source name
+  description: |
+    Name of the source as specified in the `*_optodes.tsv` file.
+    `n/a` for channels that do not contain fNIRS signals (for example, acceleration).
+  anyOf:
+    - type: string
+    - type: string
+      enum:
+        - n/a
+source__optodes:
+  name: source_type
+  display_name: Source type
+  description: |
+    The type of source. Only to be used if the field `SourceType` in `*_nirs.json` is set to `mixed`.
+  anyOf:
+    - type: string
 species:
   name: species
   display_name: Species
   description: |
     The `species` column SHOULD be a binomial species name from the
     [NCBI Taxonomy](https://www.ncbi.nlm.nih.gov/Taxonomy/Browser/wwwtax.cgi)
     (for example, `homo sapiens`, `mus musculus`, `rattus norvegicus`).
@@ -610,30 +676,97 @@
     - PUPIL
     - MISC
     - SYSCLOCK
     - ADC
     - DAC
     - REF
     - OTHER
+type__nirs_channels:
+  name: type
+  display_name: Channel type
+  description: |
+    Type of channel; MUST use the channel types listed below.
+    Note that the type MUST be in upper-case.
+  type: string
+  enum:
+    - NIRSCWAMPLITUDE
+    - NIRSCWFLUORESCENSEAMPLITUDE
+    - NIRSCWOPTICALDENSITY
+    - NIRSCWHBO
+    - NIRSCWHBR
+    - NIRSCWMUA
+    - MEGMAG
+    - MEGGRADAXIAL
+    - MEGGRADPLANAR
+    - MEGREFMAG
+    - MEGREFGRADAXIAL
+    - MEGREFGRADPLANAR
+    - MEGOTHER
+    - EEG
+    - ECOG
+    - SEEG
+    - DBS
+    - VEOG
+    - HEOG
+    - EOG
+    - ECG
+    - EMG
+    - TRIG
+    - AUDIO
+    - PD
+    - EYEGAZE
+    - PUPIL
+    - MISC
+    - SYSCLOCK
+    - ADC
+    - DAC
+    - HLU
+    - FITERR
+    - ACCEL
+    - GYRO
+    - MAGN
+    - MISC
+    - OTHER
 # type column for electrodes.tsv files
 type__electrodes:
   name: type
   display_name: Electrode type
   description: |
     Type of the electrode (for example, cup, ring, clip-on, wire, needle).
   type: string
+type__optodes:
+  name: type
+  display_name: Type
+  description: |
+    The type of the optode.
+  type: string
+  enum:
+    - source
+    - detector
+    - n/a
 units:
   name: units
   display_name: Units
   description: |
     Physical unit of the value represented in this channel,
     for example, `V` for Volt, or `fT/cm` for femto Tesla per centimeter
     (see [Units](SPEC_ROOT/02-common-principles.md#units)).
   type: string
   format: unit
+units__nirs:
+  name: units
+  display_name: Units
+  description: |
+    Physical unit of the value represented in this channel,
+    specified according to the SI unit symbol and possibly prefix symbol,
+    or as a derived SI unit (for example, `V`, or unitless for changes in optical densities).
+    For guidelines about units see the [Appendix](SPEC_ROOT/appendices/units.md)
+    and [Common Principles](SPEC_ROOT/02-common-principles.md#units) pages.
+  type: string
+  format: unit
 value:
   name: value
   display_name: Marker value
   description: |
     Marker value associated with the event (for example, the value of a TTL
     trigger that was recorded at the onset of the event).
   anyOf:
@@ -648,14 +781,42 @@
   type: string
   enum:
     - control
     - label
     - m0scan
     - deltam
     - cbf
+wavelength_nominal:
+  name: wavelength_nominal
+  display_name: Wavelength nominal
+  description: |
+    Specified wavelength of light in nm.
+    `n/a` for channels that do not contain raw NIRS signals (for example, acceleration).
+    This field is equivalent to `/nirs(i)/probe/wavelengths` in the SNIRF specification.
+  anyOf:
+    - type: number
+    - type: string
+      enum:
+        - n/a
+wavelength_actual:
+  name: wavelength_actual
+  display_name: Wavelength actual
+  description: |
+    Measured wavelength of light in nm.
+    `n/a` for channels that do not contain raw NIRS signals (acceleration).
+    This field is equivalent to `measurementList.wavelengthActual` in the SNIRF specification.
+  type: number
+wavelength_emission_actual:
+  name: wavelength_emission_actual
+  display_name: Wavelength emission actual
+  description: |
+    Measured emission wavelength of light in nm.
+    `n/a` for channels that do not contain raw NIRS signals (acceleration).
+    This field is equivalent to `measurementList.wavelengthEmissionActual` in the SNIRF specification.
+  type: number
 whole_blood_radioactivity:
   name: whole_blood_radioactivity
   display_name: Whole blood radioactivity
   description: |
     Radioactivity in whole blood samples,
     in unit of radioactivity measurements in whole blood samples (for example, `kBq/mL`).
   type: number
@@ -677,7 +838,70 @@
   description: |
     Recorded position along the z-axis.
   anyOf:
     - type: number
     - type: string
       enum:
         - n/a
+x__optodes:
+  name: x
+  display_name: X position
+  description: |
+    Recorded position along the x-axis.
+    `"n/a"` if not available.
+  anyOf:
+    - type: number
+    - type: string
+      enum:
+        - n/a
+y__optodes:
+  name: y
+  display_name: Y position
+  description: |
+    Recorded position along the y-axis.
+    `"n/a"` if not available.
+  anyOf:
+    - type: number
+    - type: string
+      enum:
+        - n/a
+z__optodes:
+  name: z
+  display_name: Z position
+  description: |
+    Recorded position along the z-axis.
+    `"n/a"` if not available.
+  anyOf:
+    - type: number
+    - type: string
+      enum:
+        - n/a
+template_x:
+  name: template_x
+  display_name: X template position
+  description: |
+    Assumed or ideal position along the x axis.
+  anyOf:
+    - type: number
+    - type: string
+      enum:
+        - n/a
+template_y:
+  name: template_y
+  display_name: Y template position
+  description: |
+    Assumed or ideal position along the y axis.
+  anyOf:
+    - type: number
+    - type: string
+      enum:
+        - n/a
+template_z:
+  name: template_z
+  display_name: Z template position
+  description: |
+    Assumed or ideal position along the z axis.
+  anyOf:
+    - type: number
+    - type: string
+      enum:
+        - n/a
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/common_principles.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/common_principles.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         8.  `ieeg` (intracranial electroencephalography)
 
         9.  `beh` (behavioral)
 
         10. `pet` (positron emission tomography)
 
         11. `micr` (microscopy)
+
+        12. `nirs` (near infrared spectroscopy)
 dataset:
   name: Dataset
   display_name: Dataset
   description: |
     A set of neuroimaging and behavioral data acquired for a purpose of a particular study.
     A dataset consists of data acquired from one or more subjects, possibly from multiple sessions.
 deprecated:
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/datatypes.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/datatypes.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -49,7 +49,11 @@
   description: |
     Blood perfusion imaging data, including arterial spin labeling (ASL)
 pet:
   value: pet
   display_name: Positron Emission Tomography
   description: |
     Positron emission tomography data
+nirs:
+  value: nirs
+  display_name: Near-Infrared Spectroscopy
+  description: Near-Infrared Spectroscopy data organized around the SNIRF format
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/entities.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/entities.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 
     This entity represents the `"MTState"` metadata field.
     Therefore, if the `mt-<label>` entity is present in a filename,
     `"MTState"` MUST be defined in the associated metadata.
     Allowed label values for this entity are `on` and `off`,
     for images acquired in presence and absence of an MT pulse, respectively.
   type: string
+  format: label
   enum:
     - 'on'
     - 'off'
 part:
   name: part
   display_name: Part
   description: |
@@ -200,14 +201,15 @@
     Phase images MAY be in radians or in arbitrary units.
     The sidecar JSON file MUST include the units of the `phase` image.
     The possible options are `"rad"` or `"arbitrary"`.
 
     When there is only a magnitude image of a given type, the `part` entity MAY be
     omitted.
   type: string
+  format: label
   enum:
     - mag
     - phase
     - real
     - imag
 processing:
   name: proc
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/extensions.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/extensions.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 chn:
   value: .chn
   display_name: KRISS CHN
   description: |
     A file generated by KRISS MEG systems containing the position of the center of the MEG coils.
 
     Each experimental run on the KRISS system produces a file with extension `.kdf`.
-    Additional files that may be available in the same folder include
+    Additional files that may be available in the same directory include
     the digitized positions of the head points (`\_digitizer.txt`),
     the position of the center of the MEG coils (`.chn`),
     and the event markers (`.trg`).
 con:
   value: .con
   display_name: KIT/Yokogawa/Ricoh Continuous Data
   description: |
@@ -66,17 +66,17 @@
 dat:
   value: .dat
   display_name: MEG Fine-Calibration Format
   description: |
     A fine-calibration file used for Neuromag/Elekta/MEGIN MEG recording hardware.
 CTF:
   value: .ds/
-  display_name: CTF MEG Dataset Folder
+  display_name: CTF MEG Dataset Directory
   description: |
-    A folder for MEG data, typically containing a `.meg4` file for the data and a `.res4` file for the resources.
+    A directory for MEG data, typically containing a `.meg4` file for the data and a `.res4` file for the resources.
 dlabelnii:
   value: .dlabel.nii
   display_name: CIFTI-2 Dense Label File
   description: |
     A CIFTI-2 dense label file.
 
     This extension may only be used in derivative datasets.
@@ -128,15 +128,15 @@
 kdf:
   value: .kdf
   display_name: KRISS KDF
   description: |
     A KRISS (file with extension `.kdf`) file.
 
     Each experimental run on the KRISS system produces a file with extension `.kdf`.
-    Additional files that may be available in the same folder include
+    Additional files that may be available in the same directory include
     the digitized positions of the head points (`\_digitizer.txt`),
     the position of the center of the MEG coils (`.chn`),
     and the event markers (`.trg`).
 labelgii:
   value: .label.gii
   display_name: GIFTI label/annotation file
   description: |
@@ -148,15 +148,15 @@
   display_name: Markdown
   description: |
     A Markdown file.
 mefd:
   value: .mefd/
   display_name: Multiscale Electrophysiology File Format Version 3.0
   description: |
-    A folder in the [MEF3](https://osf.io/e3sf9/) format.
+    A directory in the [MEF3](https://osf.io/e3sf9/) format.
 
     Each recording consists of a `.mefd` directory.
 mhd:
   value: .mhd
   display_name: ITAB Binary Header
   description: |
     Produced by ITAB-ARGOS153 systems. This file a binary header file, and is generated along with a
@@ -233,14 +233,19 @@
   value: .set
   display_name: EEGLAB SET
   description: |
     An [EEGLAB](https://sccn.ucsd.edu/eeglab) file.
 
     The format used by the MATLAB toolbox [EEGLAB](https://sccn.ucsd.edu/eeglab).
     Each recording consists of a `.set` file with an optional `.fdt` file.
+snirf:
+  value: .snirf
+  display_name: Shared Near Infrared Spectroscopy Format
+  description: |
+    HDF5 file organized according to the [SNIRF specification](https://github.com/fNIRS/snirf)
 sqd:
   value: .sqd
   display_name: SQD
   description: |
     A file containing either raw MEG data or MEG sensor coil positions.
     While this extension is still valid, it has been succeeded by `.con` for raw MEG data and `.mrk` for
     marker information.
@@ -254,15 +259,15 @@
 trg:
   value: .trg
   display_name: KRISS TRG
   description: |
     A file generated by KRISS MEG systems containing the event markers.
 
     Each experimental run on the KRISS system produces a file with extension `.kdf`.
-    Additional files that may be available in the same folder include
+    Additional files that may be available in the same directory include
     the digitized positions of the head points (`\_digitizer.txt`),
     the position of the center of the MEG coils (`.chn`),
     and the event markers (`.trg`).
 tsv:
   value: .tsv
   display_name: Tab-Delimited
   description: |
@@ -303,11 +308,11 @@
 None:
   value: ''
   display_name: No extension
   description: |
     A file with no extension.
 Directory:
   value: /
-  display_name: Folder
+  display_name: Directory
   description: |
-    A folder with no extension.
+    A directory with no extension.
     Corresponds to BTi/4D data.
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/formats.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/formats.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/metadata.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/metadata.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 ---
 # This file defines valid BIDS metadata fields.
 # These definitions include the field names, their descriptions, and valid values.
 # This file **does not** define how and when metadata fields can be used with a given file.
+ACCELChannelCount:
+  name: ACCELChannelCount
+  display_name: Accelerometer channel count
+  description: |
+    Number of accelerometer channels.
+  type: integer
+  minimum: 0
 Acknowledgements:
   name: Acknowledgements
   display_name: Acknowledgements
   description: |
     Text acknowledging contributions of individuals or institutions beyond
     those listed in Authors or Funding.
   type: string
@@ -364,15 +371,15 @@
   description: |
     Name of the cap manufacturer (for example, `"EasyCap"`).
   type: string
 CapManufacturersModelName:
   name: CapManufacturersModelName
   display_name: Cap Manufacturers Model Name
   description: |
-    Manufacturer's designation of the EEG cap model
+    Manufacturer's designation of the cap model
     (for example, `"actiCAP 64 Ch Standard-2"`).
   type: string
 CellType:
   name: CellType
   display_name: Cell Type
   description: |
     Describes the type of cell analyzed.
@@ -582,14 +589,29 @@
   type: boolean
 Description:
   name: Description
   display_name: Description
   description: |
     Free-form natural language description.
   type: string
+DetectorType:
+  name: DetectorType
+  display_name: Detector Type
+  description: |
+    Type of detector. This is a free form description with the following suggested terms:
+    `"SiPD"`, `"APD"`. Preferably a specific model/part number is supplied.
+    If individual channels have different `DetectorType`,
+    then the field here should be specified as `"mixed"`
+    and this column should be included in `optodes.tsv`.
+  anyOf:
+    - type: string
+      format: unit
+    - type: string
+      enum:
+        - mixed
 DeviceSerialNumber:
   name: DeviceSerialNumber
   display_name: Device Serial Number
   description: |
     The serial number of the equipment that produced the measurements.
     A pseudonym can also be used to prevent the equipment from being
     identifiable, so long as each pseudonym is unique within the dataset.
@@ -1123,14 +1145,21 @@
   display_name: Gradient Set Type
   description: |
     It should be possible to infer the gradient coil from the scanner model.
     If not, for example because of a custom upgrade or use of a gradient
     insert set, then the specifications of the actual gradient coil should be
     reported independently.
   type: string
+GYROChannelCount:
+  name: GYROChannelCount
+  display_name: Gyrometer Channel Count
+  description: |
+    Number of gyrometer channels.
+  type: integer
+  minimum: 0
 HED:
   name: HED
   display_name: HED
   description: |
     Hierarchical Event Descriptor (HED) information,
     see the [HED Appendix](SPEC_ROOT/appendices/hed.md) for details.
   anyOf:
@@ -1673,14 +1702,21 @@
     `"Absent"` means that no specific M0 information is present.
   type: string
   enum:
     - Separate
     - Included
     - Estimate
     - Absent
+MAGNChannelCount:
+  name: MAGNChannelCount
+  display_name: Magnetometer Channel Count
+  description: |
+    Number of magnetometer channels.
+  type: integer
+  minimum: 0
 MEGChannelCount:
   name: MEGChannelCount
   display_name: MEG Channel Count
   description: |
     Number of MEG channels (for example, `275`).
   type: integer
   minimum: 0
@@ -1959,14 +1995,95 @@
     `true` or `false` value specifying whether increasing voxel intensity
     (within sample voxels) denotes a decreased value with respect to the
     contrast suffix.
     This is commonly the case when Cerebral Blood Volume is estimated via
     usage of a contrast agent in conjunction with a T2\* weighted acquisition
     protocol.
   type: boolean
+NIRSChannelCount:
+  name: NIRSChannelCount
+  display_name: NIRS Channel Count
+  description: |
+    Total number of NIRS channels, including short channels.
+    Corresponds to the number of rows in `channels.tsv` with any NIRS type.
+  type: integer
+  minimum: 0
+NIRSSourceOptodeCount:
+  name: NIRSSourceOptodeCount
+  display_name: NIRS Source Optode Count
+  description: |
+    Number of NIRS sources.
+    Corresponds to the number of rows in `optodes.tsv` with type `"source"`.
+  type: integer
+  minimum: 1
+NIRSDetectorOptodeCount:
+  name: NIRSDetectorOptodeCount
+  display_name: NIRS Detector Optode Channel Count
+  description: |
+    Number of NIRS detectors.
+    Corresponds to the number of rows in `optodes.tsv` with type `"detector"`.
+  type: integer
+  minimum: 1
+NIRSPlacementScheme:
+  name: NIRSPlacementScheme
+  display_name: NIRS Placement Scheme
+  description: |
+    Placement scheme of NIRS optodes.
+    Either the name of a standardized placement system (for example, `"10-20"`)
+    or an array of standardized position names (for example, `["Cz", "Pz"]`).
+    This field should only be used if a cap was not used.
+    If a standard cap was used, then it should be specified in `CapManufacturer`
+    and `CapManufacturersModelName` and this field should be set to `"n/a"`
+  anyOf:
+    - type: string
+    - type: array
+      items:
+        type: string
+NIRSCoordinateSystem:
+  name: NIRSCoordinateSystem
+  display_name: NIRS Coordinate System
+  description: |
+    Defines the coordinate system in which the optode positions are expressed.
+
+    See
+    [Appendix VIII](SPEC_ROOT/appendices/coordinate-systems.md)
+    for a list of restricted keywords for coordinate systems.
+    If `"Other"`, a definition of the coordinate system MUST be
+    provided in `NIRSCoordinateSystemDescription`.
+  anyOf:
+    - $ref: objects.metadata._MEGCoordSys
+    - $ref: objects.metadata._EEGCoordSys
+    - $ref: objects.metadata._StandardTemplateCoordSys
+    - $ref: objects.metadata._StandardTemplateDeprecatedCoordSys
+NIRSCoordinateSystemDescription:
+  name: NIRSCoordinateSystemDescription
+  display_name: NIRS Coordinate System Description
+  description: |
+    Free-form text description of the coordinate system.
+    May also include a link to a documentation page or paper describing the
+    system in greater detail.
+  type: string
+NIRSCoordinateUnits:
+  name: NIRSCoordinateUnits
+  display_name: NIRS Coordinate Units
+  description: |
+    Units of the coordinates of `NIRSCoordinateSystem`.
+  type: string
+  enum:
+    - m
+    - mm
+    - cm
+    - n/a
+NIRSCoordinateProcessingDescription:
+  name: NIRSCoordinateProcessingDescription
+  display_name: NIRS Coordinate Processing Description
+  description: |
+    Has any post-processing (such as projection) been done on the optode
+    positions (for example, `"surface_projection"`, `"n/a"`).
+  type: string
 NonlinearGradientCorrection:
   name: NonlinearGradientCorrection
   display_name: Nonlinear Gradient Correction
   description: |
     Boolean stating if the image saved has been corrected for gradient
     nonlinearities by the scanner sequence.
   type: boolean
@@ -2435,15 +2552,15 @@
   exclusiveMinimum: 0
   unit: s
 RepetitionTimeExcitation:
   name: RepetitionTimeExcitation
   display_name: Repetition Time Excitation
   description: |
     The interval, in seconds, between two successive excitations.
-    [DICOM Tag 0018, 0080](http://dicomlookup.com/lookup.asp?sw=Tnumber&q=(0018,0080)
+    [DICOM Tag 0018, 0080](http://dicomlookup.com/lookup.asp?sw=Tnumber&q=(0018,0080))
     best refers to this parameter.
     This field may be used together with the `"RepetitionTimePreparation"` for
     certain use cases, such as
     [MP2RAGE](https://doi.org/10.1016/j.neuroimage.2009.10.002).
     Use `RepetitionTimeExcitation` (in combination with
     `"RepetitionTimePreparation"` if needed) for anatomy imaging data rather than
     `"RepetitionTime"` as it is already defined as the amount of time that it takes
@@ -2598,14 +2715,26 @@
   name: SamplingFrequency
   display_name: Sampling Frequency
   description: |
     Sampling frequency (in Hz) of all the data in the recording,
     regardless of their type (for example, `2400`).
   type: number
   unit: Hz
+SamplingFrequency__nirs:
+  name: SamplingFrequency
+  display_name: Sampling Frequency
+  description: |
+    Sampling frequency (in Hz) of all the data in the recording,
+    regardless of their type (for example, `2400`).
+  anyOf:
+    - type: number
+      unit: Hz
+    - type: string
+      enum:
+        - n/a
 ScaleFactor:
   name: ScaleFactor
   display_name: Scale Factor
   description: |
     Scale factor for each frame. This field MUST be defined if the imaging data (`.nii[.gz]`) are scaled.
     If this field is not defined, then it is assumed that the scaling factor is 1. Defining this field
     when the scaling factor is 1 is RECOMMENDED, for the sake of clarity.
@@ -2674,14 +2803,21 @@
     Variant of the ScanningSequence.
     Corresponds to DICOM Tag 0018, 0021 `Sequence Variant`.
   anyOf:
     - type: string
     - type: array
       items:
         type: string
+ShortChannelCount:
+  name: ShortChannelCount
+  display_name: Short Channel Count
+  description: |
+    The number of short channels. 0 indicates no short channels.
+  type: integer
+  minimum: 0
 SinglesRate:
   name: SinglesRate
   display_name: Singles Rate
   description: |
     Singles rate for each frame (same units as `Units`, for example, `"Bq/mL"`).
   type: array
   items:
@@ -2827,19 +2963,26 @@
     However, in case both X and Y are directly used in the creation of Z,
     then Z should list X and Y in `"Sources"`,
     regardless of whether X was used to generate Y.
     Using paths specified relative to the dataset root is
     [DEPRECATED](SPEC_ROOT/02-common-principles.md#definitions).
   type: array
   items:
-    anyOf:
-      - type: string
-        format: dataset_relative
-      - type: string
-        format: bids_uri
+    type: string
+    format: dataset_relative
+SourceType:
+  name: SourceType
+  display_name: Source Type
+  description: |
+    Type of source. Preferably a specific model/part number is supplied.
+    This is a freeform description, but the following keywords are suggested:
+    `"LED"`, `"LASER"`, `"VCSEL"`. If individual channels have different SourceType,
+    then the field here should be specified as "mixed"
+    and this column should be included in optodes.tsv.
+  type: string
 SpatialReference:
   name: SpatialReference
   display_name: Spatial Reference
   description: |
     For images with a single reference, the value MUST be a single string.
     For images with multiple references, such as surface and volume references,
     a JSON object MUST be used.
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/modalities.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/modalities.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -24,7 +24,10 @@
   display_name: Positron Emission Tomography
   description: |
     Data acquired with PET.
 micr:
   display_name: Microscopy
   description: |
     Data acquired with a microscope.
+nirs:
+  display_name: Near-Infrared Spectroscopy
+  description: Data acquired with NIRS.
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/suffixes.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/suffixes.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -665,14 +665,24 @@
     This suffix may only be used in derivative datasets.
 meg:
   value: meg
   display_name: Magnetoencephalography
   description: |
     Unprocessed MEG data stored in the native file format of the MEG instrument
     with which the data was collected.
+nirs:
+  value: nirs
+  display_name: Near Infrared Spectroscopy
+  description: Data associated with a Shared Near Infrared Spectroscopy Format file.
+optodes:
+  value: optodes
+  display_name: Optodes
+  description: |
+    Either a light emitting device, sometimes called a transmitter, or a photoelectric transducer, sometimes called a
+    receiver.
 pet:
   value: pet
   display_name: Positron Emission Tomography
   description: |
     PET imaging data SHOULD be stored in 4D
     (or 3D, if only one volume was acquired) NIfTI files with the `_pet` suffix.
     Volumes MUST be stored in chronological order
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/objects/top_level_files.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/objects/files.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 ---
 # This file describes files which may appear at the top level of a dataset.
 # This does not include information about whether these files are required or optional.
 # For that information, see `rules/top_level_files.yaml`.
 CHANGES:
   display_name: Changelog
+  file_type: regular
   description: |
     Version history of the dataset (describing changes, updates and corrections) MAY be provided in
     the form of a `CHANGES` text file.
     This file MUST follow the
     [CPAN Changelog convention](https://metacpan.org/pod/release/HAARG/CPAN-Changes-0.400002/lib/\
     CPAN/Changes/Spec.pod).
     The `CHANGES` file MUST be either in ASCII or UTF-8 encoding.
 LICENSE:
   display_name: License
+  file_type: regular
   description: |
     A `LICENSE` file MAY be provided in addition to the short specification of the
     used license in the `dataset_description.json` `"License"` field.
     The `"License"` field and `LICENSE` file MUST correspond.
     The `LICENSE` file MUST be either in ASCII or UTF-8 encoding.
 README:
   display_name: README
+  file_type: regular
   description: |
     A REQUIRED text file, `README`, SHOULD describe the dataset in more detail.
     The `README` file MUST be either in ASCII or UTF-8 encoding and MAY have one of the extensions:
     `.md` ([Markdown](https://www.markdownguide.org/)),
     `.rst` ([reStructuredText](https://docutils.sourceforge.io/rst.html)),
     or `.txt`.
     A BIDS dataset MUST NOT contain more than one `README` file (with or without extension)
@@ -33,26 +36,29 @@
     and does not validate the syntax of Markdown and reStructuredText.
     The `README` file SHOULD be structured such that its contents can be easily understood
     even if the used format is not rendered.
     A guideline for creating a good `README` file can be found in the
     [bids-starter-kit](https://github.com/bids-standard/bids-starter-kit/blob/master/templates/README).
 dataset_description:
   display_name: Dataset Description
+  file_type: regular
   description: |
     The file `dataset_description.json` is a JSON file describing the dataset.
 genetic_info:
   display_name: Genetic Information
+  file_type: regular
   description: |
     The `genetic_info.json` file describes the genetic information available in the
     `participants.tsv` file and/or the genetic database described in
     `dataset_description.json`.
     Datasets containing the `Genetics` field in `dataset_description.json` or the
     `genetic_id` column in `participants.tsv` MUST include this file.
 participants:
   display_name: Participant Information
+  file_type: regular
   description: |
     The purpose of this RECOMMENDED file is to describe properties of participants
     such as age, sex, handedness.
     If this file exists, it MUST contain the column `participant_id`,
     which MUST consist of `sub-<label>` values identifying one row for each participant,
     followed by a list of optional columns describing participants.
     Each participant MUST be described by one and only one row.
@@ -87,14 +93,15 @@
             `AMBIDEXTROUS`, `Ambidextrous`
 
     Throughout BIDS you can indicate missing values with `n/a` (for "not
     available").
 
 samples:
   display_name: Sample Information
+  file_type: regular
   description: |
     The purpose of this file is to describe properties of samples, indicated by the `sample` entity.
     This file is REQUIRED if `sample-<label>` is present in any file name within the dataset.
     If this file exists, it MUST contain the three following columns:
 
     -   `sample_id`: MUST consist of `sample-<label>` values identifying one row
         for each sample
@@ -115,7 +122,37 @@
     -   `pathology`: string value describing the pathology of the sample or type of control.
         When different from `healthy`, pathology SHOULD be specified in `samples.tsv`.
         The pathology MAY instead be specified in
         [Sessions files](SPEC_ROOT/03-modality-agnostic-files.md#sessions-file) in case it changes over time.
 
     -   `derived_from`: `sample-<label>` key/value pair from which a sample is derived from,
         for example a slice of tissue (`sample-02`) derived from a block of tissue (`sample-01`)
+code:
+  display_name: Code
+  file_type: directory
+  description: |
+    A directory in which to store any code
+    (for example the one used to generate the derivatives from the raw data).
+    See the [Code section](SPEC_ROOT/03-modality-agnostic-files.md#code)
+    for more information.
+derivatives:
+  display_name: Derivative data
+  file_type: directory
+  description: |
+    Derivative data (for example preprocessed files).
+    See the [relevant section](SPEC_ROOT/02-common-principles.md#source-vs-raw-vs-derived-data)
+    for more information.
+sourcedata:
+  display_name: Source data
+  file_type: directory
+  description: |
+    A directory where to store data before harmonization, reconstruction,
+    and/or file format conversion (for example, E-Prime event logs or DICOM files).
+    See the [relevant section](SPEC_ROOT/02-common-principles.md#source-vs-raw-vs-derived-data)
+    for more information.
+stimuli:
+  display_name: Stimulus files
+  file_type: directory
+  description: |
+    A directory to store any stimulus files used during an experiment.
+    See the [relevant section](SPEC_ROOT/04-modality-specific-files/05-task-events.md#stimuli-directory)
+    for more information.
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/asl.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/asl.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/dwi.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/dwi.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/events.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/events.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -5,12 +5,13 @@
   issue:
     code: EVENTS_TSV_MISSING
     message: |
       Task scans should have a corresponding events.tsv file.
       If this is a resting state scan you can ignore this warning or rename the task to include the word "rest".
     level: warning # could be an error with the proper selectors, I think
   selectors:
+    - dataset.dataset_description.DatasetType == "raw"
     - '"task" in entities'
-    - '!matches(entities.task, "rest")'
+    - '!match(entities.task, "rest")'
     - suffix != "events"
   checks:
     - '"events" in associations'
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/fmap.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/fmap.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/func.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/func.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/checks/hints.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/hints.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
       The onset of the last event is after the total duration of the corresponding scan.
       This design is suspiciously long.
     level: warning
   selectors:
     - suffix == "bold"
     - associations.events != null
   checks:
-    - max(associations.events.onset) > nifti_header.pixdim[4] * nifti_header.dim[4]
+    - max(associations.events.onset) < nifti_header.pixdim[4] * nifti_header.dim[4]
 
 SuspiciouslyShortBOLDDesign:
   issue:
     code: SUSPICIOUSLY_SHORT_EVENT_DESIGN
     message: |
       The onset of the last event is less than half the total duration of the corresponding scan.
       This design is suspiciously short.
     level: warning
   selectors:
     - suffix == "bold"
     - associations.events != null
   checks:
-    - max(associations.events.onset) < nifti_header.pixdim[4] * nifti_header.dim[4] / 2
+    - max(associations.events.onset) > nifti_header.pixdim[4] * nifti_header.dim[4] / 2
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/common_derivatives_validation.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/checks/common_derivatives.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/dataset_metadata.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/dataset_metadata.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/anat.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/anat.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/derivatives/common_imaging_derivatives.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/deriv/imaging.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,230 +1,208 @@
 ---
 anat_parametric_volumetric:
-  $ref: rules.datatypes.anat.parametric
+  $ref: rules.files.raw.anat.parametric
   entities:
-    $ref: rules.datatypes.anat.parametric.entities
+    $ref: rules.files.raw.anat.parametric.entities
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 anat_nonparametric_volumetric:
-  $ref: rules.datatypes.anat.nonparametric
+  $ref: rules.files.raw.anat.nonparametric
   entities:
-    $ref: rules.datatypes.anat.nonparametric.entities
+    $ref: rules.files.raw.anat.nonparametric.entities
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 dwi_volumetric:
-  $ref: rules.datatypes.dwi.dwi
+  $ref: rules.files.raw.dwi.dwi
   entities:
-    $ref: rules.datatypes.dwi.dwi.entities
+    $ref: rules.files.raw.dwi.dwi.entities
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 func_volumetric:
-  $ref: rules.datatypes.func.func
+  $ref: rules.files.raw.func.func
   entities:
-    $ref: rules.datatypes.func.func.entities
+    $ref: rules.files.raw.func.func.entities
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 anat_parametric_mask:
-  $ref: rules.datatypes.anat.parametric
+  $ref: rules.files.raw.anat.parametric
   suffixes:
     - mask
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.anat.parametric.entities
+    $ref: rules.files.raw.anat.parametric.entities
     space: optional
     resolution: optional
     density: optional
     label: optional
     description: optional
 
 anat_nonparametric_mask:
-  $ref: rules.datatypes.anat.nonparametric
+  $ref: rules.files.raw.anat.nonparametric
   suffixes:
     - mask
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.anat.nonparametric.entities
+    $ref: rules.files.raw.anat.nonparametric.entities
     space: optional
     resolution: optional
     density: optional
     label: optional
     description: optional
 
 dwi_mask:
-  $ref: rules.datatypes.dwi.dwi
+  $ref: rules.files.raw.dwi.dwi
   suffixes:
     - mask
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.dwi.dwi.entities
+    $ref: rules.files.raw.dwi.dwi.entities
     space: optional
     resolution: optional
     density: optional
     label: optional
     description: optional
 
 func_mask:
-  $ref: rules.datatypes.func.func
+  $ref: rules.files.raw.func.func
   suffixes:
     - mask
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.func.func.entities
+    $ref: rules.files.raw.func.func.entities
     space: optional
     resolution: optional
     density: optional
     label: optional
     description: optional
 
 anat_parametric_discrete_segmentation:
-  $ref: rules.datatypes.anat.parametric
+  $ref: rules.files.raw.anat.parametric
   suffixes:
     - dseg
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.anat.parametric.entities
+    $ref: rules.files.raw.anat.parametric.entities
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 anat_nonparametric_discrete_segmentation:
-  $ref: rules.datatypes.anat.nonparametric
+  $ref: rules.files.raw.anat.nonparametric
   suffixes:
     - dseg
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.anat.nonparametric.entities
+    $ref: rules.files.raw.anat.nonparametric.entities
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 func_discrete_segmentation:
-  $ref: rules.datatypes.func.func
+  $ref: rules.files.raw.func.func
   suffixes:
     - dseg
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.func.func.entities
+    $ref: rules.files.raw.func.func.entities
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 dwi_discrete_segmentation:
-  $ref: rules.datatypes.dwi.dwi
+  $ref: rules.files.raw.dwi.dwi
   suffixes:
     - dseg
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.dwi.dwi.entities
+    $ref: rules.files.raw.dwi.dwi.entities
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 anat_parametric_probabilistic_segmentation:
-  $ref: rules.datatypes.anat.parametric
+  $ref: rules.files.raw.anat.parametric
   suffixes:
     - probseg
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.anat.parametric.entities
+    $ref: rules.files.raw.anat.parametric.entities
     space: optional
     resolution: optional
     density: optional
     label: optional
     description: optional
 
 anat_nonparametric_probabilistic_segmentation:
-  $ref: rules.datatypes.anat.nonparametric
+  $ref: rules.files.raw.anat.nonparametric
   suffixes:
     - probseg
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.anat.nonparametric.entities
+    $ref: rules.files.raw.anat.nonparametric.entities
     space: optional
     resolution: optional
     density: optional
     label: optional
     description: optional
 
 func_probabilistic_segmentation:
-  $ref: rules.datatypes.func.func
+  $ref: rules.files.raw.func.func
   suffixes:
     - probseg
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.func.func.entities
+    $ref: rules.files.raw.func.func.entities
     space: optional
     resolution: optional
     density: optional
     label: optional
     description: optional
 
 dwi_probabilistic_segmentation:
-  $ref: rules.datatypes.dwi.dwi
+  $ref: rules.files.raw.dwi.dwi
   suffixes:
     - probseg
-  extensions:
-    - .nii.gz
   entities:
-    $ref: rules.datatypes.dwi.dwi.entities
+    $ref: rules.files.raw.dwi.dwi.entities
     space: optional
     resolution: optional
     density: optional
     label: optional
     description: optional
 
 anat_parametic_discrete_surface:
-  $ref: rules.datatypes.anat.parametric
+  $ref: rules.files.raw.anat.parametric
   suffixes:
     - dseg
   extensions:
     - .label.gii
     - .dlabel.nii
+    - .json
   entities:
-    $ref: rules.datatypes.anat.parametric.entities
+    $ref: rules.files.raw.anat.parametric.entities
     hemisphere: optional
     space: optional
     resolution: optional
     density: optional
     description: optional
 
 anat_nonparametic_discrete_surface:
-  $ref: rules.datatypes.anat.nonparametric
+  $ref: rules.files.raw.anat.nonparametric
   suffixes:
     - dseg
   extensions:
     - .label.gii
     - .dlabel.nii
+    - .json
   entities:
-    $ref: rules.datatypes.anat.nonparametric.entities
+    $ref: rules.files.raw.anat.nonparametric.entities
     hemisphere: optional
     space: optional
     resolution: optional
     density: optional
     description: optional
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/dwi.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/channels.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,77 @@
 ---
-dwi:
+channels:
   suffixes:
-    - dwi
+    - channels
   extensions:
-    - .nii.gz
-    - .nii
     - .json
-    - .bvec
-    - .bval
+    - .tsv
   datatypes:
-    - dwi
+    - eeg
+    - ieeg
+    - nirs
   entities:
     subject: required
     session: optional
+    task: required
     acquisition: optional
-    reconstruction: optional
-    direction: optional
     run: optional
-    part: optional
 
-sbref:
+# MEG has an additional entity available
+channels__meg:
+  $ref: rules.files.raw.channels.channels
+  datatypes:
+    - meg
+  entities:
+    $ref: rules.files.raw.channels.channels.entities
+    processing: optional
+
+coordsystem:
   suffixes:
-    - sbref
+    - coordsystem
   extensions:
-    - .nii.gz
-    - .nii
     - .json
   datatypes:
-    - dwi
+    - meg
+    - nirs
   entities:
     subject: required
     session: optional
     acquisition: optional
-    reconstruction: optional
-    direction: optional
-    run: optional
-    part: optional
 
-timeseries:
+# (i)EEG has a space entity
+coordsystem__eeg:
+  $ref: rules.files.raw.channels.coordsystem
+  datatypes:
+    - eeg
+    - ieeg
+  entities:
+    $ref: rules.files.raw.channels.coordsystem.entities
+    space: optional
+
+electrodes:
   suffixes:
-    - physio
-    - stim
+    - electrodes
   extensions:
-    - .tsv.gz
     - .json
+    - .tsv
   datatypes:
-    - dwi
+    - eeg
+    - ieeg
+  entities:
+    subject: required
+    session: optional
+    acquisition: optional
+    space: optional
+
+optodes:
+  suffixes:
+    - optodes
+  extensions:
+    - .tsv
+    - .json
+  datatypes:
+    - nirs
   entities:
     subject: required
     session: optional
     acquisition: optional
-    reconstruction: optional
-    direction: optional
-    run: optional
-    part: optional
-    recording: optional
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/eeg.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/fmap.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,143 @@
 ---
-eeg:
+fieldmaps:
   suffixes:
-    - eeg
+    - phasediff
+    - phase1
+    - phase2
+    - magnitude1
+    - magnitude2
+    - magnitude
+    - fieldmap
   extensions:
+    - .nii.gz
+    - .nii
     - .json
-    - .edf
-    - .vhdr
-    - .vmrk
-    - .eeg
-    - .set
-    - .fdt
-    - .bdf
   datatypes:
-    - eeg
+    - fmap
   entities:
     subject: required
     session: optional
-    task: required
     acquisition: optional
     run: optional
 
-channels:
+pepolar:
   suffixes:
-    - channels
+    - epi
+    - m0scan
   extensions:
+    - .nii.gz
+    - .nii
     - .json
-    - .tsv
   datatypes:
-    - eeg
+    - fmap
   entities:
     subject: required
     session: optional
-    task: required
     acquisition: optional
+    ceagent: optional
+    direction: required
     run: optional
 
-coordsystem:
+TB1DAM:
   suffixes:
-    - coordsystem
+    - TB1DAM
   extensions:
+    - .nii.gz
+    - .nii
     - .json
   datatypes:
-    - eeg
+    - fmap
   entities:
     subject: required
     session: optional
     acquisition: optional
-    space: optional
+    ceagent: optional
+    reconstruction: optional
+    run: optional
+    flip: required
+    inversion: optional
+    part: optional
 
-electrodes:
+TB1EPI:
   suffixes:
-    - electrodes
+    - TB1EPI
   extensions:
+    - .nii.gz
+    - .nii
     - .json
-    - .tsv
   datatypes:
-    - eeg
+    - fmap
   entities:
     subject: required
     session: optional
     acquisition: optional
-    space: optional
+    ceagent: optional
+    reconstruction: optional
+    run: optional
+    echo: required
+    flip: required
+    inversion: optional
+    part: optional
 
-events:
+RFFieldMaps:
   suffixes:
-    - events
+    - TB1AFI
+    - TB1TFL
+    - TB1RFM
+    - RB1COR
   extensions:
+    - .nii.gz
+    - .nii
     - .json
-    - .tsv
   datatypes:
-    - eeg
+    - fmap
   entities:
     subject: required
     session: optional
-    task: required
     acquisition: optional
+    ceagent: optional
+    reconstruction: optional
     run: optional
+    echo: optional
+    flip: optional
+    inversion: optional
+    part: optional
 
-photo:
+TB1SRGE:
   suffixes:
-    - photo
+    - TB1SRGE
   extensions:
-    - .jpg
-    - .png
-    - .tif
+    - .nii.gz
+    - .nii
+    - .json
   datatypes:
-    - eeg
+    - fmap
   entities:
     subject: required
     session: optional
     acquisition: optional
+    ceagent: optional
+    reconstruction: optional
+    run: optional
+    echo: optional
+    flip: required
+    inversion: required
+    part: optional
 
-timeseries:
+parametric:
   suffixes:
-    - physio
-    - stim
+    - TB1map
+    - RB1map
   extensions:
-    - .tsv.gz
+    - .nii.gz
+    - .nii
     - .json
   datatypes:
-    - eeg
+    - fmap
   entities:
     subject: required
     session: optional
-    task: required
     acquisition: optional
+    ceagent: optional
+    reconstruction: optional
     run: optional
-    recording: optional
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/fmap.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/func.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,43 @@
 ---
-fieldmaps:
+func:
   suffixes:
-    - phasediff
-    - phase1
-    - phase2
-    - magnitude1
-    - magnitude2
-    - magnitude
-    - fieldmap
+    - bold
+    - cbv
+    - sbref
   extensions:
     - .nii.gz
     - .nii
     - .json
   datatypes:
-    - fmap
-  entities:
-    subject: required
-    session: optional
-    acquisition: optional
-    run: optional
-
-pepolar:
-  suffixes:
-    - epi
-    - m0scan
-  extensions:
-    - .nii.gz
-    - .nii
-    - .json
-  datatypes:
-    - fmap
-  entities:
-    subject: required
-    session: optional
-    acquisition: optional
-    ceagent: optional
-    direction: required
-    run: optional
-
-TB1DAM:
-  suffixes:
-    - TB1DAM
-  extensions:
-    - .nii.gz
-    - .nii
-    - .json
-  datatypes:
-    - fmap
-  entities:
-    subject: required
-    session: optional
-    acquisition: optional
-    ceagent: optional
-    reconstruction: optional
-    run: optional
-    flip: required
-    inversion: optional
-    part: optional
-
-TB1EPI:
-  suffixes:
-    - TB1EPI
-  extensions:
-    - .nii.gz
-    - .nii
-    - .json
-  datatypes:
-    - fmap
-  entities:
-    subject: required
-    session: optional
-    acquisition: optional
-    ceagent: optional
-    reconstruction: optional
-    run: optional
-    echo: required
-    flip: required
-    inversion: optional
-    part: optional
-
-RFFieldMaps:
-  suffixes:
-    - TB1AFI
-    - TB1TFL
-    - TB1RFM
-    - RB1COR
-  extensions:
-    - .nii.gz
-    - .nii
-    - .json
-  datatypes:
-    - fmap
+    - func
   entities:
     subject: required
     session: optional
+    task: required
     acquisition: optional
     ceagent: optional
     reconstruction: optional
+    direction: optional
     run: optional
     echo: optional
-    flip: optional
-    inversion: optional
     part: optional
 
-TB1SRGE:
+phase:
   suffixes:
-    - TB1SRGE
+    - phase # deprecated
   extensions:
     - .nii.gz
     - .nii
     - .json
   datatypes:
-    - fmap
+    - func
   entities:
     subject: required
     session: optional
+    task: required
     acquisition: optional
     ceagent: optional
     reconstruction: optional
+    direction: optional
     run: optional
     echo: optional
-    flip: required
-    inversion: required
-    part: optional
-
-parametric:
-  suffixes:
-    - TB1map
-    - RB1map
-  extensions:
-    - .nii.gz
-    - .nii
-    - .json
-  datatypes:
-    - fmap
-  entities:
-    subject: required
-    session: optional
-    acquisition: optional
-    ceagent: optional
-    reconstruction: optional
-    run: optional
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/func.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/dwi.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,38 @@
 ---
-func:
+dwi:
   suffixes:
-    - bold
-    - cbv
-    - sbref
+    - dwi
   extensions:
     - .nii.gz
     - .nii
     - .json
+    - .bvec
+    - .bval
   datatypes:
-    - func
+    - dwi
   entities:
     subject: required
     session: optional
-    task: required
     acquisition: optional
-    ceagent: optional
     reconstruction: optional
     direction: optional
     run: optional
-    echo: optional
     part: optional
 
-phase:
+sbref:
   suffixes:
-    - phase # deprecated
+    - sbref
   extensions:
     - .nii.gz
     - .nii
     - .json
   datatypes:
-    - func
-  entities:
-    subject: required
-    session: optional
-    task: required
-    acquisition: optional
-    ceagent: optional
-    reconstruction: optional
-    direction: optional
-    run: optional
-    echo: optional
-
-events:
-  suffixes:
-    - events
-  extensions:
-    - .tsv
-    - .json
-  datatypes:
-    - func
+    - dwi
   entities:
     subject: required
     session: optional
-    task: required
     acquisition: optional
-    ceagent: optional
     reconstruction: optional
     direction: optional
     run: optional
-
-timeseries:
-  suffixes:
-    - physio
-    - stim
-  extensions:
-    - .tsv.gz
-    - .json
-  datatypes:
-    - func
-  entities:
-    subject: required
-    session: optional
-    task: required
-    acquisition: optional
-    ceagent: optional
-    reconstruction: optional
-    direction: optional
-    run: optional
-    recording: optional
+    part: optional
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/ieeg.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/meg.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,86 @@
 ---
-ieeg:
+meg:
   suffixes:
-    - ieeg
+    - meg
   extensions:
-    - .mefd/
+    - / # corresponds to BTi/4D data
+    - .ds/
     - .json
-    - .edf
-    - .vhdr
-    - .eeg
-    - .vmrk
-    - .set
-    - .fdt
-    - .nwb
+    - .fif
+    - .sqd
+    - .con
+    - .raw
+    - .ave
+    - .mrk
+    - .kdf
+    - .mhd
+    - .trg
+    - .chn
   datatypes:
-    - ieeg
+    - meg
   entities:
     subject: required
     session: optional
     task: required
     acquisition: optional
     run: optional
+    processing: optional
+    split: optional
 
-channels:
+calibration:
   suffixes:
-    - channels
+    - meg
   extensions:
-    - .json
-    - .tsv
+    - .dat
   datatypes:
-    - ieeg
+    - meg
   entities:
     subject: required
     session: optional
-    task: required
-    acquisition: optional
-    run: optional
+    acquisition:
+      level: required
+      enum:
+        - calibration
 
-coordsystem:
+crosstalk:
   suffixes:
-    - coordsystem
+    - meg
   extensions:
-    - .json
+    - .fif
   datatypes:
-    - ieeg
+    - meg
   entities:
     subject: required
     session: optional
-    acquisition: optional
-    space: optional
+    acquisition:
+      level: required
+      enum:
+        - crosstalk
 
-electrodes:
+headshape:
   suffixes:
-    - electrodes
+    - headshape
   extensions:
-    - .json
-    - .tsv
+    - .*
+    - .pos
   datatypes:
-    - ieeg
+    - meg
   entities:
     subject: required
     session: optional
     acquisition: optional
-    space: optional
 
-events:
+markers:
   suffixes:
-    - events
+    - markers
   extensions:
-    - .json
-    - .tsv
+    - .sqd
+    - .mrk
   datatypes:
-    - ieeg
+    - meg
   entities:
     subject: required
     session: optional
-    task: required
+    task: optional
     acquisition: optional
-    run: optional
-
-photo:
-  suffixes:
-    - photo
-  extensions:
-    - .jpg
-    - .png
-    - .tif
-  entities:
-    subject: required
-    session: optional
-    acquisition: optional
-
-timeseries:
-  suffixes:
-    - physio
-    - stim
-  extensions:
-    - .tsv.gz
-    - .json
-  datatypes:
-    - ieeg
-  entities:
-    subject: required
-    session: optional
-    task: required
-    acquisition: optional
-    run: optional
-    recording: optional
+    space: optional
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/datatypes/perf.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/files/raw/perf.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -42,25 +42,7 @@
     - perf
   entities:
     subject: required
     session: optional
     acquisition: optional
     reconstruction: optional
     run: optional
-
-timeseries:
-  suffixes:
-    - physio
-    - stim
-  extensions:
-    - .tsv.gz
-    - .json
-  datatypes:
-    - perf
-  entities:
-    subject: required
-    session: optional
-    acquisition: optional
-    reconstruction: optional
-    direction: optional
-    run: optional
-    recording: optional
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/errors.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/errors.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/anat.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/anat.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/asl.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/asl.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/beh.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/beh.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/continuous.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/continuous.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -54,49 +54,49 @@
     Atlas:
       level: recommended
       level_addendum: if `label` entity is defined
 
 SegmentationCommon:
   selectors:
     - dataset.dataset_description.DatasetType == "derivative"
-    - '!intersects([suffix], ["dseg", "probseg"])'
+    - 'intersects([suffix], ["dseg", "probseg"])'
   fields:
     Manual: optional
 
 SegmentationCommonAtlas:
   selectors:
     - dataset.dataset_description.DatasetType == "derivative"
-    - '!intersects([suffix], ["dseg", "probseg"])'
+    - 'intersects([suffix], ["dseg", "probseg"])'
     - '"atlas" in entities'
   fields:
     Atlas:
       level: recommended
       level_addendum: if `atlas` is present
 
 # Derivatives -> Imaging data types
 ImageDerivatives:
   selectors:
     - dataset.dataset_description.DatasetType == "derivative"
-    - '!intersects([modality], ["mri", "pet"])'
-    - '!match(extension, "^\.nii(\.gz)?$")'
+    - 'intersects([modality], ["mri", "pet"])'
+    - 'match(extension, "^\.nii(\.gz)?$")'
   fields:
     SkullStripped: required
 
 ImageDerivativeResEntity:
   selectors:
     - dataset.dataset_description.DatasetType == "derivative"
-    - '!intersects([modality], ["mri", "pet"])'
+    - 'intersects([modality], ["mri", "pet"])'
     - '"res" in entities'
   fields:
     Resolution:
       level: required
       level_addendum: if `res` is present
 
 ImageDerivativeDenEntity:
   selectors:
     - dataset.dataset_description.DatasetType == "derivative"
-    - '!intersects([modality], ["mri", "pet"])'
+    - 'intersects([modality], ["mri", "pet"])'
     - '"den" in entities'
   fields:
     Density:
       level: required
       level_addendum: if `den` is present
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/dwi.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/dwi.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/eeg.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/eeg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/entity_rules.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/entity_rules.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/fmap.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/fmap.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/func.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/func.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/ieeg.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/ieeg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/meg.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/meg.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/micr.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/micr.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/mri.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/mri.yaml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/sidecars/pet.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/sidecars/pet.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -142,24 +142,27 @@
     ReconMethodName:
       level: required
       description_addendum: This partly matches the DICOM Tag (0054,1103) `Reconstruction Method`.
     ReconMethodParameterLabels:
       level: required
       description_addendum: This partly matches the DICOM Tag (0054,1103) `Reconstruction Method`.
     ReconMethodParameterUnits:
-      level: required
+      level: recommended
+      level_addendum: required if `ReconMethodParameterLabels` does not contain `"none"`
       description_addendum: This partly matches the DICOM Tag (0054,1103) `Reconstruction Method`.
     ReconMethodParameterValues:
-      level: required
+      level: recommended
+      level_addendum: required if `ReconMethodParameterLabels` does not contain `"none"`
       description_addendum: This partly matches the DICOM Tag (0054,1103) `Reconstruction Method`.
     ReconFilterType:
       level: required
       description_addendum: This partly matches the DICOM Tag (0018,1210) `Convolution Kernel`.
     ReconFilterSize:
-      level: required
+      level: recommended
+      level_addendum: required if `ReconFilterType` is not `"none"`
       description_addendum: This partly matches the DICOM Tag (0018,1210) `Convolution Kernel`.
     AttenuationCorrection:
       level: required
       description_addendum: This corresponds to DICOM Tag (0054,1101) `Attenuation Correction Method`.
     ReconMethodImplementationVersion: recommended
     AttenuationCorrectionMethodReference: recommended
     ScaleFactor: recommended
@@ -172,14 +175,33 @@
     DoseCalibrationFactor:
       level: recommended
       description_addendum: Corresponds to DICOM Tag (0054,1322) `Dose Calibration Factor`.
     PromptRate: recommended
     SinglesRate: recommended
     RandomRate: recommended
 
+# set required reconstruction fields to optional when "none" is provided as a parameter label
+EntitiesReconMethodMetadata:
+  selectors:
+    - modality == "pet"
+    - suffix == "pet"
+    - '!intersects(sidecar.ReconMethodParameterLabels, ["none"])'
+  fields:
+    ReconMethodParameterValues: required
+    ReconMethodParameterUnits: required
+
+# set required recon filter fields to optional when FilterType is "None"
+EntitiesReconFilterMetadata:
+  selectors:
+    - modality == "pet"
+    - suffix == "pet"
+    - '!intersects(sidecar.ReconFilterType, ["none"])'
+  fields:
+    ReconFilterSize: required
+
 BloodRecording:
   selectors:
     - modality == "pet"
     - suffix == "blood"
   fields:
     PlasmaAvail: required
     MetaboliteAvail: required
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/eeg.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/eeg.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     sampling_frequency: optional
     reference__eeg: optional
     low_cutoff: optional
     high_cutoff: optional
     notch: optional
     status: optional
     status_description: optional
+  index_columns: [name__channels]
   additional_columns: allowed_if_defined
 
 EEGElectrodes:
   selectors:
     - datatype == "eeg"
     - suffix == "electrodes"
     - extension == ".tsv"
@@ -36,8 +37,9 @@
     name__electrodes: required
     x: required
     y: required
     z: required
     type__electrodes: recommended
     material: recommended
     impedance: recommended
+  index_columns: [name__electrodes]
   additional_columns: allowed_if_defined
```

### Comparing `bidsschematools-0.5.1/bidsschematools/data/schema/rules/tabular_data/meg.yaml` & `bidsschematools-0.6.0/bidsschematools/data/schema/rules/tabular_data/meg.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,9 @@
     sampling_frequency: optional
     low_cutoff: optional
     high_cutoff: optional
     notch: optional
     software_filters: optional
     status: optional
     status_description: optional
+  index_columns: [name__channels]
   additional_columns: allowed_if_defined
```

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/conftest.py` & `bidsschematools-0.6.0/bidsschematools/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/README.md` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/README.md`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asl.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_headshape.jpg` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_headshape.jpg`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_asl003/sub-Sub1/perf/sub-Sub1_m0scan.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/dataset_description.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/dataset_description.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-01_ses-01_T1w.nii`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-02_ses-01_T1w.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/anat/sub-02_ses-01_T1w.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-autosampler_blood.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-error-examples/invalid_pet001/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/CONTRIBUTING.md` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/CONTRIBUTING.md`

 * *Files 21% similar despite different names*

```diff
@@ -45,7 +45,22 @@
 - [optional] ... use `-name` with wildcard `*` to match to particular file types
 - ... for each file, execute something
 - ... namely, truncate the file
 - ... to size 0
 - `{}` is where a file name is put automatically (do not modify it)
 - `+` means, this is performed not file-wise but with a bunch of files at once.
   Could also be `\;` to have it one after the other
+
+## How to make a release
+
+We release `bids-examples` in sync with `bids-specification`.
+
+1. Make sure your local repository is up to date: `git fetch upstream`
+   (this assumes you have the `bids-standard/bids-examples` repository
+    configured as a git remote called "upstream")
+1. Tag the `master` branch: `git tag -a -m "X.X.X" X.X.X upstream/master`
+   (replace `X.X.X` with the version to be released)
+1. Push the tag upstream: `git push upstream X.X.X`
+1. Create a GitHub release using the new tag. Fill the title of the release
+   with the name of the tag. Fill the description of the release with a sentence like
+   > "Microscopy" BEP was merged into BIDS-specification (2022-02-15).
+1. You are done!
```

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/README.md` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 - [EEG datasets](#eeg-datasets)
 - [iEEG datasets](#ieeg-datasets)
 - [MRI datasets](#mri-datasets)
 - [ASL datasets](#asl-datasets)
 - [qMRI datasets](#qmri-datasets)
 - [PET datasets](#PET-datasets)
 - [Microscopy datasets](#microscopy-datasets)
-- [fNIRS datasets](#fnirs-datasets)
+- [NIRS datasets](#nirs-datasets)
 - [Multimodal datasets](#multimodal-datasets)
 
 ### EEG datasets
 
 | name                | maintained by | description                                                                                                        | link to full data                       |
 | ------------------- | ------------- | ------------------------------------------------------------------------------------------------------------------ | --------------------------------------- |
 | eeg_matchingpennies | @sappelhoff   | Offline data of BCI experiment decoding left vs. right hand movement. BrainVision data format (.eeg, .vhdr, .vmrk) | https://doi.org/10.17605/OSF.IO/CJ2DR   |
@@ -214,15 +214,15 @@
 | name          | maintained by | description                                                                                     |
 | ------------- | ------------- | ----------------------------------------------------------------------------------------------- |
 | micr_SEM      | @jcohenadad   | Example SEM dataset in PNG format with 1 sample imaged over 2 sessions                          |
 | micr_SEMzarr  | @TheChymera   | Example SEM dataset in PNG and OME-ZARR format with 1 sample imaged over 2 sessions             |
 | micr_SPIM     | @jcohenadad   | Example SPIM dataset in OME-TIFF format with 2 samples from the same subject with 4 chunks each |
 
 
-### fNIRS datasets
+### NIRS datasets
 
 | name              | maintained by     | description                                                             | link to full data                       |
 | ----------------- | ----------------- | ----------------------------------------------------------------------- | --------------------------------------- |
 | fnirs_tapping     | @rob_luke         | Example fNIRS measurement with three conditions from five subjects      | https://doi.org/10.5281/zenodo.5529797  |
 | fnirs_automaticiy | @robertoostenveld | 24 subjects performing (non-)automatic finger tapping and foot stepping | https://doi.org/10.34973/vesb-mh30      |
```

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asl.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_asllabeling.jpg`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/asl003/sub-Sub1/perf/sub-Sub1_m0scan.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm001/eeg/sub-cbm001_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm002/eeg/sub-cbm002_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm003/eeg/sub-cbm003_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm004/eeg/sub-cbm004_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm005/eeg/sub-cbm005_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm006/eeg/sub-cbm006_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm007/eeg/sub-cbm007_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm008/eeg/sub-cbm008_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm009/eeg/sub-cbm009_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm010/eeg/sub-cbm010_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm011/eeg/sub-cbm011_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm012/eeg/sub-cbm012_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm013/eeg/sub-cbm013_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm014/eeg/sub-cbm014_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm015/eeg/sub-cbm015_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm016/eeg/sub-cbm016_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm017/eeg/sub-cbm017_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm018/eeg/sub-cbm018_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm019/eeg/sub-cbm019_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_channels.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_channels.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_events.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/eeg_cbm/sub-cbm020/eeg/sub-cbm020_task-protmap_events.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SEMzarr/participants.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/README` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/README`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.ome.tif` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-01_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.ome.tif` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-02_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.ome.tif` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-03_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.ome.tif` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-A_stain-LFB_chunk-04_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.ome.tif` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-01_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.ome.tif` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-02_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.ome.tif` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-03_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.ome.tif` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/micr_SPIM/sub-01/micr/sub-01_sample-B_stain-LFB_chunk-04_SPIM.ome.tif`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/dataset_description.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/dataset_description.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_pet.nii.gz`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/pet003/sub-01/ses-01/pet/sub-01_ses-01_recording-manual_blood.tsv`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/dataset_description.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/dataset_description.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_M0map.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/anat/sub-01_T1map.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.json` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/qmri_vfa/derivatives/qMRLab/sub-01/fmap/sub-01_TB1map.json`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/bids-examples/run_tests.sh` & `bidsschematools-0.6.0/bidsschematools/tests/data/bids-examples/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/data/expected_bids_validator_xs_write.log` & `bidsschematools-0.6.0/bidsschematools/tests/data/expected_bids_validator_xs_write.log`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/test_make_testdata.py` & `bidsschematools-0.6.0/bidsschematools/tests/test_make_testdata.py`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/test_rules.py` & `bidsschematools-0.6.0/bidsschematools/tests/test_rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,34 +42,37 @@
     Additionally, this test only checks rules that fit the keys.
     """
     OBJECT_TYPE_MAPPER = {
         "metadata": "fields",  # metadata in objects is referred to as fields in rules
     }
 
     not_found = []  # A list of undefined, but referenced, objects
-    object_types = list(schema_obj["objects"].keys())
-    for object_type in object_types:
+    for object_type in schema_obj.objects:
+        # "files" is both an object name and a grouping of rules
+        # The next line would be a false positive hit
+        if object_type == "files":
+            continue
         # Find all uses of a given object type in the schema rules
         type_instances_in_rules = _dict_key_lookup(
-            schema_obj["rules"],
+            schema_obj.rules,
             OBJECT_TYPE_MAPPER.get(object_type, object_type),
         )
         if not type_instances_in_rules:
             continue
 
         for type_instance in type_instances_in_rules:
             path, instance = type_instance
             is_list = True
             if isinstance(instance, Mapping):
                 instance = list(instance)
                 is_list = False
 
             for i_use, use in enumerate(instance):
                 if use == "derivatives":
-                    # Skip derivatives folders, because the folder is treated as a "use" instead.
+                    # Skip derivatives dirs, because the dir is treated as a "use" instead.
                     continue
                 elif "[]" in use:
                     # Rules may reference metadata fields with lists.
                     # This test can't handle this yet, so skip.
                     continue
                 elif "{}" in use:
                     # Rules may reference sub-dictionaries in metadata fields.
@@ -102,35 +105,27 @@
 @pytest.mark.validate_schema
 def test_entity_order(schema_obj):
     """Check the order of the entities of the suffix group of each datatype
     and lists those that are out of order.
     """
     status_ok = True
 
-    entities_order = schema_obj["rules"]["entities"]
-    datatypes_schema_obj = schema_obj["rules"]["datatypes"]
-
-    for datatype, datatype_schema_obj in datatypes_schema_obj.items():
-
-        print(f"Checking: {datatype}")
-        # Skip over derivatives folders nested in regular folders
-        if datatype == "derivatives":
-            continue
+    entities_order = schema_obj.rules.entities
 
-        for suffix_group, suffix_group_obj in datatype_schema_obj.items():
-            entities = list(suffix_group_obj["entities"].keys())
-            correct_order = sorted(entities, key=lambda x: entities_order.index(x))
-
-            if entities != correct_order:
-                status_ok = False
-                warnings.warn(
-                    f"""
-                \nsuffix group {suffix_group} in {datatype} is out of order:
+    for key, group in schema_obj.rules.files.items(level=2):
+        print(f"Checking {key}")
+        entities = list(group.get("entities", ()))
+        correct_order = sorted(entities, key=lambda x: entities_order.index(x))
+
+        if entities != correct_order:
+            status_ok = False
+            warnings.warn(
+                f"""\n\nfilename rule {key} has entities out-of-order:
                 - got: {entities}
                 - should be: {correct_order}
                 """
-                )
+            )
 
     if not status_ok:
         raise RuntimeError(
             "Some suffix groups have their entities out of order. See warnings above."
         )
```

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/test_schema.py` & `bidsschematools-0.6.0/bidsschematools/tests/test_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests for the bidsschematools package."""
 import os
 from collections.abc import Mapping
 
 import pytest
 
-from bidsschematools import __bids_version__, schema
+from bidsschematools import __bids_version__, schema, types
 
 
 def test__get_bids_version(tmp_path):
     # Is the version being read in correctly?
     schema_path = os.path.join(
         os.path.abspath(os.path.dirname(__file__)),
         os.pardir,
@@ -37,14 +37,17 @@
     with pytest.raises(FileNotFoundError):
         schema.load_schema(bad_path)
 
     # Otherwise the function should return a dictionary
     schema_obj = schema.load_schema(schema_dir)
     assert isinstance(schema_obj, Mapping)
 
+    # Check that it is fully dereferenced
+    assert "$ref" not in str(schema_obj)
+
 
 def test_object_definitions(schema_obj):
     """Ensure that object definitions in the schema contain required fields."""
     for obj_type, obj_type_def in schema_obj["objects"].items():
         for obj_key, obj_def in obj_type_def.items():
             # Private/inheritable definitions (ones starting with "_") do not need to conform to
             # the same rules as user-facing terms, so we skip them
@@ -182,15 +185,15 @@
             "Property2": "value2",
         },
         "ReferencingObject": {
             "$ref": "ReferencedObject",
             "Property2": "value4",
         },
     }
-    dereffed = schema.dereference_mapping(orig, orig.copy())
+    dereffed = schema.dereference(orig)
     assert dereffed == {
         "ReferencedObject": {
             "Property1": "value1",
             "Property2": "value2",
         },
         "ReferencingObject": {
             "Property1": "value1",
@@ -216,17 +219,16 @@
                 "$ref": "raw.func.entities",
                 "space": "optional",
                 "desc": "optional",
             },
         },
     }
 
-    sch = schema.Namespace.build(orig)
-    expanded = schema.expand(orig)
-    dereffed = schema.dereference_mapping(sch, expanded)
+    sch = types.Namespace.build(orig)
+    dereffed = schema.dereference(sch)
     assert dereffed == {
         "raw": {
             "func": {
                 "suffix": ["bold", "cbv"],
                 "extensions": [".nii", ".nii.gz"],
                 "datatype": ["func"],
                 "entities": {
@@ -274,17 +276,16 @@
             "$ref": "raw.func",
             "entities": {
                 "$ref": "_DERIV_ENTS",
             },
         },
     }
 
-    sch = schema.Namespace.build(orig)
-    expanded = schema.expand(orig)
-    dereffed = schema.dereference_mapping(sch, expanded)
+    sch = types.Namespace.build(orig)
+    dereffed = schema.dereference(sch)
     assert dereffed == {
         "_DERIV_ENTS": {
             "space": "optional",
             "desc": "optional",
         },
         "raw": {
             "func": {
```

### Comparing `bidsschematools-0.5.1/bidsschematools/tests/test_utils.py` & `bidsschematools-0.6.0/bidsschematools/tests/test_render_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from bidsschematools import utils
+from bidsschematools.render import utils
 
 
 def test_combine_extensions():
     """A unit test for utils.combine_extensions."""
     test_extensions = ["nii.gz", "nii", "json"]
     target_combined = ["nii[.gz]", "json"]
     test_combined = utils.combine_extensions(test_extensions, pdf_format=True)
```

### Comparing `bidsschematools-0.5.1/bidsschematools/utils.py` & `bidsschematools-0.6.0/bidsschematools/render/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,10 @@
-"""Utility functions for the bids-specification schema."""
-import logging
+"""Utility functions for specification rendering tools."""
 import math
-import os.path as op
-from pprint import pprint
-
-
-def get_schema_path():
-    """Get the path to the schema directory.
-
-    Returns
-    -------
-    str
-        Absolute path to the directory containing schema-related files.
-    """
-    return op.abspath(op.join(op.dirname(__file__), "data", "schema"))
+import posixpath
 
 
 def _link_with_html(string, html_path=None, heading=None, pdf_format=False):
     """Wrap a string in an HTML hyperlink.
 
     Parameters
     ----------
@@ -101,15 +88,14 @@
                     pdf_format=pdf_format,
                 )
 
                 temp_item = temp_item + "[" + ext_string + "]"
                 new_lst.append(temp_item)
                 items_to_remove.append(item)
                 items_to_remove.append(item.replace(ext, ""))
-                continue
 
     heading_lst = [head for i, head in enumerate(heading_lst) if lst[i] not in items_to_remove]
     items_to_add = [item for item in lst if item not in items_to_remove]
     item_strings_to_add = []
     for i_item, item in enumerate(items_to_add):
         item_strings_to_add.append(
             _link_with_html(
@@ -121,52 +107,14 @@
         )
 
     new_lst += item_strings_to_add
 
     return new_lst
 
 
-def get_logger(name=None):
-    """Return a logger to use.
-
-    Parameters
-    ----------
-    name : None or str, optional
-        Name of the logger. Defaults to None.
-
-    Returns
-    -------
-    logging.Logger
-        logger object.
-    """
-    return logging.getLogger("bids-schema" + (".%s" % name if name else ""))
-
-
-def set_logger_level(lgr, level):
-    """Set the logger level.
-
-    Parameters
-    ----------
-    lgr : logging.Logger
-        logger object for which to change the level.
-    level : int or str
-        The desired level for the logger.
-    """
-    if isinstance(level, int):
-        pass
-    elif level.isnumeric():
-        level = int(level)
-    elif level.isalpha():
-        level = getattr(logging, level)
-    else:
-        lgr.warning("Do not know how to treat loglevel %s" % level)
-        return
-    lgr.setLevel(level)
-
-
 def drop_unused_entities(df):
     """Remove columns from a dataframe where all values in the column are NaNs.
 
     For entity tables, this limits each table to only entities that are used
     within the modality.
 
     Parameters
@@ -203,15 +151,14 @@
     """
     # Flatten multi-index
     vals = df.index.tolist()
     df.loc["Format"] = df.columns.get_level_values(1)
     df.columns = df.columns.get_level_values(0)
     df = df.loc[["Format"] + vals]
     df.index.name = "Entity"
-    df = df.drop(columns=["DataType"])
     return df
 
 
 def get_link(string):
     refs = {
         "array": "https://www.w3schools.com/js/js_json_arrays.asp",
         "string": "https://www.w3schools.com/js/js_json_datatypes.asp",
@@ -259,18 +206,17 @@
     elif "anyOf" in definition:
         # Use dictionary to get unique substrings while preserving insertion order
         substrings = {resolve_metadata_type(subdict): None for subdict in definition["anyOf"]}
 
         string = " or ".join(substrings)
 
     else:
-        # A hack to deal with $ref in the current schema
-        print(f"Type could not be inferred for {definition['name']}")
-        pprint(definition)
-        string = "unknown"
+        # This clause should only catch $refs.
+        # The schema should be deferenced by this point, so $refs should not exist.
+        raise ValueError(f"Type could not be inferred for {definition['name']}")
 
     return string
 
 
 def describe_valid_values(definition):
     """Build a sentence describing valid values for an object from its definition.
 
@@ -300,36 +246,109 @@
             enum_values = [
                 list(v.keys())[0] if isinstance(v, dict) else v for v in definition["enum"]
             ]
             enum_values = [f'`"{v}"`' for v in enum_values]
             description = f"Must be one of: {', '.join(enum_values)}."
 
     elif definition["type"] in ("integer", "number"):
+        minstr = maxstr = minmaxstr = ""
+
         if "minimum" in definition.keys():
             minstr = f"greater than or equal to {definition['minimum']}"
         elif "exclusiveMinimum" in definition.keys():
             minstr = f"greater than {definition['exclusiveMinimum']}"
-        else:
-            minstr = ""
 
         if "maximum" in definition.keys():
             maxstr = f"less than or equal to {definition['maximum']}"
         elif "exclusiveMaximum" in definition.keys():
             maxstr = f"less than {definition['exclusiveMaximum']}"
-        else:
-            maxstr = ""
 
         if minstr and maxstr:
             minmaxstr = f"{minstr} and {maxstr}"
-        elif minstr:
-            minmaxstr = minstr
-        elif maxstr:
-            minmaxstr = maxstr
-        else:
-            minmaxstr = ""
+        elif minstr or maxstr:
+            minmaxstr = minstr + maxstr
 
         if minmaxstr:
             description = f"Must be a number {minmaxstr}."
-        else:
-            description = ""
 
     return description
+
+
+def get_relpath(src_path):
+    """Retrieve relative path to the source root from the perspective of a Markdown file.
+
+    As a convenience, ``None`` is interpreted as the empty string, and a value of ``'.'``
+    is returned.
+
+    Examples
+    --------
+    >>> get_relpath("02-common-principles.md")
+    '.'
+    >>> get_relpath("04-modality-specific-files/01-magnetic-resonance-imaging-data.md")
+    '..'
+    >>> get_relpath("we/lack/third_levels.md")
+    '../..'
+    >>> get_relpath(None)
+    '.'
+    """
+    return posixpath.relpath(".", posixpath.dirname(src_path or ""))
+
+
+def normalize_requirements(text):
+    for level in ("optional", "recommended", "required", "deprecated"):
+        # Replace both "optional" and "Optional" with "OPTIONAL"
+        text = text.replace(level.title(), level).replace(level, level.upper())
+    return text
+
+
+def normalize_breaks(text):
+    # A backslash before a newline means continue a string
+    text = text.replace("\\\n", "")
+    # Two newlines should be respected
+    text = text.replace("\n\n", "<br>")
+    # Otherwise a newline corresponds to a space
+    return text.replace("\n", " ")
+
+
+def num2words(integer, to="ordinal"):
+    """Convert integers to words.
+
+    This is a very simplistic mapping of numbers to words,
+    to avoid adding num2words to our requirements.
+    It only works with the first few numbers.
+
+    Parameters
+    ----------
+    integer : int
+    to : {"ordinal", "cardinal"}, optional
+    """
+    if to == "ordinal":
+        mapper = {
+            1: "first",
+            2: "second",
+            3: "third",
+            4: "fourth",
+            5: "fifth",
+            6: "sixth",
+            7: "seventh",
+            8: "eighth",
+            9: "ninth",
+            10: "tenth",
+        }
+    elif to == "cardinal":
+        mapper = {
+            1: "one",
+            2: "two",
+            3: "three",
+            4: "four",
+            5: "five",
+            6: "six",
+            7: "seven",
+            8: "eight",
+            9: "nine",
+            10: "ten",
+        }
+
+    try:
+        return mapper[integer]
+    except KeyError:
+        raise ValueError(f"Input {integer} is not supported.")
```

### Comparing `bidsschematools-0.5.1/bidsschematools/validator.py` & `bidsschematools-0.6.0/bidsschematools/validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import datetime
 import json
 import os
 import re
+import typing as ty
+from collections.abc import Mapping
 from copy import deepcopy
 from functools import lru_cache
 from pathlib import Path
 
-from . import schema, utils
+import bidsschematools as bst
+import bidsschematools.schema
+import bidsschematools.types
+import bidsschematools.utils
 
-lgr = utils.get_logger()
+lgr = bst.utils.get_logger()
 
 # The list of which entities create directories could be dynamically specified by the YAML, but for
 # now, it is not.
 # Ordering is important, as "subject" follows "session" alphabetically, but is hierarchically
 # above it.
 DIR_ENTITIES = ["subject", "session"]
 
@@ -38,25 +43,19 @@
 
     Notes
     -----
     * Figure out how to return paths from BIDS root.
     * Deduplicate paths (if input dirs are subsets of other input dirs), might best be done at the
         very end.
     """
-    exclude_subdirs = [
-        rf"{os.sep}.dandi",
-        rf"{os.sep}.datalad",
-        rf"{os.sep}.git",
-    ]
     # `.bidsignore` is not, in fact, a BIDS file, as per:
     # https://github.com/bids-standard/bids-specification/issues/980
+    # Perhaps this should be parameterized for downstream flexibility and not having to keep track
+    # of downstream nuisance files here.
     exclude_files = [
-        ".gitattributes",
-        ".gitignore",
-        ".bidsignore",
         "dandiset.yaml",
     ]
 
     path_list = []
     bids_root_found = False
     for bids_path in bids_paths:
         if not accept_dummy_paths:
@@ -72,18 +71,18 @@
                 if root.endswith(tuple(pseudofile_suffixes)):
                     # Add the directory name to the validation paths list.
                     path_list.append(Path(root).as_posix() + "/")
                     # Do not index the contents of the directory.
                     dirs[:] = []
                     file_names[:] = []
                 # will break if BIDS ever puts meaningful data under `/.{dandi,datalad,git}*/`
-                if os.path.basename(root) in exclude_subdirs:
+                if os.path.basename(root).startswith("."):
                     continue
                 for file_name in file_names:
-                    if file_name in exclude_files:
+                    if file_name in exclude_files or file_name.startswith("."):
                         continue
                     file_path = os.path.join(root, file_name)
                     # This will need to be replaced with bids root finding.
                     path_list.append(Path(file_path).as_posix())
         elif os.path.isfile(bids_path) or accept_dummy_paths:
             path_list.append(Path(bids_path).as_posix())
         else:
@@ -92,265 +91,206 @@
                 "intended for path validation which does not correspond to an actual "
                 "path, please set the `accept_dummy_paths` parameter to True."
             )
 
     return path_list
 
 
-def _add_entity(regex_entities, entity, entity_shorthand, variable_field, requirement_level):
-    """Add entity pattern to filename template based on requirement level."""
-
-    # We need to do this here, although it would be easier to back-reference in the directory.
-    # This is because regex evaluates sequentially and we can not forward-reference a group.
-    if entity in DIR_ENTITIES:
-        variable_regex = f"(?P={entity})"
-    else:
-        variable_regex = f"(?P<{entity}>{variable_field})"
-
-    if requirement_level == "required":
-        if len(regex_entities.strip()):
-            regex_entities += f"_{entity_shorthand}-{variable_regex}"
-        else:
-            # Only the first entity doesn't need an underscore
-            regex_entities += f"{entity_shorthand}-{variable_regex}"
-    else:
-        if len(regex_entities.strip()):
-            regex_entities += f"(|_{entity_shorthand}-{variable_regex})"
-        else:
-            # Only the first entity doesn't need an underscore
-            regex_entities += f"(|{entity_shorthand}-{variable_regex})"
-
-    return regex_entities
+def _capture_regex(name, pattern, backref):
+    """Capture pattern to name or match back-reference to name
 
-
-def _extension_safety(extension):
+    >>> _capture_regex("run", "[0-9]+", False)
+    '(?P<run>[0-9]+)'
+    >>> _capture_regex("run", "[0-9]+", True)
+    '(?P=run)'
+    >>> re.match(_capture_regex("run", "[0-9]+", False), "123_").groupdict()
+    {'run': '123'}
+    """
+    return f"(?P={name})" if backref else f"(?P<{name}>{pattern})"
+
+
+def _optional_regex(regex, optional):
+    """Return an optional version of a regex if optional is True
+
+    A required regex is passed through unchanged:
+
+    >>> pattern = _optional_regex("xyz", False)
+    >>> pattern
+    'xyz'
+    >>> re.match(pattern, "xyz").groups()
+    ()
+    >>> re.match(pattern, "") is None
+    True
+
+    An optional regex uses a non-capturing group, to avoid interfering
+    with existing groups
+
+    >>> pattern = _optional_regex("x(?P<name>[a-z])z", True)
+    >>> pattern
+    '(?:x(?P<name>[a-z])z)?'
+    >>> re.match(pattern, "xyz").groups()
+    ('y',)
+    >>> re.match(pattern, "xyz").groupdict()
+    {'name': 'y'}
+    >>> re.match(pattern, "").groups()
+    (None,)
+    >>> re.match(pattern, "").groupdict()
+    {'name': None}
     """
-    Making extensions formatting-safe.
-    Issues covered by this function are listed under “Notes”
-
-    Parameters
-    ----------
-    extension : str
-        Extension string, as present in the BIDS YAML schema.
+    return f"(?:{regex})?" if optional else regex
 
-    Returns
-    -------
-    str
-        Extension string, safe for use in validator Regex formatting.
 
-    Notes
-    -----
-    * Bash-wildcard safety: https://github.com/bids-standard/bids-specification/issues/990
-    * Period safety: https://github.com/bids-standard/bids-specification/issues/1055
-    * Hopefully this function will be deprecated soon, but it will not break safe entries.
-    """
-    if extension == "None":
+@lru_cache()
+def _format_entity(entity, name, pattern, level, directory=False):
+    if directory and entity not in DIR_ENTITIES:
         return ""
-    if "." in extension:
-        extension = extension.replace(".", "\\.")
-    if "*" in extension:
-        extension = extension.replace("*", ".*?")
-
-    return extension
-
-
-def _add_extensions(regex_string, variant):
-    """Add extensions to a regex string."""
-    fixed_variant_extensions = []
-    for variant_extension in variant["extensions"]:
-        variant_extension = _extension_safety(variant_extension)
-        fixed_variant_extensions.append(variant_extension)
-    if len(fixed_variant_extensions) > 1:
-        regex_extensions = "({})".format("|".join(fixed_variant_extensions))
-    else:
-        regex_extensions = fixed_variant_extensions[0]
-    regex_string = f"{regex_string}{regex_extensions}"
 
-    return regex_string
+    label = _capture_regex(entity, pattern, not directory and entity in DIR_ENTITIES)
+    post = "/" if directory else "_"
 
+    return _optional_regex(f"{name}-{label}{post}", level != "required")
 
-def _add_subdirs(regex_string, variant, datatype, entity_definitions, formats, modality_datatypes):
-    """Add appropriate subdirectories as required by entities present."""
 
-    regex_dirs = "/"
-    for dir_entity in DIR_ENTITIES:
-        if dir_entity in variant["entities"].keys():
-            format_selection = formats[entity_definitions[dir_entity]["format"]]
-            variable_field = format_selection["pattern"]
-            shorthand = entity_definitions[dir_entity]["name"]
-            if variant["entities"][dir_entity] == "required":
-                regex_subdir = f"{shorthand}-(?P<{dir_entity}>{variable_field})/"
-            else:
-                regex_subdir = f"(|{shorthand}-(?P<{dir_entity}>{variable_field})/)"
-            regex_dirs = f"{regex_dirs}{regex_subdir}"
-    if datatype in modality_datatypes:
-        regex_dirs = f"{regex_dirs}{datatype}/"
-    regex_string = f"{regex_dirs}{regex_string}"
-
-    return regex_string
+def split_inheritance_rules(rule: Mapping) -> ty.List[Mapping]:
+    """Break composite rules into main and sidecar rules
 
+    Implements the inheritance principle for file naming.
+    """
+    heritable_exts = {".tsv", ".json", ".bval", ".bvec"}
+    rule_exts = set(rule["extensions"])
+
+    main_exts = rule_exts - heritable_exts
+    # If a rule only has TSV or JSON files, entities can be
+    # made required
+    if not main_exts:
+        if ".tsv" in rule_exts:
+            main_exts = {".tsv"}
+        elif ".json" in rule_exts:
+            main_exts = {".json"}
+
+    sidecar_exts = rule_exts - main_exts
+    if not sidecar_exts:
+        return [rule]
+
+    sidecar_dtypes = [""] + rule.get("datatypes", [])
+    sidecar_entities = {ent: "optional" for ent in rule.get("entities")}
+
+    main_rule = {**rule, **{"extensions": list(main_exts)}}
+    sidecar_rule = {
+        **rule,
+        **{
+            "extensions": list(sidecar_exts),
+            "datatypes": sidecar_dtypes,
+            "entities": sidecar_entities,
+        },
+    }
 
-def _add_suffixes(regex_string, variant):
-    """Add suffixes to a regex string."""
-    if len(variant["suffixes"]) == 1:
-        regex_suffixes = variant["suffixes"][0]
-    else:
-        regex_suffixes = "({})".format("|".join(variant["suffixes"]))
-    regex_string = f"{regex_string}_{regex_suffixes}"
+    return [main_rule, sidecar_rule]
 
-    return regex_string
 
+def _path_rule(rule: bst.types.Namespace):
+    return {"regex": re.escape(rule.path), "mandatory": rule.level == "required"}
 
-def load_top_level(
-    my_schema,
-):
-    """
-    Create full path regexes for top level files, as documented by a target BIDS YAML schema
-    version.
 
+def _sanitize_extension(ext: str) -> str:
+    if ext == ".*":
+        return r"\.[a-zA-Z0-9.]+"
+    return re.escape(ext)
 
-    Parameters
-    ----------
-    my_schema : dict
-        A nested dictionary, as returned by `bidsschematools.schema.load_schema()`.
 
-    Returns
-    -------
-    regex_schema : list of dict
-        A list of dictionaries, with keys including 'regex' and 'mandatory'.
-    """
+def _stem_rule(rule: bst.types.Namespace):
+    stem_regex = re.escape(rule.stem)
+    ext_match = "|".join(_sanitize_extension(ext) for ext in rule.extensions)
+    ext_regex = f"(?P<extension>{ext_match})"
 
-    top_level_files = my_schema["rules"]["top_level_files"]
+    return {"regex": stem_regex + ext_regex, "mandatory": rule.level == "required"}
 
-    regex_schema = []
-    for top_level_filename in top_level_files.keys():
-        top_level_file = top_level_files[top_level_filename]
-        # None value gets passed as list of strings...
-        extensions = top_level_file["extensions"]
-        if extensions != ["None"]:
-            extensions_regex = "|".join(map(_extension_safety, extensions))
-            regex = f".*?/{top_level_filename}({extensions_regex})$"
+
+def _entity_rule(rule: Mapping, schema: bst.types.Namespace):
+    dir_regex = []
+    entity_regex = []
+    for ent in schema.rules.entities:
+        if ent not in rule["entities"]:
+            continue
+        ent_obj = rule["entities"][ent]
+        if isinstance(ent_obj, str):
+            ent_obj = {"level": ent_obj}
+        # Allow filename rule to override original entity fields
+        entity = {**schema.objects.entities[ent], **ent_obj}
+
+        if "enum" in entity:
+            pattern = "|".join(entity["enum"])
         else:
-            regex = f".*?/{top_level_filename}$"
-        regex_entry = {
-            "regex": regex,
-            "mandatory": top_level_file["required"],
-        }
-        regex_schema.append(regex_entry)
+            pattern = schema.objects.formats[entity["format"]].pattern
 
-    return regex_schema
+        dir_regex.append(
+            _format_entity(ent, entity["name"], pattern, entity["level"], directory=True)
+        )
+        entity_regex.append(_format_entity(ent, entity["name"], pattern, entity["level"]))
+
+    dtypes = set(rule.get("datatypes", ()))
+    optional_dtype = "" in dtypes
+    if optional_dtype:
+        dtypes.remove("")
+    if dtypes:
+        pattern = f"(?P<datatype>{'|'.join(dtypes)})/"
+        if optional_dtype:
+            pattern = f"(?:{pattern})?"
+        dir_regex += pattern
+
+    # If we move to referring to suffixes by keys in the object table:
+    # suffixes = [schema.objects.suffixes[suffix].value for suffix in rule["suffixes"]]
+    suffixes = rule["suffixes"]
+    suffix_regex = f"(?P<suffix>{'|'.join(suffixes)})"
+
+    # If we move to referring to extensions by keys in the object table:
+    # extensions = [schema.objects.extensions[ext].value for ext in rule["extensions"]]
+    extensions = rule["extensions"]
+    ext_match = "|".join(_sanitize_extension(ext) for ext in extensions)
+    ext_regex = f"(?P<extension>{ext_match})"
+
+    return {
+        "regex": "".join(dir_regex + entity_regex + [suffix_regex, ext_regex]),
+        "mandatory": False,
+    }
 
 
-def load_entities(
-    my_schema,
-    inheritance_regex=r".*?\\\.(tsv|bvec|json)(\$|\||\)).*?",
+def load_filename_rules(
+    rule_group: bst.types.Namespace,
+    schema: bst.types.Namespace,
+    level: int,
 ):
-    """Create full path regexes for entities, as documented by a target BIDS YAML schema version.
+    """Load schema rules into regular expressions
 
     Parameters
     ----------
-    my_schema : dict
+    rule_group : Namespace
+        The set of rules to load from the schema
+    schema : Namespace
         A nested dictionary, as returned by `bidsschematools.schema.load_schema()`.
-    inheritance_regex : str, optional
-        Valid regex string identifying filenames to which inheritance expansion should be applied.
-
-    Notes
-    -----
-
-    * Suggest to BIDS-specification to remove the periods from the extensions, the leading period
-        is not part of the extension, but a delimiter defining the fact that it's an extension.
-        Code sections marked as `Making it period-safe` should be edited when this fix is in,
-        though they will work in any case.
-        https://github.com/bids-standard/bids-specification/issues/990
-    * More issues in comments.
+    level : int
+        The depth in rule_group to look for rules
 
     Returns
     -------
-    regex_schema : list of dict
+    rules : list of dict
         A list of dictionaries, with keys including 'regex' and 'mandatory'.
     """
-
-    # Parsing tabular_metadata as a datatype, might be done automatically if the YAML is moved
-    # to the same subdirectory
-    datatypes = {
-        "tabular_metadata": my_schema.rules.tabular_metadata,
-        **my_schema.rules.datatypes,
-    }
-    entity_order = my_schema["rules"]["entities"]
-    entity_definitions = my_schema["objects"]["entities"]
-    formats = my_schema["objects"]["formats"]
-
-    # # Descriptions are not needed and very large.
-    # for i in entity_definitions.values():
-    #     i.pop("description", None)
-
-    # Needed for non-modality file separation as per:
-    # https://github.com/bids-standard/bids-specification/pull/985#issuecomment-1019573787
-    modalities = my_schema["rules"]["modalities"]
-    modality_datatypes = []
-    for modality_key in modalities.keys():
-        for modality_datatype in modalities[modality_key]["datatypes"]:
-            modality_datatypes.append(modality_datatype)
-
     regex_schema = []
-    for datatype in datatypes:
-        if datatype == "derivatives":
-            continue
-        for variant in datatypes[datatype].values():
-            regex_entities = ""
-            for entity in entity_order:
-                # Slightly awkward construction to account for new-style file specification.
-                # As in:
-                # https://github.com/bids-standard/bids-specification/pull/987
-                try:
-                    if entity in variant["entities"]:
-                        entity_shorthand = entity_definitions[entity]["name"]
-                        if "enum" in entity_definitions[entity].keys():
-                            # Entity key-value pattern with specific allowed values
-                            # tested, works!
-                            variable_field = "|".join(entity_definitions[entity]["enum"])
-                        else:
-                            format_selection = formats[entity_definitions[entity]["format"]]
-                            variable_field = format_selection["pattern"]
-                        regex_entities = _add_entity(
-                            regex_entities,
-                            entity,
-                            entity_shorthand,
-                            variable_field,
-                            variant["entities"][entity],
-                        )
-                except KeyError:
-                    pass
-
-            regex_string = _add_suffixes(regex_entities, variant)
-            regex_string = _add_extensions(regex_string, variant)
-            regex_string = _add_subdirs(
-                regex_string,
-                variant,
-                datatype,
-                entity_definitions,
-                formats,
-                modality_datatypes,
+    for rule_template in rule_group.values(level=level):
+        # Simple rules, e.g. dataset_description.json, README
+        if "path" in rule_template:
+            regex_schema.append(_path_rule(rule_template))
+        elif "stem" in rule_template:
+            regex_schema.append(_stem_rule(rule_template))
+        else:
+            regex_schema.extend(
+                _entity_rule(rule, schema) for rule in split_inheritance_rules(rule_template)
             )
 
-            regex_string = f".*?{regex_string}$"
-            regex_entry = {
-                "regex": regex_string,
-                "mandatory": False,
-            }
-            regex_schema.append(regex_entry)
-            if re.match(inheritance_regex, regex_string):
-                expansion_list = _inheritance_expansion(regex_string, datatype)
-                for expansion in expansion_list:
-                    expansion_entry = {
-                        "regex": expansion,
-                        "mandatory": False,
-                    }
-                    regex_schema.append(expansion_entry)
-
     return regex_schema
 
 
 @lru_cache()
 def load_all(
     schema_dir,
 ):
@@ -362,28 +302,24 @@
     schema_dir : str, optional
         A string pointing to a BIDS directory for which paths should be validated.
 
     Returns
     -------
     all_regex : list of dict
         A list of dictionaries, with keys including 'regex' and 'mandatory'.
-    my_schema : list of dict
+    my_schema : Mapping
         Nested dictionaries representing the full schema.
     """
 
-    my_schema = schema.load_schema(schema_dir)
-    all_regex = load_entities(
-        my_schema=my_schema,
-    )
-    top_level_regex = load_top_level(
-        my_schema=my_schema,
-    )
-    all_regex.extend(top_level_regex)
+    schema = bst.schema.load_schema(schema_dir)
+    all_regex = []
+    for group in (schema.rules.files.common, schema.rules.files.raw):
+        all_regex.extend(load_filename_rules(group, schema, level=2))
 
-    return all_regex, my_schema
+    return all_regex, schema
 
 
 def validate_all(
     paths_list,
     regex_schema,
 ):
     """
@@ -422,15 +358,15 @@
     match_listing = []
     for target_path in paths_list:
         lgr.debug("Checking file `%s`.", target_path)
         lgr.debug("Trying file types:")
         for regex_entry in tracking_schema:
             target_regex = regex_entry["regex"]
             lgr.debug("\t* `%s`, with pattern: `%`", target_path, target_regex)
-            matched = re.match(target_regex, target_path)
+            matched = re.match(r"(?:.*/)?" + target_regex, target_path)
             itemwise_result = {}
             itemwise_result["path"] = target_path
             itemwise_result["regex"] = target_regex
             if matched:
                 lgr.debug("Match identified.")
                 itemwise_result["match"] = True
                 itemwise_results.append(itemwise_result)
@@ -699,80 +635,14 @@
                 "The `%s` regex pattern file required by BIDS was not found.",
                 entry["regex"],
             )
     for i in validation_result["path_tracking"]:
         lgr.warning("The `%s` file was not matched by any regex schema entry.", i)
 
 
-def _inheritance_expansion(
-    regex_string,
-    datatype=None,
-):
-    """
-    Generate regex strings applying BIDS inheritance expansion to an input string.
-
-    Parameters
-    ----------
-    regex_string : str
-        String representing the regex to which inheritance expansion should be applied.
-    datatype : str, optional
-        Datatype string to remove as part of inheritance expansion.
-
-    Returns
-    -------
-    expanded_regexes : list of str
-    """
-
-    # Order is important as the string is eroded.
-    # Session is eroded *together with* and *after* subject, as it is always optional
-    # and the erosion is:
-    #   * only required if a dangling leading underscore is present after subject removal.
-    #   * only BIDS-valid after the subject field is eroded from the filename.
-    expansions = [
-        {
-            "regex": [
-                r".*?(?P<remove>sub-\(\?P<subject>\[0\-9a\-zA\-Z\]\+\)/).*?",
-                r".*?(?P<remove>sub-\(\?P=subject\))",
-                r".*?/(?P<remove>\(\|ses-\(\?P<session>\[0\-9a\-zA\-Z\]\+\)/\)\(\|_ses-\("
-                r"\?P=session\)\)_).*?",
-            ],
-            "replace": ["", "", ""],
-        },
-    ]
-    if datatype:
-        # Inserting at the beginning, since datatype goes first.
-        expansions.insert(
-            0,
-            {
-                "regex": [
-                    f".*?(?P<remove>{datatype}/).*?",
-                ],
-                "replace": [
-                    "",
-                ],
-            },
-        )
-
-    expanded_regexes = []
-    lgr.debug("Applying inheritance expansion to:\n`%s`", regex_string)
-    for expansion in expansions:
-        modified = False
-        for ix, regex in enumerate(expansion["regex"]):
-            matched = re.match(regex, regex_string)
-            if matched:
-                matched = matched.groupdict()["remove"]
-                regex_string = regex_string.replace(matched, expansion["replace"][ix])
-                modified = True
-        if modified:
-            expanded_regexes.append(regex_string)
-            lgr.debug("\t* Generated expansion:\n\t%s", regex_string)
-
-    return expanded_regexes
-
-
 def _get_directory_suffixes(my_schema):
     """Query schema for suffixes which identify directory entities.
 
     Parameters
     ----------
     my_schema : dict
         Nested directory as produced by `bidsschematools.schema.load_schema()`.
@@ -841,18 +711,21 @@
         A dictionary reporting the target files for validation, the unmatched files and unmatched
         regexes, and optionally the itemwise comparison results.
         Keys include "schema_tracking", "path_tracking", "path_listing", "match_listing", and
         optionally "itemwise"
 
     Examples
     --------
-    >>> from bidsschematools import validator
-    >>> bids_paths = '~/.data2/datalad/000026/rawdata'
-    >>> schema_version='{module_path}/data/schema/'
-    >>> validator.validate_bids(bids_paths, schema_version=schema_version)"
+
+    ::
+
+        from bidsschematools import validator
+        bids_paths = '~/.data2/datalad/000026/rawdata'
+        schema_version='{module_path}/data/schema/'
+        validator.validate_bids(bids_paths, schema_version=schema_version)
 
     Notes
     -----
     * Needs to account for inheritance principle, probably somewhere deeper in the logic, might be
         as simple as pattern parsing and multiplying patterns to which inheritance applies.
         https://github.com/bids-standard/bids-specification/pull/969#issuecomment-1132119492
     """
@@ -875,15 +748,15 @@
     )
     validation_result = validate_all(
         bids_paths,
         regex_schema,
     )
 
     # Record schema version.
-    bids_version = schema._get_bids_version(bids_schema_dir)
+    bids_version = bst.schema._get_bids_version(bids_schema_dir)
     validation_result["bids_version"] = bids_version
 
     log_errors(validation_result)
 
     if report_path:
         if isinstance(report_path, str):
             write_report(validation_result, report_path=report_path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bidsschematools-0.5.1/bidsschematools.egg-info/PKG-INFO` & `bidsschematools-0.6.0/bidsschematools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bidsschematools
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python tools for working with the BIDS schema.
 Home-page: https://github.com/bids-standard/bids-specification
 Author: bids-standard developers
 Author-email: bids.maintenance@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bidsschematools-0.5.1/bidsschematools.egg-info/SOURCES.txt` & `bidsschematools-0.6.0/bidsschematools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,99 +1,110 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 bidsschematools/__init__.py
 bidsschematools/__main__.py
-bidsschematools/render.py
 bidsschematools/schema.py
 bidsschematools/utils.py
 bidsschematools/validator.py
 bidsschematools.egg-info/PKG-INFO
 bidsschematools.egg-info/SOURCES.txt
 bidsschematools.egg-info/dependency_links.txt
 bidsschematools.egg-info/entry_points.txt
 bidsschematools.egg-info/not-zip-safe
 bidsschematools.egg-info/requires.txt
 bidsschematools.egg-info/top_level.txt
 bidsschematools/data/__init__.py
 bidsschematools/data/schema/BIDS_VERSION
 bidsschematools/data/schema/SCHEMA_VERSION
 bidsschematools/data/schema/meta/context.yaml
-bidsschematools/data/schema/objects/associated_data.yaml
+bidsschematools/data/schema/meta/expression_tests.yaml
 bidsschematools/data/schema/objects/columns.yaml
 bidsschematools/data/schema/objects/common_principles.yaml
 bidsschematools/data/schema/objects/datatypes.yaml
 bidsschematools/data/schema/objects/entities.yaml
 bidsschematools/data/schema/objects/extensions.yaml
+bidsschematools/data/schema/objects/files.yaml
 bidsschematools/data/schema/objects/formats.yaml
 bidsschematools/data/schema/objects/metadata.yaml
 bidsschematools/data/schema/objects/modalities.yaml
 bidsschematools/data/schema/objects/suffixes.yaml
-bidsschematools/data/schema/objects/top_level_files.yaml
-bidsschematools/data/schema/rules/associated_data.yaml
-bidsschematools/data/schema/rules/common_derivatives_validation.yaml
 bidsschematools/data/schema/rules/common_principles.yaml
 bidsschematools/data/schema/rules/dataset_metadata.yaml
 bidsschematools/data/schema/rules/entities.yaml
 bidsschematools/data/schema/rules/errors.yaml
 bidsschematools/data/schema/rules/modalities.yaml
-bidsschematools/data/schema/rules/tabular_metadata.yaml
-bidsschematools/data/schema/rules/top_level_files.yaml
 bidsschematools/data/schema/rules/checks/asl.yaml
+bidsschematools/data/schema/rules/checks/common_derivatives.yaml
 bidsschematools/data/schema/rules/checks/dwi.yaml
 bidsschematools/data/schema/rules/checks/events.yaml
 bidsschematools/data/schema/rules/checks/fmap.yaml
 bidsschematools/data/schema/rules/checks/func.yaml
 bidsschematools/data/schema/rules/checks/hints.yaml
 bidsschematools/data/schema/rules/checks/mri.yaml
-bidsschematools/data/schema/rules/datatypes/anat.yaml
-bidsschematools/data/schema/rules/datatypes/beh.yaml
-bidsschematools/data/schema/rules/datatypes/dwi.yaml
-bidsschematools/data/schema/rules/datatypes/eeg.yaml
-bidsschematools/data/schema/rules/datatypes/fmap.yaml
-bidsschematools/data/schema/rules/datatypes/func.yaml
-bidsschematools/data/schema/rules/datatypes/ieeg.yaml
-bidsschematools/data/schema/rules/datatypes/meg.yaml
-bidsschematools/data/schema/rules/datatypes/micr.yaml
-bidsschematools/data/schema/rules/datatypes/perf.yaml
-bidsschematools/data/schema/rules/datatypes/pet.yaml
-bidsschematools/data/schema/rules/datatypes/derivatives/common_derivatives.yaml
-bidsschematools/data/schema/rules/datatypes/derivatives/common_imaging_derivatives.yaml
+bidsschematools/data/schema/rules/checks/nirs.yaml
+bidsschematools/data/schema/rules/files/common/core.yaml
+bidsschematools/data/schema/rules/files/common/tables.yaml
+bidsschematools/data/schema/rules/files/deriv/imaging.yaml
+bidsschematools/data/schema/rules/files/deriv/preprocessed_data.yaml
+bidsschematools/data/schema/rules/files/raw/anat.yaml
+bidsschematools/data/schema/rules/files/raw/beh.yaml
+bidsschematools/data/schema/rules/files/raw/channels.yaml
+bidsschematools/data/schema/rules/files/raw/dwi.yaml
+bidsschematools/data/schema/rules/files/raw/eeg.yaml
+bidsschematools/data/schema/rules/files/raw/fmap.yaml
+bidsschematools/data/schema/rules/files/raw/func.yaml
+bidsschematools/data/schema/rules/files/raw/ieeg.yaml
+bidsschematools/data/schema/rules/files/raw/meg.yaml
+bidsschematools/data/schema/rules/files/raw/micr.yaml
+bidsschematools/data/schema/rules/files/raw/nirs.yaml
+bidsschematools/data/schema/rules/files/raw/perf.yaml
+bidsschematools/data/schema/rules/files/raw/pet.yaml
+bidsschematools/data/schema/rules/files/raw/photo.yaml
+bidsschematools/data/schema/rules/files/raw/task.yaml
 bidsschematools/data/schema/rules/sidecars/anat.yaml
 bidsschematools/data/schema/rules/sidecars/asl.yaml
 bidsschematools/data/schema/rules/sidecars/beh.yaml
 bidsschematools/data/schema/rules/sidecars/continuous.yaml
 bidsschematools/data/schema/rules/sidecars/dwi.yaml
 bidsschematools/data/schema/rules/sidecars/eeg.yaml
 bidsschematools/data/schema/rules/sidecars/entity_rules.yaml
 bidsschematools/data/schema/rules/sidecars/events.yaml
 bidsschematools/data/schema/rules/sidecars/fmap.yaml
 bidsschematools/data/schema/rules/sidecars/func.yaml
 bidsschematools/data/schema/rules/sidecars/ieeg.yaml
 bidsschematools/data/schema/rules/sidecars/meg.yaml
 bidsschematools/data/schema/rules/sidecars/micr.yaml
 bidsschematools/data/schema/rules/sidecars/mri.yaml
+bidsschematools/data/schema/rules/sidecars/nirs.yaml
 bidsschematools/data/schema/rules/sidecars/pet.yaml
 bidsschematools/data/schema/rules/sidecars/derivatives/common_derivatives.yaml
 bidsschematools/data/schema/rules/tabular_data/eeg.yaml
 bidsschematools/data/schema/rules/tabular_data/ieeg.yaml
 bidsschematools/data/schema/rules/tabular_data/meg.yaml
+bidsschematools/data/schema/rules/tabular_data/modality_agnostic.yaml
+bidsschematools/data/schema/rules/tabular_data/nirs.yaml
 bidsschematools/data/schema/rules/tabular_data/perf.yaml
 bidsschematools/data/schema/rules/tabular_data/pet.yaml
 bidsschematools/data/schema/rules/tabular_data/physio.yaml
 bidsschematools/data/schema/rules/tabular_data/task.yaml
 bidsschematools/data/schema/rules/tabular_data/derivatives/common_derivatives.yaml
+bidsschematools/render/__init__.py
+bidsschematools/render/tables.py
+bidsschematools/render/text.py
+bidsschematools/render/utils.py
 bidsschematools/tests/__init__.py
 bidsschematools/tests/conftest.py
 bidsschematools/tests/test_make_testdata.py
-bidsschematools/tests/test_render.py
+bidsschematools/tests/test_render_tables.py
+bidsschematools/tests/test_render_text.py
+bidsschematools/tests/test_render_utils.py
 bidsschematools/tests/test_rules.py
 bidsschematools/tests/test_schema.py
-bidsschematools/tests/test_utils.py
 bidsschematools/tests/test_validator.py
 bidsschematools/tests/data/__init__.py
 bidsschematools/tests/data/broken_dataset_description.json
 bidsschematools/tests/data/expected_bids_validator_xs_write.log
 bidsschematools/tests/data/__pycache__/__init__.cpython-310.pyc
 bidsschematools/tests/data/bids-error-examples/CONTRIBUTING.md
 bidsschematools/tests/data/bids-error-examples/README.md
@@ -314,8 +325,10 @@
 bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.json
 bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-1_VFA.nii.gz
 bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.json
 bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/anat/sub-01_flip-2_VFA.nii.gz
 bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.json
 bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr1_TB1AFI.nii.gz
 bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.json
-bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.nii.gz
+bidsschematools/tests/data/bids-examples/qmri_vfa/sub-01/fmap/sub-01_acq-tr2_TB1AFI.nii.gz
+bidsschematools/types/__init__.py
+bidsschematools/types/namespace.py
```

### Comparing `bidsschematools-0.5.1/pyproject.toml` & `bidsschematools-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bidsschematools-0.5.1/setup.cfg` & `bidsschematools-0.6.0/setup.cfg`

 * *Files identical despite different names*

