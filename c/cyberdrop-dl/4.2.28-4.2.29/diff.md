# Comparing `tmp/cyberdrop-dl-4.2.28.tar.gz` & `tmp/cyberdrop-dl-4.2.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.28.tar", last modified: Thu May 18 06:10:18 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.29.tar", last modified: Thu May 18 16:31:35 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.28.tar` & `cyberdrop-dl-4.2.29.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17394 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.136266 cyberdrop-dl-4.2.28/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.140266 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.140266 cyberdrop-dl-4.2.28/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.140266 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17394 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.261963 cyberdrop-dl-4.2.29/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.265963 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.265963 cyberdrop-dl-4.2.29/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:31:35.261963 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 16:31:35.000000 cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 16:31:35.269963 cyberdrop-dl-4.2.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:31:20.000000 cyberdrop-dl-4.2.29/setup.py
```

### Comparing `cyberdrop-dl-4.2.28/LICENSE` & `cyberdrop-dl-4.2.29/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/PKG-INFO` & `cyberdrop-dl-4.2.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.28
+Version: 4.2.29
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.28 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.29 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.28/README.md` & `cyberdrop-dl-4.2.29/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         assert url.host is not None
         domain_obj = DomainItem(url.host.lower(), {})
 
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if await check_direct(url):
             url = url.with_name(url.name.replace('.md.', '.').replace('.th.', '.'))
-            url = await self.jpg_fish_from_church(url)
+            url = await self.jpg_church_from_fish(url)
             media_item = await create_media_item(url, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         elif "album" in url.parts or "a" in url.parts:
             await self.parse(session=session, url=url, domain_obj=domain_obj)
         elif "albums" in url.parts:
             await self.get_albums(session, url, domain_obj)
         elif 'image' in url.parts or 'img' in url.parts or 'images' in url.parts:
@@ -50,17 +50,17 @@
         else:
             await self.parse_profile(session, url, domain_obj)
 
         await self.SQL_Helper.insert_domain("sharex", url, domain_obj)
         log(f"Finished: {url}", quiet=self.quiet, style="green")
         return domain_obj
 
-    async def jpg_fish_from_church(self, url: URL) -> URL:
-        pattern2 = r"simp([1-5])\.jpg\.church/"
-        return URL(re.sub(pattern2, r'simp\1.jpg.fish/', str(url)))
+    async def jpg_church_from_fish(self, url: URL) -> URL:
+        pattern2 = r"simp([1-5])\.jpg\.fish/"
+        return URL(re.sub(pattern2, r'simp\1.jpg.church/', str(url)))
 
     async def get_albums(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for Albums"""
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
             albums = soup.select("a[class='image-container --media']")
@@ -86,15 +86,15 @@
         """Handles scraping for singular files"""
         await asyncio.sleep(1)
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
             link = URL(soup.select_one("input[id=embed-code-2]").get('value'))
             link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
-            link = await self.jpg_fish_from_church(link)
+            link = await self.jpg_church_from_fish(link)
 
             media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
             log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
@@ -143,15 +143,15 @@
             if 'jpg.fish' in url.host or 'jpg.church' in url.host:
                 links = soup.select("a[href*=img] img")
             else:
                 links = soup.select("a[href*=image] img")
             for link in links:
                 link = URL(link.get('src'))
                 link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
-                link = await self.jpg_fish_from_church(link)
+                link = await self.jpg_church_from_fish(link)
 
                 try:
                     media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", link)
                     continue
                 await domain_obj.add_media(title, media_item)
```

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.29/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.28
+Version: 4.2.29
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.28 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.29 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.29/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.28/setup.cfg` & `cyberdrop-dl-4.2.29/setup.cfg`

 * *Files identical despite different names*

