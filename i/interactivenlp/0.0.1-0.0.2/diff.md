# Comparing `tmp/interactivenlp-0.0.1.tar.gz` & `tmp/interactivenlp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.0.1.tar", last modified: Thu May 18 19:33:50 2023, max compression
+gzip compressed data, was "interactivenlp-0.0.2.tar", last modified: Thu May 18 20:29:30 2023, max compression
```

## Comparing `interactivenlp-0.0.1.tar` & `interactivenlp-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 19:33:50.751814 interactivenlp-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-05-18 19:27:11.000000 interactivenlp-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      456 2023-05-18 19:33:50.751814 interactivenlp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.0.1/README.md
--rw-rw-rw-   0        0        0      472 2023-05-18 19:33:32.000000 interactivenlp-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 19:33:50.752809 interactivenlp-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 19:33:50.721844 interactivenlp-0.0.1/src/
--rw-rw-rw-   0        0        0      281 2023-05-18 19:31:08.000000 interactivenlp-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:33:50.742810 interactivenlp-0.0.1/src/interactivenlp.egg-info/
--rw-rw-rw-   0        0        0      456 2023-05-18 19:33:50.000000 interactivenlp-0.0.1/src/interactivenlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-05-18 19:33:50.000000 interactivenlp-0.0.1/src/interactivenlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 19:33:50.000000 interactivenlp-0.0.1/src/interactivenlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-18 19:33:50.000000 interactivenlp-0.0.1/src/interactivenlp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 19:33:50.747812 interactivenlp-0.0.1/src/typedef/
--rw-rw-rw-   0        0        0     1106 2023-05-18 18:21:43.000000 interactivenlp-0.0.1/src/typedef/block.py
--rw-rw-rw-   0        0        0      189 2023-05-18 18:21:40.000000 interactivenlp-0.0.1/src/typedef/interactive.py
--rw-rw-rw-   0        0        0      159 2023-05-18 01:03:52.000000 interactivenlp-0.0.1/src/typedef/rss.py
-drwxrwxrwx   0        0        0        0 2023-05-18 19:33:50.749810 interactivenlp-0.0.1/src/web/
--rw-rw-rw-   0        0        0      967 2023-05-18 18:18:03.000000 interactivenlp-0.0.1/src/web/server.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:29:30.400629 interactivenlp-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-18 19:27:11.000000 interactivenlp-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-05-18 20:29:30.398605 interactivenlp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 20:29:30.369975 interactivenlp-0.0.2/interactivenlp/
+-rw-rw-rw-   0        0        0      281 2023-05-18 19:31:08.000000 interactivenlp-0.0.2/interactivenlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 20:29:30.397636 interactivenlp-0.0.2/interactivenlp.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-18 20:29:30.000000 interactivenlp-0.0.2/interactivenlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 20:29:30.400629 interactivenlp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      616 2023-05-18 20:27:05.000000 interactivenlp-0.0.2/setup.py
```

### Comparing `interactivenlp-0.0.1/LICENSE` & `interactivenlp-0.0.2/LICENSE`

 * *Files identical despite different names*

