# Comparing `tmp/Digikam-DB-0.2.2.tar.gz` & `tmp/Digikam-DB-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digikam-DB-0.2.2.tar", last modified: Fri May  5 18:51:55 2023, max compression
+gzip compressed data, was "Digikam-DB-0.3.0.tar", last modified: Thu May 18 14:14:14 2023, max compression
```

## Comparing `Digikam-DB-0.2.2.tar` & `Digikam-DB-0.3.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.183555 Digikam-DB-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.167555 Digikam-DB-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.171555 Digikam-DB-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/CHANGELOG.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.171555 Digikam-DB-0.2.2/Digikam_DB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:51:54.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/Digikam_DB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-05 18:51:55.183555 Digikam-DB-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.175555 Digikam-DB-0.2.2/digikamdb/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 18:51:55.000000 Digikam-DB-0.2.2/digikamdb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/albumroots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/albums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/image_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/image_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/digikamdb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.175555 Digikam-DB-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.179555 Digikam-DB-0.2.2/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/_ext/_sqla.py
--rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/_ext/digikam4.db
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/api_albums.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/api_images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/api_tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/meta.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:51:55.183555 Digikam-DB-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.179555 Digikam-DB-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:51:55.183555 Digikam-DB-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/digikamrc.mysql
--rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/digikamrc.mysql-internal
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/digikamrc.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/empty-15.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/empty-15.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/empty.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/empty.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/testdb.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data/testdb.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/digikamrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/imagedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    32756 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/newdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-05 18:51:37.000000 Digikam-DB-0.2.2/tests/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.092073 Digikam-DB-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.080072 Digikam-DB-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.084072 Digikam-DB-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/CHANGELOG.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.084072 Digikam-DB-0.3.0/Digikam_DB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:14:13.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 14:14:14.000000 Digikam-DB-0.3.0/Digikam_DB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-18 14:14:14.092073 Digikam-DB-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.084072 Digikam-DB-0.3.0/digikamdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 14:14:13.000000 Digikam-DB-0.3.0/digikamdb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/albumroots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/image_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/image_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/digikamdb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.088072 Digikam-DB-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.088072 Digikam-DB-0.3.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/_ext/_sqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/_ext/digikam4.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/api_albums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/api_images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/api_tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/meta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 14:14:14.092073 Digikam-DB-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.088072 Digikam-DB-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:14:14.092073 Digikam-DB-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/digikamrc.mysql
+-rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/digikamrc.mysql-internal
+-rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/digikamrc.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/empty-15.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/empty-15.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/empty.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/empty.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/testdb.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data/testdb.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/digikamrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/imagedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32756 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/newdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-18 14:13:57.000000 Digikam-DB-0.3.0/tests/sqlite.py
```

### Comparing `Digikam-DB-0.2.2/.github/workflows/release.yml` & `Digikam-DB-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/.github/workflows/test.yml` & `Digikam-DB-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/Digikam_DB.egg-info/PKG-INFO` & `Digikam-DB-0.3.0/Digikam_DB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digikam-DB
-Version: 0.2.2
+Version: 0.3.0
 Summary: Library to access Digikam metadata
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: documentation, https://digikam-db.readthedocs.io
 Project-URL: homepage, https://github.com/rcw-2/python-digikamdb
 Keywords: digikam
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Digikam-DB-0.2.2/Digikam_DB.egg-info/SOURCES.txt` & `Digikam-DB-0.3.0/Digikam_DB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/LICENSE` & `Digikam-DB-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/PKG-INFO` & `Digikam-DB-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digikam-DB
-Version: 0.2.2
+Version: 0.3.0
 Summary: Library to access Digikam metadata
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: documentation, https://digikam-db.readthedocs.io
 Project-URL: homepage, https://github.com/rcw-2/python-digikamdb
 Keywords: digikam
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Digikam-DB-0.2.2/README.rst` & `Digikam-DB-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/albumroots.py` & `Digikam-DB-0.3.0/digikamdb/albumroots.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,16 @@
             """
             Indicates if this album root is case sensitive.
             
             Raises:
                 DigikamVersionError:    If DBVersion < 16
             
             .. versionadded:: 0.2.2
+            
+            .. todo:: Take ``caseSensitivity`` into account when accessing images.
             """
             if self.digikam.db_version < 16:
                 raise DigikamVersionError(
                     'caseSensitivity is present in DBVersion >= 16'
                 )
             return self._caseSensitivity != 0
