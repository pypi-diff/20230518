# Comparing `tmp/talondoc-0.1.1.tar.gz` & `tmp/talondoc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talondoc-0.1.1.tar", last modified: Sat Sep  3 23:06:28 2022, max compression
+gzip compressed data, was "talondoc-0.5.1.tar", last modified: Thu May 18 12:54:39 2023, max compression
```

## Comparing `talondoc-0.1.1.tar` & `talondoc-0.5.1.tar`

### file list

```diff
@@ -1,48 +1,86 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-03 23:06:28.824488 talondoc-0.1.1/
--rw-r--r--   0 runner     (501) staff       (20)      753 2022-09-03 23:06:28.824140 talondoc-0.1.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      314 2022-09-03 23:05:48.000000 talondoc-0.1.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1563 2022-09-03 23:05:48.000000 talondoc-0.1.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-09-03 23:06:28.824598 talondoc-0.1.1/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-03 23:06:28.809069 talondoc-0.1.1/talondoc/
--rw-r--r--   0 runner     (501) staff       (20)       27 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-03 23:06:28.812955 talondoc-0.1.1/talondoc/analyze/
--rw-r--r--   0 runner     (501) staff       (20)     2235 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/analyze/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2743 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/analyze/python.py
--rw-r--r--   0 runner     (501) staff       (20)     1390 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/analyze/registry.py
--rw-r--r--   0 runner     (501) staff       (20)     2218 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/analyze/talon.py
--rw-r--r--   0 runner     (501) staff       (20)    10091 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/entries.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/py.typed
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-03 23:06:28.814263 talondoc-0.1.1/talondoc/shims/
--rw-r--r--   0 runner     (501) staff       (20)     1723 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/shims/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7755 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/shims/core.py
--rw-r--r--   0 runner     (501) staff       (20)     6548 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/shims/talon.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-03 23:06:28.815097 talondoc-0.1.1/talondoc/sphinx/
--rw-r--r--   0 runner     (501) staff       (20)      325 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-03 23:06:28.820906 talondoc-0.1.1/talondoc/sphinx/directives/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7645 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/abc.py
--rw-r--r--   0 runner     (501) staff       (20)      109 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/action.py
--rw-r--r--   0 runner     (501) staff       (20)      110 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/capture.py
--rw-r--r--   0 runner     (501) staff       (20)     1566 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/command.py
--rw-r--r--   0 runner     (501) staff       (20)     1510 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/command_hlist.py
--rw-r--r--   0 runner     (501) staff       (20)     1432 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/command_table.py
--rw-r--r--   0 runner     (501) staff       (20)      107 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/list.py
--rw-r--r--   0 runner     (501) staff       (20)      107 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/mode.py
--rw-r--r--   0 runner     (501) staff       (20)     1141 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/package.py
--rw-r--r--   0 runner     (501) staff       (20)      101 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/setting.py
--rw-r--r--   0 runner     (501) staff       (20)      106 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/tag.py
--rw-r--r--   0 runner     (501) staff       (20)      636 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/directives/user.py
--rw-r--r--   0 runner     (501) staff       (20)     4401 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/sphinx/domains.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-03 23:06:28.823617 talondoc-0.1.1/talondoc/util/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/util/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4421 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/util/desc.py
--rw-r--r--   0 runner     (501) staff       (20)     4738 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/util/describer.py
--rw-r--r--   0 runner     (501) staff       (20)      303 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/util/logging.py
--rw-r--r--   0 runner     (501) staff       (20)     3086 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/util/nodes.py
--rw-r--r--   0 runner     (501) staff       (20)      666 2022-09-03 23:05:48.000000 talondoc-0.1.1/talondoc/util/typing.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-03 23:06:28.811138 talondoc-0.1.1/talondoc.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      753 2022-09-03 23:06:28.000000 talondoc-0.1.1/talondoc.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1118 2022-09-03 23:06:28.000000 talondoc-0.1.1/talondoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-09-03 23:06:28.000000 talondoc-0.1.1/talondoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      226 2022-09-03 23:06:28.000000 talondoc-0.1.1/talondoc.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2022-09-03 23:06:28.000000 talondoc-0.1.1/talondoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-18 12:54:26.000000 talondoc-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-18 12:54:39.178819 talondoc-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-18 12:54:26.000000 talondoc-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-18 12:54:26.000000 talondoc-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:54:39.178819 talondoc-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 12:54:26.000000 talondoc-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.170819 talondoc-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/_autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/_autogen/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/conf.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/index.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/index.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/python_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/python_file.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/talon_file.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_autogen/resources/talon_file.rst.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/_cache_builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_cache_builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_util/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_util/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/analysis/live/
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/analysis/live/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/live/resources/talon_actions_dict-0.3.1-437-g8fea.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc/analysis/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/analysis/registry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/registry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/registry/data/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/registry/data/serialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/analysis/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/analysis/static/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/static/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/static/python/shims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/analysis/static/talon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/description/
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/description/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/description/describer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/sphinx/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/_util/addnodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/_util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/sphinx/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/capture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.178819 talondoc-0.5.1/src/talondoc/sphinx/directives/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/command/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/command/hlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/command/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/directives/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 12:54:26.000000 talondoc-0.5.1/src/talondoc/sphinx/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:54:39.174819 talondoc-0.5.1/src/talondoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 12:54:39.000000 talondoc-0.5.1/src/talondoc.egg-info/top_level.txt
```

### Comparing `talondoc-0.1.1/talondoc/analyze/__init__.py` & `talondoc-0.5.1/src/talondoc/analysis/static/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-import pathlib
-import typing
+from pathlib import Path
+from typing import Optional
 
