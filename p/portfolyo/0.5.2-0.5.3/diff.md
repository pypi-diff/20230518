# Comparing `tmp/portfolyo-0.5.2.tar.gz` & `tmp/portfolyo-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolyo-0.5.2.tar", last modified: Wed May 17 09:21:02 2023, max compression
+gzip compressed data, was "portfolyo-0.5.3.tar", last modified: Wed May 17 23:27:56 2023, max compression
```

## Comparing `portfolyo-0.5.2.tar` & `portfolyo-0.5.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.838975 portfolyo-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-17 09:20:48.000000 portfolyo-0.5.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 09:20:48.000000 portfolyo-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 09:21:02.838975 portfolyo-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-17 09:20:48.000000 portfolyo-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.842975 portfolyo-0.5.2/portfolyo/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-17 09:21:02.842975 portfolyo-0.5.2/portfolyo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.830975 portfolyo-0.5.2/portfolyo/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/extendpandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.830975 portfolyo-0.5.2/portfolyo/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/mixins/excelclipboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/mixins/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/mixins/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/ndframelike.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/core/pfline/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/arithmatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/children.py
--rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/dataframeexport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/developernotes.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/flat_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/flat_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/nested_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/nested_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfline/prices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/core/pfstate/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfstate/arithmatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfstate/pfstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/pfstate/pfstate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/core/suppresswarnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/dev/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/dev/mockup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/prices/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/prices/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/prices/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/prices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.834975 portfolyo-0.5.2/portfolyo/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.838975 portfolyo-0.5.2/portfolyo/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/changefreq.py
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/changeyear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/floor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/freq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/isboundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/leftandright.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/peakperiod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/right.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/righttoleft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/round.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/standardize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/tzone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/unitdefinitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/tools/wavg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.838975 portfolyo-0.5.2/portfolyo/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/visualize/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/visualize/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-17 09:20:48.000000 portfolyo-0.5.2/portfolyo/visualize/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:21:02.830975 portfolyo-0.5.2/portfolyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 09:21:02.000000 portfolyo-0.5.2/portfolyo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 09:20:48.000000 portfolyo-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 09:21:02.838975 portfolyo-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-17 09:20:48.000000 portfolyo-0.5.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-17 09:20:49.000000 portfolyo-0.5.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.872516 portfolyo-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-17 23:27:42.000000 portfolyo-0.5.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-17 23:27:42.000000 portfolyo-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 23:27:56.872516 portfolyo-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-17 23:27:42.000000 portfolyo-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.872516 portfolyo-0.5.3/portfolyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-17 23:27:56.872516 portfolyo-0.5.3/portfolyo/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.860516 portfolyo-0.5.3/portfolyo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/extendpandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.860516 portfolyo-0.5.3/portfolyo/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/mixins/excelclipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/mixins/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/mixins/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/ndframelike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.864516 portfolyo-0.5.3/portfolyo/core/pfline/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/arithmatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/children.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/dataframeexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/developernotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/flat_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/flat_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/nested_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/nested_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfline/prices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.864516 portfolyo-0.5.3/portfolyo/core/pfstate/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfstate/arithmatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfstate/pfstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/pfstate/pfstate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/core/suppresswarnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.864516 portfolyo-0.5.3/portfolyo/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/dev/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/dev/mockup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.864516 portfolyo-0.5.3/portfolyo/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/prices/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/prices/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/prices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.868517 portfolyo-0.5.3/portfolyo/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.868517 portfolyo-0.5.3/portfolyo/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/changefreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/changeyear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/isboundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/leftandright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/peakperiod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/right.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/righttoleft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/round.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/standardize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/tzone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/unitdefinitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/tools/wavg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.872516 portfolyo-0.5.3/portfolyo/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/visualize/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/visualize/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-17 23:27:42.000000 portfolyo-0.5.3/portfolyo/visualize/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 23:27:56.860516 portfolyo-0.5.3/portfolyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 23:27:56.000000 portfolyo-0.5.3/portfolyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-17 23:27:56.000000 portfolyo-0.5.3/portfolyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 23:27:56.000000 portfolyo-0.5.3/portfolyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 23:27:56.000000 portfolyo-0.5.3/portfolyo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 23:27:56.000000 portfolyo-0.5.3/portfolyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 23:27:56.000000 portfolyo-0.5.3/portfolyo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 23:27:42.000000 portfolyo-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 23:27:56.872516 portfolyo-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-17 23:27:42.000000 portfolyo-0.5.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-17 23:27:43.000000 portfolyo-0.5.3/versioneer.py
```

### Comparing `portfolyo-0.5.2/LICENCE` & `portfolyo-0.5.3/LICENCE`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/PKG-INFO` & `portfolyo-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.5.2
+Version: 0.5.3
 Summary: Analysing and manipulating timeseries related to power and gas offtake portfolios.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
 portfolyo
```

