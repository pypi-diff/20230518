# Comparing `tmp/ms2query-0.7.4.tar.gz` & `tmp/ms2query-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms2query-0.7.4.tar", last modified: Tue Apr 18 15:38:24 2023, max compression
+gzip compressed data, was "dist/ms2query-1.0.0.tar", last modified: Thu May 18 08:20:43 2023, max compression
```

## Comparing `ms2query-0.7.4.tar` & `ms2query-1.0.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-04-18 15:38:24.000000 ms2query-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-04-18 15:38:13.000000 ms2query-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21623 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/k_fold_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/visualize_mass_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/clean_and_filter_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query/create_new_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/create_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/create_new_library/train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    26008 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/old_query_from_sqlite_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/query_from_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-18 15:38:13.000000 ms2query-0.7.4/ms2query/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 15:38:24.000000 ms2query-0.7.4/ms2query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-18 15:38:24.000000 ms2query-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-18 15:38:14.000000 ms2query-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:24.000000 ms2query-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_calculate_tanimoto_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_clean_and_filter_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_collect_test_data_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_library_files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_ms2library.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_results_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_run_ms2query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_split_data_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_train_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_train_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_train_ms2query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_use_files_without_spectrum_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-04-18 15:38:14.000000 ms2query-0.7.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:43.000000 ms2query-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-05-18 08:20:43.000000 ms2query-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-05-18 08:20:29.000000 ms2query-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:43.000000 ms2query-1.0.0/ms2query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:43.000000 ms2query-1.0.0/ms2query/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21282 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/benchmarking/collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/benchmarking/k_fold_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/benchmarking/visualize_mass_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/clean_and_filter_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:43.000000 ms2query-1.0.0/ms2query/create_new_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/add_classifire_classifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/create_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/create_new_library/train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25085 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/old_query_from_sqlite_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/query_from_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-05-18 08:20:29.000000 ms2query-1.0.0/ms2query/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:43.000000 ms2query-1.0.0/ms2query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-05-18 08:20:42.000000 ms2query-1.0.0/ms2query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-18 08:20:43.000000 ms2query-1.0.0/ms2query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:20:42.000000 ms2query-1.0.0/ms2query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-18 08:20:42.000000 ms2query-1.0.0/ms2query.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:20:42.000000 ms2query-1.0.0/ms2query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-18 08:20:42.000000 ms2query-1.0.0/ms2query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 08:20:42.000000 ms2query-1.0.0/ms2query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-18 08:20:43.000000 ms2query-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-18 08:20:29.000000 ms2query-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:43.000000 ms2query-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:29.000000 ms2query-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-18 08:20:29.000000 ms2query-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-18 08:20:29.000000 ms2query-1.0.0/tests/test_add_classifier_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-18 08:20:29.000000 ms2query-1.0.0/tests/test_calculate_tanimoto_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-18 08:20:29.000000 ms2query-1.0.0/tests/test_clean_and_filter_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-18 08:20:29.000000 ms2query-1.0.0/tests/test_collect_test_data_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_library_files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_ms2library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_results_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_run_ms2query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_split_data_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_train_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_train_ms2query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-18 08:20:30.000000 ms2query-1.0.0/tests/test_utils.py
```

### Comparing `ms2query-0.7.4/PKG-INFO` & `ms2query-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 0.7.4
+Version: 1.0.0
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-0.7.4/README.md` & `ms2query-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/__init__.py` & `ms2query-1.0.0/ms2query/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/benchmarking/collect_test_data_results.py` & `ms2query-1.0.0/ms2query/benchmarking/collect_test_data_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ms2deepscore import MS2DeepScore
 from ms2deepscore.models import SiameseModel
 from spec2vec.vector_operations import cosine_similarity_matrix
 from matchms.calculate_scores import calculate_scores
 from matchms.similarity.ModifiedCosine import ModifiedCosine
 from matchms.similarity.CosineGreedy import CosineGreedy
 
-from ms2query.query_from_sqlite_database import get_metadata_from_sqlite
+from ms2query.query_from_sqlite_database import SqliteLibrary
 from ms2query.utils import save_json_file
 
 
 def generate_test_results_ms2query(ms2library: MS2Library,
                                    test_spectra: List[Spectrum]
                                    ) -> List[Tuple[float, float, bool]]:
     # pylint:disable=too-many-locals
@@ -35,23 +35,19 @@
                                               results_csv_file_location=temporary_file_csv_results)
         df_results_ms2query = pd.read_csv(temporary_file_csv_results)
 
     test_results_ms2query = []
     for i, test_spectrum in enumerate(test_spectra):
         query_spectrum_id = i + 1
         annotated = False
-        for spectrum_id, ms2query_model_prediction, query_spectrum_id_in_df in df_results_ms2query[
-            ["spectrum_ids", "ms2query_model_prediction", "query_spectrum_nr"]].to_numpy():
+        for inchikey, smiles, ms2query_model_prediction, query_spectrum_id_in_df in df_results_ms2query[
+            ["inchikey", "smiles", "ms2query_model_prediction", "query_spectrum_nr"]].to_numpy():
             if query_spectrum_id == query_spectrum_id_in_df:
-                # Get metadata belonging to spectra ids
-                lib_metadata = get_metadata_from_sqlite(
-                    ms2library.sqlite_file_name,
-                    [spectrum_id])[spectrum_id]
-                tanimoto_score = calculate_single_tanimoto_score(test_spectrum.get("smiles"), lib_metadata["smiles"])
-                exact_match = lib_metadata["inchikey"][:14] == test_spectrum.get("inchikey")[:14]
+                tanimoto_score = calculate_single_tanimoto_score(test_spectrum.get("smiles"), smiles)
+                exact_match = inchikey == test_spectrum.get("inchikey")[:14]
                 test_results_ms2query.append((ms2query_model_prediction, tanimoto_score, exact_match))
                 annotated = True
         if not annotated:
             test_results_ms2query.append(None)
     return test_results_ms2query
 
 
@@ -79,34 +75,34 @@
         ms2ds_scores,
         index=ms2ds_embeddings.index)
     return similarity_matrix_dataframe
 
 
 def select_highest_ms2ds_in_mass_range(ms2deepscores,
                                        test_spectra,
-                                       sqlite_file_location,
+                                       sqlite_library: SqliteLibrary,
                                        allowed_mass_diff: Union[None, float]) -> List[Tuple[float, float, bool]]:
     results_ms2deepscore = []
     for i, test_spectrum in tqdm(enumerate(test_spectra)):
         precursor_mz_query_spectrum = test_spectrum.get("precursor_mz")
         if allowed_mass_diff is not None:
-            spectrum_ids_and_mass = get_precursor_mz_within_range(sqlite_file_location,
-                                                                  precursor_mz_query_spectrum - allowed_mass_diff,
-                                                                  precursor_mz_query_spectrum + allowed_mass_diff)
+            spectrum_ids_and_mass = get_precursor_mz_within_range(
+                sqlite_library.sqlite_file_name,
+                precursor_mz_query_spectrum - allowed_mass_diff,
+                precursor_mz_query_spectrum + allowed_mass_diff)
             spectrum_ids = [spectrum_and_mass[0] for spectrum_and_mass in spectrum_ids_and_mass]
             if len(spectrum_ids) == 0:
                 spectrum_id_highest_ms2_deepscore_in_mass_range = None
             else:
                 spectrum_id_highest_ms2_deepscore_in_mass_range = ms2deepscores[i].loc[spectrum_ids].idxmax()
         else:
             spectrum_id_highest_ms2_deepscore_in_mass_range = ms2deepscores[i].idxmax()
         if spectrum_id_highest_ms2_deepscore_in_mass_range is not None:
             # Get metadata belonging to spectra ids
