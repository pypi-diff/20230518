# Comparing `tmp/evalda_pub2-0.0.5.tar.gz` & `tmp/evalda_pub2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalda_pub2-0.0.5.tar", max compression
+gzip compressed data, was "evalda_pub2-0.0.6.tar", max compression
```

## Comparing `evalda_pub2-0.0.5.tar` & `evalda_pub2-0.0.6.tar`

### file list

```diff
@@ -1,75 +1,68 @@
--rw-r--r--   0        0        0     1065 2023-03-23 10:21:49.117225 evalda_pub2-0.0.5/LICENSE
--rw-r--r--   0        0        0      549 2023-05-11 07:49:48.584000 evalda_pub2-0.0.5/README.md
--rw-r--r--   0        0        0       49 2023-05-11 19:56:05.410884 evalda_pub2-0.0.5/evalda_pub2/__init__.py
--rw-r--r--   0        0        0     6463 2023-04-19 16:13:42.482308 evalda_pub2-0.0.5/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-38.pyc
--rw-r--r--   0        0        0     7757 2023-05-11 11:06:07.920873 evalda_pub2-0.0.5/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-39.pyc
--rw-r--r--   0        0        0      483 2023-04-19 16:13:46.716225 evalda_pub2-0.0.5/evalda_pub2/base_tasks/__pycache__/load_model.cpython-38.pyc
--rw-r--r--   0        0        0      483 2023-05-11 11:06:12.255364 evalda_pub2-0.0.5/evalda_pub2/base_tasks/__pycache__/load_model.cpython-39.pyc
--rw-r--r--   0        0        0     3805 2023-04-19 16:13:50.367481 evalda_pub2-0.0.5/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-38.pyc
--rw-r--r--   0        0        0     5771 2023-05-11 11:06:15.805110 evalda_pub2-0.0.5/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-39.pyc
--rw-r--r--   0        0        0     9729 2023-05-03 17:07:47.956149 evalda_pub2-0.0.5/evalda_pub2/base_tasks/abc_lm_utilities.py
--rw-r--r--   0        0        0    41806 2023-05-03 17:07:47.956965 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/fillmask-danish-bert-boxto.png
--rw-r--r--   0        0        0    41198 2023-05-03 17:07:47.962956 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/fillmask-xlm-roberta-base.png
--rw-r--r--   0        0        0    39889 2023-05-03 17:07:47.964069 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert-base.png
--rw-r--r--   0        0        0      167 2023-05-03 17:07:47.964705 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert.csv
--rw-r--r--   0        0        0      167 2023-05-03 17:07:47.965139 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/fillmask_xlm.csv
--rw-r--r--   0        0        0   172315 2023-05-03 17:07:47.968269 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo.png
--rw-r--r--   0        0        0      351 2023-05-03 17:07:47.969075 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo_detailed.csv
--rw-r--r--   0        0        0      153 2023-05-03 17:07:47.969716 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo_simple.csv
--rw-r--r--   0        0        0      321 2023-05-03 17:07:47.970113 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_nb-bert-base_detailed.csv
--rw-r--r--   0        0        0      142 2023-05-03 17:07:47.970677 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_nb-bert-base_simple.csv
--rw-r--r--   0        0        0   162904 2023-05-03 17:07:47.973083 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base.png
--rw-r--r--   0        0        0      306 2023-05-03 17:07:47.974612 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base_detailed.csv
--rw-r--r--   0        0        0      138 2023-05-03 17:07:47.974908 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base_simple.csv
--rw-r--r--   0        0        0   136458 2023-05-03 17:07:47.976400 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large.png
--rw-r--r--   0        0        0      308 2023-05-03 17:07:47.976765 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large_detailed.csv
--rw-r--r--   0        0        0      138 2023-05-03 17:07:47.976940 evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large_simple.csv
--rw-r--r--   0        0        0      256 2023-04-13 13:14:23.045077 evalda_pub2-0.0.5/evalda_pub2/base_tasks/load_model.py
--rw-r--r--   0        0        0      208 2023-05-03 17:07:47.978516 evalda_pub2-0.0.5/evalda_pub2/base_tasks/requirements.txt
--rw-r--r--   0        0        0     6576 2023-05-11 08:11:25.536312 evalda_pub2-0.0.5/evalda_pub2/base_tasks/wino_fillmask_utilities.py
--rw-r--r--   0        0        0    47715 2023-05-03 17:07:47.981385 evalda_pub2-0.0.5/evalda_pub2/coref_tasks/coref_output/coref_abc.png
--rw-r--r--   0        0        0   155593 2023-05-03 17:07:47.983658 evalda_pub2-0.0.5/evalda_pub2/coref_tasks/coref_output/coref_winobias.png
--rw-r--r--   0        0        0      363 2023-05-03 17:07:47.984394 evalda_pub2-0.0.5/evalda_pub2/coref_tasks/coref_output/detailed_output_abc_coref.csv
--rw-r--r--   0        0        0      168 2023-05-03 17:07:47.984949 evalda_pub2-0.0.5/evalda_pub2/coref_tasks/coref_output/detailed_output_coref_wino_xlm.csv
--rw-r--r--   0        0        0    20070 2023-05-03 17:07:47.985819 evalda_pub2-0.0.5/evalda_pub2/coref_tasks/coref_utils.py
--rw-r--r--   0        0        0      178 2023-04-25 09:41:14.573026 evalda_pub2-0.0.5/evalda_pub2/coref_tasks/requirements.txt
--rw-r--r--   0        0        0      171 2023-04-13 13:14:23.052881 evalda_pub2-0.0.5/evalda_pub2/coref_tasks/setup.sh
--rw-r--r--   0        0        0    31060 2023-04-25 09:41:14.573856 evalda_pub2-0.0.5/evalda_pub2/coref_tasks/testing-coref.ipynb
--rw-r--r--   0        0        0    57119 2023-03-21 08:24:08.746101 evalda_pub2-0.0.5/evalda_pub2/data/DaWinoBias_anti_stereotyped_evalda.txt
--rw-r--r--   0        0        0    57118 2023-03-09 16:12:47.834912 evalda_pub2-0.0.5/evalda_pub2/data/DaWinoBias_pro_stereotyped_evalda.txt
--rw-r--r--   0        0        0   336571 2023-04-26 15:47:17.498742 evalda_pub2-0.0.5/evalda_pub2/data/abc_fem_sents.txt
--rw-r--r--   0        0        0   324943 2023-04-26 15:47:29.017834 evalda_pub2-0.0.5/evalda_pub2/data/abc_male_sents.txt
--rw-r--r--   0        0        0   706895 2023-05-03 17:07:48.000948 evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/first_names_2023_men.csv
--rw-r--r--   0        0        0   891168 2023-05-03 17:07:48.029137 evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/first_names_2023_women.csv
--rw-r--r--   0        0        0  4094899 2023-05-03 17:07:48.124266 evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/last_names_2023.csv
--rw-r--r--   0        0        0     1114 2023-05-03 17:07:48.132606 evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/overlapping_names.csv
--rw-r--r--   0        0        0    11901 2023-05-03 17:07:48.133913 evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/unisex_names.csv
--rw-r--r--   0        0        0    13252 2023-05-11 19:54:01.113957 evalda_pub2-0.0.5/evalda_pub2/evalda_pub2.py
--rw-r--r--   0        0        0      427 2023-03-21 15:07:17.952937 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/__pycache__/evaluate.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-02-16 13:19:59.521115 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/__init__.py
--rw-r--r--   0        0        0      198 2023-03-22 09:10:40.650810 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      434 2023-03-17 08:48:06.958238 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/__pycache__/apply_fn_scandi.cpython-39.pyc
--rw-r--r--   0        0        0      932 2023-03-22 14:48:24.602691 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/__pycache__/augmentation.cpython-39.pyc
--rw-r--r--   0        0        0      628 2023-03-23 13:05:20.448682 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/__pycache__/load_model.cpython-39.pyc
--rw-r--r--   0        0        0      726 2023-03-22 14:51:32.726951 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/__pycache__/overlap_fns.cpython-39.pyc
--rw-r--r--   0        0        0     2112 2023-03-23 07:54:42.282095 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/__pycache__/performance.cpython-39.pyc
--rw-r--r--   0        0        0     1557 2023-03-22 14:51:32.724071 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/__pycache__/process_names.cpython-39.pyc
--rw-r--r--   0        0        0     1097 2023-04-26 12:51:01.528045 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/augmentation.py
--rw-r--r--   0        0        0     1219 2023-05-03 17:07:48.135657 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/load_model.py
--rw-r--r--   0        0        0      409 2023-03-16 08:22:24.188834 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/overlap_fns.py
--rw-r--r--   0        0        0     3807 2023-05-03 17:07:48.136458 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/performance.py
--rw-r--r--   0        0        0     2695 2023-05-03 17:07:48.137155 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/process_names.py
--rw-r--r--   0        0        0      266 2023-05-03 17:07:48.137928 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/danish-bert_ner.csv
--rw-r--r--   0        0        0   155753 2023-05-03 17:07:48.139804 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20.png
--rw-r--r--   0        0        0      265 2023-05-03 17:07:48.140395 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20_detailed.csv
--rw-r--r--   0        0        0      116 2023-05-03 17:07:48.140749 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20_simple.csv
--rw-r--r--   0        0        0   172944 2023-05-03 17:07:48.143343 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20.png
--rw-r--r--   0        0        0      265 2023-05-03 17:07:48.143877 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20_detailed.csv
--rw-r--r--   0        0        0      115 2023-05-03 17:07:48.144202 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20_simple.csv
--rw-r--r--   0        0        0   137074 2023-05-03 17:07:48.146073 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20.png
--rw-r--r--   0        0        0      266 2023-05-03 17:07:48.146697 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20_detailed.csv
--rw-r--r--   0        0        0      116 2023-05-03 17:07:48.147077 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20_simple.csv
--rw-r--r--   0        0        0     1002 2023-05-03 17:07:48.147499 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/requirements-dacy-ner.txt
--rw-r--r--   0        0        0       82 2023-05-03 17:07:48.147901 evalda_pub2-0.0.5/evalda_pub2/ner_tasks/requirements-ner-minimum.txt
--rw-r--r--   0        0        0      640 2023-05-11 19:56:11.435750 evalda_pub2-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 evalda_pub2-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-23 10:21:49.117225 evalda_pub2-0.0.6/LICENSE
+-rw-r--r--   0        0        0      549 2023-05-11 07:49:48.584000 evalda_pub2-0.0.6/README.md
+-rw-r--r--   0        0        0       49 2023-05-18 12:03:04.412268 evalda_pub2-0.0.6/evalda_pub2/__init__.py
+-rw-r--r--   0        0        0     7660 2023-05-16 11:41:21.362905 evalda_pub2-0.0.6/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-38.pyc
+-rw-r--r--   0        0        0      483 2023-04-19 16:13:46.716225 evalda_pub2-0.0.6/evalda_pub2/base_tasks/__pycache__/load_model.cpython-38.pyc
+-rw-r--r--   0        0        0     5796 2023-05-16 11:41:27.679526 evalda_pub2-0.0.6/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-38.pyc
+-rw-r--r--   0        0        0    13345 2023-05-14 20:08:07.373372 evalda_pub2-0.0.6/evalda_pub2/base_tasks/reformat_abc.ipynb
+-rw-r--r--   0        0        0      643 2023-05-14 20:08:07.373240 evalda_pub2-0.0.6/evalda_pub2/base_tasks/test.py
+-rw-r--r--   0        0        0     8290 2023-05-18 12:02:26.894283 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/abc_utils.py
+-rw-r--r--   0        0        0    47715 2023-05-03 17:07:47.981385 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/coref_output/coref_abc.png
+-rw-r--r--   0        0        0   155593 2023-05-03 17:07:47.983658 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/coref_output/coref_winobias.png
+-rw-r--r--   0        0        0      363 2023-05-03 17:07:47.984394 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/coref_output/detailed_output_abc_coref.csv
+-rw-r--r--   0        0        0      168 2023-05-03 17:07:47.984949 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/coref_output/detailed_output_coref_wino_xlm.csv
+-rw-r--r--   0        0        0    20028 2023-05-18 12:02:26.896442 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/coref_utils_OLD(delete).py
+-rw-r--r--   0        0        0      178 2023-04-25 09:41:14.573026 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/requirements.txt
+-rw-r--r--   0        0        0      171 2023-04-13 13:14:23.052881 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/setup.sh
+-rw-r--r--   0        0        0    31060 2023-04-25 09:41:14.573856 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/testing-coref.ipynb
+-rw-r--r--   0        0        0    12485 2023-05-18 12:02:26.903295 evalda_pub2-0.0.6/evalda_pub2/coref_tasks/wino_utils.py
+-rw-r--r--   0        0        0    57119 2023-03-21 08:24:08.746101 evalda_pub2-0.0.6/evalda_pub2/data/DaWinoBias_anti_stereotyped_evalda.txt
+-rw-r--r--   0        0        0    57118 2023-03-09 16:12:47.834912 evalda_pub2-0.0.6/evalda_pub2/data/DaWinoBias_pro_stereotyped_evalda.txt
+-rw-r--r--   0        0        0   336571 2023-04-26 15:47:17.498742 evalda_pub2-0.0.6/evalda_pub2/data/abc_fem_sents.txt
+-rw-r--r--   0        0        0   324943 2023-04-26 15:47:29.017834 evalda_pub2-0.0.6/evalda_pub2/data/abc_male_sents.txt
+-rw-r--r--   0        0        0   706895 2023-05-03 17:07:48.000948 evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/first_names_2023_men.csv
+-rw-r--r--   0        0        0   891168 2023-05-03 17:07:48.029137 evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/first_names_2023_women.csv
+-rw-r--r--   0        0        0  4094899 2023-05-03 17:07:48.124266 evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/last_names_2023.csv
+-rw-r--r--   0        0        0     1114 2023-05-03 17:07:48.132606 evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/overlapping_names.csv
+-rw-r--r--   0        0        0    11901 2023-05-03 17:07:48.133913 evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/unisex_names.csv
+-rw-r--r--   0        0        0    16487 2023-05-18 12:02:26.907814 evalda_pub2-0.0.6/evalda_pub2/evalda_pub2.py
+-rw-r--r--   0        0        0    10331 2023-05-18 12:02:26.909245 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/abc_utils.py
+-rw-r--r--   0        0        0    41806 2023-05-18 12:02:26.912127 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/fillmask-danish-bert-boxto.png
+-rw-r--r--   0        0        0    41198 2023-05-18 12:02:26.914582 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/fillmask-xlm-roberta-base.png
+-rw-r--r--   0        0        0    39889 2023-05-18 12:02:26.918549 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/fillmask_nb-bert-base.png
+-rw-r--r--   0        0        0      167 2023-05-18 12:02:26.919779 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/fillmask_nb-bert.csv
+-rw-r--r--   0        0        0      167 2023-05-18 12:02:26.920472 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/fillmask_xlm.csv
+-rw-r--r--   0        0        0   172315 2023-05-18 12:02:26.939686 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_danish-bert-botxo.png
+-rw-r--r--   0        0        0      351 2023-05-18 12:02:26.940206 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_danish-bert-botxo_detailed.csv
+-rw-r--r--   0        0        0      153 2023-05-18 12:02:26.940588 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_danish-bert-botxo_simple.csv
+-rw-r--r--   0        0        0      321 2023-05-18 12:02:26.940964 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_nb-bert-base_detailed.csv
+-rw-r--r--   0        0        0      142 2023-05-18 12:02:26.941348 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_nb-bert-base_simple.csv
+-rw-r--r--   0        0        0   162904 2023-05-18 12:02:26.943705 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_xlm-base.png
+-rw-r--r--   0        0        0      306 2023-05-18 12:02:26.945415 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_xlm-base_detailed.csv
+-rw-r--r--   0        0        0      138 2023-05-18 12:02:26.945725 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_xlm-base_simple.csv
+-rw-r--r--   0        0        0   136458 2023-05-18 12:02:26.949126 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_xlm-large.png
+-rw-r--r--   0        0        0      308 2023-05-18 12:02:26.949737 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_xlm-large_detailed.csv
+-rw-r--r--   0        0        0      138 2023-05-18 12:02:26.950056 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_xlm-large_simple.csv
+-rw-r--r--   0        0        0      256 2023-05-18 12:02:26.951826 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/load_model.py
+-rw-r--r--   0        0        0      208 2023-05-18 12:02:26.952768 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/requirements.txt
+-rw-r--r--   0        0        0     6957 2023-05-18 12:02:26.953592 evalda_pub2-0.0.6/evalda_pub2/lm_tasks/wino_utils.py
+-rw-r--r--   0        0        0      427 2023-03-21 15:07:17.952937 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/__pycache__/evaluate.cpython-39.pyc
+-rw-r--r--   0        0        0     1550 2023-05-18 12:02:26.954488 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/augmentation.py
+-rw-r--r--   0        0        0      266 2023-05-18 12:02:20.192548 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/danish-bert_ner.csv
+-rw-r--r--   0        0        0   155753 2023-05-03 17:07:48.139804 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20.png
+-rw-r--r--   0        0        0      265 2023-05-03 17:07:48.140395 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20_detailed.csv
+-rw-r--r--   0        0        0      116 2023-05-03 17:07:48.140749 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20_simple.csv
+-rw-r--r--   0        0        0      266 2023-05-03 17:07:48.137928 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_danish-bert-botxo-n-20_detailed.csv
+-rw-r--r--   0        0        0   172944 2023-05-03 17:07:48.143343 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20.png
+-rw-r--r--   0        0        0      265 2023-05-03 17:07:48.143877 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20_detailed.csv
+-rw-r--r--   0        0        0      115 2023-05-03 17:07:48.144202 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20_simple.csv
+-rw-r--r--   0        0        0   137074 2023-05-03 17:07:48.146073 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20.png
+-rw-r--r--   0        0        0      266 2023-05-03 17:07:48.146697 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20_detailed.csv
+-rw-r--r--   0        0        0      116 2023-05-03 17:07:48.147077 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20_simple.csv
+-rw-r--r--   0        0        0     5755 2023-05-18 12:02:26.955388 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/performance.py
+-rw-r--r--   0        0        0     2687 2023-05-18 12:02:26.956243 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/process_names.py
+-rw-r--r--   0        0        0      252 2023-05-18 12:02:26.957034 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/requirements-dacy-ner-new.txt
+-rw-r--r--   0        0        0     1002 2023-05-03 17:07:48.147499 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/requirements-dacy-ner.txt
+-rw-r--r--   0        0        0      249 2023-05-18 12:02:26.959684 evalda_pub2-0.0.6/evalda_pub2/ner_tasks/requirements-ner-minimum.txt
+-rw-r--r--   0        0        0      637 2023-05-18 12:04:19.552891 evalda_pub2-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 evalda_pub2-0.0.6/PKG-INFO
```

### Comparing `evalda_pub2-0.0.5/LICENSE` & `evalda_pub2-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/README.md` & `evalda_pub2-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-38.pyc` & `evalda_pub2-0.0.6/evalda_pub2/base_tasks/__pycache__/abc_lm_utilities.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Apr 13 13:14:23 2023 UTC, .py size: 7812 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,404 +1,479 @@
-00000000: 550d 0d0a 0000 0000 2f00 3864 841e 0000  U......./.8d....
+00000000: 550d 0d0a 0000 0000 e394 5264 0126 0000  U.........Rd.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6402  d.l.Z.d.d.l.Z.d.
-00000060: 6403 8400 5a07 6404 6405 8400 5a08 6406  d...Z.d.d...Z.d.
-00000070: 6407 8400 5a09 6408 6409 8400 5a0a 640a  d...Z.d.d...Z.d.
-00000080: 640b 8400 5a0b 640c 640d 8400 5a0c 640e  d...Z.d.d...Z.d.
-00000090: 640f 8400 5a0d 6410 6411 8400 5a0e 6412  d...Z.d.d...Z.d.
-000000a0: 6413 8400 5a0f 6414 6415 8400 5a10 6416  d...Z.d.d...Z.d.
-000000b0: 6417 8400 5a11 6418 6419 8400 5a12 6401  d...Z.d.d...Z.d.
-000000c0: 5300 291a e900 0000 004e 6300 0000 0000  S.)......Nc.....
-000000d0: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
-000000e0: 0000 0073 5800 0000 6401 6402 6c00 6d01  ...sX...d.d.l.m.
-000000f0: 7d00 0100 7402 6a03 a004 7c00 7405 8301  }...t.j...|.t...
-00000100: 6a06 6403 1900 6404 6405 a103 7d01 7402  j.d...d.d...}.t.
-00000110: 6a03 a004 7c00 7405 8301 6a06 6403 1900  j...|.t...j.d...
-00000120: 6404 6406 a103 7d02 7407 7c01 8301 7d03  d.d...}.t.|...}.
-00000130: 7407 7c02 8301 7d04 7c03 7c04 6602 5300  t.|...}.|.|.f.S.
-00000140: 2907 4e72 0100 0000 2901 da04 5061 7468  ).Nr....)...Path
-00000150: e901 0000 00da 0464 6174 617a 1261 6263  .......dataz.abc
-00000160: 5f6d 616c 655f 7365 6e74 732e 7478 747a  _male_sents.txtz
-00000170: 1161 6263 5f66 656d 5f73 656e 7473 2e74  .abc_fem_sents.t
-00000180: 7874 2908 da07 7061 7468 6c69 6272 0200  xt)...pathlibr..
-00000190: 0000 da02 6f73 da04 7061 7468 da04 6a6f  ....os..path..jo
-000001a0: 696e da08 5f5f 6669 6c65 5f5f da07 7061  in..__file__..pa
-000001b0: 7265 6e74 73da 0a6c 6f61 645f 7365 6e74  rents..load_sent
-000001c0: 7329 0572 0200 0000 5a0b 696e 7061 7468  s).r....Z.inpath
-000001d0: 5f6d 616c 655a 0a69 6e70 6174 685f 6665  _maleZ.inpath_fe
-000001e0: 6d5a 0a6d 616c 655f 7365 6e74 735a 0966  mZ.male_sentsZ.f
-000001f0: 656d 5f73 656e 7473 a900 720c 0000 00fa  em_sents..r.....
-00000200: 772f 5573 6572 732f 6173 7472 6964 7279  w/Users/astridry
-00000210: 626e 6572 2f44 6f63 756d 656e 7473 2f63  bner/Documents/c
-00000220: 6f6f 6c2d 7072 6f67 7261 6d6d 6572 2d74  ool-programmer-t
-00000230: 6865 7369 732f 6576 616c 6461 2d70 7562  hesis/evalda-pub
-00000240: 322f 6576 616c 6461 2d70 7562 322f 6576  2/evalda-pub2/ev
-00000250: 616c 6461 5f70 7562 322f 6261 7365 5f74  alda_pub2/base_t
-00000260: 6173 6b73 2f61 6263 5f6c 6d5f 7574 696c  asks/abc_lm_util
-00000270: 6974 6965 732e 7079 da08 6c6f 6164 5f61  ities.py..load_a
-00000280: 6263 0700 0000 730c 0000 0000 010c 011a  bc....s.........
-00000290: 011a 0108 0108 0172 0e00 0000 6301 0000  .......r....c...
-000002a0: 0000 0000 0000 0000 0006 0000 0009 0000  ................
-000002b0: 0043 0000 0073 6600 0000 6700 7d01 7400  .C...sf...g.}.t.
-000002c0: 7c00 6401 8302 8f4e 7d02 7c02 a001 a100  |.d....N}.|.....
-000002d0: 7d03 6402 7d04 7c03 4400 5d36 7d05 6403  }.d.}.|.D.]6}.d.
-000002e0: 7c05 6b06 722e 7120 6404 7c05 6b06 723c  |.k.r.q d.|.k.r<
-000002f0: 6402 7d04 7120 7c04 6402 6b02 7220 7c01  d.}.q |.d.k.r |.
-00000300: a002 7c05 a003 a100 a101 0100 6405 7d04  ..|.........d.}.
-00000310: 7120 5700 3500 5100 5200 5800 7c01 5300  q W.5.Q.R.X.|.S.
-00000320: 2906 7a51 0a20 2020 2041 2066 756e 6374  ).zQ.    A funct
-00000330: 696f 6e20 7468 6174 206c 6f61 6473 2061  ion that loads a
-00000340: 6c6c 2074 6865 2072 6566 6c65 7869 7665  ll the reflexive
-00000350: 2073 656e 7465 6e63 6573 2066 726f 6d20   sentences from 
-00000360: 7468 6520 4142 4320 6461 7461 7365 742e  the ABC dataset.
-00000370: 0a20 2020 20da 0172 7201 0000 007a 0e2d  .    ..rr....z.-
-00000380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7a 032d  -------------z.-
-00000390: 2d2d 7203 0000 0029 04da 046f 7065 6eda  --r....)...open.
-000003a0: 0972 6561 646c 696e 6573 da06 6170 7065  .readlines..appe
-000003b0: 6e64 da05 7374 7269 7029 06da 0866 696c  nd..strip)...fil
-000003c0: 656e 616d 65da 0f72 6566 6c65 7869 7665  ename..reflexive
-000003d0: 5f73 656e 7473 da01 66da 056c 696e 6573  _sents..f..lines
-000003e0: da07 7265 7374 6172 74da 046c 696e 6572  ..restart..liner
-000003f0: 0c00 0000 720c 0000 0072 0d00 0000 720b  ....r....r....r.
-00000400: 0000 000f 0000 0073 1a00 0000 0004 0401  .......s........
-00000410: 0c01 0802 0401 0801 0800 0201 0801 0602  ................
-00000420: 0801 0e01 1001 720b 0000 0063 0400 0000  ......r....c....
-00000430: 0000 0000 0000 0000 0500 0000 0300 0000  ................
-00000440: 4300 0000 731a 0000 007c 027c 0017 007c  C...s....|.|...|
-00000450: 0317 007d 007c 01a0 007c 00a1 017d 047c  ...}.|...|...}.|
-00000460: 0453 0029 017a 3c0a 2020 2020 4120 6675  .S.).z<.    A fu
-00000470: 6e63 7469 6f6e 2074 6861 7420 746f 6b65  nction that toke
-00000480: 6e69 7a65 7320 7468 6520 7265 666c 6578  nizes the reflex
-00000490: 6976 6520 7365 6e74 656e 6365 732e 0a20  ive sentences.. 
-000004a0: 2020 2029 01da 0874 6f6b 656e 697a 6529     )...tokenize)
-000004b0: 05da 0873 656e 7465 6e63 65da 0974 6f6b  ...sentence..tok
-000004c0: 656e 697a 6572 da0b 7374 6172 745f 746f  enizer..start_to
-000004d0: 6b65 6eda 0973 6570 5f74 6f6b 656e da0e  ken..sep_token..
-000004e0: 746f 6b65 6e69 7a65 5f69 6e70 7574 720c  tokenize_inputr.
-000004f0: 0000 0072 0c00 0000 720d 0000 00da 1174  ...r....r......t
-00000500: 6f6b 656e 697a 655f 7365 6e74 656e 6365  okenize_sentence
-00000510: 2200 0000 7306 0000 0000 040c 010a 0172  "...s..........r
-00000520: 2000 0000 6302 0000 0000 0000 0000 0000   ...c...........
-00000530: 0006 0000 0003 0000 0043 0000 0073 4000  .........C...s@.
-00000540: 0000 6401 7d02 7400 7c00 8301 4400 5d1e  ..d.}.t.|...D.].
-00000550: 5c02 7d03 7d04 7c04 7c01 6b06 720c 7c03  \.}.}.|.|.k.r.|.
-00000560: 7d05 6402 7d02 0100 712c 710c 710c 7c02  }.d.}...q,q.q.|.
-00000570: 6401 6b02 7238 6403 5300 7c05 5300 6404  d.k.r8d.S.|.S.d.
-00000580: 5300 2905 7aaf 0a20 2020 2041 2066 756e  S.).z..    A fun
-00000590: 6374 696f 6e20 7468 6174 2074 616b 6573  ction that takes
-000005a0: 2074 6865 2074 6f6b 656e 697a 6564 2072   the tokenized r
-000005b0: 6566 6c65 7869 7665 2073 656e 7420 616e  eflexive sent an
-000005c0: 640a 2020 2020 6c6f 6361 7465 7320 696e  d.    locates in
-000005d0: 6465 7820 6f66 2070 726f 6e6f 756e 0a20  dex of pronoun. 
-000005e0: 2020 2072 6570 6c61 6365 7320 7072 6f6e     replaces pron
-000005f0: 6f75 6e20 7769 7468 206d 616c 652f 6665  oun with male/fe
-00000600: 6d61 6c65 2070 726f 6e6f 756e 200a 2020  male pronoun .  
-00000610: 2020 7265 7475 726e 7320 3220 6175 676d    returns 2 augm
-00000620: 656e 7465 6420 7365 6e74 656e 6365 7320  ented sentences 
-00000630: 0a20 2020 2054 467a 166e 6f20 7072 6f6e  .    TFz.no pron
-00000640: 6f75 6e73 2074 6f20 7265 706c 6163 654e  ouns to replaceN
-00000650: 2901 da09 656e 756d 6572 6174 6529 06da  )...enumerate)..
-00000660: 0473 656e 745a 0c70 726f 6e6f 756e 5f6c  .sentZ.pronoun_l
-00000670: 6973 745a 076e 6f5f 7072 6f6e da01 69da  istZ.no_pron..i.
-00000680: 0574 6f6b 656e 5a0a 7072 6f6e 5f69 6e64  .tokenZ.pron_ind
-00000690: 6578 720c 0000 0072 0c00 0000 720d 0000  exr....r....r...
-000006a0: 00da 0e67 6574 5f70 726f 6e5f 696e 6465  ...get_pron_inde
-000006b0: 782a 0000 0073 1400 0000 0008 0401 1001  x*...s..........
-000006c0: 0801 0401 0401 0601 0201 0800 0401 7225  ..............r%
-000006d0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000006e0: 0400 0000 0400 0000 4300 0000 7330 0000  ........C...s0..
-000006f0: 007c 00a0 00a1 007d 027c 00a0 00a1 007d  .|.....}.|.....}
-00000700: 0364 017c 0274 017c 0183 013c 0064 027c  .d.|.t.|...<.d.|
-00000710: 0374 017c 0183 013c 007c 027c 0366 0253  .t.|...<.|.|.f.S
-00000720: 0029 037a 600a 2020 2020 5461 6b65 206f  .).z`.    Take o
-00000730: 7269 6769 6e61 6c20 7365 6e74 656e 6365  riginal sentence
-00000740: 2061 6e64 2072 6570 6c61 6365 2070 726f   and replace pro
-00000750: 6e6f 756e 2077 6974 6820 616e 7469 7272  noun with antirr
-00000760: 6566 6c65 7869 7665 2070 726f 6e6f 756e  eflexive pronoun
-00000770: 7320 2868 616e 732f 6865 6e64 6573 2920  s (hans/hendes) 
-00000780: 0a20 2020 205a 0468 616e 735a 0668 656e  .    Z.hansZ.hen
-00000790: 6465 7329 02da 0463 6f70 79da 0369 6e74  des)...copy..int
-000007a0: 2904 721f 0000 00da 0369 6478 5a12 746f  ).r......idxZ.to
-000007b0: 6b65 6e69 7a65 5f6d 6173 6b5f 6d61 6c65  kenize_mask_male
-000007c0: 5a14 746f 6b65 6e69 7a65 5f6d 6173 6b5f  Z.tokenize_mask_
-000007d0: 6665 6d61 6c65 720c 0000 0072 0c00 0000  femaler....r....
-000007e0: 720d 0000 00da 1367 6574 5f61 7567 6d65  r......get_augme
-000007f0: 6e74 6564 5f73 656e 7473 3c00 0000 730a  nted_sents<...s.
-00000800: 0000 0000 0408 0108 010c 010c 0172 2900  .............r).
-00000810: 0000 6304 0000 0000 0000 0000 0000 0007  ..c.............
-00000820: 0000 0005 0000 0043 0000 0073 4000 0000  .......C...s@...
-00000830: 7400 a001 7c03 a002 7c00 a101 6701 a101  t...|...|...g...
-00000840: 7d04 7400 a001 7c03 a002 7c01 a101 6701  }.t...|...|...g.
-00000850: a101 7d05 7400 a001 7c03 a002 7c02 a101  ..}.t...|...|...
-00000860: 6701 a101 7d06 7c04 7c05 7c06 6603 5300  g...}.|.|.|.f.S.
-00000870: 2901 7a30 0a20 2020 204d 616b 6520 6175  ).z0.    Make au
-00000880: 676d 656e 7465 6420 7365 6e74 656e 6365  gmented sentence
-00000890: 7320 696e 746f 2074 656e 736f 7273 2e0a  s into tensors..
-000008a0: 2020 2020 2903 da05 746f 7263 68da 0674      )...torch..t
-000008b0: 656e 736f 725a 1563 6f6e 7665 7274 5f74  ensorZ.convert_t
-000008c0: 6f6b 656e 735f 746f 5f69 6473 2907 da05  okens_to_ids)...
-000008d0: 7472 7574 685a 046d 616c 655a 0366 656d  truthZ.maleZ.fem
-000008e0: 721c 0000 00da 0c74 656e 736f 725f 7472  r......tensor_tr
-000008f0: 7574 68da 0b74 656e 736f 725f 6d61 6c65  uth..tensor_male
-00000900: da0a 7465 6e73 6f72 5f66 656d 720c 0000  ..tensor_femr...
-00000910: 0072 0c00 0000 720d 0000 00da 0e63 7265  .r....r......cre
-00000920: 6174 655f 7465 6e73 6f72 7346 0000 0073  ate_tensorsF...s
-00000930: 0800 0000 0004 1201 1201 1201 7230 0000  ............r0..
-00000940: 0063 0400 0000 0000 0000 0000 0000 0700  .c..............
-00000950: 0000 0900 0000 4300 0000 736a 0000 0074  ......C...sj...t
-00000960: 00a0 01a1 008f 1201 007c 037c 0083 0164  .........|.|...d
-00000970: 0119 007d 0457 0035 0051 0052 0058 0074  ...}.W.5.Q.R.X.t
-00000980: 00a0 01a1 008f 1201 007c 037c 0183 0164  .........|.|...d
-00000990: 0119 007d 0557 0035 0051 0052 0058 0074  ...}.W.5.Q.R.X.t
-000009a0: 00a0 01a1 008f 1201 007c 037c 0283 0164  .........|.|...d
-000009b0: 0119 007d 0657 0035 0051 0052 0058 007c  ...}.W.5.Q.R.X.|
-000009c0: 047c 057c 0666 0353 0029 027a 7c0a 2020  .|.|.f.S.).z|.  
-000009d0: 2020 4120 6675 6e63 7469 6f6e 2074 6861    A function tha
-000009e0: 7420 7461 6b65 7320 7468 6520 3320 7365  t takes the 3 se
-000009f0: 6e74 656e 6365 7320 616e 6420 7265 7475  ntences and retu
-00000a00: 726e 7320 6d6f 6465 6c20 7072 6564 6963  rns model predic
-00000a10: 7469 6f6e 7320 666f 7220 6561 6368 206f  tions for each o
-00000a20: 6620 7468 656d 2e0a 2020 2020 5573 6564  f them..    Used
-00000a30: 2074 6f20 636f 6d70 7574 6520 6c6f 7373   to compute loss
-00000a40: 2e20 2020 0a20 2020 2072 0100 0000 2902  .   .    r....).
-00000a50: 722a 0000 005a 076e 6f5f 6772 6164 2907  r*...Z.no_grad).
-00000a60: 722d 0000 0072 2e00 0000 722f 0000 00da  r-...r....r/....
-00000a70: 056d 6f64 656c da0a 7072 6564 5f74 7275  .model..pred_tru
-00000a80: 7468 da09 7072 6564 5f6d 616c 65da 0870  th..pred_male..p
-00000a90: 7265 645f 6665 6d72 0c00 0000 720c 0000  red_femr....r...
-00000aa0: 0072 0d00 0000 da0f 6765 745f 7072 6564  .r......get_pred
-00000ab0: 6963 7469 6f6e 734f 0000 0073 0e00 0000  ictionsO...s....
-00000ac0: 0005 0a01 1601 0a01 1601 0a01 1601 7235  ..............r5
-00000ad0: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
-00000ae0: 0900 0000 0400 0000 4300 0000 734a 0000  ........C...sJ..
-00000af0: 007c 007c 02a0 00a1 007c 04a0 00a1 0083  .|.|.....|......
-00000b00: 026a 017d 057c 007c 03a0 00a1 007c 04a0  .j.}.|.|.....|..
-00000b10: 00a1 0083 026a 017d 067c 007c 01a0 00a1  .....j.}.|.|....
-00000b20: 007c 04a0 00a1 0083 026a 017d 077c 057c  .|.......j.}.|.|
-00000b30: 067c 0767 037d 087c 0853 0029 017a b40a  .|.g.}.|.S.).z..
-00000b40: 2020 2020 5461 6b65 206d 6f64 656c 2070      Take model p
-00000b50: 7265 6469 6374 696f 6e73 2061 6e64 2063  redictions and c
-00000b60: 6f6d 7075 7465 206c 6f73 7320 666f 7220  ompute loss for 
-00000b70: 616c 6c20 3320 7365 6e74 656e 6365 7320  all 3 sentences 
-00000b80: 0a20 2020 2062 7920 636f 6d70 6172 696e  .    by comparin
-00000b90: 6720 746f 2070 7265 645f 7472 7574 682c  g to pred_truth,
-00000ba0: 2077 6869 6368 2069 7320 7468 6520 7072   which is the pr
-00000bb0: 6564 6963 7469 6f6e 206f 6620 7468 6520  ediction of the 
-00000bc0: 7365 6e74 656e 6365 2077 6974 6820 7468  sentence with th
-00000bd0: 6520 636f 7272 6563 7420 2872 6566 6c65  e correct (refle
-00000be0: 7869 7665 2920 7072 6f6e 6f75 6e2e 0a20  xive) pronoun.. 
-00000bf0: 2020 2029 02da 0773 7175 6565 7a65 7204     )...squeezer.
-00000c00: 0000 0029 09da 086c 6f73 735f 6663 7472  ...)...loss_fctr
-00000c10: 3200 0000 7233 0000 0072 3400 0000 722d  2...r3...r4...r-
-00000c20: 0000 005a 096c 6f73 735f 6d61 6c65 5a08  ...Z.loss_maleZ.
-00000c30: 6c6f 7373 5f66 656d 5a08 6c6f 7373 5f72  loss_femZ.loss_r
-00000c40: 6566 5a09 6c6f 7373 5f6c 6973 7472 0c00  efZ.loss_listr..
-00000c50: 0000 720c 0000 0072 0d00 0000 da0c 636f  ..r....r......co
-00000c60: 6d70 7574 655f 6c6f 7373 5c00 0000 730a  mpute_loss\...s.
-00000c70: 0000 0000 0514 0114 0114 010a 0172 3800  .............r8.
-00000c80: 0000 6307 0000 0000 0000 0000 0000 0012  ..c.............
-00000c90: 0000 0007 0000 0043 0000 0073 9200 0000  .......C...s....
-00000ca0: 7400 7c00 7c02 7c05 7c06 8304 7d07 7401  t.|.|.|.|...}.t.
-00000cb0: 7c07 7c04 8302 7d08 7402 7c07 7c08 8302  |.|...}.t.|.|...
-00000cc0: 5c02 7d09 7d0a 7403 7c07 7c09 7c0a 7c02  \.}.}.t.|.|.|.|.
-00000cd0: 8304 5c03 7d0b 7d0c 7d0d 7404 7c0b 7c0c  ..\.}.}.}.t.|.|.
-00000ce0: 7c0d 7c03 8304 5c03 7d0e 7d0f 7d10 7405  |.|...\.}.}.}.t.
-00000cf0: 7c01 7c0e 7c0f 7c10 7c0b 8305 7d11 7406  |.|.|.|.|...}.t.
-00000d00: 7407 a008 7c11 6401 1900 a101 8301 7406  t...|.d.......t.
-00000d10: 7407 a008 7c11 6402 1900 a101 8301 7406  t...|.d.......t.
-00000d20: 7407 a008 7c11 6403 1900 a101 8301 6603  t...|.d.......f.
-00000d30: 5300 2904 6124 0200 000a 2020 2020 5461  S.).a$....    Ta
-00000d40: 6b20 6120 7365 6e74 656e 6365 2077 6974  k a sentence wit
-00000d50: 6820 6120 7265 6c66 6c65 7869 7665 2070  h a relflexive p
-00000d60: 726f 6e6f 756e 2c20 0a20 2020 2072 6570  ronoun, .    rep
-00000d70: 6c61 6365 2070 726f 6e6f 756e 2077 6974  lace pronoun wit
-00000d80: 6820 616e 7469 7265 666c 6578 6976 6573  h antireflexives
-00000d90: 2028 6d61 6c65 2f66 656d 616c 6520 7072   (male/female pr
-00000da0: 6f6e 6f75 6e29 0a20 2020 2061 6e64 2063  onoun).    and c
-00000db0: 6f6d 7075 7465 206c 6f73 7320 616e 6420  ompute loss and 
-00000dc0: 7065 7270 6c65 7869 7479 2066 6f72 2061  perplexity for a
-00000dd0: 6c6c 2033 2073 656e 7465 6e63 6573 2e0a  ll 3 sentences..
-00000de0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00000df0: 2020 7365 6e74 2028 7374 7229 3a20 4120    sent (str): A 
-00000e00: 7365 6e74 656e 6365 2077 6974 6820 7265  sentence with re
-00000e10: 666c 6578 6976 6520 7072 6f6e 6f75 6e73  flexive pronouns
-00000e20: 2e0a 2020 2020 2020 2020 6c6f 7373 5f66  ..        loss_f
-00000e30: 6374 2028 746f 7263 682e 6e6e 2e43 726f  ct (torch.nn.Cro
-00000e40: 7373 456e 7472 6f70 794c 6f73 7329 3a20  ssEntropyLoss): 
-00000e50: 4120 6c6f 7373 2066 756e 6374 696f 6e2e  A loss function.
-00000e60: 0a20 2020 2020 2020 2074 6f6b 656e 697a  .        tokeniz
-00000e70: 6572 2028 4265 7274 546f 6b65 6e69 7a65  er (BertTokenize
-00000e80: 7229 3a20 4120 746f 6b65 6e69 7a65 722e  r): A tokenizer.
-00000e90: 0a20 2020 2020 2020 206d 6f64 656c 2028  .        model (
-00000ea0: 4265 7274 466f 724d 6173 6b65 644c 4d29  BertForMaskedLM)
-00000eb0: 3a20 4120 6c61 6e67 7561 6765 206d 6f64  : A language mod
-00000ec0: 656c 2e0a 2020 2020 2020 2020 7072 6f6e  el..        pron
-00000ed0: 5f6c 6973 7420 286c 6973 7429 3a20 4120  _list (list): A 
-00000ee0: 6c69 7374 206f 6620 7072 6f6e 6f75 6e73  list of pronouns
-00000ef0: 2e0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-00000f00: 2020 2020 2020 204c 6f73 7320 616e 6420         Loss and 
-00000f10: 7065 7270 6c65 7869 7479 2076 616c 7565  perplexity value
-00000f20: 7320 666f 7220 7365 6e74 656e 6365 2077  s for sentence w
-00000f30: 6974 6820 7265 666c 6578 6976 652c 206d  ith reflexive, m
-00000f40: 616c 6520 616e 6420 6665 6d61 6c65 2070  ale and female p
-00000f50: 726f 6e6f 756e 2e20 0a20 2020 2072 0100  ronoun. .    r..
-00000f60: 0000 7203 0000 00e9 0200 0000 2909 7220  ..r.........).r 
-00000f70: 0000 0072 2500 0000 7229 0000 0072 3000  ...r%...r)...r0.
-00000f80: 0000 7235 0000 0072 3800 0000 da03 7374  ..r5...r8.....st
-00000f90: 72da 046d 6174 68da 0365 7870 2912 7222  r..math..exp).r"
-00000fa0: 0000 0072 3700 0000 721c 0000 0072 3100  ...r7...r....r1.
-00000fb0: 0000 5a09 7072 6f6e 5f6c 6973 7472 1d00  ..Z.pron_listr..
-00000fc0: 0000 721e 0000 005a 0e74 6f6b 656e 697a  ..r....Z.tokeniz
-00000fd0: 6564 5f72 6566 6cda 0569 6e64 6578 5a0e  ed_refl..indexZ.
-00000fe0: 746f 6b65 6e69 7a65 645f 6d61 6c65 5a0d  tokenized_maleZ.
-00000ff0: 746f 6b65 6e69 7a65 645f 6665 6d72 2d00  tokenized_femr-.
-00001000: 0000 722e 0000 0072 2f00 0000 7232 0000  ..r....r/...r2..
-00001010: 0072 3300 0000 7234 0000 005a 0b6c 6f73  .r3...r4...Z.los
-00001020: 735f 7661 6c75 6573 720c 0000 0072 0c00  s_valuesr....r..
-00001030: 0000 720d 0000 00da 0a73 636f 7265 5f73  ..r......score_s
-00001040: 656e 7467 0000 0073 0e00 0000 000e 0e01  entg...s........
-00001050: 0a01 0e01 1401 1401 1001 723e 0000 0063  ..........r>...c
-00001060: 0500 0000 0000 0000 0000 0000 1000 0000  ................
-00001070: 0900 0000 4300 0000 73f4 0000 0074 006a  ....C...s....t.j
-00001080: 01a0 02a1 007d 0564 0164 0264 0364 0464  .....}.d.d.d.d.d
-00001090: 0564 0667 067d 0674 036a 0474 057c 0083  .d.g.}.t.j.t.|..
-000010a0: 0164 078d 01a0 06a1 007d 0767 0067 0067  .d.......}.g.g.g
-000010b0: 0067 0066 045c 047d 087d 097d 0a7d 0b74  .g.f.\.}.}.}.}.t
-000010c0: 077c 0083 0144 005d 5a5c 027d 0c7d 0d74  .|...D.]Z\.}.}.t
-000010d0: 087c 0d7c 057c 017c 027c 067c 037c 0483  .|.|.|.|.|.|.|..
-000010e0: 077d 0e7c 07a0 097c 0ca1 0101 007c 08a0  .}.|...|.....|..
-000010f0: 0a7c 0da1 0101 007c 09a0 0a7c 0e64 0819  .|.....|...|.d..
-00001100: 00a1 0101 007c 0aa0 0a7c 0e64 0919 00a1  .....|...|.d....
-00001110: 0101 007c 0ba0 0a7c 0e64 0a19 00a1 0101  ...|...|.d......
-00001120: 0071 4a74 0ba0 0c7c 087c 097c 0a7c 0b64  .qJt...|.|.|.|.d
-00001130: 0b9c 04a1 017d 0f7c 0f64 0c19 00a0 0d74  .....}.|.d.....t
-00001140: 0ea1 017c 0f64 0c3c 007c 0f64 0d19 00a0  ...|.d.<.|.d....
-00001150: 0d74 0ea1 017c 0f64 0d3c 007c 0f64 0e19  .t...|.d.<.|.d..
-00001160: 00a0 0d74 0ea1 017c 0f64 0e3c 007c 0f53  ...t...|.d.<.|.S
-00001170: 0029 0f61 8b01 0000 0a20 2020 2052 756e  .).a.....    Run
-00001180: 2074 6865 2041 4243 2064 6174 6173 6574   the ABC dataset
-00001190: 2061 6e64 2077 7269 7465 2072 6573 756c   and write resul
-000011a0: 7473 2074 6f20 6669 6c65 2e0a 2020 2020  ts to file..    
-000011b0: 4172 6773 3a0a 2020 2020 2020 2020 6f75  Args:.        ou
-000011c0: 7470 6174 6820 2873 7472 293a 2050 6174  tpath (str): Pat
-000011d0: 6820 746f 206f 7574 7075 7420 6669 6c65  h to output file
-000011e0: 2e0a 2020 2020 2020 2020 7265 666c 6578  ..        reflex
-000011f0: 6976 655f 7365 6e74 7320 286c 6973 7429  ive_sents (list)
-00001200: 3a20 4120 6c69 7374 206f 6620 7365 6e74  : A list of sent
-00001210: 656e 6365 7320 7769 7468 2072 6566 6c65  ences with refle
-00001220: 7869 7665 2070 726f 6e6f 756e 732e 0a20  xive pronouns.. 
-00001230: 2020 2020 2020 206c 6f73 735f 6663 7420         loss_fct 
-00001240: 2874 6f72 6368 2e6e 6e2e 4372 6f73 7345  (torch.nn.CrossE
-00001250: 6e74 726f 7079 4c6f 7373 293a 2041 206c  ntropyLoss): A l
-00001260: 6f73 7320 6675 6e63 7469 6f6e 2e0a 2020  oss function..  
-00001270: 2020 2020 2020 746f 6b65 6e69 7a65 7220        tokenizer 
-00001280: 2842 6572 7454 6f6b 656e 697a 6572 293a  (BertTokenizer):
-00001290: 2041 2074 6f6b 656e 697a 6572 2e0a 2020   A tokenizer..  
-000012a0: 2020 2020 2020 6d6f 6465 6c20 2842 6572        model (Ber
-000012b0: 7446 6f72 4d61 736b 6564 4c4d 293a 2041  tForMaskedLM): A
-000012c0: 206c 616e 6775 6167 6520 6d6f 6465 6c2e   language model.
-000012d0: 0a20 2020 2020 2020 2070 726f 6e5f 6c69  .        pron_li
-000012e0: 7374 2028 6c69 7374 293a 2041 206c 6973  st (list): A lis
-000012f0: 7420 6f66 2070 726f 6e6f 756e 732e 0a20  t of pronouns.. 
-00001300: 2020 20da 0373 696e 5a03 7369 745a 0473     ..sinZ.sitZ.s
-00001310: 696e 6575 0600 0000 e296 8173 696e 7506  ineu.......sinu.
-00001320: 0000 00e2 9681 7369 7475 0700 0000 e296  ......situ......
-00001330: 8173 696e 6529 015a 066d 6178 7661 6c72  .sine).Z.maxvalr
-00001340: 0100 0000 7203 0000 0072 3900 0000 2904  ....r....r9...).
-00001350: 7222 0000 00da 0f70 6572 706c 6578 6974  r".....perplexit
-00001360: 795f 6d61 6c65 da11 7065 7270 6c65 7869  y_male..perplexi
-00001370: 7479 5f66 656d 616c 65da 1470 6572 706c  ty_female..perpl
-00001380: 6578 6974 795f 7265 666c 6578 6976 6572  exity_reflexiver
-00001390: 4000 0000 7241 0000 0072 4200 0000 290f  @...rA...rB...).
-000013a0: 722a 0000 00da 026e 6e5a 1043 726f 7373  r*.....nnZ.Cross
-000013b0: 456e 7472 6f70 794c 6f73 73da 0b70 726f  EntropyLoss..pro
-000013c0: 6772 6573 7362 6172 da0b 5072 6f67 7265  gressbar..Progre
-000013d0: 7373 4261 72da 036c 656e da05 7374 6172  ssBar..len..star
-000013e0: 7472 2100 0000 723e 0000 00da 0675 7064  tr!...r>.....upd
-000013f0: 6174 6572 1200 0000 da02 7064 da09 4461  ater......pd..Da
-00001400: 7461 4672 616d 65da 0661 7374 7970 65da  taFrame..astype.
-00001410: 0566 6c6f 6174 2910 7215 0000 0072 1c00  .float).r....r..
-00001420: 0000 7231 0000 0072 1d00 0000 721e 0000  ..r1...r....r...
-00001430: 0072 3700 0000 5a0d 7072 6f6e 6f75 6e73  .r7...Z.pronouns
-00001440: 5f6c 6973 74da 0362 6172 5a05 7365 6e74  _list..barZ.sent
-00001450: 735a 0670 6572 705f 6d5a 0670 6572 705f  sZ.perp_mZ.perp_
-00001460: 665a 0670 6572 705f 7272 2800 0000 7222  fZ.perp_rr(...r"
-00001470: 0000 005a 0673 636f 7265 73da 0264 6672  ...Z.scores..dfr
-00001480: 0c00 0000 720c 0000 0072 0d00 0000 da07  ....r....r......
-00001490: 7275 6e5f 6162 637d 0000 0073 2800 0000  run_abc}...s(...
-000014a0: 000d 0a02 1003 1402 1402 1001 1401 0a01  ................
-000014b0: 0a01 0e01 0e01 1003 0601 0201 0201 02fd  ................
-000014c0: 0805 1201 1201 1202 724f 0000 0063 0100  ........rO...c..
-000014d0: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-000014e0: 0000 4300 0000 7346 0000 007c 006a 00a0  ..C...sF...|.j..
-000014f0: 01a1 007c 006a 02a0 01a1 007c 006a 03a0  ...|.j.....|.j..
-00001500: 01a1 0003 0002 007d 017d 027d 0374 047c  .......}.}.}.t.|
-00001510: 017c 031b 0064 0183 027d 0474 047c 027c  .|...d...}.t.|.|
-00001520: 031b 0064 0183 027d 057c 057c 0466 0253  ...d...}.|.|.f.S
-00001530: 0029 024e 7239 0000 0029 0572 4000 0000  .).Nr9...).r@...
-00001540: da04 6d65 616e 7241 0000 0072 4200 0000  ..meanrA...rB...
-00001550: da05 726f 756e 6429 0672 4e00 0000 5a0c  ..round).rN...Z.
-00001560: 6466 5f6d 616c 655f 6d65 616e 5a0b 6466  df_male_meanZ.df
-00001570: 5f66 656d 5f6d 6561 6e5a 0b64 665f 7265  _fem_meanZ.df_re
-00001580: 665f 6d65 616e 5a0d 7265 6c61 7469 7665  f_meanZ.relative
-00001590: 5f6d 616c 655a 0c72 656c 6174 6976 655f  _maleZ.relative_
-000015a0: 6665 6d72 0c00 0000 720c 0000 0072 0d00  femr....r....r..
-000015b0: 0000 da08 6576 616c 5f61 6263 a700 0000  ....eval_abc....
-000015c0: 7308 0000 0000 0222 030e 010e 0272 5200  s......".....rR.
-000015d0: 0000 6304 0000 0000 0000 0000 0000 0007  ..c.............
-000015e0: 0000 000a 0000 0043 0000 0073 5a00 0000  .......C...sZ...
-000015f0: 7400 6a01 a002 6401 6402 6403 6404 6704  t.j...d.d.d.d.g.
-00001600: a101 7d04 7403 6405 7c00 9b00 6406 7c01  ..}.t.d.|...d.|.
-00001610: 9b00 6407 7c02 9b00 6408 7c03 9b00 6409  ..d.|...d.|...d.
-00001620: 9d09 8301 0100 7c00 7c01 7c02 7c03 6704  ......|.|.|.|.g.
-00001630: 6701 7d05 7400 6a04 7c05 7c04 640a 6701  g.}.t.j.|.|.d.g.
-00001640: 640b 8d03 7d06 7c06 5300 290c 4e29 02fa  d...}.|.S.).N)..
-00001650: 1946 656d 616c 6520 5374 6572 656f 7479  .Female Stereoty
-00001660: 7069 6361 6c20 4a6f 6273 5a06 4665 6d61  pical JobsZ.Fema
-00001670: 6c65 2902 7253 0000 00da 044d 616c 6529  le).rS.....Male)
-00001680: 02fa 174d 616c 6520 5374 6572 656f 7479  ...Male Stereoty
-00001690: 7069 6361 6c20 4a6f 6273 5a05 4665 616c  pical JobsZ.Feal
-000016a0: 6529 0272 5500 0000 7254 0000 007a 5873  e).rU...rT...zXs
-000016b0: 756d 6d61 7279 2074 6f20 6368 6563 6b20  ummary to check 
-000016c0: 6966 2074 6865 2072 6967 6874 206e 756d  if the right num
-000016d0: 6265 7273 2061 7265 2069 6e20 7269 6768  bers are in righ
-000016e0: 7420 636f 6c75 6d6e 730a 2020 2020 6665  t columns.    fe
-000016f0: 6d5f 7374 6572 656f 5f72 656c 6174 6976  m_stereo_relativ
-00001700: 655f 6665 6d2c 207a 1f0a 2020 2020 6665  e_fem, z..    fe
-00001710: 6d5f 7374 6572 656f 5f72 656c 6174 6976  m_stereo_relativ
-00001720: 655f 6d61 6c65 2c20 7a1f 0a20 2020 206d  e_male, z..    m
-00001730: 616c 655f 7374 6572 656f 5f72 656c 6174  ale_stereo_relat
-00001740: 6976 655f 6665 6d2c 207a 200a 2020 2020  ive_fem, z .    
-00001750: 6d61 6c65 5f73 7465 7265 6f5f 7265 6c61  male_stereo_rela
-00001760: 7469 7665 5f6d 616c 652c 207a 050a 2020  tive_male, z..  
-00001770: 2020 7a13 5265 6c61 7469 7665 2050 6572    z.Relative Per
-00001780: 706c 6578 6974 7929 02da 0763 6f6c 756d  plexity)...colum
-00001790: 6e73 723d 0000 0029 0572 4900 0000 da0a  nsr=...).rI.....
-000017a0: 4d75 6c74 6949 6e64 6578 da0b 6672 6f6d  MultiIndex..from
-000017b0: 5f74 7570 6c65 73da 0570 7269 6e74 724a  _tuples..printrJ
-000017c0: 0000 0029 07da 1766 656d 5f73 7465 7265  ...)...fem_stere
-000017d0: 6f5f 7265 6c61 7469 7665 5f66 656d da18  o_relative_fem..
-000017e0: 6665 6d5f 7374 6572 656f 5f72 656c 6174  fem_stereo_relat
-000017f0: 6976 655f 6d61 6c65 da18 6d61 6c65 5f73  ive_male..male_s
-00001800: 7465 7265 6f5f 7265 6c61 7469 7665 5f66  tereo_relative_f
-00001810: 656d da19 6d61 6c65 5f73 7465 7265 6f5f  em..male_stereo_
-00001820: 7265 6c61 7469 7665 5f6d 616c 65da 0463  relative_male..c
-00001830: 6f6c 7372 0400 0000 da07 7265 7375 6c74  olsr......result
-00001840: 7372 0c00 0000 720c 0000 0072 0d00 0000  sr....r....r....
-00001850: da12 6162 635f 7265 7375 6c74 735f 7265  ..abc_results_re
-00001860: 706f 7274 b100 0000 7322 0000 0000 0108  port....s"......
-00001870: 0102 0102 0102 fd06 0504 0102 ff04 0202  ................
-00001880: fe04 0302 fd04 0402 fc0a 080e 0212 0272  ...............r
-00001890: 6000 0000 2913 da03 7379 7372 0600 0000  `...)...sysr....
-000018a0: da06 7061 6e64 6173 7249 0000 0072 2a00  ..pandasrI...r*.
-000018b0: 0000 723b 0000 0072 4400 0000 720e 0000  ..r;...rD...r...
-000018c0: 0072 0b00 0000 7220 0000 0072 2500 0000  .r....r ...r%...
-000018d0: 7229 0000 0072 3000 0000 7235 0000 0072  r)...r0...r5...r
-000018e0: 3800 0000 723e 0000 0072 4f00 0000 7252  8...r>...rO...rR
-000018f0: 0000 0072 6000 0000 720c 0000 0072 0c00  ...r`...r....r..
-00001900: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
-00001910: 6f64 756c 653e 0100 0000 7320 0000 0010  odule>....s ....
-00001920: 0108 0108 0108 0108 0208 0808 1308 0808  ................
-00001930: 1208 0a08 0908 0d08 0b08 1608 2a08 0a    ............*..
+00000040: 6401 6c02 5a03 6400 6401 6c04 5a05 6400  d.l.Z.d.d.l.Z.d.
+00000050: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6401 6c08 5a08 6402 6403 8400 5a09 6404  d.l.Z.d.d...Z.d.
+00000070: 6405 8400 5a0a 6406 6407 8400 5a0b 6408  d...Z.d.d...Z.d.
+00000080: 6409 8400 5a0c 640a 640b 8400 5a0d 640c  d...Z.d.d...Z.d.
+00000090: 640d 8400 5a0e 640e 640f 8400 5a0f 6410  d...Z.d.d...Z.d.
+000000a0: 6411 8400 5a10 6412 6413 8400 5a11 6414  d...Z.d.d...Z.d.
+000000b0: 6415 8400 5a12 6513 6513 6416 9c02 6417  d...Z.e.e.d...d.
+000000c0: 6418 8404 5a14 6422 641a 641b 8401 5a15  d...Z.d"d.d...Z.
+000000d0: 641c 641d 8400 5a16 641e 641f 8400 5a17  d.d...Z.d.d...Z.
+000000e0: 6420 6421 8400 5a18 6401 5300 2923 e900  d d!..Z.d.S.)#..
+000000f0: 0000 004e 6300 0000 0000 0000 0000 0000  ...Nc...........
+00000100: 0005 0000 0005 0000 0043 0000 0073 5800  .........C...sX.
+00000110: 0000 6401 6402 6c00 6d01 7d00 0100 7402  ..d.d.l.m.}...t.
+00000120: 6a03 a004 7c00 7405 8301 6a06 6403 1900  j...|.t...j.d...
+00000130: 6404 6405 a103 7d01 7402 6a03 a004 7c00  d.d...}.t.j...|.
+00000140: 7405 8301 6a06 6403 1900 6404 6406 a103  t...j.d...d.d...
+00000150: 7d02 7407 7c01 8301 7d03 7407 7c02 8301  }.t.|...}.t.|...
+00000160: 7d04 7c03 7c04 6602 5300 2907 4e72 0100  }.|.|.f.S.).Nr..
+00000170: 0000 2901 da04 5061 7468 e901 0000 00da  ..)...Path......
+00000180: 0464 6174 617a 1261 6263 5f6d 616c 655f  .dataz.abc_male_
+00000190: 7365 6e74 732e 7478 747a 1161 6263 5f66  sents.txtz.abc_f
+000001a0: 656d 5f73 656e 7473 2e74 7874 2908 da07  em_sents.txt)...
+000001b0: 7061 7468 6c69 6272 0200 0000 da02 6f73  pathlibr......os
+000001c0: da04 7061 7468 da04 6a6f 696e da08 5f5f  ..path..join..__
+000001d0: 6669 6c65 5f5f da07 7061 7265 6e74 73da  file__..parents.
+000001e0: 0a6c 6f61 645f 7365 6e74 7329 0572 0200  .load_sents).r..
+000001f0: 0000 5a0b 696e 7061 7468 5f6d 616c 655a  ..Z.inpath_maleZ
+00000200: 0a69 6e70 6174 685f 6665 6d5a 0a6d 616c  .inpath_femZ.mal
+00000210: 655f 7365 6e74 735a 0966 656d 5f73 656e  e_sentsZ.fem_sen
+00000220: 7473 a900 720c 0000 00fa 772f 5573 6572  ts..r.....w/User
+00000230: 732f 6173 7472 6964 7279 626e 6572 2f44  s/astridrybner/D
+00000240: 6f63 756d 656e 7473 2f63 6f6f 6c2d 7072  ocuments/cool-pr
+00000250: 6f67 7261 6d6d 6572 2d74 6865 7369 732f  ogrammer-thesis/
+00000260: 6576 616c 6461 2d70 7562 322f 6576 616c  evalda-pub2/eval
+00000270: 6461 2d70 7562 322f 6576 616c 6461 5f70  da-pub2/evalda_p
+00000280: 7562 322f 6261 7365 5f74 6173 6b73 2f61  ub2/base_tasks/a
+00000290: 6263 5f6c 6d5f 7574 696c 6974 6965 732e  bc_lm_utilities.
+000002a0: 7079 da08 6c6f 6164 5f61 6263 0800 0000  py..load_abc....
+000002b0: 730c 0000 0000 010c 011a 011a 0108 0108  s...............
+000002c0: 0172 0e00 0000 6301 0000 0000 0000 0000  .r....c.........
+000002d0: 0000 0006 0000 0009 0000 0043 0000 0073  ...........C...s
+000002e0: 6600 0000 6700 7d01 7400 7c00 6401 8302  f...g.}.t.|.d...
+000002f0: 8f4e 7d02 7c02 a001 a100 7d03 6402 7d04  .N}.|.....}.d.}.
+00000300: 7c03 4400 5d36 7d05 6403 7c05 6b06 722e  |.D.]6}.d.|.k.r.
+00000310: 7120 6404 7c05 6b06 723c 6402 7d04 7120  q d.|.k.r<d.}.q 
+00000320: 7c04 6402 6b02 7220 7c01 a002 7c05 a003  |.d.k.r |...|...
+00000330: a100 a101 0100 6405 7d04 7120 5700 3500  ......d.}.q W.5.
+00000340: 5100 5200 5800 7c01 5300 2906 7a51 0a20  Q.R.X.|.S.).zQ. 
+00000350: 2020 2041 2066 756e 6374 696f 6e20 7468     A function th
+00000360: 6174 206c 6f61 6473 2061 6c6c 2074 6865  at loads all the
+00000370: 2072 6566 6c65 7869 7665 2073 656e 7465   reflexive sente
+00000380: 6e63 6573 2066 726f 6d20 7468 6520 4142  nces from the AB
+00000390: 4320 6461 7461 7365 742e 0a20 2020 20da  C dataset..    .
+000003a0: 0172 7201 0000 007a 0e2d 2d2d 2d2d 2d2d  .rr....z.-------
+000003b0: 2d2d 2d2d 2d2d 2d7a 032d 2d2d 7203 0000  -------z.---r...
+000003c0: 0029 04da 046f 7065 6eda 0972 6561 646c  .)...open..readl
+000003d0: 696e 6573 da06 6170 7065 6e64 da05 7374  ines..append..st
+000003e0: 7269 7029 06da 0866 696c 656e 616d 65da  rip)...filename.
+000003f0: 0f72 6566 6c65 7869 7665 5f73 656e 7473  .reflexive_sents
+00000400: da01 66da 056c 696e 6573 5a07 7265 7374  ..f..linesZ.rest
+00000410: 6172 74da 046c 696e 6572 0c00 0000 720c  art..liner....r.
+00000420: 0000 0072 0d00 0000 720b 0000 0010 0000  ...r....r.......
+00000430: 0073 1a00 0000 0004 0401 0c01 0802 0401  .s..............
+00000440: 0801 0800 0201 0801 0602 0801 0e01 1001  ................
+00000450: 720b 0000 0063 0400 0000 0000 0000 0000  r....c..........
+00000460: 0000 0500 0000 0300 0000 4300 0000 731a  ..........C...s.
+00000470: 0000 007c 027c 0017 007c 0317 007d 007c  ...|.|...|...}.|
+00000480: 01a0 007c 00a1 017d 047c 0453 0029 017a  ...|...}.|.S.).z
+00000490: 3c0a 2020 2020 4120 6675 6e63 7469 6f6e  <.    A function
+000004a0: 2074 6861 7420 746f 6b65 6e69 7a65 7320   that tokenizes 
+000004b0: 7468 6520 7265 666c 6578 6976 6520 7365  the reflexive se
+000004c0: 6e74 656e 6365 732e 0a20 2020 2029 01da  ntences..    )..
+000004d0: 0874 6f6b 656e 697a 6529 055a 0873 656e  .tokenize).Z.sen
+000004e0: 7465 6e63 65da 0974 6f6b 656e 697a 6572  tence..tokenizer
+000004f0: da0b 7374 6172 745f 746f 6b65 6eda 0973  ..start_token..s
+00000500: 6570 5f74 6f6b 656e da0e 746f 6b65 6e69  ep_token..tokeni
+00000510: 7a65 5f69 6e70 7574 720c 0000 0072 0c00  ze_inputr....r..
+00000520: 0000 720d 0000 00da 1174 6f6b 656e 697a  ..r......tokeniz
+00000530: 655f 7365 6e74 656e 6365 2300 0000 7306  e_sentence#...s.
+00000540: 0000 0000 040c 010a 0172 1e00 0000 6302  .........r....c.
+00000550: 0000 0000 0000 0000 0000 0006 0000 0003  ................
+00000560: 0000 0043 0000 0073 4000 0000 6401 7d02  ...C...s@...d.}.
+00000570: 7400 7c00 8301 4400 5d1e 5c02 7d03 7d04  t.|...D.].\.}.}.
+00000580: 7c04 7c01 6b06 720c 7c03 7d05 6402 7d02  |.|.k.r.|.}.d.}.
+00000590: 0100 712c 710c 710c 7c02 6401 6b02 7238  ..q,q.q.|.d.k.r8
+000005a0: 6403 5300 7c05 5300 6404 5300 2905 7aaf  d.S.|.S.d.S.).z.
+000005b0: 0a20 2020 2041 2066 756e 6374 696f 6e20  .    A function 
+000005c0: 7468 6174 2074 616b 6573 2074 6865 2074  that takes the t
+000005d0: 6f6b 656e 697a 6564 2072 6566 6c65 7869  okenized reflexi
+000005e0: 7665 2073 656e 7420 616e 640a 2020 2020  ve sent and.    
+000005f0: 6c6f 6361 7465 7320 696e 6465 7820 6f66  locates index of
+00000600: 2070 726f 6e6f 756e 0a20 2020 2072 6570   pronoun.    rep
+00000610: 6c61 6365 7320 7072 6f6e 6f75 6e20 7769  laces pronoun wi
+00000620: 7468 206d 616c 652f 6665 6d61 6c65 2070  th male/female p
+00000630: 726f 6e6f 756e 200a 2020 2020 7265 7475  ronoun .    retu
+00000640: 726e 7320 3220 6175 676d 656e 7465 6420  rns 2 augmented 
+00000650: 7365 6e74 656e 6365 7320 0a20 2020 2054  sentences .    T
+00000660: 467a 166e 6f20 7072 6f6e 6f75 6e73 2074  Fz.no pronouns t
+00000670: 6f20 7265 706c 6163 654e 2901 da09 656e  o replaceN)...en
+00000680: 756d 6572 6174 6529 06da 0473 656e 745a  umerate)...sentZ
+00000690: 0c70 726f 6e6f 756e 5f6c 6973 745a 076e  .pronoun_listZ.n
+000006a0: 6f5f 7072 6f6e da01 69da 0574 6f6b 656e  o_pron..i..token
+000006b0: 5a0a 7072 6f6e 5f69 6e64 6578 720c 0000  Z.pron_indexr...
+000006c0: 0072 0c00 0000 720d 0000 00da 0e67 6574  .r....r......get
+000006d0: 5f70 726f 6e5f 696e 6465 782b 0000 0073  _pron_index+...s
+000006e0: 1400 0000 0008 0401 1001 0801 0401 0401  ................
+000006f0: 0601 0201 0800 0401 7223 0000 0063 0200  ........r#...c..
+00000700: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00000710: 0000 4300 0000 7330 0000 007c 00a0 00a1  ..C...s0...|....
+00000720: 007d 027c 00a0 00a1 007d 0364 017c 0274  .}.|.....}.d.|.t
+00000730: 017c 0183 013c 0064 027c 0374 017c 0183  .|...<.d.|.t.|..
+00000740: 013c 007c 027c 0366 0253 0029 037a 600a  .<.|.|.f.S.).z`.
+00000750: 2020 2020 5461 6b65 206f 7269 6769 6e61      Take origina
+00000760: 6c20 7365 6e74 656e 6365 2061 6e64 2072  l sentence and r
+00000770: 6570 6c61 6365 2070 726f 6e6f 756e 2077  eplace pronoun w
+00000780: 6974 6820 616e 7469 7272 6566 6c65 7869  ith antirreflexi
+00000790: 7665 2070 726f 6e6f 756e 7320 2868 616e  ve pronouns (han
+000007a0: 732f 6865 6e64 6573 2920 0a20 2020 205a  s/hendes) .    Z
+000007b0: 0468 616e 735a 0668 656e 6465 7329 02da  .hansZ.hendes)..
+000007c0: 0463 6f70 79da 0369 6e74 2904 721d 0000  .copy..int).r...
+000007d0: 00da 0369 6478 5a12 746f 6b65 6e69 7a65  ...idxZ.tokenize
+000007e0: 5f6d 6173 6b5f 6d61 6c65 5a14 746f 6b65  _mask_maleZ.toke
+000007f0: 6e69 7a65 5f6d 6173 6b5f 6665 6d61 6c65  nize_mask_female
+00000800: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000810: 1367 6574 5f61 7567 6d65 6e74 6564 5f73  .get_augmented_s
+00000820: 656e 7473 3d00 0000 730a 0000 0000 0408  ents=...s.......
+00000830: 0108 010c 010c 0172 2700 0000 6304 0000  .......r'...c...
+00000840: 0000 0000 0000 0000 0007 0000 0005 0000  ................
+00000850: 0043 0000 0073 4000 0000 7400 a001 7c03  .C...s@...t...|.
+00000860: a002 7c00 a101 6701 a101 7d04 7400 a001  ..|...g...}.t...
+00000870: 7c03 a002 7c01 a101 6701 a101 7d05 7400  |...|...g...}.t.
+00000880: a001 7c03 a002 7c02 a101 6701 a101 7d06  ..|...|...g...}.
+00000890: 7c04 7c05 7c06 6603 5300 2901 7a30 0a20  |.|.|.f.S.).z0. 
+000008a0: 2020 204d 616b 6520 6175 676d 656e 7465     Make augmente
+000008b0: 6420 7365 6e74 656e 6365 7320 696e 746f  d sentences into
+000008c0: 2074 656e 736f 7273 2e0a 2020 2020 2903   tensors..    ).
+000008d0: da05 746f 7263 68da 0674 656e 736f 725a  ..torch..tensorZ
+000008e0: 1563 6f6e 7665 7274 5f74 6f6b 656e 735f  .convert_tokens_
+000008f0: 746f 5f69 6473 2907 da05 7472 7574 68da  to_ids)...truth.
+00000900: 046d 616c 655a 0366 656d 721a 0000 00da  .maleZ.femr.....
+00000910: 0c74 656e 736f 725f 7472 7574 68da 0b74  .tensor_truth..t
+00000920: 656e 736f 725f 6d61 6c65 da0a 7465 6e73  ensor_male..tens
+00000930: 6f72 5f66 656d 720c 0000 0072 0c00 0000  or_femr....r....
+00000940: 720d 0000 00da 0e63 7265 6174 655f 7465  r......create_te
+00000950: 6e73 6f72 7347 0000 0073 0800 0000 0004  nsorsG...s......
+00000960: 1201 1201 1201 722f 0000 0063 0400 0000  ......r/...c....
+00000970: 0000 0000 0000 0000 0700 0000 0900 0000  ................
+00000980: 4300 0000 736a 0000 0074 00a0 01a1 008f  C...sj...t......
+00000990: 1201 007c 037c 0083 0164 0119 007d 0457  ...|.|...d...}.W
+000009a0: 0035 0051 0052 0058 0074 00a0 01a1 008f  .5.Q.R.X.t......
+000009b0: 1201 007c 037c 0183 0164 0119 007d 0557  ...|.|...d...}.W
+000009c0: 0035 0051 0052 0058 0074 00a0 01a1 008f  .5.Q.R.X.t......
+000009d0: 1201 007c 037c 0283 0164 0119 007d 0657  ...|.|...d...}.W
+000009e0: 0035 0051 0052 0058 007c 047c 057c 0666  .5.Q.R.X.|.|.|.f
+000009f0: 0353 0029 027a 7c0a 2020 2020 4120 6675  .S.).z|.    A fu
+00000a00: 6e63 7469 6f6e 2074 6861 7420 7461 6b65  nction that take
+00000a10: 7320 7468 6520 3320 7365 6e74 656e 6365  s the 3 sentence
+00000a20: 7320 616e 6420 7265 7475 726e 7320 6d6f  s and returns mo
+00000a30: 6465 6c20 7072 6564 6963 7469 6f6e 7320  del predictions 
+00000a40: 666f 7220 6561 6368 206f 6620 7468 656d  for each of them
+00000a50: 2e0a 2020 2020 5573 6564 2074 6f20 636f  ..    Used to co
+00000a60: 6d70 7574 6520 6c6f 7373 2e20 2020 0a20  mpute loss.   . 
+00000a70: 2020 2072 0100 0000 2902 7228 0000 005a     r....).r(...Z
+00000a80: 076e 6f5f 6772 6164 2907 722c 0000 0072  .no_grad).r,...r
+00000a90: 2d00 0000 722e 0000 00da 056d 6f64 656c  -...r......model
+00000aa0: da0a 7072 6564 5f74 7275 7468 da09 7072  ..pred_truth..pr
+00000ab0: 6564 5f6d 616c 65da 0870 7265 645f 6665  ed_male..pred_fe
+00000ac0: 6d72 0c00 0000 720c 0000 0072 0d00 0000  mr....r....r....
+00000ad0: da0f 6765 745f 7072 6564 6963 7469 6f6e  ..get_prediction
+00000ae0: 7350 0000 0073 0e00 0000 0005 0a01 1601  sP...s..........
+00000af0: 0a01 1601 0a01 1601 7234 0000 0063 0500  ........r4...c..
+00000b00: 0000 0000 0000 0000 0000 0900 0000 0400  ................
+00000b10: 0000 4300 0000 734a 0000 007c 007c 02a0  ..C...sJ...|.|..
+00000b20: 00a1 007c 04a0 00a1 0083 026a 017d 057c  ...|.......j.}.|
+00000b30: 007c 03a0 00a1 007c 04a0 00a1 0083 026a  .|.....|.......j
+00000b40: 017d 067c 007c 01a0 00a1 007c 04a0 00a1  .}.|.|.....|....
+00000b50: 0083 026a 017d 077c 057c 067c 0767 037d  ...j.}.|.|.|.g.}
+00000b60: 087c 0853 0029 017a b40a 2020 2020 5461  .|.S.).z..    Ta
+00000b70: 6b65 206d 6f64 656c 2070 7265 6469 6374  ke model predict
+00000b80: 696f 6e73 2061 6e64 2063 6f6d 7075 7465  ions and compute
+00000b90: 206c 6f73 7320 666f 7220 616c 6c20 3320   loss for all 3 
+00000ba0: 7365 6e74 656e 6365 7320 0a20 2020 2062  sentences .    b
+00000bb0: 7920 636f 6d70 6172 696e 6720 746f 2070  y comparing to p
+00000bc0: 7265 645f 7472 7574 682c 2077 6869 6368  red_truth, which
+00000bd0: 2069 7320 7468 6520 7072 6564 6963 7469   is the predicti
+00000be0: 6f6e 206f 6620 7468 6520 7365 6e74 656e  on of the senten
+00000bf0: 6365 2077 6974 6820 7468 6520 636f 7272  ce with the corr
+00000c00: 6563 7420 2872 6566 6c65 7869 7665 2920  ect (reflexive) 
+00000c10: 7072 6f6e 6f75 6e2e 0a20 2020 2029 02da  pronoun..    )..
+00000c20: 0773 7175 6565 7a65 7204 0000 0029 09da  .squeezer....)..
+00000c30: 086c 6f73 735f 6663 7472 3100 0000 7232  .loss_fctr1...r2
+00000c40: 0000 0072 3300 0000 722c 0000 005a 096c  ...r3...r,...Z.l
+00000c50: 6f73 735f 6d61 6c65 5a08 6c6f 7373 5f66  oss_maleZ.loss_f
+00000c60: 656d 5a08 6c6f 7373 5f72 6566 5a09 6c6f  emZ.loss_refZ.lo
+00000c70: 7373 5f6c 6973 7472 0c00 0000 720c 0000  ss_listr....r...
+00000c80: 0072 0d00 0000 da0c 636f 6d70 7574 655f  .r......compute_
+00000c90: 6c6f 7373 5d00 0000 730a 0000 0000 0514  loss]...s.......
+00000ca0: 0114 0114 010a 0172 3700 0000 6307 0000  .......r7...c...
+00000cb0: 0000 0000 0000 0000 0012 0000 0007 0000  ................
+00000cc0: 0043 0000 0073 9200 0000 7400 7c00 7c02  .C...s....t.|.|.
+00000cd0: 7c05 7c06 8304 7d07 7401 7c07 7c04 8302  |.|...}.t.|.|...
+00000ce0: 7d08 7402 7c07 7c08 8302 5c02 7d09 7d0a  }.t.|.|...\.}.}.
+00000cf0: 7403 7c07 7c09 7c0a 7c02 8304 5c03 7d0b  t.|.|.|.|...\.}.
+00000d00: 7d0c 7d0d 7404 7c0b 7c0c 7c0d 7c03 8304  }.}.t.|.|.|.|...
+00000d10: 5c03 7d0e 7d0f 7d10 7405 7c01 7c0e 7c0f  \.}.}.}.t.|.|.|.
+00000d20: 7c10 7c0b 8305 7d11 7406 7407 a008 7c11  |.|...}.t.t...|.
+00000d30: 6401 1900 a101 8301 7406 7407 a008 7c11  d.......t.t...|.
+00000d40: 6402 1900 a101 8301 7406 7407 a008 7c11  d.......t.t...|.
+00000d50: 6403 1900 a101 8301 6603 5300 2904 6124  d.......f.S.).a$
+00000d60: 0200 000a 2020 2020 5461 6b20 6120 7365  ....    Tak a se
+00000d70: 6e74 656e 6365 2077 6974 6820 6120 7265  ntence with a re
+00000d80: 6c66 6c65 7869 7665 2070 726f 6e6f 756e  lflexive pronoun
+00000d90: 2c20 0a20 2020 2072 6570 6c61 6365 2070  , .    replace p
+00000da0: 726f 6e6f 756e 2077 6974 6820 616e 7469  ronoun with anti
+00000db0: 7265 666c 6578 6976 6573 2028 6d61 6c65  reflexives (male
+00000dc0: 2f66 656d 616c 6520 7072 6f6e 6f75 6e29  /female pronoun)
+00000dd0: 0a20 2020 2061 6e64 2063 6f6d 7075 7465  .    and compute
+00000de0: 206c 6f73 7320 616e 6420 7065 7270 6c65   loss and perple
+00000df0: 7869 7479 2066 6f72 2061 6c6c 2033 2073  xity for all 3 s
+00000e00: 656e 7465 6e63 6573 2e0a 2020 2020 4172  entences..    Ar
+00000e10: 6773 3a0a 2020 2020 2020 2020 7365 6e74  gs:.        sent
+00000e20: 2028 7374 7229 3a20 4120 7365 6e74 656e   (str): A senten
+00000e30: 6365 2077 6974 6820 7265 666c 6578 6976  ce with reflexiv
+00000e40: 6520 7072 6f6e 6f75 6e73 2e0a 2020 2020  e pronouns..    
+00000e50: 2020 2020 6c6f 7373 5f66 6374 2028 746f      loss_fct (to
+00000e60: 7263 682e 6e6e 2e43 726f 7373 456e 7472  rch.nn.CrossEntr
+00000e70: 6f70 794c 6f73 7329 3a20 4120 6c6f 7373  opyLoss): A loss
+00000e80: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
+00000e90: 2020 2074 6f6b 656e 697a 6572 2028 4265     tokenizer (Be
+00000ea0: 7274 546f 6b65 6e69 7a65 7229 3a20 4120  rtTokenizer): A 
+00000eb0: 746f 6b65 6e69 7a65 722e 0a20 2020 2020  tokenizer..     
+00000ec0: 2020 206d 6f64 656c 2028 4265 7274 466f     model (BertFo
+00000ed0: 724d 6173 6b65 644c 4d29 3a20 4120 6c61  rMaskedLM): A la
+00000ee0: 6e67 7561 6765 206d 6f64 656c 2e0a 2020  nguage model..  
+00000ef0: 2020 2020 2020 7072 6f6e 5f6c 6973 7420        pron_list 
+00000f00: 286c 6973 7429 3a20 4120 6c69 7374 206f  (list): A list o
+00000f10: 6620 7072 6f6e 6f75 6e73 2e0a 2020 2020  f pronouns..    
+00000f20: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00000f30: 204c 6f73 7320 616e 6420 7065 7270 6c65   Loss and perple
+00000f40: 7869 7479 2076 616c 7565 7320 666f 7220  xity values for 
+00000f50: 7365 6e74 656e 6365 2077 6974 6820 7265  sentence with re
+00000f60: 666c 6578 6976 652c 206d 616c 6520 616e  flexive, male an
+00000f70: 6420 6665 6d61 6c65 2070 726f 6e6f 756e  d female pronoun
+00000f80: 2e20 0a20 2020 2072 0100 0000 7203 0000  . .    r....r...
+00000f90: 00e9 0200 0000 2909 721e 0000 0072 2300  ......).r....r#.
+00000fa0: 0000 7227 0000 0072 2f00 0000 7234 0000  ..r'...r/...r4..
+00000fb0: 0072 3700 0000 da03 7374 72da 046d 6174  .r7.....str..mat
+00000fc0: 68da 0365 7870 2912 7220 0000 0072 3600  h..exp).r ...r6.
+00000fd0: 0000 721a 0000 0072 3000 0000 5a09 7072  ..r....r0...Z.pr
+00000fe0: 6f6e 5f6c 6973 7472 1b00 0000 721c 0000  on_listr....r...
+00000ff0: 005a 0e74 6f6b 656e 697a 6564 5f72 6566  .Z.tokenized_ref
+00001000: 6cda 0569 6e64 6578 5a0e 746f 6b65 6e69  l..indexZ.tokeni
+00001010: 7a65 645f 6d61 6c65 5a0d 746f 6b65 6e69  zed_maleZ.tokeni
+00001020: 7a65 645f 6665 6d72 2c00 0000 722d 0000  zed_femr,...r-..
+00001030: 0072 2e00 0000 7231 0000 0072 3200 0000  .r....r1...r2...
+00001040: 7233 0000 005a 0b6c 6f73 735f 7661 6c75  r3...Z.loss_valu
+00001050: 6573 720c 0000 0072 0c00 0000 720d 0000  esr....r....r...
+00001060: 00da 0a73 636f 7265 5f73 656e 7468 0000  ...score_senth..
+00001070: 0073 0e00 0000 000e 0e01 0a01 0e01 1401  .s..............
+00001080: 1401 1001 723d 0000 0063 0600 0000 0000  ....r=...c......
+00001090: 0000 0000 0000 1100 0000 0900 0000 4300  ..............C.
+000010a0: 0000 730c 0100 0074 006a 01a0 02a1 007d  ..s....t.j.....}
+000010b0: 0664 0164 0264 0364 0464 0564 0667 067d  .d.d.d.d.d.d.g.}
+000010c0: 0774 0364 077c 019b 0064 089d 0383 0101  .t.d.|...d......
+000010d0: 0074 046a 0574 067c 0083 0164 098d 01a0  .t.j.t.|...d....
+000010e0: 07a1 007d 0867 0067 0067 0067 0066 045c  ...}.g.g.g.g.f.\
+000010f0: 047d 097d 0a7d 0b7d 0c74 087c 0083 0144  .}.}.}.}.t.|...D
+00001100: 005d 5a5c 027d 0d7d 0e74 097c 0e7c 067c  .]Z\.}.}.t.|.|.|
+00001110: 027c 037c 077c 047c 0583 077d 0f7c 09a0  .|.|.|.|...}.|..
+00001120: 0a7c 0ea1 0101 007c 0aa0 0a7c 0f64 0a19  .|.....|...|.d..
+00001130: 00a1 0101 007c 0ba0 0a7c 0f64 0b19 00a1  .....|...|.d....
+00001140: 0101 007c 0ca0 0a7c 0f64 0c19 00a1 0101  ...|...|.d......
+00001150: 007c 08a0 0b7c 0da1 0101 0071 5a7c 08a0  .|...|.....qZ|..
+00001160: 0ca1 0001 0074 0da0 0e7c 097c 0a7c 0b7c  .....t...|.|.|.|
+00001170: 0c64 0d9c 04a1 017d 107c 1064 0e19 00a0  .d.....}.|.d....
+00001180: 0f74 10a1 017c 1064 0e3c 007c 1064 0f19  .t...|.d.<.|.d..
+00001190: 00a0 0f74 10a1 017c 1064 0f3c 007c 1064  ...t...|.d.<.|.d
+000011a0: 1019 00a0 0f74 10a1 017c 1064 103c 007c  .....t...|.d.<.|
+000011b0: 1053 0029 1161 8b01 0000 0a20 2020 2052  .S.).a.....    R
+000011c0: 756e 2074 6865 2041 4243 2064 6174 6173  un the ABC datas
+000011d0: 6574 2061 6e64 2077 7269 7465 2072 6573  et and write res
+000011e0: 756c 7473 2074 6f20 6669 6c65 2e0a 2020  ults to file..  
+000011f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00001200: 6f75 7470 6174 6820 2873 7472 293a 2050  outpath (str): P
+00001210: 6174 6820 746f 206f 7574 7075 7420 6669  ath to output fi
+00001220: 6c65 2e0a 2020 2020 2020 2020 7265 666c  le..        refl
+00001230: 6578 6976 655f 7365 6e74 7320 286c 6973  exive_sents (lis
+00001240: 7429 3a20 4120 6c69 7374 206f 6620 7365  t): A list of se
+00001250: 6e74 656e 6365 7320 7769 7468 2072 6566  ntences with ref
+00001260: 6c65 7869 7665 2070 726f 6e6f 756e 732e  lexive pronouns.
+00001270: 0a20 2020 2020 2020 206c 6f73 735f 6663  .        loss_fc
+00001280: 7420 2874 6f72 6368 2e6e 6e2e 4372 6f73  t (torch.nn.Cros
+00001290: 7345 6e74 726f 7079 4c6f 7373 293a 2041  sEntropyLoss): A
+000012a0: 206c 6f73 7320 6675 6e63 7469 6f6e 2e0a   loss function..
+000012b0: 2020 2020 2020 2020 746f 6b65 6e69 7a65          tokenize
+000012c0: 7220 2842 6572 7454 6f6b 656e 697a 6572  r (BertTokenizer
+000012d0: 293a 2041 2074 6f6b 656e 697a 6572 2e0a  ): A tokenizer..
+000012e0: 2020 2020 2020 2020 6d6f 6465 6c20 2842          model (B
+000012f0: 6572 7446 6f72 4d61 736b 6564 4c4d 293a  ertForMaskedLM):
+00001300: 2041 206c 616e 6775 6167 6520 6d6f 6465   A language mode
+00001310: 6c2e 0a20 2020 2020 2020 2070 726f 6e5f  l..        pron_
+00001320: 6c69 7374 2028 6c69 7374 293a 2041 206c  list (list): A l
+00001330: 6973 7420 6f66 2070 726f 6e6f 756e 732e  ist of pronouns.
+00001340: 0a20 2020 20da 0373 696e 5a03 7369 745a  .    ..sinZ.sitZ
+00001350: 0473 696e 6575 0600 0000 e296 8173 696e  .sineu.......sin
+00001360: 7506 0000 00e2 9681 7369 7475 0700 0000  u.......situ....
+00001370: e296 8173 696e 657a 1b52 756e 6e69 6e67  ...sinez.Running
+00001380: 2074 6573 7420 6f6e 2063 6f6e 6469 7469   test on conditi
+00001390: 6f6e 3a20 7a0d 206f 6363 7570 6174 696f  on: z. occupatio
+000013a0: 6e73 2e29 015a 066d 6178 7661 6c72 0100  ns.).Z.maxvalr..
+000013b0: 0000 7203 0000 0072 3800 0000 2904 7220  ..r....r8...).r 
+000013c0: 0000 00da 0f70 6572 706c 6578 6974 795f  .....perplexity_
+000013d0: 6d61 6c65 da11 7065 7270 6c65 7869 7479  male..perplexity
+000013e0: 5f66 656d 616c 65da 1470 6572 706c 6578  _female..perplex
+000013f0: 6974 795f 7265 666c 6578 6976 6572 3f00  ity_reflexiver?.
+00001400: 0000 7240 0000 0072 4100 0000 2911 7228  ..r@...rA...).r(
+00001410: 0000 00da 026e 6e5a 1043 726f 7373 456e  .....nnZ.CrossEn
+00001420: 7472 6f70 794c 6f73 73da 0570 7269 6e74  tropyLoss..print
+00001430: da0b 7072 6f67 7265 7373 6261 725a 0b50  ..progressbarZ.P
+00001440: 726f 6772 6573 7342 6172 da03 6c65 6eda  rogressBar..len.
+00001450: 0573 7461 7274 721f 0000 0072 3d00 0000  .startr....r=...
+00001460: 7212 0000 00da 0675 7064 6174 655a 0666  r......updateZ.f
+00001470: 696e 6973 68da 0270 64da 0944 6174 6146  inish..pd..DataF
+00001480: 7261 6d65 da06 6173 7479 7065 da05 666c  rame..astype..fl
+00001490: 6f61 7429 1172 1500 0000 da09 636f 6e64  oat).r......cond
+000014a0: 6974 696f 6e72 1a00 0000 7230 0000 0072  itionr....r0...r
+000014b0: 1b00 0000 721c 0000 0072 3600 0000 5a0d  ....r....r6...Z.
+000014c0: 7072 6f6e 6f75 6e73 5f6c 6973 74da 0362  pronouns_list..b
+000014d0: 6172 5a05 7365 6e74 735a 0670 6572 705f  arZ.sentsZ.perp_
+000014e0: 6d5a 0670 6572 705f 665a 0670 6572 705f  mZ.perp_fZ.perp_
+000014f0: 7272 2600 0000 7220 0000 005a 0673 636f  rr&...r ...Z.sco
+00001500: 7265 73da 0264 6672 0c00 0000 720c 0000  res..dfr....r...
+00001510: 0072 0d00 0000 da07 7275 6e5f 6162 637e  .r......run_abc~
+00001520: 0000 0073 2c00 0000 000d 0a02 1003 1001  ...s,...........
+00001530: 1402 1402 1001 1401 0a01 0e01 0e01 0e01  ................
+00001540: 0c01 0802 0601 0201 0201 02fd 0805 1201  ................
+00001550: 1201 1202 724f 0000 00a9 02da 0178 da01  ....rO.......x..
+00001560: 7963 0200 0000 0000 0000 0000 0000 0200  yc..............
+00001570: 0000 0500 0000 4300 0000 7314 0000 0074  ......C...s....t
+00001580: 0074 01a0 027c 007c 011b 00a1 0164 0183  .t...|.|.....d..
+00001590: 0253 0029 024e 7238 0000 0029 03da 0572  .S.).Nr8...)...r
+000015a0: 6f75 6e64 723a 0000 00da 046c 6f67 3272  oundr:.....log2r
+000015b0: 5000 0000 720c 0000 0072 0c00 0000 720d  P...r....r....r.
+000015c0: 0000 00da 086c 6f67 7261 7469 6fab 0000  .....logratio...
+000015d0: 0073 0200 0000 0001 7255 0000 0046 6302  .s......rU...Fc.
+000015e0: 0000 0000 0000 0000 0000 0007 0000 0007  ................
+000015f0: 0000 0043 0000 0073 d000 0000 7400 7c00  ...C...s....t.|.
+00001600: 6a01 a002 a100 a003 6401 a101 8301 7d02  j.......d.....}.
+00001610: 7400 7404 7405 a006 7c00 6a01 6402 6403  t.t.t...|.j.d.d.
+00001620: 6702 a102 a003 6401 a101 8301 8301 7d03  g.....d.......}.
+00001630: 7400 7c00 6a07 a002 a100 a003 6401 a101  t.|.j.......d...
+00001640: 8301 7d04 7400 7404 7405 a006 7c00 6a07  ..}.t.t.t...|.j.
+00001650: 6402 6403 6702 a102 a003 6401 a101 8301  d.d.g.....d.....
+00001660: 8301 7d05 7c01 6404 6b02 72a4 7408 7409  ..}.|.d.k.r.t.t.
+00001670: 7c02 8301 7409 7c04 8301 8302 7d06 7400  |...t.|.....}.t.
+00001680: 7c02 6405 1700 7c03 1700 8301 7400 7c04  |.d...|.....t.|.
+00001690: 6405 1700 7c05 1700 8301 7c06 6603 5300  d...|.....|.f.S.
+000016a0: 7c01 6406 6b02 72cc 7400 7c02 6405 1700  |.d.k.r.t.|.d...
+000016b0: 7c03 1700 8301 7400 7c04 6405 1700 7c05  |.....t.|.d...|.
+000016c0: 1700 8301 6602 5300 6400 5300 2907 4e72  ....f.S.d.S.).Nr
+000016d0: 3800 0000 e919 0000 00e9 4b00 0000 54da  8.........K...T.
+000016e0: 0120 4629 0a72 3900 0000 da0f 7265 6c61  . F).r9.....rela
+000016f0: 7469 7665 5f66 656d 616c 65da 066d 6564  tive_female..med
+00001700: 6961 6e72 5300 0000 da05 7475 706c 65da  ianrS.....tuple.
+00001710: 026e 70da 0a70 6572 6365 6e74 696c 65da  .np..percentile.
+00001720: 0d72 656c 6174 6976 655f 6d61 6c65 7255  .relative_malerU
+00001730: 0000 0072 4b00 0000 2907 724e 0000 00da  ...rK...).rN....
+00001740: 076c 5f72 6174 696f 5a0a 6d65 6469 616e  .l_ratioZ.median
+00001750: 5f66 656d 5a07 6971 725f 6665 6d5a 0b6d  _femZ.iqr_femZ.m
+00001760: 6564 6961 6e5f 6d61 6c65 5a08 6971 725f  edian_maleZ.iqr_
+00001770: 6d61 6c65 da05 7261 7469 6f72 0c00 0000  male..ratior....
+00001780: 720c 0000 0072 0d00 0000 da0f 6361 6c63  r....r......calc
+00001790: 5f6d 6564 6961 6e5f 6971 72ae 0000 0073  _median_iqr....s
+000017a0: 1200 0000 0003 1401 2003 1401 2001 0801  ........ ... ...
+000017b0: 1201 2201 0801 7261 0000 0063 0400 0000  .."...ra...c....
+000017c0: 0000 0000 0000 0000 0600 0000 0b00 0000  ................
+000017d0: 4300 0000 7364 0000 0064 017c 039b 009d  C...sd...d.|....
+000017e0: 0264 0264 0364 0264 0267 0464 0464 027c  .d.d.d.d.g.d.d.|
+000017f0: 0264 0264 0267 0464 0564 0664 0264 0264  .d.d.g.d.d.d.d.d
+00001800: 0767 0464 0864 027c 0064 027c 0167 0469  .g.d.d.|.d.|.g.i
+00001810: 047d 0474 00a0 017c 04a1 016a 027d 057c  .}.t...|...j.}.|
+00001820: 056a 0364 0919 007c 055f 047c 056a 0364  .j.d...|._.|.j.d
+00001830: 0a64 0085 0219 007d 057c 0553 0029 0b4e  .d.....}.|.S.).N
+00001840: 7a0f 5369 6d70 6c65 204f 7574 7075 743a  z.Simple Output:
+00001850: 20da 00da 0341 4243 fa12 4765 6e64 6572   ....ABC..Gender
+00001860: 2045 6666 6563 7420 5369 7a65 da07 5072   Effect Size..Pr
+00001870: 6f6e 6f75 6eda 0646 656d 616c 65da 044d  onoun..Female..M
+00001880: 616c 65fa 2750 6572 706c 6578 6974 7920  ale.'Perplexity 
+00001890: 4d65 6469 616e 2028 4951 5229 2052 656c  Median (IQR) Rel
+000018a0: 6174 6976 6520 7363 6f72 6573 7201 0000  ative scoresr...
+000018b0: 0072 0300 0000 a905 7248 0000 0072 4900  .r......rH...rI.
+000018c0: 0000 da01 54da 0469 6c6f 63da 0763 6f6c  ....T..iloc..col
+000018d0: 756d 6e73 2906 da10 616c 6c5f 6f63 635f  umns)...all_occ_
+000018e0: 4645 4d5f 5052 4f4e da11 616c 6c5f 6f63  FEM_PRON..all_oc
+000018f0: 635f 4d41 4c45 5f50 524f 4eda 066c 7261  c_MALE_PRON..lra
+00001900: 7469 6fda 0a6d 6f64 656c 5f6e 616d 6572  tio..model_namer
+00001910: 0400 0000 724e 0000 0072 0c00 0000 720c  ....rN...r....r.
+00001920: 0000 0072 0d00 0000 da0d 6765 745f 636f  ...r......get_co
+00001930: 6e64 656e 7365 64bd 0000 0073 1a00 0000  ndensed....s....
+00001940: 0002 0800 0a01 0200 0a01 0200 0a01 0200  ................
+00001950: 0afc 0405 0c01 0c01 0e01 7271 0000 0063  ..........rq...c
+00001960: 0800 0000 0000 0000 0000 0000 0a00 0000  ................
+00001970: 0f00 0000 4300 0000 737c 0000 0064 017c  ....C...s|...d.|
+00001980: 079b 009d 0264 0264 0364 0264 0267 0464  .....d.d.d.d.g.d
+00001990: 0464 027c 0264 0264 0267 0464 0564 0664  .d.|.d.d.g.d.d.d
+000019a0: 0264 0764 0267 0464 087c 0064 027c 0164  .d.d.g.d.|.d.|.d
+000019b0: 0267 0464 0964 0664 0764 0664 0767 0464  .g.d.d.d.d.d.g.d
+000019c0: 0a7c 037c 057c 047c 0667 0469 067d 0874  .|.|.|.|.g.i.}.t
+000019d0: 00a0 017c 08a1 016a 027d 097c 096a 0364  ...|...j.}.|.j.d
+000019e0: 0b19 007c 095f 047c 096a 0364 0c64 0085  ...|._.|.j.d.d..
+000019f0: 0219 007d 097c 0953 0029 0d4e 7a15 4465  ...}.|.S.).Nz.De
+00001a00: 7461 696c 6564 204f 7574 7075 7420 666f  tailed Output fo
+00001a10: 723a 2072 6200 0000 7263 0000 0072 6400  r: rb...rc...rd.
+00001a20: 0000 7265 0000 0072 6600 0000 7267 0000  ..re...rf...rg..
+00001a30: 0072 6800 0000 7a18 5374 6572 656f 7479  .rh...z.Stereoty
+00001a40: 7069 6361 6c20 4f63 6375 7061 7469 6f6e  pical Occupation
+00001a50: 7a28 5065 7270 6c65 7869 7479 204d 6564  z(Perplexity Med
+00001a60: 6961 6e20 2849 5152 2920 5265 6c61 7469  ian (IQR) Relati
+00001a70: 7665 2073 636f 7265 7320 7201 0000 0072  ve scores r....r
+00001a80: 0300 0000 7269 0000 0029 0a72 6d00 0000  ....ri...).rm...
+00001a90: 726e 0000 0072 6f00 0000 da10 6665 6d5f  rn...ro.....fem_
+00001aa0: 6f63 635f 4645 4d5f 5052 4f4e da11 6665  occ_FEM_PRON..fe
+00001ab0: 6d5f 6f63 635f 4d41 4c45 5f50 524f 4eda  m_occ_MALE_PRON.
+00001ac0: 116d 616c 655f 6f63 635f 4645 4d5f 5052  .male_occ_FEM_PR
+00001ad0: 4f4e da12 6d61 6c65 5f6f 6363 5f4d 414c  ON..male_occ_MAL
+00001ae0: 455f 5052 4f4e 7270 0000 0072 0400 0000  E_PRONrp...r....
+00001af0: 724e 0000 0072 0c00 0000 720c 0000 0072  rN...r....r....r
+00001b00: 0d00 0000 da0c 6765 745f 6465 7461 696c  ......get_detail
+00001b10: 6564 c800 0000 7320 0000 0000 0112 0102  ed....s ........
+00001b20: 000a 0102 000a 0102 000a 0102 000a 0102  ................
+00001b30: 000a fb04 060c 010c 010e 0172 7600 0000  ...........rv...
+00001b40: 6303 0000 0000 0000 0000 0000 000d 0000  c...............
+00001b50: 0009 0000 0043 0000 0073 b800 0000 7c00  .....C...s....|.
+00001b60: 6401 1900 7c00 6402 1900 1800 7c00 6403  d...|.d.....|.d.
+00001b70: 3c00 7c00 6404 1900 7c00 6402 1900 1800  <.|.d...|.d.....
+00001b80: 7c00 6405 3c00 7c01 6401 1900 7c01 6402  |.d.<.|.d...|.d.
+00001b90: 1900 1800 7c01 6403 3c00 7c01 6404 1900  ....|.d.<.|.d...
+00001ba0: 7c01 6402 1900 1800 7c01 6405 3c00 7400  |.d.....|.d.<.t.
+00001bb0: 6a01 7c00 7c01 6702 6406 6407 8d02 7d03  j.|.|.g.d.d...}.
+00001bc0: 7402 7c00 8301 5c02 7d04 7d05 7402 7c01  t.|...\.}.}.t.|.
+00001bd0: 8301 5c02 7d06 7d07 7402 7c03 6406 6408  ..\.}.}.t.|.d.d.
+00001be0: 8d02 5c03 7d08 7d09 7d0a 7403 7c08 7c09  ..\.}.}.}.t.|.|.
+00001bf0: 7c0a 7c02 8304 7d0b 7404 7c08 7c09 7c0a  |.|...}.t.|.|.|.
+00001c00: 7c04 7c05 7c06 7c07 7c02 8308 7d0c 7c0b  |.|.|.|.|...}.|.
+00001c10: 7c0c 6702 5300 2909 4e72 4000 0000 7241  |.g.S.).Nr@...rA
+00001c20: 0000 0072 5900 0000 723f 0000 0072 5e00  ...rY...r?...r^.
+00001c30: 0000 5429 01da 0c69 676e 6f72 655f 696e  ..T)...ignore_in
+00001c40: 6465 7829 0172 5f00 0000 2905 7248 0000  dex).r_...).rH..
+00001c50: 00da 0663 6f6e 6361 7472 6100 0000 7271  ...concatra...rq
+00001c60: 0000 0072 7600 0000 290d 5a0a 6466 5f46  ...rv...).Z.df_F
+00001c70: 454d 5f6f 6363 5a0b 6466 5f4d 414c 455f  EM_occZ.df_MALE_
+00001c80: 6f63 6372 7000 0000 5a07 414c 4c5f 6f63  occrp...Z.ALL_oc
+00001c90: 6372 7200 0000 7273 0000 0072 7400 0000  crr...rs...rt...
+00001ca0: 7275 0000 0072 6d00 0000 726e 0000 005a  ru...rm...rn...Z
+00001cb0: 096c 6f67 5f72 6174 696f 5a0d 6f75 745f  .log_ratioZ.out_
+00001cc0: 636f 6e64 656e 7365 645a 0c6f 7574 5f64  condensedZ.out_d
+00001cd0: 6574 6169 6c65 6472 0c00 0000 720c 0000  etailedr....r...
+00001ce0: 0072 0d00 0000 da0a 6765 745f 6f75 7470  .r......get_outp
+00001cf0: 7574 d400 0000 7316 0000 0000 0214 0114  ut....s.........
+00001d00: 0114 0114 0312 030c 010c 0112 030e 0316  ................
+00001d10: 0272 7900 0000 2901 4629 19da 0373 7973  .ry...).F)...sys
+00001d20: 7206 0000 00da 0670 616e 6461 7372 4800  r......pandasrH.
+00001d30: 0000 da05 6e75 6d70 7972 5c00 0000 7228  ....numpyr\...r(
+00001d40: 0000 0072 3a00 0000 7244 0000 0072 0e00  ...r:...rD...r..
+00001d50: 0000 720b 0000 0072 1e00 0000 7223 0000  ..r....r....r#..
+00001d60: 0072 2700 0000 722f 0000 0072 3400 0000  .r'...r/...r4...
+00001d70: 7237 0000 0072 3d00 0000 724f 0000 0072  r7...r=...rO...r
+00001d80: 4b00 0000 7255 0000 0072 6100 0000 7271  K...rU...ra...rq
+00001d90: 0000 0072 7600 0000 7279 0000 0072 0c00  ...rv...ry...r..
+00001da0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00001db0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001dc0: 2800 0000 1001 0801 0801 0801 0801 0802  (...............
+00001dd0: 0808 0813 0808 0812 080a 0809 080d 080b  ................
+00001de0: 0816 082d 1003 0a0f 080b 080c            ...-........
```

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-39.pyc` & `evalda_pub2-0.0.6/evalda_pub2/base_tasks/__pycache__/wino_fillmask_utilities.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May 11 08:11:25 2023 UTC, .py size: 6576 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2da3 5c64 b019 0000  a.......-.\d....
+00000000: 550d 0d0a 0000 0000 2da3 5c64 b019 0000  U.......-.\d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6401 6c01  d.l.m.Z...d.d.l.
 00000060: 5a01 6400 6401 6c03 5a03 6400 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000070: 6d07 5a07 0100 6400 6401 6c08 5a09 6400  m.Z...d.d.l.Z.d.
@@ -13,349 +13,351 @@
 000000c0: 5a12 640f 6410 8400 5a13 6411 6412 8400  Z.d.d...Z.d.d...
 000000d0: 5a14 6515 6515 6413 9c02 6414 6415 8404  Z.e.e.d...d.d...
 000000e0: 5a16 6416 6417 8400 5a17 6401 5300 2918  Z.d.d...Z.d.S.).
 000000f0: e900 0000 004e 2901 da07 436f 756e 7465  .....N)...Counte
 00000100: 7229 01da 1563 6c61 7373 6966 6963 6174  r)...classificat
 00000110: 696f 6e5f 7265 706f 7274 2901 da04 5061  ion_report)...Pa
 00000120: 7468 6301 0000 0000 0000 0000 0000 0004  thc.............
-00000130: 0000 0008 0000 0043 0000 0073 5000 0000  .......C...sP...
-00000140: 7400 7c00 8301 8f1c 7d01 7c01 a001 a100  t.|.....}.|.....
-00000150: a002 a100 7d02 5700 6401 0400 0400 8303  ....}.W.d.......
-00000160: 0100 6e10 3100 732a 3000 0100 0100 0100  ..n.1.s*0.......
-00000170: 5900 0100 6402 6403 8400 7c02 4400 8301  Y...d.d...|.D...
-00000180: 7d03 7403 a004 7c03 a101 0100 7c03 5300  }.t...|.....|.S.
-00000190: 2904 7a2e 6c6f 6164 2044 6157 696e 6f42  ).z.load DaWinoB
-000001a0: 6961 7320 7465 7874 7320 2d20 616e 6420  ias texts - and 
-000001b0: 7368 7566 666c 6520 6461 7461 200a 2020  shuffle data .  
-000001c0: 2020 4e63 0100 0000 0000 0000 0000 0000    Nc............
-000001d0: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-000001e0: 0067 007c 005d 0c7d 017c 01a0 00a1 0091  .g.|.].}.|......
-000001f0: 0271 0453 00a9 0029 01da 0573 7472 6970  .q.S...)...strip
-00000200: 2902 da02 2e30 da04 6c69 6e65 7205 0000  )....0..liner...
-00000210: 0072 0500 0000 fa7e 2f55 7365 7273 2f61  .r.....~/Users/a
-00000220: 7374 7269 6472 7962 6e65 722f 446f 6375  stridrybner/Docu
-00000230: 6d65 6e74 732f 636f 6f6c 2d70 726f 6772  ments/cool-progr
-00000240: 616d 6d65 722d 7468 6573 6973 2f65 7661  ammer-thesis/eva
-00000250: 6c64 612d 7075 6232 2f65 7661 6c64 612d  lda-pub2/evalda-
-00000260: 7075 6232 2f65 7661 6c64 615f 7075 6232  pub2/evalda_pub2
-00000270: 2f62 6173 655f 7461 736b 732f 7769 6e6f  /base_tasks/wino
-00000280: 5f66 696c 6c6d 6173 6b5f 7574 696c 6974  _fillmask_utilit
-00000290: 6965 732e 7079 da0a 3c6c 6973 7463 6f6d  ies.py..<listcom
-000002a0: 703e 0f00 0000 f300 0000 007a 1e6c 6f61  p>.........z.loa
-000002b0: 645f 7465 7874 732e 3c6c 6f63 616c 733e  d_texts.<locals>
-000002c0: 2e3c 6c69 7374 636f 6d70 3e29 05da 046f  .<listcomp>)...o
-000002d0: 7065 6eda 0472 6561 64da 0a73 706c 6974  pen..read..split
-000002e0: 6c69 6e65 73da 0672 616e 646f 6dda 0773  lines..random..s
-000002f0: 6875 6666 6c65 2904 da08 6669 6c65 7061  huffle)...filepa
-00000300: 7468 da04 6669 6c65 da04 7465 7874 da05  th..file..text..
-00000310: 6c69 6e65 7372 0500 0000 7205 0000 0072  linesr....r....r
-00000320: 0900 0000 da0a 6c6f 6164 5f74 6578 7473  ......load_texts
-00000330: 0a00 0000 730a 0000 0000 030a 012a 010e  ....s........*..
-00000340: 010a 0172 1500 0000 6301 0000 0000 0000  ...r....c.......
-00000350: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00000360: 0073 1000 0000 6401 6402 8400 7c00 4400  .s....d.d...|.D.
-00000370: 8301 6701 5300 2903 4e63 0100 0000 0000  ..g.S.).Nc......
-00000380: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00000390: 0000 7320 0000 0067 007c 005d 187d 017c  ..s ...g.|.].}.|
-000003a0: 0164 006b 0372 047c 0164 016b 0372 047c  .d.k.r.|.d.k.r.|
-000003b0: 0191 0271 0453 0029 02fa 015b fa01 5d72  ...q.S.)...[..]r
-000003c0: 0500 0000 a902 7207 0000 00da 0574 6f6b  ......r......tok
-000003d0: 656e 7205 0000 0072 0500 0000 7209 0000  enr....r....r...
-000003e0: 0072 0a00 0000 1500 0000 720b 0000 007a  .r........r....z
-000003f0: 2072 656d 6f76 655f 7371 5f62 722e 3c6c   remove_sq_br.<l
-00000400: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000410: 3e72 0500 0000 a901 da06 746f 6b65 6e73  >r........tokens
-00000420: 7205 0000 0072 0500 0000 7209 0000 00da  r....r....r.....
-00000430: 0c72 656d 6f76 655f 7371 5f62 7213 0000  .remove_sq_br...
-00000440: 0073 0200 0000 0002 721c 0000 0063 0100  .s......r....c..
-00000450: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00000460: 0000 0300 0000 7322 0000 0067 0064 01a2  ......s"...g.d..
-00000470: 017d 0187 0066 0164 0264 0384 087c 0144  .}...f.d.d...|.D
-00000480: 0083 0164 0419 007d 027c 0253 0029 057a  ...d...}.|.S.).z
-00000490: 2547 6574 2069 6e64 6578 206f 6620 7072  %Get index of pr
-000004a0: 6f6e 6f75 6e20 696e 2073 656e 7465 6e63  onoun in sentenc
-000004b0: 650a 2020 2020 290c da04 6861 6e73 da06  e.    )...hans..
-000004c0: 6865 6e64 6573 da03 6861 6eda 0368 756e  hendes..han..hun
-000004d0: da03 6861 6dda 0568 656e 6465 f506 0000  ..ham..hende....
-000004e0: 00e2 9681 6875 6ef5 0900 0000 e296 8168  ....hun........h
-000004f0: 656e 6465 73f5 0800 0000 e296 8168 656e  endes........hen
-00000500: 6465 f506 0000 00e2 9681 6861 6ef5 0700  de........han...
-00000510: 0000 e296 8168 616e 73f5 0600 0000 e296  .....hans.......
-00000520: 8168 616d 6301 0000 0000 0000 0000 0000  .hamc...........
-00000530: 0002 0000 0005 0000 0013 0000 0073 1e00  .............s..
-00000540: 0000 6700 7c00 5d16 7d01 7c01 8800 7600  ..g.|.].}.|...v.
-00000550: 7204 8800 a000 7c01 a101 9102 7104 5300  r.....|.....q.S.
-00000560: 7205 0000 0029 01da 0569 6e64 6578 a902  r....)...index..
-00000570: 7207 0000 00da 0169 721a 0000 0072 0500  r......ir....r..
-00000580: 0000 7209 0000 0072 0a00 0000 1d00 0000  ..r....r........
-00000590: 720b 0000 007a 1c69 6478 5f70 726f 6e2e  r....z.idx_pron.
-000005a0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000005b0: 6d70 3e72 0100 0000 7205 0000 0029 0372  mp>r....r....).r
-000005c0: 1b00 0000 da08 7072 6f6e 6f75 6e73 da09  ......pronouns..
-000005d0: 7072 6f6e 735f 6964 7872 0500 0000 721a  prons_idxr....r.
-000005e0: 0000 0072 0900 0000 da08 6964 785f 7072  ...r......idx_pr
-000005f0: 6f6e 1700 0000 7306 0000 0000 0408 0216  on....s.........
-00000600: 0172 2e00 0000 6305 0000 0000 0000 0000  .r....c.........
-00000610: 0000 0010 0000 0005 0000 0043 0000 0073  ...........C...s
-00000620: d600 0000 6700 6700 0200 7d05 7d06 7400  ....g.g...}.}.t.
-00000630: 6a01 7402 7c00 8301 6401 8d01 a003 a100  j.t.|...d.......
-00000640: 7d07 7404 7c00 8301 4400 5d9e 5c02 7d08  }.t.|...D.].\.}.
-00000650: 7d09 7c02 7c09 8301 7d0a 6402 6403 8400  }.|.|...}.d.d...
-00000660: 7c0a 4400 8301 7d0b 7405 7c0b 8301 6404  |.D...}.t.|...d.
-00000670: 1900 7d0b 7406 7c0b 8301 7d0c 7c0b 7c0c  ..}.t.|...}.|.|.
-00000680: 1900 7d0d 7c03 7c0b 7c0c 3c00 7c03 6405  ..}.|.|.|.<.|.d.
-00000690: 6b02 728c 7c04 6406 6b02 728c 6407 a007  k.r.|.d.k.r.d...
-000006a0: 7c0b a101 a008 6408 6405 a102 7d0e 6e0a  |.....d.d...}.n.
-000006b0: 6407 a007 7c0b a101 7d0e 7c01 7c0e 8301  d...|...}.|.|...
-000006c0: 6404 1900 6409 1900 7d0f 7c05 a009 7c0d  d...d...}.|...|.
-000006d0: a101 0100 7c06 a009 7c0f a101 0100 7c07  ....|...|.....|.
-000006e0: a00a 7c08 a101 0100 7126 7c07 a00b a100  ..|.....q&|.....
-000006f0: 0100 7c05 7c06 6602 5300 290a 4e29 01da  ..|.|.f.S.).N)..
-00000700: 066d 6178 7661 6c63 0100 0000 0000 0000  .maxvalc........
-00000710: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00000720: 7316 0000 0067 007c 005d 0e7d 017c 016a  s....g.|.].}.|.j
-00000730: 00a0 01a1 0091 0271 0453 0072 0500 0000  .......q.S.r....
-00000740: 2902 7213 0000 00da 056c 6f77 6572 7218  ).r......lowerr.
-00000750: 0000 0072 0500 0000 7205 0000 0072 0900  ...r....r....r..
-00000760: 0000 720a 0000 0029 0000 0072 0b00 0000  ..r....)...r....
-00000770: 7a22 7072 6564 6963 745f 6d61 736b 6564  z"predict_masked
-00000780: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00000790: 6f6d 703e 7201 0000 007a 063c 6d61 736b  omp>r....z.<mask
-000007a0: 3e7a 1276 6573 7465 696e 6e2f 4461 6e73  >z.vesteinn/Dans
-000007b0: 6b42 6572 74fa 0120 7a07 203c 6d61 736b  kBert.. z. <mask
-000007c0: 3eda 0974 6f6b 656e 5f73 7472 290c da0b  >..token_str)...
-000007d0: 7072 6f67 7265 7373 6261 72da 0b50 726f  progressbar..Pro
-000007e0: 6772 6573 7342 6172 da03 6c65 6eda 0573  gressBar..len..s
-000007f0: 7461 7274 da09 656e 756d 6572 6174 6572  tart..enumerater
-00000800: 1c00 0000 722e 0000 00da 046a 6f69 6eda  ....r......join.
-00000810: 0772 6570 6c61 6365 da06 6170 7065 6e64  .replace..append
-00000820: da06 7570 6461 7465 da06 6669 6e69 7368  ..update..finish
-00000830: 2910 7214 0000 00da 036e 6c70 da09 746f  ).r......nlp..to
-00000840: 6b65 6e69 7a65 72da 0a6d 6173 6b5f 746f  kenizer..mask_to
-00000850: 6b65 6eda 0a6d 6f64 656c 5f6e 616d 65da  ken..model_name.
-00000860: 066c 6162 656c 73da 0570 7265 6473 da03  .labels..preds..
-00000870: 6261 72da 0369 6478 7208 0000 005a 0e6c  bar..idxr....Z.l
-00000880: 696e 655f 746f 6b65 6e69 7a65 6472 1b00  ine_tokenizedr..
-00000890: 0000 722d 0000 005a 0f63 6f72 7265 6374  ..r-...Z.correct
-000008a0: 5f70 726f 6e6f 756e da08 7365 6e74 656e  _pronoun..senten
-000008b0: 6365 da04 7072 6564 7205 0000 0072 0500  ce..predr....r..
-000008c0: 0000 7209 0000 00da 0e70 7265 6469 6374  ..r......predict
-000008d0: 5f6d 6173 6b65 6420 0000 0073 2400 0000  _masked ...s$...
-000008e0: 0001 0a03 1402 1002 0801 0e03 0c03 0803  ................
-000008f0: 0803 0804 1001 1402 0a03 1003 0a01 0a02  ................
-00000900: 0c01 0802 7247 0000 0063 0100 0000 0000  ....rG...c......
-00000910: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
-00000920: 0000 7354 0000 0067 0064 01a2 017d 0167  ..sT...g.d...}.g
-00000930: 0064 02a2 017d 0267 007d 037c 0044 005d  .d...}.g.}.|.D.]
-00000940: 367d 047c 047c 0176 0072 307c 03a0 0064  6}.|.|.v.r0|...d
-00000950: 03a1 0101 0071 187c 047c 0276 0072 447c  .....q.|.|.v.rD|
-00000960: 03a0 0064 04a1 0101 0071 187c 03a0 0064  ...d.....q.|...d
-00000970: 05a1 0101 0071 187c 0353 0029 067a 2867  .....q.|.S.).z(g
-00000980: 726f 7570 206c 6162 656c 7320 696e 2066  roup labels in f
-00000990: 656d 616c 6520 616e 6420 6d61 6c65 2070  emale and male p
-000009a0: 726f 6e6f 756e 7329 0672 2000 0000 721e  ronouns).r ...r.
-000009b0: 0000 0072 2200 0000 7223 0000 0072 2400  ...r"...r#...r$.
-000009c0: 0000 7225 0000 0029 0672 1f00 0000 721d  ..r%...).r....r.
-000009d0: 0000 0072 2100 0000 7226 0000 0072 2700  ...r!...r&...r'.
-000009e0: 0000 7228 0000 00fa 0a68 756e 2f68 656e  ..r(.....hun/hen
-000009f0: 6465 73fa 0868 616e 2f68 616e 73da 0355  des..han/hans..U
-00000a00: 4e4b 2901 723a 0000 0029 0572 2c00 0000  NK).r:...).r,...
-00000a10: 5a0f 6665 6d61 6c65 5f70 726f 6e6f 756e  Z.female_pronoun
-00000a20: 735a 0d6d 616c 655f 7072 6f6e 6f75 6e73  sZ.male_pronouns
-00000a30: 5a0d 6772 6f75 705f 7072 6f6e 6f75 6e5a  Z.group_pronounZ
-00000a40: 0770 726f 6e6f 756e 7205 0000 0072 0500  .pronounr....r..
-00000a50: 0000 7209 0000 00da 0e67 726f 7570 5f70  ..r......group_p
-00000a60: 726f 6e6f 756e 734a 0000 0073 1400 0000  ronounsJ...s....
-00000a70: 0004 0801 0803 0403 0801 0801 0c01 0801  ................
-00000a80: 0c02 0c01 724b 0000 0063 0200 0000 0000  ....rK...c......
-00000a90: 0000 0000 0000 0300 0000 0800 0000 4300  ..............C.
-00000aa0: 0000 7322 0000 0074 00a0 0174 027c 007c  ..s"...t...t.|.|
-00000ab0: 0164 0164 0264 038d 04a1 016a 0364 0464  .d.d.d.....j.d.d
-00000ac0: 058d 017d 027c 0253 0029 067a bf43 7265  ...}.|.S.).z.Cre
-00000ad0: 6174 6520 616e 6420 7361 7665 2063 6c61  ate and save cla
-00000ae0: 7373 6966 6963 6174 696f 6e20 7265 706f  ssification repo
-00000af0: 7274 0a20 2020 2041 7267 733a 200a 2020  rt.    Args: .  
-00000b00: 2020 2020 2020 6c61 6265 6c73 3a20 6c61        labels: la
-00000b10: 6265 6c73 200a 2020 2020 2020 2020 7072  bels .        pr
-00000b20: 6564 6963 7469 6f6e 733a 206d 6f64 656c  edictions: model
-00000b30: 2070 7265 6469 6374 696f 6e73 0a20 2020   predictions.   
-00000b40: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00000b50: 2020 636c 665f 7265 706f 7274 3a20 636c    clf_report: cl
-00000b60: 6173 7369 6669 6361 7469 6f6e 2072 6570  assification rep
-00000b70: 6f72 7420 696e 2070 616e 6461 7320 6466  ort in pandas df
-00000b80: 2066 6f72 6d61 740a 2020 2020 54e9 0100   format.    T...
-00000b90: 0000 2902 da0b 6f75 7470 7574 5f64 6963  ..)...output_dic
-00000ba0: 74da 0d7a 6572 6f5f 6469 7669 7369 6f6e  t..zero_division
-00000bb0: e902 0000 0029 01da 0864 6563 696d 616c  .....)...decimal
-00000bc0: 7329 04da 0270 64da 0944 6174 6146 7261  s)...pd..DataFra
-00000bd0: 6d65 7203 0000 00da 0572 6f75 6e64 2903  mer......round).
-00000be0: 7241 0000 00da 0b70 7265 6469 6374 696f  rA.....predictio
-00000bf0: 6e73 da02 6466 7205 0000 0072 0500 0000  ns..dfr....r....
-00000c00: 7209 0000 00da 0e65 7661 6c75 6174 655f  r......evaluate_
-00000c10: 6d6f 6465 6c5e 0000 0073 0400 0000 0009  model^...s......
-00000c20: 1e01 7256 0000 0063 0400 0000 0000 0000  ..rV...c........
-00000c30: 0000 0000 1200 0000 0700 0000 4300 0000  ............C...
-00000c40: 7302 0100 0074 006a 01a0 0274 0374 0483  s....t.j...t.t..
-00000c50: 016a 0564 0119 0064 0264 03a1 037d 0474  .j.d...d.d...}.t
-00000c60: 006a 01a0 0274 0374 0483 016a 0564 0119  .j...t.t...j.d..
-00000c70: 0064 0264 04a1 037d 0574 067c 0583 017d  .d.d...}.t.|...}
-00000c80: 0674 067c 0483 017d 0774 077c 067c 017c  .t.|...}.t.|.|.|
-00000c90: 007c 027c 0364 058d 055c 027d 087d 0974  .|.|.d...\.}.}.t
-00000ca0: 077c 077c 017c 007c 027c 0364 058d 055c  .|.|.|.|.|.d...\
-00000cb0: 027d 0a7d 0b74 087c 0883 0174 087c 0983  .}.}.t.|...t.|..
-00000cc0: 0102 007d 0c7d 0d74 087c 0a83 0174 087c  ...}.}.t.|...t.|
-00000cd0: 0b83 0102 007d 0e7d 0f74 0964 067c 0383  .....}.}.t.d.|..
-00000ce0: 0201 0074 0964 0774 0a64 0864 0984 007c  ...t.d.t.d.d...|
-00000cf0: 0d44 0083 0183 0183 0201 0074 0964 0a74  .D.........t.d.t
-00000d00: 0a64 0b64 0984 007c 0d44 0083 0183 0183  .d.d...|.D......
-00000d10: 0201 0074 0964 0c74 0a64 0d64 0984 007c  ...t.d.t.d.d...|
-00000d20: 0d44 0083 0183 0183 0201 0074 0b7c 0c7c  .D.........t.|.|
-00000d30: 0d83 027d 1074 0b7c 0e7c 0f83 027d 117c  ...}.t.|.|...}.|
-00000d40: 107c 1166 0253 0029 0e4e 724c 0000 00da  .|.f.S.).NrL....
-00000d50: 0464 6174 617a 2544 6157 696e 6f42 6961  .dataz%DaWinoBia
-00000d60: 735f 7072 6f5f 7374 6572 656f 7479 7065  s_pro_stereotype
-00000d70: 645f 6576 616c 6461 2e74 7874 7a26 4461  d_evalda.txtz&Da
-00000d80: 5769 6e6f 4269 6173 5f61 6e74 695f 7374  WinoBias_anti_st
-00000d90: 6572 656f 7479 7065 645f 6576 616c 6461  ereotyped_evalda
-00000da0: 2e74 7874 2905 7214 0000 0072 3d00 0000  .txt).r....r=...
-00000db0: 723e 0000 0072 3f00 0000 7240 0000 007a  r>...r?...r@...z
-00000dc0: 066d 6f64 656c 3a7a 234e 756d 6265 7220  .model:z#Number 
-00000dd0: 6f66 2066 656d 616c 6520 7072 6f6e 2e20  of female pron. 
-00000de0: 7072 6564 6963 7469 6f6e 733a 6301 0000  predictions:c...
-00000df0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000e00: 0053 0000 0073 1800 0000 6700 7c00 5d10  .S...s....g.|.].
-00000e10: 7d01 7c01 6400 6b02 7204 7c01 9102 7104  }.|.d.k.r.|...q.
-00000e20: 5300 2901 7248 0000 0072 0500 0000 722a  S.).rH...r....r*
-00000e30: 0000 0072 0500 0000 7205 0000 0072 0900  ...r....r....r..
-00000e40: 0000 720a 0000 007d 0000 0072 0b00 0000  ..r....}...r....
-00000e50: 7a20 7275 6e5f 7769 6e6f 6269 6173 2e3c  z run_winobias.<
-00000e60: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000e70: 703e 7a21 4e75 6d62 6572 206f 6620 6d61  p>z!Number of ma
-00000e80: 6c65 2070 726f 6e2e 2070 7265 6469 6374  le pron. predict
-00000e90: 696f 6e73 3a63 0100 0000 0000 0000 0000  ions:c..........
-00000ea0: 0000 0200 0000 0400 0000 5300 0000 7318  ..........S...s.
-00000eb0: 0000 0067 007c 005d 107d 017c 0164 006b  ...g.|.].}.|.d.k
-00000ec0: 0272 047c 0191 0271 0453 0029 0172 4900  .r.|...q.S.).rI.
-00000ed0: 0000 7205 0000 0072 2a00 0000 7205 0000  ..r....r*...r...
-00000ee0: 0072 0500 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00000ef0: 7e00 0000 720b 0000 007a 204e 756d 6265  ~...r....z Numbe
-00000f00: 7220 6f66 2027 554e 4b4e 4f57 4e27 2070  r of 'UNKNOWN' p
-00000f10: 7265 6469 6374 696f 6e73 3a63 0100 0000  redictions:c....
-00000f20: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000f30: 5300 0000 7318 0000 0067 007c 005d 107d  S...s....g.|.].}
-00000f40: 017c 0164 006b 0272 047c 0191 0271 0453  .|.d.k.r.|...q.S
-00000f50: 0029 0172 4a00 0000 7205 0000 0072 2a00  .).rJ...r....r*.
-00000f60: 0000 7205 0000 0072 0500 0000 7209 0000  ..r....r....r...
-00000f70: 0072 0a00 0000 7f00 0000 720b 0000 0029  .r........r....)
-00000f80: 0cda 026f 73da 0470 6174 6872 3800 0000  ...os..pathr8...
-00000f90: 7204 0000 00da 085f 5f66 696c 655f 5fda  r......__file__.
-00000fa0: 0770 6172 656e 7473 7215 0000 0072 4700  .parentsr....rG.
-00000fb0: 0000 724b 0000 00da 0570 7269 6e74 7235  ..rK.....printr5
-00000fc0: 0000 0072 5600 0000 2912 723e 0000 0072  ...rV...).r>...r
-00000fd0: 3d00 0000 723f 0000 0072 4000 0000 5a0a  =...r?...r@...Z.
-00000fe0: 696e 7061 7468 5f70 726f 5a0b 696e 7061  inpath_proZ.inpa
-00000ff0: 7468 5f61 6e74 695a 0a61 6e74 695f 7365  th_antiZ.anti_se
-00001000: 6e74 735a 0970 726f 5f73 656e 7473 5a0c  ntsZ.pro_sentsZ.
-00001010: 616e 7469 5f6c 6162 656c 735f 5a0b 616e  anti_labels_Z.an
-00001020: 7469 5f70 7265 6473 5f5a 0b70 726f 5f6c  ti_preds_Z.pro_l
-00001030: 6162 656c 735f 5a0a 7072 6f5f 7072 6564  abels_Z.pro_pred
-00001040: 735f 5a0b 616e 7469 5f6c 6162 656c 735a  s_Z.anti_labelsZ
-00001050: 0a61 6e74 695f 7072 6564 735a 0a70 726f  .anti_predsZ.pro
-00001060: 5f6c 6162 656c 735a 0970 726f 5f70 7265  _labelsZ.pro_pre
-00001070: 6473 da0c 636c 665f 7265 705f 616e 7469  ds..clf_rep_anti
-00001080: da0b 636c 665f 7265 705f 7072 6f72 0500  ..clf_rep_pror..
-00001090: 0000 7205 0000 0072 0900 0000 da0c 7275  ..r....r......ru
-000010a0: 6e5f 7769 6e6f 6269 6173 6b00 0000 731e  n_winobiask...s.
-000010b0: 0000 0000 021a 011a 0308 0108 0316 0116  ................
-000010c0: 0312 0112 010a 0218 0118 0118 030a 010a  ................
-000010d0: 0272 5f00 0000 a902 da01 78da 0179 6302  .r_.......x..yc.
-000010e0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-000010f0: 0000 0043 0000 0073 1400 0000 7400 7401  ...C...s....t.t.
-00001100: a002 7c00 7c01 1b00 a101 6401 8302 5300  ..|.|.....d...S.
-00001110: 2902 4e72 4f00 0000 2903 7253 0000 00da  ).NrO...).rS....
-00001120: 046d 6174 68da 046c 6f67 3272 6000 0000  .math..log2r`...
-00001130: 7205 0000 0072 0500 0000 7209 0000 00da  r....r....r.....
-00001140: 086c 6f67 7261 7469 6f87 0000 0073 0200  .logratio....s..
-00001150: 0000 0001 7265 0000 0063 0300 0000 0000  ....re...c......
-00001160: 0000 0000 0000 0f00 0000 0f00 0000 4300  ..............C.
-00001170: 0000 7326 0100 007c 0064 0119 006a 0064  ..s&...|.d...j.d
-00001180: 0219 007d 037c 0164 0119 006a 0064 0219  ...}.|.d...j.d..
-00001190: 007d 0474 017c 047c 0383 027d 057c 0064  .}.t.|.|...}.|.d
-000011a0: 0319 006a 0064 0419 007d 067c 0064 0519  ...j.d...}.|.d..
-000011b0: 006a 0064 0419 007d 077c 0164 0319 006a  .j.d...}.|.d...j
-000011c0: 0064 0419 007d 087c 0164 0519 006a 0064  .d...}.|.d...j.d
-000011d0: 0419 007d 0964 067c 029b 009d 0264 0764  ...}.d.|.....d.d
-000011e0: 0867 0264 0964 077c 0567 0264 0a64 0b64  .g.d.d.|.g.d.d.d
-000011f0: 0c67 0264 0d7c 037c 0467 0269 047d 0a74  .g.d.|.|.g.i.}.t
-00001200: 02a0 037c 0aa1 016a 047d 0a7c 0a6a 0564  ...|...j.}.|.j.d
-00001210: 0219 007c 0a5f 067c 0a6a 0564 0e64 0f85  ...|._.|.j.d.d..
-00001220: 0219 007d 0b64 107c 029b 009d 0267 0064  ...}.d.|.....g.d
-00001230: 11a2 0164 0964 077c 0564 0764 0767 0464  ...d.d.|.d.d.g.d
-00001240: 0a67 0064 12a2 0164 0d7c 0364 077c 0464  .g.d...d.|.d.|.d
-00001250: 0767 0464 1367 0064 14a2 0164 157c 067c  .g.d.g.d...d.|.|
-00001260: 077c 087c 0967 0469 067d 0c74 02a0 037c  .|.|.g.i.}.t...|
-00001270: 0ca1 016a 047d 0c7c 0c6a 0564 0219 007c  ...j.}.|.j.d...|
-00001280: 0c5f 067c 0c6a 0564 0e64 0f85 0219 007d  ._.|.j.d.d.....}
-00001290: 0d7c 0b7c 0d67 027d 0e7c 0e53 0029 167a  .|.|.g.}.|.S.).z
-000012a0: ae45 7661 6c75 6174 6520 7769 6e6f 6269  .Evaluate winobi
-000012b0: 6173 2063 6f72 6566 2065 7870 6572 696d  as coref experim
-000012c0: 656e 740a 2020 2020 4172 6773 3a0a 2020  ent.    Args:.  
-000012d0: 2020 2020 2020 616e 7469 5f72 6573 3a20        anti_res: 
-000012e0: 7265 7375 6c74 7320 666f 7220 616e 7469  results for anti
-000012f0: 2d73 7465 7265 6f74 7970 6963 616c 2063  -stereotypical c
-00001300: 6f6e 6469 7469 6f6e 0a20 2020 2020 2020  ondition.       
-00001310: 2070 726f 5f72 6573 3a20 7265 7375 6c74   pro_res: result
-00001320: 7320 666f 7220 7072 6f2d 7374 6572 656f  s for pro-stereo
-00001330: 7479 7069 6361 6c20 636f 6e64 6974 696f  typical conditio
-00001340: 6e0a 2020 2020 2020 2020 0a20 2020 20da  n.        .    .
-00001350: 0861 6363 7572 6163 7972 0100 0000 7248  .accuracyr....rH
-00001360: 0000 0072 4f00 0000 7249 0000 007a 1253  ...rO...rI...z.S
-00001370: 696d 706c 6520 4f75 7470 7574 2066 6f72  imple Output for
-00001380: 20da 00da 0a44 6157 696e 6f42 6961 737a   ....DaWinoBiasz
-00001390: 1247 656e 6465 7220 4566 6665 6374 2053  .Gender Effect S
-000013a0: 697a 65da 0943 6f6e 6469 7469 6f6e fa12  ize..Condition..
-000013b0: 416e 7469 2d73 7465 7265 6f74 7970 6963  Anti-stereotypic
-000013c0: 616c fa11 5072 6f2d 7374 6572 656f 7479  al..Pro-stereoty
-000013d0: 7069 6361 6cda 0841 6363 7572 6163 7972  pical..Accuracyr
-000013e0: 4c00 0000 4e7a 1444 6574 6169 6c65 6420  L...Nz.Detailed 
-000013f0: 4f75 7470 7574 2066 6f72 2029 0472 6700  Output for ).rg.
-00001400: 0000 7268 0000 0072 6700 0000 7267 0000  ..rh...rg...rg..
-00001410: 0029 0472 6a00 0000 7267 0000 0072 6b00  .).rj...rg...rk.
-00001420: 0000 7267 0000 005a 0850 726f 6e6f 756e  ..rg...Z.Pronoun
-00001430: 7329 04da 0646 656d 616c 65da 044d 616c  s)...Female..Mal
-00001440: 6572 6d00 0000 726e 0000 00da 0246 3129  erm...rn.....F1)
-00001450: 07da 0676 616c 7565 7372 6500 0000 7251  ...valuesre...rQ
-00001460: 0000 0072 5200 0000 da01 54da 0469 6c6f  ...rR.....T..ilo
-00001470: 63da 0763 6f6c 756d 6e73 290f da08 616e  c..columns)...an
-00001480: 7469 5f72 6573 da07 7072 6f5f 7265 7372  ti_res..pro_resr
-00001490: 4000 0000 5a08 616e 7469 5f61 6363 5a07  @...Z.anti_accZ.
-000014a0: 7072 6f5f 6163 635a 1267 656e 6465 725f  pro_accZ.gender_
-000014b0: 6566 6665 6374 5f73 697a 655a 1061 6e74  effect_sizeZ.ant
-000014c0: 695f 6631 5f66 656d 5f70 726f 6e5a 1161  i_f1_fem_pronZ.a
-000014d0: 6e74 695f 6631 5f6d 616c 655f 7072 6f6e  nti_f1_male_pron
-000014e0: 5a0f 7072 6f5f 6631 5f66 656d 5f70 726f  Z.pro_f1_fem_pro
-000014f0: 6e5a 1070 726f 5f66 315f 6d61 6c65 5f70  nZ.pro_f1_male_p
-00001500: 726f 6e5a 0b73 696d 6c70 655f 6461 7461  ronZ.simlpe_data
-00001510: 5a09 7369 6d70 6c65 5f64 665a 0d64 6574  Z.simple_dfZ.det
-00001520: 6169 6c65 645f 6461 7461 5a0b 6465 7461  ailed_dataZ.deta
-00001530: 696c 6564 5f64 66da 0772 6573 756c 7473  iled_df..results
-00001540: 7205 0000 0072 0500 0000 7209 0000 00da  r....r....r.....
-00001550: 1465 7661 6c75 6174 655f 6c6d 5f77 696e  .evaluate_lm_win
-00001560: 6f62 6961 738a 0000 0073 3600 0000 0008  obias....s6.....
-00001570: 0e01 0e01 0a02 0e01 0e02 0e01 0e03 0e01  ................
-00001580: 0801 0801 08fc 0407 0c03 0c03 0e03 0e01  ................
-00001590: 0c01 0801 0c01 0801 0cfa 0409 0c03 0c03  ................
-000015a0: 0e02 0802 7277 0000 0029 18da 0574 6f72  ....rw...)...tor
-000015b0: 6368 7258 0000 00da 0573 7061 6379 720f  chrX.....spacyr.
-000015c0: 0000 00da 0b63 6f6c 6c65 6374 696f 6e73  .....collections
-000015d0: 7202 0000 00da 0f73 6b6c 6561 726e 2e6d  r......sklearn.m
-000015e0: 6574 7269 6373 7203 0000 00da 0670 616e  etricsr......pan
-000015f0: 6461 7372 5100 0000 da07 7061 7468 6c69  dasrQ.....pathli
-00001600: 6272 0400 0000 7263 0000 0072 3300 0000  br....rc...r3...
-00001610: 7215 0000 0072 1c00 0000 722e 0000 0072  r....r....r....r
-00001620: 4700 0000 724b 0000 0072 5600 0000 725f  G...rK...rV...r_
-00001630: 0000 00da 0566 6c6f 6174 7265 0000 0072  .....floatre...r
-00001640: 7700 0000 7205 0000 0072 0500 0000 7205  w...r....r....r.
-00001650: 0000 0072 0900 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001660: 653e 0100 0000 7320 0000 0020 010c 0110  e>....s ... ....
-00001670: 010c 0108 010c 0108 0108 0208 0908 0408  ................
-00001680: 0908 2a08 1408 0d08 1c10 03              ..*........
+00000130: 0000 0009 0000 0043 0000 0073 3c00 0000  .......C...s<...
+00000140: 7400 7c00 8301 8f12 7d01 7c01 a001 a100  t.|.....}.|.....
+00000150: a002 a100 7d02 5700 3500 5100 5200 5800  ....}.W.5.Q.R.X.
+00000160: 6401 6402 8400 7c02 4400 8301 7d03 7403  d.d...|.D...}.t.
+00000170: a004 7c03 a101 0100 7c03 5300 2903 7a2e  ..|.....|.S.).z.
+00000180: 6c6f 6164 2044 6157 696e 6f42 6961 7320  load DaWinoBias 
+00000190: 7465 7874 7320 2d20 616e 6420 7368 7566  texts - and shuf
+000001a0: 666c 6520 6461 7461 200a 2020 2020 6301  fle data .    c.
+000001b0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000001c0: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+000001d0: 5d0c 7d01 7c01 a000 a100 9102 7104 5300  ].}.|.......q.S.
+000001e0: a900 2901 da05 7374 7269 7029 02da 022e  ..)...strip)....
+000001f0: 30da 046c 696e 6572 0500 0000 7205 0000  0..liner....r...
+00000200: 00fa 7e2f 5573 6572 732f 6173 7472 6964  ..~/Users/astrid
+00000210: 7279 626e 6572 2f44 6f63 756d 656e 7473  rybner/Documents
+00000220: 2f63 6f6f 6c2d 7072 6f67 7261 6d6d 6572  /cool-programmer
+00000230: 2d74 6865 7369 732f 6576 616c 6461 2d70  -thesis/evalda-p
+00000240: 7562 322f 6576 616c 6461 2d70 7562 322f  ub2/evalda-pub2/
+00000250: 6576 616c 6461 5f70 7562 322f 6261 7365  evalda_pub2/base
+00000260: 5f74 6173 6b73 2f77 696e 6f5f 6669 6c6c  _tasks/wino_fill
+00000270: 6d61 736b 5f75 7469 6c69 7469 6573 2e70  mask_utilities.p
+00000280: 79da 0a3c 6c69 7374 636f 6d70 3e0f 0000  y..<listcomp>...
+00000290: 0073 0400 0000 0600 0200 7a1e 6c6f 6164  .s........z.load
+000002a0: 5f74 6578 7473 2e3c 6c6f 6361 6c73 3e2e  _texts.<locals>.
+000002b0: 3c6c 6973 7463 6f6d 703e 2905 da04 6f70  <listcomp>)...op
+000002c0: 656e da04 7265 6164 da0a 7370 6c69 746c  en..read..splitl
+000002d0: 696e 6573 da06 7261 6e64 6f6d da07 7368  ines..random..sh
+000002e0: 7566 666c 6529 04da 0866 696c 6570 6174  uffle)...filepat
+000002f0: 68da 0466 696c 65da 0474 6578 74da 056c  h..file..text..l
+00000300: 696e 6573 7205 0000 0072 0500 0000 7209  inesr....r....r.
+00000310: 0000 00da 0a6c 6f61 645f 7465 7874 730a  .....load_texts.
+00000320: 0000 0073 0a00 0000 0003 0a01 1601 0e01  ...s............
+00000330: 0a01 7214 0000 0063 0100 0000 0000 0000  ..r....c........
+00000340: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000350: 7310 0000 0064 0164 0284 007c 0044 0083  s....d.d...|.D..
+00000360: 0167 0153 0029 034e 6301 0000 0000 0000  .g.S.).Nc.......
+00000370: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00000380: 0073 2000 0000 6700 7c00 5d18 7d01 7c01  .s ...g.|.].}.|.
+00000390: 6400 6b03 7204 7c01 6401 6b03 7204 7c01  d.k.r.|.d.k.r.|.
+000003a0: 9102 7104 5300 2902 fa01 5bfa 015d 7205  ..q.S.)...[..]r.
+000003b0: 0000 00a9 0272 0700 0000 da05 746f 6b65  .....r......toke
+000003c0: 6e72 0500 0000 7205 0000 0072 0900 0000  nr....r....r....
+000003d0: 720a 0000 0015 0000 0073 0800 0000 0600  r........s......
+000003e0: 0200 0800 0800 7a20 7265 6d6f 7665 5f73  ......z remove_s
+000003f0: 715f 6272 2e3c 6c6f 6361 6c73 3e2e 3c6c  q_br.<locals>.<l
+00000400: 6973 7463 6f6d 703e 7205 0000 00a9 01da  istcomp>r.......
+00000410: 0674 6f6b 656e 7372 0500 0000 7205 0000  .tokensr....r...
+00000420: 0072 0900 0000 da0c 7265 6d6f 7665 5f73  .r......remove_s
+00000430: 715f 6272 1300 0000 7302 0000 0000 0272  q_br....s......r
+00000440: 1b00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000450: 0003 0000 000c 0000 0003 0000 0073 3600  .............s6.
+00000460: 0000 6401 6402 6403 6404 6405 6406 6407  ..d.d.d.d.d.d.d.
+00000470: 6408 6409 640a 640b 640c 670c 7d01 8700  d.d.d.d.d.g.}...
+00000480: 6601 640d 640e 8408 7c01 4400 8301 640f  f.d.d...|.D...d.
+00000490: 1900 7d02 7c02 5300 2910 7a25 4765 7420  ..}.|.S.).z%Get 
+000004a0: 696e 6465 7820 6f66 2070 726f 6e6f 756e  index of pronoun
+000004b0: 2069 6e20 7365 6e74 656e 6365 0a20 2020   in sentence.   
+000004c0: 20da 0468 616e 73da 0668 656e 6465 73da   ..hans..hendes.
+000004d0: 0368 616e da03 6875 6eda 0368 616d da05  .han..hun..ham..
+000004e0: 6865 6e64 65f5 0600 0000 e296 8168 756e  hende........hun
+000004f0: f509 0000 00e2 9681 6865 6e64 6573 f508  ........hendes..
+00000500: 0000 00e2 9681 6865 6e64 65f5 0600 0000  ......hende.....
+00000510: e296 8168 616e f507 0000 00e2 9681 6861  ...han........ha
+00000520: 6e73 f506 0000 00e2 9681 6861 6d63 0100  ns........hamc..
+00000530: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00000540: 0000 1300 0000 731e 0000 0067 007c 005d  ......s....g.|.]
+00000550: 167d 017c 0188 006b 0672 0488 00a0 007c  .}.|...k.r.....|
+00000560: 01a1 0191 0271 0453 0072 0500 0000 2901  .....q.S.r....).
+00000570: da05 696e 6465 78a9 0272 0700 0000 da01  ..index..r......
+00000580: 6972 1900 0000 7205 0000 0072 0900 0000  ir....r....r....
+00000590: 720a 0000 001d 0000 0073 0600 0000 0600  r........s......
+000005a0: 0200 0800 7a1c 6964 785f 7072 6f6e 2e3c  ....z.idx_pron.<
+000005b0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+000005c0: 703e 7201 0000 0072 0500 0000 2903 721a  p>r....r....).r.
+000005d0: 0000 00da 0870 726f 6e6f 756e 73da 0970  .....pronouns..p
+000005e0: 726f 6e73 5f69 6478 7205 0000 0072 1900  rons_idxr....r..
+000005f0: 0000 7209 0000 00da 0869 6478 5f70 726f  ..r......idx_pro
+00000600: 6e17 0000 0073 0600 0000 0004 1c02 1601  n....s..........
+00000610: 722d 0000 0063 0500 0000 0000 0000 0000  r-...c..........
+00000620: 0000 1000 0000 0500 0000 4300 0000 73d6  ..........C...s.
+00000630: 0000 0067 0067 0002 007d 057d 0674 006a  ...g.g...}.}.t.j
+00000640: 0174 027c 0083 0164 018d 01a0 03a1 007d  .t.|...d.......}
+00000650: 0774 047c 0083 0144 005d 9e5c 027d 087d  .t.|...D.].\.}.}
+00000660: 097c 027c 0983 017d 0a64 0264 0384 007c  .|.|...}.d.d...|
+00000670: 0a44 0083 017d 0b74 057c 0b83 0164 0419  .D...}.t.|...d..
+00000680: 007d 0b74 067c 0b83 017d 0c7c 0b7c 0c19  .}.t.|...}.|.|..
+00000690: 007d 0d7c 037c 0b7c 0c3c 007c 0364 056b  .}.|.|.|.<.|.d.k
+000006a0: 0272 8c7c 0464 066b 0272 8c64 07a0 077c  .r.|.d.k.r.d...|
+000006b0: 0ba1 01a0 0864 0864 05a1 027d 0e6e 0a64  .....d.d...}.n.d
+000006c0: 07a0 077c 0ba1 017d 0e7c 017c 0e83 0164  ...|...}.|.|...d
+000006d0: 0419 0064 0919 007d 0f7c 05a0 097c 0da1  ...d...}.|...|..
+000006e0: 0101 007c 06a0 097c 0fa1 0101 007c 07a0  ...|...|.....|..
+000006f0: 0a7c 08a1 0101 0071 267c 07a0 0ba1 0001  .|.....q&|......
+00000700: 007c 057c 0666 0253 0029 0a4e 2901 da06  .|.|.f.S.).N)...
+00000710: 6d61 7876 616c 6301 0000 0000 0000 0000  maxvalc.........
+00000720: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00000730: 1600 0000 6700 7c00 5d0e 7d01 7c01 6a00  ....g.|.].}.|.j.
+00000740: a001 a100 9102 7104 5300 7205 0000 0029  ......q.S.r....)
+00000750: 0272 1200 0000 da05 6c6f 7765 7272 1700  .r......lowerr..
+00000760: 0000 7205 0000 0072 0500 0000 7209 0000  ..r....r....r...
+00000770: 0072 0a00 0000 2900 0000 7304 0000 0006  .r....)...s.....
+00000780: 0002 007a 2270 7265 6469 6374 5f6d 6173  ...z"predict_mas
+00000790: 6b65 642e 3c6c 6f63 616c 733e 2e3c 6c69  ked.<locals>.<li
+000007a0: 7374 636f 6d70 3e72 0100 0000 7a06 3c6d  stcomp>r....z.<m
+000007b0: 6173 6b3e 7a12 7665 7374 6569 6e6e 2f44  ask>z.vesteinn/D
+000007c0: 616e 736b 4265 7274 da01 207a 0720 3c6d  anskBert.. z. <m
+000007d0: 6173 6b3e da09 746f 6b65 6e5f 7374 7229  ask>..token_str)
+000007e0: 0cda 0b70 726f 6772 6573 7362 6172 da0b  ...progressbar..
+000007f0: 5072 6f67 7265 7373 4261 72da 036c 656e  ProgressBar..len
+00000800: da05 7374 6172 74da 0965 6e75 6d65 7261  ..start..enumera
+00000810: 7465 721b 0000 0072 2d00 0000 da04 6a6f  ter....r-.....jo
+00000820: 696e da07 7265 706c 6163 65da 0661 7070  in..replace..app
+00000830: 656e 64da 0675 7064 6174 65da 0666 696e  end..update..fin
+00000840: 6973 6829 1072 1300 0000 da03 6e6c 70da  ish).r......nlp.
+00000850: 0974 6f6b 656e 697a 6572 da0a 6d61 736b  .tokenizer..mask
+00000860: 5f74 6f6b 656e da0a 6d6f 6465 6c5f 6e61  _token..model_na
+00000870: 6d65 da06 6c61 6265 6c73 da05 7072 6564  me..labels..pred
+00000880: 73da 0362 6172 da03 6964 7872 0800 0000  s..bar..idxr....
+00000890: 5a0e 6c69 6e65 5f74 6f6b 656e 697a 6564  Z.line_tokenized
+000008a0: 721a 0000 0072 2c00 0000 5a0f 636f 7272  r....r,...Z.corr
+000008b0: 6563 745f 7072 6f6e 6f75 6eda 0873 656e  ect_pronoun..sen
+000008c0: 7465 6e63 65da 0470 7265 6472 0500 0000  tence..predr....
+000008d0: 7205 0000 0072 0900 0000 da0e 7072 6564  r....r......pred
+000008e0: 6963 745f 6d61 736b 6564 2000 0000 7324  ict_masked ...s$
+000008f0: 0000 0000 010a 0314 0210 0208 010e 030c  ................
+00000900: 0308 0308 0308 0410 0114 020a 0310 030a  ................
+00000910: 010a 020c 0108 0272 4600 0000 6301 0000  .......rF...c...
+00000920: 0000 0000 0000 0000 0005 0000 0006 0000  ................
+00000930: 0043 0000 0073 6400 0000 6401 6402 6403  .C...sd...d.d.d.
+00000940: 6404 6405 6406 6706 7d01 6407 6408 6409  d.d.d.g.}.d.d.d.
+00000950: 640a 640b 640c 6706 7d02 6700 7d03 7c00  d.d.d.g.}.g.}.|.
+00000960: 4400 5d36 7d04 7c04 7c01 6b06 7240 7c03  D.]6}.|.|.k.r@|.
+00000970: a000 640d a101 0100 7128 7c04 7c02 6b06  ..d.....q(|.|.k.
+00000980: 7254 7c03 a000 640e a101 0100 7128 7c03  rT|...d.....q(|.
+00000990: a000 640f a101 0100 7128 7c03 5300 2910  ..d.....q(|.S.).
+000009a0: 7a28 6772 6f75 7020 6c61 6265 6c73 2069  z(group labels i
+000009b0: 6e20 6665 6d61 6c65 2061 6e64 206d 616c  n female and mal
+000009c0: 6520 7072 6f6e 6f75 6e73 721f 0000 0072  e pronounsr....r
+000009d0: 1d00 0000 7221 0000 0072 2200 0000 7223  ....r!...r"...r#
+000009e0: 0000 0072 2400 0000 721e 0000 0072 1c00  ...r$...r....r..
+000009f0: 0000 7220 0000 0072 2500 0000 7226 0000  ..r ...r%...r&..
+00000a00: 0072 2700 0000 fa0a 6875 6e2f 6865 6e64  .r'.....hun/hend
+00000a10: 6573 fa08 6861 6e2f 6861 6e73 da03 554e  es..han/hans..UN
+00000a20: 4b29 0172 3900 0000 2905 722b 0000 005a  K).r9...).r+...Z
+00000a30: 0f66 656d 616c 655f 7072 6f6e 6f75 6e73  .female_pronouns
+00000a40: 5a0d 6d61 6c65 5f70 726f 6e6f 756e 735a  Z.male_pronounsZ
+00000a50: 0d67 726f 7570 5f70 726f 6e6f 756e 5a07  .group_pronounZ.
+00000a60: 7072 6f6e 6f75 6e72 0500 0000 7205 0000  pronounr....r...
+00000a70: 0072 0900 0000 da0e 6772 6f75 705f 7072  .r......group_pr
+00000a80: 6f6e 6f75 6e73 4a00 0000 7314 0000 0000  onounsJ...s.....
+00000a90: 0410 0110 0304 0308 0108 010c 0108 010c  ................
+00000aa0: 020c 0172 4a00 0000 6302 0000 0000 0000  ...rJ...c.......
+00000ab0: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
+00000ac0: 0073 2200 0000 7400 a001 7402 7c00 7c01  .s"...t...t.|.|.
+00000ad0: 6401 6402 6403 8d04 a101 6a03 6404 6405  d.d.d.....j.d.d.
+00000ae0: 8d01 7d02 7c02 5300 2906 7abf 4372 6561  ..}.|.S.).z.Crea
+00000af0: 7465 2061 6e64 2073 6176 6520 636c 6173  te and save clas
+00000b00: 7369 6669 6361 7469 6f6e 2072 6570 6f72  sification repor
+00000b10: 740a 2020 2020 4172 6773 3a20 0a20 2020  t.    Args: .   
+00000b20: 2020 2020 206c 6162 656c 733a 206c 6162       labels: lab
+00000b30: 656c 7320 0a20 2020 2020 2020 2070 7265  els .        pre
+00000b40: 6469 6374 696f 6e73 3a20 6d6f 6465 6c20  dictions: model 
+00000b50: 7072 6564 6963 7469 6f6e 730a 2020 2020  predictions.    
+00000b60: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00000b70: 2063 6c66 5f72 6570 6f72 743a 2063 6c61   clf_report: cla
+00000b80: 7373 6966 6963 6174 696f 6e20 7265 706f  ssification repo
+00000b90: 7274 2069 6e20 7061 6e64 6173 2064 6620  rt in pandas df 
+00000ba0: 666f 726d 6174 0a20 2020 2054 e901 0000  format.    T....
+00000bb0: 0029 02da 0b6f 7574 7075 745f 6469 6374  .)...output_dict
+00000bc0: da0d 7a65 726f 5f64 6976 6973 696f 6ee9  ..zero_division.
+00000bd0: 0200 0000 2901 da08 6465 6369 6d61 6c73  ....)...decimals
+00000be0: 2904 da02 7064 da09 4461 7461 4672 616d  )...pd..DataFram
+00000bf0: 6572 0300 0000 da05 726f 756e 6429 0372  er......round).r
+00000c00: 4000 0000 da0b 7072 6564 6963 7469 6f6e  @.....prediction
+00000c10: 73da 0264 6672 0500 0000 7205 0000 0072  s..dfr....r....r
+00000c20: 0900 0000 da0e 6576 616c 7561 7465 5f6d  ......evaluate_m
+00000c30: 6f64 656c 5e00 0000 7304 0000 0000 091e  odel^...s.......
+00000c40: 0172 5500 0000 6304 0000 0000 0000 0000  .rU...c.........
+00000c50: 0000 0012 0000 0007 0000 0043 0000 0073  ...........C...s
+00000c60: 0201 0000 7400 6a01 a002 7403 7404 8301  ....t.j...t.t...
+00000c70: 6a05 6401 1900 6402 6403 a103 7d04 7400  j.d...d.d...}.t.
+00000c80: 6a01 a002 7403 7404 8301 6a05 6401 1900  j...t.t...j.d...
+00000c90: 6402 6404 a103 7d05 7406 7c05 8301 7d06  d.d...}.t.|...}.
+00000ca0: 7406 7c04 8301 7d07 7407 7c06 7c01 7c00  t.|...}.t.|.|.|.
+00000cb0: 7c02 7c03 6405 8d05 5c02 7d08 7d09 7407  |.|.d...\.}.}.t.
+00000cc0: 7c07 7c01 7c00 7c02 7c03 6405 8d05 5c02  |.|.|.|.|.d...\.
+00000cd0: 7d0a 7d0b 7408 7c08 8301 7408 7c09 8301  }.}.t.|...t.|...
+00000ce0: 0200 7d0c 7d0d 7408 7c0a 8301 7408 7c0b  ..}.}.t.|...t.|.
+00000cf0: 8301 0200 7d0e 7d0f 7409 6406 7c03 8302  ....}.}.t.d.|...
+00000d00: 0100 7409 6407 740a 6408 6409 8400 7c0d  ..t.d.t.d.d...|.
+00000d10: 4400 8301 8301 8302 0100 7409 640a 740a  D.........t.d.t.
+00000d20: 640b 6409 8400 7c0d 4400 8301 8301 8302  d.d...|.D.......
+00000d30: 0100 7409 640c 740a 640d 6409 8400 7c0d  ..t.d.t.d.d...|.
+00000d40: 4400 8301 8301 8302 0100 740b 7c0c 7c0d  D.........t.|.|.
+00000d50: 8302 7d10 740b 7c0e 7c0f 8302 7d11 7c10  ..}.t.|.|...}.|.
+00000d60: 7c11 6602 5300 290e 4e72 4b00 0000 da04  |.f.S.).NrK.....
+00000d70: 6461 7461 7a25 4461 5769 6e6f 4269 6173  dataz%DaWinoBias
+00000d80: 5f70 726f 5f73 7465 7265 6f74 7970 6564  _pro_stereotyped
+00000d90: 5f65 7661 6c64 612e 7478 747a 2644 6157  _evalda.txtz&DaW
+00000da0: 696e 6f42 6961 735f 616e 7469 5f73 7465  inoBias_anti_ste
+00000db0: 7265 6f74 7970 6564 5f65 7661 6c64 612e  reotyped_evalda.
+00000dc0: 7478 7429 0572 1300 0000 723c 0000 0072  txt).r....r<...r
+00000dd0: 3d00 0000 723e 0000 0072 3f00 0000 7a06  =...r>...r?...z.
+00000de0: 6d6f 6465 6c3a 7a23 4e75 6d62 6572 206f  model:z#Number o
+00000df0: 6620 6665 6d61 6c65 2070 726f 6e2e 2070  f female pron. p
+00000e00: 7265 6469 6374 696f 6e73 3a63 0100 0000  redictions:c....
+00000e10: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000e20: 5300 0000 7318 0000 0067 007c 005d 107d  S...s....g.|.].}
+00000e30: 017c 0164 006b 0272 047c 0191 0271 0453  .|.d.k.r.|...q.S
+00000e40: 0029 0172 4700 0000 7205 0000 0072 2900  .).rG...r....r).
+00000e50: 0000 7205 0000 0072 0500 0000 7209 0000  ..r....r....r...
+00000e60: 0072 0a00 0000 7d00 0000 7306 0000 0006  .r....}...s.....
+00000e70: 0002 0008 007a 2072 756e 5f77 696e 6f62  .....z run_winob
+00000e80: 6961 732e 3c6c 6f63 616c 733e 2e3c 6c69  ias.<locals>.<li
+00000e90: 7374 636f 6d70 3e7a 214e 756d 6265 7220  stcomp>z!Number 
+00000ea0: 6f66 206d 616c 6520 7072 6f6e 2e20 7072  of male pron. pr
+00000eb0: 6564 6963 7469 6f6e 733a 6301 0000 0000  edictions:c.....
+00000ec0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00000ed0: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
+00000ee0: 7c01 6400 6b02 7204 7c01 9102 7104 5300  |.d.k.r.|...q.S.
+00000ef0: 2901 7248 0000 0072 0500 0000 7229 0000  ).rH...r....r)..
+00000f00: 0072 0500 0000 7205 0000 0072 0900 0000  .r....r....r....
+00000f10: 720a 0000 007e 0000 0073 0600 0000 0600  r....~...s......
+00000f20: 0200 0800 7a20 4e75 6d62 6572 206f 6620  ....z Number of 
+00000f30: 2755 4e4b 4e4f 574e 2720 7072 6564 6963  'UNKNOWN' predic
+00000f40: 7469 6f6e 733a 6301 0000 0000 0000 0000  tions:c.........
+00000f50: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00000f60: 1800 0000 6700 7c00 5d10 7d01 7c01 6400  ....g.|.].}.|.d.
+00000f70: 6b02 7204 7c01 9102 7104 5300 2901 7249  k.r.|...q.S.).rI
+00000f80: 0000 0072 0500 0000 7229 0000 0072 0500  ...r....r)...r..
+00000f90: 0000 7205 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000fa0: 007f 0000 0073 0600 0000 0600 0200 0800  .....s..........
+00000fb0: 290c da02 6f73 da04 7061 7468 7237 0000  )...os..pathr7..
+00000fc0: 0072 0400 0000 da08 5f5f 6669 6c65 5f5f  .r......__file__
+00000fd0: da07 7061 7265 6e74 7372 1400 0000 7246  ..parentsr....rF
+00000fe0: 0000 0072 4a00 0000 da05 7072 696e 7472  ...rJ.....printr
+00000ff0: 3400 0000 7255 0000 0029 1272 3d00 0000  4...rU...).r=...
+00001000: 723c 0000 0072 3e00 0000 723f 0000 005a  r<...r>...r?...Z
+00001010: 0a69 6e70 6174 685f 7072 6f5a 0b69 6e70  .inpath_proZ.inp
+00001020: 6174 685f 616e 7469 5a0a 616e 7469 5f73  ath_antiZ.anti_s
+00001030: 656e 7473 5a09 7072 6f5f 7365 6e74 735a  entsZ.pro_sentsZ
+00001040: 0c61 6e74 695f 6c61 6265 6c73 5f5a 0b61  .anti_labels_Z.a
+00001050: 6e74 695f 7072 6564 735f 5a0b 7072 6f5f  nti_preds_Z.pro_
+00001060: 6c61 6265 6c73 5f5a 0a70 726f 5f70 7265  labels_Z.pro_pre
+00001070: 6473 5f5a 0b61 6e74 695f 6c61 6265 6c73  ds_Z.anti_labels
+00001080: 5a0a 616e 7469 5f70 7265 6473 5a0a 7072  Z.anti_predsZ.pr
+00001090: 6f5f 6c61 6265 6c73 5a09 7072 6f5f 7072  o_labelsZ.pro_pr
+000010a0: 6564 73da 0c63 6c66 5f72 6570 5f61 6e74  eds..clf_rep_ant
+000010b0: 69da 0b63 6c66 5f72 6570 5f70 726f 7205  i..clf_rep_pror.
+000010c0: 0000 0072 0500 0000 7209 0000 00da 0c72  ...r....r......r
+000010d0: 756e 5f77 696e 6f62 6961 736b 0000 0073  un_winobiask...s
+000010e0: 1e00 0000 0002 1a01 1a03 0801 0803 1601  ................
+000010f0: 1603 1201 1201 0a02 1801 1801 1803 0a01  ................
+00001100: 0a02 725e 0000 00a9 02da 0178 da01 7963  ..r^.......x..yc
+00001110: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001120: 0500 0000 4300 0000 7314 0000 0074 0074  ....C...s....t.t
+00001130: 01a0 027c 007c 011b 00a1 0164 0183 0253  ...|.|.....d...S
+00001140: 0029 024e 724e 0000 0029 0372 5200 0000  .).NrN...).rR...
+00001150: da04 6d61 7468 da04 6c6f 6732 725f 0000  ..math..log2r_..
+00001160: 0072 0500 0000 7205 0000 0072 0900 0000  .r....r....r....
+00001170: da08 6c6f 6772 6174 696f 8700 0000 7302  ..logratio....s.
+00001180: 0000 0000 0172 6400 0000 6303 0000 0000  .....rd...c.....
+00001190: 0000 0000 0000 000f 0000 000f 0000 0043  ...............C
+000011a0: 0000 0073 3201 0000 7c00 6401 1900 6a00  ...s2...|.d...j.
+000011b0: 6402 1900 7d03 7c01 6401 1900 6a00 6402  d...}.|.d...j.d.
+000011c0: 1900 7d04 7401 7c04 7c03 8302 7d05 7c00  ..}.t.|.|...}.|.
+000011d0: 6403 1900 6a00 6404 1900 7d06 7c00 6405  d...j.d...}.|.d.
+000011e0: 1900 6a00 6404 1900 7d07 7c01 6403 1900  ..j.d...}.|.d...
+000011f0: 6a00 6404 1900 7d08 7c01 6405 1900 6a00  j.d...}.|.d...j.
+00001200: 6404 1900 7d09 6406 7c02 9b00 9d02 6407  d...}.d.|.....d.
+00001210: 6408 6702 6409 6407 7c05 6702 640a 640b  d.g.d.d.|.g.d.d.
+00001220: 640c 6702 640d 7c03 7c04 6702 6904 7d0a  d.g.d.|.|.g.i.}.
+00001230: 7402 a003 7c0a a101 6a04 7d0a 7c0a 6a05  t...|...j.}.|.j.
+00001240: 6402 1900 7c0a 5f06 7c0a 6a05 640e 640f  d...|._.|.j.d.d.
+00001250: 8502 1900 7d0b 6410 7c02 9b00 9d02 6407  ....}.d.|.....d.
+00001260: 6408 6407 6407 6704 6409 6407 7c05 6407  d.d.d.g.d.d.|.d.
+00001270: 6407 6704 640a 640b 6407 640c 6407 6704  d.g.d.d.d.d.d.g.
+00001280: 640d 7c03 6407 7c04 6407 6704 6411 6412  d.|.d.|.d.g.d.d.
+00001290: 6413 6412 6413 6704 6414 7c06 7c07 7c08  d.d.d.g.d.|.|.|.
+000012a0: 7c09 6704 6906 7d0c 7402 a003 7c0c a101  |.g.i.}.t...|...
+000012b0: 6a04 7d0c 7c0c 6a05 6402 1900 7c0c 5f06  j.}.|.j.d...|._.
+000012c0: 7c0c 6a05 640e 640f 8502 1900 7d0d 7c0b  |.j.d.d.....}.|.
+000012d0: 7c0d 6702 7d0e 7c0e 5300 2915 7aae 4576  |.g.}.|.S.).z.Ev
+000012e0: 616c 7561 7465 2077 696e 6f62 6961 7320  aluate winobias 
+000012f0: 636f 7265 6620 6578 7065 7269 6d65 6e74  coref experiment
+00001300: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+00001310: 2020 2061 6e74 695f 7265 733a 2072 6573     anti_res: res
+00001320: 756c 7473 2066 6f72 2061 6e74 692d 7374  ults for anti-st
+00001330: 6572 656f 7479 7069 6361 6c20 636f 6e64  ereotypical cond
+00001340: 6974 696f 6e0a 2020 2020 2020 2020 7072  ition.        pr
+00001350: 6f5f 7265 733a 2072 6573 756c 7473 2066  o_res: results f
+00001360: 6f72 2070 726f 2d73 7465 7265 6f74 7970  or pro-stereotyp
+00001370: 6963 616c 2063 6f6e 6469 7469 6f6e 0a20  ical condition. 
+00001380: 2020 2020 2020 200a 2020 2020 da08 6163         .    ..ac
+00001390: 6375 7261 6379 7201 0000 0072 4700 0000  curacyr....rG...
+000013a0: 724e 0000 0072 4800 0000 7a12 5369 6d70  rN...rH...z.Simp
+000013b0: 6c65 204f 7574 7075 7420 666f 7220 da00  le Output for ..
+000013c0: 5a0a 4461 5769 6e6f 4269 6173 7a12 4765  Z.DaWinoBiasz.Ge
+000013d0: 6e64 6572 2045 6666 6563 7420 5369 7a65  nder Effect Size
+000013e0: da09 436f 6e64 6974 696f 6e7a 1241 6e74  ..Conditionz.Ant
+000013f0: 692d 7374 6572 656f 7479 7069 6361 6c7a  i-stereotypicalz
+00001400: 1150 726f 2d73 7465 7265 6f74 7970 6963  .Pro-stereotypic
+00001410: 616c da08 4163 6375 7261 6379 724b 0000  al..AccuracyrK..
+00001420: 004e 7a14 4465 7461 696c 6564 204f 7574  .Nz.Detailed Out
+00001430: 7075 7420 666f 7220 5a08 5072 6f6e 6f75  put for Z.Pronou
+00001440: 6e73 da06 4665 6d61 6c65 da04 4d61 6c65  ns..Female..Male
+00001450: da02 4631 2907 da06 7661 6c75 6573 7264  ..F1)...valuesrd
+00001460: 0000 0072 5000 0000 7251 0000 00da 0154  ...rP...rQ.....T
+00001470: da04 696c 6f63 da07 636f 6c75 6d6e 7329  ..iloc..columns)
+00001480: 0fda 0861 6e74 695f 7265 73da 0770 726f  ...anti_res..pro
+00001490: 5f72 6573 723f 0000 005a 0861 6e74 695f  _resr?...Z.anti_
+000014a0: 6163 635a 0770 726f 5f61 6363 5a12 6765  accZ.pro_accZ.ge
+000014b0: 6e64 6572 5f65 6666 6563 745f 7369 7a65  nder_effect_size
+000014c0: 5a10 616e 7469 5f66 315f 6665 6d5f 7072  Z.anti_f1_fem_pr
+000014d0: 6f6e 5a11 616e 7469 5f66 315f 6d61 6c65  onZ.anti_f1_male
+000014e0: 5f70 726f 6e5a 0f70 726f 5f66 315f 6665  _pronZ.pro_f1_fe
+000014f0: 6d5f 7072 6f6e 5a10 7072 6f5f 6631 5f6d  m_pronZ.pro_f1_m
+00001500: 616c 655f 7072 6f6e 5a0b 7369 6d6c 7065  ale_pronZ.simlpe
+00001510: 5f64 6174 615a 0973 696d 706c 655f 6466  _dataZ.simple_df
+00001520: 5a0d 6465 7461 696c 6564 5f64 6174 615a  Z.detailed_dataZ
+00001530: 0b64 6574 6169 6c65 645f 6466 da07 7265  .detailed_df..re
+00001540: 7375 6c74 7372 0500 0000 7205 0000 0072  sultsr....r....r
+00001550: 0900 0000 da14 6576 616c 7561 7465 5f6c  ......evaluate_l
+00001560: 6d5f 7769 6e6f 6269 6173 8a00 0000 734a  m_winobias....sJ
+00001570: 0000 0000 080e 010e 010a 020e 010e 020e  ................
+00001580: 010e 0308 0006 0102 0006 0102 0006 0102  ................
+00001590: 0006 fc04 070c 030c 030e 0308 000a 0102  ................
+000015a0: 000a 0102 000a 0102 000a 0102 000a 0102  ................
+000015b0: 000a fa04 090c 030c 030e 0208 0272 7300  .............rs.
+000015c0: 0000 2918 da05 746f 7263 6872 5700 0000  ..)...torchrW...
+000015d0: da05 7370 6163 7972 0e00 0000 da0b 636f  ..spacyr......co
+000015e0: 6c6c 6563 7469 6f6e 7372 0200 0000 da0f  llectionsr......
+000015f0: 736b 6c65 6172 6e2e 6d65 7472 6963 7372  sklearn.metricsr
+00001600: 0300 0000 da06 7061 6e64 6173 7250 0000  ......pandasrP..
+00001610: 00da 0770 6174 686c 6962 7204 0000 0072  ...pathlibr....r
+00001620: 6200 0000 7232 0000 0072 1400 0000 721b  b...r2...r....r.
+00001630: 0000 0072 2d00 0000 7246 0000 0072 4a00  ...r-...rF...rJ.
+00001640: 0000 7255 0000 0072 5e00 0000 da05 666c  ..rU...r^.....fl
+00001650: 6f61 7472 6400 0000 7273 0000 0072 0500  oatrd...rs...r..
+00001660: 0000 7205 0000 0072 0500 0000 7209 0000  ..r....r....r...
+00001670: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001680: 2000 0000 2001 0c01 1001 0c01 0801 0c01   ... ...........
+00001690: 0801 0802 0809 0804 0809 082a 0814 080d  ...........*....
+000016a0: 081c 1003                                ....
```

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/abc_lm_utilities.py` & `evalda_pub2-0.0.6/evalda_pub2/lm_tasks/abc_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,33 @@
-import sys, os
-import pandas as pd
+"""
+Utility functions for running the ABC language modeling task.
+
+Builds on the codebase developed for the following paper: 
+
+Title: “Type B reflexivization as an unambiguous testbed for multilingual multi-task gender bias.”
+Authors: González, A. V., Barrett, M., Hvingelby, R., Webster, K., & Søgaard, A.
+Date: 2020
+Code availability: https://github.com/anavaleriagonzalez/ABC-dataset
+"""
+import math
+import os
+import sys
+
 import numpy as np
+import pandas as pd
 import torch
-import math
-import progressbar
+from tqdm import tqdm
+
+def load_mdl(model_name):
+    print(f"[INFO] Loading model {model_name} from Hugging Face.")
+    from transformers import AutoModelForMaskedLM, AutoTokenizer
+    model = AutoModelForMaskedLM.from_pretrained(model_name)
+    tokenizer = AutoTokenizer.from_pretrained(model_name)
+    model.eval()
+    return model, tokenizer
 
 def load_abc():
     from pathlib import Path 
     inpath_male = os.path.join(Path(__file__).parents[1],"data","abc_male_sents.txt")
     inpath_fem = os.path.join(Path(__file__).parents[1],"data","abc_fem_sents.txt")
     male_sents = load_sents(inpath_male)
     fem_sents = load_sents(inpath_fem)
@@ -136,28 +156,24 @@
     """
 
     # loss function for making model predictions and loss - used for getting pperplexity scores
     loss_fct = torch.nn.CrossEntropyLoss()
 
     pronouns_list = ["sin", "sit", "sine", "▁sin", "▁sit", "▁sine"]
 
-    # intitiate progress bar
-    print(f"Running test on condition: {condition} occupations.")
-    bar = progressbar.ProgressBar(maxval=len(reflexive_sents)).start()
-
-    sents, perp_m,perp_f,perp_r = [],[],[],[]
+    print(f"[INFO] Running test on condition: {condition} occupations.")
     # loop over sentences to compute loss and perplexity
-    for idx, sent in enumerate(reflexive_sents):
+    sents, perp_m,perp_f,perp_r = [],[],[],[]
+    for idx, sent in enumerate(tqdm(reflexive_sents)):
         scores = score_sent(sent, loss_fct, tokenizer, model, pronouns_list, start_token, sep_token)
         sents.append(sent)
         perp_m.append(scores[0])
         perp_f.append(scores[1])
         perp_r.append(scores[2])
-        bar.update(idx)
-    bar.finish()
+
 
     df = pd.DataFrame({"sent":sents, 
                       "perplexity_male":perp_m,
                       "perplexity_female":perp_f,
                       "perplexity_reflexive":perp_r})
     
     df["perplexity_male"] = df["perplexity_male"].astype(float)
```

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/fillmask-danish-bert-boxto.png` & `evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/fillmask-danish-bert-boxto.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/fillmask-xlm-roberta-base.png` & `evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/fillmask-xlm-roberta-base.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/fillmask_nb-bert-base.png` & `evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/fillmask_nb-bert-base.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_danish-bert-botxo.png` & `evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_danish-bert-botxo.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-base.png` & `evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_xlm-base.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/lm_output/lm_abc_xlm-large.png` & `evalda_pub2-0.0.6/evalda_pub2/lm_tasks/lm_output/lm_abc_xlm-large.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/base_tasks/wino_fillmask_utilities.py` & `evalda_pub2-0.0.6/evalda_pub2/lm_tasks/wino_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,30 @@
-import torch, os, spacy, random 
+
+"""
+Utility functions for running the DaWinobias language modeling task.
+
+Builds on the codebase developed for the following project: 
+
+Title: “DaWinoBias: Assessing Occupational Gender Stereotypes in Danish NLP Models”
+Authors: Koppelgaard, K., Brødbæk, S. K.
+Date: 2021
+Code availability: https://github.com/NLP-exam/DaWinoBias
+"""
+import math
+import os
+import random
 from collections import Counter
