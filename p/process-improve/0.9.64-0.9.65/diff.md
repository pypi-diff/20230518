# Comparing `tmp/process-improve-0.9.64.tar.gz` & `tmp/process-improve-0.9.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-improve-0.9.64.tar", last modified: Fri Sep 16 09:39:34 2022, max compression
+gzip compressed data, was "process-improve-0.9.65.tar", last modified: Thu May 18 04:35:06 2023, max compression
```

## Comparing `process-improve-0.9.64.tar` & `process-improve-0.9.65.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.437300 process-improve-0.9.64/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     1073 2021-06-18 10:46:20.000000 process-improve-0.9.64/LICENSE
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)       45 2021-06-18 10:46:20.000000 process-improve-0.9.64/MANIFEST.in
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      769 2022-09-16 09:39:34.437300 process-improve-0.9.64/PKG-INFO
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      164 2021-06-18 10:46:20.000000 process-improve-0.9.64/README.md
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.425300 process-improve-0.9.64/process_improve/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)       89 2022-09-16 09:29:21.000000 process-improve-0.9.64/process_improve/__init__.py
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.429300 process-improve-0.9.64/process_improve/batch/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/batch/__init__.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2656 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/batch/alignment_helpers.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6478 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/batch/data_input.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    24248 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/batch/features.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    24842 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/batch/plotting.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    22836 2022-08-31 15:10:33.000000 process-improve-0.9.64/process_improve/batch/preprocessing.py
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.429300 process-improve-0.9.64/process_improve/bivariate/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/bivariate/__init__.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6150 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/bivariate/methods.py
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.425300 process-improve-0.9.64/process_improve/datasets/
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.429300 process-improve-0.9.64/process_improve/datasets/batch/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    26583 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/batch/batch-fake-data.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     3579 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/batch/details.txt
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)   667696 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/batch/dryer.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)   325044 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/batch/nylon.csv
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.429300 process-improve-0.9.64/process_improve/datasets/experiments/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     1622 2022-08-31 11:11:40.000000 process-improve-0.9.64/process_improve/datasets/experiments/test_doe1.csv
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.429300 process-improve-0.9.64/process_improve/datasets/monitoring/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2353 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/monitoring/batch-yield-and-purity.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      407 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/monitoring/rubber-colour.csv
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.429300 process-improve-0.9.64/process_improve/datasets/multivariate/
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.433300 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      317 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/C.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      498 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/Hotellings_T2_A3.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      483 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/Hotellings_T2_A6.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6913 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/LDPE.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      891 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/P.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      903 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/R.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     3257 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/T.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     3232 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/U.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      906 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/W.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2700 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/Yhat_A6.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6546 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/kamyr.csv
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)  2394760 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/datasets/multivariate/tablet-spectra.csv
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.437300 process-improve-0.9.64/process_improve/experiments/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/experiments/__init__.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6262 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/experiments/datasets.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      733 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/experiments/designs_factorial.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    11046 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/experiments/models.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     9647 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/experiments/optimization.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    24583 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/experiments/plotting.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     3029 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/experiments/simulations.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    12614 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/experiments/structures.py
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.437300 process-improve-0.9.64/process_improve/monitoring/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/monitoring/__init__.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    14636 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/monitoring/control_charts.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2696 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/monitoring/metrics.py
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.437300 process-improve-0.9.64/process_improve/multivariate/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/multivariate/__init__.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    53158 2022-09-13 08:41:09.000000 process-improve-0.9.64/process_improve/multivariate/methods.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    26231 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/multivariate/plots.py
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.437300 process-improve-0.9.64/process_improve/regression/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/regression/__init__.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    11765 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/regression/methods.py
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.437300 process-improve-0.9.64/process_improve/univariate/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.64/process_improve/univariate/__init__.py
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    31586 2022-08-31 11:12:15.000000 process-improve-0.9.64/process_improve/univariate/metrics.py
-drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2022-09-16 09:39:34.429300 process-improve-0.9.64/process_improve.egg-info/
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      769 2022-09-16 09:39:34.000000 process-improve-0.9.64/process_improve.egg-info/PKG-INFO
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2264 2022-09-16 09:39:34.000000 process-improve-0.9.64/process_improve.egg-info/SOURCES.txt
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        1 2022-09-16 09:39:34.000000 process-improve-0.9.64/process_improve.egg-info/dependency_links.txt
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      117 2022-09-16 09:39:34.000000 process-improve-0.9.64/process_improve.egg-info/requires.txt
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)       16 2022-09-16 09:39:34.000000 process-improve-0.9.64/process_improve.egg-info/top_level.txt
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)       38 2022-09-16 09:39:34.437300 process-improve-0.9.64/setup.cfg
--rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     1495 2022-09-16 09:24:58.000000 process-improve-0.9.64/setup.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.751166 process-improve-0.9.65/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     1073 2021-06-18 10:46:20.000000 process-improve-0.9.65/LICENSE
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)       45 2021-06-18 10:46:20.000000 process-improve-0.9.65/MANIFEST.in
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      732 2023-05-18 04:35:06.751166 process-improve-0.9.65/PKG-INFO
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      164 2021-06-18 10:46:20.000000 process-improve-0.9.65/README.md
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.731166 process-improve-0.9.65/process_improve/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)       89 2023-05-18 04:17:45.000000 process-improve-0.9.65/process_improve/__init__.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.735166 process-improve-0.9.65/process_improve/batch/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/batch/__init__.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2626 2023-05-18 04:33:37.000000 process-improve-0.9.65/process_improve/batch/alignment_helpers.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6396 2023-05-18 04:33:37.000000 process-improve-0.9.65/process_improve/batch/data_input.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    24083 2023-05-18 04:33:38.000000 process-improve-0.9.65/process_improve/batch/features.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    24575 2023-05-18 04:33:38.000000 process-improve-0.9.65/process_improve/batch/plotting.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    22524 2023-05-18 04:28:27.000000 process-improve-0.9.65/process_improve/batch/preprocessing.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.735166 process-improve-0.9.65/process_improve/bivariate/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/bivariate/__init__.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6040 2023-05-18 04:33:37.000000 process-improve-0.9.65/process_improve/bivariate/methods.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.727166 process-improve-0.9.65/process_improve/datasets/
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.735166 process-improve-0.9.65/process_improve/datasets/batch/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    26583 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/batch/batch-fake-data.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     3579 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/batch/details.txt
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)   667696 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/batch/dryer.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)   325044 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/batch/nylon.csv
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.739166 process-improve-0.9.65/process_improve/datasets/experiments/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     1622 2022-08-31 11:11:40.000000 process-improve-0.9.65/process_improve/datasets/experiments/test_doe1.csv
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.739166 process-improve-0.9.65/process_improve/datasets/monitoring/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2353 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/monitoring/batch-yield-and-purity.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      407 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/monitoring/rubber-colour.csv
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.739166 process-improve-0.9.65/process_improve/datasets/multivariate/
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.743166 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      317 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/C.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      498 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/Hotellings_T2_A3.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      483 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/Hotellings_T2_A6.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6913 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/LDPE.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      891 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/P.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      903 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/R.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     3257 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/T.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     3232 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/U.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      906 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/W.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2700 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/Yhat_A6.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6546 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/kamyr.csv
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)  2394760 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/datasets/multivariate/tablet-spectra.csv
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.747166 process-improve-0.9.65/process_improve/experiments/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/experiments/__init__.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     6262 2023-05-18 04:17:46.000000 process-improve-0.9.65/process_improve/experiments/datasets.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      733 2023-05-18 04:17:45.000000 process-improve-0.9.65/process_improve/experiments/designs_factorial.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    10814 2023-05-18 04:28:26.000000 process-improve-0.9.65/process_improve/experiments/models.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     9647 2022-08-31 11:12:15.000000 process-improve-0.9.65/process_improve/experiments/optimization.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    24455 2023-05-18 04:28:27.000000 process-improve-0.9.65/process_improve/experiments/plotting.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2923 2023-05-18 04:28:27.000000 process-improve-0.9.65/process_improve/experiments/simulations.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    12533 2023-05-18 04:28:27.000000 process-improve-0.9.65/process_improve/experiments/structures.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.747166 process-improve-0.9.65/process_improve/monitoring/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/monitoring/__init__.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    14234 2023-05-18 04:33:37.000000 process-improve-0.9.65/process_improve/monitoring/control_charts.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2638 2023-05-18 04:33:37.000000 process-improve-0.9.65/process_improve/monitoring/metrics.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.747166 process-improve-0.9.65/process_improve/multivariate/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/multivariate/__init__.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    52271 2023-05-18 04:28:29.000000 process-improve-0.9.65/process_improve/multivariate/methods.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    26007 2023-05-18 04:28:28.000000 process-improve-0.9.65/process_improve/multivariate/plots.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.747166 process-improve-0.9.65/process_improve/regression/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/regression/__init__.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    11449 2023-05-18 04:33:38.000000 process-improve-0.9.65/process_improve/regression/methods.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.751166 process-improve-0.9.65/process_improve/univariate/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        0 2021-06-18 10:46:20.000000 process-improve-0.9.65/process_improve/univariate/__init__.py
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)    31294 2023-05-18 04:33:39.000000 process-improve-0.9.65/process_improve/univariate/metrics.py
+drwxrwxr-x   0 kevindunn  (1001) kevindunn  (1001)        0 2023-05-18 04:35:06.731166 process-improve-0.9.65/process_improve.egg-info/
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      732 2023-05-18 04:35:06.000000 process-improve-0.9.65/process_improve.egg-info/PKG-INFO
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2279 2023-05-18 04:35:06.000000 process-improve-0.9.65/process_improve.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)        1 2023-05-18 04:35:06.000000 process-improve-0.9.65/process_improve.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)      122 2023-05-18 04:35:06.000000 process-improve-0.9.65/process_improve.egg-info/requires.txt
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)       16 2023-05-18 04:35:06.000000 process-improve-0.9.65/process_improve.egg-info/top_level.txt
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     2997 2023-05-18 04:29:57.000000 process-improve-0.9.65/pyproject.toml
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)       38 2023-05-18 04:35:06.751166 process-improve-0.9.65/setup.cfg
+-rw-rw-r--   0 kevindunn  (1001) kevindunn  (1001)     1484 2023-05-18 04:28:27.000000 process-improve-0.9.65/setup.py
```

### Comparing `process-improve-0.9.64/LICENSE` & `process-improve-0.9.65/LICENSE`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/PKG-INFO` & `process-improve-0.9.65/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: process-improve
-Version: 0.9.64
+Version: 0.9.65
 Summary: Process Improvement using Data: Designed Experiments; Latent Variables (PCA, PLS, multivariate methods with missing data); Process Monitoring; Batch data analysis.
 Home-page: https://github.com/kgdunn/process_improve
 Author: Kevin Dunn
 Author-email: kgdunn@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Process Improvement (using Data)
 
 This is a package that goes with the
 [online book](https://learnche.org/pid) of the same title,
 Process Improvement using Data.
-
-
```

### Comparing `process-improve-0.9.64/process_improve/batch/alignment_helpers.py` & `process-improve-0.9.65/process_improve/batch/alignment_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,15 @@
 
     for idx in np.arange(1, nr):
         D[idx, 0] = dist[idx, 0] + D[idx - 1, 0]
 
     for n in np.arange(1, nt):
         for m in np.arange(max((1, band[n, 0])), band[n, 1]):
             # index here must be integer!
-            D[m, n] = dist[m, n] + np.nanmin(
-                [D[m, n - 1], D[m - 1, n - 1], D[m - 1, n]]
-            )
+            D[m, n] = dist[m, n] + np.nanmin([D[m, n - 1], D[m - 1, n - 1], D[m - 1, n]])
 
     return D
 
 
 @jit(nopython=True)
 def backtrack_optimal_path(D: np.ndarray):
     nr, nt = D.shape
```

### Comparing `process-improve-0.9.64/process_improve/batch/data_input.py` & `process-improve-0.9.65/process_improve/batch/data_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,17 +60,15 @@
 
 
     Returns
     -------
     bool
         True, if it passes the checks.
     """
-    assert (
-        len(in_dict) >= 1
-    ), "At least 1 batch is required in the dataframe dictionary."
+    assert len(in_dict) >= 1, "At least 1 batch is required in the dataframe dictionary."
     batch1 = in_dict[list(in_dict.keys())[0]]
     base_columns = set(batch1.columns)
     check = True
     for bid, batch in in_dict.items():
         # Check 1
         check = check & (base_columns == set(batch.columns))
         assert check, (
@@ -86,28 +84,24 @@
         if no_nan:
             check *= batch.isna().values.sum() == 0
             assert check, f"No missing values allowed. Missing values found in {bid}."
 
     return bool(check)
 
 
-def dict_to_melted(
-    in_df: pd.DataFrame, insert_batch_id_column=True, insert_sequence_column=False
-) -> pd.DataFrame:
+def dict_to_melted(in_df: pd.DataFrame, insert_batch_id_column=True, insert_sequence_column=False) -> pd.DataFrame:
     """Reverse of `melted_to_dict`"""
     batch_id_col = "batch_id"
     all_batches = []
     num_rows = 0
     for idx, (batch_id, batch) in enumerate(in_df.items()):
         if idx == 0:
             num_rows = batch.shape[0]
             sequence = np.arange(0, num_rows)
-        assert (
-            num_rows == batch.shape[0]
-        ), "All batches must have the same number of samples"
+        assert num_rows == batch.shape[0], "All batches must have the same number of samples"
 
         subset = batch.copy()
 
         if insert_batch_id_column and batch_id_col not in batch:
             subset.insert(0, batch_id_col, batch_id)
 
         if insert_sequence_column:
@@ -125,17 +119,15 @@
     `group_by_batch`, if True, means that all the data from the first batch is on the left
     of the output dataframe, and the last batch is collected on the right.
 
     If `group_by_batch` is False, then data for the same tag are grouped together, side-by-side.
 
     TODO: `group_by_batch` is not implemented yet.
     """
-    out_df = dict_to_melted(
-        in_df=in_df, insert_batch_id_column=True, insert_sequence_column=True
-    )
+    out_df = dict_to_melted(in_df=in_df, insert_batch_id_column=True, insert_sequence_column=True)
     aligned_wide_df = out_df.pivot(index="batch_id", columns="_sequence_")
     if group_by_batch:
         pass
         # TODO: use the hierarchical indexing and regroup the columns
 
     return aligned_wide_df
 
@@ -144,17 +136,15 @@
     """
     Loads a "melted" data set, where one of the columns is the `batch_id_col`.
     The data are grouped along the unique values of `batch_id_col`, and each group is stored
     in a dictionary. The dictionary keys are the batch identifier, and the corresponding value
     is a Pandas dataframe of the batch data for that batch.
     """
     batches = {}
-    assert (
-        batch_id_col in in_df
-    ), "The `batch_id_col` column does not exist in the incoming dataframe."
+    assert batch_id_col in in_df, "The `batch_id_col` column does not exist in the incoming dataframe."
     for batch_id, batch in in_df.groupby(batch_id_col):
         batches[batch_id] = batch
 
     return batches
 
 
 def melted_to_wide(in_df: pd.DataFrame, batch_id_col) -> dict:
@@ -183,14 +173,12 @@
     return pd.DataFrame()
 
 
 def wide_to_dict():
     pass
 
 
-def melt_df_to_series(
-    in_df: pd.DataFrame, exclude_columns=["batch_id"], name=None
-) -> pd.Series:
+def melt_df_to_series(in_df: pd.DataFrame, exclude_columns=["batch_id"], name=None) -> pd.Series:
     """Returns a Series with a multilevel-index, melted from the DataFrame"""
     out = in_df.drop(exclude_columns, axis=1).T.stack()
     out.name = name
     return out
```

### Comparing `process-improve-0.9.64/process_improve/batch/features.py` & `process-improve-0.9.65/process_improve/batch/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,30 +8,24 @@
 from ..bivariate.methods import find_elbow_point
 from ..regression.methods import repeated_median_slope
 
 # General
 # ------------------------------------------
 
 
-def _prepare_data(
-    df: pd.DataFrame, tags=None, batch_col=None, phase_col=None, age_col=None
-):
+def _prepare_data(df: pd.DataFrame, tags=None, batch_col=None, phase_col=None, age_col=None):
     """
     General function, used for all feature extractions.
 
     1. Groups the ``df`` by batch firstly, and by phase, secondly.
     2. Creates the output dataframe to write the results to.
     """
 
     # Special case: a single series. Convert it to a dataframe
-    if (
-        isinstance(df, pd.Series)
-        and (tags is None)
-        and isinstance(df.index, pd.DatetimeIndex)
-    ):
+    if isinstance(df, pd.Series) and (tags is None) and isinstance(df.index, pd.DatetimeIndex):
         if df.name is None:
             name = "tag"
         else:
             name = df.name
 
         tags = [name]
         df = pd.DataFrame(df, columns=tags)
@@ -302,17 +296,15 @@
     accurate areas if the data are not evenly-spaced in time along the x-axis.
 
     The area is calculated using the trapezoidal rule.
 
     See also: f_sum, f_cumsum
     """
     base_name = "area"
-    prepared, tags, output, _ = _prepare_data(
-        data, tags, batch_col, phase_col, age_col=time_tag
-    )
+    prepared, tags, output, _ = _prepare_data(data, tags, batch_col, phase_col, age_col=time_tag)
     f_names = [(tag + "_" + base_name) for tag in tags]
 
     # We will overwrite all entries in this dataframe, one-by-one
     output = prepared.sum()
     for batch_id, this_batch in prepared:
         # Average width of the base * height. For time series, the average width of the base is
         # the same as the sampling intervals. Therefore the diff of the index.
@@ -320,19 +312,15 @@
         for tag in tags:
             # Now the sum makes sense: gets the area under the curve by adding
             # up the smaller trapezoids: consider the trapezoids as rotated by 90 degrees.
             # The parallel edges are lying vertically. Area of each one is the average of the
             # heights on the left and the right, multiplied by delta distance on the horizontal
             # index axis. Area = average(parallel lenghts) * height
             # where height = delta distance on the horizontal axis.
-            area = (
-                (this_batch[tag].iloc[0:-1].values + this_batch[tag].iloc[1:])
-                / 2
-                * half_base_factor
-            ).sum()
+            area = ((this_batch[tag].iloc[0:-1].values + this_batch[tag].iloc[1:]) / 2 * half_base_factor).sum()
             output.loc[batch_id][tag] = area
 
             # TODO: check this out still
             # Trapezoidal rule for integrated area, still add the "delta X" constant:
             # # https://en.wikipedia.org/wiki/Trapezoidal_rule
             # area = (
             #     this_batch[tag].values[0]
@@ -611,19 +599,15 @@
         batch_col,
         phase_col=None,
         age_col=time_tag,
     )
 
     f_name = tag + "_" + base_name
 
-    output = prepared.apply(
-        lambda x: cross(
-            x[tag], threshold, direction, only_index=only_index, first_point_only=True
-        )
-    )
+    output = prepared.apply(lambda x: cross(x[tag], threshold, direction, only_index=only_index, first_point_only=True))
 
     return pd.DataFrame(data={f_name: output})
 
 
 def f_elbow(
     data: pd.DataFrame,
     x_axis_tag: str,
@@ -644,23 +628,20 @@
     The function returns the *value* on the x-axis where the elbox occurs. Sometimes you might
     want the *index* of the value, so you can also find the corresponding y-axis value. Use
     `only_index=True` for such cases.
     """
     import warnings
 
     base_name = "elbow"
-    prepared, tags, output, _ = _prepare_data(
-        data, tags, batch_col, phase_col, age_col=x_axis_tag
-    )
+    prepared, tags, output, _ = _prepare_data(data, tags, batch_col, phase_col, age_col=x_axis_tag)
     f_names = [(tag + "_" + base_name) for tag in tags]
 
     # We will overwrite all entries in this dataframe, one-by-one
     output = prepared.sum()
     for batch_id, this_batch in prepared:
-
         if x_axis_tag not in this_batch:
             this_batch.reset_index(inplace=True)
         for tag in tags:
             subset = this_batch[[x_axis_tag, tag]]
             subset = subset.dropna()
             X = subset[x_axis_tag]
```

### Comparing `process-improve-0.9.64/process_improve/batch/plotting.py` & `process-improve-0.9.65/process_improve/batch/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     """
     Convert the input colour triplet (list) to a Plotly rgba(r,g,b,a) string if
     `as_string` is True. If `False` it will return the list of 3 integer RGB
     values.
 
     E.g.    [0.9677975592919913, 0.44127456009157356, 0.5358103155058701] -> 'rgba(246,112,136,1)'
     """
-    assert (
-        3 <= len(incolour) <= 4
-    ), "`incolour` must be a list of 3 or 4 values; ignores 4th entry"
+    assert 3 <= len(incolour) <= 4, "`incolour` must be a list of 3 or 4 values; ignores 4th entry"
     colours = [max(0, int(math.floor(c * 255))) for c in list(incolour)[0:3]]
     if as_string:
         return f"rgba({colours[0]},{colours[1]},{colours[2]},{float(alpha)})"
     else:
         return colours
 
 
@@ -118,39 +116,30 @@
     default_line_width = 2
     unique_items = list(df_dict.keys())
     n_colours = len(unique_items)
     random.seed(13)
     colours = list(sns.husl_palette(n_colours))
     random.shuffle(colours)
     colours = [get_rgba_from_triplet(c, as_string=True) for c in colours]
-    line_styles = {
-        k: dict(width=default_line_width, color=v)
-        for k, v in zip(unique_items, colours)
-    }
+    line_styles = {k: dict(width=default_line_width, color=v) for k, v in zip(unique_items, colours)}
     for key, val in batches_to_highlight.items():
-        line_styles.update(
-            {item: json.loads(key) for item in val if item in df_dict.keys()}
-        )
+        line_styles.update({item: json.loads(key) for item in val if item in df_dict.keys()})
 
     highlight_list = []
     for key, val in batches_to_highlight.items():
         highlight_list.extend(val)
 
     highlight_list = list(set(highlight_list))
 
     fig = go.Figure()
 
     for batch_id, batch_df in df_dict.items():
-        assert (
-            tag in batch_df.columns
-        ), f"Tag '{tag}' not found in the batch with id {batch_id}."
+        assert tag in batch_df.columns, f"Tag '{tag}' not found in the batch with id {batch_id}."
         if tag_y2:
-            assert (
-                tag_y2 in batch_df.columns
-            ), f"Tag '{tag}' not found in the batch with id {batch_id}."
+            assert tag_y2 in batch_df.columns, f"Tag '{tag}' not found in the batch with id {batch_id}."
         if time_column in batch_df.columns:
             time_data = batch_df[time_column]
         else:
             time_data = list(range(batch_df.shape[0]))
 
         if batch_id in highlight_list:
             continue  # come to this later
@@ -208,24 +197,20 @@
                         name=batch_id,
                         mode="lines",
                         opacity=0.8,
                         yaxis="y2",
                     )
                 )
 
-    yaxis1_dict = dict(
-        title=tag, gridwidth=2, matches="y1", showticklabels=True, side="left"
-    )
+    yaxis1_dict = dict(title=tag, gridwidth=2, matches="y1", showticklabels=True, side="left")
     if (y1_limits[0] is not None) or (y1_limits[1] is not None):
         yaxis1_dict["autorange"] = False
         yaxis1_dict["range"] = y1_limits
 
-    yaxis2_dict: Dict[str, Any] = dict(
-        title=tag_y2, gridwidth=2, matches="y2", showticklabels=True, side="right"
-    )
+    yaxis2_dict: Dict[str, Any] = dict(title=tag_y2, gridwidth=2, matches="y2", showticklabels=True, side="right")
     if (y2_limits[0] is not None) or (y2_limits[1] is not None):
         yaxis2_dict["autorange"] = False
         yaxis2_dict["range"] = y2_limits
 
     fig.update_layout(
         title=f"Plot of: '{tag}'"
         + (f" on left axis; with '{str(tag_y2)}' on right axis." if tag_y2 else ".")
@@ -262,29 +247,20 @@
     the value is a colour and line width setting for Plotly.
 
     override_default_colour: bool
         If True, then the default colour is used (grey: 0.5, 0.5, 0.5)
     """
     random.seed(13)
     n_colours = len(batch_ids)
-    colours = (
-        list(colour_map(n_colours))
-        if not (use_default_colour)
-        else [(0.5, 0.5, 0.5)] * n_colours
-    )
+    colours = list(colour_map(n_colours)) if not (use_default_colour) else [(0.5, 0.5, 0.5)] * n_colours
     random.shuffle(colours)
     colours = [get_rgba_from_triplet(c, as_string=True) for c in colours]
-    colour_assignment = {
-        key: dict(width=default_line_width, color=val)
-        for key, val in zip(list(batch_ids), colours)
-    }
+    colour_assignment = {key: dict(width=default_line_width, color=val) for key, val in zip(list(batch_ids), colours)}
     for key, val in batches_to_highlight.items():
-        colour_assignment.update(
-            {item: json.loads(key) for item in val if item in batch_ids}
-        )
+        colour_assignment.update({item: json.loads(key) for item in val if item in batch_ids})
     return colour_assignment
 
 
 # flake8: noqa: C901
 def plot_multitags(
     df_dict: dict,
     batch_list: list = None,
@@ -440,17 +416,15 @@
         # Afterwards, add them back, at the end.
         batch_list.extend(settings["animate_batches_to_highlight"])
 
     if time_column in tag_list:
         tag_list.remove(time_column)
 
     # Check that the tag_list is present in all batches.
-    assert check_valid_batch_dict(
-        {k: v[tag_list] for k, v in df_dict.items() if k in batch_list}, no_nan=False
-    )
+    assert check_valid_batch_dict({k: v[tag_list] for k, v in df_dict.items() if k in batch_list}, no_nan=False)
 
     if settings["ncols"] == 0:
         settings["ncols"] = int(np.ceil(len(tag_list) / int(settings["nrows"])))
 
     specs = [[{"type": "scatter"}] * int(settings["ncols"])] * int(settings["nrows"])
 
     fig.set_subplots(
@@ -466,17 +440,15 @@
     )
 
     colour_assignment = colours_per_batch_id(
         batch_ids=list(df_dict.keys()),
         batches_to_highlight=batches_to_highlight,
         default_line_width=settings["default_line_width"],
         # if animating, yes, use grey for all lines; unless `batches_to_highlight` was specified
-        use_default_colour=settings["animate"]
-        if settings["animate"] and (len(batches_to_highlight) == 0)
-        else False,
+        use_default_colour=settings["animate"] if settings["animate"] and (len(batches_to_highlight) == 0) else False,
         colour_map=settings["colour_map"],
     )
 
     # Initial plot (what is visible before animation starts)
     longest_time_length: int = 0
     for batch_id in batch_list:
         batch_df = df_dict[batch_id]
@@ -548,17 +520,15 @@
     slider_steps = []
     frame_settings = dict(
         frame={"duration": settings["animate_framerate_milliseconds"], "redraw": True},
         mode="immediate",
         transition={"duration": 0},
     )
     settings["animate_n_frames"] = (
-        settings["animate_n_frames"]
-        if settings["animate_n_frames"] >= 0
-        else longest_time_length
+        settings["animate_n_frames"] if settings["animate_n_frames"] >= 0 else longest_time_length
     )
 
     for index in np.linspace(0, longest_time_length, settings["animate_n_frames"]):
         # TO OPTIMIZE: add hover template only on the last iteration
         # TO OPTIMIZE: can you add only the incremental new piece of animation?
 
         index = int(np.floor(index))
@@ -688,15 +658,14 @@
     Returns a list of dictionaries.
     Each entry in the list is for each subplot; in the order of the subplots.
     Since each subplot is a tag, we need the `tag_list` as input.
     """
     output = []
     row = col = 1
     for tag in tag_list:
-
         for batch_id in batch_ids_to_animate:
             # These 4 lines are duplicated from the outside function
             if time_column in df_dict[batch_id].columns:
                 time_data = df_dict[batch_id][time_column]
             else:
                 time_data = list(range(df_dict[batch_id].shape[0]))
```

### Comparing `process-improve-0.9.64/process_improve/batch/preprocessing.py` & `process-improve-0.9.65/process_improve/batch/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,15 @@
         columns_to_align = batches[list(batches.keys())[0]].columns
 
     collector_rnge = []
     collector_mins = []
     for _, batch in batches.items():
         if settings["robust"]:
             # TODO: consider f_iqr feature here. Would that work?
-            rnge = batch[columns_to_align].quantile(0.98) - batch[
-                columns_to_align
-            ].quantile(0.02)
+            rnge = batch[columns_to_align].quantile(0.98) - batch[columns_to_align].quantile(0.02)
         else:
             rnge = batch[columns_to_align].max() - batch[columns_to_align].min()
 
         rnge[rnge.values == 0] = 1.0
         collector_rnge.append(rnge)
         collector_mins.append(batch.min(axis=0))
 
@@ -106,18 +104,16 @@
         elif isinstance(batches, pd.DataFrame):
             columns_to_align = batches.columns
         else:
             assert False, "Undefined input type"
     out = {}
     for batch_id, batch in batches.items():
         out[batch_id] = batch[columns_to_align].copy()
-        for tag, column in out[batch_id].iteritems():
-            out[batch_id][tag] = (column - scale_df.loc[tag, "Minimum"]) / scale_df.loc[
-                tag, "Range"
-            ]
+        for tag, column in out[batch_id].items():
+            out[batch_id][tag] = (column - scale_df.loc[tag, "Minimum"]) / scale_df.loc[tag, "Range"]
     return out
 
 
 def reverse_scaling(
     batches: Dict[str, pd.DataFrame],
     scale_df: pd.DataFrame,
     columns_to_align: List = None,
@@ -129,18 +125,16 @@
         elif isinstance(batches, pd.DataFrame):
             columns_to_align = batches.columns
         else:
             assert False, "Undefined input type"
     out = {}
     for batch_id, batch in batches.items():
         out[batch_id] = batch[columns_to_align].copy()
-        for tag, column in out[batch_id].iteritems():
-            out[batch_id][tag] = (
-                column * scale_df.loc[tag, "Range"] + scale_df.loc[tag, "Minimum"]
-            )
+        for tag, column in out[batch_id].items():
+            out[batch_id][tag] = column * scale_df.loc[tag, "Range"] + scale_df.loc[tag, "Minimum"]
     return out
 
 
 class DTWresult:
     """Result class."""
 
     def __init__(
@@ -179,15 +173,14 @@
 
     return pd.DataFrame(
         synced,
     )
 
 
 def dtw_core(test, ref, weight_matrix: np.ndarray):
-
     show_plot = False
     nt = test.shape[0]  # 'test' data; will be align to the 'reference' data
     nr = ref.shape[0]
     assert test.shape[1] == ref.shape[1]
 
     D = distance_matrix(test.values, ref.values, weight_matrix)
     md_path, distance = backtrack_optimal_path(D)
@@ -238,17 +231,15 @@
     settings = default_settings
 
     aligned_batches = {}
     distances = []
     average_batch = refbatch_sc.copy().reset_index(drop=True) * 0.0
     successful_alignments = 0
 
-    for batch_id, batch in tqdm(
-        batches_scaled.items(), disable=not (settings["show_progress"])
-    ):
+    for batch_id, batch in tqdm(batches_scaled.items(), disable=not (settings["show_progress"])):
         try:
             # see Kassidas, page 180
             batch_subset = batch.iloc[:: int(settings["subsample"]), :]
             result = dtw_core(batch_subset, refbatch_sc, weight_matrix=weight_matrix)
             average_batch += result.synced
             aligned_batches[batch_id] = result
             successful_alignments += 1
@@ -328,36 +319,28 @@
         interpolate_time_axis_delta=1,
         interpolate_method="cubic",  # any method from scipy.interpolate.interp1d allowed
     )
     if settings:
         default_settings.update(settings)
     settings = default_settings
     assert settings["maximum_iterations"] >= 3, "At least 3 iterations are required"
-    assert (
-        reference_batch in batches
-    ), "`reference_batch` was not found in the dict of batches."
+    assert reference_batch in batches, "`reference_batch` was not found in the dict of batches."
 
-    assert check_valid_batch_dict(
-        {k: v[columns_to_align] for k, v in batches.items()}, no_nan=True
-    )
+    assert check_valid_batch_dict({k: v[columns_to_align] for k, v in batches.items()}, no_nan=True)
 
-    scale_df = determine_scaling(
-        batches=batches, columns_to_align=columns_to_align, settings=settings
-    )
+    scale_df = determine_scaling(batches=batches, columns_to_align=columns_to_align, settings=settings)
     batches_scaled = apply_scaling(batches, scale_df, columns_to_align)
     refbatch_sc = batches_scaled[reference_batch].iloc[:: int(settings["subsample"]), :]
     weight_vector = np.ones(refbatch_sc.shape[1])
     weight_matrix = np.diag(weight_vector)
     weight_history = np.zeros_like(weight_vector) * np.nan
     average_batch = None
     delta_weight = np.linalg.norm(weight_vector)
     iter = 0
-    while (np.linalg.norm(delta_weight) > settings["tolerance"]) and (
-        iter <= settings["maximum_iterations"]
-    ):
+    while (np.linalg.norm(delta_weight) > settings["tolerance"]) and (iter <= settings["maximum_iterations"]):
         if settings["show_progress"]:
             message = f"Iter = {iter} and norm = {np.linalg.norm(delta_weight)}"
             print(message)
 
         iter += 1
         weight_matrix = np.diag(weight_vector)
         weight_history = np.vstack((weight_history, weight_vector.copy()))
@@ -371,32 +354,28 @@
             weight_matrix=weight_matrix,
             settings=settings,
         )
 
         # Deviations from the average batch:
         next_weights = np.zeros((1, refbatch_sc.shape[1]))
         for batch_id, result in aligned_batches.items():
-            next_weights += np.nansum(
-                np.power(result.synced - average_batch, 2), axis=0
-            )
+            next_weights += np.nansum(np.power(result.synced - average_batch, 2), axis=0)
             # TODO: use quadratic weights for now, but try sum of the absolute values instead
             #  np.abs(result.synced - average_batch).sum(axis=0)
 
             # TODO: leave out worst batches when computing the weights
             # dist_df = pd.DataFrame(distances).set_index("batch_id")
             # dist_df.hist("Distance", bins=50)
             # Now find the average trajectory, but ignore problematic batches:
             #      for example, top 5% of the distances.
             # TODO: make this a configurable setting
             # problematic_threshold = dist_df["Distance"].quantile(0.95)
 
         next_weights = 1.0 / np.where(next_weights > epsqrt, next_weights, 10000)
-        weight_vector = (
-            next_weights / np.sum(next_weights) * len(columns_to_align)
-        ).ravel()
+        weight_vector = (next_weights / np.sum(next_weights) * len(columns_to_align)).ravel()
         # If change in delta_weight is small, we terminate early; no need to fine-tune excessively.
         delta_weight = np.diag(weight_matrix) - weight_vector  # old - new
 
     # OK, the weights are found: now use the last iteration's result to get back to original
     # scaling for the trajectories
     weight_history = weight_history[1:, :]
     aligned_df_collection: List[pd.DataFrame] = []
@@ -407,33 +386,31 @@
     )
 
     for batch_id, result in tqdm(
         aligned_batches.items(),
         desc="Interpolating",
         disable=not (settings["show_progress"]),
     ):
