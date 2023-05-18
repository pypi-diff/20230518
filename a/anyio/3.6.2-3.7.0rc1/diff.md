# Comparing `tmp/anyio-3.6.2.tar.gz` & `tmp/anyio-3.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyio-3.6.2.tar", last modified: Wed Oct 19 10:08:20 2022, max compression
+gzip compressed data, was "anyio-3.7.0rc1.tar", last modified: Thu May 18 16:06:13 2023, max compression
```

## Comparing `anyio-3.6.2.tar` & `anyio-3.7.0rc1.tar`

### file list

```diff
@@ -1,113 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.150153 anyio-3.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.134153 anyio-3.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.138153 anyio-3.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-10-19 10:08:05.000000 anyio-3.6.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-10-19 10:08:05.000000 anyio-3.6.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-19 10:08:05.000000 anyio-3.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-10-19 10:08:05.000000 anyio-3.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-19 10:08:05.000000 anyio-3.6.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-10-19 10:08:05.000000 anyio-3.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-10-19 10:08:20.150153 anyio-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-10-19 10:08:05.000000 anyio-3.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.142153 anyio-3.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     5937 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8379 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/cancellation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/fileio.rst
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5773 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6049 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/networking.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12265 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/streams.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/subprocesses.rst
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/support.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4829 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/synchronization.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5761 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6565 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/threads.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/typedattrs.rst
--rw-r--r--   0 runner    (1001) docker     (121)    31428 2022-10-19 10:08:05.000000 anyio-3.6.2/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-10-19 10:08:05.000000 anyio-3.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-10-19 10:08:20.150153 anyio-3.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-10-19 10:08:05.000000 anyio-3.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.138153 anyio-3.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.142153 anyio-3.6.2/src/anyio/
--rw-r--r--   0 runner    (1001) docker     (121)     4037 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.142153 anyio-3.6.2/src/anyio/_backends/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    69238 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_backends/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)    29696 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_backends/_trio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.142153 anyio-3.6.2/src/anyio/_core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5790 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    18298 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_fileio.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_signals.py
--rw-r--r--   0 runner    (1001) docker     (121)    19820 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (121)    16822 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/_core/_typedattr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.146153 anyio-3.6.2/src/anyio/abc/
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/abc/_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     5754 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/abc/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (121)     6501 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/abc/_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     2071 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/abc/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/abc/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1928 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/abc/_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    16497 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/from_thread.py
--rw-r--r--   0 runner    (1001) docker     (121)     4679 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5134 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.146153 anyio-3.6.2/src/anyio/streams/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/streams/buffered.py
--rw-r--r--   0 runner    (1001) docker     (121)     4353 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/streams/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     9209 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/streams/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     4258 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/streams/stapled.py
--rw-r--r--   0 runner    (1001) docker     (121)     5014 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/streams/text.py
--rw-r--r--   0 runner    (1001) docker     (121)    12040 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/streams/tls.py
--rw-r--r--   0 runner    (1001) docker     (121)     9247 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/to_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-10-19 10:08:05.000000 anyio-3.6.2/src/anyio/to_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.142153 anyio-3.6.2/src/anyio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-10-19 10:08:20.000000 anyio-3.6.2/src/anyio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-10-19 10:08:20.000000 anyio-3.6.2/src/anyio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 10:08:20.000000 anyio-3.6.2/src/anyio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-19 10:08:20.000000 anyio-3.6.2/src/anyio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 10:08:20.000000 anyio-3.6.2/src/anyio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-10-19 10:08:20.000000 anyio-3.6.2/src/anyio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-19 10:08:20.000000 anyio-3.6.2/src/anyio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.146153 anyio-3.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:20.150153 anyio-3.6.2/tests/streams/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/streams/test_buffered.py
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/streams/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    10877 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/streams/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     5587 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/streams/test_stapled.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/streams/test_text.py
--rw-r--r--   0 runner    (1001) docker     (121)    14419 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/streams/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (121)     7107 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4901 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_debugging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (121)    18117 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (121)    18210 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_from_thread.py
--rw-r--r--   0 runner    (1001) docker     (121)     3363 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (121)     9200 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (121)    51084 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (121)     5443 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (121)    16927 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (121)    30834 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_taskgroups.py
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_to_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     7711 2022-10-19 10:08:05.000000 anyio-3.6.2/tests/test_to_thread.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-19 10:08:05.000000 anyio-3.6.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/cancellation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/fileio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/networking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/subprocesses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/synchronization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/threads.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/typedattrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34214 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio/_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67067 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30046 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/_trio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20667 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_typedattr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/stapled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/tests/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_stapled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51369 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34173 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_taskgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_to_thread.py
```

### Comparing `anyio-3.6.2/.github/workflows/publish.yml` & `anyio-3.7.0rc1/.github/workflows/publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 name: Publish packages to PyPI
 
 on:
   push:
     tags:
       - "[0-9]+.[0-9]+.[0-9]+"
+      - "[0-9]+.[0-9]+.[0-9]+.post[0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+[a-b][0-9]+"
       - "[0-9]+.[0-9]+.[0-9]+rc[0-9]+"
 
 jobs:
   publish:
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.x
     - name: Install dependencies
       run: pip install build
     - name: Create packages
-      run: python -m build -s -w .
+      run: python -m build
     - name: Upload packages
-      uses: pypa/gh-action-pypi-publish@master
-      with:
-        user: __token__
-        password: ${{ secrets.pypi_password }}
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `anyio-3.6.2/.github/workflows/test.yml` & `anyio-3.7.0rc1/.github/workflows/test.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,72 @@
 name: test suite
 
 on:
   push:
-    branches: [master]
+    branches: [master, 3.x]
   pull_request:
 
 jobs:
   pyright:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.x
-    - uses: actions/cache@v2
+    - uses: actions/cache@v3
       with:
         path: ~/.cache/pip
         key: pip-pyright
     - name: Install dependencies
       run: pip install -e . pyright pytest
     - name: Run pyright
       run: pyright --verifytypes anyio
 
   test:
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", pypy-3.7]
-        exclude:
+        os: [ubuntu-latest]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", pypy-3.8]
+        include:
         - os: macos-latest
           python-version: "3.7"
         - os: macos-latest
-          python-version: "3.8"
-        - os: macos-latest
-          python-version: "3.9"
-        - os: macos-latest
-          python-version: pypy-3.7
+          python-version: "3.11"
         - os: windows-latest
           python-version: "3.7"
         - os: windows-latest
-          python-version: "3.8"
-        - os: windows-latest
-          python-version: "3.9"
-        - os: windows-latest
-          python-version: pypy-3.7  # https://github.com/python-trio/trio/issues/1361
+          python-version: "3.11"
     runs-on: ${{ matrix.os }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-    - uses: actions/cache@v2
-      with:
-        path: ~/.cache/pip
-        key: pip-test-${{ matrix.python-version }}-${{ matrix.os }}
+        cache: pip
+        cache-dependency-path: setup.cfg
     - name: Install dependencies
       run: pip install .[test,trio] coveralls
     - name: Test with pytest
-      run: coverage run -m pytest
+      run: coverage run -m pytest -v
+      timeout-minutes: 5
       env:
         PYTEST_DISABLE_PLUGIN_AUTOLOAD: 1
     - name: Upload Coverage
       run: coveralls --service=github
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         COVERALLS_FLAG_NAME: ${{ matrix.test-name }}
         COVERALLS_PARALLEL: true
 
   coveralls:
     name: Finish Coveralls
     needs: test
     runs-on: ubuntu-latest
-    container: python:3-slim
     steps:
     - name: Finished
-      run: |
-        pip install coveralls
-        coveralls --service=github --finish
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+      uses: coverallsapp/github-action@v2
+      with:
+        parallel-finished: true
```

### Comparing `anyio-3.6.2/LICENSE` & `anyio-3.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/PKG-INFO` & `anyio-3.7.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 3.6.2
+Version: 3.7.0rc1
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
-Author: Alex Grönholm
-Author-email: alex.gronholm@nextday.fi
+Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
+Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AnyIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.2
-Provides-Extra: test
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: trio
+Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/agronholm/anyio/actions/workflows/test.yml/badge.svg
   :target: https://github.com/agronholm/anyio/actions/workflows/test.yml
   :alt: Build Status
 .. image:: https://coveralls.io/repos/github/agronholm/anyio/badge.svg?branch=master
@@ -35,33 +36,33 @@
   :target: https://anyio.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation
 .. image:: https://badges.gitter.im/gitterHQ/gitter.svg
   :target: https://gitter.im/python-trio/AnyIO
   :alt: Gitter chat
 
 AnyIO is an asynchronous networking and concurrency library that works on top of either asyncio_ or
-trio_. It implements trio-like `structured concurrency`_ (SC) on top of asyncio, and works in harmony
+trio_. It implements trio-like `structured concurrency`_ (SC) on top of asyncio and works in harmony
 with the native SC of trio itself.
 
 Applications and libraries written against AnyIO's API will run unmodified on either asyncio_ or
 trio_. AnyIO can also be adopted into a library or application incrementally – bit by bit, no full
-refactoring necessary. It will blend in with native libraries of your chosen backend.
+refactoring necessary. It will blend in with the native libraries of your chosen backend.
 
 Documentation
 -------------
 
 View full documentation at: https://anyio.readthedocs.io/
 
 Features
 --------
 
 AnyIO offers the following functionality:
 
 * Task groups (nurseries_ in trio terminology)
-* High level networking (TCP, UDP and UNIX sockets)
+* High-level networking (TCP, UDP and UNIX sockets)
 
   * `Happy eyeballs`_ algorithm for TCP connections (more robust than that of asyncio on Python
     3.8)
   * async/await style UDP sockets (unlike asyncio where you still have to use Transports and
     Protocols)
 
 * A versatile API for byte streams and object streams
```

### Comparing `anyio-3.6.2/README.rst` & `anyio-3.7.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -8,33 +8,33 @@
   :target: https://anyio.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation
 .. image:: https://badges.gitter.im/gitterHQ/gitter.svg
   :target: https://gitter.im/python-trio/AnyIO
   :alt: Gitter chat
 
 AnyIO is an asynchronous networking and concurrency library that works on top of either asyncio_ or
-trio_. It implements trio-like `structured concurrency`_ (SC) on top of asyncio, and works in harmony
+trio_. It implements trio-like `structured concurrency`_ (SC) on top of asyncio and works in harmony
 with the native SC of trio itself.
 
 Applications and libraries written against AnyIO's API will run unmodified on either asyncio_ or
 trio_. AnyIO can also be adopted into a library or application incrementally – bit by bit, no full
-refactoring necessary. It will blend in with native libraries of your chosen backend.
+refactoring necessary. It will blend in with the native libraries of your chosen backend.
 
 Documentation
 -------------
 
 View full documentation at: https://anyio.readthedocs.io/
 
 Features
 --------
 
 AnyIO offers the following functionality:
 
 * Task groups (nurseries_ in trio terminology)
-* High level networking (TCP, UDP and UNIX sockets)
+* High-level networking (TCP, UDP and UNIX sockets)
 
   * `Happy eyeballs`_ algorithm for TCP connections (more robust than that of asyncio on Python
     3.8)
   * async/await style UDP sockets (unlike asyncio where you still have to use Transports and
     Protocols)
 
 * A versatile API for byte streams and object streams
```

### Comparing `anyio-3.6.2/docs/api.rst` & `anyio-3.7.0rc1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/basics.rst` & `anyio-3.7.0rc1/docs/basics.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 The basics
 ==========
 
 .. py:currentmodule:: anyio
 
-AnyIO requires Python 3.6.2 or later to run. It is recommended that you set up a virtualenv_ when
+AnyIO requires Python 3.7 or later to run. It is recommended that you set up a virtualenv_ when
 developing or playing around with AnyIO.
 
 Installation
 ------------
 
 To install AnyIO, run:
```

### Comparing `anyio-3.6.2/docs/cancellation.rst` & `anyio-3.7.0rc1/docs/cancellation.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/conf.py` & `anyio-3.7.0rc1/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 from importlib.metadata import version as get_version
 
 from packaging.version import parse
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
@@ -16,19 +18,18 @@
 author = "Alex Grönholm"
 copyright = "2018, " + author
 
 v = parse(get_version("anyio"))
 version = v.base_version
 release = v.public
 
-language = None
+language = "en"
 
 exclude_patterns = ["_build"]
 pygments_style = "sphinx"
 autodoc_default_options = {"members": True, "show-inheritance": True}
 todo_include_todos = False
 
 html_theme = "sphinx_rtd_theme"
-html_static_path = ["_static"]
 htmlhelp_basename = "anyiodoc"
 
 intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
```

### Comparing `anyio-3.6.2/docs/contributing.rst` & `anyio-3.7.0rc1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/faq.rst` & `anyio-3.7.0rc1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/fileio.rst` & `anyio-3.7.0rc1/docs/fileio.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/migration.rst` & `anyio-3.7.0rc1/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/networking.rst` & `anyio-3.7.0rc1/docs/networking.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/signals.rst` & `anyio-3.7.0rc1/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/streams.rst` & `anyio-3.7.0rc1/docs/streams.rst`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 It can mean either in-process communication or sending data over a network.
 AnyIO divides streams into two categories: byte streams and object streams.
 
 Byte streams ("Streams" in Trio lingo) are objects that receive and/or send chunks of bytes.
 They are modelled after the limitations of the stream sockets, meaning the boundaries are not
 respected. In practice this means that if, for example, you call ``.send(b'hello ')`` and then
 ``.send(b'world')``, the other end will receive the data chunked in any arbitrary way, like
-(``b'hello'`` and ``b'world'``), ``b'hello world'`` or (``b'hel'``, ``b'lo wo'``, ``b'rld'``).
+(``b'hello'`` and ``b' world'``), ``b'hello world'`` or (``b'hel'``, ``b'lo wo'``, ``b'rld'``).
 
 Object streams ("Channels" in Trio lingo), on the other hand, deal with Python objects. The most
 commonly used implementation of these is the memory object stream. The exact semantics of object
 streams vary a lot by implementation.
 
 Many stream implementations wrap other streams. Of these, some can wrap any bytes-oriented streams,
 meaning ``ObjectStream[bytes]`` and ``ByteStream``. This enables many interesting use cases.
```

### Comparing `anyio-3.6.2/docs/subprocesses.rst` & `anyio-3.7.0rc1/docs/subprocesses.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/support.rst` & `anyio-3.7.0rc1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/synchronization.rst` & `anyio-3.7.0rc1/docs/synchronization.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/tasks.rst` & `anyio-3.7.0rc1/docs/tasks.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     from anyio.abc import TaskStatus
 
 
     async def handler(stream):
         ...
 
 
-    async def start_some_service(port: int, *, task_status: TaskStatus = TASK_STATUS_IGNORED):
+    async def start_some_service(port: int, *, task_status: TaskStatus[None] = TASK_STATUS_IGNORED):
         async with await create_tcp_listener(local_host='127.0.0.1', local_port=port) as listener:
             task_status.started()
             await listener.serve(handler)
 
 
     async def main():
         async with create_task_group() as tg:
```

### Comparing `anyio-3.6.2/docs/testing.rst` & `anyio-3.7.0rc1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.6.2/docs/threads.rst` & `anyio-3.7.0rc1/docs/threads.rst`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 
     async def main():
         async with BlockingPortal() as portal:
             # ...hand off the portal to external threads...
             await portal.sleep_until_stopped()
 
-    anyio.run(main)
+    run(main)
 
 Spawning tasks from worker threads
 ----------------------------------
 
 When you need to spawn a task to be run in the background, you can do so using
 :meth:`~.BlockingPortal.start_task_soon`::
 
@@ -183,9 +183,24 @@
 
 When running functions in worker threads, the current context is copied to the worker thread.
 Therefore any context variables available on the task will also be available to the code running
 on the thread. As always with context variables, any changes made to them will not propagate back
 to the calling asynchronous task.
 
 When calling asynchronous code from worker threads, context is again copied to the task that calls
-the target function in the event loop thread. Note, however, that this **does not work** on asyncio
-when running on Python 3.6.
+the target function in the event loop thread.
+
+Adjusting the default maximum worker thread count
+-------------------------------------------------
+
+The default AnyIO worker thread limiter has a value of **40**, meaning that any calls
+to :func:`.to_thread.run` without an explicit ``limiter`` argument will cause a maximum
+of 40 threads to be spawned. You can adjust this limit like this::
+
+    from anyio import to_thread
+
+    async def foo():
+        # Set the maximum number of worker threads to 60
+        to_thread.current_default_thread_limiter().total_tokens = 60
+
+.. note:: AnyIO's default thread pool limiter does not affect the default thread pool
+    executor on :mod:`asyncio`.
```

### Comparing `anyio-3.6.2/docs/typedattrs.rst` & `anyio-3.7.0rc1/docs/typedattrs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 until the attribute is either found or the end of the chain is reached. This also lets wrappers
 override attributes from the wrapped objects when necessary.
 
 A common use case is finding the IP address of the remote side of a TCP connection when the
 stream may be either :class:`~.abc.SocketStream` or :class:`~.streams.tls.TLSStream`::
 
     from anyio import connect_tcp
+    from anyio.abc import SocketAttribute
 
 
     async def connect(host, port, tls: bool):
         stream = await connect_tcp(host, port, tls=tls)
         print('Connected to', stream.extra(SocketAttribute.remote_address))
 
 Each typed attribute provider class should document the set of attributes it provides on its own.
```

### Comparing `anyio-3.6.2/docs/versionhistory.rst` & `anyio-3.7.0rc1/docs/versionhistory.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,69 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <http://semver.org/>`_.
 
+**3.7.0rc1**
+
+- Dropped support for Python 3.6
+- Improved type annotations:
+
+  - Several functions and methods that were previously annotated as accepting
+    ``Coroutine[Any, Any, Any]`` as the return type of the callable have been amended to
+    accept ``Awaitable[Any]`` instead, to allow a slightly broader set of coroutine-like
+    inputs, like ``async_generator_asend`` objects returned from the ``asend()`` method
+    of async generators, and to match the ``trio`` annotations:
+
+    - ``anyio.run()``
+    - ``anyio.from_thread.run()``
+    - ``TaskGroup.start_soon()``
+    - ``TaskGroup.start()``
+    - ``BlockingPortal.call()``
+    - ``BlockingPortal.start_task_soon()``
+    - ``BlockingPortal.start_task()``
+
+    Note that this change involved only changing the type annotations; run-time
+    functionality was not altered.
+
+  - The ``TaskStatus`` class is now a generic protocol, and should be parametrized to
+    indicate the type of the value passed to ``task_status.started()``
+  - The ``Listener`` class is now covariant in its stream type
+  - ``create_memory_object_stream()`` now allows passing only ``item_type``
+  - Object receive streams are now covariant and object send streams are correspondingly
+    contravariant
+- Changed ``TLSAttribute.shared_ciphers`` to match the documented semantics of
+  ``SSLSocket.shared_ciphers`` of always returning ``None`` for client-side streams
+- Fixed ``CapacityLimiter`` on the asyncio backend to order waiting tasks in the FIFO
+  order (instead of LIFO) (PR by Conor Stevenson)
+- Fixed ``CancelScope.cancel()`` not working on asyncio if called before entering the
+  scope
+- Fixed ``open_signal_receiver()`` inconsistently yielding integers instead of
+  ``signal.Signals`` instances on the ``trio`` backend
+- Fixed ``to_thread.run_sync()`` hanging on asyncio if the target callable raises
+  ``StopIteration``
+- Fixed ``start_blocking_portal()`` raising an unwarranted
+  ``RuntimeError: This portal is not running`` if a task raises an exception that causes
+  the event loop to be closed
+- Fixed ``current_effective_deadline()`` not returning ``-inf`` on asyncio when the
+  currently active cancel scope has been cancelled (PR by Ganden Schaffner)
+- Fixed the ``OP_IGNORE_UNEXPECTED_EOF`` flag in an SSL context created by default in
+  ``TLSStream.wrap()`` being inadvertently set on Python 3.11.3 and 3.10.11
+- Fixed ``CancelScope`` to properly handle asyncio task uncancellation on Python 3.11
+  (PR by Nikolay Bryskin)
+- Fixed ``OSError`` when trying to use ``create_tcp_listener()`` to bind to a link-local
+  IPv6 address (and worked around related bugs in ``uvloop``)
+- Worked around a `PyPy bug <https://foss.heptapod.net/pypy/pypy/-/issues/3938>`_
+  when using ``anyio.getaddrinfo()`` with for IPv6 link-local addresses containing
+  interface names
+
 **3.6.2**
 
 - Pinned Trio to < 0.22 to avoid incompatibility with AnyIO's ``ExceptionGroup`` class
   causing ``AttributeError: 'NonBaseMultiError' object has no attribute '_exceptions'``
-  (AnyIO 4 is unaffected)
 
 **3.6.1**
 
 - Fixed exception handler in the asyncio test runner not properly handling a context
   that does not contain the ``exception`` key
 
 **3.6.0**
```

### Comparing `anyio-3.6.2/src/anyio/__init__.py` & `anyio-3.7.0rc1/src/anyio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = (
     "maybe_async",
     "maybe_async_cm",
     "run",
     "sleep",
     "sleep_forever",
     "sleep_until",
```

### Comparing `anyio-3.6.2/src/anyio/_backends/_asyncio.py` & `anyio-3.7.0rc1/src/anyio/_backends/_asyncio.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import array
 import asyncio
 import concurrent.futures
 import math
 import socket
 import sys
 from asyncio.base_events import _run_until_complete_cb  # type: ignore[attr-defined]
@@ -29,24 +31,20 @@
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
     Collection,
     Coroutine,
     Deque,
-    Dict,
     Generator,
     Iterable,
-    List,
     Mapping,
     Optional,
     Sequence,
-    Set,
     Tuple,
-    Type,
     TypeVar,
     Union,
     cast,
 )
 from weakref import WeakKeyDictionary
 
 import sniffio
@@ -55,137 +53,52 @@
 from .._core._compat import DeprecatedAsyncContextManager, DeprecatedAwaitable
 from .._core._eventloop import claim_worker_thread, threadlocals
 from .._core._exceptions import (
     BrokenResourceError,
     BusyResourceError,
     ClosedResourceError,
     EndOfStream,
+    WouldBlock,
 )
 from .._core._exceptions import ExceptionGroup as BaseExceptionGroup
-from .._core._exceptions import WouldBlock
 from .._core._sockets import GetAddrInfoReturnType, convert_ipv6_sockaddr
 from .._core._synchronization import CapacityLimiter as BaseCapacityLimiter
 from .._core._synchronization import Event as BaseEvent
 from .._core._synchronization import ResourceGuard
 from .._core._tasks import CancelScope as BaseCancelScope
 from ..abc import IPSockAddrType, UDPPacketType
 from ..lowlevel import RunVar
 
 if sys.version_info >= (3, 8):
 
-    def get_coro(task: asyncio.Task) -> Union[Generator, Awaitable[Any]]:
+    def get_coro(task: asyncio.Task) -> Generator | Awaitable[Any]:
         return task.get_coro()
 
 else:
 
-    def get_coro(task: asyncio.Task) -> Union[Generator, Awaitable[Any]]:
+    def get_coro(task: asyncio.Task) -> Generator | Awaitable[Any]:
         return task._coro
 
 
-if sys.version_info >= (3, 7):
-    from asyncio import all_tasks, create_task, current_task, get_running_loop
-    from asyncio import run as native_run
-
-    def _get_task_callbacks(task: asyncio.Task) -> Iterable[Callable]:
-        return [cb for cb, context in task._callbacks]  # type: ignore[attr-defined]
-
-else:
-    _T = TypeVar("_T")
-
-    def _get_task_callbacks(task: asyncio.Task) -> Iterable[Callable]:
-        return task._callbacks
-
-    def native_run(main, *, debug=False):
-        # Snatched from Python 3.7
-        from asyncio import coroutines, events, tasks
-
-        def _cancel_all_tasks(loop):
-            to_cancel = all_tasks(loop)
-            if not to_cancel:
-                return
-
-            for task in to_cancel:
-                task.cancel()
-
-            loop.run_until_complete(
-                tasks.gather(*to_cancel, loop=loop, return_exceptions=True)
-            )
-
-            for task in to_cancel:
-                if task.cancelled():
-                    continue
-                if task.exception() is not None:
-                    loop.call_exception_handler(
-                        {
-                            "message": "unhandled exception during asyncio.run() shutdown",
-                            "exception": task.exception(),
-                            "task": task,
-                        }
-                    )
+from asyncio import all_tasks, create_task, current_task, get_running_loop
+from asyncio import run as native_run
 
-        if events._get_running_loop() is not None:
-            raise RuntimeError(
-                "asyncio.run() cannot be called from a running event loop"
-            )
 
-        if not coroutines.iscoroutine(main):
-            raise ValueError(f"a coroutine was expected, got {main!r}")
-
-        loop = events.new_event_loop()
-        try:
-            events.set_event_loop(loop)
-            loop.set_debug(debug)
-            return loop.run_until_complete(main)
-        finally:
-            try:
-                _cancel_all_tasks(loop)
-                loop.run_until_complete(loop.shutdown_asyncgens())
-            finally:
-                events.set_event_loop(None)
-                loop.close()
-
-    def create_task(
-        coro: Union[Generator[Any, None, _T], Awaitable[_T]], *, name: object = None
-    ) -> asyncio.Task:
-        return get_running_loop().create_task(coro)
-
-    def get_running_loop() -> asyncio.AbstractEventLoop:
-        loop = asyncio._get_running_loop()
-        if loop is not None:
-            return loop
-        else:
-            raise RuntimeError("no running event loop")
-
-    def all_tasks(
-        loop: Optional[asyncio.AbstractEventLoop] = None,
-    ) -> Set[asyncio.Task]:
-        """Return a set of all tasks for the loop."""
-        from asyncio import Task
-
-        if loop is None:
-            loop = get_running_loop()
-
-        return {t for t in Task.all_tasks(loop) if not t.done()}
-
-    def current_task(
-        loop: Optional[asyncio.AbstractEventLoop] = None,
-    ) -> Optional[asyncio.Task]:
-        if loop is None:
-            loop = get_running_loop()
-
-        return asyncio.Task.current_task(loop)
+def _get_task_callbacks(task: asyncio.Task) -> Iterable[Callable]:
+    return [cb for cb, context in task._callbacks]
 
 
 T_Retval = TypeVar("T_Retval")
+T_contra = TypeVar("T_contra", contravariant=True)
 
 # Check whether there is native support for task names in asyncio (3.8+)
 _native_task_names = hasattr(asyncio.Task, "get_name")
 
 
-_root_task: RunVar[Optional[asyncio.Task]] = RunVar("_root_task")
+_root_task: RunVar[asyncio.Task | None] = RunVar("_root_task")
 
 
 def find_root_task() -> asyncio.Task:
     root_task = _root_task.get(None)
     if root_task is not None and not root_task.done():
         return root_task
 
@@ -244,15 +157,15 @@
             )
         except AttributeError:
             # task coro is async_genenerator_asend https://bugs.python.org/issue37771
             raise Exception(f"Cannot determine if task {task} has started or not")
 
 
 def _maybe_set_event_loop_policy(
-    policy: Optional[asyncio.AbstractEventLoopPolicy], use_uvloop: bool
+    policy: asyncio.AbstractEventLoopPolicy | None, use_uvloop: bool
 ) -> None:
     # On CPython, use uvloop when possible if no other policy has been given and if not
     # explicitly disabled
     if policy is None and use_uvloop and sys.implementation.name == "cpython":
         try:
             import uvloop
         except ImportError:
@@ -269,15 +182,15 @@
 
 
 def run(
     func: Callable[..., Awaitable[T_Retval]],
     *args: object,
     debug: bool = False,
     use_uvloop: bool = False,
-    policy: Optional[asyncio.AbstractEventLoopPolicy] = None,
+    policy: asyncio.AbstractEventLoopPolicy | None = None,
 ) -> T_Retval:
     @wraps(func)
     async def wrapper() -> T_Retval:
         task = cast(asyncio.Task, current_task())
         task_state = TaskState(None, get_callable_name(func), None)
         _task_states[task] = task_state
         if _native_task_names:
@@ -305,30 +218,31 @@
 
 CancelledError = asyncio.CancelledError
 
 
 class CancelScope(BaseCancelScope):
     def __new__(
         cls, *, deadline: float = math.inf, shield: bool = False
-    ) -> "CancelScope":
+    ) -> CancelScope:
         return object.__new__(cls)
 
     def __init__(self, deadline: float = math.inf, shield: bool = False):
         self._deadline = deadline
         self._shield = shield
-        self._parent_scope: Optional[CancelScope] = None
+        self._parent_scope: CancelScope | None = None
         self._cancel_called = False
         self._active = False
-        self._timeout_handle: Optional[asyncio.TimerHandle] = None
-        self._cancel_handle: Optional[asyncio.Handle] = None
-        self._tasks: Set[asyncio.Task] = set()
-        self._host_task: Optional[asyncio.Task] = None
+        self._timeout_handle: asyncio.TimerHandle | None = None
+        self._cancel_handle: asyncio.Handle | None = None
+        self._tasks: set[asyncio.Task] = set()
+        self._host_task: asyncio.Task | None = None
         self._timeout_expired = False
+        self._cancel_calls: int = 0
 
-    def __enter__(self) -> "CancelScope":
+    def __enter__(self) -> CancelScope:
         if self._active:
             raise RuntimeError(
                 "Each CancelScope may only be used for a single 'with' block"
             )
 
         self._host_task = host_task = cast(asyncio.Task, current_task())
         self._tasks.add(host_task)
@@ -340,22 +254,27 @@
             _task_states[host_task] = task_state
         else:
             self._parent_scope = task_state.cancel_scope
             task_state.cancel_scope = self
 
         self._timeout()
         self._active = True
+
+        # Start cancelling the host task if the scope was cancelled before entering
+        if self._cancel_called:
+            self._deliver_cancellation()
+
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         if not self._active:
             raise RuntimeError("This cancel scope is not active")
         if current_task() is not self._host_task:
             raise RuntimeError(
                 "Attempted to exit cancel scope in a different task than it was "
                 "entered in"
             )
@@ -384,24 +303,36 @@
 
         if exc_val is not None:
             exceptions = (
                 exc_val.exceptions if isinstance(exc_val, ExceptionGroup) else [exc_val]
             )
             if all(isinstance(exc, CancelledError) for exc in exceptions):
                 if self._timeout_expired:
-                    return True
+                    return self._uncancel()
                 elif not self._cancel_called:
                     # Task was cancelled natively
                     return None
                 elif not self._parent_cancelled():
                     # This scope was directly cancelled
-                    return True
+                    return self._uncancel()
 
         return None
 
+    def _uncancel(self) -> bool:
+        if sys.version_info < (3, 11) or self._host_task is None:
+            self._cancel_calls = 0
+            return True
+
+        # Uncancel all AnyIO cancellations
+        for i in range(self._cancel_calls):
+            self._host_task.uncancel()
+
+        self._cancel_calls = 0
+        return not self._host_task.cancelling()
+
     def _timeout(self) -> None:
         if self._deadline != math.inf:
             loop = get_running_loop()
             if loop.time() >= self._deadline:
                 self._timeout_expired = True
                 self.cancel()
             else:
@@ -428,28 +359,29 @@
                 else:
                     cancel_scope = cancel_scope._parent_scope
             else:
                 should_retry = True
                 if task is not current and (
                     task is self._host_task or _task_started(task)
                 ):
+                    self._cancel_calls += 1
                     task.cancel()
 
         # Schedule another callback if there are still tasks left
         if should_retry:
             self._cancel_handle = get_running_loop().call_soon(
                 self._deliver_cancellation
             )
         else:
             self._cancel_handle = None
 
     def _deliver_cancellation_to_parent(self) -> None:
         """Start cancellation effort in the farthest directly cancelled parent scope"""
         scope = self._parent_scope
-        scope_to_cancel: Optional[CancelScope] = None
+        scope_to_cancel: CancelScope | None = None
         while scope is not None:
             if scope._cancel_called and scope._cancel_handle is None:
                 scope_to_cancel = scope
 
             # No point in looking beyond any shielded scope
             if scope._shield:
                 break
@@ -473,15 +405,16 @@
     def cancel(self) -> DeprecatedAwaitable:
         if not self._cancel_called:
             if self._timeout_handle:
                 self._timeout_handle.cancel()
                 self._timeout_handle = None
 
             self._cancel_called = True
-            self._deliver_cancellation()
+            if self._host_task is not None:
+                self._deliver_cancellation()
 
         return DeprecatedAwaitable(self.cancel)
 
     @property
     def deadline(self) -> float:
         return self._deadline
 
@@ -544,15 +477,18 @@
         cancel_scope = _task_states[current_task()].cancel_scope  # type: ignore[index]
     except KeyError:
         return math.inf
 
     deadline = math.inf
     while cancel_scope:
         deadline = min(deadline, cancel_scope.deadline)
-        if cancel_scope.shield:
+        if cancel_scope._cancel_called:
+            deadline = -math.inf
+            break
+        elif cancel_scope.shield:
             break
         else:
             cancel_scope = cancel_scope._parent_scope
 
     return deadline
 
 
