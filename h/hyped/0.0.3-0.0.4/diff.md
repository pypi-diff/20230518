# Comparing `tmp/hyped-0.0.3.tar.gz` & `tmp/hyped-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyped-0.0.3.tar", last modified: Sun May 14 17:00:16 2023, max compression
+gzip compressed data, was "hyped-0.0.4.tar", last modified: Thu May 18 15:51:14 2023, max compression
```

## Comparing `hyped-0.0.3.tar` & `hyped-0.0.4.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.750982 hyped-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 17:00:07.000000 hyped-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 17:00:16.746982 hyped-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-14 17:00:07.000000 hyped-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.742982 hyped-0.0.3/hyped/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.742982 hyped-0.0.3/hyped/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/datasets/cas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.742982 hyped-0.0.3/hyped/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/evaluate/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/evaluate/metrics/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/modeling/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/heads/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/heads/cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/heads/tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/modeling/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/pipeline/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/filters/msl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/pipeline/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/processors/bio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/pipeline/processors/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/scripts/utils/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.746982 hyped-0.0.3/hyped/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/utils/typedlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-14 17:00:07.000000 hyped-0.0.3/hyped/utils/typedmapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:00:16.742982 hyped-0.0.3/hyped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 17:00:16.000000 hyped-0.0.3/hyped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:00:16.750982 hyped-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-14 17:00:07.000000 hyped-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.105875 hyped-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 15:51:02.000000 hyped-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-18 15:51:14.101875 hyped-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-18 15:51:02.000000 hyped-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.085875 hyped-0.0.4/hyped/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.089875 hyped-0.0.4/hyped/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/datasets/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/datasets/xcr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.089875 hyped-0.0.4/hyped/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.093875 hyped-0.0.4/hyped/evaluate/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/mlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/metrics/seqeval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/evaluate/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.093875 hyped-0.0.4/hyped/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.093875 hyped-0.0.4/hyped/modeling/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/mlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/heads/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/modeling/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.097875 hyped-0.0.4/hyped/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.097875 hyped-0.0.4/hyped/pipeline/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/filters/msl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.101875 hyped-0.0.4/hyped/pipeline/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/processors/bio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/pipeline/processors/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.101875 hyped-0.0.4/hyped/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/scripts/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/scripts/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.101875 hyped-0.0.4/hyped/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/utils/typedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-18 15:51:02.000000 hyped-0.0.4/hyped/utils/typedmapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:14.085875 hyped-0.0.4/hyped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 15:51:14.000000 hyped-0.0.4/hyped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:51:14.105875 hyped-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-18 15:51:02.000000 hyped-0.0.4/setup.py
```

### Comparing `hyped-0.0.3/LICENSE` & `hyped-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/PKG-INFO` & `hyped-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: hyped
-Version: 0.0.3
-Summary: A collection of data pipelines to ease the training of transformer models
-Home-page: https://github.com/ndoll1998/hyped/tree/master
-Author: Niclas Doll
-Author-email: niclas@amazonis.net
-Classifier: License :: Freely Distributable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # :boom: hyped
 ![Publish Master](https://github.com/ndoll1998/hyped/workflows/PyPI/badge.svg)
 
 A collection of data pipelines to ease the training of transformer models
 
 ## installation
 
@@ -51,34 +38,51 @@
 ```bash
 # data preparation stage
 # runs the data preparation pipeline specified in the
 # configuration file and saves the prepared dataset
 # to the specified location
 python -m hyped.scripts.prepare \
     -c examples/text_cls/imdb/distilbert_data.json \
-    -o output/distilbert_data.bin
+    -o output/distilbert_data
 
 # model training stage
 # trains a model on the prepared data generated by the
 # previous stage
 python -m hyped.scripts.train \
     -c examples/text_cls/imdb/distilbert_run.json \
-    -d output/distilbert_data.bin \
+    -d output/distilbert_data \
     -o output/model
 
 # model evaluation stage
 # evaluates the trained model on the test split of the
 # prepared dataset generated earlier
 python -m hyped.scripts.evaluate \
     -c examples/text_cls/imdb/distilbert_run.json \
-    -d output/distilbert_data.bin \
+    -d output/distilbert_data \
     -m output/model/best-model
 ```
 
 ## features
 
 `hyped` currently implements all components required to train and evaluate models for the following NLP tasks:
 
  - Text Classification
  - Named Entity Recognition
+ - Multi-label Classification
+
+
+## roadmap
 
+`hyped` is still in its very early stages. With time the goal is to make the framework applicable to a wide variety of tasks and setups. Planned features include the following:
 
+ - ~~support adapter training~~
+ - support more tasks
+   - Masked Language Modeling
+   - Causal Language Modeling
+   - nested Named Entity Recognition
+   - Question Answering
+ - support multi-modal encoders
+   - LayoutLM
+   - LiLT
+ - support distributed training/inference
+   - deepspeed
+   - pytorch DDP and FSDP
```

### Comparing `hyped-0.0.3/hyped/datasets/cas.py` & `hyped-0.0.4/hyped/datasets/cas.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/hyped/evaluate/auto.py` & `hyped-0.0.4/hyped/evaluate/auto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,99 @@
 from . import metrics
-from .metrics.base import HypedMetrics
-from .metrics.collection import HypedMetricsCollection
+from .metrics.base import HypedMetric, HypedMetricConfig
+from .collection import HypedMetricCollection
 from transformers.adapters import heads
 from hyped.utils.typedmapping import typedmapping
 
-class HypedAutoMetrics(object):
+class HypedAutoMetric(object):
     METRICS_MAPPING = typedmapping[
         type[heads.PredictionHead],
-        type[HypedMetrics]
+        typedmapping
     ]()
 
     @classmethod
-    def from_head(cls, head:heads.PredictionHead, **kwargs):
-        # find metric type for given head
-        for head_t, metrics_t in cls.METRICS_MAPPING.items():
+    def from_head(
+        cls,
+        head:heads.PredictionHead,
+        config:HypedMetricConfig
+    ) -> HypedMetric:
+        # find metrics for head
+        for head_t, metrics_mapping in cls.METRICS_MAPPING.items():
             if isinstance(head, head_t):
+                # find specific metric
+                metric_t = metrics_mapping.get(type(config), None)
+                # check if metric type found
+                if metric_t is None:
+                    raise ValueError("Invalid metric type `%s`." % config.metric_type)
                 # create metric instance
-                metrics = metrics_t(head, **kwargs)
-                return metrics
-        # no metric found for head of type
-        raise ValueError("No metrics found for head of type %s." % type(head))
+                metric = metric_t(head, config)
+                return metric
+        # no metric found for head
+        raise ValueError("No metric registered for head of type `%s`." % type(head))
 
     @classmethod
     def from_model(
         cls,
         model:heads.ModelWithFlexibleHeadsAdaptersMixin,
-        metrics_kwargs:dict ={},
-        label_order:None|list[str] =None
-    ) -> HypedMetrics:
+        metric_configs:dict[str, list[HypedMetricConfig]],
+        label_order:list[str]
+    ) -> HypedMetricCollection:
         # type checking
         if not isinstance(model, heads.ModelWithFlexibleHeadsAdaptersMixin):
             raise ValueError("Expected model with `ModelWithFlexibleHeadsAdaptersMixin`, got %s." % type(model))
         if model.active_head is None:
             raise ValueError("No active head detected in model!")
 
         if isinstance(model.active_head, str):
             # single active head
             head = model.heads[model.active_head]