-import os, random 
-from sklearn.metrics import classification_report
+from pathlib import Path
+
 import pandas as pd
-from pathlib import Path 
-import math
-import progressbar
+import spacy
+import torch
+from sklearn.metrics import classification_report
+from tqdm import tqdm
+
 
 def load_texts(filepath):
     """load DaWinoBias texts - and shuffle data 
     """    
     with open(filepath) as file:
         text = file.read().splitlines()
     lines = [line.strip() for line in text]
@@ -25,21 +40,19 @@
     """    
     #define pronouns
     pronouns = ['hans', 'hendes', 'han', 'hun', 'ham', 'hende','▁hun', '▁hendes', '▁hende', '▁han', '▁hans', '▁ham']
     # find idx of pronouns 
     prons_idx = [tokens.index(i) for i in pronouns if i in tokens][0]
     return prons_idx
 
-def predict_masked(lines, nlp, tokenizer, mask_token, model_name): 
+def predict_masked(lines, condition, nlp, tokenizer, mask_token, model_name): 
     labels, preds = [], []
-    
-    # Progress bar
-    bar = progressbar.ProgressBar(maxval=len(lines)).start()
 
-    for idx, line in enumerate(lines):
+    print(f"[INFO] Running test on condition: {condition} sentences.")
+    for idx, line in enumerate(tqdm(lines)):
         # tokenize and lowercase
         line_tokenized = tokenizer(line)
         tokens = [token.text.lower() for token in line_tokenized]
         
         # remove square brackets from tokens
         tokens = remove_sq_br(tokens)[0]
 
@@ -47,32 +60,28 @@
         prons_idx = idx_pron(tokens)
 
         #save correct pronoun
         correct_pronoun = tokens[prons_idx]
         
         # MASK pronouns
         tokens[prons_idx] = mask_token
-        #tokens[prons_idx] = '<mask>'
                  
         # join sentence into one string 
         if mask_token == '<mask>' and model_name == "vesteinn/DanskBert": 
             sentence = ' '.join(tokens).replace(" <mask>", "<mask>")
         else: 
             sentence = ' '.join(tokens)
         
         # compute fill-mask prediction
         pred = nlp(sentence)[0]['token_str']
         
         # save labels and predictions
         labels.append(correct_pronoun)
         preds.append(pred)
         
-        bar.update(idx)
-    bar.finish()
-
     return labels, preds
 
 def group_pronouns(pronouns): 
     '''group labels in female and male pronouns'''
 
     #define groups of pronouns
     female_pronouns = ['hun', 'hendes', 'hende', '▁hun', '▁hendes', '▁hende']
@@ -110,25 +119,25 @@
     inpath_anti = os.path.join(Path(__file__).parents[1],"data","DaWinoBias_anti_stereotyped_evalda.txt")
 
     # load data
     anti_sents = load_texts(inpath_anti)
     pro_sents = load_texts(inpath_pro)
 
     # mask and predict pronoun
-    anti_labels_, anti_preds_ = predict_masked(lines = anti_sents, nlp = nlp, tokenizer = tokenizer, mask_token = mask_token, model_name = model_name)
-    pro_labels_, pro_preds_ = predict_masked(lines = pro_sents, nlp = nlp, tokenizer = tokenizer, mask_token = mask_token, model_name = model_name)
+    anti_labels_, anti_preds_ = predict_masked(lines = anti_sents, condition = "anti-stereotypical", nlp = nlp, tokenizer = tokenizer, mask_token = mask_token, model_name = model_name)
+    pro_labels_, pro_preds_ = predict_masked(lines = pro_sents, condition = "pro-stereotypical", nlp = nlp, tokenizer = tokenizer, mask_token = mask_token, model_name = model_name)
 
     # group pronouns into male/female category 
     anti_labels, anti_preds = group_pronouns(anti_labels_),group_pronouns(anti_preds_) 
     pro_labels, pro_preds = group_pronouns(pro_labels_),group_pronouns(pro_preds_) 
-    print( "model:", model_name)
+    print( "[INFO] Raw predictions for model:", model_name)
     
-    print("Number of female pron. predictions:", len([i for i in anti_preds if i =='hun/hendes']))
-    print("Number of male pron. predictions:", len([i for i in anti_preds if i =='han/hans']))
-    print("Number of 'UNKNOWN' predictions:", len([i for i in anti_preds if i =='UNK']))
+    print("[INFO] Number of female pron. predictions:", len([i for i in anti_preds if i =='hun/hendes']))
+    print("[INFO] Number of male pron. predictions:", len([i for i in anti_preds if i =='han/hans']))
+    print("[INFO] Number of 'UNKNOWN' predictions:", len([i for i in anti_preds if i =='UNK']))
     
     # evaluate performance
     clf_rep_anti = evaluate_model(anti_labels, anti_preds)
     clf_rep_pro = evaluate_model(pro_labels, pro_preds)
     
     return clf_rep_anti, clf_rep_pro
```

### Comparing `evalda_pub2-0.0.5/evalda_pub2/coref_tasks/coref_output/coref_abc.png` & `evalda_pub2-0.0.6/evalda_pub2/coref_tasks/coref_output/coref_abc.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/coref_tasks/coref_output/coref_winobias.png` & `evalda_pub2-0.0.6/evalda_pub2/coref_tasks/coref_output/coref_winobias.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/coref_tasks/coref_utils.py` & `evalda_pub2-0.0.6/evalda_pub2/coref_tasks/coref_utils_OLD(delete).py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 
-from danlp.models import load_xlmr_coref_model
-from sklearn.metrics import classification_report, f1_score
-import numpy as np
-import sys, os, spacy, random, torch, json
+import json
+import math
+import os
+import random
+import sys
 from pathlib import Path
+
+import fairlearn.metrics as flm
+import nltk  # only wino
 import numpy as np
 import pandas as pd
-import nltk #only wino
 import progressbar
-import fairlearn.metrics as flm
-import math
-
+import spacy
+import torch
+from danlp.models import load_xlmr_coref_model
 from sklearn.exceptions import UndefinedMetricWarning
+from sklearn.metrics import classification_report, f1_score
+
 
 def warn(*args, **kwargs):
     pass
 import warnings
+
 warnings.warn = warn
 
 ######## ABC COREFERENCE FUNCTIONS ########
 
 def run_abc_coref(coref_model):
     ''' 
     Run the coreference model on the ABC dataset and return predictions. (Duration approx. 20 min.)
@@ -228,24 +234,23 @@
     detailed_df = detailed_data.iloc[1:]
     results = [simple_df, detailed_df]
 
     return results
 
 ######## WINOBIAS COREFERENCE ########
 
-def load_texts(filepath): # NB same fn used to load wino data for lm task - no hopefully not, because it shuffles lines??
-    '''
-    load DaWinoBias texts - and shuffle data 
-    '''    
+def load_texts(filepath): # NB same fn used to load wino data for lm task - no hopefully not, because it shuffles lines??       
     with open(filepath) as file:
         text = file.read().splitlines()
         lines = [line.strip() for line in text]
         random.shuffle(lines)
     return lines
 
+
+
 def remove_sq_br(tokens):
     """Remove square brackets from tokens
 
     Arguments:
         tokens {[type]} -- [tokenized line]
 
     Returns:
