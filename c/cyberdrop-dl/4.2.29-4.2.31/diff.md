# Comparing `tmp/cyberdrop-dl-4.2.29.tar.gz` & `tmp/cyberdrop-dl-4.2.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.29.tar", last modified: Thu May 18 16:31:35 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.31.tar", last modified: Thu May 18 19:01:55 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.29.tar` & `cyberdrop-dl-4.2.31.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17394 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.261963 cyberdrop-dl-4.2.29/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.265963 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.265963 cyberdrop-dl-4.2.29/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.261963 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.703730 cyberdrop-dl-4.2.31/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.707730 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.707730 cyberdrop-dl-4.2.31/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18528 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19831 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.715730 cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:01:55.703730 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 19:01:55.000000 cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 19:01:55.719730 cyberdrop-dl-4.2.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:01:46.000000 cyberdrop-dl-4.2.31/setup.py
```

### Comparing `cyberdrop-dl-4.2.29/LICENSE` & `cyberdrop-dl-4.2.31/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/PKG-INFO` & `cyberdrop-dl-4.2.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.29
+Version: 4.2.31
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -145,21 +145,24 @@
 --skip-hosts            doesn't allow downloads and scraping from these hosts
 
 --allow-insecure-connections            allows insecure connections from content hosts
 --attempts                              number of attempts to download each file
 --block-sub-folders                     block sub folders from being created
 --disable-attempt-limit                 disables the attempt limitation
 --include-id                            include the ID in the download folder name
+--max-concurrent-threads                number of threads to download simultaneously
+--max-concurrent-domains                number of domains to download simultaneously
+--max-concurrent-albums                 number of albums to download simultaneously
+--max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
 --proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
---simultaneous-downloads-per-domain     number of simultaneous downloads to use per domain
 
 --sort-downloads        sorts downloaded files after downloads have finished
 --sort-directory        folder to download files to
 --sorted-audio          schema to sort audio
 --sorted-images         schema to sort images
 --sorted-others         schema to sort other
 --sorted-videos         schema to sort videos
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.29 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.31 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -126,38 +126,41 @@
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
 download each file --block-sub-folders block sub folders from being created --
 disable-attempt-limit disables the attempt limitation --include-id include the