-            return cls.from_head(head, **metrics_kwargs.get(model.active_head, {}))
+            # build metric collection
+            return HypedMetricCollection(
+                metrics=[cls.from_head(head, config) for config in metric_configs[head.name]],
+                head_order=[model.active_head],
+                label_order=label_order
+            )
 
         elif isinstance(model.active_head, list):
             # check if label order is given
             if label_order is None:
                 raise ValueError("Label order is required for multi head models, got label_order=%s!" % label_order)
             # build metric for each head
             metrics = [
-                cls.from_head(model.heads[head_name], **metrics_kwargs.get(head_name, {}))
+                cls.from_head(model.heads[head_name], config)
                 for head_name in model.active_head
+                for config in metric_configs[head_name]
             ]
             # build metrics collection and return
-            return HypedMetricsCollection(metrics, model.active_head, label_order)
+            return HypedMetricCollection(metrics, model.active_head, label_order)
 
         raise Exception("Unexpected active head %s!" % model.active_head)
 
     @classmethod
-    def register(cls, head_t:type[heads.PredictionHead], metrics_t:type[HypedMetrics]):
-        cls.METRICS_MAPPING[head_t] = metrics_t
-
-# register metrics
-HypedAutoMetrics.register(heads.ClassificationHead, metrics.HypedClsMetrics)
-HypedAutoMetrics.register(heads.TaggingHead, metrics.HypedTaggingMetrics)
+    def register(
+        cls,
+        head_t:type[heads.PredictionHead],
+        config_t:type[HypedMetricConfig],
+        metrics_t:type[HypedMetric]
+    ):
+        if head_t not in cls.METRICS_MAPPING:
+            cls.METRICS_MAPPING[head_t] = typedmapping[
+                type[HypedMetricConfig], type[HypedMetric]
+            ]()
+
+        cls.METRICS_MAPPING[head_t][config_t] = metrics_t
+
+HypedAutoMetric.register(
+    head_t=heads.ClassificationHead,
+    config_t=metrics.ClassificationMetricConfig,
+    metrics_t=metrics.ClassificationMetric
+)
+HypedAutoMetric.register(
+    head_t=heads.MultiLabelClassificationHead,
+    config_t=metrics.MlcMetricConfig,
+    metrics_t=metrics.MlcMetric
+)
+HypedAutoMetric.register(
+    head_t=heads.TaggingHead,
+    config_t=metrics.SeqEvalMetricConfig,
+    metrics_t=metrics.SeqEvalMetric
+)
```

### Comparing `hyped-0.0.3/hyped/evaluate/metrics/collection.py` & `hyped-0.0.4/hyped/evaluate/collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,66 @@
-import numpy as np
-from .base import HypedMetrics
+from .metrics.base import HypedMetric
 from transformers import EvalPrediction
-from transformers.adapters.heads import PredictionHead
+from collections import defaultdict
 
 def get_labels(labels:dict, label_names:list[str]):
     if len(label_names) == 1:
         return labels[label_names[0]]
     return [labels[name] for name in label_names]
 
-class HypedMetricsCollection(HypedMetrics):
+class HypedMetricCollection(object):
 
     def __init__(
         self,
-        metrics:list[HypedMetrics],
+        metrics:list[HypedMetric],
         head_order:list[str],
         label_order:list[str]
     ) -> None:
-        # has no specific head
-        super().__init__(None)
-        # save metrics
-        self.metrics = metrics
-        # save label order
+        # save head and label order
         self.head_order = head_order
         self.label_order = label_order
-        # one metric per head
-        if len(metrics) != len(self.head_order):
-            raise ValueError("Expected exactly one metric per head!")
-
-    def __call__(self,eval_pred:EvalPrediction) -> dict[str, float]:
-        # avoid adding head prefix
-        return self.compute(eval_pred)
 
