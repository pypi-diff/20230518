# Comparing `tmp/plone.distribution-1.0.0a3.tar.gz` & `tmp/plone.distribution-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.distribution-1.0.0a3.tar", last modified: Wed Feb  8 20:17:09 2023, max compression
+gzip compressed data, was "plone.distribution-1.0.0a4.tar", last modified: Thu May 18 19:01:28 2023, max compression
```

## Comparing `plone.distribution-1.0.0a3.tar` & `plone.distribution-1.0.0a4.tar`

### file list

```diff
@@ -1,84 +1,117 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.242109 plone.distribution-1.0.0a3/
--rw-r--r--   0 ericof     (501) staff       (20)      974 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)      444 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/.gitignore
--rw-r--r--   0 ericof     (501) staff       (20)     1021 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)       95 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/CONTRIBUTING.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/LICENSE
--rw-r--r--   0 ericof     (501) staff       (20)      177 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     3751 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)     8890 2023-02-08 20:17:09.241955 plone.distribution-1.0.0a3/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     6662 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/README.md
--rw-r--r--   0 ericof     (501) staff       (20)     1303 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-02-08 20:17:09.242144 plone.distribution-1.0.0a3/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2086 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.232357 plone.distribution-1.0.0a3/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.234965 plone.distribution-1.0.0a3/src/plone/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.237178 plone.distribution-1.0.0a3/src/plone/distribution/
--rw-r--r--   0 ericof     (501) staff       (20)      127 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.237520 plone.distribution-1.0.0a3/src/plone/distribution/api/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/api/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1345 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/api/distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     3696 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/api/site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.238106 plone.distribution-1.0.0a3/src/plone/distribution/browser/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/admin.py
--rw-r--r--   0 ericof     (501) staff       (20)      970 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/image.py
--rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/overrides.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.238875 plone.distribution-1.0.0a3/src/plone/distribution/browser/static/
--rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/static/plone-logo.png
--rw-r--r--   0 ericof     (501) staff       (20)      712 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/static/plone-overview.min.css
--rw-r--r--   0 ericof     (501) staff       (20)   521416 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/static/plone-overview.min.js
--rw-r--r--   0 ericof     (501) staff       (20)      812 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/static/plone.svg
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.239013 plone.distribution-1.0.0a3/src/plone/distribution/browser/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     1306 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/browser/templates/plone-overview.pt
--rw-r--r--   0 ericof     (501) staff       (20)      288 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     3121 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/core.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.232981 plone.distribution-1.0.0a3/src/plone/distribution/distributions/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.239529 plone.distribution-1.0.0a3/src/plone/distribution/distributions/classic/
--rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/distributions/classic/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      191 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/distributions/classic/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/distributions/classic/schema.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.240018 plone.distribution-1.0.0a3/src/plone/distribution/distributions/default/
--rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/distributions/default/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      210 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/distributions/default/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/distributions/default/schema.json
--rw-r--r--   0 ericof     (501) staff       (20)      491 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/distributions.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1004 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/handler.py
--rw-r--r--   0 ericof     (501) staff       (20)      698 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)      373 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/meta.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4173 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/registry.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.240233 plone.distribution-1.0.0a3/src/plone/distribution/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.240586 plone.distribution-1.0.0a3/src/plone/distribution/services/auth/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/auth/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      348 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/auth/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/auth/login.py
--rw-r--r--   0 ericof     (501) staff       (20)      334 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.241074 plone.distribution-1.0.0a3/src/plone/distribution/services/sites/
--rw-r--r--   0 ericof     (501) staff       (20)       77 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/sites/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1698 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/sites/add.py
--rw-r--r--   0 ericof     (501) staff       (20)      895 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/sites/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4367 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/services/sites/get.py
--rw-r--r--   0 ericof     (501) staff       (20)      503 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.241429 plone.distribution-1.0.0a3/src/plone/distribution/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/utils/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      914 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/utils/request.py
--rw-r--r--   0 ericof     (501) staff       (20)     4510 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/utils/schema.py
--rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/src/plone/distribution/zcml.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.235966 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     8890 2023-02-08 20:17:09.000000 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     2458 2023-02-08 20:17:09.000000 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-02-08 20:17:09.000000 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)       40 2023-02-08 20:17:09.000000 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-02-08 20:17:09.000000 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-02-08 20:17:09.000000 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      167 2023-02-08 20:17:09.000000 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-02-08 20:17:09.000000 plone.distribution-1.0.0a3/src/plone.distribution.egg-info/top_level.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.241656 plone.distribution-1.0.0a3/tests/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/tests/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-02-08 20:17:09.241779 plone.distribution-1.0.0a3/tests/api/
--rw-r--r--   0 ericof     (501) staff       (20)     1169 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/tests/api/test_api_distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)      215 2023-02-08 20:17:08.000000 plone.distribution-1.0.0a3/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.391337 plone.distribution-1.0.0a4/
+-rw-r--r--   0 ericof     (501) staff       (20)      974 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      477 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)     1275 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       95 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/CONTRIBUTING.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/LICENSE
+-rw-r--r--   0 ericof     (501) staff       (20)      177 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     5797 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)     9121 2023-05-18 19:01:28.391123 plone.distribution-1.0.0a4/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/constraints.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      172 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/instance.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      577 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/mx.ini
+-rw-r--r--   0 ericof     (501) staff       (20)     1324 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)      393 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/requirements-docs.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-05-18 19:01:28.391406 plone.distribution-1.0.0a4/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.375949 plone.distribution-1.0.0a4/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.379380 plone.distribution-1.0.0a4/src/plone/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.382055 plone.distribution-1.0.0a4/src/plone/distribution/
+-rw-r--r--   0 ericof     (501) staff       (20)      127 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.382393 plone.distribution-1.0.0a4/src/plone/distribution/api/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/api/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/api/distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4319 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/api/site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.383004 plone.distribution-1.0.0a4/src/plone/distribution/browser/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/admin.py
+-rw-r--r--   0 ericof     (501) staff       (20)      970 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/image.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/overrides.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.383869 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/
+-rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-logo.png
+-rw-r--r--   0 ericof     (501) staff       (20)      712 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-overview.min.css
+-rw-r--r--   0 ericof     (501) staff       (20)   521416 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-overview.min.js
+-rw-r--r--   0 ericof     (501) staff       (20)      812 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone.svg
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.383993 plone.distribution-1.0.0a4/src/plone/distribution/browser/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     1306 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/templates/plone-overview.pt
+-rw-r--r--   0 ericof     (501) staff       (20)      446 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3121 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/core.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.376598 plone.distribution-1.0.0a4/src/plone/distribution/distributions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.384658 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.385325 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/
+-rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/content.json
+-rw-r--r--   0 ericof     (501) staff       (20)      336 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/defaultpages.json
+-rw-r--r--   0 ericof     (501) staff       (20)      257 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/ordering.json
+-rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)      613 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/portlets.json
+-rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      148 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/schema.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.385962 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.386082 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/content/
+-rw-r--r--   0 ericof     (501) staff       (20)    25845 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      175 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/schema.json
+-rw-r--r--   0 ericof     (501) staff       (20)      491 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.387180 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      795 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4547 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/exportimport.py
+-rw-r--r--   0 ericof     (501) staff       (20)      265 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/serializer.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.387412 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     1807 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/templates/export_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1143 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/templates/import_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1161 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/handler.py
+-rw-r--r--   0 ericof     (501) staff       (20)      698 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)      373 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/meta.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4173 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/registry.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.387628 plone.distribution-1.0.0a4/src/plone/distribution/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.388103 plone.distribution-1.0.0a4/src/plone/distribution/services/auth/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/auth/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      348 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/auth/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/auth/login.py
+-rw-r--r--   0 ericof     (501) staff       (20)      334 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.388579 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/
+-rw-r--r--   0 ericof     (501) staff       (20)       77 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/add.py
+-rw-r--r--   0 ericof     (501) staff       (20)      895 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4340 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/get.py
+-rw-r--r--   0 ericof     (501) staff       (20)      813 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.388909 plone.distribution-1.0.0a4/src/plone/distribution/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/utils/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      914 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/utils/request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4396 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/utils/schema.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/zcml.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.380764 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     9121 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     3556 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       40 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      208 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.389458 plone.distribution-1.0.0a4/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.389751 plone.distribution-1.0.0a4/tests/api/
+-rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/api/test_api_distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1247 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/api/test_api_site.py
+-rw-r--r--   0 ericof     (501) staff       (20)      363 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.390126 plone.distribution-1.0.0a4/tests/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/services/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      243 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/services/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/services/test_services_site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.390478 plone.distribution-1.0.0a4/tests/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.390828 plone.distribution-1.0.0a4/tests/utils/data/
+-rw-r--r--   0 ericof     (501) staff       (20)      969 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/data/invalid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/data/valid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1167 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/test_utils_request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2519 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/test_utils_schema.py
```

### Comparing `plone.distribution-1.0.0a3/.editorconfig` & `plone.distribution-1.0.0a4/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/CHANGES.md` & `plone.distribution-1.0.0a4/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,28 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2023-05-18)
+
+
+### New features:
+
+- Increase test coverage.
+  [ericof] #12
+- Implement JSON import of content [pbauer] #13
+- Use mxdev.
+  [ericof] #18
+- Implement default content for default and classic distributions as JSON.
+  [ericof] #20
+
+
 ## 1.0.0a3 (2023-02-08)
 
 
 ### Bug fixes:
 
 - Fix Basic Authentication for Chrome [@ericof] #10
