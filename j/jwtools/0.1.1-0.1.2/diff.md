# Comparing `tmp/jwtools-0.1.1.tar.gz` & `tmp/jwtools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtools-0.1.1.tar", last modified: Wed May 17 09:04:50 2023, max compression
+gzip compressed data, was "jwtools-0.1.2.tar", last modified: Thu May 18 02:17:01 2023, max compression
```

## Comparing `jwtools-0.1.1.tar` & `jwtools-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 09:04:50.459516 jwtools-0.1.1/
--rw-rw-rw-   0        0        0      435 2023-05-17 09:04:50.458516 jwtools-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-17 06:49:57.000000 jwtools-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 09:04:50.438820 jwtools-0.1.1/jwtools/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.1/jwtools/__init__.py
--rw-rw-rw-   0        0        0      380 2023-05-17 06:57:06.000000 jwtools-0.1.1/jwtools/func.py
-drwxrwxrwx   0        0        0        0 2023-05-17 09:04:50.457517 jwtools-0.1.1/jwtools.egg-info/
--rw-rw-rw-   0        0        0      435 2023-05-17 09:04:50.000000 jwtools-0.1.1/jwtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-17 09:04:50.000000 jwtools-0.1.1/jwtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 09:04:50.000000 jwtools-0.1.1/jwtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 09:04:50.000000 jwtools-0.1.1/jwtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 09:04:50.459516 jwtools-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-05-17 09:04:26.000000 jwtools-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:17:01.616776 jwtools-0.1.2/
+-rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      907 2023-05-18 02:17:01.615776 jwtools-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-18 02:11:32.000000 jwtools-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 02:17:01.606777 jwtools-0.1.2/jwtools/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.2/jwtools/__init__.py
+-rw-rw-rw-   0        0        0     1303 2023-05-18 02:16:45.000000 jwtools-0.1.2/jwtools/func.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:17:01.612781 jwtools-0.1.2/jwtools.egg-info/
+-rw-rw-rw-   0        0        0      907 2023-05-18 02:17:01.000000 jwtools-0.1.2/jwtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-18 02:17:01.000000 jwtools-0.1.2/jwtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 02:17:01.000000 jwtools-0.1.2/jwtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-18 02:17:01.000000 jwtools-0.1.2/jwtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 02:17:01.616776 jwtools-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-05-18 02:08:17.000000 jwtools-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 02:17:01.614776 jwtools-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      210 2023-05-18 02:01:21.000000 jwtools-0.1.2/tests/test1.py
```