-ID in the download folder name --skip-download-mark-completed sets the scraped
-files as downloaded without downloading --output-errored-urls sets the failed
-urls to be output to the errored urls file --output-unsupported-urls sets the
-unsupported urls to be output to the unsupported urls file --proxy HTTP/HTTPS
-proxy used for downloading, format [protocal]://[ip]:[port] --remove-bunkr-
-identifier removes the bunkr added identifier from output filenames --required-
-free-space required free space (in gigabytes) for the program to run --
-simultaneous-downloads-per-domain number of simultaneous downloads to use per
-domain --sort-downloads sorts downloaded files after downloads have finished --
-sort-directory folder to download files to --sorted-audio schema to sort audio
---sorted-images schema to sort images --sorted-others schema to sort other --
-sorted-videos schema to sort videos --connection-timeout number of seconds to
-wait attempting to connect to a URL during the downloading phase --ratelimit
-this applies to requests made in the program during scraping, the number you
-provide is in requests/seconds --throttle this is a throttle between requests
-during the downloading phase, the number is in seconds --output-last-forum-post
-outputs the last post of a forum scrape to use as a starting point for future
-runs --scrape-single-post scrapes a single post from a forum thread --separate-
-posts separates forum scraping into folders by post number --gofile-api-key api
-key for premium gofile --pixeldrain-api-key api key for premium pixeldrain --
-nudostar-username username to login to nudostar --nudostar-password password to
-login to nudostar --simpcity-username username to login to simpcity --simpcity-
-password password to login to simpcity --socialmediagirls-username username to
-login to socialmediagirls --socialmediagirls-password password to login to
+ID in the download folder name --max-concurrent-threads number of threads to
+download simultaneously --max-concurrent-domains number of domains to download
+simultaneously --max-concurrent-albums number of albums to download
+simultaneously --max-concurrent-downloads-per-domain number of simultaneous
+downloads per domain --skip-download-mark-completed sets the scraped files as
+downloaded without downloading --output-errored-urls sets the failed urls to be
+output to the errored urls file --output-unsupported-urls sets the unsupported
+urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
+for downloading, format [protocal]://[ip]:[port] --remove-bunkr-identifier
+removes the bunkr added identifier from output filenames --required-free-space
+required free space (in gigabytes) for the program to run --sort-downloads
+sorts downloaded files after downloads have finished --sort-directory folder to
+download files to --sorted-audio schema to sort audio --sorted-images schema to
+sort images --sorted-others schema to sort other --sorted-videos schema to sort
+videos --connection-timeout number of seconds to wait attempting to connect to
+a URL during the downloading phase --ratelimit this applies to requests made in
+the program during scraping, the number you provide is in requests/seconds --
+throttle this is a throttle between requests during the downloading phase, the
+number is in seconds --output-last-forum-post outputs the last post of a forum
+scrape to use as a starting point for future runs --scrape-single-post scrapes
+a single post from a forum thread --separate-posts separates forum scraping
+into folders by post number --gofile-api-key api key for premium gofile --
+pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
+to login to nudostar --nudostar-password password to login to nudostar --
+simpcity-username username to login to simpcity --simpcity-password password to
+login to simpcity --socialmediagirls-username username to login to
+socialmediagirls --socialmediagirls-password password to login to
 socialmediagirls --xbunker-username username to login to xbunker --xbunker-
 password password to login to xbunker --apply-jdownloader enables sending
 unsupported URLs to a running jdownloader2 instance to download --jdownloader-
 username username to login to jdownloader --jdownloader-password password to
 login to jdownloader --jdownloader-device device name to login to for
 jdownloader --hide-new-progress disables the new rich progress entirely and
 uses older methods --hide-overall-progress removes overall progress section
