# Comparing `tmp/chrislab-0.5.1.tar.gz` & `tmp/chrislab-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.5.1.tar", last modified: Sun May 14 13:42:44 2023, max compression
+gzip compressed data, was "chrislab-0.5.2.tar", last modified: Thu May 18 18:31:14 2023, max compression
```

## Comparing `chrislab-0.5.1.tar` & `chrislab-0.5.2.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-12 08:42:23.000000 chrislab-0.5.1/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-14 13:42:44.617095 chrislab-0.5.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-05-12 08:42:23.000000 chrislab-0.5.1/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-12 08:42:23.000000 chrislab-0.5.1/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1203 2023-05-14 13:42:44.617095 chrislab-0.5.1/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/chrislab/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/chrislab/common/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/common/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/common/downloader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14529 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/common/tokenizer_korbert.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13164 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/common/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/chrislab/language/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/converter.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/evaluater.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/finetuner.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/modeling.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/chrislab/language/predictor.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/chrislab.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1442 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      164 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      249 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-14 13:42:44.000000 chrislab-0.5.1/src/chrislab.egg-info/zip-safe
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.613095 chrislab-0.5.1/src/nlpbook/
--rw-rw-r--   0 chris     (1000) chris     (1000)       70 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6033 2023-05-14 13:30:52.000000 chrislab-0.5.1/src/nlpbook/arguments.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/cls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/cls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5289 2023-05-14 13:16:43.000000 chrislab-0.5.1/src/nlpbook/cls/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5726 2023-05-14 13:15:00.000000 chrislab-0.5.1/src/nlpbook/cls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1740 2023-05-14 13:20:25.000000 chrislab-0.5.1/src/nlpbook/cls/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/data_utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      663 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/generation/
--rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/generation/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/generation/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5371 2023-05-14 13:19:21.000000 chrislab-0.5.1/src/nlpbook/generation/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/generation/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-05-14 13:21:01.000000 chrislab-0.5.1/src/nlpbook/generation/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/ner/
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/ner/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7513 2023-05-14 13:16:43.000000 chrislab-0.5.1/src/nlpbook/ner/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    11914 2023-05-14 13:20:25.000000 chrislab-0.5.1/src/nlpbook/ner/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8099 2023-05-14 13:20:25.000000 chrislab-0.5.1/src/nlpbook/ner/task.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/paircls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/paircls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2656 2023-05-14 13:15:23.000000 chrislab-0.5.1/src/nlpbook/paircls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/paircls/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-14 13:42:44.617095 chrislab-0.5.1/src/nlpbook/qa/
--rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/qa/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/qa/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17104 2023-05-14 13:20:44.000000 chrislab-0.5.1/src/nlpbook/qa/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-12 08:42:23.000000 chrislab-0.5.1/src/nlpbook/qa/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-05-14 13:20:34.000000 chrislab-0.5.1/src/nlpbook/qa/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1468 2023-05-14 13:19:09.000000 chrislab-0.5.1/src/nlpbook/trainer.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8696 2023-05-12 08:57:23.000000 chrislab-0.5.1/src/nlpbook/utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-14 13:51:34.000000 chrislab-0.5.2/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-18 18:31:14.963521 chrislab-0.5.2/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-05-14 13:51:34.000000 chrislab-0.5.2/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-14 13:51:34.000000 chrislab-0.5.2/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1203 2023-05-18 18:31:14.963521 chrislab-0.5.2/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/chrislab/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/chrislab/common/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/common/__init__.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/common/downloader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12638 2023-05-16 05:20:42.000000 chrislab-0.5.2/src/chrislab/common/tokenizer_korbert.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13164 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/common/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/chrislab/language/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/converter.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/evaluater.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/finetuner.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/modeling.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/chrislab/language/predictor.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.959521 chrislab-0.5.2/src/chrislab.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      830 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1420 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      164 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      249 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-18 18:31:14.000000 chrislab-0.5.2/src/chrislab.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       95 2023-05-18 12:07:19.000000 chrislab-0.5.2/src/nlpbook/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8521 2023-05-18 18:19:49.000000 chrislab-0.5.2/src/nlpbook/arguments.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/cls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/cls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8870 2023-05-18 17:57:18.000000 chrislab-0.5.2/src/nlpbook/cls/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5208 2023-05-18 14:04:27.000000 chrislab-0.5.2/src/nlpbook/cls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2674 2023-05-18 17:12:36.000000 chrislab-0.5.2/src/nlpbook/cls/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/data_utils.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3438 2023-05-18 17:45:48.000000 chrislab-0.5.2/src/nlpbook/factory.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/generation/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/generation/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/generation/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5371 2023-05-18 08:22:09.000000 chrislab-0.5.2/src/nlpbook/generation/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/generation/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1293 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/generation/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/metrics.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/ner/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/ner/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8882 2023-05-18 17:57:18.000000 chrislab-0.5.2/src/nlpbook/ner/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    11551 2023-05-18 17:55:00.000000 chrislab-0.5.2/src/nlpbook/ner/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8528 2023-05-18 16:39:33.000000 chrislab-0.5.2/src/nlpbook/ner/task.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/paircls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/paircls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2656 2023-05-18 08:22:04.000000 chrislab-0.5.2/src/nlpbook/paircls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/paircls/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-18 18:31:14.963521 chrislab-0.5.2/src/nlpbook/qa/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/qa/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/qa/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17104 2023-05-18 08:22:15.000000 chrislab-0.5.2/src/nlpbook/qa/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/qa/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2072 2023-05-14 13:51:34.000000 chrislab-0.5.2/src/nlpbook/qa/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8635 2023-05-18 15:44:30.000000 chrislab-0.5.2/src/nlpbook/utils.py
```

### Comparing `chrislab-0.5.1/LICENSE` & `chrislab-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/PKG-INFO` & `chrislab-0.5.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.1
+Version: 0.5.2
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.1/setup.cfg` & `chrislab-0.5.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrislab
-version = 0.5.1
+version = 0.5.2
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `chrislab-0.5.1/src/chrislab/common/downloader.py` & `chrislab-0.5.2/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.2/src/chrislab/common/tokenizer_korbert.py`

 * *Files 18% similar despite different names*