@@ -571,17 +507,17 @@
     because there are no guarantees about its implementation.
     """
 
     __slots__ = "parent_id", "name", "cancel_scope"
 
     def __init__(
         self,
-        parent_id: Optional[int],
-        name: Optional[str],
-        cancel_scope: Optional[CancelScope],
+        parent_id: int | None,
+        name: str | None,
+        cancel_scope: CancelScope | None,
     ):
         self.parent_id = parent_id
         self.name = name
         self.cancel_scope = cancel_scope
 
 
 _task_states = WeakKeyDictionary()  # type: WeakKeyDictionary[asyncio.Task, TaskState]
@@ -589,25 +525,25 @@
 
 #
 # Task groups
 #
 
 
 class ExceptionGroup(BaseExceptionGroup):
-    def __init__(self, exceptions: List[BaseException]):
+    def __init__(self, exceptions: list[BaseException]):
         super().__init__()
         self.exceptions = exceptions
 
 
 class _AsyncioTaskStatus(abc.TaskStatus):
     def __init__(self, future: asyncio.Future, parent_id: int):
         self._future = future
         self._parent_id = parent_id
 
-    def started(self, value: object = None) -> None:
+    def started(self, value: T_contra | None = None) -> None:
         try:
             self._future.set_result(value)
         except asyncio.InvalidStateError:
             raise RuntimeError(
                 "called 'started' twice on the same task status"
             ) from None
 
@@ -615,27 +551,27 @@
         _task_states[task].parent_id = self._parent_id
 
 
 class TaskGroup(abc.TaskGroup):
     def __init__(self) -> None:
         self.cancel_scope: CancelScope = CancelScope()
         self._active = False
-        self._exceptions: List[BaseException] = []
+        self._exceptions: list[BaseException] = []
 
-    async def __aenter__(self) -> "TaskGroup":
+    async def __aenter__(self) -> TaskGroup:
         self.cancel_scope.__enter__()
         self._active = True
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         ignore_exception = self.cancel_scope.__exit__(exc_type, exc_val, exc_tb)
         if exc_val is not None:
             self.cancel_scope.cancel()
             self._exceptions.append(exc_val)
 
         while self.cancel_scope._tasks:
             try:
@@ -667,16 +603,16 @@
             raise
 
         return ignore_exception
 
     @staticmethod
     def _filter_cancellation_errors(
         exceptions: Sequence[BaseException],
-    ) -> List[BaseException]:
-        filtered_exceptions: List[BaseException] = []
+    ) -> list[BaseException]:
+        filtered_exceptions: list[BaseException] = []
         for exc in exceptions:
             if isinstance(exc, ExceptionGroup):
                 new_exceptions = TaskGroup._filter_cancellation_errors(exc.exceptions)
                 if len(new_exceptions) > 1:
                     filtered_exceptions.append(exc)
                 elif len(new_exceptions) == 1:
                     filtered_exceptions.append(new_exceptions[0])
@@ -688,18 +624,18 @@
                     filtered_exceptions.append(new_exc)
             elif not isinstance(exc, CancelledError) or exc.args:
                 filtered_exceptions.append(exc)
 
         return filtered_exceptions
 
     async def _run_wrapped_task(
-        self, coro: Coroutine, task_status_future: Optional[asyncio.Future]
+        self, coro: Coroutine, task_status_future: asyncio.Future | None
     ) -> None:
-        # This is the code path for Python 3.6 and 3.7 on which asyncio freaks out if a task raises
-        # a BaseException.
+        # This is the code path for Python 3.7 on which asyncio freaks out if a task
+        # raises a BaseException.
         __traceback_hide__ = __tracebackhide__ = True  # noqa: F841
         task = cast(asyncio.Task, current_task())
         try:
             await coro
         except BaseException as exc:
             if task_status_future is None or task_status_future.done():
                 self._exceptions.append(exc)
@@ -714,18 +650,18 @@
         finally:
             if task in self.cancel_scope._tasks:
                 self.cancel_scope._tasks.remove(task)
                 del _task_states[task]
 
     def _spawn(
         self,
-        func: Callable[..., Coroutine],
+        func: Callable[..., Awaitable[Any]],
         args: tuple,
         name: object,
-        task_status_future: Optional[asyncio.Future] = None,
+        task_status_future: asyncio.Future | None = None,
     ) -> asyncio.Task:
         def task_done(_task: asyncio.Task) -> None:
             # This is the code path for Python 3.8+
             assert _task in self.cancel_scope._tasks
             self.cancel_scope._tasks.remove(_task)
             del _task_states[_task]
 
@@ -749,15 +685,15 @@
                 )
 
         if not self._active:
             raise RuntimeError(
                 "This task group is not active; no new tasks can be started."
             )
 
-        options = {}
+        options: dict[str, Any] = {}
         name = get_callable_name(func) if name is None else str(name)
         if _native_task_names:
             options["name"] = name
 
         kwargs = {}
         if task_status_future:
             parent_id = id(current_task())
@@ -785,20 +721,20 @@
         _task_states[task] = TaskState(
             parent_id=parent_id, name=name, cancel_scope=self.cancel_scope
         )
         self.cancel_scope._tasks.add(task)
         return task
 
     def start_soon(
-        self, func: Callable[..., Coroutine], *args: object, name: object = None
+        self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
     ) -> None:
         self._spawn(func, args, name)
 
     async def start(
-        self, func: Callable[..., Coroutine], *args: object, name: object = None
+        self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
     ) -> None:
         future: asyncio.Future = asyncio.Future()
         task = self._spawn(func, args, name, future)
 
         # If the task raises an exception after sending a start value without a switch point
         # between, the task group is cancelled and this method never proceeds to process the
         # completed future. That's why we have to have a shielded cancel scope here.
@@ -819,37 +755,42 @@
 
 class WorkerThread(Thread):
     MAX_IDLE_TIME = 10  # seconds
 
     def __init__(
         self,
         root_task: asyncio.Task,
-        workers: Set["WorkerThread"],
-        idle_workers: Deque["WorkerThread"],
+        workers: set[WorkerThread],
+        idle_workers: Deque[WorkerThread],
     ):
         super().__init__(name="AnyIO worker thread")
         self.root_task = root_task
         self.workers = workers
         self.idle_workers = idle_workers
         self.loop = root_task._loop
         self.queue: Queue[
-            Union[Tuple[Context, Callable, tuple, asyncio.Future], None]
+            tuple[Context, Callable, tuple, asyncio.Future] | None
         ] = Queue(2)
         self.idle_since = current_time()
         self.stopping = False
 
     def _report_result(
-        self, future: asyncio.Future, result: Any, exc: Optional[BaseException]
+        self, future: asyncio.Future, result: Any, exc: BaseException | None
     ) -> None:
         self.idle_since = current_time()
         if not self.stopping:
             self.idle_workers.append(self)
 
         if not future.cancelled():
             if exc is not None:
+                if isinstance(exc, StopIteration):
+                    new_exc = RuntimeError("coroutine raised StopIteration")
+                    new_exc.__cause__ = exc
+                    exc = new_exc
+
                 future.set_exception(exc)
             else:
                 future.set_result(result)
 
     def run(self) -> None:
         with claim_worker_thread("asyncio"):
             threadlocals.loop = self.loop
@@ -858,48 +799,48 @@
                 if item is None:
                     # Shutdown command received
                     return
 
                 context, func, args, future = item
                 if not future.cancelled():
                     result = None
-                    exception: Optional[BaseException] = None
+                    exception: BaseException | None = None
                     try:
                         result = context.run(func, *args)
                     except BaseException as exc:
                         exception = exc
 
                     if not self.loop.is_closed():
                         self.loop.call_soon_threadsafe(
                             self._report_result, future, result, exception
                         )
 
                 self.queue.task_done()
 
-    def stop(self, f: Optional[asyncio.Task] = None) -> None:
+    def stop(self, f: asyncio.Task | None = None) -> None:
         self.stopping = True
         self.queue.put_nowait(None)
         self.workers.discard(self)
         try:
             self.idle_workers.remove(self)
         except ValueError:
             pass
 
 
 _threadpool_idle_workers: RunVar[Deque[WorkerThread]] = RunVar(
     "_threadpool_idle_workers"
 )
-_threadpool_workers: RunVar[Set[WorkerThread]] = RunVar("_threadpool_workers")
+_threadpool_workers: RunVar[set[WorkerThread]] = RunVar("_threadpool_workers")
 
 
 async def run_sync_in_worker_thread(
     func: Callable[..., T_Retval],
     *args: object,
     cancellable: bool = False,
-    limiter: Optional["CapacityLimiter"] = None,
+    limiter: CapacityLimiter | None = None,
 ) -> T_Retval:
     await checkpoint()
 
     # If this is the first run in this event loop thread, set up the necessary variables
     try:
         idle_workers = _threadpool_idle_workers.get()
         workers = _threadpool_workers.get()
@@ -936,57 +877,53 @@
             worker.queue.put_nowait((context, func, args, future))
             return await future
 
 
 def run_sync_from_thread(
     func: Callable[..., T_Retval],
     *args: object,
-    loop: Optional[asyncio.AbstractEventLoop] = None,
+    loop: asyncio.AbstractEventLoop | None = None,
 ) -> T_Retval:
     @wraps(func)
     def wrapper() -> None:
         try:
             f.set_result(func(*args))
         except BaseException as exc:
             f.set_exception(exc)
             if not isinstance(exc, Exception):
                 raise
 
     f: concurrent.futures.Future[T_Retval] = Future()
     loop = loop or threadlocals.loop
-    if sys.version_info < (3, 7):
-        loop.call_soon_threadsafe(copy_context().run, wrapper)
-    else:
-        loop.call_soon_threadsafe(wrapper)
-
+    loop.call_soon_threadsafe(wrapper)
     return f.result()
 
 
 def run_async_from_thread(
-    func: Callable[..., Coroutine[Any, Any, T_Retval]], *args: object
+    func: Callable[..., Awaitable[T_Retval]], *args: object
 ) -> T_Retval:
     f: concurrent.futures.Future[T_Retval] = asyncio.run_coroutine_threadsafe(
         func(*args), threadlocals.loop
     )
     return f.result()
 
 
 class BlockingPortal(abc.BlockingPortal):
-    def __new__(cls) -> "BlockingPortal":
+    def __new__(cls) -> BlockingPortal:
         return object.__new__(cls)
 
     def __init__(self) -> None:
         super().__init__()
         self._loop = get_running_loop()
 
     def _spawn_task_from_thread(
         self,
         func: Callable,
         args: tuple,
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
         name: object,
         future: Future,
     ) -> None:
         run_sync_from_thread(
             partial(self._task_group.start_soon, name=name),
             self._call_func,
             func,
@@ -1028,17 +965,17 @@
     async def aclose(self) -> None:
         self._stream.close()
 
 
 @dataclass(eq=False)
 class Process(abc.Process):
     _process: asyncio.subprocess.Process
-    _stdin: Optional[StreamWriterWrapper]
-    _stdout: Optional[StreamReaderWrapper]
-    _stderr: Optional[StreamReaderWrapper]
+    _stdin: StreamWriterWrapper | None
+    _stdout: StreamReaderWrapper | None
+    _stderr: StreamReaderWrapper | None
 
     async def aclose(self) -> None:
         if self._stdin:
             await self._stdin.aclose()
         if self._stdout:
             await self._stdout.aclose()
         if self._stderr:
@@ -1059,39 +996,39 @@
         self._process.send_signal(signal)
 
     @property
     def pid(self) -> int:
         return self._process.pid
 
     @property
-    def returncode(self) -> Optional[int]:
+    def returncode(self) -> int | None:
         return self._process.returncode
 
     @property
-    def stdin(self) -> Optional[abc.ByteSendStream]:
+    def stdin(self) -> abc.ByteSendStream | None:
         return self._stdin
 
     @property
-    def stdout(self) -> Optional[abc.ByteReceiveStream]:
+    def stdout(self) -> abc.ByteReceiveStream | None:
         return self._stdout
 
     @property
-    def stderr(self) -> Optional[abc.ByteReceiveStream]:
+    def stderr(self) -> abc.ByteReceiveStream | None:
         return self._stderr
 
 
 async def open_process(
-    command: Union[str, bytes, Sequence[Union[str, bytes]]],
+    command: str | bytes | Sequence[str | bytes],
     *,
     shell: bool,
-    stdin: Union[int, IO[Any], None],
-    stdout: Union[int, IO[Any], None],
-    stderr: Union[int, IO[Any], None],
-    cwd: Union[str, bytes, PathLike, None] = None,
-    env: Optional[Mapping[str, str]] = None,
+    stdin: int | IO[Any] | None,
+    stdout: int | IO[Any] | None,
+    stderr: int | IO[Any] | None,
+    cwd: str | bytes | PathLike | None = None,
+    env: Mapping[str, str] | None = None,
     start_new_session: bool = False,
 ) -> Process:
     await checkpoint()
     if shell:
         process = await asyncio.create_subprocess_shell(
             cast(Union[str, bytes], command),
             stdin=stdin,
@@ -1115,19 +1052,19 @@
     stdin_stream = StreamWriterWrapper(process.stdin) if process.stdin else None
     stdout_stream = StreamReaderWrapper(process.stdout) if process.stdout else None
     stderr_stream = StreamReaderWrapper(process.stderr) if process.stderr else None
     return Process(process, stdin_stream, stdout_stream, stderr_stream)
 
 
 def _forcibly_shutdown_process_pool_on_exit(
-    workers: Set[Process], _task: object
+    workers: set[Process], _task: object
 ) -> None:
     """
     Forcibly shuts down worker processes belonging to this event loop."""
-    child_watcher: Optional[asyncio.AbstractChildWatcher]
+    child_watcher: asyncio.AbstractChildWatcher | None
     try:
         child_watcher = asyncio.get_event_loop_policy().get_child_watcher()
     except NotImplementedError:
         child_watcher = None
 
     # Close as much as possible (w/o async/await) to avoid warnings
     for process in workers:
@@ -1138,15 +1075,15 @@
         process._stdout._stream._transport.close()  # type: ignore[union-attr]
         process._stderr._stream._transport.close()  # type: ignore[union-attr]
         process.kill()
         if child_watcher:
             child_watcher.remove_child_handler(process.pid)
 
 
-async def _shutdown_process_pool_on_exit(workers: Set[Process]) -> None:
+async def _shutdown_process_pool_on_exit(workers: set[Process]) -> None:
     """
     Shuts down worker processes belonging to this event loop.
 
     NOTE: this only works when the event loop was started using asyncio.run() or anyio.run().
 
     """
     process: Process
@@ -1157,16 +1094,18 @@
             if process.returncode is None:
                 process.kill()
 
         for process in workers:
             await process.aclose()
 
 
-def setup_process_pool_exit_at_shutdown(workers: Set[Process]) -> None:
-    kwargs = {"name": "AnyIO process pool shutdown task"} if _native_task_names else {}
+def setup_process_pool_exit_at_shutdown(workers: set[Process]) -> None:
+    kwargs: dict[str, Any] = (
+        {"name": "AnyIO process pool shutdown task"} if _native_task_names else {}
+    )
     create_task(_shutdown_process_pool_on_exit(workers), **kwargs)
     find_root_task().add_done_callback(
         partial(_forcibly_shutdown_process_pool_on_exit, workers)
     )
 
 
 #
@@ -1174,59 +1113,59 @@
 #
 
 
 class StreamProtocol(asyncio.Protocol):
     read_queue: Deque[bytes]
     read_event: asyncio.Event
     write_event: asyncio.Event
-    exception: Optional[Exception] = None
+    exception: Exception | None = None
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         self.read_queue = deque()
         self.read_event = asyncio.Event()
         self.write_event = asyncio.Event()
         self.write_event.set()
         cast(asyncio.Transport, transport).set_write_buffer_limits(0)
 
-    def connection_lost(self, exc: Optional[Exception]) -> None:
+    def connection_lost(self, exc: Exception | None) -> None:
         if exc:
             self.exception = BrokenResourceError()
             self.exception.__cause__ = exc
 
         self.read_event.set()
         self.write_event.set()
 
     def data_received(self, data: bytes) -> None:
         self.read_queue.append(data)
         self.read_event.set()
 
-    def eof_received(self) -> Optional[bool]:
+    def eof_received(self) -> bool | None:
         self.read_event.set()
         return True
 
     def pause_writing(self) -> None:
         self.write_event = asyncio.Event()
 
     def resume_writing(self) -> None:
         self.write_event.set()
 
 
 class DatagramProtocol(asyncio.DatagramProtocol):
-    read_queue: Deque[Tuple[bytes, IPSockAddrType]]
+    read_queue: Deque[tuple[bytes, IPSockAddrType]]
     read_event: asyncio.Event
     write_event: asyncio.Event
-    exception: Optional[Exception] = None
+    exception: Exception | None = None
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         self.read_queue = deque(maxlen=100)  # arbitrary value
         self.read_event = asyncio.Event()
         self.write_event = asyncio.Event()
         self.write_event.set()
 
-    def connection_lost(self, exc: Optional[Exception]) -> None:
+    def connection_lost(self, exc: Exception | None) -> None:
         self.read_event.set()
         self.write_event.set()
 
     def datagram_received(self, data: bytes, addr: IPSockAddrType) -> None:
         addr = convert_ipv6_sockaddr(addr)
         self.read_queue.append((data, addr))
         self.read_event.set()
@@ -1322,16 +1261,16 @@
 
             self._transport.close()
             await sleep(0)
             self._transport.abort()
 
 
 class UNIXSocketStream(abc.SocketStream):
-    _receive_future: Optional[asyncio.Future] = None
-    _send_future: Optional[asyncio.Future] = None
+    _receive_future: asyncio.Future | None = None
+    _send_future: asyncio.Future | None = None
     _closing = False
 
     def __init__(self, raw_socket: socket.socket):
         self.__raw_socket = raw_socket
         self._loop = get_running_loop()
         self._receive_guard = ResourceGuard("reading from")
         self._send_guard = ResourceGuard("writing to")
@@ -1398,15 +1337,15 @@
                     if self._closing:
                         raise ClosedResourceError from None
                     else:
                         raise BrokenResourceError from exc
                 else:
                     view = view[bytes_sent:]
 
-    async def receive_fds(self, msglen: int, maxfds: int) -> Tuple[bytes, List[int]]:
+    async def receive_fds(self, msglen: int, maxfds: int) -> tuple[bytes, list[int]]:
         if not isinstance(msglen, int) or msglen < 0:
             raise ValueError("msglen must be a non-negative integer")
         if not isinstance(maxfds, int) or maxfds < 1:
             raise ValueError("maxfds must be a positive integer")
 
         loop = get_running_loop()
         fds = array.array("i")
@@ -1437,24 +1376,22 @@
                     f"cmsg_level = {cmsg_level}, cmsg_type = {cmsg_type}"
                 )
 
             fds.frombytes(cmsg_data[: len(cmsg_data) - (len(cmsg_data) % fds.itemsize)])
 
         return message, list(fds)
 
-    async def send_fds(
-        self, message: bytes, fds: Collection[Union[int, IOBase]]
-    ) -> None:
+    async def send_fds(self, message: bytes, fds: Collection[int | IOBase]) -> None:
         if not message:
             raise ValueError("message must not be empty")
         if not fds:
             raise ValueError("fds must not be empty")
 
         loop = get_running_loop()
-        filenos: List[int] = []
+        filenos: list[int] = []
         for fd in fds:
             if isinstance(fd, int):
                 filenos.append(fd)
             elif isinstance(fd, IOBase):
                 filenos.append(fd.fileno())
 
         fdarray = array.array("i", filenos)
@@ -1485,15 +1422,15 @@
             if self._receive_future:
                 self._receive_future.set_result(None)
             if self._send_future:
                 self._send_future.set_result(None)
 
 
 class TCPSocketListener(abc.SocketListener):
-    _accept_scope: Optional[CancelScope] = None
+    _accept_scope: CancelScope | None = None
     _closed = False
 
     def __init__(self, raw_socket: socket.socket):
         self.__raw_socket = raw_socket
         self._loop = cast(asyncio.BaseEventLoop, get_running_loop())
         self._accept_guard = ResourceGuard("accepting connections from")
 
@@ -1524,15 +1461,15 @@
                 finally:
                     self._accept_scope = None
 
         client_sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         transport, protocol = await self._loop.connect_accepted_socket(
             StreamProtocol, client_sock
         )
-        return SocketStream(cast(asyncio.Transport, transport), protocol)
+        return SocketStream(transport, protocol)
 
     async def aclose(self) -> None:
         if self._closed:
             return
 
         self._closed = True
         if self._accept_scope:
@@ -1600,15 +1537,15 @@
         return self._transport.get_extra_info("socket")
 
     async def aclose(self) -> None:
         if not self._transport.is_closing():
             self._closed = True
             self._transport.close()
 
-    async def receive(self) -> Tuple[bytes, IPSockAddrType]:
+    async def receive(self) -> tuple[bytes, IPSockAddrType]:
         with self._receive_guard:
             await checkpoint()
 
             # If the buffer is empty, ask for more data
             if not self._protocol.read_queue and not self._transport.is_closing():
                 self._protocol.read_event.clear()
                 await self._protocol.read_event.wait()
@@ -1680,15 +1617,15 @@
             elif self._transport.is_closing():
                 raise BrokenResourceError
             else:
                 self._transport.sendto(item)
 
 
 async def connect_tcp(
-    host: str, port: int, local_addr: Optional[Tuple[str, int]] = None
+    host: str, port: int, local_addr: tuple[str, int] | None = None
 ) -> SocketStream:
     transport, protocol = cast(
         Tuple[asyncio.Transport, StreamProtocol],
         await get_running_loop().create_connection(
             StreamProtocol, host, port, local_addr=local_addr
         ),
     )
@@ -1714,59 +1651,59 @@
             raise
         else:
             return UNIXSocketStream(raw_socket)
 
 
 async def create_udp_socket(
     family: socket.AddressFamily,
-    local_address: Optional[IPSockAddrType],
-    remote_address: Optional[IPSockAddrType],
+    local_address: IPSockAddrType | None,
+    remote_address: IPSockAddrType | None,
     reuse_port: bool,
-) -> Union[UDPSocket, ConnectedUDPSocket]:
+) -> UDPSocket | ConnectedUDPSocket:
     result = await get_running_loop().create_datagram_endpoint(
         DatagramProtocol,
         local_addr=local_address,
         remote_addr=remote_address,
         family=family,
         reuse_port=reuse_port,
     )
-    transport = cast(asyncio.DatagramTransport, result[0])
+    transport = result[0]
     protocol = result[1]
     if protocol.exception:
         transport.close()
         raise protocol.exception
 
     if not remote_address:
         return UDPSocket(transport, protocol)
     else:
         return ConnectedUDPSocket(transport, protocol)
 
 
 async def getaddrinfo(
-    host: Union[bytes, str],
-    port: Union[str, int, None],
+    host: bytes | str,
+    port: str | int | None,
     *,
-    family: Union[int, AddressFamily] = 0,
-    type: Union[int, SocketKind] = 0,
+    family: int | AddressFamily = 0,
+    type: int | SocketKind = 0,
     proto: int = 0,
     flags: int = 0,
 ) -> GetAddrInfoReturnType:
     # https://github.com/python/typeshed/pull/4304
     result = await get_running_loop().getaddrinfo(
         host, port, family=family, type=type, proto=proto, flags=flags
     )
     return cast(GetAddrInfoReturnType, result)
 
 
-async def getnameinfo(sockaddr: IPSockAddrType, flags: int = 0) -> Tuple[str, str]:
+async def getnameinfo(sockaddr: IPSockAddrType, flags: int = 0) -> tuple[str, str]:
     return await get_running_loop().getnameinfo(sockaddr, flags)
 
 
-_read_events: RunVar[Dict[Any, asyncio.Event]] = RunVar("read_events")
-_write_events: RunVar[Dict[Any, asyncio.Event]] = RunVar("write_events")
+_read_events: RunVar[dict[Any, asyncio.Event]] = RunVar("read_events")
+_write_events: RunVar[dict[Any, asyncio.Event]] = RunVar("write_events")
 
 
 async def wait_socket_readable(sock: socket.socket) -> None:
     await checkpoint()
     try:
         read_events = _read_events.get()
     except LookupError:
@@ -1821,15 +1758,15 @@
 
 #
 # Synchronization
 #
 
 
 class Event(BaseEvent):
-    def __new__(cls) -> "Event":
+    def __new__(cls) -> Event:
         return object.__new__(cls)
 
     def __init__(self) -> None:
         self._event = asyncio.Event()
 
     def set(self) -> DeprecatedAwaitable:
         self._event.set()
@@ -1845,30 +1782,30 @@
     def statistics(self) -> EventStatistics:
         return EventStatistics(len(self._event._waiters))  # type: ignore[attr-defined]
 
 
 class CapacityLimiter(BaseCapacityLimiter):
     _total_tokens: float = 0
 
-    def __new__(cls, total_tokens: float) -> "CapacityLimiter":
+    def __new__(cls, total_tokens: float) -> CapacityLimiter:
         return object.__new__(cls)
 
     def __init__(self, total_tokens: float):
-        self._borrowers: Set[Any] = set()
-        self._wait_queue: Dict[Any, asyncio.Event] = OrderedDict()
+        self._borrowers: set[Any] = set()
+        self._wait_queue: OrderedDict[Any, asyncio.Event] = OrderedDict()
         self.total_tokens = total_tokens
 
     async def __aenter__(self) -> None:
         await self.acquire()
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         self.release()
 
     @property
     def total_tokens(self) -> float:
         return self._total_tokens
 
@@ -1951,15 +1888,15 @@
         except KeyError:
             raise RuntimeError(
                 "this borrower isn't holding any of this CapacityLimiter's " "tokens"
             ) from None
 
         # Notify the next task in line if this limiter has free capacity now
         if self._wait_queue and len(self._borrowers) < self._total_tokens:
-            event = self._wait_queue.popitem()[1]
+            event = self._wait_queue.popitem(last=False)[1]
             event.set()
 
     def statistics(self) -> CapacityLimiterStatistics:
         return CapacityLimiterStatistics(
             self.borrowed_tokens,
             self.total_tokens,
             tuple(self._borrowers),
@@ -1981,44 +1918,44 @@
 
 #
 # Operating system signals
 #
 
 
 class _SignalReceiver(DeprecatedAsyncContextManager["_SignalReceiver"]):
-    def __init__(self, signals: Tuple[int, ...]):
+    def __init__(self, signals: tuple[int, ...]):
         self._signals = signals
         self._loop = get_running_loop()
         self._signal_queue: Deque[int] = deque()
         self._future: asyncio.Future = asyncio.Future()
-        self._handled_signals: Set[int] = set()
+        self._handled_signals: set[int] = set()
 
     def _deliver(self, signum: int) -> None:
         self._signal_queue.append(signum)
         if not self._future.done():
             self._future.set_result(None)
 
-    def __enter__(self) -> "_SignalReceiver":
+    def __enter__(self) -> _SignalReceiver:
         for sig in set(self._signals):
             self._loop.add_signal_handler(sig, self._deliver, sig)
             self._handled_signals.add(sig)
 
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         for sig in self._handled_signals:
             self._loop.remove_signal_handler(sig)
         return None
 
-    def __aiter__(self) -> "_SignalReceiver":
+    def __aiter__(self) -> _SignalReceiver:
         return self
 
     async def __anext__(self) -> int:
         await checkpoint()
         if not self._signal_queue:
             self._future = asyncio.Future()
             await self._future
@@ -2047,15 +1984,15 @@
     return TaskInfo(id(task), parent_id, name, get_coro(task))
 
 
 def get_current_task() -> TaskInfo:
     return _create_task_info(current_task())  # type: ignore[arg-type]
 
 
-def get_running_tasks() -> List[TaskInfo]:
+def get_running_tasks() -> list[TaskInfo]:
     return [_create_task_info(task) for task in all_tasks() if not task.done()]
 
 
 async def wait_all_tasks_blocked() -> None:
     await checkpoint()
     this_task = current_task()
     while True:
@@ -2071,17 +2008,17 @@
 
 
 class TestRunner(abc.TestRunner):
     def __init__(
         self,
         debug: bool = False,
         use_uvloop: bool = False,
-        policy: Optional[asyncio.AbstractEventLoopPolicy] = None,
+        policy: asyncio.AbstractEventLoopPolicy | None = None,
     ):
-        self._exceptions: List[BaseException] = []
+        self._exceptions: list[BaseException] = []
         _maybe_set_event_loop_policy(policy, use_uvloop)
         self._loop = asyncio.new_event_loop()
         self._loop.set_debug(debug)
         self._loop.set_exception_handler(self._exception_handler)
         asyncio.set_event_loop(self._loop)
 
     def _cancel_all_tasks(self) -> None:
@@ -2099,15 +2036,15 @@
         for task in to_cancel:
             if task.cancelled():
                 continue
             if task.exception() is not None:
                 raise cast(BaseException, task.exception())
 
     def _exception_handler(
-        self, loop: asyncio.AbstractEventLoop, context: Dict[str, Any]
+        self, loop: asyncio.AbstractEventLoop, context: dict[str, Any]
     ) -> None:
         if isinstance(context.get("exception"), Exception):
             self._exceptions.append(context["exception"])
         else:
             loop.default_exception_handler(context)
 
     def _raise_async_exceptions(self) -> None:
@@ -2126,15 +2063,15 @@
         finally:
             asyncio.set_event_loop(None)
             self._loop.close()
 
     def run_asyncgen_fixture(
         self,
         fixture_func: Callable[..., AsyncGenerator[T_Retval, Any]],
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
     ) -> Iterable[T_Retval]:
         async def fixture_runner() -> None:
             agen = fixture_func(**kwargs)
             try:
                 retval = await agen.asend(None)
                 self._raise_async_exceptions()
             except BaseException as exc:
@@ -2160,22 +2097,22 @@
         event.set()
         self._loop.run_until_complete(fixture_task)
         self._raise_async_exceptions()
 
     def run_fixture(
         self,
         fixture_func: Callable[..., Coroutine[Any, Any, T_Retval]],
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
     ) -> T_Retval:
         retval = self._loop.run_until_complete(fixture_func(**kwargs))
         self._raise_async_exceptions()
         return retval
 
     def run_test(
-        self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: Dict[str, Any]
+        self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: dict[str, Any]
     ) -> None:
         try:
             self._loop.run_until_complete(test_func(**kwargs))
         except Exception as exc:
             self._exceptions.append(exc)
 
         self._raise_async_exceptions()
```

### Comparing `anyio-3.6.2/src/anyio/_backends/_trio.py` & `anyio-3.7.0rc1/src/anyio/_backends/_trio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import array
 import math
 import socket
 from concurrent.futures import Future
 from contextvars import copy_context
 from dataclasses import dataclass
 from functools import partial
@@ -10,44 +12,37 @@
 from signal import Signals
 from types import TracebackType
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     AsyncGenerator,
+    AsyncIterator,
     Awaitable,
     Callable,
     Collection,
-    ContextManager,
     Coroutine,
     Deque,
-    Dict,
     Generic,
     Iterable,
-    List,
     Mapping,
     NoReturn,
-    Optional,
     Sequence,
-    Set,
-    Tuple,
-    Type,
     TypeVar,
-    Union,
     cast,
 )
 
 import sniffio
 import trio.from_thread
 from outcome import Error, Outcome, Value
 from trio.socket import SocketType as TrioSocketType
 from trio.to_thread import run_sync
 
 from .. import CapacityLimiterStatistics, EventStatistics, TaskInfo, abc
-from .._core._compat import DeprecatedAsyncContextManager, DeprecatedAwaitable, T
+from .._core._compat import DeprecatedAsyncContextManager, DeprecatedAwaitable
 from .._core._eventloop import claim_worker_thread
 from .._core._exceptions import (
     BrokenResourceError,
     BusyResourceError,
     ClosedResourceError,
     EndOfStream,
 )
@@ -67,17 +62,20 @@
 except ImportError:
     from trio import hazmat as trio_lowlevel  # type: ignore[no-redef]
     from trio.hazmat import wait_readable, wait_writable
 else:
     from trio.lowlevel import wait_readable, wait_writable
 
 try:
-    trio_open_process = trio_lowlevel.open_process  # type: ignore[attr-defined]
+    trio_open_process = trio_lowlevel.open_process
 except AttributeError:
-    from trio import open_process as trio_open_process
+    # isort: off
+    from trio import (  # type: ignore[attr-defined, no-redef]
+        open_process as trio_open_process,
+    )
 
 T_Retval = TypeVar("T_Retval")
 T_SockAddr = TypeVar("T_SockAddr", str, IPSockAddrType)
 
 
 #
 # Event loop
@@ -98,34 +96,35 @@
 #
 # Timeouts and cancellation
 #
 
 
 class CancelScope(BaseCancelScope):
     def __new__(
-        cls, original: Optional[trio.CancelScope] = None, **kwargs: object
-    ) -> "CancelScope":
+        cls, original: trio.CancelScope | None = None, **kwargs: object
+    ) -> CancelScope:
         return object.__new__(cls)
 
-    def __init__(
-        self, original: Optional[trio.CancelScope] = None, **kwargs: Any
-    ) -> None:
+    def __init__(self, original: trio.CancelScope | None = None, **kwargs: Any) -> None:
         self.__original = original or trio.CancelScope(**kwargs)
 
-    def __enter__(self) -> "CancelScope":
+    def __enter__(self) -> CancelScope:
         self.__original.__enter__()
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
-        return self.__original.__exit__(exc_type, exc_val, exc_tb)
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
+        # https://github.com/python-trio/trio-typing/pull/79
+        return self.__original.__exit__(  # type: ignore[func-returns-value]
+            exc_type, exc_val, exc_tb
+        )
 
     def cancel(self) -> DeprecatedAwaitable:
         self.__original.cancel()
         return DeprecatedAwaitable(self.cancel)
 
     @property
     def deadline(self) -> float:
@@ -167,43 +166,45 @@
 
 class TaskGroup(abc.TaskGroup):
     def __init__(self) -> None:
         self._active = False
         self._nursery_manager = trio.open_nursery()
         self.cancel_scope = None  # type: ignore[assignment]
 
-    async def __aenter__(self) -> "TaskGroup":
+    async def __aenter__(self) -> TaskGroup:
         self._active = True
         self._nursery = await self._nursery_manager.__aenter__()
         self.cancel_scope = CancelScope(self._nursery.cancel_scope)
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         try:
             return await self._nursery_manager.__aexit__(exc_type, exc_val, exc_tb)
         except trio.MultiError as exc:
             raise ExceptionGroup(exc.exceptions) from None
         finally:
             self._active = False
 
-    def start_soon(self, func: Callable, *args: object, name: object = None) -> None:
+    def start_soon(
+        self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
+    ) -> None:
         if not self._active:
             raise RuntimeError(
                 "This task group is not active; no new tasks can be started."
             )
 
         self._nursery.start_soon(func, *args, name=name)
 
     async def start(
-        self, func: Callable[..., Coroutine], *args: object, name: object = None
+        self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
     ) -> object:
         if not self._active:
             raise RuntimeError(
                 "This task group is not active; no new tasks can be started."
             )
 
         return await self._nursery.start(func, *args, name=name)
@@ -214,15 +215,15 @@
 #
 
 
 async def run_sync_in_worker_thread(
     func: Callable[..., T_Retval],
     *args: object,
     cancellable: bool = False,
-    limiter: Optional[trio.CapacityLimiter] = None,
+    limiter: trio.CapacityLimiter | None = None,
 ) -> T_Retval:
     def wrapper() -> T_Retval:
         with claim_worker_thread("trio"):
             return func(*args)
 
     # TODO: remove explicit context copying when trio 0.20 is the minimum requirement
     context = copy_context()
@@ -244,40 +245,40 @@
             __tracebackhide__ = True
             retval = await fn(*args)
 
         async with trio.open_nursery() as n:
             context.run(n.start_soon, inner)
 
         __tracebackhide__ = True
-        return retval
+        return retval  # noqa: F821
 
     context = copy_context()
     context.run(sniffio.current_async_library_cvar.set, "trio")
     return trio.from_thread.run(wrapper)
 
 
 def run_sync_from_thread(fn: Callable[..., T_Retval], *args: Any) -> T_Retval:
     # TODO: remove explicit context copying when trio 0.20 is the minimum requirement
     retval = trio.from_thread.run_sync(copy_context().run, fn, *args)
     return cast(T_Retval, retval)
 
 
 class BlockingPortal(abc.BlockingPortal):
-    def __new__(cls) -> "BlockingPortal":
+    def __new__(cls) -> BlockingPortal:
         return object.__new__(cls)
 
     def __init__(self) -> None:
         super().__init__()
         self._token = trio.lowlevel.current_trio_token()
 
     def _spawn_task_from_thread(
         self,
         func: Callable,
         args: tuple,
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
         name: object,
         future: Future,
     ) -> None:
         context = copy_context()
         context.run(sniffio.current_async_library_cvar.set, "trio")
         trio.from_thread.run_sync(
             context.run,
@@ -296,15 +297,15 @@
 #
 
 
 @dataclass(eq=False)
 class ReceiveStreamWrapper(abc.ByteReceiveStream):
     _stream: trio.abc.ReceiveStream
 
-    async def receive(self, max_bytes: Optional[int] = None) -> bytes:
+    async def receive(self, max_bytes: int | None = None) -> bytes:
         try:
             data = await self._stream.receive_some(max_bytes)
         except trio.ClosedResourceError as exc:
             raise ClosedResourceError from exc.__cause__
         except trio.BrokenResourceError as exc:
             raise BrokenResourceError from exc.__cause__
 
@@ -332,17 +333,17 @@
     async def aclose(self) -> None:
         await self._stream.aclose()
 
 
 @dataclass(eq=False)
 class Process(abc.Process):
     _process: trio.Process
-    _stdin: Optional[abc.ByteSendStream]
-    _stdout: Optional[abc.ByteReceiveStream]
-    _stderr: Optional[abc.ByteReceiveStream]
+    _stdin: abc.ByteSendStream | None
+    _stdout: abc.ByteReceiveStream | None
+    _stderr: abc.ByteReceiveStream | None
 
     async def aclose(self) -> None:
         if self._stdin:
             await self._stdin.aclose()
         if self._stdout:
             await self._stdout.aclose()
         if self._stderr:
@@ -363,43 +364,43 @@
         self._process.send_signal(signal)
 
     @property
     def pid(self) -> int:
         return self._process.pid
 
     @property
-    def returncode(self) -> Optional[int]:
+    def returncode(self) -> int | None:
         return self._process.returncode
 
     @property
-    def stdin(self) -> Optional[abc.ByteSendStream]:
+    def stdin(self) -> abc.ByteSendStream | None:
         return self._stdin
 
     @property
-    def stdout(self) -> Optional[abc.ByteReceiveStream]:
+    def stdout(self) -> abc.ByteReceiveStream | None:
         return self._stdout
 
     @property
-    def stderr(self) -> Optional[abc.ByteReceiveStream]:
+    def stderr(self) -> abc.ByteReceiveStream | None:
         return self._stderr
 
 
 async def open_process(
-    command: Union[str, bytes, Sequence[Union[str, bytes]]],
+    command: str | bytes | Sequence[str | bytes],
     *,
     shell: bool,
-    stdin: Union[int, IO[Any], None],
-    stdout: Union[int, IO[Any], None],
-    stderr: Union[int, IO[Any], None],
-    cwd: Union[str, bytes, PathLike, None] = None,
-    env: Optional[Mapping[str, str]] = None,
+    stdin: int | IO[Any] | None,
+    stdout: int | IO[Any] | None,
+    stderr: int | IO[Any] | None,
+    cwd: str | bytes | PathLike | None = None,
+    env: Mapping[str, str] | None = None,
     start_new_session: bool = False,
 ) -> Process:
-    process = await trio_open_process(
-        command,
+    process = await trio_open_process(  # type: ignore[misc]
+        command,  # type: ignore[arg-type]
         stdin=stdin,
         stdout=stdout,
         stderr=stderr,
         shell=shell,
         cwd=cwd,
         env=env,
         start_new_session=start_new_session,
@@ -416,29 +417,29 @@
 
 
 current_default_worker_process_limiter: RunVar = RunVar(
     "current_default_worker_process_limiter"
 )
 
 
-async def _shutdown_process_pool(workers: Set[Process]) -> None:
+async def _shutdown_process_pool(workers: set[Process]) -> None:
     process: Process
     try:
         await sleep(math.inf)
     except trio.Cancelled:
         for process in workers:
             if process.returncode is None:
                 process.kill()
 
         with CancelScope(shield=True):
             for process in workers:
                 await process.aclose()
 
 
-def setup_process_pool_exit_at_shutdown(workers: Set[Process]) -> None:
+def setup_process_pool_exit_at_shutdown(workers: set[Process]) -> None:
     trio.lowlevel.spawn_system_task(_shutdown_process_pool, workers)
 
 
 #
 # Sockets and networking
 #
 
@@ -459,15 +460,15 @@
         return self._trio_socket._sock  # type: ignore[attr-defined]
 
     async def aclose(self) -> None:
         if self._trio_socket.fileno() >= 0:
             self._closed = True
             self._trio_socket.close()
 
-    def _convert_socket_error(self, exc: BaseException) -> "NoReturn":
+    def _convert_socket_error(self, exc: BaseException) -> NoReturn:
         if isinstance(exc, trio.ClosedResourceError):
             raise ClosedResourceError from exc
         elif self._trio_socket.fileno() < 0 and self._closed:
             raise ClosedResourceError from None
         elif isinstance(exc, OSError):
             raise BrokenResourceError from exc
         else:
@@ -504,15 +505,15 @@
                 view = view[bytes_sent:]
 
     async def send_eof(self) -> None:
         self._trio_socket.shutdown(socket.SHUT_WR)
 
 
 class UNIXSocketStream(SocketStream, abc.UNIXSocketStream):
-    async def receive_fds(self, msglen: int, maxfds: int) -> Tuple[bytes, List[int]]:
+    async def receive_fds(self, msglen: int, maxfds: int) -> tuple[bytes, list[int]]:
         if not isinstance(msglen, int) or msglen < 0:
             raise ValueError("msglen must be a non-negative integer")
         if not isinstance(maxfds, int) or maxfds < 1:
             raise ValueError("maxfds must be a positive integer")
 
         fds = array.array("i")
         await checkpoint()
@@ -537,23 +538,21 @@
                     f"cmsg_level = {cmsg_level}, cmsg_type = {cmsg_type}"
                 )
 
             fds.frombytes(cmsg_data[: len(cmsg_data) - (len(cmsg_data) % fds.itemsize)])
 
         return message, list(fds)
 
-    async def send_fds(
-        self, message: bytes, fds: Collection[Union[int, IOBase]]
-    ) -> None:
+    async def send_fds(self, message: bytes, fds: Collection[int | IOBase]) -> None:
         if not message:
             raise ValueError("message must not be empty")
         if not fds:
             raise ValueError("fds must not be empty")
 
-        filenos: List[int] = []
+        filenos: list[int] = []
         for fd in fds:
             if isinstance(fd, int):
                 filenos.append(fd)
             elif isinstance(fd, IOBase):
                 filenos.append(fd.fileno())
 
         fdarray = array.array("i", filenos)
@@ -609,15 +608,15 @@
 
 class UDPSocket(_TrioSocketMixin[IPSockAddrType], abc.UDPSocket):
     def __init__(self, trio_socket: TrioSocketType) -> None:
         super().__init__(trio_socket)
         self._receive_guard = ResourceGuard("reading from")
         self._send_guard = ResourceGuard("writing to")
 
-    async def receive(self) -> Tuple[bytes, IPSockAddrType]:
+    async def receive(self) -> tuple[bytes, IPSockAddrType]:
         with self._receive_guard:
             try:
                 data, addr = await self._trio_socket.recvfrom(65536)
                 return data, convert_ipv6_sockaddr(addr)
             except BaseException as exc:
                 self._convert_socket_error(exc)
 
@@ -647,15 +646,15 @@
             try:
                 await self._trio_socket.send(item)
             except BaseException as exc:
                 self._convert_socket_error(exc)
 
 
 async def connect_tcp(
-    host: str, port: int, local_address: Optional[IPSockAddrType] = None
+    host: str, port: int, local_address: IPSockAddrType | None = None
 ) -> SocketStream:
     family = socket.AF_INET6 if ":" in host else socket.AF_INET
     trio_socket = trio.socket.socket(family)
     trio_socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
     if local_address:
         await trio_socket.bind(local_address)
 
@@ -677,18 +676,18 @@
         raise
 
     return UNIXSocketStream(trio_socket)
 
 
 async def create_udp_socket(
     family: socket.AddressFamily,
-    local_address: Optional[IPSockAddrType],
-    remote_address: Optional[IPSockAddrType],
+    local_address: IPSockAddrType | None,
+    remote_address: IPSockAddrType | None,
     reuse_port: bool,
-) -> Union[UDPSocket, ConnectedUDPSocket]:
+) -> UDPSocket | ConnectedUDPSocket:
     trio_socket = trio.socket.socket(family=family, type=socket.SOCK_DGRAM)
 
     if reuse_port:
         trio_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
 
     if local_address:
         await trio_socket.bind(local_address)
@@ -724,15 +723,15 @@
 
 #
 # Synchronization
 #
 
 
 class Event(BaseEvent):
-    def __new__(cls) -> "Event":
+    def __new__(cls) -> Event:
         return object.__new__(cls)
 
     def __init__(self) -> None:
         self.__original = trio.Event()
 
     def is_set(self) -> bool:
         return self.__original.is_set()
@@ -746,32 +745,32 @@
 
     def set(self) -> DeprecatedAwaitable:
         self.__original.set()
         return DeprecatedAwaitable(self.set)
 
 
 class CapacityLimiter(BaseCapacityLimiter):
-    def __new__(cls, *args: object, **kwargs: object) -> "CapacityLimiter":
+    def __new__(cls, *args: object, **kwargs: object) -> CapacityLimiter:
         return object.__new__(cls)
 
     def __init__(
-        self, *args: Any, original: Optional[trio.CapacityLimiter] = None
+        self, *args: Any, original: trio.CapacityLimiter | None = None
     ) -> None:
         self.__original = original or trio.CapacityLimiter(*args)
 
     async def __aenter__(self) -> None:
         return await self.__original.__aenter__()
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
-        return await self.__original.__aexit__(exc_type, exc_val, exc_tb)
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        await self.__original.__aexit__(exc_type, exc_val, exc_tb)
 
     @property
     def total_tokens(self) -> float:
         return self.__original.total_tokens
 
     @total_tokens.setter
     def total_tokens(self, value: float) -> None:
@@ -830,33 +829,43 @@
 
 
 #
 # Signal handling
 #
 
 
-class _SignalReceiver(DeprecatedAsyncContextManager[T]):
-    def __init__(self, cm: ContextManager[T]):
-        self._cm = cm
+class _SignalReceiver(DeprecatedAsyncContextManager["_SignalReceiver"]):
+    _iterator: AsyncIterator[int]
+
+    def __init__(self, signals: tuple[Signals, ...]):
+        self._signals = signals
 
-    def __enter__(self) -> T:
-        return self._cm.__enter__()
+    def __enter__(self) -> _SignalReceiver:
+        self._cm = trio.open_signal_receiver(*self._signals)
+        self._iterator = self._cm.__enter__()
+        return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         return self._cm.__exit__(exc_type, exc_val, exc_tb)
 
+    def __aiter__(self) -> _SignalReceiver:
+        return self
+
+    async def __anext__(self) -> Signals:
+        signum = await self._iterator.__anext__()
+        return Signals(signum)
+
 
 def open_signal_receiver(*signals: Signals) -> _SignalReceiver:
-    cm = trio.open_signal_receiver(*signals)
-    return _SignalReceiver(cm)
+    return _SignalReceiver(signals)
 
 
 #
 # Testing and debugging
 #
 
 
@@ -866,20 +875,20 @@
     parent_id = None
     if task.parent_nursery and task.parent_nursery.parent_task:
         parent_id = id(task.parent_nursery.parent_task)
 
     return TaskInfo(id(task), parent_id, task.name, task.coro)
 
 
-def get_running_tasks() -> List[TaskInfo]:
+def get_running_tasks() -> list[TaskInfo]:
     root_task = trio_lowlevel.current_root_task()
     task_infos = [TaskInfo(id(root_task), None, root_task.name, root_task.coro)]
     nurseries = root_task.child_nurseries
     while nurseries:
-        new_nurseries: List[trio.Nursery] = []
+        new_nurseries: list[trio.Nursery] = []
         for nursery in nurseries:
             for task in nursery.child_tasks:
                 task_infos.append(
                     TaskInfo(id(task), id(nursery.parent_task), task.name, task.coro)
                 )
                 new_nurseries.extend(task.child_nurseries)
 
@@ -895,18 +904,18 @@
 
 
 class TestRunner(abc.TestRunner):
     def __init__(self, **options: Any) -> None:
         from collections import deque
         from queue import Queue
 
-        self._call_queue: "Queue[Callable[..., object]]" = Queue()
+        self._call_queue: Queue[Callable[..., object]] = Queue()
         self._result_queue: Deque[Outcome] = deque()
-        self._stop_event: Optional[trio.Event] = None
-        self._nursery: Optional[trio.Nursery] = None
+        self._stop_event: trio.Event | None = None
+        self._nursery: trio.Nursery | None = None
         self._options = options
 
     async def _trio_main(self) -> None:
         self._stop_event = trio.Event()
         async with trio.open_nursery() as self._nursery:
             await self._stop_event.wait()
 
@@ -951,17 +960,17 @@
             self._stop_event.set()
             while self._nursery is not None:
                 self._call_queue.get()()
 
     def run_asyncgen_fixture(
         self,
         fixture_func: Callable[..., AsyncGenerator[T_Retval, Any]],
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
     ) -> Iterable[T_Retval]:
-        async def fixture_runner(*, task_status: "TaskStatus") -> None:
+        async def fixture_runner(*, task_status: TaskStatus[T_Retval]) -> None:
             agen = fixture_func(**kwargs)
             retval = await agen.asend(None)
             task_status.started(retval)
             await teardown_event.wait()
             try:
                 await agen.asend(None)
             except StopAsyncIteration:
@@ -974,15 +983,15 @@
         fixture_value = self._call(lambda: self._get_nursery().start(fixture_runner))
         yield fixture_value
         teardown_event.set()
 
     def run_fixture(
         self,
         fixture_func: Callable[..., Coroutine[Any, Any, T_Retval]],
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
     ) -> T_Retval:
         return self._call(fixture_func, **kwargs)
 
     def run_test(
-        self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: Dict[str, Any]
+        self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: dict[str, Any]
     ) -> None:
         self._call(test_func, **kwargs)
```

### Comparing `anyio-3.6.2/src/anyio/_core/_compat.py` & `anyio-3.7.0rc1/src/anyio/_core/_compat.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,22 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
 from contextlib import AbstractContextManager
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
     Callable,
     ContextManager,
     Generator,
     Generic,
     Iterable,
     List,
-    Optional,
-    Tuple,
-    Type,
     TypeVar,
     Union,
     overload,
 )
 from warnings import warn
 
 if TYPE_CHECKING:
@@ -36,31 +35,31 @@
 
 @overload
 async def maybe_async(__obj: TaskInfo) -> TaskInfo:
     ...
 
 
 @overload
-async def maybe_async(__obj: "DeprecatedAwaitableFloat") -> float:
+async def maybe_async(__obj: DeprecatedAwaitableFloat) -> float:
     ...
 
 
 @overload
-async def maybe_async(__obj: "DeprecatedAwaitableList[T]") -> List[T]:
+async def maybe_async(__obj: DeprecatedAwaitableList[T]) -> list[T]:
     ...
 
 
 @overload
-async def maybe_async(__obj: "DeprecatedAwaitable") -> None:
+async def maybe_async(__obj: DeprecatedAwaitable) -> None:
     ...
 
 
 async def maybe_async(
-    __obj: "AnyDeprecatedAwaitable[T]",
-) -> Union[TaskInfo, float, List[T], None]:
+    __obj: AnyDeprecatedAwaitable[T],
+) -> TaskInfo | float | list[T] | None:
     """
     Await on the given object if necessary.
 
     This function is intended to bridge the gap between AnyIO 2.x and 3.x where some functions and
     methods were converted from coroutine functions into regular functions.
 
     Do **not** try to use this for any other purpose!