### Comparing `portfolyo-0.5.2/README.rst` & `portfolyo-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/__init__.py` & `portfolyo-0.5.3/portfolyo/__init__.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/mixins/excelclipboard.py` & `portfolyo-0.5.3/portfolyo/core/mixins/excelclipboard.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/mixins/plot.py` & `portfolyo-0.5.3/portfolyo/core/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/mixins/text.py` & `portfolyo-0.5.3/portfolyo/core/mixins/text.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/ndframelike.py` & `portfolyo-0.5.3/portfolyo/core/ndframelike.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/arithmatic.py` & `portfolyo-0.5.3/portfolyo/core/pfline/arithmatic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Enable arithmatic with PfLine classes."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Union
 
+import numpy as np
 import pandas as pd
 
 from ... import testing, tools
 from . import classes, create, interop
 from .enums import Kind, Structure
 
 if TYPE_CHECKING:  # needed to avoid circular imports
@@ -112,14 +113,26 @@
         def wrapper(pfl: PfLine, other: Any):
             if other is None:
                 return pfl
             return fn(pfl, other)
 
         return wrapper
 
+    def returnself_if_otherzerofloatseries(fn):
+        def wrapper(pfl: PfLine, other: Any):
+            if isinstance(other, pd.Series):
+                if other.dtype == "pint[dimensionless]":
+                    other = other.pint.m
+                if other.dtype in [int, float] and np.allclose(other.values, 0.0):
+                    return pfl
+
+            return fn(pfl, other)
+
+        return wrapper
+
     def raiseerror_if_otherNone(fn):
         def wrapper(pfl: PfLine, other: Any):
             if other is None:
                 raise NotImplementedError("Cannot do this operation with this operand.")
             return fn(pfl, other)
 
         return wrapper
@@ -135,24 +148,26 @@
 
 class PfLineArithmatic:
     def __neg__(self: PfLine) -> PfLine:
         return self * -1  # defer to __mul__
 
     @Prep.standardize_other  # other converted to None, a PfLine, or dimless Series
     @Prep.returnself_if_otherNone  # other is now a PfLine or dimless Series
+    @Prep.returnself_if_otherzerofloatseries  # catch pfline + 0
     @Prep.raiseerror_if_otherdimlessseries  # other is now a PfLine...
     @Prep.assert_objects_indexcompatibility  # ...with a compatible index
     def __add__(self: PfLine, other: Any) -> PfLine:
         return Add.two_pflines(self, other)
 
     def __radd__(self: PfLine, other: Any) -> PfLine:
         return self + other  # defer to __add__
 
     @Prep.standardize_other  # other converted to None, a PfLine, or dimless Series
     @Prep.returnself_if_otherNone  # catch pfline - None
+    @Prep.returnself_if_otherzerofloatseries  # cach pfline - 0
     def __sub__(self: PfLine, other: Any) -> PfLine:
         return self + -other  # defer to __add__ and __neg__
 
     def __rsub__(self: PfLine, other: Any) -> PfLine:
         return -self + other  # defer to __add__ and __neg__
 
     @Prep.standardize_other  # other converted to None, a PfLine, or dimless Series
