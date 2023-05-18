# Comparing `tmp/starrail-toolkit-0.5.6.tar.gz` & `tmp/starrail-toolkit-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.5.6.tar", last modified: Thu May 11 18:40:15 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.5.8.tar", last modified: Thu May 18 17:24:08 2023, max compression
```

## Comparing `starrail-toolkit-0.5.6.tar` & `starrail-toolkit-0.5.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.563663 starrail-toolkit-0.5.6/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     5400 2023-05-11 18:40:15.563530 starrail-toolkit-0.5.6/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     4893 2023-05-11 18:36:26.000000 starrail-toolkit-0.5.6/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-11 18:40:15.563702 starrail-toolkit-0.5.6/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.557408 starrail-toolkit-0.5.6/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-11 13:36:54.000000 starrail-toolkit-0.5.6/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.557901 starrail-toolkit-0.5.6/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3000 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      988 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.559207 starrail-toolkit-0.5.6/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1103 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5078 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3665 2023-05-11 14:02:35.000000 starrail-toolkit-0.5.6/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.559445 starrail-toolkit-0.5.6/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5958 2023-05-09 19:22:18.000000 starrail-toolkit-0.5.6/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.560070 starrail-toolkit-0.5.6/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      978 2023-05-11 13:36:55.000000 starrail-toolkit-0.5.6/starrail/gui/common/config.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1136 2023-05-11 13:36:49.000000 starrail-toolkit-0.5.6/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.560906 starrail-toolkit-0.5.6/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    12864 2023-05-11 14:01:58.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-11 18:38:07.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4285 2023-05-11 18:38:38.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.561359 starrail-toolkit-0.5.6/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5401 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.561847 starrail-toolkit-0.5.6/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1855 2023-05-11 18:32:57.000000 starrail-toolkit-0.5.6/starrail/utils/accounts.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      937 2023-05-09 19:22:18.000000 starrail-toolkit-0.5.6/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.562617 starrail-toolkit-0.5.6/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     3088 2023-05-11 14:19:58.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-11 18:37:45.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6791 2023-05-11 18:38:18.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-09 12:43:20.000000 starrail-toolkit-0.5.6/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-11 14:03:34.000000 starrail-toolkit-0.5.6/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-11 18:40:15.563366 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     5400 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1530 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-11 18:40:15.000000 starrail-toolkit-0.5.6/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.630131 starrail-toolkit-0.5.8/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5497 2023-05-18 17:24:08.630006 starrail-toolkit-0.5.8/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4990 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-18 17:24:08.630169 starrail-toolkit-0.5.8/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.624603 starrail-toolkit-0.5.8/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.625084 starrail-toolkit-0.5.8/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3000 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      988 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.626150 starrail-toolkit-0.5.8/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1103 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5092 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4547 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.626385 starrail-toolkit-0.5.8/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6046 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.626983 starrail-toolkit-0.5.8/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      978 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/common/config.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      260 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.627624 starrail-toolkit-0.5.8/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1842 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    13661 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4267 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.628033 starrail-toolkit-0.5.8/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.628458 starrail-toolkit-0.5.8/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1832 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/utils/accounts.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      937 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.629146 starrail-toolkit-0.5.8/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3291 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     7271 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-15 03:28:48.000000 starrail-toolkit-0.5.8/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-18 17:23:29.000000 starrail-toolkit-0.5.8/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-18 17:24:08.629842 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5497 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1530 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-18 17:24:08.000000 starrail-toolkit-0.5.8/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.5.6/LICENSE` & `starrail-toolkit-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/PKG-INFO` & `starrail-toolkit-0.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.6
+Version: 0.5.8
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,25 +14,25 @@
 License-File: LICENSE
 
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
-
-
 ## 开发状态
 
