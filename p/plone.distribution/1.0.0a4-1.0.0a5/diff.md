# Comparing `tmp/plone.distribution-1.0.0a4.tar.gz` & `tmp/plone.distribution-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.distribution-1.0.0a4.tar", last modified: Thu May 18 19:01:28 2023, max compression
+gzip compressed data, was "plone.distribution-1.0.0a5.tar", last modified: Thu May 18 21:06:20 2023, max compression
```

## Comparing `plone.distribution-1.0.0a4.tar` & `plone.distribution-1.0.0a5.tar`

### file list

```diff
@@ -1,117 +1,137 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.391337 plone.distribution-1.0.0a4/
--rw-r--r--   0 ericof     (501) staff       (20)      974 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)      477 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/.gitignore
--rw-r--r--   0 ericof     (501) staff       (20)     1275 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)       95 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/CONTRIBUTING.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/LICENSE
--rw-r--r--   0 ericof     (501) staff       (20)      177 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     5797 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)     9121 2023-05-18 19:01:28.391123 plone.distribution-1.0.0a4/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/constraints.txt
--rw-r--r--   0 ericof     (501) staff       (20)      172 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/instance.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      577 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/mx.ini
--rw-r--r--   0 ericof     (501) staff       (20)     1324 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)      393 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/requirements-docs.txt
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-05-18 19:01:28.391406 plone.distribution-1.0.0a4/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.375949 plone.distribution-1.0.0a4/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.379380 plone.distribution-1.0.0a4/src/plone/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.382055 plone.distribution-1.0.0a4/src/plone/distribution/
--rw-r--r--   0 ericof     (501) staff       (20)      127 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.382393 plone.distribution-1.0.0a4/src/plone/distribution/api/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/api/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/api/distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     4319 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/api/site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.383004 plone.distribution-1.0.0a4/src/plone/distribution/browser/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/admin.py
--rw-r--r--   0 ericof     (501) staff       (20)      970 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/image.py
--rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/overrides.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.383869 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/
--rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-logo.png
--rw-r--r--   0 ericof     (501) staff       (20)      712 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-overview.min.css
--rw-r--r--   0 ericof     (501) staff       (20)   521416 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-overview.min.js
--rw-r--r--   0 ericof     (501) staff       (20)      812 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone.svg
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.383993 plone.distribution-1.0.0a4/src/plone/distribution/browser/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     1306 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/browser/templates/plone-overview.pt
--rw-r--r--   0 ericof     (501) staff       (20)      446 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     3121 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/core.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.376598 plone.distribution-1.0.0a4/src/plone/distribution/distributions/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.384658 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.385325 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/
--rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/content.json
--rw-r--r--   0 ericof     (501) staff       (20)      336 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/defaultpages.json
--rw-r--r--   0 ericof     (501) staff       (20)      257 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/ordering.json
--rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)      613 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/portlets.json
--rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      148 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/schema.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.385962 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.386082 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/content/
--rw-r--r--   0 ericof     (501) staff       (20)    25845 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      175 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/schema.json
--rw-r--r--   0 ericof     (501) staff       (20)      491 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/distributions.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.387180 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      795 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4547 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/exportimport.py
--rw-r--r--   0 ericof     (501) staff       (20)      265 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/serializer.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.387412 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     1807 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/templates/export_all.pt
--rw-r--r--   0 ericof     (501) staff       (20)     1143 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/exportimport/templates/import_all.pt
--rw-r--r--   0 ericof     (501) staff       (20)     1161 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/handler.py
--rw-r--r--   0 ericof     (501) staff       (20)      698 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)      373 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/meta.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4173 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/registry.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.387628 plone.distribution-1.0.0a4/src/plone/distribution/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.388103 plone.distribution-1.0.0a4/src/plone/distribution/services/auth/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/auth/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      348 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/auth/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/auth/login.py
--rw-r--r--   0 ericof     (501) staff       (20)      334 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.388579 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/
--rw-r--r--   0 ericof     (501) staff       (20)       77 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/add.py
--rw-r--r--   0 ericof     (501) staff       (20)      895 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4340 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/services/sites/get.py
--rw-r--r--   0 ericof     (501) staff       (20)      813 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.388909 plone.distribution-1.0.0a4/src/plone/distribution/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/utils/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      914 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/utils/request.py
--rw-r--r--   0 ericof     (501) staff       (20)     4396 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/utils/schema.py
--rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/src/plone/distribution/zcml.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.380764 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     9121 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     3556 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)       40 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      208 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-05-18 19:01:28.000000 plone.distribution-1.0.0a4/src/plone.distribution.egg-info/top_level.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.389458 plone.distribution-1.0.0a4/tests/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.389751 plone.distribution-1.0.0a4/tests/api/
--rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/api/test_api_distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     1247 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/api/test_api_site.py
--rw-r--r--   0 ericof     (501) staff       (20)      363 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/conftest.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.390126 plone.distribution-1.0.0a4/tests/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/services/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      243 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/services/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/services/test_services_site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.390478 plone.distribution-1.0.0a4/tests/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 19:01:28.390828 plone.distribution-1.0.0a4/tests/utils/data/
--rw-r--r--   0 ericof     (501) staff       (20)      969 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/data/invalid.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/data/valid.json
--rw-r--r--   0 ericof     (501) staff       (20)     1167 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/test_utils_request.py
--rw-r--r--   0 ericof     (501) staff       (20)     2519 2023-05-18 19:01:27.000000 plone.distribution-1.0.0a4/tests/utils/test_utils_schema.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.858627 plone.distribution-1.0.0a5/
+-rw-r--r--   0 ericof     (501) staff       (20)      974 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      477 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)     1393 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       95 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/CONTRIBUTING.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/LICENSE
+-rw-r--r--   0 ericof     (501) staff       (20)      269 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     5797 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)     9239 2023-05-18 21:06:20.858460 plone.distribution-1.0.0a5/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/constraints.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.847728 plone.distribution-1.0.0a5/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     7078 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/Makefile
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.848173 plone.distribution-1.0.0a5/docs/_static/
+-rw-r--r--   0 ericof     (501) staff       (20)     5430 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/_static/favicon.ico
+-rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/_static/logo.svg
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/_static/print.css
+-rw-r--r--   0 ericof     (501) staff       (20)     7814 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/_static/styles.css
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.848517 plone.distribution-1.0.0a5/docs/api/
+-rw-r--r--   0 ericof     (501) staff       (20)      469 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/api/distribution.md
+-rw-r--r--   0 ericof     (501) staff       (20)      709 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/api/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)      439 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/api/site.md
+-rw-r--r--   0 ericof     (501) staff       (20)      308 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/changelog_template.jinja
+-rw-r--r--   0 ericof     (501) staff       (20)     2813 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/conf.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.848626 plone.distribution-1.0.0a5/docs/development/
+-rw-r--r--   0 ericof     (501) staff       (20)       26 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/development/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     1329 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/index.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.848956 plone.distribution-1.0.0a5/docs/usage/
+-rw-r--r--   0 ericof     (501) staff       (20)     2255 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/usage/code-examples.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2010 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/usage/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     4505 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/usage/package-structure.md
+-rw-r--r--   0 ericof     (501) staff       (20)      172 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/instance.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      577 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/mx.ini
+-rw-r--r--   0 ericof     (501) staff       (20)     1324 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)      393 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/requirements-docs.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-05-18 21:06:20.858665 plone.distribution-1.0.0a5/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.844132 plone.distribution-1.0.0a5/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.849065 plone.distribution-1.0.0a5/src/plone/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.851101 plone.distribution-1.0.0a5/src/plone/distribution/
+-rw-r--r--   0 ericof     (501) staff       (20)      127 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.851437 plone.distribution-1.0.0a5/src/plone/distribution/api/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/api/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/api/distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4319 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/api/site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.852005 plone.distribution-1.0.0a5/src/plone/distribution/browser/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/admin.py
+-rw-r--r--   0 ericof     (501) staff       (20)      970 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/image.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/overrides.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.852785 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/
+-rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-logo.png
+-rw-r--r--   0 ericof     (501) staff       (20)      712 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-overview.min.css
+-rw-r--r--   0 ericof     (501) staff       (20)   521416 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-overview.min.js
+-rw-r--r--   0 ericof     (501) staff       (20)      812 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone.svg
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.852909 plone.distribution-1.0.0a5/src/plone/distribution/browser/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     1306 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/templates/plone-overview.pt
+-rw-r--r--   0 ericof     (501) staff       (20)      446 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3121 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/core.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.844739 plone.distribution-1.0.0a5/src/plone/distribution/distributions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.853431 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.854212 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/
+-rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/content.json
+-rw-r--r--   0 ericof     (501) staff       (20)      336 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/defaultpages.json
+-rw-r--r--   0 ericof     (501) staff       (20)      257 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/ordering.json
+-rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)      613 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/portlets.json
+-rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      148 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/schema.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.854732 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.854856 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/content/
+-rw-r--r--   0 ericof     (501) staff       (20)    25845 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      175 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/schema.json
+-rw-r--r--   0 ericof     (501) staff       (20)      491 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.855433 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      795 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4540 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/exportimport.py
+-rw-r--r--   0 ericof     (501) staff       (20)      265 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/serializer.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.855659 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     1807 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/export_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1143 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/import_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1161 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/handler.py
+-rw-r--r--   0 ericof     (501) staff       (20)      698 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)      373 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/meta.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4173 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/registry.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.855876 plone.distribution-1.0.0a5/src/plone/distribution/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.856196 plone.distribution-1.0.0a5/src/plone/distribution/services/auth/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/auth/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      348 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/auth/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/auth/login.py
+-rw-r--r--   0 ericof     (501) staff       (20)      334 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.856643 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/
+-rw-r--r--   0 ericof     (501) staff       (20)       77 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/add.py
+-rw-r--r--   0 ericof     (501) staff       (20)      895 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4340 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/get.py
+-rw-r--r--   0 ericof     (501) staff       (20)      813 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.856958 plone.distribution-1.0.0a5/src/plone/distribution/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/utils/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      914 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/utils/request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4396 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/utils/schema.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/zcml.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.849987 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     9239 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     3887 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       40 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      208 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.857158 plone.distribution-1.0.0a5/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.857379 plone.distribution-1.0.0a5/tests/api/
+-rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/api/test_api_distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1247 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/api/test_api_site.py
+-rw-r--r--   0 ericof     (501) staff       (20)      363 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.857689 plone.distribution-1.0.0a5/tests/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/services/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      243 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/services/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/services/test_services_site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.858000 plone.distribution-1.0.0a5/tests/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.858220 plone.distribution-1.0.0a5/tests/utils/data/
+-rw-r--r--   0 ericof     (501) staff       (20)      969 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/data/invalid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/data/valid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1167 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/test_utils_request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2519 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/test_utils_schema.py
```

### Comparing `plone.distribution-1.0.0a4/.editorconfig` & `plone.distribution-1.0.0a5/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/CHANGES.md` & `plone.distribution-1.0.0a5/CHANGES.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a5 (2023-05-18)
+
+
+### Bug fixes:
+
+- Import did not import any steps except content and portal. [pbauer] #22
+
+
 ## 1.0.0a4 (2023-05-18)
 
 
 ### New features:
 
 - Increase test coverage.
   [ericof] #12
