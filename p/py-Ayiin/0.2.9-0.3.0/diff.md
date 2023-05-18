# Comparing `tmp/py-Ayiin-0.2.9.tar.gz` & `tmp/py-Ayiin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.2.9.tar", last modified: Sat May  6 06:10:44 2023, max compression
+gzip compressed data, was "py-Ayiin-0.3.0.tar", last modified: Thu May 18 06:36:12 2023, max compression
```

## Comparing `py-Ayiin-0.2.9.tar` & `py-Ayiin-0.3.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.500676 py-Ayiin-0.2.9/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.500676 py-Ayiin-0.2.9/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38206 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-06 06:10:44.000000 py-Ayiin-0.2.9/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-06 06:10:44.000000 py-Ayiin-0.2.9/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:10:44.000000 py-Ayiin-0.2.9/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-06 06:10:44.000000 py-Ayiin-0.2.9/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 06:10:44.000000 py-Ayiin-0.2.9/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 06:10:44.504677 py-Ayiin-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-06 06:10:27.000000 py-Ayiin-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.263418 py-Ayiin-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-18 06:36:12.263418 py-Ayiin-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.259418 py-Ayiin-0.3.0/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.259418 py-Ayiin-0.3.0/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.259418 py-Ayiin-0.3.0/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/gcast_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.259418 py-Ayiin-0.3.0/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.263418 py-Ayiin-0.3.0/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.263418 py-Ayiin-0.3.0/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.263418 py-Ayiin-0.3.0/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.263418 py-Ayiin-0.3.0/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:36:12.263418 py-Ayiin-0.3.0/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-18 06:36:12.000000 py-Ayiin-0.3.0/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-18 06:36:12.000000 py-Ayiin-0.3.0/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:36:12.000000 py-Ayiin-0.3.0/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-18 06:36:12.000000 py-Ayiin-0.3.0/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 06:36:12.000000 py-Ayiin-0.3.0/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:36:12.263418 py-Ayiin-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-18 06:35:58.000000 py-Ayiin-0.3.0/setup.py
```

### Comparing `py-Ayiin-0.2.9/LICENSE` & `py-Ayiin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/NOTICE` & `py-Ayiin-0.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/PKG-INFO` & `py-Ayiin-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.2.9/README.md` & `py-Ayiin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.3.0/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/Clients/client.py` & `py-Ayiin-0.3.0/pyAyiin/Clients/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,62 @@
+from pyrogram import Client as PyroClient
 from fipper import Client
 
+from telethon import TelegramClient
+from telethon.sessions import MemorySession
+
+from . import *
+
+from config import Var
+
+
+
 from ..config import Var as Variable
 
 Var = Variable()
 
 
 hndlr = f"{Var.HNDLR[0]} {Var.HNDLR[1]} {Var.HNDLR[2]} {Var.HNDLR[3]} {Var.HNDLR[4]} {Var.HNDLR[5]}"
 
-'''
+
 try:
-    import pytgcalls
+    from pytgcalls import PyTgCalls
 except ImportError:
-    print("'pytgcalls' not found")
     pytgcalls = None
-'''
+
+
+TeleBot = TelegramClient(
+    MemorySession(), 
+    Var.API_ID, 
+    Var.API_HASH
+)
+
+
+assist = PyroClient(
+    api_id=Var.API_ID, 
+    api_hash=Var.API_HASH, 
+    session_name=str(Var.ASS_STRING),
+)
+assistant = PyTgCalls(
+    assist,
+    cache_duration=100,
+    overload_quiet_mode=True,
+)
 
 
 tgbot = (
     Client(
         name="tgbot",
         api_id=Var.API_ID,
         api_hash=Var.API_HASH,
         bot_token=Var.BOT_TOKEN,
     )
 )
 
+
 # For Publik Repository
 AYIIN1 = (
     Client(
         name="AYIIN1",
         api_id=Var.API_ID,
         api_hash=Var.API_HASH,
         session_string=Var.STRING_1,
@@ -679,17 +707,7 @@
         AYIIN46,
         AYIIN47,
         AYIIN48,
         AYIIN49,
         AYIIN50,
     ] if bot
 ]