```diff
@@ -149,84 +149,54 @@
             else:
                 output_tokens.extend(sub_tokens)
         return output_tokens
 
 
 if __name__ == "__main__":
     tokenizer1A = AutoTokenizer.from_pretrained(
-        "pretrained/KoELECTRA-Base-v3",
+        "/dat/proj/pretrained-com/KcELECTRA-Base",
         max_len=512,
         use_fast=True,
     )
     tokenizer1B = BertTokenizer(
-        vocab_file="pretrained/KoELECTRA-Base-v3/vocab.txt",
+        vocab_file="/dat/proj/pretrained-com/KcELECTRA-Base/vocab.txt",
         do_lower_case=False,
         tokenize_chinese_chars=False,
     )
     tokenizer2A = KorbertTokenizer.from_pretrained(
-        "pretrained/ELECTRA-morp20.05",
+        "/dat/proj/pretrained-pro/ETRI-ELECTRA-Base-morp20.05",
         max_len=512,
         use_fast=False,
         do_lower_case=False,
         tokenize_chinese_chars=False,
     )
     tokenizer2B = KorbertTokenizer(
-        vocab_file="pretrained/ELECTRA-morp20.05/vocab.txt",
+        vocab_file="/dat/proj/pretrained-pro/ETRI-ELECTRA-Base-morp20.05/vocab.txt",
         do_lower_case=False,
     )
     tokenizer3A = AutoTokenizer.from_pretrained(
-        "pretrained/RoBERTa-bbpe21.07-added",
+        "/dat/proj/pretrained-pro/ETRI-RoBERTa-Base-bbpe22.07",
         max_len=512,
         use_fast=False,
         do_lower_case=False,
     )
     tokenizer3B = RobertaTokenizer(
-        "pretrained/RoBERTa-bbpe21.07-added/vocab.json",
-        "pretrained/RoBERTa-bbpe21.07-added/merges.txt",
+        "/dat/proj/pretrained-pro/ETRI-RoBERTa-Base-bbpe22.07/vocab.json",
+        "/dat/proj/pretrained-pro/ETRI-RoBERTa-Base-bbpe22.07/merges.txt",
         max_len=512,
         use_fast=False,
         do_lower_case=False,
     )
     # https://github.com/huggingface/transformers/issues/1413#issuecomment-538083512
-    # tokenizer3A.add_tokens(["/NN", "/NP", "/NR", "/VV", "/VA",
-    #                         "/VX", "/VC", "/MM", "/MA", "/IC",
-    #                         "/JK", "/JX", "/JC", "/EP", "/EF",
-    #                         "/EC", "/ET", "/XP", "/XS", "/XR",
-    #                         "/SF", "/SP", "/SS", "/SE", "/SO",
-    #                         "/SW", "/SL", "/SH", "/SN"])
-    # tokenizer3A.add_tokens(["/NNG", "/NNP", "/NNB", "/NP", "/NR",
-    #                         "/VV", "/VA", "/VX", "/VCP", "/VCN",  # 10
-    #                         "/MM", "/MAG", "/MAJ", "/IC",  # 14
-    #                         "/JKS", "/JKC", "/JKG", "/JKO", "/JKB",  # 19
-    #                         "/JKV", "/JKQ", "/JX", "/JC",  # 23
-    #                         "/EP", "/EF", "/EC", "/ETN", "/ETM",  # 28
-    #                         "/XPN", "/XSN", "/XSV", "/XSA", "/XR",  # 33
-    #                         "/SF", "/SP", "/SS", "/SE", "/SO",  # 38
-    #                         "/SW", "/SL", "/SH", "/SN"])  # 42
-    bbpe_tokenizer = ByteLevelBPETokenizer("pretrained/RoBERTa-bbpe21.07-added/vocab.json", "pretrained/RoBERTa-bbpe21.07-added/merges.txt", lowercase=False)
-    # bbpe_tokenizer.add_tokens(["/NN", "/NP", "/NR", "/VV", "/VA",
-    #                            "/VX", "/VC", "/MM", "/MA", "/IC",
-    #                            "/JK", "/JX", "/JC", "/EP", "/EF",
-    #                            "/EC", "/ET", "/XP", "/XS", "/XR",
-    #                            "/SF", "/SP", "/SS", "/SE", "/SO",
-    #                            "/SW", "/SL", "/SH", "/SN"])
-    # bbpe_tokenizer.add_tokens(["/NNG", "/NNP", "/NNB", "/NP", "/NR",
-    #                            "/VV", "/VA", "/VX", "/VCP", "/VCN",  # 10
-    #                            "/MM", "/MAG", "/MAJ", "/IC",  # 14
-    #                            "/JKS", "/JKC", "/JKG", "/JKO", "/JKB",  # 19
-    #                            "/JKV", "/JKQ", "/JX", "/JC",  # 23
-    #                            "/EP", "/EF", "/EC", "/ETN", "/ETM",  # 28
-    #                            "/XPN", "/XSN", "/XSV", "/XSA", "/XR",  # 33
-    #                            "/SF", "/SP", "/SS", "/SE", "/SO",  # 38
-    #                            "/SW", "/SL", "/SH", "/SN"])  # 42
+    bbpe_tokenizer = ByteLevelBPETokenizer("/dat/proj/pretrained-pro/ETRI-RoBERTa-Base-bbpe22.07/vocab.json", "/dat/proj/pretrained-pro/ETRI-RoBERTa-Base-bbpe22.07/merges.txt", lowercase=False)
     print(f"tokenizer3A(#={len(tokenizer3A)})({type(tokenizer3A)}) = {tokenizer3A}")
     print(f"tokenizer3B(#={len(tokenizer3B)})({type(tokenizer3B)}) = {tokenizer3B}")
     print(f"bbpe_tokenizer()({type(bbpe_tokenizer)}) = {bbpe_tokenizer}")
     vocab_items = []
-    with Path("pretrained/RoBERTa-bbpe21.07-added/vocab.json").open() as inp, Path("pretrained/RoBERTa-bbpe21.07-added/vocab_items.txt").open('w') as out:
+    with Path("/dat/proj/pretrained-pro/ETRI-RoBERTa-Base-bbpe22.07/vocab.json").open() as inp, Path("/dat/proj/pretrained-pro/ETRI-RoBERTa-Base-bbpe22.07/vocab_items.txt").open('w') as out:
         for t, i in list(json.load(inp).items()):
             vocab_items.append({
                 'id': i,
                 'encoded': t,
                 'decoded': no_space(no_replacement(no_nonprintable(bbpe_tokenizer.decode([i]))))
             })
         out.writelines([f"{x['id']}\t{x['encoded']}\t{x['decoded']}\n" for x in vocab_items])
@@ -239,34 +209,34 @@
     sentence2_lemma = "지금 까지 금해 졌 다 ."
 
     # plain = "[CLS] 한국어 사전학습 모델을 공유합니다. [SEP] 지금까지 금해졌다."
     # morps = "[CLS] 한국어/NNP 사전/NNG 학습/NNG 모델/NNG 을/JKO 공유/NNG 하/XSV ㅂ니다/EF ./SF [SEP] 지금/NNG 까지/JX 금하/VV 어/EC 지/VX 었/EP 다/EF ./SF"
     # print(f"plain={plain}")
     # print(f"morps={morps}")
 
-    # print('tokenizer1A:', tokenizer1A.cls_token, tokenizer1A.cls_token_id, tokenizer1A.sep_token, tokenizer1A.sep_token_id, tokenizer1A.pad_token, tokenizer1A.pad_token_id)
-    # print('tokenizer2A:', tokenizer2A.cls_token, tokenizer2A.cls_token_id, tokenizer2A.sep_token, tokenizer2A.sep_token_id, tokenizer2A.pad_token, tokenizer2A.pad_token_id)
+    print('tokenizer1A:', tokenizer1A.cls_token, tokenizer1A.cls_token_id, tokenizer1A.sep_token, tokenizer1A.sep_token_id, tokenizer1A.pad_token, tokenizer1A.pad_token_id)
+    print('tokenizer2A:', tokenizer2A.cls_token, tokenizer2A.cls_token_id, tokenizer2A.sep_token, tokenizer2A.sep_token_id, tokenizer2A.pad_token, tokenizer2A.pad_token_id)
     print('tokenizer3A:', tokenizer3A.cls_token, tokenizer3A.cls_token_id, tokenizer3A.sep_token, tokenizer3A.sep_token_id, tokenizer3A.pad_token, tokenizer3A.pad_token_id)
 
 
     def tokenized_ids(tokenized):
         return ' '.join(map(lambda x: f'{x:05d}',
                             tokenizer3A.convert_tokens_to_ids(tokenized)))
 
 
     def tokenized_lemmas(tokenized):
         return ' '.join(map(lambda x: no_space(no_replacement(no_nonprintable(bbpe_tokenizer.decode([x])))),
                             tokenizer3A.convert_tokens_to_ids(tokenized)))
 
 
     print(f"tokens from plain={tokenizer1A.tokenize(f'{tokenizer1A.cls_token} {sentence1_plain} {tokenizer1A.sep_token} {sentence2_plain} {tokenizer1A.pad_token}')}")
-    # print(f"tokens from plain={tokenizer1B.tokenize(f'{tokenizer1B.cls_token} {sentence1_plain} {tokenizer1B.sep_token} {sentence2_plain} {tokenizer1B.pad_token}')}")
+    print(f"tokens from plain={tokenizer1B.tokenize(f'{tokenizer1B.cls_token} {sentence1_plain} {tokenizer1B.sep_token} {sentence2_plain} {tokenizer1B.pad_token}')}")
 
     print(f"tokens from morps={tokenizer2A.tokenize(f'{tokenizer2A.cls_token} {sentence1_morps} {tokenizer2A.sep_token} {sentence2_morps} {tokenizer2A.pad_token}')}")
-    # print(f"tokens from morps={tokenizer2B.tokenize(f'{tokenizer2B.cls_token} {sentence1_morps} {tokenizer2B.sep_token} {sentence2_morps} {tokenizer2B.pad_token}')}")
+    print(f"tokens from morps={tokenizer2B.tokenize(f'{tokenizer2B.cls_token} {sentence1_morps} {tokenizer2B.sep_token} {sentence2_morps} {tokenizer2B.pad_token}')}")
 
     print(f"tokens from plain={tokenizer3A.tokenize(f'{tokenizer3A.cls_token} {sentence1_plain} {tokenizer3A.sep_token} {sentence2_plain} {tokenizer3A.pad_token}')}")
     print(f"tokens from lemma={tokenizer3A.tokenize(f'{tokenizer3A.cls_token} {sentence1_lemma} {tokenizer3A.sep_token} {sentence2_lemma} {tokenizer3A.pad_token}')}")
     print(f"tokens from morps={tokenizer3A.tokenize(f'{tokenizer3A.cls_token} {sentence1_morps} {tokenizer3A.sep_token} {sentence2_morps} {tokenizer3A.pad_token}')}")
 
     print(f"plain -> tokenize(#={len(tokenizer3A.tokenize(f'{tokenizer3A.cls_token} {sentence1_plain} {tokenizer3A.sep_token} {sentence2_plain} {tokenizer3A.pad_token}'))}) -> tokens_to_ids -> str"
           f" = {tokenized_ids(tokenizer3A.tokenize(f'{tokenizer3A.cls_token} {sentence1_plain} {tokenizer3A.sep_token} {sentence2_plain} {tokenizer3A.pad_token}'))}")
```

