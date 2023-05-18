# Comparing `tmp/biobookshelf-0.2.5.tar.gz` & `tmp/biobookshelf-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobookshelf-0.2.5.tar", last modified: Tue May  9 04:56:14 2023, max compression
+gzip compressed data, was "biobookshelf-0.2.6.tar", last modified: Thu May 18 11:51:21 2023, max compression
```

## Comparing `biobookshelf-0.2.5.tar` & `biobookshelf-0.2.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.668303 biobookshelf-0.2.5/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    34600 2022-04-04 14:27:30.000000 biobookshelf-0.2.5/LICENSE
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        0 2022-04-04 14:27:30.000000 biobookshelf-0.2.5/MANIFEST.in
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-09 04:56:14.668303 biobookshelf-0.2.5/PKG-INFO
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      221 2022-04-04 14:27:30.000000 biobookshelf-0.2.5/README.md
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.032290 biobookshelf-0.2.5/biobookshelf/
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.064290 biobookshelf-0.2.5/biobookshelf/BA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       30 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/BA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     7975 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/BA/bitarray_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.084291 biobookshelf-0.2.5/biobookshelf/CLI/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/CLI/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3013 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/CLI/unclassified_programs.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.116291 biobookshelf-0.2.5/biobookshelf/INT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/INT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      389 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/INT/integer.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.128291 biobookshelf-0.2.5/biobookshelf/IT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       35 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/IT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       32 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/IT/interval_tree_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.140292 biobookshelf-0.2.5/biobookshelf/L/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/L/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       39 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/L/l_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.168292 biobookshelf-0.2.5/biobookshelf/MAP/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/MAP/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      594 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/MAP/mapping.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.228294 biobookshelf-0.2.5/biobookshelf/MP/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/MP/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      260 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/MP/multiprocessing_utils.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.228294 biobookshelf-0.2.5/biobookshelf/ONT/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       34 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/ONT/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69306 2023-05-08 16:30:42.000000 biobookshelf-0.2.5/biobookshelf/ONT/nanopore_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.236294 biobookshelf-0.2.5/biobookshelf/PD/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/PD/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       85 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/PD/pd_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.268294 biobookshelf-0.2.5/biobookshelf/PDB/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       19 2022-04-04 14:27:31.000000 biobookshelf-0.2.5/biobookshelf/PDB/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    29100 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/PDB/pdb.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.316295 biobookshelf-0.2.5/biobookshelf/PKG/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/PKG/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3095 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/PKG/package_util.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.336296 biobookshelf-0.2.5/biobookshelf/RNA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/RNA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    19437 2023-05-01 11:20:30.000000 biobookshelf-0.2.5/biobookshelf/RNA/rnaseq.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.376297 biobookshelf-0.2.5/biobookshelf/SAM/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2022-04-04 14:27:31.000000 biobookshelf-0.2.5/biobookshelf/SAM/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69402 2023-05-01 11:20:32.000000 biobookshelf-0.2.5/biobookshelf/SAM/sam_util.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.412297 biobookshelf-0.2.5/biobookshelf/SC/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/SC/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   122849 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/SC/single_cell.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.440298 biobookshelf-0.2.5/biobookshelf/SEQ/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/SEQ/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14831 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/SEQ/sequence.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.500299 biobookshelf-0.2.5/biobookshelf/STR/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/STR/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14367 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/STR/string.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.548300 biobookshelf-0.2.5/biobookshelf/UniProt/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.5/biobookshelf/UniProt/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      837 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/UniProt/uniprot.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.576301 biobookshelf-0.2.5/biobookshelf/WEB/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       31 2022-04-04 14:27:31.000000 biobookshelf-0.2.5/biobookshelf/WEB/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8727 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/WEB/web_application.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.604301 biobookshelf-0.2.5/biobookshelf/ZA/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/ZA/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       12 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/ZA/zarr_utils.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      370 2023-05-09 04:54:53.000000 biobookshelf-0.2.5/biobookshelf/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      162 2023-05-01 11:20:29.000000 biobookshelf-0.2.5/biobookshelf/__main__.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.636302 biobookshelf-0.2.5/biobookshelf/main/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2022-04-18 07:53:18.000000 biobookshelf-0.2.5/biobookshelf/main/__init__.py
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   712244 2023-05-02 03:16:15.000000 biobookshelf-0.2.5/biobookshelf/main/unclassified_functions.py
-drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-09 04:56:14.048290 biobookshelf-0.2.5/biobookshelf.egg-info/
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      571 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/PKG-INFO
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     1538 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/SOURCES.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        1 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/dependency_links.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      394 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/entry_points.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      480 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/requires.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       13 2023-05-09 04:56:13.000000 biobookshelf-0.2.5/biobookshelf.egg-info/top_level.txt
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2023-05-09 04:56:14.668303 biobookshelf-0.2.5/setup.cfg
--rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2122 2023-05-09 04:55:14.000000 biobookshelf-0.2.5/setup.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.926895 biobookshelf-0.2.6/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    34600 2022-04-04 14:27:30.000000 biobookshelf-0.2.6/LICENSE
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        0 2022-04-04 14:27:30.000000 biobookshelf-0.2.6/MANIFEST.in
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      598 2023-05-18 11:51:21.922895 biobookshelf-0.2.6/PKG-INFO
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      221 2022-04-04 14:27:30.000000 biobookshelf-0.2.6/README.md
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:20.750867 biobookshelf-0.2.6/biobookshelf/
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:20.890871 biobookshelf-0.2.6/biobookshelf/BA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       30 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/BA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     7975 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/BA/bitarray_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:20.938872 biobookshelf-0.2.6/biobookshelf/CLI/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/CLI/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3013 2023-05-02 03:16:15.000000 biobookshelf-0.2.6/biobookshelf/CLI/unclassified_programs.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.006873 biobookshelf-0.2.6/biobookshelf/INT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/INT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      389 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/INT/integer.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.050875 biobookshelf-0.2.6/biobookshelf/IT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       35 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/IT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       32 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/IT/interval_tree_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.086875 biobookshelf-0.2.6/biobookshelf/L/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/L/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       39 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/L/l_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.122876 biobookshelf-0.2.6/biobookshelf/MAP/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/MAP/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      594 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/MAP/mapping.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.162877 biobookshelf-0.2.6/biobookshelf/MP/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       37 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/MP/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      260 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/MP/multiprocessing_utils.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.182878 biobookshelf-0.2.6/biobookshelf/ONT/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       34 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/ONT/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    70067 2023-05-17 10:45:05.000000 biobookshelf-0.2.6/biobookshelf/ONT/nanopore_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.250879 biobookshelf-0.2.6/biobookshelf/PD/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/PD/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       85 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/PD/pd_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.318881 biobookshelf-0.2.6/biobookshelf/PDB/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       19 2022-04-04 14:27:31.000000 biobookshelf-0.2.6/biobookshelf/PDB/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    29100 2023-05-02 03:16:15.000000 biobookshelf-0.2.6/biobookshelf/PDB/pdb.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.370882 biobookshelf-0.2.6/biobookshelf/PKG/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       28 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/PKG/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     3095 2023-05-02 03:16:15.000000 biobookshelf-0.2.6/biobookshelf/PKG/package_util.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.414883 biobookshelf-0.2.6/biobookshelf/RNA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/RNA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    19437 2023-05-01 11:20:30.000000 biobookshelf-0.2.6/biobookshelf/RNA/rnaseq.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.478885 biobookshelf-0.2.6/biobookshelf/SAM/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2022-04-04 14:27:31.000000 biobookshelf-0.2.6/biobookshelf/SAM/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    69402 2023-05-01 11:20:32.000000 biobookshelf-0.2.6/biobookshelf/SAM/sam_util.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.550886 biobookshelf-0.2.6/biobookshelf/SC/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       27 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/SC/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   127184 2023-05-17 10:47:42.000000 biobookshelf-0.2.6/biobookshelf/SC/single_cell.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.598887 biobookshelf-0.2.6/biobookshelf/SEQ/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       24 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/SEQ/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14831 2023-05-02 03:16:15.000000 biobookshelf-0.2.6/biobookshelf/SEQ/sequence.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.654888 biobookshelf-0.2.6/biobookshelf/STR/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       22 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/STR/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)    14367 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/STR/string.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.722890 biobookshelf-0.2.6/biobookshelf/UniProt/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       23 2022-04-04 14:27:31.000000 biobookshelf-0.2.6/biobookshelf/UniProt/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      837 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/UniProt/uniprot.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.786892 biobookshelf-0.2.6/biobookshelf/WEB/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       31 2022-04-04 14:27:31.000000 biobookshelf-0.2.6/biobookshelf/WEB/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     8727 2023-05-02 03:16:15.000000 biobookshelf-0.2.6/biobookshelf/WEB/web_application.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.826893 biobookshelf-0.2.6/biobookshelf/ZA/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       26 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/ZA/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       12 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/ZA/zarr_utils.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      370 2023-05-17 10:43:00.000000 biobookshelf-0.2.6/biobookshelf/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      162 2023-05-01 11:20:29.000000 biobookshelf-0.2.6/biobookshelf/__main__.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:21.882894 biobookshelf-0.2.6/biobookshelf/main/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2022-04-18 07:53:18.000000 biobookshelf-0.2.6/biobookshelf/main/__init__.py
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)   712244 2023-05-02 03:16:15.000000 biobookshelf-0.2.6/biobookshelf/main/unclassified_functions.py
+drwxrwxr-x   0 merit_an  (1001) merit_an  (1001)        0 2023-05-18 11:51:20.846870 biobookshelf-0.2.6/biobookshelf.egg-info/
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      598 2023-05-18 11:51:19.000000 biobookshelf-0.2.6/biobookshelf.egg-info/PKG-INFO
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     1538 2023-05-18 11:51:19.000000 biobookshelf-0.2.6/biobookshelf.egg-info/SOURCES.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)        1 2023-05-18 11:51:19.000000 biobookshelf-0.2.6/biobookshelf.egg-info/dependency_links.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      394 2023-05-18 11:51:19.000000 biobookshelf-0.2.6/biobookshelf.egg-info/entry_points.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)      480 2023-05-18 11:51:19.000000 biobookshelf-0.2.6/biobookshelf.egg-info/requires.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       13 2023-05-18 11:51:19.000000 biobookshelf-0.2.6/biobookshelf.egg-info/top_level.txt
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)       38 2023-05-18 11:51:21.926895 biobookshelf-0.2.6/setup.cfg
+-rw-rw-r--   0 merit_an  (1001) merit_an  (1001)     2155 2023-05-17 10:47:42.000000 biobookshelf-0.2.6/setup.py
```

### Comparing `biobookshelf-0.2.5/LICENSE` & `biobookshelf-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/PKG-INFO` & `biobookshelf-0.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: biobookshelf
-Version: 0.2.5
+Version: 0.2.6
 Summary: a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python
 Home-page: https://github.com/ahs2202/biobookshelf
 Author: Hyunsu An
 Author-email: ahs2202@gm.gist.ac.kr
 License: GPLv3
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Bio-Bookshelf
 
 [![PyPI version](https://badge.fury.io/py/biobookshelf.svg)](https://badge.fury.io/py/biobookshelf)
```

### Comparing `biobookshelf-0.2.5/biobookshelf/BA/bitarray_utils.py` & `biobookshelf-0.2.6/biobookshelf/BA/bitarray_utils.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/CLI/unclassified_programs.py` & `biobookshelf-0.2.6/biobookshelf/CLI/unclassified_programs.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/MAP/mapping.py` & `biobookshelf-0.2.6/biobookshelf/MAP/mapping.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/ONT/nanopore_functions.py` & `biobookshelf-0.2.6/biobookshelf/ONT/nanopore_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,26 @@
         n_threads=int_num_cpus,
         drop_unaligned=False,
         return_bash_shellscript=False,
         path_file_junc_bed=path_file_splice_junc,
     )  # perform alignment
 
 
-
 def create_gene_count_from_raw_ont_data(
     l_path_folder_nanopore_sequencing_data: Union[
         str, list, None
     ] = None,  # list of folders containing nanopore sequencing data
     l_name_config: Union[str, List] = None,  # a name of config or a list of name_config
     l_barcoding_kit: Union[
         str, List, None
     ] = None,  # a name of barcoding kit or a list of barcoding kits. if barcoding kits were not used, use None
     path_folder_output: Union[str, None] = None,  # a path to the output folder
-    dict_name_bc_to_name_sample: Union[str, dict, None] = None,  # barcode to name_sample
+    dict_name_bc_to_name_sample: Union[
+        str, dict, None
+    ] = None,  # barcode to name_sample
     dict_name_sample_to_organism: Union[
         dict, None
     ] = None,  # define organism for each sample
     dict_anno: Union[
         dict, None
     ] = None,  # a dictionary containing annotation information for each organism
     int_num_cpus: Union[
@@ -52,15 +53,15 @@
     flag_include_failed: bool = True,  # include the failed reads into the fastq output
     int_max_num_reads_for_drawing_size_distribution: int = 100000,  # the maximum number of reads to use to draw a size distribution
     int_max_size_for_displaying_size_distribution: int = 2000,  # max molecule length to display in the histogram
     int_num_bins_for_displaying_size_distribution: int = 200,  # number of bins for drawing histogram
     flag_require_barcodes_both_ends: bool = True,  # require barcodes for both ends. if unclassified are too large, consider turning of this option to recover barcodes from the unclassified reads.
     flag_rerun_guppy=False,  # rename the the output folder (if it exists) and rerun guppy if the flag is True
 ):
-    """# 2023-05-09 00:42:08 
+    """# 2023-05-09 00:42:08
     l_path_folder_nanopore_sequencing_data : list, # list of folders containing nanopore sequencing data
     l_name_config : Union[ str, List ], # a name of config or a list of name_config
     l_barcoding_kit : Union[ str, List, None ], # a name of barcoding kit or a list of barcoding kits. if barcoding kits were not used, use None
     path_folder_output : str, # a path to the output folder
     dict_name_bc_to_name_sample : Union[ dict, str, None ], # barcode to name_sample. if not given, exit after combining fastq files. If barcoding is not used, a single string representing name of the sample can be given.
     dict_name_sample_to_organism : Union[ dict, None ], # define organism for each sample. if not given, does not align reads to genome and transcriptomes
     dict_anno : Union[ dict, None ], # a dictionary containing annotation information for each organism. if not given, does not align reads to genome and transcriptomes
@@ -118,35 +119,63 @@
 
         for path_folder_nanopore_data, name_config, id_barcoding_kit in zip(
             l_path_folder_nanopore_sequencing_data, l_name_config, l_barcoding_kit
         ):
             # retrieve a flag indicating the barcoding kit was used.
             flag_barcoding = id_barcoding_kit is not None
             # automatically detect output file type
-            raw_data_type = 'fast5' if len( glob.glob(f"{path_folder_nanopore_data}fast5*/") ) > 0 else 'pod5'
+            raw_data_type = (
+                "fast5"
+                if len(glob.glob(f"{path_folder_nanopore_data}fast5*/")) > 0
+                else "pod5"
+            )
             # create folders
             path_folder_raw = f"{path_folder_nanopore_data}{raw_data_type}_all/"
             path_folder_guppy_output = f"{path_folder_nanopore_data}guppy_out/"
             for path_folder in [path_folder_raw, path_folder_guppy_output]:
                 os.makedirs(path_folder, exist_ok=True)
             # if skipped raw data does not exist, indicating all raw data has been analyzed by MinKNOW, search for fastq output files and move the fastq output files to the guppy_out folder
-            if not os.path.exists(f"{path_folder_nanopore_data}{raw_data_type}_skip/") and len( glob.glob(f"{path_folder_nanopore_data}fastq*/") ) > 0 : # if skipped raw data does not exist and fastq output files exist, move these files into the guppy_out folder
-                bk.OS_Run( ["mv", f"{path_folder_nanopore_data}fastq_fail/", f"{path_folder_nanopore_data}guppy_out/fail/" ] ) 
-                bk.OS_Run( ["mv", f"{path_folder_nanopore_data}fastq_pass/", f"{path_folder_nanopore_data}guppy_out/pass/" ] ) 
-                with open( f"{path_folder_guppy_output}sequencing_summary.txt", 'w' ) as newfile : # create a file that functions as a flag.
-                    newfile.write( 'minknow output' )
+            if (
+                not os.path.exists(f"{path_folder_nanopore_data}{raw_data_type}_skip/")
+                and len(glob.glob(f"{path_folder_nanopore_data}fastq*/")) > 0
+            ):  # if skipped raw data does not exist and fastq output files exist, move these files into the guppy_out folder
+                bk.OS_Run(
+                    [
+                        "mv",
+                        f"{path_folder_nanopore_data}fastq_fail/",
+                        f"{path_folder_nanopore_data}guppy_out/fail/",
+                    ]
+                )
+                bk.OS_Run(
+                    [
+                        "mv",
+                        f"{path_folder_nanopore_data}fastq_pass/",
+                        f"{path_folder_nanopore_data}guppy_out/pass/",
+                    ]
+                )
+                with open(
+                    f"{path_folder_guppy_output}sequencing_summary.txt", "w"
+                ) as newfile:  # create a file that functions as a flag.
+                    newfile.write("minknow output")
 
             # collect raw output files
             for path_file in (
-                glob.glob(f"{path_folder_nanopore_data}{raw_data_type}_skip/*.{raw_data_type}")
-                + glob.glob(f"{path_folder_nanopore_data}{raw_data_type}_fail/{'*/' if flag_barcoding else ''}*.{raw_data_type}")
-                + glob.glob(f"{path_folder_nanopore_data}{raw_data_type}_pass/{'*/' if flag_barcoding else ''}*.{raw_data_type}")
+                glob.glob(
+                    f"{path_folder_nanopore_data}{raw_data_type}_skip/*.{raw_data_type}"
+                )
+                + glob.glob(
+                    f"{path_folder_nanopore_data}{raw_data_type}_fail/{'*/' if flag_barcoding else ''}*.{raw_data_type}"
+                )
+                + glob.glob(
+                    f"{path_folder_nanopore_data}{raw_data_type}_pass/{'*/' if flag_barcoding else ''}*.{raw_data_type}"
+                )
             ):
                 os.rename(
-                    path_file, f"{path_folder_raw}{bk.UUID( )}.{path_file.rsplit( '/', 1 )[ 1 ]}" # add uuid to avoid collision
+                    path_file,
+                    f"{path_folder_raw}{bk.UUID( )}.{path_file.rsplit( '/', 1 )[ 1 ]}",  # add uuid to avoid collision
                 )
 
             # run guppy
             l_args = [
                 "guppy_basecaller",
                 "-c",
                 name_config,
@@ -158,15 +187,17 @@
                 "auto",
                 "--compress_fastq",
             ]
             if (
                 flag_require_barcodes_both_ends
             ):  # if 'flag_require_barcodes_both_ends' is True
                 l_args += ["--require_barcodes_both_ends"]
-            if id_barcoding_kit is not None:  # if valid 'id_barcoding_kit' has been given
+            if (
+                id_barcoding_kit is not None
+            ):  # if valid 'id_barcoding_kit' has been given
                 l_args += ["--barcode_kits", id_barcoding_kit]
             print(" ".join(l_args))  # print the guppy_basecaller command
 
             flag_output_exists = os.path.exists(
                 f"{path_folder_guppy_output}sequencing_summary.txt"
             )  # retrieve a flag indicating that the guppy output folder already exists
             if (
@@ -202,51 +233,62 @@
         )
 
         # filter fastq files
         if not flag_include_failed:
             df_fq = PD_Select(df_fq, wildcard_0="pass")  # use only passed reads.
 
         # combine fastq files
-        if flag_barcoding : # combine files for each barcode
+        if flag_barcoding:  # combine files for each barcode
             for name_bc in df_fq.wildcard_1.unique():
                 df_fq_for_name_bc = bk.PD_Select(df_fq, wildcard_1=name_bc)
-                path_file_output= f"{path_folder_output}{name_bc}.fastq.gz"
+                path_file_output = f"{path_folder_output}{name_bc}.fastq.gz"
                 path_file_temp = f"{path_folder_output}{name_bc}.fastq.gz.partial"
                 bk.OS_Run(
                     ["cat"] + list(df_fq_for_name_bc.path.values),
                     path_file_stdout=path_file_temp,
                     stdout_binary=True,
-                ) # combine fastq files into a single temorary file
-                os.rename( path_file_temp, path_file_output ) # rename the temporary file to the output file
-        else :
-            path_file_output= f"{path_folder_output}combined.fastq.gz"
+                )  # combine fastq files into a single temorary file
+                os.rename(
+                    path_file_temp, path_file_output
+                )  # rename the temporary file to the output file
+        else:
+            path_file_output = f"{path_folder_output}combined.fastq.gz"
             path_file_temp = f"{path_folder_output}combined.fastq.gz.partial"
             bk.OS_Run(
                 ["cat"] + list(df_fq.path.values),
                 path_file_stdout=path_file_temp,
                 stdout_binary=True,
-            ) # combine fastq files into a single temorary file
-            os.rename( path_file_temp, path_file_output ) # rename the temporary file to the output file
+            )  # combine fastq files into a single temorary file
+            os.rename(
+                path_file_temp, path_file_output
+            )  # rename the temporary file to the output file
 
     # if 'dict_name_bc_to_name_sample' has given, rename fastq files and remove files that are not needed.
     if dict_name_bc_to_name_sample is not None:
-        if flag_barcoding and isinstance( dict_name_bc_to_name_sample, dict ) :
+        if flag_barcoding and isinstance(dict_name_bc_to_name_sample, dict):
             for path_file_fq in glob.glob(
                 f"{path_folder_pipeline}*.fastq.gz"
             ):  # for each fastq file
                 name_file = path_file_fq.rsplit("/", 1)[1].rsplit(".fastq.gz", 1)[0]
                 if (
                     name_file in dict_name_bc_to_name_sample
                 ):  # if 'name_sample' is available for the barcode, rename the file
                     name_sample = dict_name_bc_to_name_sample[name_file]
-                    os.rename(path_file_fq, f"{path_folder_pipeline}{name_sample}.fastq.gz")
+                    os.rename(
+                        path_file_fq, f"{path_folder_pipeline}{name_sample}.fastq.gz"
+                    )
                 else:  # if 'name_sample' is not available for the barcode, remove the file
                     os.remove(path_file_fq)
-        elif not flag_barcoding and isinstance( dict_name_bc_to_name_sample, str ) : # if barcoding was not used.
-            os.rename(f"{path_folder_pipeline}combined.fastq.gz", f"{path_folder_pipeline}{dict_name_bc_to_name_sample}.fastq.gz")
+        elif not flag_barcoding and isinstance(
+            dict_name_bc_to_name_sample, str
+        ):  # if barcoding was not used.
+            os.rename(
+                f"{path_folder_pipeline}combined.fastq.gz",
+                f"{path_folder_pipeline}{dict_name_bc_to_name_sample}.fastq.gz",
+            )
 
     # draw molecule length distribution of each sample
     df_fastq = bk.GLOB_Retrive_Strings_in_Wildcards(
         f"{path_folder_pipeline}*.fastq.gz"
     )  # retrieve the paths of input fastq files
     int_num_samples = len(
         df_fastq
@@ -511,14 +553,16 @@
         )
         os.makedirs(
             f"{path_folder_graph}accumulated_sequencing_throughput/", exist_ok=True
         )  # create the output folder
         fig.write_html(
             f"{path_folder_graph}accumulated_sequencing_throughput/{name_sample}.accumulated_sequencing_throughput.gene_level.html"
         )  # write the graph