```

### Comparing `Digikam-DB-0.2.2/digikamdb/albums.py` & `Digikam-DB-0.3.0/digikamdb/albums.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .table import DigikamTable
 from .exceptions import DigikamDataIntegrityError, DigikamVersionError
 
 
 log = logging.getLogger(__name__)
 
 
-def _album_class(dk: 'Digikam') -> type:                    # noqa: F821
+def _album_class(dk: 'Digikam') -> type:                    # noqa: F821, C901
     """
     Defines the Album class
     """
     
     if not dk.is_mysql:
         from sqlalchemy.dialects import sqlite
```

### Comparing `Digikam-DB-0.2.2/digikamdb/conn.py` & `Digikam-DB-0.3.0/digikamdb/conn.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/exceptions.py` & `Digikam-DB-0.3.0/digikamdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/image_comments.py` & `Digikam-DB-0.3.0/digikamdb/image_comments.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/image_helpers.py` & `Digikam-DB-0.3.0/digikamdb/image_helpers.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/images.py` & `Digikam-DB-0.3.0/digikamdb/images.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/properties.py` & `Digikam-DB-0.3.0/digikamdb/properties.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/settings.py` & `Digikam-DB-0.3.0/digikamdb/settings.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/table.py` & `Digikam-DB-0.3.0/digikamdb/table.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/digikamdb/tags.py` & `Digikam-DB-0.3.0/digikamdb/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             elif isinstance(value, str):
                 self._icon = None
                 self._iconkde = value
             else:
                 raise DigikamAssignmentError('Tag.icon must be Image, str, or None')
         
         @property
-        def images(self) -> Iterable['Image']:              # noqa: F821
+        def images(self) -> Iterable['Image']:                  # noqa: F821
             """Images belonging to the tag (no setter)"""
             return self._images
         
         @property
         def _ancestors(self) -> List:
             """
             Returns the ancestors of a tag.
@@ -211,15 +211,15 @@
             Returns the tag's parent object.
             
             Returns ``None`` for
             
             * the root tag on MySQL or
             * tags at top level on SQLite
             
-            .. todo:: Check for fresh MySQL DB with DBversion > 10
+            .. todo:: Support moving tags
             """
 
             # Tags without a parent
             if self._is_mysql:
                 if self.pid < 0:
                     return None
             else:
```

### Comparing `Digikam-DB-0.2.2/digikamdb/types.py` & `Digikam-DB-0.3.0/digikamdb/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 """Some auxilliary class definitions"""
 
 
 from enum import IntEnum
 from typing import Any, Mapping, Union
 
 
+class ExifEnum(IntEnum):
+    """
+    Adds more readable string representations to Exif types.
+    
+    .. versionadded:: 0.3.0
+    """
+    def __str__(self) -> str:
+        return self.name.capitalize().replace('_', ' ')
+
+
 class AlbumRootStatus(IntEnum):
     """Class for :attr:`AlbumRoot.status<_sqla.AlbumRoot.status>`"""
     LocationAvailable   = 0
     LocationUnavailable = 2
     LocationHidden      = 1
 
 
@@ -50,23 +60,26 @@
     INDEXED             = 4
     YCBCR               = 5
     CMYK                = 6
     CIELAB              = 7
     COLORMODELRAW       = 8
 
 