```

### Comparing `evalda_pub2-0.0.5/evalda_pub2/coref_tasks/testing-coref.ipynb` & `evalda_pub2-0.0.6/evalda_pub2/coref_tasks/testing-coref.ipynb`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/DaWinoBias_anti_stereotyped_evalda.txt` & `evalda_pub2-0.0.6/evalda_pub2/data/DaWinoBias_anti_stereotyped_evalda.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/DaWinoBias_pro_stereotyped_evalda.txt` & `evalda_pub2-0.0.6/evalda_pub2/data/DaWinoBias_pro_stereotyped_evalda.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/abc_fem_sents.txt` & `evalda_pub2-0.0.6/evalda_pub2/data/abc_fem_sents.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/abc_male_sents.txt` & `evalda_pub2-0.0.6/evalda_pub2/data/abc_male_sents.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/first_names_2023_men.csv` & `evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/first_names_2023_men.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/first_names_2023_women.csv` & `evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/first_names_2023_women.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/last_names_2023.csv` & `evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/last_names_2023.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/overlapping_names.csv` & `evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/overlapping_names.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/data/name_aug_csv_files/unisex_names.csv` & `evalda_pub2-0.0.6/evalda_pub2/data/name_aug_csv_files/unisex_names.csv`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/ner_tasks/helper_fns/process_names.py` & `evalda_pub2-0.0.6/evalda_pub2/ner_tasks/process_names.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import pandas as pd
-from dacy.datasets import muslim_names, load_names
+""" 
+Utility functions for creating the names lists used to run the NER task.
+
+Builds on early versions of the codebase developed for the following publication: 
+
+Title: “Detecting intersectionality in NER models: A data-driven approach.”
+Authors: Lassen, I. M., Almasi, M., Enevoldsen, K., & Kristensen-mclachlan, R. 
+Date: 2023
+Code availability: https://github.com/centre-for-humanities-computing/Danish-NER-bias
+"""
 import os
 from pathlib import Path