@@ -78,23 +77,23 @@
         self._cm = cm
 
     async def __aenter__(self) -> T:
         return self._cm.__enter__()
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         return self._cm.__exit__(exc_type, exc_val, exc_tb)
 
 
 def maybe_async_cm(
-    cm: Union[ContextManager[T], AsyncContextManager[T]]
+    cm: ContextManager[T] | AsyncContextManager[T],
 ) -> AsyncContextManager[T]:
     """
     Wrap a regular context manager as an async one if necessary.
 
     This function is intended to bridge the gap between AnyIO 2.x and 3.x where some functions and
     methods were changed to return regular context managers instead of async ones.
 
@@ -107,112 +106,112 @@
     if not isinstance(cm, AbstractContextManager):
         raise TypeError("Given object is not an context manager")
 
     return _ContextManagerWrapper(cm)
 
 
 def _warn_deprecation(
-    awaitable: "AnyDeprecatedAwaitable[Any]", stacklevel: int = 1
+    awaitable: AnyDeprecatedAwaitable[Any], stacklevel: int = 1
 ) -> None:
     warn(
         f'Awaiting on {awaitable._name}() is deprecated. Use "await '
         f"anyio.maybe_async({awaitable._name}(...)) if you have to support both AnyIO 2.x "
         f'and 3.x, or just remove the "await" if you are completely migrating to AnyIO 3+.',
         DeprecationWarning,
         stacklevel=stacklevel + 1,
     )
 
 
 class DeprecatedAwaitable:
-    def __init__(self, func: Callable[..., "DeprecatedAwaitable"]):
+    def __init__(self, func: Callable[..., DeprecatedAwaitable]):
         self._name = f"{func.__module__}.{func.__qualname__}"
 
     def __await__(self) -> Generator[None, None, None]:
         _warn_deprecation(self)
         if False:
             yield
 
-    def __reduce__(self) -> Tuple[Type[None], Tuple[()]]:
+    def __reduce__(self) -> tuple[type[None], tuple[()]]:
         return type(None), ()
 
     def _unwrap(self) -> None:
         return None
 
 
 class DeprecatedAwaitableFloat(float):
     def __new__(
-        cls, x: float, func: Callable[..., "DeprecatedAwaitableFloat"]
-    ) -> "DeprecatedAwaitableFloat":
+        cls, x: float, func: Callable[..., DeprecatedAwaitableFloat]
+    ) -> DeprecatedAwaitableFloat:
         return super().__new__(cls, x)
 
-    def __init__(self, x: float, func: Callable[..., "DeprecatedAwaitableFloat"]):
+    def __init__(self, x: float, func: Callable[..., DeprecatedAwaitableFloat]):
         self._name = f"{func.__module__}.{func.__qualname__}"
 
     def __await__(self) -> Generator[None, None, float]:
         _warn_deprecation(self)
         if False:
             yield
 
         return float(self)
 
-    def __reduce__(self) -> Tuple[Type[float], Tuple[float]]:
+    def __reduce__(self) -> tuple[type[float], tuple[float]]:
         return float, (float(self),)
 
     def _unwrap(self) -> float:
         return float(self)
 
 
 class DeprecatedAwaitableList(List[T]):
     def __init__(
         self,
         iterable: Iterable[T] = (),
         *,
-        func: Callable[..., "DeprecatedAwaitableList[T]"],
+        func: Callable[..., DeprecatedAwaitableList[T]],
     ):
         super().__init__(iterable)
         self._name = f"{func.__module__}.{func.__qualname__}"
 
-    def __await__(self) -> Generator[None, None, List[T]]:
+    def __await__(self) -> Generator[None, None, list[T]]:
         _warn_deprecation(self)
         if False:
             yield
 
         return list(self)
 
-    def __reduce__(self) -> Tuple[Type[List[T]], Tuple[List[T]]]:
+    def __reduce__(self) -> tuple[type[list[T]], tuple[list[T]]]:
         return list, (list(self),)
 
-    def _unwrap(self) -> List[T]:
+    def _unwrap(self) -> list[T]:
         return list(self)
 
 
 class DeprecatedAsyncContextManager(Generic[T], metaclass=ABCMeta):
     @abstractmethod
     def __enter__(self) -> T:
         pass
 
     @abstractmethod
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         pass
 
     async def __aenter__(self) -> T:
         warn(
             f"Using {self.__class__.__name__} as an async context manager has been deprecated. "
             f'Use "async with anyio.maybe_async_cm(yourcontextmanager) as foo:" if you have to '
             f'support both AnyIO 2.x and 3.x, or just remove the "async" from "async with" if '
             f"you are completely migrating to AnyIO 3+.",
             DeprecationWarning,
         )
         return self.__enter__()
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         return self.__exit__(exc_type, exc_val, exc_tb)
```

### Comparing `anyio-3.6.2/src/anyio/_core/_eventloop.py` & `anyio-3.7.0rc1/src/anyio/_core/_eventloop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
+from __future__ import annotations
+
 import math
 import sys
 import threading
 from contextlib import contextmanager
 from importlib import import_module
 from typing import (
     Any,
+    Awaitable,
     Callable,
-    Coroutine,
-    Dict,
     Generator,
-    Optional,
-    Tuple,
-    Type,
     TypeVar,
 )
 
 import sniffio
 
 # This must be updated when new backends are introduced
 from ._compat import DeprecatedAwaitableFloat
@@ -23,18 +21,18 @@
 BACKENDS = "asyncio", "trio"
 
 T_Retval = TypeVar("T_Retval")
 threadlocals = threading.local()
 
 
 def run(
-    func: Callable[..., Coroutine[Any, Any, T_Retval]],
+    func: Callable[..., Awaitable[T_Retval]],
     *args: object,
     backend: str = "asyncio",
-    backend_options: Optional[Dict[str, Any]] = None,
+    backend_options: dict[str, Any] | None = None,
 ) -> T_Retval:
     """
     Run the given coroutine function in an asynchronous event loop.
 
     The current thread must not be already running an event loop.
 
     :param func: a coroutine function
@@ -115,20 +113,20 @@
 
     :return: the clock value (seconds)
 
     """
     return DeprecatedAwaitableFloat(get_asynclib().current_time(), current_time)
 
 
-def get_all_backends() -> Tuple[str, ...]:
+def get_all_backends() -> tuple[str, ...]:
     """Return a tuple of the names of all built-in backends."""
     return BACKENDS
 
 
-def get_cancelled_exc_class() -> Type[BaseException]:
+def get_cancelled_exc_class() -> type[BaseException]:
     """Return the current async library's cancellation exception class."""
     return get_asynclib().CancelledError
 
 
 #
 # Private API
 #
@@ -140,15 +138,15 @@
     threadlocals.current_async_module = module
     try:
         yield
     finally:
         del threadlocals.current_async_module
 
 
-def get_asynclib(asynclib_name: Optional[str] = None) -> Any:
+def get_asynclib(asynclib_name: str | None = None) -> Any:
     if asynclib_name is None:
         asynclib_name = sniffio.current_async_library()
 
     modulename = "anyio._backends._" + asynclib_name
     try:
         return sys.modules[modulename]
     except KeyError:
```

### Comparing `anyio-3.6.2/src/anyio/_core/_exceptions.py` & `anyio-3.7.0rc1/src/anyio/_core/_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 from traceback import format_exception
-from typing import List
 
 
 class BrokenResourceError(Exception):
     """
     Raised when trying to use a resource that has been rendered unusable due to external causes
     (e.g. a send stream whose peer has disconnected).
     """
@@ -48,15 +49,15 @@
     Raised when multiple exceptions have been raised in a task group.
 
     :var ~typing.Sequence[BaseException] exceptions: the sequence of exceptions raised together
     """
 
     SEPARATOR = "----------------------------\n"
 
-    exceptions: List[BaseException]
+    exceptions: list[BaseException]
 
     def __str__(self) -> str:
         tracebacks = [
             "".join(format_exception(type(exc), exc, exc.__traceback__))
             for exc in self.exceptions
         ]
         return (
```

### Comparing `anyio-3.6.2/src/anyio/_core/_fileio.py` & `anyio-3.7.0rc1/src/anyio/_core/_fileio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import pathlib
 import sys
 from dataclasses import dataclass
 from functools import partial
 from os import PathLike
 from typing import (
@@ -10,19 +12,15 @@
     Any,
     AnyStr,
     AsyncIterator,
     Callable,
     Generic,
     Iterable,
     Iterator,
-    List,
-    Optional,
     Sequence,
-    Tuple,
-    Union,
     cast,
     overload,
 )
 
 from .. import to_thread
 from ..abc import AsyncResource
 
@@ -90,105 +88,103 @@
 
     async def aclose(self) -> None:
         return await to_thread.run_sync(self._fp.close)
 
     async def read(self, size: int = -1) -> AnyStr:
         return await to_thread.run_sync(self._fp.read, size)
 
-    async def read1(self: "AsyncFile[bytes]", size: int = -1) -> bytes:
+    async def read1(self: AsyncFile[bytes], size: int = -1) -> bytes:
         return await to_thread.run_sync(self._fp.read1, size)
 
     async def readline(self) -> AnyStr:
         return await to_thread.run_sync(self._fp.readline)
 
-    async def readlines(self) -> List[AnyStr]:
+    async def readlines(self) -> list[AnyStr]:
         return await to_thread.run_sync(self._fp.readlines)
 
-    async def readinto(self: "AsyncFile[bytes]", b: WriteableBuffer) -> bytes:
+    async def readinto(self: AsyncFile[bytes], b: WriteableBuffer) -> bytes:
         return await to_thread.run_sync(self._fp.readinto, b)
 
-    async def readinto1(self: "AsyncFile[bytes]", b: WriteableBuffer) -> bytes:
+    async def readinto1(self: AsyncFile[bytes], b: WriteableBuffer) -> bytes:
         return await to_thread.run_sync(self._fp.readinto1, b)
 
     @overload
-    async def write(self: "AsyncFile[bytes]", b: ReadableBuffer) -> int:
+    async def write(self: AsyncFile[bytes], b: ReadableBuffer) -> int:
         ...
 
     @overload
-    async def write(self: "AsyncFile[str]", b: str) -> int:
+    async def write(self: AsyncFile[str], b: str) -> int:
         ...
 
-    async def write(self, b: Union[ReadableBuffer, str]) -> int:
+    async def write(self, b: ReadableBuffer | str) -> int:
         return await to_thread.run_sync(self._fp.write, b)
 
     @overload
     async def writelines(
-        self: "AsyncFile[bytes]", lines: Iterable[ReadableBuffer]
+        self: AsyncFile[bytes], lines: Iterable[ReadableBuffer]
     ) -> None:
         ...
 
     @overload
-    async def writelines(self: "AsyncFile[str]", lines: Iterable[str]) -> None:
+    async def writelines(self: AsyncFile[str], lines: Iterable[str]) -> None:
         ...
 
-    async def writelines(
-        self, lines: Union[Iterable[ReadableBuffer], Iterable[str]]
-    ) -> None:
+    async def writelines(self, lines: Iterable[ReadableBuffer] | Iterable[str]) -> None:
         return await to_thread.run_sync(self._fp.writelines, lines)
 
-    async def truncate(self, size: Optional[int] = None) -> int:
+    async def truncate(self, size: int | None = None) -> int:
         return await to_thread.run_sync(self._fp.truncate, size)
 
-    async def seek(self, offset: int, whence: Optional[int] = os.SEEK_SET) -> int:
+    async def seek(self, offset: int, whence: int | None = os.SEEK_SET) -> int:
         return await to_thread.run_sync(self._fp.seek, offset, whence)
 
     async def tell(self) -> int:
         return await to_thread.run_sync(self._fp.tell)
 
     async def flush(self) -> None:
         return await to_thread.run_sync(self._fp.flush)
 
 
 @overload
 async def open_file(
-    file: Union[str, "PathLike[str]", int],
+    file: str | PathLike[str] | int,
     mode: OpenBinaryMode,
     buffering: int = ...,
-    encoding: Optional[str] = ...,
-    errors: Optional[str] = ...,
-    newline: Optional[str] = ...,
+    encoding: str | None = ...,
+    errors: str | None = ...,
+    newline: str | None = ...,
     closefd: bool = ...,
-    opener: Optional[Callable[[str, int], int]] = ...,
+    opener: Callable[[str, int], int] | None = ...,
 ) -> AsyncFile[bytes]:
     ...
 
 
 @overload
 async def open_file(
-    file: Union[str, "PathLike[str]", int],
+    file: str | PathLike[str] | int,
     mode: OpenTextMode = ...,
     buffering: int = ...,
-    encoding: Optional[str] = ...,
-    errors: Optional[str] = ...,
-    newline: Optional[str] = ...,
+    encoding: str | None = ...,
+    errors: str | None = ...,
+    newline: str | None = ...,
     closefd: bool = ...,
-    opener: Optional[Callable[[str, int], int]] = ...,
+    opener: Callable[[str, int], int] | None = ...,
 ) -> AsyncFile[str]:
     ...
 
 
 async def open_file(
-    file: Union[str, "PathLike[str]", int],
+    file: str | PathLike[str] | int,
     mode: str = "r",
     buffering: int = -1,
-    encoding: Optional[str] = None,
-    errors: Optional[str] = None,
-    newline: Optional[str] = None,
+    encoding: str | None = None,
+    errors: str | None = None,
+    newline: str | None = None,
     closefd: bool = True,
-    opener: Optional[Callable[[str, int], int]] = None,
+    opener: Callable[[str, int], int] | None = None,
 ) -> AsyncFile[Any]:
     """
     Open a file asynchronously.
 
     The arguments are exactly the same as for the builtin :func:`open`.
 
     :return: an asynchronous file object
@@ -209,17 +205,17 @@
 
     """
     return AsyncFile(file)
 
 
 @dataclass(eq=False)
 class _PathIterator(AsyncIterator["Path"]):
-    iterator: Iterator["PathLike[str]"]
+    iterator: Iterator[PathLike[str]]
 
-    async def __anext__(self) -> "Path":
+    async def __anext__(self) -> Path:
         nextval = await to_thread.run_sync(next, self.iterator, None, cancellable=True)
         if nextval is None:
             raise StopAsyncIteration from None
 
         return Path(cast("PathLike[str]", nextval))
 
 
@@ -274,15 +270,15 @@
     * :meth:`~pathlib.Path.rglob`
     """
 
     __slots__ = "_path", "__weakref__"
 
     __weakref__: Any
 
-    def __init__(self, *args: Union[str, "PathLike[str]"]) -> None:
+    def __init__(self, *args: str | PathLike[str]) -> None:
         self._path: Final[pathlib.Path] = pathlib.Path(*args)
 
     def __fspath__(self) -> str:
         return self._path.__fspath__()
 
     def __str__(self) -> str:
         return self._path.__str__()
@@ -296,38 +292,38 @@
     def __hash__(self) -> int:
         return self._path.__hash__()
 
     def __eq__(self, other: object) -> bool:
         target = other._path if isinstance(other, Path) else other
         return self._path.__eq__(target)
 
-    def __lt__(self, other: "Path") -> bool:
+    def __lt__(self, other: Path) -> bool:
         target = other._path if isinstance(other, Path) else other
         return self._path.__lt__(target)
 
-    def __le__(self, other: "Path") -> bool:
+    def __le__(self, other: Path) -> bool:
         target = other._path if isinstance(other, Path) else other
         return self._path.__le__(target)
 
-    def __gt__(self, other: "Path") -> bool:
+    def __gt__(self, other: Path) -> bool:
         target = other._path if isinstance(other, Path) else other
         return self._path.__gt__(target)
 
-    def __ge__(self, other: "Path") -> bool:
+    def __ge__(self, other: Path) -> bool:
         target = other._path if isinstance(other, Path) else other
         return self._path.__ge__(target)
 
-    def __truediv__(self, other: Any) -> "Path":
+    def __truediv__(self, other: Any) -> Path:
         return Path(self._path / other)
 
-    def __rtruediv__(self, other: Any) -> "Path":
+    def __rtruediv__(self, other: Any) -> Path:
         return Path(other) / self
 
     @property
-    def parts(self) -> Tuple[str, ...]:
+    def parts(self) -> tuple[str, ...]:
         return self._path.parts
 
     @property
     def drive(self) -> str:
         return self._path.drive
 
     @property
@@ -335,87 +331,87 @@
         return self._path.root
 
     @property
     def anchor(self) -> str:
         return self._path.anchor
 
     @property
-    def parents(self) -> Sequence["Path"]:
+    def parents(self) -> Sequence[Path]:
         return tuple(Path(p) for p in self._path.parents)
 
     @property
-    def parent(self) -> "Path":
+    def parent(self) -> Path:
         return Path(self._path.parent)
 
     @property
     def name(self) -> str:
         return self._path.name
 
     @property
     def suffix(self) -> str:
         return self._path.suffix
 
     @property
-    def suffixes(self) -> List[str]:
+    def suffixes(self) -> list[str]:
         return self._path.suffixes
 
     @property
     def stem(self) -> str:
         return self._path.stem
 
-    async def absolute(self) -> "Path":
+    async def absolute(self) -> Path:
         path = await to_thread.run_sync(self._path.absolute)
         return Path(path)
 
     def as_posix(self) -> str:
         return self._path.as_posix()
 
     def as_uri(self) -> str:
         return self._path.as_uri()
 
     def match(self, path_pattern: str) -> bool:
         return self._path.match(path_pattern)
 
-    def is_relative_to(self, *other: Union[str, "PathLike[str]"]) -> bool:
+    def is_relative_to(self, *other: str | PathLike[str]) -> bool:
         try:
             self.relative_to(*other)
             return True
         except ValueError:
             return False
 
     async def chmod(self, mode: int, *, follow_symlinks: bool = True) -> None:
         func = partial(os.chmod, follow_symlinks=follow_symlinks)
         return await to_thread.run_sync(func, self._path, mode)
 
     @classmethod
-    async def cwd(cls) -> "Path":
+    async def cwd(cls) -> Path:
         path = await to_thread.run_sync(pathlib.Path.cwd)
         return cls(path)
 
     async def exists(self) -> bool:
         return await to_thread.run_sync(self._path.exists, cancellable=True)
 
-    async def expanduser(self) -> "Path":
+    async def expanduser(self) -> Path:
         return Path(await to_thread.run_sync(self._path.expanduser, cancellable=True))
 
-    def glob(self, pattern: str) -> AsyncIterator["Path"]:
+    def glob(self, pattern: str) -> AsyncIterator[Path]:
         gen = self._path.glob(pattern)
         return _PathIterator(gen)
 
     async def group(self) -> str:
         return await to_thread.run_sync(self._path.group, cancellable=True)
 
-    async def hardlink_to(self, target: Union[str, pathlib.Path, "Path"]) -> None:
+    async def hardlink_to(self, target: str | pathlib.Path | Path) -> None:
         if isinstance(target, Path):
             target = target._path
 
         await to_thread.run_sync(os.link, target, self)
 
     @classmethod
-    async def home(cls) -> "Path":
+    async def home(cls) -> Path:
         home_path = await to_thread.run_sync(pathlib.Path.home)
         return cls(home_path)
 
     def is_absolute(self) -> bool:
         return self._path.is_absolute()
 
     async def is_block_device(self) -> bool:
@@ -441,19 +437,19 @@
 
     async def is_socket(self) -> bool:
         return await to_thread.run_sync(self._path.is_socket, cancellable=True)
 
     async def is_symlink(self) -> bool:
         return await to_thread.run_sync(self._path.is_symlink, cancellable=True)
 
-    def iterdir(self) -> AsyncIterator["Path"]:
+    def iterdir(self) -> AsyncIterator[Path]:
         gen = self._path.iterdir()
         return _PathIterator(gen)
 
-    def joinpath(self, *args: Union[str, "PathLike[str]"]) -> "Path":
+    def joinpath(self, *args: str | PathLike[str]) -> Path:
         return Path(self._path.joinpath(*args))
 
     async def lchmod(self, mode: int) -> None:
         await to_thread.run_sync(self._path.lchmod, mode)
 
     async def lstat(self) -> os.stat_result:
         return await to_thread.run_sync(self._path.lstat, cancellable=True)