-class ExifOrientation(IntEnum):
+class ExifOrientation(ExifEnum):
     """
     Exif ImageOrientation Tag
     
     The constants describe the position of row 0 and column 0 in the visual
     image, as specified in the Exif documentation. The mirrored orientations
     will usually not show up in digital photos.
     
     Used by :attr:`ImageInformation.orientation<_sqla.ImageInformation.orientation>`
+    
+    .. versionchanged:: 0.3.0
+        More readable string representation
     """
     #: Landscape, camera held upright
     TOP_LEFT        = 1
     #: 1 mirrored
     TOP_RIGHT       = 2
     #: Landscape, camera held upside down
     BOTTOM_RIGHT    = 3
@@ -78,106 +91,155 @@
     RIGHT_TOP       = 6
     #: 8 mirrored
     RIGHT_BOTTOM    = 7
     #: Portrait, camera turned left
     LEFT_BOTTOM     = 8
 
 
-class ExifExposureMode(IntEnum):
+class ExifExposureMode(ExifEnum):
     """
     Exif ExposureMode Tag
     
     Used by :attr:`ImageMetadata.exposureMode<_sqla.ImageMetadata.exposureMode>`
+    
+    .. versionchanged:: 0.3.0
+        More readable string representation
     """
     AUTO_EXPOSURE   = 0
     MANUAL_EXPOSURE = 1
     AUTO_BRACKET    = 2
 
 
-class ExifExposureProgram(IntEnum):
+class ExifExposureProgram(ExifEnum):
     """
     Exif ExposureProgram Tag
     
     Used by :attr:`ImageMetadata.exposureProgram<_sqla.ImageMetadata.exposureProgram>`
+    
+    .. versionchanged:: 0.3.0
+        More readable string representation
     """
     NOT_DEFINED         = 0
     MANUAL              = 1
     NORMAL_PROGRAM      = 2
     APERTURE_PRIORITY   = 3
     SHUTTER_PRIORITY    = 4
     CREATIVE_PROGRAM    = 5
     ACTION_PROGRAM      = 6
     PORTRAIT_MODE       = 7
     LANDSCAPE_MODE      = 8
 
 
-class ExifWhiteBalance(IntEnum):
+class ExifWhiteBalance(ExifEnum):
     """
     Exif WhiteBalance Tag
     
     Used by :attr:`ImageMetadata.whiteBalance<_sqla.ImageMetadata.whiteBalance>`
+    
+    .. versionchanged:: 0.3.0
+        More readable string representation
     """
     AUTO    = 0
     MANUAL  = 1
 
 
-class ExifMeteringMode(IntEnum):
+class ExifMeteringMode(ExifEnum):
     """
     Exif MeteringMode Tag
     
     Used by :attr:`ImageMetadata.meteringMode<_sqla.ImageMetadata.meteringMode>`
+    
+    .. versionchanged:: 0.3.0
+        More readable string representation
     """
     UNKNOWN                 = 0
     AVERAGE                 = 1
     CENTER_WEIGHTED_AVERAGE = 2
     SPOT                    = 3
     MULTI_SPOT              = 4
     PATTERN                 = 5
     PARTIAL                 = 6
     OTHER                   = 255
 
 
-class ExifSubjectDistanceRange(IntEnum):
+class ExifSubjectDistanceRange(ExifEnum):
     """
     Exif SubjectDistanceRange
     
     Used by
     :attr:`ImageMetadata.subjectDistanceCategory<_sqla.ImageMetadata.subjectDistanceCategory>`
+    
+    .. versionchanged:: 0.3.0
+        More readable string representation
     """                                                     # noqa: E501
     UNKNOWN         = 0
     MACRO           = 1
     CLOSE_VIEW      = 2
     DISTANT_VIEW    = 3
 
 
-class ExifFlashReturn(IntEnum):
-    """Exif Flash Return (part of :class:`ExifFlash` Tag)"""
+_exif_flash_return_str_value = [
+    'No detection function',
+    '(reserved)',
+    'Return not detected',
+    'Return detected'
+]
+
+
+class ExifFlashReturn(ExifEnum):
+    """
+    Exif Flash Return (part of :class:`ExifFlash` Tag)
+    
+    .. versionchanged:: 0.3.0
+        More readable string representation
+    """
     NO_STROBE_RETURN_DETECTION_FUNCTION = 0
     RESERVED                            = 1
     STROBE_RETURN_LIGHT_DETECTED        = 2
     STROBE_RETURN_LIGHT_NOT_DETECTED    = 3
 