-    def compute(self, eval_pred:EvalPrediction) -> dict[str, float]:
+        self.metrics = metrics
+        self.processors = defaultdict(set)
+
+        for metric in metrics:
+            self.processors[metric.head].add(metric.processor)
+
+    def compute(self, eval_pred):
         scores = {}
-        # unpack and create labels lookup
+        # unpack and make sure labels is list
         preds, labels = eval_pred
+        labels = labels if len(self.label_order) > 1 else [labels]
+        # create labels lookup
         labels = dict(zip(self.label_order, labels))
         # compute all metrics
         for metric in self.metrics:
             scores.update(metric(
                 EvalPrediction(
-                    predictions=preds[metric.head.name],
+                    predictions=preds[metric.head.name, metric.processor],
                     label_ids=get_labels(labels, metric.head.get_label_names())
                 )
             ))
         # return all scores
         return scores
 
-    def preprocess(self, logits:np.ndarray, labels:np.ndarray) -> np.ndarray:
+    def preprocess(self, logits, labels):
+        # make sure logits and labels are lists
+        logits = logits if len(self.head_order) > 1 else [logits]
+        labels = labels if len(self.label_order) > 1 else [labels]
+        # check sizes
         assert len(logits) == len(self.head_order)
         assert len(labels) == len(self.label_order)
         # unpack logits
         logits = [l.logits if hasattr(l, 'logits') else l for l in logits]
-        # create look ups
+        # create look-ups
         logits = dict(zip(self.head_order, logits))
         labels = dict(zip(self.label_order, labels))