-
-'''
-if pytgcalls is not None:
-    for bot in Bots:
-        if not hasattr(bot, "group_call"):
-            try:
-                setattr(bot, "group_call", pytgcalls.GroupCallFactory(bot).get_group_call())
-            except AttributeError:
-                pass
-'''
```

### Comparing `py-Ayiin-0.2.9/pyAyiin/Clients/startup.py` & `py-Ayiin-0.3.0/pyAyiin/Clients/startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,27 @@
             display_module=False,
             exclude=Var.NO_LOAD,
         )
         logs.info(f"{plugins} Total Plugins User")
     except BaseException as e:
         logs.info(e)
         sys.exit()
+    if Var.TELEBOT == "True":
+        logs.info('Starting Telethon Bot...')
+        await TeleBot.start(bot_token=Var.BOT_TOKEN)
+        me = await TeleBot.get_me()
+        bot_id = me.id
+        if me.last_name:
+            bot_name = me.first_name + " " + me.last_name
+        else:
+            bot_name = me.first_name
+        logs.info(
+            f"TeleBot in {bot_name} | [ {bot_id} ]"
+        )
+        client_id.append(bot_id)
     if tgbot:
         await tgbot.start()
         me = await tgbot.get_me()
         tgbot.id = me.id
         tgbot.mention = me.mention
         tgbot.username = me.username
         if me.last_name:
```

### Comparing `py-Ayiin-0.2.9/pyAyiin/__init__.py` & `py-Ayiin-0.3.0/pyAyiin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,27 +29,29 @@
 
 # Bot Logs setup:
 logging.basicConfig(
     format="[%(name)s] - [%(levelname)s] - %(message)s",
     level=logging.INFO,
 )
 logging.getLogger("pyAyiin").setLevel(logging.INFO)
+logging.getLogger("pytgcalls").setLevel(logging.INFO)
 logging.getLogger("fipper").setLevel(logging.ERROR)
 logging.getLogger("fipper.client").setLevel(logging.ERROR)
 logging.getLogger("fipper.session.auth").setLevel(logging.ERROR)
 logging.getLogger("fipper.session.session").setLevel(logging.ERROR)
+logging.getLogger("telethon").setLevel(logging.INFO)
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.2.9"
-ayiin_ver = "0.0.9"
+__version__ = "0.3.0"
+ayiin_ver = "0.1.0"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
 ]
```

### Comparing `py-Ayiin-0.2.9/pyAyiin/__main__.py` & `py-Ayiin-0.3.0/pyAyiin/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from fipper import idle
 
 from pyAyiin import __version__
 
 from . import *
 
 from .config import Var
+from .Clients.client import assistant
 from .Clients.startup import StartPyrogram
 from .exceptions import DependencyMissingError
 
-yins = Var()
+yinsxd = Var()
 xd = PyrogramXd()
 
 
 try:
     from uvloop import install
 except:
     install = None
