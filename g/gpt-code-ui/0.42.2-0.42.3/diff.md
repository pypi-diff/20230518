# Comparing `tmp/gpt_code_ui-0.42.2.tar.gz` & `tmp/gpt_code_ui-0.42.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_ui-0.42.2.tar", last modified: Thu May 18 10:36:34 2023, max compression
+gzip compressed data, was "gpt_code_ui-0.42.3.tar", last modified: Thu May 18 10:41:38 2023, max compression
```

## Comparing `gpt_code_ui-0.42.2.tar` & `gpt_code_ui-0.42.3.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:36:34.700781 gpt_code_ui-0.42.2/
--rw-r--r--   0 rick      (1000) rick      (1000)      186 2023-05-18 10:36:34.700781 gpt_code_ui-0.42.2/PKG-INFO
--rw-r--r--   0 rick      (1000) rick      (1000)      902 2023-05-18 10:30:13.000000 gpt_code_ui-0.42.2/README.md
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:36:34.700781 gpt_code_ui-0.42.2/gpt_code_ui/
--rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-12 07:34:59.000000 gpt_code_ui-0.42.2/gpt_code_ui/__init__.py
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:36:34.700781 gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/
--rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-18 10:32:42.000000 gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/__init__.py
--rw-r--r--   0 rick      (1000) rick      (1000)      396 2023-05-10 19:08:20.000000 gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/config.py
--rw-r--r--   0 rick      (1000) rick      (1000)     6801 2023-05-18 10:35:50.000000 gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/kernel_manager.py
--rw-r--r--   0 rick      (1000) rick      (1000)      100 2023-05-10 18:53:26.000000 gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/launch_kernel.py
--rw-r--r--   0 rick      (1000) rick      (1000)     3588 2023-05-18 10:23:42.000000 gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/main.py
--rw-r--r--   0 rick      (1000) rick      (1000)      943 2023-05-18 10:23:41.000000 gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/utils.py
--rw-r--r--   0 rick      (1000) rick      (1000)     2984 2023-05-18 10:23:40.000000 gpt_code_ui-0.42.2/gpt_code_ui/main.py
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:36:34.700781 gpt_code_ui-0.42.2/gpt_code_ui/webapp/
--rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-18 10:32:38.000000 gpt_code_ui-0.42.2/gpt_code_ui/webapp/__init__.py
--rw-r--r--   0 rick      (1000) rick      (1000)     5496 2023-05-18 10:36:08.000000 gpt_code_ui-0.42.2/gpt_code_ui/webapp/main.py
-drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:36:34.700781 gpt_code_ui-0.42.2/gpt_code_ui.egg-info/
--rw-r--r--   0 rick      (1000) rick      (1000)      186 2023-05-18 10:36:34.000000 gpt_code_ui-0.42.2/gpt_code_ui.egg-info/PKG-INFO
--rw-r--r--   0 rick      (1000) rick      (1000)      568 2023-05-18 10:36:34.000000 gpt_code_ui-0.42.2/gpt_code_ui.egg-info/SOURCES.txt
--rw-r--r--   0 rick      (1000) rick      (1000)        1 2023-05-18 10:36:34.000000 gpt_code_ui-0.42.2/gpt_code_ui.egg-info/dependency_links.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       51 2023-05-18 10:36:34.000000 gpt_code_ui-0.42.2/gpt_code_ui.egg-info/entry_points.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       94 2023-05-18 10:36:34.000000 gpt_code_ui-0.42.2/gpt_code_ui.egg-info/requires.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       12 2023-05-18 10:36:34.000000 gpt_code_ui-0.42.2/gpt_code_ui.egg-info/top_level.txt
--rw-r--r--   0 rick      (1000) rick      (1000)       38 2023-05-18 10:36:34.700781 gpt_code_ui-0.42.2/setup.cfg
--rw-r--r--   0 rick      (1000) rick      (1000)      432 2023-05-18 10:36:16.000000 gpt_code_ui-0.42.2/setup.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:41:38.455327 gpt_code_ui-0.42.3/
+-rw-r--r--   0 rick      (1000) rick      (1000)      186 2023-05-18 10:41:38.455327 gpt_code_ui-0.42.3/PKG-INFO
+-rw-r--r--   0 rick      (1000) rick      (1000)      902 2023-05-18 10:30:13.000000 gpt_code_ui-0.42.3/README.md
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:41:38.451327 gpt_code_ui-0.42.3/gpt_code_ui/
+-rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-12 07:34:59.000000 gpt_code_ui-0.42.3/gpt_code_ui/__init__.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:41:38.451327 gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/
+-rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-18 10:32:42.000000 gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/__init__.py
+-rw-r--r--   0 rick      (1000) rick      (1000)      396 2023-05-10 19:08:20.000000 gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/config.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     6801 2023-05-18 10:35:50.000000 gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/kernel_manager.py
+-rw-r--r--   0 rick      (1000) rick      (1000)      100 2023-05-10 18:53:26.000000 gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/launch_kernel.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     3588 2023-05-18 10:23:42.000000 gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/main.py
+-rw-r--r--   0 rick      (1000) rick      (1000)      943 2023-05-18 10:23:41.000000 gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/utils.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     2984 2023-05-18 10:23:40.000000 gpt_code_ui-0.42.3/gpt_code_ui/main.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:41:38.451327 gpt_code_ui-0.42.3/gpt_code_ui/webapp/
+-rw-r--r--   0 rick      (1000) rick      (1000)        0 2023-05-18 10:32:38.000000 gpt_code_ui-0.42.3/gpt_code_ui/webapp/__init__.py
+-rw-r--r--   0 rick      (1000) rick      (1000)     5496 2023-05-18 10:36:08.000000 gpt_code_ui-0.42.3/gpt_code_ui/webapp/main.py
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:41:38.451327 gpt_code_ui-0.42.3/gpt_code_ui/webapp/static/
+-rw-r--r--   0 rick      (1000) rick      (1000)      312 2023-05-17 14:38:37.000000 gpt_code_ui-0.42.3/gpt_code_ui/webapp/static/assistant.svg
+-rw-r--r--   0 rick      (1000) rick      (1000)      463 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.3/gpt_code_ui/webapp/static/index.html
+drwxr-xr-x   0 rick      (1000) rick      (1000)        0 2023-05-18 10:41:38.451327 gpt_code_ui-0.42.3/gpt_code_ui.egg-info/
+-rw-r--r--   0 rick      (1000) rick      (1000)      186 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.3/gpt_code_ui.egg-info/PKG-INFO
+-rw-r--r--   0 rick      (1000) rick      (1000)      645 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.3/gpt_code_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)        1 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.3/gpt_code_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       51 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.3/gpt_code_ui.egg-info/entry_points.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       94 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.3/gpt_code_ui.egg-info/requires.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       12 2023-05-18 10:41:38.000000 gpt_code_ui-0.42.3/gpt_code_ui.egg-info/top_level.txt
+-rw-r--r--   0 rick      (1000) rick      (1000)       38 2023-05-18 10:41:38.455327 gpt_code_ui-0.42.3/setup.cfg
+-rw-r--r--   0 rick      (1000) rick      (1000)      487 2023-05-18 10:41:20.000000 gpt_code_ui-0.42.3/setup.py
```

### Comparing `gpt_code_ui-0.42.2/README.md` & `gpt_code_ui-0.42.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/kernel_manager.py` & `gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/kernel_manager.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/main.py` & `gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/main.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.2/gpt_code_ui/kernel_program/utils.py` & `gpt_code_ui-0.42.3/gpt_code_ui/kernel_program/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.2/gpt_code_ui/main.py` & `gpt_code_ui-0.42.3/gpt_code_ui/main.py`

 * *Files identical despite different names*

### Comparing `gpt_code_ui-0.42.2/gpt_code_ui/webapp/main.py` & `gpt_code_ui-0.42.3/gpt_code_ui/webapp/main.py`

 * *Files identical despite different names*