-
+        # preprocess all logits
         return {
-            metric.head.name: metric.preprocess(
-                logits=logits[metric.head.name],
-                labels=get_labels(labels, metric.head.get_label_names())
+            (h.name, p): p(
+                logits=logits[h.name],
+                labels=get_labels(labels, h.get_label_names())
             )
-            for metric in self.metrics
+            for h, ps in self.processors.items()
+            for p in ps
         }
```

### Comparing `hyped-0.0.3/hyped/evaluate/metrics/tagging.py` & `hyped-0.0.4/hyped/evaluate/metrics/seqeval.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,36 @@
 import evaluate
 import numpy as np
-from .base import HypedMetrics
 from transformers import EvalPrediction
-from transformers.adapters import PredictionHead
+from transformers.adapters.heads import PredictionHead
+from .base import HypedMetric, HypedMetricConfig
+from ..processors import ArgMaxLogitsProcessor
+from dataclasses import dataclass, field
+from functools import partial
+from typing import Literal
 
-class HypedTaggingMetrics(HypedMetrics):
+@dataclass
+class SeqEvalMetricConfig(HypedMetricConfig):
+    metric_type:Literal['seqeval'] = 'seqeval'
+    # additional arguments
+    suffix:bool = False
+    scheme:None|Literal["IOB1","IOB2","IOE1","IOE2","IOBES","BILOU"] = None
+    mode:None|str =None
+    zero_division:Literal[0,1,"warn"] = 0
 
-    def __init__(self, head:PredictionHead):
-        super(HypedTaggingMetrics, self).__init__(head)
-        # load all metrics
-        self.seqeval = evaluate.load("seqeval")
+class SeqEvalMetric(HypedMetric):
+
+    def __init__(self, head:PredictionHead, config:SeqEvalMetricConfig) -> None:
+        super(SeqEvalMetric, self).__init__(
+            head=head,
+            config=config,
+            processor=ArgMaxLogitsProcessor()
+        )
+        # load seceval metric
+        self.metric = evaluate.load('seqeval')
 
         # get label mapping from head config
         label2id = head.config.get('label2id', None)
         if label2id is None:
             raise ValueError("Config of head type %s has no `label2id` entry." % type(head))
         # build label space array from mapping
         self.label_space = np.empty(len(label2id), dtype=object)
@@ -21,18 +38,20 @@
             self.label_space[i] = label
 
     def compute(self, eval_pred:EvalPrediction) -> dict[str, float]:
         # unpack predicitons and labels
         preds, labels = eval_pred
         # compute valid mask and lengths
         mask = (labels >= 0)
-        lengths = mask.sum(axis=-1)
+        splits = np.cumsum(mask.sum(axis=-1)[:-1])
         # compute metric
-        return self.seqeval.compute(
+        return self.metric.compute(
             # apply valid mask, convert label ids to label names
             # and split into seperate examples (masking flattens the arrays)
-            predictions=np.array_split(self.label_space[preds[mask]], lengths[:-1]),
-            references=np.array_split(self.label_space[labels[mask]], lengths[:-1])
+            predictions=np.array_split(self.label_space[preds[mask]], splits),
+            references=np.array_split(self.label_space[labels[mask]], splits),
+            # additional arguments
+            suffix=self.config.suffix,
+            scheme=self.config.scheme,
+            mode=self.config.mode,
+            zero_division=self.config.zero_division
         )
-
-    def preprocess(self, logits:np.ndarray, labels:np.ndarray) -> np.ndarray:
-        return logits.argmax(dim=-1)
```

### Comparing `hyped-0.0.3/hyped/modeling/auto.py` & `hyped-0.0.4/hyped/modeling/auto.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,8 +57,9 @@
 
     @classmethod
     def register_custom_head(cls, head_name, head_type):
         cls.CUSTOM_HEAD_MAPPING[head_name] = head_type
 
 # register prediction heads
 HypedAutoAdapterModel.register_custom_head(heads.HypedClsHeadConfig.head_type, heads.HypedClsHead)
+HypedAutoAdapterModel.register_custom_head(heads.HypedMlcHeadConfig.head_type, heads.HypedMlcHead)
 HypedAutoAdapterModel.register_custom_head(heads.HypedTaggingHeadConfig.head_type, heads.HypedTaggingHead)
```

### Comparing `hyped-0.0.3/hyped/modeling/heads/base.py` & `hyped-0.0.4/hyped/modeling/heads/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import torch
+import logging
 from abc import ABC, abstractmethod
 from transformers.adapters.heads import PredictionHead
 from dataclasses import dataclass
 from datasets.features import Features
-from typing import Literal
-import logging
+from typing import Literal, Any
 
 logger = logging.getLogger(__name__)
 
 @dataclass
 class HypedPredictionHeadConfig(ABC):
     # specify the head type identifier
     # this identifier is resolved to the actual head type
@@ -85,7 +86,12 @@
 
         # return output
         return out
 
     @abstractmethod
     def wrapped_forward(self, *args, **kwargs):
         ...
+
+    def collate_labels(self, labels:list, return_tensors:str ='pt'):
+        if return_tensors != 'pt':
+            raise NotImplementedError()
+        return torch.stack(labels, dim=0)
```

### Comparing `hyped-0.0.3/hyped/modeling/heads/cls.py` & `hyped-0.0.4/hyped/modeling/heads/cls.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/hyped/modeling/heads/tagging.py` & `hyped-0.0.4/hyped/modeling/heads/tagging.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/hyped/modeling/trainer.py` & `hyped-0.0.4/hyped/modeling/trainer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import torch
 from transformers import Trainer
 from transformers.adapters import AdapterTrainer
 from transformers.adapters.heads import MultiHeadOutput
 
-class MultiHeadTrainer(Trainer):
-
+class MultiHeadLossMixin(object):
     def compute_loss(self, model, inputs, return_outputs=False):
 
         # apply model and
         output = model(**inputs)
 
         if isinstance(output, MultiHeadOutput) and (output.get('loss', None) is None):
             # check if all heads computed a loss
@@ -22,7 +21,14 @@
                     "The model did not return a loss from the inputs, only the following keys: "
                     f"{','.join(outputs.keys())}. For reference, the inputs it received are {','.join(inputs.keys())}."
                 )
 
         # get loss from output and return
         loss = output['loss'] if isinstance(output, dict) else output[0]
         return (loss, output) if return_outputs else loss
+
+class MultiHeadTrainer(MultiHeadLossMixin, Trainer):
+    """ Transformers trainer for multi-head models """
+
+class MultiHeadAdapterTrainer(MultiHeadLossMixin, AdapterTrainer):
+    """ Adapter trainer for multi-head models """
+
```

### Comparing `hyped-0.0.3/hyped/pipeline/auto.py` & `hyped-0.0.4/hyped/pipeline/auto.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/hyped/pipeline/filters/base.py` & `hyped-0.0.4/hyped/pipeline/filters/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/hyped/pipeline/filters/msl.py` & `hyped-0.0.4/hyped/pipeline/filters/msl.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/hyped/pipeline/pipeline.py` & `hyped-0.0.4/hyped/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         self.processors = DataProcessorList[DataProcessor]()
         self.filters = DataFilterList[DataFilter]()
         # add processors and filters
         self.processors.extend(processors)
         self.filters.extend(filters)
 
     @property
-    def features(self) -> datasets.Features:
-        return self.processors[0].features
+    def in_features(self) -> datasets.Features:
+        return self.processors[0].in_features
 
     @property
     def out_features(self) -> datasets.Features:
         return self.processors[-1].out_features
 
     def prepare(self, features:datasets.Features) -> datasets.Features:
         # prepare all processors
```

### Comparing `hyped-0.0.3/hyped/pipeline/processors/base.py` & `hyped-0.0.4/hyped/pipeline/processors/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 from abc import ABC, abstractmethod
 from datasets import Features
 
 from inspect import signature
 from dataclasses import dataclass
 
 import numpy as np
+import pyarrow as pa
 from typing import Any, Literal
 
 @dataclass
 class DataProcessorConfig(object):
     processor_type:Literal['abstract-data-processor'] = 'abstract-data-processor'
 
 class DataProcessor(ABC):
     """Abstract Data Processor"""
 
     def __init__(self, config:DataProcessorConfig) -> None:
         self.config = config
         self._in_features:Features = None
-        self._out_features:Features = None
+        self._new_features:Features = None
 
     @property
     def is_prepared(self) -> bool:
-        return (self._in_features is not None) and (self._out_features is not None)
+        return (self._in_features is not None) and (self._new_features is not None)
 
     @property
-    def features(self) -> Features:
+    def in_features(self) -> Features:
         # check if data processor is prepared
         if not self.is_prepared:
             raise RuntimeError("Data processor not prepared. Did you forget to call `prepare` before execution?")
         # return features
         return self._in_features
 
     @property
-    def out_features(self) -> Features:
+    def new_features(self) -> Features:
         # check if data processor is prepared
         if not self.is_prepared:
             raise RuntimeError("Data processor not prepared. Did you forget to call `prepare` before execution?")
         # return features
-        return self._out_features
+        return self._new_features
+
+    @property
+    def out_features(self) -> Features:
+        return Features(self.in_features | self.new_features)
 
     def prepare(self, features:Features) -> Features:
         # check if data processor is already prepared
         if self.is_prepared:
             raise RuntimeError("Data processor already prepared!")
         # map input features to output features
         # copy as preparation might disturb features inplace
-        out_features = self.map_features(features.copy())
+        new_features = self.map_features(features.copy())
         # set features
         self._in_features = features
-        self._out_features = out_features
+        self._new_features = new_features
         # return output features
         return self.out_features
 
     @property
     def requires_rank(self) -> bool:
         return 'rank' in signature(self.process).parameters
 
     @property
     def requires_index(self) -> bool:
         return 'index' in signature(self.process).parameters
 
     @abstractmethod
     def map_features(self, features:Features) -> Features:
+        """ Map input features to *new* features. This specifies the exact output of the `process` function."""
         ...
 
     @abstractmethod
     def process(self, example:Any) -> dict[str, np.ndarray]:
         ...
     @abstractmethod
     def process(self, example:Any, rank:int) -> dict[str, np.ndarray]:
@@ -73,9 +79,19 @@
     @abstractmethod
     def process(self, example:Any, index:int) -> dict[str, np.ndarray]:
         ...
     @abstractmethod
     def process(self, example:Any, index:int, rank:int) -> dict[str, np.ndarray]:
         ...
 
-    def __call__(self, *args, **kwargs):
-        return self.process(*args, **kwargs)
+    def __call__(self, example, *args, **kwargs):
+        # run data processor
+        features = self.process(example, *args, **kwargs)
+        example.update(features)
+        # TODO: only necessary for non-batched data processors
+        for k, f in example.items():
+            example[k] = [f]
+        # convert to py-arrow table with correct schema
+        return pa.table(
+            data=dict(example),
+            schema=self.out_features.arrow_schema
+        )
```

### Comparing `hyped-0.0.3/hyped/pipeline/processors/bio.py` & `hyped-0.0.4/hyped/pipeline/processors/bio.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     """BIO Labeling Scheme Processor"""
 
     @property
     def entity_names(self) -> list[str]:
         if self.config.token_bio_column is not None:
             raise NotImplementedError()
         # return entity names from input features
-        return self.features[self.config.token_span_column]['type'].feature.names
+        return self.in_features[self.config.token_span_column]['type'].feature.names
 
     @property
     def out_tag_id(self) -> int:
         return self.bio_label2id(self.config.out_tag)
 
     @property
     def bio_tags(self) -> list[str]:
@@ -88,25 +88,26 @@
         f = features[self.config.word_ids_column]
         if not (isinstance(f, Sequence) and (f.feature == Value('int32'))):
             raise TypeError("Expected word ids to be a sequence of ints, got %s." % feature)
 
         # get length of word-ids sequence
         l = f.length
 
+        out_feature = None
         if self.config.token_bio_column is not None:
             # check if token bio labels column is present
             if self.config.token_bio_column not in features:
                 raise KeyError("`%s` not present in features!" % self.config.token_bio_column)
             # check type of bio labels feature
             f = features[self.config.token_bio_column]
             if not (isinstance(f, Sequence) and isinstance(f.feature, ClassLabel)):
                 raise TypeError("Expected bio labels to be a `Sequence` of `ClassLabels`, got %s." % f)
 
             # add feature
-            features[self.config.output_column] = Sequence(ClassLabel(names=f.feature.names), length=l)
+            out_feature = Sequence(ClassLabel(names=f.feature.names), length=l)
 
         elif self.config.token_span_column is not None:
             # check if token span column is present
             if self.config.token_span_column not in features:
                 raise KeyError("`%s` not present in features!" % self.config.token_span_column)
             # check type of span column
             # TODO: check feature type (must containt begin, end, type of correct feature types)
@@ -117,19 +118,18 @@
             bio_tags = [self.config.out_tag] + [
                 "%s%s" % (prefix, name) for name in names for prefix in (
                     self.config.begin_tag_prefix,
                     self.config.in_tag_prefix
                 )
             ]
             # add feature
-            features[self.config.output_column] = Sequence(ClassLabel(names=bio_tags), length=l)
+            out_feature = Sequence(ClassLabel(names=bio_tags), length=l)
 
-        # return updated features
-        assert self.config.output_column in features
-        return features
+        assert out_feature is not None
+        return Features({self.config.output_column: out_feature})
 
     def process(self, example:dict[str, Any]) -> dict[str, np.ndarray]:
 
         # get word ids from examples and compute special tokens mask
         word_ids = np.asarray(example[self.config.word_ids_column])
         special_tokens_mask = (word_ids < 0)
```

### Comparing `hyped-0.0.3/hyped/pipeline/processors/tokenizer.py` & `hyped-0.0.4/hyped/pipeline/processors/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.tokenizer = AutoTokenizer.from_pretrained(
             config.pretrained_ckpt,
             use_fast=True,
             add_prefix_space=True
         )
 
     def map_features(self, features:Features) -> Features:
+
         # make sure text column is present
         if self.config.text_column not in features:
             raise KeyError("`%s` not present in features!" % self.config.text_column)
         # check type of input feature
         f = features[self.config.text_column]
         if self.config.is_split_into_words and not (isinstance(f, Sequence) and (f.feature == Value('string'))):
             raise TypeError("Input feature `%s` must be sequence of strings, got %s." % (self.config.text_column, features[self.config.text_column]))
@@ -60,33 +61,36 @@
             raise TypeError("Input feature `%s` must be string, got %s." % (self.config.text_column, features[self.config.text_column]))
 
         # check for constant length
         is_constant = (self.config.max_length is not None) and \
             (self.config.padding == 'max_length') and \
             (self.config.truncation in (True, 'longest_first', 'only_first', 'only_second'))
         length = self.config.max_length if is_constant else -1
+
+        # create new features
+        new_features = Features()
         # add features
-        features['input_ids'] = Sequence(Value(dtype='int64'), length=length)
+        new_features['input_ids'] = Sequence(Value(dtype='int64'), length=length)
         if self.config.return_token_type_ids:
-            features['token_type_ids'] = Sequence(Value(dtype='int64'), length=length)
+            new_features['token_type_ids'] = Sequence(Value(dtype='int64'), length=length)
         if self.config.return_attention_mask:
-            features['attention_mask'] = Sequence(Value(dtype='int32'), length=length)
+            new_features['attention_mask'] = Sequence(Value(dtype='int32'), length=length)
         if self.config.return_overflowing_tokens:
-            features['overflowing_tokens'] = Sequence(Value(dtype='string'))
-            features['num_truncated_tokens'] = Value(dtype='int32')
+            new_features['overflowing_tokens'] = Sequence(Value(dtype='string'))
+            new_features['num_truncated_tokens'] = Value(dtype='int32')
         if self.config.return_special_tokens_mask:
-            features['special_tokens_mask'] = Sequence(Value(dtype='int32'), length=length)
+            new_features['special_tokens_mask'] = Sequence(Value(dtype='int32'), length=length)
         if self.config.return_special_tokens_mask:
-            features['special_tokens_mask'] = Sequence(Value(dtype='int32'), length=length)
+            new_features['special_tokens_mask'] = Sequence(Value(dtype='int32'), length=length)
         if self.config.return_length:
-            features['length'] = Value(dtype='int32')
+            new_features['length'] = Value(dtype='int32')
         if self.config.return_word_ids:
-            features['word_ids'] = Sequence(Value(dtype='int32'), length=length)
+            new_features['word_ids'] = Sequence(Value(dtype='int32'), length=length)
         # return updated features
-        return features
+        return new_features
 
     @property
     def tokenization_kwargs(self) -> dict:
         kwargs = asdict(self.config)
         kwargs.pop('processor_type')
         kwargs.pop('pretrained_ckpt')
         kwargs.pop('text_column')
```

### Comparing `hyped-0.0.3/hyped/scripts/evaluate.py` & `hyped-0.0.4/hyped/scripts/evaluate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import json
-import torch
 import hyped
 import datasets
 import logging
 # utils
-from hyped.scripts.train import build_trainer
-from hyped.scripts.utils.configs import RunConfig
+from itertools import product
+from hyped.scripts.train import (
+    RunConfig,
+    build_trainer,
+    load_data_split
+)
 
 logger = logging.getLogger(__name__)
 
 def main():
     from argparse import ArgumentParser
     # build argument parser
     parser = ArgumentParser(description="Train Transformer model on prepared datasets")
@@ -30,42 +33,52 @@
     config = RunConfig.parse_file(args.config)
 
     # prepare config for evaluation
     config.trainer.save_strategy = 'no'
     # not used but created and there is no way around i guess
     config.trainer.output_dir = os.path.join("/tmp", config.trainer.output_dir)
 
-    # load model and activate all heads
+    # load model and activate first adapter and all heads
     model = hyped.modeling.HypedAutoAdapterModel.from_pretrained(args.model_ckpt)
-    model.active_heads = list(model.heads.keys())
-    # build trainer but we're only using it for evaluation
-    trainer = build_trainer(
-        model=model,
-        args=config.trainer,
-        metrics_kwargs=config.metrics,
-        disable_tqdm=False
-    )
+    # ativate adapter
+    if config.model.adapter is not None:
+        # fallback to first adapter in model
+        adapter = config.model.adapter_name or next(iter(model.config.adapters))
+        model.active_adapters = adapter
+    # activate all prediciton heads
+    model.active_heads = list(config.model.heads.keys())
+
+    # trainer but we're only using it for evaluation
+    trainer = None
 
     # create directory to save metrics in
     fpath = os.path.join(args.model_ckpt, "metrics")
     fpath = args.out_dir if args.out_dir is not None else fpath
     os.makedirs(fpath, exist_ok=True)
 
-    for dpath in args.data:
-        # load data dump
-        dump = torch.load(dpath)
-        name = dump.name
+    for path, split in product(args.data, args.splits):
+        # load dataset
+        data = load_data_split(path, split)
+        name = data.info.builder_name
+
+        # build trainer on first iteration
+        trainer = trainer or build_trainer(
+            trainer_t=config.model.trainer_t,
+            model=model,
+            args=config.trainer,
+            features=data.features,
+            metric_configs=config.metrics,
+            disable_tqdm=False
+        )
         # log dataset to evaluate
         logger.info("Evaluating dataset %s" % name)
 
-        for split in args.splits:
-            if split in dump.datasets:
-                # evaluate model on dataset
-                metrics = trainer.evaluate(dump.datasets[split], metric_key_prefix=split)
-                logger.info(metrics)
-                # save metrics in checkpoint directory
-                with open(os.path.join(fpath, "%s-%s.json" % (name, split)), 'w+') as f:
-                    f.write(json.dumps(metrics, indent=2))
+        # evaluate model on dataset
+        metrics = trainer.evaluate(data, metric_key_prefix=split)
+        logger.info(metrics)
+        # save metrics in checkpoint directory
+        with open(os.path.join(fpath, "%s-%s.json" % (name, split)), 'w+') as f:
+            f.write(json.dumps(metrics, indent=2))
 
 if __name__ == '__main__':
     logging.basicConfig(level=logging.INFO)
     main()
```

### Comparing `hyped-0.0.3/hyped/scripts/prepare.py` & `hyped-0.0.4/hyped/scripts/prepare.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,87 @@
-"""Script to prepare a dataset.
-
-Dataset Preparation consists of the following steps:
-    0. download raw data (if necessary)
-    1. apply data processor
-    2. filter dataset
-    3. convert to faster data format (NamedTensorDataset)
-"""
 import os
 import hyped
-import torch
 import datasets
 import transformers
 import numpy as np
+import pydantic
 import logging
+# register packaged datasets
+import hyped.datasets
 # utils
-from hyped.scripts.utils.data import NamedTensorDataset, DataDump
-from hyped.scripts.utils.configs import PrepareConfig
+from typing_extensions import Annotated
 
 logger = logging.getLogger(__name__)
 
+class DataConfig(pydantic.BaseModel):
+    """Data Configuration Model"""
+    dataset:str
+    splits:dict[str, str] = {
+        datasets.Split.TRAIN: datasets.Split.TRAIN,
+        datasets.Split.VALIDATION: datasets.Split.VALIDATION,
+        datasets.Split.TEST: datasets.Split.TEST
+    }
+    kwargs:dict = {}
+
+    @pydantic.root_validator(pre=False)
+    def _check_dataset(cls, v):
+
+        if v.get('dataset', None) is None:
+            raise ValueError("No Dataset provided by configuration!")
+        try:
+            # try to load dataset builder
+            builder = datasets.load_dataset_builder(v['dataset'], **v['kwargs'])
+            return v
+        except FileNotFoundError as e:
+            # raise exception if dataset builder cannot be found
+            raise ValueError("Dataset not found: %s" % v) from e
+
+    @pydantic.validator('kwargs')
+    def _prepare_kwargs(cls, v):
+        if 'data_files' in v:
+            data_files = v['data_files']
+            # make data files absolut paths
+            if isinstance(data_files, str):
+                data_files = os.path.abspath(data_files)
+            elif isinstance(data_files, (tuple, list)):
+                data_files = [os.path.abspath(f) for f in data_files]
+            elif isinstance(data_files, dict):
+                data_files = {k: os.path.abspath(f) for k,f in data_files.items()}
+            # update data files
+            v['data_files'] = data_files
+        return v
+
+class PrepareConfig(pydantic.BaseModel):
+    """Data Configuration Model"""
+    # dataset config
+    data:DataConfig
+    # preprocessing pipeline
+    pipeline:list[
+        Annotated[
+            hyped.pipeline.AnyProcessorConfig,
+            pydantic.Field(..., discriminator='processor_type')
+        ]
+    ]
+    filters:list[hyped.pipeline.AnyFilterConfig]
+    # columns to keep
+    columns:dict[str, str]
+
+    # data filters
+    #filters:list[
+    #    Annotated[
+    #        hyped.AnyFilterConfig,
+    #        pydantic.Field(..., discriminator='filter_type')
+    #    ]
+    #]
+
 def prepare_dataset(
     ds:datasets.DatasetDict,
     config:PrepareConfig,
     max_size:int | None =None,
-) -> DataDump:
+) -> datasets.DatasetDict:
 
     # get dataset info
     info = next(iter(ds.values())).info
 
     # create pipeline
     pipe = hyped.pipeline.Pipeline(
         processors=config.pipeline,
@@ -40,56 +94,45 @@
             logger.info("Sampling %s/%s data points from %s split" % (max_size, len(d), s))
             idx = np.random.choice(len(d), max_size, replace=False)
             ds[s] = d.select(idx)
 
     # prepare pipeline and pass datasets through
     features = pipe.prepare(info.features)
     ds = pipe(ds)
+    # check features
+    assert features == next(iter(ds.values())).features
 
     # rename columns
     for t, s in config.columns.items():
         if t != s:
             ds = ds.rename_column(s, t)
+
     # set data format to torch
     ds.set_format(type='torch', columns=list(config.columns.keys()))
 
     # get data schema after pipeline, column renaming and formatting
     features = datasets.Features({t: features[s] for t, s in config.columns.items()})
     logger.debug("Dataset Features: %s" % str(features))
 
     # log some info
     logger.info("Data Preprocessing Complete.")
     for s, d in ds.items():
         logger.info("Generated %s split of %i documents" % (s, len(d)))
 
-    # check if all features are stackable
-    for n, f in features.items():
-        if isinstance(f, datasets.Sequence) and (f.length == -1):
-            logger.info("Feature %s has undefined length, cannot converting to Tensor Dataset!" % n)
-            break
-    else:
-        # convert to tensor dataset as all sequences have fixed length
-        return DataDump(
-            name=info.builder_name,
-            features=features,
-            datasets={s: NamedTensorDataset.from_dataset(d) for s, d in ds.items()}
-        )
-
-    # return as is
-    return DataDump(name=info.builder_name, features=features, datasets=ds)
+    return ds
 
 
 def main():
     from argparse import ArgumentParser
     # build argument parser
     parser = ArgumentParser(description="Prepare dataset for training")
     parser.add_argument("-c", "--config", type=str, required=True, help="Path to run configuration file in .json format")
     parser.add_argument("-n", "--max-size", type=int, default=None, help="Maximum number of data points per split")
     parser.add_argument("-s", "--splits", type=str, nargs='*', default=[], help="Subset of data splits to prepare")
-    parser.add_argument("-o", "--out-file", type=str, required=True, help="File to store prepared dataset in")
+    parser.add_argument("-o", "--out-dir", type=str, required=True, help="Path to store prepared dataset in")
     # parse arguments
     args = parser.parse_args()
 
     # check if config exists
     if not os.path.isfile(args.config):
         raise FileNotFoundError(args.config)
 
@@ -112,18 +155,16 @@
         split=config.data.splits,
         **config.data.kwargs
     )
     # prepare dataset
     logger.info("Preparing dataset splits")
     ds = prepare_dataset(ds, config, max_size=args.max_size)
 