-            lib_metadata = get_metadata_from_sqlite(
-                sqlite_file_location,
+            lib_metadata = sqlite_library.get_metadata_from_sqlite(
                 [spectrum_id_highest_ms2_deepscore_in_mass_range])[spectrum_id_highest_ms2_deepscore_in_mass_range]
             tanimoto_score = calculate_single_tanimoto_score(test_spectrum.get("smiles"), lib_metadata["smiles"])
             exact_match = lib_metadata["inchikey"][:14] == test_spectrum.get("inchikey")[:14]
             results_ms2deepscore.append((float(ms2deepscores[i][spectrum_id_highest_ms2_deepscore_in_mass_range]),
                                          tanimoto_score,
                                          exact_match))
         else:
@@ -262,24 +258,24 @@
         # Generate MS2Deepscore results
         ms2ds_scores = get_all_ms2ds_scores(ms2library.ms2ds_model,
                                             ms2library.ms2ds_embeddings,
                                             test_spectra)
         if not os.path.isfile(ms2ds_results_100_file_name):
             ms2ds_test_results_mass_diff_100 = select_highest_ms2ds_in_mass_range(ms2ds_scores,
                                                                                   test_spectra,
-                                                                                  ms2library.sqlite_file_name,
+                                                                                  ms2library.sqlite_library,
                                                                                   allowed_mass_diff=100)
             save_json_file(ms2ds_test_results_mass_diff_100, ms2ds_results_100_file_name)
         else:
             print(f"File already exists so not remade: {ms2ds_results_100_file_name}")
 
         if not os.path.isfile(ms2ds_results_all_file_name):
             ms2ds_test_results_all = select_highest_ms2ds_in_mass_range(ms2ds_scores,
                                                                         test_spectra,
-                                                                        ms2library.sqlite_file_name,
+                                                                        ms2library.sqlite_library,
                                                                         allowed_mass_diff=None)
             save_json_file(ms2ds_test_results_all, ms2ds_results_all_file_name)
         else:
             print(f"File already exists so not remade: {ms2ds_results_all_file_name}")
     else:
         print("MS2Deepscore files already exist")
 
@@ -344,24 +340,24 @@
         # Generate MS2Deepscore results
         ms2ds_scores = get_all_ms2ds_scores(ms2library.ms2ds_model,
                                             ms2library.ms2ds_embeddings,
                                             test_spectra)
         if not os.path.isfile(ms2ds_results_0_25_file_name):
             ms2ds_test_results_mass_diff_100 = select_highest_ms2ds_in_mass_range(ms2ds_scores,
                                                                                   test_spectra,
-                                                                                  ms2library.sqlite_file_name,
+                                                                                  ms2library.sqlite_library,
                                                                                   allowed_mass_diff=0.25)
             save_json_file(ms2ds_test_results_mass_diff_100, ms2ds_results_0_25_file_name)
         else:
             print(f"File already exists so not remade: {ms2ds_results_0_25_file_name}")
 
         if not os.path.isfile(ms2ds_results_all_file_name):
             ms2ds_test_results_all = select_highest_ms2ds_in_mass_range(ms2ds_scores,
                                                                         test_spectra,
-                                                                        ms2library.sqlite_file_name,
+                                                                        ms2library.sqlite_library,
                                                                         allowed_mass_diff=None)
             save_json_file(ms2ds_test_results_all, ms2ds_results_all_file_name)
         else:
             print(f"File already exists so not remade: {ms2ds_results_all_file_name}")
     else:
         print("MS2Deepscore files already exist")
```

### Comparing `ms2query-0.7.4/ms2query/benchmarking/create_accuracy_vs_recall_plot.py` & `ms2query-1.0.0/ms2query/benchmarking/create_accuracy_vs_recall_plot.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/benchmarking/k_fold_cross_validation.py` & `ms2query-1.0.0/ms2query/benchmarking/k_fold_cross_validation.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/benchmarking/visualize_mass_distribution.py` & `ms2query-1.0.0/ms2query/benchmarking/visualize_mass_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/benchmarking/visualize_tanimoto_score_distribution.py` & `ms2query-1.0.0/ms2query/benchmarking/visualize_tanimoto_score_distribution.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/clean_and_filter_spectra.py` & `ms2query-1.0.0/ms2query/clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/create_new_library/calculate_tanimoto_scores.py` & `ms2query-1.0.0/ms2query/create_new_library/calculate_tanimoto_scores.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/create_new_library/create_sqlite_database.py` & `ms2query-1.0.0/ms2query/create_new_library/create_sqlite_database.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 new models
 """
 
 import sqlite3
 from typing import Dict, List
 from matchms import Spectrum
 from tqdm import tqdm
+import pandas as pd
 
 from ms2query.create_new_library.calculate_tanimoto_scores import calculate_highest_tanimoto_score
+from ms2query.utils import return_non_existing_file_name
 
 
 def make_sqlfile_wrapper(sqlite_file_name: str,
                          list_of_spectra: List[Spectrum],
                          columns_dict: Dict[str, str] = None,
+                         compound_classes: pd.DataFrame = None,
                          progress_bars: bool = True):
     """Wrapper to create sqlite file containing spectrum information needed for MS2Query
 
     Args:
     -------
     sqlite_file_name:
         Name of sqlite_file that should be created, if it already exists the
@@ -33,23 +36,32 @@
         since these values will be automatically added in the function
         add_list_of_spectra_to_sqlite.
         Default = None results in the default columns.
     progress_bars:
         If progress_bars is True progress bars will be shown for the different
         parts of the progress.
     """
-    initialize_tables(sqlite_file_name, additional_metadata_columns_dict=columns_dict)
+    sqlite_file_name = return_non_existing_file_name(sqlite_file_name)
+    additional_inchikey_columns = []
+    if compound_classes is not None:
+        additional_inchikey_columns = list(compound_classes.columns)
+        assert compound_classes.index.name == "inchikey", "Expected a pandas dataframe with inchikey as index name"
+
+    initialize_tables(sqlite_file_name, additional_metadata_columns_dict=columns_dict,
+                      additional_inchikey_columns=additional_inchikey_columns)
     fill_spectrum_data_table(sqlite_file_name, list_of_spectra, progress_bar=progress_bars)
 
     fill_inchikeys_table(sqlite_file_name, list_of_spectra,
+                         compound_classes=compound_classes,
                          progress_bars=progress_bars)
 
 
 def initialize_tables(sqlite_file_name: str,
-                      additional_metadata_columns_dict: Dict[str, str] = None):
+                      additional_metadata_columns_dict: Dict[str, str] = None,
+                      additional_inchikey_columns = None):
     """Creates a new sqlite file, with the empty tables spectrum_data and incikeys
 
     On default the columns spectrum_id and metadata are
     created. The column spectrum_id will be the primary key.
 
     Args:
     -------
@@ -62,39 +74,41 @@
         the default columns and as values the datatype. The defaults columns
         are spectrum_id, peaks, intensities and metadata. The additional
         columns should be the same names that are in the metadata dictionary,
         since these values will be automatically added in the function
         add_list_of_spectra_to_sqlite.
         Default = None results in the default columns.
     """
-    # Initialize spectrum_data_table
-    # Combine default columns and additional metadata columns
-    default_columns_dict = {"spectrumid": "INTEGER",
-                            "metadata": "TEXT"}
-    if additional_metadata_columns_dict is None:
-        additional_metadata_columns_dict = {}
-    combined_columns_dict = {**default_columns_dict, **additional_metadata_columns_dict}
-
-    initialize_spectrum_data_table = """
-    DROP TABLE IF EXISTS 'spectrum_data';
-    CREATE TABLE 'spectrum_data' (
-    """
-    # add all columns with the type specified in combined_columns_dict
-    for column_header in combined_columns_dict:
-        initialize_spectrum_data_table += column_header + " " \
-                                + combined_columns_dict[column_header] + ",\n"
-    initialize_spectrum_data_table += "PRIMARY KEY (spectrumid));"
+    additional_columns_txt = ""
+    if additional_metadata_columns_dict is not None:
+        # add all columns with the type specified in combined_columns_dict
+        additional_columns_txt = "".join(f"{column_header} {additional_metadata_columns_dict[column_header]},\n"
+                                         for column_header in additional_metadata_columns_dict)
+
+    initialize_spectrum_data_table = f"""
+        DROP TABLE IF EXISTS 'spectrum_data';
+        CREATE TABLE 'spectrum_data' (
+        'spectrumid' INTEGER,
+        'metadata' TEXT,
+        {additional_columns_txt}
+        PRIMARY KEY (spectrumid));"""
+
+    additional_inchikey_columns_txt = ""
+    if additional_inchikey_columns is not None:
+        # add all columns with the type specified in combined_columns_dict
+        additional_inchikey_columns_txt = "".join(f"{column_header} TEXT,\n" for column_header in additional_inchikey_columns)
 
     # Initialize inchikeys table
-    initialize_inchikeys_table = """;
+    initialize_inchikeys_table = f""";
     DROP TABLE IF EXISTS 'inchikeys';
     CREATE TABLE 'inchikeys'(
         'inchikey' TEXT,
         spectrum_ids_belonging_to_inchikey14 TEXT,
         closest_related_inchikeys TEXT,
+        {additional_inchikey_columns_txt}
         PRIMARY KEY ('inchikey')
         );
     """
 
     conn = sqlite3.connect(sqlite_file_name)
     cur = conn.cursor()
     cur.executescript(initialize_spectrum_data_table)
@@ -160,23 +174,26 @@
 
     conn.commit()
     conn.close()
 
 
 def fill_inchikeys_table(sqlite_file_name: str,
                          list_of_spectra: List[Spectrum],
+                         compound_classes: pd.DataFrame,
                          progress_bars: bool = True):
     """Fills the inchikeys table with Inchikeys, spectrum_ids_belonging_to_inchikey and closest related inchikeys
 
     sqlite_file_name:
         Name of sqlite_file that should be created, if it already exists the
         tables are added. If the tables in this sqlite file already exist, they
         will be overwritten.
     list_of_spectra:
         List of spectrum objects
+    compound_classes:
+        Dataframe with compound classes of inchikeys
     progress_bars:
         If True progress bars will show the progress of the different steps
         in the process.
     """
     # Get spectra belonging to each inchikey14
     spectra_belonging_to_inchikey14 = \
         get_spectra_belonging_to_inchikey14(list_of_spectra)
@@ -187,19 +204,27 @@
     closest_related_inchikey14s = calculate_highest_tanimoto_score(list_of_spectra, list_of_spectra, 10)
 
     # Fill table
     for inchikey14 in tqdm(spectra_belonging_to_inchikey14,
                            desc="Adding inchikey14s to sqlite table",
                            disable=not progress_bars):
         matching_spectrum_ids = str(spectra_belonging_to_inchikey14[inchikey14])
+        if compound_classes is not None:
+            # Select the compound classes
+            compound_class = list(compound_classes.loc[inchikey14])
+            compound_class_string = "".join(f',\n"{value}"' for value in compound_class)
+        else:
+            compound_class_string = ""
+
         add_row_to_table_command = \
             f"""INSERT INTO 'inchikeys' 
             values ("{inchikey14}", 
             "{matching_spectrum_ids}",
-            "{str(closest_related_inchikey14s[inchikey14])}");"""
+            "{str(closest_related_inchikey14s[inchikey14])}"
+            {compound_class_string});"""
         cur.execute(add_row_to_table_command)
     conn.commit()
     conn.close()
 
 
 def get_spectra_belonging_to_inchikey14(spectra: List[Spectrum]
                                         ) -> Dict[str, List[int]]:
```

### Comparing `ms2query-0.7.4/ms2query/create_new_library/library_files_creator.py` & `ms2query-1.0.0/ms2query/create_new_library/library_files_creator.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from matchms.Spectrum import Spectrum
 from ms2deepscore import MS2DeepScore
 from ms2deepscore.models import load_model as load_ms2ds_model
 from spec2vec.vector_operations import calc_vector
 from tqdm import tqdm
 from ms2query.create_new_library.create_sqlite_database import make_sqlfile_wrapper
 from ms2query.clean_and_filter_spectra import create_spectrum_documents
+from ms2query.create_new_library.add_classifire_classifications import select_compound_classes, convert_to_dataframe
 
 
 class LibraryFilesCreator:
     """Class to build a MS2Query library from input spectra and trained
     MS2DeepScore as well as Spec2Vec models.
 
     For example:
@@ -43,14 +44,15 @@
         library_creator.create_all_library_files()
     """
     def __init__(self,
                  library_spectra: List[Spectrum],
                  output_directory: Union[str, Path],
                  s2v_model_file_name: str = None,
                  ms2ds_model_file_name: str = None,
+                 add_compound_classes: bool = True
                  ):
         """Creates files needed to run queries on a library
 
         Parameters
         ----------
         library_spectra:
             A list containing matchms spectra objects for the library spectra.
@@ -61,14 +63,15 @@
             For ms2ds_embeddings: "ms2ds_embeddings.pickle"
             For s2v_embeddings: "s2v_embeddings.pickle"
         s2v_model_file_name:
             file name of a s2v model
         ms2ds_model_file_name:
             File name of a ms2ds model
         """
+        # pylint: disable=too-many-arguments
         self.progress_bars = True
         self.output_directory = output_directory
         if not os.path.exists(self.output_directory):
             os.mkdir(self.output_directory)
         self.sqlite_file_name = os.path.join(output_directory, "ms2query_library.sqlite")
         self.ms2ds_embeddings_file_name = os.path.join(output_directory, "ms2ds_embeddings.pickle")
         self.s2v_embeddings_file_name = os.path.join(output_directory, "s2v_embeddings.pickle")
@@ -88,14 +91,15 @@
             self.ms2ds_model = load_ms2ds_model(ms2ds_model_file_name)
         # Initialise spectra
         self.list_of_spectra = library_spectra
 
         # Run default filters
         self.list_of_spectra = [msfilters.default_filters(s) for s in tqdm(self.list_of_spectra,
                                                                            desc="Applying default filters to spectra")]
+        self.add_compound_classes = add_compound_classes
 
     def _check_for_existing_files(self):
         assert not os.path.exists(self.sqlite_file_name), \
             f"The file {self.sqlite_file_name} already exists," \
             f" choose a different output_base_filename"
         assert not os.path.exists(self.ms2ds_embeddings_file_name), \
             f"The file {self.ms2ds_embeddings_file_name} " \
@@ -108,18 +112,24 @@
         """Creates files with embeddings and a sqlite file with spectra data
         """
         self.create_sqlite_file()
         self.store_s2v_embeddings()
         self.store_ms2ds_embeddings()
 
     def create_sqlite_file(self):
+        if self.add_compound_classes:
+            compound_classes = select_compound_classes(self.list_of_spectra)
+            compound_classes_df = convert_to_dataframe(compound_classes)
+        else:
+            compound_classes_df = None
         make_sqlfile_wrapper(
             self.sqlite_file_name,
             self.list_of_spectra,
             columns_dict={"precursor_mz": "REAL"},
+            compound_classes=compound_classes_df,
             progress_bars=self.progress_bars,
         )
 
     def store_ms2ds_embeddings(self):
         """Creates a pickled file with embeddings scores for spectra
 
         A dataframe with as index randomly generated spectrum indexes and as columns the indexes
```

### Comparing `ms2query-0.7.4/ms2query/create_new_library/split_data_for_training.py` & `ms2query-1.0.0/ms2query/create_new_library/split_data_for_training.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/create_new_library/train_models.py` & `ms2query-1.0.0/ms2query/create_new_library/train_models.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/create_new_library/train_ms2deepscore.py` & `ms2query-1.0.0/ms2query/create_new_library/train_ms2deepscore.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/create_new_library/train_ms2query_model.py` & `ms2query-1.0.0/ms2query/create_new_library/train_ms2query_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import List
 import pandas as pd
 from tqdm import tqdm
 from matchms import Spectrum
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.metrics import mean_squared_error
 from ms2query import MS2Library
-from ms2query.query_from_sqlite_database import get_metadata_from_sqlite
+from ms2query.query_from_sqlite_database import SqliteLibrary
 from ms2query.create_new_library.library_files_creator import LibraryFilesCreator
 from ms2query.create_new_library.split_data_for_training import split_spectra_on_inchikeys, split_training_and_validation_spectra
 from ms2query.create_new_library.calculate_tanimoto_scores import calculate_tanimoto_scores_from_smiles
 from ms2query.utils import save_pickled_file
 
 
 class DataCollectorForTraining():
@@ -56,15 +56,15 @@
                                    desc="Get scores and tanimoto scores",
                                    disable=not self.ms2library.settings["progress_bars"]):
             results_table = self.ms2library.calculate_features_single_spectrum(query_spectrum,
                                                                                self.preselection_cut_off)
 
             # Get tanimoto scores
             library_spectrum_ids = list(results_table.data.index)