### Comparing `chrislab-0.5.1/src/chrislab/common/util.py` & `chrislab-0.5.2/src/chrislab/common/util.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/chrislab/language/cli.py` & `chrislab-0.5.2/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/chrislab/language/converter.py` & `chrislab-0.5.2/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/chrislab/language/evaluater.py` & `chrislab-0.5.2/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/chrislab/language/finetuner.py` & `chrislab-0.5.2/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/chrislab/language/modeling.py` & `chrislab-0.5.2/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/chrislab/language/predictor.py` & `chrislab-0.5.2/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.2/src/chrislab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.5.1
+Version: 0.5.2
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrislab-0.5.1/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.2/src/chrislab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 src/chrislab/language/evaluater.py
 src/chrislab/language/finetuner.py
 src/chrislab/language/modeling.py
 src/chrislab/language/predictor.py
 src/nlpbook/__init__.py
 src/nlpbook/arguments.py
 src/nlpbook/data_utils.py
-src/nlpbook/deploy.py
+src/nlpbook/factory.py
 src/nlpbook/metrics.py
-src/nlpbook/trainer.py
 src/nlpbook/utils.py
 src/nlpbook/cls/__init__.py
 src/nlpbook/cls/cli.py
 src/nlpbook/cls/corpus.py
 src/nlpbook/cls/task.py
 src/nlpbook/generation/__init__.py
 src/nlpbook/generation/arguments.py
```

### Comparing `chrislab-0.5.1/src/nlpbook/cls/corpus.py` & `chrislab-0.5.2/src/nlpbook/cls/corpus.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from pathlib import Path
 from typing import List, Optional
 
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
-from nlpbook.arguments import NLUTrainerArguments
+from nlpbook.arguments import TrainerArguments, TesterArguments
 from transformers import PreTrainedTokenizer
 
-logger = logging.getLogger("ratsnlp")
+logger = logging.getLogger("nlpbook")
 
 
 @dataclass
 class ClassificationExample:
     text_a: str
     text_b: Optional[str] = None
     label: Optional[str] = None
@@ -32,18 +32,17 @@
 
 
 class NsmcCorpus:
 
     def __init__(self):
         pass
 
-    def get_examples(self, data_root_path, mode):
-        data_fpath = os.path.join(data_root_path, f"ratings_{mode}.txt")
-        logger.info(f"loading {mode} data... LOOKING AT {data_fpath}")
-        lines = list(csv.reader(open(data_fpath, "r", encoding="utf-8"), delimiter="\t", quotechar='"'))
+    def get_examples(self, data_path):
+        logger.info(f"loading data from {data_path}...")
+        lines = list(csv.reader(open(data_path, "r", encoding="utf-8"), delimiter="\t", quotechar='"'))
         examples = []
         for (i, line) in enumerate(lines):
             if i == 0:
                 continue
             _, text_a, label = line
             examples.append(ClassificationExample(text_a=text_a, text_b=None, label=label))
         return examples
@@ -52,44 +51,40 @@
         return ["0", "1"]
 
     @property
     def num_labels(self):
         return len(self.get_labels())
 
 