```

### Comparing `plone.distribution-1.0.0a3/LICENSE` & `plone.distribution-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/PKG-INFO` & `plone.distribution-1.0.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -237,19 +237,18 @@
 
 **WIP**: Folder containing json data exported by `collective.exportimport`
 
 ## Advanced Usage
 
 ### Hiding Distributions
 
-By default, `plone.distribution` ships with 3 ready-to-use distributions:
+By default, `plone.distribution` ships with two ready-to-use distributions:
 
 * **default**: Plone Site (Volto frontend)
 * **classic**: Plone Site (Classic UI)
-* **intranet**: Intranet
 
 If you want to limit your users option to select a distribution, it is possible to set the environment variable `ALLOWED_DISTRIBUTIONS` with fewer options:
 
 ```shell
 ALLOWED_DISTRIBUTIONS=default
 ```
 
@@ -273,14 +272,28 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2023-05-18)
+
+
+### New features:
+
+- Increase test coverage.
+  [ericof] #12
+- Implement JSON import of content [pbauer] #13
+- Use mxdev.
+  [ericof] #18
+- Implement default content for default and classic distributions as JSON.
+  [ericof] #20
+
+
 ## 1.0.0a3 (2023-02-08)
 
 
 ### Bug fixes:
 
 - Fix Basic Authentication for Chrome [@ericof] #10