```

### Comparing `cyberdrop-dl-4.2.29/README.md` & `cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: cyberdrop-dl
+Version: 4.2.31
+Summary: Bulk downloader for multiple file hosts and forum sites
+Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
+Author: Jules-WinnfieldX
+Author-email: JulesWinnfieldII@protonmail.com
+Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `cyberdrop-dl`
 
 **Bulk downloader for multiple file hosts**
 
 [![PyPI version](https://badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl)](https://pepy.tech/project/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/month)](https://pepy.tech/project/cyberdrop-dl)
@@ -133,21 +145,24 @@
 --skip-hosts            doesn't allow downloads and scraping from these hosts
 
 --allow-insecure-connections            allows insecure connections from content hosts
 --attempts                              number of attempts to download each file
 --block-sub-folders                     block sub folders from being created
 --disable-attempt-limit                 disables the attempt limitation
 --include-id                            include the ID in the download folder name
+--max-concurrent-threads                number of threads to download simultaneously
+--max-concurrent-domains                number of domains to download simultaneously
+--max-concurrent-albums                 number of albums to download simultaneously
+--max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
 --proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
---simultaneous-downloads-per-domain     number of simultaneous downloads to use per domain
 
 --sort-downloads        sorts downloaded files after downloads have finished
 --sort-directory        folder to download files to
 --sorted-audio          schema to sort audio
 --sorted-images         schema to sort images
 --sorted-others         schema to sort other
 --sorted-videos         schema to sort videos
```

#### html2text {}

```diff
@@ -1,22 +1,28 @@
-# `cyberdrop-dl` **Bulk downloader for multiple file hosts** [![PyPI version]
-(https://badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/
-cyberdrop-dl) [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl)]
-(https://pepy.tech/project/cyberdrop-dl) [![Downloads](https://
-static.pepy.tech/badge/cyberdrop-dl/month)](https://pepy.tech/project/
-cyberdrop-dl) [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/week)]
-(https://pepy.tech/project/cyberdrop-dl) [![Discord Banner 3](https://
-discordapp.com/api/guilds/1070206871564197908/widget.png?style=banner3)](https:
-//discord.com/invite/kbZCxz22Qp) Brand new and improved! Cyberdrop-DL now has
-an updated paint job, fantastic new look. On top of this it also downloads from
-different domains simultaneously. ![Screenshot 2023-02-19 183052](https://user-
-images.githubusercontent.com/61347133/219989561-759bd8b1-34d2-4d61-8fa7-
-0d0b3680e83f.png) ## Support Cyberdrop-DL Development [Buy_Me_A_Coffee] If you
-want to support me and my effort you can buy me a coffee or send me some
-crypto: BTC: bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.31 Summary: Bulk
+downloader for multiple file hosts and forum sites Home-page: https://
+github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
+Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
+/github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
+**Bulk downloader for multiple file hosts** [![PyPI version](https://
+badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
+[Downloads](https://static.pepy.tech/badge/cyberdrop-dl)](https://pepy.tech/
+project/cyberdrop-dl) [![Downloads](https://static.pepy.tech/badge/cyberdrop-
+dl/month)](https://pepy.tech/project/cyberdrop-dl) [![Downloads](https://
+static.pepy.tech/badge/cyberdrop-dl/week)](https://pepy.tech/project/cyberdrop-
+dl) [![Discord Banner 3](https://discordapp.com/api/guilds/1070206871564197908/
+widget.png?style=banner3)](https://discord.com/invite/kbZCxz22Qp) Brand new and
+improved! Cyberdrop-DL now has an updated paint job, fantastic new look. On top
+of this it also downloads from different domains simultaneously. ![Screenshot
+2023-02-19 183052](https://user-images.githubusercontent.com/61347133/
+219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png) ## Support Cyberdrop-DL
+Development [Buy_Me_A_Coffee] If you want to support me and my effort you can
+buy me a coffee or send me some crypto: BTC:
+bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B XMR:
 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
 ## More Information Read the [Wiki](https://github.com/Jules-WinnfieldX/
 CyberDropDownloader/wiki/)! ## Supported Sites | Website | Supported Link Types
 | |-----------------------------------------|----------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
@@ -120,38 +126,41 @@
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
 download each file --block-sub-folders block sub folders from being created --
 disable-attempt-limit disables the attempt limitation --include-id include the
-ID in the download folder name --skip-download-mark-completed sets the scraped
-files as downloaded without downloading --output-errored-urls sets the failed
-urls to be output to the errored urls file --output-unsupported-urls sets the
-unsupported urls to be output to the unsupported urls file --proxy HTTP/HTTPS
-proxy used for downloading, format [protocal]://[ip]:[port] --remove-bunkr-
-identifier removes the bunkr added identifier from output filenames --required-
-free-space required free space (in gigabytes) for the program to run --
-simultaneous-downloads-per-domain number of simultaneous downloads to use per
-domain --sort-downloads sorts downloaded files after downloads have finished --
-sort-directory folder to download files to --sorted-audio schema to sort audio
---sorted-images schema to sort images --sorted-others schema to sort other --
-sorted-videos schema to sort videos --connection-timeout number of seconds to
-wait attempting to connect to a URL during the downloading phase --ratelimit
-this applies to requests made in the program during scraping, the number you
-provide is in requests/seconds --throttle this is a throttle between requests
-during the downloading phase, the number is in seconds --output-last-forum-post
-outputs the last post of a forum scrape to use as a starting point for future
-runs --scrape-single-post scrapes a single post from a forum thread --separate-
-posts separates forum scraping into folders by post number --gofile-api-key api
-key for premium gofile --pixeldrain-api-key api key for premium pixeldrain --
-nudostar-username username to login to nudostar --nudostar-password password to
-login to nudostar --simpcity-username username to login to simpcity --simpcity-
-password password to login to simpcity --socialmediagirls-username username to
-login to socialmediagirls --socialmediagirls-password password to login to
+ID in the download folder name --max-concurrent-threads number of threads to
+download simultaneously --max-concurrent-domains number of domains to download
+simultaneously --max-concurrent-albums number of albums to download
+simultaneously --max-concurrent-downloads-per-domain number of simultaneous
+downloads per domain --skip-download-mark-completed sets the scraped files as
+downloaded without downloading --output-errored-urls sets the failed urls to be
+output to the errored urls file --output-unsupported-urls sets the unsupported
+urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
+for downloading, format [protocal]://[ip]:[port] --remove-bunkr-identifier
+removes the bunkr added identifier from output filenames --required-free-space
+required free space (in gigabytes) for the program to run --sort-downloads
+sorts downloaded files after downloads have finished --sort-directory folder to
+download files to --sorted-audio schema to sort audio --sorted-images schema to
+sort images --sorted-others schema to sort other --sorted-videos schema to sort
+videos --connection-timeout number of seconds to wait attempting to connect to
+a URL during the downloading phase --ratelimit this applies to requests made in
+the program during scraping, the number you provide is in requests/seconds --
+throttle this is a throttle between requests during the downloading phase, the
+number is in seconds --output-last-forum-post outputs the last post of a forum
+scrape to use as a starting point for future runs --scrape-single-post scrapes
+a single post from a forum thread --separate-posts separates forum scraping
+into folders by post number --gofile-api-key api key for premium gofile --
+pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
+to login to nudostar --nudostar-password password to login to nudostar --
+simpcity-username username to login to simpcity --simpcity-password password to
+login to simpcity --socialmediagirls-username username to login to
+socialmediagirls --socialmediagirls-password password to login to
 socialmediagirls --xbunker-username username to login to xbunker --xbunker-
 password password to login to xbunker --apply-jdownloader enables sending
 unsupported URLs to a running jdownloader2 instance to download --jdownloader-
 username username to login to jdownloader --jdownloader-password password to
 login to jdownloader --jdownloader-device device name to login to for
 jdownloader --hide-new-progress disables the new rich progress entirely and
 uses older methods --hide-overall-progress removes overall progress section
```

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,20 +68,23 @@
         },
         "Runtime": {
             "allow_insecure_connections": False,
             "attempts": 10,
             "block_sub_folders": False,
             "disable_attempt_limit": False,
             "include_id": False,
+            "max_concurrent_threads": 0,
+            "max_concurrent_domains": 0,
+            "max_concurrent_albums": 0,
+            "max_concurrent_downloads_per_domain": 4,
             "output_errored_urls": False,
             "output_unsupported_urls": False,
             "proxy": "",
             "remove_bunkr_identifier": False,
             "required_free_space": 5,
-            "simultaneous_downloads_per_domain": 4,
             "skip_download_mark_completed": False,
             "user_agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/112.0",
         },
         "Sorting": {
             "sort_downloads": False,
             "sort_directory": "Sorted Downloads",
             "sorted_audio": "{sort_dir}/{base_dir}/Audio",
```

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     """Checks if there is enough free space on the drive to continue operating"""
     free_space = shutil.disk_usage(download_directory.parent).free
     free_space_gb = free_space / 1024 ** 3
     return free_space_gb >= required_space_gb
 
 
 def get_threads_number(args: Dict, domain: str) -> int:
-    threads = args["Runtime"]["simultaneous_downloads_per_domain"] or multiprocessing.cpu_count()
+    threads = args["Runtime"]["max_concurrent_downloads_per_domain"] or multiprocessing.cpu_count()
     if any(s in domain for s in ('anonfiles', 'bunkr', 'pixeldrain')):
         return min(threads, 2)
     return threads
 
 
 async def is_4xx_client_error(status_code: int) -> bool:
     """Checks whether the HTTP status code is 4xx client error"""
```

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/downloaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import asyncio
 import contextlib
 import itertools
 import logging
 from http import HTTPStatus
 from random import gauss
-from typing import TYPE_CHECKING, Any, Dict, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Tuple, Coroutine, List, Optional
 
 import aiofiles
 import aiohttp.client_exceptions
 from rich.live import Live
 
 from cyberdrop_dl.base_functions.base_functions import (
     clear,
@@ -45,14 +45,25 @@
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from rich.progress import TaskID
 
 
+def _limit_concurrency(coroutines: List[Coroutine], semaphore: Optional[asyncio.Semaphore]) -> List[Coroutine]:
+    if not semaphore:
+        return coroutines
+
+    async def limit_concurrency(coroutine: Coroutine) -> Coroutine:
+        async with semaphore:
+            return await coroutine
+
+    return [limit_concurrency(coroutine) for coroutine in coroutines]
+
+
 class CDLHelper:
     def __init__(self, args: Dict, client: Client, files: OverallFileProgress, SQL_Helper: SQLHelper):
         self.args = args
 
         # CDL Objects
         self.client = client
         self.files = files
@@ -73,14 +84,19 @@
         self.allowed_attempts = args["Runtime"]["attempts"]
         self.disable_attempt_limit = args["Runtime"]["disable_attempt_limit"]
         self.download_dir = args["Files"]["output_folder"]
         self.mark_downloaded = args["Runtime"]["skip_download_mark_completed"]
         self.proxy = args["Runtime"]["proxy"]
         self.required_free_space = args["Runtime"]["required_free_space"]
 
+        # Concurrency Limits
+        self.threads_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_threads"]) if args["Runtime"]["max_concurrent_threads"] else None
+        self.domains_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_domains"]) if args["Runtime"]["max_concurrent_domains"] else None
+        self.albums_limit = asyncio.Semaphore(args["Runtime"]["max_concurrent_albums"]) if args["Runtime"]["max_concurrent_albums"] else None
+
         # Output Args
         self.errored_output = args['Runtime']['output_errored_urls']
         self.errored_file = args['Files']['errored_urls_file']
 
         # API Keys
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
@@ -317,41 +333,41 @@
 
         progress_table = await self.Progress_Master.get_table()
         with Live(progress_table, refresh_per_second=self.Progress_Master.refresh_rate):
             forum_task = self.Progress_Master.ForumProgress.add_forum(len(self.Forums.threads))
             cascade_tasks = []
             for title, Cascade in self.Forums.threads.items():
                 cascade_tasks.append(self.start_cascade(forum_task, title, Cascade))
-            await asyncio.gather(*cascade_tasks)
+            await asyncio.gather(*_limit_concurrency(cascade_tasks, self.CDL_Helper.threads_limit))
 
         await clear()
         completed_files, skipped_files, failed_files = self.Progress_Master.OverallFileProgress.return_totals()
         log(f"| [green]Files Complete: {completed_files}[/green] - [yellow]Files Skipped:  {skipped_files}[/yellow] - [red]Files Failed: {failed_files}[/red] |")
 
         for downloader in self.Download_Manager.downloaders.values():
             await downloader.download_session.exit_handler()
 
     async def start_cascade(self, forum_task: TaskID, title: str, Cascade: CascadeItem) -> None:
         cascade_task = self.Progress_Master.CascadeProgress.add_cascade(title, len(Cascade.domains))
         domain_tasks = []
         for domain, domain_obj in Cascade.domains.items():
             domain_tasks.append(self.start_domain(cascade_task, title, domain, domain_obj))
-        await asyncio.gather(*domain_tasks)
+        await asyncio.gather(*_limit_concurrency(domain_tasks, self.CDL_Helper.domains_limit))
         self.Progress_Master.CascadeProgress.mark_cascade_completed(cascade_task)
         self.Progress_Master.ForumProgress.advance_forum(forum_task)
 
     async def start_domain(self, cascade_task: TaskID, title: str, domain: str, domain_obj: DomainItem) -> None:
         """Handler for domains and the progress bars for it"""
         downloader = await self.Download_Manager.get_downloader(domain)
 
         domain_task = self.Progress_Master.DomainProgress.add_domain(domain, len(domain_obj.albums))
         album_tasks = []
         for album, album_obj in domain_obj.albums.items():
             album_tasks.append(self.start_album(downloader, domain_task, domain, album, album_obj))
-        await asyncio.gather(*album_tasks)
+        await asyncio.gather(*_limit_concurrency(album_tasks, self.CDL_Helper.albums_limit))
         self.Progress_Master.CascadeProgress.advance_cascade(cascade_task)
         self.Progress_Master.DomainProgress.mark_domain_completed(domain, domain_task)
 
     async def start_album(self, downloader: Downloader, domain_task: TaskID, domain: str, album: str,
                           album_obj: AlbumItem) -> None:
         """Handler for albums and the progress bars for it"""
         if await album_obj.is_empty():
```

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,21 +65,24 @@
     config_group = config_data["Runtime"]
     runtime_opts = parser.add_argument_group("Runtime options")
     runtime_opts.add_argument("--allow-insecure-connections", help="allows insecure connections from content hosts", action="store_true")
     runtime_opts.add_argument("--attempts", type=int, help="number of attempts to download each file (default: %(default)s)", default=config_group["attempts"])
     runtime_opts.add_argument("--block-sub-folders", help="block sub folders from being created", action="store_true")
     runtime_opts.add_argument("--disable-attempt-limit", help="disables the attempt limitation", action="store_true")
     runtime_opts.add_argument("--include-id", help="include the ID in the download folder name", action="store_true")
+    runtime_opts.add_argument("--max_concurrent-threads", type=int, default=config_group["max_concurrent_threads"], help="Number of threads to download simultaneously (default: %(default)s)")
+    runtime_opts.add_argument("--max_concurrent-domains", type=int, default=config_group["max_concurrent_domains"], help="Number of domains to download simultaneously (default: %(default)s)")
+    runtime_opts.add_argument("--max_concurrent-albums", type=int, default=config_group["max_concurrent_albums"], help="Number of albums to download simultaneously (default: %(default)s)")
+    runtime_opts.add_argument("--max_concurrent-downloads-per-domain", type=int, default=config_group["max_concurrent_downloads_per_domain"], help="Number of simultaneous downloads per domain (default: %(default)s)")
     runtime_opts.add_argument("--skip-download-mark-completed", help="sets the scraped files as downloaded without downloading", action="store_true")
     runtime_opts.add_argument("--output-errored-urls", help="sets the failed urls to be output to the errored urls file", action="store_true")
     runtime_opts.add_argument("--output-unsupported-urls", help="sets the unsupported urls to be output to the unsupported urls file", action="store_true")
     runtime_opts.add_argument("--proxy", help="HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]", default=config_group["proxy"])
     runtime_opts.add_argument("--remove-bunkr-identifier", help="removes the bunkr added identifier from output filenames", action="store_true")
     runtime_opts.add_argument("--required-free-space", type=int, default=config_group["required_free_space"], help="required free space (in gigabytes) for the program to run (default: %(default)s)")
-    runtime_opts.add_argument("--simultaneous-downloads-per-domain", type=int, default=config_group["simultaneous_downloads_per_domain"], help="Number of simultaneous downloads to use per domain (default: %(default)s)")
 
     # Sorting
     config_group = config_data["Sorting"]
     sort_opts = parser.add_argument_group("Sorting options")
     sort_opts.add_argument("--sort-downloads", help="sorts downloaded files after downloads have finished", action="store_true")
     sort_opts.add_argument("--sort-directory", type=Path, help="folder to download files to (default: %(default)s)", default=config_group["sort_directory"])
     sort_opts.add_argument("--sorted-audio", help="schema to sort audio (default: %(default)s)", default=config_group["sorted_audio"])
```

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.31/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.31/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cyberdrop-dl
-Version: 4.2.29
-Summary: Bulk downloader for multiple file hosts and forum sites
-Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
-Author: Jules-WinnfieldX
-Author-email: JulesWinnfieldII@protonmail.com
-Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `cyberdrop-dl`
 
 **Bulk downloader for multiple file hosts**
 
 [![PyPI version](https://badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl)](https://pepy.tech/project/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/month)](https://pepy.tech/project/cyberdrop-dl)
@@ -145,21 +133,24 @@
 --skip-hosts            doesn't allow downloads and scraping from these hosts
 
 --allow-insecure-connections            allows insecure connections from content hosts
 --attempts                              number of attempts to download each file
 --block-sub-folders                     block sub folders from being created
 --disable-attempt-limit                 disables the attempt limitation
 --include-id                            include the ID in the download folder name
+--max-concurrent-threads                number of threads to download simultaneously
+--max-concurrent-domains                number of domains to download simultaneously
+--max-concurrent-albums                 number of albums to download simultaneously
+--max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
 --proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
---simultaneous-downloads-per-domain     number of simultaneous downloads to use per domain
 
 --sort-downloads        sorts downloaded files after downloads have finished
 --sort-directory        folder to download files to
 --sorted-audio          schema to sort audio
 --sorted-images         schema to sort images
 --sorted-others         schema to sort other
 --sorted-videos         schema to sort videos
```

#### html2text {}

```diff
@@ -1,28 +1,22 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.29 Summary: Bulk
-downloader for multiple file hosts and forum sites Home-page: https://
-github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
-Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
-/github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
-**Bulk downloader for multiple file hosts** [![PyPI version](https://
-badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
-[Downloads](https://static.pepy.tech/badge/cyberdrop-dl)](https://pepy.tech/
-project/cyberdrop-dl) [![Downloads](https://static.pepy.tech/badge/cyberdrop-
-dl/month)](https://pepy.tech/project/cyberdrop-dl) [![Downloads](https://
-static.pepy.tech/badge/cyberdrop-dl/week)](https://pepy.tech/project/cyberdrop-
-dl) [![Discord Banner 3](https://discordapp.com/api/guilds/1070206871564197908/
-widget.png?style=banner3)](https://discord.com/invite/kbZCxz22Qp) Brand new and
-improved! Cyberdrop-DL now has an updated paint job, fantastic new look. On top
-of this it also downloads from different domains simultaneously. ![Screenshot
-2023-02-19 183052](https://user-images.githubusercontent.com/61347133/
-219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png) ## Support Cyberdrop-DL
-Development [Buy_Me_A_Coffee] If you want to support me and my effort you can
-buy me a coffee or send me some crypto: BTC:
-bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
+# `cyberdrop-dl` **Bulk downloader for multiple file hosts** [![PyPI version]
+(https://badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/
+cyberdrop-dl) [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl)]
+(https://pepy.tech/project/cyberdrop-dl) [![Downloads](https://
+static.pepy.tech/badge/cyberdrop-dl/month)](https://pepy.tech/project/
+cyberdrop-dl) [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/week)]
+(https://pepy.tech/project/cyberdrop-dl) [![Discord Banner 3](https://
+discordapp.com/api/guilds/1070206871564197908/widget.png?style=banner3)](https:
+//discord.com/invite/kbZCxz22Qp) Brand new and improved! Cyberdrop-DL now has
+an updated paint job, fantastic new look. On top of this it also downloads from
+different domains simultaneously. ![Screenshot 2023-02-19 183052](https://user-
+images.githubusercontent.com/61347133/219989561-759bd8b1-34d2-4d61-8fa7-
+0d0b3680e83f.png) ## Support Cyberdrop-DL Development [Buy_Me_A_Coffee] If you
+want to support me and my effort you can buy me a coffee or send me some
+crypto: BTC: bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B XMR:
 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
 ## More Information Read the [Wiki](https://github.com/Jules-WinnfieldX/
 CyberDropDownloader/wiki/)! ## Supported Sites | Website | Supported Link Types
 | |-----------------------------------------|----------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
@@ -126,38 +120,41 @@
 downloading of video files --ignore-cache ignores previous runs cached scrape
 history --ignore-history ignores previous download history --only-hosts only
 allows downloads and scraping from these hosts --skip-hosts doesn't allow
 downloads and scraping from these hosts --allow-insecure-connections allows
 insecure connections from content hosts --attempts number of attempts to
 download each file --block-sub-folders block sub folders from being created --
 disable-attempt-limit disables the attempt limitation --include-id include the
-ID in the download folder name --skip-download-mark-completed sets the scraped
-files as downloaded without downloading --output-errored-urls sets the failed
-urls to be output to the errored urls file --output-unsupported-urls sets the
-unsupported urls to be output to the unsupported urls file --proxy HTTP/HTTPS
-proxy used for downloading, format [protocal]://[ip]:[port] --remove-bunkr-
-identifier removes the bunkr added identifier from output filenames --required-
-free-space required free space (in gigabytes) for the program to run --
-simultaneous-downloads-per-domain number of simultaneous downloads to use per
-domain --sort-downloads sorts downloaded files after downloads have finished --
-sort-directory folder to download files to --sorted-audio schema to sort audio
---sorted-images schema to sort images --sorted-others schema to sort other --
-sorted-videos schema to sort videos --connection-timeout number of seconds to
-wait attempting to connect to a URL during the downloading phase --ratelimit
-this applies to requests made in the program during scraping, the number you
-provide is in requests/seconds --throttle this is a throttle between requests
-during the downloading phase, the number is in seconds --output-last-forum-post
-outputs the last post of a forum scrape to use as a starting point for future
-runs --scrape-single-post scrapes a single post from a forum thread --separate-
-posts separates forum scraping into folders by post number --gofile-api-key api
-key for premium gofile --pixeldrain-api-key api key for premium pixeldrain --
-nudostar-username username to login to nudostar --nudostar-password password to
-login to nudostar --simpcity-username username to login to simpcity --simpcity-
-password password to login to simpcity --socialmediagirls-username username to
-login to socialmediagirls --socialmediagirls-password password to login to
+ID in the download folder name --max-concurrent-threads number of threads to
+download simultaneously --max-concurrent-domains number of domains to download
+simultaneously --max-concurrent-albums number of albums to download
+simultaneously --max-concurrent-downloads-per-domain number of simultaneous
+downloads per domain --skip-download-mark-completed sets the scraped files as
+downloaded without downloading --output-errored-urls sets the failed urls to be
+output to the errored urls file --output-unsupported-urls sets the unsupported
+urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
+for downloading, format [protocal]://[ip]:[port] --remove-bunkr-identifier
+removes the bunkr added identifier from output filenames --required-free-space
+required free space (in gigabytes) for the program to run --sort-downloads
+sorts downloaded files after downloads have finished --sort-directory folder to
+download files to --sorted-audio schema to sort audio --sorted-images schema to
+sort images --sorted-others schema to sort other --sorted-videos schema to sort
+videos --connection-timeout number of seconds to wait attempting to connect to
+a URL during the downloading phase --ratelimit this applies to requests made in
+the program during scraping, the number you provide is in requests/seconds --
+throttle this is a throttle between requests during the downloading phase, the
+number is in seconds --output-last-forum-post outputs the last post of a forum
+scrape to use as a starting point for future runs --scrape-single-post scrapes
+a single post from a forum thread --separate-posts separates forum scraping
+into folders by post number --gofile-api-key api key for premium gofile --
+pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
+to login to nudostar --nudostar-password password to login to nudostar --
+simpcity-username username to login to simpcity --simpcity-password password to
+login to simpcity --socialmediagirls-username username to login to
+socialmediagirls --socialmediagirls-password password to login to
 socialmediagirls --xbunker-username username to login to xbunker --xbunker-
 password password to login to xbunker --apply-jdownloader enables sending
 unsupported URLs to a running jdownloader2 instance to download --jdownloader-
 username username to login to jdownloader --jdownloader-password password to
 login to jdownloader --jdownloader-device device name to login to for
 jdownloader --hide-new-progress disables the new rich progress entirely and
 uses older methods --hide-overall-progress removes overall progress section
```

### Comparing `cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.31/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.29/setup.cfg` & `cyberdrop-dl-4.2.31/setup.cfg`

 * *Files identical despite different names*