-from .overlap_fns import remove_duplicates 
+
+import pandas as pd
+from dacy.datasets import load_names, muslim_names
+
+def remove_duplicates(all_names, names_to_filter_away):
+    all_names = [name for name in all_names if name not in names_to_filter_away]
+    return all_names
 
 # path to names files 
-data_folder = os.path.join(Path(__file__).parents[2], "data","name_aug_csv_files") 
+data_folder = os.path.join(Path(__file__).parents[1], "data","name_aug_csv_files") 
 
-### DEFINE NAMES ### 
+### Define majority/danish names
 
-## last names ##
+# get last names 
 last_names_2023 = pd.read_csv(os.path.join(data_folder, "last_names_2023.csv"))
-last_names_2023["Navn"] = last_names_2023["Navn"].str.title() #capitalize
+last_names_2023["Navn"] = last_names_2023["Navn"].str.title() # capitalize
 last_names_2023 = list(last_names_2023["Navn"])[:500] # subset to only 500 to match 500 first names
 
-## men and women first names ##
+# men and women first names
 men_2023 = pd.read_csv(os.path.join(data_folder, "first_names_2023_men.csv"))
 women_2023 = pd.read_csv(os.path.join(data_folder, "first_names_2023_women.csv"))
 
-#capitalize
+# capitalize
 men_2023["Navn"] = men_2023["Navn"].str.title()
 women_2023["Navn"] = women_2023["Navn"].str.title()
 
 # subset names to 500 
 men_2023 = list(men_2023["Navn"])[:500]
 women_2023 = list(women_2023["Navn"])[:500]
 
