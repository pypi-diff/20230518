# Comparing `tmp/timepunch-1.0.0.tar.gz` & `tmp/timepunch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timepunch-1.0.0.tar", last modified: Thu May 18 01:36:34 2023, max compression
+gzip compressed data, was "timepunch-1.0.1.tar", last modified: Thu May 18 01:54:03 2023, max compression
```

## Comparing `timepunch-1.0.0.tar` & `timepunch-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-18 01:36:34.716045 timepunch-1.0.0/
--rw-r--r--   0 itsknk     (501) staff       (20)      334 2023-05-18 01:36:34.715660 timepunch-1.0.0/PKG-INFO
--rw-r--r--   0 itsknk     (501) staff       (20)      173 2023-05-18 01:36:30.000000 timepunch-1.0.0/README.md
--rw-r--r--   0 itsknk     (501) staff       (20)       38 2023-05-18 01:36:34.716169 timepunch-1.0.0/setup.cfg
--rw-r--r--   0 itsknk     (501) staff       (20)      469 2023-05-18 01:35:52.000000 timepunch-1.0.0/setup.py
-drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-18 01:36:34.715155 timepunch-1.0.0/timepunch.egg-info/
--rw-r--r--   0 itsknk     (501) staff       (20)      334 2023-05-18 01:36:34.000000 timepunch-1.0.0/timepunch.egg-info/PKG-INFO
--rw-r--r--   0 itsknk     (501) staff       (20)      186 2023-05-18 01:36:34.000000 timepunch-1.0.0/timepunch.egg-info/SOURCES.txt
--rw-r--r--   0 itsknk     (501) staff       (20)        1 2023-05-18 01:36:34.000000 timepunch-1.0.0/timepunch.egg-info/dependency_links.txt
--rw-r--r--   0 itsknk     (501) staff       (20)       37 2023-05-18 01:36:34.000000 timepunch-1.0.0/timepunch.egg-info/entry_points.txt
--rw-r--r--   0 itsknk     (501) staff       (20)        6 2023-05-18 01:36:34.000000 timepunch-1.0.0/timepunch.egg-info/top_level.txt
+drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-18 01:54:03.805644 timepunch-1.0.1/
+-rw-r--r--   0 itsknk     (501) staff       (20)      334 2023-05-18 01:54:03.805258 timepunch-1.0.1/PKG-INFO
+-rw-r--r--   0 itsknk     (501) staff       (20)      173 2023-05-18 01:36:30.000000 timepunch-1.0.1/README.md
+-rw-r--r--   0 itsknk     (501) staff       (20)       38 2023-05-18 01:54:03.805784 timepunch-1.0.1/setup.cfg
+-rw-r--r--   0 itsknk     (501) staff       (20)      473 2023-05-18 01:53:35.000000 timepunch-1.0.1/setup.py
+drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-18 01:54:03.804753 timepunch-1.0.1/timepunch.egg-info/
+-rw-r--r--   0 itsknk     (501) staff       (20)      334 2023-05-18 01:54:03.000000 timepunch-1.0.1/timepunch.egg-info/PKG-INFO
+-rw-r--r--   0 itsknk     (501) staff       (20)      186 2023-05-18 01:54:03.000000 timepunch-1.0.1/timepunch.egg-info/SOURCES.txt
+-rw-r--r--   0 itsknk     (501) staff       (20)        1 2023-05-18 01:54:03.000000 timepunch-1.0.1/timepunch.egg-info/dependency_links.txt
+-rw-r--r--   0 itsknk     (501) staff       (20)       41 2023-05-18 01:54:03.000000 timepunch-1.0.1/timepunch.egg-info/entry_points.txt
+-rw-r--r--   0 itsknk     (501) staff       (20)        6 2023-05-18 01:54:03.000000 timepunch-1.0.1/timepunch.egg-info/top_level.txt
```

