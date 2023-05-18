# Comparing `tmp/mly_pipeline-0.3.1.2.tar.gz` & `tmp/mly_pipeline-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.3.1.2.tar", last modified: Fri May 12 11:19:42 2023, max compression
+gzip compressed data, was "mly_pipeline-0.4.tar", last modified: Thu May 18 09:26:30 2023, max compression
```

## Comparing `mly_pipeline-0.3.1.2.tar` & `mly_pipeline-0.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.366246 mly_pipeline-0.3.1.2/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      101 2023-05-11 15:58:46.000000 mly_pipeline-0.3.1.2/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-10 09:58:07.000000 mly_pipeline-0.3.1.2/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:08.000000 mly_pipeline-0.3.1.2/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6683 2023-05-12 11:19:42.365246 mly_pipeline-0.3.1.2/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.3.1.2/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:41.756240 mly_pipeline-0.3.1.2/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.2/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:41.632239 mly_pipeline-0.3.1.2/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.056243 mly_pipeline-0.3.1.2/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2070494 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6320 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13735 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    66958 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    72638 2023-05-04 11:10:20.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.107244 mly_pipeline-0.3.1.2/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.110244 mly_pipeline-0.3.1.2/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.3.1.2/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.117244 mly_pipeline-0.3.1.2/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.212245 mly_pipeline-0.3.1.2/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15205 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9799 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1139 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      419 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3121 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7025 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9665 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1490 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.2/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27021 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3424 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21120 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26724 2023-05-04 11:10:20.000000 mly_pipeline-0.3.1.2/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.221245 mly_pipeline-0.3.1.2/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5971 2023-05-04 11:02:00.000000 mly_pipeline-0.3.1.2/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2708 2023-05-04 11:22:06.000000 mly_pipeline-0.3.1.2/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14708 2023-05-04 11:18:26.000000 mly_pipeline-0.3.1.2/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13712 2023-05-04 11:10:15.000000 mly_pipeline-0.3.1.2/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.237245 mly_pipeline-0.3.1.2/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      727 2023-05-10 09:44:52.000000 mly_pipeline-0.3.1.2/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    26455 2023-05-04 09:25:08.000000 mly_pipeline-0.3.1.2/mly_pipeline/continious_FAR.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25296 2023-05-12 11:18:19.000000 mly_pipeline-0.3.1.2/mly_pipeline/initialization.py
--rwxrwxrwx   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-10 09:57:38.000000 mly_pipeline-0.3.1.2/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22791 2023-05-11 14:52:48.000000 mly_pipeline-0.3.1.2/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5939 2023-04-14 10:51:44.000000 mly_pipeline-0.3.1.2/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    20321 2023-05-04 09:19:17.000000 mly_pipeline-0.3.1.2/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16260 2023-05-04 12:51:13.000000 mly_pipeline-0.3.1.2/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35533 2023-05-11 10:45:05.000000 mly_pipeline-0.3.1.2/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.363246 mly_pipeline-0.3.1.2/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.3.1.2/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-05-10 09:05:55.000000 mly_pipeline-0.3.1.2/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.244245 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6683 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2594 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      134 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      699 2023-05-12 11:19:24.000000 mly_pipeline-0.3.1.2/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-05-12 11:19:42.366246 mly_pipeline-0.3.1.2/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.472821 mly_pipeline-0.4/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      101 2023-05-16 13:28:31.000000 mly_pipeline-0.4/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-16 13:29:19.000000 mly_pipeline-0.4/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-16 13:28:31.000000 mly_pipeline-0.4/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6679 2023-05-18 09:26:30.471821 mly_pipeline-0.4/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.4/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.368820 mly_pipeline-0.4/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.4/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.357820 mly_pipeline-0.4/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.390820 mly_pipeline-0.4/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.4/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.4/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2070494 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6320 2023-05-04 11:02:10.000000 mly_pipeline-0.4/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13735 2023-05-04 11:02:10.000000 mly_pipeline-0.4/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    66958 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    72638 2023-05-04 11:10:20.000000 mly_pipeline-0.4/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.411821 mly_pipeline-0.4/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.414821 mly_pipeline-0.4/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.4/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.419821 mly_pipeline-0.4/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.444821 mly_pipeline-0.4/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15205 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9799 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1139 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      419 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.4/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.4/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.4/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3121 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7025 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9665 2023-05-04 11:02:10.000000 mly_pipeline-0.4/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1490 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.4/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27021 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3424 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21120 2023-05-04 11:18:30.000000 mly_pipeline-0.4/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26724 2023-05-04 11:10:20.000000 mly_pipeline-0.4/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.450821 mly_pipeline-0.4/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5971 2023-05-04 11:02:00.000000 mly_pipeline-0.4/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.4/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2708 2023-05-04 11:22:06.000000 mly_pipeline-0.4/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14708 2023-05-04 11:18:26.000000 mly_pipeline-0.4/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13712 2023-05-04 11:10:15.000000 mly_pipeline-0.4/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.461821 mly_pipeline-0.4/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      726 2023-05-12 12:55:33.000000 mly_pipeline-0.4/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    26641 2023-05-16 14:05:59.000000 mly_pipeline-0.4/mly_pipeline/continuous_FAR.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26705 2023-05-17 13:41:02.000000 mly_pipeline-0.4/mly_pipeline/initialization.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-16 13:28:31.000000 mly_pipeline-0.4/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22792 2023-05-16 13:28:31.000000 mly_pipeline-0.4/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5939 2023-05-16 13:28:31.000000 mly_pipeline-0.4/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    20322 2023-05-16 13:28:31.000000 mly_pipeline-0.4/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16261 2023-05-16 13:28:31.000000 mly_pipeline-0.4/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35491 2023-05-16 13:28:31.000000 mly_pipeline-0.4/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.470821 mly_pipeline-0.4/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.4/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-05-16 13:28:31.000000 mly_pipeline-0.4/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-18 09:26:30.468821 mly_pipeline-0.4/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6679 2023-05-18 09:26:30.000000 mly_pipeline-0.4/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2594 2023-05-18 09:26:30.000000 mly_pipeline-0.4/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-05-18 09:26:30.000000 mly_pipeline-0.4/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      194 2023-05-18 09:26:30.000000 mly_pipeline-0.4/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-05-18 09:26:30.000000 mly_pipeline-0.4/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-05-18 09:26:30.000000 mly_pipeline-0.4/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      759 2023-05-18 09:26:06.000000 mly_pipeline-0.4/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-05-18 09:26:30.472821 mly_pipeline-0.4/setup.cfg
```

### Comparing `mly_pipeline-0.3.1.2/.gitlab-ci.yml` & `mly_pipeline-0.4/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     - .python:pytest
   stage: test
   needs: [build]
   variables:
     # we're installing from the tarball, so we don't need the git repo
     GIT_STRATEGY: none
     # use the tarball we got from 'build'
