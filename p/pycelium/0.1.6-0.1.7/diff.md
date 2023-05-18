# Comparing `tmp/pycelium-0.1.6.tar.gz` & `tmp/pycelium-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycelium-0.1.6.tar", last modified: Thu May 18 06:44:36 2023, max compression
+gzip compressed data, was "pycelium-0.1.7.tar", last modified: Thu May 18 06:51:22 2023, max compression
```

## Comparing `pycelium-0.1.6.tar` & `pycelium-0.1.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:44:36.381963 pycelium-0.1.6/
--rw-rw-r--   0 agp       (1000) agp       (1000)      168 2022-08-06 09:24:18.000000 pycelium-0.1.6/AUTHORS.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     3541 2022-08-06 09:24:18.000000 pycelium-0.1.6/CONTRIBUTING.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       89 2022-08-06 09:24:19.000000 pycelium-0.1.6/HISTORY.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     1510 2022-08-06 09:24:19.000000 pycelium-0.1.6/LICENSE
--rw-rw-r--   0 agp       (1000) agp       (1000)      262 2022-08-06 09:24:19.000000 pycelium-0.1.6/MANIFEST.in
--rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:44:36.381963 pycelium-0.1.6/PKG-INFO
--rw-rw-r--   0 agp       (1000) agp       (1000)      876 2022-08-06 09:24:18.000000 pycelium-0.1.6/README.rst
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:44:36.377963 pycelium-0.1.6/docs/
--rw-rw-r--   0 agp       (1000) agp       (1000)      609 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/Makefile
--rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/authors.rst
--rwxrwxr-x   0 agp       (1000) agp       (1000)     4803 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/conf.py
--rw-rw-r--   0 agp       (1000) agp       (1000)       33 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/contributing.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/history.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)      305 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/index.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     1150 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/installation.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)      806 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/make.bat
--rw-rw-r--   0 agp       (1000) agp       (1000)       27 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/readme.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       71 2022-08-06 09:24:19.000000 pycelium-0.1.6/docs/usage.rst
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:44:36.381963 pycelium-0.1.6/pycelium/
--rw-rw-r--   0 agp       (1000) agp       (1000)      138 2023-05-18 06:17:42.000000 pycelium-0.1.6/pycelium/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    27746 2023-05-17 04:24:18.000000 pycelium-0.1.6/pycelium/action.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      687 2023-05-13 06:02:42.000000 pycelium-0.1.6/pycelium/agent.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      402 2022-08-06 09:24:19.000000 pycelium-0.1.6/pycelium/cli.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.6/pycelium/containers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     3786 2023-05-17 04:29:20.000000 pycelium-0.1.6/pycelium/definitions.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    17819 2023-05-16 04:07:05.000000 pycelium-0.1.6/pycelium/gathering.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      641 2023-04-30 12:58:35.000000 pycelium-0.1.6/pycelium/grafana.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    21784 2023-05-17 10:58:38.000000 pycelium-0.1.6/pycelium/modem.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     2224 2023-05-15 11:18:29.000000 pycelium-0.1.6/pycelium/network.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     4593 2023-05-05 11:46:38.000000 pycelium-0.1.6/pycelium/packages.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     8408 2023-05-17 03:54:41.000000 pycelium-0.1.6/pycelium/pastor.py
--r-xrwxr-x   0 agp       (1000) agp       (1000)    32037 2023-05-15 04:32:19.000000 pycelium-0.1.6/pycelium/pawn.py
--rw-rw-r--   0 agp       (1000) agp       (1000)       19 2022-08-06 09:24:19.000000 pycelium-0.1.6/pycelium/pycelium.py
--rwxrwxr-x   0 agp       (1000) agp       (1000)    50518 2023-05-15 14:44:47.000000 pycelium-0.1.6/pycelium/scanner.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    51220 2023-05-18 06:29:00.000000 pycelium-0.1.6/pycelium/service.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    52755 2023-05-17 04:18:41.000000 pycelium-0.1.6/pycelium/shell.py
--rw-rw-r--   0 agp       (1000) agp       (1000)        0 2023-05-04 05:10:26.000000 pycelium-0.1.6/pycelium/ssh.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:44:36.381963 pycelium-0.1.6/pycelium/tools/
--rw-rw-r--   0 agp       (1000) agp       (1000)    40887 2023-04-27 11:46:47.000000 pycelium-0.1.6/pycelium/tools/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    10670 2023-04-21 04:23:40.000000 pycelium-0.1.6/pycelium/tools/calls.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:44:36.381963 pycelium-0.1.6/pycelium/tools/cli/
--rw-rw-r--   0 agp       (1000) agp       (1000)        0 2023-05-18 06:42:31.000000 pycelium-0.1.6/pycelium/tools/cli/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     5635 2023-04-28 16:38:57.000000 pycelium-0.1.6/pycelium/tools/cli/config.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      236 2023-04-27 19:31:20.000000 pycelium-0.1.6/pycelium/tools/cli/get.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     1549 2023-04-28 04:29:29.000000 pycelium-0.1.6/pycelium/tools/cli/main.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     2250 2023-04-27 09:51:56.000000 pycelium-0.1.6/pycelium/tools/cli/run.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     1500 2022-04-04 14:07:37.000000 pycelium-0.1.6/pycelium/tools/colors.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    22598 2022-05-07 15:33:49.000000 pycelium-0.1.6/pycelium/tools/configurations.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.6/pycelium/tools/containers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     5199 2023-04-28 10:31:35.000000 pycelium-0.1.6/pycelium/tools/helpers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    15780 2022-12-30 19:34:03.000000 pycelium-0.1.6/pycelium/tools/logs.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     6092 2023-05-02 11:20:30.000000 pycelium-0.1.6/pycelium/tools/metrics.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     1786 2023-05-07 06:20:55.000000 pycelium-0.1.6/pycelium/tools/mixer.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     5734 2023-05-07 06:32:41.000000 pycelium-0.1.6/pycelium/tools/persistence.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     2520 2023-05-13 06:35:01.000000 pycelium-0.1.6/pycelium/tools/templating.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     3641 2023-05-17 04:16:27.000000 pycelium-0.1.6/pycelium/watch.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    14729 2023-03-28 18:29:00.000000 pycelium-0.1.6/pycelium/wingdbstub.old.py
--rw-r--r--   0 agp       (1000) agp       (1000)    14020 2023-03-28 18:27:21.000000 pycelium-0.1.6/pycelium/wingdbstub.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     9127 2023-05-18 05:53:27.000000 pycelium-0.1.6/pycelium/wireguard.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:44:36.381963 pycelium-0.1.6/pycelium.egg-info/
--rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:44:36.000000 pycelium-0.1.6/pycelium.egg-info/PKG-INFO
--rw-rw-r--   0 agp       (1000) agp       (1000)     1418 2023-05-18 06:44:36.000000 pycelium-0.1.6/pycelium.egg-info/SOURCES.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        1 2023-05-18 06:44:36.000000 pycelium-0.1.6/pycelium.egg-info/dependency_links.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)       47 2023-05-18 06:44:36.000000 pycelium-0.1.6/pycelium.egg-info/entry_points.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.000000 pycelium-0.1.6/pycelium.egg-info/not-zip-safe
--rw-rw-r--   0 agp       (1000) agp       (1000)      277 2023-05-18 06:44:36.000000 pycelium-0.1.6/pycelium.egg-info/requires.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        9 2023-05-18 06:44:36.000000 pycelium-0.1.6/pycelium.egg-info/top_level.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)      425 2023-05-18 06:44:36.385963 pycelium-0.1.6/setup.cfg
--rw-rw-r--   0 agp       (1000) agp       (1000)     1752 2023-05-18 06:44:29.000000 pycelium-0.1.6/setup.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:44:36.381963 pycelium-0.1.6/tests/
--rw-rw-r--   0 agp       (1000) agp       (1000)       38 2022-08-06 09:24:19.000000 pycelium-0.1.6/tests/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      544 2023-04-16 20:55:03.000000 pycelium-0.1.6/tests/test_init.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      984 2022-08-06 09:24:19.000000 pycelium-0.1.6/tests/test_pycelium.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:51:22.032978 pycelium-0.1.7/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      168 2022-08-06 09:24:18.000000 pycelium-0.1.7/AUTHORS.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3541 2022-08-06 09:24:18.000000 pycelium-0.1.7/CONTRIBUTING.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       89 2022-08-06 09:24:19.000000 pycelium-0.1.7/HISTORY.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1510 2022-08-06 09:24:19.000000 pycelium-0.1.7/LICENSE
+-rw-rw-r--   0 agp       (1000) agp       (1000)      262 2022-08-06 09:24:19.000000 pycelium-0.1.7/MANIFEST.in
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:51:22.032978 pycelium-0.1.7/PKG-INFO
+-rw-rw-r--   0 agp       (1000) agp       (1000)      876 2022-08-06 09:24:18.000000 pycelium-0.1.7/README.rst
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:51:22.028979 pycelium-0.1.7/docs/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      609 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/Makefile
+-rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/authors.rst
+-rwxrwxr-x   0 agp       (1000) agp       (1000)     4803 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/conf.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)       33 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/contributing.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/history.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)      305 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/index.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1150 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/installation.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)      806 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/make.bat
+-rw-rw-r--   0 agp       (1000) agp       (1000)       27 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/readme.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       71 2022-08-06 09:24:19.000000 pycelium-0.1.7/docs/usage.rst
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:51:22.028979 pycelium-0.1.7/pycelium/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      138 2023-05-18 06:50:45.000000 pycelium-0.1.7/pycelium/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    27746 2023-05-17 04:24:18.000000 pycelium-0.1.7/pycelium/action.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      687 2023-05-13 06:02:42.000000 pycelium-0.1.7/pycelium/agent.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      402 2022-08-06 09:24:19.000000 pycelium-0.1.7/pycelium/cli.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.7/pycelium/containers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3786 2023-05-17 04:29:20.000000 pycelium-0.1.7/pycelium/definitions.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    17819 2023-05-16 04:07:05.000000 pycelium-0.1.7/pycelium/gathering.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      641 2023-04-30 12:58:35.000000 pycelium-0.1.7/pycelium/grafana.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    21784 2023-05-17 10:58:38.000000 pycelium-0.1.7/pycelium/modem.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2224 2023-05-15 11:18:29.000000 pycelium-0.1.7/pycelium/network.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     4593 2023-05-05 11:46:38.000000 pycelium-0.1.7/pycelium/packages.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     8408 2023-05-17 03:54:41.000000 pycelium-0.1.7/pycelium/pastor.py
+-r-xrwxr-x   0 agp       (1000) agp       (1000)    32037 2023-05-15 04:32:19.000000 pycelium-0.1.7/pycelium/pawn.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)       19 2022-08-06 09:24:19.000000 pycelium-0.1.7/pycelium/pycelium.py
+-rwxrwxr-x   0 agp       (1000) agp       (1000)    50518 2023-05-15 14:44:47.000000 pycelium-0.1.7/pycelium/scanner.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    51220 2023-05-18 06:29:00.000000 pycelium-0.1.7/pycelium/service.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    52755 2023-05-17 04:18:41.000000 pycelium-0.1.7/pycelium/shell.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)        0 2023-05-04 05:10:26.000000 pycelium-0.1.7/pycelium/ssh.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:51:22.032978 pycelium-0.1.7/pycelium/tools/
+-rw-rw-r--   0 agp       (1000) agp       (1000)    40887 2023-04-27 11:46:47.000000 pycelium-0.1.7/pycelium/tools/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    10670 2023-04-21 04:23:40.000000 pycelium-0.1.7/pycelium/tools/calls.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:51:22.032978 pycelium-0.1.7/pycelium/tools/cli/
+-rw-rw-r--   0 agp       (1000) agp       (1000)       31 2023-05-18 06:45:56.000000 pycelium-0.1.7/pycelium/tools/cli/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5635 2023-04-28 16:38:57.000000 pycelium-0.1.7/pycelium/tools/cli/config.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      236 2023-04-27 19:31:20.000000 pycelium-0.1.7/pycelium/tools/cli/get.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1549 2023-04-28 04:29:29.000000 pycelium-0.1.7/pycelium/tools/cli/main.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2250 2023-04-27 09:51:56.000000 pycelium-0.1.7/pycelium/tools/cli/run.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1500 2022-04-04 14:07:37.000000 pycelium-0.1.7/pycelium/tools/colors.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    22598 2022-05-07 15:33:49.000000 pycelium-0.1.7/pycelium/tools/configurations.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.7/pycelium/tools/containers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5199 2023-04-28 10:31:35.000000 pycelium-0.1.7/pycelium/tools/helpers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    15780 2022-12-30 19:34:03.000000 pycelium-0.1.7/pycelium/tools/logs.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     6092 2023-05-02 11:20:30.000000 pycelium-0.1.7/pycelium/tools/metrics.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1786 2023-05-07 06:20:55.000000 pycelium-0.1.7/pycelium/tools/mixer.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5734 2023-05-07 06:32:41.000000 pycelium-0.1.7/pycelium/tools/persistence.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2520 2023-05-13 06:35:01.000000 pycelium-0.1.7/pycelium/tools/templating.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3641 2023-05-17 04:16:27.000000 pycelium-0.1.7/pycelium/watch.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    14729 2023-03-28 18:29:00.000000 pycelium-0.1.7/pycelium/wingdbstub.old.py
+-rw-r--r--   0 agp       (1000) agp       (1000)    14020 2023-03-28 18:27:21.000000 pycelium-0.1.7/pycelium/wingdbstub.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     9127 2023-05-18 05:53:27.000000 pycelium-0.1.7/pycelium/wireguard.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:51:22.028979 pycelium-0.1.7/pycelium.egg-info/
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:51:21.000000 pycelium-0.1.7/pycelium.egg-info/PKG-INFO
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1418 2023-05-18 06:51:22.000000 pycelium-0.1.7/pycelium.egg-info/SOURCES.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        1 2023-05-18 06:51:21.000000 pycelium-0.1.7/pycelium.egg-info/dependency_links.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)       47 2023-05-18 06:51:21.000000 pycelium-0.1.7/pycelium.egg-info/entry_points.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.000000 pycelium-0.1.7/pycelium.egg-info/not-zip-safe
+-rw-rw-r--   0 agp       (1000) agp       (1000)      277 2023-05-18 06:51:21.000000 pycelium-0.1.7/pycelium.egg-info/requires.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        9 2023-05-18 06:51:21.000000 pycelium-0.1.7/pycelium.egg-info/top_level.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)      425 2023-05-18 06:51:22.032978 pycelium-0.1.7/setup.cfg
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1752 2023-05-18 06:50:45.000000 pycelium-0.1.7/setup.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:51:22.032978 pycelium-0.1.7/tests/
+-rw-rw-r--   0 agp       (1000) agp       (1000)       38 2022-08-06 09:24:19.000000 pycelium-0.1.7/tests/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      544 2023-04-16 20:55:03.000000 pycelium-0.1.7/tests/test_init.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      984 2022-08-06 09:24:19.000000 pycelium-0.1.7/tests/test_pycelium.py
```

### Comparing `pycelium-0.1.6/CONTRIBUTING.rst` & `pycelium-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/LICENSE` & `pycelium-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/PKG-INFO` & `pycelium-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycelium
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python Mycelium Edge Swarm Network
 Home-page: https://github.com/asteriogonzalez/pycelium
 Author: Asterio Gonzalez
 Author-email: asterio.gonzalez@gmail.com
 License: BSD license
 Keywords: pycelium
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pycelium-0.1.6/README.rst` & `pycelium-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/docs/Makefile` & `pycelium-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/docs/conf.py` & `pycelium-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/docs/installation.rst` & `pycelium-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/docs/make.bat` & `pycelium-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/action.py` & `pycelium-0.1.7/pycelium/action.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/agent.py` & `pycelium-0.1.7/pycelium/agent.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/containers.py` & `pycelium-0.1.7/pycelium/containers.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/definitions.py` & `pycelium-0.1.7/pycelium/definitions.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/gathering.py` & `pycelium-0.1.7/pycelium/gathering.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/grafana.py` & `pycelium-0.1.7/pycelium/grafana.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/modem.py` & `pycelium-0.1.7/pycelium/modem.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/network.py` & `pycelium-0.1.7/pycelium/network.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/packages.py` & `pycelium-0.1.7/pycelium/packages.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/pastor.py` & `pycelium-0.1.7/pycelium/pastor.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/pawn.py` & `pycelium-0.1.7/pycelium/pawn.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/scanner.py` & `pycelium-0.1.7/pycelium/scanner.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/service.py` & `pycelium-0.1.7/pycelium/service.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/shell.py` & `pycelium-0.1.7/pycelium/shell.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/__init__.py` & `pycelium-0.1.7/pycelium/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/calls.py` & `pycelium-0.1.7/pycelium/tools/calls.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/cli/config.py` & `pycelium-0.1.7/pycelium/tools/cli/config.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/cli/main.py` & `pycelium-0.1.7/pycelium/tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/cli/run.py` & `pycelium-0.1.7/pycelium/tools/cli/run.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/colors.py` & `pycelium-0.1.7/pycelium/tools/colors.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/configurations.py` & `pycelium-0.1.7/pycelium/tools/configurations.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/containers.py` & `pycelium-0.1.7/pycelium/tools/containers.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/helpers.py` & `pycelium-0.1.7/pycelium/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/logs.py` & `pycelium-0.1.7/pycelium/tools/logs.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/metrics.py` & `pycelium-0.1.7/pycelium/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/mixer.py` & `pycelium-0.1.7/pycelium/tools/mixer.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/persistence.py` & `pycelium-0.1.7/pycelium/tools/persistence.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/tools/templating.py` & `pycelium-0.1.7/pycelium/tools/templating.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/watch.py` & `pycelium-0.1.7/pycelium/watch.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/wingdbstub.old.py` & `pycelium-0.1.7/pycelium/wingdbstub.old.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/wingdbstub.py` & `pycelium-0.1.7/pycelium/wingdbstub.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium/wireguard.py` & `pycelium-0.1.7/pycelium/wireguard.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/pycelium.egg-info/PKG-INFO` & `pycelium-0.1.7/pycelium.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycelium
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python Mycelium Edge Swarm Network
 Home-page: https://github.com/asteriogonzalez/pycelium
 Author: Asterio Gonzalez
 Author-email: asterio.gonzalez@gmail.com
 License: BSD license
 Keywords: pycelium
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pycelium-0.1.6/pycelium.egg-info/SOURCES.txt` & `pycelium-0.1.7/pycelium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/setup.py` & `pycelium-0.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,10 +61,10 @@
     include_package_data=True,
     keywords='pycelium',
     name='pycelium',
     packages=find_packages(include=['pycelium', 'pycelium.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/asteriogonzalez/pycelium',
-    version='0.1.6',
+    version='0.1.7',
     zip_safe=False,
 )
```

### Comparing `pycelium-0.1.6/tests/test_init.py` & `pycelium-0.1.7/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.6/tests/test_pycelium.py` & `pycelium-0.1.7/tests/test_pycelium.py`

 * *Files identical despite different names*