-            tanimoto_scores = calculate_tanimoto_scores_with_library(self.ms2library.sqlite_file_name, query_spectrum,
+            tanimoto_scores = calculate_tanimoto_scores_with_library(self.ms2library.sqlite_library, query_spectrum,
                                                                      library_spectrum_ids)
             # Add tanimoto scores for training data
             all_tanimoto_scores = \
                 all_tanimoto_scores.append(tanimoto_scores,
                                            ignore_index=True)
             # Select the features (remove inchikey, since this should not be
             # used for training
@@ -74,20 +74,19 @@
                 tanimoto_scores.index]
             info_of_matches_with_tanimoto = \
                 info_of_matches_with_tanimoto.append(matches_with_tanimoto,
                                                      ignore_index=True)
         return info_of_matches_with_tanimoto, all_tanimoto_scores
 
 
-def calculate_tanimoto_scores_with_library(sqlite_file_name,
+def calculate_tanimoto_scores_with_library(sqlite_library: SqliteLibrary,
                                            query_spectrum: Spectrum,
-                                           spectra_ids_list: List[str]):
+                                           spectra_ids_list: List[int]):
     # Get inchikeys belonging to spectra ids
-    metadata_dict = get_metadata_from_sqlite(
-        sqlite_file_name,
+    metadata_dict = sqlite_library.get_metadata_from_sqlite(
         spectra_ids_list)
     library_smiles_list = [metadata_dict[spectrum_id]["smiles"] for spectrum_id in spectra_ids_list]
     tanimoto_scores = calculate_tanimoto_scores_from_smiles(library_smiles_list, [query_spectrum.get("smiles")])
     tanimoto_df = pd.DataFrame(tanimoto_scores, index=spectra_ids_list, columns=["Tanimoto_score"])
     return tanimoto_df
 
 
@@ -120,25 +119,24 @@
     library_spectra, single_spectra_query_spectra = split_training_and_validation_spectra(library_spectra,
                                                                                           fraction_for_training)
     query_spectra_for_training = unique_inchikey_query_spectra + single_spectra_query_spectra
 
     # Create library files for training ms2query
     library_creator_for_training = LibraryFilesCreator(library_spectra, output_directory=library_files_folder,
                                                        s2v_model_file_name=s2v_model_file_name,
-                                                       ms2ds_model_file_name=ms2ds_model_file_name)
+                                                       ms2ds_model_file_name=ms2ds_model_file_name,
+                                                       add_compound_classes=False)
     library_creator_for_training.create_all_library_files()
 
-    ms2library_for_training = MS2Library(
-        sqlite_file_name=library_creator_for_training.sqlite_file_name,
-        s2v_model_file_name=s2v_model_file_name,
-        ms2ds_model_file_name=ms2ds_model_file_name,
-        pickled_s2v_embeddings_file_name=library_creator_for_training.s2v_embeddings_file_name,
-        pickled_ms2ds_embeddings_file_name=library_creator_for_training.ms2ds_embeddings_file_name,
-        ms2query_model_file_name=None,
-        classifier_csv_file_name=None)
+    ms2library_for_training = MS2Library(sqlite_file_name=library_creator_for_training.sqlite_file_name,
+                                         s2v_model_file_name=s2v_model_file_name,
+                                         ms2ds_model_file_name=ms2ds_model_file_name,
+                                         pickled_s2v_embeddings_file_name=library_creator_for_training.s2v_embeddings_file_name,
+                                         pickled_ms2ds_embeddings_file_name=library_creator_for_training.ms2ds_embeddings_file_name,
+                                         ms2query_model_file_name=None)
     # Create training data MS2Query model
     collector = DataCollectorForTraining(ms2library_for_training)
     training_scores, training_labels = collector.get_matches_info_and_tanimoto(query_spectra_for_training)
 
     save_pickled_file(training_scores, os.path.join(library_files_folder, "training_scores_ms2query"))
     save_pickled_file(training_labels, os.path.join(library_files_folder, "training_labels_ms2query"))
```

### Comparing `ms2query-0.7.4/ms2query/ms2library.py` & `ms2query-1.0.0/ms2query/ms2library.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from gensim.models import Word2Vec
 from matchms.Spectrum import Spectrum
 from ms2deepscore import MS2DeepScore
 from ms2deepscore.models import load_model as load_ms2ds_model
 from spec2vec.vector_operations import calc_vector, cosine_similarity_matrix
 from tqdm import tqdm
 from onnxruntime import InferenceSession
-from ms2query.query_from_sqlite_database import (get_inchikey_information,
-                                                 get_precursor_mz, get_ionization_mode_library)
+from ms2query.query_from_sqlite_database import SqliteLibrary
 from ms2query.results_table import ResultsTable
 from ms2query.clean_and_filter_spectra import (clean_metadata,
                                                create_spectrum_documents,
                                                normalize_and_filter_peaks)
 from ms2query.utils import (column_names_for_output, load_ms2query_model,
                             load_pickled_file, SettingsRunMS2Query, predict_onnx_model,
                             select_files_in_directory)
@@ -40,15 +39,14 @@
     def __init__(self,
                  sqlite_file_name: str,
                  s2v_model_file_name: str,
                  ms2ds_model_file_name: str,
                  pickled_s2v_embeddings_file_name: str,
                  pickled_ms2ds_embeddings_file_name: str,
                  ms2query_model_file_name: Union[str, None],
-                 classifier_csv_file_name: Union[str, None] = None,
                  **settings):
         """
         Parameters
         ----------
         sqlite_file_name:
             The location at which the sqlite_file_is_stored. The file is
             expected to have 3 tables: tanimoto_scores, inchikeys and
@@ -63,16 +61,14 @@
             File location of a pickled file with Spec2Vec embeddings in a
             pd.Dataframe with as index the spectrum id.
         pickled_ms2ds_embeddings_file_name:
             File location of a pickled file with ms2ds embeddings in a
             pd.Dataframe with as index the spectrum id.
         ms2query_model_file_name:
             File location of ms2query model with .hdf5 extension.
-        classifier_csv_file_name:
-            Csv file location containing classifier annotations per inchikey
 
         **settings:
             As additional parameters predefined settings can be changed.
         spectrum_id_column_name:
             The name of the column or key in dictionaries under which the
             spectrum id is stored. Default = "spectrumid"
         progress_bars:
@@ -80,17 +76,16 @@
         """
         # pylint: disable=too-many-arguments
 
         # Change default settings to values given in **settings
         self.settings = self._set_settings(settings)
 
         # Load models and set file locations
-        self.classifier_file_name = classifier_csv_file_name
         assert os.path.isfile(sqlite_file_name), f"The given sqlite file does not exist: {sqlite_file_name}"
-        self.sqlite_file_name = sqlite_file_name
+        self.sqlite_library = SqliteLibrary(sqlite_file_name)
 
         if ms2query_model_file_name is not None:
             self.ms2query_model = load_ms2query_model(ms2query_model_file_name)
 
         self.s2v_model = Word2Vec.load(s2v_model_file_name)
         self.ms2ds_model = load_ms2ds_model(ms2ds_model_file_name)
 
@@ -100,28 +95,26 @@
         self.ms2ds_embeddings: pd.DataFrame = load_pickled_file(
             pickled_ms2ds_embeddings_file_name)
         
         assert self.ms2ds_model.base.output_shape[1] == self.ms2ds_embeddings.shape[1], \
             "Dimension of pre-computed MS2DeepScore embeddings does not fit given model."
 
         # load precursor mz's
-        self.precursors_library = get_precursor_mz(
-            self.sqlite_file_name)
+        self.precursors_library = self.sqlite_library.get_precursor_mz()
 
         assert self.ms2ds_embeddings.shape[0] == self.s2v_embeddings.shape[0], \
             "The number ms2deepscore embeddings is not equal to the number of spectra with s2v embeddings"
 
         assert self.ms2ds_embeddings.shape[0] == len(self.precursors_library), \
             "Mismatch of library files. " \
             "The number of spectra in the sqlite library is not equal to the number of spectra in the embeddings"
 
-        self.ionization_mode = get_ionization_mode_library(self.sqlite_file_name)
-        self.spectra_of_inchikey14s, \
-            self.closely_related_inchikey14s = \
-            get_inchikey_information(self.sqlite_file_name)
+        self.ionization_mode = self.sqlite_library.get_ionization_mode_library()
+        self.spectra_of_inchikey14s, self.closely_related_inchikey14s = \
+            self.sqlite_library.get_inchikey_information()
         self.inchikey14s_of_spectra = {}
         for inchikey, list_of_spectrum_ids in \
                 self.spectra_of_inchikey14s.items():
             for spectrum_id in list_of_spectrum_ids:
                 self.inchikey14s_of_spectra[spectrum_id] = inchikey
 
     @staticmethod
@@ -169,20 +162,16 @@
             assert query_ionmode == self.ionization_mode, \
                 f"The spectrum is in {query_ionmode} ionization mode, while the library is for {self.ionization_mode} ionization mode. " \
                 f"Check the readme to download a library in the {query_ionmode} ionization mode"
 
 
         ms2deepscore_scores = self._get_all_ms2ds_scores(query_spectrum)
         # Initialize result table