-    # save data splits to file
-    logger.info("Saving dataset to %s" % args.out_file)
-    # create output directory
-    dirname = os.path.dirname(args.out_file)
-    if len(dirname) > 0:
-        os.makedirs(os.path.dirname(args.out_file), exist_ok=True)
-    torch.save(ds, args.out_file)
+    # convert dataset dict keys to string for save to disk
+    ds = datasets.DatasetDict({str(k): d for k, d in ds.items()})
+    # save dataset to disk
+    logger.info("Saving dataset to %s" % args.out_dir)
+    ds.save_to_disk(args.out_dir)
 
 if __name__ == '__main__':
     logging.basicConfig(level=logging.INFO)
     main()
```

### Comparing `hyped-0.0.3/hyped/utils/typedlist.py` & `hyped-0.0.4/hyped/utils/typedlist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/hyped/utils/typedmapping.py` & `hyped-0.0.4/hyped/utils/typedmapping.py`

 * *Files identical despite different names*

### Comparing `hyped-0.0.3/hyped.egg-info/PKG-INFO` & `hyped-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyped
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of data pipelines to ease the training of transformer models
 Home-page: https://github.com/ndoll1998/hyped/tree/master
 Author: Niclas Doll
 Author-email: niclas@amazonis.net
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
@@ -51,34 +51,51 @@
 ```bash
 # data preparation stage
 # runs the data preparation pipeline specified in the
 # configuration file and saves the prepared dataset
 # to the specified location
 python -m hyped.scripts.prepare \
     -c examples/text_cls/imdb/distilbert_data.json \
-    -o output/distilbert_data.bin
+    -o output/distilbert_data
 
 # model training stage
 # trains a model on the prepared data generated by the
 # previous stage
 python -m hyped.scripts.train \
     -c examples/text_cls/imdb/distilbert_run.json \
-    -d output/distilbert_data.bin \
+    -d output/distilbert_data \
     -o output/model
 
 # model evaluation stage
 # evaluates the trained model on the test split of the
 # prepared dataset generated earlier
 python -m hyped.scripts.evaluate \
     -c examples/text_cls/imdb/distilbert_run.json \
-    -d output/distilbert_data.bin \
+    -d output/distilbert_data \
     -m output/model/best-model
 ```
 
 ## features
 
 `hyped` currently implements all components required to train and evaluate models for the following NLP tasks:
 
  - Text Classification
  - Named Entity Recognition