-from ..entries import CallbackEntry, FileEntry, PackageEntry
-from ..shims import talon_shims
-from .python import analyse_python_file, python_package
-from .registry import Registry
-from .talon import analyse_talon_file
-from tree_sitter_talon import ParseError
+from ..registry import Registry
+from ..registry.data import Package
+from ..registry.data.abc import Location
+from .python import analyse_files as analyse_python_files
+from .talon import analyse_files as analyse_talon_files
 
-from ..util.logging import getLogger
 
-_logger = getLogger(__name__)
+def _include_file(
+    file_path: Path,
+    *,
+    include: tuple[str, ...] = (),
+    exclude: tuple[str, ...] = (),
+) -> bool:
+    return (
+        not exclude
+        or not any(file_path.match(exclude_pattern) for exclude_pattern in exclude)
+        or any(file_path.match(include_pattern) for include_pattern in include)
+    )
 
 
 def analyse_package(
     registry: Registry,
-    package_root: pathlib.Path,
+    package_dir: Path,
     *,
-    name: typing.Optional[str] = None,
+    package_name: Optional[str] = None,
     include: tuple[str, ...] = (),
     exclude: tuple[str, ...] = (),
     trigger: tuple[str, ...] = (),
-) -> PackageEntry:
-    def _include_file(
-        file_path: pathlib.Path,
-    ) -> bool:
-        return (
-            not exclude
-            or not any(file_path.match(exclude_pattern) for exclude_pattern in exclude)
-            or any(file_path.match(include_pattern) for include_pattern in include)
-        )
-
-    package_entry = PackageEntry(name=name, path=package_root.absolute())
-    with talon_shims(registry):
-        with python_package(package_entry):
-            for file_path in package_entry.path.glob("**/*"):
-                file_path = file_path.relative_to(package_entry.path)
-                if _include_file(file_path):
-                    try:
-                        analyse_file(registry, file_path, package_entry)
-                    except ParseError as e:
-                        _logger.exception(e)
-
-            # Register package:
-            registry.register(package_entry)
-
-            # Trigger callbacks:
-            for event_code in trigger:
-                callback_entries = typing.cast(
-                    list[CallbackEntry],
-                    registry.lookup(f"callback:{event_code}"),
-                )
-                for callback_entry in callback_entries:
-                    callback_entry.callback()
-
-    return package_entry
-
-
-def analyse_file(
-    registry: Registry, file_path: pathlib.Path, package_entry: PackageEntry
-) -> typing.Optional[FileEntry]:
-    if file_path.match("*.py"):
-        return analyse_python_file(registry, file_path, package_entry)
-    elif file_path.match("*.talon"):
-        return analyse_talon_file(registry, file_path, package_entry)
-    else:
-        return None
+    show_progress: bool = False,
+    continue_on_error: bool = True,
+) -> None:
+    # Activate the registry:
+    registry.activate()
+
+    # Retrieve or create package entry:
+    package = Package(
+        name=package_name or package_dir.parts[-1],
+        location=Location.from_path(package_dir.absolute()),
+    )
+    registry.register(package)
+    paths = [
+        path
+        for path in package.location.path.glob("**/*")
+        if _include_file(path, include=include, exclude=exclude)
+    ]
+
+    # Analyse Python files
+    python_paths = [
+        path for path in paths if path.is_file() and path.suffix.endswith(".py")
+    ]
+    analyse_python_files(
+        registry,
+        python_paths,
+        package,
+        trigger=trigger,
+        show_progress=show_progress,
+        continue_on_error=continue_on_error,
+    )
+
+    # Analyse Talon files
+    talon_paths = [
+        path for path in paths if path.is_file() and path.suffix.endswith(".talon")
+    ]
+    analyse_talon_files(
+        registry,
+        talon_paths,
+        package,
+        show_progress=show_progress,
+    )
+
+    # Deactivate the registry:
+    registry.deactivate()
```

### Comparing `talondoc-0.1.1/talondoc/sphinx/directives/abc.py` & `talondoc-0.5.1/src/talondoc/sphinx/directives/command/abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,232 +1,272 @@
-import typing
-from collections.abc import Iterator
+import re
+from typing import ClassVar, Iterator, Optional, Sequence, cast
 
-import sphinx.directives
 from docutils import nodes
 from sphinx import addnodes
-from talonfmt.main import talonfmt
+from talonfmt import talonfmt
 from tree_sitter_talon import TalonComment
-from tree_sitter_talon.re import compile
+from typing_extensions import final
 