-        results_table = ResultsTable(
-            preselection_cut_off=preselection_cut_off,
-            ms2deepscores=ms2deepscore_scores,
-            query_spectrum=query_spectrum,
-            sqlite_file_name=self.sqlite_file_name,
-            classifier_csv_file_name=self.classifier_file_name)
+        results_table = ResultsTable(preselection_cut_off=preselection_cut_off, ms2deepscores=ms2deepscore_scores,
+                                     query_spectrum=query_spectrum, sqlite_library=self.sqlite_library)
         results_table = \
             self._calculate_features_for_random_forest_model(results_table)
         return results_table
 
     def analog_search_return_results_tables(self,
                                             query_spectra: List[Spectrum],
                                             preselection_cut_off: int = 2000,
@@ -242,20 +231,20 @@
             settings = SettingsRunMS2Query()
         # Create csv file if it does not exist already
         assert not os.path.exists(results_csv_file_location), "Csv file location for results already exists"
         assert self.ms2query_model is not None, \
             "MS2Query model should be given when creating ms2library object"
 
         with open(results_csv_file_location, "w", encoding="utf-8") as csv_file:
-            if self.classifier_file_name is None:
-                csv_file.write(",".join(column_names_for_output(True, False, settings.additional_metadata_columns,
-                                                                settings.additional_ms2query_score_columns)) + "\n")
-            else:
-                csv_file.write(",".join(column_names_for_output(True, True, settings.additional_metadata_columns,
-                                                                settings.additional_ms2query_score_columns)) + "\n")
+            # Check if sqlite file has class annotations stored
+            add_class_annotations: bool = self.sqlite_library.contains_class_annotation()
+
+            csv_file.write(",".join(
+                column_names_for_output(True, add_class_annotations, settings.additional_metadata_columns,
+                                        settings.additional_ms2query_score_columns)) + "\n")
 
         for i, query_spectrum in \
                 tqdm(enumerate(query_spectra),
                      desc="Predicting matches for query spectra",
                      disable=not self.settings["progress_bars"],
                      total=len(query_spectra)):
             query_spectrum.set("spectrum_nr", i+1)
@@ -411,15 +400,15 @@
                 sum(average_inchikey_scores[closely_related_inchikey14] for closely_related_inchikey14 in closest_library_structures)
             average_ms2deepscore_multiple_library_structures = sum_of_average_ms2ds_multiple_library_structures/ len(closest_library_structures)
             results_per_inchikey[inchikey] = (average_ms2deepscore_multiple_library_structures, average_tanimoto_score_multiple_library_spectra)
         return results_per_inchikey
 
     def _get_s2v_scores(self,
                         query_spectrum: Spectrum,
-                        preselection_of_library_ids: List[str]
+                        preselection_of_library_ids: List[int]
                         ) -> np.ndarray:
         """Returns the s2v scores
 
         query_spectrum:
             Spectrum object
         preselection_of_library_ids:
             list of spectrum ids for which the s2v scores should be calculated
@@ -454,15 +443,15 @@
     result_table.add_ms2query_meta_score(predictions)
     return result_table
 
 
 def select_files_for_ms2query(file_names: List[str], files_to_select=None):
     """Selects the files needed for MS2Library based on their file extensions. """
     dict_with_file_extensions = \
-        {"sqlite": ".sqlite", "classifiers": "CF_NPC_classes.txt", "s2v_model": ".model", "ms2ds_model": ".hdf5",
+        {"sqlite": ".sqlite", "s2v_model": ".model", "ms2ds_model": ".hdf5",
          "ms2query_model": ".onnx", "s2v_embeddings": "s2v_embeddings.pickle",
          "ms2ds_embeddings": "ms2ds_embeddings.pickle"}
     if files_to_select is not None:
         dict_with_file_extensions = {key: value for key, value in dict_with_file_extensions.items()
                                      if key in files_to_select}
     # Create a dictionary with None as values.
     dict_with_file_names = {key: None for key in dict_with_file_extensions}
@@ -482,16 +471,14 @@
     for file_type, stored_file_name in dict_with_file_names.items():
         if file_type == "ms2query_model" and stored_file_name is None:
             assert dict_with_file_names["ms2query_model_pickle"] is None, \
                 "Only a MS2Query model in pickled format was found. The current version of MS2Query needs a .onnx format. " \
                 "To download the new format check the readme https://github.com/iomega/ms2query. " \
                 "Alternatively MS2Query can be downgraded to version <= 0.6.7"
             assert False, "The MS2Query model was not found in the directory"
-        elif file_type == "classifiers" and stored_file_name is None:
-            print("The classifiers file has not been specified, therefore no classes will be predicted.")
         elif file_type != "ms2query_model_pickle":
             assert stored_file_name is not None, \
                 f"The file type {file_type} was not found in the file names: {file_names}"
     return dict_with_file_names
 
 
 def create_library_object_from_one_dir(directory_containing_library_and_models: str) -> MS2Library:
@@ -509,14 +496,10 @@
     # Adds the path in front of the file names
     dict_with_file_paths = {}
     for key, file_name in dict_with_file_names.items():
         if file_name is not None:
             dict_with_file_paths[key] = os.path.join(directory_containing_library_and_models, file_name)
         else:
             dict_with_file_paths[key] = None
-    return MS2Library(dict_with_file_paths["sqlite"],
-                      dict_with_file_paths["s2v_model"],
-                      dict_with_file_paths["ms2ds_model"],
-                      dict_with_file_paths["s2v_embeddings"],
-                      dict_with_file_paths["ms2ds_embeddings"],
-                      dict_with_file_paths["ms2query_model"],
-                      dict_with_file_paths["classifiers"])
+    return MS2Library(dict_with_file_paths["sqlite"], dict_with_file_paths["s2v_model"],
+                      dict_with_file_paths["ms2ds_model"], dict_with_file_paths["s2v_embeddings"],
+                      dict_with_file_paths["ms2ds_embeddings"], dict_with_file_paths["ms2query_model"])
```

### Comparing `ms2query-0.7.4/ms2query/old_query_from_sqlite_functions.py` & `ms2query-1.0.0/ms2query/old_query_from_sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/ms2query/results_table.py` & `ms2query-1.0.0/ms2query/results_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Tuple, Union
 import numpy as np
 import pandas as pd
 from matchms.Spectrum import Spectrum
-from ms2query.query_from_sqlite_database import get_metadata_from_sqlite
-from ms2query.utils import (column_names_for_output,
-                            get_classifier_from_csv_file)
+from ms2query.query_from_sqlite_database import SqliteLibrary
+from ms2query.utils import (column_names_for_output)
 
 
 class ResultsTable:
     default_columns = ["spectrum_ids",
                        "inchikey",
                        "precursor_mz_library_spectrum",
                        "precursor_mz_difference",
@@ -16,48 +15,46 @@
                        "ms2ds_score",
                        "average_ms2deepscore_multiple_library_structures",
                        "average_tanimoto_score_library_structures"]
 
     def __init__(self, preselection_cut_off: int,
                  ms2deepscores: pd.Series,
                  query_spectrum: Spectrum,
-                 sqlite_file_name: str,
-                 classifier_csv_file_name: Union[str, None] = None,
+                 sqlite_library: SqliteLibrary,
                  **kwargs):
-        # pylint: disable=too-many-arguments
 
         self.data = pd.DataFrame(columns=self.default_columns, **kwargs)
         self.ms2deepscores = ms2deepscores
         self.preselection_cut_off = preselection_cut_off
         self.query_spectrum = query_spectrum
         self.precursor_mz = query_spectrum.get("precursor_mz")
-        self.sqlite_file_name = sqlite_file_name
-        self.classifier_csv_file_name = classifier_csv_file_name
+        self.sqlite_library = sqlite_library
 
     def __eq__(self, other):
         if not isinstance(other, ResultsTable):
             return False
 
         # Round is used to prevent returning float for float rounding errors
+        # We cannot check the sqlite file location, since this will have a different path on a virtual machine.
         return other.preselection_cut_off == self.preselection_cut_off and \
             other.precursor_mz == self.precursor_mz and \
             self.data.round(5).equals(other.data.round(5)) and \
             self.ms2deepscores.round(5).equals(other.ms2deepscores.round(5)) and \
-            self.query_spectrum.__eq__(other.query_spectrum) and \
-            self.sqlite_file_name == other.sqlite_file_name
+            self.query_spectrum.__eq__(other.query_spectrum)
 
     def assert_results_table_equal(self, other):
         """Assert if results tables are equal except for the spectrum metadata and sqlite file name"""
         assert isinstance(other, ResultsTable), "Expected ResultsTable"
         assert other.preselection_cut_off == self.preselection_cut_off
         assert other.precursor_mz == self.precursor_mz
         pd.testing.assert_frame_equal(self.data, other.data, check_less_precise=True, check_dtype=False)
         assert self.ms2deepscores.round(5).equals(other.ms2deepscores.round(5)), f"ms2deepscores are not equal {self.ms2deepscores} != {other.ms2deepscores}"
         assert self.query_spectrum.peaks == other.query_spectrum.peaks
         assert self.query_spectrum.losses == other.query_spectrum.losses
+        # We cannot check the sqlite file location, since this will have a different path on a virtual machine.
 
     def set_index(self, column_name):
         self.data = self.data.set_index(column_name)
 
     def add_related_inchikey_scores(self, related_inchikey_scores):
 
         self.data["average_ms2deepscore_multiple_library_structures"] = \
@@ -98,16 +95,16 @@
                           "average_ms2deepscore_multiple_library_structures",
                           "average_tanimoto_score_library_structures"]]
 
     def export_to_dataframe(
             self,
             nr_of_top_spectra: int,
             minimal_ms2query_score: Union[float, int] = 0.0,
-            additional_metadata_columns: Tuple[str] = None,
-            additional_ms2query_score_columns: Tuple[str] = None
+            additional_metadata_columns: Tuple[str, ...] = None,
+            additional_ms2query_score_columns: Tuple[str, ...] = None
             ) -> Union[None, pd.DataFrame]:
         """Returns a dataframe with analogs results from results table
 
         Args:
         ------
         nr_of_top_spectra:
             Number of spectra that should be returned.
@@ -131,44 +128,46 @@
             (selected_analogs["ms2query_model_prediction"] > minimal_ms2query_score)]
         nr_of_analogs = len(selected_analogs)
         # Return None if know analogs are selected.
         if selected_analogs.empty:
             return None
 
         # For each analog the compound name is selected from sqlite
-        metadata_dict = get_metadata_from_sqlite(self.sqlite_file_name,
-                                                 list(selected_analogs["spectrum_ids"]))
+        metadata_dict = self.sqlite_library.get_metadata_from_sqlite(list(selected_analogs["spectrum_ids"]))
         compound_name_list = [metadata_dict[analog_spectrum_id]["compound_name"]
                               for analog_spectrum_id
                               in list(selected_analogs["spectrum_ids"])]
+        smiles_list = [metadata_dict[analog_spectrum_id]["smiles"]
+                       for analog_spectrum_id
+                       in list(selected_analogs["spectrum_ids"])]
 
         # Add inchikey and ms2query model prediction to results df
         # results_df = selected_analogs.loc[:, ["spectrum_ids", "ms2query_model_prediction", "inchikey"]]
         results_df = pd.DataFrame({"query_spectrum_nr": self.query_spectrum.get("spectrum_nr"),
-                                   "spectrum_ids": selected_analogs["spectrum_ids"],
+                                   # "spectrum_ids": selected_analogs["spectrum_ids"],
                                    "ms2query_model_prediction": selected_analogs["ms2query_model_prediction"],
                                    "inchikey": selected_analogs["inchikey"],
                                    "precursor_mz_analog": selected_analogs["precursor_mz_library_spectrum"],
                                    "precursor_mz_query_spectrum": [self.precursor_mz] * nr_of_analogs,
+                                   "smiles": smiles_list,
                                    "analog_compound_name": compound_name_list,
-                                   "precursor_mz_difference": selected_analogs["precursor_mz_difference"]
+                                   "precursor_mz_difference": selected_analogs["precursor_mz_difference"],
                                    })
         if additional_metadata_columns is not None:
             for metadata_name in additional_metadata_columns:
                 results_df[metadata_name] = [self.query_spectrum.get(metadata_name)] * nr_of_analogs
         if additional_ms2query_score_columns is not None:
             for score in additional_ms2query_score_columns:
                 results_df[score] = selected_analogs[score]
 
         # Orders the columns in the right way
         results_df = results_df.reindex(
             columns=column_names_for_output(True, False, additional_metadata_columns,
                                             additional_ms2query_score_columns))
+
         # Add classifiers to dataframe
-        if self.classifier_csv_file_name is not None:
-            classifiers_df = \
-                get_classifier_from_csv_file(self.classifier_csv_file_name,
-                                             results_df["inchikey"].unique())
+        if self.sqlite_library.contains_class_annotation():
+            classifiers_df = self.sqlite_library.get_classes_inchikeys(results_df["inchikey"].unique())
             results_df = pd.merge(results_df,
                                   classifiers_df,
                                   on="inchikey")
         return results_df
```

### Comparing `ms2query-0.7.4/ms2query/run_ms2query.py` & `ms2query-1.0.0/ms2query/run_ms2query.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from urllib.request import urlopen, urlretrieve
 from ms2query.ms2library import MS2Library
 from ms2query.utils import load_matchms_spectrum_objects_from_file, SettingsRunMS2Query, return_non_existing_file_name
 
 
 def zenodo_dois(ionisation_mode):
     "Returns the most up to date url for Zenodo"
