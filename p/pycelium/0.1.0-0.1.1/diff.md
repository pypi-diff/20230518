# Comparing `tmp/pycelium-0.1.0.tar.gz` & `tmp/pycelium-0.1.1.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycelium-0.1.0.tar", last modified: Sat Aug  6 09:24:48 2022, max compression
+gzip compressed data, was "pycelium-0.1.1.linux-x86_64.tar", last modified: Thu May 18 05:54:40 2023, max compression
```

## Comparing `pycelium-0.1.0.tar` & `pycelium-0.1.1.linux-x86_64.tar`

### file list

```diff
@@ -1,36 +1,86 @@
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2022-08-06 09:24:48.722711 pycelium-0.1.0/
--rw-rw-r--   0 agp       (1000) agp       (1000)      168 2022-08-06 09:24:18.000000 pycelium-0.1.0/AUTHORS.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     3541 2022-08-06 09:24:18.000000 pycelium-0.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       89 2022-08-06 09:24:19.000000 pycelium-0.1.0/HISTORY.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     1510 2022-08-06 09:24:19.000000 pycelium-0.1.0/LICENSE
--rw-rw-r--   0 agp       (1000) agp       (1000)      262 2022-08-06 09:24:19.000000 pycelium-0.1.0/MANIFEST.in
--rw-rw-r--   0 agp       (1000) agp       (1000)     2036 2022-08-06 09:24:48.722711 pycelium-0.1.0/PKG-INFO
--rw-rw-r--   0 agp       (1000) agp       (1000)      876 2022-08-06 09:24:18.000000 pycelium-0.1.0/README.rst
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2022-08-06 09:24:48.722711 pycelium-0.1.0/docs/
--rw-rw-r--   0 agp       (1000) agp       (1000)      609 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/Makefile
--rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/authors.rst
--rwxrwxr-x   0 agp       (1000) agp       (1000)     4803 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/conf.py
--rw-rw-r--   0 agp       (1000) agp       (1000)       33 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/contributing.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       28 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/history.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)      305 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/index.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)     1150 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/installation.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)      806 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/make.bat
--rw-rw-r--   0 agp       (1000) agp       (1000)       27 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/readme.rst
--rw-rw-r--   0 agp       (1000) agp       (1000)       71 2022-08-06 09:24:19.000000 pycelium-0.1.0/docs/usage.rst
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2022-08-06 09:24:48.722711 pycelium-0.1.0/pycelium/
--rw-rw-r--   0 agp       (1000) agp       (1000)      138 2022-08-06 09:24:19.000000 pycelium-0.1.0/pycelium/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      402 2022-08-06 09:24:19.000000 pycelium-0.1.0/pycelium/cli.py
--rw-rw-r--   0 agp       (1000) agp       (1000)       19 2022-08-06 09:24:19.000000 pycelium-0.1.0/pycelium/pycelium.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2022-08-06 09:24:48.722711 pycelium-0.1.0/pycelium.egg-info/
--rw-rw-r--   0 agp       (1000) agp       (1000)     2036 2022-08-06 09:24:48.000000 pycelium-0.1.0/pycelium.egg-info/PKG-INFO
--rw-rw-r--   0 agp       (1000) agp       (1000)      579 2022-08-06 09:24:48.000000 pycelium-0.1.0/pycelium.egg-info/SOURCES.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.000000 pycelium-0.1.0/pycelium.egg-info/dependency_links.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)       48 2022-08-06 09:24:48.000000 pycelium-0.1.0/pycelium.egg-info/entry_points.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.000000 pycelium-0.1.0/pycelium.egg-info/not-zip-safe
--rw-rw-r--   0 agp       (1000) agp       (1000)       11 2022-08-06 09:24:48.000000 pycelium-0.1.0/pycelium.egg-info/requires.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)        9 2022-08-06 09:24:48.000000 pycelium-0.1.0/pycelium.egg-info/top_level.txt
--rw-rw-r--   0 agp       (1000) agp       (1000)      425 2022-08-06 09:24:48.722711 pycelium-0.1.0/setup.cfg
--rw-rw-r--   0 agp       (1000) agp       (1000)     1397 2022-08-06 09:24:18.000000 pycelium-0.1.0/setup.py
-drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2022-08-06 09:24:48.722711 pycelium-0.1.0/tests/
--rw-rw-r--   0 agp       (1000) agp       (1000)       38 2022-08-06 09:24:19.000000 pycelium-0.1.0/tests/__init__.py
--rw-rw-r--   0 agp       (1000) agp       (1000)      984 2022-08-06 09:24:19.000000 pycelium-0.1.0/tests/test_pycelium.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.615617 ./
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.615617 ./usr/
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.747617 ./usr/local/
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.747617 ./usr/local/bin/
+-rwxrwxr-x   0 agp       (1000) agp       (1000)      963 2023-05-18 05:54:40.747617 ./usr/local/bin/pycelium
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.615617 ./usr/local/lib/
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.615617 ./usr/local/lib/python3.10/
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.687617 ./usr/local/lib/python3.10/dist-packages/
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      138 2022-08-06 09:24:19.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/__init__.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.679617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/
+-rw-rw-r--   0 agp       (1000) agp       (1000)      303 2023-05-18 05:54:40.671617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    17883 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/action.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1217 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/agent.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)      577 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    47875 2023-05-18 05:54:40.663617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/containers.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2270 2023-05-18 05:54:40.663617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/definitions.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    14662 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/gathering.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)      766 2023-05-18 05:54:40.671617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/grafana.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    17100 2023-05-18 05:54:40.679617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/modem.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2338 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/network.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     4224 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/packages.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     4822 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/pastor.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    21293 2023-05-18 05:54:40.679617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/pawn.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)      177 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/pycelium.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    34149 2023-05-18 05:54:40.643617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/scanner.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    38422 2023-05-18 05:54:40.651617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/service.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    40112 2023-05-18 05:54:40.671617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/shell.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)      148 2023-05-18 05:54:40.671617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/ssh.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3179 2023-05-18 05:54:40.675617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/watch.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     6213 2023-05-18 05:54:40.651617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/wingdbstub.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     6499 2023-05-18 05:54:40.647617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/wingdbstub.old.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     6981 2023-05-18 05:54:40.647617 ./usr/local/lib/python3.10/dist-packages/pycelium/__pycache__/wireguard.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    27746 2023-05-17 04:24:18.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/action.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      687 2023-05-13 06:02:42.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/agent.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      402 2022-08-06 09:24:19.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/cli.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/containers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3786 2023-05-17 04:29:20.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/definitions.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    17819 2023-05-16 04:07:05.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/gathering.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)      641 2023-04-30 12:58:35.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/grafana.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    21784 2023-05-17 10:58:38.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/modem.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2224 2023-05-15 11:18:29.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/network.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     4593 2023-05-05 11:46:38.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/packages.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     8408 2023-05-17 03:54:41.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/pastor.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    32037 2023-05-15 04:32:19.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/pawn.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)       19 2022-08-06 09:24:19.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/pycelium.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    50518 2023-05-15 14:44:47.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/scanner.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    51226 2023-05-17 04:19:30.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/service.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    52755 2023-05-17 04:18:41.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/shell.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)        0 2023-05-04 05:10:26.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/ssh.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.619617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/
+-rw-rw-r--   0 agp       (1000) agp       (1000)    40887 2023-04-27 11:46:47.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__init__.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/
+-rw-rw-r--   0 agp       (1000) agp       (1000)    33973 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     7172 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/calls.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1433 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/colors.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    18006 2023-05-18 05:54:40.635617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/configurations.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    47881 2023-05-18 05:54:40.631617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/containers.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     4861 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/helpers.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    13364 2023-05-18 05:54:40.619617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/logs.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5187 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/metrics.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1974 2023-05-18 05:54:40.631617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/mixer.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     4277 2023-05-18 05:54:40.639617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/persistence.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2076 2023-05-18 05:54:40.623617 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/__pycache__/templating.cpython-310.pyc
+-rw-rw-r--   0 agp       (1000) agp       (1000)    10670 2023-04-21 04:23:40.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/calls.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1500 2022-04-04 14:07:37.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/colors.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    22598 2022-05-07 15:33:49.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/configurations.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    67899 2023-05-16 05:36:04.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/containers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5199 2023-04-28 10:31:35.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/helpers.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    15780 2022-12-30 19:34:03.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/logs.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     6092 2023-05-02 11:20:30.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/metrics.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1786 2023-05-07 06:20:55.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/mixer.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     5734 2023-05-07 06:32:41.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/persistence.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     2520 2023-05-13 06:35:01.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/tools/templating.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     3641 2023-05-17 04:16:27.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/watch.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    14729 2023-03-28 18:29:00.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/wingdbstub.old.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)    14020 2023-03-28 18:27:21.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/wingdbstub.py
+-rw-rw-r--   0 agp       (1000) agp       (1000)     9127 2023-05-18 05:53:27.000000 ./usr/local/lib/python3.10/dist-packages/pycelium/wireguard.py
+drwxrwxr-x   0 agp       (1000) agp       (1000)        0 2023-05-18 05:54:40.687617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1677 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/PKG-INFO
+-rw-rw-r--   0 agp       (1000) agp       (1000)     1279 2023-05-18 05:54:40.599617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/SOURCES.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        1 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/dependency_links.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)       47 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/entry_points.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        1 2022-08-06 09:24:48.682711 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/not-zip-safe
+-rw-rw-r--   0 agp       (1000) agp       (1000)       11 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/requires.txt
+-rw-rw-r--   0 agp       (1000) agp       (1000)        9 2023-05-18 05:54:40.591617 ./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/top_level.txt
```

### Comparing `pycelium-0.1.0/PKG-INFO` & `./usr/local/lib/python3.10/dist-packages/pycelium-0.1.1-py3.10.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,68 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pycelium
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Mycelium Edge Swarm Network
 Home-page: https://github.com/asteriogonzalez/pycelium
 Author: Asterio Gonzalez
 Author-email: asterio.gonzalez@gmail.com
 License: BSD license
-Description: ========
-        pycelium
-        ========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/pycelium.svg
-                :target: https://pypi.python.org/pypi/pycelium
-        
-        .. image:: https://img.shields.io/travis/asteriogonzalez/pycelium.svg
-                :target: https://travis-ci.com/asteriogonzalez/pycelium
-        
-        .. image:: https://readthedocs.org/projects/pycelium/badge/?version=latest
-                :target: https://pycelium.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Python Mycelium Edge Swarm Network
-        
-        
-        * Free software: BSD license
-        * Documentation: https://pycelium.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2022-08-06)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: pycelium
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.9
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+========
+pycelium
+========
+
+
+.. image:: https://img.shields.io/pypi/v/pycelium.svg
+        :target: https://pypi.python.org/pypi/pycelium
+
+.. image:: https://img.shields.io/travis/asteriogonzalez/pycelium.svg
+        :target: https://travis-ci.com/asteriogonzalez/pycelium
+
+.. image:: https://readthedocs.org/projects/pycelium/badge/?version=latest
+        :target: https://pycelium.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+
+
+
+Python Mycelium Edge Swarm Network
+
+
+* Free software: BSD license
+* Documentation: https://pycelium.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2022-08-06)
+------------------
+
+* First release on PyPI.
```

