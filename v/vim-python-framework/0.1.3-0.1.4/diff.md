# Comparing `tmp/vim-python-framework-0.1.3.tar.gz` & `tmp/vim-python-framework-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vim-python-framework-0.1.3.tar", last modified: Mon May 15 21:05:33 2023, max compression
+gzip compressed data, was "vim-python-framework-0.1.4.tar", last modified: Thu May 18 06:52:18 2023, max compression
```

## Comparing `vim-python-framework-0.1.3.tar` & `vim-python-framework-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 21:05:33.760091 vim-python-framework-0.1.3/
--rw-r--r--   0 david     (1000) david     (1000)      199 2023-05-15 21:05:33.760091 vim-python-framework-0.1.3/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-05-15 21:05:33.760091 vim-python-framework-0.1.3/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      445 2023-05-15 21:05:29.000000 vim-python-framework-0.1.3/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 21:05:33.759091 vim-python-framework-0.1.3/vim_python_framework/
--rw-r--r--   0 david     (1000) david     (1000)      132 2023-04-25 22:53:56.000000 vim-python-framework-0.1.3/vim_python_framework/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 21:05:33.760091 vim-python-framework-0.1.3/vim_python_framework/include/
--rw-r--r--   0 david     (1000) david     (1000)       16 2023-04-10 02:22:52.000000 vim-python-framework-0.1.3/vim_python_framework/include/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      324 2023-05-08 22:33:37.000000 vim-python-framework-0.1.3/vim_python_framework/include/mymodule.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 21:05:33.760091 vim-python-framework-0.1.3/vim_python_framework/src/
--rw-r--r--   0 david     (1000) david     (1000)       18 2023-04-10 02:45:09.000000 vim-python-framework-0.1.3/vim_python_framework/src/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)       42 2023-04-10 02:38:31.000000 vim-python-framework-0.1.3/vim_python_framework/src/calculator.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-15 21:05:33.760091 vim-python-framework-0.1.3/vim_python_framework.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      199 2023-05-15 21:05:33.000000 vim-python-framework-0.1.3/vim_python_framework.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      422 2023-05-15 21:05:33.000000 vim-python-framework-0.1.3/vim_python_framework.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-15 21:05:33.000000 vim-python-framework-0.1.3/vim_python_framework.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       64 2023-05-15 21:05:33.000000 vim-python-framework-0.1.3/vim_python_framework.egg-info/entry_points.txt
--rw-r--r--   0 david     (1000) david     (1000)       21 2023-05-15 21:05:33.000000 vim-python-framework-0.1.3/vim_python_framework.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-18 06:52:18.341343 vim-python-framework-0.1.4/
+-rw-r--r--   0 david     (1000) david     (1000)      199 2023-05-18 06:52:18.341343 vim-python-framework-0.1.4/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-05-18 06:52:18.341343 vim-python-framework-0.1.4/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)      445 2023-05-18 06:33:42.000000 vim-python-framework-0.1.4/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-18 06:52:18.340343 vim-python-framework-0.1.4/vim_python_framework/
+-rw-r--r--   0 david     (1000) david     (1000)      132 2023-04-25 22:53:56.000000 vim-python-framework-0.1.4/vim_python_framework/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     1592 2023-04-26 00:29:12.000000 vim-python-framework-0.1.4/vim_python_framework/create_plugin.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-18 06:52:18.340343 vim-python-framework-0.1.4/vim_python_framework/include/
+-rw-r--r--   0 david     (1000) david     (1000)       16 2023-04-10 02:22:52.000000 vim-python-framework-0.1.4/vim_python_framework/include/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      324 2023-05-08 22:33:37.000000 vim-python-framework-0.1.4/vim_python_framework/include/mymodule.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-18 06:52:18.341343 vim-python-framework-0.1.4/vim_python_framework/src/
+-rw-r--r--   0 david     (1000) david     (1000)       18 2023-04-10 02:45:09.000000 vim-python-framework-0.1.4/vim_python_framework/src/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)       42 2023-04-10 02:38:31.000000 vim-python-framework-0.1.4/vim_python_framework/src/calculator.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-05-18 06:52:18.340343 vim-python-framework-0.1.4/vim_python_framework.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      199 2023-05-18 06:52:18.000000 vim-python-framework-0.1.4/vim_python_framework.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      460 2023-05-18 06:52:18.000000 vim-python-framework-0.1.4/vim_python_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-05-18 06:52:18.000000 vim-python-framework-0.1.4/vim_python_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       64 2023-05-18 06:52:18.000000 vim-python-framework-0.1.4/vim_python_framework.egg-info/entry_points.txt
+-rw-r--r--   0 david     (1000) david     (1000)       21 2023-05-18 06:52:18.000000 vim-python-framework-0.1.4/vim_python_framework.egg-info/top_level.txt
```