-
         initial_row = batches[batch_id].iloc[result.md_path[0, 0], :].copy()
         synced = align_with_path(
             result.md_path,
             batches[batch_id].iloc[:: int(settings["subsample"]), :],
             initial_row=initial_row,
         )
         # Resample the trajectories of the aligned data now along this sequence.
         sequence = np.linspace(
             0,
-            settings["interpolate_time_axis_maximum"]
-            - settings["interpolate_time_axis_delta"],
+            settings["interpolate_time_axis_maximum"] - settings["interpolate_time_axis_delta"],
             synced.shape[0],
         )
         assert new_time_axis.min() == sequence.min()
         assert new_time_axis.max() == sequence.max()
 
         synced_interpolated = pd.DataFrame()
-        for column, _ in synced.iteritems():
+        for column, _ in synced.items():
             if column in ["batch_id", "_sequence_"]:
                 continue
 
             interp_column = sp.interpolate.interp1d(
                 sequence,
                 synced[column],
                 kind=settings["interpolate_method"],
@@ -500,15 +477,15 @@
     target_time = np.arange(0, batches[reference_batch].shape[0])
     target_time = target_time / target_time[-1]
 
     for batch_id, batch in batches.items():
         to_resample = np.arange(0, batch.shape[0])
         to_resample = to_resample / to_resample[-1]
         out_df = {}
-        for column, series in batch.iteritems():
+        for column, series in batch.items():
             if column in columns_to_align:
                 out_df[column] = sp.interpolate.interp1d(
                     to_resample,
                     series.values,
                     copy=False,
                     kind=settings["interpolate_kind"],
                 )(target_time)
@@ -539,31 +516,25 @@
     default_settings = {
         "robust": True,  # use robust metric to calculate average batch length
     }
     if settings:
         default_settings.update(settings)
     settings = default_settings
 
-    batch_lengths = pd.Series(
-        {batch_id: df.shape[0] for batch_id, df in batches.items()}
-    )
+    batch_lengths = pd.Series({batch_id: df.shape[0] for batch_id, df in batches.items()})
     if settings["robust"]:
         # If multiple batches of the median length, return the last one.
         try:
-            return batch_lengths.index[
-                np.where((batch_lengths == batch_lengths.median()).values)[0][-1]
-            ]
+            return batch_lengths.index[np.where((batch_lengths == batch_lengths.median()).values)[0][-1]]
         except IndexError:
             # Very exceptional: if batch_lengths.median() is computed as the average of 2 numbers
             # and therefore the median length batch doesn't actually exist
             return find_average_length(batches, settings=dict(robust=False))
     else:
-        return batch_lengths.index[
-            (batch_lengths - batch_lengths.mean()).abs().argmin()
-        ]
+        return batch_lengths.index[(batch_lengths - batch_lengths.mean()).abs().argmin()]
 
 
 def find_reference_batch(
     batches: Dict[str, pd.DataFrame],
     columns_to_align: list,
     settings: Dict[str, Any] = None,
 ):
```

### Comparing `process-improve-0.9.64/process_improve/bivariate/methods.py` & `process-improve-0.9.65/process_improve/bivariate/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,15 @@
     Will probably not work well on few data points. If so, try fitting a spline
     to the raw data and then repeat with the interpolated data.
 
     """
     start = 5
     # assert divmod(max_iter, 2)[1]  # must be odd number; to ensure we calculate the median later
 
-    def calculate_line_length(
-        x1: float, y1: float, x2: np.ndarray, y2: np.ndarray
-    ) -> Union[float, np.ndarray]:
+    def calculate_line_length(x1: float, y1: float, x2: np.ndarray, y2: np.ndarray) -> Union[float, np.ndarray]:
         """Returns the length of the line between 2 points (x1, y1) and (x2, y2), defined as:
         :math:`\\sqrt{(x2 - x1)^2 + (y2 - y1)^2}`
         """
         return np.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
 
     # Ensure it is a Numpy array: pandas objects and lists are correctly handled.
     x = np.array(x.copy())
@@ -50,17 +48,15 @@
 
     # Stop if everything is missing:
     if np.isnan(np.nanmedian(x)) or np.isnan(np.nanmedian(y)):
         return -1
 
     # Eliminate missing values in x and y simultaneously.
     x, y = x[~(np.isnan(x) | np.isnan(y))], y[~(np.isnan(x) | np.isnan(y))]
-    assert (
-        len(x) > 10
-    ), "Requires more than 10 values in the vectors (not including missing data)."
+    assert len(x) > 10, "Requires more than 10 values in the vectors (not including missing data)."
     idx_sort = x.argsort()
     x = x[idx_sort]
     y = y[idx_sort]
     N = x.size
     # Left and right anchor points: use median of the 5 points at start and end
     lft_x_avg = np.median(x[0:start])
     rgt_x_avg = np.median(x[-start:])
@@ -93,35 +89,30 @@
             lft_line = calculate_line_length(int_x, int_y, lft_x_avg, lft_y)
             rgt_line = calculate_line_length(int_x, int_y, rgt_x_avg, rgt_y)
             hypotenuse_line = calculate_line_length(lft_x_avg, lft_y, rgt_x_avg, rgt_y)
             lft_line_list.append(lft_line)
             rgt_line_list.append(rgt_line)
 
             angle = (
-                np.arccos(
-                    (lft_line**2 + rgt_line**2 - hypotenuse_line**2)
-                    / (2 * lft_line * rgt_line)
-                )
+                np.arccos((lft_line**2 + rgt_line**2 - hypotenuse_line**2) / (2 * lft_line * rgt_line))
                 * 180.0
                 / np.pi
             )
             angle_list.append(angle)
 
     # Visualize the elbow point
     if False:
         import pandas as pd
 
         data = pd.DataFrame(data={"x": x, "y": y})
         ax = data.plot.scatter(x="x", y="y")
 
         intersections = pd.DataFrame(data={"x_int": int_x_list, "y_int": int_y_list})
         intersections.plot.scatter(x="x_int", y="y_int", ax=ax)
-        pd.DataFrame(intersections.median()).T.plot.scatter(
-            x="x_int", y="y_int", color="red", ax=ax
-        )
+        pd.DataFrame(intersections.median()).T.plot.scatter(x="x_int", y="y_int", color="red", ax=ax)
         ax.grid(True)
 
     # Elbow point is taken as the average intersection point which is closest
     # to the raw data. Handle the case for even and odd number of data points
     if divmod(len(int_x_list), 2)[1] == 0:
         mid_idx = np.argmin((np.array(int_x_list) - np.nanmedian(int_x_list)) ** 2)
     else:
```

### Comparing `process-improve-0.9.64/process_improve/datasets/batch/batch-fake-data.csv` & `process-improve-0.9.65/process_improve/datasets/batch/batch-fake-data.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/batch/details.txt` & `process-improve-0.9.65/process_improve/datasets/batch/details.txt`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/batch/dryer.csv` & `process-improve-0.9.65/process_improve/datasets/batch/dryer.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/batch/nylon.csv` & `process-improve-0.9.65/process_improve/datasets/batch/nylon.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/experiments/test_doe1.csv` & `process-improve-0.9.65/process_improve/datasets/experiments/test_doe1.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/monitoring/batch-yield-and-purity.csv` & `process-improve-0.9.65/process_improve/datasets/monitoring/batch-yield-and-purity.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/LDPE.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/LDPE.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/P.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/P.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/R.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/R.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/T.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/T.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/U.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/U.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/W.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/W.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/LDPE/Yhat_A6.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/LDPE/Yhat_A6.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/kamyr.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/kamyr.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/datasets/multivariate/tablet-spectra.csv` & `process-improve-0.9.65/process_improve/datasets/multivariate/tablet-spectra.csv`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/experiments/datasets.py` & `process-improve-0.9.65/process_improve/experiments/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# (c) Kevin Dunn, 2010-2022. MIT License. Based on own private work over the years.
+# (c) Kevin Dunn, 2010-2023. MIT License. Based on own private work over the years.
 
 import pandas as pd
 
 
 def distillateflow():
     """The flow rate of distillate from the top of a distillation column.
```

### Comparing `process-improve-0.9.64/process_improve/experiments/designs_factorial.py` & `process-improve-0.9.65/process_improve/experiments/designs_factorial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# (c) Kevin Dunn, 2010-2022. MIT License.
+# (c) Kevin Dunn, 2010-2023. MIT License.
 
 """
 Various factorial designs
 """
 from typing import Optional
 
 from .structures import c, create_names, expand_grid
```

### Comparing `process-improve-0.9.64/process_improve/experiments/models.py` & `process-improve-0.9.65/process_improve/experiments/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# (c) Kevin Dunn, 2010-2022. MIT License. Based on own private work over the years.
+# (c) Kevin Dunn, 2010-2023. MIT License. Based on own private work over the years.
 
 import warnings
 from collections import defaultdict
 from typing import Any, List, Optional
 
 import numpy as np
 import pandas as pd
@@ -145,23 +145,19 @@
         alias_strings: List[Any] = []
         if len(self.aliasing.keys()) == 0:
             return alias_strings
 
         params = self.get_parameters(drop_intercept=drop_intercept)
         for p_name in params.index.values:
             if websafe:
-                aliasing = (
-                    '<span style="font-size: 130%; font-weight: 700">'
-                    f"{p_name}</span>"
-                )
+                aliasing = '<span style="font-size: 130%; font-weight: 700">' f"{p_name}</span>"
             else:
                 aliasing = p_name
             suffix = ""
             for alias in self.aliasing[tuple([p_name])]:
-
                 # Subtract "-1" because the first list entry tracks the sign
                 if (len(alias) - 1) <= aliasing_up_to_level:
                     aliasing += f" {alias[0]} {':'.join(alias[1:])}"
                 if (len(alias) - 1) > aliasing_up_to_level:
                     if websafe:
                         suffix = r" + <i>higher interactions</i>"
                     else:
@@ -236,27 +232,19 @@
                         pass
                     else:
                         corrcoef[idx, j] = c[idx, j] / stddev[idx] / stddev[j]
 
                 # corrcoef = c / stddev[idx, None]
                 # corrcoef = corrcoef / stddev[None, idx]
 
-                candidates = [
-                    i
-                    for i, val in enumerate(np.abs(corrcoef[idx, :]))
-                    if (val > threshold_correlation)
-                ]
+                candidates = [i for i, val in enumerate(np.abs(corrcoef[idx, :])) if (val > threshold_correlation)]
                 signs = [np.sign(j) for j in corrcoef[idx, :]]
             else:
                 # Columns with no variation
-                candidates = [
-                    i
-                    for i, j in enumerate(has_variation)
-                    if (j <= threshold_correlation)
-                ]
+                candidates = [i for i, j in enumerate(has_variation) if (j <= threshold_correlation)]
 
             # Track the correlation signs
             signs = [np.sign(j) for j in dot_product[idx, :]]
 
             # Now drop out the candidates with the longest word lengths
             alias_len = [(len(terms[i].factors), i) for i in candidates]
             alias_len.sort(reverse=True)
@@ -264,15 +252,14 @@
                 drop_columns.append(entry[1])
 
             for col in candidates:
                 if col == idx:
                     # It is of course perfectly correlated with itself
                     pass
                 else:
-
                     aliases = [t.name() for t in terms[col].factors]
                     if len(aliases) == 0:
                         aliases = ["Intercept"]
 
                     key = tuple([t.name() for t in terms[idx].factors])
                     if len(key) == 0:
                         key = ("Intercept",)
@@ -289,17 +276,15 @@
             alias_len.sort()
             aliasing[key] = [i[1] for i in alias_len]
 
         return aliasing, list(set(drop_columns))
 
     pre_model = smf.ols(model_spec, data=data)
     model_description = ModelDesc.from_formula(model_spec)
-    aliasing, drop_columns = find_aliases(
-        pre_model, model_description, threshold_correlation=alias_threshold
-    )
+    aliasing, drop_columns = find_aliases(pre_model, model_description, threshold_correlation=alias_threshold)
     drop_column_names = [pre_model.data.xnames[i] for i in drop_columns]
 
     post_model = smf.ols(model_spec, data=data, drop_cols=drop_column_names)
 
     name = name or data.pi_title
     out = Model(
         OLS_instance=post_model.fit(),
```

### Comparing `process-improve-0.9.64/process_improve/experiments/optimization.py` & `process-improve-0.9.65/process_improve/experiments/optimization.py`

 * *Files identical despite different names*

### Comparing `process-improve-0.9.64/process_improve/experiments/plotting.py` & `process-improve-0.9.65/process_improve/experiments/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# (c) Kevin Dunn, 2010-2022. MIT License.
+# (c) Kevin Dunn, 2010-2023. MIT License.
 import webbrowser
 
 import numpy as np
 from bokeh.colors import RGB
 from bokeh.models import (
     BasicTicker,
     ColorBar,
@@ -44,15 +44,14 @@
     positive=("Positive effects", "#FF8000"),
     show=True,
     plot_width=500,
     plot_height=None,
     # In the hover over the bars
     aliasing_up_to_level=2,
 ):
-
     # TODO: show full variable names + units on pareto plot for main factors
     #       an interactions
 
     """
     Plots the Pareto plot for a given model.
 
     Parameters
@@ -101,17 +100,15 @@
     # )
     # error_bars = model._OLS.conf_int()
     # http://holoviews.org/reference/elements/bokeh/ErrorBars.html
     # https://docs.bokeh.org/en/latest/docs/user_guide/annotations.html
 
     params = model.get_parameters()
     if up_to_level:
-        assert isinstance(up_to_level, int), (
-            "Specify an integer value for " "`up_to_level`."
-        )
+        assert isinstance(up_to_level, int), "Specify an integer value for " "`up_to_level`."
         keep = []
         for k in range(up_to_level):
             keep.extend(model.get_factor_names(level=k + 1))
 
         params = params.filter(keep)
 
     param_values = params.values
@@ -119,15 +116,15 @@
     bar_colours = [negative[1] if p < 0 else positive[1] for p in param_values]
     bar_signs = ["Positive" if i > 0 else "Negative" for i in param_values]
 
     # Show the absolute parameter values, but we will colour code them
     params = params.abs()
     base_parameters = model.get_factor_names(level=1)
     full_names = []
-    for param_name, _ in params.iteritems():
+    for param_name, _ in params.items():
         if param_name in base_parameters:
             fname = model.data.pi_source.get(param_name, param_name)
             full_names.append(fname)
         else:
             full_names.append(f"Interaction between {param_name}")
 
     # Shuffle the collected information in the same way
@@ -139,17 +136,15 @@
 
     TOOLTIPS = [
         ("Short name", "@factor_names"),
         ("Full name", "@full_names"),
         ("Magnitude and sign", "@original_magnitude_with_sign"),
     ]
 
-    alias_strings = model.get_aliases(
-        aliasing_up_to_level, drop_intercept=True, websafe=True
-    )
+    alias_strings = model.get_aliases(aliasing_up_to_level, drop_intercept=True, websafe=True)
 
     if len(alias_strings) != 0:
         TOOLTIPS.append(
             ("Aliasing", "@alias_strings{safe}"),
         )
     else:
         alias_strings = [""] * len(params.values)
@@ -305,17 +300,15 @@
         # Look at which factors are included, and pop them out. The remaining
         # factors are specified at their zero level
 
         unspecified_factors = [i for i in pure_factors if i not in kwargs.keys()]
         for factor in unspecified_factors:
             kwargs[factor] = np.zeros_like(h_grid)
 
-        assert sorted(kwargs.keys()) == sorted(
-            pure_factors
-        ), "Not all factors were specified."
+        assert sorted(kwargs.keys()) == sorted(pure_factors), "Not all factors were specified."
         Z = predict(model, **kwargs)
         Z = Z.values.reshape(N, N)
 
         # Create a simple contour plot with labels using default colors.  The
         # inline argument to clabel will control whether the labels are draw
         # over the line segments of the contour, removing the lines beneath
         # the label
@@ -379,15 +372,14 @@
     colour_function="terrain",
     show=True,
     show_expt_data=True,
     figsize=(10, 10),
     dpi=50,
     other_factors=None,
 ):
-
     # TODO: show labels of contour plot
 
     # https://stackoverflow.com/questions/33533047/how-to-make-a-contour-plot-in-python-using-bokeh-or-other-libs
 
     dpi_max = dpi**3.5
     N = min(dpi, np.power(dpi_max, 0.5))
 
@@ -414,17 +406,15 @@
     # Look at which factors are included, and pop them out. The remaining
     # factors are specified at their zero level
 
     unspecified_factors = [i for i in pure_factors if i not in kwargs.keys()]
     for factor in unspecified_factors:
         kwargs[factor] = np.zeros_like(h_grid)
 
-    assert sorted(kwargs.keys()) == sorted(pure_factors), (
-        "Not all factors " "were specified."
-    )
+    assert sorted(kwargs.keys()) == sorted(pure_factors), "Not all factors " "were specified."
     Z = predict(model, **kwargs)
     Z = Z.values.reshape(N, N)
     z_min, z_max = Z.min(), Z.max()
     levels = np.linspace(z_min, z_max, N)
 
     import matplotlib
     import matplotlib.pyplot as plt
@@ -506,15 +496,14 @@
             y = cccontour[0][:, 1]
             p.line(x, y, line_dash="dashed", color="darkgrey", line_width=1)
 
     # TODO: bigger experimental markers
     # TODO: hover for the data point shows the factor settings for the data point
 
     if show_expt_data:
-
         source = ColumnDataSource(
             data=dict(
                 x=model.data[xlabel],
                 y=model.data[ylabel],
                 output=model.data[model.get_response_name()].to_list(),
             )
         )
@@ -648,17 +637,15 @@
     xlim = kwargs.get("xlim", (xrange[0] - xdelta * 0.05, xrange[1] + xdelta * 0.05))
     h_grid = np.linspace(xlim[0], xlim[1], num=per_axis_points)
     plotdata = {x_column: h_grid}
 
     if not oneD:
         yrange = model.data[y_column].min(), model.data[y_column].max()
         ydelta = yrange[1] - yrange[0]
-        ylim = kwargs.get(
-            "ylim", (yrange[0] - ydelta * 0.05, yrange[1] + ydelta * 0.05)
-        )
+        ylim = kwargs.get("ylim", (yrange[0] - ydelta * 0.05, yrange[1] + ydelta * 0.05))
 
         v_grid = np.linspace(ylim[0], ylim[1], num=per_axis_points)
         H, V = np.meshgrid(h_grid, v_grid)
         h_grid, v_grid = H.ravel(), V.ravel()
         plotdata[x_column] = h_grid
         plotdata[y_column] = v_grid
 
@@ -681,17 +668,15 @@
 
     if not oneD:
         assert False
     else:
         plotdata[y_column] = Z
         yrange = Z.min(), Z.max()
         ydelta = yrange[1] - yrange[0]
-        ylim = kwargs.get(
-            "ylim", (yrange[0] - ydelta * 0.05, yrange[1] + ydelta * 0.05)
-        )
+        ylim = kwargs.get("ylim", (yrange[0] - ydelta * 0.05, yrange[1] + ydelta * 0.05))
 
     if fig:
         p = fig
         prior_figure = True
     else:
         prior_figure = False
         p = figure(
@@ -758,15 +743,14 @@
     p.xaxis.axis_label_text_font_style = "bold"
 
     p.yaxis.major_label_text_font_size = "14pt"
     p.yaxis.axis_label = y_column
     p.yaxis.axis_label_text_font_size = "14pt"
     p.yaxis.axis_label_text_font_style = "bold"
     if prior_figure:
-
         # p.xaxis.bounds =
         p.x_range = Range1d(
             min(xlim[0], p.x_range.start, min(model.data[x_column])),
             max(xlim[1], p.x_range.end, max(model.data[x_column])),
         )
         p.y_range = Range1d(
             min(ylim[0], p.y_range.start, min(model.data[y_column])),
```

### Comparing `process-improve-0.9.64/process_improve/experiments/simulations.py` & `process-improve-0.9.65/process_improve/experiments/simulations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# (c) Kevin Dunn, 2010-2022. MIT License. Based on own private work over the years.
+# (c) Kevin Dunn, 2010-2023. MIT License. Based on own private work over the years.
 
 import pandas as pd
 from numpy.random import normal
 
 
 def popcorn(t=120, T=None):
     """
@@ -27,15 +27,15 @@
 
     Returns
     -------
     The number of edible popcorn kernels. Random noise is added for realism.
 
     Source
     ------
-    Kevin Dunn, Process Improvement using Data, Chapter 5, 2010 to 2022,
+    Kevin Dunn, Process Improvement using Data, Chapter 5, 2010 to 2023,
     https://learnche.org/pid
 
 
     Examples
     --------
     >>> popcorn(t=55)    # will fail
     >>> popcorn(t=120)
@@ -67,43 +67,34 @@
 
     Typical values are p = $3.50 and h = 150cm
     The outcome is: profit made per hour [dollars/hour], with random noise
                     added, for realism.
 
     Source
     ------
-    Kevin Dunn, Process Improvement using Data, Chapter 5, 2010 to 2022,
+    Kevin Dunn, Process Improvement using Data, Chapter 5, 2010 to 2023,
     https://learnche.org/pid
 
     """
     if P is None:
         P = p
     if H is None:
         H = h
 
     if (len(P) > 1) | (len(H) > 1):
-        assert (
-            False
-        ), "Running the grocery store experiments in parallel is (intentionally) not allowed."
+        assert False, "Running the grocery store experiments in parallel is (intentionally) not allowed."
 
     if pd.isna(P) or pd.isna(H):
         assert False, "All function inputs must be finite numbers."
     elif P < 0:
         assert False, "Please provide a positive sales price, P."
     elif H < 0:
         assert False, "The height of the shelving, H, must be a positive value."
 
     a_coded = (P - 3.2) / 0.2
     b_coded = (H - 50) / 100
     y = round(
-        (
-            18 * a_coded
-            + 12 * b_coded
-            - 7 * a_coded * a_coded
-            - 6.0 * b_coded * b_coded
-            - 8.5 * a_coded * b_coded
-            + 60
-        )
+        (18 * a_coded + 12 * b_coded - 7 * a_coded * a_coded - 6.0 * b_coded * b_coded - 8.5 * a_coded * b_coded + 60)
         * 10.0
         + normal(0, 1) * 2
     )
     return y
```

### Comparing `process-improve-0.9.64/process_improve/experiments/structures.py` & `process-improve-0.9.65/process_improve/experiments/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# (c) Kevin Dunn, 2010-2022. MIT License. Based on own private work over the years.
+# (c) Kevin Dunn, 2010-2023. MIT License. Based on own private work over the years.
 
 import itertools
 from collections import defaultdict
 from collections.abc import Iterable
 
 import numpy as np
 import pandas as pd
@@ -153,18 +153,15 @@
             out.append(chr(65 + n))
 
     else:
         longest = 0
         if padded:
             longest = len(str(start_at + n - 1))
 
-        out = [
-            f'{str(prefix)}{str(i).rjust(longest, "0")}'
-            for i in range(start_at, n + start_at)
-        ]
+        out = [f'{str(prefix)}{str(i).rjust(longest, "0")}' for i in range(start_at, n + start_at)]
 
     return out
 
 
 def c(*args, **kwargs) -> Column:  # noqa: C901
     """
     Performs the equivalent of the R function "c(...)", to combine data elements
@@ -237,17 +234,15 @@
                 numeric = False
                 sanitize.append(j)
 
     # Index creation
     default_idx = list(range(1, len(sanitize) + 1))
     index = kwargs.get("index", default_idx)
     if len(index) != len(sanitize):
-        raise IndexError(
-            ('Length of "index" must match the ' "number of numeric inputs.")
-        )
+        raise IndexError(('Length of "index" must match the ' "number of numeric inputs."))
 
     out = Column(data=sanitize, index=index, name=None)
     # Use sensible defaults, if not provided
     out.pi_index = True
     out.pi_lo = None
     out.pi_hi = None
     out.pi_range = None
@@ -256,15 +251,14 @@
     out.pi_units = None
     out.pi_name = None
     out.pi_is_coded = True
 
     out.pi_name = kwargs.get("name", "Unnamed")
     out.name = out.pi_name
     if numeric:
-
         # If any of 'lo', 'hi', 'center', or 'range' are specified, then it
         # is assumed that the variable is NOT coded
         try:
             out.pi_lo = kwargs["lo"]
             out.pi_is_coded = False
         except KeyError:
             out.pi_lo = out.min()
@@ -281,17 +275,15 @@
         except KeyError:
             out.pi_range = (out.pi_lo, out.pi_hi)
 
         try:
             _ = (e for e in out.pi_range)
         except TypeError:
             assert False, "The `range` input must be an iterable, with " "2 values."
-        assert len(out.pi_range) == 2, (
-            "The `range` variable must be a tuple, " "with 2 values."
-        )
+        assert len(out.pi_range) == 2, "The `range` variable must be a tuple, " "with 2 values."
         out.pi_range = tuple(out.pi_range)
 
         try:
             out.pi_center = kwargs["center"]
             out.pi_is_coded = False
         except KeyError:
             out.pi_center = np.mean(out.pi_range)
```

### Comparing `process-improve-0.9.64/process_improve/monitoring/control_charts.py` & `process-improve-0.9.65/process_improve/monitoring/control_charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,15 @@
         are used, otherwise these values are estimated.
         """
         self._given_target = target
         self._given_s = s
 
         if s is not None:
             self.s = float(s)
-            assert (
-                s > 0.0
-            ), "The given standard deviation cannot be zero, and must be positive."
+            assert s > 0.0, "The given standard deviation cannot be zero, and must be positive."
             assert s < 1e300, "The given standard deviation cannot be this large."
 
         if target is not None:
             self.target = float(target)
 
         self.df["y"] = y.ravel()
         self.N = self.df.shape[0]
@@ -180,17 +178,15 @@
             # User has provided their own lambda_1 and lambda_2 values.
             assert self.ld_1 >= 0.0, "Lambda_1 must be greater than or equal to zero."
             assert self.ld_2 >= 0.0, "Lambda_2 must be greater than or equal to zero."
             assert self.ld_s >= 0.0, "Lambda_s must be greater than or equal to zero."
             assert self.ld_1 <= 1.0, "Lambda_1 must be less than or equal to 1.0."
             assert self.ld_2 <= 1.0, "Lambda_2 must be less than or equal to 1.0."
             assert self.ld_s <= 1.0, "Lambda_s must be less than or equal to 1.0."
-            self._holt_winters_warmup_fit(
-                ld_1=self.ld_1, ld_2=self.ld_2, ld_s=self.ld_s
-            )
+            self._holt_winters_warmup_fit(ld_1=self.ld_1, ld_2=self.ld_2, ld_s=self.ld_s)
 
         else:
             # User wants to find an value for ld_1 and ld_2 that best fits the data
 
             ld_1_index = np.linspace(0.1, 0.9, num=5, endpoint=True)
             ld_2_index = np.linspace(0.1, 0.9, num=5, endpoint=True)
             residuals, _ = np.meshgrid(ld_1_index, ld_2_index)
@@ -216,30 +212,26 @@
             self.ld_2 = best_ld_2
             self._residuals_HW = residuals
             self._holt_winters_warmup_fit(ld_1=best_ld_1, ld_2=best_ld_2, ld_s=ld_s)
 
         # Common code for both branches of if-else above
         future_errors = self.df["error"][self.train_samples]
         S_T_median_error = 1.48 * future_errors.abs().median()  # must handle NaNs!
-        resids = np.power(S_T_median_error, 2) * np.nanmean(
-            rho_func(future_errors / S_T_median_error)
-        )
+        resids = np.power(S_T_median_error, 2) * np.nanmean(rho_func(future_errors / S_T_median_error))
 
         # Ensure no negative square root is taken
         self._tau = np.sqrt(max(0.0, resids))
         if self.target is None:
             # Estimate the target as the median of the y-star (cleaned) y-values
             self.target = self.df["y_star"].median()
         else:
             self._target_calculated_best = self.df["y_star"].median()
 
         if self.s is None:
-            self.s = (
-                self._tau
-            )  # or an alternative: self.df["sigma_hat"] is approximately OK
+            self.s = self._tau  # or an alternative: self.df["sigma_hat"] is approximately OK
 
         # The "delta" emphasizes that it is the deviation from the target.
         self._delta_UCL_3sigma = +3.0 * self._tau
         self._delta_LCL_3sigma = -3.0 * self._tau
 
     def _holt_winters_warmup_fit(self, ld_1=0.5, ld_2=0.8, ld_s=0.2):
         """
@@ -263,40 +255,30 @@
         self.warm_up["y_zero_robust"] = y_warm_up.median()
 
         if isinstance(self.target, float):
             self.warm_up["alpha_0"] = self.target
             self.warm_up["beta_0"] = 0.0
         else:
             # p 290 of the paper, https://onlinelibrary.wiley.com/doi/abs/10.1002/for.1125
-            self.warm_up["beta_0"] = repeated_median_slope(
-                np.arange(self.warm_up["M"]), y_warm_up
-            )
-            self.warm_up["alpha_0"] = np.nanmedian(
-                y_warm_up - self.warm_up["beta_0"] * np.arange(self.warm_up["M"])
-            )
+            self.warm_up["beta_0"] = repeated_median_slope(np.arange(self.warm_up["M"]), y_warm_up)
+            self.warm_up["alpha_0"] = np.nanmedian(y_warm_up - self.warm_up["beta_0"] * np.arange(self.warm_up["M"]))
 
         if isinstance(self.s, float):
             self.warm_up["sigma_0"] = self.s
 
         else:
             # p 290 of the paper, https://onlinelibrary.wiley.com/doi/abs/10.1002/for.1125
-            warm_up_residuals = (
-                y_warm_up - self.warm_up["alpha_0"] - self.warm_up["beta_0"]
-            )
+            warm_up_residuals = y_warm_up - self.warm_up["alpha_0"] - self.warm_up["beta_0"]
 
             # Some other method that does not rely on SciPy for 1 function.
-            self.warm_up["sigma_0"] = median_abs_deviation(
-                warm_up_residuals, nan_policy="omit"
-            )
+            self.warm_up["sigma_0"] = median_abs_deviation(warm_up_residuals, nan_policy="omit")
             self.warm_up["residuals"] = warm_up_residuals
 
         df.loc[0, "rho_input"] = (
-            self.warm_up["y_zero_robust"]
-            - self.warm_up["alpha_0"]
-            - self.warm_up["beta_0"]
+            self.warm_up["y_zero_robust"] - self.warm_up["alpha_0"] - self.warm_up["beta_0"]
         ) / self.warm_up["sigma_0"]
         df.loc[0, "psi_input"] = df["rho_input"][0]
         df.loc[0, "y_star"] = self.warm_up["y_zero_robust"]
         df.loc[0, "alpha_hat"] = self.warm_up["alpha_0"]
         df.loc[0, "beta_hat"] = self.warm_up["beta_0"]
         df.loc[0, "sigma_hat"] = self.warm_up["sigma_0"]
 
@@ -308,28 +290,19 @@
             error_i = df["y"][i] - (df["alpha_hat"][i - 1] + df["beta_hat"][i - 1])
             if np.isnan(error_i):
                 # If there is an error, replace it with the median of the last 10 error estimates
                 # or as many points as available.
                 error_i = df["error"].iloc[max(i - 10, 0) : i].abs().median()
             rho_i = error_i / df["sigma_hat"][i - 1]
             prior_variance = np.power(df["sigma_hat"][i - 1], 2)
-            sigma_i = np.sqrt(
-                rho(rho_i) * ld_s * prior_variance + (1.0 - ld_s) * prior_variance
-            )
+            sigma_i = np.sqrt(rho(rho_i) * ld_s * prior_variance + (1.0 - ld_s) * prior_variance)
             psi_i = error_i / sigma_i
-            y_star_i = (
-                psi(psi_i) * sigma_i + df["alpha_hat"][i - 1] + df["beta_hat"][i - 1]
-            )
-            alpha_i = ld_1 * y_star_i + (1 - ld_1) * (
-                df["alpha_hat"][i - 1] + df["beta_hat"][i - 1]
-            )
-            beta_i = (
-                ld_2 * (alpha_i - df["alpha_hat"][i - 1])
-                + (1 - ld_2) * df["beta_hat"][i - 1]
-            )
+            y_star_i = psi(psi_i) * sigma_i + df["alpha_hat"][i - 1] + df["beta_hat"][i - 1]
+            alpha_i = ld_1 * y_star_i + (1 - ld_1) * (df["alpha_hat"][i - 1] + df["beta_hat"][i - 1])
+            beta_i = ld_2 * (alpha_i - df["alpha_hat"][i - 1]) + (1 - ld_2) * df["beta_hat"][i - 1]
             df.loc[i] = [
                 df["y"][i],
                 psi_i,
                 rho_i,
                 y_star_i,
                 alpha_i,
                 beta_i,
```

### Comparing `process-improve-0.9.64/process_improve/monitoring/metrics.py` & `process-improve-0.9.65/process_improve/monitoring/metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,26 +38,22 @@
         The Cpk value.
     """
     assert trim_percentile >= 0
     assert trim_percentile < 40  # typically a max of 10 to 20 is advised.
     lower_spec, upper_spec = specifications
 
     if lower_spec is None:
-        Cpk_lower_spec = float(
-            np.nanpercentile(df[which_column].values, [trim_percentile])
-        )
+        Cpk_lower_spec = float(np.nanpercentile(df[which_column].values, [trim_percentile]))
     elif isinstance(lower_spec, str):
         Cpk_lower_spec = df[lower_spec]
     else:
         Cpk_lower_spec = float(lower_spec)
 
     if upper_spec is None:
-        Cpk_upper_spec = float(
-            np.nanpercentile(df[which_column].values, [100 - trim_percentile])
-        )
+        Cpk_upper_spec = float(np.nanpercentile(df[which_column].values, [100 - trim_percentile]))
     elif isinstance(upper_spec, str):
         Cpk_upper_spec = df[upper_spec]
     else:
         Cpk_upper_spec = float(upper_spec)
 
     metric_lower = df[which_column] - Cpk_lower_spec
     metric_upper = Cpk_upper_spec - df[which_column]
@@ -66,11 +62,9 @@
         center_lower, center_upper = metric_lower.median(), metric_upper.median()
         spread_lower, spread_upper = Sn(metric_lower), Sn(metric_upper)
     else:
         center_lower, center_upper = metric_lower.mean(), metric_upper.mean()
         spread_lower, spread_upper = metric_lower.std(), metric_upper.std()
 
     # TODO: return the RSD also: rsd = (spread / center) * 100
-    Cpk = np.nanmin(
-        [center_lower / (3 * spread_lower), center_upper / (3 * spread_upper)]
-    )
+    Cpk = np.nanmin([center_lower / (3 * spread_lower), center_upper / (3 * spread_upper)])
     return Cpk
```

### Comparing `process-improve-0.9.64/process_improve/multivariate/methods.py` & `process-improve-0.9.65/process_improve/multivariate/methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# (c) Kevin Dunn, 2010-2022. MIT License. Based on own private work over the years.
+# (c) Kevin Dunn, 2010-2023. MIT License. Based on own private work over the years.
 import time
 import warnings
 from functools import partial
 from typing import Any, Optional
 
 import numpy as np
 import pandas as pd
@@ -163,17 +163,15 @@
         self.Hotellings_T2 = pd.DataFrame(
             np.zeros(shape=(self.N, self.A)),
             columns=component_names,
             index=X.index,
             # name="Hotelling's T^2 statistic, per component",
         )
         if self.has_missing_data:
-            self.x_scores = pd.DataFrame(
-                self.x_scores_, columns=component_names, index=X.index
-            )
+            self.x_scores = pd.DataFrame(self.x_scores_, columns=component_names, index=X.index)
             self.squared_prediction_error = pd.DataFrame(
                 self.squared_prediction_error_,
                 columns=component_names,
                 index=X.index.copy(),
             )
             self.R2 = pd.Series(
                 self.R2_,
@@ -188,17 +186,15 @@
             self.R2X_cum = pd.DataFrame(
                 self.R2X_cum_,
                 columns=component_names,
                 index=X.columns,
                 # name ="Per variable R^2, per component"
             )
         else:
-            self.x_scores = pd.DataFrame(
-                super().fit_transform(X), columns=component_names, index=X.index
-            )
+            self.x_scores = pd.DataFrame(super().fit_transform(X), columns=component_names, index=X.index)
             self.squared_prediction_error = pd.DataFrame(
                 np.zeros((self.N, self.A)),
                 columns=component_names,
                 index=X.index.copy(),
             )
             self.R2 = pd.Series(
                 np.zeros(shape=(self.A,)),
@@ -242,16 +238,15 @@
                 else:
                     self.R2.iloc[a] = self.R2cum.iloc[a]
         # end: has no missing data
 
         for a in range(self.A):
             self.Hotellings_T2.iloc[:, a] = (
                 self.Hotellings_T2.iloc[:, max(0, a - 1)]
-                + (self.x_scores.iloc[:, a] / self.scaling_factor_for_scores.iloc[a])
-                ** 2
+                + (self.x_scores.iloc[:, a] / self.scaling_factor_for_scores.iloc[a]) ** 2
             )
 
         # Replace `self.loadings` with self.x_loadings
         self.x_loadings = self.loadings
         self.ellipse_coordinates = partial(
             ellipse_coordinates,
             n_components=self.n_components,
@@ -279,32 +274,28 @@
         class State(object):
             """Class object to hold the prediction results together."""
 
             pass
 
         state = State()
         state.N, state.K = X.shape
-        assert (
-            self.K == state.K
-        ), "Prediction data must have same number of columns as training data."
+        assert self.K == state.K, "Prediction data must have same number of columns as training data."
 
         state.x_scores = X @ self.x_loadings
 
         # TODO: handle the missing data version here still
         for a in range(self.A):
             pass
             # p = self.x_loadings.iloc[:, [a]]
             # temp = X @ self.x_loadings.iloc[:, [a]]
             # X_mcuv -= temp @ p.T
             # state.x_scores[:, [a]] = temp
 
         # Scores are calculated, now do the rest
-        state.Hotellings_T2 = np.sum(
-            np.power((state.x_scores / self.scaling_factor_for_scores.values), 2), 1
-        )
+        state.Hotellings_T2 = np.sum(np.power((state.x_scores / self.scaling_factor_for_scores.values), 2), 1)
         # Calculate SPE-residuals (sum over rows of the errors)
         X_mcuv = X.copy()
         X_mcuv -= state.x_scores @ self.x_loadings.T
         state.squared_prediction_error = np.sqrt(np.power(X_mcuv, 2).sum(axis=1))
         return state
 
 
@@ -329,31 +320,24 @@
         n_components=None,
         copy: bool = True,
         missing_data_settings=dict,
     ):
         self.n_components = n_components
         self.missing_data_settings = missing_data_settings
         self.has_missing_data = True
-        self.missing_data_settings["md_max_iter"] = int(
-            self.missing_data_settings["md_max_iter"]
-        )
+        self.missing_data_settings["md_max_iter"] = int(self.missing_data_settings["md_max_iter"])
 
-        assert (
-            self.missing_data_settings["md_tol"] < 10
-        ), "Tolerance should not be too large"
-        assert (
-            self.missing_data_settings["md_tol"] > epsqrt**1.95
-        ), "Tolerance must exceed machine precision"
+        assert self.missing_data_settings["md_tol"] < 10, "Tolerance should not be too large"
+        assert self.missing_data_settings["md_tol"] > epsqrt**1.95, "Tolerance must exceed machine precision"
 
         assert self.missing_data_settings["md_method"] in self.valid_md_methods, (
             f"Missing data method is not recognized. Must be one of {self.valid_md_methods}.",
         )
 
     def fit(self, X, y=None):
-
         # Force input to NumPy array:
         self.data = np.asarray(X.copy())
 
         # Other setups:
         self.n_components = self.A
         self.n_samples_ = self.N
         self.n_features_ = self.K
@@ -382,17 +366,15 @@
             "R2cum_",
             "R2X_cum_",
             "squared_prediction_error_",
         ]
         assert all([getattr(self, attr, None) is not None for attr in required_fields])
 
         # Additional calculations, which can be done after the missing data method is complete.
-        self.explained_variance_ = np.diag(self.x_scores_.T @ self.x_scores_) / (
-            self.N - 1
-        )
+        self.explained_variance_ = np.diag(self.x_scores_.T @ self.x_scores_) / (self.N - 1)
         return self
 
     def transform(self, X):
         check_is_fitted(self, "blah")
 
         X = X.copy()
         return X
@@ -416,15 +398,14 @@
 
         # Initialize storage:
         self.extra_info = {}
         self.extra_info["timing"] = np.zeros(A) * np.nan
         self.extra_info["iterations"] = np.zeros(A) * np.nan
 
         for a in np.arange(A):
-
             # Timers and housekeeping
             start_time = time.time()
             itern = 0
             start_SS_col = ssq(Xd, axis=0)
 
             if sum(start_SS_col) < epsqrt:
                 emsg = (
@@ -436,18 +417,15 @@
             # Initialize t_a with random numbers, or carefully select a column
             # from X. <-- Don't do this anymore.
             # Rather: Pick a column from X as the initial guess instead.
             t_a_guess = Xd[:, [0]]  # .reshape(self.N, 1)
             t_a_guess[np.isnan(t_a_guess)] = 0
             t_a = t_a_guess + 1.0
             p_a = np.zeros((K, 1))
-            while not (
-                terminate_check(t_a_guess, t_a, iterations=itern, settings=settings)
-            ):
-
+            while not (terminate_check(t_a_guess, t_a, iterations=itern, settings=settings)):
                 # 0: Richardson's acceleration, or any numerical acceleration
                 #    method for PCA where there is slow convergence?
 
                 # 0: starting point for convergence checking on next loop
                 t_a_guess = t_a.copy()
 
                 # 1: Regress the score, t_a, onto every column in X, compute the
@@ -554,28 +532,24 @@
         _, _, V = np.linalg.svd(S, full_matrices=False)
         self.extra_info["iterations"] = itern
         self.extra_info["timing"] = time.time() - start_time
         self.x_loadings = (V[0:A, :]).T  # transpose result to the right shape: K x A
         self.x_scores_ = (Xd - np.mean(Xd, axis=0)) @ self.x_loadings
 
         for a in range(A):
-            residuals = (
-                self.x_scores_[:, : a + 1] @ self.x_loadings[:, : a + 1].T - self.data
-            )
+            residuals = self.x_scores_[:, : a + 1] @ self.x_loadings[:, : a + 1].T - self.data
             self.R2cum_[a] = 1 - ssq(residuals, axis=None) / base_variance
             if a > 0:
                 self.R2_[a] = self.R2cum_[a] - self.R2cum_[a - 1]
             else:
                 self.R2_[a] = self.R2cum_[a]
 
             # Per component, what is the SPE? We define SPE as a standard deviation like quantity.
             # So take the square root of the sum of squares of the residuals.
-            self.squared_prediction_error_[:, a] = np.sqrt(
-                ssq(residuals, axis=1)
-            )  # N x A matrix
+            self.squared_prediction_error_[:, a] = np.sqrt(ssq(residuals, axis=1))  # N x A matrix
 
 
 class PLS(PLS_sklearn):
     def __init__(
         self,
         n_components: int = 2,
         *,
@@ -621,16 +595,15 @@
 
         Abdi, "Partial least squares regression and projection on latent structure
         regression (PLS Regression)", 2010, DOI: 10.1002/wics.51
         """
         self.N, self.K = X.shape
         self.Ny, self.M = Y.shape
         assert self.Ny == self.N, (
-            f"The X and Y arrays must have the same number of rows: X has {self.N} and "
-            f"Y has {self.Ny}."
+            f"The X and Y arrays must have the same number of rows: X has {self.N} and " f"Y has {self.Ny}."
         )
 
         # Check if number of components is supported against maximum requested
         min_dim = min(self.N, self.K)
         self.A = min_dim if self.n_components is None else int(self.n_components)
         if self.A > min_dim:
             warn = (
@@ -645,17 +618,15 @@
         if np.any(Y.isna()) or np.any(X.isna()):
             # If there are missing data, then the missing data settings apply. Defaults are:
             #
             #       md_method = "tsr"
             #       md_tol = np.sqrt(np.finfo(float).eps)
             #       md_max_iter = self.max_iter
 
-            default_mds = dict(
-                md_method="tsr", md_tol=epsqrt, md_max_iter=self.max_iter
-            )
+            default_mds = dict(md_method="tsr", md_tol=epsqrt, md_max_iter=self.max_iter)
             if isinstance(self.missing_data_settings, dict):
                 default_mds.update(self.missing_data_settings)
 
             self.missing_data_settings = default_mds
             self = PLS_missing_values(
                 n_components=self.n_components,
                 missing_data_settings=self.missing_data_settings,
@@ -680,53 +651,31 @@
             self.extra_info["iterations"] = np.array(self.n_iter_)
 
         # We have now fitted the model. Apply some convenience shortcuts for the user.
         self.A = self.n_components
 
         # Further convenience calculations
         # "direct_weights" is matrix R = W(P'W)^{-1}  [R is KxA matrix]; useful since T = XR
-        direct_weights = self.x_weights_ @ np.linalg.inv(
-            self.x_loadings_.T @ self.x_weights_
-        )
+        direct_weights = self.x_weights_ @ np.linalg.inv(self.x_loadings_.T @ self.x_weights_)
         # beta = RC' [KxA by AxM = KxM]: the KxM matrix gives the direct link from the k-th (input)
         # X variable, to the m-th (output) Y variable.
         beta_coefficients = direct_weights @ self.y_loadings_.T
 
         # Initialize storage:
         component_names = [a + 1 for a in range(self.A)]
-        self.x_scores = pd.DataFrame(
-            self.x_scores_, index=X.index, columns=component_names
-        )
-        self.y_scores = pd.DataFrame(
-            self.y_scores_, index=Y.index, columns=component_names
-        )
-        self.x_weights = pd.DataFrame(
-            self.x_weights_, index=X.columns, columns=component_names
-        )
-        self.y_weights = pd.DataFrame(
-            self.y_weights_, index=Y.columns, columns=component_names
-        )
-        self.x_loadings = pd.DataFrame(
-            self.x_loadings_, index=X.columns, columns=component_names
-        )
-        self.y_loadings = pd.DataFrame(
-            self.y_loadings_, index=Y.columns, columns=component_names
-        )
-        self.predictions = pd.DataFrame(
-            self.x_scores @ self.y_loadings.T, index=Y.index, columns=Y.columns
-        )
-        self.direct_weights = pd.DataFrame(
-            direct_weights, index=X.columns, columns=component_names
-        )
-        self.beta_coefficients = pd.DataFrame(
-            beta_coefficients, index=X.columns, columns=Y.columns
-        )
-        self.explained_variance = np.diag(self.x_scores.T @ self.x_scores) / (
-            self.N - 1
-        )
+        self.x_scores = pd.DataFrame(self.x_scores_, index=X.index, columns=component_names)
+        self.y_scores = pd.DataFrame(self.y_scores_, index=Y.index, columns=component_names)
+        self.x_weights = pd.DataFrame(self.x_weights_, index=X.columns, columns=component_names)
+        self.y_weights = pd.DataFrame(self.y_weights_, index=Y.columns, columns=component_names)
+        self.x_loadings = pd.DataFrame(self.x_loadings_, index=X.columns, columns=component_names)
+        self.y_loadings = pd.DataFrame(self.y_loadings_, index=Y.columns, columns=component_names)
+        self.predictions = pd.DataFrame(self.x_scores @ self.y_loadings.T, index=Y.index, columns=Y.columns)
+        self.direct_weights = pd.DataFrame(direct_weights, index=X.columns, columns=component_names)
+        self.beta_coefficients = pd.DataFrame(beta_coefficients, index=X.columns, columns=Y.columns)
+        self.explained_variance = np.diag(self.x_scores.T @ self.x_scores) / (self.N - 1)
         self.scaling_factor_for_scores = pd.Series(
             np.sqrt(self.explained_variance),
             index=component_names,
             name="Standard deviation per score",
         )
         self.Hotellings_T2 = pd.DataFrame(
             np.zeros(shape=(self.N, self.A)),
@@ -762,34 +711,28 @@
         )
         self.R2Y_cum.index.name = "R^2 per variable (row), per component (col)"
         self.RMSE = pd.DataFrame(
             np.zeros(shape=(self.M, self.A)),
             index=Y.columns.copy(),
             columns=component_names,
         )
-        self.RMSE.index.name = (
-            "Root mean square error per variable (row), per component (col)"
-        )
+        self.RMSE.index.name = "Root mean square error per variable (row), per component (col)"
 
         Xd = X.copy()
         Yd = Y.copy()
         prior_SSX_col = ssq(Xd.values, axis=0)
         prior_SSY_col = ssq(Yd.values, axis=0)
         base_variance_Y = np.sum(prior_SSY_col)
         for a in range(self.A):
             self.Hotellings_T2.iloc[:, a] = (
                 self.Hotellings_T2.iloc[:, max(0, a - 1)]
-                + (self.x_scores.iloc[:, a] / self.scaling_factor_for_scores.iloc[a])
-                ** 2
+                + (self.x_scores.iloc[:, a] / self.scaling_factor_for_scores.iloc[a]) ** 2
             )
             Xd -= self.x_scores.iloc[:, [a]] @ self.x_loadings.iloc[:, [a]].T
-            y_hat = (
-                self.x_scores.iloc[:, 0 : (a + 1)]
-                @ self.y_loadings.iloc[:, 0 : (a + 1)].T
-            )
+            y_hat = self.x_scores.iloc[:, 0 : (a + 1)] @ self.y_loadings.iloc[:, 0 : (a + 1)].T
             # These are the Residual Sums of Squares (RSS); i.e X-X_hat
             row_SSX = ssq(Xd.values, axis=1)
             col_SSX = ssq(Xd.values, axis=0)
             row_SSY = ssq(y_hat.values, axis=1)
             col_SSY = ssq(y_hat.values, axis=0)
             # R2 and cumulative R2 value for the whole block
             self.R2cum.iloc[a] = sum(row_SSY) / base_variance_Y
@@ -831,33 +774,29 @@
         class State(object):
             """Class object to hold the prediction results together."""
 
             pass
 
         state = State()
         state.N, state.K = X.shape
-        assert (
-            self.K == state.K
-        ), "Prediction data must have same number of columns as training data."
+        assert self.K == state.K, "Prediction data must have same number of columns as training data."
 
         state.x_scores = X @ self.direct_weights
 
         # TODO: handle the missing data version here still
         for a in range(self.A):
             pass
             # p = self.x_loadings.iloc[:, [a]]
             # w = self.x_weights.iloc[:, [a]]
             # temp = X @ self.direct_weights.iloc[:, [a]]
             # X_mcuv -= temp @ p.T
             # state.x_scores[:, [a]] = temp
 
         # Scores are calculated, now do the rest
-        state.Hotellings_T2 = np.sum(
-            np.power((state.x_scores / self.scaling_factor_for_scores.values), 2), 1
-        )
+        state.Hotellings_T2 = np.sum(np.power((state.x_scores / self.scaling_factor_for_scores.values), 2), 1)
         # Calculate SPE-residuals (sum over rows of the errors)
         X_mcuv = X.copy()
         X_mcuv -= state.x_scores @ self.x_loadings.T
         state.squared_prediction_error = np.sqrt(np.power(X_mcuv, 2).sum(axis=1))
         # Predicted values from the model (user still has to un-preprocess these predictions!)
         state.y_hat = state.x_scores @ self.y_loadings.T
 
@@ -897,24 +836,18 @@
         n_components=None,
         copy: bool = True,
         missing_data_settings=dict,
     ):
         self.n_components = n_components
         self.missing_data_settings = missing_data_settings
         self.has_missing_data = True
-        self.missing_data_settings["md_max_iter"] = int(
-            self.missing_data_settings["md_max_iter"]
-        )
+        self.missing_data_settings["md_max_iter"] = int(self.missing_data_settings["md_max_iter"])
 
-        assert (
-            self.missing_data_settings["md_tol"] < 10
-        ), "Tolerance should not be too large"
-        assert (
-            self.missing_data_settings["md_tol"] > epsqrt**1.95
-        ), "Tolerance must exceed machine precision"
+        assert self.missing_data_settings["md_tol"] < 10, "Tolerance should not be too large"
+        assert self.missing_data_settings["md_tol"] > epsqrt**1.95, "Tolerance must exceed machine precision"
 
         assert self.missing_data_settings["md_method"] in self.valid_md_methods, (
             f"Missing data method is not recognized. Must be one of {self.valid_md_methods}.",
         )
 
     def fit(self, X, Y):
         """
@@ -979,15 +912,14 @@
 
         # Initialize storage:
         self.extra_info = {}
         self.extra_info["timing"] = np.zeros(A) * np.nan
         self.extra_info["iterations"] = np.zeros(A) * np.nan
 
         for a in np.arange(A):
-
             # Timers and housekeeping
             start_time = time.time()
             itern = 0
 
             start_SSX_col = ssq(self.Xd, axis=0)
             start_SSY_col = ssq(self.Yd, axis=0)
 
@@ -1007,18 +939,15 @@
             # Initialize t_a with random numbers, or carefully select a column from X or Y?
             # Find a column with the largest variance as t1_start; replace missing with zeros
             # All columns have the same variance if the data have been scaled to unit variance!
             u_a_guess = self.Yd[:, [0]]
             u_a_guess[np.isnan(u_a_guess)] = 0
             u_a = u_a_guess + 1.0
 
-            while not (
-                terminate_check(u_a_guess, u_a, iterations=itern, settings=settings)
-            ):
-
+            while not (terminate_check(u_a_guess, u_a, iterations=itern, settings=settings)):
                 # 0: starting point for convergence checking on next loop
                 u_a_guess = u_a.copy()
 
                 # 1: Regress the score, u_a, onto every column in X, compute the
                 #    regression coefficient and store in w_a
                 # w_a = X.T * u_a / (u_a.T * u_a)
                 w_a = quick_regress(self.Xd, u_a)
@@ -1045,17 +974,15 @@
 
                 itern += 1
 
             self.extra_info["timing"][a] = time.time() - start_time
             self.extra_info["iterations"][a] = itern
 
             if itern > settings["md_max_iter"]:
-                Warning(
-                    "PLS missing data [SCP method]: maximum number of iterations reached!"
-                )
+                Warning("PLS missing data [SCP method]: maximum number of iterations reached!")
 
             # Loop terminated!
             # 6: Now deflate the X-matrix.  To do that we need to calculate loadings for the
             # X-space.  Regress columns of t_a onto each column in X and calculate loadings, p_a.
             # Use this p_a to deflate afterwards.
             p_a = quick_regress(self.Xd, t_a)  # Note the similarity with step 4!
             self.Xd -= np.dot(t_a, p_a.T)  # and that similarity helps understand
@@ -1111,17 +1038,15 @@
     out = 0.0
     if axis is None:
         out = np.nansum(X**2)
 
     return out
 
 
-def terminate_check(
-    t_a_guess: np.ndarray, t_a: np.ndarray, iterations: int, settings: dict
-) -> bool:
+def terminate_check(t_a_guess: np.ndarray, t_a: np.ndarray, iterations: int, settings: dict) -> bool:
     """The PCA iterative algorithm is terminated when any one of these conditions is True:
 
     #. scores converge: the norm between two successive iterations
     #. maximum number of iterations is reached
     """
     score_tol = np.linalg.norm(t_a_guess - t_a, ord=None)
     converged = score_tol < settings["md_tol"]
@@ -1355,17 +1280,15 @@
     assert score_horiz <= n_components
     assert score_vert <= n_components
     assert T2_limit_conf_level > 0
     assert T2_limit_conf_level < 1
     assert n_rows > 0
     s_h = scaling_factor_for_scores.iloc[score_horiz - 1]
     s_v = scaling_factor_for_scores.iloc[score_vert - 1]
-    T2_limit_specific = np.sqrt(
-        T2_limit(T2_limit_conf_level, n_components=n_components, n_rows=n_rows)
-    )
+    T2_limit_specific = np.sqrt(T2_limit(T2_limit_conf_level, n_components=n_components, n_rows=n_rows))
     dt = 2 * np.pi / (n_points - 1)
     steps = np.linspace(0, n_points - 1, n_points)
     x = np.cos(steps * dt) * T2_limit_specific * s_h
     y = np.sin(steps * dt) * T2_limit_specific * s_v
     return x, y
```

### Comparing `process-improve-0.9.64/process_improve/multivariate/plots.py` & `process-improve-0.9.65/process_improve/multivariate/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 # -*- coding: utf-8 -*-
-# (c) Kevin Dunn, 2010-2022. MIT License. Based on own private work over the years.
+# (c) Kevin Dunn, 2010-2023. MIT License. Based on own private work over the years.
 
 # Built-in libraries
 import json
 from typing import Dict
 
 import plotly.graph_objects as go
 from pydantic import BaseModel, validator
 
 
 def plot_pre_checks(model, pc_horiz, pc_vert, pc_depth) -> bool:
-    assert (
-        0 < pc_horiz <= model.A
-    ), f"The model has {model.A} components. Ensure that 1 <= pc_horiz<={model.A}."
-    assert (
-        0 < pc_vert <= model.A
-    ), f"The model has {model.A} components. Ensure that 1 <= pc_vert<={model.A}."
-    assert (
-        -1 <= pc_depth <= model.A
-    ), f"The model has {model.A} components. Ensure that 1 <= pc_depth<={model.A}."
-    assert (
-        len(set([pc_horiz, pc_vert, pc_depth])) == 3
-    ), "Specify distinct components for each axis"
+    assert 0 < pc_horiz <= model.A, f"The model has {model.A} components. Ensure that 1 <= pc_horiz<={model.A}."
+    assert 0 < pc_vert <= model.A, f"The model has {model.A} components. Ensure that 1 <= pc_vert<={model.A}."
+    assert -1 <= pc_depth <= model.A, f"The model has {model.A} components. Ensure that 1 <= pc_depth<={model.A}."
+    assert len(set([pc_horiz, pc_vert, pc_depth])) == 3, "Specify distinct components for each axis"
 
     return True
 
 
 def score_plot(
     model,
     pc_horiz: int = 1,
@@ -106,27 +98,23 @@
         setdict = Settings(**settings).dict()
     else:
         setdict = Settings().dict()
     if fig is None:
         fig = go.Figure()
 
     name = "X-space scores [T]"
-    fig.update_layout(
-        xaxis_title_text=f"PC {pc_horiz}", yaxis_title_text=f"PC {pc_vert}"
-    )
+    fig.update_layout(xaxis_title_text=f"PC {pc_horiz}", yaxis_title_text=f"PC {pc_vert}")
 
     highlights: Dict[str, list] = {}
     default_index = model.x_scores.index
     if items_to_highlight is not None:
         highlights = items_to_highlight.copy()
         for key, items in items_to_highlight.items():
             highlights[key] = list(set(items) & set(default_index))
-            default_index = (set(default_index) ^ set(highlights[key])) & set(
-                default_index
-            )
+            default_index = (set(default_index) ^ set(highlights[key])) & set(default_index)
 
     # Ensure it is back to a list
     default_index = list(default_index)
 
     # 3D plot
     if pc_depth >= 1:
         fig.add_trace(
@@ -255,17 +243,15 @@
                     gridwidth=1,
                 ),
             ),
         )
     return fig
 
 
-def loadings_plot(
-    model, loadings_type="p", pc_horiz=1, pc_vert=2, settings: Dict = None, fig=None
-) -> go.Figure:
+def loadings_plot(model, loadings_type="p", pc_horiz=1, pc_vert=2, settings: Dict = None, fig=None) -> go.Figure:
     """Generates a 2-dimensional loadings for the given latent variable model.
 
     Parameters
     ----------
     model : MVmodel object (PCA, or PLS)
         A latent variable model generated by this library.
 
@@ -299,18 +285,15 @@
 
         }
     """
     plot_pre_checks(model, pc_horiz, pc_vert, pc_depth=0)
     margin_dict: Dict = dict(l=10, r=10, b=5, t=80)  # Defaults: l=80, r=80, t=100, b=80
 
     class Settings(BaseModel):
-        title: str = (
-            f"Loadings plot [{loadings_type.upper()}] of component {pc_horiz} vs "
-            f"component {pc_vert}"
-        )
+        title: str = f"Loadings plot [{loadings_type.upper()}] of component {pc_horiz} vs " f"component {pc_vert}"
         show_labels: bool = True
         html_image_height: float = 500.0
         html_aspect_ratio_w_over_h: float = 16 / 9.0
 
     if settings:
         setdict = Settings(**settings).dict()
     else:
@@ -368,17 +351,15 @@
                     size=8,
                 ),
                 text=extra.index,
                 textposition="bottom center",
             )
         )
 
-    fig.update_layout(
-        xaxis_title_text=f"PC {pc_horiz}", yaxis_title_text=f"PC {pc_vert}"
-    )
+    fig.update_layout(xaxis_title_text=f"PC {pc_horiz}", yaxis_title_text=f"PC {pc_vert}")
     fig.add_hline(y=0, line_color="black")
     fig.add_vline(x=0, line_color="black")
     fig.update_layout(
         title_text=setdict["title"],
         margin=margin_dict,
         hovermode="closest",
         showlegend=add_legend,
@@ -502,17 +483,15 @@
     name = f"SPE values after {with_a} component{'s' if with_a > 1 else ''}"
     highlights: Dict[str, list] = {}
     default_index = model.squared_prediction_error.index
     if items_to_highlight is not None:
         highlights = items_to_highlight.copy()
         for key, items in items_to_highlight.items():
             highlights[key] = list(set(items) & set(default_index))
-            default_index = (set(default_index) ^ set(highlights[key])) & set(
-                default_index
-            )
+            default_index = (set(default_index) ^ set(highlights[key])) & set(default_index)
 
     # Ensure it is back to a list
     default_index = list(default_index)
     fig.add_trace(
         go.Scatter(
             x=default_index,
             y=model.squared_prediction_error.loc[default_index, with_a],
@@ -669,17 +648,15 @@
     name = f"T2 values after {with_a} component{'s' if with_a > 1 else ''}"
     highlights: Dict[str, list] = {}
     default_index = model.Hotellings_T2.index
     if items_to_highlight is not None:
         highlights = items_to_highlight.copy()
         for key, items in items_to_highlight.items():
             highlights[key] = list(set(items) & set(default_index))
-            default_index = (set(default_index) ^ set(highlights[key])) & set(
-                default_index
-            )
+            default_index = (set(default_index) ^ set(highlights[key])) & set(default_index)
 
     # Ensure it is back to a list
     default_index = list(default_index)
     fig.add_trace(
         go.Scatter(
             x=default_index,
             y=model.Hotellings_T2.loc[default_index, with_a],
```

### Comparing `process-improve-0.9.64/process_improve/regression/methods.py` & `process-improve-0.9.65/process_improve/regression/methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,15 @@
     intercept. Returns a list: [intercept, slope] of the fit. No extra
     checking on data consistency is done.
 
     See also:
 
     regression.repeated_median_slope
     """
-    rlm_model = sm.RLM(
-        y, np.vstack([np.ones(x.size), x.ravel()]).T, M=sm.robust.norms.HuberT()
-    )
+    rlm_model = sm.RLM(y, np.vstack([np.ones(x.size), x.ravel()]).T, M=sm.robust.norms.HuberT())
     rlm_results = rlm_model.fit()
     return rlm_results.params
 
 
 def repeated_median_slope(x, y, nowarn=False):
     """
     Robust slope calculation.
@@ -53,17 +51,15 @@
                 inner_medians.append((y[j] - y[i]) / den)
 
         medians.append(np.nanmedian(inner_medians))
 
     return np.nanmedian(medians)
 
 
-def simple_robust_regression(
-    x, y, na_rm=None, conflevel=0.95, nowarn=False, pi_resolution=50
-):
+def simple_robust_regression(x, y, na_rm=None, conflevel=0.95, nowarn=False, pi_resolution=50):
     """
     x and y: iterables
     na_rm: None; no effect for robust regression. Here for consistency with the non-robust case.
     nowarn: If True, then no error checking/warnings are issued. The user is committing to do that
     themselves ahead of time.
 
     TODO: handle the missing values case still. See the `multiple_linear_regression` function,
@@ -83,17 +79,15 @@
     slope = repeated_median_slope(x, y, nowarn=nowarn)
     intercept = np.nanmedian(y - slope * x)
     mean_x, mean_y = np.mean(x), np.mean(y)
     total_ssq = np.sum(np.power(y - mean_y, 2))
 
     out = {}
 
-    out["N"] = min(
-        x.size - np.count_nonzero(np.isnan(x)), y.size - np.count_nonzero(np.isnan(y))
-    )
+    out["N"] = min(x.size - np.count_nonzero(np.isnan(x)), y.size - np.count_nonzero(np.isnan(y)))
     out["intercept"] = intercept
     out["coefficients"] = [
         slope,
     ]
     out["fitted_values"] = intercept + slope * x
     regression_ssq = np.sum(np.power(out["fitted_values"] - mean_y, 2))
     out["residuals"] = y - out["fitted_values"]
@@ -114,23 +108,19 @@
         out["standard_error_intercept"] = SE_b0 = np.NaN
         out["standard_errors"] = [
             np.NaN,
         ]
         out["pi_range"] = np.vstack([pi_range, pi_y_pred, pi_y_pred]).T
 
     else:
-        out["standard_error_intercept"] = SE_b0 = out["SE"] * np.sqrt(
-            (1 / out["N"] + (mean_x) ** 2 / out["x_ssq"])
-        )
+        out["standard_error_intercept"] = SE_b0 = out["SE"] * np.sqrt((1 / out["N"] + (mean_x) ** 2 / out["x_ssq"]))
         out["standard_errors"] = [
             out["SE"] * 1 / np.sqrt(out["x_ssq"]),
         ]
-        var_y = (out["SE"] ** 2) * (
-            1 + 1 / out["N"] + (pi_range - np.mean(x)) ** 2 / out["x_ssq"]
-        )
+        var_y = (out["SE"] ** 2) * (1 + 1 / out["N"] + (pi_range - np.mean(x)) ** 2 / out["x_ssq"])
         std_y = np.sqrt(var_y)
         lower = pi_y_pred - c_t * std_y
         upper = pi_y_pred + c_t * std_y
         out["pi_range"] = np.vstack([pi_range, lower, upper]).T
 
     out["conf_interval_intercept"] = np.array(
         [out["intercept"] - c_t * SE_b0, out["intercept"] + c_t * SE_b0],
@@ -145,25 +135,21 @@
     )
     out["leverage"] = 1 / out["N"] + np.power(x - mean_x, 2) / out["x_ssq"]
     out["k"] = 2
     if out["SE"] < __eps:
         out["influence"] = out["residuals"] * 0.0
     else:
         out["influence"] = (
-            np.power(out["residuals"] / ((1 - out["leverage"]) * out["SE"]), 2)
-            * out["leverage"]
-            / out["k"]
+            np.power(out["residuals"] / ((1 - out["leverage"]) * out["SE"]), 2) * out["leverage"] / out["k"]
         )
 
     return out
 
 
-def multiple_linear_regression(
-    X, y, fit_intercept=True, na_rm=True, conflevel=0.95, pi_resolution=50
-):
+def multiple_linear_regression(X, y, fit_intercept=True, na_rm=True, conflevel=0.95, pi_resolution=50):
     """
     Linear regression of the N rows and K columns of matrix `X` onto the single column 'y'.
 
     The matrix `X` will be augmented with a column of 1's if `fit_intercept` is True.
     `na_rm`: True:  removes all observations with one or more missing values.
 
     Notes and limitations:
@@ -246,27 +232,23 @@
     x_vector = X_.copy()
     if fit_intercept:
         # Was this: X_ = sm.add_constant(X_); but this created warnings/noise.
         X_["__constant__"] = 1.0
         X_.insert(0, "__constant__", X_.pop("__constant__"))
         k = k + 1
 
-    assert (
-        out["N"] >= k
-    ), "N >= K: You need at least as many rows as there are columns to fit a linear regression."
+    assert out["N"] >= k, "N >= K: You need at least as many rows as there are columns to fit a linear regression."
     assert out["N"] == y_.size
 
     if x_vector.shape[1] == 1:
         mean_X = np.mean(x_vector, axis=0)
         out["x_ssq"] = np.sum(np.power(x_vector - mean_X, 2))[0]
 
         # Can be calculated before the model is even fit:
-        out["leverage"] = (
-            1 / out["N"] + np.power(x_vector - mean_X, 2) / out["x_ssq"]
-        ).values.ravel()
+        out["leverage"] = (1 / out["N"] + np.power(x_vector - mean_X, 2) / out["x_ssq"]).values.ravel()
 
     # Do the work
     model = sm.OLS(y_, X_)
     results = model.fit()
 
     #  Report the results:
     if fit_intercept:
@@ -283,46 +265,34 @@
         out["standard_errors"] = results._results.bse[:]
         out["conf_intervals"] = results._results.conf_int(alpha)
 
     out["fitted_values"] = results._results.fittedvalues
     out["R2"] = results._results.rsquared
     regression_ssq = np.sum(np.power(out["fitted_values"] - mean_y, 2))
 
-    out["residuals"] = (
-        np.nan * np.ones((1, len(y))).ravel()
-    )  # NOTE: the original y-shape is used, not y_'s shape!
+    out["residuals"] = np.nan * np.ones((1, len(y))).ravel()  # NOTE: the original y-shape is used, not y_'s shape!
     # residuals are defined as: y.values.ravel() - out["fitted_values"]
     out["residuals"][~missing_idx] = results._results.resid
     residual_ssq = np.nansum(out["residuals"] * out["residuals"])
     out["R2_regression_based"] = regression_ssq / total_ssq
     out["R2_residual_based"] = 1 - (residual_ssq / total_ssq)
     out["SE"] = np.sqrt(results._results.scale)  # np.sqrt(residual_ssq / (len(x_) - 2))
     out["k"] = k
 
     if x_vector.shape[1] == 1 and fit_intercept:
         # "pi" = prediction interval
-        pi_range = np.linspace(
-            np.min(X_.values[:, 1]), np.max(X_.values[:, 1]), pi_resolution
-        )
+        pi_range = np.linspace(np.min(X_.values[:, 1]), np.max(X_.values[:, 1]), pi_resolution)
         pi_y_pred = out["intercept"] + out["coefficients"][0] * pi_range
         if out["SE"] < __eps:
             out["influence"] = out["residuals"] * 0.0
         else:
             out["influence"] = (
-                np.power(
-                    results._results.resid / ((1 - out["leverage"]) * out["SE"]), 2
-                )
-                * out["leverage"]
-                / k
-            )
-            var_y = (out["SE"] ** 2) * (
-                1
-                + 1 / out["N"]
-                + (pi_range - np.mean(X_.values[:, 1])) ** 2 / out["x_ssq"]
+                np.power(results._results.resid / ((1 - out["leverage"]) * out["SE"]), 2) * out["leverage"] / k
             )
+            var_y = (out["SE"] ** 2) * (1 + 1 / out["N"] + (pi_range - np.mean(X_.values[:, 1])) ** 2 / out["x_ssq"])
             std_y = np.sqrt(var_y)
             c_t = t_value(1 - (1 - conflevel) / 2, out["N"] - 2)  # 2 fitted parameters
             lower = pi_y_pred - c_t * std_y
             upper = pi_y_pred + c_t * std_y
             out["pi_range"] = np.vstack([pi_range, lower, upper]).T
 
     return out
```

### Comparing `process-improve-0.9.64/process_improve/univariate/metrics.py` & `process-improve-0.9.65/process_improve/univariate/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,17 +176,15 @@
 
 def _contains_nan(a, nan_policy="propagate"):
     """
     From scipy.stats.stats
     """
     policies = ["propagate", "raise", "omit"]
     if nan_policy not in policies:
-        raise ValueError(
-            "nan_policy must be one of {%s}" % ", ".join("'%s'" % s for s in policies)
-        )
+        raise ValueError("nan_policy must be one of {%s}" % ", ".join("'%s'" % s for s in policies))
     try:
         # Calling np.sum to avoid creating a huge array into memory
         # e.g. np.isnan(a).any()
         with np.errstate(invalid="ignore"):
             contains_nan = np.isnan(np.sum(a))
     except TypeError:
         # This can happen when attempting to sum things which are not
@@ -195,16 +193,15 @@
             contains_nan = np.nan in set(a.ravel())
         except TypeError:  # pragma: no cover
             # Don't know what to do. Fall back to omitting nan values and
             # issue a warning.
             contains_nan = False
             nan_policy = "omit"
             warnings.warn(
-                "The input array could not be properly checked for nan "
-                "values. nan values will be ignored.",
+                "The input array could not be properly checked for nan " "values. nan values will be ignored.",
                 RuntimeWarning,
             )
 
     if contains_nan and nan_policy == "raise":
         raise ValueError("The input contains nan values")
 
     return (contains_nan, nan_policy)
@@ -255,17 +252,15 @@
         "ConfInt: Hi": confint_hi,
         "p value": 2 * t_value_cdf(-np.abs(z_variate), df),
         "Degrees of freedom": df,
         "Pooled standard deviation": sd_z_variate,
     }
 
 
-def ttest_difference(
-    df: pd.DataFrame, grouper_column: str, values_column: str, conflevel=0.995
-):
+def ttest_difference(df: pd.DataFrame, grouper_column: str, values_column: str, conflevel=0.995):
     """
     Calculates the t-test for differences between two or more groups and returns a confidence
     interval for the difference. The test is for UNPAIRED differences.
 
     The dataframe `df` contains a `grouper_column` with 2 or more unique values (e.g. 'A' and 'B').
     All unique values of the `grouper_column` are used, and t-tests are done between the values
     in the `values_column`.
@@ -300,21 +295,16 @@
     data_subset = data_subset.dropna()
     groups = df[grouper_column].unique()
     output = pd.DataFrame()
     groups = list(groups)
     while len(groups) > 0:
         groupA_name = groups.pop(0)
         for groupB_name in groups:
-
-            sample_A = data_subset[data_subset[grouper_column].eq(groupA_name)][
-                values_column
-            ]
-            sample_B = data_subset[data_subset[grouper_column].eq(groupB_name)][
-                values_column
-            ]
+            sample_A = data_subset[data_subset[grouper_column].eq(groupA_name)][values_column]
+            sample_B = data_subset[data_subset[grouper_column].eq(groupB_name)][values_column]
             sample_A = sample_A.astype(np.float64)
             sample_B = sample_B.astype(np.float64)
             basic_stats = ttest_difference_calculate(sample_A, sample_B, conflevel)
             basic_stats.update(
                 {
                     "Group A name": groupA_name,
                     "Group B name": groupB_name,
@@ -366,17 +356,15 @@
         "ConfInt: Hi": confint_hi,
         "p value": 2 * t_value_cdf(-np.abs(z_variate), dof),
         "Degrees of freedom": dof,
         "Standard deviation": sd_z_variate,
     }
 
 
-def ttest_paired_difference(
-    df: pd.DataFrame, grouper_column: str, values_column: str, conflevel=0.995
-):
+def ttest_paired_difference(df: pd.DataFrame, grouper_column: str, values_column: str, conflevel=0.995):
     """
     Calculates the t-test for paired differences between two or more groups and returns a
     confidence interval for the difference. The test is for PAIRED differences.
     The differences is always defined as the A values minus the B values: after - before, or A - B.
 
     The dataframe `df` contains a `grouper_column` with 2 or more unique values (e.g. 'A' and 'B').
     All unique values of the `grouper_column` are used, and t-tests are done between the values
@@ -407,27 +395,20 @@
     data_subset = data_subset.dropna()
     groups = df[grouper_column].unique()
     output = pd.DataFrame()
     groups = list(groups)
     while len(groups) > 0:
         groupA_name = groups.pop(0)
         for groupB_name in groups:
-
-            sample_A = data_subset[data_subset[grouper_column].eq(groupA_name)][
-                values_column
-            ]
-            sample_B = data_subset[data_subset[grouper_column].eq(groupB_name)][
-                values_column
-            ]
+            sample_A = data_subset[data_subset[grouper_column].eq(groupA_name)][values_column]
+            sample_B = data_subset[data_subset[grouper_column].eq(groupB_name)][values_column]
             sample_A = sample_A.astype(np.float64)
             sample_B = sample_B.astype(np.float64)
             assert sample_A.shape[0] == sample_B.shape[0]
-            differences = (
-                sample_A - sample_B.values
-            )  # only the .values of one vector are needed!
+            differences = sample_A - sample_B.values  # only the .values of one vector are needed!
             basic_stats = ttest_paired_difference_calculate(differences, conflevel)
             basic_stats.update(
                 {
                     "Group A name": groupA_name,
                     "Group B name": groupB_name,
                     "Group A number": sample_A.shape[0],
                     "Group B number": sample_B.shape[0],
@@ -436,17 +417,15 @@
                 }
             )
             output = pd.concat([output, pd.DataFrame(basic_stats, index=[0])])
 
     return output
 
 
-def confidence_interval(
-    df: pd.DataFrame, column_name: str, conflevel=0.95, style="robust"
-) -> tuple:
+def confidence_interval(df: pd.DataFrame, column_name: str, conflevel=0.95, style="robust") -> tuple:
     """
     Calculates the confidence interval, returned as a tuple, for the `column_name` (str) in the
     dataframe `df`, for a given confidence level `conflevel` (default: 0.95).
 
     `style`: ['robust'; 'regular']: indicates which style of estimates to use for the center and
                                     spread. Default: 'robust'
 
@@ -492,17 +471,15 @@
         return np.nan
     # Edge cases have been handled, so do the basic MAD calculation.
     med = center(x)
     mad = np.median(np.abs(x - med))
     return mad
 
 
-def median_abs_deviation(
-    x, axis=0, center=np.median, scale="normal", nan_policy="omit"
-):
+def median_abs_deviation(x, axis=0, center=np.median, scale="normal", nan_policy="omit"):
     r"""
 
     Taken from `scipy.stats.stats`: we want the same functionality, but with a slightly different
     default function signature:
 
     *   `scale='normal'` instead of `scale=1.0`.
     *   `nan_policy='omit'` instead of `nan_policy='propogate'`
@@ -610,18 +587,15 @@
     >>> stats.median_abs_deviation(x)
     1.3487398527041636
     >>> stats.median_abs_deviation(x, scale='normal')
     1.9996446978061115
     """
     assert axis is not None, "axis=None is now depricated. Unraval the array."
     if not callable(center):
-        raise TypeError(
-            "The argument 'center' must be callable. The given "
-            f"value {repr(center)} is not callable."
-        )
+        raise TypeError("The argument 'center' must be callable. The given " f"value {repr(center)} is not callable.")
 
     # An error may be raised here, so fail-fast, before doing lengthy
     # computations, even though `scale` is not used until later
     if isinstance(scale, str):
         if scale.lower() == "normal":
             scale = 0.6744897501960817  # special.ndtri(0.75)
         else:
@@ -638,15 +612,14 @@
         return np.full(nan_shape, np.nan)  # pragma: no cover
 
     contains_nan, nan_policy = _contains_nan(x, nan_policy)
 
     if contains_nan:
         mad = np.apply_along_axis(_mad_1d, axis, x, center, nan_policy)
     else:
-
         # Wrap the call to center() in expand_dims() so it acts like
         # keepdims=True was used.
         med = np.expand_dims(center(x, axis=axis), axis)
         mad = np.median(np.abs(x - med), axis=axis)
 
     return mad / scale
 
@@ -690,19 +663,15 @@
     out["iqr"] = out["percentile_75"] - out["percentile_25"]
     out["min"] = np.nanmin(x)
     out["max"] = np.nanmax(x)
     out["N_non_missing"] = np.sum(~np.isnan(x))
 
     if method.lower() == "robust":
         out["center"], out["spread"] = out["median"], Sn(x)
-        if (
-            ((out["max"] - out["min"]) > 0)
-            and (out["spread"] == 0)
-            and (out["N_non_missing"] > 0)
-        ):
+        if ((out["max"] - out["min"]) > 0) and (out["spread"] == 0) and (out["N_non_missing"] > 0):
             # Don't fully trust the Sn() yet. It works strangely on quantized data when there is
             # little variation. Replace the RSD with the classically calculated version in this
             # very specific case. This example shows it: [99, 95, 95, 100, 100, 100, 100, 95, 100,
             # 100, 100, 100, 105, 105, 100, 95, 105, 100, 95, 100]
             out["center"], out["spread"] = out["mean"], out["std_ddof1"]
 
     else:
@@ -775,15 +744,14 @@
 
         # 2. https://www.itl.nist.gov/div898/handbook/eda/section3/eda35h3.htm
         x = x.copy(deep=True)
         extra_out = defaultdict(list)
         N = x.shape[0] - pd.isna(x).sum()
 
         for k in range(max_outliers_detected):
-
             i = k + 1
             extra_out["i"].append(i)
 
             if robust_variant:
                 variation = median_abs_deviation(x)
                 R = ((x - x.median()) / variation).abs()
             else:
@@ -812,15 +780,17 @@
             if variation > __eps:
                 # The variation, if zero or small, will fail to drop this index
                 x.drop(R_i_idx, inplace=True)
 
         try:
             cutoff_i = np.where(
                 np.array(extra_out["R_i"]) - np.array(extra_out["lambda"]) >= 0,
-            )[0][0]
+            )[
+                0
+            ][0]
         except IndexError:
             cutoff_i = -1
 
         # The outlier indices are the points from the start of
         # `extra_out['R_i_idx']`, up to, and including, the `cutoff_i` index
         # in the list.
         extra_out["cutoff"] = cutoff_i
@@ -886,17 +856,15 @@
 
     # Between groups: the ANOVA relationship is such that SSQ(total) = SSQ(between) + SSQ(within).
     # Therefore the between-group statistics are found by differencing
     between_dof = max(0, total_dof - within_dof)
     if between_dof == 0:
         between_ms = 0
     else:
-        between_ms = max(
-            0.0, (total_ms * total_dof - within_ms * within_dof) / between_dof
-        )
+        between_ms = max(0.0, (total_ms * total_dof - within_ms * within_dof) / between_dof)
 
     return {
         "total_ms": total_ms,
         "total_dof": total_dof,
         "within_ms": within_ms,
         "within_stddev": np.sqrt(within_ms),
         "within_dof": within_dof,
```

### Comparing `process-improve-0.9.64/process_improve.egg-info/PKG-INFO` & `process-improve-0.9.65/process_improve.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: process-improve
-Version: 0.9.64
+Version: 0.9.65
 Summary: Process Improvement using Data: Designed Experiments; Latent Variables (PCA, PLS, multivariate methods with missing data); Process Monitoring; Batch data analysis.
 Home-page: https://github.com/kgdunn/process_improve
 Author: Kevin Dunn
 Author-email: kgdunn@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Process Improvement (using Data)
 
 This is a package that goes with the
 [online book](https://learnche.org/pid) of the same title,
 Process Improvement using Data.
-
-
```

### Comparing `process-improve-0.9.64/process_improve.egg-info/SOURCES.txt` & `process-improve-0.9.65/process_improve.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 process_improve/__init__.py
 process_improve.egg-info/PKG-INFO
 process_improve.egg-info/SOURCES.txt
 process_improve.egg-info/dependency_links.txt
 process_improve.egg-info/requires.txt
 process_improve.egg-info/top_level.txt
```

### Comparing `process-improve-0.9.64/setup.py` & `process-improve-0.9.65/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open(pathlib.Path(".") / "process_improve" / "__init__.py") as fh:
-    version_number = [
-        line.split("=")[1].strip()
-        for line in fh.read().split("\n")
-        if line.startswith("__version__")
-    ][0].replace('"', "")
+    version_number = [line.split("=")[1].strip() for line in fh.read().split("\n") if line.startswith("__version__")][
+        0
+    ].replace('"', "")
 
 setuptools.setup(
     name="process-improve",
     version=version_number,
     author="Kevin Dunn",
     author_email="kgdunn@gmail.com",
     description=(
@@ -34,15 +32,15 @@
     python_requires=">=3.8",
     install_requires=[
         "pandas",
         "numpy",
         "statsmodels",
         "matplotlib",
         "bokeh",
-        "sklearn",
+        "scikit-learn",
         "patsy",
         "scikit-image",
         "scikit-learn",
         "plotly",
         "numba",
         "seaborn",
         "pydantic",
```