-from ...analyze.registry import Registry
-from ...entries import CommandEntry, PackageEntry, TalonFileEntry
-from ...util.desc import InvalidInterpolation
-from ...util.describer import TalonScriptDescriber
-from ...util.logging import getLogger
-from ...util.nodes import desc_content, desc_name, paragraph
-
-_logger = getLogger(__name__)
-
-if typing.TYPE_CHECKING:
-    from talondoc.sphinx.domains import TalonDomain
-else:
-    TalonDomain = typing.Any
-
-
-class TalonDocDirective(sphinx.directives.SphinxDirective):
-    @property
-    def talon(self) -> TalonDomain:
-        return typing.cast(TalonDomain, self.env.get_domain("talon"))
-
-
-class TalonDocObjectDescription(sphinx.directives.ObjectDescription, TalonDocDirective):
-    pass
-
-
-def include_command(
-    candidate: CommandEntry,
-    sig: typing.Optional[str] = None,
-    *,
-    fullmatch: bool = True,
-    default: str = "include",
-    include: tuple[str, ...] = (),
-    exclude: tuple[str, ...] = (),
-    captures: dict[str, str] = {},
-    lists: dict[str, str] = {},
-):
-    assert default in ["include", "exclude"]
-    pattern = compile(candidate.ast.rule, captures=captures, lists=lists)
-
-    def match(sig: str) -> bool:
-        return bool(pattern.fullmatch(sig) if fullmatch else pattern.match(sig))
-
-    def excluded() -> bool:
-        return (
-            bool(exclude)
-            and any(match(exclude_sig) for exclude_sig in exclude)
-            and not any(match(include_sig) for include_sig in include)
-        )
-
-    def included() -> bool:
-        return any(match(include_sig) for include_sig in include) and not any(
-            match(exclude_sig) for exclude_sig in exclude
-        )
-
-    if default == "include":
-        return (not sig or match(sig)) and not excluded()
-    else:
-        return (sig and match(sig)) or included()
-
-
-def describe_rule(command: CommandEntry) -> nodes.Text:
-    return nodes.Text(talonfmt(command.ast.rule, safe=False))
-
-
-def try_describe_script_via_action_docstrings(
-    command: CommandEntry, *, registry: Registry
-) -> typing.Optional[nodes.Text]:
-    """
-    Describe the script using the docstrings on the actions used by the script.
-    """
-    try:
-        describer = TalonScriptDescriber(registry)
-        desc = describer.describe(command.ast)
-        if desc:
-            return nodes.Text(str(desc))
-    except InvalidInterpolation as e:
-        _logger.exception(e)
-    return None
-
-
-def try_describe_script_via_script_docstrings(
-    command: CommandEntry,
-) -> typing.Optional[nodes.Text]:
-    """
-    Describe the script using the docstrings present in the script itself.
-    """
-    comments = []
-    children = [*command.ast.children, *command.ast.script.children]
-    for child in children:
-        if isinstance(child, TalonComment):
-            comment = child.text.strip()
-            if comment.startswith("###"):
-                comments.append(comment.removeprefix("###").strip())
-    if comments:
-        return nodes.Text(" ".join(comments))
-    else:
-        return None
+from ...._util.logging import getLogger
+from ....analysis.registry import data
+from ....description import InvalidInterpolation
+from ....description.describer import TalonScriptDescriber
+from ....sphinx.directives import TalonDocObjectDescription
+from ....sphinx.typing import TalonDocstringHook_Callable
+from ..._util.addnodes import desc_content, desc_name, paragraph
+from ..errors import AmbiguousSignature, UnmatchedSignature
+
+_LOGGER = getLogger(__name__)
+
+
+class TalonDocCommandDescription(TalonDocObjectDescription):
+    @property
+    def contexts(self) -> Optional[Iterator[str]]:
+        result = [*self.options.get("context", []), *self.options.get("contexts", [])]
+        return iter(result) if result else None
+
+    @property
+    def always_include_script(self) -> bool:
+        return bool(self.options.get("always_include_script", False))
+
+    @final
+    def find_command(
+        self,
+        text: str,
+        *,
+        fullmatch: bool = False,
+        restrict_to: Optional[Iterator[str]] = None,
+    ) -> data.Command:
+        commands = list(
+            self.find_commands(text, fullmatch=fullmatch, restrict_to=restrict_to)
+        )
+        if len(commands) == 0:
+            raise UnmatchedSignature(self.get_location(), text)
+        if len(commands) >= 2:
+            raise AmbiguousSignature(
+                self.get_location(),
+                text,
+                [
+                    f"{command.location}: {talonfmt(command.rule, safe=False)}"
+                    for command in commands
+                ],
+            )
+        return commands[0]
+
+    @final
+    def get_commands(
+        self,
+        *,
+        restrict_to: Optional[Iterator[str]] = None,
+    ) -> Iterator[data.Command]:
+        yield from self.talon.registry.get_commands(restrict_to=restrict_to)
+
+    @final
+    def find_commands(
+        self,
+        text: str,
+        *,
+        fullmatch: bool = False,
+        restrict_to: Optional[Iterator[str]] = None,
+    ) -> Iterator[data.Command]:
+        _LOGGER.debug(
+            f"searching for commands matching '{text}' (restricted by {restrict_to})"
+        )
+        yield from self.talon.registry.find_commands(
+            self._split_phrase(text),
+            fullmatch=fullmatch,
+            restrict_to=restrict_to,
+        )
+
+    _RE_WHITESPACE: ClassVar[re.Pattern[str]] = re.compile(r"\s+")
 
+    @final
+    def _split_phrase(self, text: str) -> Sequence[str]:
+        return self.__class__._RE_WHITESPACE.split(text)
+
+    @final
+    def describe_command(
+        self,
+        command: data.Command,
+        signode: addnodes.desc_signature,
+        *,
+        always_include_script: bool,
+        docstring_hook: Optional[TalonDocstringHook_Callable],
+    ) -> addnodes.desc_signature:
+        signode += desc_name(self.describe_rule(command.rule))
+        signode += desc_content(
+            *self.describe_script(
+                command,
+                always_include_script=always_include_script,
+                docstring_hook=docstring_hook,
+            )
+        )
+        return signode
 