+ - Multi-label Classification
 
 
+## roadmap
+
+`hyped` is still in its very early stages. With time the goal is to make the framework applicable to a wide variety of tasks and setups. Planned features include the following:
+
+ - ~~support adapter training~~
+ - support more tasks
+   - Masked Language Modeling
+   - Causal Language Modeling
+   - nested Named Entity Recognition
+   - Question Answering
+ - support multi-modal encoders
+   - LayoutLM
+   - LiLT
+ - support distributed training/inference
+   - deepspeed
+   - pytorch DDP and FSDP
```

### Comparing `hyped-0.0.3/hyped.egg-info/SOURCES.txt` & `hyped-0.0.4/hyped.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,32 @@
 hyped.egg-info/PKG-INFO
 hyped.egg-info/SOURCES.txt
 hyped.egg-info/dependency_links.txt
 hyped.egg-info/requires.txt
 hyped.egg-info/top_level.txt
 hyped/datasets/__init__.py
 hyped/datasets/cas.py
+hyped/datasets/xcr.py
 hyped/evaluate/__init__.py
 hyped/evaluate/auto.py
+hyped/evaluate/collection.py
+hyped/evaluate/processors.py
 hyped/evaluate/metrics/__init__.py
 hyped/evaluate/metrics/base.py
 hyped/evaluate/metrics/cls.py
