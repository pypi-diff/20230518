# Comparing `tmp/ucampurestorage-1.0.1.tar.gz` & `tmp/ucampurestorage-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucampurestorage-1.0.1.tar", last modified: Mon May 15 15:29:02 2023, max compression
+gzip compressed data, was "ucampurestorage-1.0.2.tar", last modified: Thu May 18 15:57:43 2023, max compression
```

## Comparing `ucampurestorage-1.0.1.tar` & `ucampurestorage-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,250 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 15:29:02.937391 ucampurestorage-1.0.1/
--rw-rw-rw-   0        0        0       67 2023-05-05 16:24:57.000000 ucampurestorage-1.0.1/.coveragerc
--rw-rw-rw-   0        0        0       67 2023-05-05 18:40:40.000000 ucampurestorage-1.0.1/.flake8
--rw-rw-rw-   0        0        0      633 2023-05-15 15:13:48.000000 ucampurestorage-1.0.1/.gitignore
--rw-rw-rw-   0        0        0      636 2023-05-05 16:24:57.000000 ucampurestorage-1.0.1/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      112 2023-05-04 13:24:07.000000 ucampurestorage-1.0.1/Dockerfile
--rw-rw-rw-   0        0        0     1115 2023-05-05 16:24:57.000000 ucampurestorage-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    20115 2023-05-15 15:29:02.934393 ucampurestorage-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    19733 2023-05-15 13:54:36.000000 ucampurestorage-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 15:29:02.755379 ucampurestorage-1.0.1/compose/
--rw-rw-rw-   0        0        0      179 2023-05-06 11:35:00.000000 ucampurestorage-1.0.1/compose/pytest.Dockerfile
--rw-rw-rw-   0        0        0      177 2023-05-06 11:34:34.000000 ucampurestorage-1.0.1/compose/tox.Dockerfile
--rw-rw-rw-   0        0        0      165 2023-05-05 16:24:57.000000 ucampurestorage-1.0.1/compose/tox.env
--rw-rw-rw-   0        0        0      388 2023-05-05 16:24:57.000000 ucampurestorage-1.0.1/compose/tox.yml
--rw-rw-rw-   0        0        0   127824 2023-05-15 13:10:35.000000 ucampurestorage-1.0.1/pure_storage.jpg
--rw-rw-rw-   0        0        0      849 2023-05-15 14:46:51.000000 ucampurestorage-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       66 2023-05-12 15:53:22.000000 ucampurestorage-1.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       63 2023-05-15 13:55:11.000000 ucampurestorage-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 15:29:02.938383 ucampurestorage-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-05-05 19:34:06.000000 ucampurestorage-1.0.1/tox.ini
-drwxrwxrwx   0        0        0        0 2023-05-15 15:29:02.770380 ucampurestorage-1.0.1/ucampurestorage/
--rw-rw-rw-   0        0        0       79 2023-05-15 15:28:30.000000 ucampurestorage-1.0.1/ucampurestorage/__init__.py
--rw-rw-rw-   0        0        0     1441 2023-05-15 10:07:34.000000 ucampurestorage-1.0.1/ucampurestorage/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 15:29:02.886381 ucampurestorage-1.0.1/ucampurestorage/lib/
--rw-rw-rw-   0        0        0        0 2023-05-05 16:24:57.000000 ucampurestorage-1.0.1/ucampurestorage/lib/__init__.py
--rw-rw-rw-   0        0        0     2654 2023-05-05 16:24:57.000000 ucampurestorage-1.0.1/ucampurestorage/lib/httpclient.py
--rw-rw-rw-   0        0        0    38789 2023-05-15 15:26:23.000000 ucampurestorage-1.0.1/ucampurestorage/lib/options.py
--rw-rw-rw-   0        0        0    23778 2023-05-12 15:53:22.000000 ucampurestorage-1.0.1/ucampurestorage/lib/process.py
--rw-rw-rw-   0        0        0    48360 2023-05-15 10:02:11.000000 ucampurestorage-1.0.1/ucampurestorage/lib/pureconnect.py
--rw-rw-rw-   0        0        0     6216 2023-05-15 13:35:54.000000 ucampurestorage-1.0.1/ucampurestorage/lib/tokencreater.py
-drwxrwxrwx   0        0        0        0 2023-05-15 15:29:02.924387 ucampurestorage-1.0.1/ucampurestorage/tests/
--rw-rw-rw-   0        0        0        0 2023-05-05 16:24:57.000000 ucampurestorage-1.0.1/ucampurestorage/tests/__init__.py
--rw-rw-rw-   0        0        0      721 2023-05-05 18:59:22.000000 ucampurestorage-1.0.1/ucampurestorage/tests/test_httpclient.py
--rw-rw-rw-   0        0        0     7160 2023-05-05 19:04:06.000000 ucampurestorage-1.0.1/ucampurestorage/tests/test_process.py
--rw-rw-rw-   0        0        0     3435 2023-05-05 19:05:02.000000 ucampurestorage-1.0.1/ucampurestorage/tests/test_pureconnection.py
--rw-rw-rw-   0        0        0        0 2023-03-18 23:11:10.000000 ucampurestorage-1.0.1/ucampurestorage/tests/test_tasks.py
--rw-rw-rw-   0        0        0     2253 2023-05-05 19:01:18.000000 ucampurestorage-1.0.1/ucampurestorage/tests/test_tokencreater.py
-drwxrwxrwx   0        0        0        0 2023-05-15 15:29:02.846395 ucampurestorage-1.0.1/ucampurestorage.egg-info/
--rw-rw-rw-   0        0        0    20115 2023-05-15 15:29:02.000000 ucampurestorage-1.0.1/ucampurestorage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-05-15 15:29:02.000000 ucampurestorage-1.0.1/ucampurestorage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 15:29:02.000000 ucampurestorage-1.0.1/ucampurestorage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-15 15:29:02.000000 ucampurestorage-1.0.1/ucampurestorage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      109 2023-05-15 15:29:02.000000 ucampurestorage-1.0.1/ucampurestorage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 15:29:02.000000 ucampurestorage-1.0.1/ucampurestorage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:43.133458 ucampurestorage-1.0.2/
+-rw-rw-rw-   0        0        0       67 2023-05-05 16:24:57.000000 ucampurestorage-1.0.2/.coveragerc
+-rw-rw-rw-   0        0        0       67 2023-05-05 18:40:40.000000 ucampurestorage-1.0.2/.flake8
+-rw-rw-rw-   0        0        0      633 2023-05-15 15:13:48.000000 ucampurestorage-1.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1471 2023-05-18 15:32:02.000000 ucampurestorage-1.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      112 2023-05-04 13:24:07.000000 ucampurestorage-1.0.2/Dockerfile
+-rw-rw-rw-   0        0        0     1115 2023-05-05 16:24:57.000000 ucampurestorage-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    20212 2023-05-18 15:57:43.128445 ucampurestorage-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19830 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:28.040221 ucampurestorage-1.0.2/compose/
+-rw-rw-rw-   0        0        0      518 2023-05-16 16:32:36.000000 ucampurestorage-1.0.2/compose/docs.Dockerfile
+-rw-rw-rw-   0        0        0      282 2023-05-16 15:45:04.000000 ucampurestorage-1.0.2/compose/docs.yml
+-rw-rw-rw-   0        0        0       76 2023-05-16 14:21:41.000000 ucampurestorage-1.0.2/compose/docs_http.Dockerfile
+-rw-rw-rw-   0        0        0      179 2023-05-06 11:35:00.000000 ucampurestorage-1.0.2/compose/pytest.Dockerfile
+-rw-rw-rw-   0        0        0      177 2023-05-06 11:34:34.000000 ucampurestorage-1.0.2/compose/tox.Dockerfile
+-rw-rw-rw-   0        0        0      165 2023-05-05 16:24:57.000000 ucampurestorage-1.0.2/compose/tox.env
+-rw-rw-rw-   0        0        0      388 2023-05-05 16:24:57.000000 ucampurestorage-1.0.2/compose/tox.yml
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:28.648972 ucampurestorage-1.0.2/docs/
+-rw-rw-rw-   0        0        0      634 2023-05-15 16:02:06.000000 ucampurestorage-1.0.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:26.097720 ucampurestorage-1.0.2/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:28.856131 ucampurestorage-1.0.2/docs/_build/doctrees/
+-rw-rw-rw-   0        0        0     5454 2023-05-18 15:01:27.000000 ucampurestorage-1.0.2/docs/_build/doctrees/changelog.doctree
+-rw-rw-rw-   0        0        0   217487 2023-05-18 15:16:59.000000 ucampurestorage-1.0.2/docs/_build/doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     5361 2023-05-18 15:01:27.000000 ucampurestorage-1.0.2/docs/_build/doctrees/index.doctree
+-rw-rw-rw-   0        0        0     2774 2023-05-15 17:59:10.000000 ucampurestorage-1.0.2/docs/_build/doctrees/modules.doctree
+-rw-rw-rw-   0        0        0    47975 2023-05-18 15:01:29.000000 ucampurestorage-1.0.2/docs/_build/doctrees/readme.doctree
+-rw-rw-rw-   0        0        0     3364 2023-05-15 17:06:37.000000 ucampurestorage-1.0.2/docs/_build/doctrees/readme_link.doctree
+-rw-rw-rw-   0        0        0     4245 2023-05-18 15:01:29.000000 ucampurestorage-1.0.2/docs/_build/doctrees/ucampurestorage.doctree
+-rw-rw-rw-   0        0        0   392846 2023-05-18 15:16:59.000000 ucampurestorage-1.0.2/docs/_build/doctrees/ucampurestorage.lib.doctree
+-rw-rw-rw-   0        0        0    82637 2023-05-18 15:01:52.000000 ucampurestorage-1.0.2/docs/_build/doctrees/ucampurestorage.tests.doctree
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:29.146387 ucampurestorage-1.0.2/docs/_build/html/
+-rw-rw-rw-   0        0        0      234 2023-05-18 15:17:04.000000 ucampurestorage-1.0.2/docs/_build/html/.buildinfo
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:29.363729 ucampurestorage-1.0.2/docs/_build/html/_images/
+-rw-rw-rw-   0        0        0   127824 2023-05-15 13:10:35.000000 ucampurestorage-1.0.2/docs/_build/html/_images/pure_storage.jpg
+-rw-rw-rw-   0        0        0   127824 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/docs/_build/html/_images/pure_storage1.jpg
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:29.529051 ucampurestorage-1.0.2/docs/_build/html/_modules/
+-rw-rw-rw-   0        0        0     4582 2023-05-18 15:17:04.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/index.html
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:26.136405 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:31.427296 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/lib/
+-rw-rw-rw-   0        0        0    17201 2023-05-15 16:12:17.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/lib/httpclient.html
+-rw-rw-rw-   0        0        0   163281 2023-05-18 15:17:03.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/lib/options.html
+-rw-rw-rw-   0        0        0   111137 2023-05-18 15:02:00.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/lib/process.html
+-rw-rw-rw-   0        0        0   230807 2023-05-18 15:02:00.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/lib/pureconnect.html
+-rw-rw-rw-   0        0        0    27904 2023-05-15 16:12:17.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/lib/tokencreater.html
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:32.484234 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/tests/
+-rw-rw-rw-   0        0        0     7945 2023-05-15 16:12:17.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/tests/test_httpclient.html
+-rw-rw-rw-   0        0        0    39942 2023-05-15 16:12:17.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/tests/test_process.html
+-rw-rw-rw-   0        0        0    20551 2023-05-15 16:12:17.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/tests/test_pureconnection.html
+-rw-rw-rw-   0        0        0    13295 2023-05-15 16:12:17.000000 ucampurestorage-1.0.2/docs/_build/html/_modules/ucampurestorage/tests/test_tokencreater.html
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:32.730051 ucampurestorage-1.0.2/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0      314 2023-05-18 14:57:51.000000 ucampurestorage-1.0.2/docs/_build/html/_sources/changelog.rst.txt
+-rw-rw-rw-   0        0        0      593 2023-05-18 14:58:52.000000 ucampurestorage-1.0.2/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0       89 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-rw-   0        0        0    20306 2023-05-18 14:49:34.000000 ucampurestorage-1.0.2/docs/_build/html/_sources/readme.rst.txt
+-rw-rw-rw-   0        0        0       54 2023-05-15 17:06:29.000000 ucampurestorage-1.0.2/docs/_build/html/_sources/readme_link.rst.txt
+-rw-rw-rw-   0        0        0     1142 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/_build/html/_sources/ucampurestorage.lib.rst.txt
+-rw-rw-rw-   0        0        0      291 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/_build/html/_sources/ucampurestorage.rst.txt
+-rw-rw-rw-   0        0        0     1266 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/_build/html/_sources/ucampurestorage.tests.rst.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:34.160185 ucampurestorage-1.0.2/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0    15597 2023-05-18 15:17:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/basic.css
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:34.590982 ucampurestorage-1.0.2/docs/_build/html/_static/css/
+-rw-rw-rw-   0        0        0     3229 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:35.979951 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   444379 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   135235 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/css/theme.css
+-rw-rw-rw-   0        0        0    10766 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/_build/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      435 2023-05-18 15:17:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2023-05-15 16:00:53.000000 ucampurestorage-1.0.2/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0   287630 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/_build/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0        0        0    89476 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/_build/html/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:36.051719 ucampurestorage-1.0.2/docs/_build/html/_static/js/
+-rw-rw-rw-   0        0        0      934 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4370 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2734 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/js/theme.js
+-rw-rw-rw-   0        0        0    11151 2023-05-18 15:17:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2023-05-15 16:00:53.000000 ucampurestorage-1.0.2/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0     4467 2023-05-15 16:33:42.000000 ucampurestorage-1.0.2/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
+-rw-rw-rw-   0        0        0     6878 2023-05-15 17:41:56.000000 ucampurestorage-1.0.2/docs/_build/html/_static/nbsphinx-code-cells.css
+-rw-rw-rw-   0        0        0      584 2023-05-15 16:33:42.000000 ucampurestorage-1.0.2/docs/_build/html/_static/nbsphinx-gallery.css
+-rw-rw-rw-   0        0        0     2871 2023-05-15 16:33:42.000000 ucampurestorage-1.0.2/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
+-rw-rw-rw-   0        0        0       90 2023-05-15 16:00:53.000000 ucampurestorage-1.0.2/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4892 2023-05-18 15:17:04.000000 ucampurestorage-1.0.2/docs/_build/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    16634 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/_build/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0     4712 2023-05-15 16:00:53.000000 ucampurestorage-1.0.2/docs/_build/html/_static/sphinx_highlight.js
+-rw-rw-rw-   0        0        0    68420 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/_build/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    19530 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/_build/html/_static/underscore.js
+-rw-rw-rw-   0        0        0     5062 2023-05-18 15:01:57.000000 ucampurestorage-1.0.2/docs/_build/html/changelog.html
+-rw-rw-rw-   0        0        0    40545 2023-05-18 15:17:02.000000 ucampurestorage-1.0.2/docs/_build/html/genindex.html
+-rw-rw-rw-   0        0        0     6382 2023-05-18 15:17:01.000000 ucampurestorage-1.0.2/docs/_build/html/index.html
+-rw-rw-rw-   0        0        0     7722 2023-05-18 15:01:58.000000 ucampurestorage-1.0.2/docs/_build/html/modules.html
+-rw-rw-rw-   0        0        0     1660 2023-05-18 15:17:05.000000 ucampurestorage-1.0.2/docs/_build/html/objects.inv
+-rw-rw-rw-   0        0        0     7287 2023-05-18 15:17:02.000000 ucampurestorage-1.0.2/docs/_build/html/py-modindex.html
+-rw-rw-rw-   0        0        0    96514 2023-05-18 15:01:58.000000 ucampurestorage-1.0.2/docs/_build/html/readme.html
+-rw-rw-rw-   0        0        0     3848 2023-05-15 17:06:37.000000 ucampurestorage-1.0.2/docs/_build/html/readme_link.html
+-rw-rw-rw-   0        0        0     4038 2023-05-18 15:17:04.000000 ucampurestorage-1.0.2/docs/_build/html/search.html
+-rw-rw-rw-   0        0        0    16387 2023-05-18 15:17:04.000000 ucampurestorage-1.0.2/docs/_build/html/searchindex.js
+-rw-rw-rw-   0        0        0     8395 2023-05-18 15:17:01.000000 ucampurestorage-1.0.2/docs/_build/html/ucampurestorage.html
+-rw-rw-rw-   0        0        0   141877 2023-05-18 15:17:02.000000 ucampurestorage-1.0.2/docs/_build/html/ucampurestorage.lib.html
+-rw-rw-rw-   0        0        0    44963 2023-05-18 15:01:59.000000 ucampurestorage-1.0.2/docs/_build/html/ucampurestorage.tests.html
+-rw-rw-rw-   0        0        0      314 2023-05-18 14:57:51.000000 ucampurestorage-1.0.2/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1148 2023-05-15 17:58:36.000000 ucampurestorage-1.0.2/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:26.190644 ucampurestorage-1.0.2/docs/docs/
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:26.199193 ucampurestorage-1.0.2/docs/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:36.315268 ucampurestorage-1.0.2/docs/docs/_build/html/
+-rw-rw-rw-   0        0        0      234 2023-05-15 20:41:43.000000 ucampurestorage-1.0.2/docs/docs/_build/html/.buildinfo
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:36.463007 ucampurestorage-1.0.2/docs/docs/_build/html/.doctrees/
+-rw-rw-rw-   0        0        0    46948 2023-05-15 20:41:38.000000 ucampurestorage-1.0.2/docs/docs/_build/html/.doctrees/README.doctree
+-rw-rw-rw-   0        0        0   204982 2023-05-15 20:41:40.000000 ucampurestorage-1.0.2/docs/docs/_build/html/.doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     5344 2023-05-15 20:41:38.000000 ucampurestorage-1.0.2/docs/docs/_build/html/.doctrees/index.doctree
+-rw-rw-rw-   0        0        0     2774 2023-05-15 20:41:38.000000 ucampurestorage-1.0.2/docs/docs/_build/html/.doctrees/modules.doctree
+-rw-rw-rw-   0        0        0     4245 2023-05-15 20:41:38.000000 ucampurestorage-1.0.2/docs/docs/_build/html/.doctrees/ucampurestorage.doctree
+-rw-rw-rw-   0        0        0   379116 2023-05-15 20:41:40.000000 ucampurestorage-1.0.2/docs/docs/_build/html/.doctrees/ucampurestorage.lib.doctree
+-rw-rw-rw-   0        0        0    82637 2023-05-15 20:41:40.000000 ucampurestorage-1.0.2/docs/docs/_build/html/.doctrees/ucampurestorage.tests.doctree
+-rw-rw-rw-   0        0        0    96064 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/README.html
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:36.475538 ucampurestorage-1.0.2/docs/docs/_build/html/_images/
+-rw-rw-rw-   0        0        0   127824 2023-05-15 13:10:35.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_images/pure_storage.jpg
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:36.497215 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/
+-rw-rw-rw-   0        0        0     4483 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/index.html
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:26.257545 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:36.595306 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/lib/
+-rw-rw-rw-   0        0        0    17340 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/lib/httpclient.html
+-rw-rw-rw-   0        0        0   150084 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/lib/options.html
+-rw-rw-rw-   0        0        0   102915 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/lib/process.html
+-rw-rw-rw-   0        0        0   219304 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/lib/pureconnect.html
+-rw-rw-rw-   0        0        0    28043 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/lib/tokencreater.html
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:36.679304 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/tests/
+-rw-rw-rw-   0        0        0     8084 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/tests/test_httpclient.html
+-rw-rw-rw-   0        0        0    40081 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/tests/test_process.html
+-rw-rw-rw-   0        0        0    20690 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/tests/test_pureconnection.html
+-rw-rw-rw-   0        0        0    13434 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_modules/ucampurestorage/tests/test_tokencreater.html
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:36.826076 ucampurestorage-1.0.2/docs/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0    20124 2023-05-15 18:08:33.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_sources/README.rst.txt
+-rw-rw-rw-   0        0        0      579 2023-05-15 20:28:50.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0       89 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-rw-   0        0        0     1142 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_sources/ucampurestorage.lib.rst.txt
+-rw-rw-rw-   0        0        0      291 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_sources/ucampurestorage.rst.txt
+-rw-rw-rw-   0        0        0     1266 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_sources/ucampurestorage.tests.rst.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:37.113973 ucampurestorage-1.0.2/docs/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0    15597 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/basic.css
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:37.144195 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/
+-rw-rw-rw-   0        0        0     3229 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/badge_only.css
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:37.501151 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/
+-rw-rw-rw-   0        0        0    87624 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-rw-   0        0        0    67312 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-rw-   0        0        0    86288 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-rw-   0        0        0    66444 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-rw-   0        0        0   165742 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   444379 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0   323344 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-rw-   0        0        0   193308 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-rw-   0        0        0   309728 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-rw-   0        0        0   184912 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-rw-   0        0        0   328412 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-rw-   0        0        0   195704 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-rw-   0        0        0   309192 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-rw-   0        0        0   182708 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-rw-   0        0        0   135235 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/css/theme.css
+-rw-rw-rw-   0        0        0    10766 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      435 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0   287630 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0        0        0    89476 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/jquery.js
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:38.442294 ucampurestorage-1.0.2/docs/docs/_build/html/_static/js/
+-rw-rw-rw-   0        0        0      934 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/js/badge_only.js
+-rw-rw-rw-   0        0        0     4370 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-rw-   0        0        0     2734 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/js/html5shiv.min.js
+-rw-rw-rw-   0        0        0     5023 2023-05-15 16:01:04.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/js/theme.js
+-rw-rw-rw-   0        0        0    11151 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4892 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    16634 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0    68420 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    19530 2023-05-15 17:16:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/_static/underscore.js
+-rw-rw-rw-   0        0        0    38570 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/genindex.html
+-rw-rw-rw-   0        0        0     6333 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/index.html
+-rw-rw-rw-   0        0        0     7626 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/modules.html
+-rw-rw-rw-   0        0        0     1572 2023-05-15 20:41:43.000000 ucampurestorage-1.0.2/docs/docs/_build/html/objects.inv
+-rw-rw-rw-   0        0        0     7191 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/py-modindex.html
+-rw-rw-rw-   0        0        0     3942 2023-05-15 20:41:42.000000 ucampurestorage-1.0.2/docs/docs/_build/html/search.html
+-rw-rw-rw-   0        0        0    15734 2023-05-15 20:41:43.000000 ucampurestorage-1.0.2/docs/docs/_build/html/searchindex.js
+-rw-rw-rw-   0        0        0     8299 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/ucampurestorage.html
+-rw-rw-rw-   0        0        0   133119 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/ucampurestorage.lib.html
+-rw-rw-rw-   0        0        0    44612 2023-05-15 20:41:41.000000 ucampurestorage-1.0.2/docs/docs/_build/html/ucampurestorage.tests.html
+-rw-rw-rw-   0        0        0      593 2023-05-18 14:58:52.000000 ucampurestorage-1.0.2/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2023-05-15 16:02:06.000000 ucampurestorage-1.0.2/docs/make.bat
+-rw-rw-rw-   0        0        0       89 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/modules.rst
+-rw-rw-rw-   0        0        0   127824 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/docs/pure_storage.jpg
+-rw-rw-rw-   0        0        0    20306 2023-05-18 14:49:34.000000 ucampurestorage-1.0.2/docs/readme.rst
+-rw-rw-rw-   0        0        0     1142 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/ucampurestorage.lib.rst
+-rw-rw-rw-   0        0        0      291 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/ucampurestorage.rst
+-rw-rw-rw-   0        0        0     1266 2023-05-15 16:08:42.000000 ucampurestorage-1.0.2/docs/ucampurestorage.tests.rst
+-rw-rw-rw-   0        0        0   127824 2023-05-15 13:10:35.000000 ucampurestorage-1.0.2/pure_storage.jpg
+-rw-rw-rw-   0        0        0      849 2023-05-15 14:46:51.000000 ucampurestorage-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-05-16 00:48:51.000000 ucampurestorage-1.0.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       63 2023-05-15 13:55:11.000000 ucampurestorage-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 15:57:43.139183 ucampurestorage-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-05-05 19:34:06.000000 ucampurestorage-1.0.2/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:39.947380 ucampurestorage-1.0.2/ucampurecli/
+-rw-rw-rw-   0        0        0     2544 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/ucampurecli/pure_clone_volume.sh
+-rw-rw-rw-   0        0        0     3049 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/ucampurecli/pure_create_snapshot.sh
+-rw-rw-rw-   0        0        0     2620 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/ucampurecli/pure_create_volume.sh
+-rw-rw-rw-   0        0        0     2476 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/ucampurecli/pure_delete_volume.sh
+-rw-rw-rw-   0        0        0     4925 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/ucampurecli/pure_eradicate_destroyed_volume.sh
+-rw-rw-rw-   0        0        0     2102 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/ucampurecli/pure_record_destoyed_volume.sh
+-rw-rw-rw-   0        0        0     3274 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/ucampurecli/pure_replace_volume.sh
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:40.324617 ucampurestorage-1.0.2/ucampurestorage/
+-rw-rw-rw-   0        0        0       79 2023-05-18 14:33:40.000000 ucampurestorage-1.0.2/ucampurestorage/__init__.py
+-rw-rw-rw-   0        0        0     1441 2023-05-15 10:07:34.000000 ucampurestorage-1.0.2/ucampurestorage/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:43.006366 ucampurestorage-1.0.2/ucampurestorage/lib/
+-rw-rw-rw-   0        0        0        0 2023-05-05 16:24:57.000000 ucampurestorage-1.0.2/ucampurestorage/lib/__init__.py
+-rw-rw-rw-   0        0        0     2654 2023-05-05 16:24:57.000000 ucampurestorage-1.0.2/ucampurestorage/lib/httpclient.py
+-rw-rw-rw-   0        0        0    42695 2023-05-18 15:15:19.000000 ucampurestorage-1.0.2/ucampurestorage/lib/options.py
+-rw-rw-rw-   0        0        0    25595 2023-05-18 14:27:50.000000 ucampurestorage-1.0.2/ucampurestorage/lib/process.py
+-rw-rw-rw-   0        0        0    51422 2023-05-18 14:42:59.000000 ucampurestorage-1.0.2/ucampurestorage/lib/pureconnect.py
+-rw-rw-rw-   0        0        0     6216 2023-05-15 13:35:54.000000 ucampurestorage-1.0.2/ucampurestorage/lib/tokencreater.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:43.113906 ucampurestorage-1.0.2/ucampurestorage/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-05 16:24:57.000000 ucampurestorage-1.0.2/ucampurestorage/tests/__init__.py
+-rw-rw-rw-   0        0        0      721 2023-05-05 18:59:22.000000 ucampurestorage-1.0.2/ucampurestorage/tests/test_httpclient.py
+-rw-rw-rw-   0        0        0     7160 2023-05-05 19:04:06.000000 ucampurestorage-1.0.2/ucampurestorage/tests/test_process.py
+-rw-rw-rw-   0        0        0     3435 2023-05-05 19:05:02.000000 ucampurestorage-1.0.2/ucampurestorage/tests/test_pureconnection.py
+-rw-rw-rw-   0        0        0        0 2023-03-18 23:11:10.000000 ucampurestorage-1.0.2/ucampurestorage/tests/test_tasks.py
+-rw-rw-rw-   0        0        0     2253 2023-05-05 19:01:18.000000 ucampurestorage-1.0.2/ucampurestorage/tests/test_tokencreater.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:57:41.713182 ucampurestorage-1.0.2/ucampurestorage.egg-info/
+-rw-rw-rw-   0        0        0    20212 2023-05-18 15:57:21.000000 ucampurestorage-1.0.2/ucampurestorage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9189 2023-05-18 15:57:26.000000 ucampurestorage-1.0.2/ucampurestorage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:57:21.000000 ucampurestorage-1.0.2/ucampurestorage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-18 15:57:21.000000 ucampurestorage-1.0.2/ucampurestorage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-05-18 15:57:21.000000 ucampurestorage-1.0.2/ucampurestorage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 15:57:21.000000 ucampurestorage-1.0.2/ucampurestorage.egg-info/top_level.txt
```

### Comparing `ucampurestorage-1.0.1/.gitignore` & `ucampurestorage-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/LICENSE` & `ucampurestorage-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/PKG-INFO` & `ucampurestorage-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: ucampurestorage
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pure Storage module for the utilization in Cambridge University
 Author-email: Ishan Mahajan <imahajan0007@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-PURE STORAGE