-def describe_script_via_code_block(command: CommandEntry) -> addnodes.highlightlang:
-    """
-    Describe the script by including it as a code block.
-    """
-    code = talonfmt(command.ast.script, safe=False)
-    literal_block = nodes.literal_block(code, code)
-    literal_block["language"] = "python"
-    return literal_block  # type: ignore
-
-
-def describe_script(
-    command: CommandEntry,
-    *,
-    registry: Registry,
-    include_script: bool = False,
-) -> list[nodes.Element]:
-    """
-    Describe the script using the docstrings on the script, the docstrings on
-    the actions, or finally by including it as a code block.
-    """
-    desc = try_describe_script_via_script_docstrings(command)
-    desc = desc or try_describe_script_via_action_docstrings(command, registry=registry)
-    buffer = []
-    if desc:
-        buffer.append(paragraph(nodes.Text(desc)))
-    if not desc or include_script:
-        buffer.append(describe_script_via_code_block(command))
-    return buffer
-
-
-def handle_command(
-    command: CommandEntry,
-    signode: addnodes.desc_signature,
-    *,
-    registry: Registry,
-    include_script: bool = False,
-) -> addnodes.desc_signature:
-    signode += desc_name(describe_rule(command))
-    signode += desc_content(
-        *describe_script(command, registry=registry, include_script=include_script)
-    )
-    return signode
-
-
-def describe_command(
-    command: CommandEntry, *, registry: Registry, include_script: bool = False
-) -> addnodes.desc_signature:
-    return handle_command(
-        command,
-        addnodes.desc_signature(),
-        registry=registry,
-        include_script=include_script,
-    )
-
-
-class TalonCommandListDirective(TalonDocDirective):
-    def find_package(self) -> PackageEntry:
-        namespace = self.options.get("package")
-        candidate = self.talon.currentpackage
-        if candidate and (not namespace or candidate.namespace == namespace):
-            return candidate
-        candidate = self.talon.packages.get(namespace, None)
-        if candidate:
-            return candidate
-        raise ValueError(f"Could not find package '{namespace}'")
-
-    def find_file(
-        self, sig: str, *, package_entry: typing.Optional[PackageEntry] = None
-    ) -> TalonFileEntry:
-        # Find the package:
-        if package_entry is None:
-            try:
-                package_entry = self.find_package()
-            except ValueError as e:
-                raise ValueError(f"Could not find file '{sig}'", e)
-
-        # Find the file:
-        for file in package_entry.files:
-            if isinstance(file, TalonFileEntry):
-                if (
-                    sig == file.name
-                    or sig == str(file.path)
-                    or f"{sig}.talon" == file.name
-                    or f"{sig}.talon" == str(file.path)
-                ):
-                    return file
-        raise ValueError(f"Could not find file '{sig}'")
-
-    def find_commands(self) -> Iterator[CommandEntry]:
-        exclude = self.options.get("exclude", ())
-        include = self.options.get("include", ())
-
-        if self.arguments:
-            # If file arguments were given, return all commands in that file
-            # which have not been explicitly excluded:
-            for sig in self.arguments:
-                default = self.options.get("default", "include")
-                for command in self.find_file(sig).commands:
-                    if include_command(
-                        command, default=default, exclude=exclude, include=include
-                    ):
-                        yield command
+    @final
+    def describe_rule(self, rule: data.Rule) -> nodes.Text:
+        return nodes.Text(talonfmt(rule, safe=False))
+
+    @final
+    def describe_script(
+        self,
+        command: data.Command,
+        *,
+        always_include_script: bool,
+        docstring_hook: Optional[TalonDocstringHook_Callable],
+    ) -> Sequence[nodes.Element]:
+        """
+        Describe the script using the docstrings on the script, the docstrings on
+        the actions, or finally by including it as a code block.
+        """
+        buffer = []
+
+        # 1. Use the Talon docstrings in the command script. Talon docstrings are comments which start with ###.
+        desc = self._try_describe_script_with_script_docstrings(command)
+
+        # 2. Use the Python docstrings from the actions used in the command script.
+        if desc is None:
+            desc = self._try_describe_script_with_action_docstrings(
+                command, docstring_hook=docstring_hook
+            )
+
+        # Append the description.
+        if desc is not None:
+            buffer.append(paragraph(nodes.Text(str(desc))))
+
+        if desc is None or always_include_script:
+            # 3. Include the command script.
+            buffer.append(self._describe_script_with_script(command))
+
+        return buffer
+
+    @final
+    def _try_describe_script_with_script_docstrings(
+        self,
+        command: data.Command,
+    ) -> Optional[nodes.Text]:
+        """
+        Describe the script using the docstrings present in the script itself.
+        """
+        comments = []
+        for child in command.script.children:
+            if isinstance(child, TalonComment):
+                comment = child.text.strip()
+                if comment.startswith("###"):
+                    comments.append(comment.removeprefix("###").strip())
+        if comments:
+            return nodes.Text(" ".join(comments))
         else:
-            # If no file arguments were given, return all commands in the package
-            # which have been explicitly included:
-            default = self.options.get("default", "exclude")
-            for command in self.talon.commands:
-                if include_command(
-                    command, default=default, exclude=exclude, include=include
-                ):
-                    yield command
-
-    def caption(self) -> Iterator[str]:
-        # Get caption from options
-        caption = self.options.get("caption", None)
-        if caption:
-            yield caption
-            return
-        # Get caption from file name
-        if len(self.arguments) == 1:
-            file = self.find_file(self.arguments[0])
-            yield file.name.removesuffix(".talon")
-            return
+            return None
+
+    @final
+    def _try_describe_script_with_action_docstrings(
+        self,
+        command: data.Command,
+        *,
+        docstring_hook: Optional[TalonDocstringHook_Callable],
+    ) -> Optional[nodes.Text]:
+        """
+        Describe the script using the docstrings on the actions used by the script.
+        """
+        try:
+            describer = TalonScriptDescriber(
+                self.talon.registry, docstring_hook=docstring_hook
+            )
+            desc = describer.describe(command.script)
+            if desc:
+                return nodes.Text(str(desc))
+        except InvalidInterpolation as e:
+            _LOGGER.exception(e)
+        return None
+
+    @final
+    def _describe_script_with_script(
+        self, command: data.Command
+    ) -> nodes.literal_block:
+        """
+        Describe the script by including it as a code block.
+        """
+        code = talonfmt(command.script, safe=False)
+        literal_block = nodes.literal_block(code, code)
+        literal_block["language"] = "python"
+        return literal_block
+
+
+class TalonDocCommandListDescription(TalonDocCommandDescription):
+    @property
+    def caption(self) -> str:
+        # Get caption from options or from file name
+        return cast(str, self.options.get("caption", None) or ".".join(self.arguments))
+
+    @property
+    def include(self) -> Sequence[Sequence[str]]:
+        return tuple(
+            self._split_phrase(phrase) for phrase in self.options.get("include", ())
+        )
+
+    @property
+    def exclude(self) -> Sequence[Sequence[str]]:
+        return tuple(
+            self._split_phrase(phrase) for phrase in self.options.get("exclude", ())
+        )
+
+    @property
+    def columns(self) -> int:
+        return cast(int, self.options.get("columns", 2))
+
+    @property
+    def commands(self) -> Iterator[data.Command]:
+        for command in self.get_commands(restrict_to=self.contexts):
+            if self._should_include(command.rule):
+                yield command
+
+    def _should_include(
+        self,
+        rule: data.Rule,
+        *,
+        fullmatch: bool = False,
+    ) -> bool:
+        # If both :include: and :exclude:
+        # Does command match :include: and not match :exclude:?
+        # If :include: but no :exclude:
+        # Does command match :include:?
+        # If :exclude: but no :include:
+        # Does command not match exclude?
+        _should_include = self._matches_include(rule, fullmatch=fullmatch)
+        _should_exclude = self._matches_exclude(rule, fullmatch=fullmatch)
+        return _should_include and not _should_exclude
+
+    @final
+    def _matches_include(
+        self,
+        rule: data.Rule,
+        *,
+        fullmatch: bool = False,
+    ) -> bool:
+        return self._match_any_of(rule, self.include, default=True, fullmatch=fullmatch)
+
+    @final
+    def _matches_exclude(
+        self,
+        rule: data.Rule,
+        *,
+        fullmatch: bool = False,
+    ) -> bool:
+        return self._match_any_of(
+            rule, self.exclude, default=False, fullmatch=fullmatch
+        )
+
+    @final
+    def _match_any_of(
+        self,
+        rule: data.Rule,
+        phrases: Sequence[Sequence[str]],
+        *,
+        default: bool,
+        fullmatch: bool = False,
+    ) -> bool:
+        return any(
+            self.talon.registry.match(phrase, rule, fullmatch=fullmatch)
+            for phrase in phrases
+        )
```

### Comparing `talondoc-0.1.1/talondoc/sphinx/directives/command_hlist.py` & `talondoc-0.5.1/src/talondoc/sphinx/directives/command/table.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 import sys
 
 from docutils import nodes
-from sphinx import addnodes
 from sphinx.util.typing import OptionSpec
 
-from ...util.logging import getLogger
-from ...util.nodes import bullet_list, title
-from ...util.typing import optional_str, optional_strlist
-from .abc import TalonCommandListDirective, describe_command
+from ...._util.logging import getLogger
+from ..._util.addnodes import colspec, entry, row, table, tbody, tgroup, title
+from ..._util.typing import flag, optional_str, optional_strlist
+from .abc import TalonDocCommandListDescription
 
-_logger = getLogger(__name__)
+_LOGGER = getLogger(__name__)
 
 
-class TalonCommandHListDirective(TalonCommandListDirective):
-
+class TalonCommandTableDirective(TalonDocCommandListDescription):
     has_content = False
     required_arguments = 0
     optional_arguments = sys.maxsize
     option_spec: OptionSpec = {
-        "package": optional_str,
+        "context": optional_strlist,
+        "contexts": optional_strlist,
+        "always_include_script": flag,
         "caption": optional_str,
-        "default": optional_str,
         "include": optional_strlist,
         "exclude": optional_strlist,
-        "columns": int,
     }
     final_argument_whitespace = False
 
     def run(self) -> list[nodes.Node]:
-        ncolumns = self.options.get("columns", 2)
-        fulllist = [
-            describe_command(command, registry=self.talon)
-            for command in self.find_commands()
+        return [
+            table(
+                title(nodes.Text(self.caption)),
+                tgroup(
+                    colspec(colwidth=1),
+                    colspec(colwidth=1),
+                    tbody(
+                        row(
+                            entry(self.describe_rule(command.rule)),
+                            entry(
+                                *self.describe_script(
+                                    command,
+                                    always_include_script=self.always_include_script,
+                                    docstring_hook=self.docstring_hook,
+                                )
+                            ),
+                        )
+                        for command in self.commands
+                    ),
+                    cols=2,
+                ),
+                classes="compact",
+            )
         ]
-        # create a hlist node where the items are distributed
-        # (source: sphinx.directives.other.HList)
-        npercol, nmore = divmod(len(fulllist), ncolumns)
-        index = 0
-        hlist = addnodes.hlist()
-        hlist["ncolumns"] = str(ncolumns)
-        for column in range(ncolumns):
-            endindex = index + ((npercol + 1) if column < nmore else npercol)
-            hlist += addnodes.hlistcol("", bullet_list(*fulllist[index:endindex]))
-            index = endindex
-        return [hlist]
```

### Comparing `talondoc-0.1.1/talondoc/sphinx/directives/package.py` & `talondoc-0.5.1/src/talondoc/sphinx/directives/command/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-from pathlib import Path
+import sys
+from typing import List
 
-from docutils.nodes import Element
+from sphinx import addnodes
 from sphinx.util.typing import OptionSpec
+from typing_extensions import override
 
-from ...analyze import analyse_package
-from ...util.typing import optional_str, optional_strlist
-from .abc import TalonDocDirective
+from ...._util.logging import getLogger
+from ..._util.typing import flag, optional_strlist
+from ..errors import AmbiguousSignature, UnmatchedSignature
+from .abc import TalonDocCommandDescription
 
+_LOGGER = getLogger(__name__)
 
-class TalonPackageDirective(TalonDocDirective):
 
-    has_content = False
+class TalonCommandDirective(TalonDocCommandDescription):
+    has_content = True
     required_arguments = 1
-    optional_arguments = 0
+    optional_arguments = sys.maxsize
     option_spec: OptionSpec = {
-        "name": optional_str,
-        "include": optional_strlist,
-        "exclude": optional_strlist,
-        "trigger": optional_strlist,
+        "context": optional_strlist,
+        "contexts": optional_strlist,
+        "always_include_script": flag,
     }
     final_argument_whitespace = False
 
-    def run(self) -> list[Element]:
-
-        # Always reread documents with Talon package directives.
-        self.env.note_reread()
-
-        # Analyse the referenced Talon package:
-        analyse_package(
-            registry=self.talon,
-            package_root=Path(self.arguments[0].strip()),
-            name=self.options.get("name", "user"),
-            include=tuple(self.options.get("include", ())),
-            exclude=tuple(self.options.get("exclude", ())),
-            trigger=tuple(self.options.get("trigger", ())),
-        )
-
-        return []
+    @override
+    def get_signatures(self) -> List[str]:
+        return [" ".join(self.arguments)]
+
+    @override
+    def handle_signature(self, sig: str, signode: addnodes.desc_signature):
+        try:
+            command = self.find_command(sig, fullmatch=False, restrict_to=self.contexts)
+            signode = self.describe_command(
+                command,
+                signode,
+                always_include_script=self.always_include_script,
+                docstring_hook=self.docstring_hook,
+            )
+            return command.name
+        except (UnmatchedSignature, AmbiguousSignature) as e:
+            _LOGGER.error(e)
+            raise ValueError(e)
```

### Comparing `talondoc-0.1.1/talondoc/util/desc.py` & `talondoc-0.5.1/src/talondoc/description/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,95 @@
-import collections.abc
 import dataclasses
 import re
-import typing
+from collections.abc import Iterable
+from typing import Optional, Union
 
-import docstring_parser.google as docstring_google
+import docstring_parser
 
-from ..util.logging import getLogger
+from .._util.logging import getLogger
 
-_logger = getLogger(__name__)
+_LOGGER = getLogger(__name__)
 
 
 @dataclasses.dataclass
 class InvalidInterpolation(Exception):
     """Exception raised when attempting to interpolate a multiline doc string."""
 
-    argument: typing.Optional["Desc"]
-    template: typing.Optional["StepsTemplate"] = None
+    argument: Optional["Description"]
+    template: Optional["StepsTemplate"] = None
 
     def __str__(self) -> str:
         msg = f"Cannot interpolate '{repr(self.argument)}'"
         if self.template:
             msg += f" into template '{repr(self.template)}'"
         return msg
 
 
-class Desc:
+class Description:
     def as_steps(self) -> "Steps":
         """
         Lift a description to steps.
         """
+        return Steps(())
 
 
-DescLike = typing.Union[None, str, Desc, collections.abc.Iterable[Desc]]
+DescLike = Union[None, str, Description, Iterable[Description]]
 
 
-@dataclasses.dataclass(frozen=True)
-class Value(Desc):
+@dataclasses.dataclass
+class Value(Description):
     """
     The description of a value.
     """
 
     desc: str
 
     def __str__(self) -> str:
         return self.desc
 
     def as_steps(self) -> "Steps":
         return Steps(steps=(Step(self),))
 
 
-@dataclasses.dataclass(frozen=True)
-class Step(Desc):
+@dataclasses.dataclass
+class Step(Description):
     """
     The description of one step in a series of steps.
     """
 
-    desc: typing.Union[str, Value]
+    desc: Union[str, Value]
 
     def __str__(self) -> str:
         return str(self.desc)
 
     def as_steps(self) -> "Steps":
         return Steps(steps=(self,))
 
 
-@dataclasses.dataclass(frozen=True)
-class Steps(Desc):
+@dataclasses.dataclass
+class Steps(Description):
     """
     The description of a series of steps.
     """
 
     steps: tuple[Step, ...] = dataclasses.field(default_factory=tuple)
 
     def __str__(self) -> str:
         return "\n".join(str(step) for step in self.steps)
 
     def as_steps(self) -> "Steps":
         return self
 
 
 @dataclasses.dataclass
-class StepsTemplate(Desc):
+class StepsTemplate(Description):
     template: str
     names: tuple[str, ...]
 
-    def __call__(self, values: tuple[typing.Optional[Desc], ...]) -> Steps:
+    def __call__(self, values: tuple[Optional[Description], ...]) -> Steps:
         ret = self.template
         for name, value in zip(self.names, values):
             if isinstance(value, Value):
                 ret = ret.replace(f"<{name}>", value.desc)
             else:
                 raise InvalidInterpolation(argument=value, template=self)
         return Steps(steps=tuple(Step(desc=desc) for desc in ret.splitlines()))
@@ -97,54 +98,54 @@
         return self.template
 
     def as_steps(self) -> "Steps":
         return Steps(steps=(Step(desc=str(self)),))
 
 
 def and_then(
-    desc1: typing.Optional[Desc], desc2: typing.Optional[Desc]
-) -> typing.Optional[Desc]:
+    desc1: Optional[Description], desc2: Optional[Description]
+) -> Optional[Description]:
     if desc1 is None:
         return desc2
     elif desc2 is None:
         return desc1
     elif isinstance(desc1, Value) and isinstance(desc2, Value):
         return Value(f"{desc1} {desc2}")
     else:
         return Steps(steps=(*desc1.as_steps().steps, *desc2.as_steps().steps))
 
 
