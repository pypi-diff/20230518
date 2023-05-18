# Comparing `tmp/jeeves_shell-2.1.6.tar.gz` & `tmp/jeeves_shell-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_shell-2.1.6.tar", max compression
+gzip compressed data, was "jeeves_shell-2.1.8.tar", max compression
```

## Comparing `jeeves_shell-2.1.6.tar` & `jeeves_shell-2.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.6/LICENSE
--rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.6/README.md
--rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.6/jeeves_shell/__init__.py
--rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.6/jeeves_shell/cli.py
--rw-r--r--   0        0        0     3353 2023-04-15 21:43:00.746449 jeeves_shell-2.1.6/jeeves_shell/discover.py
--rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.6/jeeves_shell/entry_points.py
--rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.6/jeeves_shell/errors.py
--rw-r--r--   0        0        0      256 2023-05-05 17:26:27.544054 jeeves_shell-2.1.6/jeeves_shell/import_by_path.py
--rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.6/jeeves_shell/jeeves.py
--rw-r--r--   0        0        0     1562 2023-05-05 17:26:27.548054 jeeves_shell-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 jeeves_shell-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.8/LICENSE
+-rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.8/README.md
+-rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.8/jeeves_shell/__init__.py
+-rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.8/jeeves_shell/cli.py
+-rw-r--r--   0        0        0     3353 2023-04-15 21:43:00.746449 jeeves_shell-2.1.8/jeeves_shell/discover.py
+-rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.8/jeeves_shell/entry_points.py
+-rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.8/jeeves_shell/errors.py
+-rw-r--r--   0        0        0      256 2023-05-05 17:26:27.544054 jeeves_shell-2.1.8/jeeves_shell/import_by_path.py
+-rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.8/jeeves_shell/jeeves.py
+-rw-r--r--   0        0        0     1685 2023-05-18 19:56:46.496379 jeeves_shell-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 jeeves_shell-2.1.8/PKG-INFO
```

### Comparing `jeeves_shell-2.1.6/LICENSE` & `jeeves_shell-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.6/README.md` & `jeeves_shell-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.6/jeeves_shell/cli.py` & `jeeves_shell-2.1.8/jeeves_shell/cli.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.6/jeeves_shell/discover.py` & `jeeves_shell-2.1.8/jeeves_shell/discover.py`

 * *Files identical despite different names*