-==============
-![Pure Storage](./pure_storage.jpg "Pure Storage logo")
+# UCAM PURE STORAGE 
+![Pure Storage](pure_storage.jpg "Pure Storage logo")
 
+###### [Module Document](http://ifs-test-client1.srv.uis.private.cam.ac.uk:8080/index.html)
 
-# Introduction
+### Introduction
 The CLI developed in this project allows the user to interact with PureStorage using REST API.
 
 
 With this CLI, you can list the existing volumes, servers, etc, on the Dell SCs, clone volumes, create snapshots, replace existing volumes with a golden image, etc. It is also able to configure system /etc/fstab and multipath when needed in some operations like volume mapping and mounting.
 
-## Running the Application
+### Running the Application
 
 #### Prerequisites
 * [requests 2.30.0](https://pypi.org/project/requests/2.30.0/)
 * [pyjwt](https://pypi.org/project/PyJWT/2.7.0/)[[crypto]](https://pypi.org/project/cryptography/40.0.2/)
 * [paramiko 3.1.0](https://pypi.org/project/paramiko/3.1.0/)
 * [distro 1.8.0](https://pypi.org/project/distro/1.8.0/)
 
 Download the private key from the 1PASSWORD utilized to create the API account on the purestorage and fetch the credentials required.
 1. Pure Storage Arrays [user and passowrd]
 2. PureAPI information [client_id, key_id, client_name, storage, keyfile]
 
-## Installation
+### Installation
 To install the ucampurestorage pip package
 
 ```
 pip3 install ucampurestorage
 ```
 
 CLI
 The help shows how to use ucampurestorage.
+
 ```
     usage: __main__.py [-h] [-v] [--storage STORAGE] [--port PORT] [--client_id CLIENT_ID] [--key_id KEY_ID] [--client_name CLIENT_NAME] [--user USER] [--password PASSWORD] [--is_secure IS_SECURE]
                    [--record_config RECORD_CONFIG] [--file FILE] [--keyfile KEYFILE]
                    {tokengen,list,volume,host,snapshot} ...
 
     Manage Pure Storage Manager objects via REST API.
 
@@ -70,69 +71,81 @@
     --password PASSWORD   Pure Storage password
     --is_secure IS_SECURE
                             Secure connection. Default: False
     --record_config RECORD_CONFIG
                             Record multipath and file system config details. Default: False (do not record system config details)
     --file FILE           Read arguments from json file
     --keyfile KEYFILE     path to private keys inorder to generate token for the API call
+
 ```
 
 For instance to get the list of volumes:
 
 ```
+
     python -m ucampurestorage  --client_id "25********************************0d" --key_id "f**************************************d" --client_nam "apitest" --user "pureuser" --password "****" --keyfile "/tmp/fa2xprivate.pem" list --object volumes
     05/15/2023 13:15:09 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
-````
+
+```
 
 You get prompt for client_id, key_id, client_name, storage, user, keyfile, password
+
 ```
+
     ucampurestorage  list --object volumes
     Username: pureuser
     Client ID: 25********************************0d
     Key ID: f**************************************d
     Client Name: apitest
     Private file location: /tmp/fa2xprivate.pem
     Password:
     05/15/2023 13:15:09 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
+
 ```
 
 The CLI can also read arguments from the a json file:
+
 ```
+
     {
     "client_id": "25********************************0d",
     "key_id": "f**************************************d",
     "client_name": "apitest",
     "storage": "purestorage.cam.ac.uk",
     "user": "pureuser",
     "password": "********,
     "keyfile": "/tmp/fa2xprivate.pem"
     }
+
 ```
 
+
 To use a config file, use the option --file:
+
 ```
+
     ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object volumes
     05/15/2023 13:09:11 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:09:11 [INFO] [Command succeeded - Returns True]
+
 ```
 
-Application logging
-====================
+#### Application logging
 Logs generated by cli are located in /var/log/ucampurestorage/
```

### Comparing `ucampurestorage-1.0.1/README.md` & `ucampurestorage-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-PURE STORAGE
-==============
-![Pure Storage](./pure_storage.jpg "Pure Storage logo")
+# UCAM PURE STORAGE 
+![Pure Storage](pure_storage.jpg "Pure Storage logo")
 
+###### [Module Document](http://ifs-test-client1.srv.uis.private.cam.ac.uk:8080/index.html)
 
-# Introduction
+### Introduction
 The CLI developed in this project allows the user to interact with PureStorage using REST API.
 
 
 With this CLI, you can list the existing volumes, servers, etc, on the Dell SCs, clone volumes, create snapshots, replace existing volumes with a golden image, etc. It is also able to configure system /etc/fstab and multipath when needed in some operations like volume mapping and mounting.
 
-## Running the Application
+### Running the Application
 
 #### Prerequisites
 * [requests 2.30.0](https://pypi.org/project/requests/2.30.0/)
 * [pyjwt](https://pypi.org/project/PyJWT/2.7.0/)[[crypto]](https://pypi.org/project/cryptography/40.0.2/)
 * [paramiko 3.1.0](https://pypi.org/project/paramiko/3.1.0/)
 * [distro 1.8.0](https://pypi.org/project/distro/1.8.0/)
 
 Download the private key from the 1PASSWORD utilized to create the API account on the purestorage and fetch the credentials required.
 1. Pure Storage Arrays [user and passowrd]
 2. PureAPI information [client_id, key_id, client_name, storage, keyfile]
 
-## Installation
+### Installation
 To install the ucampurestorage pip package
 
 ```
 pip3 install ucampurestorage
 ```
 
 CLI
 The help shows how to use ucampurestorage.
+
 ```
     usage: __main__.py [-h] [-v] [--storage STORAGE] [--port PORT] [--client_id CLIENT_ID] [--key_id KEY_ID] [--client_name CLIENT_NAME] [--user USER] [--password PASSWORD] [--is_secure IS_SECURE]
                    [--record_config RECORD_CONFIG] [--file FILE] [--keyfile KEYFILE]
                    {tokengen,list,volume,host,snapshot} ...
 
     Manage Pure Storage Manager objects via REST API.
 
@@ -59,69 +60,81 @@
     --password PASSWORD   Pure Storage password
     --is_secure IS_SECURE
                             Secure connection. Default: False
     --record_config RECORD_CONFIG
                             Record multipath and file system config details. Default: False (do not record system config details)
     --file FILE           Read arguments from json file
     --keyfile KEYFILE     path to private keys inorder to generate token for the API call
+
 ```
 
 For instance to get the list of volumes:
 
 ```
+
     python -m ucampurestorage  --client_id "25********************************0d" --key_id "f**************************************d" --client_nam "apitest" --user "pureuser" --password "****" --keyfile "/tmp/fa2xprivate.pem" list --object volumes
     05/15/2023 13:15:09 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
-````
+
+```
 
 You get prompt for client_id, key_id, client_name, storage, user, keyfile, password
+
 ```
+
     ucampurestorage  list --object volumes
     Username: pureuser
     Client ID: 25********************************0d
     Key ID: f**************************************d
     Client Name: apitest
     Private file location: /tmp/fa2xprivate.pem
     Password:
     05/15/2023 13:15:09 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
+
 ```
 
 The CLI can also read arguments from the a json file:
+
 ```
+
     {
     "client_id": "25********************************0d",
     "key_id": "f**************************************d",
     "client_name": "apitest",
     "storage": "purestorage.cam.ac.uk",
     "user": "pureuser",
     "password": "********,
     "keyfile": "/tmp/fa2xprivate.pem"
     }
+
 ```
 
+
 To use a config file, use the option --file:
+
 ```
+
     ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object volumes
     05/15/2023 13:09:11 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:09:11 [INFO] [Command succeeded - Returns True]
+
 ```
 
-Application logging
-====================
+#### Application logging
 Logs generated by cli are located in /var/log/ucampurestorage/
```

### Comparing `ucampurestorage-1.0.1/pure_storage.jpg` & `ucampurestorage-1.0.2/docs/_build/html/_images/pure_storage.jpg`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/pyproject.toml` & `ucampurestorage-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/tox.ini` & `ucampurestorage-1.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/ucampurestorage/__main__.py` & `ucampurestorage-1.0.2/ucampurestorage/__main__.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/ucampurestorage/lib/httpclient.py` & `ucampurestorage-1.0.2/ucampurestorage/lib/httpclient.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/ucampurestorage/lib/options.py` & `ucampurestorage-1.0.2/ucampurestorage/lib/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import logging
 import getpass
 from argparse import ArgumentParser, ArgumentTypeError, Action
 from ucampurestorage.lib.tokencreater import TokenCreater as token
 from ucampurestorage.lib.pureconnect import PureConnection as PureStorage
 from ucampurestorage.lib.pureconnect import PureAdvanceConnection as PureAdvance
+from ucampurestorage.lib.process import Process
 from ucampurestorage import VERSION
 
 LOG = logging.getLogger(__name__)
 
 
 class LoadFromFile(Action):
     def __call__(self, parser, namespace, values, option_string=None):
@@ -29,14 +30,15 @@
         return False
     else:
         raise ArgumentTypeError("Boolean value expected.")
 
 
 class Options:
     def __init__(self):
+        self.process = Process()
         self._init_parser()
 
     def _init_parser(self):
         """Define arguments for the CLI."""
         self.parser = ArgumentParser(
             description="Manage Pure Storage Manager objects via REST API."
         )
@@ -106,14 +108,15 @@
             "--object",
             required=True,
             choices=[
                 "arrays",
                 "controllers",
                 "hosts",
                 "volumes",
+                "destroyed_volumes",
                 "volumegroups",
                 "hostgroups",
                 "volumesnapshots",
                 "targetports",
                 "networkports",
                 "volumeconnections",
                 "protectiongroups",
@@ -161,16 +164,36 @@
         self.deletevol = self.volumeoperation.add_parser("delete", help="delete Volume")
         self.deletevol.add_argument(
             "--name",
             required=True,
             help="Name of the volume to be deleted on Pure Array.",
         )
         self.deletevol.add_argument(
-            "-nop", "--no_prompt", required=False, action="store_true"
+            "-nop",
+            "--no_prompt",
+            required=False,
+            action="store_true",
+            help="No prompt of validation for deletion of volume.",
+        )
+        self.eradicatevol = self.volumeoperation.add_parser(
+            "eradicate", help="eradicate Volume"
+        )
+        self.eradicatevol.add_argument(
+            "--name",
+            required=True,
+            help="Name of the volume to be eradicate on Pure Array.",
+        )
+        self.eradicatevol.add_argument(
+            "-nop",
+            "--no_prompt",
+            required=False,
+            action="store_true",
+            help="No prompt of validation for eradicate of volume.",
         )
+
         self.connectvol = self.volumeoperation.add_parser(
             "connect", help="Connect Volume to Host"
         )
         self.connectvol.add_argument(
             "--hostname",
             required=True,
             help="Name of the host specified on Pure Array for initiators to which the volume has to be mapped.",
@@ -207,14 +230,21 @@
         )
         self.mapvol.add_argument(
             "--mp",
             required=False,
             help="OPTIONAL. If specified, it is the path of the mountpoint \
                                             to mount the volume on. Otherwise, no mount attempt will take place.",
         )
+        self.mapvol.add_argument(
+            "-new",
+            "--new_volume",
+            required=False,
+            action="store_true",
+            help="NOTE: If volume is create but never formated then use this flag",
+        )
         self.unmapvol = self.volumeoperation.add_parser(
             "unmap",
             help="Unmaps the volume from local server and \
                                                       Volume must be unmounted.",
         )
         self.unmapvol.add_argument(
             "--name",
@@ -317,15 +347,19 @@
         self.deletehost = self.hostoperation.add_parser("delete", help="delete host")
         self.deletehost.add_argument(
             "--name",
             required=True,
             help="Name of the host to be deleted on Pure Array.",
         )
         self.deletehost.add_argument(
-            "-nop", "--no_prompt", required=False, action="store_true"
+            "-nop",
+            "--no_prompt",
+            required=False,
+            action="store_true",
+            help="No prompt of validation for deletion of host.",
         )
         self.parser_snapshot_operations = self.subparsers.add_parser(
             "snapshot", help="Operations with respect to snapshots in the Pure objects."
         )
         self.snapoperation = self.parser_snapshot_operations.add_subparsers(
             dest="snapoperation"
         )
@@ -389,15 +423,24 @@
         }
 
         _checkuserparms(check_dict)
 
         if self.known.password is None:
             self.known.password = getpass.getpass()
 
+        # If enabled, record system config before running ucamdsm command
+        if self.known.record_config:
+            self.process.record_config_details()
+
         result = run_option(self.known.subparser, self.known)
+
+        # If enabled, record system config after running ucamdsm command
+        if self.known.record_config:
+            self.process.record_config_details()
+
         return result
 
 
 def _token_object(args):
     token_obj = token()
     if token_obj.current_token is None:
         if hasattr(args, "outputfile"):
@@ -427,14 +470,15 @@
 
 def create_token(args):
     """
     Generate Pure Storage token.
 
     Example: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
         --client_name=<ClientName> --keyfile="privatekey.pem"  tokengen
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  tokengen
     """
     token_obj = _token_object(args)
     LOG.info(f"\nAccess token for {args.client_name}:\n\n{token_obj.current_token}")
 
 
 def run_option(subparser, args):
@@ -455,18 +499,20 @@
     return subcommand_func(args) if subcommand_func is not None else None
 
 
 def list_object(args):
     """
     List Pure Storage objects.
 
-    Example: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
-        --client_name=<ClientName> --keyfile=".\\privatekey.pem" list --object controllers
-    Example: ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object controllers
-    Example: ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object controllers --format=json
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+        --client_name=<ClientName> --keyfile="privatekey.pem" list --object controllers
+
+    Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object controllers
+
+    Example 3: ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object controllers --format=json
     """
     token_obj = _token_object(args)
     PureObj = PureStorage(
         args.storage,
         args.port,
         args.user,
         args.password,
@@ -488,40 +534,43 @@
 
 
 def volume_operations(args):
     """
     Perform Pure Storage volume level Operations.
 
     Example: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
-        --client_name=<ClientName> --keyfile="privatekey.pem"  volume {list,create,delete,connect,\
+        --client_name=<ClientName> --keyfile="privatekey.pem"  volume {list,create,delete,eradicate,connect,\
                                         disconnect,map,unmap,replace,clone}
-    Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume {list,create,delete,\
+
+    Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume {list,create,delete,eradicate,\
                                         connect,disconnect,map,unmap,replace,clone}
     """
     volume_operations = {
         "list": detail_volume,
         "create": create_volume,
         "connect": connect_volume,
         "disconnect": disconnect_volume,
         "map": map_volume,
         "unmap": unmap_volume,
         "delete": delete_volume,
         "replace": replace_volume,
         "clone": clone_volume,
+        "eradicate": eradicate_volume,
     }
     subcommand_func = volume_operations.get(args.volumeoperation)
     return subcommand_func(args) if subcommand_func is not None else None
 
 
 def host_operations(args):
     """
     Perform Pure Storage host level Operations.
 
     Example: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
         --client_name=<ClientName> --keyfile="privatekey.pem"  host {list,create,delete}
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  host {list,create,delete}
     """
     host_operations = {
         "list": detail_host,
         "create": create_host,
         "delete": delete_host,
     }
@@ -529,16 +578,17 @@
     return subcommand_func(args) if subcommand_func is not None else None
 
 
 def snap_operations(args):
     """
     Perform Pure Storage Snapshot level Operations.
 
-    Example: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
         --client_name=<ClientName> --keyfile="privatekey.pem"  snapshot {list,create,delete}
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  snapshot {list,create,delete}
     """
     snap_operations = {
         "list": list_snapshots,
         "create": create_snapshot,
         "delete": delete_snapshot,
     }
@@ -548,15 +598,17 @@
 
 def detail_host(args):
     """
     List the detail information of the host connected to the  Pure Storage.
 
     Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem"  host  list  --name cs-dev-db2
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  host list --name cs-dev-db2
+
     Example 3: ucampurestorage --file=./ucampurestorage/lib/secrets.json  host list --name cs-dev-db2 --format=json
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
@@ -582,14 +634,15 @@
 
 def create_host(args):
     """Create host defination on the Purestorage.
 
     Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem"  host  create  --name <HOSTNAME> --iqn <IQN number>\
             --personality <aix,esxi,hpux,solaris,vms,oracle-vm-server,none>
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json host create --name <HOSTNAME> \
             --iqn <IQN number> --personality <aix,esxi,hpux,solaris,vms,oracle-vm-server,none>
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
@@ -609,14 +662,15 @@
 
 
 def delete_host(args):
     """Delete host defination on the Pure Storage.
 
     Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem"  host  delete  --name <HOSTNAME>
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json host delete --name <HOSTNAME>
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
@@ -655,17 +709,19 @@
         return result
 
 
 def detail_volume(args):
     """
     List the detail information of the volume from the  Pure Storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
         --client_name=<ClientName> --keyfile="privatekey.pem"  volume  list  --name TEST113
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume list  --name TEST113
+
     Example 3: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume list  --name TEST113 --format=json
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
@@ -688,16 +744,17 @@
         )
         return result
 
 
 def create_volume(args):
     """Create Volume on the Pure storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
         --client_name=<ClientName> --keyfile="privatekey.pem"  volume  create  --name TEST113 --size 1T
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume create  --name TEST113 --size 1T
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
@@ -712,16 +769,17 @@
         LOG.error(f"Failure in {args.name} created")
     return result
 
 
 def delete_volume(args):
     """Delete Volume from the Pure storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
         --client_name=<ClientName> --keyfile="privatekey.pem"  volume  delete  --name TEST113
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume delete  --name TEST113
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
@@ -755,25 +813,75 @@
         if result:
             LOG.info(f"Successfully {args.name} deleted !!")
         else:
             LOG.error(f"Failed in deletion of Volume : {args.name}")
         return result
 
 
+def eradicate_volume(args):
+    """eradicate Volume from the Pure storage.
+
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
+        --client_name=<ClientName> --keyfile="privatekey.pem"  volume  eradicate  --name TEST113
+
+    Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume eradicate  --name TEST113
+    """
+    token_obj = _token_object(args)
+    PureObj = PureAdvance(
+        args.storage,
+        args.port,
+        args.user,
+        args.password,
+        token_obj.current_token,
+        args.is_secure,
+    )
+    if not args.no_prompt:
+        valid_inputs = ["y", "yes", "n", "no"]
+        invalid = True
+        while invalid:
+            validate_eradicate = input(
+                f"Are you sure you want to delete {args.name} [Y/N](yes/no) : "
+            )
+            user_entry = validate_eradicate.lower()
+            if user_entry in valid_inputs and user_entry in valid_inputs[:2]:
+                result = PureObj.eradicate_volume(args.name)
+                if result:
+                    LOG.info(f"Successfully {args.name} eradicated !!")
+                    invalid = False
+                else:
+                    LOG.error(f"Failed in Eradication of Volume : {args.name}")
+                return result
+            elif user_entry in valid_inputs and user_entry in valid_inputs[2:]:
+                LOG.warning(f"Eradication of {args.name} has been cancelled !!")
+                invalid = False
+            else:
+                LOG.error(f"{user_entry} is invalid input")
+    else:
+        result = PureObj.eradicate_volume(args.name)
+        if result:
+            LOG.info(f"Successfully {args.name} eradicated !!")
+        else:
+            LOG.error(f"Failed in Eradication of Volume : {args.name}")
+        return result
+
+
 def connect_volume(args):
     """Connect Volume to the host on the Pure storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
         --client_name=<ClientName> --keyfile="privatekey.pem"  volume  connect --hostname HOST01 --volname TEST113
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume connect  \
         --hostname HOST01 --volname TEST113
+
     [optionally define the LUNID]
-    Example 3: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 3: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
         --client_name=<ClientName> --keyfile="privatekey.pem"  volume  connect --hostname HOST01 --volname \
             TEST113 --lunid 77
+
     Example 4: ucampurestorage --file=./ucampurestorage/lib/secrets.json  volume connect  --hostname HOST01 \
         --volname TEST113  --lunid 77
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
@@ -791,16 +899,17 @@
         )
     return result
 
 
 def disconnect_volume(args):
     """Disconnect Volume from the host on the Pure storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem"  volume  disconnect --hostname HOST01 --volname TEST113
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json volume disconnect \
             --hostname HOST01 --volname TEST113
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
@@ -820,16 +929,17 @@
         )
     return result
 
 
 def replace_volume(args):
     """Replace the mounted clone volume with new clone from Pure storage and mount to the local server.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem" volume replace --src_mp /t1  --dst_mp /t2
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json volume replace --src_mp /t1  --dst_mp /t2
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
@@ -844,17 +954,18 @@
         LOG.error(f"failed the replace the volume {args.src_mp} with {args.dst_mp}")
     return result
 
 
 def clone_volume(args):
     """Clone volume on Pure storage and mount to the local server.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem" volume clone --name TEST113_clone --srcvol \
             TEST113 --target_mp /t2
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json volume clone --name TEST113_clone \
         --srcvol TEST113 --target_mp /t2
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
@@ -874,17 +985,19 @@
     return result
 
 
 def list_snapshots(args):
     """
     List the detail information of the snapshot from the  Pure Storage.
 
-    Example: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem"  snapshot list --volname TEST12
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  snapshot list --volname TEST12
+
     Example 3: ucampurestorage --file=./ucampurestorage/lib/secrets.json  snapshot list --volname TEST12  --format=json
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
@@ -906,16 +1019,17 @@
         )
     return result
 
 
 def create_snapshot(args):
     """Create snapshot of the volume on the Pure storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem" snapshot create --srcvol TEST113 --suffix snap01
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  snapshot create \
             --srcvol TEST113 --suffix snap01
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
@@ -935,16 +1049,17 @@
         )
     return result
 
 
 def delete_snapshot(args):
     """Delete snapshot of the volume on the Pure storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem" snapshot delete --snapname TEST113.snap01
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json  snapshot delete --snapname TEST113.snap01
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
@@ -959,44 +1074,56 @@
         LOG.error(f"Failure in deletion of the snapshot : {args.snapname}")
     return result
 
 
 def map_volume(args):
     """Map volume to the local server which  is provided by Pure storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
         --client_name=<ClientName> --keyfile="privatekey.pem" volume map --name TEST113 --mp /t2
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json volume map --name TEST113 --mp /t2
+
+    [NOTE: New volume need to be formated therefore -new flag is required]
+
+    Example 3: ucampurestorage --file=./ucampurestorage/lib/secrets.json volume map --name TEST113_new --mp /t2 -new
+
+    Example 4: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd> \
+        --client_name=<ClientName> --keyfile="privatekey.pem" volume map --name TEST113 --mp /t2 -new
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
         args.password,
         token_obj.current_token,
         args.is_secure,
     )
-    result = PureObj.map_volume(args.name, args.mp)
+    result = PureObj.map_volume(args.name, args.mp, args.new_volume)
     if result:
         LOG.info(f"mapping of {args.name} to mountpoint {args.mp}")
     else:
         LOG.error(f"Fail in mapping of {args.name} to mountpoint {args.mp}")
     return result
 
 
 def unmap_volume(args):
     """Map volume to the local server which  is provided by Pure storage.
 
-    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+    Example 1: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
         --client_name=<ClientName> --keyfile="privatekey.pem" volume unmap --name TEST113
+
     Example 2: ucampurestorage --file=./ucampurestorage/lib/secrets.json volume unmap --name TEST113
-    [optionally define the LUNID]
-    Example 3: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>
+
+    [optionally define the WWN]
+
+    Example 3: ucampurestorage --client_id=<clientID> --key_id=<KeyID> --user=<User> --password=<passwd>\
         --client_name=<ClientName> --keyfile="privatekey.pem" volume unmap --wwn <WWN number>
+
     Example 4: ucampurestorage --file=./ucampurestorage/lib/secrets.json volume unmap --wwn <WWN number>
     """
     token_obj = _token_object(args)
     PureObj = PureAdvance(
         args.storage,
         args.port,
         args.user,
```

### Comparing `ucampurestorage-1.0.1/ucampurestorage/lib/process.py` & `ucampurestorage-1.0.2/ucampurestorage/lib/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -737,7 +737,72 @@
         content = None
         try:
             content = open(filename).read()
         except Exception as e:
             LOG.error("Cannot read %s. Error: %s", filename, e)
 
         return content
+
+    def is_dir_exist(self, path):
+        """
+        Checks if a directory is exists.
+
+        :param path: path of the directory to check.
+        :returns: `True` if the directory, `False` otherwise.
+        """
+        return Path(path).exists()
+
+    def create_dir(self, path):
+        """
+        Create a directory if provided.
+
+        :returns: `True` for success, `False` for error.
+        """
+        if self.is_dir_exist(path):
+            LOG.error(f'Directory "{path}" alreay exists.')
+            return False
+        cmd = f"mkdir {path}"
+        result = self.run(cmd)
+
+        return True if result[0] == 0 else False
+
+    def create_partition(self, dev: str) -> bool:
+        """Create partition on the dev.
+
+        Args:
+            dev (str): multipath dev path
+
+        Returns:
+            bool: TRUE if dev is partitioned
+        """
+        cmd = f"sgdisk -n 1:0:0 {dev}"
+        result = self.run(cmd)
+
+        return True if result[0] == 0 else False
+
+    def update_system_partition(self, part: str) -> bool:
+        """Update about the partition to the local system.
+
+        Args:
+            part (str): partition name crated on the local system.
+
+        Returns:
+            bool: TRUE if partition is updated
+        """
+        cmd = f"kpartx -a {part}"
+        result = self.run(cmd)
+
+        return True if result[0] == 0 else False
+
+    def format_partition_with_ext4(self, part: str) -> bool:
+        """Format the partition with ext4.
+
+        Args:
+            part (str): partition name crated on the local system.
+
+        Returns:
+            bool: TRUE if partition is updated
+        """
+        cmd = f"mkfs.ext4 {part}"
+        result = self.run(cmd)
+
+        return True if result[0] == 0 else False
```

### Comparing `ucampurestorage-1.0.1/ucampurestorage/lib/pureconnect.py` & `ucampurestorage-1.0.2/ucampurestorage/lib/pureconnect.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         self.networkports = None
         self.volumeconnections = None
         self.protectiongroups = None
         self.protectiongroupsnapshots = None
         self.protectiongroupvolmembers = None
         self.pods = None
         self.remotepods = None
+        self.destroyed_volume = None
 
     def _get_json(self, blob):
         """
         Returns a dict from the JSON of a REST response.
 
         :param blob: The response from a REST call.
         :returns: JSON or None on error.
@@ -101,14 +102,15 @@
         :return: couple of (result of object get function, object data structure)
         """
         function_switcher = {
             "arrays": (self.get_arrays, "arrays"),
             "controllers": (self.get_controllers, "controllers"),
             "hosts": (self.get_hosts, "hosts"),
             "volumes": (self.get_volumes, "volumes"),
+            "destroyed_volumes": (self.get_vol_destroyed, "destroyed_volumes"),
             "volumegroups": (self.get_volumegroups, "volumegroups"),
             "hostgroups": (self.get_hostgroups, "hostgroups"),
             "volumesnapshots": (self.get_volumesnapshots, "volumesnapshots"),
             "targetports": (self.get_targetports, "targetports"),
             "networkports": (self.get_networkports, "networkports"),
             "volumeconnections": (self.get_volumeconnections, "volumeconnections"),
             "protectiongroups": (self.get_protectiongroups, "protectiongroups"),
@@ -698,14 +700,25 @@
         fetch_all_vol = self.get_volumes()
         if fetch_all_vol:
             for key, value in self.volumes.items():
                 if value["serial"].lower() == wwn[-24:].lower():
                     return key
             return False
 
+    def get_vol_destroyed(self):
+        self.destroyed_volumes = {}
+        fetch_all_vol = self.get_volumes()
+        if fetch_all_vol:
+            for name, info in self.volumes.items():
+                if self.volumes[name]["destroyed"]:
+                    self.destroyed_volumes[name] = info
+            return True
+        else:
+            return False
+
 
 class SystemTask(PureConnection):
     def __init__(
         self, host: any, port: int, user: str, password: any, token: any, verify: bool
     ):
         super().__init__(host, port, user, password, token, verify)
         self.process = Process()
@@ -816,14 +829,32 @@
             "destroyed": True,
         }
         response = self.client.patch(path, data)
         if not self._check_result(response):
             return False
         return True
 
+    def eradicate_volume(self, name: str) -> bool:
+        """Eradicate volume.
+
+        Args:
+            name (str): Name of the volume to be eradicate on PureStorage Array
+
+        Returns:
+            boolean: `True` for success, `False` on error.
+        """
+        path = "/volumes"
+        data = {
+            "names": name,
+        }
+        response = self.client.delete(path, data)
+        if not self._check_result(response):
+            return False
+        return True
+
     def connect_volume(self, hostname: str, volname: str, **kwargs) -> bool:
         """Connect volume.
 
         Args:
             hostname (str): Name of the host specified on PureStorage Array with which volume need to be connect
             volname (str): Name of the volume specified on PureStorage Array which need to be connect
 
@@ -859,20 +890,21 @@
             "volume_names": volname,
         }
         response = self.client.delete(path, data)
         if not self._check_result(response):
             return False
         return True
 
-    def map_volume(self, name, mountpoint=None):
+    def map_volume(self, name, mountpoint=None, new_vol=False):
         """Map volume to local server and mount it to `mountpoint`.
 
         Args:
             name (str): Name of the volume to map to local server.
-            mountpoint (str): Name of the volume to be deleted on PureStorage Array
+            mountpoint (str): Name of the mountpoint on local server to be mounted
+            new_vol (bool): Is the volume name newly created in PureStorage Array
 
         Returns:
             boolean: `True` for success, `False` on error.
         """
         # check if the volume exist
         volume_exist = self.get_volumes(name)
         if not volume_exist:
@@ -919,35 +951,61 @@
         if not self.process.add_multipath_alias(wwn):
             return False
 
         # reload multipath
         if not self.process.reload_multipathd():
             return False
 
-        # if a mountpoint is specified, update fstab file and mount the volume
+        # if mountpoint is not specified then nothing to do
         if mountpoint is None:
             LOG.info("Mountpoint is not specified.")
             return True
 
+        # if mountpoint specified doesn't exist then make directory
+        if not self.process.is_dir_exist(mountpoint):
+            if not self.process.create_dir(mountpoint):
+                LOG.error(f"Direcory {mountpoint} creation failed")
+                return False
+
+        # if a mountpoint is specified, update fstab file and mount the volume
+        # If the volume is new then partition and create the directory id not already created\
+        #  for specified mountpoint
         new_alias = self.process.get_mpath_from_wwn(wwn)
         if new_alias is not None:
+            new_dev = f"/dev/mapper/{new_alias}"
             new_fsdevice = f"/dev/mapper/{new_alias}p1"
+
+            # if the new volume is created and never formated
+            if new_vol:
+                # create partion
+                if not self.process.create_partition(new_dev):
+                    LOG.error(f"partion creation failed for {new_dev}")
+                    return False
+                if not self.process.update_system_partition(new_dev):
+                    LOG.error(f"Partition of system not updated: {new_dev}")
+                    return False
+                # Format partition to the ext4
+                if not self.process.format_partition_with_ext4(new_fsdevice):
+                    LOG.error(f"Formating of the Partition failed: {new_fsdevice}")
+                    return False
+
             if not self.process.add_entry_in_fstab(new_fsdevice, mountpoint):
                 LOG.error("%s cannot be added to /etc/fstab", new_fsdevice)
                 return False
             if not self.process.daemon_reload():
                 return False
         else:
             LOG.error("Alias for the volume with WWN %s does not exist.", mountpoint)
             return False
 
         # mount target_mountpoint if it's not mounted
         # found it gets mounted after reload multipath, is it an expected behaviour?
         if not self.process.mountpoint_exists(mountpoint):
             if not self.process.mount(mountpoint):
+                LOG.error('Mount operation has failed. Use "-new" for new volume')
                 return False
 
         return True
 
     def unmap_volume(self, name=None, wwn=None):
         """
         Unmaps a Pure Storage volume with `WWN`. Unmounting the volume should be performed manually.
@@ -1205,28 +1263,40 @@
         """
         path = "/volumes"
         data = {
             "names": cln_name,
             "source": {"name": src_name},
         }
 
+        # check if the volume name of source exist
+        volume_exist = self.get_volumes(src_name)
+        if not volume_exist or self.volumes is None:
+            LOG.error(f'Source volume "{src_name}" is not present on Array')
+            return False
+
         # check if the volume name of clone exist
         volume_exist = self.get_volumes(cln_name)
         if volume_exist and self.volumes is not None:
             LOG.error(f'Clone volume "{cln_name}" already exists')
             return False
 
         # if mt_pt is provided then check otherwise create the clone volume
         if mt_pt:
+            # Check the provided mointpoint is already created, if not created then create.
+            if not self.process.is_dir_exist(mt_pt):
+                LOG.info(f'"{mt_pt}" was not present so, created new dir "{mt_pt}"')
+                self.process.create_dir(mt_pt)
+
             # Check the provided mountpoint is empty
             if not self.process.is_dir_empty(mt_pt):
                 return False
 
             # Check the provided mountpoint exist
             if self.process.mountpoint_exists(mt_pt):
+                LOG.error(f'Specified Target mountpoint "{mt_pt}" is already mounted')
                 return False
 
         # Create clone of the volume
         response = self.client.post(path, data)
         if not self._check_result(response):
             return False
```

### Comparing `ucampurestorage-1.0.1/ucampurestorage/lib/tokencreater.py` & `ucampurestorage-1.0.2/ucampurestorage/lib/tokencreater.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/ucampurestorage/tests/test_httpclient.py` & `ucampurestorage-1.0.2/ucampurestorage/tests/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/ucampurestorage/tests/test_process.py` & `ucampurestorage-1.0.2/ucampurestorage/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/ucampurestorage/tests/test_pureconnection.py` & `ucampurestorage-1.0.2/ucampurestorage/tests/test_pureconnection.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/ucampurestorage/tests/test_tokencreater.py` & `ucampurestorage-1.0.2/ucampurestorage/tests/test_tokencreater.py`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.1/ucampurestorage.egg-info/PKG-INFO` & `ucampurestorage-1.0.2/ucampurestorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: ucampurestorage
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pure Storage module for the utilization in Cambridge University
 Author-email: Ishan Mahajan <imahajan0007@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-PURE STORAGE
-==============
-![Pure Storage](./pure_storage.jpg "Pure Storage logo")
+# UCAM PURE STORAGE 
+![Pure Storage](pure_storage.jpg "Pure Storage logo")
 
+###### [Module Document](http://ifs-test-client1.srv.uis.private.cam.ac.uk:8080/index.html)
 
-# Introduction
+### Introduction
 The CLI developed in this project allows the user to interact with PureStorage using REST API.
 
 
 With this CLI, you can list the existing volumes, servers, etc, on the Dell SCs, clone volumes, create snapshots, replace existing volumes with a golden image, etc. It is also able to configure system /etc/fstab and multipath when needed in some operations like volume mapping and mounting.
 
-## Running the Application
+### Running the Application
 
 #### Prerequisites
 * [requests 2.30.0](https://pypi.org/project/requests/2.30.0/)
 * [pyjwt](https://pypi.org/project/PyJWT/2.7.0/)[[crypto]](https://pypi.org/project/cryptography/40.0.2/)
 * [paramiko 3.1.0](https://pypi.org/project/paramiko/3.1.0/)
 * [distro 1.8.0](https://pypi.org/project/distro/1.8.0/)
 
 Download the private key from the 1PASSWORD utilized to create the API account on the purestorage and fetch the credentials required.
 1. Pure Storage Arrays [user and passowrd]
 2. PureAPI information [client_id, key_id, client_name, storage, keyfile]
 
-## Installation
+### Installation
 To install the ucampurestorage pip package
 
 ```
 pip3 install ucampurestorage
 ```
 
 CLI
 The help shows how to use ucampurestorage.
+
 ```
     usage: __main__.py [-h] [-v] [--storage STORAGE] [--port PORT] [--client_id CLIENT_ID] [--key_id KEY_ID] [--client_name CLIENT_NAME] [--user USER] [--password PASSWORD] [--is_secure IS_SECURE]
                    [--record_config RECORD_CONFIG] [--file FILE] [--keyfile KEYFILE]
                    {tokengen,list,volume,host,snapshot} ...
 
     Manage Pure Storage Manager objects via REST API.
 
@@ -70,69 +71,81 @@
     --password PASSWORD   Pure Storage password
     --is_secure IS_SECURE
                             Secure connection. Default: False
     --record_config RECORD_CONFIG
                             Record multipath and file system config details. Default: False (do not record system config details)
     --file FILE           Read arguments from json file
     --keyfile KEYFILE     path to private keys inorder to generate token for the API call
+
 ```
 
 For instance to get the list of volumes:
 
 ```
+
     python -m ucampurestorage  --client_id "25********************************0d" --key_id "f**************************************d" --client_nam "apitest" --user "pureuser" --password "****" --keyfile "/tmp/fa2xprivate.pem" list --object volumes
     05/15/2023 13:15:09 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
-````
+
+```
 
 You get prompt for client_id, key_id, client_name, storage, user, keyfile, password
+
 ```
+
     ucampurestorage  list --object volumes
     Username: pureuser
     Client ID: 25********************************0d
     Key ID: f**************************************d
     Client Name: apitest
     Private file location: /tmp/fa2xprivate.pem
     Password:
     05/15/2023 13:15:09 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
+
 ```
 
 The CLI can also read arguments from the a json file:
+
 ```
+
     {
     "client_id": "25********************************0d",
     "key_id": "f**************************************d",
     "client_name": "apitest",
     "storage": "purestorage.cam.ac.uk",
     "user": "pureuser",
     "password": "********,
     "keyfile": "/tmp/fa2xprivate.pem"
     }
+
 ```
 
+
 To use a config file, use the option --file:
+
 ```
+
     ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object volumes
     05/15/2023 13:09:11 [INFO] List of volumes:
     ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
     05/15/2023 13:09:11 [INFO] [Command succeeded - Returns True]
+
 ```
 
-Application logging
-====================
+#### Application logging
 Logs generated by cli are located in /var/log/ucampurestorage/
```