@@ -464,104 +460,104 @@
         await to_thread.run_sync(self._path.mkdir, mode, parents, exist_ok)
 
     @overload
     async def open(
         self,
         mode: OpenBinaryMode,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> AsyncFile[bytes]:
         ...
 
     @overload
     async def open(
         self,
         mode: OpenTextMode = ...,
         buffering: int = ...,
-        encoding: Optional[str] = ...,
-        errors: Optional[str] = ...,
-        newline: Optional[str] = ...,
+        encoding: str | None = ...,
+        errors: str | None = ...,
+        newline: str | None = ...,
     ) -> AsyncFile[str]:
         ...
 
     async def open(
         self,
         mode: str = "r",
         buffering: int = -1,
-        encoding: Optional[str] = None,
-        errors: Optional[str] = None,
-        newline: Optional[str] = None,
+        encoding: str | None = None,
+        errors: str | None = None,
+        newline: str | None = None,
     ) -> AsyncFile[Any]:
         fp = await to_thread.run_sync(
             self._path.open, mode, buffering, encoding, errors, newline
         )
         return AsyncFile(fp)
 
     async def owner(self) -> str:
         return await to_thread.run_sync(self._path.owner, cancellable=True)
 
     async def read_bytes(self) -> bytes:
         return await to_thread.run_sync(self._path.read_bytes)
 
     async def read_text(
-        self, encoding: Optional[str] = None, errors: Optional[str] = None
+        self, encoding: str | None = None, errors: str | None = None
     ) -> str:
         return await to_thread.run_sync(self._path.read_text, encoding, errors)
 
-    def relative_to(self, *other: Union[str, "PathLike[str]"]) -> "Path":
+    def relative_to(self, *other: str | PathLike[str]) -> Path:
         return Path(self._path.relative_to(*other))
 
-    async def readlink(self) -> "Path":
+    async def readlink(self) -> Path:
         target = await to_thread.run_sync(os.readlink, self._path)
         return Path(cast(str, target))
 
-    async def rename(self, target: Union[str, pathlib.PurePath, "Path"]) -> "Path":
+    async def rename(self, target: str | pathlib.PurePath | Path) -> Path:
         if isinstance(target, Path):
             target = target._path
 
         await to_thread.run_sync(self._path.rename, target)
         return Path(target)
 
-    async def replace(self, target: Union[str, pathlib.PurePath, "Path"]) -> "Path":
+    async def replace(self, target: str | pathlib.PurePath | Path) -> Path:
         if isinstance(target, Path):
             target = target._path
 
         await to_thread.run_sync(self._path.replace, target)
         return Path(target)
 
-    async def resolve(self, strict: bool = False) -> "Path":
+    async def resolve(self, strict: bool = False) -> Path:
         func = partial(self._path.resolve, strict=strict)
         return Path(await to_thread.run_sync(func, cancellable=True))
 
-    def rglob(self, pattern: str) -> AsyncIterator["Path"]:
+    def rglob(self, pattern: str) -> AsyncIterator[Path]:
         gen = self._path.rglob(pattern)
         return _PathIterator(gen)
 
     async def rmdir(self) -> None:
         await to_thread.run_sync(self._path.rmdir)
 
     async def samefile(
-        self, other_path: Union[str, bytes, int, pathlib.Path, "Path"]
+        self, other_path: str | bytes | int | pathlib.Path | Path
     ) -> bool:
         if isinstance(other_path, Path):
             other_path = other_path._path
 
         return await to_thread.run_sync(
             self._path.samefile, other_path, cancellable=True
         )
 
     async def stat(self, *, follow_symlinks: bool = True) -> os.stat_result:
         func = partial(os.stat, follow_symlinks=follow_symlinks)
         return await to_thread.run_sync(func, self._path, cancellable=True)
 
     async def symlink_to(
         self,
-        target: Union[str, pathlib.Path, "Path"],
+        target: str | pathlib.Path | Path,
         target_is_directory: bool = False,
     ) -> None:
         if isinstance(target, Path):
             target = target._path
 
         await to_thread.run_sync(self._path.symlink_to, target, target_is_directory)
 
@@ -571,32 +567,32 @@
     async def unlink(self, missing_ok: bool = False) -> None:
         try:
             await to_thread.run_sync(self._path.unlink)
         except FileNotFoundError:
             if not missing_ok:
                 raise
 
-    def with_name(self, name: str) -> "Path":
+    def with_name(self, name: str) -> Path:
         return Path(self._path.with_name(name))
 
-    def with_stem(self, stem: str) -> "Path":
+    def with_stem(self, stem: str) -> Path:
         return Path(self._path.with_name(stem + self._path.suffix))
 
-    def with_suffix(self, suffix: str) -> "Path":
+    def with_suffix(self, suffix: str) -> Path:
         return Path(self._path.with_suffix(suffix))
 
     async def write_bytes(self, data: bytes) -> int:
         return await to_thread.run_sync(self._path.write_bytes, data)
 
     async def write_text(
         self,
         data: str,
-        encoding: Optional[str] = None,
-        errors: Optional[str] = None,
-        newline: Optional[str] = None,
+        encoding: str | None = None,
+        errors: str | None = None,
+        newline: str | None = None,
     ) -> int:
         # Path.write_text() does not support the "newline" parameter before Python 3.10
         def sync_write_text() -> int:
             with self._path.open(
                 "w", encoding=encoding, errors=errors, newline=newline
             ) as fp:
                 return fp.write(data)
```

### Comparing `anyio-3.6.2/src/anyio/_core/_signals.py` & `anyio-3.7.0rc1/src/anyio/_core/_signals.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import AsyncIterator
 
 from ._compat import DeprecatedAsyncContextManager
 from ._eventloop import get_asynclib
 
 
 def open_signal_receiver(
```

### Comparing `anyio-3.6.2/src/anyio/_core/_sockets.py` & `anyio-3.7.0rc1/src/anyio/_core/_sockets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import socket
 import ssl
 import sys
 from ipaddress import IPv6Address, ip_address
 from os import PathLike, chmod
 from pathlib import Path
 from socket import AddressFamily, SocketKind
-from typing import Awaitable, List, Optional, Tuple, Union, cast, overload
+from typing import Awaitable, List, Tuple, cast, overload
 
 from .. import to_thread
 from ..abc import (
     ConnectedUDPSocket,
     IPAddressType,
     IPSockAddrType,
     SocketListener,
@@ -42,101 +44,102 @@
 
 # tls_hostname given
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
-    local_host: Optional[IPAddressType] = ...,
-    ssl_context: Optional[ssl.SSLContext] = ...,
+    local_host: IPAddressType | None = ...,
+    ssl_context: ssl.SSLContext | None = ...,
     tls_standard_compatible: bool = ...,
     tls_hostname: str,
     happy_eyeballs_delay: float = ...,
 ) -> TLSStream:
     ...
 
 
 # ssl_context given
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
-    local_host: Optional[IPAddressType] = ...,
+    local_host: IPAddressType | None = ...,
     ssl_context: ssl.SSLContext,
     tls_standard_compatible: bool = ...,
-    tls_hostname: Optional[str] = ...,
+    tls_hostname: str | None = ...,
     happy_eyeballs_delay: float = ...,
 ) -> TLSStream:
     ...
 
 
 # tls=True
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
-    local_host: Optional[IPAddressType] = ...,
+    local_host: IPAddressType | None = ...,
     tls: Literal[True],
-    ssl_context: Optional[ssl.SSLContext] = ...,
+    ssl_context: ssl.SSLContext | None = ...,
     tls_standard_compatible: bool = ...,
-    tls_hostname: Optional[str] = ...,
+    tls_hostname: str | None = ...,
     happy_eyeballs_delay: float = ...,
 ) -> TLSStream:
     ...
 
 
 # tls=False
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
-    local_host: Optional[IPAddressType] = ...,
+    local_host: IPAddressType | None = ...,
     tls: Literal[False],
-    ssl_context: Optional[ssl.SSLContext] = ...,
+    ssl_context: ssl.SSLContext | None = ...,
     tls_standard_compatible: bool = ...,
-    tls_hostname: Optional[str] = ...,
+    tls_hostname: str | None = ...,
     happy_eyeballs_delay: float = ...,
 ) -> SocketStream:
     ...
 
 
 # No TLS arguments
 @overload
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
-    local_host: Optional[IPAddressType] = ...,
+    local_host: IPAddressType | None = ...,
     happy_eyeballs_delay: float = ...,
 ) -> SocketStream:
     ...
 
 
 async def connect_tcp(
     remote_host: IPAddressType,
     remote_port: int,
     *,
-    local_host: Optional[IPAddressType] = None,
+    local_host: IPAddressType | None = None,
     tls: bool = False,
-    ssl_context: Optional[ssl.SSLContext] = None,
+    ssl_context: ssl.SSLContext | None = None,
     tls_standard_compatible: bool = True,
-    tls_hostname: Optional[str] = None,
+    tls_hostname: str | None = None,
     happy_eyeballs_delay: float = 0.25,
-) -> Union[SocketStream, TLSStream]:
+) -> SocketStream | TLSStream:
     """
     Connect to a host using the TCP protocol.
 
-    This function implements the stateless version of the Happy Eyeballs algorithm (RFC 6555).
-    If ``address`` is a host name that resolves to multiple IP addresses, each one is tried until
-    one connection attempt succeeds. If the first attempt does not connected within 250
-    milliseconds, a second attempt is started using the next address in the list, and so on.
-    On IPv6 enabled systems, an IPv6 address (if available) is tried first.
+    This function implements the stateless version of the Happy Eyeballs algorithm (RFC
+    6555). If ``remote_host`` is a host name that resolves to multiple IP addresses,
+    each one is tried until one connection attempt succeeds. If the first attempt does
+    not connected within 250 milliseconds, a second attempt is started using the next
+    address in the list, and so on. On IPv6 enabled systems, an IPv6 address (if
+    available) is tried first.
 
     When the connection has been established, a TLS handshake will be done if either
     ``ssl_context`` or ``tls_hostname`` is not ``None``, or if ``tls`` is ``True``.
 
     :param remote_host: the IP address or host name to connect to
     :param remote_port: port on the target host to connect to
     :param local_host: the interface address or name to bind the socket to before connecting
@@ -152,15 +155,15 @@
         of ``remote_host``)
     :param happy_eyeballs_delay: delay (in seconds) before starting the next connection attempt
     :return: a socket stream object if no TLS handshake was done, otherwise a TLS stream
     :raises OSError: if the connection attempt fails
 
     """
     # Placed here due to https://github.com/python/mypy/issues/7057
-    connected_stream: Optional[SocketStream] = None
+    connected_stream: SocketStream | None = None
 
     async def try_connect(remote_host: str, event: Event) -> None:
         nonlocal connected_stream
         try:
             stream = await asynclib.connect_tcp(remote_host, remote_port, local_address)
         except OSError as exc:
             oserrors.append(exc)
@@ -171,15 +174,15 @@
                 tg.cancel_scope.cancel()
             else:
                 await stream.aclose()
         finally:
             event.set()
 
     asynclib = get_asynclib()
-    local_address: Optional[IPSockAddrType] = None
+    local_address: IPSockAddrType | None = None
     family = socket.AF_UNSPEC
     if local_host:
         gai_res = await getaddrinfo(str(local_host), None)
         family, *_, local_address = gai_res[0]
 
     target_host = str(remote_host)
     try:
@@ -189,15 +192,15 @@
         gai_res = await getaddrinfo(
             target_host, remote_port, family=family, type=socket.SOCK_STREAM
         )
 
         # Organize the list so that the first address is an IPv6 address (if available) and the
         # second one is an IPv4 addresses. The rest can be in whatever order.
         v6_found = v4_found = False
-        target_addrs: List[Tuple[socket.AddressFamily, str]] = []
+        target_addrs: list[tuple[socket.AddressFamily, str]] = []
         for af, *rest, sa in gai_res:
             if af == socket.AF_INET6 and not v6_found:
                 v6_found = True
                 target_addrs.insert(0, (af, sa[0]))
             elif af == socket.AF_INET and not v4_found and v6_found:
                 v4_found = True
                 target_addrs.insert(1, (af, sa[0]))
@@ -205,15 +208,15 @@
                 target_addrs.append((af, sa[0]))
     else:
         if isinstance(addr_obj, IPv6Address):
             target_addrs = [(socket.AF_INET6, addr_obj.compressed)]
         else:
             target_addrs = [(socket.AF_INET, addr_obj.compressed)]
 
-    oserrors: List[OSError] = []
+    oserrors: list[OSError] = []
     async with create_task_group() as tg:
         for i, (af, addr) in enumerate(target_addrs):
             event = Event()
             tg.start_soon(try_connect, addr, event)
             with move_on_after(happy_eyeballs_delay):
                 await event.wait()
 
@@ -233,15 +236,15 @@
         except BaseException:
             await aclose_forcefully(connected_stream)
             raise
 
     return connected_stream
 
 
-async def connect_unix(path: Union[str, "PathLike[str]"]) -> UNIXSocketStream:
+async def connect_unix(path: str | PathLike[str]) -> UNIXSocketStream:
     """
     Connect to the given UNIX socket.
 
     Not available on Windows.
 
     :param path: path to the socket
     :return: a socket stream object
@@ -249,50 +252,57 @@
     """
     path = str(Path(path))
     return await get_asynclib().connect_unix(path)
 
 
 async def create_tcp_listener(
     *,
-    local_host: Optional[IPAddressType] = None,
+    local_host: IPAddressType | None = None,
     local_port: int = 0,
     family: AnyIPAddressFamily = socket.AddressFamily.AF_UNSPEC,
     backlog: int = 65536,
     reuse_port: bool = False,
 ) -> MultiListener[SocketStream]:
     """
     Create a TCP socket listener.
 
     :param local_port: port number to listen on
-    :param local_host: IP address of the interface to listen on. If omitted, listen on all IPv4
-        and IPv6 interfaces. To listen on all interfaces on a specific address family, use
-        ``0.0.0.0`` for IPv4 or ``::`` for IPv6.
-    :param family: address family (used if ``interface`` was omitted)
-    :param backlog: maximum number of queued incoming connections (up to a maximum of 2**16, or
-        65536)
-    :param reuse_port: ``True`` to allow multiple sockets to bind to the same address/port
-        (not supported on Windows)
+    :param local_host: IP address of the interface to listen on. If omitted, listen on
+        all IPv4 and IPv6 interfaces. To listen on all interfaces on a specific address
+        family, use ``0.0.0.0`` for IPv4 or ``::`` for IPv6.
+    :param family: address family (used if ``local_host`` was omitted)
+    :param backlog: maximum number of queued incoming connections (up to a maximum of
+        2**16, or 65536)
+    :param reuse_port: ``True`` to allow multiple sockets to bind to the same
+        address/port (not supported on Windows)
     :return: a list of listener objects
 
     """
     asynclib = get_asynclib()
     backlog = min(backlog, 65536)
     local_host = str(local_host) if local_host is not None else None
     gai_res = await getaddrinfo(
         local_host,  # type: ignore[arg-type]
         local_port,
         family=family,
-        type=socket.SOCK_STREAM,
+        type=socket.SocketKind.SOCK_STREAM if sys.platform == "win32" else 0,
         flags=socket.AI_PASSIVE | socket.AI_ADDRCONFIG,
     )
-    listeners: List[SocketListener] = []
+    listeners: list[SocketListener] = []
     try:
         # The set() is here to work around a glibc bug:
         # https://sourceware.org/bugzilla/show_bug.cgi?id=14969
-        for fam, *_, sockaddr in sorted(set(gai_res)):
+        sockaddr: tuple[str, int] | tuple[str, int, int, int]
+        for fam, kind, *_, sockaddr in sorted(set(gai_res)):
+            # Workaround for an uvloop bug where we don't get the correct scope ID for
+            # IPv6 link-local addresses when passing type=socket.SOCK_STREAM to
+            # getaddrinfo(): https://github.com/MagicStack/uvloop/issues/539
+            if sys.platform != "win32" and kind is not SocketKind.SOCK_STREAM:
+                continue
+
             raw_socket = socket.socket(fam)
             raw_socket.setblocking(False)
 
             # For Windows, enable exclusive address use. For others, enable address reuse.
             if sys.platform == "win32":
                 raw_socket.setsockopt(socket.SOL_SOCKET, socket.SO_EXCLUSIVEADDRUSE, 1)
             else:
@@ -301,31 +311,36 @@
             if reuse_port:
                 raw_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
 
             # If only IPv6 was requested, disable dual stack operation
             if fam == socket.AF_INET6:
                 raw_socket.setsockopt(IPPROTO_IPV6, socket.IPV6_V6ONLY, 1)
 
+                # Workaround for #554
+                if "%" in sockaddr[0]:
+                    addr, scope_id = sockaddr[0].split("%", 1)
+                    sockaddr = (addr, sockaddr[1], 0, int(scope_id))
+
             raw_socket.bind(sockaddr)
             raw_socket.listen(backlog)
             listener = asynclib.TCPSocketListener(raw_socket)
             listeners.append(listener)
     except BaseException:
         for listener in listeners:
             await listener.aclose()
 
         raise
 
     return MultiListener(listeners)
 
 
 async def create_unix_listener(
-    path: Union[str, "PathLike[str]"],
+    path: str | PathLike[str],
     *,
-    mode: Optional[int] = None,
+    mode: int | None = None,
     backlog: int = 65536,
 ) -> SocketListener:
     """
     Create a UNIX socket listener.
 
     Not available on Windows.
 
@@ -358,23 +373,23 @@
         raw_socket.close()
         raise
 
 
 async def create_udp_socket(
     family: AnyIPAddressFamily = AddressFamily.AF_UNSPEC,
     *,
-    local_host: Optional[IPAddressType] = None,
+    local_host: IPAddressType | None = None,
     local_port: int = 0,
     reuse_port: bool = False,
 ) -> UDPSocket:
     """
     Create a UDP socket.
 
-    If ``port`` has been given, the socket will be bound to this port on the local machine,
-    making this socket suitable for providing UDP based services.
+    If ``local_port`` has been given, the socket will be bound to this port on the local
+    machine, making this socket suitable for providing UDP based services.
 
     :param family: address family (``AF_INET`` or ``AF_INET6``) – automatically determined from
         ``local_host`` if omitted
     :param local_host: IP address or host name of the local interface to bind to
     :param local_port: local port to bind to
     :param reuse_port: ``True`` to allow multiple sockets to bind to the same address/port
         (not supported on Windows)
@@ -405,15 +420,15 @@
 
 
 async def create_connected_udp_socket(
     remote_host: IPAddressType,
     remote_port: int,
     *,
     family: AnyIPAddressFamily = AddressFamily.AF_UNSPEC,
-    local_host: Optional[IPAddressType] = None,
+    local_host: IPAddressType | None = None,
     local_port: int = 0,
     reuse_port: bool = False,
 ) -> ConnectedUDPSocket:
     """
     Create a connected UDP socket.
 
     Connected UDP sockets can only communicate with the specified remote host/port, and any packets
@@ -450,19 +465,19 @@
 
     return await get_asynclib().create_udp_socket(
         family, local_address, remote_address, reuse_port
     )
 
 
 async def getaddrinfo(
-    host: Union[bytearray, bytes, str],
-    port: Union[str, int, None],
+    host: bytearray | bytes | str,
+    port: str | int | None,
     *,
-    family: Union[int, AddressFamily] = 0,
-    type: Union[int, SocketKind] = 0,
+    family: int | AddressFamily = 0,
+    type: int | SocketKind = 0,
     proto: int = 0,
     flags: int = 0,
 ) -> GetAddrInfoReturnType:
     """
     Look up a numeric IP address given a host name.
 
     Internationalized domain names are translated according to the (non-transitional) IDNA 2008
@@ -498,15 +513,15 @@
     )
     return [
         (family, type, proto, canonname, convert_ipv6_sockaddr(sockaddr))
         for family, type, proto, canonname, sockaddr in gai_res
     ]
 
 
-def getnameinfo(sockaddr: IPSockAddrType, flags: int = 0) -> Awaitable[Tuple[str, str]]:
+def getnameinfo(sockaddr: IPSockAddrType, flags: int = 0) -> Awaitable[tuple[str, str]]:
     """
     Look up the host name of an IP address.
 
     :param sockaddr: socket address (e.g. (ipaddress, port) for IPv4)
     :param flags: flags to pass to upstream ``getnameinfo()``
     :return: a tuple of (host name, service name)
 
@@ -558,16 +573,16 @@
 
 #
 # Private API
 #
 
 
 def convert_ipv6_sockaddr(
-    sockaddr: Union[Tuple[str, int, int, int], Tuple[str, int]]
-) -> Tuple[str, int]:
+    sockaddr: tuple[str, int, int, int] | tuple[str, int]
+) -> tuple[str, int]:
     """
     Convert a 4-tuple IPv6 socket address to a 2-tuple (address, port) format.
 
     If the scope ID is nonzero, it is added to the address, separated with ``%``.
     Otherwise the flow id and scope id are simply cut off from the tuple.
     Any other kinds of socket addresses are returned as-is.
 
@@ -575,13 +590,18 @@
     :return: the converted socket address
 
     """
     # This is more complicated than it should be because of MyPy
     if isinstance(sockaddr, tuple) and len(sockaddr) == 4:
         host, port, flowinfo, scope_id = cast(Tuple[str, int, int, int], sockaddr)
         if scope_id:
+            # PyPy (as of v7.3.11) leaves the interface name in the result, so
+            # we discard it and only get the scope ID from the end
+            # (https://foss.heptapod.net/pypy/pypy/-/issues/3938)
+            host = host.split("%")[0]
+
             # Add scope_id to the address
             return f"{host}%{scope_id}", port
         else:
             return host, port
     else:
         return cast(Tuple[str, int], sockaddr)
```

### Comparing `anyio-3.6.2/src/anyio/_core/_streams.py` & `anyio-3.7.0rc1/src/anyio/_core/_streams.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
+from __future__ import annotations
+
 import math
-from typing import Any, Optional, Tuple, Type, TypeVar, overload
+from typing import Any, TypeVar, overload
 
 from ..streams.memory import (
     MemoryObjectReceiveStream,
     MemoryObjectSendStream,
     MemoryObjectStreamState,
 )
 
 T_Item = TypeVar("T_Item")
 
 
 @overload
 def create_memory_object_stream(
-    max_buffer_size: float, item_type: Type[T_Item]
-) -> Tuple[MemoryObjectSendStream[T_Item], MemoryObjectReceiveStream[T_Item]]:
+    max_buffer_size: float = ...,
+) -> tuple[MemoryObjectSendStream[Any], MemoryObjectReceiveStream[Any]]:
     ...
 
 
 @overload
 def create_memory_object_stream(
-    max_buffer_size: float = 0,
-) -> Tuple[MemoryObjectSendStream[Any], MemoryObjectReceiveStream[Any]]:
+    max_buffer_size: float = ..., item_type: type[T_Item] = ...
+) -> tuple[MemoryObjectSendStream[T_Item], MemoryObjectReceiveStream[T_Item]]:
     ...
 
 
 def create_memory_object_stream(
-    max_buffer_size: float = 0, item_type: Optional[Type[T_Item]] = None
-) -> Tuple[MemoryObjectSendStream[Any], MemoryObjectReceiveStream[Any]]:
+    max_buffer_size: float = 0, item_type: type[T_Item] | None = None
+) -> tuple[MemoryObjectSendStream[Any], MemoryObjectReceiveStream[Any]]:
     """
     Create a memory object stream.
 
     :param max_buffer_size: number of items held in the buffer until ``send()`` starts blocking
     :param item_type: type of item, for marking the streams with the right generic type for
         static typing (not used at run time)
     :return: a tuple of (send stream, receive stream)
```

### Comparing `anyio-3.6.2/src/anyio/_core/_subprocesses.py` & `anyio-3.7.0rc1/src/anyio/_core/_subprocesses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,37 @@
+from __future__ import annotations
+
 from io import BytesIO
 from os import PathLike
 from subprocess import DEVNULL, PIPE, CalledProcessError, CompletedProcess
 from typing import (
     IO,
     Any,
     AsyncIterable,
-    List,
     Mapping,
-    Optional,
     Sequence,
-    Union,
     cast,
 )
 
 from ..abc import Process
 from ._eventloop import get_asynclib
 from ._tasks import create_task_group
 
 
 async def run_process(
-    command: Union[str, bytes, Sequence[Union[str, bytes]]],
+    command: str | bytes | Sequence[str | bytes],
     *,
-    input: Optional[bytes] = None,
-    stdout: Union[int, IO[Any], None] = PIPE,
-    stderr: Union[int, IO[Any], None] = PIPE,
+    input: bytes | None = None,
+    stdout: int | IO[Any] | None = PIPE,
+    stderr: int | IO[Any] | None = PIPE,
     check: bool = True,
-    cwd: Union[str, bytes, "PathLike[str]", None] = None,
-    env: Optional[Mapping[str, str]] = None,
+    cwd: str | bytes | PathLike[str] | None = None,
+    env: Mapping[str, str] | None = None,
     start_new_session: bool = False,
-) -> "CompletedProcess[bytes]":
+) -> CompletedProcess[bytes]:
     """
     Run an external command in a subprocess and wait until it completes.
 
     .. seealso:: :func:`subprocess.run`
 
     :param command: either a string to pass to the shell, or an iterable of strings containing the
         executable name or path and its arguments
@@ -65,15 +64,15 @@
         stdin=PIPE if input else DEVNULL,
         stdout=stdout,
         stderr=stderr,
         cwd=cwd,
         env=env,
         start_new_session=start_new_session,
     ) as process:
-        stream_contents: List[Optional[bytes]] = [None, None]
+        stream_contents: list[bytes | None] = [None, None]
         try:
             async with create_task_group() as tg:
                 if process.stdout:
                     tg.start_soon(drain_stream, process.stdout, 0)
                 if process.stderr:
                     tg.start_soon(drain_stream, process.stderr, 1)
                 if process.stdin and input:
@@ -89,21 +88,21 @@
     if check and process.returncode != 0:
         raise CalledProcessError(cast(int, process.returncode), command, output, errors)
 
     return CompletedProcess(command, cast(int, process.returncode), output, errors)
 
 
 async def open_process(
-    command: Union[str, bytes, Sequence[Union[str, bytes]]],
+    command: str | bytes | Sequence[str | bytes],
     *,
-    stdin: Union[int, IO[Any], None] = PIPE,
-    stdout: Union[int, IO[Any], None] = PIPE,
-    stderr: Union[int, IO[Any], None] = PIPE,
-    cwd: Union[str, bytes, "PathLike[str]", None] = None,
-    env: Optional[Mapping[str, str]] = None,
+    stdin: int | IO[Any] | None = PIPE,
+    stdout: int | IO[Any] | None = PIPE,
+    stderr: int | IO[Any] | None = PIPE,
+    cwd: str | bytes | PathLike[str] | None = None,
+    env: Mapping[str, str] | None = None,
     start_new_session: bool = False,
 ) -> Process:
     """
     Start an external command in a subprocess.
 
     .. seealso:: :class:`subprocess.Popen`
```

### Comparing `anyio-3.6.2/src/anyio/_core/_synchronization.py` & `anyio-3.7.0rc1/src/anyio/_core/_synchronization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 from collections import deque
 from dataclasses import dataclass
 from types import TracebackType
-from typing import Deque, Optional, Tuple, Type
+from typing import Deque
 from warnings import warn
 
 from ..lowlevel import cancel_shielded_checkpoint, checkpoint, checkpoint_if_cancelled
 from ._compat import DeprecatedAwaitable
 from ._eventloop import get_asynclib
 from ._exceptions import BusyResourceError, WouldBlock
 from ._tasks import CancelScope
@@ -30,29 +32,29 @@
         limiter
     :ivar int tasks_waiting: number of tasks waiting on :meth:`~.CapacityLimiter.acquire` or
         :meth:`~.CapacityLimiter.acquire_on_behalf_of`
     """
 
     borrowed_tokens: int
     total_tokens: float
-    borrowers: Tuple[object, ...]
+    borrowers: tuple[object, ...]
     tasks_waiting: int
 
 
 @dataclass(frozen=True)
 class LockStatistics:
     """
     :ivar bool locked: flag indicating if this lock is locked or not
     :ivar ~anyio.TaskInfo owner: task currently holding the lock (or ``None`` if the lock is not
         held by any task)
     :ivar int tasks_waiting: number of tasks waiting on :meth:`~.Lock.acquire`
     """
 
     locked: bool
-    owner: Optional[TaskInfo]
+    owner: TaskInfo | None
     tasks_waiting: int
 
 
 @dataclass(frozen=True)
 class ConditionStatistics:
     """
     :ivar int tasks_waiting: number of tasks blocked on :meth:`~.Condition.wait`
@@ -70,15 +72,15 @@
 
     """
 
     tasks_waiting: int
 
 
 class Event:
-    def __new__(cls) -> "Event":
+    def __new__(cls) -> Event:
         return get_asynclib().Event()
 
     def set(self) -> DeprecatedAwaitable:
         """Set the flag, notifying all listeners."""
         raise NotImplementedError
 
     def is_set(self) -> bool:
@@ -96,27 +98,27 @@
 
     def statistics(self) -> EventStatistics:
         """Return statistics about the current state of this event."""
         raise NotImplementedError
 
 
 class Lock:
-    _owner_task: Optional[TaskInfo] = None
+    _owner_task: TaskInfo | None = None
 
     def __init__(self) -> None:
-        self._waiters: Deque[Tuple[TaskInfo, Event]] = deque()
+        self._waiters: Deque[tuple[TaskInfo, Event]] = deque()
 
     async def __aenter__(self) -> None:
         await self.acquire()
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         self.release()
 
     async def acquire(self) -> None:
         """Acquire the lock."""
         await checkpoint_if_cancelled()
         try:
@@ -183,28 +185,28 @@
 
         .. versionadded:: 3.0
         """
         return LockStatistics(self.locked(), self._owner_task, len(self._waiters))
 
 
 class Condition:
-    _owner_task: Optional[TaskInfo] = None
+    _owner_task: TaskInfo | None = None
 
-    def __init__(self, lock: Optional[Lock] = None):
+    def __init__(self, lock: Lock | None = None):
         self._lock = lock or Lock()
         self._waiters: Deque[Event] = deque()
 
     async def __aenter__(self) -> None:
         await self.acquire()
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         self.release()
 
     def _check_acquired(self) -> None:
         if self._owner_task != get_current_task():
             raise RuntimeError("The current task is not holding the underlying lock")
 
@@ -274,15 +276,15 @@
 
         .. versionadded:: 3.0
         """
         return ConditionStatistics(len(self._waiters), self._lock.statistics())
 
 
 class Semaphore:
-    def __init__(self, initial_value: int, *, max_value: Optional[int] = None):
+    def __init__(self, initial_value: int, *, max_value: int | None = None):
         if not isinstance(initial_value, int):
             raise TypeError("initial_value must be an integer")
         if initial_value < 0:
             raise ValueError("initial_value must be >= 0")
         if max_value is not None:
             if not isinstance(max_value, int):
                 raise TypeError("max_value must be an integer or None")
@@ -291,23 +293,23 @@
                     "max_value must be equal to or higher than initial_value"
                 )
 
         self._value = initial_value
         self._max_value = max_value
         self._waiters: Deque[Event] = deque()
 
-    async def __aenter__(self) -> "Semaphore":
+    async def __aenter__(self) -> Semaphore:
         await self.acquire()
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         self.release()
 
     async def acquire(self) -> None:
         """Decrement the semaphore value, blocking if necessary."""
         await checkpoint_if_cancelled()
         try:
@@ -357,40 +359,40 @@
 
     @property
     def value(self) -> int:
         """The current value of the semaphore."""
         return self._value
 
     @property
-    def max_value(self) -> Optional[int]:
+    def max_value(self) -> int | None:
         """The maximum value of the semaphore."""
         return self._max_value
 
     def statistics(self) -> SemaphoreStatistics:
         """
         Return statistics about the current state of this semaphore.
 
         .. versionadded:: 3.0
         """
         return SemaphoreStatistics(len(self._waiters))
 
 
 class CapacityLimiter:
-    def __new__(cls, total_tokens: float) -> "CapacityLimiter":
+    def __new__(cls, total_tokens: float) -> CapacityLimiter:
         return get_asynclib().CapacityLimiter(total_tokens)
 
     async def __aenter__(self) -> None:
         raise NotImplementedError
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         raise NotImplementedError
 
     @property
     def total_tokens(self) -> float:
         """
         The total number of tokens available for borrowing.
 
@@ -497,15 +499,15 @@
        Use :class:`~Lock` directly.
 
     """
     warn("create_lock() is deprecated -- use Lock() directly", DeprecationWarning)
     return Lock()
 
 
-def create_condition(lock: Optional[Lock] = None) -> Condition:
+def create_condition(lock: Lock | None = None) -> Condition:
     """
     Create an asynchronous condition.
 
     :param lock: the lock to base the condition object on
     :return: a condition object
 
     .. deprecated:: 3.0
@@ -529,15 +531,15 @@
        Use :class:`~Event` directly.
 
     """
     warn("create_event() is deprecated -- use Event() directly", DeprecationWarning)
     return get_asynclib().Event()
 
 
-def create_semaphore(value: int, *, max_value: Optional[int] = None) -> Semaphore:
+def create_semaphore(value: int, *, max_value: int | None = None) -> Semaphore:
     """
     Create an asynchronous semaphore.
 
     :param value: the semaphore's initial value
     :param max_value: if set, makes this a "bounded" semaphore that raises :exc:`ValueError` if the
         semaphore's value would exceed this number
     :return: a semaphore object
@@ -583,13 +585,13 @@
         if self._guarded:
             raise BusyResourceError(self.action)
 
         self._guarded = True
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         self._guarded = False
         return None
```

### Comparing `anyio-3.6.2/src/anyio/_core/_tasks.py` & `anyio-3.7.0rc1/src/anyio/_core/_tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from __future__ import annotations
+
 import math
 from types import TracebackType
-from typing import Optional, Type
 from warnings import warn
 
 from ..abc._tasks import TaskGroup, TaskStatus
 from ._compat import (
     DeprecatedAsyncContextManager,
     DeprecatedAwaitable,
     DeprecatedAwaitableFloat,
 )
 from ._eventloop import get_asynclib
 
 
-class _IgnoredTaskStatus(TaskStatus):
+class _IgnoredTaskStatus(TaskStatus[object]):
     def started(self, value: object = None) -> None:
         pass
 
 
 TASK_STATUS_IGNORED = _IgnoredTaskStatus()
 
 
@@ -26,15 +27,15 @@
 
     :param deadline: The time (clock value) when this scope is cancelled automatically
     :param shield: ``True`` to shield the cancel scope from external cancellation
     """
 
     def __new__(
         cls, *, deadline: float = math.inf, shield: bool = False
-    ) -> "CancelScope":
+    ) -> CancelScope:
         return get_asynclib().CancelScope(shield=shield, deadline=deadline)
 
     def cancel(self) -> DeprecatedAwaitable:
         """Cancel this scope immediately."""
         raise NotImplementedError
 
     @property
@@ -66,23 +67,23 @@
         """
         raise NotImplementedError
 
     @shield.setter
     def shield(self, value: bool) -> None:
         raise NotImplementedError
 
-    def __enter__(self) -> "CancelScope":
+    def __enter__(self) -> CancelScope:
         raise NotImplementedError
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         raise NotImplementedError
 
 
 def open_cancel_scope(*, shield: bool = False) -> CancelScope:
     """
     Open a cancel scope.
 
@@ -105,26 +106,26 @@
         self._cancel_scope = cancel_scope
 
     def __enter__(self) -> CancelScope:
         return self._cancel_scope.__enter__()
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         retval = self._cancel_scope.__exit__(exc_type, exc_val, exc_tb)
         if self._cancel_scope.cancel_called:
             raise TimeoutError
 
         return retval
 
 
-def fail_after(delay: Optional[float], shield: bool = False) -> FailAfterContextManager:
+def fail_after(delay: float | None, shield: bool = False) -> FailAfterContextManager:
     """
     Create a context manager which raises a :class:`TimeoutError` if does not finish in time.
 
     :param delay: maximum allowed time (in seconds) before raising the exception, or ``None`` to
         disable the timeout
     :param shield: ``True`` to shield the cancel scope from external cancellation
     :return: a context manager that yields a cancel scope
@@ -134,15 +135,15 @@
     deadline = (
         (get_asynclib().current_time() + delay) if delay is not None else math.inf
     )
     cancel_scope = get_asynclib().CancelScope(deadline=deadline, shield=shield)
     return FailAfterContextManager(cancel_scope)
 
 
-def move_on_after(delay: Optional[float], shield: bool = False) -> CancelScope:
+def move_on_after(delay: float | None, shield: bool = False) -> CancelScope:
     """
     Create a cancel scope with a deadline that expires after the given delay.
 
     :param delay: maximum allowed time (in seconds) before exiting the context block, or ``None``
         to disable the timeout
     :param shield: ``True`` to shield the cancel scope from external cancellation
     :return: a cancel scope
@@ -154,25 +155,26 @@
     return get_asynclib().CancelScope(deadline=deadline, shield=shield)
 
 
 def current_effective_deadline() -> DeprecatedAwaitableFloat:
     """
     Return the nearest deadline among all the cancel scopes effective for the current task.
 