-def concat(*desclike: DescLike) -> typing.Optional[Desc]:
-    ret: typing.Optional[Desc] = None
+def concat(*desclike: DescLike) -> Optional[Description]:
+    ret: Optional[Description] = None
     for desc in desclike:
         if desc is None:
             pass
         elif isinstance(desc, str):
             ret = and_then(ret, Step(desc))
-        elif isinstance(desc, Desc):
+        elif isinstance(desc, Description):
             ret = and_then(ret, desc)
         else:
             ret = and_then(ret, concat(*desc))
     return ret
 
 
-def from_docstring(docstring: str) -> typing.Optional[Desc]:
+def from_docstring(docstring: str) -> Optional[Description]:
     # Attempt to create a description:
-    desc: typing.Optional[Desc]
+    desc: Optional[Description]
 
     # Handle docstrings of the form "Return XXX":
     return_value_desc_en = re.match("^[Rr]eturns? (.*)", docstring)
     if return_value_desc_en:
         desc = Value(desc=return_value_desc_en.group(0))
         return desc
 
     # Handle Google-style docstrings:
     try:
         # Parse a Google-style docstring:
-        doc = docstring_google.parse(docstring)
+        doc = docstring_parser.parse(docstring)
 
         # Actions which document their parameters become
         # step templates that can interpolate their arguments:
         if doc.short_description and len(doc.params) > 0:
             desc = StepsTemplate(
                 template=doc.short_description,
                 names=tuple(param.arg_name for param in doc.params),
@@ -153,13 +154,13 @@
 
         # Actions which document their return values become
         # value descriptions that can be used inline:
         if doc.returns and doc.returns.description:
             desc = Value(desc=doc.returns.description)
             return desc
 
-    except docstring_google.ParseError as e:
+    except docstring_parser.ParseError as e:
         pass
 
     # Treat the docstring as a series of steps:
     desc = concat(*docstring.splitlines())
     return desc
```

### Comparing `talondoc-0.1.1/talondoc/util/describer.py` & `talondoc-0.5.1/src/talondoc/description/describer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import dataclasses
-import typing
+from collections.abc import Callable
 from functools import singledispatchmethod
+from typing import Optional, TypeVar
 
 from tree_sitter_talon import (
     Node,
     TalonAction,
     TalonAssignmentStatement,
     TalonBinaryOperator,
     TalonBlock,
@@ -20,136 +20,133 @@
     TalonSleepAction,
     TalonString,
     TalonStringContent,
     TalonStringEscapeSequence,
     TalonVariable,
 )
 
-from talondoc.entries import ActionGroupEntry
+from .._util.logging import getLogger
+from ..analysis.registry import Registry, data
+from ..analysis.registry.data.abc import Data
+from . import Description, Step, StepsTemplate, Value, concat, from_docstring
 
-from ..analyze.registry import Registry
-from ..util.logging import getLogger
-from .desc import Desc, Step, StepsTemplate, Value, concat, from_docstring
-
-_logger = getLogger(__name__)
-
-
-NodeVar = typing.TypeVar("NodeVar", bound=Node)
-
-
-def _only_child(
-    children: typing.Sequence[typing.Union[NodeVar, TalonComment]]
-) -> NodeVar:
-    ret: typing.Optional[NodeVar] = None
-    for child in children:
-        if not isinstance(child, TalonComment):
-            if __debug__ and ret:
-                raise AssertionError(f"Multiple non-comments in {children}.")
-            ret = child
-            if not __debug__:
-                break
-    if ret is None:
-        raise AssertionError(f"Only comments in {children}.")
-    return ret
+_LOGGER = getLogger(__name__)
+
+
+NodeVar = TypeVar("NodeVar", bound=Node)
 
 
 class TalonScriptDescriber:
-    def __init__(self, registry: Registry) -> None:
+    def __init__(
+        self,
+        registry: Registry,
+        *,
+        docstring_hook: Optional[Callable[[str, str], Optional[str]]] = None,
+    ) -> None:
         self.registry = registry
+        self.docstring_hook = docstring_hook or (lambda clsname, name: None)
 
     @singledispatchmethod
-    def describe(self, ast: Node) -> typing.Optional[Desc]:
+    def describe(self, ast: Node) -> Optional[Description]:
         raise TypeError(type(ast))
 
     @describe.register
-    def _(self, ast: TalonCommandDeclaration) -> typing.Optional[Desc]:
-        return self.describe(ast.script)
+    def _(self, ast: TalonCommandDeclaration) -> Optional[Description]:
+        return self.describe(ast.right)
 
     @describe.register
-    def _(self, ast: TalonBlock) -> typing.Optional[Desc]:
+    def _(self, ast: TalonBlock) -> Optional[Description]:
         buffer = []
         for child in ast.children:
             buffer.append(self.describe(child))
         return concat(*buffer)
 
     @describe.register
-    def _(self, ast: TalonExpressionStatement) -> typing.Optional[Desc]:
-        return self.describe(ast.expression)
+    def _(self, ast: TalonExpressionStatement) -> Optional[Description]:
+        desc = self.describe(ast.expression)
+        if isinstance(ast.expression, TalonString):
+            return Step(desc=f'Insert "{desc}"')
+        return desc
 
     @describe.register
-    def _(self, ast: TalonAssignmentStatement) -> typing.Optional[Desc]:
+    def _(self, ast: TalonAssignmentStatement) -> Optional[Description]:
         right = self.describe(ast.right)
         return Step(f"Let <{ast.left.text}> be {right}")
 
     @describe.register
-    def _(self, ast: TalonBinaryOperator) -> typing.Optional[Desc]:
+    def _(self, ast: TalonBinaryOperator) -> Optional[Description]:
         left = self.describe(ast.left)
         right = self.describe(ast.right)
         return Value(f"{left} {ast.operator.text} {right}")
 
     @describe.register
-    def _(self, ast: TalonVariable) -> typing.Optional[Desc]:
+    def _(self, ast: TalonVariable) -> Optional[Description]:
         return Value(f"<{ast.text}>")
 
     @describe.register
-    def _(self, ast: TalonKeyAction) -> typing.Optional[Desc]:
+    def _(self, ast: TalonKeyAction) -> Optional[Description]:
         return Step(f"Press {ast.arguments.text.strip()}.")
 
     @describe.register
-    def _(self, ast: TalonSleepAction, **kwargs) -> typing.Optional[Desc]:
+    def _(self, ast: TalonSleepAction, **kwargs) -> Optional[Description]:
         return None
 
+    def get_docstring(
+        self,
+        cls: type[Data],
+        name: str,
+    ) -> Optional[str]:
+        # Try the docstring_hook:
+        docstring = self.docstring_hook(cls.__name__, name)
+        # Try the registry:
+        docstring = docstring or self.registry.lookup_description(cls, name)
+        return docstring
+
     @describe.register
-    def _(self, ast: TalonAction) -> typing.Optional[Desc]:
+    def _(self, ast: TalonAction) -> Optional[Description]:
         # TODO: resolve self.*
-        action_group_entry = typing.cast(
-            typing.Optional[ActionGroupEntry],
-            self.registry.lookup(f"action-group:{ast.action_name.text}"),
-        )
-        if (
-            action_group_entry
-            and action_group_entry.default
-            and action_group_entry.default.desc
-        ):
-            desc = from_docstring(action_group_entry.default.desc)
+        name = ast.action_name.text
+        docstring = self.get_docstring(data.Action, name)
+        if docstring:
+            desc = from_docstring(docstring)
             if isinstance(desc, StepsTemplate):
                 desc = desc(
                     tuple(
                         self.describe(arg)
                         for arg in ast.arguments.children
                         if isinstance(arg, TalonExpression)
                     )
                 )
             return desc
         return None
 
     @describe.register
-    def _(self, ast: TalonParenthesizedExpression) -> typing.Optional[Desc]:
-        return self.describe(_only_child(ast.children))
+    def _(self, ast: TalonParenthesizedExpression) -> Optional[Description]:
+        return self.describe(ast.get_child())
 
     @describe.register
-    def _(self, ast: TalonComment) -> typing.Optional[Desc]:
+    def _(self, ast: TalonComment) -> Optional[Description]:
         return None
 
     @describe.register
-    def _(self, ast: TalonInteger) -> typing.Optional[Desc]:
+    def _(self, ast: TalonInteger) -> Optional[Description]:
         return Value(ast.text)
 
     @describe.register
-    def _(self, ast: TalonFloat) -> typing.Optional[Desc]:
+    def _(self, ast: TalonFloat) -> Optional[Description]:
         return Value(ast.text)
 
     @describe.register
-    def _(self, ast: TalonImplicitString) -> typing.Optional[Desc]:
+    def _(self, ast: TalonImplicitString) -> Optional[Description]:
         return Value(ast.text)
 
     @describe.register
-    def _(self, ast: TalonString) -> typing.Optional[Desc]:
+    def _(self, ast: TalonString) -> Optional[Description]:
         return concat(*(self.describe(child) for child in ast.children))
 
     @describe.register
-    def _(self, ast: TalonStringContent) -> typing.Optional[Desc]:
+    def _(self, ast: TalonStringContent) -> Optional[Description]:
         return Value(ast.text)
 
     @describe.register
-    def _(self, ast: TalonStringEscapeSequence) -> typing.Optional[Desc]:
+    def _(self, ast: TalonStringEscapeSequence) -> Optional[Description]:
         return Value(ast.text)
```

### Comparing `talondoc-0.1.1/talondoc/util/nodes.py` & `talondoc-0.5.1/src/talondoc/sphinx/_util/addnodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 
 def _with_children_and_attributes(
     node: NodeVar, *children: NodeLike, **attributes: AttributeValue
 ) -> NodeVar:
     for child in children:
         if isinstance(child, nodes.Node):
-            node += child  # type: ignore
+            node += child  # type: ignore[operator]
         else:
             for grandchild in child:
-                node += grandchild  # type: ignore
+                node += grandchild  # type: ignore[operator]
     for attribute_name, attribute_value in attributes.items():
         if isinstance(attribute_value, Sequence):
-            node[attribute_name].append(attribute_value)  # type: ignore
+            node[attribute_name].append(attribute_value)  # type: ignore[index]
         else:
-            node[attribute_name] = attribute_value  # type: ignore
+            node[attribute_name] = attribute_value  # type: ignore[index]
     return node
 
 
 def desc_name(*children: NodeLike, **attributes: AttributeValue) -> addnodes.desc_name:
     return _with_children_and_attributes(addnodes.desc_name(), *children, **attributes)
```