-| 主分支版本 | 开发分支版本 | PyPI 版本 |
-| :--------: | :----------: | :-------: |
-|   0.5.4    |    0.5.6     |   0.5.6   |
+| 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
+| :--------: | :----------: | :-------: | :--------: |
+|   0.5.8    |    0.5.8     |   0.5.8   |   0.5.4    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [ ] 支持更多的可设置选项
+- [ ] 支持国际服
+- [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
 - [ ] 美化抽卡导出页面
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
```

### Comparing `starrail-toolkit-0.5.6/README.md` & `starrail-toolkit-0.5.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
-
-
 ## 开发状态
 
-| 主分支版本 | 开发分支版本 | PyPI 版本 |
-| :--------: | :----------: | :-------: |
-|   0.5.4    |    0.5.6     |   0.5.6   |
+| 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
+| :--------: | :----------: | :-------: | :--------: |
+|   0.5.8    |    0.5.8     |   0.5.8   |   0.5.4    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [ ] 支持更多的可设置选项
+- [ ] 支持国际服
+- [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
 - [ ] 美化抽卡导出页面
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
```

### Comparing `starrail-toolkit-0.5.6/setup.py` & `starrail-toolkit-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/__init__.py` & `starrail-toolkit-0.5.8/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/config.py` & `starrail-toolkit-0.5.8/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/entry/cli.py` & `starrail-toolkit-0.5.8/starrail/entry/cli.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/entry/gui.py` & `starrail-toolkit-0.5.8/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/entry/setup.py` & `starrail-toolkit-0.5.8/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gacha/autodet.py` & `starrail-toolkit-0.5.8/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gacha/database.py` & `starrail-toolkit-0.5.8/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gacha/fetch.py` & `starrail-toolkit-0.5.8/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gacha/fileio.py` & `starrail-toolkit-0.5.8/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gacha/parse.py` & `starrail-toolkit-0.5.8/starrail/gacha/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         total_items = len(self.data)
         if not total_items or not count:
             return dict(
                 rank_type=rank_type,
                 count='0',
                 basic_prob='',
                 compr_prob='',
-                since_last='',
+                since_last=f'{total_items}',
                 attempts=[],
                 average='',
             )
         if rank_type == '3':
             return dict(
                 rank_type=rank_type,
                 count=f'{count}',
```

### Comparing `starrail-toolkit-0.5.6/starrail/gacha/service.py` & `starrail-toolkit-0.5.8/starrail/gacha/service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import time
 from datetime import datetime
 
 import starrail.gacha.fileio as fileio
 from starrail.gacha.autodet import detect_api_url
 from starrail.gacha.fetch import fetch_json
@@ -18,32 +19,29 @@
     r = 1
     while True:
         yield r
         r += 1
 
 
 def check_response(payload, code):
-    if payload is None or not 200 <= code < 300:
-        logger.info(f'Whether payload is None: {payload is None}')
-        logger.info(f'Status code: {code}')
-        return False
-    if 'data' not in payload or 'list' not in payload['data']:
-        logger.info(f'Whether payload contains `data`: {"data" in payload}')
-        logger.info(
-            f'Whether payload data contains `list`:'
-            f'{"list" in payload["data"]}',
-        )
-        return False
-    if not payload['data']['list']:
-        logger.info(
-            f'Length of payload.data.list: '
-            f'{len(payload["data"]["list"])}',
-        )
-        return False
-    return True
+    # returns: is_valid, should_stop, massage
+    resp = json.dumps(payload, ensure_ascii=False)
+    if payload is None:  # check payload
+        return False, True, f'Payload is None, response: {resp}'
+    elif not 200 <= code < 300:  # check request
+        return False, True, f'Request fail, code: {code}, response: {resp}'
+    elif 'data' not in payload:  # check data
+        return False, True, f'data is not in payload, response: {resp}'
+    elif not payload['data']:  # check data empty or null
+        return False, True, f'data is empty or None, response: {resp}'
+    elif 'list' not in payload['data']:  # check field
+        return False, True, f'data.list is missing, response: {resp}'
+    elif not payload['data']['list']:  # check data list
+        return True, True, 'valid but reaching the end of list'
+    return True, False, 'ok'
 
 
 def export_gacha_type(
     api_template: str,
     gacha_type: GachaType,
     request_interval: float,
 ):
@@ -54,52 +52,72 @@
         api_url = get_api_url(
             api_template, end_id, str(gacha_type.value),
             str(page), '5',
         )
         logger.debug(f'Requesting {api_url}')
         response, code = fetch_json(api_url)
         time.sleep(request_interval)
-        if not check_response(response, code):
+        _, should_stop, msg = check_response(response, code)
+        logger.info(f'check_response: {msg}')
+        if should_stop:
             break
         data_list = response['data']['list']
         r.extend(data_list)
         end_id = data_list[-1]['id']
     return r
 
 
+def deduce_uid(record_cache):
+    for gacha_type in GachaType:
+        records = record_cache[gacha_type.value]
+        if records:
+            return records[0]['uid']
+    return ''
+
+
 def export_gacha_from_api(api_url, export, request_interval):
     if not api_url:
         api_url = detect_api_url()
     response, code = fetch_json(api_url)
-    valid = check_response(response, code)
+    valid, _, msg = check_response(response, code)
+    logger.info(f'check_response (api): {msg}')
     if not valid:
         logger.fatal('Error while checking response from api URL, exitting')
         raise ValueError('Invalid or expired api, please check your input')
 
     api_template = get_url_template(api_url)
-
-    uid = response['data']['list'][0]['uid']
-    manager = GachaDataManager(uid)
-    logger.info(f'Successfully connected to cache of uid {uid}')
-    manager.log_stats()
+    record_cache = dict()
 
     for gacha_type in GachaType:
         records = export_gacha_type(
             api_template,
             gacha_type,
             request_interval,
         )
-        manager.add_records(gacha_type.value, records)
-        manager.gacha[gacha_type.value].sort()
+        record_cache[gacha_type.value] = records
         logger.info(f'Finish downloading records of {gacha_type.name}')
 
+    uid = deduce_uid(record_cache)
+    if not uid:
+        logger.fatal(
+            'Cannot deduce uid from records, there may be no gacha '
+            'record. Please check your account and try again.',
+        )
+        raise ValueError('Cannot deduce uid from records')
+    manager = GachaDataManager(uid)
+    logger.info(f'Successfully connected to cache of uid {uid}')
+    manager.log_stats()
+
+    for gacha_type in GachaType:
+        manager.add_records(gacha_type.value, record_cache[gacha_type.value])
+        manager.gacha[gacha_type.value].sort()
+
     fileio.export_as_sql(manager, manager.cache_path)
 
     account_record.update_timestamp(uid)
-
     manager.log_stats()
 
     export_hooks = dict(
         csv=fileio.export_as_csv,
         html=fileio.export_as_html,
         json=fileio.export_as_json,
         md=fileio.export_as_md,
```

### Comparing `starrail-toolkit-0.5.6/starrail/gacha/url.py` & `starrail-toolkit-0.5.8/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gui/application.py` & `starrail-toolkit-0.5.8/starrail/gui/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import qfluentwidgets
 from PySide6.QtCore import QEasingCurve, Qt, Signal
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QApplication, QFrame, QHBoxLayout, QWidget
 from qfluentwidgets import NavigationInterface, NavigationItemPosition
 from qframelesswindow import FramelessWindow
 
+from starrail.gui.common.config import qcfg
 from starrail.gui.common.icon import Icon
 from starrail.gui.common.stylesheet import StyleSheet
 from starrail.gui.common.utils import checkUpdate
 from starrail.gui.interfaces.gacha_sync import GachaSyncInterface
 from starrail.gui.interfaces.home import HomeInterface
 from starrail.gui.interfaces.setting import SettingInterface
 from starrail.gui.interfaces.users import UsersInterface
@@ -175,8 +176,9 @@
         StyleSheet.STAR_RAIL_TOOLKIT.apply(self)
 
     def resizeEvent(self, _):
         self.titleBar.move(46, 0)
         self.titleBar.resize(self.width() - 46, self.titleBar.height())
 
     def afterShow(self):
-        checkUpdate(self)
+        if qcfg.get(qcfg.check_update):
+            checkUpdate(self)
```

### Comparing `starrail-toolkit-0.5.6/starrail/gui/common/config.py` & `starrail-toolkit-0.5.8/starrail/gui/common/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.5.8/starrail/gui/common/stylesheet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.5.8/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.5.8/starrail/gui/interfaces/gacha_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,43 +55,60 @@
             api_url = service.get_api_url(
                 api_template, end_id, str(gacha_type.value),
                 str(page), '5',
             )
             logger.debug(f'Requesting {api_url}')
             response, code = service.fetch_json(api_url)
             time.sleep(request_interval)
-            if not service.check_response(response, code):
+            _, should_stop, msg = service.check_response(response, code)
+            logger.info(f'check_response: {msg}')
+            if should_stop:
                 break
             data_list = response['data']['list']
             r.extend(data_list)
             end_id = data_list[-1]['id']
         return r
 
     def syncGachaData(self):
         self.logAndUpdateState(babelfish.ui_extracting_api_url())
         api_url = service.detect_api_url()
         response, code = service.fetch_json(api_url)
-        valid = service.check_response(response, code)
+        valid, _, msg = service.check_response(response, code)
+        logger.info(f'check_response (api): {msg}')
         if not valid:
             self.syncFailSignal.emit(babelfish.ui_extract_api_fail())
-            raise ValueError(babelfish.ui_extract_api_fail())
+            raise ValueError(babelfish.ui_extract_api_fail_with_msg(msg))
 
         api_template = service.get_url_template(api_url)
-
-        uid = response['data']['list'][0]['uid']
-        manager = service.GachaDataManager(uid)
-        manager.log_stats()
+        record_cache = dict()
 
         for gacha_type in service.GachaType:
             records = self.exportGachaType(
                 api_template,
                 gacha_type,
                 0.15,
             )
-            manager.add_records(gacha_type.value, records)
+            record_cache[gacha_type.value] = records
+            logger.info(f'Finish downloading records of {gacha_type.name}')
+
+        uid = service.deduce_uid(record_cache)
+        if not uid:
+            logger.critical(
+                'Cannot deduce uid from records, there may be no '
+                'record. Please check and try again.',
+            )
+            raise ValueError(babelfish.ui_deduce_uid_fail())
+        manager = service.GachaDataManager(uid)
+        logger.info(f'Successfully connected to cache of uid {uid}')
+        manager.log_stats()
+
+        for gacha_type in service.GachaType:
+            manager.add_records(
+                gacha_type.value, record_cache[gacha_type.value],
+            )
             manager.gacha[gacha_type.value].sort()
 
         service.fileio.export_as_sql(manager, manager.cache_path)
         manager.log_stats()
 
         return uid
 
@@ -332,19 +349,20 @@
         self.saveButton.setEnabled(True)
 
         self.onSyncSuccess()
 
     def syncFailSlot(self, message: str):
         logger.info(f'[GUI] Gacha data sync fail with message {message}')
 
-        self.syncToolTip.setTitle(babelfish.ui_sync_gacha_fail())
-        self.syncToolTip.setContent('')
-        self.syncToolTip.setState(True)
-        self.syncToolTip = None
-        self.syncThread = None
+        if self.syncToolTip is not None:
+            self.syncToolTip.setTitle(babelfish.ui_sync_gacha_fail())
+            self.syncToolTip.setContent('')
+            self.syncToolTip.setState(True)
+            self.syncToolTip = None
+            self.syncThread = None
 
         qfw.InfoBar.error(
             title=babelfish.ui_sync_gacha_fail(),
             content=message,
             orient=Qt.Orientation.Horizontal,
             isClosable=True,
             duration=-1,
```

### Comparing `starrail-toolkit-0.5.6/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.5.8/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.5.8/starrail/gui/interfaces/setting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-from functools import partial
-
 import qfluentwidgets as qfw
-from PySide6.QtCore import Qt, Signal
+from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QLabel, QWidget
 from qfluentwidgets import FluentIcon
 
 from starrail import __version__
 from starrail.gui.common.config import qcfg
 from starrail.gui.common.stylesheet import StyleSheet
 from starrail.gui.common.utils import checkUpdate
 from starrail.utils import babelfish
 
 
 class SettingInterface(qfw.ScrollArea):
 
-    checkUpdateSig = Signal()
-
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.scrollWidget = QWidget()
         self.expandLayout = qfw.ExpandLayout(self.scrollWidget)
 
         self.settingLabel = QLabel(babelfish.ui_settings(), self)
 
@@ -80,17 +76,15 @@
             babelfish.ui_about_this(),
             (
                 f'{babelfish.ui_copyright(2023)} '
                 f'{babelfish.ui_current_version(__version__)}'
             ),
             self.aboutGroup,
         )
-        self.aboutCard.button.clicked.connect(
-            partial(checkUpdate, parent=self.parent()),
-        )
+        self.aboutCard.button.clicked.connect(self.checkUpdateAction)
 
         self.__initWidget()
         self.__initLayout()
         self.__connectSignalToSlot()
 
     def __initWidget(self):
         self.resize(1000, 800)
@@ -118,7 +112,10 @@
         self.expandLayout.setSpacing(28)
         self.expandLayout.setContentsMargins(36, 10, 36, 0)
         self.expandLayout.addWidget(self.personalGroup)
         self.expandLayout.addWidget(self.aboutGroup)
 
     def __connectSignalToSlot(self):
         qfw.qconfig.themeChanged.connect(qfw.setTheme)
+
+    def checkUpdateAction(self):
+        checkUpdate(parent=self.parent(), show_success=True)
```

### Comparing `starrail-toolkit-0.5.6/starrail/gui/widgets/dialog.py` & `starrail-toolkit-0.5.8/starrail/gui/widgets/dialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,27 +112,28 @@
         StyleSheet.CHECK_UPDATE_DIALOG.apply(self)
 
         self.cancelButton.adjustSize()
         self.ghButton.adjustSize()
         self.ndButton.adjustSize()
 
     def __adjustText(self):
-        if self.isWindow():
-            if self.parent():
-                w = max(self.titleLabel.width(), self.parent().width())
-                chars = max(min(w / 9, 140), 30)
-            else:
-                chars = 100
-        else:
-            w = max(self.titleLabel.width(), self.window().width())
-            chars = max(min(w / 9, 100), 30)
+        # if self.isWindow():
+        #     if self.parent():
+        #         w = max(self.titleLabel.width(), self.parent().width())
+        #         chars = max(min(w / 9, 140), 30)
+        #     else:
+        #         chars = 100
+        # else:
+        #     w = max(self.titleLabel.width(), self.window().width())
+        #     chars = max(min(w / 9, 100), 30)
 
-        self.contentLabel.setText(
-            qfw.TextWrap.wrap(self.content, chars, False)[0],
-        )
+        # self.contentLabel.setText(
+        #     qfw.TextWrap.wrap(self.content, chars, False)[0],
+        # )
+        pass
 
     def onCancelClicked(self):
         self.reject()
 
     def onGhClicked(self):
         self.accept()
         if self.dist is not None and self.dist['GitHub_dist']:
```

### Comparing `starrail-toolkit-0.5.6/starrail/gui/widgets/link_card.py` & `starrail-toolkit-0.5.8/starrail/gui/widgets/link_card.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.5.8/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/utils/accounts.py` & `starrail-toolkit-0.5.8/starrail/utils/accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
         self.flush()
 
     def latest_uid(self):
         return self.meta['latest']
 
 
 account_record = AccountRecord(cfg.account_record_path)
-account_record.flush()
 
 
 def get_latest_uid():
     if account_record.latest_uid():
         return account_record.latest_uid()
     if os.path.isdir(cfg.db_dir):
         caches = os.listdir(cfg.db_dir)
```

### Comparing `starrail-toolkit-0.5.6/starrail/utils/auto_update.py` & `starrail-toolkit-0.5.8/starrail/utils/auto_update.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.5.8/starrail/utils/babelfish/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 html_thead = dictionary.html_thead
 markdown_thead = dictionary.markdown_thead
 ui_about = dictionary.ui_about
 ui_about_this = dictionary.ui_about_this
 ui_cancel_update = dictionary.ui_cancel_update
 ui_check_update = dictionary.ui_check_update
 ui_check_update_fail = dictionary.ui_check_update_fail
+ui_check_update_success = dictionary.ui_check_update_success
 ui_copyright = dictionary.ui_copyright
 ui_current_version = dictionary.ui_current_version
+ui_deduce_uid_fail = dictionary.ui_deduce_uid_fail
 ui_downloading_gacha = dictionary.ui_downloading_gacha
 ui_extract_api_fail = dictionary.ui_extract_api_fail
+ui_extract_api_fail_with_msg = dictionary.ui_extract_api_fail_with_msg
 ui_extracting_api_url = dictionary.ui_extracting_api_url
 ui_fine = dictionary.ui_fine
 ui_fine1 = dictionary.ui_fine1
 ui_fine2 = dictionary.ui_fine2
 ui_gacha_basic_prob = dictionary.ui_gacha_basic_prob
 ui_gacha_count = dictionary.ui_gacha_count
 ui_gacha_since_last = dictionary.ui_gacha_since_last
@@ -29,14 +32,15 @@
 ui_gacha_sync_desc = dictionary.ui_gacha_sync_desc
 ui_gacha_true_prob = dictionary.ui_gacha_true_prob
 ui_gacha_type = dictionary.ui_gacha_type
 ui_get_started = dictionary.ui_get_started
 ui_get_started_desc = dictionary.ui_get_started_desc
 ui_github_repo = dictionary.ui_github_repo
 ui_github_repo_desc = dictionary.ui_github_repo_desc
+ui_is_latest_version = dictionary.ui_is_latest_version
 ui_no_data = dictionary.ui_no_data
 ui_not_good = dictionary.ui_not_good
 ui_ooops = dictionary.ui_ooops
 ui_open_docs = dictionary.ui_open_docs
 ui_open_issues = dictionary.ui_open_issues
 ui_open_repo = dictionary.ui_open_repo
 ui_open_troubleshooting = dictionary.ui_open_troubleshooting
@@ -62,10 +66,9 @@
 ui_troubleshooting = dictionary.ui_troubleshooting
 ui_troubleshooting_desc = dictionary.ui_troubleshooting_desc
 ui_update_available = dictionary.ui_update_available
 ui_update_desc = dictionary.ui_update_desc
 ui_users = dictionary.ui_users
 ui_users_desc = dictionary.ui_users_desc
 ui_welcome = dictionary.ui_welcome
-ui_welcome = dictionary.ui_welcome
 
 __all__ = ['constants', 'translate']
```

### Comparing `starrail-toolkit-0.5.6/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.5.8/starrail/utils/babelfish/dictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,30 +47,42 @@
 ui_about_this = _MS(en='About This Application', zhs='关于本软件')
 ui_cancel_update = _MS(en='Cancel Update', zhs='暂不更新')
 ui_check_update = _MS(en='Check Update', zhs='检查更新')
 ui_check_update_fail = _MS(
     en='Check update failed. Please check your network connection.',
     zhs='检查更新失败，请检查你的网络连接并重试。（不重试也行，但是你可能没联网）',
 )
+ui_check_update_success = _MS(
+    en='Check update finished',
+    zhs='检查更新完成',
+)
 ui_copyright = _MS(
     en='Copyright © {} LittleNyima.',
     zhs='版权所有 © {} LittleNyima。',
 )
 ui_current_version = _MS(
     en='Current version: {}.',
     zhs='当前版本：{}。',
 )
+ui_deduce_uid_fail = _MS(
+    en='Fail to deduce uid. There may be no record. Please check.',
+    zhs='检测 UID 失败，账号可能没有抽卡记录，请重试。',
+)
 ui_downloading_gacha = _MS(
     en='Downloading page {page} of type {name}',
     zhs='正在导出{name}的第{page}页',
 )
 ui_extract_api_fail = _MS(
     en='Extracting API URL failed. Please retry after exiting the game.',
     zhs='提取 API URL 失败，请关闭游戏或重新查询抽卡信息后重试。',
 )
+ui_extract_api_fail_with_msg = _MS(
+    en='Extracting API URL failed. Failed with: {}',
+    zhs='提取 API URL 失败，遇到的问题：{}',
+)
 ui_extracting_api_url = _MS(
     en='Extracting API URL',
     zhs='正在提取 API URL',
 )
 ui_fine = _MS(en='Fine', zhs='好')
 ui_fine1 = _MS(en='Fine', zhs='好的')
 ui_fine2 = _MS(en='Fine', zhs='好吧')
@@ -93,14 +105,18 @@
     zhs='学习本工具箱的基本使用方法。',
 )
 ui_github_repo = _MS(en='GitHub Repo', zhs='开源代码')
 ui_github_repo_desc = _MS(
     en='This project is open-resource, licenced under GPLv3. View code here.',
     zhs='本项目代码开源，以 GPLv3 分发。点此查看源代码。',
 )
+ui_is_latest_version = _MS(
+    en='Your application is the latest version.',
+    zhs='已经是最新版本啦',
+)
 ui_no_data = _MS(en='No Data', zhs='暂无数据')
 ui_not_good = _MS(en='No', zhs='不好')
 ui_ooops = _MS(en='OOOPS!', zhs='出错了！')
 ui_open_docs = _MS(en='Open Documentations', zhs='打开帮助页面')
 ui_open_issues = _MS(en='Open Issue Page', zhs='打开反馈页面')
 ui_open_repo = _MS(en='Open GitHub Repo', zhs='打开代码仓库')
 ui_open_troubleshooting = _MS(en='Open Troubleshooting', zhs='打开常见问题')
@@ -164,10 +180,9 @@
 )
 ui_users = _MS(en='Users', zhs='用户管理')
 ui_users_desc = _MS(en='Multi-user management', zhs='如果有多个账号可以用这个切换')
 ui_welcome = _MS(
     en='Welcome to HKSR Toolkit!',
     zhs='欢迎登车！',
 )
-ui_welcome = _MS(en='Welcome', zhs='欢迎页面')
 
 # === END OF PRE-DEFINED VOCABULARIES ===
```

### Comparing `starrail-toolkit-0.5.6/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.5.8/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail/utils/loggings.py` & `starrail-toolkit-0.5.8/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.5.6/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.5.8/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.5.6
+Version: 0.5.8
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,25 +14,25 @@
 License-File: LICENSE
 
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
-
-
 ## 开发状态
 
-| 主分支版本 | 开发分支版本 | PyPI 版本 |
-| :--------: | :----------: | :-------: |
-|   0.5.4    |    0.5.6     |   0.5.6   |
+| 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
+| :--------: | :----------: | :-------: | :--------: |
+|   0.5.8    |    0.5.8     |   0.5.8   |   0.5.4    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [ ] 支持更多的可设置选项
+- [ ] 支持国际服
+- [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
 - [ ] 美化抽卡导出页面
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
```

### Comparing `starrail-toolkit-0.5.6/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.5.8/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

