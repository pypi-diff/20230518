# Comparing `tmp/moat-0.1.0.tar.gz` & `tmp/moat-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moat-0.1.0.tar", last modified: Sat Jun 21 11:00:54 2014, max compression
+gzip compressed data, was "moat-0.1.17.tar", last modified: Thu May 18 20:05:35 2023, max compression
```

## Comparing `moat-0.1.0.tar` & `moat-0.1.17.tar`

### file list

```diff
@@ -1,9 +1,29 @@
-drwxr-xr-x   0 joelcox    (502) staff       (20)        0 2014-06-21 11:00:54.000000 moat-0.1.0/
--rw-r--r--   0 joelcox    (502) staff       (20)       81 2014-06-21 10:23:04.000000 moat-0.1.0/CHANGELOG.rst
--rw-r--r--   0 joelcox    (502) staff       (20)     1052 2014-06-21 10:24:19.000000 moat-0.1.0/LICENSE
-drwxr-xr-x   0 joelcox    (502) staff       (20)        0 2014-06-21 11:00:54.000000 moat-0.1.0/moat/
--rw-r--r--   0 joelcox    (502) staff       (20)     1604 2014-06-21 10:10:23.000000 moat-0.1.0/moat/__init__.py
--rw-rw-rw-   0 joelcox    (502) staff       (20)     1834 2014-06-21 10:10:08.000000 moat-0.1.0/moat/repositories.py
--rw-r--r--   0 joelcox    (502) staff       (20)     2072 2014-06-21 11:00:54.000000 moat-0.1.0/PKG-INFO
--rw-r--r--   0 joelcox    (502) staff       (20)     1392 2014-06-21 10:57:03.000000 moat-0.1.0/README.rst
--rw-r--r--   0 joelcox    (502) staff       (20)      443 2014-06-21 11:00:29.000000 moat-0.1.0/setup.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 20:05:35.042065 moat-0.1.17/
+-rw-r--r--   0 smurf      (501) smurf      (501)      508 2023-04-17 17:33:37.000000 moat-0.1.17/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      912 2023-05-15 06:43:49.000000 moat-0.1.17/.gitmodules
+-rw-r--r--   0 smurf      (501) smurf      (501)     3870 2023-03-10 18:02:54.000000 moat-0.1.17/HACKING.md
+-rw-r--r--   0 smurf      (501) smurf      (501)      541 2022-09-14 08:57:55.000000 moat-0.1.17/LICENSE.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      265 2023-04-17 17:27:49.000000 moat-0.1.17/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)     4686 2023-05-18 20:05:35.042065 moat-0.1.17/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     3416 2023-04-17 07:36:31.000000 moat-0.1.17/README.md
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 20:05:35.042065 moat-0.1.17/moat/
+-rw-r--r--   0 smurf      (501) smurf      (501)      149 2023-04-22 10:09:21.000000 moat-0.1.17/moat/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      105 2023-04-17 17:02:13.000000 moat-0.1.17/moat/__main__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      617 2023-05-15 17:45:10.000000 moat-0.1.17/moat/_config.yaml
+-rw-r--r--   0 smurf      (501) smurf      (501)     2012 2023-05-15 17:09:00.000000 moat-0.1.17/moat/_dev_fix.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1139 2023-05-08 13:35:33.000000 moat-0.1.17/moat/main.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 20:05:35.042065 moat-0.1.17/moat.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)     4686 2023-05-18 20:05:34.000000 moat-0.1.17/moat.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)      398 2023-05-18 20:05:35.000000 moat-0.1.17/moat.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-05-18 20:05:34.000000 moat-0.1.17/moat.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       39 2023-05-18 20:05:34.000000 moat-0.1.17/moat.egg-info/entry_points.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       40 2023-05-18 20:05:34.000000 moat-0.1.17/moat.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        5 2023-05-18 20:05:34.000000 moat-0.1.17/moat.egg-info/top_level.txt
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      174 2023-04-17 16:17:50.000000 moat-0.1.17/mt
+-rw-r--r--   0 smurf      (501) smurf      (501)     1975 2023-05-18 20:00:57.000000 moat-0.1.17/pyproject.toml
+-rw-r--r--   0 smurf      (501) smurf      (501)       66 2023-03-10 18:02:54.000000 moat-0.1.17/requirements.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       38 2023-05-18 20:05:35.042065 moat-0.1.17/setup.cfg
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      742 2023-03-10 18:02:54.000000 moat-0.1.17/setup.sh
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 20:05:35.042065 moat-0.1.17/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2023-04-17 16:32:03.000000 moat-0.1.17/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      181 2023-04-22 10:10:10.000000 moat-0.1.17/tests/test_basic.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