-    :return: a clock value from the event loop's internal clock (``float('inf')`` if there is no
-        deadline in effect)
+    :return: a clock value from the event loop's internal clock (or ``float('inf')`` if
+        there is no deadline in effect, or ``float('-inf')`` if the current scope has
+        been cancelled)
     :rtype: float
 
     """
     return DeprecatedAwaitableFloat(
         get_asynclib().current_effective_deadline(), current_effective_deadline
     )
 
 
-def create_task_group() -> "TaskGroup":
+def create_task_group() -> TaskGroup:
     """
     Create a task group.
 
     :return: a task group
 
     """
     return get_asynclib().TaskGroup()
```

### Comparing `anyio-3.6.2/src/anyio/_core/_testing.py` & `anyio-3.7.0rc1/src/anyio/_core/_testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Awaitable, Generator, Optional, Union
+from __future__ import annotations
+
+from typing import Any, Awaitable, Generator
 
 from ._compat import DeprecatedAwaitableList, _warn_deprecation
 from ._eventloop import get_asynclib
 
 
 class TaskInfo:
     """
@@ -16,45 +18,45 @@
     """
 
     __slots__ = "_name", "id", "parent_id", "name", "coro"
 
     def __init__(
         self,
         id: int,
-        parent_id: Optional[int],
-        name: Optional[str],
-        coro: Union[Generator, Awaitable[Any]],
+        parent_id: int | None,
+        name: str | None,
+        coro: Generator[Any, Any, Any] | Awaitable[Any],
     ):
         func = get_current_task
         self._name = f"{func.__module__}.{func.__qualname__}"
         self.id: int = id
-        self.parent_id: Optional[int] = parent_id
-        self.name: Optional[str] = name
-        self.coro: Union[Generator, Awaitable[Any]] = coro
+        self.parent_id: int | None = parent_id
+        self.name: str | None = name
+        self.coro: Generator[Any, Any, Any] | Awaitable[Any] = coro
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, TaskInfo):
             return self.id == other.id
 
         return NotImplemented
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id!r}, name={self.name!r})"
 
-    def __await__(self) -> Generator[None, None, "TaskInfo"]:
+    def __await__(self) -> Generator[None, None, TaskInfo]:
         _warn_deprecation(self)
         if False:
             yield
 
         return self
 
-    def _unwrap(self) -> "TaskInfo":
+    def _unwrap(self) -> TaskInfo:
         return self
 
 
 def get_current_task() -> TaskInfo:
     """
     Return the current task.
```

### Comparing `anyio-3.6.2/src/anyio/_core/_typedattr.py` & `anyio-3.7.0rc1/src/anyio/_core/_typedattr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import sys
-from typing import Any, Callable, Dict, Mapping, TypeVar, Union, overload
+from typing import Any, Callable, Mapping, TypeVar, overload
 
 from ._exceptions import TypedAttributeLookupError
 
 if sys.version_info >= (3, 8):
     from typing import final
 else:
     from typing_extensions import final
@@ -22,15 +24,15 @@
     """
     Superclass for typed attribute collections.
 
     Checks that every public attribute of every subclass has a type annotation.
     """
 
     def __init_subclass__(cls) -> None:
-        annotations: Dict[str, Any] = getattr(cls, "__annotations__", {})
+        annotations: dict[str, Any] = getattr(cls, "__annotations__", {})
         for attrname in dir(cls):
             if not attrname.startswith("_") and attrname not in annotations:
                 raise TypeError(
                     f"Attribute {attrname!r} is missing its type annotation"
                 )
 
         super().__init_subclass__()
@@ -52,15 +54,15 @@
         return {}
 
     @overload
     def extra(self, attribute: T_Attr) -> T_Attr:
         ...
 
     @overload
-    def extra(self, attribute: T_Attr, default: T_Default) -> Union[T_Attr, T_Default]:
+    def extra(self, attribute: T_Attr, default: T_Default) -> T_Attr | T_Default:
         ...
 
     @final
     def extra(self, attribute: Any, default: object = undefined) -> object:
         """
         extra(attribute, default=undefined)
```

### Comparing `anyio-3.6.2/src/anyio/abc/__init__.py` & `anyio-3.7.0rc1/src/anyio/abc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = (
     "AsyncResource",
     "IPAddressType",
     "IPSockAddrType",
     "SocketAttribute",
     "SocketStream",
     "SocketListener",
```

### Comparing `anyio-3.6.2/src/anyio/abc/_resources.py` & `anyio-3.7.0rc1/src/anyio/abc/_resources.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
 from types import TracebackType
-from typing import Optional, Type, TypeVar
+from typing import TypeVar
 
 T = TypeVar("T")
 
 
 class AsyncResource(metaclass=ABCMeta):
     """
     Abstract base class for all closeable asynchronous resources.
@@ -14,16 +16,16 @@
     """
 
     async def __aenter__(self: T) -> T:
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         await self.aclose()
 
     @abstractmethod
     async def aclose(self) -> None:
         """Close the resource."""
```

### Comparing `anyio-3.6.2/src/anyio/abc/_sockets.py` & `anyio-3.7.0rc1/src/anyio/abc/_sockets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,41 @@
+from __future__ import annotations
+
 import socket
 from abc import abstractmethod
+from contextlib import AsyncExitStack
 from io import IOBase
 from ipaddress import IPv4Address, IPv6Address
 from socket import AddressFamily
-from types import TracebackType
 from typing import (
     Any,
-    AsyncContextManager,
     Callable,
     Collection,
-    Dict,
-    List,
     Mapping,
-    Optional,
     Tuple,
-    Type,
     TypeVar,
     Union,
 )
 
+from .._core._tasks import create_task_group
 from .._core._typedattr import (
     TypedAttributeProvider,
     TypedAttributeSet,
     typed_attribute,
 )
-from ._streams import ByteStream, Listener, T_Stream, UnreliableObjectStream
+from ._streams import ByteStream, Listener, UnreliableObjectStream
 from ._tasks import TaskGroup
 
 IPAddressType = Union[str, IPv4Address, IPv6Address]
 IPSockAddrType = Tuple[str, int]
 SockAddrType = Union[IPSockAddrType, str]
 UDPPacketType = Tuple[bytes, IPSockAddrType]
 T_Retval = TypeVar("T_Retval")
 
 
-class _NullAsyncContextManager:
-    async def __aenter__(self) -> None:
-        pass
-
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
-        return None
-
-
 class SocketAttribute(TypedAttributeSet):
     #: the address family of the underlying socket
     family: AddressFamily = typed_attribute()
     #: the local socket address of the underlying socket
     local_address: SockAddrType = typed_attribute()
     #: for IP addresses, the local port the underlying socket is bound to
     local_port: int = typed_attribute()
@@ -63,25 +48,23 @@
 
 
 class _SocketProvider(TypedAttributeProvider):
     @property
     def extra_attributes(self) -> Mapping[Any, Callable[[], Any]]:
         from .._core._sockets import convert_ipv6_sockaddr as convert
 
-        attributes: Dict[Any, Callable[[], Any]] = {
+        attributes: dict[Any, Callable[[], Any]] = {
             SocketAttribute.family: lambda: self._raw_socket.family,
             SocketAttribute.local_address: lambda: convert(
                 self._raw_socket.getsockname()
             ),
             SocketAttribute.raw_socket: lambda: self._raw_socket,
         }
         try:
-            peername: Optional[Tuple[str, int]] = convert(
-                self._raw_socket.getpeername()
-            )
+            peername: tuple[str, int] | None = convert(self._raw_socket.getpeername())
         except OSError:
             peername = None
 
         # Provide the remote address for connected sockets
         if peername is not None:
             attributes[SocketAttribute.remote_address] = lambda: peername
 
@@ -108,27 +91,25 @@
 
     Supports all relevant extra attributes from :class:`~SocketAttribute`.
     """
 
 
 class UNIXSocketStream(SocketStream):
     @abstractmethod
-    async def send_fds(
-        self, message: bytes, fds: Collection[Union[int, IOBase]]
-    ) -> None:
+    async def send_fds(self, message: bytes, fds: Collection[int | IOBase]) -> None:
         """
         Send file descriptors along with a message to the peer.
 
         :param message: a non-empty bytestring
         :param fds: a collection of files (either numeric file descriptors or open file or socket
             objects)
         """
 
     @abstractmethod
-    async def receive_fds(self, msglen: int, maxfds: int) -> Tuple[bytes, List[int]]:
+    async def receive_fds(self, msglen: int, maxfds: int) -> tuple[bytes, list[int]]:
         """
         Receive file descriptors along with a message from the peer.
 
         :param msglen: length of the message to expect from the peer
         :param maxfds: maximum number of file descriptors to expect from the peer
         :return: a tuple of (message, file descriptors)
         """
@@ -142,26 +123,22 @@
     """
 
     @abstractmethod
     async def accept(self) -> SocketStream:
         """Accept an incoming connection."""
 
     async def serve(
-        self, handler: Callable[[T_Stream], Any], task_group: Optional[TaskGroup] = None
+        self,
+        handler: Callable[[SocketStream], Any],
+        task_group: TaskGroup | None = None,
     ) -> None:
-        from .. import create_task_group
-
-        context_manager: AsyncContextManager
-        if task_group is None:
-            task_group = context_manager = create_task_group()
-        else:
-            # Can be replaced with AsyncExitStack once on py3.7+
-            context_manager = _NullAsyncContextManager()
+        async with AsyncExitStack() as exit_stack:
+            if task_group is None:
+                task_group = await exit_stack.enter_async_context(create_task_group())
 
-        async with context_manager:
             while True:
                 stream = await self.accept()
                 task_group.start_soon(handler, stream)
 
 
 class UDPSocket(UnreliableObjectStream[UDPPacketType], _SocketProvider):
     """
```

### Comparing `anyio-3.6.2/src/anyio/abc/_streams.py` & `anyio-3.7.0rc1/src/anyio/abc/_streams.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,69 @@
+from __future__ import annotations
+
 from abc import abstractmethod
-from typing import Any, Callable, Generic, Optional, TypeVar, Union
+from typing import Any, Callable, Generic, TypeVar, Union
 
 from .._core._exceptions import EndOfStream
 from .._core._typedattr import TypedAttributeProvider
 from ._resources import AsyncResource
 from ._tasks import TaskGroup
 
 T_Item = TypeVar("T_Item")
-T_Stream = TypeVar("T_Stream")
+T_co = TypeVar("T_co", covariant=True)
+T_contra = TypeVar("T_contra", contravariant=True)
 
 
 class UnreliableObjectReceiveStream(
-    Generic[T_Item], AsyncResource, TypedAttributeProvider
+    Generic[T_co], AsyncResource, TypedAttributeProvider
 ):
     """
     An interface for receiving objects.
 
     This interface makes no guarantees that the received messages arrive in the order in which they
     were sent, or that no messages are missed.
 
     Asynchronously iterating over objects of this type will yield objects matching the given type
     parameter.
     """
 
-    def __aiter__(self) -> "UnreliableObjectReceiveStream[T_Item]":
+    def __aiter__(self) -> UnreliableObjectReceiveStream[T_co]:
         return self
 
-    async def __anext__(self) -> T_Item:
+    async def __anext__(self) -> T_co:
         try:
             return await self.receive()
         except EndOfStream:
             raise StopAsyncIteration
 
     @abstractmethod
-    async def receive(self) -> T_Item:
+    async def receive(self) -> T_co:
         """
         Receive the next item.
 
         :raises ~anyio.ClosedResourceError: if the receive stream has been explicitly
             closed
         :raises ~anyio.EndOfStream: if this stream has been closed from the other end
         :raises ~anyio.BrokenResourceError: if this stream has been rendered unusable
             due to external causes
         """
 
 
 class UnreliableObjectSendStream(
-    Generic[T_Item], AsyncResource, TypedAttributeProvider
+    Generic[T_contra], AsyncResource, TypedAttributeProvider
 ):
     """
     An interface for sending objects.
 
     This interface makes no guarantees that the messages sent will reach the recipient(s) in the
     same order in which they were sent, or at all.
     """
 
     @abstractmethod
-    async def send(self, item: T_Item) -> None:
+    async def send(self, item: T_contra) -> None:
         """
         Send an item to the peer(s).
 
         :param item: the item to send
         :raises ~anyio.ClosedResourceError: if the send stream has been explicitly
             closed
         :raises ~anyio.BrokenResourceError: if this stream has been rendered unusable
@@ -73,22 +76,22 @@
 ):
     """
     A bidirectional message stream which does not guarantee the order or reliability of message
     delivery.
     """
 
 
-class ObjectReceiveStream(UnreliableObjectReceiveStream[T_Item]):
+class ObjectReceiveStream(UnreliableObjectReceiveStream[T_co]):
     """
     A receive message stream which guarantees that messages are received in the same order in
     which they were sent, and that no messages are missed.
     """
 
 
-class ObjectSendStream(UnreliableObjectSendStream[T_Item]):
+class ObjectSendStream(UnreliableObjectSendStream[T_contra]):
     """
     A send message stream which guarantees that messages are delivered in the same order in which
     they were sent, without missing any messages in the middle.
     """
 
 
 class ObjectStream(
@@ -114,15 +117,15 @@
     """
     An interface for receiving bytes from a single peer.
 
     Iterating this byte stream will yield a byte string of arbitrary length, but no more than
     65536 bytes.
     """
 
-    def __aiter__(self) -> "ByteReceiveStream":
+    def __aiter__(self) -> ByteReceiveStream:
         return self
 
     async def __anext__(self) -> bytes:
         try:
             return await self.receive()
         except EndOfStream:
             raise StopAsyncIteration
@@ -178,20 +181,22 @@
 AnyByteReceiveStream = Union[ObjectReceiveStream[bytes], ByteReceiveStream]
 #: Type alias for all bytes-oriented send streams.
 AnyByteSendStream = Union[ObjectSendStream[bytes], ByteSendStream]
 #: Type alias for all bytes-oriented streams.
 AnyByteStream = Union[ObjectStream[bytes], ByteStream]
 
 
-class Listener(Generic[T_Stream], AsyncResource, TypedAttributeProvider):
+class Listener(Generic[T_co], AsyncResource, TypedAttributeProvider):
     """An interface for objects that let you accept incoming connections."""
 
     @abstractmethod
     async def serve(
-        self, handler: Callable[[T_Stream], Any], task_group: Optional[TaskGroup] = None
+        self,
+        handler: Callable[[T_co], Any],
+        task_group: TaskGroup | None = None,
     ) -> None:
         """
         Accept incoming connections as they come in and start tasks to handle them.
 
         :param handler: a callable that will be used to handle each accepted connection
         :param task_group: the task group that will be used to start tasks for handling each
             accepted connection (if omitted, an ad-hoc task group will be created)
```

### Comparing `anyio-3.6.2/src/anyio/abc/_subprocesses.py` & `anyio-3.7.0rc1/src/anyio/abc/_subprocesses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 from signal import Signals
-from typing import Optional
 
 from ._resources import AsyncResource
 from ._streams import ByteReceiveStream, ByteSendStream
 
 
 class Process(AsyncResource):
     """An asynchronous version of :class:`subprocess.Popen`."""
@@ -52,27 +53,27 @@
     @property
     @abstractmethod
     def pid(self) -> int:
         """The process ID of the process."""
 
     @property
     @abstractmethod
-    def returncode(self) -> Optional[int]:
+    def returncode(self) -> int | None:
         """
         The return code of the process. If the process has not yet terminated, this will be
         ``None``.
         """
 
     @property
     @abstractmethod
-    def stdin(self) -> Optional[ByteSendStream]:
+    def stdin(self) -> ByteSendStream | None:
         """The stream for the standard input of the process."""
 
     @property
     @abstractmethod
-    def stdout(self) -> Optional[ByteReceiveStream]:
+    def stdout(self) -> ByteReceiveStream | None:
         """The stream for the standard output of the process."""
 
     @property
     @abstractmethod
-    def stderr(self) -> Optional[ByteReceiveStream]:
+    def stderr(self) -> ByteReceiveStream | None:
         """The stream for the standard error output of the process."""
```

### Comparing `anyio-3.6.2/src/anyio/abc/_tasks.py` & `anyio-3.7.0rc1/src/anyio/abc/_tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,37 @@
-import typing
+from __future__ import annotations
+
+import sys
 from abc import ABCMeta, abstractmethod
 from types import TracebackType
-from typing import Any, Callable, Coroutine, Optional, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, TypeVar, overload
 from warnings import warn
 
-if typing.TYPE_CHECKING:
+if sys.version_info >= (3, 8):
+    from typing import Protocol
+else:
+    from typing_extensions import Protocol
+
+if TYPE_CHECKING:
     from anyio._core._tasks import CancelScope
 
 T_Retval = TypeVar("T_Retval")
+T_contra = TypeVar("T_contra", contravariant=True)
 
 
-class TaskStatus(metaclass=ABCMeta):
-    @abstractmethod
-    def started(self, value: object = None) -> None:
+class TaskStatus(Protocol[T_contra]):
+    @overload
+    def started(self: TaskStatus[None]) -> None:
+        ...
+
+    @overload
+    def started(self, value: T_contra) -> None:
+        ...
+
+    def started(self, value: T_contra | None = None) -> None:
         """
         Signal that the task has started.
 
         :param value: object passed back to the starter of the task
         """
 
 
@@ -24,21 +39,21 @@
     """
     Groups several asynchronous tasks together.
 
     :ivar cancel_scope: the cancel scope inherited by all child tasks
     :vartype cancel_scope: CancelScope
     """
 
-    cancel_scope: "CancelScope"
+    cancel_scope: CancelScope
 
     async def spawn(
         self,
-        func: Callable[..., Coroutine[Any, Any, Any]],
+        func: Callable[..., Awaitable[Any]],
         *args: object,
-        name: object = None
+        name: object = None,
     ) -> None:
         """
         Start a new task in this task group.
 
         :param func: a coroutine function
         :param args: positional arguments to call the function with
         :param name: name of the task, for the purposes of introspection and debugging
@@ -53,52 +68,52 @@
             DeprecationWarning,
         )
         self.start_soon(func, *args, name=name)
 
     @abstractmethod
     def start_soon(
         self,
-        func: Callable[..., Coroutine[Any, Any, Any]],
+        func: Callable[..., Awaitable[Any]],
         *args: object,
-        name: object = None
+        name: object = None,
     ) -> None:
         """
         Start a new task in this task group.
 
         :param func: a coroutine function
         :param args: positional arguments to call the function with
         :param name: name of the task, for the purposes of introspection and debugging
 
         .. versionadded:: 3.0
         """
 
     @abstractmethod
     async def start(
         self,
-        func: Callable[..., Coroutine[Any, Any, Any]],
+        func: Callable[..., Awaitable[Any]],
         *args: object,
-        name: object = None
-    ) -> object:
+        name: object = None,
+    ) -> Any:
         """
         Start a new task and wait until it signals for readiness.
 
         :param func: a coroutine function
         :param args: positional arguments to call the function with
         :param name: name of the task, for the purposes of introspection and debugging
         :return: the value passed to ``task_status.started()``
         :raises RuntimeError: if the task finishes without calling ``task_status.started()``
 
         .. versionadded:: 3.0
         """
 
     @abstractmethod
-    async def __aenter__(self) -> "TaskGroup":
+    async def __aenter__(self) -> TaskGroup:
         """Enter the task group context and allow starting new tasks."""
 
     @abstractmethod
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         """Exit the task group context waiting for all tasks to finish."""
```

### Comparing `anyio-3.6.2/src/anyio/abc/_testing.py` & `anyio-3.7.0rc1/src/anyio/abc/_testing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,70 @@
+from __future__ import annotations
+
 import types
 from abc import ABCMeta, abstractmethod
 from collections.abc import AsyncGenerator, Iterable
-from typing import Any, Callable, Coroutine, Dict, Optional, Type, TypeVar
+from typing import Any, Callable, Coroutine, TypeVar
 
 _T = TypeVar("_T")
 
 
 class TestRunner(metaclass=ABCMeta):
     """
     Encapsulates a running event loop. Every call made through this object will use the same event
     loop.
     """
 
-    def __enter__(self) -> "TestRunner":
+    def __enter__(self) -> TestRunner:
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[types.TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: types.TracebackType | None,
+    ) -> bool | None:
         self.close()
         return None
 
     @abstractmethod
     def close(self) -> None:
         """Close the event loop."""
 
     @abstractmethod
     def run_asyncgen_fixture(
         self,
-        fixture_func: Callable[..., "AsyncGenerator[_T, Any]"],
-        kwargs: Dict[str, Any],
-    ) -> "Iterable[_T]":
+        fixture_func: Callable[..., AsyncGenerator[_T, Any]],
+        kwargs: dict[str, Any],
+    ) -> Iterable[_T]:
         """
         Run an async generator fixture.
 
         :param fixture_func: the fixture function
         :param kwargs: keyword arguments to call the fixture function with
         :return: an iterator yielding the value yielded from the async generator
         """
 
     @abstractmethod
     def run_fixture(
         self,
         fixture_func: Callable[..., Coroutine[Any, Any, _T]],
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
     ) -> _T:
         """
         Run an async fixture.
 
         :param fixture_func: the fixture function
         :param kwargs: keyword arguments to call the fixture function with
         :return: the return value of the fixture function
         """
 
     @abstractmethod
     def run_test(
-        self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: Dict[str, Any]
+        self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: dict[str, Any]
     ) -> None:
         """
         Run an async test function.
 
         :param test_func: the test function
         :param kwargs: keyword arguments to call the test function with
         """
```

### Comparing `anyio-3.6.2/src/anyio/from_thread.py` & `anyio-3.7.0rc1/src/anyio/from_thread.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
+from __future__ import annotations
+
 import threading
 from asyncio import iscoroutine
 from concurrent.futures import FIRST_COMPLETED, Future, ThreadPoolExecutor, wait
 from contextlib import AbstractContextManager, contextmanager
 from types import TracebackType
 from typing import (
     Any,
     AsyncContextManager,
+    Awaitable,
     Callable,
     ContextManager,
-    Coroutine,
-    Dict,
     Generator,
+    Generic,
     Iterable,
-    Optional,
-    Tuple,
-    Type,
     TypeVar,
-    Union,
     cast,
     overload,
 )
 from warnings import warn
 
 from ._core import _eventloop
 from ._core._eventloop import get_asynclib, get_cancelled_exc_class, threadlocals
@@ -28,15 +26,15 @@
 from ._core._tasks import CancelScope, create_task_group
 from .abc._tasks import TaskStatus
 
 T_Retval = TypeVar("T_Retval")
 T_co = TypeVar("T_co")
 
 
-def run(func: Callable[..., Coroutine[Any, Any, T_Retval]], *args: object) -> T_Retval:
+def run(func: Callable[..., Awaitable[T_Retval]], *args: object) -> T_Retval:
     """
     Call a coroutine function from a worker thread.
 
     :param func: a coroutine function
     :param args: positional arguments for the callable
     :return: the return value of the coroutine function
 
@@ -46,15 +44,15 @@
     except AttributeError:
         raise RuntimeError("This function can only be run from an AnyIO worker thread")
 
     return asynclib.run_async_from_thread(func, *args)
 
 
 def run_async_from_thread(
-    func: Callable[..., Coroutine[Any, Any, T_Retval]], *args: object
+    func: Callable[..., Awaitable[T_Retval]], *args: object
 ) -> T_Retval:
     warn(
         "run_async_from_thread() has been deprecated, use anyio.from_thread.run() instead",
         DeprecationWarning,
     )
     return run(func, *args)
 
@@ -80,27 +78,27 @@
     warn(
         "run_sync_from_thread() has been deprecated, use anyio.from_thread.run_sync() instead",
         DeprecationWarning,
     )
     return run_sync(func, *args)
 
 
-class _BlockingAsyncContextManager(AbstractContextManager):
+class _BlockingAsyncContextManager(Generic[T_co], AbstractContextManager):
     _enter_future: Future
     _exit_future: Future
     _exit_event: Event
-    _exit_exc_info: Tuple[
-        Optional[Type[BaseException]], Optional[BaseException], Optional[TracebackType]
+    _exit_exc_info: tuple[
+        type[BaseException] | None, BaseException | None, TracebackType | None
     ] = (None, None, None)
 
-    def __init__(self, async_cm: AsyncContextManager[T_co], portal: "BlockingPortal"):
+    def __init__(self, async_cm: AsyncContextManager[T_co], portal: BlockingPortal):
         self._async_cm = async_cm
         self._portal = portal
 
-    async def run_async_cm(self) -> Optional[bool]:
+    async def run_async_cm(self) -> bool | None:
         try:
             self._exit_event = Event()
             value = await self._async_cm.__aenter__()
         except BaseException as exc:
             self._enter_future.set_exception(exc)
             raise
         else:
@@ -123,18 +121,18 @@
         self._enter_future = Future()
         self._exit_future = self._portal.start_task_soon(self.run_async_cm)
         cm = self._enter_future.result()
         return cast(T_co, cm)
 
     def __exit__(
         self,
-        __exc_type: Optional[Type[BaseException]],
-        __exc_value: Optional[BaseException],
-        __traceback: Optional[TracebackType],
-    ) -> Optional[bool]:
+        __exc_type: type[BaseException] | None,
+        __exc_value: BaseException | None,
+        __traceback: TracebackType | None,
+    ) -> bool | None:
         self._exit_exc_info = __exc_type, __exc_value, __traceback
         self._portal.call(self._exit_event.set)
         return self._exit_future.result()
 
 
 class _BlockingPortalTaskStatus(TaskStatus):
     def __init__(self, future: Future):
@@ -143,33 +141,33 @@
     def started(self, value: object = None) -> None:
         self._future.set_result(value)
 
 
 class BlockingPortal:
     """An object that lets external threads run code in an asynchronous event loop."""
 
-    def __new__(cls) -> "BlockingPortal":
+    def __new__(cls) -> BlockingPortal:
         return get_asynclib().BlockingPortal()
 
     def __init__(self) -> None:
-        self._event_loop_thread_id: Optional[int] = threading.get_ident()
+        self._event_loop_thread_id: int | None = threading.get_ident()
         self._stop_event = Event()
         self._task_group = create_task_group()
         self._cancelled_exc_class = get_cancelled_exc_class()
 
-    async def __aenter__(self) -> "BlockingPortal":
+    async def __aenter__(self) -> BlockingPortal:
         await self._task_group.__aenter__()
         return self
 
     async def __aexit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         await self.stop()
         return await self._task_group.__aexit__(exc_type, exc_val, exc_tb)
 
     def _check_running(self) -> None:
         if self._event_loop_thread_id is None:
             raise RuntimeError("This portal is not running")
         if self._event_loop_thread_id == threading.get_ident():
@@ -194,15 +192,15 @@
         """
         self._event_loop_thread_id = None
         self._stop_event.set()
         if cancel_remaining:
             self._task_group.cancel_scope.cancel()
 
     async def _call_func(
-        self, func: Callable, args: tuple, kwargs: Dict[str, Any], future: Future
+        self, func: Callable, args: tuple, kwargs: dict[str, Any], future: Future
     ) -> None:
         def callback(f: Future) -> None:
             if f.cancelled() and self._event_loop_thread_id not in (
                 None,
                 threading.get_ident(),
             ):
                 self.call(scope.cancel)
@@ -232,15 +230,15 @@
         finally:
             scope = None  # type: ignore[assignment]
 
     def _spawn_task_from_thread(
         self,
         func: Callable,
         args: tuple,
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
         name: object,
         future: Future,
     ) -> None:
         """
         Spawn a new task using the given callable.
 
         Implementors must ensure that the future is resolved when the task finishes.
@@ -252,27 +250,23 @@
         :param future: a future that will resolve to the return value of the callable, or the
             exception raised during its execution
 
         """
         raise NotImplementedError
 
     @overload
-    def call(
-        self, func: Callable[..., Coroutine[Any, Any, T_Retval]], *args: object
-    ) -> T_Retval:
+    def call(self, func: Callable[..., Awaitable[T_Retval]], *args: object) -> T_Retval:
         ...
 
     @overload
     def call(self, func: Callable[..., T_Retval], *args: object) -> T_Retval:
         ...
 
     def call(
-        self,
-        func: Callable[..., Union[Coroutine[Any, Any, T_Retval], T_Retval]],
-        *args: object
+        self, func: Callable[..., Awaitable[T_Retval] | T_Retval], *args: object
     ) -> T_Retval:
         """
         Call the given function in the event loop thread.
 
         If the callable returns a coroutine object, it is awaited on.
 
         :param func: any callable
@@ -281,32 +275,32 @@
 
         """
         return cast(T_Retval, self.start_task_soon(func, *args).result())
 
     @overload
     def spawn_task(
         self,
-        func: Callable[..., Coroutine[Any, Any, T_Retval]],
+        func: Callable[..., Awaitable[T_Retval]],
         *args: object,
-        name: object = None
-    ) -> "Future[T_Retval]":
+        name: object = None,
+    ) -> Future[T_Retval]:
         ...
 
     @overload
     def spawn_task(
         self, func: Callable[..., T_Retval], *args: object, name: object = None
-    ) -> "Future[T_Retval]":
+    ) -> Future[T_Retval]:
         ...
 
     def spawn_task(
         self,
-        func: Callable[..., Union[Coroutine[Any, Any, T_Retval], T_Retval]],
+        func: Callable[..., Awaitable[T_Retval] | T_Retval],
         *args: object,
-        name: object = None
-    ) -> "Future[T_Retval]":
+        name: object = None,
+    ) -> Future[T_Retval]:
         """
         Start a task in the portal's task group.
 
         :param func: the target coroutine function
         :param args: positional arguments passed to ``func``
         :param name: name of the task (will be coerced to a string if not ``None``)
         :return: a future that resolves with the return value of the callable if the task completes
@@ -325,39 +319,39 @@
             DeprecationWarning,
         )
         return self.start_task_soon(func, *args, name=name)  # type: ignore[arg-type]
 
     @overload
     def start_task_soon(
         self,
-        func: Callable[..., Coroutine[Any, Any, T_Retval]],
+        func: Callable[..., Awaitable[T_Retval]],
         *args: object,
-        name: object = None
-    ) -> "Future[T_Retval]":
+        name: object = None,
+    ) -> Future[T_Retval]:
         ...
 
     @overload
     def start_task_soon(
         self, func: Callable[..., T_Retval], *args: object, name: object = None
-    ) -> "Future[T_Retval]":
+    ) -> Future[T_Retval]:
         ...
 
     def start_task_soon(
         self,
-        func: Callable[..., Union[Coroutine[Any, Any, T_Retval], T_Retval]],
+        func: Callable[..., Awaitable[T_Retval] | T_Retval],
         *args: object,
-        name: object = None
-    ) -> "Future[T_Retval]":
+        name: object = None,
+    ) -> Future[T_Retval]:
         """
         Start a task in the portal's task group.
 
         The task will be run inside a cancel scope which can be cancelled by cancelling the
         returned future.
 
-        :param func: the target coroutine function
+        :param func: the target function
         :param args: positional arguments passed to ``func``
         :param name: name of the task (will be coerced to a string if not ``None``)
         :return: a future that resolves with the return value of the callable if the task completes
             successfully, or with the exception raised in the task
         :raises RuntimeError: if the portal is not running or if this method is called from within
             the event loop thread
 
@@ -366,25 +360,22 @@
         """
         self._check_running()
         f: Future = Future()
         self._spawn_task_from_thread(func, args, {}, name, f)
         return f
 
     def start_task(
-        self,
-        func: Callable[..., Coroutine[Any, Any, Any]],
-        *args: object,
-        name: object = None
-    ) -> Tuple["Future[Any]", Any]:
+        self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
+    ) -> tuple[Future[Any], Any]:
         """
         Start a task in the portal's task group and wait until it signals for readiness.
 
         This method works the same way as :meth:`TaskGroup.start`.
 
-        :param func: the target coroutine function
+        :param func: the target function
         :param args: positional arguments passed to ``func``
         :param name: name of the task (will be coerced to a string if not ``None``)
         :return: a tuple of (future, task_status_value) where the ``task_status_value`` is the
             value passed to ``task_status.started()`` from within the target function
 
         .. versionadded:: 3.0
 
@@ -445,15 +436,15 @@
         DeprecationWarning,
     )
     return BlockingPortal()
 
 
 @contextmanager
 def start_blocking_portal(
-    backend: str = "asyncio", backend_options: Optional[Dict[str, Any]] = None
+    backend: str = "asyncio", backend_options: dict[str, Any] | None = None
 ) -> Generator[BlockingPortal, Any, None]:
     """
     Start a new event loop in a new thread and run a blocking portal in its main task.
 
     The parameters are the same as for :func:`~anyio.run`.
 
     :param backend: name of the backend
@@ -487,16 +478,20 @@
         except BaseException:
             future.cancel()
             run_future.cancel()
             raise
 
         if future.done():
             portal = future.result()
+            cancel_remaining_tasks = False
             try:
                 yield portal
             except BaseException:
-                portal.call(portal.stop, True)
+                cancel_remaining_tasks = True
                 raise
-
-            portal.call(portal.stop, False)
+            finally:
+                try:
+                    portal.call(portal.stop, cancel_remaining_tasks)
+                except RuntimeError:
+                    pass
 
         run_future.result()
```

### Comparing `anyio-3.6.2/src/anyio/lowlevel.py` & `anyio-3.7.0rc1/src/anyio/lowlevel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import enum
 import sys
 from dataclasses import dataclass
-from typing import Any, Dict, Generic, Set, TypeVar, Union, overload
+from typing import Any, Generic, TypeVar, overload
 from weakref import WeakKeyDictionary
 
 from ._core._eventloop import get_asynclib
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -20,14 +22,15 @@
     Check for cancellation and allow the scheduler to switch to another task.
 
     Equivalent to (but more efficient than)::
 
         await checkpoint_if_cancelled()
         await cancel_shielded_checkpoint()
 
+
     .. versionadded:: 3.0
 
     """
     await get_asynclib().checkpoint()
 
 
 async def checkpoint_if_cancelled() -> None:
@@ -47,27 +50,28 @@
     Allow the scheduler to switch to another task but without checking for cancellation.
 
     Equivalent to (but potentially more efficient than)::
 
         with CancelScope(shield=True):
             await checkpoint()
 
+
     .. versionadded:: 3.0
 
     """
     await get_asynclib().cancel_shielded_checkpoint()
 
 
 def current_token() -> object:
     """Return a backend specific token object that can be used to get back to the event loop."""
     return get_asynclib().current_token()
 
 
-_run_vars = WeakKeyDictionary()  # type: WeakKeyDictionary[Any, Dict[str, Any]]
-_token_wrappers: Dict[Any, "_TokenWrapper"] = {}
+_run_vars: WeakKeyDictionary[Any, dict[str, Any]] = WeakKeyDictionary()
+_token_wrappers: dict[Any, _TokenWrapper] = {}
 
 
 @dataclass(frozen=True)
 class _TokenWrapper:
     __slots__ = "_token", "__weakref__"
     _token: object
 
@@ -75,41 +79,41 @@
 class _NoValueSet(enum.Enum):
     NO_VALUE_SET = enum.auto()
 
 
 class RunvarToken(Generic[T]):
     __slots__ = "_var", "_value", "_redeemed"
 
-    def __init__(
-        self, var: "RunVar[T]", value: Union[T, Literal[_NoValueSet.NO_VALUE_SET]]
-    ):
+    def __init__(self, var: RunVar[T], value: T | Literal[_NoValueSet.NO_VALUE_SET]):
         self._var = var
-        self._value: Union[T, Literal[_NoValueSet.NO_VALUE_SET]] = value
+        self._value: T | Literal[_NoValueSet.NO_VALUE_SET] = value
         self._redeemed = False
 
 
 class RunVar(Generic[T]):