-## unisex ##
-unisex_first_names = pd.read_csv(os.path.join(data_folder, 'unisex_names.csv'))
-unisex_first_names["Navn"] = unisex_first_names["Navn"].str.title() #capitalize
-unisex_first_names = list(unisex_first_names['Navn'])[:500]
-
 # create dictionaries 
-all_danish_2023_first_names = men_2023 + women_2023
-
-#dk_name_dict = {'first_name':all_danish_2023_first_names, 'last_name':last_names_2023}
 m_name_dict = {'first_name':men_2023, 'last_name':last_names_2023}
 f_name_dict = {'first_name':women_2023, 'last_name':last_names_2023}
-unisex_name_dict = {'first_name':unisex_first_names, 'last_name':last_names_2023}
 
-## muslim names ##
+### Define muslim/minority names 
 muslim_name_dict = muslim_names()
 muslim_m_dict = load_names(ethnicity="muslim", gender="male", min_prop_gender=0.5)
 muslim_f_dict = load_names(ethnicity="muslim", gender="female", min_prop_gender=0.5)
 
-### REMOVE OVERLAPS ##
-
+### Remove overlaps 
 # read in annotated
 overlaps = pd.read_csv(os.path.join(data_folder, "overlapping_names.csv"))
 
-# create muslim/minority only list and danish only list 
+# create muslim/minority only list and majority/danish only list 
 muslim_only=list(overlaps.query("origin=='M'")["duplicates"])
 danish_only=list(overlaps.query("origin=='DK'")["duplicates"])
 