-    INSTALL_TARGET: "mly-pipeline-*.tar.*"
+    INSTALL_TARGET: "mly_pipeline-*.tar.*"
     # point pytest at the installed package
-    PYTEST_OPTIONS: "--pyargs mly-pipeline"
+    PYTEST_OPTIONS: "--pyargs mly_pipeline"
 
 # actually run the tests for each python version we support
 test:3.7:
   extends: [.test]
   image: python:3.7
 
 test:3.9:
```

### Comparing `mly_pipeline-0.3.1.2/LICENSE` & `mly_pipeline-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/PKG-INFO` & `mly_pipeline-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.3.1.2
+Version: 0.4
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.3.1.2/README.md` & `mly_pipeline-0.4/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/Makefile` & `mly_pipeline-0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.4/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.4/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/environment.pickle` & `mly_pipeline-0.4/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.4/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.4/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/index.doctree` & `mly_pipeline-0.4/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.4/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/runningasearch.doctree` & `mly_pipeline-0.4/docs/build/doctrees/runningasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/doctrees/settingupasearch.doctree` & `mly_pipeline-0.4/docs/build/doctrees/settingupasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/Getting Started.html` & `mly_pipeline-0.4/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/GettingStarted.html` & `mly_pipeline-0.4/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/How to use.html` & `mly_pipeline-0.4/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/HowToUse.html` & `mly_pipeline-0.4/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/Installation.html` & `mly_pipeline-0.4/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_modules/index.html` & `mly_pipeline-0.4/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_modules/io.html` & `mly_pipeline-0.4/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.4/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.4/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.4/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.4/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.4/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.4/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/basic.css` & `mly_pipeline-0.4/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.4/docs/build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.4/docs/build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.4/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.4/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/doctools.js` & `mly_pipeline-0.4/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.4/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/jquery.js` & `mly_pipeline-0.4/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/language_data.js` & `mly_pipeline-0.4/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/pygments.css` & `mly_pipeline-0.4/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.4/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.4/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/underscore.js` & `mly_pipeline-0.4/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/_static/websupport.js` & `mly_pipeline-0.4/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/genindex.html` & `mly_pipeline-0.4/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/gettingstarted.html` & `mly_pipeline-0.4/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/howtouse.html` & `mly_pipeline-0.4/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/index.html` & `mly_pipeline-0.4/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/installation.html` & `mly_pipeline-0.4/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/objects.inv` & `mly_pipeline-0.4/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/py-modindex.html` & `mly_pipeline-0.4/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/runningasearch.html` & `mly_pipeline-0.4/docs/build/html/runningasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/search.html` & `mly_pipeline-0.4/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/searchindex.js` & `mly_pipeline-0.4/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/build/html/settingupasearch.html` & `mly_pipeline-0.4/docs/build/html/settingupasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/source/conf.py` & `mly_pipeline-0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/source/index.rst` & `mly_pipeline-0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/source/installation.rst` & `mly_pipeline-0.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/source/runningasearch.rst` & `mly_pipeline-0.4/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/docs/source/settingupasearch.rst` & `mly_pipeline-0.4/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/__init__.py` & `mly_pipeline-0.4/mly_pipeline/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with MLY.  If not, see <http://www.gnu.org/licenses/>.
 
 """mly-pipeline.
-"""
+"""
```

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/continious_FAR.py` & `mly_pipeline-0.4/mly_pipeline/continuous_FAR.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,20 +107,25 @@
 
 
 if mode == 'inference':
 
     import tensorflow as tf
     from tensorflow.keras.models import load_model
 
-    # our hermes imports
-    from hermes import quiver as qv
-    from hermes.aeriel.client import InferenceClient
-    from hermes.aeriel.serve import serve
-#    from hermes.stillwater import ServerMonitor
-
+    try:
+        # our hermes imports
+        from hermes import quiver as qv
+        from hermes.aeriel.client import InferenceClient
+        from hermes.aeriel.serve import serve
+    except Exception as e:
+        print(f"Exception for importing hermes from environment: {e}")
+        sys.path.append("/home/vasileios.skliris/hermes/hermes")
+        from hermes import quiver as qv
+        from hermes.aeriel.client import InferenceClient
+        from hermes.aeriel.serve import serve
 
 
 
 
 def dataToQueue(dataSet_Q, dataSetName_Q): # Depricated until Hermes issue solved
 
     already_used=[]
@@ -373,30 +378,28 @@
 
             error = config["falseAlarmRates"]+"/condor/"+file[:-4]+"_DAG"+'/error'
             output = config["falseAlarmRates"]+"/condor/"+file[:-4]+"_DAG"+'/output'
             log = config["falseAlarmRates"]+"/condor/"+file[:-4]+"_DAG"+'/log'
             submit = config["falseAlarmRates"]+"/condor/"+file[:-4]+"_DAG"+'/submit'
 
             dagman = Dagman(name=file[:-4]+"_DAG",submit=submit)
-
-            os.system('chmod 777 '+config['mlyPipelineSource']+'/continious_FAR.py')
             
             job_list=[]
 
             for batch in np.arange(batches):
 
                 jobname = file[:-4]+"_"+str(batch)
 
 
                 thearguments = ("--mode=sub_generation" 
                                 +" --dataSet="+file
                                 +" --batchNumber="+str(batch))
 
                 job = Job(name = jobname
-                        ,executable = config['mlyPipelineSource']+"/continious_FAR.py"
+                        ,executable = "python -m mly_pipeline.continuous_FAR"
                         ,arguments = thearguments
                         ,submit=submit
                         ,error=error
                         ,output=output
                         ,log=log
                         ,getenv=True
                         ,dag=dagman
```

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/initialization.py` & `mly_pipeline-0.4/mly_pipeline/initialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,30 +116,28 @@
         if dir in path_to_connect.split('/'):
             common_part.append(dir)
         else:
             break
 
     common_part = '/'.join(common_part)
 
-    print(common_part)
-
     new_path_to_change = path_to_change.split(common_part)
     
     return '..'+new_path_to_change[-1]
 
 def createRunAllScript(**kwargs):
     
     """ Creating a script called runall.sh that withing the search director will
     run and manage all the scripts needed for the search.
     """
         
     with open(kwargs['path'] + '/' + 'runall.sh','w') as f:
         
         # Sourcing mlyPipeline module
-        f.write("source=" + kwargs['mlyPipelineSource'] + "\n")
+        #f.write("source=" + kwargs['mlyPipelineSource'] + "\n")
         
         # Things to write only if OFFLINE mode is active 
         # (OFFLINE is not complete)
         if "OFFLINE" not in kwargs['search_mode']:
             
             # Loop that checks the state of the jobs and doesn't stop
             f.write("while true" + "\n")
@@ -153,28 +151,28 @@
             # !Note: If you change this from the config, you will have to 
             #        edit in the runall.sh script by hand.
             f.write("   STEP="+str(kwargs['parallel_scripts'])+ "\n\n")
             
             # Lopp to run the scripts for the search
             f.write("   for INITIAL in `seq 0 $(($STEP-1))`" + "\n")
             f.write("   do" + "\n\n")
-            f.write("       nohup python $source/search.py"
+            f.write("       nohup python -m mly_pipeline.search.py"
                             +" --splitter [$STEP,$INITIAL]"
                             +" --time_reference $unixtime" 
-                            +" &> search_step_$INITIAL.out & processID+=($(echo $!))" + "\n\n")
+                            +" &> search_step_$INITIAL.out & processID+=($(echo $!)) ; echo $!>>.jobids.txt" + "\n\n")
             f.write("   done" + "\n\n\n")
         
             # Script that runs the manager script
-            f.write("   nohup python $source/manager.py &> manager.out & processID+=($(echo $!))" + "\n")
+            f.write("   nohup python -m mly_pipeline.manager &> manager.out & processID+=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
             
             # If the search runs as expected by default, it will also run scripts
             # for generating timelags and running FAR tests.
             if kwargs['search_mode'] not in ["O3MDC" , 'BENCHMARK_MDC_OFFLINE']:
-                f.write("   nohup python $source/continuous_FAR.py --mode generation &> continuous_FAR_generation.out & processID+=($(echo $!))" + "\n")
-                f.write("   nohup python $source/continuous_FAR.py --mode inference &> continuous_FAR_inference.out & inferenceID=($(echo $!))" + "\n")
+                f.write("   nohup python -m mly_pipeline.continuous_FAR --mode generation &> continuous_FAR_generation.out & processID+=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
+                f.write("   nohup python -m mly_pipeline.continuous_FAR --mode inference &> continuous_FAR_inference.out & inferenceID=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
             
             # # # Maintenance of jobs 
             
             # If total_failure becomes 1, the script runs everything from scratch
             f.write("    total_failure=0" + "\n")
             
             # Sometimes the FAR script might stal indefinetly for unknow reasons
@@ -228,41 +226,41 @@
                 # In case inference script gets killed or we have at least 5 minutes
                 # of staling, we restart inference script. Although, we keep the 
                 # corresponding unix time it got killed in the name of the  output
                 # file.
                 f.write("        if ! ps $inferenceID > /dev/null || [ $staling_points -gt 5 ]"+ "\n")
                 f.write("        then" + "\n")
                 f.write("            singularity instance stop --all" + "\n")
-                f.write("            nohup python $source/continuous_FAR.py --mode inference >"
+                f.write("            nohup python -m mly_pipeline.continuous_FAR --mode inference >"
                                     +" continuous_FAR_inference_$(date +%s).out 2>&1"
-                                    +" & inferenceID=($(echo $!))" + "\n")
+                                    +" & inferenceID=($(echo $!)) ; echo $!>>.jobids.txt" + "\n")
                 f.write("        fi" + "\n")
 
                     
             f.write("   done" + "\n")
                     
             # If the previous loop exits, it means there was a total_failure=1
             # So we will have to rerun everything. But first we kill the python
             # scripts (inference included).
             # !Note: We are not remove any condor jobs from the lag generation
             #        script because they do not interfere with the scripts.
             f.write("   for pid in \"${processID[@]}\"" + "\n")
             f.write("   do" + "\n")
             f.write("       kill $pid" + "\n")
             f.write("   done" + "\n")
-                    
+            
             if kwargs['search_mode'] not in ["O3MDC" , 'BENCHMARK_MDC_OFFLINE']:
                 f.write("   kill $inferenceID" + "\n")
                 f.write("   singularity instance stop --all" + "\n")
 
             f.write("done" + "\n")
         
         # Currently the offline script is very simple (under developement)
         else:
-            f.write("nohup python $source/offline_search.py &> search.out &" + "\n\n")
+            f.write("nohup python -m mly_pipeline.offline_search &> search.out & ; echo $!>>.jobids.txt" + "\n\n")
 
 
 
 def main():
     
     kwargs = _parser()
 
@@ -301,15 +299,15 @@
         
         os.system("mkdir "+kwargs['path'])
         
     else:
         raise ValueError("Wrong input for file", os.path.isfile(kwargs['path'])
                          , kwargs['reset'] == True)
         
-    print(kwargs['search_mode'])
+    print(f"Search mode selected: {kwargs['search_mode']}")
 
     frames_dict = dict(DEFAULT_ONLINE = {'H':""
                                  ,'L':""
                                  ,'V':""}
                         ,DEFAULT_OFFLINE = {'H':""
                                  ,'L':""
                                  ,'V':""}
@@ -581,22 +579,60 @@
     args = parser.parse_args()
     
 
     search_path = getattr(args, "search_path")      
 
     if os.path.isfile(search_path+"runall.sh"):
 
-        os.system(f"nohup sh {search_path}runall.sh &> {search_path}runall.out &")
+        os.system(f"cd {search_path} ; nohup sh runall.sh &> runall.out & echo $!>>.jobids.txt")
+        print("Search has started for ")
 
     else:
 
         raise FileNotFoundError(f"The path provided {search_path} does not have a runall.sh file to start the search.")
 
       
-        
-        
-if __name__ == "__main__":
+def _end_search():
+
+        #Construct argument parser:
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument('-p', '--search_path', type=str
+                        , default = "./"
+                        , help = "The path to the search to start"
+                        , required = False)
+
+    # Pass arguments:
+    args = parser.parse_args()
     
-     main()
 
+    search_path = getattr(args, "search_path")      
+
+    if os.path.isfile(search_path+".jobids.txt"):
+
+        with open(f"{search_path}/.jobids.txt", "r") as idfile:
+            idfile_ = idfile.read()
+  
+        # replacing end of line('/n') with ' ' and
+        # splidfile.read()
+    
+        # replacing end of line('/n') with ' ' and
+        # splitting the text it further when '.' is seen.
+        job_id_list = idfile_.replace('\n', ' ').split(" ")
+    
+        for id_ in job_id_list:
+            try:
+                print(f"kill {str(id_)}")
+                os.system(f"kill {str(id_)}")
+            except Exception as e:
+                pass
+        os.system(f">{search_path}/.jobids.txt")
+    else:
 
+        raise FileNotFoundError(f"The path provided {search_path} does not have a .jobids.txt file to start the search.")
+
+
+
+if __name__ == "__main__":
+    
+     main()
```

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.4/mly_pipeline/make_eff_estimation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/manager.py` & `mly_pipeline-0.4/mly_pipeline/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Sourcing the submodule of mly in a very unpythonic way 
 sys.path.append("/".join(sys.argv[0].split("/")[:-1])+"/mly/")
 
 
 
 from mly.tools import dirlist
 from mly.datatools import *
-from search_functions import *
+from .search_functions import *
 
 # # # Initialising logging
 
 # create logger
 logger = logging.getLogger("logger_for_manager")
 logger.setLevel(logging.INFO)
```

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.4/mly_pipeline/mly_to_grace.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/offline_search.py` & `mly_pipeline-0.4/mly_pipeline/offline_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Sourcing the submodule of mly in a very unpythonic way 
 sys.path.append("/".join(sys.argv[0].split("/")[:-1])+"/mly/")
 
 
 from mly.datatools import DataPod
 from mly.validators import Validator
 from mly.null_energy_map import *
-from search_functions import *
+from .search_functions import *
 
 from mly.null_energy_map import *
 from ligo.skymap.io import fits
 
 import matplotlib.pyplot as plt
 
 from pycondor import Job, Dagman
```

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/search.py` & `mly_pipeline-0.4/mly_pipeline/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 print("/".join(sys.argv[0].split("/")[:-1])+"/mly/")
 
 
 from mly.datatools import DataPod
 from mly.validators import Validator
 from mly.null_energy_map import *
-from search_functions import *
+from .search_functions import *
 
 
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
 
 # # # Initialising logging
```

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/search_functions.py` & `mly_pipeline-0.4/mly_pipeline/search_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1076,10 +1076,7 @@
         _pod = DataPod(pod.strain[pod.detectors.index(det)]
                        ,detectors = [det]
                        ,fs = pod.fs
                        ,gps = [_gps])
         
         _pod.save(masterDirectory+'temp/'+det+'/'+str(_gps)+'_1')
     
-
-def helloworld():
-    print("helloworld")
```

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.4/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.4/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.4/mly_pipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.3.1.2
+Version: 0.4
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.3.1.2/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.4/mly_pipeline.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 docs/build/html/_static/websupport.js
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/runningasearch.rst
 docs/source/settingupasearch.rst
 mly_pipeline/__init__.py
-mly_pipeline/continious_FAR.py
+mly_pipeline/continuous_FAR.py
 mly_pipeline/initialization.py
 mly_pipeline/make_eff_estimation.py
 mly_pipeline/manager.py
 mly_pipeline/mly_to_grace.py
 mly_pipeline/offline_search.py
 mly_pipeline/search.py
 mly_pipeline/search_functions.py
```

### Comparing `mly_pipeline-0.3.1.2/pyproject.toml` & `mly_pipeline-0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.3.1.2"
+version = "0.4"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
@@ -19,9 +19,12 @@
 dependencies = [
     "mly"
 ]
 
 [project.scripts]
 mly-pipeline-init = "mly_pipeline.initialization:main"
 mly-pipeline-start = "mly_pipeline.initialization:_start_search"
+mly-pipeline-stop = "mly_pipeline.initialization:_end_search"
+
+
```