```

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/children.py` & `portfolyo-0.5.3/portfolyo/core/pfline/children.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/classes.py` & `portfolyo-0.5.3/portfolyo/core/pfline/classes.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/create.py` & `portfolyo-0.5.3/portfolyo/core/pfline/create.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/dataframeexport.py` & `portfolyo-0.5.3/portfolyo/core/pfline/dataframeexport.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/decorators.py` & `portfolyo-0.5.3/portfolyo/core/pfline/decorators.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/developernotes.py` & `portfolyo-0.5.3/portfolyo/core/pfline/developernotes.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/enums.py` & `portfolyo-0.5.3/portfolyo/core/pfline/enums.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/flat_helper.py` & `portfolyo-0.5.3/portfolyo/core/pfline/flat_helper.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/flat_methods.py` & `portfolyo-0.5.3/portfolyo/core/pfline/flat_methods.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/interop.py` & `portfolyo-0.5.3/portfolyo/core/pfline/interop.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/nested_helper.py` & `portfolyo-0.5.3/portfolyo/core/pfline/nested_helper.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/nested_methods.py` & `portfolyo-0.5.3/portfolyo/core/pfline/nested_methods.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfline/prices.py` & `portfolyo-0.5.3/portfolyo/core/pfline/prices.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfstate/arithmatic.py` & `portfolyo-0.5.3/portfolyo/core/pfstate/arithmatic.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfstate/pfstate.py` & `portfolyo-0.5.3/portfolyo/core/pfstate/pfstate.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/core/pfstate/pfstate_helper.py` & `portfolyo-0.5.3/portfolyo/core/pfstate/pfstate_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,14 @@
     sourced = create.pfline(sourced)
     if sourced.kind is not Kind.COMPLETE:
         raise ValueError("Parameter ``sourced`` does not contain price and volume.")
     try:
         testing.assert_indices_compatible(ref_idx, sourced.index)
     except AssertionError as e:
         raise ValueError from e
-    # Workaround for error in pandas intersection (#46702):
+    # HACK: Workaround for error in pandas intersection (#46702):
     if len(tools.intersect.indices(ref_idx, sourced.index)) < len(ref_idx):
         raise ValueError(
             "Parameter ``sourced``: does not cover entire delivery period of"
             " ``offtakevolume``."
         )
     return sourced.loc[ref_idx]
```

### Comparing `portfolyo-0.5.2/portfolyo/dev/develop.py` & `portfolyo-0.5.3/portfolyo/dev/develop.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/dev/mockup.py` & `portfolyo-0.5.3/portfolyo/dev/mockup.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/prices/convert.py` & `portfolyo-0.5.3/portfolyo/prices/convert.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/prices/hedge.py` & `portfolyo-0.5.3/portfolyo/prices/hedge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Functionality to hedge an offtake profile with a price profile."""
 
 from typing import Tuple
 
 import pandas as pd
 
 from .. import tools
-from . import convert
-from .utils import is_peak_hour
+from . import convert, utils
 
 
 def _hedge(df: pd.DataFrame, how: str, po: bool) -> pd.Series:
     """
     Hedge a power timeseries, for given price timeseries.
 
     Parameters
@@ -37,16 +36,17 @@
     of equal duration.
     """
 
     # Split into peak and offpeak.
 
     if po:
         apply_f = lambda df: _hedge(df, how, po=False)  # noqa
-        # s = df.groupby(is_peak_hour).apply(apply_f) # calls group_f on EACH ts
-        s = df.groupby(is_peak_hour(df.index)).apply(apply_f)  # calls group_f on index
+        # s = df.groupby(utils.is_peak_hour).apply(apply_f) # calls group_f on EACH ts
+        is_peak_hour = utils.is_peak_hour(df.index)
+        s = df.groupby(is_peak_hour).apply(apply_f)  # calls group_f on index
         return s.rename(index={True: "peak", False: "offpeak"}).stack()
 
     # Don't split into peak and offpeak.
 
     if df.index.freq:
         # Use magnitude only, so that, if w and p are float series, their return
         # series are also floats (instead of dimensionless Quantities).