```

### Comparing `plone.distribution-1.0.0a3/README.md` & `plone.distribution-1.0.0a4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -205,19 +205,18 @@
 
 **WIP**: Folder containing json data exported by `collective.exportimport`
 
 ## Advanced Usage
 
 ### Hiding Distributions
 
-By default, `plone.distribution` ships with 3 ready-to-use distributions:
+By default, `plone.distribution` ships with two ready-to-use distributions:
 
 * **default**: Plone Site (Volto frontend)
 * **classic**: Plone Site (Classic UI)
-* **intranet**: Intranet
 
 If you want to limit your users option to select a distribution, it is possible to set the environment variable `ALLOWED_DISTRIBUTIONS` with fewer options:
 
 ```shell
 ALLOWED_DISTRIBUTIONS=default
 ```
```

### Comparing `plone.distribution-1.0.0a3/pyproject.toml` & `plone.distribution-1.0.0a4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.pytest.ini_options]
-addopts = "--cov-report term --cov=plone.distribution"
+addopts = "--cov-report term-missing --cov=plone.distribution"
 testpaths = [
     "tests",
 ]
 
 [tool.towncrier]
 filename = "CHANGES.md"
 directory = "news/"
@@ -64,8 +64,8 @@
 
 [tool.flakeheaven.plugins]
 pycodestyle = ["+*"]
 pyflakes = ["+*"]
 "flake8-*" = ["+*"]
 
 [tool.plone-code-analysis]