```

### Comparing `plone.distribution-1.0.0a4/LICENSE` & `plone.distribution-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/Makefile` & `plone.distribution-1.0.0a5/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/PKG-INFO` & `plone.distribution-1.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -272,14 +272,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a5 (2023-05-18)
+
+
+### Bug fixes:
+
+- Import did not import any steps except content and portal. [pbauer] #22
+
+
 ## 1.0.0a4 (2023-05-18)
 
 
 ### New features:
 
 - Increase test coverage.
   [ericof] #12
```

### Comparing `plone.distribution-1.0.0a4/README.md` & `plone.distribution-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/mx.ini` & `plone.distribution-1.0.0a5/mx.ini`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/pyproject.toml` & `plone.distribution-1.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/setup.py` & `plone.distribution-1.0.0a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.distribution",
-    version="1.0.0a4",
+    version="1.0.0a5",
     description="Plone distribution support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/api/distribution.py` & `plone.distribution-1.0.0a5/src/plone/distribution/api/distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/api/site.py` & `plone.distribution-1.0.0a5/src/plone/distribution/api/site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/admin.py` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/admin.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/configure.zcml` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/image.py` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/image.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/overrides.zcml` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/overrides.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-logo.png` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-logo.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-overview.min.css` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-overview.min.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone-overview.min.js` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-overview.min.js`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/static/plone.svg` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/browser/templates/plone-overview.pt` & `plone.distribution-1.0.0a5/src/plone/distribution/browser/templates/plone-overview.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/core.py` & `plone.distribution-1.0.0a5/src/plone/distribution/core.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/content.json` & `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/content.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/portal.json` & `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/content/portlets.json` & `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/portlets.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/image.png` & `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/distributions/classic/schema.json` & `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/content/portal.json` & `plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/content/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/image.png` & `plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/distributions/default/schema.json` & `plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/exportimport/configure.zcml` & `plone.distribution-1.0.0a5/src/plone/distribution/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/exportimport/exportimport.py` & `plone.distribution-1.0.0a5/src/plone/distribution/exportimport/exportimport.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             "defaultpages",
             "discussion",
             "portlets",
             "redirects",
         ]
         for name in other_imports:
             view = api.content.get_view(f"import_{name}", self.context, request)