@@ -33,24 +34,34 @@
 <b>╰╼┅━━━━━╍━━━━━┅╾</b>
 """
 
 async def start_main():
     await StartPyrogram()
     try:
         await tgbot.send_message(
-            yins.LOG_CHAT,
+            yinsxd.LOG_CHAT,
             MSG_ON.format(
                 __version__,
                 HOSTED_ON,
                 ayiin_ver, 
                 len(CMD_HELP),
             )
         )
     except BaseException as s:
         print(s)
+    if yinsxd.ASS_STRING:
+        try:
+            await assistant.start()
+            await Yins.stream_call(
+                Var.LOG_CHAT,
+                "http://docs.evostream.com/sample_content/assets/sintel1m720p.mp4"
+            )
+        except BaseException as e:
+            logs.info(e)
+        await Yins.decorators()
     print(f"AyiinUbot Version - {ayiin_ver}\n[🔥 BERHASIL DIAKTIFKAN! 🔥]")
     await idle()
     await aiosession.close()
 
 if __name__ == "__main__":
     install()
     xd.heroku()
```

### Comparing `py-Ayiin-0.2.9/pyAyiin/assistant.py` & `py-Ayiin-0.3.0/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/config.py` & `py-Ayiin-0.3.0/pyAyiin/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 class Var(object):
     # mandatory
     API_ID = int(getenv("API_ID"))
     API_HASH = str(getenv("API_HASH"))
     # Extras
     ALIVE_PIC = getenv("ALIVE_PIC", "https://telegra.ph//file/78ec83169711f650f0188.jpg")
     ALIVE_TEXT = getenv("ALIVE_TEXT", "Hai, Saya AyiinUbot")
+    ASS_STRING = getenv("ASS_STRING", "")
+    TELEBOT = getenv("TELEBOT", "False")
     # Telethon Session
     STRING_1 = getenv("STRING_1", "")
     STRING_2 = getenv("STRING_2", "")
     STRING_3 = getenv("STRING_3", "")
     STRING_4 = getenv("STRING_4", "")
     STRING_5 = getenv("STRING_5", "")
     STRING_6 = getenv("STRING_6", "")
```

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/__init__.py` & `py-Ayiin-0.3.0/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/absen.py` & `py-Ayiin-0.3.0/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/admins.py` & `py-Ayiin-0.3.0/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/auth.py` & `py-Ayiin-0.3.0/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.3.0/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.3.0/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/gban.py` & `py-Ayiin-0.3.0/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/langs.py` & `py-Ayiin-0.3.0/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/logdb.py` & `py-Ayiin-0.3.0/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.3.0/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/premium.py` & `py-Ayiin-0.3.0/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/start.py` & `py-Ayiin-0.3.0/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/sudo.py` & `py-Ayiin-0.3.0/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/variable.py` & `py-Ayiin-0.3.0/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.3.0/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/dB/welcome.py` & `py-Ayiin-0.3.0/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/decorator.py` & `py-Ayiin-0.3.0/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/exceptions.py` & `py-Ayiin-0.3.0/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/__init__.py` & `py-Ayiin-0.3.0/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/_misc.py` & `py-Ayiin-0.3.0/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/changer.py` & `py-Ayiin-0.3.0/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/converter.py` & `py-Ayiin-0.3.0/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/func.py` & `py-Ayiin-0.3.0/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/funcb.py` & `py-Ayiin-0.3.0/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/helpers.py` & `py-Ayiin-0.3.0/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/hosting.py` & `py-Ayiin-0.3.0/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.3.0/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/queue.py` & `py-Ayiin-0.3.0/pyAyiin/methods/queue.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 # t.me/AyiinChat & t.me/AyiinSupport
 
 
 # ========================×========================
 #            Jangan Hapus Credit Ngentod
 # ========================×========================
 
+from pycover.types.input_stream import AudioPiped, AudioVideoPiped
+from pycover.types.input_stream.quality import (
+    HighQualityAudio,
+    HighQualityVideo,
+    LowQualityVideo,
+    MediumQualityVideo,
+)
 
 class Queues(object):
     def __init__(self):
         self.queue = {}
 
     def add_to_queue(self, chat_id, songname, link, ref, type, quality):
         if chat_id in self.queue:
@@ -44,32 +51,40 @@
         return 0
     
     async def skip_song(self, client, chat_id):
         try:
             if chat_id in self.queue:
                 chat_queue = self.get_queue(chat_id)
                 if len(chat_queue) == 1:
-                    await client.group_call.leave()
+                    await client.leave_group_call(chat_id)
                     self.clear_queue(chat_id)
                     return 1
                 else:
                     songname = chat_queue[1][0]
                     url = chat_queue[1][1]
                     link = chat_queue[1][2]
                     type = chat_queue[1][3]
-                    chat_queue[1][4]
+                    RESOLUSI = chat_queue[1][4]
                     if type == "Audio":
-                        await client.group_call.start_audio(
-                            url,
-                            repeat=False,
+                        await client.change_stream(
+                            chat_id,
+                            AudioPiped(
+                                url,
+                                HighQualityAudio(),
+                            ),
                         )
                     elif type == "Video":
-                        await client.group_call.start_video(
-                            url,
-                            repeat=False,
+                        if RESOLUSI == 720:
+                            hm = HighQualityVideo()
+                        elif RESOLUSI == 480:
+                            hm = MediumQualityVideo()
+                        elif RESOLUSI == 360:
+                            hm = LowQualityVideo()
+                        await client.change_stream(
+                            chat_id, AudioVideoPiped(url, HighQualityAudio(), hm)
                         )
                     self.pop_an_item(chat_id)
                     return [songname, link, type]
             else:
                 return 0
         except Exception as e:
             print(e)
```

### Comparing `py-Ayiin-0.2.9/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.3.0/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.3.0/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.3.0/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.3.0/pyAyiin/telethon/ayiin/misc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,277 +1,212 @@
-# AyiinXd
-# Copyright (C) 2022-2023 @AyiinXd
+# Ultroid - UserBot
+# Copyright (C) 2021-2022 TeamUltroid
 #
-# This file is a part of < https://github.com/AyiinXd/AyiinXd >
+# This file is a part of < https://github.com/TeamUltroid/Ultroid/ >
 # PLease read the GNU Affero General Public License in
-# <https://www.github.com/AyiinXd/AyiinXd/blob/main/LICENSE/>.
+# <https://www.github.com/TeamUltroid/pyUltroid/blob/main/LICENSE/>.
 #
-# FROM AyiinXd <https://github.com/AyiinXd/AyiinXd>
-# t.me/AyiinChat & t.me/AyiinSupport
+# Ported by @mrismanaziz
+# FROM Man-Userbot <https://github.com/mrismanaziz/Man-Userbot>
+# t.me/SharingUserbot & t.me/Lunatic0de
 
-
-# ========================×========================
-#            Jangan Hapus Credit Ngentod
-# ========================×========================
-
-import aiohttp
-import asyncio
-import importlib
-import math
+import base64
 import os
-import shlex
-import textwrap
-from typing import Tuple, Union
+import os.path
 from io import BytesIO
 
-from pymediainfo import MediaInfo
-from fipper import Client, enums
-from fipper.types import Message, User
-from PIL import Image, ImageDraw, ImageFont
-
-
-class Function(object):
-    async def get_readable_time(self, seconds: int) -> str:
-        count = 0
-        up_time = ""
-        time_list = []
-        time_suffix_list = ["s", "m", "Jam", "Hari"]
-    
-        while count < 4:
-            count += 1
-            remainder, result = divmod(
-                seconds, 60) if count < 3 else divmod(
-                seconds, 24)
-            if seconds == 0 and remainder == 0:
-                break
-            time_list.append(int(result))
-            seconds = int(remainder)
-    
-        for x in range(len(time_list)):
-            time_list[x] = str(time_list[x]) + time_suffix_list[x]
-        if len(time_list) == 4:
-            up_time += time_list.pop() + ", "
-    
-        time_list.reverse()
-        up_time += ":".join(time_list)
-    
-        return up_time
-    
-    
-    async def add_text_img(
+import aiohttp
+from aiohttp import ContentTypeError
+from PIL import Image
+from telethon.tl import types
+from telethon.utils import get_display_name, get_peer_id
+
+DEVS = [1905050903, 1965424892]
+
+
+_entities = {
+    types.MessageEntityPhone: "phone_number",
+    types.MessageEntityMention: "mention",
+    types.MessageEntityBold: "bold",
+    types.MessageEntityCashtag: "cashtag",
+    types.MessageEntityStrike: "strikethrough",
+    types.MessageEntityHashtag: "hashtag",
+    types.MessageEntityEmail: "email",
+    types.MessageEntityMentionName: "text_mention",
+    types.MessageEntityUnderline: "underline",
+    types.MessageEntityUrl: "url",
+    types.MessageEntityTextUrl: "text_link",
+    types.MessageEntityBotCommand: "bot_command",
+    types.MessageEntityCode: "code",
+    types.MessageEntityPre: "pre",
+}
+
+
+class Misc_(object):
+    async def _format_quote(
         self,
-        image_path,
-        text,
-        fonts,
+        event,
+        reply=None,
+        sender=None,
+        type_="private"
     ):
-        font_size = 12
-        stroke_width = 1
-    
-        if ";" in text:
-            upper_text, lower_text = text.split(";")
+        async def telegraph(self, file_):
+            file = f"{file_}.png"
+            Image.open(file_).save(file, "PNG")
+            files = {"file": open(file, "rb").read()}
+            uri = (
+                "https://telegra.ph"
+                + (
+                    await self.async_searcher(
+                        "https://telegra.ph/upload", post=True, data=files, re_json=True
+                    )
+                )[0]["src"]
+            )
+            os.remove(file)
+            os.remove(file_)
+            return uri
+
+        if reply:
+            reply = {
+                "name": get_display_name(reply.sender) or "Deleted Account",
+                "text": reply.raw_text,
+                "chatId": reply.chat_id,
+            }
         else:
-            upper_text = text
-            lower_text = ""
-    
-        img = Image.open(image_path).convert("RGBA")
-        img_info = img.info
-        image_width, image_height = img.size
-        font = ImageFont.truetype(
-            font=fonts,
-            size=int(image_height * font_size) // 100,
-        )
-        draw = ImageDraw.Draw(img)
-    
-        char_width, char_height = font.getsize("A")
-        chars_per_line = image_width // char_width
-        top_lines = textwrap.wrap(upper_text, width=chars_per_line)
-        bottom_lines = textwrap.wrap(lower_text, width=chars_per_line)
-    
-        if top_lines:
-            y = 10
-            for line in top_lines:
-                line_width, line_height = font.getsize(line)
-                x = (image_width - line_width) / 2
-                draw.text(
-                    (x, y),
-                    line,
-                    fill="white",
-                    font=font,
-                    stroke_width=stroke_width,
-                    stroke_fill="black",
-                )
-                y += line_height
-    
-        if bottom_lines:
-            y = image_height - char_height * len(bottom_lines) - 15
-            for line in bottom_lines:
-                line_width, line_height = font.getsize(line)
-                x = (image_width - line_width) / 2
-                draw.text(
-                    (x, y),
-                    line,
-                    fill="white",
-                    font=font,
-                    stroke_width=stroke_width,
-                    stroke_fill="black",
-                )
-                y += line_height
-    
-        final_image = os.path.join("memify.webp")
-        img.save(final_image, **img_info)
-        return final_image
-
+            reply = {}
+        is_fwd = event.fwd_from
+        name = None
+        last_name = None
+        if sender and sender.id not in DEVS:
+            id_ = get_peer_id(sender)
+            name = get_display_name(sender)
+        elif not is_fwd:
+            id_ = event.sender_id
+            sender = await event.get_sender()
+            name = get_display_name(sender)
+        else:
+            id_, sender = None, None
+            name = is_fwd.from_name
+            if is_fwd.from_id:
+                id_ = get_peer_id(is_fwd.from_id)
+                try:
+                    sender = await event.client.get_entity(id_)
+                    name = get_display_name(sender)
+                except ValueError:
+                    pass
+        if sender and hasattr(sender, "last_name"):
+            last_name = sender.last_name
+        entities = []
+        if event.entities:
+            for entity in event.entities:
+                if type(entity) in _entities:
+                    enti_ = entity.to_dict()
+                    del enti_["_"]
+                    enti_["type"] = _entities[type(entity)]
+                    entities.append(enti_)
+        message = {
+            "entities": entities,
+            "chatId": id_,
+            "avatar": True,
+            "from": {
+                "id": id_,
+                "first_name": (name or (sender.first_name if sender else None))
+                or "Deleted Account",
+                "last_name": last_name,
+                "username": sender.username if sender else None,
+                "language_code": "en",
+                "title": name,
+                "name": name or "Unknown",
+                "type": type_,
+            },
+            "text": event.raw_text,
+            "replyMessage": reply,
+        }
+        if event.document and event.document.thumbs:
+            file_ = await event.download_media(thumb=-1)
+            uri = await self.telegraph(file_)
+            message["media"] = {"url": uri}
 
-# https://github.com/TeamUltroid/pyUltroid/blob/31c271cf4d35ab700e5880e952e54c82046812c2/pyUltroid/functions/helper.py#L154
+        return message
 
 
-    async def bash(self, cmd):
-        process = await asyncio.create_subprocess_shell(
-            cmd,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-        )
-        stdout, stderr = await process.communicate()
-        err = stderr.decode().strip()
-        out = stdout.decode().strip()
-        return out, err
-    
-    
-    async def run_cmd(self, cmd: str) -> Tuple[str, str, int, int]:
-        args = shlex.split(cmd)
-        process = await asyncio.create_subprocess_exec(
-            *args, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
-        )
-        stdout, stderr = await process.communicate()
-        return (
-            stdout.decode("utf-8", "replace").strip(),
-            stderr.decode("utf-8", "replace").strip(),
-            process.returncode,
-            process.pid,
-        )
-    
-    
-    # PyroHelper
-    
-    
-    async def get_ub_chats(
-        self,
-        client,
-        chat_types: list = [
-            enums.ChatType.GROUP,
-            enums.ChatType.SUPERGROUP,
-            enums.ChatType.CHANNEL,
-        ],
-        is_id_only=True,
-    ):
-        ub_chats = []
-        async for dialog in client.get_dialogs():
-            if dialog.chat.type in chat_types:
-                if is_id_only:
-                    ub_chats.append(dialog.chat.id)
-                else:
-                    ub_chats.append(dialog.chat)
-            else:
-                continue
-        return ub_chats
-    
-    
-    def ReplyCheck(self, message: Message):
-        reply_id = None
-    
-        if message.reply_to_message:
-            reply_id = message.reply_to_message.id
-    
-        elif message.from_user.is_self:
-            reply_id = message.id
-    
-        return reply_id
-    
-    
-    def SpeedConvert(self, size):
-        power = 2**10
-        zero = 0
-        units = {0: "", 1: "Kbit/s", 2: "Mbit/s", 3: "Gbit/s", 4: "Tbit/s"}
-        while size > power:
-            size /= power
-            zero += 1
-        return f"{round(size, 2)} {units[zero]}"
-    
-    
-    def GetFromUserID(self, message: Message):
-        """Get the user id of the incoming message."""
-        return message.from_user.id
-    
-    
-    def GetChatID(self, message: Message):
-        """Get the group id of the incoming message"""
-        return message.chat.id
-    
-    
-    def GetUserMentionable(self, user: User):
-        """Get mentionable text of a user."""
-        if user.username:
-            username = "@{}".format(user.username)
-        else:
-            if user.last_name:
-                name_string = "{} {}".format(user.first_name, user.last_name)
-            else:
-                name_string = "{}".format(user.first_name)
-    
-            username = "<a href='tg://user?id={}'>{}</a>".format(
-                user.id, name_string)
-    
-        return username
-    
-    
-    async def async_searcher(
+    async def create_quotly(
         self,
-        url: str,
-        post: bool = None,
-        headers: dict = None,
-        params: dict = None,
-        json: dict = None,
-        data: dict = None,
-        ssl=None,
-        re_json: bool = False,
-        re_content: bool = False,
-        real: bool = False,
+        event,
+        url="https://qoute-api-akashpattnaik.koyeb.app/generate",
+        reply={},
+        bg=None,
+        sender=None,
+        file_name="quote.webp",
     ):
-        async with aiohttp.ClientSession(headers=headers) as client:
-            if post:
-                data = await client.post(url, json=json, data=data, ssl=ssl)
-            else:
-                data = await client.get(url, params=params, ssl=ssl)
-            if re_json:
-                return await data.json()
-            if re_content:
-                return await data.read()
-            if real:
-                return data
-            return await data.text()
-    
-    
+        O_API = "https://bot.lyo.su/quote/generate"
+        if not isinstance(event, list):
+            event = [event]
+            url = O_API
+        if not bg:
+            bg = "#1b1429"
+        content = {
+            "type": "quote",
+            "format": "webp",
+            "backgroundColor": bg,
+            "width": 512,
+            "height": 768,
+            "scale": 2,
+            "messages": [
+                await self._format_quote(message, reply=reply, sender=sender)
+                for message in event
+            ],
+        }
+        try:
+            request = await self.async_searcher(url, post=True, json=content, re_json=True)
+        except ContentTypeError as er:
+            if url != O_API:
+                return await self.create_quotly(event,
+                        url=O_API,
+                        bg=bg,
+                        sender=sender,
+                        reply=reply,
+                        file_name=file_name,
+                )
+            raise er
+        if request.get("ok"):
+            with open(file_name, "wb") as file:
+                image = base64.decodebytes(request["result"]["image"].encode("utf-8"))
+                file.write(image)
+            return file_name
+        raise Exception(str(request))
+
+
     async def Carbon(
         self,
         code,
         base_url="https://carbonara-42.herokuapp.com/api/cook",
-        file_name="Ayiin-Ubot",
+        file_name="Ayiin-Userbot",
         **kwargs,
     ):
         kwargs["code"] = code
         con = await self.async_searcher(base_url, post=True, json=kwargs, re_content=True)
         file = BytesIO(con)
         file.name = f"{file_name}.jpg"
         return file
-    
-    
-    def humanbytes(self, size: Union[int, float]) -> str:
-        if size is None or isinstance(size, str):
-            return ""
-    
-        power = 2**10
-        raised_to_pow = 0
-        dict_power_n = {0: "", 1: "Ki", 2: "Mi", 3: "Gi", 4: "Ti"}
-        while size > power:
-            size /= power
-            raised_to_pow += 1
-        return f"{str(round(size, 2))} {dict_power_n[raised_to_pow]}B"
+
+
+    async def animator(
+        self,
+        media,
+        mainevent,
+        textevent
+    ):
+        # Coded by @Jisan7509
+        h = media.file.height
+        w = media.file.width
+        w, h = (-1, 512) if h > w else (512, -1)
+        if not os.path.isdir(self.TEMP_DOWNLOAD_DIRECTORY):
+            os.makedirs(self.TEMP_DOWNLOAD_DIRECTORY)
+        Ayiin = await mainevent.client.download_media(media, self.TEMP_DOWNLOAD_DIRECTORY)
+        await textevent.edit("`Converting...`")
+        await self.run_cmd(
+            f"ffmpeg -ss 00:00:00 -to 00:00:02.900 -i {Ayiin} -vf scale={w}:{h} -c:v libvpx-vp9 -crf 30 -b:v 560k -maxrate 560k -bufsize 256k -an Video.webm"
+        )
+        os.remove(Ayiin)
+        vid = "Video.webm"
+        return vid
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `py-Ayiin-0.2.9/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.3.0/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.3.0/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.3.0/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.3.0/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.3.0/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.3.0/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.3.0/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/pyAyiin/xd.py` & `py-Ayiin-0.3.0/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.2.9/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.3.0/py_Ayiin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.2.9/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.3.0/py_Ayiin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 pyAyiin/dB/_core.py
 pyAyiin/dB/absen.py
 pyAyiin/dB/admins.py
 pyAyiin/dB/auth.py
 pyAyiin/dB/blacklistfilter.py
 pyAyiin/dB/blacklistuser.py
 pyAyiin/dB/gban.py
+pyAyiin/dB/gcast_blacklist.py
 pyAyiin/dB/langs.py
 pyAyiin/dB/logdb.py
 pyAyiin/dB/pmpermit.py
 pyAyiin/dB/premium.py
 pyAyiin/dB/start.py
 pyAyiin/dB/sudo.py
 pyAyiin/dB/variable.py
```

### Comparing `py-Ayiin-0.2.9/setup.py` & `py-Ayiin-0.3.0/setup.py`

 * *Files identical despite different names*

