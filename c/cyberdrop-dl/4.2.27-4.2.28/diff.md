# Comparing `tmp/cyberdrop-dl-4.2.27.tar.gz` & `tmp/cyberdrop-dl-4.2.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.27.tar", last modified: Tue May 16 22:37:48 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.28.tar", last modified: Thu May 18 06:10:18 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.27.tar` & `cyberdrop-dl-4.2.28.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:48.780181 cyberdrop-dl-4.2.27/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-16 22:37:48.780181 cyberdrop-dl-4.2.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17394 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:48.772181 cyberdrop-dl-4.2.27/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:48.776181 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:48.776181 cyberdrop-dl-4.2.27/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:48.776181 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:48.780181 cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17721 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:48.780181 cyberdrop-dl-4.2.27/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:37:48.772181 cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-16 22:37:48.000000 cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-16 22:37:48.000000 cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:37:48.000000 cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 22:37:48.000000 cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 22:37:48.000000 cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 22:37:48.000000 cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 22:37:48.780181 cyberdrop-dl-4.2.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:37:39.000000 cyberdrop-dl-4.2.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17394 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.136266 cyberdrop-dl-4.2.28/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.140266 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.140266 cyberdrop-dl-4.2.28/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:10:18.140266 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 06:10:18.000000 cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-18 06:10:18.144266 cyberdrop-dl-4.2.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:10:09.000000 cyberdrop-dl-4.2.28/setup.py
```

### Comparing `cyberdrop-dl-4.2.27/LICENSE` & `cyberdrop-dl-4.2.28/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/PKG-INFO` & `cyberdrop-dl-4.2.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.27
+Version: 4.2.28
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.27 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.28 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.27/README.md` & `cyberdrop-dl-4.2.28/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 title = await make_title_safe(title)
 
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
             pages_tag = soup.select("a[onclick*=loadImages]")[-1]
             assert pages_tag is not None
             pages_str = pages_tag.get('onclick')
             assert isinstance(pages_str, str)
-            total_pages = int(pages_str.split(',')[2])
+            total_pages = int(pages_str.split(',')[2].split(")")[0].strip())
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
                 with contextlib.suppress(TypeError):
                     folder_id = listing.get('folderid')
                     if not folder_id:
                         continue
                     assert isinstance(folder_id, str)
@@ -204,15 +204,15 @@
                 content = await session.post(self.load_files, data)
             text = content['html']
             title = title if title else content['page_title']
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
 
             page_ref = soup.select("a[onclick*=loadImages]")[-1].get('onclick')
             assert isinstance(page_ref, str)
-            total_pages = int(page_ref.split(',')[2])
+            total_pages = int(page_ref.split(',')[2].split(")")[0].strip())
 
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
                 with contextlib.suppress(TypeError, AttributeError):
                     filename = listing.select_one('span[class=filename]')
                     if filename:
                         temp_title = title + '/' + await make_title_safe(filename.text)
```

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,39 +141,31 @@
 
             if url_path not in self.current_attempt:
                 self.current_attempt[url_path] = 0
 
             complete_file = (self.CDL_Helper.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
-            fake_download = False
-            if self.CDL_Helper.mark_downloaded:
-                fake_download = True
-
             complete_file, partial_file, proceed = await self.check_file_exists(complete_file, partial_file, media,
                                                                                 album, url_path, original_filename,
                                                                                 self.throttle)
-            if not proceed:
-                fake_download = True
+            fake_download = self.CDL_Helper.mark_downloaded or not proceed
 
             await self.CDL_Helper.SQL_Helper.update_pre_download(complete_file, media.filename, url_path,
                                                                  original_filename)
 
-            resume_point = 0
             await self.CDL_Helper.SQL_Helper.sql_insert_temp(str(partial_file))
-            range_num = None
-            if partial_file.exists():
-                resume_point = partial_file.stat().st_size
-                range_num = f'bytes={resume_point}-'
+            resume_point = partial_file.stat().st_size if partial_file.exists() else 0
 
             assert media.url.host is not None
-            headers = {"Authorization": await basic_auth("Cyberdrop-DL", self.CDL_Helper.pixeldrain_api_key)} \
-                if (self.CDL_Helper.pixeldrain_api_key and "pixeldrain" in media.url.host) else {}
-            if range_num:
-                headers['Range'] = range_num
+            headers = {}
+            if self.CDL_Helper.pixeldrain_api_key and "pixeldrain" in media.url.host:
+                headers["Authorization"] = await basic_auth("Cyberdrop-DL", self.CDL_Helper.pixeldrain_api_key)
+            if resume_point:
+                headers['Range'] = f'bytes={resume_point}-'
 
             file_task = self.Progress_Master.FileProgress.add_file(media.filename)
 
             if not await self.CDL_Helper.SQL_Helper.sql_check_old_existing(url_path) and not fake_download:
                 await self.download_session.download_file(self.Progress_Master, media, partial_file, self.throttle,
                                                           resume_point, self.CDL_Helper.proxy, headers, file_task)
                 partial_file.rename(complete_file)
```

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,42 +145,34 @@
 
             current_throttle = self.client.throttle
 
             original_filename = media.filename
             complete_file = (self.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
-            fake_download = False
-            if self.mark_downloaded:
-                fake_download = True
-
             complete_file, partial_file, proceed = await self.check_file_exists(complete_file, partial_file, media,
                                                                                 album, url_path, original_filename,
                                                                                 current_throttle)
-            if not proceed:
-                fake_download = True
+            fake_download = self.mark_downloaded or not proceed
 
             await self.SQL_Helper.update_pre_download(complete_file, media.filename, url_path, original_filename)
 
-            resume_point = 0
             await self.SQL_Helper.sql_insert_temp(str(partial_file))
-            range_num = None
-            if partial_file.exists():
-                resume_point = partial_file.stat().st_size
-                range_num = f'bytes={resume_point}-'
+            resume_point = partial_file.stat().st_size if partial_file.exists() else 0
 
             assert media.url.host is not None
             for key, value in self.delay.items():
                 if key in media.url.host:
                     current_throttle = value
 
-            headers = {"Authorization": await basic_auth("Cyberdrop-DL", self.pixeldrain_api_key)} \
-                if (self.pixeldrain_api_key and "pixeldrain" in media.url.host) else {}
-            if range_num:
-                headers['Range'] = range_num
+            headers = {}
+            if self.pixeldrain_api_key and "pixeldrain" in media.url.host:
+                headers["Authorization"] = await basic_auth("Cyberdrop-DL", self.pixeldrain_api_key)
+            if resume_point:
+                headers['Range'] = f'bytes={resume_point}-'
 
             if not await self.SQL_Helper.sql_check_old_existing(url_path) and not fake_download:
                 await self.download_session.old_download_file(media, partial_file, current_throttle, resume_point,
                                                               self.proxy, headers)
                 partial_file.rename(complete_file)
 
             await self.SQL_Helper.mark_complete(url_path, original_filename)
```

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.28/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.27
+Version: 4.2.28
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.27 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.28 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.27/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.28/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.27/setup.cfg` & `cyberdrop-dl-4.2.28/setup.cfg`

 * *Files identical despite different names*