-def _convert_examples_to_classification_features(
+def _convert_examples_to_cls_features(
         examples: List[ClassificationExample],
         tokenizer: PreTrainedTokenizer,
-        args: NLUTrainerArguments,
+        args: TrainerArguments,
         label_list: List[str],
 ):
     label_map = {label: i for i, label in enumerate(label_list)}
     labels = [label_map[example.label] for example in examples]
 
-    logger.info(
-        "tokenize sentences, it could take a lot of time..."
-    )
+    logger.info("tokenize sentences, it could take a lot of time...")
     start = time.time()
     batch_encoding = tokenizer(
         [(example.text_a, example.text_b) for example in examples],
-        max_length=args.max_seq_length,
+        max_length=args.model.max_seq_length,
         padding="max_length",
         truncation=True,
     )
-    logger.info(
-        "tokenize sentences [took %.3f s]", time.time() - start
-    )
+    logger.info("tokenize sentences [took %.3f s]", time.time() - start)
 
     features = []
     for i in range(len(examples)):
         inputs = {k: batch_encoding[k][i] for k in batch_encoding}
         feature = ClassificationFeatures(**inputs, label=labels[i])
         features.append(feature)
 
-    for i, example in enumerate(examples[:5]):
+    for i, example in enumerate(examples[:3]):
         logger.info("*** Example ***")
         if example.text_b is None:
             logger.info("sentence: %s" % (example.text_a))
         else:
             sentence = example.text_a + " + " + example.text_b
             logger.info("sentence A, B: %s" % (sentence))
         logger.info("tokens: %s" % (" ".join(tokenizer.convert_ids_to_tokens(features[i].input_ids))))
@@ -99,72 +94,48 @@
     return features
 
 
 class ClassificationDataset(Dataset):
 
     def __init__(
             self,
-            args: NLUTrainerArguments,
+            split: str,
+            args: TrainerArguments | TesterArguments,
             tokenizer: PreTrainedTokenizer,
-            corpus,
-            mode: Optional[str] = "train",
-            convert_examples_to_features_fn=_convert_examples_to_classification_features,
+            corpus: NsmcCorpus,
+            convert_examples_to_features_fn=_convert_examples_to_cls_features,
     ):
-        if corpus is not None:
-            self.corpus = corpus
-        else:
-            raise KeyError("corpus is not valid")
-        if not mode in ["train", "val", "test"]:
-            raise KeyError(f"mode({mode}) is not a valid split name")
-        # Load data features from cache or dataset file
-        cached_features_file = os.path.join(
-            args.downstream_data_home,
-            args.downstream_data_name,
-            "cached_{}_{}_{}_{}_{}".format(
-                Path(args.downstream_data_file).stem,
-                tokenizer.__class__.__name__,
-                str(args.max_seq_length),
-                args.downstream_data_name,
-                args.downstream_task_name,
-            ),
-        )
-
-        # Make sure only the first process in distributed training processes the dataset,
-        # and the others will use the cache.
-        lock_path = cached_features_file + ".lock"
-        with FileLock(lock_path):
+        assert corpus, "corpus is not valid"
+        self.corpus = corpus
+
+        assert args.data.home, f"No data_home: {args.data.home}"
+        assert args.data.name, f"No data_name: {args.data.name}"
+        data_file_dict: dict = args.data.files.to_dict()
+        assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
+        assert data_file_dict[split], f"No data_file for '{split}' split: {args.data.files}"
+        text_data_path: Path = Path(args.data.home) / args.data.name / data_file_dict[split]
+        cache_data_path = text_data_path \
+            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-with-{args.model.max_seq_length}") \
+            .with_suffix(".cache")
+        cache_lock_path = cache_data_path.with_suffix(".lock")
 
-            if os.path.exists(cached_features_file) and not args.overwrite_cache:
+        with FileLock(cache_lock_path):
+            if os.path.exists(cache_data_path) and args.data.caching:
                 start = time.time()
-                self.features = torch.load(cached_features_file)
-                logger.info(
-                    f"Loading features from cached file {cached_features_file} [took %.3f s]", time.time() - start
-                )
+                self.features = torch.load(cache_data_path)
+                logger.info(f"Loading features from cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
             else:
-                corpus_path = os.path.join(
-                    args.downstream_data_home,
-                    args.downstream_data_name,
-                    args.downstream_data_file,
-                )
-                logger.info(f"Creating features from dataset file at {corpus_path}")
-                examples = self.corpus.get_examples(corpus_path)
-                self.features = convert_examples_to_features_fn(
-                    examples,
-                    tokenizer,
-                    args,
-                    label_list=self.corpus.get_labels(),
-                )
+                assert text_data_path.exists() and text_data_path.is_file(), f"No data_text_path: {text_data_path}"
+                logger.info(f"Creating features from dataset file at {text_data_path}")
+                examples = self.corpus.get_examples(text_data_path)
+                self.features = convert_examples_to_features_fn(examples, tokenizer, args, label_list=self.corpus.get_labels())
                 start = time.time()
-                logger.info(
-                    "Saving features into cached file, it could take a lot of time..."
-                )
-                torch.save(self.features, cached_features_file)
-                logger.info(
-                    "Saving features into cached file %s [took %.3f s]", cached_features_file, time.time() - start
-                )
+                logger.info("Saving features into cached file, it could take a lot of time...")
+                torch.save(self.features, cache_data_path)
+                logger.info(f"Saving features into cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
 
     def __len__(self):
         return len(self.features)
 
     def __getitem__(self, i):
         return self.features[i]
```

### Comparing `chrislab-0.5.1/src/nlpbook/data_utils.py` & `chrislab-0.5.2/src/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/generation/arguments.py` & `chrislab-0.5.2/src/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/generation/corpus.py` & `chrislab-0.5.2/src/nlpbook/generation/corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
 from nlpbook.generation.arguments import GenerationTrainArguments
 from transformers import PreTrainedTokenizerFast
 
-logger = logging.getLogger("ratsnlp")
+logger = logging.getLogger("nlpbook")
 
 
 @dataclass
 class GenerationExample:
     text: str
```

### Comparing `chrislab-0.5.1/src/nlpbook/generation/deploy.py` & `chrislab-0.5.2/src/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/generation/task.py` & `chrislab-0.5.2/src/nlpbook/generation/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/metrics.py` & `chrislab-0.5.2/src/nlpbook/metrics.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/ner/cli.py` & `chrislab-0.5.2/src/nlpbook/ner/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,147 +1,164 @@
+import logging
 from pathlib import Path
 
+import pytorch_lightning as pl
 import torch
+from flask import Flask
+from torch import Tensor
 from torch.utils.data import DataLoader, RandomSampler
 from torch.utils.data import SequentialSampler
 from typer import Typer
 
-from chrisbase.io import JobTimer, out_hr
 import nlpbook
-from nlpbook.arguments import NLUTrainerArguments, NLUServerArguments, NLUTesterArguments
-from nlpbook.deploy import get_web_service_app
+from chrisbase.io import JobTimer, err_hr
+from nlpbook.arguments import TrainerArguments, ServerArguments, TesterArguments, RuntimeChecking
 from nlpbook.ner.corpus import NERCorpus, NERDataset
 from nlpbook.ner.task import NERTask
-from transformers import BertConfig, BertForTokenClassification
-from transformers import BertTokenizer
+from transformers import BertConfig, BertForTokenClassification, BertTokenizer
+from transformers.modeling_outputs import TokenClassifierOutput
 
 app = Typer()
+logger = logging.getLogger("nlpbook")
 
 
 @app.command()
-def train_ner(config: Path | str):
-    config = Path(config)
-    assert config.exists(), f"No config file: {config}"
-    args = NLUTrainerArguments.from_json(config.read_text())
-    args.print_dataframe()
-
-    with JobTimer(f"chrialab.ratsnlp train_ner {config}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        nlpbook.set_seed(args)
-        nlpbook.set_logger()
+def train(args_file: Path | str):
+    nlpbook.set_logger()
+    args_file = Path(args_file)
+    assert args_file.exists(), f"No args_file: {args_file}"
+    args: TrainerArguments = TrainerArguments.from_json(args_file.read_text()).show()
+    nlpbook.set_seed(args)
+
+    with JobTimer(f"chrialab.nlpbook.ner train {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
         nlpbook.download_downstream_dataset(args)
-        out_hr(c='-')
+        err_hr(c='-')
 
         corpus = NERCorpus(args)
-        tokenizer = BertTokenizer.from_pretrained(args.pretrained_model_path, do_lower_case=False)
-        train_dataset = NERDataset(args=args, corpus=corpus, tokenizer=tokenizer)
+        # tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
+        # assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
+        tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
+        train_dataset = NERDataset("train", args=args, corpus=corpus, tokenizer=tokenizer)
         train_dataloader = DataLoader(train_dataset,
-                                      batch_size=args.batch_size,
+                                      batch_size=args.hardware.batch_size,
+                                      num_workers=args.hardware.cpu_workers,
                                       sampler=RandomSampler(train_dataset, replacement=False),
                                       collate_fn=nlpbook.data_collator,
-                                      drop_last=False,
-                                      num_workers=args.cpu_workers)
-        out_hr(c='-')
+                                      drop_last=False)
+        err_hr(c='-')
 
-        val_dataset = NERDataset(args=args, corpus=corpus, tokenizer=tokenizer)
+        val_dataset = NERDataset("valid", args=args, corpus=corpus, tokenizer=tokenizer)
         val_dataloader = DataLoader(val_dataset,
-                                    batch_size=args.batch_size,
+                                    batch_size=args.hardware.batch_size,
+                                    num_workers=args.hardware.cpu_workers,
                                     sampler=SequentialSampler(val_dataset),
                                     collate_fn=nlpbook.data_collator,
-                                    drop_last=False,
-                                    num_workers=args.cpu_workers)
-        out_hr(c='-')
+                                    drop_last=False)
+        err_hr(c='-')
 
         pretrained_model_config = BertConfig.from_pretrained(
-            args.pretrained_model_path,
+            args.model.pretrained,
             num_labels=corpus.num_labels
         )
         model = BertForTokenClassification.from_pretrained(
-            args.pretrained_model_path,
+            args.model.pretrained,
             config=pretrained_model_config
         )
-        out_hr(c='-')
+        err_hr(c='-')
 
-        torch.set_float32_matmul_precision('high')
-        nlpbook.get_trainer(args).fit(NERTask(model, args),
-                                      train_dataloaders=train_dataloader,
-                                      val_dataloaders=val_dataloader)
+        with RuntimeChecking(nlpbook.setup_csv_out(args)):
+            torch.set_float32_matmul_precision('high')
+            trainer: pl.Trainer = nlpbook.make_trainer(args)
+            trainer.fit(NERTask(model, args, trainer),
+                        train_dataloaders=train_dataloader,
+                        val_dataloaders=val_dataloader)
 
 
 @app.command()
-def test_ner(config: Path | str):
-    config = Path(config)
-    assert config.exists(), f"No config file: {config}"
-    args = NLUTesterArguments.from_json(config.read_text())
-    args.print_dataframe()
-
-    with JobTimer(f"chrialab.ratsnlp test_ner {config}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        downstream_model_path = args.downstream_model_home / args.downstream_model_file
-        assert downstream_model_path.exists(), f"No downstream model file: {downstream_model_path}"
-        nlpbook.set_logger()
+def test(args_file: Path | str):
+    nlpbook.set_logger()
+    args_file = Path(args_file)
+    assert args_file.exists(), f"No args_file: {args_file}"
+    args = TesterArguments.from_json(args_file.read_text()).show()
+
+    with JobTimer(f"chrialab.nlpbook.ner test {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
+        checkpoint_path = args.output.dir_path / args.model.finetuning_name
+        assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
+        logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
+        err_hr(c='-')
+
         nlpbook.download_downstream_dataset(args)
-        out_hr(c='-')
+        err_hr(c='-')
 
         corpus = NERCorpus(args)
-        tokenizer = BertTokenizer.from_pretrained(args.pretrained_model_path, do_lower_case=False)
-        test_dataset = NERDataset(args=args, corpus=corpus, tokenizer=tokenizer)
+        # tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
+        # assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
+        tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
+        test_dataset = NERDataset("test", args=args, corpus=corpus, tokenizer=tokenizer)
         test_dataloader = DataLoader(test_dataset,
-                                     batch_size=args.batch_size,
+                                     batch_size=args.hardware.batch_size,
+                                     num_workers=args.hardware.cpu_workers,
                                      sampler=SequentialSampler(test_dataset),
                                      collate_fn=nlpbook.data_collator,
-                                     drop_last=False,
-                                     num_workers=args.cpu_workers)
-        out_hr(c='-')
+                                     drop_last=False)
+        err_hr(c='-')
 
         pretrained_model_config = BertConfig.from_pretrained(
-            args.pretrained_model_path,
+            args.model.pretrained,
             num_labels=corpus.num_labels
         )
         model = BertForTokenClassification.from_pretrained(
-            args.pretrained_model_path,
+            args.model.pretrained,
             config=pretrained_model_config
         )
-        out_hr(c='-')
+        err_hr(c='-')
 
-        torch.set_float32_matmul_precision('high')
-        nlpbook.get_tester(args).test(NERTask(model, args),
-                                      dataloaders=test_dataloader,
-                                      ckpt_path=downstream_model_path)
+        with RuntimeChecking(nlpbook.setup_csv_out(args)):
+            torch.set_float32_matmul_precision('high')
+            tester: pl.Trainer = nlpbook.make_tester(args)
+            tester.test(NERTask(model, args, tester),
+                        dataloaders=test_dataloader,
+                        ckpt_path=checkpoint_path)
 
 
 @app.command()
-def serve_ner(config: Path | str):
-    config = Path(config)
-    assert config.exists(), f"No config file: {config}"
-    args = NLUServerArguments.from_json(config.read_text())
-    args.print_dataframe()
-
-    with JobTimer(f"chrialab.ratsnlp serve_ner {config}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
-        downstream_model_path = args.downstream_model_home / args.downstream_model_file
-        assert downstream_model_path.exists(), f"No downstream model file: {downstream_model_path}"
-        downstream_model_ckpt = torch.load(downstream_model_path, map_location=torch.device("cpu"))
+def serve(args_file: Path | str):
+    nlpbook.set_logger()
+    args_file = Path(args_file)
+    assert args_file.exists(), f"No args_file file: {args_file}"
+    args: ServerArguments = ServerArguments.from_json(args_file.read_text()).show()
+
+    with JobTimer(f"chrialab.nlpbook serve_ner {args_file}", mt=1, mb=1, rt=1, rb=1, rc='=', verbose=True, flush_sec=0.3):
+        checkpoint_path = args.output.dir_path / args.model.finetuning_name
+        assert checkpoint_path.exists(), f"No checkpoint file: {checkpoint_path}"
+        checkpoint: dict = torch.load(checkpoint_path, map_location=torch.device("cpu"))
+        logger.info(f"Using finetuned checkpoint file at {checkpoint_path}")
+        err_hr(c='-')
+
+        # tokenizer: PreTrainedTokenizerFast = AutoTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False, use_fast=True)
+        # assert isinstance(tokenizer, PreTrainedTokenizerFast), f"tokenizer is not PreTrainedTokenizerFast: {type(tokenizer)}"
+        tokenizer: BertTokenizer = BertTokenizer.from_pretrained(args.model.pretrained, do_lower_case=False)
+        label_map_path: Path = args.output.dir_path / "label_map.txt"
+        assert label_map_path.exists(), f"No downstream label file: {label_map_path}"
+        labels = label_map_path.read_text().splitlines(keepends=False)
+        id_to_label = {idx: label for idx, label in enumerate(labels)}
+
         pretrained_model_config = BertConfig.from_pretrained(
-            args.pretrained_model_path,
-            num_labels=downstream_model_ckpt['state_dict']['model.classifier.bias'].shape.numel(),
+            args.model.pretrained,
+            num_labels=checkpoint['state_dict']['model.classifier.bias'].shape.numel(),
         )
         model = BertForTokenClassification(pretrained_model_config)
-        model.load_state_dict({k.replace("model.", ""): v for k, v in downstream_model_ckpt['state_dict'].items()})
+        model.load_state_dict({k.replace("model.", ""): v for k, v in checkpoint['state_dict'].items()})
         model.eval()
-
-        tokenizer = BertTokenizer.from_pretrained(args.pretrained_model_path, do_lower_case=False)
-        downstream_label_path: Path = args.downstream_model_home / "label_map.txt"
-        assert downstream_label_path.exists(), f"No downstream label file: {downstream_label_path}"
-        labels = downstream_label_path.read_text().splitlines(keepends=False)
-        id_to_label = {idx: label for idx, label in enumerate(labels)}
+        err_hr(c='-')
 
         def inference_fn(sentence):
-            from transformers.modeling_outputs import TokenClassifierOutput
-            from torch import Tensor
             inputs = tokenizer(
                 [sentence],
-                max_length=args.max_seq_length,
+                max_length=args.model.max_seq_length,
                 padding="max_length",
                 truncation=True,
             )
             with torch.no_grad():
                 outputs: TokenClassifierOutput = model(**{k: torch.tensor(v) for k, v in inputs.items()})
                 all_probs: Tensor = outputs.logits[0].softmax(dim=1)
                 top_probs, top_preds = torch.topk(all_probs, dim=1, k=1)
@@ -157,9 +174,12 @@
                         "prob": f"{round(top_prob[0].item(), 4):.4f}",
                     })
             return {
                 'sentence': sentence,
                 'result': result,
             }
 
-        service = get_web_service_app(inference_fn, template_file="serve_ner.html", ngrok_home=args.env.working_path)
-        service.run()
+        with RuntimeChecking(nlpbook.setup_csv_out(args)):
+            server: Flask = nlpbook.make_server(inference_fn,
+                                                template_file="serve_ner.html",
+                                                ngrok_home=args.env.working_path)
+            server.run()
```

### Comparing `chrislab-0.5.1/src/nlpbook/ner/corpus.py` & `chrislab-0.5.2/src/nlpbook/ner/corpus.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from pathlib import Path
 from typing import List, Optional
 
 import torch
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 
-from nlpbook.arguments import NLUTrainerArguments, NLUTesterArguments
+from chrisbase.io import make_parent_dir
+from nlpbook.arguments import TrainerArguments, TesterArguments
 from transformers import BertTokenizer
 from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy
 
-logger = logging.getLogger("ratsnlp")
+logger = logging.getLogger("nlpbook")
 
 # 자체 제작 NER 코퍼스 기준의 레이블 시퀀스를 만들기 위한 ID 체계
 # 나 는 삼성 에 입사 했다
 # O O 기관 O O O > [CLS] O O 기관 O O O [SEP] [PAD] [PAD] ...
 NER_CLS_TOKEN = "[CLS]"
 NER_SEP_TOKEN = "[SEP]"
 NER_PAD_TOKEN = "[PAD]"
@@ -40,53 +41,46 @@
     label_ids: Optional[List[int]] = None
 
 
 class NERCorpus:
 
     def __init__(
             self,
-            args: NLUTrainerArguments | NLUTesterArguments,
+            args: TrainerArguments | TesterArguments,
     ):
         self.args = args
 
     def get_examples(self, data_path):
         logger.info(f"loading data from {data_path}...")
         examples = []
         for line in open(data_path, "r", encoding="utf-8").readlines():
             text, label = line.split("\u241E")
             examples.append(NERExample(text=text, label=label))
         return examples
 
     def get_labels(self):
-        label_map_path = os.path.join(
-            self.args.downstream_model_home,
-            "label_map.txt",
-        )
-        if not os.path.exists(label_map_path):
+        label_map_path = make_parent_dir(self.args.output.dir_path / "label_map.txt")
+        if not label_map_path.exists():
             logger.info("processing NER tag dictionary...")
-            os.makedirs(self.args.downstream_model_home, exist_ok=True)
+            os.makedirs(self.args.model.finetuning_home, exist_ok=True)
             ner_tags = []
             regex_ner = re.compile('<(.+?):[A-Z]{3}>')
-            train_corpus_path = os.path.join(
-                self.args.downstream_data_home,
-                self.args.downstream_data_name,
-                "train.txt",
-            )
+            train_corpus_path = self.args.data.home / self.args.data.name / "train.txt"
             target_sentences = [line.split("\u241E")[1].strip()
-                                for line in open(train_corpus_path, "r", encoding="utf-8").readlines()]
+                                for line in train_corpus_path.open("r", encoding="utf-8").readlines()]
             for target_sentence in target_sentences:
                 regex_filter_res = regex_ner.finditer(target_sentence)
                 for match_item in regex_filter_res:
                     ner_tag = match_item[0][-4:-1]
                     if ner_tag not in ner_tags:
                         ner_tags.append(ner_tag)
             b_tags = [f"B-{ner_tag}" for ner_tag in ner_tags]
             i_tags = [f"I-{ner_tag}" for ner_tag in ner_tags]
             labels = [NER_CLS_TOKEN, NER_SEP_TOKEN, NER_PAD_TOKEN, NER_MASK_TOKEN, "O"] + b_tags + i_tags
-            with open(label_map_path, "w", encoding="utf-8") as f:
+            with label_map_path.open("w", encoding="utf-8") as f:
                 for tag in labels:
                     f.writelines(tag + "\n")
         else:
             labels = [tag.strip() for tag in open(label_map_path, "r", encoding="utf-8").readlines()]
         return labels
 
     @property
@@ -200,15 +194,15 @@
     label_ids = [label_map[label] for label in label_sequence]
     return label_ids
 
 
 def _convert_examples_to_ner_features(
         examples: List[NERExample],
         tokenizer: BertTokenizer,
-        args: NLUTrainerArguments,
+        args: TrainerArguments,
         label_list: List[str],
         cls_token_at_end: Optional[bool] = False,
 ):
     """
     `cls_token_at_end` define the location of the CLS token:
             - False (Default, BERT/XLM pattern): [CLS] + A + [SEP] + B + [SEP]
             - True (XLNet/GPT pattern): A + [SEP] + B + [SEP] + [CLS]
@@ -217,99 +211,77 @@
     id_to_label = {i: label for i, label in enumerate(label_list)}
 
     features = []
     for example in examples:
         tokens = tokenizer.tokenize(example.text)
         inputs = tokenizer._encode_plus(
             tokens,
-            max_length=args.max_seq_length,
+            max_length=args.model.max_seq_length,
             truncation_strategy=TruncationStrategy.LONGEST_FIRST,
             padding_strategy=PaddingStrategy.MAX_LENGTH,
         )
         label_ids = _process_target_sentence(
             tokens=tokens,
             origin_sentence=example.text,
             target_sentence=example.label,
-            max_length=args.max_seq_length,
+            max_length=args.model.max_seq_length,
             label_map=label_map,
             tokenizer=tokenizer,
             cls_token_at_end=cls_token_at_end,
         )
         features.append(NERFeatures(**inputs, label_ids=label_ids))
 
-    for i, example in enumerate(examples[:5]):
+    for i, example in enumerate(examples[:3]):
         logger.info("*** Example ***")
         logger.info("sentence: %s" % (example.text))
         logger.info("target: %s" % (example.label))
         logger.info("tokens: %s" % (" ".join(tokenizer.convert_ids_to_tokens(features[i].input_ids))))
         logger.info("label: %s" % (" ".join([id_to_label[label_id] for label_id in features[i].label_ids])))
         logger.info("features: %s" % features[i])
 
     return features
 
 
 class NERDataset(Dataset):
-
     def __init__(
             self,
-            args: NLUTrainerArguments | NLUTesterArguments,
+            split: str,
+            args: TrainerArguments | TesterArguments,
             tokenizer: BertTokenizer,
             corpus: NERCorpus,
             convert_examples_to_features_fn=_convert_examples_to_ner_features,
     ):
-        if corpus is not None:
-            self.corpus = corpus
-        else:
-            raise KeyError("corpus is not valid")
-        # Load data features from cache or dataset file
-        cached_features_file = os.path.join(
-            args.downstream_data_home,
-            args.downstream_data_name,
-            "cached_{}_{}_{}_{}_{}".format(
-                Path(args.downstream_data_file).stem,
-                tokenizer.__class__.__name__,
-                str(args.max_seq_length),
-                args.downstream_data_name,
-                args.downstream_task_name,
-            ),
-        )
+        assert corpus, "corpus is not valid"
+        self.corpus = corpus
 
-        # Make sure only the first process in distributed training processes the dataset,
-        # and the others will use the cache.
-        lock_path = cached_features_file + ".lock"
-        with FileLock(lock_path):
+        assert args.data.home, f"No data_home: {args.data.home}"
+        assert args.data.name, f"No data_name: {args.data.name}"
+        data_file_dict: dict = args.data.files.to_dict()
+        assert split in data_file_dict, f"No '{split}' split in data_file: should be one of {list(data_file_dict.keys())}"
+        assert data_file_dict[split], f"No data_file for '{split}' split: {args.data.files}"
+        text_data_path: Path = Path(args.data.home) / args.data.name / data_file_dict[split]
+        cache_data_path = text_data_path \
+            .with_stem(text_data_path.stem + f"-by-{tokenizer.__class__.__name__}-with-{args.model.max_seq_length}") \
+            .with_suffix(".cache")
+        cache_lock_path = cache_data_path.with_suffix(".lock")
 
-            if os.path.exists(cached_features_file) and not args.overwrite_cache:
+        with FileLock(cache_lock_path):
+            if os.path.exists(cache_data_path) and args.data.caching:
                 start = time.time()
-                self.features = torch.load(cached_features_file)
-                logger.info(
-                    f"Loading features from cached file {cached_features_file} [took %.3f s]", time.time() - start
-                )
+                self.features = torch.load(cache_data_path)
+                logger.info(f"Loading features from cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
             else:
-                corpus_path = os.path.join(
-                    args.downstream_data_home,
-                    args.downstream_data_name,
-                    args.downstream_data_file,
-                )
-                logger.info(f"Creating features from dataset file at {corpus_path}")
-                examples = self.corpus.get_examples(corpus_path)
-                self.features = convert_examples_to_features_fn(
-                    examples,
-                    tokenizer,
-                    args,
-                    label_list=self.corpus.get_labels(),
-                )
+                assert text_data_path.exists() and text_data_path.is_file(), f"No data_text_path: {text_data_path}"
+                logger.info(f"Creating features from dataset file at {text_data_path}")
+                examples = self.corpus.get_examples(text_data_path)
+                self.features = convert_examples_to_features_fn(examples, tokenizer, args, label_list=self.corpus.get_labels())
                 start = time.time()
-                logger.info(
-                    "Saving features into cached file, it could take a lot of time..."
-                )
-                torch.save(self.features, cached_features_file)
-                logger.info(
-                    "Saving features into cached file %s [took %.3f s]", cached_features_file, time.time() - start
-                )
+                logger.info("Saving features into cached file, it could take a lot of time...")
+                torch.save(self.features, cache_data_path)
+                logger.info(f"Saving features into cached file at {cache_data_path} [took {time.time() - start:.3f} s]")
 
     def __len__(self):
         return len(self.features)
 
     def __getitem__(self, i):
         return self.features[i]
```

### Comparing `chrislab-0.5.1/src/nlpbook/ner/task.py` & `chrislab-0.5.2/src/nlpbook/ner/task.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,70 @@
 from typing import List, Dict
 
+import pytorch_lightning as pl
 import torch
 from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
-from nlpbook.arguments import NLUTrainerArguments, NLUTesterArguments
+from nlpbook.arguments import TrainerArguments, TesterArguments
 from nlpbook.metrics import accuracy
 from nlpbook.ner import NER_PAD_ID
-from transformers import BertPreTrainedModel
+from transformers import PreTrainedModel
 from transformers.modeling_outputs import TokenClassifierOutput
 
 
 class NERTask(LightningModule):
-    def __init__(self,
-                 model: BertPreTrainedModel,
-                 args: NLUTrainerArguments | NLUTesterArguments,
-                 ):
+    def __init__(self, model: PreTrainedModel,
+                 args: TrainerArguments | TesterArguments,
+                 trainer: pl.Trainer):
         super().__init__()
         self.model = model
         self.args = args
+        self.trainer = trainer
+        self.train_acc = -1.0
+        self.train_loss = -1.0
 
     def configure_optimizers(self):
-        optimizer = AdamW(self.parameters(), lr=self.args.learning_rate)
+        optimizer = AdamW(self.parameters(), lr=self.args.learning.speed)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
         return {
             'optimizer': optimizer,
             'lr_scheduler': scheduler,
         }
 
     def training_step(self, inputs, batch_idx):
         outputs: TokenClassifierOutput = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
         acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
-        self.log("loss", outputs.loss, prog_bar=False, logger=True, on_step=True, on_epoch=False)
-        self.log("acc", acc, prog_bar=True, logger=True, on_step=True, on_epoch=False)
-        return outputs.loss
+        self.train_acc = acc
+        self.train_loss = outputs.loss
+        return {"loss": outputs.loss, "acc": acc}
 
     def validation_step(self, inputs, batch_idx):
         outputs: TokenClassifierOutput = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
         acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
-        self.log("val_loss", outputs.loss, prog_bar=True, logger=True, on_step=False, on_epoch=True)
-        self.log("val_acc", acc, prog_bar=True, logger=True, on_step=False, on_epoch=True)
-        return outputs.loss
+        self.log("train_loss", self.train_loss, prog_bar=True, logger=False, on_step=False, on_epoch=True)
+        self.log("train_acc", self.train_acc, prog_bar=True, logger=False, on_step=False, on_epoch=True)
+        self.log("val_loss", outputs.loss, prog_bar=True, logger=False, on_step=False, on_epoch=True)
+        self.log("val_acc", acc, prog_bar=True, logger=False, on_step=False, on_epoch=True)
+        self.log("global_step", self.trainer.lightning_module.global_step * 1.0, prog_bar=True, logger=False, on_step=True, on_epoch=False)
+        return {"val_loss": outputs.loss, "val_acc": acc}
 
     def test_step(self, inputs, batch_idx):
         outputs: TokenClassifierOutput = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
         acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
-        self.log("test_loss", outputs.loss, prog_bar=True, logger=True, on_step=False, on_epoch=True)
-        self.log("test_acc", acc, prog_bar=True, logger=True, on_step=False, on_epoch=True)
-        return outputs.loss
+        self.log("test_loss", outputs.loss, prog_bar=False, logger=True, on_step=False, on_epoch=True)
+        self.log("test_acc", acc, prog_bar=False, logger=True, on_step=False, on_epoch=True)
+        return {"test_loss": outputs.loss, "test_acc": acc}
 
     def x_validation_epoch_end(
             self, outputs: List[Dict[str, torch.Tensor]], data_type: str = "valid", write_predictions: bool = False
     ) -> None:
         """When validation step ends, either token- or character-level predicted
         labels are aligned with the original character-level labels and then
         evaluated.
```

### Comparing `chrislab-0.5.1/src/nlpbook/paircls/corpus.py` & `chrislab-0.5.2/src/nlpbook/paircls/corpus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import json
 import logging
 from nlpbook.cls.corpus import ClassificationExample
 
 
-logger = logging.getLogger("ratsnlp")
+logger = logging.getLogger("nlpbook")
 
 
 class KlueNLICorpus:
 
     def __init__(self):
         pass
```

### Comparing `chrislab-0.5.1/src/nlpbook/paircls/deploy.py` & `chrislab-0.5.2/src/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/qa/arguments.py` & `chrislab-0.5.2/src/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/qa/corpus.py` & `chrislab-0.5.2/src/nlpbook/qa/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from filelock import FileLock
 from torch.utils.data.dataset import Dataset
 from tqdm import tqdm
 
 from nlpbook.qa import QATrainArguments
 from transformers import PreTrainedTokenizer
 
-logger = logging.getLogger("ratsnlp")
+logger = logging.getLogger("nlpbook")
 
 
 @dataclass
 class QAExample:
     # 질문 : 임종석이 여의도 농민 폭력 시위를 주도한 혐의로 지명수배 된 날은?
     question_text: str
     # (답 찾는 대상인)지문 : 1989년 2월 15일 여의도 농민 폭력 시위를 주도한 혐의 ... 서울지방경찰청 공안분실로 인계되었다.
```

### Comparing `chrislab-0.5.1/src/nlpbook/qa/deploy.py` & `chrislab-0.5.2/src/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/qa/task.py` & `chrislab-0.5.2/src/nlpbook/qa/task.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.5.1/src/nlpbook/utils.py` & `chrislab-0.5.2/src/nlpbook/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import logging
 import os
 import sys
-import tqdm
-import logging
+
 import requests
-from transformers import HfArgumentParser
+import tqdm
 
+from transformers import HfArgumentParser
+from .arguments import TrainerArguments, TesterArguments
 
 REMOTE_DATA_MAP = {
     "nsmc": {
         "train": {
             "web_url": "https://github.com/e9t/nsmc/raw/master/ratings_train.txt",
             "fname": "train.txt",
         },
@@ -30,15 +32,15 @@
     "kmou-ner": {
         "train": {
             "googledrive_file_id": "1RP764owqs1kZeHcjFnCX7zXt2EcjGY1i",
             "fname": "train.txt",
         },
         "val": {
             "googledrive_file_id": "1bEPNWT5952rD3xjg0LfJBy3hLHry3yUL",
-            "fname": "val.txt",
+            "fname": "valid.txt",
         },
     },
     "korquad-v1": {
         "train": {
             "web_url": "https://korquad.github.io/dataset/KorQuAD_v1.0_train.json",
             "fname": "KorQuAD_v1.0_train.json",
         },
@@ -66,15 +68,15 @@
         "config": {
             "googledrive_file_id": "1z6obNRWPHoVrMzT9THElblebdovuDLUZ",
             "fname": "config.json",
         },
     },
 }
 GOOGLE_DRIVE_URL = "https://docs.google.com/uc?export=download"
-logger = logging.getLogger("ratsnlp")  # pylint: disable=invalid-name
+logger = logging.getLogger("nlpbook")
 
 
 def save_response_content(response, save_path):
     with open(save_path, "wb") as f:
         content_length = response.headers.get("Content-Length")
         total = int(content_length) if content_length is not None else None
         progress = tqdm.tqdm(
@@ -109,14 +111,15 @@
                     cache_dir="~/cache",
                     force_download=False):
     def get_confirm_token(response):
         for key, value in response.cookies.items():
             if key.startswith('download_warning'):
                 return value
         return None
+
     valid_save_path = get_valid_path(cache_dir, save_fname)
     # 캐시 파일이 있으면 캐시 사용
     if os.path.exists(valid_save_path) and not force_download:
         logger.info(f"cache file({valid_save_path}) exists, using cache!")
         return valid_save_path
     # init a HTTP session
     session = requests.Session()
@@ -160,32 +163,32 @@
     if etag is None:
         raise ValueError(f"not valid URL({url}), cannot download resources")
     response = requests.get(url, stream=True)
     save_response_content(response, valid_save_path)
     return valid_save_path
 
 
-def download_downstream_dataset(args):
-    data_name = args.downstream_data_name.lower()
+def download_downstream_dataset(args: TesterArguments):
+    data_name = args.data.name.lower()
     if data_name in REMOTE_DATA_MAP.keys():
-        cache_dir = os.path.join(args.downstream_data_home, data_name)
+        cache_dir = os.path.join(args.data.home, data_name)
         for value in REMOTE_DATA_MAP[data_name].values():
             if "web_url" in value.keys():
                 web_download(
                     url=value["web_url"],
                     save_fname=value["fname"],
                     cache_dir=cache_dir,
-                    force_download=args.force_download,
+                    force_download=args.data.redownload,
                 )
             else:
                 google_download(
                     file_id=value["googledrive_file_id"],
                     save_fname=value["fname"],
                     cache_dir=cache_dir,
-                    force_download=args.force_download
+                    force_download=args.data.redownload
                 )
     else:
         raise ValueError(f"not valid data name({data_name}), cannot download resources")
 
 
 def download_pretrained_model(args, config_only=False):
     pretrained_model_name = args.pretrained_model_path.lower()
@@ -193,51 +196,47 @@
         for key, value in REMOTE_MODEL_MAP[pretrained_model_name].items():
             if not config_only or (config_only and key == "config"):
                 if "web_url" in value.keys():
                     web_download(
                         url=value["web_url"],
                         save_fname=value["fname"],
                         cache_dir=args.pretrained_model_cache_dir,
-                        force_download=args.force_download,
                     )
                 else:
                     google_download(
                         file_id=value["googledrive_file_id"],
                         save_fname=value["fname"],
                         cache_dir=args.pretrained_model_cache_dir,
-                        force_download=args.force_download,
                     )
     else:
         raise ValueError(f"not valid model name({pretrained_model_name}), cannot download resources")
 
 
-def set_logger():
+def set_seed(args: TrainerArguments):
+    if args.learning.seed is not None:
+        from transformers import set_seed
+        set_seed(args.learning.seed)
+        from pytorch_lightning import seed_everything
+        seed_everything(args.learning.seed)
+    else:
+        print("not fixed seed", file=sys.stderr)
+
+
+def set_logger(level=logging.INFO):
     import torch
     if torch.cuda.is_available():
         stream_handler = logging.StreamHandler()
-        formatter = logging.Formatter(
-            fmt="%(levelname)s:%(name)s:%(message)s",
-        )
+        formatter = logging.Formatter(fmt="%(levelname)s:%(name)s:%(message)s")
         stream_handler.setFormatter(formatter)
         logger.addHandler(stream_handler)
-    logger.setLevel(logging.INFO)
-
-
-def set_seed(args):
-    if args.seed is not None:
-        # 향후 pytorch-lightning의 seed_everything까지 확장
-        from transformers import set_seed
-        set_seed(args.seed)
-        print(f"set seed: {args.seed}")
-    else:
-        print("not fixed seed")
+    logger.setLevel(level)
 
 
 def load_arguments(argument_class, json_file_path=None):
     parser = HfArgumentParser(argument_class)
     if json_file_path is not None:
         args, = parser.parse_json_file(json_file=json_file_path)
     elif len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
         args, = parser.parse_json_file(json_file=os.path.abspath(sys.argv[1]))
     else:
         args, = parser.parse_args_into_dataclasses()
-    return args
+    return args
```