-# overall 
-#dk_name_dict["first_name"] = remove_duplicates(dk_name_dict["first_name"], muslim_only)
-#muslim_name_dict["first_name"] = remove_duplicates(muslim_name_dict["first_name"], danish_only)
-
-# danish genders
+# majority/danish seperate genders into seperate dicts
 f_name_dict["first_name"] = remove_duplicates(f_name_dict["first_name"], muslim_only)
 m_name_dict["first_name"] = remove_duplicates(m_name_dict["first_name"], muslim_only)
 
-# muslim genders
+# muslim/minority seperate genders into seperate dicts
 muslim_f_dict["first_name"] = remove_duplicates(muslim_f_dict["first_name"], danish_only)
 muslim_m_dict["first_name"] = remove_duplicates(muslim_m_dict["first_name"], danish_only)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20.png` & `evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_dacy-large-n-20.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20.png` & `evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_scandi-n-20.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20.png` & `evalda_pub2-0.0.6/evalda_pub2/ner_tasks/ner_output/ner_spacy-large-n-20.png`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/evalda_pub2/ner_tasks/requirements-dacy-ner.txt` & `evalda_pub2-0.0.6/evalda_pub2/ner_tasks/requirements-dacy-ner.txt`

 * *Files identical despite different names*

### Comparing `evalda_pub2-0.0.5/PKG-INFO` & `evalda_pub2-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: evalda-pub2
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for quantifying bias in Danish language models.
 Home-page: https://github.com/DaDebias/evalda-pub2
 License: MIT
 Author: Astrid Rybner
 Author-email: astrid.rybner@hotmail.com
-Requires-Python: >=3.8.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: augmenty (==1.3.1)
 Requires-Dist: dacy (==2.3.1)
 Requires-Dist: gensim (>=4.3.1,<5.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
```

