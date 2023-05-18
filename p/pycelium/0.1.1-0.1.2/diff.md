# Comparing `tmp/pycelium-0.1.1.linux-x86_64.tar.gz` & `tmp/pycelium-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycelium-0.1.1.linux-x86_64.tar", last modified: Thu May 18 05:54:40 2023, max compression
+gzip compressed data, was "pycelium-0.1.2.tar", last modified: Thu May 18 06:04:19 2023, max compression
```

## Comparing `pycelium-0.1.1.linux-x86_64.tar` & `pycelium-0.1.2.tar`

### file list

```diff
@@ -1,86 +1,68 @@
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.615617 ./
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.615617 ./usr/
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.747617 ./usr/local/
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.747617 ./usr/local/bin/
--rwxrwxr-x   0 agp       (1000) agp       (1000)      963 2023-05-18 05:54:40.747617 ./usr/local/bin/pycelium
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.615617 ./usr/local/lib/
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.615617 ./usr/local/lib/python3.10/
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.687617 ./usr/local/lib/python3.10/dist-packages/
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/
--rw-rw-r--   0 agp       (1000) agp       (1000)      138 2022-08-06 09:24:19.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/__init__.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.679617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/
--rw-rw-r--   0 agp       (1000) agp       (1000)      303 2023-05-18 05:54:40.671617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    17883 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/action.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     1217 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/agent.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)      577 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    47875 2023-05-18 05:54:40.663617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/containers.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     2270 2023-05-18 05:54:40.663617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/definitions.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    14662 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/gathering.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)      766 2023-05-18 05:54:40.671617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/grafana.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    17100 2023-05-18 05:54:40.679617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/modem.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     2338 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/network.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     4224 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/packages.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     4822 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/pastor.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    21293 2023-05-18 05:54:40.679617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/pawn.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)      177 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/pycelium.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    34149 2023-05-18 05:54:40.643617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/scanner.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    38422 2023-05-18 05:54:40.651617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/service.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    40112 2023-05-18 05:54:40.671617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/shell.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)      148 2023-05-18 05:54:40.671617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/ssh.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     3179 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/watch.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     6213 2023-05-18 05:54:40.651617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/wingdbstub.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     6499 2023-05-18 05:54:40.647617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/wingdbstub.old.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     6981 2023-05-18 05:54:40.647617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/wireguard.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    27746 2023-05-17 04:24:18.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/action.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      687 2023-05-13 06:02:42.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/agent.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      402 2022-08-06 09:24:19.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/cli.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/containers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     3786 2023-05-17 04:29:20.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/definitions.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    17819 2023-05-16 04:07:05.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/gathering.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      641 2023-04-30 12:58:35.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/grafana.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    21784 2023-05-17 10:58:38.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/modem.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     2224 2023-05-15 11:18:29.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/network.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     4593 2023-05-05 11:46:38.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/packages.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     8408 2023-05-17 03:54:41.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/pastor.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    32037 2023-05-15 04:32:19.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/pawn.py
--rw-rw-r--   0 agp       (1000) agp       (1000)       19 2022-08-06 09:24:19.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/pycelium.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    50518 2023-05-15 14:44:47.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/scanner.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    51226 2023-05-17 04:19:30.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/service.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    52755 2023-05-17 04:18:41.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/shell.py
--rw-rw-r--   0 agp       (1000) agp       (1000)        0 2023-05-04 05:10:26.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/ssh.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.619617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/
--rw-rw-r--   0 agp       (1000) agp       (1000)    40887 2023-04-27 11:46:47.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__init__.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/
--rw-rw-r--   0 agp       (1000) agp       (1000)    33973 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     7172 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/calls.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     1433 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/colors.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    18006 2023-05-18 05:54:40.635617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/configurations.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    47881 2023-05-18 05:54:40.631617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/containers.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     4861 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/helpers.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    13364 2023-05-18 05:54:40.619617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/logs.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     5187 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/metrics.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     1974 2023-05-18 05:54:40.631617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/mixer.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     4277 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/persistence.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)     2076 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/templating.cpython-310.pyc
--rw-rw-r--   0 agp       (1000) agp       (1000)    10670 2023-04-21 04:23:40.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/calls.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     1500 2022-04-04 14:07:37.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/colors.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    22598 2022-05-07 15:33:49.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/configurations.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/containers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     5199 2023-04-28 10:31:35.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/helpers.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    15780 2022-12-30 19:34:03.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/logs.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     6092 2023-05-02 11:20:30.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/metrics.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     1786 2023-05-07 06:20:55.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/mixer.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     5734 2023-05-07 06:32:41.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/persistence.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     2520 2023-05-13 06:35:01.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/templating.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     3641 2023-05-17 04:16:27.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/watch.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    14729 2023-03-28 18:29:00.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/wingdbstub.old.py
--rw-rw-r--   0 agp       (1000) agp       (1000)    14020 2023-03-28 18:27:21.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/wingdbstub.py
--rw-rw-r--   0 agp       (1000) agp       (1000)     9127 2023-05-18 05:53:27.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/wireguard.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.687617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/
--rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/PKG-INFO
--rw-rw-r--   0 agp       (1000) agp       (1000)     1279 2023-05-18 05:54:40.599617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/SOURCES.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        1 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/dependency_links.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)       47 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/entry_points.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.682711 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/not-zip-safe
--rw-rw-r--   0 agp       (1000) agp       (1000)       11 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/requires.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        9 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/top_level.txt
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      168 2022-08-06 09:24:18.000000 pycelium-0.1.2/AUTHORS.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3541 2022-08-06 09:24:18.000000 pycelium-0.1.2/CONTRIBUTING.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       89 2022-08-06 09:24:19.000000 pycelium-0.1.2/HISTORY.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1510 2022-08-06 09:24:19.000000 pycelium-0.1.2/LICENSE
+-rw-rw-r--   0 agp       (1000) agp       (1000)      262 2022-08-06 09:24:19.000000 pycelium-0.1.2/MANIFEST.in
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:04:19.927050 pycelium-0.1.2/PKG-INFO
+-rw-rw-r--   0 agp       (1000) agp       (1000)      876 2022-08-06 09:24:18.000000 pycelium-0.1.2/README.rst
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.923050 pycelium-0.1.2/docs/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      609 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/Makefile
+-rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/authors.rst
+-rwxrwxr-x   0 agp       (1000) agp       (1000)     4803 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/conf.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)       33 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/contributing.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/history.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)      305 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/index.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1150 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/installation.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)      806 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/make.bat
+-rw-rw-r--   0 agp       (1000) agp       (1000)       27 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/readme.rst
+-rw-rw-r--   0 agp       (1000) agp       (1000)       71 2022-08-06 09:24:19.000000 pycelium-0.1.2/docs/usage.rst
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/pycelium/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      138 2022-08-06 09:24:19.000000 pycelium-0.1.2/pycelium/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    27746 2023-05-17 04:24:18.000000 pycelium-0.1.2/pycelium/action.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      687 2023-05-13 06:02:42.000000 pycelium-0.1.2/pycelium/agent.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      402 2022-08-06 09:24:19.000000 pycelium-0.1.2/pycelium/cli.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.2/pycelium/containers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3786 2023-05-17 04:29:20.000000 pycelium-0.1.2/pycelium/definitions.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    17819 2023-05-16 04:07:05.000000 pycelium-0.1.2/pycelium/gathering.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      641 2023-04-30 12:58:35.000000 pycelium-0.1.2/pycelium/grafana.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    21784 2023-05-17 10:58:38.000000 pycelium-0.1.2/pycelium/modem.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2224 2023-05-15 11:18:29.000000 pycelium-0.1.2/pycelium/network.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     4593 2023-05-05 11:46:38.000000 pycelium-0.1.2/pycelium/packages.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     8408 2023-05-17 03:54:41.000000 pycelium-0.1.2/pycelium/pastor.py
+-r-xrwxr-x   0 agp       (1000) agp       (1000)    32037 2023-05-15 04:32:19.000000 pycelium-0.1.2/pycelium/pawn.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)       19 2022-08-06 09:24:19.000000 pycelium-0.1.2/pycelium/pycelium.py
+-rwxrwxr-x   0 agp       (1000) agp       (1000)    50518 2023-05-15 14:44:47.000000 pycelium-0.1.2/pycelium/scanner.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    51226 2023-05-17 04:19:30.000000 pycelium-0.1.2/pycelium/service.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    52755 2023-05-17 04:18:41.000000 pycelium-0.1.2/pycelium/shell.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)        0 2023-05-04 05:10:26.000000 pycelium-0.1.2/pycelium/ssh.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/pycelium/tools/
+-rw-rw-r--   0 agp       (1000) agp       (1000)    40887 2023-04-27 11:46:47.000000 pycelium-0.1.2/pycelium/tools/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    10670 2023-04-21 04:23:40.000000 pycelium-0.1.2/pycelium/tools/calls.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1500 2022-04-04 14:07:37.000000 pycelium-0.1.2/pycelium/tools/colors.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    22598 2022-05-07 15:33:49.000000 pycelium-0.1.2/pycelium/tools/configurations.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 pycelium-0.1.2/pycelium/tools/containers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5199 2023-04-28 10:31:35.000000 pycelium-0.1.2/pycelium/tools/helpers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    15780 2022-12-30 19:34:03.000000 pycelium-0.1.2/pycelium/tools/logs.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     6092 2023-05-02 11:20:30.000000 pycelium-0.1.2/pycelium/tools/metrics.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1786 2023-05-07 06:20:55.000000 pycelium-0.1.2/pycelium/tools/mixer.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5734 2023-05-07 06:32:41.000000 pycelium-0.1.2/pycelium/tools/persistence.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2520 2023-05-13 06:35:01.000000 pycelium-0.1.2/pycelium/tools/templating.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3641 2023-05-17 04:16:27.000000 pycelium-0.1.2/pycelium/watch.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    14729 2023-03-28 18:29:00.000000 pycelium-0.1.2/pycelium/wingdbstub.old.py
+-rw-r--r--   0 agp       (1000) agp       (1000)    14020 2023-03-28 18:27:21.000000 pycelium-0.1.2/pycelium/wingdbstub.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     9127 2023-05-18 05:53:27.000000 pycelium-0.1.2/pycelium/wireguard.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/pycelium.egg-info/
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/PKG-INFO
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1279 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/SOURCES.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        1 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/dependency_links.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)       47 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/entry_points.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.000000 pycelium-0.1.2/pycelium.egg-info/not-zip-safe
+-rw-rw-r--   0 agp       (1000) agp       (1000)       11 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/requires.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        9 2023-05-18 06:04:19.000000 pycelium-0.1.2/pycelium.egg-info/top_level.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)      425 2023-05-18 06:04:19.927050 pycelium-0.1.2/setup.cfg
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1407 2023-05-18 06:02:40.000000 pycelium-0.1.2/setup.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 06:04:19.927050 pycelium-0.1.2/tests/
+-rw-rw-r--   0 agp       (1000) agp       (1000)       38 2022-08-06 09:24:19.000000 pycelium-0.1.2/tests/__init__.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      544 2023-04-16 20:55:03.000000 pycelium-0.1.2/tests/test_init.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      984 2022-08-06 09:24:19.000000 pycelium-0.1.2/tests/test_pycelium.py
```

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/action.py` & `pycelium-0.1.2/pycelium/action.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/agent.py` & `pycelium-0.1.2/pycelium/agent.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/containers.py` & `pycelium-0.1.2/pycelium/containers.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/definitions.py` & `pycelium-0.1.2/pycelium/definitions.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/gathering.py` & `pycelium-0.1.2/pycelium/gathering.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/grafana.py` & `pycelium-0.1.2/pycelium/grafana.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/modem.py` & `pycelium-0.1.2/pycelium/modem.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/network.py` & `pycelium-0.1.2/pycelium/network.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/packages.py` & `pycelium-0.1.2/pycelium/packages.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/pastor.py` & `pycelium-0.1.2/pycelium/pastor.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/pawn.py` & `pycelium-0.1.2/pycelium/pawn.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/scanner.py` & `pycelium-0.1.2/pycelium/scanner.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/service.py` & `pycelium-0.1.2/pycelium/service.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/shell.py` & `pycelium-0.1.2/pycelium/shell.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/__init__.py` & `pycelium-0.1.2/pycelium/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/calls.py` & `pycelium-0.1.2/pycelium/tools/calls.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/colors.py` & `pycelium-0.1.2/pycelium/tools/colors.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/configurations.py` & `pycelium-0.1.2/pycelium/tools/configurations.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/containers.py` & `pycelium-0.1.2/pycelium/tools/containers.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/helpers.py` & `pycelium-0.1.2/pycelium/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/logs.py` & `pycelium-0.1.2/pycelium/tools/logs.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/metrics.py` & `pycelium-0.1.2/pycelium/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/mixer.py` & `pycelium-0.1.2/pycelium/tools/mixer.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/persistence.py` & `pycelium-0.1.2/pycelium/tools/persistence.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/tools/templating.py` & `pycelium-0.1.2/pycelium/tools/templating.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/watch.py` & `pycelium-0.1.2/pycelium/watch.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/wingdbstub.old.py` & `pycelium-0.1.2/pycelium/wingdbstub.old.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/wingdbstub.py` & `pycelium-0.1.2/pycelium/wingdbstub.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium/wireguard.py` & `pycelium-0.1.2/pycelium/wireguard.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/PKG-INFO` & `pycelium-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycelium
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Mycelium Edge Swarm Network
 Home-page: https://github.com/asteriogonzalez/pycelium
 Author: Asterio Gonzalez
 Author-email: asterio.gonzalez@gmail.com
 License: BSD license
 Keywords: pycelium
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/SOURCES.txt` & `pycelium-0.1.2/pycelium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

