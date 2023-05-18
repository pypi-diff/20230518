# Comparing `tmp/hollihop_api_client-0.0.3.tar.gz` & `tmp/hollihop_api_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hollihop_api_client-0.0.3.tar", last modified: Thu May 18 11:39:24 2023, max compression
+gzip compressed data, was "hollihop_api_client-0.0.4.tar", last modified: Thu May 18 12:11:03 2023, max compression
```

## Comparing `hollihop_api_client-0.0.3.tar` & `hollihop_api_client-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.401786 hollihop_api_client-0.0.3/
--rw-r--r--   0 malts.tech   (501) staff       (20)     1073 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/LICENSE
--rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-18 11:39:24.401646 hollihop_api_client-0.0.3/PKG-INFO
--rw-r--r--   0 malts.tech   (501) staff       (20)     1753 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/README.md
--rw-r--r--   0 malts.tech   (501) staff       (20)      716 2023-05-18 11:39:04.000000 hollihop_api_client-0.0.3/pyproject.toml
--rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-18 11:39:24.401821 hollihop_api_client-0.0.3/setup.cfg
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.393800 hollihop_api_client-0.0.3/src/
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.395381 hollihop_api_client-0.0.3/src/hollihop_api_client/
--rw-r--r--   0 malts.tech   (501) staff       (20)       94 2023-05-18 11:24:48.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/__init__.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.396467 hollihop_api_client-0.0.3/src/hollihop_api_client/api/
--rw-r--r--   0 malts.tech   (501) staff       (20)      138 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/api/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      594 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/api/abc.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     2687 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/api/api.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.396796 hollihop_api_client-0.0.3/src/hollihop_api_client/base/
--rw-r--r--   0 malts.tech   (501) staff       (20)       63 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/base/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      520 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/base/category.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      933 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/categories.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.397749 hollihop_api_client-0.0.3/src/hollihop_api_client/methods/
--rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/methods/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     6766 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/methods/ed_unit_students.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     6434 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/methods/ed_units.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     2765 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/methods/leads.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1303 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/methods/locations.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1611 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/methods/offices.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1436 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/test.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.399239 hollihop_api_client-0.0.3/src/hollihop_api_client/tests/
--rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-03-11 10:01:33.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/tests/__init__.py
--rw-r--r--   0 malts.tech   (501) staff       (20)     1528 2023-03-12 11:14:09.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/tests/conftest.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      474 2023-03-12 18:14:57.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/tests/test_ed_unit_students.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      995 2023-03-12 11:19:09.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/tests/test_ed_units.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      165 2023-03-12 11:17:10.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/tests/test_lead.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      374 2023-03-12 11:16:33.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/tests/test_locations.py
--rw-r--r--   0 malts.tech   (501) staff       (20)      636 2023-03-12 11:15:54.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/tests/test_offices.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.399489 hollihop_api_client-0.0.3/src/hollihop_api_client/tools/
--rw-r--r--   0 malts.tech   (501) staff       (20)     3143 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/tools/__init__.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.394221 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.401451 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      673 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2html.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      795 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2html4.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)     1130 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2html5.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      872 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2latex.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      695 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2man.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      861 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2odt.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      667 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      680 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      716 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2s5.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      952 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2xetex.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      681 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2xml.py
--rwxr-xr-x   0 malts.tech   (501) staff       (20)      749 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rstpep2html.py
-drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:39:24.395944 hollihop_api_client-0.0.3/src/hollihop_api_client.egg-info/
--rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-18 11:39:24.000000 hollihop_api_client-0.0.3/src/hollihop_api_client.egg-info/PKG-INFO
--rw-r--r--   0 malts.tech   (501) staff       (20)     1709 2023-05-18 11:39:24.000000 hollihop_api_client-0.0.3/src/hollihop_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 malts.tech   (501) staff       (20)        1 2023-05-18 11:39:24.000000 hollihop_api_client-0.0.3/src/hollihop_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 malts.tech   (501) staff       (20)       20 2023-05-18 11:39:24.000000 hollihop_api_client-0.0.3/src/hollihop_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.940166 hollihop_api_client-0.0.4/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1073 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/LICENSE
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-18 12:11:03.940019 hollihop_api_client-0.0.4/PKG-INFO
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1753 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/README.md
+-rw-r--r--   0 malts.tech   (501) staff       (20)      716 2023-05-18 12:10:53.000000 hollihop_api_client-0.0.4/pyproject.toml
+-rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-18 12:11:03.940204 hollihop_api_client-0.0.4/setup.cfg
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.926486 hollihop_api_client-0.0.4/src/
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.927908 hollihop_api_client-0.0.4/src/hollihop_api_client/
+-rw-r--r--   0 malts.tech   (501) staff       (20)       94 2023-05-18 11:24:48.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/__init__.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.934952 hollihop_api_client-0.0.4/src/hollihop_api_client/api/
+-rw-r--r--   0 malts.tech   (501) staff       (20)      138 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/api/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      594 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/api/abc.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2667 2023-05-18 12:10:40.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/api/api.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.935384 hollihop_api_client-0.0.4/src/hollihop_api_client/base/
+-rw-r--r--   0 malts.tech   (501) staff       (20)       63 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/base/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      520 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/base/category.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      933 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/categories.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.936402 hollihop_api_client-0.0.4/src/hollihop_api_client/methods/
+-rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/methods/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     6766 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/methods/ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     6434 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/methods/ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2765 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/methods/leads.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1303 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/methods/locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1611 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/methods/offices.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1436 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/test.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.937736 hollihop_api_client-0.0.4/src/hollihop_api_client/tests/
+-rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-03-11 10:01:33.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/tests/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1528 2023-03-12 11:14:09.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/tests/conftest.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      474 2023-03-12 18:14:57.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/tests/test_ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      995 2023-03-12 11:19:09.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/tests/test_ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      165 2023-03-12 11:17:10.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/tests/test_lead.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      374 2023-03-12 11:16:33.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/tests/test_locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      636 2023-03-12 11:15:54.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/tests/test_offices.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.937980 hollihop_api_client-0.0.4/src/hollihop_api_client/tools/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     3143 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/tools/__init__.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.926891 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.939828 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      673 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2html.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      795 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2html4.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)     1130 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2html5.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      872 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2latex.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      695 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2man.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      861 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2odt.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      667 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      680 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      716 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2s5.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      952 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      681 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2xml.py
+-rwxr-xr-x   0 malts.tech   (501) staff       (20)      749 2023-05-18 11:11:38.000000 hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rstpep2html.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 12:11:03.934336 hollihop_api_client-0.0.4/src/hollihop_api_client.egg-info/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-18 12:11:03.000000 hollihop_api_client-0.0.4/src/hollihop_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1709 2023-05-18 12:11:03.000000 hollihop_api_client-0.0.4/src/hollihop_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)        1 2023-05-18 12:11:03.000000 hollihop_api_client-0.0.4/src/hollihop_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)       20 2023-05-18 12:11:03.000000 hollihop_api_client-0.0.4/src/hollihop_api_client.egg-info/top_level.txt
```

### Comparing `hollihop_api_client-0.0.3/LICENSE` & `hollihop_api_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/PKG-INFO` & `hollihop_api_client-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hollihop_api_client
-Version: 0.0.3
+Version: 0.0.4
 Summary: This library helps you easily create a python application with Hollihop API
 Author-email: Nicholas Maltseb <nmmaltsev@outlook.com>
 Project-URL: Homepage, https://github.com/nicholasChieftain/hollihop_api_client/
 Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollihop_api_client/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `hollihop_api_client-0.0.3/README.md` & `hollihop_api_client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/pyproject.toml` & `hollihop_api_client-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hollihop_api_client"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Nicholas Maltseb", email="nmmaltsev@outlook.com" },
 ]
 description = "This library helps you easily create a python application with Hollihop API"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/api/abc.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/api/abc.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/api/api.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,92 +1,95 @@
 from typing import NoReturn, TYPE_CHECKING
 
 from requests import Response, Session, get
 
+from hollihop_api_client.categories import APICategories
+
 from .abc import AbstractAPI
 
 
 class HolliHopAPIError(Exception):
     _response_not_ok = '''Запрос к {url} не выполнен.
     Статус код {status_code}.
     {error_message}'''
     _other_errors = '''{error_message}'''
 
     def __init__(
             self,
             error_message: str,
             status_code: None | int = None,
             url: None | str = None
-            ):
+    ):
         self._status_code = status_code
         self._error_message = error_message
         self._url = url
 
     def __str__(self) -> str:
         if self._status_code is None:
             return self._other_errors.format(
-                    error_message=self._error_message
-                    )
+                error_message=self._error_message
+            )
         else:
             return self._response_not_ok.format(
-                    url=self._url,
-                    status_code=self._status_code,
-                    error_message=self._error_message
-                )
+                url=self._url,
+                status_code=self._status_code,
+                error_message=self._error_message
+            )
 
 
 class HolliHopAPI(AbstractAPI):
     __api_version__ = 'Api/V2/'
 
     def __init__(
             self,
             domain: str = None,
             api_key: str = None
-            ):
+    ):
         if api_key is None:
             raise HolliHopAPIError(
-                    error_message='Не указан ключ доступа к API'
-                    )
+                error_message='Не указан ключ доступа к API'
+            )
         if domain is None:
             raise HolliHopAPIError(
-                    error_message='Не указан домен для доступа к API'
-                    )
+                error_message='Не указан домен для доступа к API'
+            )
         self._domain = domain
         self._api_key = api_key
 
         super().__init__(self)
+        self.categories = APICategories(self)
 
     def request(
             self,
             method: str,
             http_method: str = 'GET',
             data: dict | None = None
-            ) -> None | dict:
+    ) -> None | dict:
         url = self._domain + self.__api_version__ + method
         data.update({'authkey': self._api_key})
         with Session() as session:
             response = session.request(
-                    method=http_method,
-                    url=url,
-                    data=data,
-                    )
+                method=http_method,
+                url=url,
+                data=data,
+            )
 
         response = self._validate_response(response)
 
         return response
 
     def _validate_response(
             self,
             response: Response,
-            ) -> (None | dict) | NoReturn:
+    ) -> (None | dict) | NoReturn:
         if response.status_code == 200:
             return response.json()
         else:
             print(response.json())
             raise HolliHopAPIError(
-                    response.url,
-                    response.status_code,
-                    'Ошибка выполнения запроса'
-                    )
+                response.url,
+                response.status_code,
+                'Ошибка выполнения запроса'
+            )
 
 
 __all__ = ['HolliHopAPI', 'HolliHopAPIError']
```

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/base/category.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/base/category.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/categories.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/categories.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/methods/ed_unit_students.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/methods/ed_unit_students.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/methods/ed_units.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/methods/ed_units.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/methods/leads.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/methods/leads.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/methods/locations.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/methods/locations.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/methods/offices.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/methods/offices.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/test.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/test.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/tests/conftest.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/tests/test_ed_units.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/tests/test_ed_units.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/tests/test_offices.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/tests/test_offices.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/tools/__init__.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2html.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2html4.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2html5.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2latex.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2man.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2odt.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2pseudoxml.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2s5.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2xetex.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rst2xml.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client/venv/bin/rstpep2html.py` & `hollihop_api_client-0.0.4/src/hollihop_api_client/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client.egg-info/PKG-INFO` & `hollihop_api_client-0.0.4/src/hollihop_api_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hollihop-api-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: This library helps you easily create a python application with Hollihop API
 Author-email: Nicholas Maltseb <nmmaltsev@outlook.com>
 Project-URL: Homepage, https://github.com/nicholasChieftain/hollihop_api_client/
 Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollihop_api_client/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `hollihop_api_client-0.0.3/src/hollihop_api_client.egg-info/SOURCES.txt` & `hollihop_api_client-0.0.4/src/hollihop_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