```

### Comparing `portfolyo-0.5.2/portfolyo/prices/utils.py` & `portfolyo-0.5.3/portfolyo/prices/utils.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/testing/testing.py` & `portfolyo-0.5.3/portfolyo/testing/testing.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/ceil.py` & `portfolyo-0.5.3/portfolyo/tools/ceil.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/changefreq.py` & `portfolyo-0.5.3/portfolyo/tools/changefreq.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,22 +76,22 @@
     offset = dt.timedelta(hours=start_of_day.hour, minutes=start_of_day.minute)
 
     source_vs_daily = tools_freq.up_or_down(s.index.freq, "D")
     target_vs_daily = tools_freq.up_or_down(freq, "D")
 
     # Several isuses with pandas resampling:
 
-    # 1. When upsampling from to yearly to monthly values with `.resample()`, the
+    # HACK: (1): When upsampling from to yearly to monthly values with `.resample()`, the
     # start-of-day is lost. We need to do it in two steps; first upsampling to days and
     # then downsampling to months.
 
     if source_vs_daily > 0 and target_vs_daily > 0:
         return _downsample_avgable(_upsample_avgable(s, "D"), freq)
 
-    # 2. We cannot simply `.resample()`, because in that case the final value is not
+    # HACK: (2): We cannot simply `.resample()`, because in that case the final value is not
     # duplicated. Solution: add a dummy value, which we eventually remove again.
 
     # So, first, add additional row...
     # (original code to add additional row, does not work if unit-aware. Maybe with future release of pint_pandas?)
     # s = s.copy()
     # s.loc[s.index.right[-1]] = None
     # (Workaround: turn into dataframe, change frequency, and turn back into series.)
```

### Comparing `portfolyo-0.5.2/portfolyo/tools/changeyear.py` & `portfolyo-0.5.3/portfolyo/tools/changeyear.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/duration.py` & `portfolyo-0.5.3/portfolyo/tools/duration.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/floor.py` & `portfolyo-0.5.3/portfolyo/tools/floor.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/frame.py` & `portfolyo-0.5.3/portfolyo/tools/frame.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/freq.py` & `portfolyo-0.5.3/portfolyo/tools/freq.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/intersect.py` & `portfolyo-0.5.3/portfolyo/tools/intersect.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/isboundary.py` & `portfolyo-0.5.3/portfolyo/tools/isboundary.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/leftandright.py` & `portfolyo-0.5.3/portfolyo/tools/leftandright.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/peakperiod.py` & `portfolyo-0.5.3/portfolyo/tools/peakperiod.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/right.py` & `portfolyo-0.5.3/portfolyo/tools/right.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/righttoleft.py` & `portfolyo-0.5.3/portfolyo/tools/righttoleft.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/round.py` & `portfolyo-0.5.3/portfolyo/tools/round.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/standardize.py` & `portfolyo-0.5.3/portfolyo/tools/standardize.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/trim.py` & `portfolyo-0.5.3/portfolyo/tools/trim.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/tzone.py` & `portfolyo-0.5.3/portfolyo/tools/tzone.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/unit.py` & `portfolyo-0.5.3/portfolyo/tools/unit.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/unitdefinitions.txt` & `portfolyo-0.5.3/portfolyo/tools/unitdefinitions.txt`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/tools/wavg.py` & `portfolyo-0.5.3/portfolyo/tools/wavg.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/visualize/categories.py` & `portfolyo-0.5.3/portfolyo/visualize/categories.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/visualize/colors.py` & `portfolyo-0.5.3/portfolyo/visualize/colors.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo/visualize/plot.py` & `portfolyo-0.5.3/portfolyo/visualize/plot.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/portfolyo.egg-info/PKG-INFO` & `portfolyo-0.5.3/portfolyo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolyo
-Version: 0.5.2
+Version: 0.5.3
 Summary: Analysing and manipulating timeseries related to power and gas offtake portfolios.
 Author: Ruud Wijtvliet
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE
 
 portfolyo
```

### Comparing `portfolyo-0.5.2/portfolyo.egg-info/SOURCES.txt` & `portfolyo-0.5.3/portfolyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/setup.py` & `portfolyo-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `portfolyo-0.5.2/versioneer.py` & `portfolyo-0.5.3/versioneer.py`

 * *Files identical despite different names*