-    """Like a :class:`~contextvars.ContextVar`, expect scoped to the running event loop."""
+    """
+    Like a :class:`~contextvars.ContextVar`, except scoped to the running event loop.
+    """
 
     __slots__ = "_name", "_default"
 
     NO_VALUE_SET: Literal[_NoValueSet.NO_VALUE_SET] = _NoValueSet.NO_VALUE_SET
 
-    _token_wrappers: Set[_TokenWrapper] = set()
+    _token_wrappers: set[_TokenWrapper] = set()
 
     def __init__(
         self,
         name: str,
-        default: Union[T, Literal[_NoValueSet.NO_VALUE_SET]] = NO_VALUE_SET,
+        default: T | Literal[_NoValueSet.NO_VALUE_SET] = NO_VALUE_SET,
     ):
         self._name = name
         self._default = default
 
     @property
-    def _current_vars(self) -> Dict[str, T]:
+    def _current_vars(self) -> dict[str, T]:
         token = current_token()
         while True:
             try:
                 return _run_vars[token]
             except TypeError:
                 # Happens when token isn't weak referable (TrioToken).
                 # This workaround does mean that some memory will leak on Trio until the problem
@@ -117,24 +121,24 @@
                 token = _TokenWrapper(token)
                 self._token_wrappers.add(token)
             except KeyError:
                 run_vars = _run_vars[token] = {}
                 return run_vars
 
     @overload
-    def get(self, default: D) -> Union[T, D]:
+    def get(self, default: D) -> T | D:
         ...
 
     @overload
     def get(self) -> T:
         ...
 
     def get(
-        self, default: Union[D, Literal[_NoValueSet.NO_VALUE_SET]] = NO_VALUE_SET
-    ) -> Union[T, D]:
+        self, default: D | Literal[_NoValueSet.NO_VALUE_SET] = NO_VALUE_SET
+    ) -> T | D:
         try:
             return self._current_vars[self._name]
         except KeyError:
             if default is not RunVar.NO_VALUE_SET:
                 return default
             elif self._default is not RunVar.NO_VALUE_SET:
                 return self._default
```

### Comparing `anyio-3.6.2/src/anyio/pytest_plugin.py` & `anyio-3.7.0rc1/src/anyio/pytest_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,35 @@
+from __future__ import annotations
+
 from contextlib import contextmanager
 from inspect import isasyncgenfunction, iscoroutinefunction
-from typing import TYPE_CHECKING, Any, Dict, Generator, Optional, Tuple, cast
+from typing import Any, Dict, Generator, Tuple, cast
 
 import pytest
 import sniffio
-from _pytest.fixtures import FixtureRequest
 
 from ._core._eventloop import get_all_backends, get_asynclib
 from .abc import TestRunner
 
-if TYPE_CHECKING:
-    from _pytest.config import Config
-
-_current_runner: Optional[TestRunner] = None
+_current_runner: TestRunner | None = None
 
 
-def extract_backend_and_options(backend: object) -> Tuple[str, Dict[str, Any]]:
+def extract_backend_and_options(backend: object) -> tuple[str, dict[str, Any]]:
     if isinstance(backend, str):
         return backend, {}
     elif isinstance(backend, tuple) and len(backend) == 2:
         if isinstance(backend[0], str) and isinstance(backend[1], dict):
             return cast(Tuple[str, Dict[str, Any]], backend)
 
     raise TypeError("anyio_backend must be either a string or tuple of (string, dict)")
 
 
 @contextmanager
 def get_runner(
-    backend_name: str, backend_options: Dict[str, Any]
+    backend_name: str, backend_options: dict[str, Any]
 ) -> Generator[TestRunner, object, None]:
     global _current_runner
     if _current_runner:
         yield _current_runner
         return
 
     asynclib = get_asynclib(backend_name)
@@ -47,23 +45,23 @@
             yield runner
     finally:
         _current_runner = None
         if token:
             sniffio.current_async_library_cvar.reset(token)
 
 
-def pytest_configure(config: "Config") -> None:
+def pytest_configure(config: Any) -> None:
     config.addinivalue_line(
         "markers",
         "anyio: mark the (coroutine function) test to be run "
         "asynchronously via anyio.",
     )
 
 
-def pytest_fixture_setup(fixturedef: Any, request: FixtureRequest) -> None:
+def pytest_fixture_setup(fixturedef: Any, request: Any) -> None:
     def wrapper(*args, anyio_backend, **kwargs):  # type: ignore[no-untyped-def]
         backend_name, backend_options = extract_backend_and_options(anyio_backend)
         if has_backend_arg:
             kwargs["anyio_backend"] = anyio_backend
 
         with get_runner(backend_name, backend_options) as runner:
             if isasyncgenfunction(func):
@@ -90,15 +88,15 @@
             marker = collector.get_closest_marker("anyio")
             own_markers = getattr(obj, "pytestmark", ())
             if marker or any(marker.name == "anyio" for marker in own_markers):
                 pytest.mark.usefixtures("anyio_backend")(obj)
 
 
 @pytest.hookimpl(tryfirst=True)
-def pytest_pyfunc_call(pyfuncitem: Any) -> Optional[bool]:
+def pytest_pyfunc_call(pyfuncitem: Any) -> bool | None:
     def run_with_hypothesis(**kwargs: Any) -> None:
         with get_runner(backend_name, backend_options) as runner:
             runner.run_test(original_func, kwargs)
 
     backend = pyfuncitem.funcargs.get("anyio_backend")
     if backend:
         backend_name, backend_options = extract_backend_and_options(backend)
@@ -133,12 +131,12 @@
     if isinstance(anyio_backend, str):
         return anyio_backend
     else:
         return anyio_backend[0]
 
 
 @pytest.fixture
-def anyio_backend_options(anyio_backend: Any) -> Dict[str, Any]:
+def anyio_backend_options(anyio_backend: Any) -> dict[str, Any]:
     if isinstance(anyio_backend, str):
         return {}
     else:
         return anyio_backend[1]
```

### Comparing `anyio-3.6.2/src/anyio/streams/buffered.py` & `anyio-3.7.0rc1/src/anyio/streams/buffered.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass, field
 from typing import Any, Callable, Mapping
 
 from .. import ClosedResourceError, DelimiterNotFound, EndOfStream, IncompleteRead
 from ..abc import AnyByteReceiveStream, ByteReceiveStream
```

### Comparing `anyio-3.6.2/src/anyio/streams/file.py` & `anyio-3.7.0rc1/src/anyio/streams/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 from io import SEEK_SET, UnsupportedOperation
 from os import PathLike
 from pathlib import Path
-from typing import Any, BinaryIO, Callable, Dict, Mapping, Union, cast
+from typing import Any, BinaryIO, Callable, Mapping, cast
 
 from .. import (
     BrokenResourceError,
     ClosedResourceError,
     EndOfStream,
     TypedAttributeSet,
     to_thread,
@@ -28,15 +30,15 @@
         self._file = file
 
     async def aclose(self) -> None:
         await to_thread.run_sync(self._file.close)
 
     @property
     def extra_attributes(self) -> Mapping[Any, Callable[[], Any]]:
-        attributes: Dict[Any, Callable[[], Any]] = {
+        attributes: dict[Any, Callable[[], Any]] = {
             FileStreamAttribute.file: lambda: self._file,
         }
 
         if hasattr(self._file, "name"):
             attributes[FileStreamAttribute.path] = lambda: Path(self._file.name)
 
         try:
@@ -55,15 +57,15 @@
 
     :param file: a file that has been opened for reading in binary mode
 
     .. versionadded:: 3.0
     """
 
     @classmethod
-    async def from_path(cls, path: Union[str, "PathLike[str]"]) -> "FileReadStream":
+    async def from_path(cls, path: str | PathLike[str]) -> FileReadStream:
         """
         Create a file read stream by opening the given file.
 
         :param path: path of the file to read from
 
         """
         file = await to_thread.run_sync(Path(path).open, "rb")
@@ -118,16 +120,16 @@
     :param file: a file that has been opened for writing in binary mode
 
     .. versionadded:: 3.0
     """
 
     @classmethod
     async def from_path(
-        cls, path: Union[str, "PathLike[str]"], append: bool = False
-    ) -> "FileWriteStream":
+        cls, path: str | PathLike[str], append: bool = False
+    ) -> FileWriteStream:
         """
         Create a file write stream by opening the given file for writing.
 
         :param path: path of the file to write to
         :param append: if ``True``, open the file for appending; if ``False``, any existing file
             at the given path will be truncated
```

### Comparing `anyio-3.6.2/src/anyio/streams/memory.py` & `anyio-3.7.0rc1/src/anyio/streams/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+from __future__ import annotations
+
 from collections import OrderedDict, deque
 from dataclasses import dataclass, field
 from types import TracebackType
-from typing import Deque, Generic, List, NamedTuple, Optional, Type, TypeVar
+from typing import Deque, Generic, NamedTuple, TypeVar
 
 from .. import (
     BrokenResourceError,
     ClosedResourceError,
     EndOfStream,
     WouldBlock,
     get_cancelled_exc_class,
 )
 from .._core._compat import DeprecatedAwaitable
 from ..abc import Event, ObjectReceiveStream, ObjectSendStream
 from ..lowlevel import checkpoint
 
 T_Item = TypeVar("T_Item")
+T_co = TypeVar("T_co", covariant=True)
+T_contra = TypeVar("T_contra", contravariant=True)
 
 
 class MemoryObjectStreamStatistics(NamedTuple):
     current_buffer_used: int  #: number of items stored in the buffer
     #: maximum number of items that can be stored on this stream (or :data:`math.inf`)
     max_buffer_size: float
     open_send_streams: int  #: number of unclosed clones of the send stream
@@ -30,18 +34,18 @@
 
 @dataclass(eq=False)
 class MemoryObjectStreamState(Generic[T_Item]):
     max_buffer_size: float = field()
     buffer: Deque[T_Item] = field(init=False, default_factory=deque)
     open_send_channels: int = field(init=False, default=0)
     open_receive_channels: int = field(init=False, default=0)
-    waiting_receivers: "OrderedDict[Event, List[T_Item]]" = field(
+    waiting_receivers: OrderedDict[Event, list[T_Item]] = field(
         init=False, default_factory=OrderedDict
     )
-    waiting_senders: "OrderedDict[Event, T_Item]" = field(
+    waiting_senders: OrderedDict[Event, T_Item] = field(
         init=False, default_factory=OrderedDict
     )
 
     def statistics(self) -> MemoryObjectStreamStatistics:
         return MemoryObjectStreamStatistics(
             len(self.buffer),
             self.max_buffer_size,
@@ -49,22 +53,22 @@
             self.open_receive_channels,
             len(self.waiting_senders),
             len(self.waiting_receivers),
         )
 
 
 @dataclass(eq=False)
-class MemoryObjectReceiveStream(Generic[T_Item], ObjectReceiveStream[T_Item]):
-    _state: MemoryObjectStreamState[T_Item]
+class MemoryObjectReceiveStream(Generic[T_co], ObjectReceiveStream[T_co]):
+    _state: MemoryObjectStreamState[T_co]
     _closed: bool = field(init=False, default=False)
 
     def __post_init__(self) -> None:
         self._state.open_receive_channels += 1
 
-    def receive_nowait(self) -> T_Item:
+    def receive_nowait(self) -> T_co:
         """
         Receive the next item if it can be done without waiting.
 
         :return: the received item
         :raises ~anyio.ClosedResourceError: if this send stream has been closed
         :raises ~anyio.EndOfStream: if the buffer is empty and this stream has been
             closed from the sending end
@@ -84,22 +88,22 @@
         if self._state.buffer:
             return self._state.buffer.popleft()
         elif not self._state.open_send_channels:
             raise EndOfStream
 
         raise WouldBlock
 
-    async def receive(self) -> T_Item:
+    async def receive(self) -> T_co:
         await checkpoint()
         try:
             return self.receive_nowait()
         except WouldBlock:
             # Add ourselves in the queue
             receive_event = Event()
-            container: List[T_Item] = []
+            container: list[T_co] = []
             self._state.waiting_receivers[receive_event] = container
 
             try:
                 await receive_event.wait()
             except get_cancelled_exc_class():
                 # Ignore the immediate cancellation if we already received an item, so as not to
                 # lose it
@@ -109,15 +113,15 @@
                 self._state.waiting_receivers.pop(receive_event, None)
 
             if container:
                 return container[0]
             else:
                 raise EndOfStream
 
-    def clone(self) -> "MemoryObjectReceiveStream[T_Item]":
+    def clone(self) -> MemoryObjectReceiveStream[T_co]:
         """
         Create a clone of this receive stream.
 
         Each clone can be closed separately. Only when all clones have been closed will the
         receiving end of the memory stream be considered closed by the sending ends.
 
         :return: the cloned stream
@@ -151,35 +155,35 @@
         """
         Return statistics about the current state of this stream.
 
         .. versionadded:: 3.0
         """
         return self._state.statistics()
 
-    def __enter__(self) -> "MemoryObjectReceiveStream[T_Item]":
+    def __enter__(self) -> MemoryObjectReceiveStream[T_co]:
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         self.close()
 
 
 @dataclass(eq=False)
-class MemoryObjectSendStream(Generic[T_Item], ObjectSendStream[T_Item]):
-    _state: MemoryObjectStreamState[T_Item]
+class MemoryObjectSendStream(Generic[T_contra], ObjectSendStream[T_contra]):
+    _state: MemoryObjectStreamState[T_contra]
     _closed: bool = field(init=False, default=False)
 
     def __post_init__(self) -> None:
         self._state.open_send_channels += 1
 
-    def send_nowait(self, item: T_Item) -> DeprecatedAwaitable:
+    def send_nowait(self, item: T_contra) -> DeprecatedAwaitable:
         """
         Send an item immediately if it can be done without waiting.
 
         :param item: the item to send
         :raises ~anyio.ClosedResourceError: if this send stream has been closed
         :raises ~anyio.BrokenResourceError: if the stream has been closed from the
             receiving end
@@ -199,15 +203,15 @@
         elif len(self._state.buffer) < self._state.max_buffer_size:
             self._state.buffer.append(item)
         else:
             raise WouldBlock
 
         return DeprecatedAwaitable(self.send_nowait)
 
-    async def send(self, item: T_Item) -> None:
+    async def send(self, item: T_contra) -> None:
         await checkpoint()
         try:
             self.send_nowait(item)
         except WouldBlock:
             # Wait until there's someone on the receiving end
             send_event = Event()
             self._state.waiting_senders[send_event] = item
@@ -216,15 +220,15 @@
             except BaseException:
                 self._state.waiting_senders.pop(send_event, None)  # type: ignore[arg-type]
                 raise
 
             if self._state.waiting_senders.pop(send_event, None):  # type: ignore[arg-type]
                 raise BrokenResourceError
 
-    def clone(self) -> "MemoryObjectSendStream[T_Item]":
+    def clone(self) -> MemoryObjectSendStream[T_contra]:
         """
         Create a clone of this send stream.
 
         Each clone can be closed separately. Only when all clones have been closed will the
         sending end of the memory stream be considered closed by the receiving ends.
 
         :return: the cloned stream
@@ -259,17 +263,17 @@
         """
         Return statistics about the current state of this stream.
 
         .. versionadded:: 3.0
         """
         return self._state.statistics()
 
-    def __enter__(self) -> "MemoryObjectSendStream[T_Item]":
+    def __enter__(self) -> MemoryObjectSendStream[T_contra]:
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         self.close()
```

### Comparing `anyio-3.6.2/src/anyio/streams/stapled.py` & `anyio-3.7.0rc1/src/anyio/streams/stapled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import Any, Callable, Generic, List, Mapping, Optional, Sequence, TypeVar
+from typing import Any, Callable, Generic, Mapping, Sequence, TypeVar
 
 from ..abc import (
     ByteReceiveStream,
     ByteSendStream,
     ByteStream,
     Listener,
     ObjectReceiveStream,
@@ -102,26 +104,26 @@
     :param listeners: listeners to serve
     :type listeners: Sequence[Listener[T_Stream]]
     """
 
     listeners: Sequence[Listener[T_Stream]]
 
     def __post_init__(self) -> None:
-        listeners: List[Listener[T_Stream]] = []
+        listeners: list[Listener[T_Stream]] = []
         for listener in self.listeners:
             if isinstance(listener, MultiListener):
                 listeners.extend(listener.listeners)
                 del listener.listeners[:]  # type: ignore[attr-defined]
             else:
                 listeners.append(listener)
 
         self.listeners = listeners
 
     async def serve(
-        self, handler: Callable[[T_Stream], Any], task_group: Optional[TaskGroup] = None
+        self, handler: Callable[[T_Stream], Any], task_group: TaskGroup | None = None
     ) -> None:
         from .. import create_task_group
 
         async with create_task_group() as tg:
             for listener in self.listeners:
                 tg.start_soon(listener.serve, handler, task_group)
```

### Comparing `anyio-3.6.2/src/anyio/streams/text.py` & `anyio-3.7.0rc1/src/anyio/streams/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import codecs
 from dataclasses import InitVar, dataclass, field
-from typing import Any, Callable, Mapping, Tuple
+from typing import Any, Callable, Mapping
 
 from ..abc import (
     AnyByteReceiveStream,
     AnyByteSendStream,
     AnyByteStream,
     ObjectReceiveStream,
     ObjectSendStream,
@@ -67,15 +69,15 @@
 
     .. _codecs module documentation: https://docs.python.org/3/library/codecs.html#codec-objects
     """
 
     transport_stream: AnyByteSendStream
     encoding: InitVar[str] = "utf-8"
     errors: str = "strict"
-    _encoder: Callable[..., Tuple[bytes, int]] = field(init=False)
+    _encoder: Callable[..., tuple[bytes, int]] = field(init=False)
 
     def __post_init__(self, encoding: str) -> None:
         self._encoder = codecs.getencoder(encoding)
 
     async def send(self, item: str) -> None:
         encoded = self._encoder(item, self.errors)[0]
         await self.transport_stream.send(encoded)
```

### Comparing `anyio-3.6.2/src/anyio/streams/tls.py` & `anyio-3.7.0rc1/src/anyio/streams/tls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import logging
 import re
 import ssl
 from dataclasses import dataclass
 from functools import wraps
-from typing import Any, Callable, Dict, List, Mapping, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Mapping, Tuple, TypeVar
 
 from .. import (
     BrokenResourceError,
     EndOfStream,
     aclose_forcefully,
     get_cancelled_exc_class,
 )
@@ -19,30 +21,29 @@
 _PCTRTTT = Tuple[_PCTRTT, ...]
 
 
 class TLSAttribute(TypedAttributeSet):
     """Contains Transport Layer Security related attributes."""
 
     #: the selected ALPN protocol
-    alpn_protocol: Optional[str] = typed_attribute()
+    alpn_protocol: str | None = typed_attribute()
     #: the channel binding for type ``tls-unique``
     channel_binding_tls_unique: bytes = typed_attribute()
     #: the selected cipher
-    cipher: Tuple[str, str, int] = typed_attribute()
+    cipher: tuple[str, str, int] = typed_attribute()
     #: the peer certificate in dictionary form (see :meth:`ssl.SSLSocket.getpeercert` for more
     #: information)
-    peer_certificate: Optional[
-        Dict[str, Union[str, _PCTRTTT, _PCTRTT]]
-    ] = typed_attribute()
+    peer_certificate: dict[str, str | _PCTRTTT | _PCTRTT] | None = typed_attribute()
     #: the peer certificate in binary form
-    peer_certificate_binary: Optional[bytes] = typed_attribute()
+    peer_certificate_binary: bytes | None = typed_attribute()
     #: ``True`` if this is the server side of the connection
     server_side: bool = typed_attribute()
-    #: ciphers shared between both ends of the TLS connection
-    shared_ciphers: List[Tuple[str, str, int]] = typed_attribute()
+    #: ciphers shared by the client during the TLS handshake (``None`` if this is the
+    #: client side)
+    shared_ciphers: list[tuple[str, str, int]] | None = typed_attribute()
     #: the :class:`~ssl.SSLObject` used for encryption
     ssl_object: ssl.SSLObject = typed_attribute()
     #: ``True`` if this stream does (and expects) a closing TLS handshake when the stream is being
     #: closed
     standard_compatible: bool = typed_attribute()
     #: the TLS protocol version (e.g. ``TLSv1.2``)
     tls_version: str = typed_attribute()
@@ -67,19 +68,19 @@
     _write_bio: ssl.MemoryBIO
 
     @classmethod
     async def wrap(
         cls,
         transport_stream: AnyByteStream,
         *,
-        server_side: Optional[bool] = None,
-        hostname: Optional[str] = None,
-        ssl_context: Optional[ssl.SSLContext] = None,
+        server_side: bool | None = None,
+        hostname: str | None = None,
+        ssl_context: ssl.SSLContext | None = None,
         standard_compatible: bool = True,
-    ) -> "TLSStream":
+    ) -> TLSStream:
         """
         Wrap an existing stream with Transport Layer Security.
 
         This performs a TLS handshake with the peer.
 
         :param transport_stream: a bytes-transporting stream to wrap
         :param server_side: ``True`` if this is the server side of the connection, ``False`` if
@@ -101,15 +102,15 @@
             purpose = (
                 ssl.Purpose.CLIENT_AUTH if server_side else ssl.Purpose.SERVER_AUTH
             )
             ssl_context = ssl.create_default_context(purpose)
 
             # Re-enable detection of unexpected EOFs if it was disabled by Python
             if hasattr(ssl, "OP_IGNORE_UNEXPECTED_EOF"):
-                ssl_context.options ^= ssl.OP_IGNORE_UNEXPECTED_EOF  # type: ignore[attr-defined]
+                ssl_context.options &= ~ssl.OP_IGNORE_UNEXPECTED_EOF
 
         bio_in = ssl.MemoryBIO()
         bio_out = ssl.MemoryBIO()
         ssl_object = ssl_context.wrap_bio(
             bio_in, bio_out, server_side=server_side, server_hostname=hostname
         )
         wrapper = cls(
@@ -165,15 +166,15 @@
             else:
                 # Flush any pending writes first
                 if self._write_bio.pending:
                     await self.transport_stream.send(self._write_bio.read())
 
                 return result
 
-    async def unwrap(self) -> Tuple[AnyByteStream, bytes]:
+    async def unwrap(self) -> tuple[AnyByteStream, bytes]:
         """
         Does the TLS closing handshake.
 
         :return: a tuple of (wrapped byte stream, bytes left in the read buffer)
 
         """
         await self._call_sslobject_method(self._ssl_object.unwrap)
@@ -224,15 +225,17 @@
             TLSAttribute.channel_binding_tls_unique: self._ssl_object.get_channel_binding,
             TLSAttribute.cipher: self._ssl_object.cipher,
             TLSAttribute.peer_certificate: lambda: self._ssl_object.getpeercert(False),
             TLSAttribute.peer_certificate_binary: lambda: self._ssl_object.getpeercert(
                 True
             ),
             TLSAttribute.server_side: lambda: self._ssl_object.server_side,
-            TLSAttribute.shared_ciphers: lambda: self._ssl_object.shared_ciphers(),
+            TLSAttribute.shared_ciphers: lambda: self._ssl_object.shared_ciphers()
+            if self._ssl_object.server_side
+            else None,
             TLSAttribute.standard_compatible: lambda: self.standard_compatible,
             TLSAttribute.ssl_object: lambda: self._ssl_object,
             TLSAttribute.tls_version: self._ssl_object.version,
         }
 
 
 @dataclass(eq=False)
@@ -283,15 +286,15 @@
         # Only reraise base exceptions and cancellation exceptions
         if not isinstance(exc, Exception) or isinstance(exc, get_cancelled_exc_class()):
             raise
 
     async def serve(
         self,
         handler: Callable[[TLSStream], Any],
-        task_group: Optional[TaskGroup] = None,
+        task_group: TaskGroup | None = None,
     ) -> None:
         @wraps(handler)
         async def handler_wrapper(stream: AnyByteStream) -> None:
             from .. import fail_after
 
             try:
                 with fail_after(self.handshake_timeout):
```

### Comparing `anyio-3.6.2/src/anyio/to_process.py` & `anyio-3.7.0rc1/src/anyio/to_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
+from __future__ import annotations
+
 import os
 import pickle
 import subprocess
 import sys
 from collections import deque
 from importlib.util import module_from_spec, spec_from_file_location
-from typing import Callable, Deque, List, Optional, Set, Tuple, TypeVar, cast
+from typing import Callable, Deque, TypeVar, cast
 
 from ._core._eventloop import current_time, get_asynclib, get_cancelled_exc_class
 from ._core._exceptions import BrokenWorkerProcess
 from ._core._subprocesses import open_process
 from ._core._synchronization import CapacityLimiter
 from ._core._tasks import CancelScope, fail_after
 from .abc import ByteReceiveStream, ByteSendStream, Process
 from .lowlevel import RunVar, checkpoint_if_cancelled
 from .streams.buffered import BufferedByteReceiveStream
 
 WORKER_MAX_IDLE_TIME = 300  # 5 minutes
 
 T_Retval = TypeVar("T_Retval")
-_process_pool_workers: RunVar[Set[Process]] = RunVar("_process_pool_workers")
-_process_pool_idle_workers: RunVar[Deque[Tuple[Process, float]]] = RunVar(
+_process_pool_workers: RunVar[set[Process]] = RunVar("_process_pool_workers")
+_process_pool_idle_workers: RunVar[Deque[tuple[Process, float]]] = RunVar(
     "_process_pool_idle_workers"
 )
 _default_process_limiter: RunVar[CapacityLimiter] = RunVar("_default_process_limiter")
 
 
 async def run_sync(
     func: Callable[..., T_Retval],
     *args: object,
     cancellable: bool = False,
-    limiter: Optional[CapacityLimiter] = None,
+    limiter: CapacityLimiter | None = None,
 ) -> T_Retval:
     """
     Call the given function with the given arguments in a worker process.
 
     If the ``cancellable`` option is enabled and the task waiting for its completion is cancelled,
     the worker process running it will be abruptly terminated using SIGKILL (or
     ``terminateProcess()`` on Windows).
@@ -105,15 +107,15 @@
                 buffered = BufferedByteReceiveStream(
                     cast(ByteReceiveStream, process.stdout)
                 )
 
                 # Prune any other workers that have been idle for WORKER_MAX_IDLE_TIME seconds or
                 # longer
                 now = current_time()
-                killed_processes: List[Process] = []
+                killed_processes: list[Process] = []
                 while idle_workers:
                     if now - idle_workers[0][1] < WORKER_MAX_IDLE_TIME:
                         break
 
                     process, idle_since = idle_workers.popleft()
                     process.kill()
                     workers.remove(process)
@@ -204,15 +206,15 @@
             if command == "run":
                 func, args = args
                 try:
                     retval = func(*args)
                 except BaseException as exc:
                     exception = exc
             elif command == "init":
-                main_module_path: Optional[str]
+                main_module_path: str | None
                 sys.path, main_module_path = args
                 del sys.modules["__main__"]
                 if main_module_path:
                     # Load the parent's main module but as __mp_main__ instead of __main__
                     # (like multiprocessing does) to avoid infinite recursion
                     try:
                         spec = spec_from_file_location("__mp_main__", main_module_path)
```

### Comparing `anyio-3.6.2/src/anyio/to_thread.py` & `anyio-3.7.0rc1/src/anyio/to_thread.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Callable, Optional, TypeVar
+from __future__ import annotations
+
+from typing import Callable, TypeVar
 from warnings import warn
 
 from ._core._eventloop import get_asynclib
 from .abc import CapacityLimiter
 
 T_Retval = TypeVar("T_Retval")
 
 
 async def run_sync(
     func: Callable[..., T_Retval],
     *args: object,
     cancellable: bool = False,
-    limiter: Optional[CapacityLimiter] = None
+    limiter: CapacityLimiter | None = None,
 ) -> T_Retval:
     """
     Call the given function with the given arguments in a worker thread.
 
     If the ``cancellable`` option is enabled and the task waiting for its completion is cancelled,
     the thread will still run its course but its return value (or any raised exception) will be
     ignored.
@@ -33,15 +35,15 @@
     )
 
 
 async def run_sync_in_worker_thread(
     func: Callable[..., T_Retval],
     *args: object,
     cancellable: bool = False,
-    limiter: Optional[CapacityLimiter] = None
+    limiter: CapacityLimiter | None = None,
 ) -> T_Retval:
     warn(
         "run_sync_in_worker_thread() has been deprecated, use anyio.to_thread.run_sync() instead",
         DeprecationWarning,
     )
     return await run_sync(func, *args, cancellable=cancellable, limiter=limiter)
```

### Comparing `anyio-3.6.2/src/anyio.egg-info/PKG-INFO` & `anyio-3.7.0rc1/src/anyio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 3.6.2
+Version: 3.7.0rc1
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
-Author: Alex Grönholm
-Author-email: alex.gronholm@nextday.fi
+Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
+Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AnyIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.2
-Provides-Extra: test
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: trio
+Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/agronholm/anyio/actions/workflows/test.yml/badge.svg
   :target: https://github.com/agronholm/anyio/actions/workflows/test.yml
   :alt: Build Status
 .. image:: https://coveralls.io/repos/github/agronholm/anyio/badge.svg?branch=master
@@ -35,33 +36,33 @@
   :target: https://anyio.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation
 .. image:: https://badges.gitter.im/gitterHQ/gitter.svg
   :target: https://gitter.im/python-trio/AnyIO
   :alt: Gitter chat
 
 AnyIO is an asynchronous networking and concurrency library that works on top of either asyncio_ or
-trio_. It implements trio-like `structured concurrency`_ (SC) on top of asyncio, and works in harmony
+trio_. It implements trio-like `structured concurrency`_ (SC) on top of asyncio and works in harmony
 with the native SC of trio itself.
 
 Applications and libraries written against AnyIO's API will run unmodified on either asyncio_ or
 trio_. AnyIO can also be adopted into a library or application incrementally – bit by bit, no full
-refactoring necessary. It will blend in with native libraries of your chosen backend.
+refactoring necessary. It will blend in with the native libraries of your chosen backend.
 
 Documentation
 -------------
 
 View full documentation at: https://anyio.readthedocs.io/
 
 Features
 --------
 
 AnyIO offers the following functionality:
 
 * Task groups (nurseries_ in trio terminology)
-* High level networking (TCP, UDP and UNIX sockets)
+* High-level networking (TCP, UDP and UNIX sockets)
 
   * `Happy eyeballs`_ algorithm for TCP connections (more robust than that of asyncio on Python
     3.8)
   * async/await style UDP sockets (unlike asyncio where you still have to use Transports and
     Protocols)
 
 * A versatile API for byte streams and object streams
```

### Comparing `anyio-3.6.2/src/anyio.egg-info/SOURCES.txt` & `anyio-3.7.0rc1/src/anyio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
-tox.ini
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/api.rst
 docs/basics.rst
 docs/cancellation.rst
 docs/conf.py
 docs/contributing.rst
@@ -36,15 +33,14 @@
 src/anyio/pytest_plugin.py
 src/anyio/to_process.py
 src/anyio/to_thread.py
 src/anyio.egg-info/PKG-INFO
 src/anyio.egg-info/SOURCES.txt
 src/anyio.egg-info/dependency_links.txt
 src/anyio.egg-info/entry_points.txt
-src/anyio.egg-info/not-zip-safe
 src/anyio.egg-info/requires.txt
 src/anyio.egg-info/top_level.txt
 src/anyio/_backends/__init__.py
 src/anyio/_backends/_asyncio.py
 src/anyio/_backends/_trio.py
 src/anyio/_core/__init__.py
 src/anyio/_core/_compat.py
```

### Comparing `anyio-3.6.2/tests/conftest.py` & `anyio-3.7.0rc1/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import asyncio
 import ssl
 from ssl import SSLContext
-from typing import Any, Dict, Generator, Tuple
+from typing import Any, Generator
 
 import pytest
 import trustme
 from _pytest.fixtures import SubRequest
 from trustme import CA
 
 uvloop_marks = []
@@ -37,38 +39,38 @@
             ("asyncio", {"debug": True, "policy": uvloop_policy}),
             marks=uvloop_marks,
             id="asyncio+uvloop",
         ),
         pytest.param("trio"),
     ]
 )
-def anyio_backend(request: SubRequest) -> Tuple[str, Dict[str, Any]]:
+def anyio_backend(request: SubRequest) -> tuple[str, dict[str, Any]]:
     return request.param
 
 
 @pytest.fixture(scope="session")
 def ca() -> CA:
     return trustme.CA()
 
 
 @pytest.fixture(scope="session")
 def server_context(ca: CA) -> SSLContext:
     server_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
     if hasattr(ssl, "OP_IGNORE_UNEXPECTED_EOF"):
-        server_context.options ^= ssl.OP_IGNORE_UNEXPECTED_EOF  # type: ignore[attr-defined]
+        server_context.options &= ~ssl.OP_IGNORE_UNEXPECTED_EOF
 
     ca.issue_cert("localhost").configure_cert(server_context)
     return server_context
 
 
 @pytest.fixture(scope="session")
 def client_context(ca: CA) -> SSLContext:
     client_context = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
     if hasattr(ssl, "OP_IGNORE_UNEXPECTED_EOF"):
-        client_context.options ^= ssl.OP_IGNORE_UNEXPECTED_EOF  # type: ignore[attr-defined]
+        client_context.options &= ~ssl.OP_IGNORE_UNEXPECTED_EOF
 
     ca.configure_trust(client_context)
     return client_context
 
 
 @pytest.fixture
 def asyncio_event_loop() -> Generator[asyncio.AbstractEventLoop, None, None]:
```

### Comparing `anyio-3.6.2/tests/streams/test_buffered.py` & `anyio-3.7.0rc1/tests/streams/test_buffered.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from anyio import IncompleteRead, create_memory_object_stream
 from anyio.streams.buffered import BufferedByteReceiveStream
 
 pytestmark = pytest.mark.anyio
```

### Comparing `anyio-3.6.2/tests/streams/test_file.py` & `anyio-3.7.0rc1/tests/streams/test_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Union
 
 import pytest
 from _pytest.fixtures import SubRequest
 from _pytest.tmpdir import TempPathFactory
 
 from anyio import ClosedResourceError, EndOfStream
 from anyio.abc import ByteReceiveStream
@@ -16,26 +17,24 @@
     @pytest.fixture(scope="class")
     def file_path(self, tmp_path_factory: TempPathFactory) -> Path:
         path = tmp_path_factory.mktemp("filestream") / "data.txt"
         path.write_text("Hello")
         return path
 
     @pytest.fixture(params=[False, True], ids=["str", "path"])
-    def file_path_or_str(
-        self, request: SubRequest, file_path: Path
-    ) -> Union[Path, str]:
+    def file_path_or_str(self, request: SubRequest, file_path: Path) -> Path | str:
         return file_path if request.param else str(file_path)
 
     async def _run_filestream_test(self, stream: ByteReceiveStream) -> None:
         assert await stream.receive(3) == b"Hel"
         assert await stream.receive(3) == b"lo"
         with pytest.raises(EndOfStream):
             await stream.receive(1)
 
-    async def test_read_file_as_path(self, file_path_or_str: Union[Path, str]) -> None:
+    async def test_read_file_as_path(self, file_path_or_str: Path | str) -> None:
         async with await FileReadStream.from_path(file_path_or_str) as stream:
             await self._run_filestream_test(stream)
 
     async def test_read_file(self, file_path: Path) -> None:
         with file_path.open("rb") as file:
             async with FileReadStream(file) as stream:
                 await self._run_filestream_test(stream)