-    zenodo_DOIs = {"positive": 7753249,
-                   "negative": 7753267}
+    zenodo_DOIs = {"positive": 6124552,
+                   "negative": 7104184}
     assert ionisation_mode in zenodo_DOIs, "Expected 'positive' or 'negative' as input"
     zenodo_doi = zenodo_DOIs[ionisation_mode]
     zenodo_metadata_url = "https://zenodo.org/api/records/" + str(zenodo_doi)
     zenodo_files_url = f"https://zenodo.org/record/{zenodo_doi}/files/"
     return zenodo_metadata_url, zenodo_files_url
```

### Comparing `ms2query-0.7.4/ms2query/utils.py` & `ms2query-1.0.0/ms2query/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import sys
 import json
 from typing import List, Union, Tuple, Optional
 import numpy as np
-import pandas as pd
 from matchms import importing
 from spec2vec.Spec2Vec import Spectrum
 from skl2onnx import convert_sklearn
 from skl2onnx.common.data_types import FloatTensorType
 from onnxruntime import InferenceSession
 
 
@@ -121,57 +120,18 @@
     else:
         for spectrum in spectrum_list:
             if spectrum.get("charge") is None:
                 spectrum.set("charge", charge_to_use)
     return spectrum_list
 
 
-def get_classifier_from_csv_file(classifier_file_name: str,
-                                 list_of_inchikeys: List[str]):
-    """Returns a dataframe with the classifiers for a selection of inchikeys
-
-    Args:
-    ------
-    csv_file_name:
-        File name of text file with tap separated columns, with classifier
-        information.
-    list_of_inchikeys:
-        list with the first 14 letters of inchikeys, that are selected from
-        the classifier file.
-    """
-    assert os.path.isfile(classifier_file_name), \
-        f"The given classifier csv file does not exist: {classifier_file_name}"
-    classifiers_df = pd.read_csv(classifier_file_name, sep="\t")
-    classifiers_df.rename(columns={"inchi_key": "inchikey"}, inplace=True)
-    columns_to_keep = ["inchikey"] + column_names_for_output(False, True)
-    list_of_classifiers = []
-    for inchikey in list_of_inchikeys:
-        classifiers = classifiers_df.loc[
-            classifiers_df["inchikey"].str.startswith(inchikey)]
-        if classifiers.empty:
-            list_of_classifiers.append(pd.DataFrame(np.array(
-                [[inchikey] + [np.nan] * (len(columns_to_keep) - 1)]),
-                columns=columns_to_keep))
-        else:
-            classifiers = classifiers[columns_to_keep].iloc[:1]
-
-            list_of_classifiers.append(classifiers)
-    if len(list_of_classifiers) == 0:
-        results = pd.DataFrame(columns=columns_to_keep)
-    else:
-        results = pd.concat(list_of_classifiers, axis=0, ignore_index=True)
-
-    results["inchikey"] = list_of_inchikeys
-    return results
-
-
 def column_names_for_output(return_non_classifier_columns: bool,
                             return_classifier_columns: bool,
-                            additional_metadata_columns: Tuple[str] = None,
-                            additional_ms2query_score_columns: Tuple[str] = None) -> List[str]:
+                            additional_metadata_columns: Tuple[str, ...] = None,
+                            additional_ms2query_score_columns: Tuple[str, ...] = None) -> List[str]:
     """Returns the column names for the output of results table
 
     This is used by the functions MS2Library.analog_search_store_in_csv, ResultsTable.export_to_dataframe
     and get_classifier_from_csv_file. The column names are used to select which data is added from the ResultsTable to
     the dataframe and the order of these columns is also used as order for the columns in this dataframe.
 
     Args:
@@ -186,20 +146,20 @@
         True, only the classifier columns are returned.
     additional_metadata_columns:
         These columns are appended to the standard columns and returned when return_non_classifier_columns is true
     additional_ms2query_score_columns:
         These columns are appended to the standard columns and returned when return_non_classifier_columns is true
     """
     standard_columns = ["query_spectrum_nr", "ms2query_model_prediction", "precursor_mz_difference", "precursor_mz_query_spectrum",
-                        "precursor_mz_analog", "inchikey", "spectrum_ids", "analog_compound_name"]
+                        "precursor_mz_analog", "inchikey", "analog_compound_name", "smiles",]
     if additional_metadata_columns is not None:
         standard_columns += additional_metadata_columns
     if additional_ms2query_score_columns is not None:
         standard_columns += additional_ms2query_score_columns