+    def __str__(self) -> str:
+        return _exif_flash_return_str_value[int(self)]
 
-class ExifFlashMode(IntEnum):
-    """Exif Flash Mode (part of :class:`ExifFlash` Tag)"""
+
+_exif_flash_mode_str_value = ['Unknown', 'On', 'Off', 'Auto']
+
+class ExifFlashMode(ExifEnum):
+    """
+    Exif Flash Mode (part of :class:`ExifFlash` Tag)
+    
+    .. versionchanged:: 0.3.0
+        More readable string representation
+    """
     UNKNOWN                         = 0
     COMPULSORY_FLASH_FIRING         = 1
     COMPULSORY_FLASH_SUPPRESSION    = 2
     AUTO_MODE                       = 3
+    
+    def __str__(self) -> str:
+        return _exif_flash_mode_str_value[int(self)]
 
 
 class ExifFlash:
     """
     Exif Flash Tag
     
-    Used by :attr:`ImageMetadata.flash<_sqla.ImageMetadata.flash>`
+    Used by :attr:`ImageMetadata.flash<_sqla.ImageMetadata.flash>`. To get the
+    numeric value of the flash tag, use ``int(flash_tag)``
     
     Args:
         value:  The :class:`int` value of flash tag, or a :class:`dict`
                 containing the flash information.
+    
+    .. versionchanged:: 0.3.0
+        *   For more consistency with the Exif standard, ``flash_function`` has been
+            replaced by ``no_flash_function`` (its logical negation). The numeric
+            representation has not changed and always conformed to the standard.
+        *   ``__repr__`` shows the fields' names
+        *   More readable ``__str__``
     """
     def __init__(
         self,
         value: Union[int, Mapping]
     ):
         if isinstance(value, int):
             self._value = value
@@ -185,25 +247,60 @@
             self._value = 0
             if 'flash_fired' in value and value['flash_fired']:
                 self._value |= 1
             if 'flash_return' in value and value['flash_return']:
                 self._value |= (value['flash_return'] << 1)
             if 'flash_mode' in value and value['flash_mode']:
                 self._value |= (value['flash_mode'] << 3)
-            if 'flash_function' in value and not value['flash_function']:
+            if 'no_flash_function' in value and value['no_flash_function']:
                 self._value |= 32
             if 'red_eye_reduction' in value and value['red_eye_reduction']:
                 self._value |= 64
         else:
             raise TypeError('Flash constructor Argument must be int or dict')
     
-    def __int__(self):
+    def __repr__(self) -> str:
+        desc = []
+        if self.flash_fired:
+            desc.append('FIRED')
+        if self.flash_mode:
+            desc.append(self.flash_mode.name)
+        if self.flash_return:
+            desc.append(self.flash_return.name)
+        if self.red_eye_reduction:
+            desc.append('RED_EYE_REDUCTION')
+        if self.no_flash_function:
+            desc.append('NO_FUNCTION')
+        return '<{}({})>'.format(
+            self.__class__.__name__,
+            ','.join(desc)
+        )
+    
+    def __str__(self) -> str:
+        desc = []
+        if self.flash_mode:
+            desc.append(str(self.flash_mode))
+        if self.flash_fired:
+            desc.append('Fired')
+        else:
+            desc.append('Did not fire')
+        if self.red_eye_reduction:
+            desc.append('Red-eye reduction')
+        if self.flash_return:
+            desc.append(str(self.flash_return))
+        if self.no_flash_function:
+            desc.append('No flash function')
+        return ', '.join(desc)
+    
+    def __int__(self) -> int:
         return self._value
     
-    def __eq__(self, other: Any):
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, ExifFlash):
+            return int(other) == self._value
         return other == self._value
     
     @property
     def flash_fired(self) -> bool:
         """Indicates if the flash fired."""
         return bool(self._value & 1)
     