-hyped/evaluate/metrics/collection.py
-hyped/evaluate/metrics/tagging.py
+hyped/evaluate/metrics/mlc.py
+hyped/evaluate/metrics/seqeval.py
 hyped/modeling/__init__.py
 hyped/modeling/auto.py
+hyped/modeling/collator.py
 hyped/modeling/trainer.py
 hyped/modeling/heads/__init__.py
 hyped/modeling/heads/base.py
 hyped/modeling/heads/cls.py
+hyped/modeling/heads/mlc.py
 hyped/modeling/heads/tagging.py
 hyped/pipeline/__init__.py
 hyped/pipeline/auto.py
 hyped/pipeline/pipeline.py
 hyped/pipeline/filters/__init__.py
 hyped/pipeline/filters/base.py
 hyped/pipeline/filters/msl.py
@@ -33,13 +38,10 @@
 hyped/pipeline/processors/base.py
 hyped/pipeline/processors/bio.py
 hyped/pipeline/processors/tokenizer.py
 hyped/scripts/__init__.py
 hyped/scripts/evaluate.py
 hyped/scripts/prepare.py
 hyped/scripts/train.py
-hyped/scripts/utils/__init__.py
-hyped/scripts/utils/configs.py
-hyped/scripts/utils/data.py
 hyped/utils/__init__.py
 hyped/utils/typedlist.py
 hyped/utils/typedmapping.py
```

### Comparing `hyped-0.0.3/setup.py` & `hyped-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hyped",
-    version="0.0.3",
+    version="0.0.4",
     description="A collection of data pipelines to ease the training of transformer models",
     long_description=open("README.md", "r").read(),
     long_description_content_type='text/markdown',
     author="Niclas Doll",
     author_email="niclas@amazonis.net",
     url="https://github.com/ndoll1998/hyped/tree/master",
     packages=find_packages(exclude='tests'),
```

