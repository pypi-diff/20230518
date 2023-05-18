# Comparing `tmp/mpqhsi-0.0.6.tar.gz` & `tmp/mpqhsi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpqhsi-0.0.6.tar", last modified: Tue Mar 14 07:39:53 2023, max compression
+gzip compressed data, was "mpqhsi-0.0.7.tar", last modified: Thu May 18 05:30:49 2023, max compression
```

## Comparing `mpqhsi-0.0.6.tar` & `mpqhsi-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 07:39:53.528890 mpqhsi-0.0.6/
--rw-rw-rw-   0        0        0      217 2023-03-14 07:39:53.528250 mpqhsi-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-14 07:39:53.514332 mpqhsi-0.0.6/mpqhsi/
--rw-rw-rw-   0        0        0   113664 2023-03-14 07:38:04.000000 mpqhsi-0.0.6/mpqhsi/My_HSI.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0     3884 2023-02-10 05:36:00.000000 mpqhsi-0.0.6/mpqhsi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 07:39:53.527249 mpqhsi-0.0.6/mpqhsi.egg-info/
--rw-rw-rw-   0        0        0      217 2023-03-14 07:39:53.000000 mpqhsi-0.0.6/mpqhsi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-03-14 07:39:53.000000 mpqhsi-0.0.6/mpqhsi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 07:39:53.000000 mpqhsi-0.0.6/mpqhsi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-14 07:39:53.000000 mpqhsi-0.0.6/mpqhsi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-14 07:39:53.528890 mpqhsi-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-03-14 07:39:00.000000 mpqhsi-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:30:49.036711 mpqhsi-0.0.7/
+-rw-rw-rw-   0        0        0      217 2023-05-18 05:30:49.036711 mpqhsi-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 05:30:49.026711 mpqhsi-0.0.7/mpqhsi/
+-rw-rw-rw-   0        0        0   133632 2023-05-18 05:29:38.000000 mpqhsi-0.0.7/mpqhsi/My_HSI.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     5453 2023-05-18 05:28:03.000000 mpqhsi-0.0.7/mpqhsi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:30:49.036711 mpqhsi-0.0.7/mpqhsi.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-05-18 05:30:48.000000 mpqhsi-0.0.7/mpqhsi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-05-18 05:30:48.000000 mpqhsi-0.0.7/mpqhsi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 05:30:48.000000 mpqhsi-0.0.7/mpqhsi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 05:30:48.000000 mpqhsi-0.0.7/mpqhsi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 05:30:49.036711 mpqhsi-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      422 2023-05-17 08:24:59.000000 mpqhsi-0.0.7/setup.py
```

