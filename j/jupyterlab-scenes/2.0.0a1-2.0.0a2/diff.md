# Comparing `tmp/jupyterlab_scenes-2.0.0a1.tar.gz` & `tmp/jupyterlab_scenes-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_scenes-2.0.0a1.tar", last modified: Tue Feb 21 22:42:02 2023, max compression
+gzip compressed data, was "jupyterlab_scenes-2.0.0a2.tar", last modified: Mon Feb 27 21:53:04 2023, max compression
```

## Comparing `jupyterlab_scenes-2.0.0a1.tar` & `jupyterlab_scenes-2.0.0a2.tar`

### file list

```diff
@@ -1,57 +1,81 @@
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       86 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/CHANGELOG.md
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     1522 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/LICENSE
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      424 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/MANIFEST.in
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2473 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/PKG-INFO
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     1409 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/README.md
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     1901 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/RELEASE.md
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      195 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/install.json
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.860740 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      319 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/__init__.py
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      625 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/_version.py
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.860740 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    20337 2023-02-21 22:28:46.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/build_log.json
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2945 2023-02-21 22:28:47.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/package.json
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.860740 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/schemas/
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/schemas/jupyterlab_scenes/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2803 2023-02-21 22:28:46.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/schemas/jupyterlab_scenes/package.json.orig
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      388 2023-02-21 22:28:46.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/schemas/jupyterlab_scenes/plugin.json
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49328 2023-02-21 22:28:47.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/lib_index_js.ee4dbc9980b7e689c6f6.js
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    43751 2023-02-21 22:28:47.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/lib_index_js.ee4dbc9980b7e689c6f6.js.map
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    29569 2023-02-21 22:28:47.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/remoteEntry.ec56600e3e74782839f0.js
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-21 22:28:47.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/remoteEntry.ec56600e3e74782839f0.js.map
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      160 2023-02-21 22:28:46.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/style.js
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28243 2023-02-21 22:28:47.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/style_index_js.af8725b98d07f334206d.js
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    26647 2023-02-21 22:28:47.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/style_index_js.af8725b98d07f334206d.js.map
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.860740 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes.egg-info/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2473 2023-02-21 22:42:02.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes.egg-info/PKG-INFO
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     1431 2023-02-21 22:42:02.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes.egg-info/SOURCES.txt
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)        1 2023-02-21 22:42:02.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes.egg-info/dependency_links.txt
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)        1 2022-08-22 14:44:18.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes.egg-info/not-zip-safe
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       21 2023-02-21 22:42:02.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes.egg-info/requires.txt
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       18 2023-02-21 22:42:02.000000 jupyterlab_scenes-2.0.0a1/jupyterlab_scenes.egg-info/top_level.txt
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2803 2023-02-21 22:30:02.000000 jupyterlab_scenes-2.0.0a1/package.json
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      603 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/pyproject.toml
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/schema/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      388 2023-02-21 22:15:50.000000 jupyterlab_scenes-2.0.0a1/schema/plugin.json
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       38 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/setup.cfg
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2918 2023-02-21 22:41:32.000000 jupyterlab_scenes-2.0.0a1/setup.py
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/src/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    20773 2023-02-21 22:18:26.000000 jupyterlab_scenes-2.0.0a1/src/backend.ts
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     7208 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/src/components.tsx
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      939 2023-02-21 21:52:37.000000 jupyterlab_scenes-2.0.0a1/src/index.ts
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       87 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/src/svg.d.ts
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    10011 2023-02-21 21:52:36.000000 jupyterlab_scenes-2.0.0a1/src/widget.tsx
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/style/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     3720 2022-08-22 16:32:51.000000 jupyterlab_scenes-2.0.0a1/style/base.css
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       25 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/style/index.css
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       21 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/style/index.js
-drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-21 22:42:02.864740 jupyterlab_scenes-2.0.0a1/style/svg/
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      325 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/style/svg/arrowDown.svg
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      326 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/style/svg/arrowUp.svg
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      385 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/style/svg/cellDown.svg
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      387 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/style/svg/cellUp.svg
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      307 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a1/style/svg/scenesLogo.svg
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      554 2023-02-20 21:35:13.000000 jupyterlab_scenes-2.0.0a1/tsconfig.json
--rw-rw-r--   0 schmidi   (1000) schmidi   (1000)   186123 2023-02-21 22:30:02.000000 jupyterlab_scenes-2.0.0a1/yarn.lock
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.053955 jupyterlab_scenes-2.0.0a2/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       86 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/CHANGELOG.md
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     1522 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/LICENSE
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      424 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/MANIFEST.in
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2840 2023-02-27 21:53:04.053955 jupyterlab_scenes-2.0.0a2/PKG-INFO
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     1776 2023-02-27 19:18:12.000000 jupyterlab_scenes-2.0.0a2/README.md
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     1901 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/RELEASE.md
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      195 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/install.json
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.049955 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      319 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/__init__.py
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      625 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/_version.py
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.049955 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    20338 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/build_log.json
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2945 2023-02-27 19:30:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/package.json
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.049955 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/schemas/
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.049955 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/schemas/jupyterlab_scenes/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2803 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/schemas/jupyterlab_scenes/package.json.orig
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      388 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/schemas/jupyterlab_scenes/plugin.json
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.053955 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49909 2023-02-27 18:52:22.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.0aa35e0458ae63cde8ee.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    44413 2023-02-27 18:52:22.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.0aa35e0458ae63cde8ee.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49505 2023-02-23 21:25:07.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.464c8e8f3b11e19e4131.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    43955 2023-02-23 21:25:07.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.464c8e8f3b11e19e4131.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49731 2023-02-27 18:31:48.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.78369b03b66fdbe5eac3.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    44224 2023-02-27 18:31:48.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.78369b03b66fdbe5eac3.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49401 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.96021e5ad2af4f2e5eba.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    43839 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.96021e5ad2af4f2e5eba.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49752 2023-02-23 21:41:11.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.96d057f53bf6361735d7.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    44226 2023-02-23 21:41:11.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.96d057f53bf6361735d7.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49682 2023-02-23 21:37:49.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.a4e6c74e170d0f4c67ca.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    44150 2023-02-23 21:37:49.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.a4e6c74e170d0f4c67ca.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49575 2023-02-23 21:42:31.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.dbc5e6bf4d36e92df0a4.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    44031 2023-02-23 21:42:31.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.dbc5e6bf4d36e92df0a4.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    50065 2023-02-27 18:46:32.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.f465585239b61c842ee4.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    44606 2023-02-27 18:46:32.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.f465585239b61c842ee4.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    49607 2023-02-23 21:32:16.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.fe968cb4f1e9e644c518.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    44069 2023-02-23 21:32:16.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.fe968cb4f1e9e644c518.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-23 21:25:07.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.080c207a518f60ccdd6f.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-23 21:37:49.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.2cbe9eadc8c75dd93db6.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-23 21:41:11.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.2f951cd84781e8cbc7cc.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.5c3d93e2489ccdb015f2.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-27 18:46:32.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.6cdd85bef6a183b66628.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    29569 2023-02-27 18:52:22.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.9fa23aea731399224cde.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-27 18:52:22.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.9fa23aea731399224cde.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-23 21:32:16.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.a6c424642a6232f9b8ec.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-23 21:42:31.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.d5385516e4e68c4923d2.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28394 2023-02-27 18:31:48.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.f17efb85ce84c5f7f976.js.map
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      160 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/style.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    28243 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/style_index_js.af8725b98d07f334206d.js
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    26647 2023-02-23 21:12:17.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/style_index_js.af8725b98d07f334206d.js.map
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.049955 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes.egg-info/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2840 2023-02-27 21:53:04.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes.egg-info/PKG-INFO
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     3287 2023-02-27 21:53:04.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes.egg-info/SOURCES.txt
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)        1 2023-02-27 21:53:04.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes.egg-info/dependency_links.txt
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)        1 2022-08-22 14:44:18.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes.egg-info/not-zip-safe
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       21 2023-02-27 21:53:04.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes.egg-info/requires.txt
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       18 2023-02-27 21:53:04.000000 jupyterlab_scenes-2.0.0a2/jupyterlab_scenes.egg-info/top_level.txt
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2803 2023-02-27 19:30:16.000000 jupyterlab_scenes-2.0.0a2/package.json
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      603 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/pyproject.toml
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.053955 jupyterlab_scenes-2.0.0a2/schema/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      388 2023-02-21 22:15:50.000000 jupyterlab_scenes-2.0.0a2/schema/plugin.json
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       38 2023-02-27 21:53:04.053955 jupyterlab_scenes-2.0.0a2/setup.cfg
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     2918 2023-02-21 22:41:32.000000 jupyterlab_scenes-2.0.0a2/setup.py
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.053955 jupyterlab_scenes-2.0.0a2/src/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    21005 2023-02-27 18:46:32.000000 jupyterlab_scenes-2.0.0a2/src/backend.ts
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     7208 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/src/components.tsx
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      939 2023-02-21 21:52:37.000000 jupyterlab_scenes-2.0.0a2/src/index.ts
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       87 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/src/svg.d.ts
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)    10347 2023-02-27 18:52:18.000000 jupyterlab_scenes-2.0.0a2/src/widget.tsx
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.053955 jupyterlab_scenes-2.0.0a2/style/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)     3720 2022-08-22 16:32:51.000000 jupyterlab_scenes-2.0.0a2/style/base.css
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       25 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/style/index.css
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)       21 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/style/index.js
+drwxrwxr-x   0 schmidi   (1000) schmidi   (1000)        0 2023-02-27 21:53:04.053955 jupyterlab_scenes-2.0.0a2/style/svg/
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      325 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/style/svg/arrowDown.svg
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      326 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/style/svg/arrowUp.svg
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      385 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/style/svg/cellDown.svg
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      387 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/style/svg/cellUp.svg
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      307 2022-08-22 14:38:07.000000 jupyterlab_scenes-2.0.0a2/style/svg/scenesLogo.svg
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)      554 2023-02-20 21:35:13.000000 jupyterlab_scenes-2.0.0a2/tsconfig.json
+-rw-rw-r--   0 schmidi   (1000) schmidi   (1000)   186123 2023-02-21 22:30:02.000000 jupyterlab_scenes-2.0.0a2/yarn.lock
```

### Comparing `jupyterlab_scenes-2.0.0a1/LICENSE` & `jupyterlab_scenes-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/PKG-INFO` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyterlab_scenes
-Version: 2.0.0a1
+Name: jupyterlab-scenes
+Version: 2.0.0a2
 Summary: Define subsets of code cells as scenes and execute them.
 Home-page: https://github.com/schmidi314/jupyterlab_scenes
 Author: Manuel Schmidt
 Author-email: Manuel.J.Schmidt@t-online.de
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
@@ -45,17 +45,25 @@
 * By clicking the `init` button, one scene can be chosen to be automatically executed as the kernel becomes ready (due to a restart or at the initial loading of the notebook).
 * If a notebook with an already running kernel is opened, the init scene is __not__ executed.
 * Only one scene can be an init scene.
 
 ![Initialization](https://github.com/schmidi314/jupyterlab-scenes/blob/master/gifs/scenes_init.gif?raw=true)
 
 
+* To run a scene named `My Favourite Scene` programatically, do
+    ```
+    from ipylab import JupyterFrontEnd
+    JupyterFrontEnd().commands.execute('scenes:run-scene', 'My Favourite Scene')
+    ```
+    But you may run only one scene at a time. No excessive looping as the scenes are executed only after the cell that launches the `run-scene` command is finished.
+
+
 ## Requirements
 
-* JupyterLab >= 3.0
+* JupyterLab >= 4.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab_scenes
```