```

### Comparing `anyio-3.6.2/tests/streams/test_memory.py` & `anyio-3.7.0rc1/tests/streams/test_memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import List, Union
+from __future__ import annotations
 
 import pytest
 
 from anyio import (
     BrokenResourceError,
     CancelScope,
     ClosedResourceError,
     EndOfStream,
     WouldBlock,
     create_memory_object_stream,
     create_task_group,
     fail_after,
     wait_all_tasks_blocked,
 )
+from anyio.abc import ObjectReceiveStream, ObjectSendStream
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 
 pytestmark = pytest.mark.anyio
 
 
 def test_invalid_max_buffer() -> None:
     pytest.raises(ValueError, create_memory_object_stream, 1.0).match(
@@ -32,30 +33,30 @@
 
 async def test_receive_then_send() -> None:
     async def receiver() -> None:
         received_objects.append(await receive.receive())
         received_objects.append(await receive.receive())
 
     send, receive = create_memory_object_stream(0)
-    received_objects: List[str] = []
+    received_objects: list[str] = []
     async with create_task_group() as tg:
         tg.start_soon(receiver)
         await wait_all_tasks_blocked()
         await send.send("hello")
         await send.send("anyio")
 
     assert received_objects == ["hello", "anyio"]
 
 
 async def test_receive_then_send_nowait() -> None:
     async def receiver() -> None:
         received_objects.append(await receive.receive())
 
     send, receive = create_memory_object_stream(0)
-    received_objects: List[str] = []
+    received_objects: list[str] = []
     async with create_task_group() as tg:
         tg.start_soon(receiver)
         tg.start_soon(receiver)
         await wait_all_tasks_blocked()
         send.send_nowait("hello")
         send.send_nowait("anyio")
 
@@ -93,15 +94,15 @@
 
 async def test_iterate() -> None:
     async def receiver() -> None:
         async for item in receive:
             received_objects.append(item)
 
     send, receive = create_memory_object_stream()
-    received_objects: List[str] = []
+    received_objects: list[str] = []
     async with create_task_group() as tg:
         tg.start_soon(receiver)
         await send.send("hello")
         await send.send("anyio")
         await send.aclose()
 
     assert received_objects == ["hello", "anyio"]
@@ -219,15 +220,15 @@
     operation.
 
     """
 
     async def receiver() -> None:
         received.append(await receive.receive())
 
-    received: List[str] = []
+    received: list[str] = []
     send, receive = create_memory_object_stream()
     async with create_task_group() as tg:
         tg.start_soon(receiver)
         with CancelScope() as scope:
             scope.cancel()
             await send.send("hello")
 
@@ -247,15 +248,15 @@
     async def scoped_receiver() -> None:
         nonlocal receiver_scope
         with CancelScope() as receiver_scope:
             received.append(await receive.receive())
 
         assert receiver_scope.cancel_called
 
-    received: List[str] = []
+    received: list[str] = []
     send, receive = create_memory_object_stream()
     async with create_task_group() as tg:
         tg.start_soon(scoped_receiver)
         await wait_all_tasks_blocked()
         send.send_nowait("hello")
         assert receiver_scope is not None
         receiver_scope.cancel()
@@ -276,17 +277,18 @@
     async with create_task_group() as tg:
         tg.start_soon(send)
         tg.start_soon(receive)
 
 
 async def test_statistics() -> None:
     send_stream, receive_stream = create_memory_object_stream(1)
-    streams: List[
-        Union[MemoryObjectReceiveStream[int], MemoryObjectSendStream[int]]
-    ] = [send_stream, receive_stream]
+    streams: list[MemoryObjectReceiveStream[int] | MemoryObjectSendStream[int]] = [
+        send_stream,
+        receive_stream,
+    ]
     for stream in streams:
         statistics = stream.statistics()
         assert statistics.max_buffer_size == 1
         assert statistics.current_buffer_used == 0
         assert statistics.open_send_streams == 1
         assert statistics.open_receive_streams == 1
         assert statistics.tasks_waiting_send == 0
@@ -340,7 +342,22 @@
         pass
 
     with pytest.raises(ClosedResourceError):
         send_stream.send_nowait(None)
 
     with pytest.raises(ClosedResourceError):
         receive_stream.receive_nowait()
+
+
+async def test_type_variance() -> None:
+    """
+    This test does not do anything at run time, but since the test suite is also checked
+    with a static type checker, it ensures that the memory object stream
+    co/contravariance works as intended. If it doesn't, one or both of the following
+    reassignments will trip the type checker.
+
+    """
+    send, receive = create_memory_object_stream(item_type=float)
+    receive1: MemoryObjectReceiveStream[complex] = receive  # noqa: F841
+    receive2: ObjectReceiveStream[complex] = receive  # noqa: F841
+    send1: MemoryObjectSendStream[int] = send  # noqa: F841
+    send2: ObjectSendStream[int] = send  # noqa: F841
```

### Comparing `anyio-3.6.2/tests/streams/test_stapled.py` & `anyio-3.7.0rc1/tests/streams/test_stapled.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 from collections import deque
 from dataclasses import InitVar, dataclass, field
-from typing import Deque, Iterable, List, TypeVar
+from typing import Deque, Iterable, TypeVar
 
 import pytest
 
 from anyio import ClosedResourceError, EndOfStream
 from anyio.abc import (
     ByteReceiveStream,
     ByteSendStream,
@@ -117,15 +119,15 @@
 
     async def aclose(self) -> None:
         self._closed = True
 
 
 @dataclass
 class DummyObjectSendStream(ObjectSendStream[T_Item]):
-    buffer: List[T_Item] = field(init=False, default_factory=list)
+    buffer: list[T_Item] = field(init=False, default_factory=list)
     _closed: bool = field(init=False, default=False)
 
     async def send(self, item: T_Item) -> None:
         if self._closed:
             raise ClosedResourceError
 
         self.buffer.append(item)
```

### Comparing `anyio-3.6.2/tests/streams/test_text.py` & `anyio-3.7.0rc1/tests/streams/test_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import platform
 import sys
 
 import pytest
 
 from anyio import create_memory_object_stream
 from anyio.streams.stapled import StapledObjectStream
```

### Comparing `anyio-3.6.2/tests/streams/test_tls.py` & `anyio-3.7.0rc1/tests/streams/test_tls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,39 @@
+from __future__ import annotations
+
 import socket
 import ssl
+import sys
 from contextlib import ExitStack
 from threading import Thread
 from typing import ContextManager, NoReturn
 
 import pytest
+from pytest_mock import MockerFixture
 from trustme import CA
 
 from anyio import (
     BrokenResourceError,
     EndOfStream,
     Event,
     connect_tcp,
+    create_memory_object_stream,
     create_task_group,
     create_tcp_listener,
+    to_thread,
 )
 from anyio.abc import AnyByteStream, SocketAttribute, SocketStream
+from anyio.streams.stapled import StapledObjectStream
 from anyio.streams.tls import TLSAttribute, TLSListener, TLSStream
 
 pytestmark = pytest.mark.anyio
+skip_on_broken_openssl = pytest.mark.skipif(
+    (ssl.OPENSSL_VERSION_INFO[0] > 1 and sys.version_info < (3, 8)),
+    reason="Python 3.7 does not work with OpenSSL versions higher than 1.X",
+)
 
 
 class TestTLSStream:
     async def test_send_receive(
         self, server_context: ssl.SSLContext, client_context: ssl.SSLContext
     ) -> None:
         def serve_sync() -> None:
@@ -91,15 +102,15 @@
                 )
                 assert isinstance(wrapper.extra(TLSAttribute.cipher), tuple)
                 assert isinstance(wrapper.extra(TLSAttribute.peer_certificate), dict)
                 assert isinstance(
                     wrapper.extra(TLSAttribute.peer_certificate_binary), bytes
                 )
                 assert wrapper.extra(TLSAttribute.server_side) is False
-                assert isinstance(wrapper.extra(TLSAttribute.shared_ciphers), list)
+                assert wrapper.extra(TLSAttribute.shared_ciphers) is None
                 assert isinstance(wrapper.extra(TLSAttribute.ssl_object), ssl.SSLObject)
                 assert wrapper.extra(TLSAttribute.standard_compatible) is False
                 assert wrapper.extra(TLSAttribute.tls_version).startswith("TLSv")
                 await wrapper.send(b"\x00")
 
         server_thread.join()
         server_sock.close()
@@ -178,14 +189,15 @@
         [
             pytest.param(True, True, id="both_standard"),
             pytest.param(True, False, id="server_standard"),
             pytest.param(False, True, id="client_standard"),
             pytest.param(False, False, id="neither_standard"),
         ],
     )
+    @skip_on_broken_openssl
     async def test_ragged_eofs(
         self,
         server_context: ssl.SSLContext,
         client_context: ssl.SSLContext,
         server_compatible: bool,
         client_compatible: bool,
     ) -> None:
@@ -234,14 +246,15 @@
         server_sock.close()
         if not client_compatible and server_compatible:
             assert isinstance(server_exc, OSError)
             assert not isinstance(server_exc, socket.timeout)
         else:
             assert server_exc is None
 
+    @skip_on_broken_openssl
     async def test_ragged_eof_on_receive(
         self, server_context: ssl.SSLContext, client_context: ssl.SSLContext
     ) -> None:
         server_exc = None
 
         def serve_sync() -> None:
             nonlocal server_exc
@@ -364,16 +377,31 @@
                 await wrapper.send_eof()
 
             exc.match(expected_pattern)
 
         server_thread.join()
         server_sock.close()
 
+    @pytest.mark.skipif(
+        not hasattr(ssl, "OP_IGNORE_UNEXPECTED_EOF"),
+        reason="The ssl module does not have the OP_IGNORE_UNEXPECTED_EOF attribute",
+    )
+    async def test_default_context_ignore_unexpected_eof_flag_off(
+        self, mocker: MockerFixture
+    ) -> None:
+        send1, receive1 = create_memory_object_stream()
+        client_stream = StapledObjectStream(send1, receive1)
+        mocker.patch.object(TLSStream, "_call_sslobject_method")
+        tls_stream = await TLSStream.wrap(client_stream)
+        ssl_context = tls_stream.extra(TLSAttribute.ssl_object).context
+        assert not ssl_context.options & ssl.OP_IGNORE_UNEXPECTED_EOF
+
 
 class TestTLSListener:
+    @skip_on_broken_openssl
     async def test_handshake_fail(self, server_context: ssl.SSLContext) -> None:
         def handler(stream: object) -> NoReturn:
             pytest.fail("This function should never be called in this scenario")
 
         exception = None
 
         class CustomTLSListener(TLSListener):
@@ -395,7 +423,78 @@
             sock = socket.socket()
             sock.connect(listener.extra(SocketAttribute.local_address))
             sock.close()
             await event.wait()
             tg.cancel_scope.cancel()
 
         assert isinstance(exception, BrokenResourceError)
+
+    async def test_extra_attributes(
+        self, client_context: ssl.SSLContext, server_context: ssl.SSLContext, ca: CA
+    ) -> None:
+        def connect_sync(addr: tuple[str, int]) -> None:
+            with socket.create_connection(addr) as plain_sock:
+                plain_sock.settimeout(2)
+                with client_context.wrap_socket(
+                    plain_sock,
+                    server_side=False,
+                    server_hostname="localhost",
+                    suppress_ragged_eofs=False,
+                ) as conn:
+                    conn.recv(1)
+                    conn.unwrap()
+
+        class CustomTLSListener(TLSListener):
+            @staticmethod
+            async def handle_handshake_error(
+                exc: BaseException, stream: AnyByteStream
+            ) -> None:
+                await TLSListener.handle_handshake_error(exc, stream)
+                pytest.fail("TLS handshake failed")
+
+        async def handler(stream: TLSStream) -> None:
+            async with stream:
+                try:
+                    assert stream.extra(TLSAttribute.alpn_protocol) == "h2"
+                    assert isinstance(
+                        stream.extra(TLSAttribute.channel_binding_tls_unique), bytes
+                    )
+                    assert isinstance(stream.extra(TLSAttribute.cipher), tuple)
+                    assert isinstance(stream.extra(TLSAttribute.peer_certificate), dict)
+                    assert isinstance(
+                        stream.extra(TLSAttribute.peer_certificate_binary), bytes
+                    )
+                    assert stream.extra(TLSAttribute.server_side) is True
+                    shared_ciphers = stream.extra(TLSAttribute.shared_ciphers)
+                    assert isinstance(shared_ciphers, list)
+                    assert len(shared_ciphers) > 1
+                    assert isinstance(
+                        stream.extra(TLSAttribute.ssl_object), ssl.SSLObject
+                    )
+                    assert stream.extra(TLSAttribute.standard_compatible) is True
+                    assert stream.extra(TLSAttribute.tls_version).startswith("TLSv")
+                finally:
+                    event.set()
+                    await stream.send(b"\x00")
+
+        # Issue a client certificate and make the server trust it
+        client_cert = ca.issue_cert("dummy-client")
+        client_cert.configure_cert(client_context)
+        ca.configure_trust(server_context)
+        server_context.verify_mode = ssl.CERT_REQUIRED
+
+        event = Event()
+        server_context.set_alpn_protocols(["h2"])
+        client_context.set_alpn_protocols(["h2"])
+        listener = await create_tcp_listener(local_host="127.0.0.1")
+        tls_listener = CustomTLSListener(listener, server_context)
+        async with tls_listener, create_task_group() as tg:
+            assert tls_listener.extra(TLSAttribute.standard_compatible) is True
+            tg.start_soon(tls_listener.serve, handler)
+            client_thread = Thread(
+                target=connect_sync,
+                args=[listener.extra(SocketAttribute.local_address)],
+            )
+            client_thread.start()
+            await event.wait()
+            await to_thread.run_sync(client_thread.join)
+            tg.cancel_scope.cancel()
```

### Comparing `anyio-3.6.2/tests/test_compat.py` & `anyio-3.7.0rc1/tests/test_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
+
 import pickle
 import signal
 import sys
 import threading
-from typing import Union
 
 import pytest
 
 from anyio import (
     CancelScope,
     CapacityLimiter,
     Condition,
@@ -215,14 +216,14 @@
 
         obj = fn()
         result = pickle.loads(pickle.dumps(obj))
         assert type(result) is float
         assert result == 2.3
 
     def test_deprecated_awaitable_list(self) -> None:
-        def fn() -> DeprecatedAwaitableList[Union[str, int]]:
+        def fn() -> DeprecatedAwaitableList[str | int]:
             return DeprecatedAwaitableList([1, "a"], func=fn)
 
         obj = fn()
         result = pickle.loads(pickle.dumps(obj))
         assert type(result) is list
         assert result == [1, "a"]
```

### Comparing `anyio-3.6.2/tests/test_debugging.py` & `anyio-3.7.0rc1/tests/test_debugging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+from __future__ import annotations
+
 import asyncio
 import sys
 from typing import (
     Any,
     AsyncGenerator,
     Coroutine,
-    Dict,
     Generator,
-    List,
-    Optional,
-    Union,
     cast,
 )
 
 import pytest
 
 import anyio
 from anyio import (
@@ -34,15 +32,15 @@
 else:
 
     def get_coro(self: asyncio.Task) -> Any:
         return self._coro
 
 
 def test_main_task_name(
-    anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+    anyio_backend_name: str, anyio_backend_options: dict[str, Any]
 ) -> None:
     task_name = None
 
     async def main() -> None:
         nonlocal task_name
         task_name = get_current_task().name
 
@@ -68,15 +66,15 @@
         (None, "tests.test_debugging.test_non_main_task_name.<locals>.non_main"),
         (b"name", "b'name'"),
         ("name", "name"),
         ("", ""),
     ],
 )
 async def test_non_main_task_name(
-    name_input: Optional[Union[bytes, str]], expected: str
+    name_input: bytes | str | None, expected: str
 ) -> None:
     async def non_main(*, task_status: TaskStatus) -> None:
         task_status.started(anyio.get_current_task().name)
 
     async with anyio.create_task_group() as tg:
         name = await tg.start(non_main, name=name_input)
 
@@ -87,15 +85,15 @@
     async def inspect() -> None:
         await wait_all_tasks_blocked()
         new_tasks = set(get_running_tasks()) - existing_tasks
         task_infos[:] = sorted(new_tasks, key=lambda info: info.name or "")
         event.set()
 
     event = Event()
-    task_infos: List[TaskInfo] = []
+    task_infos: list[TaskInfo] = []
     host_task = get_current_task()
     async with create_task_group() as tg:
         existing_tasks = set(get_running_tasks())
         tg.start_soon(event.wait, name="task1")
         tg.start_soon(event.wait, name="task2")
         tg.start_soon(inspect)
 
@@ -121,30 +119,24 @@
 def test_wait_generator_based_task_blocked(
     asyncio_event_loop: asyncio.AbstractEventLoop,
 ) -> None:
     async def native_coro_part() -> None:
         await wait_all_tasks_blocked()
         gen = cast(Generator, get_coro(gen_task))
         assert not gen.gi_running
-        if sys.version_info < (3, 7):
-            assert gen.gi_yieldfrom.gi_code.co_name == "wait"
-        else:
-            coro = cast(Coroutine, gen.gi_yieldfrom)
-            assert coro.cr_code.co_name == "wait"
-
+        coro = cast(Coroutine, gen.gi_yieldfrom)
+        assert coro.cr_code.co_name == "wait"
         event.set()
 
-    @asyncio.coroutine
+    @asyncio.coroutine  # type: ignore[attr-defined]
     def generator_part() -> Generator[object, BaseException, None]:
-        yield from event.wait()
+        yield from event.wait()  # type: ignore[misc]
 
     event = asyncio.Event()
-    gen_task: asyncio.Task[None] = asyncio_event_loop.create_task(
-        generator_part()  # type: ignore[arg-type]
-    )
+    gen_task: asyncio.Task[None] = asyncio_event_loop.create_task(generator_part())
     asyncio_event_loop.run_until_complete(native_coro_part())
 
 
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_wait_all_tasks_blocked_asend(anyio_backend: str) -> None:
     """Test that wait_all_tasks_blocked() does not crash on an `asend()` object."""
```

### Comparing `anyio-3.6.2/tests/test_eventloop.py` & `anyio-3.7.0rc1/tests/test_eventloop.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
+import asyncio
 import math
 import sys
 
 import pytest
 from pytest_mock.plugin import MockerFixture
 
-from anyio import sleep_forever, sleep_until
+from anyio import run, sleep_forever, sleep_until
 
 if sys.version_info < (3, 8):
     from mock import AsyncMock
 else:
     from unittest.mock import AsyncMock
 
 pytestmark = pytest.mark.anyio
@@ -32,7 +35,17 @@
     await sleep_until(deadline)
     fake_sleep.assert_called_once_with(0)
 
 
 async def test_sleep_forever(fake_sleep: AsyncMock) -> None:
     await sleep_forever()
     fake_sleep.assert_called_once_with(math.inf)
+
+
+def test_run_task() -> None:
+    """Test that anyio.run() on asyncio will work with a callable returning a Future."""
+
+    async def async_add(x: int, y: int) -> int:
+        return x + y
+
+    result = run(asyncio.create_task, async_add(1, 2), backend="asyncio")
+    assert result == 3
```

### Comparing `anyio-3.6.2/tests/test_fileio.py` & `anyio-3.7.0rc1/tests/test_fileio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from __future__ import annotations
+
 import os
 import pathlib
 import platform
 import socket
 import stat
-from typing import Tuple
 
 import pytest
 from _pytest.tmpdir import TempPathFactory
 
 from anyio import AsyncFile, Path, open_file, wrap_file
 
 pytestmark = pytest.mark.anyio
@@ -275,15 +276,15 @@
         assert not await Path(path).is_symlink()
         path.symlink_to("/foo")
         assert await Path(path).is_symlink()
 
     @pytest.mark.parametrize(
         "args, result", [(("/xyz", "abc"), True), (("/xyz", "baz"), False)]
     )
-    def test_is_relative_to(self, args: Tuple[str], result: bool) -> None:
+    def test_is_relative_to(self, args: tuple[str], result: bool) -> None:
         assert Path("/xyz/abc/foo").is_relative_to(*args) == result
 
     async def test_glob(self, populated_tmpdir: pathlib.Path) -> None:
         all_paths = []
         async for path in Path(populated_tmpdir).glob("**/*.txt"):
             assert isinstance(path, Path)
             all_paths.append(path.name)
```

### Comparing `anyio-3.6.2/tests/test_from_thread.py` & `anyio-3.7.0rc1/tests/test_from_thread.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+from __future__ import annotations
+
 import sys
 import threading
 import time
 from concurrent.futures import CancelledError
-from contextlib import suppress
+from contextlib import asynccontextmanager, suppress
 from contextvars import ContextVar
-from typing import Any, AsyncGenerator, Dict, List, NoReturn, Optional
+from typing import (
+    Any,
+    AsyncGenerator,
+    Awaitable,
+    Callable,
+    NoReturn,
+    TypeVar,
+)
 
 import pytest
 from _pytest.logging import LogCaptureFixture
 
 from anyio import (
     Event,
     create_task_group,
@@ -25,48 +34,60 @@
 from anyio.lowlevel import checkpoint
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-if sys.version_info >= (3, 7):
-    from contextlib import asynccontextmanager
-else:
-    from contextlib2 import asynccontextmanager
+pytestmark = pytest.mark.anyio
 
+T_Retval = TypeVar("T_Retval")
 
-pytestmark = pytest.mark.anyio
 
+async def async_add(a: int, b: int) -> int:
+    assert threading.current_thread() is threading.main_thread()
+    return a + b
+
+
+async def asyncgen_add(a: int, b: int) -> AsyncGenerator[int, Any]:
+    yield a + b
 
-class TestRunAsyncFromThread:
-    async def test_run_async_from_thread(self) -> None:
-        async def add(a: int, b: int) -> int:
-            assert threading.get_ident() == event_loop_thread_id
-            return a + b
-
-        def worker(a: int, b: int) -> int:
-            assert threading.get_ident() != event_loop_thread_id
-            return from_thread.run(add, a, b)
 
-        event_loop_thread_id = threading.get_ident()
-        result = await to_thread.run_sync(worker, 1, 2)
+def sync_add(a: int, b: int) -> int:
+    assert threading.current_thread() is threading.main_thread()
+    return a + b
+
+
+def thread_worker_async(
+    func: Callable[..., Awaitable[T_Retval]], *args: Any
+) -> T_Retval:
+    assert threading.current_thread() is not threading.main_thread()
+    return from_thread.run(func, *args)
+
+
+def thread_worker_sync(func: Callable[..., T_Retval], *args: Any) -> T_Retval:
+    assert threading.current_thread() is not threading.main_thread()
+    return from_thread.run_sync(func, *args)
+
+
+class TestRunAsyncFromThread:
+    async def test_run_corofunc_from_thread(self) -> None:
+        result = await to_thread.run_sync(thread_worker_async, async_add, 1, 2)
         assert result == 3
 
-    async def test_run_sync_from_thread(self) -> None:
-        def add(a: int, b: int) -> int:
-            assert threading.get_ident() == event_loop_thread_id
-            return a + b
-
-        def worker(a: int, b: int) -> int:
-            assert threading.get_ident() != event_loop_thread_id
-            return from_thread.run_sync(add, a, b)
+    async def test_run_asyncgen_from_thread(self) -> None:
+        gen = asyncgen_add(1, 2)
+        try:
+            result = await to_thread.run_sync(thread_worker_async, gen.__anext__)
+            assert result == 3
+        finally:
+            await gen.aclose()
 
-        event_loop_thread_id = threading.get_ident()
-        result = await to_thread.run_sync(worker, 1, 2)
+    async def test_run_sync_from_thread(self) -> None:
+        result = await to_thread.run_sync(thread_worker_sync, sync_add, 1, 2)
         assert result == 3
 
     def test_run_sync_from_thread_pooling(self) -> None:
         async def main() -> None:
             thread_ids = set()
             for _ in range(5):
                 thread_ids.add(await to_thread.run_sync(threading.get_ident))
@@ -85,40 +106,22 @@
                 return
 
             time.sleep(0.1)
 
         pytest.fail("Worker thread did not exit within 1 second")
 
     async def test_run_async_from_thread_exception(self) -> None:
-        async def add(a: int, b: int) -> int:
-            assert threading.get_ident() == event_loop_thread_id
-            return a + b
-
-        def worker(a: int, b: int) -> int:
-            assert threading.get_ident() != event_loop_thread_id
-            return from_thread.run(add, a, b)
-
-        event_loop_thread_id = threading.get_ident()
         with pytest.raises(TypeError) as exc:
-            await to_thread.run_sync(worker, 1, "foo")
+            await to_thread.run_sync(thread_worker_async, async_add, 1, "foo")
 
         exc.match("unsupported operand type")
 
     async def test_run_sync_from_thread_exception(self) -> None:
-        def add(a: int, b: int) -> int:
-            assert threading.get_ident() == event_loop_thread_id
-            return a + b
-
-        def worker(a: int, b: int) -> int:
-            assert threading.get_ident() != event_loop_thread_id
-            return from_thread.run_sync(add, a, b)
-
-        event_loop_thread_id = threading.get_ident()
         with pytest.raises(TypeError) as exc:
-            await to_thread.run_sync(worker, 1, "foo")
+            await to_thread.run_sync(thread_worker_sync, sync_add, 1, "foo")
 
         exc.match("unsupported operand type")
 
     async def test_run_anyio_async_func_from_thread(self) -> None:
         def worker(*args: int) -> Literal[True]:
             from_thread.run(sleep, *args)
             return True
@@ -129,17 +132,14 @@
         async def foo() -> None:
             pass
 
         exc = pytest.raises(RuntimeError, from_thread.run, foo)
         exc.match("This function can only be run from an AnyIO worker thread")
 
     async def test_contextvar_propagation(self, anyio_backend_name: str) -> None:
-        if anyio_backend_name == "asyncio" and sys.version_info < (3, 7):
-            pytest.skip("Asyncio does not propagate context before Python 3.7")
-
         var = ContextVar("var", default=1)
 
         async def async_func() -> int:
             await checkpoint()
             return var.get()
 
         def worker() -> int:
@@ -176,43 +176,40 @@
             return "test"
 
         async def __aexit__(
             self, exc_type: object, exc_val: object, exc_tb: object
         ) -> bool:
             return self.ignore_error
 
-    async def test_successful_call(self) -> None:
-        async def async_get_thread_id() -> int:
-            return threading.get_ident()
-
-        def external_thread() -> None:
-            thread_ids.append(portal.call(threading.get_ident))
-            thread_ids.append(portal.call(async_get_thread_id))
-
-        thread_ids: List[int] = []
+    async def test_call_corofunc(self) -> None:
         async with BlockingPortal() as portal:
-            thread = threading.Thread(target=external_thread)
-            thread.start()
-            await to_thread.run_sync(thread.join)
+            result = await to_thread.run_sync(portal.call, async_add, 1, 2)
+            assert result == 3
 
-        for thread_id in thread_ids:
-            assert thread_id == threading.get_ident()
+    async def test_call_anext(self) -> None:
+        gen = asyncgen_add(1, 2)
+        try:
+            async with BlockingPortal() as portal:
+                result = await to_thread.run_sync(portal.call, gen.__anext__)
+                assert result == 3
+        finally:
+            await gen.aclose()
 
     async def test_aexit_with_exception(self) -> None:
         """Test that when the portal exits with an exception, all tasks are cancelled."""
 
         def external_thread() -> None:
             try:
                 portal.call(sleep, 3)
             except BaseException as exc:
                 results.append(exc)
             else:
                 results.append(None)
 
-        results: List[Optional[BaseException]] = []
+        results: list[BaseException | None] = []
         with suppress(Exception):
             async with BlockingPortal() as portal:
                 thread1 = threading.Thread(target=external_thread)
                 thread1.start()
                 thread2 = threading.Thread(target=external_thread)
                 thread2.start()
                 await sleep(0.1)
@@ -233,15 +230,15 @@
             try:
                 portal.call(sleep, 0.2)
             except BaseException as exc:
                 results.append(exc)
             else:
                 results.append(None)
 
-        results: List[Optional[BaseException]] = []
+        results: list[BaseException | None] = []
         async with BlockingPortal() as portal:
             thread1 = threading.Thread(target=external_thread)
             thread1.start()
             thread2 = threading.Thread(target=external_thread)
             thread2.start()
             await sleep(0.1)
             assert not results
@@ -253,15 +250,15 @@
 
     async def test_call_portal_from_event_loop_thread(self) -> None:
         async with BlockingPortal() as portal:
             exc = pytest.raises(RuntimeError, portal.call, threading.get_ident)
             exc.match("This method cannot be called from the event loop thread")
 
     def test_start_with_new_event_loop(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         async def async_get_thread_id() -> int:
             return threading.get_ident()
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             thread_id = portal.call(async_get_thread_id)
 
@@ -272,25 +269,25 @@
         with pytest.raises(LookupError) as exc:
             with start_blocking_portal("foo"):
                 pass
 
         exc.match("No such backend: foo")
 
     def test_call_stopped_portal(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             pass
 
         pytest.raises(RuntimeError, portal.call, threading.get_ident).match(
             "This portal is not running"
         )
 
     def test_start_task_soon(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         async def event_waiter() -> Literal["test"]:
             await event1.wait()
             event2.set()
             return "test"
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
@@ -298,28 +295,28 @@
             event2 = portal.call(Event)
             future = portal.start_task_soon(event_waiter)
             portal.call(event1.set)
             portal.call(event2.wait)
             assert future.result() == "test"
 
     def test_start_task_soon_cancel_later(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         async def noop() -> None:
             await sleep(2)
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             future = portal.start_task_soon(noop)
             portal.call(wait_all_tasks_blocked)
             future.cancel()
 
         assert future.cancelled()
 
     def test_start_task_soon_cancel_immediately(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         cancelled = False
 
         async def event_waiter() -> None:
             nonlocal cancelled
             try:
                 await sleep(3)
@@ -329,61 +326,61 @@
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             future = portal.start_task_soon(event_waiter)
             future.cancel()
 
         assert cancelled
 
     def test_start_task_soon_with_name(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         task_name = None
 
         async def taskfunc() -> None:
             nonlocal task_name
             task_name = get_current_task().name
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             portal.start_task_soon(taskfunc, name="testname")
 
         assert task_name == "testname"
 
     def test_async_context_manager_success(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             with portal.wrap_async_context_manager(
                 TestBlockingPortal.AsyncCM(False)
             ) as cm:
                 assert cm == "test"
 
     def test_async_context_manager_error(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             with pytest.raises(Exception) as exc:
                 with portal.wrap_async_context_manager(
                     TestBlockingPortal.AsyncCM(False)
                 ) as cm:
                     assert cm == "test"
                     raise Exception("should NOT be ignored")
 
                 exc.match("should NOT be ignored")
 
     def test_async_context_manager_error_ignore(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             with portal.wrap_async_context_manager(
                 TestBlockingPortal.AsyncCM(True)
             ) as cm:
                 assert cm == "test"
                 raise Exception("should be ignored")
 
     def test_async_context_manager_exception_in_task_group(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         """Regression test for #381."""
 
         async def failing_func() -> None:
             0 / 0
 
         @asynccontextmanager
@@ -394,99 +391,93 @@
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             with pytest.raises(ZeroDivisionError):
                 with portal.wrap_async_context_manager(run_in_context()):
                     pass
 
     def test_start_no_value(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         def taskfunc(*, task_status: TaskStatus) -> None:
             task_status.started()
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             future, value = portal.start_task(taskfunc)  # type: ignore[arg-type]
             assert value is None
             assert future.result() is None
 
     def test_start_with_value(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         def taskfunc(*, task_status: TaskStatus) -> None:
             task_status.started("foo")
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             future, value = portal.start_task(taskfunc)  # type: ignore[arg-type]
             assert value == "foo"
             assert future.result() is None
 
     def test_start_crash_before_started_call(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         def taskfunc(*, task_status: object) -> NoReturn:
             raise Exception("foo")
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             with pytest.raises(Exception, match="foo"):
                 portal.start_task(taskfunc)
 
     def test_start_crash_after_started_call(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         def taskfunc(*, task_status: TaskStatus) -> NoReturn:
             task_status.started(2)
             raise Exception("foo")
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             future, value = portal.start_task(taskfunc)
             assert value == 2
             with pytest.raises(Exception, match="foo"):
                 future.result()
 
     def test_start_no_started_call(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         def taskfunc(*, task_status: TaskStatus) -> None:
             pass
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             with pytest.raises(RuntimeError, match="Task exited"):
                 portal.start_task(taskfunc)  # type: ignore[arg-type]
 
     def test_start_with_name(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         def taskfunc(*, task_status: TaskStatus) -> None:
             task_status.started(get_current_task().name)
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             future, start_value = portal.start_task(
                 taskfunc, name="testname"  # type: ignore[arg-type]
             )
             assert start_value == "testname"
 
     def test_contextvar_propagation_sync(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
-        if anyio_backend_name == "asyncio" and sys.version_info < (3, 7):
-            pytest.skip("Asyncio does not propagate context before Python 3.7")
-
         var = ContextVar("var", default=1)
         var.set(6)
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             propagated_value = portal.call(var.get)
 
         assert propagated_value == 6
 
     def test_contextvar_propagation_async(
-        self, anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
-        if anyio_backend_name == "asyncio" and sys.version_info < (3, 7):
-            pytest.skip("Asyncio does not propagate context before Python 3.7")
-
         var = ContextVar("var", default=1)
         var.set(6)
 
         async def get_var() -> int:
             await checkpoint()
             return var.get()
 
@@ -502,7 +493,28 @@
         async def in_loop() -> None:
             raise CancelledError
 
         async with BlockingPortal() as portal:
             await to_thread.run_sync(portal.start_task_soon, in_loop)
 
         assert not caplog.text
+
+    def test_raise_baseexception_from_task(
+        self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
+    ) -> None:
+        """
+        Test that when a task raises a BaseException, it does not trigger additional
+        exceptions when trying to close the portal.
+
+        """
+
+        async def raise_baseexception() -> None:
+            raise BaseException("fatal error")
+
+        with pytest.raises(BaseException, match="fatal error"):
+            with start_blocking_portal(
+                anyio_backend_name, anyio_backend_options
+            ) as portal:
+                with pytest.raises(BaseException, match="fatal error") as exc:
+                    portal.call(raise_baseexception)
+
+                assert exc.value.__context__ is None
```

### Comparing `anyio-3.6.2/tests/test_lowlevel.py` & `anyio-3.7.0rc1/tests/test_lowlevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Dict
+from __future__ import annotations
+
+from typing import Any
 
 import pytest
 
 from anyio import create_task_group, run
 from anyio.lowlevel import (
     RunVar,
     cancel_shielded_checkpoint,
@@ -86,15 +88,15 @@
     assert second_finished
 
 
 class TestRunVar:
     def test_get_set(
         self,
         anyio_backend_name: str,
-        anyio_backend_options: Dict[str, Any],
+        anyio_backend_options: dict[str, Any],
     ) -> None:
         async def taskfunc(index: int) -> None:
             assert var.get() == index
             var.set(index + 1)
 
         async def main() -> None:
             pytest.raises(LookupError, var.get)
```

### Comparing `anyio-3.6.2/tests/test_pytest_plugin.py` & `anyio-3.7.0rc1/tests/test_pytest_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 from _pytest.logging import LogCaptureFixture
 from _pytest.pytester import Pytester
 
 from anyio import get_all_backends
 
 pytestmark = pytest.mark.filterwarnings(
```

### Comparing `anyio-3.6.2/tests/test_signals.py` & `anyio-3.7.0rc1/tests/test_signals.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import signal
 import sys
 from typing import AsyncIterable
 
 import pytest
 
@@ -17,16 +19,21 @@
 
 
 async def test_receive_signals() -> None:
     with open_signal_receiver(signal.SIGUSR1, signal.SIGUSR2) as sigiter:
         await to_thread.run_sync(os.kill, os.getpid(), signal.SIGUSR1)
         await to_thread.run_sync(os.kill, os.getpid(), signal.SIGUSR2)
         with fail_after(1):
-            assert await sigiter.__anext__() == signal.SIGUSR1
-            assert await sigiter.__anext__() == signal.SIGUSR2
+            sigusr1 = await sigiter.__anext__()
+            assert isinstance(sigusr1, signal.Signals)
+            assert sigusr1 == signal.Signals.SIGUSR1
+
+            sigusr2 = await sigiter.__anext__()
+            assert isinstance(sigusr2, signal.Signals)
+            assert sigusr2 == signal.Signals.SIGUSR2
 
 
 async def test_task_group_cancellation_open() -> None:
     async def signal_handler() -> None:
         with open_signal_receiver(signal.SIGUSR1) as sigiter:
             async for v in sigiter:
                 pytest.fail("SIGUSR1 should not be sent")
```

### Comparing `anyio-3.6.2/tests/test_sockets.py` & `anyio-3.7.0rc1/tests/test_sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import array
 import gc
 import io
 import os
 import platform
 import socket
 import sys
@@ -12,23 +14,20 @@
 from socket import AddressFamily
 from ssl import SSLContext, SSLError
 from threading import Thread
 from typing import (
     Any,
     Iterable,
     Iterator,
-    List,
     NoReturn,
-    Tuple,
-    Type,
     TypeVar,
-    Union,
     cast,
 )
 
+import psutil
 import pytest
 from _pytest.fixtures import SubRequest
 from _pytest.logging import LogCaptureFixture
 from _pytest.monkeypatch import MonkeyPatch
 from _pytest.tmpdir import TempPathFactory
 
 from anyio import (
@@ -83,14 +82,16 @@
             s.close()
             del s
     except OSError:
         pass
     else:
         has_ipv6 = True
 
+skip_ipv6_mark = pytest.mark.skipif(not has_ipv6, reason="IPv6 is not available")
+
 
 @pytest.fixture
 def fake_localhost_dns(monkeypatch: MonkeyPatch) -> None:
     def fake_getaddrinfo(*args: Any, **kwargs: Any) -> object:
         # Make it return IPv4 addresses first so we can test the IPv6 preference
         results = real_getaddrinfo(*args, **kwargs)
         return sorted(results, key=lambda item: item[0])
@@ -98,19 +99,15 @@
     real_getaddrinfo = socket.getaddrinfo
     monkeypatch.setattr("socket.getaddrinfo", fake_getaddrinfo)
 
 
 @pytest.fixture(
     params=[
         pytest.param(AddressFamily.AF_INET, id="ipv4"),
-        pytest.param(
-            AddressFamily.AF_INET6,
-            id="ipv6",
-            marks=[pytest.mark.skipif(not has_ipv6, reason="no IPv6 support")],
-        ),
+        pytest.param(AddressFamily.AF_INET6, id="ipv6", marks=[skip_ipv6_mark]),
     ]
 )
 def family(request: SubRequest) -> AnyIPAddressFamily:
     return request.param
 
 
 @pytest.fixture
@@ -154,21 +151,21 @@
         sock.settimeout(1)
         sock.bind(("localhost", 0))
         sock.listen()
         yield sock
         sock.close()
 
     @pytest.fixture
-    def server_addr(self, server_sock: socket.socket) -> Tuple[str, int]:
+    def server_addr(self, server_sock: socket.socket) -> tuple[str, int]:
         return server_sock.getsockname()[:2]
 
     async def test_extra_attributes(
         self,
         server_sock: socket.socket,
-        server_addr: Tuple[str, int],
+        server_addr: tuple[str, int],
         family: AnyIPAddressFamily,
     ) -> None:
         async with await connect_tcp(*server_addr) as stream:
             raw_socket = stream.extra(SocketAttribute.raw_socket)
             assert stream.extra(SocketAttribute.family) == family
             assert (
                 stream.extra(SocketAttribute.local_address)
@@ -177,28 +174,28 @@
             assert (
                 stream.extra(SocketAttribute.local_port) == raw_socket.getsockname()[1]
             )
             assert stream.extra(SocketAttribute.remote_address) == server_addr
             assert stream.extra(SocketAttribute.remote_port) == server_addr[1]
 
     async def test_send_receive(
-        self, server_sock: socket.socket, server_addr: Tuple[str, int]
+        self, server_sock: socket.socket, server_addr: tuple[str, int]
     ) -> None:
         async with await connect_tcp(*server_addr) as stream:
             client, _ = server_sock.accept()
             await stream.send(b"blah")
             request = client.recv(100)
             client.sendall(request[::-1])
             response = await stream.receive()
             client.close()
 
         assert response == b"halb"
 
     async def test_send_large_buffer(
-        self, server_sock: socket.socket, server_addr: Tuple[str, int]
+        self, server_sock: socket.socket, server_addr: tuple[str, int]
     ) -> None:
         def serve() -> None:
             client, _ = server_sock.accept()
             client.sendall(buffer)
             client.close()
 
         buffer = (
@@ -211,15 +208,15 @@
             while len(response) < len(buffer):
                 response += await stream.receive()
 
         thread.join()
         assert response == buffer
 
     async def test_send_eof(
-        self, server_sock: socket.socket, server_addr: Tuple[str, int]
+        self, server_sock: socket.socket, server_addr: tuple[str, int]
     ) -> None:
         def serve() -> None:
             client, _ = server_sock.accept()
             request = b""
             while True:
                 data = client.recv(100)
                 request += data
@@ -237,15 +234,15 @@
             await stream.send_eof()
             response = await stream.receive()
 
         thread.join()
         assert response == b"\ndlrow ,olleh"
 
     async def test_iterate(
-        self, server_sock: socket.socket, server_addr: Tuple[str, int]
+        self, server_sock: socket.socket, server_addr: tuple[str, int]
     ) -> None:
         def serve() -> None:
             client, _ = server_sock.accept()
             client.sendall(b"bl")
             event.wait(1)
             client.sendall(b"ah")
             client.close()
@@ -259,21 +256,21 @@
                 chunks.append(chunk)
                 event.set()
 
         thread.join()
         assert chunks == [b"bl", b"ah"]
 
     async def test_socket_options(
-        self, family: AnyIPAddressFamily, server_addr: Tuple[str, int]
+        self, family: AnyIPAddressFamily, server_addr: tuple[str, int]
     ) -> None:
         async with await connect_tcp(*server_addr) as stream:
             raw_socket = stream.extra(SocketAttribute.raw_socket)
             assert raw_socket.getsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY) != 0
 
-    @pytest.mark.skipif(not has_ipv6, reason="IPv6 is not available")
+    @skip_ipv6_mark
     @pytest.mark.parametrize(
         "local_addr, expected_client_addr",
         [
             pytest.param("", "::1", id="dualstack"),
             pytest.param("127.0.0.1", "127.0.0.1", id="ipv4"),
             pytest.param("::1", "::1", id="ipv6"),
         ],
@@ -307,28 +304,23 @@
         server_sock.close()
         assert client_addr[0] == expected_client_addr
 
     @pytest.mark.parametrize(
         "target, exception_class",
         [
             pytest.param(
-                "localhost",
-                ExceptionGroup,
-                id="multi",
-                marks=[
-                    pytest.mark.skipif(not has_ipv6, reason="IPv6 is not available")
-                ],
+                "localhost", ExceptionGroup, id="multi", marks=[skip_ipv6_mark]
             ),
             pytest.param("127.0.0.1", ConnectionRefusedError, id="single"),
         ],
     )
     async def test_connection_refused(
         self,
         target: str,
-        exception_class: Union[Type[ExceptionGroup], Type[ConnectionRefusedError]],
+        exception_class: type[ExceptionGroup] | type[ConnectionRefusedError],
         fake_localhost_dns: None,
     ) -> None:
         dummy_socket = socket.socket(AddressFamily.AF_INET6)
         dummy_socket.bind(("::", 0))
         free_port = dummy_socket.getsockname()[1]
         dummy_socket.close()
 
@@ -338,15 +330,15 @@
         assert exc.match("All connection attempts failed")
         assert isinstance(exc.value.__cause__, exception_class)
         if isinstance(exc.value.__cause__, ExceptionGroup):
             for exception in exc.value.__cause__.exceptions:
                 assert isinstance(exception, ConnectionRefusedError)
 
     async def test_receive_timeout(
-        self, server_sock: socket.socket, server_addr: Tuple[str, int]
+        self, server_sock: socket.socket, server_addr: tuple[str, int]
     ) -> None:
         def serve() -> None:
             conn, _ = server_sock.accept()
             time.sleep(1)
             conn.close()
 
         thread = Thread(target=serve, daemon=True)
@@ -355,60 +347,60 @@
             start_time = time.monotonic()
             with move_on_after(0.1):
                 while time.monotonic() - start_time < 0.3:
                     await stream.receive(1)
 
                 pytest.fail("The timeout was not respected")
 
-    async def test_concurrent_send(self, server_addr: Tuple[str, int]) -> None:
+    async def test_concurrent_send(self, server_addr: tuple[str, int]) -> None:
         async def send_data() -> NoReturn:
             while True:
                 await stream.send(b"\x00" * 4096)
 
         async with await connect_tcp(*server_addr) as stream:
             async with create_task_group() as tg:
                 tg.start_soon(send_data)
                 await wait_all_tasks_blocked()
                 with pytest.raises(BusyResourceError) as exc:
                     await stream.send(b"foo")
 
                 exc.match("already writing to")
                 tg.cancel_scope.cancel()
 
-    async def test_concurrent_receive(self, server_addr: Tuple[str, int]) -> None:
+    async def test_concurrent_receive(self, server_addr: tuple[str, int]) -> None:
         async with await connect_tcp(*server_addr) as client:
             async with create_task_group() as tg:
                 tg.start_soon(client.receive)
                 await wait_all_tasks_blocked()
                 try:
                     with pytest.raises(BusyResourceError) as exc:
                         await client.receive()
 
                     exc.match("already reading from")
                 finally:
                     tg.cancel_scope.cancel()
 
-    async def test_close_during_receive(self, server_addr: Tuple[str, int]) -> None:
+    async def test_close_during_receive(self, server_addr: tuple[str, int]) -> None:
         async def interrupt() -> None:
             await wait_all_tasks_blocked()
             await stream.aclose()
 
         async with await connect_tcp(*server_addr) as stream:
             async with create_task_group() as tg:
                 tg.start_soon(interrupt)
                 with pytest.raises(ClosedResourceError):
                     await stream.receive()
 
-    async def test_receive_after_close(self, server_addr: Tuple[str, int]) -> None:
+    async def test_receive_after_close(self, server_addr: tuple[str, int]) -> None:
         stream = await connect_tcp(*server_addr)
         await stream.aclose()
         with pytest.raises(ClosedResourceError):
             await stream.receive()
 
-    async def test_send_after_close(self, server_addr: Tuple[str, int]) -> None:
+    async def test_send_after_close(self, server_addr: tuple[str, int]) -> None:
         stream = await connect_tcp(*server_addr)
         await stream.aclose()
         with pytest.raises(ClosedResourceError):
             await stream.send(b"foo")
 
     async def test_send_after_peer_closed(self, family: AnyIPAddressFamily) -> None:
         def serve_once() -> None:
@@ -432,15 +424,15 @@
         thread.join()
 
     async def test_connect_tcp_with_tls(
         self,
         server_context: SSLContext,
         client_context: SSLContext,
         server_sock: socket.socket,
-        server_addr: Tuple[str, int],
+        server_addr: tuple[str, int],
     ) -> None:
         def serve() -> None:
             with suppress(socket.timeout):
                 client, addr = server_sock.accept()
                 client.settimeout(1)
                 client = server_context.wrap_socket(client, server_side=True)
                 data = client.recv(100)
@@ -460,15 +452,15 @@
         assert response == b"olleh"
         thread.join()
 
     async def test_connect_tcp_with_tls_cert_check_fail(
         self,
         server_context: SSLContext,
         server_sock: socket.socket,
-        server_addr: Tuple[str, int],
+        server_addr: tuple[str, int],
     ) -> None:
         thread_exception = None
 
         def serve() -> None:
             nonlocal thread_exception
             client, addr = server_sock.accept()
             with client:
@@ -552,24 +544,16 @@
                     SocketAttribute.remote_port,
                 )
 
     @pytest.mark.parametrize(
         "family",
         [
             pytest.param(AddressFamily.AF_INET, id="ipv4"),
-            pytest.param(
-                AddressFamily.AF_INET6,
-                id="ipv6",
-                marks=[pytest.mark.skipif(not has_ipv6, reason="no IPv6 support")],
-            ),
-            pytest.param(
-                socket.AF_UNSPEC,
-                id="both",
-                marks=[pytest.mark.skipif(not has_ipv6, reason="no IPv6 support")],
-            ),
+            pytest.param(AddressFamily.AF_INET6, id="ipv6", marks=[skip_ipv6_mark]),
+            pytest.param(socket.AF_UNSPEC, id="both", marks=[skip_ipv6_mark]),
         ],
     )
     async def test_accept(self, family: AnyIPAddressFamily) -> None:
         async with await create_tcp_listener(
             local_host="localhost", family=family
         ) as multi:
             for listener in multi.listeners:
@@ -690,27 +674,47 @@
                             await sleep(0)
                         else:
                             assert message == b"Hello\n"
                             break
 
             tg.cancel_scope.cancel()
 
+    @skip_ipv6_mark
+    @pytest.mark.skipif(
+        sys.platform == "win32",
+        reason="Windows does not support interface name suffixes",
+    )
+    async def test_bind_link_local(self) -> None:
+        # Regression test for #554
+        link_local_ipv6_address = next(
+            (
+                addr.address
+                for addresses in psutil.net_if_addrs().values()
+                for addr in addresses
+                if addr.address.startswith("fe80::") and "%" in addr.address
+            ),
+            None,
+        )
+        if link_local_ipv6_address is None:
+            pytest.fail("Could not find a link-local IPv6 interface")
+
+        async with await create_tcp_listener(local_host=link_local_ipv6_address):
+            pass
+
 
 @pytest.mark.skipif(
     sys.platform == "win32", reason="UNIX sockets are not available on Windows"
 )
 class TestUNIXStream:
     @pytest.fixture
     def socket_path(self, tmp_path_factory: TempPathFactory) -> Path:
         return tmp_path_factory.mktemp("unix").joinpath("socket")
 
     @pytest.fixture(params=[False, True], ids=["str", "path"])
-    def socket_path_or_str(
-        self, request: SubRequest, socket_path: Path
-    ) -> Union[Path, str]:
+    def socket_path_or_str(self, request: SubRequest, socket_path: Path) -> Path | str:
         return socket_path if request.param else str(socket_path)
 
     @pytest.fixture
     def server_sock(self, socket_path: Path) -> Iterable[socket.socket]:
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         sock.settimeout(1)
         sock.bind(str(socket_path))
@@ -732,15 +736,15 @@
                 TypedAttributeLookupError, stream.extra, SocketAttribute.local_port
             )
             pytest.raises(
                 TypedAttributeLookupError, stream.extra, SocketAttribute.remote_port
             )
 
     async def test_send_receive(
-        self, server_sock: socket.socket, socket_path_or_str: Union[Path, str]
+        self, server_sock: socket.socket, socket_path_or_str: Path | str
     ) -> None:
         async with await connect_unix(socket_path_or_str) as stream:
             client, _ = server_sock.accept()
             await stream.send(b"blah")
             request = client.recv(100)
             client.sendall(request[::-1])
             response = await stream.receive()
@@ -975,17 +979,15 @@
 )
 class TestUNIXListener:
     @pytest.fixture
     def socket_path(self, tmp_path_factory: TempPathFactory) -> Path:
         return tmp_path_factory.mktemp("unix").joinpath("socket")
 
     @pytest.fixture(params=[False, True], ids=["str", "path"])
-    def socket_path_or_str(
-        self, request: SubRequest, socket_path: Path
-    ) -> Union[Path, str]:
+    def socket_path_or_str(self, request: SubRequest, socket_path: Path) -> Path | str:
         return socket_path if request.param else str(socket_path)
 
     async def test_extra_attributes(self, socket_path: Path) -> None:
         async with await create_unix_listener(socket_path) as listener:
             raw_socket = listener.extra(SocketAttribute.raw_socket)
             assert listener.extra(SocketAttribute.family) == socket.AF_UNIX
             assert (
@@ -1000,15 +1002,15 @@
                 listener.extra,
                 SocketAttribute.remote_address,
             )
             pytest.raises(
                 TypedAttributeLookupError, listener.extra, SocketAttribute.remote_port
             )
 
-    async def test_accept(self, socket_path_or_str: Union[Path, str]) -> None:
+    async def test_accept(self, socket_path_or_str: Path | str) -> None:
         async with await create_unix_listener(socket_path_or_str) as listener:
             client = socket.socket(socket.AF_UNIX)
             client.settimeout(1)
             client.connect(str(socket_path_or_str))
             stream = await listener.accept()
             client.sendall(b"blah")
             request = await stream.receive()
@@ -1073,21 +1075,21 @@
 
 async def test_multi_listener(tmp_path_factory: TempPathFactory) -> None:
     async def handle(stream: SocketStream) -> None:
         client_addresses.append(stream.extra(SocketAttribute.remote_address))
         event.set()
         await stream.aclose()
 
-    client_addresses: List[Union[str, IPSockAddrType]] = []
-    listeners: List[Listener] = [await create_tcp_listener(local_host="localhost")]
+    client_addresses: list[str | IPSockAddrType] = []
+    listeners: list[Listener] = [await create_tcp_listener(local_host="localhost")]
     if sys.platform != "win32":
         socket_path = tmp_path_factory.mktemp("unix").joinpath("socket")
         listeners.append(await create_unix_listener(socket_path))
 
-    expected_addresses: List[Union[str, IPSockAddrType]] = []
+    expected_addresses: list[str | IPSockAddrType] = []
     async with MultiListener(listeners) as multi_listener:
         async with create_task_group() as tg:
             tg.start_soon(multi_listener.serve, handle)
             for listener in multi_listener.listeners:
                 event = Event()
                 local_address = listener.extra(SocketAttribute.local_address)
                 if (
```

### Comparing `anyio-3.6.2/tests/test_subprocesses.py` & `anyio-3.7.0rc1/tests/test_subprocesses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
+
 import os
 import platform
 import sys
 from pathlib import Path
 from subprocess import CalledProcessError
 from textwrap import dedent
-from typing import List, Union
 
 import pytest
 
 from anyio import open_process, run_process
 from anyio.streams.buffered import BufferedByteReceiveStream
 
 pytestmark = pytest.mark.anyio
@@ -36,15 +37,15 @@
             False,
             [sys.executable, "-c", "import sys; print(sys.stdin.read()[::-1])"],
             id="exec",
         ),
     ],
 )
 async def test_run_process(
-    shell: bool, command: Union[str, List[str]], anyio_backend_name: str
+    shell: bool, command: str | list[str], anyio_backend_name: str
 ) -> None:
     process = await run_process(command, input=b"abc")
     assert process.returncode == 0
     assert process.stdout.rstrip() == b"cba"
 
 
 async def test_run_process_checked() -> None:
```

### Comparing `anyio-3.6.2/tests/test_synchronization.py` & `anyio-3.7.0rc1/tests/test_synchronization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 import asyncio
-from typing import Optional
 
 import pytest
 
 from anyio import (
     CancelScope,
     Condition,
     Event,
@@ -344,15 +345,15 @@
                     await wait_all_tasks_blocked()
                     semaphore.release()
 
         assert not acquired
         assert semaphore.value == 1
 
     @pytest.mark.parametrize("max_value", [2, None])
-    async def test_max_value(self, max_value: Optional[int]) -> None:
+    async def test_max_value(self, max_value: int | None) -> None:
         semaphore = Semaphore(0, max_value=max_value)
         assert semaphore.max_value == max_value
 
     async def test_max_value_exceeded(self) -> None:
         semaphore = Semaphore(1, max_value=2)
         semaphore.release()
         pytest.raises(ValueError, semaphore.release)
@@ -520,7 +521,26 @@
 
         loop = asyncio.get_event_loop()
         task1 = loop.create_task(acquire())
         task2 = loop.create_task(acquire())
         await asyncio.sleep(0)
         task1.cancel()
         await asyncio.wait_for(task2, 1)
+
+    async def test_ordered_queue(self) -> None:
+        limiter = CapacityLimiter(1)
+        results = []
+        event = Event()
+
+        async def append(x: int, task_status: TaskStatus) -> None:
+            task_status.started()
+            async with limiter:
+                await event.wait()
+                results.append(x)
+
+        async with create_task_group() as tg:
+            for i in [0, 1, 2]:
+                await tg.start(append, i)
+
+            event.set()
+
+        assert results == [0, 1, 2]
```

### Comparing `anyio-3.6.2/tests/test_taskgroups.py` & `anyio-3.7.0rc1/tests/test_taskgroups.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from __future__ import annotations
+
 import asyncio
+import math
 import re
 import sys
 import time
 from typing import (
     Any,
     AsyncGenerator,
     Coroutine,
-    Dict,
     Generator,
     NoReturn,
-    Optional,
-    Set,
+    cast,
 )
 
 import pytest
 
 import anyio
 from anyio import (
+    TASK_STATUS_IGNORED,
     CancelScope,
     ExceptionGroup,
     create_task_group,
     current_effective_deadline,
     current_time,
     fail_after,
     get_cancelled_exc_class,
@@ -28,19 +30,14 @@
     move_on_after,
     sleep,
     wait_all_tasks_blocked,
 )
 from anyio.abc import TaskGroup, TaskStatus
 from anyio.lowlevel import checkpoint
 
-if sys.version_info < (3, 7):
-    current_task = asyncio.Task.current_task
-else:
-    current_task = asyncio.current_task
-
 pytestmark = pytest.mark.anyio
 
 
 async def async_error(text: str, delay: float = 0.1) -> NoReturn:
     try:
         if delay:
             await sleep(delay)
@@ -58,15 +55,15 @@
     exc.match("This task group is not active; no new tasks can be started")
 
 
 async def test_success() -> None:
     async def async_add(value: str) -> None:
         results.add(value)
 
-    results: Set[str] = set()
+    results: set[str] = set()
     async with create_task_group() as tg:
         tg.start_soon(async_add, "a")
         tg.start_soon(async_add, "b")
 
     assert results == {"a", "b"}
 
 
@@ -223,15 +220,15 @@
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_start_native_child_cancelled() -> None:
     task = None
     finished = False
 
     async def taskfunc(*, task_status: TaskStatus) -> None:
         nonlocal task, finished
-        task = current_task()
+        task = asyncio.current_task()
         await sleep(2)
         finished = True
 
     async def start_another() -> None:
         async with create_task_group() as tg2:
             await tg2.start(taskfunc)
 
@@ -393,14 +390,26 @@
         tg.start_soon(subgroup)
         await wait_all_tasks_blocked()
         tg.cancel_scope.cancel()
 
     assert cancel_received
 
 
+async def test_cancel_before_entering_scope() -> None:
+    """
+    Test that CancelScope.cancel() is honored even if called before entering the scope.
+
+    """
+    cancel_scope = anyio.CancelScope()
+    cancel_scope.cancel()
+    with cancel_scope:
+        await anyio.sleep(1)  # Checkpoint to allow anyio to check for cancellation
+        pytest.fail("execution should not reach this point")
+
+
 async def test_exception_group_children() -> None:
     with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(async_error, "task1")
             tg.start_soon(async_error, "task2", 0.15)
 
     assert len(exc.value.exceptions) == 2
@@ -533,22 +542,35 @@
 
 
 async def test_cancel_from_shielded_scope() -> None:
     async with create_task_group() as tg:
         with CancelScope(shield=True) as inner_scope:
             assert inner_scope.shield
             tg.cancel_scope.cancel()
+            assert current_effective_deadline() == math.inf
+
+        assert current_effective_deadline() == -math.inf
 
         with pytest.raises(get_cancelled_exc_class()):
             await sleep(0.01)
 
         with pytest.raises(get_cancelled_exc_class()):
             await sleep(0.01)
 
 
+async def test_cancel_shielded_scope() -> None:
+    with CancelScope(shield=True) as cancel_scope:
+        assert cancel_scope.shield
+        cancel_scope.cancel()
+        assert current_effective_deadline() == -math.inf
+
+        with pytest.raises(get_cancelled_exc_class()):
+            await sleep(0)
+
+
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_cancel_host_asyncgen() -> None:
     done = False
 
     async def host_task() -> None:
         nonlocal done
         async with create_task_group() as tg:
@@ -769,23 +791,23 @@
     async with create_task_group() as tg:
         tg.start_soon(taskfunc)
 
     assert not got_past_checkpoint
 
 
 def test_task_group_in_generator(
-    anyio_backend_name: str, anyio_backend_options: Dict[str, Any]
+    anyio_backend_name: str, anyio_backend_options: dict[str, Any]
 ) -> None:
     async def task_group_generator() -> AsyncGenerator[None, None]:
         async with create_task_group():
             yield
 
     gen = task_group_generator()
     anyio.run(
-        gen.__anext__,  # type: ignore[arg-type]
+        gen.__anext__,
         backend=anyio_backend_name,
         backend_options=anyio_backend_options,
     )
     pytest.raises(
         StopAsyncIteration,
         anyio.run,
         gen.__anext__,
@@ -845,25 +867,25 @@
     sys.version_info >= (3, 11),
     reason="Generator based coroutines have been removed in Python 3.11",
 )
 @pytest.mark.filterwarnings(
     'ignore:"@coroutine" decorator is deprecated:DeprecationWarning'
 )
 def test_cancel_generator_based_task() -> None:
-    from asyncio import coroutine
+    from asyncio import coroutine  # type: ignore[attr-defined]
 
     async def native_coro_part() -> None:
         with CancelScope() as scope:
             scope.cancel()
 
     @coroutine
     def generator_part() -> Generator[object, BaseException, None]:
-        yield from native_coro_part()
+        yield from native_coro_part()  # type: ignore[misc]
 
-    anyio.run(generator_part, backend="asyncio")  # type: ignore[arg-type]
+    anyio.run(generator_part, backend="asyncio")
 
 
 async def test_suppress_exception_context() -> None:
     """
     Test that the __context__ attribute has been cleared when the exception is re-raised in the
     exception group. This prevents recursive tracebacks.
 
@@ -1050,15 +1072,15 @@
             await wait_all_tasks_blocked()
             assert isinstance(task, asyncio.Task)
             task.cancel("blah")
 
 
 async def test_start_soon_parent_id() -> None:
     root_task_id = get_current_task().id
-    parent_id: Optional[int] = None
+    parent_id: int | None = None
 
     async def subtask() -> None:
         nonlocal parent_id
         parent_id = get_current_task().parent_id
 
     async def starter_task() -> None:
         tg.start_soon(subtask)
@@ -1067,17 +1089,17 @@
         tg.start_soon(starter_task)
 
     assert parent_id == root_task_id
 
 
 async def test_start_parent_id() -> None:
     root_task_id = get_current_task().id
-    starter_task_id: Optional[int] = None
-    initial_parent_id: Optional[int] = None
-    permanent_parent_id: Optional[int] = None
+    starter_task_id: int | None = None
+    initial_parent_id: int | None = None
+    permanent_parent_id: int | None = None
 
     async def subtask(*, task_status: TaskStatus) -> None:
         nonlocal initial_parent_id, permanent_parent_id
         initial_parent_id = get_current_task().parent_id
         task_status.started()
         permanent_parent_id = get_current_task().parent_id
 
@@ -1088,7 +1110,78 @@
 
     async with anyio.create_task_group() as tg:
         tg.start_soon(starter_task)
 
     assert initial_parent_id != permanent_parent_id
     assert initial_parent_id == starter_task_id
     assert permanent_parent_id == root_task_id
+
+
+@pytest.mark.skipif(
+    sys.version_info < (3, 11),
+    reason="Task uncancelling is only supported on Python 3.11",
+)
+@pytest.mark.parametrize("anyio_backend", ["asyncio"])
+class TestUncancel:
+    async def test_uncancel_after_native_cancel(self) -> None:
+        task = cast(asyncio.Task, asyncio.current_task())
+        with pytest.raises(asyncio.CancelledError), CancelScope():
+            task.cancel()
+            await anyio.sleep(0)
+
+        assert task.cancelling() == 1
+        task.uncancel()
+
+    async def test_uncancel_after_scope_cancel(self) -> None:
+        task = cast(asyncio.Task, asyncio.current_task())
+        with CancelScope() as scope:
+            scope.cancel()
+            await anyio.sleep(0)
+
+        assert task.cancelling() == 0
+
+    async def test_uncancel_after_scope_and_native_cancel(self) -> None:
+        task = cast(asyncio.Task, asyncio.current_task())
+        with pytest.raises(asyncio.CancelledError), CancelScope() as scope:
+            scope.cancel()
+            task.cancel()
+            await anyio.sleep(0)
+
+        assert task.cancelling() == 1
+        task.uncancel()
+
+
+class TestTaskStatusTyping:
+    """
+    These tests do not do anything at run time, but since the test suite is also checked
+    with a static type checker, it ensures that the `TaskStatus` typing works as
+    intended.
+    """
+
+    async def typetest_None(*, task_status: TaskStatus[None]) -> None:
+        task_status.started()
+        task_status.started(None)
+
+    async def typetest_None_Union(*, task_status: TaskStatus[int | None]) -> None:
+        task_status.started()
+        task_status.started(None)
+
+    async def typetest_non_None(*, task_status: TaskStatus[int]) -> None:
+        # We use `type: ignore` and `--warn-unused-ignores` to get type checking errors
+        # if these ever stop failing.
+        task_status.started()  # type: ignore[call-arg]
+        task_status.started(None)  # type: ignore[arg-type]
+
+    async def typetest_variance_good(*, task_status: TaskStatus[float]) -> None:
+        task_status2: TaskStatus[int] = task_status
+        task_status2.started(int())
+
+    async def typetest_variance_bad(*, task_status: TaskStatus[int]) -> None:
+        # We use `type: ignore` and `--warn-unused-ignores` to get type checking errors
+        # if these ever stop failing.
+        task_status2: TaskStatus[float] = task_status  # type: ignore[assignment]
+        task_status2.started(float())
+
+    async def typetest_optional_status(
+        *, task_status: TaskStatus[int] = TASK_STATUS_IGNORED
+    ) -> None:
+        task_status.started(1)
```

### Comparing `anyio-3.6.2/tests/test_to_process.py` & `anyio-3.7.0rc1/tests/test_to_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import platform
 import sys
 import time
 from functools import partial
 
 import pytest
```

### Comparing `anyio-3.6.2/tests/test_to_thread.py` & `anyio-3.7.0rc1/tests/test_to_thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
+
 import asyncio
-import sys
 import threading
 import time
 from concurrent.futures import Future
 from contextvars import ContextVar
 from functools import partial
-from typing import Any, List, NoReturn, Optional
+from typing import Any, NoReturn
 
 import pytest
 import sniffio
 
 import anyio.to_thread
 from anyio import (
     CapacityLimiter,
@@ -17,19 +18,14 @@
     create_task_group,
     from_thread,
     sleep,
     to_thread,
     wait_all_tasks_blocked,
 )
 
-if sys.version_info < (3, 7):
-    current_task = asyncio.Task.current_task
-else:
-    current_task = asyncio.current_task
-
 pytestmark = pytest.mark.anyio
 
 
 async def test_run_in_thread_cancelled() -> None:
     state = 0
 
     def thread_worker() -> None:
@@ -56,38 +52,39 @@
     with pytest.raises(ValueError) as exc:
         await to_thread.run_sync(thread_worker)
 
     exc.match("^foo$")
 
 
 async def test_run_in_custom_limiter() -> None:
-    num_active_threads = max_active_threads = 0
+    max_active_threads = 0
 
     def thread_worker() -> None:
-        nonlocal num_active_threads, max_active_threads
-        num_active_threads += 1
-        max_active_threads = max(num_active_threads, max_active_threads)
+        nonlocal max_active_threads
+        active_threads.add(threading.current_thread())
+        max_active_threads = max(max_active_threads, len(active_threads))
         event.wait(1)
-        num_active_threads -= 1
+        active_threads.remove(threading.current_thread())
 
     async def task_worker() -> None:
         await to_thread.run_sync(thread_worker, limiter=limiter)
 
     event = threading.Event()
     limiter = CapacityLimiter(3)
+    active_threads: set[threading.Thread] = set()
     async with create_task_group() as tg:
         for _ in range(4):
             tg.start_soon(task_worker)
 
         await sleep(0.1)
-        assert num_active_threads == 3
+        assert len(active_threads) == 3
         assert limiter.borrowed_tokens == 3
         event.set()
 
-    assert num_active_threads == 0
+    assert len(active_threads) == 0
     assert max_active_threads == 3
 
 
 @pytest.mark.parametrize(
     "cancellable, expected_last_active",
     [(False, "task"), (True, "thread")],
     ids=["uncancellable", "cancellable"],
@@ -96,15 +93,15 @@
     cancellable: bool, expected_last_active: str
 ) -> None:
     """
     Test that when a task running a worker thread is cancelled, the cancellation is not acted on
     until the thread finishes.
 
     """
-    last_active: Optional[str] = None
+    last_active: str | None = None
 
     def thread_worker() -> None:
         nonlocal last_active
         from_thread.run_sync(sleep_event.set)
         time.sleep(0.2)
         last_active = "thread"
         from_thread.run_sync(finish_event.set)
@@ -152,19 +149,19 @@
 async def test_asynclib_detection() -> None:
     with pytest.raises(sniffio.AsyncLibraryNotFoundError):
         await to_thread.run_sync(sniffio.current_async_library)
 
 
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_asyncio_cancel_native_task() -> None:
-    task: "Optional[asyncio.Task[None]]" = None
+    task: asyncio.Task[None] | None = None
 
     async def run_in_thread() -> None:
         nonlocal task
-        task = current_task()
+        task = asyncio.current_task()
         await to_thread.run_sync(time.sleep, 0.2, cancellable=True)
 
     async with create_task_group() as tg:
         tg.start_soon(run_in_thread)
         await wait_all_tasks_blocked()
         assert task is not None
         task.cancel()
@@ -222,15 +219,15 @@
     asyncio_event_loop: asyncio.AbstractEventLoop,
 ) -> None:
     """Test that the thread pool shutdown callback does not raise an exception."""
 
     def exception_handler(loop: object, context: Any = None) -> None:
         exceptions.append(context["exception"])
 
-    exceptions: List[BaseException] = []
+    exceptions: list[BaseException] = []
     asyncio_event_loop.set_exception_handler(exception_handler)
     asyncio_event_loop.run_until_complete(to_thread.run_sync(time.sleep, 0))
     assert not exceptions
 
 
 def test_asyncio_run_sync_multiple(
     asyncio_event_loop: asyncio.AbstractEventLoop,
@@ -265,7 +262,21 @@
         await anyio.to_thread.run_sync(time.sleep, 0)
 
     event1 = asyncio.Event()
     event2 = asyncio.Event()
     task1 = asyncio_event_loop.create_task(taskfunc1())
     task2 = asyncio_event_loop.create_task(taskfunc2())
     asyncio_event_loop.run_until_complete(asyncio.gather(task1, task2))
+
+
+async def test_stopiteration() -> None:
+    """
+    Test that raising StopIteration in a worker thread raises a RuntimeError on the
+    caller.
+
+    """
+
+    def raise_stopiteration() -> NoReturn:
+        raise StopIteration
+
+    with pytest.raises(RuntimeError, match="coroutine raised StopIteration"):
+        await to_thread.run_sync(raise_stopiteration)
```

