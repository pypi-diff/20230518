# Comparing `tmp/oqpy-0.2.0.tar.gz` & `tmp/oqpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqpy-0.2.0.tar", max compression
+gzip compressed data, was "oqpy-0.2.1.tar", max compression
```

## Comparing `oqpy-0.2.0.tar` & `oqpy-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      231 2022-05-24 00:17:51.382265 oqpy-0.2.0/oqpy/__init__.py
--rw-r--r--   0        0        0     7473 2022-05-24 21:39:51.720076 oqpy-0.2.0/oqpy/classical_types.py
--rw-r--r--   0        0        0     1426 2022-05-24 01:36:30.322238 oqpy-0.2.0/oqpy/control_flow.py
--rw-r--r--   0        0        0     4692 2022-05-24 16:12:12.287830 oqpy-0.2.0/oqpy/program.py
--rw-r--r--   0        0        0     4184 2022-05-24 21:37:15.893169 oqpy-0.2.0/oqpy/pulse.py
--rw-r--r--   0        0        0     3452 2022-05-24 01:48:30.150772 oqpy-0.2.0/oqpy/quantum_types.py
--rw-r--r--   0        0        0     2904 2022-05-24 01:36:51.410320 oqpy-0.2.0/oqpy/subroutines.py
--rw-r--r--   0        0        0      776 2022-05-24 01:37:28.557215 oqpy-0.2.0/oqpy/timing.py
--rw-r--r--   0        0        0     1494 2022-05-24 00:17:51.399757 oqpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      670 2022-05-24 21:55:40.479668 oqpy-0.2.0/setup.py
--rw-r--r--   0        0        0      447 2022-05-24 21:55:40.479915 oqpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1510 2022-11-27 03:24:43.621227 oqpy-0.2.1/CITATION.cff
+-rw-r--r--   0        0        0    11328 2022-10-20 16:34:51.863893 oqpy-0.2.1/LICENSE
+-rw-r--r--   0        0        0       71 2022-10-20 16:34:51.864132 oqpy-0.2.1/NOTICE
+-rw-r--r--   0        0        0     6362 2022-11-27 03:24:43.621961 oqpy-0.2.1/README.md
+-rw-r--r--   0        0        0     1011 2023-05-18 15:19:04.171749 oqpy-0.2.1/oqpy/__init__.py
+-rw-r--r--   0        0        0    13022 2023-05-18 14:52:02.896855 oqpy-0.2.1/oqpy/base.py
+-rw-r--r--   0        0        0    13752 2023-05-18 14:52:02.897245 oqpy-0.2.1/oqpy/classical_types.py
+-rw-r--r--   0        0        0     4826 2023-05-18 14:52:02.897582 oqpy-0.2.1/oqpy/control_flow.py
+-rw-r--r--   0        0        0    22811 2023-05-18 14:52:02.897986 oqpy-0.2.1/oqpy/program.py
+-rw-r--r--   0        0        0     2702 2023-05-18 14:52:02.898331 oqpy-0.2.1/oqpy/pulse.py
+-rw-r--r--   0        0        0     4435 2023-05-18 14:52:02.898659 oqpy-0.2.1/oqpy/quantum_types.py
+-rw-r--r--   0        0        0     8321 2023-05-18 14:52:02.898997 oqpy-0.2.1/oqpy/subroutines.py
+-rw-r--r--   0        0        0     2506 2022-10-20 16:34:51.866749 oqpy-0.2.1/oqpy/timing.py
+-rw-r--r--   0        0        0     3670 2023-05-18 15:19:04.172581 oqpy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7808 1970-01-01 00:00:00.000000 oqpy-0.2.1/PKG-INFO
```