-            importfile = path / f"export_{name}.json"
+            importfile = path / f"{name}.json"
             if importfile.exists():
                 results = view(jsonfile=importfile.read_text(), return_json=True)
                 logger.info(results)
             else:
                 logger.info(f"Skipping import of {name} because no file {importfile}")
 
         return request.response.redirect(self.context.absolute_url())
```

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/exportimport/serializer.py` & `plone.distribution-1.0.0a5/src/plone/distribution/exportimport/serializer.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/exportimport/templates/export_all.pt` & `plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/export_all.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/exportimport/templates/import_all.pt` & `plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/import_all.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/handler.py` & `plone.distribution-1.0.0a5/src/plone/distribution/handler.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/interfaces.py` & `plone.distribution-1.0.0a5/src/plone/distribution/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/registry.py` & `plone.distribution-1.0.0a5/src/plone/distribution/registry.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/services/auth/login.py` & `plone.distribution-1.0.0a5/src/plone/distribution/services/auth/login.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/services/sites/add.py` & `plone.distribution-1.0.0a5/src/plone/distribution/services/sites/add.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/services/sites/configure.zcml` & `plone.distribution-1.0.0a5/src/plone/distribution/services/sites/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/services/sites/get.py` & `plone.distribution-1.0.0a5/src/plone/distribution/services/sites/get.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/testing.py` & `plone.distribution-1.0.0a5/src/plone/distribution/testing.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/utils/request.py` & `plone.distribution-1.0.0a5/src/plone/distribution/utils/request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/utils/schema.py` & `plone.distribution-1.0.0a5/src/plone/distribution/utils/schema.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone/distribution/zcml.py` & `plone.distribution-1.0.0a5/src/plone/distribution/zcml.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/src/plone.distribution.egg-info/PKG-INFO` & `plone.distribution-1.0.0a5/src/plone.distribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -272,14 +272,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a5 (2023-05-18)
+
+
+### Bug fixes:
+
+- Import did not import any steps except content and portal. [pbauer] #22
+
+
 ## 1.0.0a4 (2023-05-18)
 
 
 ### New features:
 
 - Increase test coverage.
   [ericof] #12
```