### Comparing `jupyterlab_scenes-2.0.0a1/README.md` & `jupyterlab_scenes-2.0.0a2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,25 @@
 * By clicking the `init` button, one scene can be chosen to be automatically executed as the kernel becomes ready (due to a restart or at the initial loading of the notebook).
 * If a notebook with an already running kernel is opened, the init scene is __not__ executed.
 * Only one scene can be an init scene.
 
 ![Initialization](https://github.com/schmidi314/jupyterlab-scenes/blob/master/gifs/scenes_init.gif?raw=true)
 
 
+* To run a scene named `My Favourite Scene` programatically, do
+    ```
+    from ipylab import JupyterFrontEnd
+    JupyterFrontEnd().commands.execute('scenes:run-scene', 'My Favourite Scene')
+    ```
+    But you may run only one scene at a time. No excessive looping as the scenes are executed only after the cell that launches the `run-scene` command is finished.
+
+
 ## Requirements
 
-* JupyterLab >= 3.0
+* JupyterLab >= 4.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab_scenes
```

### Comparing `jupyterlab_scenes-2.0.0a1/RELEASE.md` & `jupyterlab_scenes-2.0.0a2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/_version.py` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/build_log.json` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {'0': "{'bail': False}"}*

```diff
@@ -1,10 +1,10 @@
 [
     {
-        "bail": true,
+        "bail": false,
         "devtool": "source-map",
         "entry": {},
         "mode": "development",
         "module": {
             "rules": [
                 {
                     "test": "/\\.css$/",
```

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/package.json` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995039682539681%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9fa23aea731399224cde.js'}}"}*

```diff
@@ -40,15 +40,15 @@
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ec56600e3e74782839f0.js",
+            "load": "static/remoteEntry.9fa23aea731399224cde.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_scenes/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
```

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/schemas/jupyterlab_scenes/package.json.orig` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/schemas/jupyterlab_scenes/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/lib_index_js.ee4dbc9980b7e689c6f6.js` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.464c8e8f3b11e19e4131.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -215,22 +215,24 @@
                     }
                     createNewEmptyScene(scene_name) {
                         const scene_list = this.getScenesList();
                         if (scene_list.includes(scene_name))
                             return 'fail';
                         scene_list.push(scene_name);
                         this._sceneDB.setScenesList(scene_list);
+                        this._sceneDB.setActiveScene(scene_name);
                         this._scenesChanged();
                         return 'success';
                     }
                     duplicateActiveScene(new_scene_name) {
                         let retval = this.createNewEmptyScene(new_scene_name);
                         if (retval == 'fail')
                             return 'fail';
                         this._duplicateSceneTagInAllCells(this._nbTracker.currentWidget, this.getActiveScene(), new_scene_name);
+                        this._sceneDB.setActiveScene(new_scene_name);
                         this._scenesChanged();
                         return retval;
                     }
                     moveActiveSceneUp() {
                         this._moveScene(this._sceneDB.getActiveScene(), 'up');
                         this._scenesChanged();
                     }
@@ -351,16 +353,19 @@
                                 cell.model.setMetadata('init_cell', true);
                             } else {
                                 cell.model.deleteMetadata('init_cell');
                             }
                         });
                     }
                     _activateCellAndExpandParentHeadings(cell) {
-                        _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__.NotebookActions.expandParent(cell, this._nbTracker.currentWidget.content);
-                        cell.activate();
+                        let notebook = this._nbTracker.currentWidget.content;
+                        _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__.NotebookActions.expandParent(cell, notebook);
+                        notebook.scrollToCell(cell).then(() => {
+                            notebook.activeCellIndex = notebook.widgets.indexOf(cell);
+                        });
                     }
                     _moveScene(scene_name, direction) {
                         const scenes_list = this.getScenesList();
                         let idx = scenes_list.indexOf(scene_name);
                         if (direction == 'down') {
                             if (idx == scenes_list.length - 1)
                                 return;
@@ -498,15 +503,14 @@
                         }
                         let data_json = model.getMetadata(NB_METADATA_KEY);
                         let retval = {
                             scenes: data_json['scenes'],
                             active_scene: data_json['active_scene'],
                             init_scene: data_json['init_scene']
                         };
-                        console.log('got scene data', retval);
                         return retval;
                     }
                     _setSceneData(scene_data) {
                         var _a;
                         let notebook_model = (_a = this._nbTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.model;
                         if (!notebook_model)
                             return;
@@ -1151,8 +1155,8 @@
                 module.exports = "<svg xmlns=\"http://www.w3.org/2000/svg\" width=\"24\" height=\"24\" viewBox=\"0 0 24 24\">\n    <g class=\"jp-icon3\" fill=\"#616161\">\n         <path transform=\"matrix(1,0,0,1.2,0,-2.9)\" d=\"M 13.1 5.3 v 14 l 11 -7 z\"/>\n    </g>\n <ellipse rx=\"6.5\" ry=\"6.4\"\n     fill=\"#771e90\"\n     cx=\"6.4\"\n     cy=\"12\"\n     />\n</svg>\n";
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.ee4dbc9980b7e689c6f6.js.map
+//# sourceMappingURL=lib_index_js.464c8e8f3b11e19e4131.js.map
```

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/lib_index_js.ee4dbc9980b7e689c6f6.js.map` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/lib_index_js.464c8e8f3b11e19e4131.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8285714285714285%*

 * *Differences: {"'file'": "'lib_index_js.464c8e8f3b11e19e4131.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;;;AAAuD;AACV;AACG;AACL;AAC3C;AACA;AACO;AACP;AACA,iCAAiC,qDAAM;AACvC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD,gCAAgC;AACjF,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uHAAuH,0CAA0C;AACjK,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AA […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "file": "lib_index_js.ee4dbc9980b7e689c6f6.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;;;;AAAuD;AACV;AACG;AACL;AAC3C;AACA;AACO;AACP;AACA,iCAAiC,qDAAM;AACvC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD,gCAAgC;AACjF,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uHAAuH,0CAA0C;AACjK,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,+DAAgB,uCAAuC,iEAAiE;AAC5I;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,cAAc;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,QAAQ;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,QAAQ,8EAA4B;AACpC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe;AACf;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,mEAAgB;AAC/B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD,0EAA0E;AAC3H;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;AC/d+B;AAC6D;AACxC;AACX;AACI;AACI;AACF;AACI;AACnD,uBAAuB,8DAAO,GAAG,wBAAwB,kDAAM,EAAE;AACjE,yBAAyB,8DAAO,GAAG,0BAA0B,oDAAQ,EAAE;AACvE,wBAAwB,8DAAO,GAAG,yBAAyB,mDAAO,EAAE;AACpE,0BAA0B,8DAAO,GAAG,2BAA2B,qDAAS,EAAE;AACnE,4BAA4B,4CAAe;AAClD;AACA,gBAAgB,gDAAmB,UAAU,mCAAmC;AAChF,YAAY,gDAAmB,UAAU,4BAA4B;AACrE;AACA;AACA,YAAY,gDAAmB,YAAY,+BAA+B;AAC1E,YAAY,gDAAmB,eAAe,+KAA+K;AAC7N;AACA;AACA,yBAAyB,4CAAe;AACxC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4CAA4C,0EAAqC,IAAI,0BAA0B;AAC/G;AACA;AACA;AACA;AACA,4CAA4C,0EAAqC,IAAI,0BAA0B;AAC/G;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,gDAAmB,UAAU,iEAAiE;AAClH,gBAAgB,gDAAmB,aAAa,+EAA+E;AAC/H,oBAAoB,gDAAmB,CAAC,sEAAe,IAAI,mEAAmE;AAC9H,gBAAgB,gDAAmB,aAAa,yEAAyE;AACzH,oBAAoB,gDAAmB,CAAC,oEAAa,IAAI,mEAAmE;AAC5H,gBAAgB,gDAAmB,aAAa,6EAA6E;AAC7H,oBAAoB,gDAAmB,CAAC,qEAAc,IAAI,mEAAmE;AAC7H,gBAAgB,gDAAmB,UAAU,8BAA8B;AAC3E,gBAAgB,gDAAmB,UAAU,qCAAqC;AAClF,gBAAgB,gDAAmB,aAAa,sDAAsD;AACtG,SAAS;AACT,gBAAgB,gDAAmB,UAAU,+BAA+B;AAC5E;AACA;AACA,sBAAsB,4CAAe;AACrC;AACA;AACA,wCAAwC,6EAAwC;AAChF;AACA;AACA,wCAAwC,6EAAwC;AAChF;AACA;AACA,wCAAwC,kFAA6C;AACrF;AACA;AACA,wCAAwC,oFAA+C;AACvF;AACA;AACA,wCAAwC,gFAA2C;AACnF;AACA;AACA,wCAAwC,oFAA+C;AACvF;AACA,gBAAgB,gDAAmB,UAAU,6BAA6B;AAC1E,YAAY,gDAAmB,aAAa,kFAAkF;AAC9H,gBAAgB,gDAAmB,CAAC,oEAAa,IAAI,mEAAmE;AACxH,YAAY,gDAAmB,aAAa,+FAA+F;AAC3I,gBAAgB,gDAAmB,CAAC,qEAAc,IAAI,mEAAmE;AACzH,YAAY,gDAAmB,aAAa,sFAAsF;AAClI,gBAAgB,gDAAmB,sBAAsB,mEAAmE;AAC5H,YAAY,gDAAmB,aAAa,0FAA0F;AACtI,gBAAgB,gDAAmB,wBAAwB,mEAAmE;AAC9H,YAAY,gDAAmB,UAAU,qCAAqC;AAC9E,YAAY,gDAAmB,aAAa,2FAA2F;AACvI,gBAAgB,gDAAmB,uBAAuB,mEAAmE;AAC7H,YAAY,gDAAmB,aAAa,+FAA+F;AAC3I,gBAAgB,gDAAmB,qBAAqB,mEAAmE;AAC3H;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACtGoD;AACW;AACP;AACP;AACR;AACzC;AACA;AACA,8BAA8B,kDAAa;AAC3C,2CAA2C,YAAY;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,yEAAgB,EAAE,kEAAgB,EAAE,2DAAS,EAAE,8DAAS;AACvE;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;;ACnBiB;AACmD;AACtC;AAC1B;AACmB;AACD;AACS;AACrD,uBAAuB,8DAAO,GAAG,wBAAwB,sDAAU,EAAE;AACrE,4BAA4B,6DAAW;AACvC;AACA;AACA;AACA;AACA;AACA;AACA,oCAAoC,qDAAe;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT,4DAA4D,gBAAgB;AAC5E;AACA;AACA;AACA;AACA,oBAAoB,0DAAmB;AACvC,gBAAgB,0DAAmB,CAAC,sDAAa,IAAI,+OAA+O;AACpS;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA;AACA,gBAAgB,qEAAmB,GAAG,iCAAiC;AACvE;AACA;AACA;AACA,wBAAwB,sEAAgB;AACxC;AACA,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA;AACA,gBAAgB,qEAAmB,GAAG,wCAAwC;AAC9E;AACA;AACA;AACA,wBAAwB,sEAAgB;AACxC;AACA,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA;AACA;AACA,0CAA0C,wDAAM;AAChD;AACA,8BAA8B,qEAAmB,IAAI,iEAAe,GAAG,iBAAiB;AACxF,iBAAiB;AACjB;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA,gBAAgB,qEAAmB,GAAG,kDAAkD;AACxF;AACA;AACA;AACA,wBAAwB,sEAAgB;AACxC;AACA,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA;AACA;AACA,oBAAoB;AACpB;AACA;AACA,SAAS;AACT;AACA;AACA,oBAAoB;AACpB;AACA;AACA,SAAS;AACT;AACA;AACA,+BAA+B,iDAAI,GAAG,8BAA8B;AACpE;AACA,mCAAmC,qDAAqD;AACxF,mCAAmC,6CAA6C;AAChF,mCAAmC,mBAAmB;AACtD,mCAAmC,mDAAmD;AACtF,mCAAmC,mDAAmD;AACtF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACyB;AACzB",
+    "file": "lib_index_js.464c8e8f3b11e19e4131.js",
+    "mappings": ";;;;;;;;;;;;;;;;;;;;;AAAuD;AACV;AACG;AACL;AAC3C;AACA;AACO;AACP;AACA,iCAAiC,qDAAM;AACvC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD,gCAAgC;AACjF,aAAa;AACb;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uHAAuH,0CAA0C;AACjK,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,+DAAgB,uCAAuC,iEAAiE;AAC5I;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,cAAc;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kCAAkC,QAAQ;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA,QAAQ,8EAA4B;AACpC,iDAAiD,4DAA4D;AAC7G;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe;AACf;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,mEAAgB;AAC/B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iDAAiD,0EAA0E;AAC3H;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACje+B;AAC6D;AACxC;AACX;AACI;AACI;AACF;AACI;AACnD,uBAAuB,8DAAO,GAAG,wBAAwB,kDAAM,EAAE;AACjE,yBAAyB,8DAAO,GAAG,0BAA0B,oDAAQ,EAAE;AACvE,wBAAwB,8DAAO,GAAG,yBAAyB,mDAAO,EAAE;AACpE,0BAA0B,8DAAO,GAAG,2BAA2B,qDAAS,EAAE;AACnE,4BAA4B,4CAAe;AAClD;AACA,gBAAgB,gDAAmB,UAAU,mCAAmC;AAChF,YAAY,gDAAmB,UAAU,4BAA4B;AACrE;AACA;AACA,YAAY,gDAAmB,YAAY,+BAA+B;AAC1E,YAAY,gDAAmB,eAAe,+KAA+K;AAC7N;AACA;AACA,yBAAyB,4CAAe;AACxC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4CAA4C,0EAAqC,IAAI,0BAA0B;AAC/G;AACA;AACA;AACA;AACA,4CAA4C,0EAAqC,IAAI,0BAA0B;AAC/G;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,gDAAmB,UAAU,iEAAiE;AAClH,gBAAgB,gDAAmB,aAAa,+EAA+E;AAC/H,oBAAoB,gDAAmB,CAAC,sEAAe,IAAI,mEAAmE;AAC9H,gBAAgB,gDAAmB,aAAa,yEAAyE;AACzH,oBAAoB,gDAAmB,CAAC,oEAAa,IAAI,mEAAmE;AAC5H,gBAAgB,gDAAmB,aAAa,6EAA6E;AAC7H,oBAAoB,gDAAmB,CAAC,qEAAc,IAAI,mEAAmE;AAC7H,gBAAgB,gDAAmB,UAAU,8BAA8B;AAC3E,gBAAgB,gDAAmB,UAAU,qCAAqC;AAClF,gBAAgB,gDAAmB,aAAa,sDAAsD;AACtG,SAAS;AACT,gBAAgB,gDAAmB,UAAU,+BAA+B;AAC5E;AACA;AACA,sBAAsB,4CAAe;AACrC;AACA;AACA,wCAAwC,6EAAwC;AAChF;AACA;AACA,wCAAwC,6EAAwC;AAChF;AACA;AACA,wCAAwC,kFAA6C;AACrF;AACA;AACA,wCAAwC,oFAA+C;AACvF;AACA;AACA,wCAAwC,gFAA2C;AACnF;AACA;AACA,wCAAwC,oFAA+C;AACvF;AACA,gBAAgB,gDAAmB,UAAU,6BAA6B;AAC1E,YAAY,gDAAmB,aAAa,kFAAkF;AAC9H,gBAAgB,gDAAmB,CAAC,oEAAa,IAAI,mEAAmE;AACxH,YAAY,gDAAmB,aAAa,+FAA+F;AAC3I,gBAAgB,gDAAmB,CAAC,qEAAc,IAAI,mEAAmE;AACzH,YAAY,gDAAmB,aAAa,sFAAsF;AAClI,gBAAgB,gDAAmB,sBAAsB,mEAAmE;AAC5H,YAAY,gDAAmB,aAAa,0FAA0F;AACtI,gBAAgB,gDAAmB,wBAAwB,mEAAmE;AAC9H,YAAY,gDAAmB,UAAU,qCAAqC;AAC9E,YAAY,gDAAmB,aAAa,2FAA2F;AACvI,gBAAgB,gDAAmB,uBAAuB,mEAAmE;AAC7H,YAAY,gDAAmB,aAAa,+FAA+F;AAC3I,gBAAgB,gDAAmB,qBAAqB,mEAAmE;AAC3H;AACA;;;;;;;;;;;;;;;;;;;;;;;;ACtGoD;AACW;AACP;AACP;AACR;AACzC;AACA;AACA,8BAA8B,kDAAa;AAC3C,2CAA2C,YAAY;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,yEAAgB,EAAE,kEAAgB,EAAE,2DAAS,EAAE,8DAAS;AACvE;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;;ACnBiB;AACmD;AACtC;AAC1B;AACmB;AACD;AACS;AACrD,uBAAuB,8DAAO,GAAG,wBAAwB,sDAAU,EAAE;AACrE,4BAA4B,6DAAW;AACvC;AACA;AACA;AACA;AACA;AACA;AACA,oCAAoC,qDAAe;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT,4DAA4D,gBAAgB;AAC5E;AACA;AACA;AACA;AACA,oBAAoB,0DAAmB;AACvC,gBAAgB,0DAAmB,CAAC,sDAAa,IAAI,+OAA+O;AACpS;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA;AACA,gBAAgB,qEAAmB,GAAG,iCAAiC;AACvE;AACA;AACA;AACA,wBAAwB,sEAAgB;AACxC;AACA,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA;AACA,gBAAgB,qEAAmB,GAAG,wCAAwC;AAC9E;AACA;AACA;AACA,wBAAwB,sEAAgB;AACxC;AACA,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA;AACA;AACA,0CAA0C,wDAAM;AAChD;AACA,8BAA8B,qEAAmB,IAAI,iEAAe,GAAG,iBAAiB;AACxF,iBAAiB;AACjB;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA,gBAAgB,qEAAmB,GAAG,kDAAkD;AACxF;AACA;AACA;AACA,wBAAwB,sEAAgB;AACxC;AACA,iBAAiB;AACjB;AACA,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA,6BAA6B;AAC7B,SAAS;AACT;AACA;AACA;AACA;AACA,oBAAoB;AACpB;AACA;AACA,SAAS;AACT;AACA;AACA,oBAAoB;AACpB;AACA;AACA,SAAS;AACT;AACA;AACA,+BAA+B,iDAAI,GAAG,8BAA8B;AACpE;AACA,mCAAmC,qDAAqD;AACxF,mCAAmC,6CAA6C;AAChF,mCAAmC,mBAAmB;AACtD,mCAAmC,mDAAmD;AACtF,mCAAmC,mDAAmD;AACtF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACyB;AACzB",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_scenes/./lib/backend.js",
         "webpack://jupyterlab_scenes/./lib/components.js",
         "webpack://jupyterlab_scenes/./lib/index.js",
         "webpack://jupyterlab_scenes/./lib/widget.js"
     ],
     "sourcesContent": [
-        "import { NotebookActions } from '@jupyterlab/notebook';\nimport { CodeCell } from '@jupyterlab/cells';\nimport { PathExt } from '@jupyterlab/coreutils';\nimport { Signal } from '@lumino/signaling';\nconst NB_METADATA_KEY = 'scenes_data';\nconst SCENE_CELL_CLASS = 'scene-cell';\nexport class NotebookHandler {\n    constructor(nbTracker, settingRegistry) {\n        this.scenesChanged = new Signal(this);\n        /* ****************************************************************************************************************************************\n         * Handle kernel (re-)starts\n         * ****************************************************************************************************************************************/\n        this._kernelStatusDict = {};\n        this._nbTracker = nbTracker;\n        this._sceneDB = new NotebookSceneDatabase(nbTracker);\n        this._enableLegacyInits = false;\n        // load settings\n        if (settingRegistry) {\n            settingRegistry.load('jupyterlab_scenes:plugin').then(settings => {\n                this.updateSettings(settings);\n                settings.changed.connect(() => { this.updateSettings(settings); });\n            })\n                .catch(reason => {\n                console.error('Failed to load settings for jupyterlab_scenes.', reason);\n            });\n        }\n        this._setupKernelListener();\n    }\n    updateSettings(settings) {\n        this._enableLegacyInits = settings.composite.legacyInit;\n    }\n    _setupKernelListener() {\n        this._nbTracker.widgetAdded.connect(async (sender, nbPanel) => {\n            nbPanel.context.sessionContext.ready.then(() => {\n                this._kernelStatusDict[nbPanel.context.sessionContext.session.kernel.id] = 'connecting';\n                nbPanel.context.sessionContext.session.kernel.connectionStatusChanged.connect((kernel, conn_stat) => { this._kernelListener(kernel, conn_stat); });\n            });\n        });\n    }\n    _kernelListener(kernel, conn_stat) {\n        if (conn_stat == 'connecting') {\n            this._kernelStatusDict[kernel.id] = 'connecting';\n        }\n        else if (conn_stat == 'connected') {\n            if (this._kernelStatusDict[kernel.id] == 'connecting') {\n                let notebookPanelList = [];\n                this._nbTracker.forEach((nbPanel) => {\n                    if (nbPanel.context.sessionContext.session.kernel.id == kernel.id) {\n                        notebookPanelList.push(nbPanel);\n                    }\n                });\n                if (notebookPanelList.length > 0) {\n                    let init_scene = this._sceneDB.getInitScene();\n                    if (init_scene)\n                        this.runSceneInNotebook(notebookPanelList[0], init_scene);\n                }\n            }\n            delete this._kernelStatusDict[kernel.id];\n        }\n    }\n    /* ****************************************************************************************************************************************\n     * Functionality provided to the main widget\n     * ****************************************************************************************************************************************/\n    // **** simple scene getters *************************************************\n    getNotebookTitle() {\n        return this._sceneDB.getNotebookTitle();\n    }\n    getScenesList() {\n        return this._sceneDB.getScenesList();\n    }\n    getActiveScene(notebook = null) {\n        return this._sceneDB.getActiveScene(notebook);\n    }\n    getInitScene() {\n        return this._sceneDB.getInitScene();\n    }\n    // **** scene setters ********************************************************\n    toggleInitScene(scene_name) {\n        this._sceneDB.toggleInitScene(scene_name);\n        this._scenesChanged();\n    }\n    setActiveScene(scene_name) {\n        this._sceneDB.setActiveScene(scene_name);\n        this._scenesChanged();\n    }\n    renameScene(old_scene_name, new_scene_name) {\n        const scenes_list = this.getScenesList();\n        if (scenes_list.includes(new_scene_name))\n            return 'fail';\n        if (this._sceneDB.getInitScene() == old_scene_name) {\n            this._sceneDB.toggleInitScene(new_scene_name);\n        }\n        if (this._sceneDB.getActiveScene() == old_scene_name) {\n            this._sceneDB.setActiveScene(new_scene_name);\n        }\n        let idx = scenes_list.lastIndexOf(old_scene_name);\n        scenes_list[idx] = new_scene_name;\n        this._sceneDB.setScenesList(scenes_list);\n        this._renameSceneTagFromAllCells(this._nbTracker.currentWidget, old_scene_name, new_scene_name);\n        this._scenesChanged();\n        return 'success';\n    }\n    deleteScene(scene_name) {\n        let scenes_list = this._sceneDB.getScenesList();\n        if (scenes_list.length == 1)\n            return;\n        if (this._sceneDB.getInitScene() == scene_name) {\n            this._sceneDB.toggleInitScene(scene_name);\n        }\n        let resetActiveScene = this._sceneDB.getActiveScene() == scene_name;\n        this._removeSceneTagFromAllCells(this._nbTracker.currentWidget, scene_name);\n        let idx = scenes_list.lastIndexOf(scene_name);\n        scenes_list.splice(idx, 1);\n        this._sceneDB.setScenesList(scenes_list);\n        if (resetActiveScene) {\n            if (idx < scenes_list.length) {\n                this.setActiveScene(scenes_list[idx]);\n            }\n            else {\n                this.setActiveScene(scenes_list[idx - 1]);\n            }\n        }\n        this._scenesChanged();\n    }\n    toggleSceneMembershipOfSelectedCells() {\n        if (!this._nbTracker.currentWidget)\n            return;\n        if (!this._nbTracker.activeCell)\n            return;\n        const current_scene = this._sceneDB.getActiveScene();\n        const is_init_scene = current_scene == this.getInitScene();\n        const tag = 'scene__' + current_scene;\n        const notebook = this._nbTracker.currentWidget.content;\n        const set_membership = !this._nbTracker.activeCell.model.getMetadata(tag);\n        //const set_membership = !this._nbTracker.activeCell.model.getMetadata(tag);\n        notebook.widgets.forEach((cell) => {\n            if (!notebook.isSelectedOrActive(cell))\n                return;\n            if (cell.model.type != 'code')\n                return;\n            if (set_membership) {\n                cell.model.setMetadata(tag, true);\n                if (is_init_scene) {\n                    cell.model.setMetadata('init_cell', true);\n                }\n            }\n            else {\n                cell.model.deleteMetadata(tag);\n                if (is_init_scene) {\n                    cell.model.deleteMetadata('init_cell');\n                }\n            }\n            this._updateCellClassAndTags(cell, tag);\n        });\n    }\n    // **** scene management and running *****************************************\n    runActiveSceneInCurrentNotebook() {\n        const active_scene = this._sceneDB.getActiveScene();\n        if (active_scene)\n            this.runSceneInCurrentNotebook(active_scene);\n    }\n    runSceneInCurrentNotebook(scene_name) {\n        if (!this._nbTracker.currentWidget)\n            return;\n        const notebookPanel = this._nbTracker.currentWidget;\n        this.runSceneInNotebook(notebookPanel, scene_name);\n    }\n    runSceneInNotebook(notebookPanel, scene_name) {\n        const tag = this._getSceneTag(scene_name);\n        notebookPanel.content.widgets.map((cell) => {\n            if (!!cell.model.getMetadata(tag)) {\n                if (cell.model.type == 'code') {\n                    CodeCell.execute(cell, notebookPanel.sessionContext, { recordTiming: notebookPanel.content.notebookConfig.recordTiming });\n                }\n            }\n        });\n    }\n    createNewEmptyScene(scene_name) {\n        const scene_list = this.getScenesList();\n        if (scene_list.includes(scene_name))\n            return 'fail';\n        scene_list.push(scene_name);\n        this._sceneDB.setScenesList(scene_list);\n        this._scenesChanged();\n        return 'success';\n    }\n    duplicateActiveScene(new_scene_name) {\n        let retval = this.createNewEmptyScene(new_scene_name);\n        if (retval == 'fail')\n            return 'fail';\n        this._duplicateSceneTagInAllCells(this._nbTracker.currentWidget, this.getActiveScene(), new_scene_name);\n        this._scenesChanged();\n        return retval;\n    }\n    moveActiveSceneUp() {\n        this._moveScene(this._sceneDB.getActiveScene(), 'up');\n        this._scenesChanged();\n    }\n    moveActiveSceneDown() {\n        this._moveScene(this._sceneDB.getActiveScene(), 'down');\n        this._scenesChanged();\n    }\n    // **** various **************************************************************\n    updateCellClassesAndTags(notebook, scene_name = null, cell = null) {\n        // console.log('updating', scene_name)\n        if (scene_name == null)\n            scene_name = this.getActiveScene();\n        const scene_tag = this._getSceneTag(scene_name);\n        if (cell == null) {\n            notebook.widgets.map((cell) => {\n                this._updateCellClassAndTags(cell, scene_tag);\n            });\n        }\n        else {\n            this._updateCellClassAndTags(cell, scene_tag);\n        }\n    }\n    jumpToNextSceneCell() {\n        const presentCell = this._nbTracker.activeCell;\n        if (!presentCell)\n            return;\n        const tag = this._getSceneTag(this.getActiveScene());\n        const cells = this._nbTracker.currentWidget.content.widgets;\n        let cellIdx = cells.indexOf(presentCell);\n        let numCells = cells.length;\n        for (let n = cellIdx + 1; n < numCells; n++) {\n            let cell = cells[n];\n            if (cell.model.getMetadata(tag)) {\n                this._activateCellAndExpandParentHeadings(cell);\n                break;\n            }\n        }\n    }\n    jumpToPreviousSceneCell() {\n        const presentCell = this._nbTracker.activeCell;\n        if (!presentCell)\n            return;\n        const tag = this._getSceneTag(this.getActiveScene());\n        const cells = this._nbTracker.currentWidget.content.widgets;\n        let cellIdx = cells.indexOf(presentCell);\n        for (let n = cellIdx - 1; n >= 0; n--) {\n            let cell = cells[n];\n            if (cell.model.getMetadata(tag)) {\n                this._activateCellAndExpandParentHeadings(cell);\n                break;\n            }\n        }\n    }\n    importLegacyInitializationCells(notebook) {\n        if (!this._enableLegacyInits)\n            return;\n        let init_scenes_consistent = true;\n        let legacy_init_cells_exist = false;\n        let init_scene = this.getInitScene();\n        let init_scene_tag = (init_scene != null) ? this._getSceneTag(init_scene) : null;\n        // find out if there are legacy init cells and, if so, whether they are consistent with the scenes init cell\n        notebook.widgets.map((cell) => {\n            let is_legacy_init_cell = !!cell.model.getMetadata('init_cell');\n            let is_scenes_init_cell = init_scene_tag != null && !!cell.model.getMetadata(init_scene_tag);\n            if (is_legacy_init_cell) {\n                legacy_init_cells_exist = true;\n            }\n            if (is_legacy_init_cell != is_scenes_init_cell) {\n                init_scenes_consistent = false;\n            }\n        });\n        if (!init_scenes_consistent && legacy_init_cells_exist) {\n            const scene_name = 'Legacy Init';\n            notebook.widgets.map((cell) => {\n                let is_legacy_init_cell = !!cell.model.getMetadata('init_cell');\n                if (is_legacy_init_cell) {\n                    cell.model.setMetadata(this._getSceneTag(scene_name), true);\n                }\n            });\n            const scene_list = this.getScenesList();\n            if (!scene_list.includes(scene_name)) {\n                scene_list.push(scene_name);\n                this._sceneDB.setScenesList(scene_list);\n            }\n            this.toggleInitScene(scene_name);\n            this.setActiveScene(scene_name);\n        }\n    }\n    /* ****************************************************************************************************************************************\n     * Various private helper methods\n     * ****************************************************************************************************************************************/\n    _updateCellClassAndTags(cell, scene_tag) {\n        let cell_tags = [];\n        if (cell.model.getMetadata('tags')) {\n            cell_tags = cell.model.getMetadata('tags');\n        }\n        if (!!cell.model.getMetadata(scene_tag)) {\n            cell.addClass(SCENE_CELL_CLASS);\n            if (!cell_tags.includes('ActiveScene'))\n                cell_tags.push('ActiveScene');\n        }\n        else {\n            cell.removeClass(SCENE_CELL_CLASS);\n            if (cell_tags.includes('ActiveScene'))\n                cell_tags.splice(cell_tags.indexOf('ActiveScene'), 1);\n        }\n        if (cell_tags.length > 0) {\n            cell.model.setMetadata(\"tags\", cell_tags);\n        }\n        else {\n            cell.model.deleteMetadata(\"tags\");\n        }\n    }\n    _writeCellMetadataForLegacyInitializationCellsPlugin(notebook) {\n        if (!this._enableLegacyInits)\n            return;\n        let init_scene = this.getInitScene();\n        let init_scene_tag = (init_scene != null) ? this._getSceneTag(init_scene) : null;\n        notebook.widgets.map((cell) => {\n            if (init_scene_tag != null && !!cell.model.getMetadata(init_scene_tag)) {\n                cell.model.setMetadata('init_cell', true);\n            }\n            else {\n                cell.model.deleteMetadata('init_cell');\n            }\n        });\n    }\n    _activateCellAndExpandParentHeadings(cell) {\n        NotebookActions.expandParent(cell, this._nbTracker.currentWidget.content);\n        cell.activate();\n    }\n    _moveScene(scene_name, direction) {\n        const scenes_list = this.getScenesList();\n        let idx = scenes_list.indexOf(scene_name);\n        if (direction == 'down') {\n            if (idx == scenes_list.length - 1)\n                return;\n        }\n        else { // direction = 'up'\n            if (idx == 0)\n                return;\n            idx -= 1;\n        }\n        scenes_list.splice(idx, 2, scenes_list[idx + 1], scenes_list[idx]);\n        this._sceneDB.setScenesList(scenes_list);\n    }\n    _removeSceneTagFromAllCells(nbPanel, scene_name) {\n        const tag = this._getSceneTag(scene_name);\n        const notebook = nbPanel.content;\n        notebook.widgets.map((cell) => {\n            if (!!cell.model.getMetadata(tag)) {\n                cell.model.deleteMetadata(tag);\n            }\n        });\n    }\n    _renameSceneTagFromAllCells(nbPanel, old_scene_name, new_scene_name) {\n        const old_tag = this._getSceneTag(old_scene_name);\n        const new_tag = this._getSceneTag(new_scene_name);\n        const notebook = nbPanel.content;\n        notebook.widgets.map((cell) => {\n            if (!!cell.model.getMetadata(old_tag)) {\n                cell.model.deleteMetadata(old_tag);\n                cell.model.setMetadata(new_tag, true);\n            }\n        });\n    }\n    _duplicateSceneTagInAllCells(nbPanel, source_scene_name, target_scene_name) {\n        const source_tag = this._getSceneTag(source_scene_name);\n        const target_tag = this._getSceneTag(target_scene_name);\n        const notebook = nbPanel.content;\n        notebook.widgets.map((cell) => {\n            if (!!cell.model.getMetadata(source_tag)) {\n                cell.model.setMetadata(target_tag, true);\n            }\n        });\n    }\n    _scenesChanged() {\n        const activeScene = this._sceneDB.getActiveScene();\n        if (!activeScene)\n            return;\n        let activeNotebookPanel = this._nbTracker.currentWidget;\n        this._nbTracker.forEach((nbPanel) => {\n            if (nbPanel.context === activeNotebookPanel.context) {\n                this.updateCellClassesAndTags(nbPanel.content, activeScene);\n            }\n        });\n        this._writeCellMetadataForLegacyInitializationCellsPlugin(activeNotebookPanel.content);\n        this.scenesChanged.emit(void 0);\n    }\n    _getSceneTag(scene_name) {\n        return 'scene__' + scene_name;\n    }\n}\nclass NotebookSceneDatabase {\n    constructor(nbTracker) {\n        this._nbTracker = nbTracker;\n    }\n    /* ****************************************************************************************************************************************\n     * Data access\n     * ****************************************************************************************************************************************/\n    // **** simple getters *************************************************\n    getNotebookTitle() {\n        if (!this._nbTracker.currentWidget) {\n            return null;\n        }\n        return PathExt.basename(this._nbTracker.currentWidget.context.localPath);\n    }\n    getScenesList() {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return [];\n        return data['scenes'];\n    }\n    getActiveScene(notebook = null) {\n        let data = this._getSceneDataAndMaybeSetupDefaultData(notebook);\n        if (!data)\n            return null;\n        return data['active_scene'];\n    }\n    getInitScene() {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return null;\n        return data['init_scene'];\n    }\n    // **** scene setters **************************************************\n    toggleInitScene(scene_name) {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return;\n        if (data['init_scene'] == scene_name) {\n            data['init_scene'] = null;\n        }\n        else {\n            data['init_scene'] = scene_name;\n        }\n        this._setSceneData(data);\n    }\n    setActiveScene(scene_name) {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return;\n        data['active_scene'] = scene_name;\n        this._setSceneData(data);\n    }\n    setScenesList(scene_list) {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return;\n        data['scenes'] = scene_list;\n        this._setSceneData(data);\n    }\n    /* ****************************************************************************************************************************************\n     * Helpers\n     * ****************************************************************************************************************************************/\n    _getSceneDataAndMaybeSetupDefaultData(notebook = null) {\n        if (!notebook) {\n            notebook = this._nbTracker.currentWidget.content;\n        }\n        let model = notebook.model;\n        if (!model) {\n            return null;\n        }\n        if (model.getMetadata(NB_METADATA_KEY) == null) {\n            console.log('setting default scene data!!!!!!!!!!!');\n            model.setMetadata(NB_METADATA_KEY, { scenes: ['Default Scene'], active_scene: 'Default Scene', init_scene: '' });\n        }\n        let data_json = model.getMetadata(NB_METADATA_KEY);\n        let retval = {\n            scenes: data_json['scenes'],\n            active_scene: data_json['active_scene'],\n            init_scene: data_json['init_scene']\n        };\n        console.log('got scene data', retval);\n        return retval;\n    }\n    _setSceneData(scene_data) {\n        var _a;\n        let notebook_model = (_a = this._nbTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.model;\n        if (!notebook_model)\n            return;\n        notebook_model.setMetadata(NB_METADATA_KEY, scene_data);\n    }\n}\n;\n",
+        "import { NotebookActions } from '@jupyterlab/notebook';\nimport { CodeCell } from '@jupyterlab/cells';\nimport { PathExt } from '@jupyterlab/coreutils';\nimport { Signal } from '@lumino/signaling';\nconst NB_METADATA_KEY = 'scenes_data';\nconst SCENE_CELL_CLASS = 'scene-cell';\nexport class NotebookHandler {\n    constructor(nbTracker, settingRegistry) {\n        this.scenesChanged = new Signal(this);\n        /* ****************************************************************************************************************************************\n         * Handle kernel (re-)starts\n         * ****************************************************************************************************************************************/\n        this._kernelStatusDict = {};\n        this._nbTracker = nbTracker;\n        this._sceneDB = new NotebookSceneDatabase(nbTracker);\n        this._enableLegacyInits = false;\n        // load settings\n        if (settingRegistry) {\n            settingRegistry.load('jupyterlab_scenes:plugin').then(settings => {\n                this.updateSettings(settings);\n                settings.changed.connect(() => { this.updateSettings(settings); });\n            })\n                .catch(reason => {\n                console.error('Failed to load settings for jupyterlab_scenes.', reason);\n            });\n        }\n        this._setupKernelListener();\n    }\n    updateSettings(settings) {\n        this._enableLegacyInits = settings.composite.legacyInit;\n    }\n    _setupKernelListener() {\n        this._nbTracker.widgetAdded.connect(async (sender, nbPanel) => {\n            nbPanel.context.sessionContext.ready.then(() => {\n                this._kernelStatusDict[nbPanel.context.sessionContext.session.kernel.id] = 'connecting';\n                nbPanel.context.sessionContext.session.kernel.connectionStatusChanged.connect((kernel, conn_stat) => { this._kernelListener(kernel, conn_stat); });\n            });\n        });\n    }\n    _kernelListener(kernel, conn_stat) {\n        if (conn_stat == 'connecting') {\n            this._kernelStatusDict[kernel.id] = 'connecting';\n        }\n        else if (conn_stat == 'connected') {\n            if (this._kernelStatusDict[kernel.id] == 'connecting') {\n                let notebookPanelList = [];\n                this._nbTracker.forEach((nbPanel) => {\n                    if (nbPanel.context.sessionContext.session.kernel.id == kernel.id) {\n                        notebookPanelList.push(nbPanel);\n                    }\n                });\n                if (notebookPanelList.length > 0) {\n                    let init_scene = this._sceneDB.getInitScene();\n                    if (init_scene)\n                        this.runSceneInNotebook(notebookPanelList[0], init_scene);\n                }\n            }\n            delete this._kernelStatusDict[kernel.id];\n        }\n    }\n    /* ****************************************************************************************************************************************\n     * Functionality provided to the main widget\n     * ****************************************************************************************************************************************/\n    // **** simple scene getters *************************************************\n    getNotebookTitle() {\n        return this._sceneDB.getNotebookTitle();\n    }\n    getScenesList() {\n        return this._sceneDB.getScenesList();\n    }\n    getActiveScene(notebook = null) {\n        return this._sceneDB.getActiveScene(notebook);\n    }\n    getInitScene() {\n        return this._sceneDB.getInitScene();\n    }\n    // **** scene setters ********************************************************\n    toggleInitScene(scene_name) {\n        this._sceneDB.toggleInitScene(scene_name);\n        this._scenesChanged();\n    }\n    setActiveScene(scene_name) {\n        this._sceneDB.setActiveScene(scene_name);\n        this._scenesChanged();\n    }\n    renameScene(old_scene_name, new_scene_name) {\n        const scenes_list = this.getScenesList();\n        if (scenes_list.includes(new_scene_name))\n            return 'fail';\n        if (this._sceneDB.getInitScene() == old_scene_name) {\n            this._sceneDB.toggleInitScene(new_scene_name);\n        }\n        if (this._sceneDB.getActiveScene() == old_scene_name) {\n            this._sceneDB.setActiveScene(new_scene_name);\n        }\n        let idx = scenes_list.lastIndexOf(old_scene_name);\n        scenes_list[idx] = new_scene_name;\n        this._sceneDB.setScenesList(scenes_list);\n        this._renameSceneTagFromAllCells(this._nbTracker.currentWidget, old_scene_name, new_scene_name);\n        this._scenesChanged();\n        return 'success';\n    }\n    deleteScene(scene_name) {\n        let scenes_list = this._sceneDB.getScenesList();\n        if (scenes_list.length == 1)\n            return;\n        if (this._sceneDB.getInitScene() == scene_name) {\n            this._sceneDB.toggleInitScene(scene_name);\n        }\n        let resetActiveScene = this._sceneDB.getActiveScene() == scene_name;\n        this._removeSceneTagFromAllCells(this._nbTracker.currentWidget, scene_name);\n        let idx = scenes_list.lastIndexOf(scene_name);\n        scenes_list.splice(idx, 1);\n        this._sceneDB.setScenesList(scenes_list);\n        if (resetActiveScene) {\n            if (idx < scenes_list.length) {\n                this.setActiveScene(scenes_list[idx]);\n            }\n            else {\n                this.setActiveScene(scenes_list[idx - 1]);\n            }\n        }\n        this._scenesChanged();\n    }\n    toggleSceneMembershipOfSelectedCells() {\n        if (!this._nbTracker.currentWidget)\n            return;\n        if (!this._nbTracker.activeCell)\n            return;\n        const current_scene = this._sceneDB.getActiveScene();\n        const is_init_scene = current_scene == this.getInitScene();\n        const tag = 'scene__' + current_scene;\n        const notebook = this._nbTracker.currentWidget.content;\n        const set_membership = !this._nbTracker.activeCell.model.getMetadata(tag);\n        //const set_membership = !this._nbTracker.activeCell.model.getMetadata(tag);\n        notebook.widgets.forEach((cell) => {\n            if (!notebook.isSelectedOrActive(cell))\n                return;\n            if (cell.model.type != 'code')\n                return;\n            if (set_membership) {\n                cell.model.setMetadata(tag, true);\n                if (is_init_scene) {\n                    cell.model.setMetadata('init_cell', true);\n                }\n            }\n            else {\n                cell.model.deleteMetadata(tag);\n                if (is_init_scene) {\n                    cell.model.deleteMetadata('init_cell');\n                }\n            }\n            this._updateCellClassAndTags(cell, tag);\n        });\n    }\n    // **** scene management and running *****************************************\n    runActiveSceneInCurrentNotebook() {\n        const active_scene = this._sceneDB.getActiveScene();\n        if (active_scene)\n            this.runSceneInCurrentNotebook(active_scene);\n    }\n    runSceneInCurrentNotebook(scene_name) {\n        if (!this._nbTracker.currentWidget)\n            return;\n        const notebookPanel = this._nbTracker.currentWidget;\n        this.runSceneInNotebook(notebookPanel, scene_name);\n    }\n    runSceneInNotebook(notebookPanel, scene_name) {\n        const tag = this._getSceneTag(scene_name);\n        notebookPanel.content.widgets.map((cell) => {\n            if (!!cell.model.getMetadata(tag)) {\n                if (cell.model.type == 'code') {\n                    CodeCell.execute(cell, notebookPanel.sessionContext, { recordTiming: notebookPanel.content.notebookConfig.recordTiming });\n                }\n            }\n        });\n    }\n    createNewEmptyScene(scene_name) {\n        const scene_list = this.getScenesList();\n        if (scene_list.includes(scene_name))\n            return 'fail';\n        scene_list.push(scene_name);\n        this._sceneDB.setScenesList(scene_list);\n        this._sceneDB.setActiveScene(scene_name);\n        this._scenesChanged();\n        return 'success';\n    }\n    duplicateActiveScene(new_scene_name) {\n        let retval = this.createNewEmptyScene(new_scene_name);\n        if (retval == 'fail')\n            return 'fail';\n        this._duplicateSceneTagInAllCells(this._nbTracker.currentWidget, this.getActiveScene(), new_scene_name);\n        this._sceneDB.setActiveScene(new_scene_name);\n        this._scenesChanged();\n        return retval;\n    }\n    moveActiveSceneUp() {\n        this._moveScene(this._sceneDB.getActiveScene(), 'up');\n        this._scenesChanged();\n    }\n    moveActiveSceneDown() {\n        this._moveScene(this._sceneDB.getActiveScene(), 'down');\n        this._scenesChanged();\n    }\n    // **** various **************************************************************\n    updateCellClassesAndTags(notebook, scene_name = null, cell = null) {\n        // console.log('updating', scene_name)\n        if (scene_name == null)\n            scene_name = this.getActiveScene();\n        const scene_tag = this._getSceneTag(scene_name);\n        if (cell == null) {\n            notebook.widgets.map((cell) => {\n                this._updateCellClassAndTags(cell, scene_tag);\n            });\n        }\n        else {\n            this._updateCellClassAndTags(cell, scene_tag);\n        }\n    }\n    jumpToNextSceneCell() {\n        const presentCell = this._nbTracker.activeCell;\n        if (!presentCell)\n            return;\n        const tag = this._getSceneTag(this.getActiveScene());\n        const cells = this._nbTracker.currentWidget.content.widgets;\n        let cellIdx = cells.indexOf(presentCell);\n        let numCells = cells.length;\n        for (let n = cellIdx + 1; n < numCells; n++) {\n            let cell = cells[n];\n            if (cell.model.getMetadata(tag)) {\n                this._activateCellAndExpandParentHeadings(cell);\n                break;\n            }\n        }\n    }\n    jumpToPreviousSceneCell() {\n        const presentCell = this._nbTracker.activeCell;\n        if (!presentCell)\n            return;\n        const tag = this._getSceneTag(this.getActiveScene());\n        const cells = this._nbTracker.currentWidget.content.widgets;\n        let cellIdx = cells.indexOf(presentCell);\n        for (let n = cellIdx - 1; n >= 0; n--) {\n            let cell = cells[n];\n            if (cell.model.getMetadata(tag)) {\n                this._activateCellAndExpandParentHeadings(cell);\n                break;\n            }\n        }\n    }\n    importLegacyInitializationCells(notebook) {\n        if (!this._enableLegacyInits)\n            return;\n        let init_scenes_consistent = true;\n        let legacy_init_cells_exist = false;\n        let init_scene = this.getInitScene();\n        let init_scene_tag = (init_scene != null) ? this._getSceneTag(init_scene) : null;\n        // find out if there are legacy init cells and, if so, whether they are consistent with the scenes init cell\n        notebook.widgets.map((cell) => {\n            let is_legacy_init_cell = !!cell.model.getMetadata('init_cell');\n            let is_scenes_init_cell = init_scene_tag != null && !!cell.model.getMetadata(init_scene_tag);\n            if (is_legacy_init_cell) {\n                legacy_init_cells_exist = true;\n            }\n            if (is_legacy_init_cell != is_scenes_init_cell) {\n                init_scenes_consistent = false;\n            }\n        });\n        if (!init_scenes_consistent && legacy_init_cells_exist) {\n            const scene_name = 'Legacy Init';\n            notebook.widgets.map((cell) => {\n                let is_legacy_init_cell = !!cell.model.getMetadata('init_cell');\n                if (is_legacy_init_cell) {\n                    cell.model.setMetadata(this._getSceneTag(scene_name), true);\n                }\n            });\n            const scene_list = this.getScenesList();\n            if (!scene_list.includes(scene_name)) {\n                scene_list.push(scene_name);\n                this._sceneDB.setScenesList(scene_list);\n            }\n            this.toggleInitScene(scene_name);\n            this.setActiveScene(scene_name);\n        }\n    }\n    /* ****************************************************************************************************************************************\n     * Various private helper methods\n     * ****************************************************************************************************************************************/\n    _updateCellClassAndTags(cell, scene_tag) {\n        let cell_tags = [];\n        if (cell.model.getMetadata('tags')) {\n            cell_tags = cell.model.getMetadata('tags');\n        }\n        if (!!cell.model.getMetadata(scene_tag)) {\n            cell.addClass(SCENE_CELL_CLASS);\n            if (!cell_tags.includes('ActiveScene'))\n                cell_tags.push('ActiveScene');\n        }\n        else {\n            cell.removeClass(SCENE_CELL_CLASS);\n            if (cell_tags.includes('ActiveScene'))\n                cell_tags.splice(cell_tags.indexOf('ActiveScene'), 1);\n        }\n        if (cell_tags.length > 0) {\n            cell.model.setMetadata(\"tags\", cell_tags);\n        }\n        else {\n            cell.model.deleteMetadata(\"tags\");\n        }\n    }\n    _writeCellMetadataForLegacyInitializationCellsPlugin(notebook) {\n        if (!this._enableLegacyInits)\n            return;\n        let init_scene = this.getInitScene();\n        let init_scene_tag = (init_scene != null) ? this._getSceneTag(init_scene) : null;\n        notebook.widgets.map((cell) => {\n            if (init_scene_tag != null && !!cell.model.getMetadata(init_scene_tag)) {\n                cell.model.setMetadata('init_cell', true);\n            }\n            else {\n                cell.model.deleteMetadata('init_cell');\n            }\n        });\n    }\n    _activateCellAndExpandParentHeadings(cell) {\n        let notebook = this._nbTracker.currentWidget.content;\n        NotebookActions.expandParent(cell, notebook);\n        notebook.scrollToCell(cell).then(() => { notebook.activeCellIndex = notebook.widgets.indexOf(cell); });\n    }\n    _moveScene(scene_name, direction) {\n        const scenes_list = this.getScenesList();\n        let idx = scenes_list.indexOf(scene_name);\n        if (direction == 'down') {\n            if (idx == scenes_list.length - 1)\n                return;\n        }\n        else { // direction = 'up'\n            if (idx == 0)\n                return;\n            idx -= 1;\n        }\n        scenes_list.splice(idx, 2, scenes_list[idx + 1], scenes_list[idx]);\n        this._sceneDB.setScenesList(scenes_list);\n    }\n    _removeSceneTagFromAllCells(nbPanel, scene_name) {\n        const tag = this._getSceneTag(scene_name);\n        const notebook = nbPanel.content;\n        notebook.widgets.map((cell) => {\n            if (!!cell.model.getMetadata(tag)) {\n                cell.model.deleteMetadata(tag);\n            }\n        });\n    }\n    _renameSceneTagFromAllCells(nbPanel, old_scene_name, new_scene_name) {\n        const old_tag = this._getSceneTag(old_scene_name);\n        const new_tag = this._getSceneTag(new_scene_name);\n        const notebook = nbPanel.content;\n        notebook.widgets.map((cell) => {\n            if (!!cell.model.getMetadata(old_tag)) {\n                cell.model.deleteMetadata(old_tag);\n                cell.model.setMetadata(new_tag, true);\n            }\n        });\n    }\n    _duplicateSceneTagInAllCells(nbPanel, source_scene_name, target_scene_name) {\n        const source_tag = this._getSceneTag(source_scene_name);\n        const target_tag = this._getSceneTag(target_scene_name);\n        const notebook = nbPanel.content;\n        notebook.widgets.map((cell) => {\n            if (!!cell.model.getMetadata(source_tag)) {\n                cell.model.setMetadata(target_tag, true);\n            }\n        });\n    }\n    _scenesChanged() {\n        const activeScene = this._sceneDB.getActiveScene();\n        if (!activeScene)\n            return;\n        let activeNotebookPanel = this._nbTracker.currentWidget;\n        this._nbTracker.forEach((nbPanel) => {\n            if (nbPanel.context === activeNotebookPanel.context) {\n                this.updateCellClassesAndTags(nbPanel.content, activeScene);\n            }\n        });\n        this._writeCellMetadataForLegacyInitializationCellsPlugin(activeNotebookPanel.content);\n        this.scenesChanged.emit(void 0);\n    }\n    _getSceneTag(scene_name) {\n        return 'scene__' + scene_name;\n    }\n}\nclass NotebookSceneDatabase {\n    constructor(nbTracker) {\n        this._nbTracker = nbTracker;\n    }\n    /* ****************************************************************************************************************************************\n     * Data access\n     * ****************************************************************************************************************************************/\n    // **** simple getters *************************************************\n    getNotebookTitle() {\n        if (!this._nbTracker.currentWidget) {\n            return null;\n        }\n        return PathExt.basename(this._nbTracker.currentWidget.context.localPath);\n    }\n    getScenesList() {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return [];\n        return data['scenes'];\n    }\n    getActiveScene(notebook = null) {\n        let data = this._getSceneDataAndMaybeSetupDefaultData(notebook);\n        if (!data)\n            return null;\n        return data['active_scene'];\n    }\n    getInitScene() {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return null;\n        return data['init_scene'];\n    }\n    // **** scene setters **************************************************\n    toggleInitScene(scene_name) {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return;\n        if (data['init_scene'] == scene_name) {\n            data['init_scene'] = null;\n        }\n        else {\n            data['init_scene'] = scene_name;\n        }\n        this._setSceneData(data);\n    }\n    setActiveScene(scene_name) {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return;\n        data['active_scene'] = scene_name;\n        this._setSceneData(data);\n    }\n    setScenesList(scene_list) {\n        let data = this._getSceneDataAndMaybeSetupDefaultData();\n        if (!data)\n            return;\n        data['scenes'] = scene_list;\n        this._setSceneData(data);\n    }\n    /* ****************************************************************************************************************************************\n     * Helpers\n     * ****************************************************************************************************************************************/\n    _getSceneDataAndMaybeSetupDefaultData(notebook = null) {\n        if (!notebook) {\n            notebook = this._nbTracker.currentWidget.content;\n        }\n        let model = notebook.model;\n        if (!model) {\n            return null;\n        }\n        if (model.getMetadata(NB_METADATA_KEY) == null) {\n            console.log('setting default scene data!!!!!!!!!!!');\n            model.setMetadata(NB_METADATA_KEY, { scenes: ['Default Scene'], active_scene: 'Default Scene', init_scene: '' });\n        }\n        let data_json = model.getMetadata(NB_METADATA_KEY);\n        let retval = {\n            scenes: data_json['scenes'],\n            active_scene: data_json['active_scene'],\n            init_scene: data_json['init_scene']\n        };\n        return retval;\n    }\n    _setSceneData(scene_data) {\n        var _a;\n        let notebook_model = (_a = this._nbTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.model;\n        if (!notebook_model)\n            return;\n        notebook_model.setMetadata(NB_METADATA_KEY, scene_data);\n    }\n}\n;\n",
         "import * as React from 'react';\nimport { runIcon, closeIcon, editIcon, addIcon, copyIcon } from '@jupyterlab/ui-components';\nimport { LabIcon } from '@jupyterlab/ui-components';\nimport { ScenesSidebar } from './widget';\nimport cellUp from '../style/svg/cellUp.svg';\nimport cellDown from '../style/svg/cellDown.svg';\nimport arrowUp from '../style/svg/arrowUp.svg';\nimport arrowDown from '../style/svg/arrowDown.svg';\nconst cellUpIcon = new LabIcon({ name: 'cellUp', svgstr: cellUp });\nconst cellDownIcon = new LabIcon({ name: 'cellDown', svgstr: cellDown });\nconst arrowUpIcon = new LabIcon({ name: 'arrowUp', svgstr: arrowUp });\nconst arrowDownIcon = new LabIcon({ name: 'arrowDown', svgstr: arrowDown });\nexport class ScenesDisplay extends React.Component {\n    render() {\n        return (React.createElement(\"div\", { className: \"scenes-ScenesSidebar\" },\n            React.createElement(\"div\", { className: \"scenes-Header\" },\n                this.props.nbTitle,\n                \": Scenes\"),\n            React.createElement(Toolbar, { commands: this.props.commands }),\n            React.createElement(ScenesList, { scenes: this.props.scenes, currentScene: this.props.currentScene, initScene: this.props.initScene, notebookHandler: this.props.notebookHandler, commands: this.props.commands })));\n    }\n}\nclass ScenesList extends React.Component {\n    render() {\n        let list = this.props.scenes.map(scene_name => {\n            const onClickActivate = () => {\n                this.props.notebookHandler.setActiveScene(scene_name);\n            };\n            const onClickDelete = (event) => {\n                event.preventDefault();\n                event.stopPropagation();\n                this.props.commands.execute(ScenesSidebar.command_id_delete_scene, { 'scene_name': scene_name });\n            };\n            const onClickEdit = (event) => {\n                event.preventDefault();\n                event.stopPropagation();\n                this.props.commands.execute(ScenesSidebar.command_id_rename_scene, { 'scene_name': scene_name });\n            };\n            const onClickInit = (event) => {\n                event.preventDefault();\n                event.stopPropagation();\n                this.props.notebookHandler.toggleInitScene(scene_name);\n            };\n            const onClickRun = (event) => {\n                event.preventDefault();\n                event.stopPropagation();\n                this.props.notebookHandler.runSceneInCurrentNotebook(scene_name);\n            };\n            let active = this.props.currentScene == scene_name;\n            let init = this.props.initScene == scene_name;\n            let className = active ? \"scenes-SceneItem scenes-active\" : \"scenes-SceneItem\";\n            let classNameInitButton = init ? \"scenes-InitSceneButtonActive\" : \"scenes-InitSceneButton\";\n            let sceneNameDisplay = active ? \"  \" + scene_name + \" (active)\" : \"  \" + scene_name;\n            return (React.createElement(\"div\", { className: className, onClick: onClickActivate, key: scene_name },\n                React.createElement(\"button\", { className: \"scenes-ItemButton\", title: \"Delete Scene\", onClick: onClickDelete },\n                    React.createElement(closeIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" })),\n                React.createElement(\"button\", { className: \"scenes-ItemButton\", title: \"Run Scene\", onClick: onClickRun },\n                    React.createElement(runIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" })),\n                React.createElement(\"button\", { className: \"scenes-ItemButton\", title: \"Rename Scene\", onClick: onClickEdit },\n                    React.createElement(editIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" })),\n                React.createElement(\"div\", { className: \"scenes-ItemText\" }, sceneNameDisplay),\n                React.createElement(\"div\", { className: \"scenes-SceneItemSpacer\" }),\n                React.createElement(\"button\", { onClick: onClickInit, className: classNameInitButton }, \"init\")));\n        });\n        return (React.createElement(\"div\", { className: \"scenes-SceneList\" }, list));\n    }\n}\nclass Toolbar extends React.Component {\n    render() {\n        const onClickNew = () => {\n            this.props.commands.execute(ScenesSidebar.command_id_new_empty_scene);\n        };\n        const onClickDuplicate = () => {\n            this.props.commands.execute(ScenesSidebar.command_id_duplicate_scene);\n        };\n        const onClickUp = () => {\n            this.props.commands.execute(ScenesSidebar.command_id_move_active_scene_up);\n        };\n        const onClickDown = () => {\n            this.props.commands.execute(ScenesSidebar.command_id_move_active_scene_down);\n        };\n        const onClickNext = () => {\n            this.props.commands.execute(ScenesSidebar.command_id_to_next_scene_cell);\n        };\n        const onClickPrev = () => {\n            this.props.commands.execute(ScenesSidebar.command_id_to_previous_scene_cell);\n        };\n        return (React.createElement(\"div\", { className: \"scenes-Toolbar\" },\n            React.createElement(\"button\", { className: \"scenes-ToolbarButton\", title: \"New Empty Scene\", onClick: onClickNew },\n                React.createElement(addIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" })),\n            React.createElement(\"button\", { className: \"scenes-ToolbarButton\", title: \"Duplicate Active Scene\", onClick: onClickDuplicate },\n                React.createElement(copyIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" })),\n            React.createElement(\"button\", { className: \"scenes-ToolbarButton\", title: \"Move Active Scene Up\", onClick: onClickUp },\n                React.createElement(arrowUpIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" })),\n            React.createElement(\"button\", { className: \"scenes-ToolbarButton\", title: \"Move Active Scene Down\", onClick: onClickDown },\n                React.createElement(arrowDownIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" })),\n            React.createElement(\"div\", { className: \"scenes-SceneItemSpacer\" }),\n            React.createElement(\"button\", { className: \"scenes-ToolbarButton\", title: \"Jump to Next Scene Cell\", onClick: onClickNext },\n                React.createElement(cellDownIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" })),\n            React.createElement(\"button\", { className: \"scenes-ToolbarButton\", title: \"Move to Previous Scene Cell\", onClick: onClickPrev },\n                React.createElement(cellUpIcon.react, { tag: \"span\", className: \"jp-ToolbarButtonComponent-icon f1vya9e0\" }))));\n    }\n}\n",
         "import { ILabShell } from '@jupyterlab/application';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { INotebookTracker } from '@jupyterlab/notebook';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { ScenesSidebar } from './widget';\nfunction activateScenes(app, settingRegistry, nbTracker, mainMenu, labShell) {\n    // create the ScenesSidebar widget\n    const scenesSidebar = new ScenesSidebar(app, nbTracker, mainMenu, settingRegistry);\n    app.shell.add(scenesSidebar, 'left', { rank: 1000 });\n}\n/**\n * Initialization data for the jupyterlab_scenes extension.\n */\nconst plugin = {\n    id: 'jupyterlab_scenes:plugin',\n    autoStart: true,\n    optional: [ISettingRegistry, INotebookTracker, IMainMenu, ILabShell],\n    activate: activateScenes\n};\nexport default plugin;\n",
         "import { Menu } from '@lumino/widgets';\nimport { ReactWidget, InputDialog, Dialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { LabIcon } from '@jupyterlab/ui-components';\nimport React from 'react';\nimport { ScenesDisplay } from './components';\nimport { NotebookHandler } from './backend';\nimport scenesLogo from '../style/svg/scenesLogo.svg';\nconst scenesIcon = new LabIcon({ name: 'scenes', svgstr: scenesLogo });\nclass ScenesSidebar extends ReactWidget {\n    constructor(app, nbTracker, mainMenu, settingRegistry) {\n        super();\n        this._app = app;\n        this._nbTracker = nbTracker;\n        this._mainMenu = mainMenu;\n        this._scenesMenu = null;\n        this._notebookHandler = new NotebookHandler(nbTracker, settingRegistry);\n        this._setupWidget();\n        this._setupGlobalCommands();\n        this._setupKeyboardShortcuts();\n        this._setupScenesMenu();\n        // this is needed to sync ScenesSidebar and code cells on load\n        this._nbTracker.widgetAdded.connect((_x, nbpanel) => {\n            //console.log('widgetAdded', nbpanel.context.path)\n            nbpanel.context.ready.then(() => {\n                //console.log('context ready', nbpanel.context.path);\n                this._notebookHandler.updateCellClassesAndTags(nbpanel.content, this._notebookHandler.getActiveScene(nbpanel.content));\n                this._notebookHandler.importLegacyInitializationCells(nbpanel.content);\n                this.update();\n            });\n            // this is needed for handling copy/paste\n            nbpanel.content.activeCellChanged.connect((notebook, cell) => {\n                this._notebookHandler.updateCellClassesAndTags(notebook, this._notebookHandler.getActiveScene(), cell);\n            });\n        });\n        // this is needed syncing the ScenesSidebar to the current notebook panel\n        this._nbTracker.currentChanged.connect((sender, nbpanel) => {\n            //console.log('currentChanged', nbpanel!.context.path)\n            if (!(nbpanel === null || nbpanel === void 0 ? void 0 : nbpanel.context.isReady))\n                return;\n            this.update();\n        });\n        this._notebookHandler.scenesChanged.connect(() => { this.update(); });\n    }\n    render() {\n        let nb_title = this._notebookHandler.getNotebookTitle();\n        if (!nb_title)\n            return (React.createElement(\"div\", null));\n        return (React.createElement(ScenesDisplay, { nbTitle: nb_title, scenes: this._notebookHandler.getScenesList(), currentScene: this._notebookHandler.getActiveScene(), initScene: this._notebookHandler.getInitScene(), commands: this._app.commands, notebookHandler: this._notebookHandler }));\n    }\n    onNotebookChanged() {\n        this.update();\n    }\n    /* ****************************************************************************************************************************************\n     * Private helper methods\n     * ****************************************************************************************************************************************/\n    // **** setup helpers ****************************************************************************************************************\n    _setupWidget() {\n        this.id = 'scenes';\n        this.title.caption = 'Scenes';\n        this.title.icon = scenesIcon;\n    }\n    _setupGlobalCommands() {\n        this._app.commands.addCommand(ScenesSidebar.command_id_toggle_scene_cell, {\n            label: 'Toggle Scene Cell',\n            execute: () => { this._notebookHandler.toggleSceneMembershipOfSelectedCells(); }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_run_scene, {\n            label: 'Run Scene',\n            execute: () => { this._notebookHandler.runActiveSceneInCurrentNotebook(); }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_new_empty_scene, {\n            label: 'New Empty Scene',\n            execute: () => {\n                InputDialog.getText({ title: 'Name of the New Scene:' }).then((new_scene) => {\n                    if (!new_scene.value)\n                        return;\n                    if (this._notebookHandler.createNewEmptyScene(new_scene.value) == 'fail') {\n                        showErrorMessage('Error: New Scene Creation', 'Scene with name \"' + new_scene.value + '\" already exists!');\n                    }\n                });\n            }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_duplicate_scene, {\n            label: 'Duplicate Active Scene',\n            execute: () => {\n                InputDialog.getText({ title: 'Name of the Duplicated Scene:' }).then((new_scene) => {\n                    if (!new_scene.value)\n                        return;\n                    if (this._notebookHandler.duplicateActiveScene(new_scene.value) == 'fail') {\n                        showErrorMessage('Error: Scene Duplication', 'Scene with name \"' + new_scene.value + '\" already exists!');\n                    }\n                });\n            }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_delete_scene, {\n            label: 'Delete Scene',\n            execute: async (scene_name_obj) => {\n                let scene_name = scene_name_obj['scene_name'];\n                const result = await (new Dialog({\n                    title: 'Delete Scene \"' + scene_name + '\" permanently?',\n                    buttons: [Dialog.cancelButton(), Dialog.okButton({ label: 'Delete' })]\n                }).launch());\n                if (result.button.label == 'Delete') {\n                    this._notebookHandler.deleteScene(scene_name);\n                }\n            }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_rename_scene, {\n            label: 'Rename Scene',\n            execute: async (scene_name_obj) => {\n                let scene_name = scene_name_obj['scene_name'];\n                InputDialog.getText({ title: 'New Name of Scene \"' + scene_name + '\":' }).then((new_scene_name) => {\n                    if (!new_scene_name.value)\n                        return;\n                    if (this._notebookHandler.renameScene(scene_name, new_scene_name.value) == 'fail') {\n                        showErrorMessage('Error: Scene Renaming', 'Scene with name \"' + new_scene_name.value + '\" already exists!');\n                    }\n                });\n            }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_move_active_scene_up, {\n            label: 'Move Active Scene Up',\n            execute: () => { this._notebookHandler.moveActiveSceneUp(); }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_move_active_scene_down, {\n            label: 'Move Active Scene Down',\n            execute: () => { this._notebookHandler.moveActiveSceneDown(); }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_to_next_scene_cell, {\n            label: 'Jump to Next Scene Cell',\n            execute: () => { this._notebookHandler.jumpToNextSceneCell(); }\n        });\n        this._app.commands.addCommand(ScenesSidebar.command_id_to_previous_scene_cell, {\n            label: 'Jump to Previous Scene Cell',\n            execute: () => { this._notebookHandler.jumpToPreviousSceneCell(); }\n        });\n    }\n    _setupKeyboardShortcuts() {\n        this._app.commands.addKeyBinding({\n            command: ScenesSidebar.command_id_toggle_scene_cell,\n            args: {},\n            keys: ['Accel I'],\n            selector: '.jp-Notebook'\n        });\n        this._app.commands.addKeyBinding({\n            command: ScenesSidebar.command_id_run_scene,\n            args: {},\n            keys: ['Ctrl Alt R'],\n            selector: '.jp-Notebook'\n        });\n    }\n    _setupScenesMenu() {\n        this._scenesMenu = new Menu({ commands: this._app.commands });\n        this._scenesMenu.title.label = 'Scenes';\n        this._scenesMenu.addItem({ command: ScenesSidebar.command_id_toggle_scene_cell });\n        this._scenesMenu.addItem({ command: ScenesSidebar.command_id_run_scene });\n        this._scenesMenu.addItem({ type: 'separator' });\n        this._scenesMenu.addItem({ command: ScenesSidebar.command_id_new_empty_scene });\n        this._scenesMenu.addItem({ command: ScenesSidebar.command_id_duplicate_scene });\n        this._mainMenu.addMenu(this._scenesMenu);\n    }\n}\nScenesSidebar.command_id_toggle_scene_cell = 'scenes:toggle-scene-cell';\nScenesSidebar.command_id_run_scene = 'scenes:run-scene';\nScenesSidebar.command_id_new_empty_scene = 'scenes:new-empty-scene';\nScenesSidebar.command_id_duplicate_scene = 'scenes:duplicate-scene';\nScenesSidebar.command_id_rename_scene = 'scenes:rename-scene';\nScenesSidebar.command_id_delete_scene = 'scenes:delete-scene';\nScenesSidebar.command_id_move_active_scene_up = 'scenes:move-active-scene-up';\nScenesSidebar.command_id_move_active_scene_down = 'scenes:move-active-scene-down';\nScenesSidebar.command_id_to_next_scene_cell = 'scenes:jump-to-next-scene-cell';\nScenesSidebar.command_id_to_previous_scene_cell = 'scenes:jump-to-previous-scene-cell';\nexport { ScenesSidebar };\n;\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/remoteEntry.ec56600e3e74782839f0.js` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.9fa23aea731399224cde.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "ee4dbc9980b7e689c6f6",
+                "lib_index_js": "0aa35e0458ae63cde8ee",
                 "style_index_js": "af8725b98d07f334206d"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
@@ -1095,8 +1095,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab_scenes");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyterlab_scenes = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.ec56600e3e74782839f0.js.map
+//# sourceMappingURL=remoteEntry.9fa23aea731399224cde.js.map
```

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/remoteEntry.ec56600e3e74782839f0.js.map` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/remoteEntry.080c207a518f60ccdd6f.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.080c207a518f60ccdd6f.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_index_js":"464c8e8f3b11e19e4131","style_index_js":"af8725b98d07f334206d"}[chunkId] '*

 * *                     '+ ".js";\\n};\')], delete: [5]}'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.ec56600e3e74782839f0.js",
+    "file": "remoteEntry.080c207a518f60ccdd6f.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC3LA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_scenes/webpack/container-entry",
         "webpack://jupyterlab_scenes/webpack/bootstrap",
         "webpack://jupyterlab_scenes/webpack/runtime/compat get default export",
@@ -25,15 +25,15 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"ee4dbc9980b7e689c6f6\",\"style_index_js\":\"af8725b98d07f334206d\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"464c8e8f3b11e19e4131\",\"style_index_js\":\"af8725b98d07f334206d\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_scenes:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t};\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab_scenes\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_scenes\", \"2.0.0-alpha1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,0,0,,\"alpha\",19])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,4,0,0,,\"alpha\",19])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,0,,\"alpha\",19])),\n\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,4,0,0,,\"alpha\",19])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,0,0,,\"beta\",1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,0,0,,\"alpha\",19])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,0,0,,\"alpha\",34])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/cells\": () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,4,0,0,,\"alpha\",19])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,0,0,,\"alpha\",19])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,2,0,0,,\"beta\",1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/cells\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
```

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/style_index_js.af8725b98d07f334206d.js` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/style_index_js.af8725b98d07f334206d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes/labextension/static/style_index_js.af8725b98d07f334206d.js.map` & `jupyterlab_scenes-2.0.0a2/jupyterlab_scenes/labextension/static/style_index_js.af8725b98d07f334206d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/jupyterlab_scenes.egg-info/PKG-INFO` & `jupyterlab_scenes-2.0.0a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyterlab-scenes
-Version: 2.0.0a1
+Name: jupyterlab_scenes
+Version: 2.0.0a2
 Summary: Define subsets of code cells as scenes and execute them.
 Home-page: https://github.com/schmidi314/jupyterlab_scenes
 Author: Manuel Schmidt
 Author-email: Manuel.J.Schmidt@t-online.de
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab4
 Platform: Linux
@@ -45,17 +45,25 @@
 * By clicking the `init` button, one scene can be chosen to be automatically executed as the kernel becomes ready (due to a restart or at the initial loading of the notebook).
 * If a notebook with an already running kernel is opened, the init scene is __not__ executed.
 * Only one scene can be an init scene.
 
 ![Initialization](https://github.com/schmidi314/jupyterlab-scenes/blob/master/gifs/scenes_init.gif?raw=true)
 
 
+* To run a scene named `My Favourite Scene` programatically, do
+    ```
+    from ipylab import JupyterFrontEnd
+    JupyterFrontEnd().commands.execute('scenes:run-scene', 'My Favourite Scene')
+    ```
+    But you may run only one scene at a time. No excessive looping as the scenes are executed only after the cell that launches the `run-scene` command is finished.
+
+
 ## Requirements
 
-* JupyterLab >= 3.0
+* JupyterLab >= 4.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab_scenes
```

### Comparing `jupyterlab_scenes-2.0.0a1/package.json` & `jupyterlab_scenes-2.0.0a2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.0.0-alpha2'"}*

```diff
@@ -81,9 +81,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0-alpha1"
+    "version": "2.0.0-alpha2"
 }
```

### Comparing `jupyterlab_scenes-2.0.0a1/pyproject.toml` & `jupyterlab_scenes-2.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/setup.py` & `jupyterlab_scenes-2.0.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/src/backend.ts` & `jupyterlab_scenes-2.0.0a2/src/backend.ts`

 * *Files 4% similar despite different names*

```diff
@@ -201,30 +201,32 @@
                 if(cell.model.type == 'code') {
                     CodeCell.execute(cell as CodeCell, notebookPanel.sessionContext, {recordTiming: notebookPanel.content.notebookConfig.recordTiming});
                 }
             }
         });
     }
 
-    createNewEmptyScene(scene_name: string) : 'success' | 'fail' {
+    createNewEmptyScene(scene_name: string, activate_new_scene=true) : 'success' | 'fail' {
         const scene_list = this.getScenesList();
         if(scene_list.includes(scene_name)) return 'fail';
 
         scene_list.push(scene_name)
         this._sceneDB.setScenesList(scene_list);
+        if(activate_new_scene) this._sceneDB.setActiveScene(scene_name);
         this._scenesChanged();
         
         return 'success'
     }
     duplicateActiveScene(new_scene_name: string): 'success' | 'fail' {
     
-        let retval = this.createNewEmptyScene(new_scene_name);
+        let retval = this.createNewEmptyScene(new_scene_name, false);
         if(retval == 'fail') return 'fail';
 
         this._duplicateSceneTagInAllCells(this._nbTracker.currentWidget!, this.getActiveScene()!, new_scene_name);
+        this._sceneDB.setActiveScene(new_scene_name);
         this._scenesChanged();
         return retval;
     }
     moveActiveSceneUp() {
         this._moveScene(this._sceneDB.getActiveScene()!, 'up');
         this._scenesChanged();
     }
@@ -278,14 +280,15 @@
         for(let n=cellIdx-1; n>=0; n--) {
             let cell = cells[n];
             if(cell.model.getMetadata(tag)) {
                 this._activateCellAndExpandParentHeadings(cell);
                 break;
             }
         }
+
     }
     importLegacyInitializationCells(notebook: Notebook) {
 
         if(!this._enableLegacyInits) return;
 
         let init_scenes_consistent = true;
         let legacy_init_cells_exist = false;
@@ -363,19 +366,19 @@
             if(init_scene_tag != null && !!cell.model.getMetadata(init_scene_tag)) {
                 cell.model.setMetadata('init_cell', true);
             } else {
                 cell.model.deleteMetadata('init_cell');
             }
         });
     }
-
     
     private _activateCellAndExpandParentHeadings(cell: Cell) {
-        NotebookActions.expandParent(cell, this._nbTracker.currentWidget!.content);
-        cell.activate();
+        let notebook = this._nbTracker.currentWidget!.content;
+        NotebookActions.expandParent(cell, notebook);
+        notebook.scrollToCell(cell).then(() => { notebook.activeCellIndex = notebook.widgets.indexOf(cell); });
     }
 
     private _moveScene(scene_name: string, direction: 'up'|'down') {
         const scenes_list = this.getScenesList();
         let idx = scenes_list.indexOf(scene_name);
         if(direction == 'down') {
             if(idx == scenes_list.length - 1) return;
@@ -529,15 +532,15 @@
 
         let data_json = (model.getMetadata(NB_METADATA_KEY) as PartialJSONObject);
         let retval = {
             scenes:        data_json['scenes'] as string[], 
             active_scene:  data_json['active_scene'] as string, 
             init_scene:    data_json['init_scene'] as string|null
         };
-        console.log('got scene data' , retval);
+
         return retval
     }
 
     private _setSceneData(scene_data: {scenes: string[], active_scene: string, init_scene: string|null}) {
         let notebook_model = this._nbTracker.currentWidget?.content.model;
         if(!notebook_model) return;
         notebook_model.setMetadata(NB_METADATA_KEY, scene_data);
```

### Comparing `jupyterlab_scenes-2.0.0a1/src/components.tsx` & `jupyterlab_scenes-2.0.0a2/src/components.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/src/index.ts` & `jupyterlab_scenes-2.0.0a2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/src/widget.tsx` & `jupyterlab_scenes-2.0.0a2/src/widget.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,23 @@
         this._app.commands.addCommand(ScenesSidebar.command_id_toggle_scene_cell, {
             label: 'Toggle Scene Cell',
             execute: () => { this._notebookHandler.toggleSceneMembershipOfSelectedCells(); }
         });
 
         this._app.commands.addCommand(ScenesSidebar.command_id_run_scene, {
             label: 'Run Scene',
-            execute: () => { this._notebookHandler.runActiveSceneInCurrentNotebook(); }
+            execute: (scene_name) => { 
+                if(typeof scene_name == "string") {   
+                    console.log('run', scene_name)
+                    this._notebookHandler.runSceneInCurrentNotebook(scene_name);
+                } else {
+                    console.log('run active')
+                    this._notebookHandler.runActiveSceneInCurrentNotebook(); 
+                }                
+            }
         });
 
         this._app.commands.addCommand(ScenesSidebar.command_id_new_empty_scene, {
             label: 'New Empty Scene',
             execute: () => { 
                 InputDialog.getText({title: 'Name of the New Scene:'}).then( (new_scene) => {
                     if(!new_scene.value) return;
```

### Comparing `jupyterlab_scenes-2.0.0a1/style/base.css` & `jupyterlab_scenes-2.0.0a2/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/tsconfig.json` & `jupyterlab_scenes-2.0.0a2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_scenes-2.0.0a1/yarn.lock` & `jupyterlab_scenes-2.0.0a2/yarn.lock`

 * *Files identical despite different names*