+
+
 create_gene_count_from_fast5 = create_gene_count_from_raw_ont_data
 
 
 def Guppy_Run_and_Combine_Output(
     path_folder_nanopore_sequencing_data=None,
     flag_barcoding_was_used=False,
     path_folder_output_fastq=None,
```

### Comparing `biobookshelf-0.2.5/biobookshelf/PDB/pdb.py` & `biobookshelf-0.2.6/biobookshelf/PDB/pdb.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/PKG/package_util.py` & `biobookshelf-0.2.6/biobookshelf/PKG/package_util.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/RNA/rnaseq.py` & `biobookshelf-0.2.6/biobookshelf/RNA/rnaseq.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/SAM/sam_util.py` & `biobookshelf-0.2.6/biobookshelf/SAM/sam_util.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/SC/single_cell.py` & `biobookshelf-0.2.6/biobookshelf/SC/single_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,119 @@
 import base64  # for converting binary to text data (web application)
 import json  # to read and write JSON file
 import matplotlib.pyplot as plt
 import scipy.sparse
 import io
 import concurrent.futures  # for multiprocessing
 
+
+# functions for various file system access
+def filesystem_operations(
+    method: Literal["exists", "rm", "glob", "mkdir", "mv", "cp", "isdir"],
+    path_src: str,
+    path_dest: Union[str, None] = None,
+    flag_recursive: bool = True,
+    dict_kwargs_credentials_s3: dict = dict(),
+    **kwargs,
+):
+    """# 2022-12-04 00:57:45
+    perform a file system operation (either Amazon S3 or local file system)
+
+    method : Literal[
+        'exists', # check whether a file or folder exists, given through 'path_src' arguments
+        'rm', # remove file or folder, given through 'path_src' arguments
+        'glob', # retrieve path of files matching the glob pattern, given through 'path_src' arguments
+        'mkdir', # create a directory, given through 'path_src' arguments
+        'mv', # move file or folder , given through 'path_src' and 'path_dest' arguments
+        'cp', # copy file or folder , given through 'path_src' and 'path_dest' arguments
+        'isdir', # check whether the given input is a file or directory
+    ]
+
+    kwargs :
+        exist_ok : for 'mkdir' operation
+
+    dict_kwargs_credentials_s3 : dict = dict( ) # the credentials for the Amazon S3 file system as keyworded arguments
+
+    """
+    if is_s3_url(path_src) or is_s3_url(
+        path_dest
+    ):  # if at least one path is s3 locations
+        # %% Amazon s3 file system %%
+        # load the file system
+        import s3fs
+
+        fs = s3fs.S3FileSystem(**dict_kwargs_credentials_s3)
+        if method == "exists":
+            return fs.exists(path_src, **kwargs)
+        elif method == "rm":
+            return fs.rm(path_src, recursive=flag_recursive, **kwargs)  # delete files
+        elif method == "glob":
+            return list(
+                "s3://" + e for e in fs.glob(path_src, **kwargs)
+            )  # 's3://' prefix should be added
+        elif method == "mkdir":
+            # use default 'exist_ok' value
+            if "exist_ok" not in kwargs:
+                kwargs["exist_ok"] = True
+            return fs.makedirs(path_src, **kwargs)
+        elif method == "mv":
+            if not fs.exists(
+                path_dest, **kwargs
+            ):  # avoid overwriting of the existing file
+                return fs.mv(path_src, path_dest, recursive=flag_recursive, **kwargs)
+            else:
+                return "destionation file already exists, exiting"
+        elif method == "cp":
+            if is_s3_url(path_src) and is_s3_url(path_dest):  # copy from s3 to s3
+                return fs.copy(path_src, path_dest, recursive=flag_recursive, **kwargs)
+            elif is_s3_url(path_src):  # copy from s3 to local
+                return fs.get(path_src, path_dest, recursive=flag_recursive, **kwargs)
+            elif is_s3_url(path_dest):  # copy from local to s3
+                return fs.put(path_src, path_dest, recursive=flag_recursive, **kwargs)
+        elif method == "isdir":
+            return fs.isdir(path_src)
+    elif is_http_url(path_src):  # for http
+        # %% HTTP server %%
+        if method == "exists":
+            return (
+                http_response_code(path_src) == 200
+            )  # check whether http file (not tested for directory) exists
+        else:
+            return "not implemented"
+    else:
+        # %% local file system %%
+        if method == "exists":
+            return os.path.exists(path_src)
+        elif method == "rm":
+            if flag_recursive and os.path.isdir(
+                path_src
+            ):  # when the recursive option is active
+                shutil.rmtree(path_src)
+            else:
+                os.remove(path_src)
+        elif method == "glob":
+            return glob.glob(path_src)
+        elif method == "mkdir":
+            # use default 'exist_ok' value
+            if "exist_ok" not in kwargs:
+                kwargs["exist_ok"] = True
+            os.makedirs(path_src, exist_ok=kwargs["exist_ok"])
+        elif method == "mv":
+            shutil.move(path_src, path_dest)
+        elif method == "cp":
+            if flag_recursive and os.path.isdir(
+                path_src
+            ):  # when the recursive option is active
+                shutil.copytree(path_src, path_dest)
+            else:
+                shutil.copyfile(path_src, path_dest)
+        elif method == "isdir":
+            return os.path.isdir(path_src)
+
+
 """ previosuly written for biobookshelf """
 
 
 def CB_Parse_list_of_id_cell(l_id_cell, dropna=True):
     """# 2022-03-25 16:35:23
     parse a given list of id_cells into a dataframe using 'SC.CB_detect_cell_barcode_from_id_cell' function
     'dropna' : drop id_cells that does not contains cell barcodes
```

### Comparing `biobookshelf-0.2.5/biobookshelf/SEQ/sequence.py` & `biobookshelf-0.2.6/biobookshelf/SEQ/sequence.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/STR/string.py` & `biobookshelf-0.2.6/biobookshelf/STR/string.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/UniProt/uniprot.py` & `biobookshelf-0.2.6/biobookshelf/UniProt/uniprot.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/WEB/web_application.py` & `biobookshelf-0.2.6/biobookshelf/WEB/web_application.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf/main/unclassified_functions.py` & `biobookshelf-0.2.6/biobookshelf/main/unclassified_functions.py`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/biobookshelf.egg-info/PKG-INFO` & `biobookshelf-0.2.6/biobookshelf.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: biobookshelf
-Version: 0.2.5
+Version: 0.2.6
 Summary: a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python
 Home-page: https://github.com/ahs2202/biobookshelf
 Author: Hyunsu An
 Author-email: ahs2202@gm.gist.ac.kr
 License: GPLv3
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Bio-Bookshelf
 
 [![PyPI version](https://badge.fury.io/py/biobookshelf.svg)](https://badge.fury.io/py/biobookshelf)
```

### Comparing `biobookshelf-0.2.5/biobookshelf.egg-info/SOURCES.txt` & `biobookshelf-0.2.6/biobookshelf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobookshelf-0.2.5/setup.py` & `biobookshelf-0.2.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="biobookshelf",
-    version="0.2.5",
+    version="0.2.6",
     author="Hyunsu An",
     author_email="ahs2202@gm.gist.ac.kr",
     description="a collection of python scripts and functions for exploratory analysis of bioinformatic data in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/ahs2202/biobookshelf",
     license="GPLv3",
     packages=find_packages(include=["biobookshelf", "biobookshelf.*"]),
     include_package_data=True,
+    python_requires=">=3.8, <4",
     install_requires=[
         "ipython>=7.19.0",
         "plotly>=4.11.0",
         "plotnine>=0.10.1",
         "pandas>=1.1.4",
         "numpy>=1.18.5",
         "pysam>=0.16.0.1",
```

