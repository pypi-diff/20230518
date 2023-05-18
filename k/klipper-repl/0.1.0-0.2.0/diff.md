# Comparing `tmp/klipper_repl-0.1.0.tar.gz` & `tmp/klipper_repl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klipper_repl-0.1.0.tar", max compression
+gzip compressed data, was "klipper_repl-0.2.0.tar", max compression
```

## Comparing `klipper_repl-0.1.0.tar` & `klipper_repl-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1425 2023-05-18 19:00:56.474549 klipper_repl-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 13:28:37.849291 klipper_repl-0.1.0/klipper_repl/__init__.py
--rw-r--r--   0        0        0     2138 2023-05-18 12:19:50.809478 klipper_repl-0.1.0/klipper_repl/api.py
--rw-r--r--   0        0        0     4219 2023-05-18 12:16:23.339084 klipper_repl-0.1.0/klipper_repl/cli.py
--rw-r--r--   0        0        0     1099 2023-05-18 12:16:35.736526 klipper_repl-0.1.0/klipper_repl/lexer.py
--rw-r--r--   0        0        0      954 2023-05-18 16:41:21.721828 klipper_repl-0.1.0/klipper_repl/output.py
--rw-r--r--   0        0        0      456 2023-05-18 18:20:32.916106 klipper_repl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1891 1970-01-01 00:00:00.000000 klipper_repl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3585 2023-05-18 19:57:30.305265 klipper_repl-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 13:28:37.849291 klipper_repl-0.2.0/klipper_repl/__init__.py
+-rw-r--r--   0        0        0     2138 2023-05-18 12:19:50.809478 klipper_repl-0.2.0/klipper_repl/api.py
+-rw-r--r--   0        0        0     4219 2023-05-18 12:16:23.339084 klipper_repl-0.2.0/klipper_repl/cli.py
+-rw-r--r--   0        0        0     1099 2023-05-18 12:16:35.736526 klipper_repl-0.2.0/klipper_repl/lexer.py
+-rw-r--r--   0        0        0      954 2023-05-18 16:41:21.721828 klipper_repl-0.2.0/klipper_repl/output.py
+-rw-r--r--   0        0        0      456 2023-05-18 19:58:30.277316 klipper_repl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 klipper_repl-0.2.0/PKG-INFO
```

### Comparing `klipper_repl-0.1.0/klipper_repl/api.py` & `klipper_repl-0.2.0/klipper_repl/api.py`

 * *Files identical despite different names*

### Comparing `klipper_repl-0.1.0/klipper_repl/cli.py` & `klipper_repl-0.2.0/klipper_repl/cli.py`

 * *Files identical despite different names*

### Comparing `klipper_repl-0.1.0/klipper_repl/lexer.py` & `klipper_repl-0.2.0/klipper_repl/lexer.py`

 * *Files identical despite different names*

### Comparing `klipper_repl-0.1.0/klipper_repl/output.py` & `klipper_repl-0.2.0/klipper_repl/output.py`

 * *Files identical despite different names*

