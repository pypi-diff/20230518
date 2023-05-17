# Comparing `tmp/finetune_eval_harness-0.6.7.dev1.tar.gz` & `tmp/finetune_eval_harness-0.6.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetune_eval_harness-0.6.7.dev1.tar", last modified: Wed May 17 22:46:48 2023, max compression
+gzip compressed data, was "finetune_eval_harness-0.6.8.dev1.tar", last modified: Wed May 17 23:06:14 2023, max compression
```

## Comparing `finetune_eval_harness-0.6.7.dev1.tar` & `finetune_eval_harness-0.6.8.dev1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:46:48.405391 finetune_eval_harness-0.6.7.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 22:46:48.405391 finetune_eval_harness-0.6.7.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:46:48.405391 finetune_eval_harness-0.6.7.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:46:48.397390 finetune_eval_harness-0.6.7.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:46:48.397390 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:46:48.401390 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/initial_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/model_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)    54631 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/process_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:46:48.405391 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/dutch_social.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/eur_lux.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/flue.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/german_europarl.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/german_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/german_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/germeval2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/germeval2018.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/gnad10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/greek_legal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/klej_dyk.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/mapa.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/polish_dyk.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/rucola.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/spanish_conll.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/spanish_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/swedish_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/szeged_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/task_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 22:46:47.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:46:48.397390 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 22:46:48.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-17 22:46:48.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 22:46:48.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 22:46:48.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 22:46:48.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 22:46:48.000000 finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:06:14.410632 finetune_eval_harness-0.6.8.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 23:06:14.410632 finetune_eval_harness-0.6.8.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 23:06:14.410632 finetune_eval_harness-0.6.8.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:06:14.402632 finetune_eval_harness-0.6.8.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:06:14.402632 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:06:14.406632 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/initial_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/model_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54754 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/process_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:06:14.410632 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/dutch_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/eur_lux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/flue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/german_europarl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/german_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/german_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/germeval2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/germeval2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/gnad10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/greek_legal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/klej_dyk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/mapa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/polish_dyk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/rucola.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/spanish_conll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/spanish_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/swedish_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/szeged_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/task_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-17 23:06:13.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:06:14.406632 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 23:06:14.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-17 23:06:14.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 23:06:14.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 23:06:14.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 23:06:14.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 23:06:14.000000 finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/top_level.txt
```

### Comparing `finetune_eval_harness-0.6.7.dev1/LICENSE` & `finetune_eval_harness-0.6.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/PKG-INFO` & `finetune_eval_harness-0.6.8.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetune_eval_harness
-Version: 0.6.7.dev1
+Version: 0.6.8.dev1
 Summary: Finetune_Eval_Harness
 Home-page: UNKNOWN
 Author: DFKI Berlin
 Author-email: akga01@dfki.de
 License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
```

### Comparing `finetune_eval_harness-0.6.7.dev1/README.md` & `finetune_eval_harness-0.6.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/setup.py` & `finetune_eval_harness-0.6.8.dev1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name = "finetune_eval_harness",
-    version="0.6.7.dev1",
+    version="0.6.8.dev1",
     description="Finetune_Eval_Harness",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="MIT",
     author="DFKI Berlin",
     author_email="akga01@dfki.de",
```

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/__init__.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,13 +39,16 @@
 import src.finetune_eval_harness.hf_scripts
 import src.finetune_eval_harness.tasks as tasks
 import src.finetune_eval_harness.hf_scripts as hf_scripts
 '''
 
 import sys
 sys.path.append('./')
-from .tasks import *
-from .tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY, get_all_task_types, get_dataset_information
-from .hf_scripts import *
+from finetune_eval_harness.tasks import *
+from finetune_eval_harness.tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY, get_all_task_types, get_dataset_information
+from finetune_eval_harness.hf_scripts import *
+
+#from .tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY, get_all_task_types, get_dataset_information
+#from .hf_scripts import *
 
 sys.path.append('../')
 #import hf_scripts
```

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/model_args.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/model_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/trainer.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/trainer.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     LoraConfig,
 )
 from peft import PrefixTuningConfig, PromptEncoderConfig, PromptTuningConfig, TaskType
 from peft.utils.other import fsdp_auto_wrap_policy
 from os import path
 
 sys.path.append("./")
-from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY, get_all_task_types
-
+#from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY, get_all_task_types
+from finetune_eval_harness.tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY, get_all_task_types
 
 # from src.finetune_eval_harness.tasks.task_registry import (
 #     get_all_tasks,
 #     TASK_REGISTRY,
 #     TASK_TYPE_REGISTRY,
 # )
```

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/process_args.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/process_args.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import sys
 sys.path.append('./')
 from transformers import HfArgumentParser, TrainingArguments
-from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
+#from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
+from finetune_eval_harness.tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
 import logging
 sys.path.append('../')
 
-from hf_scripts.utility_functions import (
+from finetune_eval_harness.hf_scripts.utility_functions import (
     map_source_file,
     peft_choice_list,
     add_labels_data_args,
 )
 
-from hf_scripts.model_args import ModelArguments
-from hf_scripts.data_trainining_args import DataTrainingArguments
-from hf_scripts.initial_arguments import InitialArguments
+from finetune_eval_harness.hf_scripts.model_args import ModelArguments
+from finetune_eval_harness.hf_scripts.data_trainining_args import DataTrainingArguments
+from finetune_eval_harness.hf_scripts.initial_arguments import InitialArguments
 
 
 def process_arguments(args):
     """
     main method accepts argaprse arguments and process it to utilize the training scripts
     """
```

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/__init__.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/classification.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/dutch_social.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/dutch_social.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/eur_lux.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/eur_lux.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/flue.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/flue.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/german_europarl.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/german_europarl.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/german_ner.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/german_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/german_quad.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/german_quad.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/germeval2017.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/germeval2017.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/germeval2018.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/germeval2018.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/gnad10.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/gnad10.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/greek_legal.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/greek_legal.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/klej_dyk.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/klej_dyk.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/mapa.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/mapa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/ner.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/polish_dyk.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/polish_dyk.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/rucola.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/rucola.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/spanish_conll.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/spanish_conll.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/spanish_quad.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/spanish_quad.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/swedish_ner.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/swedish_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/szeged_ner.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/szeged_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/task_registry.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/task_registry.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/PKG-INFO` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetune-eval-harness
-Version: 0.6.7.dev1
+Version: 0.6.8.dev1
 Summary: Finetune_Eval_Harness
 Home-page: UNKNOWN
 Author: DFKI Berlin
 Author-email: akga01@dfki.de
 License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
```

### Comparing `finetune_eval_harness-0.6.7.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt` & `finetune_eval_harness-0.6.8.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