-    classifier_columns = ["smiles", "cf_kingdom", "cf_superclass", "cf_class", "cf_subclass",
+    classifier_columns = ["cf_kingdom", "cf_superclass", "cf_class", "cf_subclass",
                           "cf_direct_parent", "npc_class_results", "npc_superclass_results", "npc_pathway_results"]
     if return_classifier_columns and return_non_classifier_columns:
         return standard_columns + classifier_columns
     if return_classifier_columns:
         return classifier_columns
     if return_non_classifier_columns:
         return standard_columns
```

### Comparing `ms2query-0.7.4/ms2query.egg-info/PKG-INFO` & `ms2query-1.0.0/ms2query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2query
-Version: 0.7.4
+Version: 1.0.0
 Summary: Tool to query MS/MS spectra against mass spectral library
 Home-page: https://github.com/iomega/ms2query
 Author: Netherlands eScience Center
 Author-email: 
 License: Apache Software License 2.0
 Description: [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iomega/ms2query/CI_build.yml)](https://github.com/iomega/ms2query/actions/workflows/CI_build.yml)
         ![GitHub](https://img.shields.io/github/license/iomega/ms2query)
```

### Comparing `ms2query-0.7.4/ms2query.egg-info/SOURCES.txt` & `ms2query-1.0.0/ms2query.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,31 @@
 ms2query/benchmarking/__init__.py
 ms2query/benchmarking/collect_test_data_results.py
 ms2query/benchmarking/create_accuracy_vs_recall_plot.py
 ms2query/benchmarking/k_fold_cross_validation.py
 ms2query/benchmarking/visualize_mass_distribution.py
 ms2query/benchmarking/visualize_tanimoto_score_distribution.py
 ms2query/create_new_library/__init__.py
+ms2query/create_new_library/add_classifire_classifications.py
 ms2query/create_new_library/calculate_tanimoto_scores.py
 ms2query/create_new_library/create_sqlite_database.py
 ms2query/create_new_library/library_files_creator.py
 ms2query/create_new_library/split_data_for_training.py
 ms2query/create_new_library/train_models.py
 ms2query/create_new_library/train_ms2deepscore.py
 ms2query/create_new_library/train_ms2query_model.py
 tests/__init__.py
+tests/conftest.py
+tests/test_add_classifier_annotations.py
 tests/test_calculate_tanimoto_scores.py
 tests/test_clean_and_filter_spectra.py
 tests/test_collect_test_data_results.py
 tests/test_library_files_creator.py
 tests/test_ms2library.py
 tests/test_results_table.py
 tests/test_run_ms2query.py
 tests/test_split_data_for_training.py
 tests/test_sqlite.py
 tests/test_train_models.py
 tests/test_train_ms2deepscore.py
 tests/test_train_ms2query_model.py
-tests/test_use_files_without_spectrum_id.py
 tests/test_utils.py
```

### Comparing `ms2query-0.7.4/ms2query.egg-info/requires.txt` & `ms2query-1.0.0/ms2query.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/setup.py` & `ms2query-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/tests/test_calculate_tanimoto_scores.py` & `ms2query-1.0.0/tests/test_calculate_tanimoto_scores.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import pandas as pd
 
 from ms2query.clean_and_filter_spectra import normalize_and_filter_peaks_multiple_spectra
 from ms2query.create_new_library.calculate_tanimoto_scores import calculate_tanimoto_scores_unique_inchikey, \
     calculate_highest_tanimoto_score
 from ms2query.utils import load_matchms_spectrum_objects_from_file, load_pickled_file
-from tests.test_utils import path_to_general_test_files
 
 
 def test_calculate_tanimoto_scores_unique_inchikey(path_to_general_test_files):
     spectra = load_matchms_spectrum_objects_from_file(
         os.path.join(path_to_general_test_files, '100_test_spectra.pickle'))
     tanimoto_df = calculate_tanimoto_scores_unique_inchikey(spectra, spectra)
     expected_tanimoto_df = load_pickled_file(os.path.join(path_to_general_test_files,
```

### Comparing `ms2query-0.7.4/tests/test_clean_and_filter_spectra.py` & `ms2query-1.0.0/tests/test_clean_and_filter_spectra.py`

 * *Files identical despite different names*

### Comparing `ms2query-0.7.4/tests/test_collect_test_data_results.py` & `ms2query-1.0.0/tests/test_collect_test_data_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import os
 import pandas as pd
 import pytest
-from typing import Dict, List, Tuple
 import numpy as np
 from matchms import Spectrum
 from ms2query.benchmarking.collect_test_data_results import (generate_test_results_ms2query,
                                                              get_all_ms2ds_scores,
                                                              select_highest_ms2ds_in_mass_range,
                                                              get_modified_cosine_score_results,
                                                              get_cosines_score_results,
                                                              create_optimal_results,
                                                              create_random_results,
                                                              generate_test_results)
 
-from tests.test_use_files_without_spectrum_id import ms2library_without_spectrum_id
 from ms2query.utils import load_matchms_spectrum_objects_from_file, load_json_file
-from tests.test_utils import path_to_general_test_files
 
 
 @pytest.fixture
-def test_spectra():
+def local_test_spectra():
     """Returns a list with two spectra
 
     The spectra are created by using peaks from the first two spectra in
     100_test_spectra.pickle, to make sure that the peaks occur in the s2v
     model. The other values are random.
     """
     spectrum1 = Spectrum(
@@ -43,116 +40,116 @@
                   'precursor_mz': 928.0,
                   'inchikey': 'SCYRNRIZFGMUSB-STOGWRBBSA-N',
                   'smiles': "CCCCC"
                   })
     return [spectrum1, spectrum2]
 
 
-def test_generate_test_results_ms2query(ms2library_without_spectrum_id, test_spectra):
-    result = generate_test_results_ms2query(ms2library_without_spectrum_id, test_spectra)
+def test_generate_test_results_ms2query(ms2library, local_test_spectra):
+    result = generate_test_results_ms2query(ms2library, local_test_spectra)
     np.testing.assert_almost_equal(result[0], (0.5645, 0.003861003861003861, False))
     np.testing.assert_almost_equal(result[1], (0.409, 0.010610079575596816, False))
 
     # test if a spectrum that does not pass the tests is not added to the results
-    test_spectra[0] = test_spectra[0].set("precursor_mz", None)
-    test_spectra[0] = test_spectra[0].set("pepmass", None)
-    result = generate_test_results_ms2query(ms2library_without_spectrum_id, test_spectra)
+    local_test_spectra[0] = local_test_spectra[0].set("precursor_mz", None)
+    local_test_spectra[0] = local_test_spectra[0].set("pepmass", None)
+    result = generate_test_results_ms2query(ms2library, local_test_spectra)
     assert result[0] is None
     np.testing.assert_almost_equal(result[1], (0.409, 0.010610079575596816, False))
 
 
-def test_get_all_ms2ds_scores(ms2library_without_spectrum_id, test_spectra):
-    result = get_all_ms2ds_scores(ms2library_without_spectrum_id.ms2ds_model,
-                                  ms2library_without_spectrum_id.ms2ds_embeddings,
-                                  test_spectra)
+def test_get_all_ms2ds_scores(ms2library, local_test_spectra):
+    result = get_all_ms2ds_scores(ms2library.ms2ds_model,
+                                  ms2library.ms2ds_embeddings,
+                                  local_test_spectra)
     assert isinstance(result, pd.DataFrame)
     assert float(result.iloc[0, 0]).__round__(5) == 0.76655
 
 
-def test_select_highest_ms2ds_in_mass_range(ms2library_without_spectrum_id, test_spectra):
-    ms2ds = get_all_ms2ds_scores(ms2library_without_spectrum_id.ms2ds_model,
-                                 ms2library_without_spectrum_id.ms2ds_embeddings,
-                                 test_spectra)
+def test_select_highest_ms2ds_in_mass_range(ms2library, local_test_spectra):
+    ms2ds = get_all_ms2ds_scores(ms2library.ms2ds_model,
+                                 ms2library.ms2ds_embeddings,
+                                 local_test_spectra)
 
     # test with mass 100 preselection
     result = select_highest_ms2ds_in_mass_range(ms2ds,
-                                                test_spectra,
-                                                ms2library_without_spectrum_id.sqlite_file_name,
+                                                local_test_spectra,
+                                                ms2library.sqlite_library,
                                                 100)
     np.testing.assert_almost_equal(result[0], (0.8492529314990583, 0.003861003861003861, False))
     np.testing.assert_almost_equal(result[1], (0.6413115894635883, 0.013745704467353952, False))
 
     # test without mass preselection
     result_without_mass_range = select_highest_ms2ds_in_mass_range(ms2ds,
-                                                                   test_spectra,
-                                                                   ms2library_without_spectrum_id.sqlite_file_name,
+                                                                   local_test_spectra,
+                                                                   ms2library.sqlite_library,
                                                                    None)
     np.testing.assert_almost_equal(result_without_mass_range[0], (0.8492529314990583, 0.003861003861003861, False))
     np.testing.assert_almost_equal(result_without_mass_range[1], (0.8514114889698237, 0.007292616226071103, False))
 
     # test with mass preselection resulting in 0 and 1 library spectra within mass range
     result = select_highest_ms2ds_in_mass_range(ms2ds,
-                                                test_spectra,
-                                                ms2library_without_spectrum_id.sqlite_file_name,
+                                                local_test_spectra,
+                                                ms2library.sqlite_library,
                                                 5.56)
     np.testing.assert_almost_equal(result[0], (0.7368508, 0.004461, False))
     assert result[1] is None
 
 
-def test_get_modified_cosine_score_results(test_spectra):
+def test_get_modified_cosine_score_results(local_test_spectra):
     library_spectra = load_matchms_spectrum_objects_from_file(os.path.join(
         os.path.split(os.path.dirname(__file__))[0],
         'tests/test_files/general_test_files/100_test_spectra.pickle'))
-    results = get_modified_cosine_score_results(library_spectra, test_spectra, 100)
+    results = get_modified_cosine_score_results(library_spectra, local_test_spectra, 100)
     np.testing.assert_almost_equal(results,
                                    [(0.434789196140529, 0.003861003861003861, False),
                                     (0.4955472245596076, 0.007866273352999017, False)])
     # Test if no error happens when only 1 or 0 library spectra within mass range
-    results = get_modified_cosine_score_results(library_spectra, test_spectra, 5.56)
+    results = get_modified_cosine_score_results(library_spectra, local_test_spectra, 5.56)
     np.testing.assert_almost_equal(results[0],
                                    (0.0, 0.0044609665427509295, False))
     assert results[1] is None
 
 
-def test_get_cosines_score_results(test_spectra):
+def test_get_cosines_score_results(local_test_spectra):
     library_spectra = load_matchms_spectrum_objects_from_file(os.path.join(
         os.path.split(os.path.dirname(__file__))[0],
         'tests/test_files/general_test_files/100_test_spectra.pickle'))
-    result = get_cosines_score_results(library_spectra, test_spectra, 100, 0.05, 3)
+    result = get_cosines_score_results(library_spectra, local_test_spectra, 100, 0.05, 3)
     np.testing.assert_almost_equal(result,
                                    [(0.434789196140529, 0.0058997050147492625, False),
                                     (0.4955472245596076, 0.007866273352999017, False)])
     # Test if no error happens when only 1 or 0 library spectra within mass range
-    result = get_cosines_score_results(library_spectra, test_spectra, 5.56, 0.05, 0)
+    result = get_cosines_score_results(library_spectra, local_test_spectra, 5.56, 0.05, 0)
     np.testing.assert_almost_equal(result[0],
                                    (0.0, 0.004461, False))
     assert result[1] is None
 
 
-def test_create_optimal_results(test_spectra):
-    results = create_optimal_results(test_spectra, test_spectra)
+def test_create_optimal_results(local_test_spectra):
+    results = create_optimal_results(local_test_spectra, local_test_spectra)
     assert results == [(1.0, 1.0, True), (1.0, 1.0, True)]
 
 
-def test_random_results(test_spectra):
-    results = create_random_results(test_spectra,
-                                    test_spectra)
-    assert len(results) == len(test_spectra)
+def test_random_results(local_test_spectra):
+    results = create_random_results(local_test_spectra,
+                                    local_test_spectra)
+    assert len(results) == len(local_test_spectra)
 
 
-def test_generate_test_results(test_spectra,
-                               ms2library_without_spectrum_id,
+def test_generate_test_results(local_test_spectra,
+                               ms2library,
                                path_to_general_test_files,
                                tmp_path):
     library_spectra = load_matchms_spectrum_objects_from_file(os.path.join(
         path_to_general_test_files,
         '100_test_spectra.pickle'))
-    generate_test_results(ms2library_without_spectrum_id,
+    generate_test_results(ms2library,
                           library_spectra,
-                          test_spectra,
+                          local_test_spectra,
                           tmp_path)
     files_made = os.listdir(tmp_path)
     assert set(files_made) == {'cosine_score_100_da_test_results.json', 'modified_cosine_score_100_Da_test_results.json',
                           'ms2deepscore_test_results_100_Da.json', 'ms2deepscore_test_results_all.json',
                           'ms2query_test_results.json', 'optimal_results.json', 'random_results.json'}
     for file in files_made:
         result = load_json_file(os.path.join(tmp_path, file))
```

### Comparing `ms2query-0.7.4/tests/test_library_files_creator.py` & `ms2query-1.0.0/tests/test_library_files_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import pandas as pd
 import pytest
 from ms2query.create_new_library.library_files_creator import LibraryFilesCreator
 from ms2query.utils import (load_matchms_spectrum_objects_from_file,
                             load_pickled_file)
 from ms2query.clean_and_filter_spectra import normalize_and_filter_peaks
-from tests.test_utils import path_to_general_test_files
 
 
 def test_give_already_used_file_name(tmp_path, path_to_general_test_files):
     already_existing_file = os.path.join(tmp_path, "ms2query_library.sqlite")
     with open(already_existing_file, "w") as file:
         file.write("test")
 
@@ -33,15 +32,14 @@
     new_embeddings_file_name = os.path.join(base_file_name, "ms2ds_embeddings.pickle")
     assert os.path.isfile(new_embeddings_file_name), \
         "Expected file to be created"
     # Test if correct embeddings are stored
     embeddings = load_pickled_file(new_embeddings_file_name)
     expected_embeddings = load_pickled_file(os.path.join(
         path_to_general_test_files,
-        "test_files_without_spectrum_id",
         "100_test_spectra_ms2ds_embeddings.pickle"))
     pd.testing.assert_frame_equal(embeddings, expected_embeddings,
                                   check_exact=False,
                                   atol=1e-5)
 
 
 def test_store_s2v_embeddings(tmp_path, path_to_general_test_files):
@@ -57,12 +55,20 @@
 
     new_embeddings_file_name = os.path.join(base_file_name, "s2v_embeddings.pickle")
     assert os.path.isfile(new_embeddings_file_name), \
         "Expected file to be created"
     embeddings = load_pickled_file(new_embeddings_file_name)
     expected_embeddings = load_pickled_file(os.path.join(
         path_to_general_test_files,
-        "test_files_without_spectrum_id",
         "100_test_spectra_s2v_embeddings.pickle"))
     pd.testing.assert_frame_equal(embeddings, expected_embeddings,
                                   check_exact=False,
                                   atol=1e-5)
+
+
+def test_create_sqlite_file(tmp_path, path_to_general_test_files):
+    library_spectra = load_matchms_spectrum_objects_from_file(os.path.join(
+        path_to_general_test_files, '100_test_spectra.pickle'))
+    test_create_files = LibraryFilesCreator(
+        library_spectra[:20], output_directory=os.path.join(tmp_path, '100_test_spectra'))
+    test_create_files.create_sqlite_file()
+
```

### Comparing `ms2query-0.7.4/tests/test_split_data_for_training.py` & `ms2query-1.0.0/tests/test_split_data_for_training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
-import pytest
 from ms2query.utils import load_matchms_spectrum_objects_from_file
 from ms2query.create_new_library.split_data_for_training import split_spectra_on_inchikeys, \
     split_spectra_in_random_inchikey_sets, select_unique_inchikeys
-from tests.test_utils import path_to_general_test_files
 
 
 def test_split_spectra_on_inchikeys(path_to_general_test_files):
     spectra = load_matchms_spectrum_objects_from_file(
         os.path.join(path_to_general_test_files, '100_test_spectra.pickle'))
     training_spectra, validation_spectra = split_spectra_on_inchikeys(spectra, 10)
     assert isinstance(training_spectra, list)
```

### Comparing `ms2query-0.7.4/tests/test_sqlite.py` & `ms2query-1.0.0/tests/test_sqlite.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 tanimoto scores (create_sqlite_database.py) and functions to retrieve
 information from the sqlite database.
 """
 
 import os
 import sqlite3
 import numpy as np
+import pandas as pd
 from ms2query.create_new_library.create_sqlite_database import make_sqlfile_wrapper
-from ms2query.query_from_sqlite_database import get_metadata_from_sqlite, get_ionization_mode_library
 from ms2query.clean_and_filter_spectra import normalize_and_filter_peaks_multiple_spectra
-from ms2query.utils import load_pickled_file
+from ms2query.utils import load_pickled_file, column_names_for_output
+from ms2query.create_new_library.add_classifire_classifications import convert_to_dataframe
 
 
 def check_sqlite_files_are_equal(new_sqlite_file_name, reference_sqlite_file):
     """Raises an error if the two sqlite files are not equal"""
     # Test if file is made
     assert os.path.isfile(new_sqlite_file_name), \
         "Expected a file to be created"
+    assert os.path.isfile(reference_sqlite_file), \
+        "The reference file given does not exist"
 
     # Test if the file has the correct information
     get_table_names = \
         "SELECT name FROM sqlite_master WHERE type='table' order by name"
     conn1 = sqlite3.connect(new_sqlite_file_name)
     cur1 = conn1.cursor()
     table_names1 = cur1.execute(get_table_names).fetchall()
@@ -60,72 +63,103 @@
                                                verbose=True)
             else:
                 assert rows_1 == rows_2, error_msg
     conn1.close()
     conn2.close()
 
 
-def test_making_sqlite_file(tmp_path):
+def test_making_sqlite_file_without_classes(tmp_path):
     """Makes a temporary sqlite file and tests if it contains the correct info
     """
     # tmp_path is a fixture that makes sure a temporary file is created
     new_sqlite_file_name = os.path.join(tmp_path,
                                         "test_spectra_database.sqlite")
 
     path_to_general_test_files = os.path.join(
         os.path.split(os.path.dirname(__file__))[0],
         'tests/test_files/general_test_files')
 
     reference_sqlite_file = os.path.join(path_to_general_test_files,
-                                         "test_files_without_spectrum_id",
-                                         "100_test_spectra.sqlite")
+                                         "..",
+                                         "backwards_compatibility",
+                                         "100_test_spectra_without_classes.sqlite")
 
     list_of_spectra = load_pickled_file(os.path.join(
         path_to_general_test_files, "100_test_spectra.pickle"))
     list_of_spectra = normalize_and_filter_peaks_multiple_spectra(list_of_spectra)
 
     # Create sqlite file, with 3 tables
     make_sqlfile_wrapper(new_sqlite_file_name,
                          list_of_spectra,
                          columns_dict={"precursor_mz": "REAL"})
     check_sqlite_files_are_equal(new_sqlite_file_name, reference_sqlite_file)
 
 
-def test_get_metadata_from_sqlite():
-    path_to_test_files_sqlite_dir = os.path.join(
-        os.path.split(os.path.dirname(__file__))[0],
-        'tests/test_files')
-    sqlite_file_name = os.path.join(path_to_test_files_sqlite_dir,
-                                    "test_spectra_database.sqlite")
+def test_making_sqlite_file_with_compound_classes(tmp_path, path_to_general_test_files):
+    """Makes a temporary sqlite file and tests if it contains the correct info
+    """
+    def generate_compound_classes(spectra):
+        inchikeys = {spectrum.get("inchikey")[:14] for spectrum in spectra}
+        inchikey_results_list = []
+        for inchikey in inchikeys:
+            inchikey_results_list.append([inchikey, "b", "c", "d", "e", "f", "g", "h", "i", "j"])
+        compound_class_df = convert_to_dataframe(inchikey_results_list)
+        return compound_class_df
+    # tmp_path is a fixture that makes sure a temporary file is created
+    new_sqlite_file_name = os.path.join(tmp_path,
+                                        "test_spectra_database.sqlite")
+
+    reference_sqlite_file = os.path.join(path_to_general_test_files,
+                                         "100_test_spectra.sqlite")
+
+    list_of_spectra = load_pickled_file(os.path.join(
+        path_to_general_test_files, "100_test_spectra.pickle"))
+    list_of_spectra = normalize_and_filter_peaks_multiple_spectra(list_of_spectra)
+
+    # Create sqlite file, with 3 tables
+    make_sqlfile_wrapper(new_sqlite_file_name,
+                         list_of_spectra,
+                         columns_dict={"precursor_mz": "REAL"},
+                         compound_classes=generate_compound_classes(spectra=list_of_spectra))
+
+    check_sqlite_files_are_equal(new_sqlite_file_name, reference_sqlite_file)
 
-    spectra_id_list = ['CCMSLIB00000001547', 'CCMSLIB00000001549']
 
-    result = get_metadata_from_sqlite(
-        sqlite_file_name,
+def test_get_metadata_from_sqlite(sqlite_library):
+    spectra_id_list = [0, 1]
+
+    result = sqlite_library.get_metadata_from_sqlite(
         spectra_id_list,
-        spectrum_id_storage_name="spectrum_id")
+        spectrum_id_storage_name="spectrumid")
     assert isinstance(result, dict), "Expected dictionary as output"
     assert len(result) == len(spectra_id_list), \
         "Expected the same number of results as the spectra_id_list"
     for spectrum_id in spectra_id_list:
-        assert spectrum_id in result, \
+        assert spectrum_id in result.keys(), \
             f"The spectrum_id {spectrum_id} was expected as key"
         metadata = result[spectrum_id]
         assert isinstance(metadata, dict), \
             "Expected metadata to be stored as dict"
-        assert metadata['spectrum_id'] == spectrum_id, \
-            "Expected different spectrum id in metadata"
         for key in metadata.keys():
             assert isinstance(key, str), \
                 "Expected keys of metadata to be string"
-            assert isinstance(metadata[key], (str, float, int, list)), \
+            assert isinstance(metadata[key], (str, float, int, list, tuple)), \
                 f"Expected values of metadata to be string {metadata[key]}"
 
 
-def test_get_ionization_mode_library():
-    path_to_test_files_sqlite_dir = os.path.join(
-        os.path.split(os.path.dirname(__file__))[0],
-        'tests/test_files')
-    sqlite_file_name = os.path.join(path_to_test_files_sqlite_dir,
-                                    "test_spectra_database.sqlite")
-    ionization_mode = get_ionization_mode_library(sqlite_file_name)
+def test_get_ionization_mode_library(sqlite_library):
+    ionization_mode = sqlite_library.get_ionization_mode_library()
     assert ionization_mode == "positive"
+
+
+def test_get_classes_inchikeys(sqlite_library):
+    test_inchikeys = ["IYDKWWDUBYWQGF", "KNGPFNUOXXLKCN"]
+    classes = sqlite_library.get_classes_inchikeys(test_inchikeys)
+    expected_classes = pd.DataFrame([["IYDKWWDUBYWQGF", "b", "c", "d", "e", "f", "g", "h", "i"],
+                                     ["KNGPFNUOXXLKCN", "b", "c", "d", "e", "f", "g", "h", "i"]],
+                                    columns=["inchikey"] + column_names_for_output(return_non_classifier_columns=False,
+                                                                                   return_classifier_columns=True))
+    pd.testing.assert_frame_equal(expected_classes, classes)
+
+
+def test_contains_class_annotiation(sqlite_library):
+    assert sqlite_library.contains_class_annotation(), "contains_class_annotation is expected to return True"
```

### Comparing `ms2query-0.7.4/tests/test_train_models.py` & `ms2query-1.0.0/tests/test_train_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
 import pytest
 from ms2query.create_new_library.train_models import clean_and_train_models
 from ms2query.ms2library import create_library_object_from_one_dir, MS2Library
-from tests.test_utils import path_to_general_test_files
 
-
-@pytest.mark.integration
-def test_train_all_models(path_to_general_test_files, tmp_path):
-    path_to_test_spectra = os.path.join(path_to_general_test_files, "1000_test_spectra.pickle")
-    models_folder = os.path.join(tmp_path, "models")
-    clean_and_train_models(path_to_test_spectra,
-                           "positive",
-                           models_folder,
-                           {"ms2ds_fraction_validation_spectra": 2,
-                            "ms2ds_epochs": 2,
-                            "spec2vec_iterations": 2,
-                            "ms2query_fraction_for_making_pairs": 400}
-                           )
-    ms2library = create_library_object_from_one_dir(models_folder)
-    assert isinstance(ms2library, MS2Library)
+# @pytest.mark.integration
+# def test_train_all_models(path_to_general_test_files, tmp_path):
+#     path_to_test_spectra = os.path.join(path_to_general_test_files, "1000_test_spectra.pickle")
+#     models_folder = os.path.join(tmp_path, "models")
+#     clean_and_train_models(path_to_test_spectra,
+#                            "positive",
+#                            models_folder,
+#                            {"ms2ds_fraction_validation_spectra": 2,
+#                             "ms2ds_epochs": 2,
+#                             "spec2vec_iterations": 2,
+#                             "ms2query_fraction_for_making_pairs": 400}
+#                            )
+#     ms2library = create_library_object_from_one_dir(models_folder)
+#     assert isinstance(ms2library, MS2Library)
```

### Comparing `ms2query-0.7.4/tests/test_train_ms2deepscore.py` & `ms2query-1.0.0/tests/test_train_ms2deepscore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
-import pytest
 from ms2deepscore.models import SiameseModel
 from ms2deepscore.models.load_model import load_model as load_ms2deepscore_model
 from ms2query.create_new_library.train_ms2deepscore import train_ms2ds_model
 from ms2query.utils import load_matchms_spectrum_objects_from_file, load_pickled_file
-from tests.test_utils import path_to_general_test_files
 
 
 def test_train_ms2ds_model(path_to_general_test_files, tmp_path):
     spectra = load_matchms_spectrum_objects_from_file(os.path.join(path_to_general_test_files, "100_test_spectra.pickle"))
     tanimoto_df = load_pickled_file(os.path.join(path_to_general_test_files, "100_test_spectra_tanimoto_scores.pickle"))
     model_file_name = os.path.join(tmp_path, "ms2ds_model.hdf5")
     epochs = 10
```

### Comparing `ms2query-0.7.4/tests/test_train_ms2query_model.py` & `ms2query-1.0.0/tests/test_train_ms2query_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,23 @@
         'tests/test_files')
 
 
 @pytest.fixture
 def ms2library(path_to_test_dir):
     path_to_general_tests_dir = os.path.join(path_to_test_dir, 'general_test_files')
 
-    return MS2Library(
-        sqlite_file_name= os.path.join(path_to_general_tests_dir, "100_test_spectra.sqlite"),
-        s2v_model_file_name=os.path.join(path_to_general_tests_dir, "100_test_spectra_s2v_model.model"),
-        ms2ds_model_file_name=os.path.join(path_to_general_tests_dir, "ms2ds_siamese_210301_5000_500_400.hdf5"),
-        pickled_s2v_embeddings_file_name=os.path.join(path_to_general_tests_dir, "100_test_spectra_s2v_embeddings.pickle"),
-        pickled_ms2ds_embeddings_file_name=os.path.join(path_to_general_tests_dir, "100_test_spectra_ms2ds_embeddings.pickle"),
-        ms2query_model_file_name=None,
-        classifier_csv_file_name=None)
+    return MS2Library(sqlite_file_name=os.path.join(path_to_general_tests_dir, "100_test_spectra.sqlite"),
+                      s2v_model_file_name=os.path.join(path_to_general_tests_dir, "100_test_spectra_s2v_model.model"),
+                      ms2ds_model_file_name=os.path.join(path_to_general_tests_dir,
+                                                         "ms2ds_siamese_210301_5000_500_400.hdf5"),
+                      pickled_s2v_embeddings_file_name=os.path.join(path_to_general_tests_dir,
+                                                                    "100_test_spectra_s2v_embeddings.pickle"),
+                      pickled_ms2ds_embeddings_file_name=os.path.join(path_to_general_tests_dir,
+                                                                      "100_test_spectra_ms2ds_embeddings.pickle"),
+                      ms2query_model_file_name=None)
 
 
 @pytest.fixture
 def query_spectra(path_to_test_dir):
     training_spectra_file_name = os.path.join(
         path_to_test_dir,
         "test_files_train_ms2query_nn/20_training_spectra.pickle")
@@ -61,16 +62,16 @@
     pd.testing.assert_frame_equal(result[0], expected_result[0], check_dtype=False, check_exact=False, rtol=1e-1)
     pd.testing.assert_frame_equal(result[1], expected_result[1], check_dtype=False, check_exact=False, rtol=1e-1)
 
 
 def test_calculate_all_tanimoto_scores(tmp_path, ms2library, query_spectra):
     query_spectrum = query_spectra[0]
     spectra_ids_list = \
-        ['CCMSLIB00000001603', 'CCMSLIB00000001652', 'CCMSLIB00000001640']
-    result = calculate_tanimoto_scores_with_library(ms2library.sqlite_file_name, query_spectrum, spectra_ids_list)
+        [38, 3, 60]
+    result = calculate_tanimoto_scores_with_library(ms2library.sqlite_library, query_spectrum, spectra_ids_list)
     expected_result = pd.DataFrame([0.199695, 0.177669, 0.192504],
                                    index=spectra_ids_list,
                                    columns=["Tanimoto_score"])
     assert isinstance(result, pd.DataFrame), "Expected a pd.Dataframe"
     pd.testing.assert_frame_equal(result, expected_result, check_dtype=False)
```

### Comparing `ms2query-0.7.4/tests/test_use_files_without_spectrum_id.py` & `ms2query-1.0.0/tests/test_run_ms2query.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,107 @@
 import os
 import sys
-import pytest
-from ms2query.run_ms2query import run_complete_folder
-from ms2query.utils import SettingsRunMS2Query
-from tests.test_ms2library import (MS2Library,
-                                   test_spectra)
-from tests.test_utils import create_test_classifier_csv_file
 
+import pandas as pd
+
+from ms2query.ms2library import create_library_object_from_one_dir, select_files_for_ms2query
+from ms2query.run_ms2query import download_zenodo_files, run_complete_folder, zenodo_dois, available_zenodo_files
+from ms2query.utils import SettingsRunMS2Query
+from tests.test_ms2library import MS2Library
+from tests.test_utils import check_correct_results_csv_file
 
 if sys.version_info < (3, 8):
     import pickle5 as pickle
 else:
     import pickle
 
 
-@pytest.fixture
-def ms2library_without_spectrum_id():
-    """Returns file names of the files needed to create MS2Library object"""
-    path_to_tests_dir = os.path.join(
-        os.path.split(os.path.dirname(__file__))[0],
-        'tests/test_files/')
-    sqlite_file_loc = os.path.join(
-        path_to_tests_dir,
-        "general_test_files", "test_files_without_spectrum_id", "100_test_spectra.sqlite")
-    spec2vec_model_file_loc = os.path.join(
-        path_to_tests_dir,
-        "general_test_files/100_test_spectra_s2v_model.model")
-    s2v_pickled_embeddings_file = os.path.join(
-        path_to_tests_dir,
-        "general_test_files", "test_files_without_spectrum_id", "100_test_spectra_s2v_embeddings.pickle")
-    ms2ds_model_file_name = os.path.join(
-        path_to_tests_dir,
-        "general_test_files/ms2ds_siamese_210301_5000_500_400.hdf5")
-    ms2ds_embeddings_file_name = os.path.join(
-        path_to_tests_dir,
-        "general_test_files", "test_files_without_spectrum_id", "100_test_spectra_ms2ds_embeddings.pickle")
-    spectrum_id_column_name = "spectrumid"
-    ms2q_model_file_name = os.path.join(path_to_tests_dir,
-        "general_test_files", "test_ms2q_rf_model.onnx")
-    ms2library = MS2Library(sqlite_file_loc,
-                            spec2vec_model_file_loc,
-                            ms2ds_model_file_name,
-                            s2v_pickled_embeddings_file,
-                            ms2ds_embeddings_file_name,
-                            ms2q_model_file_name,
-                            spectrum_id_column_name=spectrum_id_column_name)
-    return ms2library
+def test_download_zenodo():
+    """Tests if the files on zenodo match the load library from one dir settings"""
+    for ionisation_mode in ["positive", "negative"]:
+        zenodo_metadata_url, zenodo_files_url = zenodo_dois(ionisation_mode)
+        file_names_and_sizes = available_zenodo_files(zenodo_metadata_url)
+        file_names = [file_name for file_name in file_names_and_sizes]
+        select_files_for_ms2query(file_names)
+
+
+def test_download_models_only():
+    """Tests if downloading the models only works"""
+    for ionisation_mode in ["positive", "negative"]:
+        zenodo_metadata_url, zenodo_files_url = zenodo_dois(ionisation_mode)
+        file_names_and_sizes = available_zenodo_files(zenodo_metadata_url, only_models=True)
+        file_names = [file_name for file_name in file_names_and_sizes]
+        assert len(file_names) == 5
+
+
+def test_download_default_models(tmp_path):
+    """Tests downloading small files from zenodo
+
+    The files are a total of 20 MB from https://zenodo.org/record/7108049#.Yy2nPKRBxPY"""
+    run_test = False # Run test is set to false, since downloading takes too long for default testing
+    if run_test:
+        dir_to_store_positive_files = os.path.join(tmp_path, "positive_model")
+        dir_to_store_negative_files = os.path.join(tmp_path, "negative_model")
+
+        download_zenodo_files("positive", dir_to_store_positive_files)
+        download_zenodo_files("negative", dir_to_store_negative_files)
+        assert os.path.exists(dir_to_store_positive_files)
+        assert os.path.exists(dir_to_store_negative_files)
+        pos_ms2library = create_library_object_from_one_dir(dir_to_store_positive_files)
+        neg_ms2library = create_library_object_from_one_dir(dir_to_store_negative_files)
+        assert isinstance(pos_ms2library, MS2Library)
+        assert isinstance(neg_ms2library, MS2Library)
 
 
 def create_test_folder_with_spectra_files(path, spectra):
     """Creates a folder with two files containing two test spectra"""
     spectra_files_folder = os.path.join(path, "spectra_files_folder")
     os.mkdir(spectra_files_folder)
 
     pickle.dump(spectra, open(os.path.join(spectra_files_folder, "spectra_file_1.pickle"), "wb"))
     pickle.dump(spectra, open(os.path.join(spectra_files_folder, "spectra_file_2.pickle"), "wb"))
     return spectra_files_folder
 
 
-def test_run_complete_folder(tmp_path, ms2library_without_spectrum_id, test_spectra):
+def test_run_complete_folder(tmp_path, ms2library, test_spectra):
     folder_with_spectra = create_test_folder_with_spectra_files(tmp_path, test_spectra)
     results_directory = os.path.join(folder_with_spectra, "results")
 
-    run_complete_folder(ms2library=ms2library_without_spectrum_id,
+    run_complete_folder(ms2library=ms2library,
                         folder_with_spectra=folder_with_spectra)
     assert os.path.exists(results_directory), "Expected results directory to be created"
-
     assert os.listdir(os.path.join(results_directory)).sort() == ['spectra_file_1.csv', 'spectra_file_2.csv'].sort()
 
-    with open(os.path.join(os.path.join(results_directory, 'spectra_file_1.csv')), "r") as file:
-        assert file.readlines() == \
-               ['query_spectrum_nr,ms2query_model_prediction,precursor_mz_difference,precursor_mz_query_spectrum,precursor_mz_analog,inchikey,spectrum_ids,analog_compound_name,retention_time,retention_index\n',
-                '1,0.5645,33.2500,907.0000,940.2500,KNGPFNUOXXLKCN,1,Hoiamide B,,\n',
-                '2,0.4090,61.3670,928.0000,866.6330,GRJSOZDXIUZXEW,16,Halovir A,,\n']
-
-    with open(os.path.join(os.path.join(results_directory, 'spectra_file_2.csv')), "r") as file:
-        assert file.readlines() == \
-               ['query_spectrum_nr,ms2query_model_prediction,precursor_mz_difference,precursor_mz_query_spectrum,precursor_mz_analog,inchikey,spectrum_ids,analog_compound_name,retention_time,retention_index\n',
-                '1,0.5645,33.2500,907.0000,940.2500,KNGPFNUOXXLKCN,1,Hoiamide B,,\n',
-                '2,0.4090,61.3670,928.0000,866.6330,GRJSOZDXIUZXEW,16,Halovir A,,\n']
-
-
-def test_run_complete_folder_with_classifiers(tmp_path, ms2library_without_spectrum_id, test_spectra):
-    classifiers_file_location = create_test_classifier_csv_file(tmp_path)
-    ms2library_without_spectrum_id.classifier_file_name = classifiers_file_location
+    expected_headers = ['query_spectrum_nr', 'ms2query_model_prediction', 'precursor_mz_difference',
+                        'precursor_mz_query_spectrum', 'precursor_mz_analog', 'inchikey',
+                        'analog_compound_name', 'smiles', 'retention_time', 'retention_index']
+    check_correct_results_csv_file(pd.read_csv(os.path.join(os.path.join(results_directory, 'spectra_file_1.csv'))),
+                                   expected_headers)
+    check_correct_results_csv_file(pd.read_csv(os.path.join(os.path.join(results_directory, 'spectra_file_2.csv'))),
+                                   expected_headers)
+
 
+def test_run_complete_folder_with_classifiers(tmp_path, ms2library, test_spectra):
     folder_with_spectra = create_test_folder_with_spectra_files(tmp_path, test_spectra)
     results_directory = os.path.join(folder_with_spectra, "results")
     settings = SettingsRunMS2Query(minimal_ms2query_metascore=0,
                                    additional_metadata_columns=("charge",),
                                    additional_ms2query_score_columns=("s2v_score", "ms2ds_score"))
-    run_complete_folder(ms2library=ms2library_without_spectrum_id,
+    run_complete_folder(ms2library=ms2library,
                         folder_with_spectra=folder_with_spectra,
                         settings=settings
                         )
     assert os.path.exists(results_directory), "Expected results directory to be created"
 
     assert os.listdir(os.path.join(results_directory)).sort() == ['spectra_file_1.csv', 'spectra_file_2.csv'].sort()
 
-    with open(os.path.join(os.path.join(results_directory, 'spectra_file_1.csv')), "r") as file:
-        assert file.readlines() == \
-               ['query_spectrum_nr,ms2query_model_prediction,precursor_mz_difference,precursor_mz_query_spectrum,precursor_mz_analog,inchikey,spectrum_ids,analog_compound_name,charge,s2v_score,ms2ds_score,smiles,cf_kingdom,cf_superclass,cf_class,cf_subclass,cf_direct_parent,npc_class_results,npc_superclass_results,npc_pathway_results\n',
-                '1,0.5645,33.2500,907.0000,940.2500,KNGPFNUOXXLKCN,1,Hoiamide B,1,0.9996,0.9232,CCC[C@@H](C)[C@@H]([C@H](C)[C@@H]1[C@H]([C@H](Cc2nc(cs2)C3=N[C@](CS3)(C4=N[C@](CS4)(C(=O)N[C@H]([C@H]([C@H](C(=O)O[C@H](C(=O)N[C@H](C(=O)O1)[C@@H](C)O)[C@@H](C)CC)C)O)[C@@H](C)CC)C)C)OC)C)O,Organic compounds,Organic acids and derivatives,Peptidomimetics,Depsipeptides,Cyclic depsipeptides,Cyclic peptides,Oligopeptides,Amino acids and Peptides\n',
-                '2,0.4090,61.3670,928.0000,866.6330,GRJSOZDXIUZXEW,16,Halovir A,0,0.9621,0.4600,nan,nan,nan,nan,nan,nan,nan,nan,nan\n']
-    with open(os.path.join(os.path.join(results_directory, 'spectra_file_2.csv')), "r") as file:
-        assert file.readlines() == \
-               ['query_spectrum_nr,ms2query_model_prediction,precursor_mz_difference,precursor_mz_query_spectrum,precursor_mz_analog,inchikey,spectrum_ids,analog_compound_name,charge,s2v_score,ms2ds_score,smiles,cf_kingdom,cf_superclass,cf_class,cf_subclass,cf_direct_parent,npc_class_results,npc_superclass_results,npc_pathway_results\n',
-                '1,0.5645,33.2500,907.0000,940.2500,KNGPFNUOXXLKCN,1,Hoiamide B,1,0.9996,0.9232,CCC[C@@H](C)[C@@H]([C@H](C)[C@@H]1[C@H]([C@H](Cc2nc(cs2)C3=N[C@](CS3)(C4=N[C@](CS4)(C(=O)N[C@H]([C@H]([C@H](C(=O)O[C@H](C(=O)N[C@H](C(=O)O1)[C@@H](C)O)[C@@H](C)CC)C)O)[C@@H](C)CC)C)C)OC)C)O,Organic compounds,Organic acids and derivatives,Peptidomimetics,Depsipeptides,Cyclic depsipeptides,Cyclic peptides,Oligopeptides,Amino acids and Peptides\n',
-                '2,0.4090,61.3670,928.0000,866.6330,GRJSOZDXIUZXEW,16,Halovir A,0,0.9621,0.4600,nan,nan,nan,nan,nan,nan,nan,nan,nan\n']
+    expected_headers = \
+        ['query_spectrum_nr', "ms2query_model_prediction", "precursor_mz_difference", "precursor_mz_query_spectrum",
+         "precursor_mz_analog", "inchikey", "analog_compound_name", "smiles", "charge", "s2v_score",
+         "ms2ds_score", "cf_kingdom", "cf_superclass", "cf_class", "cf_subclass", "cf_direct_parent",
+         "npc_class_results", "npc_superclass_results", "npc_pathway_results"]
+    check_correct_results_csv_file(
+        pd.read_csv(os.path.join(os.path.join(results_directory, 'spectra_file_1.csv'))),
+        expected_headers)
+    check_correct_results_csv_file(
+        pd.read_csv(os.path.join(os.path.join(results_directory, 'spectra_file_2.csv'))),
+        expected_headers)
```

