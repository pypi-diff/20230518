# Comparing `tmp/featurepy-0.1.0.tar.gz` & `tmp/featurepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurepy-0.1.0.tar", max compression
+gzip compressed data, was "featurepy-0.1.1.tar", max compression
```

## Comparing `featurepy-0.1.0.tar` & `featurepy-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.1.0/LICENSE
--rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.1.0/README.md
--rw-r--r--   0        0        0      572 2023-05-12 20:02:11.767922 featurepy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-05-12 16:12:13.998544 featurepy-0.1.0/src/featurepy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.1.0/src/featurepy/scripts/__init__.py
--rw-r--r--   0        0        0      488 2023-05-10 23:40:04.611517 featurepy-0.1.0/src/featurepy/scripts/features.py
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 featurepy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35129 2023-04-16 16:56:28.332885 featurepy-0.1.1/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-10 21:32:16.081018 featurepy-0.1.1/README.md
+-rw-r--r--   0        0        0      729 2023-05-18 01:57:23.242787 featurepy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-05-12 16:12:13.998544 featurepy-0.1.1/src/featurepy/__init__.py
+-rw-r--r--   0        0        0       20 2023-05-18 01:57:23.243033 featurepy-0.1.1/src/featurepy/flask/__init__.py
+-rw-r--r--   0        0        0      640 2023-05-18 01:57:23.243406 featurepy-0.1.1/src/featurepy/flask/views.py
+-rw-r--r--   0        0        0        0 2023-05-10 23:04:00.786133 featurepy-0.1.1/src/featurepy/scripts/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-15 20:05:33.947104 featurepy-0.1.1/src/featurepy/scripts/features.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 featurepy-0.1.1/PKG-INFO
```

### Comparing `featurepy-0.1.0/LICENSE` & `featurepy-0.1.1/LICENSE`

 * *Files identical despite different names*

