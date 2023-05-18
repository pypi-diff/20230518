# Comparing `tmp/pygeoapi-0.8.0.tar.gz` & `tmp/pygeoapi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygeoapi-0.8.0.tar", last modified: Fri Jun  5 15:57:15 2020, max compression
+gzip compressed data, was "dist/pygeoapi-0.9.0.tar", last modified: Thu Nov 19 15:36:47 2020, max compression
```

## Comparing `pygeoapi-0.8.0.tar` & `pygeoapi-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,75 @@
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1096 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/LICENSE.md
--rw-r--r--   0 tomkralidis   (501) staff       (20)      116 2019-09-22 21:48:22.000000 pygeoapi-0.8.0/MANIFEST.in
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1579 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/PKG-INFO
--rw-r--r--   0 tomkralidis   (501) staff       (20)      791 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/README.md
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     2147 2020-06-05 15:56:54.000000 pygeoapi-0.8.0/pygeoapi/__init__.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)    50974 2020-06-04 22:38:14.000000 pygeoapi-0.8.0/pygeoapi/api.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     8272 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/flask_app.py
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/formatter/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1319 2019-09-22 21:48:22.000000 pygeoapi-0.8.0/pygeoapi/formatter/__init__.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     2161 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/formatter/base.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     3303 2019-09-22 21:48:22.000000 pygeoapi-0.8.0/pygeoapi/formatter/csv_.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     7503 2020-06-05 00:23:23.000000 pygeoapi-0.8.0/pygeoapi/linked_data.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     2377 2019-09-22 21:48:22.000000 pygeoapi-0.8.0/pygeoapi/log.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)    20479 2020-06-05 01:27:57.000000 pygeoapi-0.8.0/pygeoapi/openapi.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     3561 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/plugin.py
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/process/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1353 2019-09-22 21:48:22.000000 pygeoapi-0.8.0/pygeoapi/process/__init__.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     2054 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/process/base.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     3084 2020-04-09 18:21:50.000000 pygeoapi-0.8.0/pygeoapi/process/hello_world.py
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/provider/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1355 2019-09-22 21:48:22.000000 pygeoapi-0.8.0/pygeoapi/provider/__init__.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     4102 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/provider/base.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     6172 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/provider/csv_.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)    13650 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/provider/elasticsearch_.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     9384 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/provider/filesystem.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     6915 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/provider/geojson.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     6384 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/provider/mongo.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)    27044 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/provider/ogr.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)    14888 2020-06-05 01:27:57.000000 pygeoapi-0.8.0/pygeoapi/provider/postgresql.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)    11707 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/provider/sqlite.py
--rw-r--r--   0 tomkralidis   (501) staff       (20)     9302 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/starlette_app.py
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/static/
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/static/css/
--rw-r--r--   0 tomkralidis   (501) staff       (20)      705 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/static/css/default.css
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/static/img/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1150 2019-09-22 21:48:22.000000 pygeoapi-0.8.0/pygeoapi/static/img/favicon.ico
--rw-r--r--   0 tomkralidis   (501) staff       (20)    21458 2019-10-14 21:50:24.000000 pygeoapi-0.8.0/pygeoapi/static/img/logo.png
--rw-r--r--   0 tomkralidis   (501) staff       (20)    21458 2019-10-14 21:50:24.000000 pygeoapi-0.8.0/pygeoapi/static/img/pygeoapi.png
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/templates/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     3687 2020-04-11 21:49:45.000000 pygeoapi-0.8.0/pygeoapi/templates/base.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     2421 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/collection.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1712 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/collections.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)      437 2020-04-06 17:30:36.000000 pygeoapi-0.8.0/pygeoapi/templates/conformance.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     3733 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/item.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     4571 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/items.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1741 2019-11-07 00:58:51.000000 pygeoapi-0.8.0/pygeoapi/templates/openapi.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1790 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/process.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1378 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/processes.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1375 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/queryables.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     5527 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/root.html
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi/templates/stac/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1156 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/stac/catalog.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     3424 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/stac/item.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1855 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/pygeoapi/templates/stac/root.html
--rw-r--r--   0 tomkralidis   (501) staff       (20)     7253 2020-06-05 01:28:59.000000 pygeoapi-0.8.0/pygeoapi/util.py
-drwxr-xr-x   0 tomkralidis   (501) staff       (20)        0 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/pygeoapi.egg-info/
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1579 2020-06-05 15:57:14.000000 pygeoapi-0.8.0/pygeoapi.egg-info/PKG-INFO
--rw-r--r--   0 tomkralidis   (501) staff       (20)     1483 2020-06-05 15:57:14.000000 pygeoapi-0.8.0/pygeoapi.egg-info/SOURCES.txt
--rw-r--r--   0 tomkralidis   (501) staff       (20)        1 2020-06-05 15:57:14.000000 pygeoapi-0.8.0/pygeoapi.egg-info/dependency_links.txt
--rw-r--r--   0 tomkralidis   (501) staff       (20)       43 2020-06-05 15:57:14.000000 pygeoapi-0.8.0/pygeoapi.egg-info/entry_points.txt
--rw-r--r--   0 tomkralidis   (501) staff       (20)       51 2020-06-05 15:57:14.000000 pygeoapi-0.8.0/pygeoapi.egg-info/requires.txt
--rw-r--r--   0 tomkralidis   (501) staff       (20)        9 2020-06-05 15:57:14.000000 pygeoapi-0.8.0/pygeoapi.egg-info/top_level.txt
--rw-r--r--   0 tomkralidis   (501) staff       (20)       51 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/requirements.txt
--rw-r--r--   0 tomkralidis   (501) staff       (20)       38 2020-06-05 15:57:15.000000 pygeoapi-0.8.0/setup.cfg
--rw-r--r--   0 tomkralidis   (501) staff       (20)     5078 2020-06-04 19:19:59.000000 pygeoapi-0.8.0/setup.py
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1584 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/PKG-INFO
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1096 2020-06-23 01:07:16.000000 pygeoapi-0.9.0/LICENSE.md
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/
+-rw-r--r--   0 tkralidi   (501) staff       (20)     2377 2019-09-22 21:48:22.000000 pygeoapi-0.9.0/pygeoapi/log.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    10088 2020-10-08 21:24:53.000000 pygeoapi-0.9.0/pygeoapi/util.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    36205 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/openapi.py
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/provider/
+-rw-r--r--   0 tkralidi   (501) staff       (20)     6921 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/provider/csv_.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     3850 2020-10-10 20:04:18.000000 pygeoapi-0.9.0/pygeoapi/provider/tile.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    15082 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/provider/postgresql.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     6466 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/provider/mongo.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    10023 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/provider/filesystem.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1355 2019-09-22 21:48:22.000000 pygeoapi-0.9.0/pygeoapi/provider/__init__.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    22141 2020-10-29 22:16:23.000000 pygeoapi-0.9.0/pygeoapi/provider/xarray_.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    11901 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/provider/sqlite.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     9856 2020-09-24 22:49:30.000000 pygeoapi-0.9.0/pygeoapi/provider/mvt.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    27612 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/provider/ogr.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    17305 2020-10-29 22:16:23.000000 pygeoapi-0.9.0/pygeoapi/provider/rasterio_.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     8095 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/provider/geojson.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    14379 2020-11-13 02:33:26.000000 pygeoapi-0.9.0/pygeoapi/provider/elasticsearch_.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     5451 2020-10-10 20:04:18.000000 pygeoapi-0.9.0/pygeoapi/provider/base.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     2179 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/__init__.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    85323 2020-11-18 14:16:44.000000 pygeoapi-0.9.0/pygeoapi/api.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     7503 2020-06-23 01:07:16.000000 pygeoapi-0.9.0/pygeoapi/linked_data.py
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/formatter/
+-rw-r--r--   0 tkralidi   (501) staff       (20)     3303 2019-09-22 21:48:22.000000 pygeoapi-0.9.0/pygeoapi/formatter/csv_.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1319 2019-09-22 21:48:22.000000 pygeoapi-0.9.0/pygeoapi/formatter/__init__.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     2161 2020-10-10 20:04:18.000000 pygeoapi-0.9.0/pygeoapi/formatter/base.py
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/static/
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/static/css/
+-rw-r--r--   0 tkralidi   (501) staff       (20)      705 2020-06-23 01:07:17.000000 pygeoapi-0.9.0/pygeoapi/static/css/default.css
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/static/img/
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1150 2019-09-22 21:48:22.000000 pygeoapi-0.9.0/pygeoapi/static/img/favicon.ico
+-rw-r--r--   0 tkralidi   (501) staff       (20)    21458 2019-10-14 21:50:24.000000 pygeoapi-0.9.0/pygeoapi/static/img/pygeoapi.png
+-rw-r--r--   0 tkralidi   (501) staff       (20)    21458 2019-10-14 21:50:24.000000 pygeoapi-0.9.0/pygeoapi/static/img/logo.png
+-rw-r--r--   0 tkralidi   (501) staff       (20)     3597 2020-09-24 22:49:30.000000 pygeoapi-0.9.0/pygeoapi/plugin.py
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/templates/
+-rw-r--r--   0 tkralidi   (501) staff       (20)      775 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/queryables.html
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/templates/stac/
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1280 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/stac/root.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1009 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/stac/catalog.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     3267 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/stac/item.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1402 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/domainset.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1741 2020-07-25 00:08:37.000000 pygeoapi-0.9.0/pygeoapi/templates/openapi.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     4444 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/tiles.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)      437 2020-04-06 17:30:36.000000 pygeoapi-0.9.0/pygeoapi/templates/conformance.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1458 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/process.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     3687 2020-04-11 21:49:45.000000 pygeoapi-0.9.0/pygeoapi/templates/base.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1826 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/collection.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)      946 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/tiles_metadata.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)      604 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/rangetype.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1184 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/processes.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     4906 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/landing_page.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     4571 2020-06-23 01:07:17.000000 pygeoapi-0.9.0/pygeoapi/templates/items.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1163 2020-11-19 15:35:29.000000 pygeoapi-0.9.0/pygeoapi/templates/collections.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)     3733 2020-06-29 18:04:53.000000 pygeoapi-0.9.0/pygeoapi/templates/item.html
+-rw-r--r--   0 tkralidi   (501) staff       (20)    12313 2020-10-08 21:24:59.000000 pygeoapi-0.9.0/pygeoapi/flask_app.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)    13795 2020-10-08 21:06:36.000000 pygeoapi-0.9.0/pygeoapi/starlette_app.py
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi/process/
+-rw-r--r--   0 tkralidi   (501) staff       (20)     3084 2020-04-09 18:21:50.000000 pygeoapi-0.9.0/pygeoapi/process/hello_world.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1353 2019-09-22 21:48:22.000000 pygeoapi-0.9.0/pygeoapi/process/__init__.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)     2054 2020-06-23 01:07:17.000000 pygeoapi-0.9.0/pygeoapi/process/base.py
+-rw-r--r--   0 tkralidi   (501) staff       (20)       67 2020-10-29 22:16:23.000000 pygeoapi-0.9.0/requirements.txt
+-rw-r--r--   0 tkralidi   (501) staff       (20)      116 2019-09-22 21:48:22.000000 pygeoapi-0.9.0/MANIFEST.in
+-rw-r--r--   0 tkralidi   (501) staff       (20)      796 2020-06-23 01:07:31.000000 pygeoapi-0.9.0/README.md
+-rw-r--r--   0 tkralidi   (501) staff       (20)     5078 2020-06-23 01:07:17.000000 pygeoapi-0.9.0/setup.py
+drwxr-xr-x   0 tkralidi   (501) staff       (20)        0 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/pygeoapi.egg-info/
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1584 2020-11-19 15:36:46.000000 pygeoapi-0.9.0/pygeoapi.egg-info/PKG-INFO
+-rw-r--r--   0 tkralidi   (501) staff       (20)     1739 2020-11-19 15:36:46.000000 pygeoapi-0.9.0/pygeoapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tkralidi   (501) staff       (20)       43 2020-11-19 15:36:46.000000 pygeoapi-0.9.0/pygeoapi.egg-info/entry_points.txt
+-rw-r--r--   0 tkralidi   (501) staff       (20)       67 2020-11-19 15:36:46.000000 pygeoapi-0.9.0/pygeoapi.egg-info/requires.txt
+-rw-r--r--   0 tkralidi   (501) staff       (20)        9 2020-11-19 15:36:46.000000 pygeoapi-0.9.0/pygeoapi.egg-info/top_level.txt
+-rw-r--r--   0 tkralidi   (501) staff       (20)        1 2020-11-19 15:36:46.000000 pygeoapi-0.9.0/pygeoapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tkralidi   (501) staff       (20)       38 2020-11-19 15:36:47.000000 pygeoapi-0.9.0/setup.cfg
```

### Comparing `pygeoapi-0.8.0/LICENSE.md` & `pygeoapi-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/PKG-INFO` & `pygeoapi-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pygeoapi
-Version: 0.8.0
+Version: 0.9.0
 Summary: pygeoapi provides an API to geospatial data
 Home-page: https://pygeoapi.io
 Author: Tom Kralidis
 Author-email: tomkralidis@gmail.com
 Maintainer: Tom Kralidis
 Maintainer-email: tomkralidis@gmail.com
 License: MIT
 Description: # pygeoapi
         
         [![Build Status](https://travis-ci.org/geopython/pygeoapi.png)](https://travis-ci.org/geopython/pygeoapi)
         <a href="https://json-ld.org"><img src="https://json-ld.org/images/json-ld-button-88.png" height="20"/></a>
         
-        [pygeoapi](https://pygeoapi.io) is a Python server implementation of the [OGC API](http://ogcapi.org) suite of standards. The project emerged as part of the next generation OGC API efforts in 2018 and provides the capability for organizations to deploy a RESTful OGC API endpoint using OpenAPI, GeoJSON, and HTML. pygeoapi is [open source](https://opensource.org/) and released under an [MIT license](https://github.com/geopython/pygeoapi/blob/master/LICENSE.md).
+        [pygeoapi](https://pygeoapi.io) is a Python server implementation of the [OGC API](https://ogcapi.ogc.org) suite of standards. The project emerged as part of the next generation OGC API efforts in 2018 and provides the capability for organizations to deploy a RESTful OGC API endpoint using OpenAPI, GeoJSON, and HTML. pygeoapi is [open source](https://opensource.org/) and released under an [MIT license](https://github.com/geopython/pygeoapi/blob/master/LICENSE.md).
         
         Please read the docs at [https://docs.pygeoapi.io](https://docs.pygeoapi.io) for more information.
 Keywords: geospatial data api
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: pygeoapi Version: 0.8.0 Summary: pygeoapi provides
+Metadata-Version: 2.1 Name: pygeoapi Version: 0.9.0 Summary: pygeoapi provides
 an API to geospatial data Home-page: https://pygeoapi.io Author: Tom Kralidis
 Author-email: tomkralidis@gmail.com Maintainer: Tom Kralidis Maintainer-email:
 tomkralidis@gmail.com License: MIT Description: # pygeoapi [![Build Status]
 (https://travis-ci.org/geopython/pygeoapi.png)](https://travis-ci.org/
 geopython/pygeoapi) [https://json-ld.org/images/json-ld-button-88.png]
 [pygeoapi](https://pygeoapi.io) is a Python server implementation of the [OGC
-API](http://ogcapi.org) suite of standards. The project emerged as part of the
-next generation OGC API efforts in 2018 and provides the capability for
+API](https://ogcapi.ogc.org) suite of standards. The project emerged as part of
+the next generation OGC API efforts in 2018 and provides the capability for
 organizations to deploy a RESTful OGC API endpoint using OpenAPI, GeoJSON, and
 HTML. pygeoapi is [open source](https://opensource.org/) and released under an
 [MIT license](https://github.com/geopython/pygeoapi/blob/master/LICENSE.md).
 Please read the docs at [https://docs.pygeoapi.io](https://docs.pygeoapi.io)
 for more information. Keywords: geospatial data api Platform: all Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
```

### Comparing `pygeoapi-0.8.0/README.md` & `pygeoapi-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # pygeoapi
 
 [![Build Status](https://travis-ci.org/geopython/pygeoapi.png)](https://travis-ci.org/geopython/pygeoapi)
 <a href="https://json-ld.org"><img src="https://json-ld.org/images/json-ld-button-88.png" height="20"/></a>
 
-[pygeoapi](https://pygeoapi.io) is a Python server implementation of the [OGC API](http://ogcapi.org) suite of standards. The project emerged as part of the next generation OGC API efforts in 2018 and provides the capability for organizations to deploy a RESTful OGC API endpoint using OpenAPI, GeoJSON, and HTML. pygeoapi is [open source](https://opensource.org/) and released under an [MIT license](https://github.com/geopython/pygeoapi/blob/master/LICENSE.md).
+[pygeoapi](https://pygeoapi.io) is a Python server implementation of the [OGC API](https://ogcapi.ogc.org) suite of standards. The project emerged as part of the next generation OGC API efforts in 2018 and provides the capability for organizations to deploy a RESTful OGC API endpoint using OpenAPI, GeoJSON, and HTML. pygeoapi is [open source](https://opensource.org/) and released under an [MIT license](https://github.com/geopython/pygeoapi/blob/master/LICENSE.md).
 
 Please read the docs at [https://docs.pygeoapi.io](https://docs.pygeoapi.io) for more information.
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # pygeoapi [![Build Status](https://travis-ci.org/geopython/pygeoapi.png)]
 (https://travis-ci.org/geopython/pygeoapi) [https://json-ld.org/images/json-ld-
 button-88.png] [pygeoapi](https://pygeoapi.io) is a Python server
-implementation of the [OGC API](http://ogcapi.org) suite of standards. The
+implementation of the [OGC API](https://ogcapi.ogc.org) suite of standards. The
 project emerged as part of the next generation OGC API efforts in 2018 and
 provides the capability for organizations to deploy a RESTful OGC API endpoint
 using OpenAPI, GeoJSON, and HTML. pygeoapi is [open source](https://
 opensource.org/) and released under an [MIT license](https://github.com/
 geopython/pygeoapi/blob/master/LICENSE.md). Please read the docs at [https://
 docs.pygeoapi.io](https://docs.pygeoapi.io) for more information.
```

### Comparing `pygeoapi-0.8.0/pygeoapi/__init__.py` & `pygeoapi-0.9.0/pygeoapi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,24 @@
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 #
 # =================================================================
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 import click
 from pygeoapi.openapi import generate_openapi_document
 
 
-cli = click.Group()
-cli.version = __version__
+@click.group()
+@click.version_option(version=__version__)
+def cli():
+    pass
 
 
 @cli.command()
 @click.option('--flask', 'server', flag_value="flask", default=True)
 @click.option('--starlette', 'server', flag_value="starlette")
 @click.pass_context
 def serve(ctx, server):
```

### Comparing `pygeoapi-0.8.0/pygeoapi/api.py` & `pygeoapi-0.9.0/pygeoapi/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # =================================================================
 #
 # Authors: Tom Kralidis <tomkralidis@gmail.com>
+#          Francesco Bartoli <xbartolone@gmail.com>
 #
 # Copyright (c) 2020 Tom Kralidis
+# Copyright (c) 2020 Francesco Bartoli
 #
 # Permission is hereby granted, free of charge, to any person
 # obtaining a copy of this software and associated documentation
 # files (the "Software"), to deal in the Software without
 # restriction, including without limitation the rights to use,
 # copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the
@@ -27,32 +29,41 @@
 #
 # =================================================================
 """ Root level code of pygeoapi, parsing content provided by webframework.
 Returns content from plugins and sets reponses
 """
 
 from datetime import datetime
+from functools import partial
 import json
 import logging
 import os
+import re
 import urllib.parse
 
 from dateutil.parser import parse as dateparse
 import pytz
 
 from pygeoapi import __version__
 from pygeoapi.linked_data import (geojson2geojsonld, jsonldify,
                                   jsonldify_collection)
 from pygeoapi.log import setup_logger
 from pygeoapi.plugin import load_plugin, PLUGINS
 from pygeoapi.provider.base import (
     ProviderGenericError, ProviderConnectionError, ProviderNotFoundError,
-    ProviderQueryError, ProviderItemNotFoundError)
-from pygeoapi.util import (dategetter, filter_dict_by_key_value, json_serial,
-                           render_j2_template, str2bool, TEMPLATES)
+    ProviderInvalidQueryError, ProviderNoDataError, ProviderQueryError,
+    ProviderItemNotFoundError, ProviderTypeError)
+
+from pygeoapi.provider.tile import (ProviderTileNotFoundError,
+                                    ProviderTileQueryError,
+                                    ProviderTilesetIdNotFoundError)
+from pygeoapi.util import (dategetter, filter_dict_by_key_value,
+                           get_provider_by_type, get_provider_default,
+                           get_typed_value, render_j2_template, str2bool,
+                           TEMPLATES, to_json)
 
 LOGGER = logging.getLogger(__name__)
 
 #: Return headers for requests (e.g:X-Powered-By)
 HEADERS = {
     'Content-Type': 'application/json',
     'X-Powered-By': 'pygeoapi {}'.format(__version__)
@@ -61,17 +72,24 @@
 #: Formats allowed for ?f= requests
 FORMATS = ['json', 'html', 'jsonld']
 
 CONFORMANCE = [
     'http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core',
     'http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/oas30',
     'http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/html',
-    'http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/geojson'
+    'http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/geojson',
+    'http://www.opengis.net/spec/ogcapi_coverages-1/1.0/conf/core',
+    'http://www.opengis.net/spec/ogcapi-coverages-1/1.0/conf/oas30',
+    'http://www.opengis.net/spec/ogcapi-coverages-1/1.0/conf/html',
+    'http://www.opengis.net/spec/ogcapi-tiles-1/1.0/req/core',
+    'http://www.opengis.net/spec/ogcapi-tiles-1/1.0/req/collections'
 ]
 
+OGC_RELTYPES_BASE = 'http://www.opengis.net/def/rel/ogc/1.0'
+
 
 def pre_process(func):
     """
         Decorator performing header copy and format\
         checking before sending arguments to methods
 
         :param func: decorated function
@@ -106,19 +124,24 @@
 
         self.config = config
         self.config['server']['url'] = self.config['server']['url'].rstrip('/')
 
         if 'templates' not in self.config['server']:
             self.config['server']['templates'] = TEMPLATES
 
+        if 'pretty_print' not in self.config['server']:
+            self.config['server']['pretty_print'] = False
+
+        self.pretty_print = self.config['server']['pretty_print']
+
         setup_logger(self.config['logging'])
 
     @pre_process
     @jsonldify
-    def root(self, headers_, format_):
+    def landing_page(self, headers_, format_):
         """
         Provide API
 
         :param headers_: copy of HEADERS object
         :param format_: format of requests, pre checked by
                         pre_process decorator
 
@@ -127,15 +150,15 @@
 
         if format_ is not None and format_ not in FORMATS:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         fcm = {
             'links': [],
             'title': self.config['metadata']['identification']['title'],
             'description':
                 self.config['metadata']['identification']['description']
         }
@@ -180,22 +203,34 @@
               'title': 'Collections',
               'href': '{}/collections'.format(self.config['server']['url'])
             }
         ]
 
         if format_ == 'html':  # render
             headers_['Content-Type'] = 'text/html'
-            content = render_j2_template(self.config, 'root.html', fcm)
+
+            fcm['processes'] = False
+            fcm['stac'] = False
+
+            if filter_dict_by_key_value(self.config['resources'],
+                                        'type', 'process'):
+                fcm['processes'] = True
+
+            if filter_dict_by_key_value(self.config['resources'],
+                                        'type', 'stac-collection'):
+                fcm['stac'] = True
+
+            content = render_j2_template(self.config, 'landing_page.html', fcm)
             return headers_, 200, content
 
         if format_ == 'jsonld':
             headers_['Content-Type'] = 'application/ld+json'
-            return headers_, 200, json.dumps(self.fcmld)
+            return headers_, 200, to_json(self.fcmld, self.pretty_print)
 
-        return headers_, 200, json.dumps(fcm)
+        return headers_, 200, to_json(fcm, self.pretty_print)
 
     @pre_process
     def openapi(self, headers_, format_, openapi):
         """
         Provide OpenAPI document
 
 
@@ -209,30 +244,30 @@
 
         if format_ is not None and format_ not in FORMATS:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         path = '/'.join([self.config['server']['url'].rstrip('/'), 'openapi'])
 
         if format_ == 'html':
             data = {
                 'openapi-document-path': path
             }
             headers_['Content-Type'] = 'text/html'
             content = render_j2_template(self.config, 'openapi.html', data)
             return headers_, 200, content
 
         headers_['Content-Type'] = \
             'application/vnd.oai.openapi+json;version=3.0'
 
-        return headers_, 200, json.dumps(openapi)
+        return headers_, 200, to_json(openapi, self.pretty_print)
 
     @pre_process
     def conformance(self, headers_, format_):
         """
         Provide conformance definition
 
         :param headers_: copy of HEADERS object
@@ -244,27 +279,27 @@
 
         if format_ is not None and format_ not in FORMATS:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         conformance = {
             'conformsTo': CONFORMANCE
         }
 
         if format_ == 'html':  # render
             headers_['Content-Type'] = 'text/html'
             content = render_j2_template(self.config, 'conformance.html',
                                          conformance)
             return headers_, 200, content
 
-        return headers_, 200, json.dumps(conformance)
+        return headers_, 200, to_json(conformance, self.pretty_print)
 
     @pre_process
     @jsonldify
     def describe_collections(self, headers_, format_, dataset=None):
         """
         Provide collection metadata
 
@@ -278,15 +313,15 @@
 
         if format_ is not None and format_ not in FORMATS:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         fcm = {
             'collections': [],
             'links': []
         }
 
         collections = filter_dict_by_key_value(self.config['resources'],
@@ -294,21 +329,28 @@
 
         if all([dataset is not None, dataset not in collections.keys()]):
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid collection'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         LOGGER.debug('Creating collections')
         for k, v in collections.items():
+            collection_data = get_provider_default(v['providers'])
+            collection_data_type = collection_data['type']
+
+            collection_data_format = None
+
+            if 'format' in collection_data:
+                collection_data_format = collection_data['format']
+
             collection = {'links': []}
             collection['id'] = k
-            collection['itemType'] = 'Feature'
             collection['title'] = v['title']
             collection['description'] = v['description']
             collection['keywords'] = v['keywords']
 
             bbox = v['extents']['spatial']['bbox']
             # The output should be an array of bbox, so if the user only
             # provided a single bbox, wrap it in a array.
@@ -344,50 +386,14 @@
                     lnk['hreflang'] = link['hreflang']
 
                 collection['links'].append(lnk)
 
             LOGGER.debug('Adding JSON and HTML link relations')
             collection['links'].append({
                 'type': 'application/json',
-                'rel': 'queryables',
-                'title': 'Queryables for this collection as JSON',
-                'href': '{}/collections/{}/queryables?f=json'.format(
-                    self.config['server']['url'], k)
-            })
-            collection['links'].append({
-                'type': 'text/html',
-                'rel': 'queryables',
-                'title': 'Queryables for this collection as HTML',
-                'href': '{}/collections/{}/queryables?f=html'.format(
-                    self.config['server']['url'], k)
-            })
-
-            collection['links'].append({
-                'type': 'application/geo+json',
-                'rel': 'items',
-                'title': 'items as GeoJSON',
-                'href': '{}/collections/{}/items?f=json'.format(
-                    self.config['server']['url'], k)
-            })
-            collection['links'].append({
-                'type': 'application/ld+json',
-                'rel': 'items',
-                'title': 'items as RDF (GeoJSON-LD)',
-                'href': '{}/collections/{}/items?f=jsonld'.format(
-                    self.config['server']['url'], k)
-            })
-            collection['links'].append({
-                'type': 'text/html',
-                'rel': 'items',
-                'title': 'Items as HTML',
-                'href': '{}/collections/{}/items?f=html'.format(
-                    self.config['server']['url'], k)
-            })
-            collection['links'].append({
-                'type': 'application/json',
                 'rel': 'self' if not format_
                 or format_ == 'json' else 'alternate',
                 'title': 'This document as JSON',
                 'href': '{}/collections/{}?f=json'.format(
                     self.config['server']['url'], k)
             })
             collection['links'].append({
@@ -401,14 +407,154 @@
                 'type': 'text/html',
                 'rel': 'self' if format_ == 'html' else 'alternate',
                 'title': 'This document as HTML',
                 'href': '{}/collections/{}?f=html'.format(
                     self.config['server']['url'], k)
             })
 
+            if collection_data_type == 'feature':
+                collection['itemType'] = collection_data_type.capitalize()
+                LOGGER.debug('Adding feature based links')
+                collection['links'].append({
+                    'type': 'application/json',
+                    'rel': 'queryables',
+                    'title': 'Queryables for this collection as JSON',
+                    'href': '{}/collections/{}/queryables?f=json'.format(
+                        self.config['server']['url'], k)
+                })
+                collection['links'].append({
+                    'type': 'text/html',
+                    'rel': 'queryables',
+                    'title': 'Queryables for this collection as HTML',
+                    'href': '{}/collections/{}/queryables?f=html'.format(
+                        self.config['server']['url'], k)
+                })
+                collection['links'].append({
+                    'type': 'application/geo+json',
+                    'rel': 'items',
+                    'title': 'items as GeoJSON',
+                    'href': '{}/collections/{}/items?f=json'.format(
+                        self.config['server']['url'], k)
+                })
+                collection['links'].append({
+                    'type': 'application/ld+json',
+                    'rel': 'items',
+                    'title': 'items as RDF (GeoJSON-LD)',
+                    'href': '{}/collections/{}/items?f=jsonld'.format(
+                        self.config['server']['url'], k)
+                })
+                collection['links'].append({
+                    'type': 'text/html',
+                    'rel': 'items',
+                    'title': 'Items as HTML',
+                    'href': '{}/collections/{}/items?f=html'.format(
+                        self.config['server']['url'], k)
+                })
+
+            elif collection_data_type == 'coverage':
+                LOGGER.debug('Adding coverage based links')
+                collection['links'].append({
+                    'type': 'application/json',
+                    'rel': 'collection',
+                    'title': 'Detailed Coverage metadata in JSON',
+                    'href': '{}/collections/{}?f=json'.format(
+                        self.config['server']['url'], k)
+                })
+                collection['links'].append({
+                    'type': 'text/html',
+                    'rel': 'collection',
+                    'title': 'Detailed Coverage metadata in HTML',
+                    'href': '{}/collections/{}?f=html'.format(
+                        self.config['server']['url'], k)
+                })
+                coverage_url = '{}/collections/{}/coverage'.format(
+                        self.config['server']['url'], k)
+
+                collection['links'].append({
+                    'type': 'application/json',
+                    'rel': '{}/coverage-domainset'.format(OGC_RELTYPES_BASE),
+                    'title': 'Coverage domain set of collection in JSON',
+                    'href': '{}/domainset?f=json'.format(coverage_url)
+                })
+                collection['links'].append({
+                    'type': 'text/html',
+                    'rel': '{}/coverage-domainset'.format(OGC_RELTYPES_BASE),
+                    'title': 'Coverage domain set of collection in HTML',
+                    'href': '{}/domainset?f=html'.format(coverage_url)
+                })
+                collection['links'].append({
+                    'type': 'application/json',
+                    'rel': '{}/coverage-rangetype'.format(OGC_RELTYPES_BASE),
+                    'title': 'Coverage range type of collection in JSON',
+                    'href': '{}/rangetype?f=json'.format(coverage_url)
+                })
+                collection['links'].append({
+                    'type': 'text/html',
+                    'rel': '{}/coverage-rangetype'.format(OGC_RELTYPES_BASE),
+                    'title': 'Coverage range type of collection in HTML',
+                    'href': '{}/rangetype?f=html'.format(coverage_url)
+                })
+                collection['links'].append({
+                    'type': 'application/prs.coverage+json',
+                    'rel': '{}/coverage'.format(OGC_RELTYPES_BASE),
+                    'title': 'Coverage data',
+                    'href': '{}/collections/{}/coverage?f=json'.format(
+                        self.config['server']['url'], k)
+                })
+                if collection_data_format is not None:
+                    collection['links'].append({
+                        'type': collection_data_format['mimetype'],
+                        'rel': '{}/coverage'.format(OGC_RELTYPES_BASE),
+                        'title': 'Coverage data as {}'.format(
+                            collection_data_format['name']),
+                        'href': '{}/collections/{}/coverage?f={}'.format(
+                            self.config['server']['url'], k,
+                            collection_data_format['name'])
+                    })
+                if dataset is not None:
+                    LOGGER.debug('Creating extended coverage metadata')
+                    try:
+                        p = load_plugin('provider', get_provider_by_type(
+                            self.config['resources'][dataset]['providers'],
+                            'coverage'))
+                    except ProviderConnectionError:
+                        exception = {
+                           'code': 'NoApplicableCode',
+                           'description': 'connection error (check logs)'
+                        }
+                        LOGGER.error(exception)
+                        return headers_, 500, to_json(exception,
+                                                      self.pretty_print)
+
+                    collection['crs'] = [p.crs]
+                    collection['domainset'] = p.get_coverage_domainset()
+                    collection['rangetype'] = p.get_coverage_rangetype()
+
+            try:
+                tile = get_provider_by_type(v['providers'], 'tile')
+            except ProviderTypeError:
+                tile = None
+
+            if tile:
+                LOGGER.debug('Adding tile links')
+                collection['links'].append({
+                    'type': 'application/json',
+                    'rel': 'tiles',
+                    'title': 'Tiles as JSON',
+                    'href': '{}/collections/{}/tiles?f=json'.format(
+                        self.config['server']['url'], k)
+                })
+                collection['links'].append({
+                    'type': 'text/html',
+                    'rel': 'tiles',
+                    'title': 'Tiles as HTML',
+                    'href': '{}/collections/{}/tiles?f=html'.format(
+                        self.config['server']['url'], k)
+                })
+
             if dataset is not None and k == dataset:
                 fcm = collection
                 break
 
             fcm['collections'].append(collection)
 
         if dataset is None:
@@ -456,17 +602,17 @@
                     map(
                         lambda collection: jsonldify_collection(
                             self, collection
                         ), fcm.get('collections', [])
                     )
                 )
             headers_['Content-Type'] = 'application/ld+json'
-            return headers_, 200, json.dumps(jsonld)
+            return headers_, 200, to_json(jsonld, self.pretty_print)
 
-        return headers_, 200, json.dumps(fcm, default=json_serial)
+        return headers_, 200, to_json(fcm, self.pretty_print)
 
     @pre_process
     @jsonldify
     def get_collection_queryables(self, headers_, format_, dataset=None):
         """
         Provide collection queryables
 
@@ -480,45 +626,45 @@
 
         if format_ is not None and format_ not in FORMATS:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         if any([dataset is None,
                 dataset not in self.config['resources'].keys()]):
 
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid collection'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         LOGGER.debug('Creating collection queryables')
         LOGGER.debug('Loading provider')
         try:
-            p = load_plugin('provider',
-                            self.config['resources'][dataset]['provider'])
+            p = load_plugin('provider', get_provider_by_type(
+                self.config['resources'][dataset]['providers'], 'feature'))
         except ProviderConnectionError:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'connection error (check logs)'
             }
             LOGGER.error(exception)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
         except ProviderQueryError:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'query error (check logs)'
             }
             LOGGER.error(exception)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
 
         queryables = {
             'queryables': []
         }
 
         for k, v in p.fields.items():
             show_field = False
@@ -538,15 +684,15 @@
             queryables['title'] = self.config['resources'][dataset]['title']
             headers_['Content-Type'] = 'text/html'
             content = render_j2_template(self.config, 'queryables.html',
                                          queryables)
 
             return headers_, 200, content
 
-        return headers_, 200, json.dumps(queryables, default=json_serial)
+        return headers_, 200, to_json(queryables, self.pretty_print)
 
     def get_collection_items(self, headers, args, dataset, pathinfo=None):
         """
         Queries collection
 
         :param headers: dict of HTTP headers
         :param args: dict of HTTP request parameters
@@ -556,203 +702,156 @@
         :returns: tuple of headers, status code, content
         """
 
         headers_ = HEADERS.copy()
 
         properties = []
         reserved_fieldnames = ['bbox', 'f', 'limit', 'startindex',
-                               'resulttype', 'datetime', 'sortby']
+                               'resulttype', 'datetime', 'sortby',
+                               'properties', 'skipGeometry']
         formats = FORMATS
         formats.extend(f.lower() for f in PLUGINS['formatter'].keys())
 
         collections = filter_dict_by_key_value(self.config['resources'],
                                                'type', 'collection')
 
         if dataset not in collections.keys():
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid collection'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception, default=json_serial)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         format_ = check_format(args, headers)
 
         if format_ is not None and format_ not in formats:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         LOGGER.debug('Processing query parameters')
 
         LOGGER.debug('Processing startindex parameter')
         try:
             startindex = int(args.get('startindex'))
             if startindex < 0:
                 exception = {
                     'code': 'InvalidParameterValue',
                     'description': 'startindex value should be positive ' +
                                    'or zero'
                 }
                 LOGGER.error(exception)
-                return headers_, 400, json.dumps(exception)
+                return headers_, 400, to_json(exception, self.pretty_print)
         except (TypeError) as err:
             LOGGER.warning(err)
             startindex = 0
         except ValueError as err:
             LOGGER.warning(err)
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'startindex value should be an integer'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         LOGGER.debug('Processing limit parameter')
         try:
             limit = int(args.get('limit'))
             # TODO: We should do more validation, against the min and max
             # allowed by the server configuration
             if limit <= 0:
                 exception = {
                     'code': 'InvalidParameterValue',
                     'description': 'limit value should be strictly positive'
                 }
                 LOGGER.error(exception)
-                return headers_, 400, json.dumps(exception)
+                return headers_, 400, to_json(exception, self.pretty_print)
         except TypeError as err:
             LOGGER.warning(err)
             limit = int(self.config['server']['limit'])
         except ValueError as err:
             LOGGER.warning(err)
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'limit value should be an integer'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         resulttype = args.get('resulttype') or 'results'
 
         LOGGER.debug('Processing bbox parameter')
-        try:
-            bbox = args.get('bbox').split(',')
-            if len(bbox) != 4:
+
+        bbox = args.get('bbox')
+
+        if bbox is None:
+            bbox = []
+        else:
+            try:
+                bbox = validate_bbox(bbox)
+            except ValueError as err:
                 exception = {
                     'code': 'InvalidParameterValue',
-                    'description': 'bbox values should be minx,miny,maxx,maxy'
+                    'description': str(err)
                 }
                 LOGGER.error(exception)
-                return headers_, 400, json.dumps(exception)
-        except AttributeError:
-            bbox = []
-        try:
-            bbox = [float(c) for c in bbox]
-        except ValueError:
-            exception = {
-                'code': 'InvalidParameterValue',
-                'description': 'bbox values must be numbers'
-            }
-            LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+                return headers_, 400, to_json(exception, self.pretty_print)
 
         LOGGER.debug('Processing datetime parameter')
-        # TODO: pass datetime to query as a `datetime` object
-        # we would need to ensure partial dates work accordingly
-        # as well as setting '..' values to `None` so that underlying
-        # providers can just assume a `datetime.datetime` object
-        #
-        # NOTE: needs testing when passing partials from API to backend
         datetime_ = args.get('datetime')
-        datetime_invalid = False
-
-        if (datetime_ is not None and
-                'temporal' in collections[dataset]['extents']):
-            te = collections[dataset]['extents']['temporal']
-
-            if te['begin'] is not None and te['begin'].tzinfo is None:
-                te['begin'] = te['begin'].replace(tzinfo=pytz.UTC)
-            if te['end'] is not None and te['end'].tzinfo is None:
-                te['end'] = te['end'].replace(tzinfo=pytz.UTC)
-
-            if '/' in datetime_:  # envelope
-                LOGGER.debug('detected time range')
-                LOGGER.debug('Validating time windows')
-                datetime_begin, datetime_end = datetime_.split('/')
-                if datetime_begin != '..':
-                    datetime_begin = dateparse(datetime_begin)
-                    if datetime_begin.tzinfo is None:
-                        datetime_begin = datetime_begin.replace(
-                            tzinfo=pytz.UTC)
-
-                if datetime_end != '..':
-                    datetime_end = dateparse(datetime_end)
-                    if datetime_end.tzinfo is None:
-                        datetime_end = datetime_end.replace(tzinfo=pytz.UTC)
-
-                if te['begin'] is not None and datetime_begin != '..':
-                    if datetime_begin < te['begin']:
-                        datetime_invalid = True
-
-                if te['end'] is not None and datetime_end != '..':
-                    if datetime_end > te['end']:
-                        datetime_invalid = True
-
-            else:  # time instant
-                datetime__ = dateparse(datetime_)
-                if datetime__ != '..':
-                    if datetime__.tzinfo is None:
-                        datetime__ = datetime__.replace(tzinfo=pytz.UTC)
-                LOGGER.debug('detected time instant')
-                if te['begin'] is not None and datetime__ != '..':
-                    if datetime__ < te['begin']:
-                        datetime_invalid = True
-                if te['end'] is not None and datetime__ != '..':
-                    if datetime__ > te['end']:
-                        datetime_invalid = True
-
-        if datetime_invalid:
+        try:
+            datetime_ = validate_datetime(collections[dataset]['extents'],
+                                          datetime_)
+        except ValueError as err:
             exception = {
                 'code': 'InvalidParameterValue',
-                'description': 'datetime parameter out of range'
+                'description': str(err)
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         LOGGER.debug('Loading provider')
         try:
-            p = load_plugin('provider',
-                            collections[dataset]['provider'])
+            p = load_plugin('provider', get_provider_by_type(
+                collections[dataset]['providers'], 'feature'))
+        except ProviderTypeError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'invalid provider type'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
         except ProviderConnectionError:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'connection error (check logs)'
             }
             LOGGER.error(exception)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
         except ProviderQueryError:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'query error (check logs)'
             }
             LOGGER.error(exception)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
 
         LOGGER.debug('processing property parameters')
         for k, v in args.items():
             if k not in reserved_fieldnames and k not in p.fields.keys():
                 exception = {
                     'code': 'InvalidParameterValue',
                     'description': 'unknown query parameter'
                 }
                 LOGGER.error(exception)
-                return headers_, 400, json.dumps(exception)
+                return headers_, 400, to_json(exception, self.pretty_print)
             elif k not in reserved_fieldnames and k in p.fields.keys():
                 LOGGER.debug('Add property filter {}={}'.format(k, v))
                 properties.append((k, v))
 
         LOGGER.debug('processing sort parameter')
         val = args.get('sortby')
 
@@ -764,61 +863,93 @@
                     prop, order = s.split(':')
                     if order not in ['A', 'D']:
                         exception = {
                             'code': 'InvalidParameterValue',
                             'description': 'sort order should be A or D'
                         }
                         LOGGER.error(exception)
-                        return headers_, 400, json.dumps(exception)
+                        return headers_, 400, to_json(exception,
+                                                      self.pretty_print)
                     sortby.append({'property': prop, 'order': order})
                 else:
                     sortby.append({'property': s, 'order': 'A'})
             for s in sortby:
                 if s['property'] not in p.fields.keys():
                     exception = {
                         'code': 'InvalidParameterValue',
                         'description': 'bad sort property'
                     }
                     LOGGER.error(exception)
-                    return headers_, 400, json.dumps(exception)
+                    return headers_, 400, to_json(exception, self.pretty_print)
         else:
             sortby = []
 
+        LOGGER.debug('processing properties parameter')
+        val = args.get('properties')
+
+        if val is not None:
+            select_properties = val.split(',')
+            properties_to_check = set(p.properties) | set(p.fields.keys())
+
+            if (len(list(set(select_properties) -
+                         set(properties_to_check))) > 0):
+                exception = {
+                    'code': 'InvalidParameterValue',
+                    'description': 'unknown properties specified'
+                }
+                LOGGER.error(exception)
+                return headers_, 400, to_json(exception, self.pretty_print)
+        else:
+            select_properties = []
+
+        LOGGER.debug('processing skipGeometry parameter')
+        val = args.get('skipGeometry')
+        if val is not None:
+            skip_geometry = str2bool(val)
+        else:
+            skip_geometry = False
+
         LOGGER.debug('Querying provider')
         LOGGER.debug('startindex: {}'.format(startindex))
         LOGGER.debug('limit: {}'.format(limit))
         LOGGER.debug('resulttype: {}'.format(resulttype))
         LOGGER.debug('sortby: {}'.format(sortby))
+        LOGGER.debug('bbox: {}'.format(bbox))
+        LOGGER.debug('datetime: {}'.format(datetime_))
+        LOGGER.debug('properties: {}'.format(select_properties))
+        LOGGER.debug('skipGeometry: {}'.format(skip_geometry))
 
         try:
             content = p.query(startindex=startindex, limit=limit,
                               resulttype=resulttype, bbox=bbox,
-                              datetime=datetime_, properties=properties,
-                              sortby=sortby)
+                              datetime_=datetime_, properties=properties,
+                              sortby=sortby,
+                              select_properties=select_properties,
+                              skip_geometry=skip_geometry)
         except ProviderConnectionError as err:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'connection error (check logs)'
             }
             LOGGER.error(err)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
         except ProviderQueryError as err:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'query error (check logs)'
             }
             LOGGER.error(err)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
         except ProviderGenericError as err:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'generic error (check logs)'
             }
             LOGGER.error(err)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
 
         serialized_query_params = ''
         for k, v in args.items():
             if k not in ('f', 'startindex'):
                 serialized_query_params += '&'
                 serialized_query_params += urllib.parse.quote(k, safe='')
                 serialized_query_params += '='
@@ -905,16 +1036,17 @@
             return headers_, 200, content
         elif format_ == 'csv':  # render
             formatter = load_plugin('formatter', {'name': 'CSV', 'geom': True})
 
             content = formatter.write(
                 data=content,
                 options={
-                    'provider_def':
-                        collections[dataset]['provider']
+                    'provider_def': get_provider_by_type(
+                                        collections[dataset]['providers'],
+                                        'feature')
                 }
             )
 
             headers_['Content-Type'] = '{}; charset={}'.format(
                 formatter.mimetype, self.config['server']['encoding'])
 
             cd = 'attachment; filename="{}.csv"'.format(dataset)
@@ -922,15 +1054,15 @@
 
             return headers_, 200, content
         elif format_ == 'jsonld':
             headers_['Content-Type'] = 'application/ld+json'
             content = geojson2geojsonld(self.config, content, dataset)
             return headers_, 200, content
 
-        return headers_, 200, json.dumps(content, default=json_serial)
+        return headers_, 200, to_json(content, self.pretty_print)
 
     @pre_process
     def get_collection_item(self, headers_, format_, dataset, identifier):
         """
         Get a single collection item
 
         :param headers_: copy of HEADERS object
@@ -944,71 +1076,79 @@
 
         if format_ is not None and format_ not in FORMATS:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         LOGGER.debug('Processing query parameters')
 
         collections = filter_dict_by_key_value(self.config['resources'],
                                                'type', 'collection')
 
         if dataset not in collections.keys():
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid collection'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         LOGGER.debug('Loading provider')
-        p = load_plugin('provider', collections[dataset]['provider'])
-
+        try:
+            p = load_plugin('provider', get_provider_by_type(
+                collections[dataset]['providers'], 'feature'))
+        except ProviderTypeError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'invalid provider type'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
         try:
             LOGGER.debug('Fetching id {}'.format(identifier))
             content = p.get(identifier)
         except ProviderConnectionError as err:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'connection error (check logs)'
             }
             LOGGER.error(err)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
         except ProviderItemNotFoundError:
             exception = {
                 'code': 'NotFound',
                 'description': 'identifier not found'
             }
             LOGGER.error(exception)
-            return headers_, 404, json.dumps(exception)
+            return headers_, 404, to_json(exception, self.pretty_print)
         except ProviderQueryError as err:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'query error (check logs)'
             }
             LOGGER.error(err)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
         except ProviderGenericError as err:
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'generic error (check logs)'
             }
             LOGGER.error(err)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
 
         if content is None:
             exception = {
                 'code': 'NotFound',
                 'description': 'identifier not found'
             }
             LOGGER.error(exception)
-            return headers_, 404, json.dumps(exception)
+            return headers_, 404, to_json(exception, self.pretty_print)
 
         content['links'] = [{
             'rel': 'self' if not format_ or format_ == 'json' else 'alternate',
             'type': 'application/geo+json',
             'title': 'This document as GeoJSON',
             'href': '{}/collections/{}/items/{}?f=json'.format(
                 self.config['server']['url'], dataset, identifier)
@@ -1053,162 +1193,640 @@
         elif format_ == 'jsonld':
             headers_['Content-Type'] = 'application/ld+json'
             content = geojson2geojsonld(
                 self.config, content, dataset, identifier=identifier
             )
             return headers_, 200, content
 
-        return headers_, 200, json.dumps(content, default=json_serial)
+        return headers_, 200, to_json(content, self.pretty_print)
+
+    @jsonldify
+    def get_collection_coverage(self, headers, args, dataset):
+        """
+        Returns a subset of a collection coverage
+
+        :param headers: dict of HTTP headers
+        :param args: dict of HTTP request parameters
+        :param dataset: dataset name
+
+        :returns: tuple of headers, status code, content
+        """
+
+        headers_ = HEADERS.copy()
+        query_args = {}
+        format_ = 'json'
+
+        LOGGER.debug('Processing query parameters')
+
+        subsets = {}
+
+        LOGGER.debug('Loading provider')
+        try:
+            collection_def = get_provider_by_type(
+                self.config['resources'][dataset]['providers'], 'coverage')
+
+            p = load_plugin('provider', collection_def)
+        except KeyError:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'collection does not exist'
+            }
+            LOGGER.error(exception)
+            return headers_, 404, to_json(exception, self.pretty_print)
+        except ProviderTypeError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'invalid provider type'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+        except ProviderConnectionError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'connection error (check logs)'
+            }
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
+
+        LOGGER.debug('Processing bbox parameter')
+
+        bbox = args.get('bbox')
+
+        if bbox is None:
+            bbox = []
+        else:
+            try:
+                bbox = validate_bbox(bbox)
+            except ValueError as err:
+                exception = {
+                    'code': 'InvalidParameterValue',
+                    'description': str(err)
+                }
+                LOGGER.error(exception)
+                return headers_, 400, to_json(exception, self.pretty_print)
+
+        query_args['bbox'] = bbox
+
+        LOGGER.debug('Processing datetime parameter')
+
+        datetime_ = args.get('datetime', None)
+
+        try:
+            datetime_ = validate_datetime(
+                self.config['resources'][dataset]['extents'], datetime_)
+        except ValueError as err:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': str(err)
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+
+        query_args['datetime_'] = datetime_
+
+        if 'f' in args:
+            query_args['format_'] = format_ = args['f']
+
+        if 'rangeSubset' in args:
+            LOGGER.debug('Processing rangeSubset parameter')
+
+            query_args['range_subset'] = list(
+                filter(None, args['rangeSubset'].split(',')))
+            LOGGER.debug('Fields: {}'.format(query_args['range_subset']))
+
+            for a in query_args['range_subset']:
+                if a not in p.fields:
+                    exception = {
+                        'code': 'InvalidParameterValue',
+                        'description': 'Invalid field specified'
+                    }
+                    LOGGER.error(exception)
+                    return headers_, 400, to_json(exception, self.pretty_print)
+
+        if 'subset' in args:
+            LOGGER.debug('Processing subset parameter')
+            for s in args['subset'].split(','):
+                try:
+                    if '"' not in s:
+                        m = re.search(r'(.*)\((.*):(.*)\)', s)
+                    else:
+                        m = re.search(r'(.*)\(\"(\S+)\":\"(\S+.*)\"\)', s)
+
+                    subset_name = m.group(1)
+
+                    if subset_name not in p.axes:
+                        exception = {
+                            'code': 'InvalidParameterValue',
+                            'description': 'Invalid axis name'
+                        }
+                        LOGGER.error(exception)
+                        return (headers_, 400, to_json(exception,
+                                self.pretty_print))
+
+                    subsets[subset_name] = list(map(
+                        get_typed_value, m.group(2, 3)))
+                except AttributeError:
+                    exception = {
+                        'code': 'InvalidParameterValue',
+                        'description': 'subset should be like "axis(min:max)"'
+                    }
+                    LOGGER.error(exception)
+                    return headers_, 400, to_json(exception, self.pretty_print)
+
+            query_args['subsets'] = subsets
+            LOGGER.debug('Subsets: {}'.format(query_args['subsets']))
+
+        LOGGER.debug('Querying coverage')
+        try:
+            data = p.query(**query_args)
+        except ProviderInvalidQueryError as err:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'query error: {}'.format(err),
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+        except ProviderNoDataError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'No data found'
+            }
+            LOGGER.debug(exception)
+            return headers_, 204, to_json(exception, self.pretty_print)
+        except ProviderQueryError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'query error (check logs)'
+            }
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
+
+        mt = collection_def['format']['name']
+
+        if format_ == mt:
+            headers_['Content-Type'] = collection_def['format']['mimetype']
+            return headers_, 200, data
+        elif format_ == 'json':
+            headers_['Content-Type'] = 'application/prs.coverage+json'
+            return headers_, 200, to_json(data, self.pretty_print)
+        else:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'invalid format parameter'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(data, self.pretty_print)
+
+    @jsonldify
+    def get_collection_coverage_domainset(self, headers, args, dataset):
+        """
+        Returns a collection coverage domainset
+
+        :param headers: dict of HTTP headers
+        :param args: dict of HTTP request parameters
+        :param dataset: dataset name
+
+        :returns: tuple of headers, status code, content
+        """
+
+        headers_ = HEADERS.copy()
+
+        format_ = check_format(args, headers)
+        if format_ is None:
+            format_ = 'json'
+
+        LOGGER.debug('Loading provider')
+        try:
+            collection_def = get_provider_by_type(
+                self.config['resources'][dataset]['providers'], 'coverage')
+
+            p = load_plugin('provider', collection_def)
+
+            data = p.get_coverage_domainset()
+        except KeyError:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'collection does not exist'
+            }
+            LOGGER.error(exception)
+            return headers_, 404, to_json(exception, self.pretty_print)
+        except ProviderTypeError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'invalid provider type'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+        except ProviderConnectionError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'connection error (check logs)'
+            }
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
+
+        if format_ == 'json':
+            return headers_, 200, to_json(data, self.pretty_print)
+        elif format_ == 'html':
+            data['id'] = dataset
+            data['title'] = self.config['resources'][dataset]['title']
+            content = render_j2_template(self.config, 'domainset.html',
+                                         data)
+            headers_['Content-Type'] = 'text/html'
+            return headers_, 200, content
+        else:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'invalid format parameter'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+
+    @jsonldify
+    def get_collection_coverage_rangetype(self, headers, args, dataset):
+        """
+        Returns a collection coverage rangetype
+
+        :param headers: dict of HTTP headers
+        :param args: dict of HTTP request parameters
+        :param dataset: dataset name
+
+        :returns: tuple of headers, status code, content
+        """
+
+        headers_ = HEADERS.copy()
+        format_ = check_format(args, headers)
+        if format_ is None:
+            format_ = 'json'
+
+        LOGGER.debug('Loading provider')
+        try:
+            collection_def = get_provider_by_type(
+                self.config['resources'][dataset]['providers'], 'coverage')
+
+            p = load_plugin('provider', collection_def)
+
+            data = p.get_coverage_rangetype()
+        except KeyError:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'collection does not exist'
+            }
+            LOGGER.error(exception)
+            return headers_, 404, to_json(exception, self.pretty_print)
+        except ProviderTypeError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'invalid provider type'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+        except ProviderConnectionError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'connection error (check logs)'
+            }
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
+
+        if format_ == 'json':
+            return (headers_, 200, to_json(data, self.pretty_print))
+        elif format_ == 'html':
+            data['id'] = dataset
+            data['title'] = self.config['resources'][dataset]['title']
+            content = render_j2_template(self.config, 'rangetype.html',
+                                         data)
+            headers_['Content-Type'] = 'text/html'
+            return headers_, 200, content
+        else:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'invalid format parameter'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
     @pre_process
     @jsonldify
-    def get_stac_root(self, headers_, format_):
+    def get_collection_tiles(self, headers_, format_, dataset=None):
+        """
+        Provide collection tiles
+
+        :param headers_: copy of HEADERS object
+        :param format_: format of requests,
+                        pre checked by pre_process decorator
+        :param dataset: name of collection
+
+        :returns: tuple of headers, status code, content
+        """
 
         if format_ is not None and format_ not in FORMATS:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
             return headers_, 400, json.dumps(exception)
 
-        id_ = 'pygeoapi-stac'
-        stac_version = '0.6.2'
-        stac_url = os.path.join(self.config['server']['url'], 'stac')
+        if any([dataset is None,
+                dataset not in self.config['resources'].keys()]):
 
-        content = {
-            'id': id_,
-            'stac_version': stac_version,
-            'title': self.config['metadata']['identification']['title'],
-            'description': self.config['metadata']['identification']['description'],  # noqa
-            'license': self.config['metadata']['license']['name'],
-            'providers': [{
-                'name': self.config['metadata']['provider']['name'],
-                'url': self.config['metadata']['provider']['url'],
-            }],
-            'links': []
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid collection'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, json.dumps(exception)
+
+        LOGGER.debug('Creating collection tiles')
+        LOGGER.debug('Loading provider')
+        try:
+            t = get_provider_by_type(
+                    self.config['resources'][dataset]['providers'], 'tile')
+            p = load_plugin('provider', t)
+        except (KeyError, ProviderTypeError):
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid collection tiles'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception)
+        except ProviderConnectionError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'connection error (check logs)'
+            }
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception)
+        except ProviderQueryError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'query error (check logs)'
+            }
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception)
+
+        tiles = {
+            'title': dataset,
+            'description': self.config['resources'][dataset]['description'],
+            'links': [],
+            'tileMatrixSetLinks': []
         }
 
-        stac_collections = filter_dict_by_key_value(self.config['resources'],
-                                                    'type', 'stac-collection')
+        tiles['links'].append({
+            'type': 'application/json',
+            'rel': 'self' if format_ == 'json' else 'alternate',
+            'title': 'This document as JSON',
+            'href': '{}/collections/{}/tiles?f=json'.format(
+                self.config['server']['url'], dataset)
+        })
+        tiles['links'].append({
+            'type': 'application/ld+json',
+            'rel': 'self' if format_ == 'jsonld' else 'alternate',
+            'title': 'This document as RDF (JSON-LD)',
+            'href': '{}/collections/{}/tiles?f=jsonld'.format(
+                self.config['server']['url'], dataset)
+        })
+        tiles['links'].append({
+            'type': 'text/html',
+            'rel': 'self' if format_ == 'html' else 'alternate',
+            'title': 'This document as HTML',
+            'href': '{}/collections/{}/tiles?f=html'.format(
+                self.config['server']['url'], dataset)
+        })
 
-        for key, value in stac_collections.items():
-            content['links'].append({
-                'rel': 'collection',
-                'href': '{}/{}?f=json'.format(stac_url, key),
-                'type': 'application/json'
-            })
-            content['links'].append({
-                'rel': 'collection',
-                'href': '{}/{}'.format(stac_url, key),
-                'type': 'text/html'
-            })
+        for service in p.get_tiles_service(
+            baseurl=self.config['server']['url'],
+            servicepath='/collections/{}/\
+tiles/{{{}}}/{{{}}}/{{{}}}/{{{}}}?f=mvt'
+            .format(dataset, 'tileMatrixSetId',
+                    'tileMatrix', 'tileRow', 'tileCol'))['links']:
+            tiles['links'].append(service)
+
+        tiles['tileMatrixSetLinks'] = p.get_tiling_schemes()
+        metadata_format = p.options['metadata_format']
 
         if format_ == 'html':  # render
+            tiles['id'] = dataset
+            tiles['title'] = self.config['resources'][dataset]['title']
+            tiles['tilesets'] = [
+                scheme['tileMatrixSet'] for scheme in p.get_tiling_schemes()]
+            tiles['format'] = metadata_format
+            tiles['bounds'] = \
+                self.config['resources'][dataset]['extents']['spatial']['bbox']
+            tiles['minzoom'] = p.options['zoom']['min']
+            tiles['maxzoom'] = p.options['zoom']['max']
+
             headers_['Content-Type'] = 'text/html'
-            content = render_j2_template(self.config, 'stac/root.html',
-                                         content)
+            content = render_j2_template(self.config, 'tiles.html', tiles)
+
             return headers_, 200, content
 
-        return headers_, 200, json.dumps(content, default=json_serial)
+        return headers_, 200, to_json(tiles, self.pretty_print)
 
-    @pre_process
     @jsonldify
-    def get_stac_path(self, headers_, format_, path):
+    def get_collection_tiles_data(self, headers, format_, dataset=None,
+                                  matrix_id=None, z_idx=None, y_idx=None,
+                                  x_idx=None):
+        """
+        Get collection items tiles
 
-        if format_ is not None and format_ not in FORMATS:
+        :param headers: copy of HEADERS object
+        :param format_: format of requests,
+                        pre checked by pre_process decorator
+        :param dataset: dataset name
+        :param matrix_id: matrix identifier
+        :param z_idx: z index
+        :param y_idx: y index
+        :param x_idx: x index
+
+        :returns: tuple of headers, status code, content
+        """
+
+        headers_ = HEADERS.copy()
+#        format_ = check_format({}, headers)
+
+        if format_ is None and format_ not in ['mvt']:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception)
 
-        LOGGER.debug('Path: {}'.format(path))
-        dir_tokens = path.split('/')
-        if dir_tokens:
-            dataset = dir_tokens[0]
+        LOGGER.debug('Processing tiles')
 
-        stac_collections = filter_dict_by_key_value(self.config['resources'],
-                                                    'type', 'stac-collection')
+        collections = filter_dict_by_key_value(self.config['resources'],
+                                               'type', 'collection')
 
-        if dataset not in stac_collections:
+        if dataset not in collections.keys():
             exception = {
-                'code': 'NotFound',
-                'description': 'collection not found'
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid collection'
             }
             LOGGER.error(exception)
-            return headers_, 404, json.dumps(exception)
+            return headers_, 400, to_json(exception)
 
-        LOGGER.debug('Loading provider')
+        LOGGER.debug('Loading tile provider')
         try:
-            p = load_plugin('provider', stac_collections[dataset]['provider'])
+            t = get_provider_by_type(
+                self.config['resources'][dataset]['providers'], 'tile')
+            p = load_plugin('provider', t)
+
+            format_ = p.format_type
+            headers_['Content-Type'] = format_
+
+            LOGGER.debug('Fetching tileset id {} and tile {}/{}/{}'.format(
+                matrix_id, z_idx, y_idx, x_idx))
+            content = p.get_tiles(layer=p.get_layer(), tileset=matrix_id,
+                                  z=z_idx, y=y_idx, x=x_idx, format_=format_)
+            if content is None:
+                exception = {
+                    'code': 'NotFound',
+                    'description': 'identifier not found'
+                }
+                LOGGER.error(exception)
+                return headers_, 404, to_json(exception)
+            else:
+                return headers_, 202, content
+        # @TODO: figure out if the spec requires to return json errors
+        except KeyError:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid collection tiles'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception)
         except ProviderConnectionError as err:
-            LOGGER.error(err)
             exception = {
                 'code': 'NoApplicableCode',
                 'description': 'connection error (check logs)'
             }
+            LOGGER.error(err)
+            return headers_, 500, to_json(exception)
+        except ProviderTilesetIdNotFoundError:
+            exception = {
+                'code': 'NotFound',
+                'description': 'Tileset id not found'
+            }
             LOGGER.error(exception)
-            return headers_, 500, json.dumps(exception)
+            return headers_, 404, to_json(exception)
+        except ProviderTileQueryError as err:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'Tile not found'
+            }
+            LOGGER.error(err)
+            return headers_, 500, to_json(exception)
+        except ProviderTileNotFoundError as err:
+            exception = {
+                'code': 'NoMatch',
+                'description': 'tile not found (check logs)'
+            }
+            LOGGER.error(err)
+            return headers_, 404, to_json(exception)
+        except ProviderGenericError as err:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'generic error (check logs)'
+            }
+            LOGGER.error(err)
+            return headers_, 500, to_json(exception)
 
-        id_ = '{}-stac'.format(dataset)
-        stac_version = '0.6.2'
-        description = stac_collections[dataset]['description']
+    @pre_process
+    @jsonldify
+    def get_collection_tiles_metadata(self, headers_, format_, dataset=None,
+                                      matrix_id=None):
+        """
+        Get collection items tiles
 
-        content = {
-            'id': id_,
-            'stac_version': stac_version,
-            'description': description,
-            'links': []
-        }
+        :param headers_: copy of HEADERS object
+        :param format_: format of requests,
+                        pre checked by pre_process decorator
+        :param dataset: dataset name
+        :param matrix_id: matrix identifier
+
+        :returns: tuple of headers, status code, content
+        """
+
+        if format_ is not None and format_ not in FORMATS:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid format'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+
+        if any([dataset is None,
+                dataset not in self.config['resources'].keys()]):
+
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid collection'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+
+        LOGGER.debug('Creating collection tiles')
+        LOGGER.debug('Loading provider')
         try:
-            stac_data = p.get_data_path(
-                os.path.join(self.config['server']['url'], 'stac'),
-                path,
-                path.replace(dataset, '', 1)
-            )
-        except ProviderNotFoundError as err:
-            LOGGER.error(err)
+            t = get_provider_by_type(
+                self.config['resources'][dataset]['providers'], 'tile')
+            p = load_plugin('provider', t)
+        except KeyError:
             exception = {
-                'code': 'NotFound',
-                'description': 'resource not found'
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid collection tiles'
             }
-            return headers_, 404, json.dumps(exception)
-        except Exception as err:
-            LOGGER.error(err)
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+        except ProviderConnectionError:
             exception = {
                 'code': 'NoApplicableCode',
-                'description': 'data query error'
+                'description': 'connection error (check logs)'
+            }
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
+        except ProviderQueryError:
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'query error (check logs)'
             }
-            return headers_, 500, json.dumps(exception)
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
 
-        if isinstance(stac_data, dict):
-            content.update(stac_data)
-            content['links'].extend(stac_collections[dataset]['links'])
+        if matrix_id not in p.options['schemes']:
+            exception = {
+                'code': 'NotFound',
+                'description': 'tileset not found'
+            }
+            LOGGER.error(exception)
+            return headers_, 404, to_json(exception, self.pretty_print)
 
-            if format_ == 'html':  # render
-                headers_['Content-Type'] = 'text/html'
-                content['path'] = path
-                if 'assets' in content:  # item view
-                    content = render_j2_template(self.config,
-                                                 'stac/item.html',
-                                                 content)
-                else:
-                    content = render_j2_template(self.config,
-                                                 'stac/catalog.html',
-                                                 content)
+        metadata_format = p.options['metadata_format']
+        tilejson = True if (metadata_format == 'tilejson') else False
 
-                return headers_, 200, content
+        tiles_metadata = p.get_metadata(
+            dataset=dataset, server_url=self.config['server']['url'],
+            layer=p.get_layer(), tileset=matrix_id, tilejson=tilejson)
 
-            return headers_, 200, json.dumps(content, default=json_serial)
+        if format_ == 'html':  # render
+            metadata = dict(metadata=tiles_metadata)
+            metadata['id'] = dataset
+            metadata['title'] = self.config['resources'][dataset]['title']
+            metadata['tileset'] = matrix_id
+            metadata['format'] = metadata_format
+            headers_['Content-Type'] = 'text/html'
 
-        else:  # send back file
-            headers_.pop('Content-Type', None)
-            return headers_, 200, stac_data
+            content = render_j2_template(self.config, 'tiles_metadata.html',
+                                         metadata)
+
+            return headers_, 200, content
+
+        return headers_, 200, to_json(tiles_metadata, self.pretty_print)
 
     @pre_process
     @jsonldify
     def describe_processes(self, headers_, format_, process=None):
         """
         Provide processes metadata
 
@@ -1221,40 +1839,39 @@
 
         if format_ is not None and format_ not in FORMATS:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': 'Invalid format'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         processes_config = filter_dict_by_key_value(self.config['resources'],
                                                     'type', 'process')
 
         if processes_config:
             if process is not None:
                 if process not in processes_config.keys():
                     exception = {
                         'code': 'NotFound',
                         'description': 'identifier not found'
                     }
                     LOGGER.error(exception)
-                    return headers_, 404, json.dumps(exception)
+                    return headers_, 404, to_json(exception, self.pretty_print)
 
                 p = load_plugin('process',
                                 processes_config[process]['processor'])
                 p.metadata['jobControlOptions'] = ['sync-execute']
                 p.metadata['outputTransmission'] = ['value']
                 response = p.metadata
             else:
                 processes = []
                 for k, v in processes_config.items():
                     p = load_plugin('process',
                                     processes_config[k]['processor'])
-                    p.metadata['itemType'] = 'process'
                     p.metadata['jobControlOptions'] = ['sync-execute']
                     p.metadata['outputTransmission'] = ['value']
                     processes.append(p.metadata)
                 response = {
                     'processes': processes
                 }
         else:
@@ -1268,15 +1885,15 @@
                                               p.metadata)
             else:
                 response = render_j2_template(self.config, 'processes.html',
                                               {'processes': processes})
 
             return headers_, 200, response
 
-        return headers_, 200, json.dumps(response)
+        return headers_, 200, to_json(response, self.pretty_print)
 
     def execute_process(self, headers, args, data, process):
         """
         Execute process
 
         :param headers: dict of HTTP headers
         :param args: dict of HTTP request parameters
@@ -1293,51 +1910,204 @@
 
         if not data:
             exception = {
                 'code': 'MissingParameterValue',
                 'description': 'missing request data'
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
 
         processes = filter_dict_by_key_value(self.config['resources'],
                                              'type', 'process')
 
         if process not in processes:
             exception = {
                 'code': 'NotFound',
                 'description': 'identifier not found'
             }
             LOGGER.error(exception)
-            return headers_, 404, json.dumps(exception)
+            return headers_, 404, to_json(exception, self.pretty_print)
 
         p = load_plugin('process',
                         processes[process]['processor'])
 
         data_ = json.loads(data)
         for input_ in data_['inputs']:
             data_dict[input_['id']] = input_['value']
 
         try:
             outputs = p.execute(data_dict)
             m = p.metadata
-            if 'raw' in args and str2bool(args['raw']):
+            if 'response' in args and args['response'] == 'raw':
                 headers_['Content-Type'] = \
                     m['outputs'][0]['output']['formats'][0]['mimeType']
-                response = outputs
+                if 'json' in headers_['Content-Type']:
+                    response = to_json(outputs)
+                else:
+                    response = outputs
             else:
                 response['outputs'] = outputs
-            return headers_, 201, json.dumps(response)
+                response = to_json(response)
+            return headers_, 200, response
         except Exception as err:
             exception = {
                 'code': 'InvalidParameterValue',
                 'description': str(err)
             }
             LOGGER.error(exception)
-            return headers_, 400, json.dumps(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+
+    @pre_process
+    @jsonldify
+    def get_stac_root(self, headers_, format_):
+
+        if format_ is not None and format_ not in FORMATS:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid format'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+
+        id_ = 'pygeoapi-stac'
+        stac_version = '0.6.2'
+        stac_url = os.path.join(self.config['server']['url'], 'stac')
+
+        content = {
+            'id': id_,
+            'stac_version': stac_version,
+            'title': self.config['metadata']['identification']['title'],
+            'description': self.config['metadata']['identification']['description'],  # noqa
+            'license': self.config['metadata']['license']['name'],
+            'providers': [{
+                'name': self.config['metadata']['provider']['name'],
+                'url': self.config['metadata']['provider']['url'],
+            }],
+            'links': []
+        }
+
+        stac_collections = filter_dict_by_key_value(self.config['resources'],
+                                                    'type', 'stac-collection')
+
+        for key, value in stac_collections.items():
+            content['links'].append({
+                'rel': 'collection',
+                'href': '{}/{}?f=json'.format(stac_url, key),
+                'type': 'application/json'
+            })
+            content['links'].append({
+                'rel': 'collection',
+                'href': '{}/{}'.format(stac_url, key),
+                'type': 'text/html'
+            })
+
+        if format_ == 'html':  # render
+            headers_['Content-Type'] = 'text/html'
+            content = render_j2_template(self.config, 'stac/root.html',
+                                         content)
+            return headers_, 200, content
+
+        return headers_, 200, to_json(content, self.pretty_print)
+
+    @pre_process
+    @jsonldify
+    def get_stac_path(self, headers_, format_, path):
+
+        if format_ is not None and format_ not in FORMATS:
+            exception = {
+                'code': 'InvalidParameterValue',
+                'description': 'Invalid format'
+            }
+            LOGGER.error(exception)
+            return headers_, 400, to_json(exception, self.pretty_print)
+
+        LOGGER.debug('Path: {}'.format(path))
+        dir_tokens = path.split('/')
+        if dir_tokens:
+            dataset = dir_tokens[0]
+
+        stac_collections = filter_dict_by_key_value(self.config['resources'],
+                                                    'type', 'stac-collection')
+
+        if dataset not in stac_collections:
+            exception = {
+                'code': 'NotFound',
+                'description': 'collection not found'
+            }
+            LOGGER.error(exception)
+            return headers_, 404, to_json(exception, self.pretty_print)
+
+        LOGGER.debug('Loading provider')
+        try:
+            p = load_plugin('provider', get_provider_by_type(
+                stac_collections[dataset]['providers'], 'stac'))
+        except ProviderConnectionError as err:
+            LOGGER.error(err)
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'connection error (check logs)'
+            }
+            LOGGER.error(exception)
+            return headers_, 500, to_json(exception, self.pretty_print)
+
+        id_ = '{}-stac'.format(dataset)
+        stac_version = '0.6.2'
+        description = stac_collections[dataset]['description']
+
+        content = {
+            'id': id_,
+            'stac_version': stac_version,
+            'description': description,
+            'extent': stac_collections[dataset]['extents'],
+            'links': []
+        }
+        try:
+            stac_data = p.get_data_path(
+                os.path.join(self.config['server']['url'], 'stac'),
+                path,
+                path.replace(dataset, '', 1)
+            )
+        except ProviderNotFoundError as err:
+            LOGGER.error(err)
+            exception = {
+                'code': 'NotFound',
+                'description': 'resource not found'
+            }
+            return headers_, 404, to_json(exception, self.pretty_print)
+        except Exception as err:
+            LOGGER.error(err)
+            exception = {
+                'code': 'NoApplicableCode',
+                'description': 'data query error'
+            }
+            return headers_, 500, to_json(exception, self.pretty_print)
+
+        if isinstance(stac_data, dict):
+            content.update(stac_data)
+            content['links'].extend(stac_collections[dataset]['links'])
+
+            if format_ == 'html':  # render
+                headers_['Content-Type'] = 'text/html'
+                content['path'] = path
+                if 'assets' in content:  # item view
+                    content = render_j2_template(self.config,
+                                                 'stac/item.html',
+                                                 content)
+                else:
+                    content = render_j2_template(self.config,
+                                                 'stac/catalog.html',
+                                                 content)
+
+                return headers_, 200, content
+
+            return headers_, 200, to_json(content, self.pretty_print)
+
+        else:  # send back file
+            headers_.pop('Content-Type', None)
+            return headers_, 200, stac_data
 
 
 def check_format(args, headers):
     """
     check format requested from arguments or headers
 
     :param args: dict of request keyword value pairs
@@ -1368,7 +2138,119 @@
             format_ = 'html'
         elif 'application/ld+json' in headers_:
             format_ = 'jsonld'
         elif 'application/json' in headers_:
             format_ = 'json'
 
     return format_
+
+
+def validate_bbox(value=None):
+    """
+    Helper function to validate bbox parameter
+
+    :param bbox: `list` of minx, miny, maxx, maxy
+
+    :returns: `list` of bbox as `float`s
+    """
+
+    if value is None:
+        LOGGER.debug('bbox is empty')
+        return []
+
+    bbox = value.split(',')
+
+    if len(bbox) != 4:
+        msg = 'bbox should be 4 values (minx,miny,maxx,maxy)'
+        LOGGER.debug(msg)
+        raise ValueError(msg)
+
+    try:
+        bbox = [float(c) for c in bbox]
+    except ValueError as err:
+        msg = 'bbox values must be numbers'
+        err.args = (msg,)
+        LOGGER.debug(msg)
+        raise
+
+    if bbox[0] > bbox[2] or bbox[1] > bbox[3]:
+        msg = 'min values should be less than max values'
+        LOGGER.debug(msg)
+        raise ValueError(msg)
+
+    return bbox
+
+
+def validate_datetime(resource_def, datetime_=None):
+    """
+    Helper function to validate temporal parameter
+
+    :param resource_def: `dict` of configuration resource definition
+    :param datetime_: `str` of datetime parameter
+
+    :returns: `str` datetime_ input, if valid
+    """
+
+    # TODO: pass datetime to query as a `datetime` object
+    # we would need to ensure partial dates work accordingly
+    # as well as setting '..' values to `None` so that underlying
+    # providers can just assume a `datetime.datetime` object
+    #
+    # NOTE: needs testing when passing partials from API to backend
+
+    datetime_invalid = False
+
+    if (datetime_ is not None and 'temporal' in resource_def):
+
+        dateparse_begin = partial(dateparse, default=datetime.min)
+        dateparse_end = partial(dateparse, default=datetime.max)
+        unix_epoch = datetime(1970, 1, 1, 0, 0, 0)
+        dateparse_ = partial(dateparse, default=unix_epoch)
+
+        te = resource_def['temporal']
+
+        if te['begin'] is not None and te['begin'].tzinfo is None:
+            te['begin'] = te['begin'].replace(tzinfo=pytz.UTC)
+        if te['end'] is not None and te['end'].tzinfo is None:
+            te['end'] = te['end'].replace(tzinfo=pytz.UTC)
+
+        if '/' in datetime_:  # envelope
+            LOGGER.debug('detected time range')
+            LOGGER.debug('Validating time windows')
+            datetime_begin, datetime_end = datetime_.split('/')
+            if datetime_begin != '..':
+                datetime_begin = dateparse_begin(datetime_begin)
+                if datetime_begin.tzinfo is None:
+                    datetime_begin = datetime_begin.replace(
+                        tzinfo=pytz.UTC)
+
+            if datetime_end != '..':
+                datetime_end = dateparse_end(datetime_end)
+                if datetime_end.tzinfo is None:
+                    datetime_end = datetime_end.replace(tzinfo=pytz.UTC)
+
+            datetime_invalid = any([
+                (te['begin'] is not None and datetime_begin != '..' and
+                    datetime_begin < te['begin']),
+                (te['end'] is not None and datetime_end != '..' and
+                    datetime_end > te['end'])
+            ])
+
+        else:  # time instant
+            LOGGER.debug('detected time instant')
+            datetime__ = dateparse_(datetime_)
+            if datetime__ != '..':
+                if datetime__.tzinfo is None:
+                    datetime__ = datetime__.replace(tzinfo=pytz.UTC)
+            datetime_invalid = any([
+                (te['begin'] is not None and datetime__ != '..' and
+                    datetime__ < te['begin']),
+                (te['end'] is not None and datetime__ != '..' and
+                    datetime__ > te['end'])
+            ])
+
+    if datetime_invalid:
+        msg = 'datetime parameter out of range'
+        LOGGER.debug(msg)
+        raise ValueError(msg)
+
+    return datetime_
```

### Comparing `pygeoapi-0.8.0/pygeoapi/formatter/__init__.py` & `pygeoapi-0.9.0/pygeoapi/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/formatter/base.py` & `pygeoapi-0.9.0/pygeoapi/formatter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def __init__(self, formatter_def):
         """
         Initialize object
 
         :param formatter_def: formatter definition
 
-        :returns: pygeoapi.providers.base.BaseFormatter
+        :returns: pygeoapi.formatter.base.BaseFormatter
         """
 
         self.mimetype = None
         self.geom = False
 
         self.name = formatter_def['name']
         if 'geom' in formatter_def:
```

### Comparing `pygeoapi-0.8.0/pygeoapi/formatter/csv_.py` & `pygeoapi-0.9.0/pygeoapi/formatter/csv_.py`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/linked_data.py` & `pygeoapi-0.9.0/pygeoapi/linked_data.py`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/log.py` & `pygeoapi-0.9.0/pygeoapi/log.py`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/openapi.py` & `pygeoapi-0.9.0/pygeoapi/openapi.py`

 * *Files 27% similar despite different names*

```diff
@@ -30,22 +30,29 @@
 from copy import deepcopy
 import logging
 import os
 
 import click
 import yaml
 
+from pygeoapi import __version__
 from pygeoapi.plugin import load_plugin
-from pygeoapi.util import filter_dict_by_key_value, yaml_load
+from pygeoapi.provider.base import ProviderTypeError
+from pygeoapi.util import (filter_dict_by_key_value, get_provider_by_type,
+                           filter_providers_by_type, yaml_load)
 
 LOGGER = logging.getLogger(__name__)
 
 OPENAPI_YAML = {
     'oapif': 'http://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/ogcapi-features-1.yaml',  # noqa
-    'oapip': 'https://raw.githubusercontent.com/opengeospatial/wps-rest-binding/master/core/openapi'  # noqa
+    'oapip': 'https://raw.githubusercontent.com/opengeospatial/wps-rest-binding/master/core/openapi',  # noqa
+#    'oacov': 'https://raw.githubusercontent.com/opengeospatial/OGC-API-Sprint-August-2020/master/docs/Draft_Spring_Guide_for_OGC_API_Coverages/openapi'  # noqa
+    'oacov': 'https://raw.githubusercontent.com/tomkralidis/ogcapi-coverages-1/fix-cis/yaml-unresolved',  # noqa
+    'oapit': 'https://raw.githubusercontent.com/opengeospatial/OGC-API-Tiles/master/openapi/swaggerhub/tiles.yaml',  # noqa
+    'oapimt': 'https://raw.githubusercontent.com/opengeospatial/OGC-API-Tiles/master/openapi/swaggerhub/map-tiles.yaml'  # noqa
 }
 
 
 def get_ogc_schemas_location(server_config):
 
     osl = server_config.get('ogc_schemas_location', None)
 
@@ -135,104 +142,121 @@
             'url': cfg['metadata']['provider']['url'],
             'email': cfg['metadata']['contact']['email']
         },
         'license': {
             'name': cfg['metadata']['license']['name'],
             'url': cfg['metadata']['license']['url']
         },
-        'version': '3.0.2'
+        'version': __version__
     }
     oas['info'] = info
 
     oas['servers'] = [{
         'url': cfg['server']['url'],
         'description': cfg['metadata']['identification']['description']
     }]
 
     paths['/'] = {
         'get': {
             'summary': 'Landing page',
             'description': 'Landing page',
             'tags': ['server'],
+            'operationId': 'getLandingPage',
             'parameters': [
                 {'$ref': '#/components/parameters/f'}
             ],
             'responses': {
-                200: {'$ref': '{}#/components/responses/LandingPage'.format(OPENAPI_YAML['oapif'])},  # noqa
-                400: {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
-                500: {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                '200': {'$ref': '{}#/components/responses/LandingPage'.format(OPENAPI_YAML['oapif'])},  # noqa
+                '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
             }
         }
     }
 
     paths['/openapi'] = {
         'get': {
             'summary': 'This document',
             'description': 'This document',
             'tags': ['server'],
+            'operationId': 'getOpenapi',
             'parameters': [
                 {'$ref': '#/components/parameters/f'}
             ],
             'responses': {
-                200: {'$ref': '#/components/responses/200'},
-                400: {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                '200': {'$ref': '#/components/responses/200'},
+                '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
                 'default': {'$ref': '#/components/responses/default'}
             }
         }
     }
 
     paths['/conformance'] = {
         'get': {
             'summary': 'API conformance definition',
             'description': 'API conformance definition',
             'tags': ['server'],
+            'operationId': 'getConformanceDeclaration',
             'parameters': [
                 {'$ref': '#/components/parameters/f'}
             ],
             'responses': {
-                200: {'$ref': '{}#/components/responses/ConformanceDeclaration'.format(OPENAPI_YAML['oapif'])},  # noqa
-                400: {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
-                500: {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                '200': {'$ref': '{}#/components/responses/ConformanceDeclaration'.format(OPENAPI_YAML['oapif'])},  # noqa
+                '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
             }
         }
     }
 
     paths['/collections'] = {
         'get': {
             'summary': 'Collections',
             'description': 'Collections',
             'tags': ['server'],
+            'operationId': 'getCollections',
             'parameters': [
                 {'$ref': '#/components/parameters/f'}
             ],
             'responses': {
-                200: {'$ref': '{}#/components/responses/Collections'.format(OPENAPI_YAML['oapif'])},  # noqa
-                400: {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
-                500: {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                '200': {'$ref': '{}#/components/responses/Collections'.format(OPENAPI_YAML['oapif'])},  # noqa
+                '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
             }
         }
     }
 
     oas['tags'].append({
-        'name': 'server',
-        'description': cfg['metadata']['identification']['description'],
-        'externalDocs': {
-            'description': 'information',
-            'url': cfg['metadata']['identification']['url']}
+            'name': 'server',
+            'description': cfg['metadata']['identification']['description'],
+            'externalDocs': {
+                'description': 'information',
+                'url': cfg['metadata']['identification']['url']}
+        }
+    )
+    oas['tags'].append({
+            'name': 'stac',
+            'description': 'SpatioTemporal Asset Catalog'
         }
     )
 
     oas['components'] = {
         'responses': {
             '200': {
                 'description': 'successful operation',
             },
             'default': {
-               'description': 'Unexpected error',
-               'content': gen_media_type_object('application/json', 'oapip', 'schemas/exception.yaml')  # noqa
+                'description': 'Unexpected error',
+                'content': gen_media_type_object('application/json', 'oapip', 'schemas/exception.yaml')  # noqa
+            },
+            'Queryables': {
+                'description': 'successful queryables operation',
+                'content': {
+                    'application/json': {
+                        'schema': {'$ref': '#/components/schemas/queryables'}
+                    }
+                }
             }
         },
         'parameters': {
             'f': {
                 'name': 'f',
                 'in': 'query',
                 'description': 'The optional f parameter indicates the output format which the server shall provide as part of the response document.  The default format is GeoJSON.',  # noqa
@@ -241,14 +265,40 @@
                     'type': 'string',
                     'enum': ['json', 'html', 'jsonld'],
                     'default': 'json'
                 },
                 'style': 'form',
                 'explode': False
             },
+            'properties': {
+                'name': 'properties',
+                'in': 'query',
+                'description': 'The properties that should be included for each feature. The parameter value is a comma-separated list of property names.',  # noqa
+                'required': False,
+                'style': 'form',
+                'explode': False,
+                'schema': {
+                    'type': 'array',
+                    'items': {
+                        'type': 'string'
+                    }
+                }
+            },
+            'skipGeometry': {
+                'name': 'skipGeometry',
+                'in': 'query',
+                'description': 'This option can be used to skip response geometries for each feature.',  # noqa
+                'required': False,
+                'style': 'form',
+                'explode': False,
+                'schema': {
+                    'type': 'boolean',
+                    'default': False
+                }
+            },
             'sortby': {
                 'name': 'sortby',
                 'in': 'query',
                 'description': 'The optional sortby parameter indicates the sort property and order on which the server shall present results in the response document using the convention `sortby=PROPERTY:X`, where `PROPERTY` is the sort property and `X` is the sort order (`A` is ascending, `D` is descending). Sorting by multiple properties is supported by providing a comma-separated list.',  # noqa
                 'required': False,
                 'schema': {
                     'type': 'string',
@@ -265,14 +315,66 @@
                     'type': 'integer',
                     'minimum': 0,
                     'default': 0
                 },
                 'style': 'form',
                 'explode': False
             }
+        },
+        'schemas': {
+            # TODO: change this schema once OGC will definitively publish it
+            'queryable': {
+                'type': 'object',
+                'required': [
+                    'queryable',
+                    'type'
+                ],
+                'properties': {
+                    'queryable': {
+                        'description': 'the token that may be used in a CQL predicate', # noqa
+                        'type': 'string'
+                    },
+                    'title': {
+                        'description': 'a human readable title for the queryable', # noqa
+                        'type': 'string'
+                    },
+                    'description': {
+                        'description': 'a human-readable narrative describing the queryable', # noqa
+                        'type': 'string'
+                    },
+                    'language': {
+                        'description': 'the language used for the title and description', # noqa
+                        'type': 'string',
+                        'default': [
+                            'en'
+                        ]
+                    },
+                    'type': {
+                        'description': 'the data type of the queryable', # noqa
+                        'type': 'string'
+                    },
+                    'type-ref': {
+                        'description': 'a reference to the formal definition of the type', # noqa
+                        'type': 'string',
+                        'format': 'url'
+                    }
+                }
+            },
+            'queryables': {
+                'type': 'object',
+                'required': [
+                    'queryables'
+                ],
+                'properties': {
+                    'queryables': {
+                        'type': 'array',
+                        'items': {'$ref': '#/components/schemas/queryable'}
+                    }
+                }
+            }
         }
     }
 
     items_f = deepcopy(oas['components']['parameters']['f'])
     items_f['schema']['enum'].append('csv')
 
     LOGGER.debug('setting up datasets')
@@ -297,162 +399,369 @@
         oas['tags'].append(tag)
 
         paths[collection_name_path] = {
             'get': {
                 'summary': 'Get collection metadata'.format(v['title']),  # noqa
                 'description': v['description'],
                 'tags': [k],
+                'operationId': 'describe{}Collection'.format(k.capitalize()),
                 'parameters': [
                     {'$ref': '#/components/parameters/f'}
                 ],
                 'responses': {
-                    200: {'$ref': '{}#/components/responses/Collection'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    400: {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    404: {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    500: {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                    '200': {'$ref': '{}#/components/responses/Collection'.format(OPENAPI_YAML['oapif'])},  # noqa
+                    '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                    '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                    '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
                 }
             }
         }
 
-        items_path = '{}/items'.format(collection_name_path)
+        LOGGER.debug('setting up feature endpoints')
+        try:
+            p = load_plugin('provider', get_provider_by_type(
+                            collections[k]['providers'], 'feature'))
 
-        paths[items_path] = {
-            'get': {
-                'summary': 'Get {} items'.format(v['title']),
-                'description': v['description'],
-                'tags': [k],
-                'parameters': [
-                    items_f,
-                    {'$ref': '{}#/components/parameters/bbox'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    {'$ref': '{}#/components/parameters/limit'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    {'$ref': '#/components/parameters/sortby'},
-                    {'$ref': '#/components/parameters/startindex'}
-                ],
-                'responses': {
-                    200: {'$ref': '{}#/components/responses/Features'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    400: {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    404: {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    500: {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+            items_path = '{}/items'.format(collection_name_path)
+
+            coll_properties = deepcopy(oas['components']['parameters']['properties'])  # noqa
+
+            coll_properties['schema']['items']['enum'] = list(p.fields.keys())
+
+            paths[items_path] = {
+                'get': {
+                    'summary': 'Get {} items'.format(v['title']),
+                    'description': v['description'],
+                    'tags': [k],
+                    'operationId': 'get{}Features'.format(k.capitalize()),
+                    'parameters': [
+                        items_f,
+                        {'$ref': '{}#/components/parameters/bbox'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        {'$ref': '{}#/components/parameters/limit'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        coll_properties,
+                        {'$ref': '#/components/parameters/skipGeometry'},
+                        {'$ref': '#/components/parameters/sortby'},
+                        {'$ref': '#/components/parameters/startindex'}
+                    ],
+                    'responses': {
+                        '200': {'$ref': '{}#/components/responses/Features'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                    }
                 }
             }
-        }
 
-        p = load_plugin('provider', collections[k]['provider'])
+            if p.fields:
+                queryables_path = '{}/queryables'.format(collection_name_path)
+
+                paths[queryables_path] = {
+                    'get': {
+                        'summary': 'Get {} queryables'.format(v['title']),
+                        'description': v['description'],
+                        'tags': [k],
+                        'operationId': 'get{}Queryables'.format(
+                            k.capitalize()),
+                        'parameters': [
+                            items_f,
+                        ],
+                        'responses': {
+                            '200': {'$ref': '#/components/responses/Queryables'},  # noqa
+                            '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                            '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                            '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                        }
+                    }
+                }
+
+            if p.time_field is not None:
+                paths[items_path]['get']['parameters'].append(
+                    {'$ref': '{}#/components/parameters/datetime'.format(OPENAPI_YAML['oapif'])})  # noqa
+
+            for field, type in p.fields.items():
+
+                if p.properties and field not in p.properties:
+                    LOGGER.debug('Provider specified not to advertise property')  # noqa
+                    continue
+
+                if type == 'date':
+                    schema = {
+                        'type': 'string',
+                        'format': 'date'
+                    }
+                elif type == 'float':
+                    schema = {
+                        'type': 'number',
+                        'format': 'float'
+                    }
+                elif type == 'long':
+                    schema = {
+                        'type': 'integer',
+                        'format': 'int64'
+                    }
+                else:
+                    schema = {
+                        'type': type
+                    }
+
+                path_ = '{}/items'.format(collection_name_path)
+                paths['{}'.format(path_)]['get']['parameters'].append({
+                    'name': field,
+                    'in': 'query',
+                    'required': False,
+                    'schema': schema,
+                    'style': 'form',
+                    'explode': False
+                })
+
+            paths['{}/items/{{featureId}}'.format(collection_name_path)] = {
+                'get': {
+                    'summary': 'Get {} item by id'.format(v['title']),
+                    'description': v['description'],
+                    'tags': [k],
+                    'operationId': 'get{}Feature'.format(k.capitalize()),
+                    'parameters': [
+                        {'$ref': '{}#/components/parameters/featureId'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        {'$ref': '#/components/parameters/f'}
+                    ],
+                    'responses': {
+                        '200': {'$ref': '{}#/components/responses/Feature'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                    }
+                }
+            }
+        except ProviderTypeError:
+            LOGGER.debug('collection is not feature based')
+
+        LOGGER.debug('setting up coverage endpoints')
+        try:
+            load_plugin('provider', get_provider_by_type(
+                        collections[k]['providers'], 'coverage'))
 
-        if p.fields:
-            queryables_path = '{}/queryables'.format(collection_name_path)
+            coverage_path = '{}/coverage'.format(collection_name_path)
 
-            paths[queryables_path] = {
+            paths[coverage_path] = {
                 'get': {
-                    'summary': 'Get {} queryables'.format(v['title']),
+                    'summary': 'Get {} coverage'.format(v['title']),
                     'description': v['description'],
                     'tags': [k],
+                    'operationId': 'get{}Coverage'.format(k.capitalize()),
                     'parameters': [
                         items_f,
                     ],
                     'responses': {
-                        200: {'$ref': '{}#/components/responses/Features'.format(OPENAPI_YAML['oapif'])},  # noqa
-                        400: {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
-                        404: {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
-                        500: {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                        '200': {'$ref': '{}#/components/responses/Features'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
                     }
                 }
             }
 
-        if p.time_field is not None:
-            paths[items_path]['get']['parameters'].append(
-                {'$ref': '{}#/components/parameters/datetime'.format(OPENAPI_YAML['oapif'])})  # noqa
+            coverage_domainset_path = '{}/coverage/domainset'.format(
+                collection_name_path)
 
-        for field, type in p.fields.items():
+            paths[coverage_domainset_path] = {
+                'get': {
+                    'summary': 'Get {} coverage domain set'.format(v['title']),
+                    'description': v['description'],
+                    'tags': [k],
+                    'operationId': 'get{}CoverageDomainSet'.format(
+                        k.capitalize()),
+                    'parameters': [
+                        items_f,
+                    ],
+                    'responses': {
+                        '200': {'$ref': '{}/schemas/cis_1.1/domainSet.yaml'.format(OPENAPI_YAML['oacov'])},  # noqa
+                        '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                    }
+                }
+            }
 
-            if p.properties and field not in p.properties:
-                LOGGER.debug('Provider specified not to advertise property')
-                continue
+            coverage_rangetype_path = '{}/coverage/rangetype'.format(
+                collection_name_path)
 
-            if type == 'date':
-                schema = {
-                    'type': 'string',
-                    'format': 'date'
+            paths[coverage_rangetype_path] = {
+                'get': {
+                    'summary': 'Get {} coverage range type'.format(v['title']),
+                    'description': v['description'],
+                    'tags': [k],
+                    'operationId': 'get{}CoverageRangeType'.format(
+                        k.capitalize()),
+                    'parameters': [
+                        items_f,
+                    ],
+                    'responses': {
+                        '200': {'$ref': '{}/schemas/cis_1.1/rangeType.yaml'.format(OPENAPI_YAML['oacov'])},  # noqa
+                        '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                    }
                 }
-            elif type == 'float':
-                schema = {
-                    'type': 'number',
-                    'format': 'float'
+            }
+        except ProviderTypeError:
+            LOGGER.debug('collection is not coverage based')
+
+        LOGGER.debug('setting up tiles endpoints')
+        tile_extension = filter_providers_by_type(
+            collections[k]['providers'], 'tile')
+
+        if tile_extension:
+            tp = load_plugin('provider', tile_extension)
+            oas['components']['responses'].update({
+                    'Tiles': {
+                        'description': 'Retrieves the tiles description for this collection', # noqa
+                        'content': {
+                            'application/json': {
+                                'schema': {
+                                    '$ref': '#/components/schemas/tiles'
+                                }
+                            }
+                        }
+                    }
                 }
-            elif type == 'long':
-                schema = {
-                    'type': 'integer',
-                    'format': 'int64'
+            )
+
+            oas['components']['schemas'].update({
+                    'tilematrixsetlink': {
+                        'type': 'object',
+                        'required': ['tileMatrixSet'],
+                        'properties': {
+                            'tileMatrixSet': {
+                                'type': 'string'
+                            },
+                            'tileMatrixSetURI': {
+                                'type': 'string'
+                            }
+                        }
+                    },
+                    'tiles': {
+                        'type': 'object',
+                        'required': [
+                            'tileMatrixSetLinks',
+                            'links'
+                        ],
+                        'properties': {
+                            'tileMatrixSetLinks': {
+                                'type': 'array',
+                                'items': {
+                                    '$ref': '#/components/schemas/tilematrixsetlink' # noqa
+                                }
+                            },
+                            'links': {
+                                'type': 'array',
+                                'items': {'$ref': '{}#/components/schemas/link'.format(OPENAPI_YAML['oapit'])},  # noqa
+                            }
+                        }
+                    }
                 }
-            else:
-                schema = {
-                    'type': type
+            )
+
+            tiles_path = '{}/tiles'.format(collection_name_path)
+
+            paths[tiles_path] = {
+                'get': {
+                    'summary': 'Fetch a {} tiles description'.format(v['title']), # noqa
+                    'description': v['description'],
+                    'tags': [k],
+                    'operationId': 'describe{}Tiles'.format(k.capitalize()),
+                    'parameters': [
+                        items_f,
+                    ],
+                    'responses': {
+                        '200': {'$ref': '#/components/responses/Tiles'},
+                        '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                    }
                 }
+            }
 
-            path_ = '{}/items'.format(collection_name_path)
-            paths['{}'.format(path_)]['get']['parameters'].append({
-                'name': field,
-                'in': 'query',
-                'required': False,
-                'schema': schema,
-                'style': 'form',
-                'explode': False
-            })
+            tiles_data_path = '{}/tiles/{{tileMatrixSetId}}/{{tileMatrix}}/{{tileRow}}/{{tileCol}}'.format(collection_name_path)  # noqa
 
-        paths['{}/items/{{featureId}}'.format(collection_name_path)] = {
-            'get': {
-                'summary': 'Get {} item by id'.format(v['title']),
-                'description': v['description'],
-                'tags': [k],
-                'parameters': [
-                    {'$ref': '{}#/components/parameters/featureId'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    {'$ref': '#/components/parameters/f'}
-                ],
-                'responses': {
-                    200: {'$ref': '{}#/components/responses/Feature'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    400: {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    404: {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
-                    500: {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+            paths[tiles_data_path] = {
+                'get': {
+                    'summary': 'Get a {} tile'.format(v['title']),
+                    'description': v['description'],
+                    'tags': [k],
+                    'operationId': 'get{}Tiles'.format(k.capitalize()),
+                    'parameters': [{
+                        'name': 'f',
+                        'in': 'query',
+                        'description': 'The optional f parameter indicates the output format which the server shall provide as part of the response document.',  # noqa
+                        'required': False,
+                        'schema': {
+                            'type': 'string',
+                            'enum': [tp.format_type],
+                            'default': tp.format_type
+                        },
+                        'style': 'form',
+                        'explode': False
+                    }],
+                    'responses': {
+                        '400': {'$ref': '{}#/components/responses/InvalidParameter'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '404': {'$ref': '{}#/components/responses/NotFound'.format(OPENAPI_YAML['oapif'])},  # noqa
+                        '500': {'$ref': '{}#/components/responses/ServerError'.format(OPENAPI_YAML['oapif'])}  # noqa
+                    }
+                }
+            }
+            mimetype = tile_extension['format']['mimetype']
+            paths[tiles_data_path]['get']['responses']['200'] = {
+                'content': {
+                    mimetype: {
+                        'schema': {
+                            'type': 'string',
+                            'format': 'binary'
+                        }
+                    }
                 }
             }
-        }
 
     LOGGER.debug('setting up STAC')
-    paths['/stac'] = {
-        'get': {
-            'summary': 'SpatioTemporal Asset Catalog',
-            'description': 'SpatioTemporal Asset Catalog',
-            'tags': ['stac'],
-            'parameters': [],
-            'responses': {
-                200: {'$ref': '#/components/responses/200'},
-                'default': {'$ref': '#/components/responses/default'}
+    stac_collections = filter_dict_by_key_value(cfg['resources'],
+                                                'type', 'stac-collection')
+    if stac_collections:
+        paths['/stac'] = {
+            'get': {
+                'summary': 'SpatioTemporal Asset Catalog',
+                'description': 'SpatioTemporal Asset Catalog',
+                'tags': ['stac'],
+                'operationId': 'getStacCatalog',
+                'parameters': [],
+                'responses': {
+                    '200': {'$ref': '#/components/responses/200'},
+                    'default': {'$ref': '#/components/responses/default'}
+                }
             }
         }
-    }
 
     LOGGER.debug('setting up processes')
-    paths['/processes'] = {
-        'get': {
-            'summary': 'Processes',
-            'description': 'Processes',
-            'tags': ['server'],
-            'parameters': [
-                {'$ref': '#/components/parameters/f'}
-            ],
-            'responses': {
-                200: {'$ref': '#/components/responses/200'},
-                'default': {'$ref': '#/components/responses/default'}
-            }
-        }
-    }
-
     processes = filter_dict_by_key_value(cfg['resources'], 'type', 'process')
 
     if processes:
+        paths['/processes'] = {
+            'get': {
+                'summary': 'Processes',
+                'description': 'Processes',
+                'tags': ['server'],
+                'operationId': 'getProcesses',
+                'parameters': [
+                    {'$ref': '#/components/parameters/f'}
+                ],
+                'responses': {
+                    '200': {'$ref': '{}/responses/ProcessList.yaml'.format(OPENAPI_YAML['oapip'])},  # noqa
+                    'default': {'$ref': '#/components/responses/default'}
+                }
+            }
+        }
+
         for k, v in processes.items():
             p = load_plugin('process', v['processor'])
 
             process_name_path = '/processes/{}'.format(k)
             tag = {
                 'name': k,
                 'description': p.metadata['description'],
@@ -469,41 +778,58 @@
             oas['tags'].append(tag)
 
             paths[process_name_path] = {
                 'get': {
                     'summary': 'Get process metadata',
                     'description': p.metadata['description'],
                     'tags': [k],
+                    'operationId': 'describe{}Process'.format(k.capitalize()),
                     'parameters': [
                         {'$ref': '#/components/parameters/f'}
                     ],
                     'responses': {
-                        200: {'$ref': '#/components/responses/200'},
+                        '200': {'$ref': '#/components/responses/200'},
                         'default': {'$ref': '#/components/responses/default'}
                     }
                 }
             }
             paths['{}/jobs'.format(process_name_path)] = {
                 'get': {
                     'summary': 'Retrieve job list for process',
                     'description': p.metadata['description'],
                     'tags': [k],
+                    'operationId': 'get{}Jobs'.format(k.capitalize()),
                     'responses': {
-                        200: {'$ref': '#/components/responses/200'},
+                        '200': {'$ref': '#/components/responses/200'},
+                        '404': {'$ref': '{}/responses/NotFound.yaml'.format(OPENAPI_YAML['oapip'])},  # noqa
                         'default': {'$ref': '#/components/responses/default'}
                     }
                 },
                 'post': {
                     'summary': 'Process {} execution'.format(
                         p.metadata['title']),
                     'description': p.metadata['description'],
                     'tags': [k],
-                    'parameters': [],
+                    'operationId': 'execute{}Job'.format(k.capitalize()),
+                    'parameters': [{
+                        'name': 'response',
+                        'in': 'query',
+                        'description': 'Response type',
+                        'required': False,
+                        'schema': {
+                            'type': 'string',
+                            'enum': ['raw', 'document'],
+                            'default': 'document'
+                        }
+                    }],
                     'responses': {
-                        200: {'$ref': '#/components/responses/200'},
+                        '200': {'$ref': '#/components/responses/200'},
+                        '201': {'$ref': '{}/responses/ExecuteAsync.yaml'.format(OPENAPI_YAML['oapip'])},  # noqa
+                        '404': {'$ref': '{}/responses/NotFound.yaml'.format(OPENAPI_YAML['oapip'])},  # noqa
+                        '500': {'$ref': '{}/responses/ServerError.yaml'.format(OPENAPI_YAML['oapip'])},  # noqa
                         'default': {'$ref': '#/components/responses/default'}
                     },
                     'requestBody': {
                         'description': 'Mandatory execute request JSON',
                         'required': True,
                         'content': {
                             'application/json': {
```

### Comparing `pygeoapi-0.8.0/pygeoapi/plugin.py` & `pygeoapi-0.9.0/pygeoapi/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,30 +26,32 @@
 # OTHER DEALINGS IN THE SOFTWARE.
 #
 # =================================================================
 """Plugin loader"""
 
 import importlib
 import logging
-import os
 
 LOGGER = logging.getLogger(__name__)
 
 #: Loads provider plugins to be used by pygeoapi,\
 #: formatters and processes available
 PLUGINS = {
     'provider': {
         'CSV': 'pygeoapi.provider.csv_.CSVProvider',
         'Elasticsearch': 'pygeoapi.provider.elasticsearch_.ElasticsearchProvider',  # noqa
         'GeoJSON': 'pygeoapi.provider.geojson.GeoJSONProvider',
         'OGR': 'pygeoapi.provider.ogr.OGRProvider',
         'PostgreSQL': 'pygeoapi.provider.postgresql.PostgreSQLProvider',
         'SQLiteGPKG': 'pygeoapi.provider.sqlite.SQLiteGPKGProvider',
         'MongoDB': 'pygeoapi.provider.mongo.MongoProvider',
-        'FileSystem': 'pygeoapi.provider.filesystem.FileSystemProvider'
+        'FileSystem': 'pygeoapi.provider.filesystem.FileSystemProvider',
+        'rasterio': 'pygeoapi.provider.rasterio_.RasterioProvider',
+        'xarray': 'pygeoapi.provider.xarray_.XarrayProvider',
+        'MVT': 'pygeoapi.provider.mvt.MVTProvider'
     },
     'formatter': {
         'CSV': 'pygeoapi.formatter.csv_.CSVFormatter'
     },
     'process': {
         'HelloWorld': 'pygeoapi.process.hello_world.HelloWorldProcessor'
     }
@@ -64,18 +66,14 @@
     :param plugin_def: plugin definition
 
     :returns: plugin object
     """
 
     name = plugin_def['name']
 
-    if name == "OGR":
-        os.environ["OGR_GEOJSON_MAX_OBJ_SIZE"] = os.environ.get(
-            "OGR_GEOJSON_MAX_OBJ_SIZE", "20MB")
-
     if plugin_type not in PLUGINS.keys():
         msg = 'Plugin type {} not found'.format(plugin_type)
         LOGGER.exception(msg)
         raise InvalidPluginError(msg)
 
     plugin_list = PLUGINS[plugin_type]
```

### Comparing `pygeoapi-0.8.0/pygeoapi/process/__init__.py` & `pygeoapi-0.9.0/pygeoapi/process/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/process/base.py` & `pygeoapi-0.9.0/pygeoapi/process/base.py`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/process/hello_world.py` & `pygeoapi-0.9.0/pygeoapi/process/hello_world.py`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/__init__.py` & `pygeoapi-0.9.0/pygeoapi/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/base.py` & `pygeoapi-0.9.0/pygeoapi/provider/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,25 +37,38 @@
 
     def __init__(self, provider_def):
         """
         Initialize object
 
         :param provider_def: provider definition
 
-        :returns: pygeoapi.providers.base.BaseProvider
+        :returns: pygeoapi.provider.base.BaseProvider
         """
 
-        self.name = provider_def['name']
-        self.data = provider_def['data']
+        try:
+            self.name = provider_def['name']
+            self.type = provider_def['type']
+            self.data = provider_def['data']
+        except KeyError:
+            raise RuntimeError('name/type/data are required')
+
+        self.options = provider_def.get('options', None)
         self.id_field = provider_def.get('id_field', None)
+        self.x_field = provider_def.get('x_field', None)
+        self.y_field = provider_def.get('y_field', None)
         self.time_field = provider_def.get('time_field')
         self.properties = provider_def.get('properties', [])
         self.file_types = provider_def.get('file_types', [])
         self.fields = {}
 
+        # for coverage providers
+        self.axes = []
+        self.crs = None
+        self.num_bands = None
+
     def get_fields(self):
         """
         Get provider field information (names, types)
 
         :returns: dict of fields
         """
 
@@ -70,19 +83,29 @@
         :param dirpath: directory basepath (equivalent of URL)
 
         :returns: `dict` of file listing or `dict` of GeoJSON item or raw file
         """
 
         raise NotImplementedError()
 
+    def get_metadata(self):
+        """
+        Provide data/file metadata
+
+        :returns: `dict` of metadata construct (format
+                  determined by provider/standard)
+        """
+
+        raise NotImplementedError()
+
     def query(self):
         """
         query the provider
 
-        :returns: dict of 0..n GeoJSON features
+        :returns: dict of 0..n GeoJSON features or coverage data
         """
 
         raise NotImplementedError()
 
     def get(self, identifier):
         """
         query the provider by id
@@ -104,16 +127,34 @@
 
         :param identifier: feature id
         :param new_feature: new GeoJSON feature dictionary
         """
 
         raise NotImplementedError()
 
+    def get_coverage_domainset(self):
+        """
+        Provide coverage domainset
+
+        :returns: CIS JSON object of domainset metadata
+        """
+
+        raise NotImplementedError()
+
+    def get_coverage_rangetype(self):
+        """
+        Provide coverage rangetype
+
+        :returns: CIS JSON object of rangetype metadata
+        """
+
+        raise NotImplementedError()
+
     def delete(self, identifier):
-        """Updates an existing feature id with new_feature
+        """Deletes an existing feature
 
         :param identifier: feature id
         """
 
         raise NotImplementedError()
 
     def __repr__(self):
@@ -126,21 +167,36 @@
 
 
 class ProviderConnectionError(ProviderGenericError):
     """provider connection error"""
     pass
 
 
+class ProviderTypeError(ProviderGenericError):
+    """provider type error"""
+    pass
+
+
+class ProviderInvalidQueryError(ProviderGenericError):
+    """provider invalid query error"""
+    pass
+
+
 class ProviderQueryError(ProviderGenericError):
     """provider query error"""
     pass
 
 
 class ProviderItemNotFoundError(ProviderGenericError):
-    """provider query error"""
+    """provider item not found query error"""
+    pass
+
+
+class ProviderNoDataError(ProviderGenericError):
+    """provider no data error"""
     pass
 
 
 class ProviderNotFoundError(ProviderGenericError):
     """provider not found error"""
     pass
```

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/csv_.py` & `pygeoapi-0.9.0/pygeoapi/provider/csv_.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def __init__(self, provider_def):
         """
         Initialize object
 
         :param provider_def: provider definition
 
-        :returns: pygeoapi.providers.csv_.CSVProvider
+        :returns: pygeoapi.provider.csv_.CSVProvider
         """
 
         BaseProvider.__init__(self, provider_def)
         self.geometry_x = provider_def['geometry']['x_field']
         self.geometry_y = provider_def['geometry']['y_field']
         self.fields = self.get_fields()
 
@@ -68,22 +68,26 @@
             data_ = csv.DictReader(ff)
             fields = {}
             for f in data_.fieldnames:
                 fields[f] = 'string'
             return fields
 
     def _load(self, startindex=0, limit=10, resulttype='results',
-              identifier=None, bbox=[], datetime=None, properties=[]):
+              identifier=None, bbox=[], datetime_=None, properties=[],
+              select_properties=[], skip_geometry=False):
         """
         Load CSV data
 
         :param startindex: starting record to return (default 0)
         :param limit: number of records to return (default 10)
+        :param datetime_: temporal (datestamp or extent)
         :param resulttype: return results or hit limit (default results)
         :param properties: list of tuples (name, value)
+        :param select_properties: list of property names
+        :param skip_geometry: bool of whether to skip geometry (default False)
 
         :returns: dict of GeoJSON FeatureCollection
         """
 
         found = False
         result = None
         feature_collection = {
@@ -98,24 +102,27 @@
                 LOGGER.debug('Returning hits only')
                 feature_collection['numberMatched'] = len(list(data_))
                 return feature_collection
             LOGGER.debug('Slicing CSV rows')
             for row in itertools.islice(data_, startindex, startindex+limit):
                 feature = {'type': 'Feature'}
                 feature['id'] = row.pop(self.id_field)
-                feature['geometry'] = {
-                    'type': 'Point',
-                    'coordinates': [
-                        float(row.pop(self.geometry_x)),
-                        float(row.pop(self.geometry_y))
-                    ]
-                }
-                if self.properties:
+                if not skip_geometry:
+                    feature['geometry'] = {
+                        'type': 'Point',
+                        'coordinates': [
+                            float(row.pop(self.geometry_x)),
+                            float(row.pop(self.geometry_y))
+                        ]
+                    }
+                else:
+                    feature['geometry'] = None
+                if self.properties or select_properties:
                     feature['properties'] = OrderedDict()
-                    for p in self.properties:
+                    for p in set(self.properties) | set(select_properties):
                         try:
                             feature['properties'][p] = row[p]
                         except KeyError as err:
                             LOGGER.error(err)
                             raise ProviderQueryError()
                 else:
                     feature['properties'] = row
@@ -134,30 +141,35 @@
 
         feature_collection['numberReturned'] = len(
             feature_collection['features'])
 
         return feature_collection
 
     def query(self, startindex=0, limit=10, resulttype='results',
-              bbox=[], datetime=None, properties=[], sortby=[]):
+              bbox=[], datetime_=None, properties=[], sortby=[],
+              select_properties=[], skip_geometry=False):
         """
         CSV query
 
         :param startindex: starting record to return (default 0)
         :param limit: number of records to return (default 10)
         :param resulttype: return results or hit limit (default results)
         :param bbox: bounding box [minx,miny,maxx,maxy]
-        :param datetime: temporal (datestamp or extent)
+        :param datetime_: temporal (datestamp or extent)
         :param properties: list of tuples (name, value)
         :param sortby: list of dicts (property, order)
+        :param select_properties: list of property names
+        :param skip_geometry: bool of whether to skip geometry (default False)
 
         :returns: dict of GeoJSON FeatureCollection
         """
 
-        return self._load(startindex, limit, resulttype)
+        return self._load(startindex, limit, resulttype,
+                          select_properties=select_properties,
+                          skip_geometry=skip_geometry)
 
     def get(self, identifier):
         """
         query CSV id
 
         :param identifier: feature id
```

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/elasticsearch_.py` & `pygeoapi-0.9.0/pygeoapi/provider/elasticsearch_.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 #
 # =================================================================
 
 from collections import OrderedDict
+import json
 import logging
 
 from elasticsearch import Elasticsearch, exceptions, helpers
 from elasticsearch.client.indices import IndicesClient
 
 from pygeoapi.provider.base import (BaseProvider, ProviderConnectionError,
                                     ProviderQueryError,
@@ -45,15 +46,15 @@
 
     def __init__(self, provider_def):
         """
         Initialize object
 
         :param provider_def: provider definition
 
-        :returns: pygeoapi.providers.elasticsearch_.ElasticsearchProvider
+        :returns: pygeoapi.provider.elasticsearch_.ElasticsearchProvider
         """
 
         BaseProvider.__init__(self, provider_def)
 
         url_tokens = self.data.split('/')
 
         LOGGER.debug('Setting Elasticsearch properties')
@@ -110,25 +111,28 @@
                 else:
                     type_ = v['type']
                 fields_[k] = type_
 
         return fields_
 
     def query(self, startindex=0, limit=10, resulttype='results',
-              bbox=[], datetime=None, properties=[], sortby=[]):
+              bbox=[], datetime_=None, properties=[], sortby=[],
+              select_properties=[], skip_geometry=False):
         """
         query Elasticsearch index
 
         :param startindex: starting record to return (default 0)
         :param limit: number of records to return (default 10)
         :param resulttype: return results or hit limit (default results)
         :param bbox: bounding box [minx,miny,maxx,maxy]
-        :param datetime: temporal (datestamp or extent)
+        :param datetime_: temporal (datestamp or extent)
         :param properties: list of tuples (name, value)
         :param sortby: list of dicts (property, order)
+        :param select_properties: list of property names
+        :param skip_geometry: bool of whether to skip geometry (default False)
 
         :returns: dict of 0..n GeoJSON features
         """
 
         query = {'track_total_hits': True, 'query': {'bool': {'filter': []}}}
         filter_ = []
 
@@ -154,25 +158,25 @@
                         'relation': 'intersects'
                     }
                 }
             }
 
             query['query']['bool']['filter'].append(bbox_filter)
 
-        if datetime is not None:
+        if datetime_ is not None:
             LOGGER.debug('processing datetime parameter')
             if self.time_field is None:
                 LOGGER.error('time_field not enabled for collection')
                 raise ProviderQueryError()
 
             time_field = self.mask_prop(self.time_field)
 
-            if '/' in datetime:  # envelope
+            if '/' in datetime_:  # envelope
                 LOGGER.debug('detected time range')
-                time_begin, time_end = datetime.split('/')
+                time_begin, time_end = datetime_.split('/')
 
                 range_ = {
                     'range': {
                         time_field: {
                             'gte': time_begin,
                             'lte': time_end
                         }
@@ -183,18 +187,18 @@
                 elif time_end == '..':
                     range_['range'][time_field].pop('lte')
 
                 filter_.append(range_)
 
             else:  # time instant
                 LOGGER.debug('detected time instant')
-                filter_.append({'match': {time_field: datetime}})
+                filter_.append({'match': {time_field: datetime_}})
 
             LOGGER.debug(filter_)
-            query['query']['bool']['filter'].append(filter_)
+            query['query']['bool']['filter'].append(*filter_)
 
         if properties:
             LOGGER.debug('processing properties')
             for prop in properties:
                 pf = {
                     'match': {
                         self.mask_prop(prop[0]): prop[1]
@@ -223,25 +227,34 @@
                 sort_ = {
                     sort_property: {
                         'order': sort_order
                     }
                 }
                 query['sort'].append(sort_)
 
-        if self.properties:
+        if self.properties or select_properties:
             LOGGER.debug('including specified fields: {}'.format(
                 self.properties))
             query['_source'] = {
-                'includes': list(map(self.mask_prop, self.properties))
+                'includes': list(map(self.mask_prop,
+                                 set(self.properties) | set(select_properties)))  # noqa
             }
             query['_source']['includes'].append(self.mask_prop(self.id_field))
             query['_source']['includes'].append('type')
             query['_source']['includes'].append('geometry')
+        if skip_geometry:
+            LOGGER.debug('limiting to specified fields: {}'.format(
+                select_properties))
+            try:
+                query['_source']['excludes'] = ['geometry']
+            except KeyError:
+                query['_source'] = {'excludes': ['geometry']}
         try:
             LOGGER.debug('querying Elasticsearch')
+            LOGGER.debug(json.dumps(query, indent=4))
 
             LOGGER.debug('Setting ES paging zero-based')
             if startindex > 0:
                 startindex2 = startindex - 1
             else:
                 startindex2 = startindex
 
@@ -346,31 +359,32 @@
 
         if 'properties' not in doc['_source']:
             LOGGER.debug('Looks like a GDAL ES 7 document')
             id_ = doc['_source'][self.id_field]
             if 'type' not in doc['_source']:
                 feature_['id'] = id_
                 feature_['type'] = 'Feature'
-            feature_['geometry'] = doc['_source']['geometry']
+            feature_['geometry'] = doc['_source'].get('geometry')
             feature_['properties'] = {}
             for key, value in doc['_source'].items():
                 if key == 'geometry':
                     continue
                 feature_['properties'][key] = value
         else:
             LOGGER.debug('Looks like true GeoJSON document')
             feature_ = doc['_source']
             id_ = doc['_source']['properties'][self.id_field]
             feature_['id'] = id_
+            feature_['geometry'] = doc['_source'].get('geometry')
 
         if self.properties:
             feature_thinned = {
                 'id': id_,
                 'type': feature_['type'],
-                'geometry': feature_['geometry'],
+                'geometry': feature_.get('geometry'),
                 'properties': OrderedDict()
             }
             for p in self.properties:
                 try:
                     feature_thinned['properties'][p] = feature_['properties'][p]  # noqa
                 except KeyError as err:
                     LOGGER.error(err)
```

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/filesystem.py` & `pygeoapi-0.9.0/pygeoapi/provider/filesystem.py`

 * *Files 8% similar despite different names*

```diff
@@ -136,15 +136,20 @@
             raise ProviderNotFoundError(msg)
 
         if resource_type == 'raw_file':
             with io.open(data_path, 'rb') as fh:
                 return fh.read()
 
         elif resource_type == 'directory':
-            for dc in os.listdir(data_path):
+            dirpath2 = os.listdir(data_path)
+            dirpath2.sort()
+            for dc in dirpath2:
+                # @TODO: handle a generic directory for tiles
+                if dc == "tiles":
+                    continue
                 fullpath = os.path.join(data_path, dc)
                 if os.path.isdir(fullpath):
                     newpath = os.path.join(baseurl, urlpath, dc)
                     child_links.append({
                         'rel': 'child',
                         'href': '{}?f=json'.format(newpath),
                         'type': 'application/json'
@@ -212,14 +217,16 @@
         'bbox': None,
         'geometry': None,
         'properties': {}
     }
 
     try:
         import rasterio
+        from rasterio.crs import CRS
+        from rasterio.warp import transform_bounds
         LOGGER.warning('rasterio not found. Cannot derive geospatial properties')  # noqa
     except ImportError as err:
         LOGGER.warning(err)
         return content
 
     try:
         import fiona
@@ -248,36 +255,46 @@
             ]]
         }
         for k, v in d.tags(1).items():
             content['properties'][k] = v
     except rasterio.errors.RasterioIOError:
         LOGGER.debug('Testing vector data detection')
         d = fiona.open(filepath)
+        scrs = CRS(d.crs)
+        if scrs.to_epsg() is not None and scrs.to_epsg() != 4326:
+            tcrs = CRS.from_epsg(4326)
+            bnds = transform_bounds(scrs, tcrs,
+                                    d.bounds[0], d.bounds[1],
+                                    d.bounds[2], d.bounds[3])
+            content['properties']['projection'] = scrs.to_epsg()
+        else:
+            bnds = d.bounds
 
         if d.schema['geometry'] not in [None, 'None']:
             content['bbox'] = [
-                d.bounds[0],
-                d.bounds[1],
-                d.bounds[2],
-                d.bounds[3]
+                bnds[0],
+                bnds[1],
+                bnds[2],
+                bnds[3]
             ]
             content['geometry'] = {
                 'type': 'Polygon',
                 'coordinates': [[
-                    [d.bounds[0], d.bounds[1]],
-                    [d.bounds[0], d.bounds[3]],
-                    [d.bounds[2], d.bounds[3]],
-                    [d.bounds[2], d.bounds[1]],
-                    [d.bounds[0], d.bounds[1]]
+                    [bnds[0], bnds[1]],
+                    [bnds[0], bnds[3]],
+                    [bnds[2], bnds[3]],
+                    [bnds[2], bnds[1]],
+                    [bnds[0], bnds[1]]
                 ]]
             }
+
         for k, v in d.schema['properties'].items():
             content['properties'][k] = v
 
         if d.driver == 'ESRI Shapefile':
             id_ = os.path.splitext(os.path.basename(filepath))[0]
             content['assets'] = {}
-            for suffix in ['shx', 'dbf', 'prj']:
+            for suffix in ['shx', 'dbf', 'prj', 'shp.xml']:
                 content['assets'][suffix] = {
                     'href': './{}.{}'.format(id_, suffix)
                 }
     return content
```

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/geojson.py` & `pygeoapi-0.9.0/pygeoapi/provider/geojson.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     must be present and be unique strings. Otherwise it will break.
     * How to raise errors in the provider implementation such that
     * appropriate HTTP responses will be raised
     """
 
     def __init__(self, provider_def):
         """initializer"""
+
         BaseProvider.__init__(self, provider_def)
         self.fields = self.get_fields()
 
     def get_fields(self):
         """
          Get provider field information (names, types)
 
@@ -79,15 +80,15 @@
             with open(self.data) as src:
                 data = json.loads(src.read())
             fields = {}
             for f in data['features'][0]['properties'].keys():
                 fields[f] = 'string'
             return fields
 
-    def _load(self):
+    def _load(self, skip_geometry=None, select_properties=[]):
         """Load and validate the source GeoJSON file
         at self.data
 
         Yes loading from disk, deserializing and validation
         happens on every request. This is not efficient.
         """
 
@@ -99,36 +100,45 @@
                 'type': 'FeatureCollection',
                 'features': []}
 
         # Must be a FeatureCollection
         assert data['type'] == 'FeatureCollection'
         # All features must have ids, TODO must be unique strings
         for i in data['features']:
-            i['id'] = i['properties'][self.id_field]
-
+            if 'id' not in i and self.id_field in i['properties']:
+                i['id'] = i['properties'][self.id_field]
+            if skip_geometry:
+                i['geometry'] = None
+            if self.properties or select_properties:
+                i['properties'] = {k: v for k, v in i['properties'].items()
+                                   if k in set(self.properties) | set(select_properties)}  # noqa
         return data
 
     def query(self, startindex=0, limit=10, resulttype='results',
-              bbox=[], datetime=None, properties=[], sortby=[]):
+              bbox=[], datetime_=None, properties=[], sortby=[],
+              select_properties=[], skip_geometry=False):
         """
         query the provider
 
         :param startindex: starting record to return (default 0)
         :param limit: number of records to return (default 10)
         :param resulttype: return results or hit limit (default results)
         :param bbox: bounding box [minx,miny,maxx,maxy]
-        :param datetime: temporal (datestamp or extent)
+        :param datetime_: temporal (datestamp or extent)
         :param properties: list of tuples (name, value)
         :param sortby: list of dicts (property, order)
+        :param select_properties: list of property names
+        :param skip_geometry: bool of whether to skip geometry (default False)
 
         :returns: FeatureCollection dict of 0..n GeoJSON features
         """
 
         # TODO filter by bbox without resorting to third-party libs
-        data = self._load()
+        data = self._load(skip_geometry=skip_geometry,
+                          select_properties=select_properties)
 
         data['numberMatched'] = len(data['features'])
 
         if resulttype == 'hits':
             data['features'] = []
         else:
             data['features'] = data['features'][startindex:startindex+limit]
@@ -141,32 +151,34 @@
         query the provider by id
 
         :param identifier: feature id
         :returns: dict of single GeoJSON feature
         """
 
         all_data = self._load()
+        # if matches
         for feature in all_data['features']:
-            if str(feature['properties'][self.id_field]) == identifier:
+            if str(feature.get('id')) == identifier:
                 return feature
-
         # default, no match
         err = 'item {} not found'.format(identifier)
         LOGGER.error(err)
         raise ProviderItemNotFoundError(err)
 
     def create(self, new_feature):
         """Create a new feature
 
         :param new_feature: new GeoJSON feature dictionary
         """
+
         all_data = self._load()
 
-        # Hijack the feature id and make sure it's unique
-        new_feature['properties']['id'] = str(uuid.uuid4())
+        if self.id_field not in new_feature and\
+           self.id_field not in new_feature['properties']:
+            new_feature['properties'][self.id_field] = str(uuid.uuid4())
 
         all_data['features'].append(new_feature)
 
         with open(self.data, 'w') as dst:
             dst.write(json.dumps(all_data))
 
     def update(self, identifier, new_feature):
@@ -174,33 +186,37 @@
 
         :param identifier: feature id
         :param new_feature: new GeoJSON feature dictionary
         """
 
         all_data = self._load()
         for i, feature in enumerate(all_data['features']):
-            if feature['properties']['id'] == identifier:
-                # ensure new_feature retains id
-                new_feature['properties']['id'] = identifier
-                all_data['features'][i] = new_feature
-                break
-
+            if self.id_field in feature:
+                if feature[self.id_field] == identifier:
+                    new_feature['properties'][self.id_field] = identifier
+                    all_data['features'][i] = new_feature
+            elif self.id_field in feature['properties']:
+                if feature['properties'][self.id_field] == identifier:
+                    new_feature['properties'][self.id_field] = identifier
+                    all_data['features'][i] = new_feature
         with open(self.data, 'w') as dst:
             dst.write(json.dumps(all_data))
 
     def delete(self, identifier):
-        """Updates an existing feature id with new_feature
+        """Deletes an existing feature
 
         :param identifier: feature id
         """
 
         all_data = self._load()
         for i, feature in enumerate(all_data['features']):
-            if feature['properties']['id'] == identifier:
-                all_data['features'].pop(i)
-                break
-
+            if self.id_field in feature:
+                if feature[self.id_field] == identifier:
+                    all_data['features'].pop(i)
+            elif self.id_field in feature['properties']:
+                if feature['properties'][self.id_field] == identifier:
+                    all_data['features'].pop(i)
         with open(self.data, 'w') as dst:
             dst.write(json.dumps(all_data))
 
     def __repr__(self):
         return '<GeoJSONProvider> {}'.format(self.data)
```

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/mongo.py` & `pygeoapi-0.9.0/pygeoapi/provider/mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 #
 # =================================================================
 
+from datetime import datetime
 import logging
 
 from bson import Code
 from pymongo import MongoClient
 from pymongo import GEOSPHERE
 from pymongo import ASCENDING, DESCENDING
 from pymongo.collection import ObjectId
@@ -46,15 +47,15 @@
     def __init__(self, provider_def):
         """
         MongoProvider Class constructor
 
         :param provider_def: provider definitions from yml pygeoapi-config.
                              data,id_field, name set in parent class
 
-        :returns: pygeoapi.providers.mongo.MongoProvider
+        :returns: pygeoapi.provider.mongo.MongoProvider
         """
         # this is dummy value never used in case of Mongo.
         # Mongo id field is _id
         provider_def.setdefault('id_field', '_id')
 
         BaseProvider.__init__(self, provider_def)
 
@@ -91,32 +92,33 @@
         featurelist = list(featurecursor)
         for item in featurelist:
             item['id'] = str(item.pop('_id'))
 
         return featurelist, matchCount
 
     def query(self, startindex=0, limit=10, resulttype='results',
-              bbox=[], datetime=None, properties=[], sortby=[]):
+              bbox=[], datetime_=None, properties=[], sortby=[],
+              select_properties=[], skip_geometry=False):
         """
         query the provider
 
         :returns: dict of 0..n GeoJSON features
         """
         and_filter = []
 
         if len(bbox) == 4:
             x, y, w, h = map(float, bbox)
             and_filter.append(
                 {'geometry': {'$geoWithin': {'$box': [[x, y], [w, h]]}}})
 
         # This parameter is not working yet!
         # gte is not sufficient to check date range
-        if datetime is not None:
-            assert isinstance(datetime.datetime, datetime)
-            and_filter.append({'properties.datetime': {'$gte': datetime}})
+        if datetime_ is not None:
+            assert isinstance(datetime_, datetime)
+            and_filter.append({'properties.datetime': {'$gte': datetime_}})
 
         for prop in properties:
             and_filter.append({"properties."+prop[0]: {'$eq': prop[1]}})
 
         filterobj = {'$and': and_filter} if and_filter else {}
 
         sort_list = [("properties." + sort['property'],
@@ -168,13 +170,13 @@
         :param new_feature: new GeoJSON feature dictionary
         """
         data = {k: v for k, v in updated_feature.items() if k != 'id'}
         self.featuredb[self.collection].update_one(
             {'_id': ObjectId(identifier)}, {"$set": data})
 
     def delete(self, identifier):
-        """Delets an existing feature
+        """Deletes an existing feature
 
         :param identifier: feature id
         """
         self.featuredb[self.collection].delete_one(
             {'_id': ObjectId(identifier)})
```

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/ogr.py` & `pygeoapi-0.9.0/pygeoapi/provider/ogr.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 #
 # =================================================================
 
+import functools
 import importlib
 import logging
-import functools
+import os
 from typing import Any
 
 from osgeo import gdal as osgeo_gdal
 from osgeo import ogr as osgeo_ogr
 from osgeo import osr as osgeo_osr
 
 from pygeoapi.provider.base import (
@@ -63,14 +64,16 @@
 
     # To deal with some OGR Source-Driver specifics.
     SOURCE_HELPERS = {
         'ESRIJSON': 'pygeoapi.provider.ogr.ESRIJSONHelper',
         'WFS': 'pygeoapi.provider.ogr.WFSHelper',
         '*': 'pygeoapi.provider.ogr.CommonSourceHelper'
     }
+    os.environ['OGR_GEOJSON_MAX_OBJ_SIZE'] = os.environ.get(
+        'OGR_GEOJSON_MAX_OBJ_SIZE', '20MB')
 
     # Setting for traditional CRS axis order.
     OAMS_TRADITIONAL_GIS_ORDER = osgeo_osr.OAMS_TRADITIONAL_GIS_ORDER
 
     def __init__(self, provider_def):
         """
         Initialize object
@@ -99,15 +102,15 @@
 
             id_field: gml_id
             layer: rdinfo:stations
 
 
         :param provider_def: provider definition
 
-        :returns: pygeoapi.providers.ogr.OGRProvider
+        :returns: pygeoapi.provider.ogr.OGRProvider
         """
 
         BaseProvider.__init__(self, provider_def)
 
         self.ogr = osgeo_ogr
         # http://trac.osgeo.org/gdal/wiki/PythonGotchas
         self.gdal = osgeo_gdal
@@ -280,25 +283,28 @@
 
         finally:
             self._close()
 
         return fields
 
     def query(self, startindex=0, limit=10, resulttype='results',
-              bbox=[], datetime=None, properties=[], sortby=[]):
+              bbox=[], datetime_=None, properties=[], sortby=[],
+              select_properties=[], skip_geometry=False):
         """
         Query OGR source
 
         :param startindex: starting record to return (default 0)
         :param limit: number of records to return (default 10)
         :param resulttype: return results or hit limit (default results)
         :param bbox: bounding box [minx,miny,maxx,maxy]
-        :param datetime: temporal (datestamp or extent)
+        :param datetime_: temporal (datestamp or extent)
         :param properties: list of tuples (name, value)
         :param sortby: list of dicts (property, order)
+        :param select_properties: list of property names
+        :param skip_geometry: bool of whether to skip geometry (default False)
 
         :returns: dict of 0..n GeoJSON features
         """
         result = None
         try:
             if self.source_capabilities['paging']:
                 self.source_helper.enable_paging(startindex, limit)
@@ -420,25 +426,30 @@
         packagename, classname = source_helper_class.rsplit('.', 1)
         module = importlib.import_module(packagename)
         class_ = getattr(module, classname)
         self.source_helper = class_(self)
 
     def _get_next_feature(self, layer, feature_id):
         try:
+            if layer.GetFeatureCount() == 0:
+                LOGGER.error("item {} is not found".format(feature_id))
+                raise ProviderItemNotFoundError(
+                    "item {} not found".format(feature_id))
             # Ignore gdal error
             next_feature = _ignore_gdal_error(layer, 'GetNextFeature')
             if next_feature:
                 if all(val is None for val in next_feature.items().values()):
                     self.gdal.Error(
                         self.gdal.CE_Failure, 1,
                         "Object properties are all null"
                     )
             else:
-                raise ProviderItemNotFoundError(
-                    "item {} not found".format(feature_id))
+                raise RuntimeError(
+                    "GDAL has returned a null feature for item {}".format(
+                        feature_id))
             return next_feature
         except RuntimeError as gdalerr:
             LOGGER.error(self.gdal.GetLastErrorMsg())
             raise gdalerr
 
     def _ogr_feature_to_json(self, ogr_feature):
         geom = ogr_feature.GetGeometryRef()
@@ -523,15 +534,15 @@
 
     def __init__(self, provider):
         """
         Initialize object with related OGRProvider object.
 
         :param provider: provider instance
 
-        :returns: pygeoapi.providers.ogr.SourceHelper
+        :returns: pygeoapi.provider.ogr.SourceHelper
         """
         self.provider = provider
 
     def close(self):
         """
         OGR Driver-specific handling of closing dataset.
         Default is no specific handling.
@@ -578,15 +589,15 @@
     """
     def __init__(self, provider):
         """
         Initialize object
 
         :param provider: provider instance
 
-        :returns: pygeoapi.providers.ogr.SourceHelper
+        :returns: pygeoapi.provider.ogr.SourceHelper
         """
         SourceHelper.__init__(self, provider)
         self.startindex = -1
         self.limit = -1
         self.result_set = None
 
     def close(self):
@@ -662,15 +673,15 @@
 
     def __init__(self, provider):
         """
         Initialize object
 
         :param provider: provider instance
 
-        :returns: pygeoapi.providers.ogr.SourceHelper
+        :returns: pygeoapi.provider.ogr.SourceHelper
         """
         CommonSourceHelper.__init__(self, provider)
 
     def enable_paging(self, startindex=-1, limit=-1):
         """
         Enable paged access to dataset (OGR Driver-specific)
 
@@ -725,15 +736,15 @@
 
     def __init__(self, provider):
         """
         Initialize object
 
         :param provider: provider instance
 
-        :returns: pygeoapi.providers.ogr.SourceHelper
+        :returns: pygeoapi.provider.ogr.SourceHelper
         """
         SourceHelper.__init__(self, provider)
 
     def enable_paging(self, startindex=-1, limit=-1):
         """
         Enable paged access to dataset (OGR Driver-specific)
 
@@ -762,29 +773,29 @@
 
 class GdalErrorHandler:
 
     def __init__(self):
         """
         Initialize the error handler
 
-        :returns: pygeoapi.providers.ogr.GdalErrorHandler
+        :returns: pygeoapi.provider.ogr.GdalErrorHandler
         """
         self.err_level = osgeo_gdal.CE_None
         self.err_num = 0
         self.err_msg = ''
 
     def handler(self, err_level, err_num, err_msg):
         """
         Define custom GDAL error handler function
 
         :param err_level: error level
         :param err_num: internal gdal error number
         :param err_msg: error message
 
-        :returns: pygeoapi.providers.ogr.GdalErrorHandler
+        :returns: pygeoapi.provider.ogr.GdalErrorHandler
         """
 
         err_type = {
             osgeo_gdal.CE_None: 'None',
             osgeo_gdal.CE_Debug: 'Debug',
             osgeo_gdal.CE_Warning: 'Warning',
             osgeo_gdal.CE_Failure: 'Failure',
```

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/postgresql.py` & `pygeoapi-0.9.0/pygeoapi/provider/postgresql.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         PostgreSQLProvider Class constructor
 
         :param provider_def: provider definitions from yml pygeoapi-config.
                              data,id_field, name set in parent class
                              data contains the connection information
                              for class DatabaseCursor
 
-        :returns: pygeoapi.providers.base.PostgreSQLProvider
+        :returns: pygeoapi.provider.base.PostgreSQLProvider
         """
 
         BaseProvider.__init__(self, provider_def)
 
         self.table = provider_def['table']
         self.id_field = provider_def['id_field']
         self.conn_dic = provider_def['data']
@@ -201,27 +201,30 @@
                 SQL(' AND ').join(where_conditions))
         else:
             where_clause = SQL('')
 
         return where_clause
 
     def query(self, startindex=0, limit=10, resulttype='results',
-              bbox=[], datetime=None, properties=[], sortby=[]):
+              bbox=[], datetime_=None, properties=[], sortby=[],
+              select_properties=[], skip_geometry=False):
         """
         Query Postgis for all the content.
         e,g: http://localhost:5000/collections/hotosm_bdi_waterways/items?
         limit=1&resulttype=results
 
         :param startindex: starting record to return (default 0)
         :param limit: number of records to return (default 10)
         :param resulttype: return results or hit limit (default results)
         :param bbox: bounding box [minx,miny,maxx,maxy]
-        :param datetime: temporal (datestamp or extent)
+        :param datetime_: temporal (datestamp or extent)
         :param properties: list of tuples (name, value)
         :param sortby: list of dicts (property, order)
+        :param select_properties: list of property names
+        :param skip_geometry: bool of whether to skip geometry (default False)
 
         :returns: GeoJSON FeaturesCollection
         """
         LOGGER.debug('Querying PostGIS')
 
         if resulttype == 'hits':
```

### Comparing `pygeoapi-0.8.0/pygeoapi/provider/sqlite.py` & `pygeoapi-0.9.0/pygeoapi/provider/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def __init__(self, provider_def):
         """
         SQLiteGPKGProvider Class constructor
 
         :param provider_def: provider definitions from yml pygeoapi-config.
                              data,id_field, name set in parent class
 
-        :returns: pygeoapi.providers.base.SQLiteProvider
+        :returns: pygeoapi.provider.base.SQLiteProvider
         """
         BaseProvider.__init__(self, provider_def)
 
         self.table = provider_def['table']
         self.application_id = None
         self.geom_col = None
 
@@ -247,28 +247,31 @@
 
         if self.application_id:
             self.table = "vgpkg_{}".format(self.table)
 
         return cursor
 
     def query(self, startindex=0, limit=10, resulttype='results',
-              bbox=[], datetime=None, properties=[], sortby=[]):
+              bbox=[], datetime_=None, properties=[], sortby=[],
+              select_properties=[], skip_geometry=False):
         """
         Query SQLite/GPKG for all the content.
         e,g: http://localhost:5000/collections/countries/items?
         limit=5&startindex=2&resulttype=results&continent=Europe&admin=Albania&bbox=29.3373,-3.4099,29.3761,-3.3924
         http://localhost:5000/collections/countries/items?continent=Africa&bbox=29.3373,-3.4099,29.3761,-3.3924
 
         :param startindex: starting record to return (default 0)
         :param limit: number of records to return (default 10)
         :param resulttype: return results or hit limit (default results)
         :param bbox: bounding box [minx,miny,maxx,maxy]
-        :param datetime: temporal (datestamp or extent)
+        :param datetime_: temporal (datestamp or extent)
         :param properties: list of tuples (name, value)
         :param sortby: list of dicts (property, order)
+        :param select_properties: list of property names
+        :param skip_geometry: bool of whether to skip geometry (default False)
 
         :returns: GeoJSON FeaturesCollection
         """
         LOGGER.debug('Querying SQLite/GPKG')
 
         where_clause, where_values = self.__get_where_clauses(
             properties=properties, bbox=bbox)
```

### Comparing `pygeoapi-0.8.0/pygeoapi/static/css/default.css` & `pygeoapi-0.9.0/pygeoapi/static/css/default.css`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/static/img/favicon.ico` & `pygeoapi-0.9.0/pygeoapi/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/static/img/logo.png` & `pygeoapi-0.9.0/pygeoapi/static/img/pygeoapi.png`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/static/img/pygeoapi.png` & `pygeoapi-0.9.0/pygeoapi/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/templates/base.html` & `pygeoapi-0.9.0/pygeoapi/templates/base.html`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/templates/collections.html` & `pygeoapi-0.9.0/pygeoapi/templates/stac/root.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 {% extends "base.html" %}
-{% block title %}{{ super() }} Collections {% endblock %}
+{% block title %}{{ super() }} SpatioTemporal Asset Catalog {% endblock %}
 {% block crumbs %}{{ super() }}
-/ <a href="./collections">Collections</a>
+/ <a href="./stac">SpatioTemporal Asset Catalog</a>
 {% endblock %}
 {% block body %}
-    <section id="collections" itemscope itemtype="https://schema.org/DataCatalog">
-    <meta itemprop="url" content="{{ config['server']['url'] }}" />
-    <meta itemprop="name" content="{{ config['metadata']['identification']['title'] | striptags }}" />
-    <meta itemprop="description" content="{{ config['metadata']['identification']['description'] | striptags }}" />
-      <h2>Collections in this service</h2>
+
+    <section id="identification">
+      <h4>STAC Version: {{ data['stac_version'] }}</h4>
+    </section>
+
+    <section id="collections">
+      <h2>Collections</h2>
             <table class="striped">
               <thead>
               <tr>
                 <th>Name</th>
                 <th>Description</th>
               </tr>
               </thead>
               <tbody>
-                {% for k, v in filter_dict_by_key_value(config['resources'], 'type', 'collection').items() %}
-                <tr itemprop="dataset" itemscope itemtype="https://schema.org/Dataset">
+                {% for k, v in filter_dict_by_key_value(config['resources'], 'type', 'stac-collection').items() %}
+                <tr>
                   <td data-label="name">
-                    <meta itemprop="url" content="{{ config['server']['url'] }}/collections/{{ k }}" />
                     <a  title="{{ v['title'] | striptags | truncate }}"
-                      href="{{ config['server']['url'] }}/collections/{{ k }}">
-                      <span itemprop="name">{{ v['title'] | striptags | truncate }}</span></a>
+                      href="{{ config['server']['url'] }}/stac/{{ k }}">
+                      <span>{{ v['title'] | striptags | truncate }}</span></a>
                   </td>
-                  <td itemprop="description" data-label="description">
+                  <td data-label="description">
                     {{ v['description'] | striptags | truncate }}
                   </td>
                 </tr>
                 {% endfor %}
               </tbody>
             </table>
     </section>
+
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends "base.html" %} {% block title %}{{ super() }} Collections {%
-endblock %} {% block crumbs %}{{ super() }} / Collections {% endblock %} {%
-block body %}
+{% extends "base.html" %} {% block title %}{{ super() }} SpatioTemporal Asset
+Catalog {% endblock %} {% block crumbs %}{{ super() }} / SpatioTemporal_Asset
+Catalog {% endblock %} {% block body %}
+*** STAC Version: {{ data['stac_version'] }} ***
 
-
-***** Collections in this service *****
-Name                                     Description
- {{_v['title']_|_striptags_|_truncate_}} {{ v['description'] | striptags |
-                                         truncate }}
+***** Collections *****
+Name                                    Description
+{{_v['title']_|_striptags_|_truncate_}} {{ v['description'] | striptags |
+                                        truncate }}
  {% endblock %}
```

### Comparing `pygeoapi-0.8.0/pygeoapi/templates/item.html` & `pygeoapi-0.9.0/pygeoapi/templates/item.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "base.html" %}
 {# Optionally renders an img element, otherwise standard value or link rendering #}
 {% macro render_item_value(v, width) -%}
-    {% set val = v | string | trim | lower %}
-    {% if val|length and val.endswith(('.jpg', '.jpeg', '.png', '.gif', '.bmp')) %}
+    {% set val = v | string | trim %}
+    {% if val|length and val.lower().endswith(('.jpg', '.jpeg', '.png', '.gif', '.bmp')) %}
         {# Ends with image extension: render img element with link to image #}
         <a href="{{ val }}"><img src="{{ val }}" alt="" width="{{ width }}"/></a>
     {% else %}
         {# All other cases: text or link value #}
         {{ v | urlize() }}
     {% endif %}
 {%- endmacro %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "base.html" %} {# Optionally renders an img element, otherwise
 standard value or link rendering #} {% macro render_item_value(v, width) -%} {%
-set val = v | string | trim | lower %} {% if val|length and val.endswith(
+set val = v | string | trim %} {% if val|length and val.lower().endswith(
 ('.jpg', '.jpeg', '.png', '.gif', '.bmp')) %} {# Ends with image extension:
 render img element with link to image #}  {% else %} {# All other cases: text
 or link value #} {{ v | urlize() }} {% endif %} {%- endmacro %} {% block title
 %}{{ super() }} {{ data['title'] }} - {{ data['id'] }}{% endblock %} {% block
 crumbs %}{{ super() }} / Collections {% for link in data['links'] %} {% if
 link.rel == 'collection' %} / {{_link['title']_}} {% endif %} {% endfor %} /
 Items / Item_{{_data['id']_}} {% endblock %} {% block extrahead %}
```

### Comparing `pygeoapi-0.8.0/pygeoapi/templates/items.html` & `pygeoapi-0.9.0/pygeoapi/templates/items.html`

 * *Files identical despite different names*

### Comparing `pygeoapi-0.8.0/pygeoapi/templates/openapi.html` & `pygeoapi-0.9.0/pygeoapi/templates/openapi.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!-- HTML for static distribution bundle build -->
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8">
     <title>Swagger UI - {{ config['metadata']['identification']['title'] }}</title>
-    <link rel="stylesheet" type="text/css" href="https://unpkg.com/swagger-ui-dist@3.22.2/swagger-ui.css" >
-    <link rel="icon" type="image/png" href="https://unpkg.com/swagger-ui-dist@3.22.2/favicon-32x32.png" sizes="32x32" />
-    <link rel="icon" type="image/png" href="https://unpkg.com/swagger-ui-dist@3.22.2/favicon-16x16.png" sizes="16x16" />
+    <link rel="stylesheet" type="text/css" href="https://unpkg.com/swagger-ui-dist@3.28.0/swagger-ui.css" >
+    <link rel="icon" type="image/png" href="https://unpkg.com/swagger-ui-dist@3.28.0/favicon-32x32.png" sizes="32x32" />
+    <link rel="icon" type="image/png" href="https://unpkg.com/swagger-ui-dist@3.28.0/favicon-16x16.png" sizes="16x16" />
     <style>
       html
       {
         box-sizing: border-box;
         overflow: -moz-scrollbars-vertical;
         overflow-y: scroll;
       }
@@ -26,16 +26,16 @@
         background: #fafafa;
       }
     </style>
   </head>
 
   <body>
     <div id="swagger-ui"></div>
-    <script src="https://unpkg.com/swagger-ui-dist@3.22.2/swagger-ui-bundle.js"> </script>
-    <script src="https://unpkg.com/swagger-ui-dist@3.22.2/swagger-ui-standalone-preset.js"> </script>
+    <script src="https://unpkg.com/swagger-ui-dist@3.28.0/swagger-ui-bundle.js"> </script>
+    <script src="https://unpkg.com/swagger-ui-dist@3.28.0/swagger-ui-standalone-preset.js"> </script>
     <script>
     window.onload = function() {
       // Begin Swagger UI call region
       ui = SwaggerUIBundle({
         url: '{{ data['openapi-document-path'] }}',
         dom_id: '#swagger-ui',
         deepLinking: true,
```

### Comparing `pygeoapi-0.8.0/pygeoapi/templates/root.html` & `pygeoapi-0.9.0/pygeoapi/templates/landing_page.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 {% extends "base.html" %}
 {% block title %}{{ super() }} Home {% endblock %}
 {% block body %}
 
 <br/>
-<section id="collections" itemscope itemtype="https://schema.org/DataCatalog">
-  <meta itemprop="url" content="{{ config['server']['url'] }}" />
+<section id="collections">
 <div class="row">
   <div class="col-md-8 col-sm-12">
 
   <section id="identification">
-    <h1 itemprop="name">{{ config['metadata']['identification']['title'] }}</h1>
-    <p itemprop="description">{{ config['metadata']['identification']['description'] }}</p>
+    <h1>{{ config['metadata']['identification']['title'] }}</h1>
+    <p>{{ config['metadata']['identification']['description'] }}</p>
 
-    <p itemprop="keywords">
+    <p>
         {% for kw in config['metadata']['identification']['keywords'] %}
           <mark class="tag">{{ kw }}</mark>
         {% endfor %}
     </p>
 
     <div class="card large">
       <div class="section">
@@ -32,40 +31,44 @@
         {% endif %}
         {% if config['metadata']['license']['url'] %}
           <div class="row">
               <div class="col-sm-4">
                 License
               </div>
               <div class="col-sm-8">
-                  <a itemprop="license" href="{{ config['metadata']['license']['url'] }}">
+                  <a href="{{ config['metadata']['license']['url'] }}">
                     {{ config['metadata']['license']['name'] or config['metadata']['license']['url'] }}</a>
               </div>
           </div>
         {% endif %}
       </div>
     </div>
   </section>
   <section id="collections">
     <h2>Collections</h2>
     <p>
       <a href="{{ config['server']['url'] }}/collections?f=html">View the collections in this service</a>
     </p>
   </section>
+ {% if data['stac'] %}
   <section id="collections">
     <h2>SpatioTemporal Assets</h2>
     <p>
       <a href="{{ config['server']['url'] }}/stac?f=html">View the SpatioTemporal Assets in this service</a>
     </p>
   </section>
+ {% endif %}
+ {% if data['processes'] %}
   <section id="processes">
       <h2>Processes</h2>
       <p>
         <a href="{{ config['server']['url'] }}/processes?f=html">View the processes in this service</a>
       </p>
   </section>
+ {% endif %}
   <section id="openapi">
       <h2>API Definition</h2>
       <p>
         <a href="{{ config['server']['url'] }}/openapi?f=html">Documentation</a>
       </p>
       <p>
         <a href="{{ config['server']['url'] }}/openapi?f=json">OpenAPI Document</a>
@@ -74,59 +77,59 @@
   <section id="conformance">
       <h2>Conformance</h2>
       <p>
         <a href="{{ config['server']['url'] }}/conformance?f=html">View the conformance classes of this service</a>
       </p>
   </section>
   </div>
-  <div class="col-md-4 col-sm-12" itemprop="provider" itemscope itemtype="https://schema.org/Organization">
+  <div class="col-md-4 col-sm-12">
     <div class="card fluid">
       <div class="section dark">
        <b>Provider</b>
       </div>
       <div class="section">
-        <b itemprop="name">{{ config['metadata']['provider']['name'] }}</b><br/>
-        <a itemprop="url" href="{{ config['metadata']['provider']['url'] }}">{{ config['metadata']['provider']['url'] }}</a><br/>
+        <b>{{ config['metadata']['provider']['name'] }}</b><br/>
+        <a href="{{ config['metadata']['provider']['url'] }}">{{ config['metadata']['provider']['url'] }}</a><br/>
       </div>
     </div>
     <div class="card fluid">
       <div class="section dark">
           <b>Contact point</b>
       </div>
       <div class="section">
         <b>Address</b><br/>
-        <div class="section" itemprop="address" itemscope itemtype="https://schema.org/PostalAddress">
-          <span itemprop="streetAddress">{{ config['metadata']['contact']['address'] }}</span><br/>
-          <span itemprop="addressLocality">{{ config['metadata']['contact']['city'] }}</span>,
-          <span itemprop="addressRegion">{{ config['metadata']['contact']['stateorprovince'] }}</span><br/>
-          <span itemprop="postalCode">{{ config['metadata']['contact']['postalcode'] }}</span><br/>
-          <span itemprop="addressCountry">{{ config['metadata']['contact']['country'] }}</span>
+        <div class="section">
+          <span>{{ config['metadata']['contact']['address'] }}</span><br/>
+          <span>{{ config['metadata']['contact']['city'] }}</span>,
+          <span>{{ config['metadata']['contact']['stateorprovince'] }}</span><br/>
+          <span>{{ config['metadata']['contact']['postalcode'] }}</span><br/>
+          <span>{{ config['metadata']['contact']['country'] }}</span>
         </div>
-        <div itemprop="contactPoint" itemscope itemtype="https://schema.org/ContactPoint">
+        <div>
           <b>Email</b><br/>
-          <span itemprop="Email"><a href="mailto:{{ config['metadata']['contact']['email'] }}">{{ config['metadata']['contact']['email'] }}</a></span><br/>
+          <span><a href="mailto:{{ config['metadata']['contact']['email'] }}">{{ config['metadata']['contact']['email'] }}</a></span><br/>
           {% if config['metadata']['contact']['phone'] %}
             <b>Telephone</b><br/>
-            <span itemprop="Telephone"><a href="tel:{{ config['metadata']['contact']['phone'] }}">{{ config['metadata']['contact']['phone'] }}</a></span><br/>
+            <span><a href="tel:{{ config['metadata']['contact']['phone'] }}">{{ config['metadata']['contact']['phone'] }}</a></span><br/>
           {% endif %}
           {% if config['metadata']['contact']['fax'] %}
             <b>Fax</b><br/>
-            <span itemprop="faxNumber"><a href="tel:{{ config['metadata']['contact']['fax'] }}">{{ config['metadata']['contact']['fax'] }}</a></span><br/>
+            <span><a href="tel:{{ config['metadata']['contact']['fax'] }}">{{ config['metadata']['contact']['fax'] }}</a></span><br/>
           {% endif %}
           {% if config['metadata']['contact']['url'] %}
             <b>Contact URL</b><br/>
-            <span itemprop="url"><a href="{{ config['metadata']['contact']['url'] }}">{{ config['metadata']['contact']['url'] }}</a></span><br/>
+            <span><a href="{{ config['metadata']['contact']['url'] }}">{{ config['metadata']['contact']['url'] }}</a></span><br/>
           {% endif %}
           {% if config['metadata']['contact']['hours'] %}
             <b>Hours</b><br/>
-            <span itemprop="hoursAvailable">{{ config['metadata']['contact']['hours'] }}</span><br/>
+            <span>{{ config['metadata']['contact']['hours'] }}</span><br/>
           {% endif %}
           {% if config['metadata']['contact']['instructions'] %}
             <b>Contact instructions</b><br/>
-            <span itemprop="contactType">{{ config['metadata']['contact']['instructions'] }}</span>
+            <span>{{ config['metadata']['contact']['instructions'] }}</span>
           {% endif %}
         </div>
       </div>
     </div>
   </div>
 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% extends "base.html" %} {% block title %}{{ super() }} Home {% endblock %} {%
 block body %}
-
 ****** {{ config['metadata']['identification']['title'] }} ******
 {{ config['metadata']['identification']['description'] }}
 {% for kw in config['metadata']['identification']['keywords'] %} {{ kw }} {%
 endfor %}
 {% if config['metadata']['identification']['terms_of_service'] %}
 Terms of service
 {{ config['metadata']['identification']['terms_of_service'] | urlize() }}
@@ -12,21 +11,21 @@
 License
 {{_config['metadata']['license']['name']_or_config['metadata']['license']
 ['url']_}}
 {% endif %}
 
 ***** Collections *****
 View_the_collections_in_this_service
-
+ {% if data['stac'] %}
 ***** SpatioTemporal Assets *****
 View_the_SpatioTemporal_Assets_in_this_service
-
+ {% endif %} {% if data['processes'] %}
 ***** Processes *****
 View_the_processes_in_this_service
-
+ {% endif %}
 ***** API Definition *****
 Documentation
 OpenAPI_Document
 
 ***** Conformance *****
 View_the_conformance_classes_of_this_service
 Provider
```

### Comparing `pygeoapi-0.8.0/pygeoapi/templates/stac/catalog.html` & `pygeoapi-0.9.0/pygeoapi/templates/stac/catalog.html`

 * *Files 23% similar despite different names*

```diff
@@ -16,19 +16,18 @@
         <tr>
           <th>Name</th>
         </tr>
       </thead>
       <tbody>
         {% for link in data['links'] %}
         {% if link['type'] == 'text/html' and link['rel'] in ['child', 'item'] %}
-        <tr itemprop="dataset" itemscope itemtype="https://schema.org/Dataset">
+        <tr>
           <td data-label="name">
-            <meta itemprop="url" content="{{ link['href'] }}"/>
             <a title="{{ link['href'] }}" href="{{ link['href'] }}">
-             <span itemprop="name">{{ link['href'] | get_path_basename }}</span></a>
+             <span>{{ link['href'] | get_path_basename }}</span></a>
           </td>
         </tr>
         {% endif %}
         {% endfor %}
       </tbody>
     </table>
   </section>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% extends "base.html" %} {% block title %}{{ super() }} stac/{{ data['path']
 }} {% endblock %} {% block crumbs %}{{ super() }} / SpatioTemporal_Asset
 Catalog {% for link in get_breadcrumbs(data['path']) %} / {{_link['title']_}}
 {% endfor %} {% endblock %} {% block body %}
 ***** Links *****
 Name
- {{_link['href']_|_get_path_basename_}}
+{{_link['href']_|_get_path_basename_}}
  {% endblock %}
```

### Comparing `pygeoapi-0.8.0/pygeoapi/templates/stac/item.html` & `pygeoapi-0.9.0/pygeoapi/templates/stac/item.html`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,18 @@
                   <thead>
                     <tr>
                       <th>URL</th>
                     </tr>
                   </thead>
                   <tbody>
                   {% for k, link in data['assets'].items() %}
-                  <tr itemprop="dataset" itemscope itemtype="https://schema.org/Dataset">
+                  <tr>
                     <td data-label="name">
-                      <meta itemprop="url" content="{{ link['href'] }}"/>
                       <a title="{{ link['href'] }}" href="{{ link['href'] }}">
-                      <span itemprop="name">{{ link['href'] | get_path_basename }}</span></a>
+                      <span>{{ link['href'] | get_path_basename }}</span></a>
                     </td>
                   </tr>
                   {% endfor %}
                   </tbody>
                 </table>
               </div>
             </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 }} {% endblock %} {% block crumbs %}{{ super() }} / SpatioTemporal_Asset
 Catalog {% for link in get_breadcrumbs(data['path']) %} / {{_link['title']_}}
 {% endfor %} {% endblock %} {% block extrahead %}
  {% endblock %} {% block body %}
 ***** Item {{ data['id'] }} *****
 *** Assets ***
 URL
- {{_link['href']_|_get_path_basename_}}
+{{_link['href']_|_get_path_basename_}}
 Property Value
 id       {{ data.id }}
              * {% for l in v %}
 {{ k }}      * {{_l['title']_}} {{ v }}
              * {% endfor %}
  {% endblock %} {% block extrafoot %}
  {% endblock %}
```

### Comparing `pygeoapi-0.8.0/pygeoapi.egg-info/PKG-INFO` & `pygeoapi-0.9.0/pygeoapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pygeoapi
-Version: 0.8.0
+Version: 0.9.0
 Summary: pygeoapi provides an API to geospatial data
 Home-page: https://pygeoapi.io
 Author: Tom Kralidis
 Author-email: tomkralidis@gmail.com
 Maintainer: Tom Kralidis
 Maintainer-email: tomkralidis@gmail.com
 License: MIT
 Description: # pygeoapi
         
         [![Build Status](https://travis-ci.org/geopython/pygeoapi.png)](https://travis-ci.org/geopython/pygeoapi)
         <a href="https://json-ld.org"><img src="https://json-ld.org/images/json-ld-button-88.png" height="20"/></a>
         
-        [pygeoapi](https://pygeoapi.io) is a Python server implementation of the [OGC API](http://ogcapi.org) suite of standards. The project emerged as part of the next generation OGC API efforts in 2018 and provides the capability for organizations to deploy a RESTful OGC API endpoint using OpenAPI, GeoJSON, and HTML. pygeoapi is [open source](https://opensource.org/) and released under an [MIT license](https://github.com/geopython/pygeoapi/blob/master/LICENSE.md).
+        [pygeoapi](https://pygeoapi.io) is a Python server implementation of the [OGC API](https://ogcapi.ogc.org) suite of standards. The project emerged as part of the next generation OGC API efforts in 2018 and provides the capability for organizations to deploy a RESTful OGC API endpoint using OpenAPI, GeoJSON, and HTML. pygeoapi is [open source](https://opensource.org/) and released under an [MIT license](https://github.com/geopython/pygeoapi/blob/master/LICENSE.md).
         
         Please read the docs at [https://docs.pygeoapi.io](https://docs.pygeoapi.io) for more information.
 Keywords: geospatial data api
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: pygeoapi Version: 0.8.0 Summary: pygeoapi provides
+Metadata-Version: 2.1 Name: pygeoapi Version: 0.9.0 Summary: pygeoapi provides
 an API to geospatial data Home-page: https://pygeoapi.io Author: Tom Kralidis
 Author-email: tomkralidis@gmail.com Maintainer: Tom Kralidis Maintainer-email:
 tomkralidis@gmail.com License: MIT Description: # pygeoapi [![Build Status]
 (https://travis-ci.org/geopython/pygeoapi.png)](https://travis-ci.org/
 geopython/pygeoapi) [https://json-ld.org/images/json-ld-button-88.png]
 [pygeoapi](https://pygeoapi.io) is a Python server implementation of the [OGC
-API](http://ogcapi.org) suite of standards. The project emerged as part of the
-next generation OGC API efforts in 2018 and provides the capability for
+API](https://ogcapi.ogc.org) suite of standards. The project emerged as part of
+the next generation OGC API efforts in 2018 and provides the capability for
 organizations to deploy a RESTful OGC API endpoint using OpenAPI, GeoJSON, and
 HTML. pygeoapi is [open source](https://opensource.org/) and released under an
 [MIT license](https://github.com/geopython/pygeoapi/blob/master/LICENSE.md).
 Please read the docs at [https://docs.pygeoapi.io](https://docs.pygeoapi.io)
 for more information. Keywords: geospatial data api Platform: all Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
```

### Comparing `pygeoapi-0.8.0/pygeoapi.egg-info/SOURCES.txt` & `pygeoapi-0.9.0/pygeoapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,28 +27,36 @@
 pygeoapi/provider/__init__.py
 pygeoapi/provider/base.py
 pygeoapi/provider/csv_.py
 pygeoapi/provider/elasticsearch_.py
 pygeoapi/provider/filesystem.py
 pygeoapi/provider/geojson.py
 pygeoapi/provider/mongo.py
+pygeoapi/provider/mvt.py
 pygeoapi/provider/ogr.py
 pygeoapi/provider/postgresql.py
+pygeoapi/provider/rasterio_.py
 pygeoapi/provider/sqlite.py
+pygeoapi/provider/tile.py
+pygeoapi/provider/xarray_.py
 pygeoapi/static/css/default.css
 pygeoapi/static/img/favicon.ico
 pygeoapi/static/img/logo.png
 pygeoapi/static/img/pygeoapi.png
 pygeoapi/templates/base.html
 pygeoapi/templates/collection.html
 pygeoapi/templates/collections.html
 pygeoapi/templates/conformance.html
+pygeoapi/templates/domainset.html
 pygeoapi/templates/item.html
 pygeoapi/templates/items.html
+pygeoapi/templates/landing_page.html
 pygeoapi/templates/openapi.html
 pygeoapi/templates/process.html
 pygeoapi/templates/processes.html
 pygeoapi/templates/queryables.html
-pygeoapi/templates/root.html
+pygeoapi/templates/rangetype.html
+pygeoapi/templates/tiles.html
+pygeoapi/templates/tiles_metadata.html
 pygeoapi/templates/stac/catalog.html
 pygeoapi/templates/stac/item.html
 pygeoapi/templates/stac/root.html
```

### Comparing `pygeoapi-0.8.0/setup.py` & `pygeoapi-0.9.0/setup.py`

 * *Files identical despite different names*