-paths = "setup.py src/ tests/"
+paths = "setup.py src/ tests/ docs/conf.py"
```

### Comparing `plone.distribution-1.0.0a3/setup.py` & `plone.distribution-1.0.0a4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.distribution",
-    version="1.0.0a3",
+    version="1.0.0a4",
     description="Plone distribution support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -46,24 +46,25 @@
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         "Plone",
         "setuptools",
         "z3c.unconfigure",
+        "collective.exportimport>=1.9",
     ],
     extras_require={
         "test": [
             "zest.releaser[recommended]",
             "zestreleaser.towncrier",
+            "plone.volto",
             "plone.app.testing",
             "plone.restapi[test]",
             "pytest",
             "pytest-cov",
             "pytest-plone>=0.2.0",
         ]
     },
-    entry_points="""
-    [z3c.autoinclude.plugin]
-    target = plone
-    """,
+    entry_points={
+        "z3c.autoinclude.plugin": ["target = plone"],
+    },
 )
```

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/api/distribution.py` & `plone.distribution-1.0.0a4/src/plone/distribution/api/distribution.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,28 +15,49 @@
     allowed_distributions = os.environ.get("ALLOWED_DISTRIBUTIONS", "")
     if allowed_distributions:
         allowed_distributions = allowed_distributions.split(",")
     return allowed_distributions
 
 
 def get_registry() -> DistributionRegistry:
-    """Return the Distribution Registry."""
+    """Return the Distribution Registry.
+
+    :returns: Distribution Registry instance.
+
+    :Example: :ref:`api-distribution-get_registry-example`
+    """
     return _distribution_registry
 
 
 def get_distributions(filter: bool = True) -> List[Distribution]:
-    """Get available Plone distributions."""
+    """Get available Plone distributions.
+
+    :param filter: Return only registered Distributions that
+                   are also listed on **ALLOWED_DISTRIBUTIONS**
+                   environment variable.
+    :returns: List of registered distributions.
+
+    :Example: :ref:`api-distribution-get_distributions-example`
+    """
     registry = get_registry()
     all_distributions = registry.enumerate_distributions()
     allowed_distributions = _allow_list()
     if filter and allowed_distributions:
         return [d for d in all_distributions if d.name in allowed_distributions]
     return all_distributions
 
 
 def get(name: str) -> Distribution:
-    """Get a distribution."""
+    """Get a distribution.
+
+    :param name: Distribution name.
+    :raises:
+        :class:`ValueError`,
+    :returns: A Plone Distribution
+
+    :Example: :ref:`api-distribution-get-example`
+    """
     registry = get_registry()
     distribution = registry.lookup(name)
     if not distribution:
         raise ValueError(f"No distribution named {name}")
     return distribution
```

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/api/site.py` & `plone.distribution-1.0.0a4/src/plone/distribution/api/site.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,23 @@
     try:
         return answers[key]
     except KeyError:
         raise KeyError(f"A value for {key} is required.")
 
 
 def get_sites(context=None) -> List[PloneSite]:
-    """Get all Plone sites."""
+    """Get all Plone sites.
+
+    :param context: Base context to search for Plone Sites.
+    :raises:
+        :class:`ValueError`,
+    :returns: A list of Plone Sites
+
+    :Example: :ref:`api-site-get_sites-example`
+    """
     if not context:
         raise ValueError("Need to provide application root")
     result = []
     secman = getSecurityManager()
     candidates = (obj for obj in context.values() if not isinstance(obj, Broken))
     for obj in candidates:
         if obj.meta_type == "Folder":
@@ -46,15 +54,28 @@
 
 def create(
     context,
     distribution_name: str,
     answers: dict,
     profile_id: str = _DEFAULT_PROFILE,
 ) -> PloneSite:
-    """Create a new Plone site using one of the distributions."""
+    """Create a new Plone site using one of the distributions.
+
+    :param context: Context where the site will be created.
+    :param distribution_name: Name of distribution to be used.
+    :param answers: Payload for site creation.
+    :param profile_id: Base profile to be used.
+                       default: `Products.CMFPlone:plone`
+    :raises:
+        :class:`ValueError`,
+        :class:`KeyError`,
+    :returns: Created Plone Site
+
+    :Example: :ref:`api-site-create-example`
+    """
     distribution = dist_api.get(distribution_name)
     handler = distribution.handler if distribution.handler else default_handler
     post_handler = distribution.post_handler
     # Attributes used during site creation
     site_id = _required_str_value(answers, "site_id")
     title = _required_str_value(answers, "title")
     description = answers.get("description", "")
