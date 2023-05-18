# Comparing `tmp/pycelium-0.1.2.tar.gz` & `tmp/pycelium-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycelium-0.1.2.tar", last modified: Thu May 18 06:04:19 2023, max compression
+gzip compressed data, was "pycelium-0.1.3.tar", last modified: Thu May 18 06:19:23 2023, max compression
```

## Comparing `pycelium-0.1.2.tar` & `pycelium-0.1.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/
--rw-rw-r--   0 agp       (1000) agp       (1000)      168 2022-08-06 09:24:18.000000 pycelium-0.1.2/AUTHORS.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     3541 2022-08-06 09:24:18.000000 pycelium-0.1.2/CONTRIBUTING.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       89 2022-08-06 09:24:19.000000 pycelium-0.1.2/HISTORY.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     1510 2022-08-06 09:24:19.000000 pycelium-0.1.2/LICENSE
--rw-rw-r--   0 agp       (1000) agp       (1000)      262 2022-08-06 09:24:19.000000 pycelium-0.1.2/MANIFEST.in
--rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:04:19.927050 pycelium-0.1.2/PKG-INFO
--rw-rw-r--   0 agp       (1000) agp       (1000)      876 2022-08-06 09:24:18.000000 pycelium-0.1.2/README.rst
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.923050 pycelium-0.1.2/docs/
--rw-rw-r--   0 agp       (1000) agp       (1000)      609 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/Makefile
--rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/authors.rst
--rwxrwxr-x   0 agp       (1000) agp       (1000)     4803 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/conf.py
--rw-rw-r--   0 agp       (1000) agp       (1000)       33 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/contributing.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/history.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)      305 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/index.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     1150 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/installation.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)      806 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/make.bat
--rw-rw-r--   0 agp       (1000) agp       (1000)       27 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/readme.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       71 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/usage.rst
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/pycelium/
--rw-rw-r--   0 agp       (1000) agp       (1000)      138 2022-08-06 09:24:19.000000 pycelium-0.1.2/pycelium/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    27746 2023-05-17 04:24:18.000000 pycelium-0.1.2/pycelium/action.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      687 2023-05-13 06:02:42.000000 pycelium-0.1.2/pycelium/agent.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      402 2022-08-06 09:24:19.000000 pycelium-0.1.2/pycelium/cli.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.2/pycelium/containers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     3786 2023-05-17 04:29:20.000000 pycelium-0.1.2/pycelium/definitions.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    17819 2023-05-16 04:07:05.000000 pycelium-0.1.2/pycelium/gathering.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      641 2023-04-30 12:58:35.000000 pycelium-0.1.2/pycelium/grafana.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    21784 2023-05-17 10:58:38.000000 pycelium-0.1.2/pycelium/modem.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     2224 2023-05-15 11:18:29.000000 pycelium-0.1.2/pycelium/network.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     4593 2023-05-05 11:46:38.000000 pycelium-0.1.2/pycelium/packages.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     8408 2023-05-17 03:54:41.000000 pycelium-0.1.2/pycelium/pastor.py
--r-xrwxr-x   0 agp       (1000) agp       (1000)    32037 2023-05-15 04:32:19.000000 pycelium-0.1.2/pycelium/pawn.py
--rw-rw-r--   0 agp       (1000) agp       (1000)       19 2022-08-06 09:24:19.000000 pycelium-0.1.2/pycelium/pycelium.py
--rwxrwxr-x   0 agp       (1000) agp       (1000)    50518 2023-05-15 14:44:47.000000 pycelium-0.1.2/pycelium/scanner.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    51226 2023-05-17 04:19:30.000000 pycelium-0.1.2/pycelium/service.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    52755 2023-05-17 04:18:41.000000 pycelium-0.1.2/pycelium/shell.py
--rw-rw-r--   0 agp       (1000) agp       (1000)        0 2023-05-04 05:10:26.000000 pycelium-0.1.2/pycelium/ssh.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/pycelium/tools/
--rw-rw-r--   0 agp       (1000) agp       (1000)    40887 2023-04-27 11:46:47.000000 pycelium-0.1.2/pycelium/tools/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    10670 2023-04-21 04:23:40.000000 pycelium-0.1.2/pycelium/tools/calls.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     1500 2022-04-04 14:07:37.000000 pycelium-0.1.2/pycelium/tools/colors.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    22598 2022-05-07 15:33:49.000000 pycelium-0.1.2/pycelium/tools/configurations.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.2/pycelium/tools/containers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     5199 2023-04-28 10:31:35.000000 pycelium-0.1.2/pycelium/tools/helpers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    15780 2022-12-30 19:34:03.000000 pycelium-0.1.2/pycelium/tools/logs.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     6092 2023-05-02 11:20:30.000000 pycelium-0.1.2/pycelium/tools/metrics.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     1786 2023-05-07 06:20:55.000000 pycelium-0.1.2/pycelium/tools/mixer.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     5734 2023-05-07 06:32:41.000000 pycelium-0.1.2/pycelium/tools/persistence.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     2520 2023-05-13 06:35:01.000000 pycelium-0.1.2/pycelium/tools/templating.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     3641 2023-05-17 04:16:27.000000 pycelium-0.1.2/pycelium/watch.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    14729 2023-03-28 18:29:00.000000 pycelium-0.1.2/pycelium/wingdbstub.old.py
--rw-r--r--   0 agp       (1000) agp       (1000)    14020 2023-03-28 18:27:21.000000 pycelium-0.1.2/pycelium/wingdbstub.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     9127 2023-05-18 05:53:27.000000 pycelium-0.1.2/pycelium/wireguard.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/pycelium.egg-info/
--rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/PKG-INFO
--rw-rw-r--   0 agp       (1000) agp       (1000)     1279 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/SOURCES.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        1 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/dependency_links.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)       47 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/entry_points.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.000000 pycelium-0.1.2/pycelium.egg-info/not-zip-safe
--rw-rw-r--   0 agp       (1000) agp       (1000)       11 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/requires.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        9 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/top_level.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)      425 2023-05-18 06:04:19.927050 pycelium-0.1.2/setup.cfg
--rw-rw-r--   0 agp       (1000) agp       (1000)     1407 2023-05-18 06:02:40.000000 pycelium-0.1.2/setup.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/tests/
--rw-rw-r--   0 agp       (1000) agp       (1000)       38 2022-08-06 09:24:19.000000 pycelium-0.1.2/tests/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      544 2023-04-16 20:55:03.000000 pycelium-0.1.2/tests/test_init.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      984 2022-08-06 09:24:19.000000 pycelium-0.1.2/tests/test_pycelium.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:19:23.190192 pycelium-0.1.3/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      168 2022-08-06 09:24:18.000000 pycelium-0.1.3/AUTHORS.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3541 2022-08-06 09:24:18.000000 pycelium-0.1.3/CONTRIBUTING.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       89 2022-08-06 09:24:19.000000 pycelium-0.1.3/HISTORY.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1510 2022-08-06 09:24:19.000000 pycelium-0.1.3/LICENSE
+-rw-rw-r--   0 agp       (1000) agp       (1000)      262 2022-08-06 09:24:19.000000 pycelium-0.1.3/MANIFEST.in
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:19:23.190192 pycelium-0.1.3/PKG-INFO
+-rw-rw-r--   0 agp       (1000) agp       (1000)      876 2022-08-06 09:24:18.000000 pycelium-0.1.3/README.rst
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:19:23.186192 pycelium-0.1.3/docs/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      609 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/Makefile
+-rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/authors.rst
+-rwxrwxr-x   0 agp       (1000) agp       (1000)     4803 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/conf.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)       33 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/contributing.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/history.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)      305 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/index.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1150 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/installation.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)      806 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/make.bat
+-rw-rw-r--   0 agp       (1000) agp       (1000)       27 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/readme.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       71 2022-08-06 09:24:19.000000 pycelium-0.1.3/docs/usage.rst
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:19:23.190192 pycelium-0.1.3/pycelium/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      138 2023-05-18 06:17:42.000000 pycelium-0.1.3/pycelium/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    27746 2023-05-17 04:24:18.000000 pycelium-0.1.3/pycelium/action.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      687 2023-05-13 06:02:42.000000 pycelium-0.1.3/pycelium/agent.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      402 2022-08-06 09:24:19.000000 pycelium-0.1.3/pycelium/cli.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.3/pycelium/containers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3786 2023-05-17 04:29:20.000000 pycelium-0.1.3/pycelium/definitions.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    17819 2023-05-16 04:07:05.000000 pycelium-0.1.3/pycelium/gathering.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      641 2023-04-30 12:58:35.000000 pycelium-0.1.3/pycelium/grafana.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    21784 2023-05-17 10:58:38.000000 pycelium-0.1.3/pycelium/modem.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2224 2023-05-15 11:18:29.000000 pycelium-0.1.3/pycelium/network.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     4593 2023-05-05 11:46:38.000000 pycelium-0.1.3/pycelium/packages.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     8408 2023-05-17 03:54:41.000000 pycelium-0.1.3/pycelium/pastor.py
+-r-xrwxr-x   0 agp       (1000) agp       (1000)    32037 2023-05-15 04:32:19.000000 pycelium-0.1.3/pycelium/pawn.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)       19 2022-08-06 09:24:19.000000 pycelium-0.1.3/pycelium/pycelium.py
+-rwxrwxr-x   0 agp       (1000) agp       (1000)    50518 2023-05-15 14:44:47.000000 pycelium-0.1.3/pycelium/scanner.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    51226 2023-05-17 04:19:30.000000 pycelium-0.1.3/pycelium/service.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    52755 2023-05-17 04:18:41.000000 pycelium-0.1.3/pycelium/shell.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)        0 2023-05-04 05:10:26.000000 pycelium-0.1.3/pycelium/ssh.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:19:23.190192 pycelium-0.1.3/pycelium/tools/
+-rw-rw-r--   0 agp       (1000) agp       (1000)    40887 2023-04-27 11:46:47.000000 pycelium-0.1.3/pycelium/tools/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    10670 2023-04-21 04:23:40.000000 pycelium-0.1.3/pycelium/tools/calls.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1500 2022-04-04 14:07:37.000000 pycelium-0.1.3/pycelium/tools/colors.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    22598 2022-05-07 15:33:49.000000 pycelium-0.1.3/pycelium/tools/configurations.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.3/pycelium/tools/containers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5199 2023-04-28 10:31:35.000000 pycelium-0.1.3/pycelium/tools/helpers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    15780 2022-12-30 19:34:03.000000 pycelium-0.1.3/pycelium/tools/logs.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     6092 2023-05-02 11:20:30.000000 pycelium-0.1.3/pycelium/tools/metrics.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1786 2023-05-07 06:20:55.000000 pycelium-0.1.3/pycelium/tools/mixer.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5734 2023-05-07 06:32:41.000000 pycelium-0.1.3/pycelium/tools/persistence.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2520 2023-05-13 06:35:01.000000 pycelium-0.1.3/pycelium/tools/templating.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3641 2023-05-17 04:16:27.000000 pycelium-0.1.3/pycelium/watch.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    14729 2023-03-28 18:29:00.000000 pycelium-0.1.3/pycelium/wingdbstub.old.py
+-rw-r--r--   0 agp       (1000) agp       (1000)    14020 2023-03-28 18:27:21.000000 pycelium-0.1.3/pycelium/wingdbstub.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     9127 2023-05-18 05:53:27.000000 pycelium-0.1.3/pycelium/wireguard.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:19:23.190192 pycelium-0.1.3/pycelium.egg-info/
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:19:23.000000 pycelium-0.1.3/pycelium.egg-info/PKG-INFO
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1279 2023-05-18 06:19:23.000000 pycelium-0.1.3/pycelium.egg-info/SOURCES.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        1 2023-05-18 06:19:23.000000 pycelium-0.1.3/pycelium.egg-info/dependency_links.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)       47 2023-05-18 06:19:23.000000 pycelium-0.1.3/pycelium.egg-info/entry_points.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.000000 pycelium-0.1.3/pycelium.egg-info/not-zip-safe
+-rw-rw-r--   0 agp       (1000) agp       (1000)       41 2023-05-18 06:19:23.000000 pycelium-0.1.3/pycelium.egg-info/requires.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        9 2023-05-18 06:19:23.000000 pycelium-0.1.3/pycelium.egg-info/top_level.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)      425 2023-05-18 06:19:23.190192 pycelium-0.1.3/setup.cfg
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1473 2023-05-18 06:19:14.000000 pycelium-0.1.3/setup.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:19:23.190192 pycelium-0.1.3/tests/
+-rw-rw-r--   0 agp       (1000) agp       (1000)       38 2022-08-06 09:24:19.000000 pycelium-0.1.3/tests/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      544 2023-04-16 20:55:03.000000 pycelium-0.1.3/tests/test_init.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      984 2022-08-06 09:24:19.000000 pycelium-0.1.3/tests/test_pycelium.py
```

### Comparing `pycelium-0.1.2/CONTRIBUTING.rst` & `pycelium-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/LICENSE` & `pycelium-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/PKG-INFO` & `pycelium-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycelium
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Mycelium Edge Swarm Network
 Home-page: https://github.com/asteriogonzalez/pycelium
 Author: Asterio Gonzalez
 Author-email: asterio.gonzalez@gmail.com
 License: BSD license
 Keywords: pycelium
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pycelium-0.1.2/README.rst` & `pycelium-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/docs/Makefile` & `pycelium-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/docs/conf.py` & `pycelium-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/docs/installation.rst` & `pycelium-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/docs/make.bat` & `pycelium-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/action.py` & `pycelium-0.1.3/pycelium/action.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/agent.py` & `pycelium-0.1.3/pycelium/agent.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/containers.py` & `pycelium-0.1.3/pycelium/containers.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/definitions.py` & `pycelium-0.1.3/pycelium/definitions.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/gathering.py` & `pycelium-0.1.3/pycelium/gathering.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/grafana.py` & `pycelium-0.1.3/pycelium/grafana.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/modem.py` & `pycelium-0.1.3/pycelium/modem.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/network.py` & `pycelium-0.1.3/pycelium/network.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/packages.py` & `pycelium-0.1.3/pycelium/packages.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/pastor.py` & `pycelium-0.1.3/pycelium/pastor.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/pawn.py` & `pycelium-0.1.3/pycelium/pawn.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/scanner.py` & `pycelium-0.1.3/pycelium/scanner.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/service.py` & `pycelium-0.1.3/pycelium/service.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/shell.py` & `pycelium-0.1.3/pycelium/shell.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/__init__.py` & `pycelium-0.1.3/pycelium/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/calls.py` & `pycelium-0.1.3/pycelium/tools/calls.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/colors.py` & `pycelium-0.1.3/pycelium/tools/colors.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/configurations.py` & `pycelium-0.1.3/pycelium/tools/configurations.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/containers.py` & `pycelium-0.1.3/pycelium/tools/containers.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/helpers.py` & `pycelium-0.1.3/pycelium/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/logs.py` & `pycelium-0.1.3/pycelium/tools/logs.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/metrics.py` & `pycelium-0.1.3/pycelium/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/mixer.py` & `pycelium-0.1.3/pycelium/tools/mixer.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/persistence.py` & `pycelium-0.1.3/pycelium/tools/persistence.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/tools/templating.py` & `pycelium-0.1.3/pycelium/tools/templating.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/watch.py` & `pycelium-0.1.3/pycelium/watch.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/wingdbstub.old.py` & `pycelium-0.1.3/pycelium/wingdbstub.old.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/wingdbstub.py` & `pycelium-0.1.3/pycelium/wingdbstub.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium/wireguard.py` & `pycelium-0.1.3/pycelium/wireguard.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/pycelium.egg-info/PKG-INFO` & `pycelium-0.1.3/pycelium.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycelium
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Mycelium Edge Swarm Network
 Home-page: https://github.com/asteriogonzalez/pycelium
 Author: Asterio Gonzalez
 Author-email: asterio.gonzalez@gmail.com
 License: BSD license
 Keywords: pycelium
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pycelium-0.1.2/pycelium.egg-info/SOURCES.txt` & `pycelium-0.1.3/pycelium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/setup.py` & `pycelium-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,20 @@
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
     'Click>=7.0',
+    'python-dateutil',
+    'glom',
+    'jmespath',
 ]
 
-test_requirements = [
+test_requirements = requirements + [
     'pytest>=3',
 ]
 
 setup(
     author="Asterio Gonzalez",
     author_email='asterio.gonzalez@gmail.com',
     python_requires='>=3.9',
@@ -44,10 +47,10 @@
     include_package_data=True,
     keywords='pycelium',
     name='pycelium',
     packages=find_packages(include=['pycelium', 'pycelium.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/asteriogonzalez/pycelium',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `pycelium-0.1.2/tests/test_init.py` & `pycelium-0.1.3/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pycelium-0.1.2/tests/test_pycelium.py` & `pycelium-0.1.3/tests/test_pycelium.py`

 * *Files identical despite different names*