### Comparing `plone.distribution-1.0.0a4/src/plone.distribution.egg-info/SOURCES.txt` & `plone.distribution-1.0.0a5/src/plone.distribution.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -9,14 +9,29 @@
 constraints.txt
 instance.yaml
 mx.ini
 pyproject.toml
 requirements-docs.txt
 requirements.txt
 setup.py
+docs/Makefile
+docs/changelog_template.jinja
+docs/conf.py
+docs/index.md
+docs/_static/favicon.ico
+docs/_static/logo.svg
+docs/_static/print.css
+docs/_static/styles.css
+docs/api/distribution.md
+docs/api/index.md
+docs/api/site.md
+docs/development/index.md
+docs/usage/code-examples.md
+docs/usage/index.md
+docs/usage/package-structure.md
 src/plone/__init__.py
 src/plone.distribution.egg-info/PKG-INFO
 src/plone.distribution.egg-info/SOURCES.txt
 src/plone.distribution.egg-info/dependency_links.txt
 src/plone.distribution.egg-info/entry_points.txt
 src/plone.distribution.egg-info/namespace_packages.txt
 src/plone.distribution.egg-info/not-zip-safe
```

### Comparing `plone.distribution-1.0.0a4/tests/api/test_api_distribution.py` & `plone.distribution-1.0.0a5/tests/api/test_api_distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/tests/api/test_api_site.py` & `plone.distribution-1.0.0a5/tests/api/test_api_site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/tests/services/test_services_site.py` & `plone.distribution-1.0.0a5/tests/services/test_services_site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/tests/utils/data/invalid.json` & `plone.distribution-1.0.0a5/tests/utils/data/invalid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/tests/utils/data/valid.json` & `plone.distribution-1.0.0a5/tests/utils/data/valid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/tests/utils/test_utils_request.py` & `plone.distribution-1.0.0a5/tests/utils/test_utils_request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a4/tests/utils/test_utils_schema.py` & `plone.distribution-1.0.0a5/tests/utils/test_utils_schema.py`

 * *Files identical despite different names*