```

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/admin.py` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/admin.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/configure.zcml` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/image.py` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/image.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/overrides.zcml` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/overrides.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/static/plone-logo.png` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-logo.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/static/plone-overview.min.css` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-overview.min.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/static/plone-overview.min.js` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-overview.min.js`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/static/plone.svg` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/browser/templates/plone-overview.pt` & `plone.distribution-1.0.0a4/src/plone/distribution/browser/templates/plone-overview.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/core.py` & `plone.distribution-1.0.0a4/src/plone/distribution/core.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/distributions/classic/image.png` & `plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/distributions/classic/schema.json` & `plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/distributions/default/image.png` & `plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/distributions/default/schema.json` & `plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/interfaces.py` & `plone.distribution-1.0.0a4/src/plone/distribution/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/registry.py` & `plone.distribution-1.0.0a4/src/plone/distribution/registry.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/services/auth/login.py` & `plone.distribution-1.0.0a4/src/plone/distribution/services/auth/login.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/services/sites/add.py` & `plone.distribution-1.0.0a4/src/plone/distribution/services/sites/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Service to create a Plone Site."""
 from plone.distribution.api import site as site_api
 from plone.restapi.deserializer import json_body
 from plone.restapi.services import Service
 from zExceptions import BadRequest
+from zExceptions import NotFound
 from zope.interface import alsoProvides
 from zope.interface import implementer
 from zope.publisher.interfaces import IPublishTraverse
 
 import plone.protect.interfaces
 
 
@@ -34,17 +35,18 @@
         # Create site
         try:
             site = site_api.create(
                 self.context,
                 distribution_name=distribution_name,
                 answers=data,
             )
+        except ValueError:
+            raise NotFound(f"No distribution named {distribution_name}.")
         except KeyError:
             raise BadRequest("Error creating the site.")
-        else:
-            return {
-                "@id": site.absolute_url(),
-                "id": site.id,
-                "title": site.title,
-                "description": site.description,
-                "needs_upgrade": False,
-            }
+        site_info = {
+            "@id": site.absolute_url(),
+            "id": site.id,
+            "title": site.title,
+            "description": site.description,
+        }
+        return site_info
```

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/services/sites/configure.zcml` & `plone.distribution-1.0.0a4/src/plone/distribution/services/sites/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/services/sites/get.py` & `plone.distribution-1.0.0a4/src/plone/distribution/services/sites/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 
 DEFAULT_ID = "Plone"
 
 
 def _is_outdated(site) -> bool:
     """Check if site needs an upgrade."""
     mig = getattr(site, "portal_migration", None) or site.get("portal_migration", None)
-    if mig is not None:
-        return mig.needUpgrading()
-    return False
+    return mig.needUpgrading() if mig else False
 
 
 _no_content_marker = object()
 
 
 @implementer(IPublishTraverse)
 class SitesGet(Service):
```

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/utils/request.py` & `plone.distribution-1.0.0a4/src/plone/distribution/utils/request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/utils/schema.py` & `plone.distribution-1.0.0a4/src/plone/distribution/utils/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,12 @@
     uischema = enrich_uischema(raw_schema.get("uischema", {}), jsonschema)
     return {"schema": jsonschema, "uischema": uischema}
 
 
 def validate_jsonschema(schema: dict, strict: bool = False) -> bool:
     """Validate if jsonschema has required information."""
     required_properties = ["site_id", "title", "setup_content"]
-    recommended_properties = ["default_language", "portal_timezone"]
+    if strict:
+        required_properties.extend(["default_language", "portal_timezone"])
     properties = [key for key in schema.get("properties")]
     missing = [key for key in required_properties if key not in properties]
-    if strict:
-        missing = missing.extend(
-            [key for key in recommended_properties if key not in properties]
-        )
     return False if missing else True
```

### Comparing `plone.distribution-1.0.0a3/src/plone/distribution/zcml.py` & `plone.distribution-1.0.0a4/src/plone/distribution/zcml.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a3/src/plone.distribution.egg-info/PKG-INFO` & `plone.distribution-1.0.0a4/src/plone.distribution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -237,19 +237,18 @@
 
 **WIP**: Folder containing json data exported by `collective.exportimport`
 
 ## Advanced Usage
 
 ### Hiding Distributions
 
-By default, `plone.distribution` ships with 3 ready-to-use distributions:
+By default, `plone.distribution` ships with two ready-to-use distributions:
 
 * **default**: Plone Site (Volto frontend)
 * **classic**: Plone Site (Classic UI)
-* **intranet**: Intranet
 
 If you want to limit your users option to select a distribution, it is possible to set the environment variable `ALLOWED_DISTRIBUTIONS` with fewer options:
 
 ```shell
 ALLOWED_DISTRIBUTIONS=default
 ```
 
@@ -273,14 +272,28 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2023-05-18)
+
+
+### New features:
+
+- Increase test coverage.
+  [ericof] #12
+- Implement JSON import of content [pbauer] #13
+- Use mxdev.
+  [ericof] #18
+- Implement default content for default and classic distributions as JSON.
+  [ericof] #20
+
+
 ## 1.0.0a3 (2023-02-08)
 
 
 ### Bug fixes:
 
 - Fix Basic Authentication for Chrome [@ericof] #10
```

### Comparing `plone.distribution-1.0.0a3/src/plone.distribution.egg-info/SOURCES.txt` & `plone.distribution-1.0.0a4/src/plone.distribution.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 .gitignore
 CHANGES.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
+constraints.txt
+instance.yaml
+mx.ini
 pyproject.toml
+requirements-docs.txt
 requirements.txt
 setup.py
 src/plone/__init__.py
 src/plone.distribution.egg-info/PKG-INFO
 src/plone.distribution.egg-info/SOURCES.txt
 src/plone.distribution.egg-info/dependency_links.txt
 src/plone.distribution.egg-info/entry_points.txt
@@ -40,25 +44,47 @@
 src/plone/distribution/browser/static/plone-overview.min.css
 src/plone/distribution/browser/static/plone-overview.min.js
 src/plone/distribution/browser/static/plone.svg
 src/plone/distribution/browser/templates/plone-overview.pt
 src/plone/distribution/distributions/classic/image.png
 src/plone/distribution/distributions/classic/profiles.json
 src/plone/distribution/distributions/classic/schema.json
+src/plone/distribution/distributions/classic/content/content.json
+src/plone/distribution/distributions/classic/content/defaultpages.json
+src/plone/distribution/distributions/classic/content/ordering.json
+src/plone/distribution/distributions/classic/content/portal.json
+src/plone/distribution/distributions/classic/content/portlets.json
 src/plone/distribution/distributions/default/image.png
 src/plone/distribution/distributions/default/profiles.json
 src/plone/distribution/distributions/default/schema.json
+src/plone/distribution/distributions/default/content/portal.json
+src/plone/distribution/exportimport/__init__.py
+src/plone/distribution/exportimport/configure.zcml
+src/plone/distribution/exportimport/exportimport.py
+src/plone/distribution/exportimport/interfaces.py
+src/plone/distribution/exportimport/serializer.py
+src/plone/distribution/exportimport/templates/export_all.pt
+src/plone/distribution/exportimport/templates/import_all.pt
 src/plone/distribution/services/__init__.py
 src/plone/distribution/services/configure.zcml
 src/plone/distribution/services/auth/__init__.py
 src/plone/distribution/services/auth/configure.zcml
 src/plone/distribution/services/auth/login.py
 src/plone/distribution/services/sites/__init__.py
 src/plone/distribution/services/sites/add.py
 src/plone/distribution/services/sites/configure.zcml
 src/plone/distribution/services/sites/get.py
 src/plone/distribution/utils/__init__.py
 src/plone/distribution/utils/request.py
 src/plone/distribution/utils/schema.py
 tests/__init__.py
 tests/conftest.py
-tests/api/test_api_distribution.py
+tests/api/test_api_distribution.py
+tests/api/test_api_site.py
+tests/services/__init__.py
+tests/services/conftest.py
+tests/services/test_services_site.py
+tests/utils/__init__.py
+tests/utils/test_utils_request.py
+tests/utils/test_utils_schema.py
+tests/utils/data/invalid.json
+tests/utils/data/valid.json
```