@@ -214,17 +311,17 @@
     
     @property
     def flash_mode(self) -> ExifFlashMode:
         """Flash mode"""
         return ExifFlashMode((self._value >> 3) & 3)
     
     @property
-    def flash_function(self) -> bool:
+    def no_flash_function(self) -> bool:
         """Flash function supported?"""
-        return not bool((self._value >> 5) & 1)
+        return bool((self._value >> 5) & 1)
     
     @property
     def red_eye_reduction(self) -> bool:
         """Red eye reduction supported?"""
         return bool((self._value >> 6) & 1)
```

### Comparing `Digikam-DB-0.2.2/docs/Makefile` & `Digikam-DB-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/docs/_ext/_sqla.py` & `Digikam-DB-0.3.0/docs/_ext/_sqla.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/docs/_ext/digikam4.db` & `Digikam-DB-0.3.0/docs/_ext/digikam4.db`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/docs/api.rst` & `Digikam-DB-0.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/docs/api_albums.rst` & `Digikam-DB-0.3.0/docs/api_albums.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/docs/api_images.rst` & `Digikam-DB-0.3.0/docs/api_images.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/docs/conf.py` & `Digikam-DB-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/docs/intro.rst` & `Digikam-DB-0.3.0/docs/intro.rst`

 * *Files 10% similar despite different names*

```diff
@@ -75,24 +75,19 @@
 Limitations
 ------------
 
 * Adding or deleting albumroots, albums and images is not supported.
 * Digikam-DB will probably not run under Windows or MacOS.
 * Fractions of seconds on datetime fields are ignored (this is standard on
   MySQL, but not on SQLite).
-* The only tables implemented are:
+* Digikam-DB only implements the Core database of Digikam, not the Thumbs,
+  Faces, and Similarity databases.
+* There is no interface to the following tables of the Core DB:
   
-  * AlbumRoots
-  * Albums
-  * ImageComments
-  * ImageCopyright
-  * ImageInformation
-  * ImageHistory
-  * ImageMetadata
-  * ImagePositions
-  * Images
-  * ImageTags
-  * Settings
-  * TagProperties
-  * Tags
-  * VideoMetadata
+  * DownloadHistory
+  * ImageRelations
+  * ImageTagProperties
+  * Searches
+  
+
+
```

### Comparing `Digikam-DB-0.2.2/docs/tutorial.rst` & `Digikam-DB-0.3.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/pyproject.toml` & `Digikam-DB-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/__init__.py` & `Digikam-DB-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/base.py` & `Digikam-DB-0.3.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/digikamrc.mysql` & `Digikam-DB-0.3.0/tests/data/digikamrc.mysql`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/digikamrc.mysql-internal` & `Digikam-DB-0.3.0/tests/data/digikamrc.mysql-internal`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/digikamrc.sqlite` & `Digikam-DB-0.3.0/tests/data/digikamrc.sqlite`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/empty-15.sql.xz` & `Digikam-DB-0.3.0/tests/data/empty-15.sql.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/empty-15.tar.xz` & `Digikam-DB-0.3.0/tests/data/empty-15.tar.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/empty.sql.xz` & `Digikam-DB-0.3.0/tests/data/empty.sql.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/empty.tar.xz` & `Digikam-DB-0.3.0/tests/data/empty.tar.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/testdb.sql.xz` & `Digikam-DB-0.3.0/tests/data/testdb.sql.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data/testdb.tar.gz` & `Digikam-DB-0.3.0/tests/data/testdb.tar.gz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/data.py` & `Digikam-DB-0.3.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/digikamrc.py` & `Digikam-DB-0.3.0/tests/digikamrc.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/imagedata.py` & `Digikam-DB-0.3.0/tests/imagedata.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/mysql.py` & `Digikam-DB-0.3.0/tests/mysql.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/newdata.py` & `Digikam-DB-0.3.0/tests/newdata.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/sanity.py` & `Digikam-DB-0.3.0/tests/sanity.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.2/tests/sqlite.py` & `Digikam-DB-0.3.0/tests/sqlite.py`

 * *Files identical despite different names*

