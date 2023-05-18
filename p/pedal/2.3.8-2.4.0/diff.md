# Comparing `tmp/pedal-2.3.8.tar.gz` & `tmp/pedal-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedal-2.3.8.tar", last modified: Tue Jun 29 12:28:23 2021, max compression
+gzip compressed data, was "pedal-2.4.0.tar", last modified: Thu May 18 18:37:44 2023, max compression
```

## Comparing `pedal-2.3.8.tar` & `pedal-2.4.0.tar`

### file list

```diff
@@ -1,136 +1,154 @@
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:23.138303 pedal-2.3.8/
--rw-rw-rw-   0        0        0     2924 2021-06-29 12:28:23.138303 pedal-2.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:21.816761 pedal-2.3.8/Pedal.egg-info/
--rw-rw-rw-   0        0        0     2924 2021-06-29 12:28:21.000000 pedal-2.3.8/Pedal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3217 2021-06-29 12:28:21.000000 pedal-2.3.8/Pedal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-29 12:28:21.000000 pedal-2.3.8/Pedal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2021-06-29 12:28:21.000000 pedal-2.3.8/Pedal.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2021-06-29 12:28:21.000000 pedal-2.3.8/Pedal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-06-29 12:28:21.000000 pedal-2.3.8/Pedal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1901 2020-10-17 19:58:17.000000 pedal-2.3.8/README.rst
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:21.803792 pedal-2.3.8/pedal/
--rw-rw-rw-   0        0        0      352 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/__main__.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:21.963366 pedal-2.3.8/pedal/assertions/
--rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/assertions/__init__.py
--rw-rw-rw-   0        0        0     3197 2021-03-17 16:46:42.000000 pedal-2.3.8/pedal/assertions/commands.py
--rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/assertions/constants.py
--rw-rw-rw-   0        0        0    20063 2021-06-29 12:25:15.000000 pedal-2.3.8/pedal/assertions/feedbacks.py
--rw-rw-rw-   0        0        0     7167 2020-12-05 02:26:27.000000 pedal-2.3.8/pedal/assertions/functions.py
--rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.3.8/pedal/assertions/organizers.py
--rw-rw-rw-   0        0        0    29143 2021-06-28 18:36:37.000000 pedal-2.3.8/pedal/assertions/runtime.py
--rw-rw-rw-   0        0        0     3254 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/assertions/setup.py
--rw-rw-rw-   0        0        0    24144 2020-10-22 05:57:53.000000 pedal-2.3.8/pedal/assertions/static.py
--rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/assertions/unittest.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.109973 pedal-2.3.8/pedal/cait/
--rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.3.8/pedal/cait/__init__.py
--rw-rw-rw-   0        0        0     2254 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/cait/ast_helpers.py
--rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.3.8/pedal/cait/ast_map.py
--rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.3.8/pedal/cait/cait_api.py
--rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/cait/cait_node.py
--rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/cait/constants.py
--rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.3.8/pedal/cait/find_node.py
--rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.3.8/pedal/cait/stretchy_tree_matching.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.176796 pedal-2.3.8/pedal/command_line/
--rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/command_line/__init__.py
--rw-rw-rw-   0        0        0     7886 2021-02-26 19:20:58.000000 pedal-2.3.8/pedal/command_line/command_line.py
--rw-rw-rw-   0        0        0     7493 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/command_line/mocks.py
--rw-rw-rw-   0        0        0    23734 2021-06-29 12:25:34.000000 pedal-2.3.8/pedal/command_line/modes.py
--rw-rw-rw-   0        0        0     3365 2021-05-27 16:08:59.000000 pedal-2.3.8/pedal/command_line/report.py
--rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.3.8/pedal/command_line/verify.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.321485 pedal-2.3.8/pedal/core/
--rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/core/__init__.py
--rw-rw-rw-   0        0        0     8152 2020-11-14 02:23:58.000000 pedal-2.3.8/pedal/core/commands.py
--rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/core/environment.py
--rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/core/errors.py
--rw-rw-rw-   0        0        0    17328 2020-12-09 16:59:44.000000 pedal-2.3.8/pedal/core/feedback.py
--rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/core/feedback_category.py
--rw-rw-rw-   0        0        0     5042 2021-03-27 20:21:20.000000 pedal-2.3.8/pedal/core/final_feedback.py
--rw-rw-rw-   0        0        0     7245 2021-02-04 21:29:35.000000 pedal-2.3.8/pedal/core/formatting.py
--rw-rw-rw-   0        0        0     1770 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/core/location.py
--rw-rw-rw-   0        0        0    12979 2021-01-26 19:25:08.000000 pedal-2.3.8/pedal/core/report.py
--rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/core/resolver.py
--rw-rw-rw-   0        0        0     3745 2021-04-02 19:26:30.000000 pedal-2.3.8/pedal/core/scoring.py
--rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.3.8/pedal/core/submission.py
--rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/core/tag.py
--rw-rw-rw-   0        0        0     2588 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/core/tool.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.407256 pedal-2.3.8/pedal/environments/
--rw-rw-rw-   0        0        0      657 2020-11-08 17:16:23.000000 pedal-2.3.8/pedal/environments/__init__.py
--rw-rw-rw-   0        0        0     3042 2021-02-26 19:18:08.000000 pedal-2.3.8/pedal/environments/blockpy.py
--rw-rw-rw-   0        0        0     9666 2021-04-30 18:58:54.000000 pedal-2.3.8/pedal/environments/gradescope.py
--rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.3.8/pedal/environments/jupyter.py
--rw-rw-rw-   0        0        0    10351 2021-02-02 16:30:22.000000 pedal-2.3.8/pedal/environments/nbgrader.py
--rw-rw-rw-   0        0        0      368 2020-11-08 17:19:12.000000 pedal-2.3.8/pedal/environments/none.py
--rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/environments/sandbox.py
--rw-rw-rw-   0        0        0     3650 2021-06-28 17:08:38.000000 pedal-2.3.8/pedal/environments/standard.py
--rw-rw-rw-   0        0        0     6259 2020-11-13 04:58:08.000000 pedal-2.3.8/pedal/environments/vpl.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.432189 pedal-2.3.8/pedal/extensions/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/extensions/__init__.py
--rw-rw-rw-   0        0        0     9562 2020-10-22 09:20:21.000000 pedal-2.3.8/pedal/extensions/plotting.py
--rw-rw-rw-   0        0        0      643 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/extensions/turtles.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.505993 pedal-2.3.8/pedal/questions/
--rw-rw-rw-   0        0        0      566 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/questions/__init__.py
--rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/questions/constants.py
--rw-rw-rw-   0        0        0     4347 2020-10-17 18:51:03.000000 pedal-2.3.8/pedal/questions/graders.py
--rw-rw-rw-   0        0        0    21620 2020-10-17 18:50:35.000000 pedal-2.3.8/pedal/questions/loader.py
--rw-rw-rw-   0        0        0     2319 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/questions/pool.py
--rw-rw-rw-   0        0        0     2110 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/questions/questions.py
--rw-rw-rw-   0        0        0     1602 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/questions/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.573849 pedal-2.3.8/pedal/resolvers/
--rw-rw-rw-   0        0        0     1015 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/resolvers/__init__.py
--rw-rw-rw-   0        0        0      654 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/resolvers/core.py
--rw-rw-rw-   0        0        0     1786 2021-04-18 15:06:27.000000 pedal-2.3.8/pedal/resolvers/full.py
--rw-rw-rw-   0        0        0     1949 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/resolvers/sectional.py
--rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.3.8/pedal/resolvers/silent.py
--rw-rw-rw-   0        0        0     5119 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/resolvers/simple.py
--rw-rw-rw-   0        0        0     1176 2020-11-03 17:24:20.000000 pedal-2.3.8/pedal/resolvers/statistics.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.707454 pedal-2.3.8/pedal/sandbox/
--rw-rw-rw-   0        0        0      625 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/sandbox/__init__.py
--rw-rw-rw-   0        0        0    15988 2021-02-04 19:02:04.000000 pedal-2.3.8/pedal/sandbox/commands.py
--rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/sandbox/constants.py
--rw-rw-rw-   0        0        0     8121 2020-10-20 19:37:49.000000 pedal-2.3.8/pedal/sandbox/data.py
--rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.3.8/pedal/sandbox/exceptions.py
--rw-rw-rw-   0        0        0    10515 2020-10-17 21:03:41.000000 pedal-2.3.8/pedal/sandbox/feedbacks.py
--rw-rw-rw-   0        0        0    16478 2021-02-26 17:01:01.000000 pedal-2.3.8/pedal/sandbox/mocked.py
--rw-rw-rw-   0        0        0    14838 2021-03-10 20:46:13.000000 pedal-2.3.8/pedal/sandbox/result.py
--rw-rw-rw-   0        0        0    34366 2021-06-28 19:11:03.000000 pedal-2.3.8/pedal/sandbox/sandbox.py
--rw-rw-rw-   0        0        0     5048 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/sandbox/timeout.py
--rw-rw-rw-   0        0        0     4997 2021-06-28 19:01:22.000000 pedal-2.3.8/pedal/sandbox/tracer.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.775273 pedal-2.3.8/pedal/source/
--rw-rw-rw-   0        0        0      871 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/source/__init__.py
--rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/source/constants.py
--rw-rw-rw-   0        0        0     4558 2021-02-04 17:32:32.000000 pedal-2.3.8/pedal/source/feedbacks.py
--rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/source/sections.py
--rw-rw-rw-   0        0        0     7085 2021-02-04 17:30:12.000000 pedal-2.3.8/pedal/source/source.py
--rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/source/substitutions.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.885978 pedal-2.3.8/pedal/tifa/
--rw-rw-rw-   0        0        0     2802 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/tifa/__init__.py
--rw-rw-rw-   0        0        0     1544 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/tifa/commands.py
--rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/tifa/constants.py
--rw-rw-rw-   0        0        0     2632 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/tifa/contexts.py
--rw-rw-rw-   0        0        0    19757 2020-11-08 17:26:34.000000 pedal-2.3.8/pedal/tifa/feedbacks.py
--rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/tifa/identifier.py
--rw-rw-rw-   0        0        0     3496 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/tifa/state.py
--rw-rw-rw-   0        0        0    22386 2021-03-12 16:41:54.000000 pedal-2.3.8/pedal/tifa/tifa_core.py
--rw-rw-rw-   0        0        0    38694 2020-11-03 15:01:53.000000 pedal-2.3.8/pedal/tifa/tifa_visitor.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:22.944820 pedal-2.3.8/pedal/types/
--rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/types/__init__.py
--rw-rw-rw-   0        0        0    11385 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/types/builtin.py
--rw-rw-rw-   0        0        0    20286 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/types/definitions.py
--rw-rw-rw-   0        0        0    12726 2020-11-02 19:33:45.000000 pedal-2.3.8/pedal/types/normalize.py
--rw-rw-rw-   0        0        0     6447 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/types/operations.py
-drwxrwxrwx   0        0        0        0 2021-06-29 12:28:23.136308 pedal-2.3.8/pedal/utilities/
--rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/utilities/__init__.py
--rw-rw-rw-   0        0        0     6335 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/utilities/ast_tools.py
--rw-rw-rw-   0        0        0     6171 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/utilities/comparisons.py
--rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/utilities/dictionaries.py
--rw-rw-rw-   0        0        0     8208 2020-10-27 16:45:39.000000 pedal-2.3.8/pedal/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.3.8/pedal/utilities/files.py
--rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/utilities/operators.py
--rw-rw-rw-   0        0        0     6727 2021-03-07 16:37:27.000000 pedal-2.3.8/pedal/utilities/progsnap.py
--rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/utilities/sorting.py
--rw-rw-rw-   0        0        0      326 2021-06-28 19:25:31.000000 pedal-2.3.8/pedal/utilities/system.py
--rw-rw-rw-   0        0        0     1844 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/utilities/text.py
--rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.3.8/pedal/utilities/types.py
--rw-rw-rw-   0        0        0      121 2021-06-29 12:28:23.140298 pedal-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1148 2021-06-29 12:27:12.000000 pedal-2.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:44.112724 pedal-2.4.0/
+-rw-rw-rw-   0        0        0     1103 2020-10-17 16:15:21.000000 pedal-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2924 2023-05-18 18:37:44.114730 pedal-2.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.795722 pedal-2.4.0/Pedal.egg-info/
+-rw-rw-rw-   0        0        0     2924 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3702 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 18:37:41.000000 pedal-2.4.0/Pedal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1901 2020-10-17 19:58:17.000000 pedal-2.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.772724 pedal-2.4.0/pedal/
+-rw-rw-rw-   0        0        0      382 2023-05-18 18:14:23.000000 pedal-2.4.0/pedal/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.912720 pedal-2.4.0/pedal/assertions/
+-rw-rw-rw-   0        0        0      549 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/assertions/__init__.py
+-rw-rw-rw-   0        0        0     8710 2022-09-25 02:42:31.000000 pedal-2.4.0/pedal/assertions/classes.py
+-rw-rw-rw-   0        0        0    13288 2023-01-17 17:53:58.000000 pedal-2.4.0/pedal/assertions/commands.py
+-rw-rw-rw-   0        0        0       73 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/assertions/constants.py
+-rw-rw-rw-   0        0        0    20378 2022-09-17 21:23:34.000000 pedal-2.4.0/pedal/assertions/feedbacks.py
+-rw-rw-rw-   0        0        0     8307 2021-12-05 16:26:04.000000 pedal-2.4.0/pedal/assertions/functions.py
+-rw-rw-rw-   0        0        0     5722 2021-01-26 15:12:38.000000 pedal-2.4.0/pedal/assertions/organizers.py
+-rw-rw-rw-   0        0        0    33479 2023-01-17 17:50:34.000000 pedal-2.4.0/pedal/assertions/runtime.py
+-rw-rw-rw-   0        0        0     3254 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/assertions/setup.py
+-rw-rw-rw-   0        0        0    30229 2022-11-17 14:15:37.000000 pedal-2.4.0/pedal/assertions/static.py
+-rw-rw-rw-   0        0        0     6471 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/assertions/unittest.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.005721 pedal-2.4.0/pedal/cait/
+-rw-rw-rw-   0        0        0      445 2020-10-17 20:34:56.000000 pedal-2.4.0/pedal/cait/__init__.py
+-rw-rw-rw-   0        0        0     2254 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/cait/ast_helpers.py
+-rw-rw-rw-   0        0        0    11371 2021-03-12 21:12:46.000000 pedal-2.4.0/pedal/cait/ast_map.py
+-rw-rw-rw-   0        0        0    10523 2021-01-08 04:00:46.000000 pedal-2.4.0/pedal/cait/cait_api.py
+-rw-rw-rw-   0        0        0    22471 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/cait/cait_node.py
+-rw-rw-rw-   0        0        0       59 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/cait/constants.py
+-rw-rw-rw-   0        0        0     4693 2021-06-28 19:26:48.000000 pedal-2.4.0/pedal/cait/find_node.py
+-rw-rw-rw-   0        0        0    34016 2021-03-12 21:12:46.000000 pedal-2.4.0/pedal/cait/stretchy_tree_matching.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.089720 pedal-2.4.0/pedal/command_line/
+-rw-rw-rw-   0        0        0       94 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/command_line/__init__.py
+-rw-rw-rw-   0        0        0     7897 2022-04-30 18:25:37.000000 pedal-2.4.0/pedal/command_line/command_line.py
+-rw-rw-rw-   0        0        0     7493 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/command_line/mocks.py
+-rw-rw-rw-   0        0        0    25271 2022-11-11 18:14:58.000000 pedal-2.4.0/pedal/command_line/modes.py
+-rw-rw-rw-   0        0        0     3323 2022-03-26 13:30:52.000000 pedal-2.4.0/pedal/command_line/report.py
+-rw-rw-rw-   0        0        0     3540 2020-11-08 16:28:36.000000 pedal-2.4.0/pedal/command_line/verify.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.250713 pedal-2.4.0/pedal/core/
+-rw-rw-rw-   0        0        0      107 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/__init__.py
+-rw-rw-rw-   0        0        0     8756 2022-11-11 16:40:07.000000 pedal-2.4.0/pedal/core/commands.py
+-rw-rw-rw-   0        0        0     2687 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/environment.py
+-rw-rw-rw-   0        0        0      707 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/errors.py
+-rw-rw-rw-   0        0        0    20881 2023-01-17 17:46:13.000000 pedal-2.4.0/pedal/core/feedback.py
+-rw-rw-rw-   0        0        0     4173 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/feedback_category.py
+-rw-rw-rw-   0        0        0     6107 2022-11-17 14:35:13.000000 pedal-2.4.0/pedal/core/final_feedback.py
+-rw-rw-rw-   0        0        0     7639 2023-01-17 17:14:11.000000 pedal-2.4.0/pedal/core/formatting.py
+-rw-rw-rw-   0        0        0     1915 2022-06-12 19:44:51.000000 pedal-2.4.0/pedal/core/location.py
+-rw-rw-rw-   0        0        0    13385 2022-11-28 05:44:51.000000 pedal-2.4.0/pedal/core/report.py
+-rw-rw-rw-   0        0        0      822 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/resolver.py
+-rw-rw-rw-   0        0        0     3985 2022-11-17 14:35:11.000000 pedal-2.4.0/pedal/core/scoring.py
+-rw-rw-rw-   0        0        0     6266 2021-02-02 16:05:08.000000 pedal-2.4.0/pedal/core/submission.py
+-rw-rw-rw-   0        0        0      405 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/core/tag.py
+-rw-rw-rw-   0        0        0     2286 2023-01-17 16:07:35.000000 pedal-2.4.0/pedal/core/tool.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.350729 pedal-2.4.0/pedal/environments/
+-rw-rw-rw-   0        0        0      657 2020-11-08 17:16:23.000000 pedal-2.4.0/pedal/environments/__init__.py
+-rw-rw-rw-   0        0        0     3042 2021-02-26 19:18:08.000000 pedal-2.4.0/pedal/environments/blockpy.py
+-rw-rw-rw-   0        0        0     9569 2022-11-23 18:26:45.000000 pedal-2.4.0/pedal/environments/gradescope.py
+-rw-rw-rw-   0        0        0    15874 2021-01-26 15:29:49.000000 pedal-2.4.0/pedal/environments/jupyter.py
+-rw-rw-rw-   0        0        0    10351 2021-02-02 16:30:22.000000 pedal-2.4.0/pedal/environments/nbgrader.py
+-rw-rw-rw-   0        0        0      368 2020-11-08 17:19:12.000000 pedal-2.4.0/pedal/environments/none.py
+-rw-rw-rw-   0        0        0      766 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/environments/sandbox.py
+-rw-rw-rw-   0        0        0     3651 2023-04-19 22:17:37.000000 pedal-2.4.0/pedal/environments/standard.py
+-rw-rw-rw-   0        0        0     6259 2020-11-13 04:58:08.000000 pedal-2.4.0/pedal/environments/vpl.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.398719 pedal-2.4.0/pedal/extensions/
+-rw-rw-rw-   0        0        0        0 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/extensions/__init__.py
+-rw-rw-rw-   0        0        0    13908 2022-07-24 19:32:33.000000 pedal-2.4.0/pedal/extensions/microbit.py
+-rw-rw-rw-   0        0        0    11604 2022-11-26 00:03:07.000000 pedal-2.4.0/pedal/extensions/plotting.py
+-rw-rw-rw-   0        0        0       81 2022-07-17 15:14:06.000000 pedal-2.4.0/pedal/extensions/turtles.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.502725 pedal-2.4.0/pedal/questions/
+-rw-rw-rw-   0        0        0      669 2021-12-05 16:49:53.000000 pedal-2.4.0/pedal/questions/__init__.py
+-rw-rw-rw-   0        0        0       66 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/questions/constants.py
+-rw-rw-rw-   0        0        0      624 2021-09-15 19:16:10.000000 pedal-2.4.0/pedal/questions/feedbacks.py
+-rw-rw-rw-   0        0        0     6045 2022-11-16 17:32:45.000000 pedal-2.4.0/pedal/questions/graders.py
+-rw-rw-rw-   0        0        0     3477 2021-12-05 16:42:01.000000 pedal-2.4.0/pedal/questions/loader.py
+-rw-rw-rw-   0        0        0     2808 2021-12-05 15:58:25.000000 pedal-2.4.0/pedal/questions/pool.py
+-rw-rw-rw-   0        0        0     3784 2021-09-16 06:51:15.000000 pedal-2.4.0/pedal/questions/questions.py
+-rw-rw-rw-   0        0        0     1660 2022-11-11 17:53:28.000000 pedal-2.4.0/pedal/questions/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.578717 pedal-2.4.0/pedal/resolvers/
+-rw-rw-rw-   0        0        0     1043 2023-05-18 18:14:56.000000 pedal-2.4.0/pedal/resolvers/__init__.py
+-rw-rw-rw-   0        0        0      654 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/resolvers/core.py
+-rw-rw-rw-   0        0        0     2099 2023-05-13 15:07:02.000000 pedal-2.4.0/pedal/resolvers/full.py
+-rw-rw-rw-   0        0        0     1886 2022-11-23 18:27:16.000000 pedal-2.4.0/pedal/resolvers/sectional.py
+-rw-rw-rw-   0        0        0      268 2021-01-26 15:52:26.000000 pedal-2.4.0/pedal/resolvers/silent.py
+-rw-rw-rw-   0        0        0     5119 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/resolvers/simple.py
+-rw-rw-rw-   0        0        0     1176 2020-11-03 17:24:20.000000 pedal-2.4.0/pedal/resolvers/statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.687740 pedal-2.4.0/pedal/sandbox/
+-rw-rw-rw-   0        0        0      662 2023-05-13 15:07:02.000000 pedal-2.4.0/pedal/sandbox/__init__.py
+-rw-rw-rw-   0        0        0    17919 2023-05-18 18:30:27.000000 pedal-2.4.0/pedal/sandbox/commands.py
+-rw-rw-rw-   0        0        0       72 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/sandbox/constants.py
+-rw-rw-rw-   0        0        0     9652 2023-05-13 15:13:44.000000 pedal-2.4.0/pedal/sandbox/data.py
+-rw-rw-rw-   0        0        0     1048 2021-02-24 17:20:18.000000 pedal-2.4.0/pedal/sandbox/exceptions.py
+-rw-rw-rw-   0        0        0    10750 2022-10-04 22:22:33.000000 pedal-2.4.0/pedal/sandbox/feedbacks.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.738721 pedal-2.4.0/pedal/sandbox/library/
+-rw-rw-rw-   0        0        0      222 2022-07-17 15:26:46.000000 pedal-2.4.0/pedal/sandbox/library/__init__.py
+-rw-rw-rw-   0        0        0     5028 2022-08-18 18:00:00.000000 pedal-2.4.0/pedal/sandbox/library/designer.py
+-rw-rw-rw-   0        0        0     5733 2022-07-17 15:20:41.000000 pedal-2.4.0/pedal/sandbox/library/matplotlib.py
+-rw-rw-rw-   0        0        0     6973 2022-08-08 01:23:51.000000 pedal-2.4.0/pedal/sandbox/library/microbit.py
+-rw-rw-rw-   0        0        0     3400 2022-07-28 21:17:36.000000 pedal-2.4.0/pedal/sandbox/library/turtles.py
+-rw-rw-rw-   0        0        0     9976 2023-05-18 18:17:30.000000 pedal-2.4.0/pedal/sandbox/mocked.py
+-rw-rw-rw-   0        0        0    14839 2022-11-25 23:20:23.000000 pedal-2.4.0/pedal/sandbox/result.py
+-rw-rw-rw-   0        0        0    38481 2023-05-18 18:30:27.000000 pedal-2.4.0/pedal/sandbox/sandbox.py
+-rw-rw-rw-   0        0        0     5048 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/sandbox/timeout.py
+-rw-rw-rw-   0        0        0     5577 2021-10-28 00:27:49.000000 pedal-2.4.0/pedal/sandbox/tracer.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.796721 pedal-2.4.0/pedal/source/
+-rw-rw-rw-   0        0        0      912 2022-07-24 20:13:29.000000 pedal-2.4.0/pedal/source/__init__.py
+-rw-rw-rw-   0        0        0      145 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/source/constants.py
+-rw-rw-rw-   0        0        0     5345 2022-10-04 00:04:29.000000 pedal-2.4.0/pedal/source/feedbacks.py
+-rw-rw-rw-   0        0        0     4609 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/source/sections.py
+-rw-rw-rw-   0        0        0     7441 2022-11-23 18:29:38.000000 pedal-2.4.0/pedal/source/source.py
+-rw-rw-rw-   0        0        0      484 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/source/substitutions.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.881719 pedal-2.4.0/pedal/tifa/
+-rw-rw-rw-   0        0        0     3049 2022-11-28 05:46:58.000000 pedal-2.4.0/pedal/tifa/__init__.py
+-rw-rw-rw-   0        0        0     2143 2022-10-06 14:36:45.000000 pedal-2.4.0/pedal/tifa/commands.py
+-rw-rw-rw-   0        0        0       91 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/tifa/constants.py
+-rw-rw-rw-   0        0        0     2833 2022-10-07 13:52:35.000000 pedal-2.4.0/pedal/tifa/contexts.py
+-rw-rw-rw-   0        0        0    23536 2022-09-09 22:57:22.000000 pedal-2.4.0/pedal/tifa/feedbacks.py
+-rw-rw-rw-   0        0        0     1171 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/tifa/identifier.py
+-rw-rw-rw-   0        0        0      908 2022-06-07 19:06:45.000000 pedal-2.4.0/pedal/tifa/settings.py
+-rw-rw-rw-   0        0        0     3649 2022-07-17 15:33:15.000000 pedal-2.4.0/pedal/tifa/state.py
+-rw-rw-rw-   0        0        0    24173 2022-10-07 14:11:04.000000 pedal-2.4.0/pedal/tifa/tifa_core.py
+-rw-rw-rw-   0        0        0    42481 2022-09-22 03:35:00.000000 pedal-2.4.0/pedal/tifa/tifa_visitor.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.930717 pedal-2.4.0/pedal/types/
+-rw-rw-rw-   0        0        0       86 2022-06-09 18:41:53.000000 pedal-2.4.0/pedal/types/__init__.py
+-rw-rw-rw-   0        0        0     9115 2022-11-28 06:00:50.000000 pedal-2.4.0/pedal/types/builtin.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:43.991722 pedal-2.4.0/pedal/types/library/
+-rw-rw-rw-   0        0        0      192 2022-07-26 18:00:27.000000 pedal-2.4.0/pedal/types/library/__init__.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:46:58.000000 pedal-2.4.0/pedal/types/library/cs1_curriculum.py
+-rw-rw-rw-   0        0        0     3499 2022-11-28 05:49:16.000000 pedal-2.4.0/pedal/types/library/designer.py
+-rw-rw-rw-   0        0        0      792 2022-11-28 05:51:17.000000 pedal-2.4.0/pedal/types/library/matplotlib.py
+-rw-rw-rw-   0        0        0     1615 2022-11-28 05:51:25.000000 pedal-2.4.0/pedal/types/library/microbit.py
+-rw-rw-rw-   0        0        0      441 2022-11-28 05:52:06.000000 pedal-2.4.0/pedal/types/library/turtles.py
+-rw-rw-rw-   0        0        0    51752 2022-11-28 05:43:22.000000 pedal-2.4.0/pedal/types/new_types.py
+-rw-rw-rw-   0        0        0    14813 2022-11-23 18:45:05.000000 pedal-2.4.0/pedal/types/normalize.py
+-rw-rw-rw-   0        0        0     8465 2022-10-21 18:56:52.000000 pedal-2.4.0/pedal/types/operations.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:44.104718 pedal-2.4.0/pedal/utilities/
+-rw-rw-rw-   0        0        0      524 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6352 2022-09-19 04:45:01.000000 pedal-2.4.0/pedal/utilities/ast_tools.py
+-rw-rw-rw-   0        0        0     6580 2022-07-27 17:31:05.000000 pedal-2.4.0/pedal/utilities/comparisons.py
+-rw-rw-rw-   0        0        0      679 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/dictionaries.py
+-rw-rw-rw-   0        0        0     8300 2022-09-23 12:51:56.000000 pedal-2.4.0/pedal/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1504 2021-02-04 17:26:41.000000 pedal-2.4.0/pedal/utilities/files.py
+-rw-rw-rw-   0        0        0     1302 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/operators.py
+-rw-rw-rw-   0        0        0     7037 2022-12-31 17:53:00.000000 pedal-2.4.0/pedal/utilities/progsnap.py
+-rw-rw-rw-   0        0        0     1456 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/sorting.py
+-rw-rw-rw-   0        0        0      326 2021-06-28 19:25:31.000000 pedal-2.4.0/pedal/utilities/system.py
+-rw-rw-rw-   0        0        0     2313 2022-07-27 16:49:13.000000 pedal-2.4.0/pedal/utilities/text.py
+-rw-rw-rw-   0        0        0      769 2020-10-17 16:15:22.000000 pedal-2.4.0/pedal/utilities/types.py
+-rw-rw-rw-   0        0        0      121 2023-05-18 18:37:44.120723 pedal-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-05-18 18:33:43.000000 pedal-2.4.0/setup.py
```

### Comparing `pedal-2.3.8/PKG-INFO` & `pedal-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.3.8
+Version: 2.4.0
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.3.8/Pedal.egg-info/PKG-INFO` & `pedal-2.4.0/Pedal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pedal
-Version: 2.3.8
+Version: 2.4.0
 Summary: Tools to provide feedback on student code.
 Home-page: https://pedal-edu.github.io/pedal
 Author: acbart,lukesg08
 Author-email: acbart@udel.edu
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Description: Pedal
         =====
```

### Comparing `pedal-2.3.8/Pedal.egg-info/SOURCES.txt` & `pedal-2.4.0/Pedal.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.cfg
 setup.py
 Pedal.egg-info/PKG-INFO
 Pedal.egg-info/SOURCES.txt
 Pedal.egg-info/dependency_links.txt
 Pedal.egg-info/top_level.txt
@@ -10,14 +11,15 @@
 pedal.egg-info/PKG-INFO
 pedal.egg-info/SOURCES.txt
 pedal.egg-info/dependency_links.txt
 pedal.egg-info/entry_points.txt
 pedal.egg-info/requires.txt
 pedal.egg-info/top_level.txt
 pedal/assertions/__init__.py
+pedal/assertions/classes.py
 pedal/assertions/commands.py
 pedal/assertions/constants.py
 pedal/assertions/feedbacks.py
 pedal/assertions/functions.py
 pedal/assertions/organizers.py
 pedal/assertions/runtime.py
 pedal/assertions/setup.py
@@ -58,18 +60,20 @@
 pedal/environments/jupyter.py
 pedal/environments/nbgrader.py
 pedal/environments/none.py
 pedal/environments/sandbox.py
 pedal/environments/standard.py
 pedal/environments/vpl.py
 pedal/extensions/__init__.py
+pedal/extensions/microbit.py
 pedal/extensions/plotting.py
 pedal/extensions/turtles.py
 pedal/questions/__init__.py
 pedal/questions/constants.py
+pedal/questions/feedbacks.py
 pedal/questions/graders.py
 pedal/questions/loader.py
 pedal/questions/pool.py
 pedal/questions/questions.py
 pedal/questions/setup.py
 pedal/resolvers/__init__.py
 pedal/resolvers/core.py
@@ -85,34 +89,46 @@
 pedal/sandbox/exceptions.py
 pedal/sandbox/feedbacks.py
 pedal/sandbox/mocked.py
 pedal/sandbox/result.py
 pedal/sandbox/sandbox.py
 pedal/sandbox/timeout.py
 pedal/sandbox/tracer.py
+pedal/sandbox/library/__init__.py
+pedal/sandbox/library/designer.py
+pedal/sandbox/library/matplotlib.py
+pedal/sandbox/library/microbit.py
+pedal/sandbox/library/turtles.py
 pedal/source/__init__.py
 pedal/source/constants.py
 pedal/source/feedbacks.py
 pedal/source/sections.py
 pedal/source/source.py
 pedal/source/substitutions.py
 pedal/tifa/__init__.py
 pedal/tifa/commands.py
 pedal/tifa/constants.py
 pedal/tifa/contexts.py
 pedal/tifa/feedbacks.py
 pedal/tifa/identifier.py
+pedal/tifa/settings.py
 pedal/tifa/state.py
 pedal/tifa/tifa_core.py
 pedal/tifa/tifa_visitor.py
 pedal/types/__init__.py
 pedal/types/builtin.py
-pedal/types/definitions.py
+pedal/types/new_types.py
 pedal/types/normalize.py
 pedal/types/operations.py
+pedal/types/library/__init__.py
+pedal/types/library/cs1_curriculum.py
+pedal/types/library/designer.py
+pedal/types/library/matplotlib.py
+pedal/types/library/microbit.py
+pedal/types/library/turtles.py
 pedal/utilities/__init__.py
 pedal/utilities/ast_tools.py
 pedal/utilities/comparisons.py
 pedal/utilities/dictionaries.py
 pedal/utilities/exceptions.py
 pedal/utilities/files.py
 pedal/utilities/operators.py
```

### Comparing `pedal-2.3.8/README.rst` & `pedal-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/assertions/__init__.py` & `pedal-2.4.0/pedal/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/assertions/feedbacks.py` & `pedal-2.4.0/pedal/assertions/feedbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,25 +374,32 @@
 
     TODO: Decorator version
 
     """
 
     message_template = ("Student code failed instructor tests.\n"
                         "{summary_statistics}\n"
+                        "{extra_context}"
                         "{tables}")
 
-    def __init__(self, name, try_all=True, **kwargs):
+    def __init__(self, name, try_all=True, context=None, **kwargs):
         super().__init__(delay_condition=True, **kwargs)
         self.name = name
         self.try_all = try_all
         self.successes = []
         self.failures = []
         self.errors = []
         self.all_feedback = []
 
+        self.fields['extra_context'] = ""
+        if context:
+            formatted_messages = format_contexts([context], self.report.format)
+            if formatted_messages.strip():
+                self.fields['extra_context'] = formatted_messages + '\n'
+
     def __enter__(self):
         self.report.start_group(self)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         # Go through all my collected assertions
         # Count failures, errors, successes
```

### Comparing `pedal-2.3.8/pedal/assertions/functions.py` & `pedal-2.4.0/pedal/assertions/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -167,7 +167,35 @@
         fields['name'] = name
         fields['name_message'] = report.format.name(name)
         fields['actual'] = actual
         fields['actual_message'] = actual.precise_description()
         fields['expected'] = expected
         fields['expected_message'] = expected.precise_description()
         super().__init__(fields=fields, **kwargs)
+
+
+class name_is_not_a_function(AssertionFeedback):
+    """ The name is not a function """
+    title = "Name Is Not a Function"
+    message_template = "You defined `{name_message}`, but did not define it as a function."
+
+    def __init__(self, name, **kwargs):
+        report = kwargs.get("report", MAIN_REPORT)
+        fields = kwargs.get("fields", {})
+        fields['name'] = name
+        fields['name_message'] = report.format.name(name)
+        super().__init__(fields=fields, **kwargs)
+
+
+class function_not_available(AssertionFeedback):
+    """ The name is not a function """
+    title = "Function Not Available"
+    message_template = ("You may have defined `{name_message}`, but it was not available"
+                        " to be called in the top-level scope. Perhaps you mistakenly defined"
+                        " it inside another function or scope?")
+
+    def __init__(self, name, **kwargs):
+        report = kwargs.get("report", MAIN_REPORT)
+        fields = kwargs.get("fields", {})
+        fields['name'] = name
+        fields['name_message'] = report.format.name(name)
+        super().__init__(fields=fields, **kwargs)
```

### Comparing `pedal-2.3.8/pedal/assertions/organizers.py` & `pedal-2.4.0/pedal/assertions/organizers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/assertions/runtime.py` & `pedal-2.4.0/pedal/assertions/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,30 @@
 TODO: assert_has_class
 TODO: assertGraphType, assertGraphValues
 TODO: assert_coverage
 TODO: assert_ran (latest run produced no expections)
 """
 import re
 
+try:
+    from dataclasses import _FIELDS
+except Exception:
+    _FIELDS = '__dataclass_fields__'
+
 from pedal.assertions.feedbacks import (RuntimeAssertionFeedback,
                                         SandboxedValue, ExactValue,
                                         RuntimePrintingAssertionFeedback, AssertionFeedback, assert_group)
+from pedal.assertions.functions import function_not_available, name_is_not_a_function
 from pedal.core.report import MAIN_REPORT
+from pedal.core.feedback import CompositeFeedbackFunction
 from pedal.sandbox import Sandbox
-from pedal.sandbox.commands import check_coverage, get_call_arguments
-from pedal.sandbox.result import share_sandbox_context
+from pedal.sandbox.commands import check_coverage, get_call_arguments, get_student_data, evaluate
+from pedal.sandbox.result import share_sandbox_context, is_sandbox_result, unwrap_value
 from pedal.types.normalize import normalize_type, get_pedal_type_from_value
-from pedal.types.operations import are_types_equal
+from pedal.types.new_types import is_subtype
 from pedal.utilities.comparisons import equality_test
 
 
 def errors(*executions):
     for e in executions:
         if e.is_error:
             return True
@@ -36,15 +43,16 @@
             same, for each character. If False (the default), then strings will
             be normalized (lowercased, trailing decimals chopped, punctuation
             removed, lines are flattened, and all characters are sorted).
         delta (float): When comparing floats, how close the values must be.
             If delta is None, then the default Delta will be used (.001).
     """
     DELTA = .001
-    justification = "Left and right were not equal"
+    justification_template = ("Left ({left}) and right ({right}) were not equal",
+                              "Left ({left}) and right ({right}) were equal")
     _expected_verb = "to be equal to"
     _aggregate_verb = "Expected"
     _inverse_operator = "!="
 
     def __init__(self, left, right, exact_strings=False, delta=DELTA, **kwargs):
         super().__init__(SandboxedValue(left), SandboxedValue(right),
                          exact_strings=exact_strings, delta=delta, **kwargs)
@@ -277,14 +285,46 @@
     def condition(self, left, right):
         """ Tests if the left and right are equal """
         if left.is_sandboxed:
             return left.value._actual_value is None
         return left.value is None
 
 
+class assert_is_dataclass(RuntimeAssertionFeedback):
+    """
+    Determine if the ``value`` is a dataclass.
+    """
+    justification = "Value does not evaluate to a dataclass"
+    _expected_verb = "to evaluate to"
+    _inverse_operator = "to not evaluate to"
+
+    def __init__(self, value, **kwargs):
+        super().__init__(SandboxedValue(value), ExactValue("a dataclass"), **kwargs)
+
+    def condition(self, left, right):
+        """ Tests if the left evaluates to true """
+        return not hasattr(left.value, _FIELDS)
+
+
+class assert_is_not_dataclass(RuntimeAssertionFeedback):
+    """
+    Determine if the ``value`` is not a dataclass.
+    """
+    justification = "Value does not evaluate to a dataclass"
+    _expected_verb = "to not evaluate to"
+    _inverse_operator = "to evaluate to"
+
+    def __init__(self, value, **kwargs):
+        super().__init__(SandboxedValue(value), ExactValue("a dataclass"), **kwargs)
+
+    def condition(self, left, right):
+        """ Tests if the left evaluates to true """
+        return hasattr(left.value, _FIELDS)
+
+
 class assert_true(RuntimeAssertionFeedback):
     """
     Determine if the ``value`` is true.
     """
     justification = "Value does not evaluate to true"
     _expected_verb = "evaluates to"
     _inverse_operator = "does not evaluate to"
@@ -420,15 +460,18 @@
     _inverse_operator = "is not an instance of"
 
     def __init__(self, obj, cls, **kwargs):
         super().__init__(SandboxedValue(obj), SandboxedValue(cls), **kwargs)
 
     def condition(self, obj, cls):
         """ Tests if the left and right are equal """
-        return not isinstance(obj.value, cls.value)
+        value = cls.value
+        if value == int or value == float:
+            value = (int, float)
+        return not isinstance(obj.value, value)
 
 
 class assert_not_is_instance(RuntimeAssertionFeedback):
     """
     Determine if the ``obj`` is an instance of ``cls``
     """
     justification = "Object is an instance of class"
@@ -446,43 +489,54 @@
 class _compare_type(RuntimeAssertionFeedback):
     """
     TODO: Failing for assert_type({"test":1}, dict)
     """
 
     def __init__(self, value, expected_type, **kwargs):
         fields = kwargs.setdefault('fields', {})
-        value_pedal_type = get_pedal_type_from_value(value)
-        expected_pedal_type = normalize_type(expected_type)
-        singular_name = share_sandbox_context(value_pedal_type.singular_name, value)
+        if isinstance(unwrap_value(value), Exception):
+            value_pedal_type = "An error"
+        else:
+            value_pedal_type = get_pedal_type_from_value(unwrap_value(value), evaluate)
+        evaluated_expected_type = evaluate(expected_type) if isinstance(expected_type, str) else expected_type
+        expected_pedal_type = normalize_type(evaluated_expected_type, evaluate)
+        if not isinstance(expected_pedal_type, Exception):
+            expected_pedal_type = expected_pedal_type.as_type()
+            expected_pedal_type_name = expected_pedal_type.singular_name
+        else:
+            expected_pedal_type_name = ""
+        singular_name = share_sandbox_context(value_pedal_type if
+                                              isinstance(value_pedal_type, str) else
+                                              value_pedal_type.singular_name, value)
         fields['value_raw'] = value
         fields['value_type'] = value_pedal_type
         fields['value_type_name'] = singular_name
         fields['expected_type_raw'] = expected_type
         fields['expected_type'] = expected_pedal_type
-        fields['expected_type_name'] = expected_pedal_type.singular_name
+        fields['expected_type_name'] = expected_pedal_type_name
         super().__init__(SandboxedValue(singular_name),
-                         SandboxedValue(expected_pedal_type.singular_name), **kwargs)
+                         SandboxedValue(expected_pedal_type_name), **kwargs)
 
     def condition(self, value, expected_type):
         """ Tests if the left and right are equal """
         value_type = self.fields['value_type']
         expected_type = self.fields['expected_type']
-        return not are_types_equal(value_type, expected_type)
+        return not is_subtype(value_type, expected_type)
 
 
 class assert_type(_compare_type):
     """ Same as assert_is_instance, but has a slightly different wording. """
     justification = "Value is not of type"
-    _expected_verb = ("to not be a value of type", "to not be the type of")
+    _expected_verb = ("to be a value of type", "to be the type of")
     _inverse_operator = "is a value of type"
 
 
 class assert_not_type(_compare_type):
     justification = "Value is of type"
-    _expected_verb = ("to be a value of type", "to be the type of")
+    _expected_verb = ("to not be a value of type", "to not be the type of")
     _inverse_operator = "is not a value of type"
 
     def condition(self, value, expected_type):
         return not super().condition(value, expected_type)
 
 
 class assert_regex(RuntimeAssertionFeedback):
@@ -524,68 +578,91 @@
 class assert_not_almost_equal(assert_not_equal):
     """ Test if the two values are not almost equal; equivalent to
     assert_not_equal. """
 
 
 class assert_output(RuntimePrintingAssertionFeedback):
     """
-    Determine if the ``execution`` outputs ``text``
+    Determine if the ``execution`` outputs ``text``. Uses the `==` operator to do the final comparison.
+    In this case, you can think of the output as a single string with newlines, as opposed to a list
+    of strings (i.e., it is retrieved with `raw_output`).
+
+    If the `exact_strings` parameter is set to be `False`, then output is first normalized following
+    this strategy:
+    * Make strings lowercase
+    * Remove all punctuation characters
+    * Split the string by newlines into a list
+    * Split each individual line by spaces (aka into words)
+    * Remove all empty lines
+    * Sorts the lines by default order
+
+    So the default check will be fairly generous about checking output; as long as all the lines are
+    there (in whatever order), ignoring punctuation and case, the text will be found.
     """
     justification = "Did not print the output"
     _expected_verb = "the output to be"
     _inverse_operator = "does not have the text"
 
     def condition(self, execution, text, exact_strings):
         """ Tests if the regex does not match the text """
-        return errors(execution) or not equality_test(self.get_output(execution), text.value,
+        return errors(execution) or not equality_test(self.get_output(execution), str(text.value),
                                                       _exact_strings=exact_strings, _delta=None)
 
 
 class assert_prints(assert_output):
     """ Deprecated version of assert_output """
 
 
 class assert_not_output(RuntimePrintingAssertionFeedback):
     """
-    Determine if the ``execution`` does not output ``text``
+    Determine if the ``execution`` does not output ``text``. Simply the inverse of
+    :py:func:`pedal.assertions.runtime.assert_output` so check the rules there for more information.
     """
     justification = "Printed the output"
     _expected_verb = "the output to not be"
     _inverse_operator = "has the text"
 
     def condition(self, execution, text, exact_strings):
         """ Tests if the regex does not match the text """
-        return equality_test(self.get_output(execution), text.value,
+        return equality_test(self.get_output(execution), str(text.value),
                              _exact_strings=exact_strings, _delta=None)
 
 
 class assert_output_contains(RuntimePrintingAssertionFeedback):
     """
-    Determine if the ``execution`` outputs ``text``
+    Determine if the ``execution`` outputs ``text`` anywhere. Unlike :py:func:`pedal.assertions.runtime.assert_output`,
+    this function uses the `in` operator. If the `exact_strings` parameter is `False`, then both strings are only
+    lowercased first (but the other normalization rules from `assert_output` are not applied). Can be a more flexible
+    check since it just looks for whether the run of characters is ANYWHERE in the output. Remember that newlines are
+    part of the output, though, so the check will not work across lines unless the `text` includes those newlines.
     """
     justification = "Did not contain the printed output"
     _expected_verb = "the output to contain"
     _inverse_operator = "does not contain the text"
 
     def condition(self, execution, text, exact_strings):
         """ Tests if the regex does not match the text """
-        return text.value not in self.get_output(execution)
+        if not exact_strings:
+            return str(text.value).lower() not in self.get_output(execution).lower()
+        return str(text.value) not in self.get_output(execution)
 
 
 class assert_not_output_contains(RuntimePrintingAssertionFeedback):
     """
     Determine if the ``execution`` outputs ``text``
     """
     justification = "Contained the printed output"
     _expected_verb = "the output to not contain"
     _inverse_operator = "contained the text"
 
     def condition(self, execution, text, exact_strings):
         """ Tests if the regex does not match the text """
-        return text.value in self.get_output(execution)
+        if not exact_strings:
+            return str(text.value).lower() in self.get_output(execution).lower()
+        return str(text.value) in self.get_output(execution)
 
 
 class assert_has_attr(RuntimeAssertionFeedback):
     """
     Determine if the ``object`` has the ``name``
     """
     justification = "Contained the attribute"
@@ -633,15 +710,14 @@
 
     def __init__(self, sandbox, function_name, **kwargs):
         super().__init__(SandboxedValue(sandbox),
                          ExactValue(function_name), **kwargs)
 
     def format_assertion(self, sandbox, function_name, contexts):
         sandbox = sandbox.value
-        function_name = function_name.value
         if isinstance(sandbox, Sandbox):
             return "Sandbox does not contain the function."
         else:
             return "The result does not contain the function."
 
     def condition(self, sandbox, function_name):
         sandbox = sandbox.value
@@ -652,17 +728,17 @@
             function = sandbox.get(function_name, None)
         elif hasattr(sandbox, function_name):
             function = getattr(sandbox, function_name)
         else:
             function = None
         return not callable(function)
 
-
 # TODO: This one is at Runtime, but is not an assertion... Should these be "tests"?
 
+
 class ensure_coverage(AssertionFeedback):
     """
     Verifies that the most recent executed and traced student code has
     ``at_least`` the given ratio of covered (executed) lines.
 
     Args:
         at_least (float): The ratio of covered lines. A value of 1.0 is all
@@ -683,16 +759,15 @@
         unexecuted_lines, coverage = check_coverage(report)
         fields['unexecuted_lines'] = unexecuted_lines
         fields['coverage'] = coverage
         fields['coverage_message'] = str(int(round(100*coverage)))
         super().__init__(coverage, at_least, **kwargs)
 
     def condition(self, coverage, at_least):
-        return coverage <= at_least
-
+        return coverage < at_least
 
 
 class ensure_called_uniquely(AssertionFeedback):
     """
     Verifies that the most recent executed and traced student code has
     ``at_least`` called the given function uniquely that number of times.
     In other words, it prevents students from calling the same function repeatedly
@@ -724,28 +799,40 @@
         fields['at_least'] = at_least
         if ignore is None:
             ignore = set()
         else:
             ignore = set(ignore)
         fields['ignore'] = ignore
         calls = get_call_arguments(function_name, report)
-        unique_calls = set([tuple(args.values()) for args in calls])
+        unique_calls = set([tuple(map(repr, args.values())) for args in calls])
         fields['instructor_ignored'] = instructor_ignored = len(unique_calls & ignore)
         if instructor_ignored:
             fields['instructor_ignore_message'] = f" (but your instructor did not count {instructor_ignored} of the tests{why_ignored})"
         else:
             fields['instructor_ignore_message'] = ""
         fields['total_calls'] = len(calls)
         unique_call_count = len(unique_calls - ignore)
         fields['unique_calls'] = unique_call_count
         super().__init__(unique_call_count, at_least, **kwargs)
 
     def condition(self, unique_call_count, at_least):
-        return unique_call_count <= at_least
+        return unique_call_count < at_least
+
 
+@CompositeFeedbackFunction(function_not_available, name_is_not_a_function)
+def ensure_function_callable(name, **kwargs):
+    report = kwargs.get("report", MAIN_REPORT)
+    values = get_student_data(report)
+    # 2.1. Does the name exist in the values?
+    if name not in values:
+        return function_not_available(name, **kwargs)
+    function_value = values[name]
+    # 2.2. Is the name bound to a callable?
+    if not callable(function_value):
+        return name_is_not_a_function(name)
 
 # Alias conventional camel-case names to our functions
 
 assertEqual = assert_equal
 assertNotEqual = assert_not_equal
 assertLess = assert_less
 assertLessEqual = assert_less_equal
```

### Comparing `pedal-2.3.8/pedal/assertions/setup.py` & `pedal-2.4.0/pedal/assertions/setup.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/assertions/static.py` & `pedal-2.4.0/pedal/assertions/static.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 """
 Collection of feedback functions related to static checks of student code.
 """
+try:
+    import dataclasses
+except ImportError:
+    dataclasses = None
+import ast
+
+from pedal.assertions.classes import (missing_dataclass, dataclass_not_available,
+                                      missing_field_type, too_few_fields, too_many_fields,
+                                      duplicate_dataclass_definition, invalid_field_type,
+                                      wrong_fields_type, name_is_not_a_dataclass, missing_dataclass_annotation,
+                                      unknown_field, wrong_field_order)
 from pedal.assertions.functions import *
 from pedal.cait.cait_api import parse_program
 from pedal.assertions.feedbacks import AssertionFeedback
 from pedal.cait.find_node import find_operation, find_function_calls, find_function_definition
 from pedal.core.feedback import CompositeFeedbackFunction
 from pedal.core.location import Location
 from pedal.core.report import MAIN_REPORT
 from pedal.core.commands import compliment as core_compliment, give_partial
+from pedal.tifa.commands import tifa_type_check
 from pedal.types.normalize import normalize_type
-from pedal.types.operations import are_types_equal
+from pedal.types.new_types import is_subtype
 from pedal.utilities.ast_tools import AST_NODE_NAMES
 
 
 class EnsureAssertionFeedback(AssertionFeedback):
     """ Abstract base class for assertions preventing things. """
     def __init__(self, name, at_least=1, root=None, **kwargs):
         report = kwargs.get('report', MAIN_REPORT)
         root = root or parse_program(report=report)
+        root_message = "" if not root else " (inside of some other code)"
         fields = {'name': name, 'at_least': at_least, 'capacity': '',
-                  'root': root, 'name_message': report.format.name(name)}
+                  'root': root, 'name_message': report.format.name(name),
+                  'root_message': root_message}
         super().__init__(fields=fields, **kwargs)
 
     def _check_usage(self, field_name, uses):
         at_least = self.fields['at_least']
         self.fields[field_name] = use_count = len(uses)
         if at_least > use_count:
             if at_least == 1:
@@ -37,16 +51,18 @@
 
 
 class PreventAssertionFeedback(AssertionFeedback):
     """ Abstract base class for assertions preventing things. """
     def __init__(self, name, at_most=0, root=None, **kwargs):
         report = kwargs.get('report', MAIN_REPORT)
         root = root or parse_program(report=report)
+        root_message = "" if not root else " (inside of some other code)"
         fields = {'name': name, 'at_most': at_most, 'capacity': '',
-                  'root': root, 'name_message': report.format.name(name)}
+                  'root': root, 'name_message': report.format.name(name),
+                  'root_message': root_message}
         super().__init__(fields=fields, **kwargs)
 
     def _check_usage(self, field_name, uses):
         at_most = self.fields['at_most']
         self.fields[field_name] = use_count = len(uses)
         if use_count and at_most < use_count:
             if at_most == 0:
@@ -158,14 +174,18 @@
         self.fields['name_message'] = self.report.format.python_expression(name)
         uses = list(find_operation(name, root=self.fields['root']))
         if uses:
             self.update_location(Location.from_ast(uses[-1]))
         return self._check_usage('use_count', uses)
 
 
+ensure_operator = ensure_operation
+prevent_operator = prevent_operation
+
+
 class prevent_literal(PreventAssertionFeedback):
     """ Make sure that the given literal value does not appear in the student's
     code. """
     title = "May Not Use Literal Value"
     message_template = ("You used the literal value {literal_message:python_expression} on line "
                         "{location.line}. You may not use that value"
                         "{capacity}.")
@@ -181,14 +201,15 @@
         literal = self.fields['literal']
         uses = self.fields['root'].find_matches(repr(literal))
         if uses:
             self.update_location(uses[-1].match_location(False))
         return self._check_usage('use_count', uses)
 
 
+# TODO: ensure_literal does not recognize None?
 class ensure_literal(EnsureAssertionFeedback):
     """ Make sure that the given literal value does appear in the student's
         code. """
     title = "Must Use Literal Value"
     message_template = "You must use the literal value {literal_message}{capacity}."
 
     def __init__(self, literal, at_least=1, root=None, **kwargs):
@@ -292,14 +313,16 @@
         at_most (int): The maximum number of times you are allowed to use this
             AST. Defaults to ``0``.
     """
     title = "May Not Use Code"
     message_template = ("You used {name_message} on line "
                         "{location.line}. You may not use that"
                         "{capacity}.")
+    justification_template = ("Incorrectly found a {name_message}{capacity}{root_message}.",
+                              "Correctly found a {name_message}{capacity}{root_message}.")
 
     def condition(self):
         """ Use find_all to check number of occurrences. """
         name = self.fields['name']
         self.fields['name_message'] = AST_NODE_NAMES.get(name, name)
         uses = list(self.fields['root'].find_all(name))
         if uses:
@@ -318,14 +341,16 @@
     Args:
         name (str): The name of the node.
         at_least (int): The minimum number of times you must use this
             node. Defaults to ``1``.
     """
     title = "Must Use Code"
     message_template = "You must use {name_message}{capacity}."
+    justification_template = ("Failed to find a {name_message}{capacity}{root_message}.",
+                              "Successfully found a {name_message}{capacity}{root_message}.")
 
     def condition(self):
         """ Use find_all to check number of occurrences. """
         name = self.fields['name']
         self.fields['name_message'] = AST_NODE_NAMES.get(name, name)
         uses = list(self.fields['root'].find_all(name))
         if uses:
@@ -454,15 +479,19 @@
 function_prints => ensure_function_call('print', root=match_signature('name')
 
 """
 
 
 # TODO: wait, is this a positive feedback group waiting to happen?
 
-@CompositeFeedbackFunction(missing_function, duplicate_function_definition)
+@CompositeFeedbackFunction(missing_function, duplicate_function_definition,
+                           too_few_parameters, too_many_parameters,
+                           missing_parameter_type, invalid_parameter_type,
+                           wrong_parameter_type, wrong_return_type,
+                           missing_return_type)
 def ensure_function(name, arity=None, parameters=None,
                     returns=None, root=None, compliment=False, **kwargs):
     """ Checks that the function exists and has the right signature. """
     report = kwargs.get('report', MAIN_REPORT)
     root = root or parse_program(report=report)
     defs = root.find_all('FunctionDef')
     defs = [a_def for a_def in defs if a_def._name == name]
@@ -481,57 +510,146 @@
             return too_few_parameters(name, actual_arity, expected_arity, **kwargs)
         elif actual_arity > expected_arity:
             return too_many_parameters(name, actual_arity, expected_arity, **kwargs)
     # 1.2.2 'parameters' style - checks each parameter's name and type
     if parameters is not None:
         actual_parameters = definition.args.args
         for expected_parameter, actual_parameter in zip(parameters, actual_parameters):
-            expected_parameter_type = normalize_type(expected_parameter)
+            expected_parameter_type = normalize_type(expected_parameter, tifa_type_check).as_type()
             actual_parameter_name = (actual_parameter.id if actual_parameter.id is not None
                                      else actual_parameter.arg)
             if actual_parameter.annotation is None:
                 return missing_parameter_type(name, actual_parameter_name,
                                               expected_parameter_type,
                                               **kwargs)
             try:
-                actual_parameter_type = normalize_type(actual_parameter.annotation.ast_node)
+                actual_parameter_type = normalize_type(actual_parameter.annotation.ast_node,
+                                                       tifa_type_check).as_type()
             except ValueError as e:
                 return invalid_parameter_type(name, actual_parameter_name,
                                               actual_parameter.annotation,
                                               expected_parameter_type,
                                               **kwargs)
-            if not are_types_equal(actual_parameter_type, expected_parameter_type):
+            if not is_subtype(actual_parameter_type, expected_parameter_type):
                 return wrong_parameter_type(name, actual_parameter_name,
                                             actual_parameter_type,
                                             expected_parameter_type, **kwargs)
     # 1.2.3. 'returns' style - checks the return type explicitly
     if returns is not None:
-        expected_returns = normalize_type(returns)
+        expected_returns = normalize_type(returns, tifa_type_check).as_type()
         if definition.returns is None:
             return missing_return_type(name, expected_returns, **kwargs)
         try:
-            actual_returns = normalize_type(definition.returns.ast_node)
+            actual_returns = normalize_type(definition.returns.ast_node,
+                                            tifa_type_check).as_type()
         except ValueError as e:
             return invalid_return_type(name, definition.returns,
                                        expected_returns, **kwargs)
-        if not are_types_equal(actual_returns, expected_returns):
+        if not is_subtype(actual_returns, expected_returns):
             return wrong_return_type(name, actual_returns, expected_returns,
                                      **kwargs)
     # Alternatively, returns positive FF?
     if compliment:
         if isinstance(compliment, str):
             core_compliment(compliment, label="function_defined", **kwargs)
         elif compliment is True:
             core_compliment(f"Defined {name}", label="function_defined", **kwargs)
     elif kwargs.get("score"):
         give_partial(kwargs.pop("score"), label="function_defined", **kwargs)
 
     return None
 
 
+@CompositeFeedbackFunction(missing_dataclass, duplicate_dataclass_definition,
+                           too_few_fields, too_many_fields, invalid_field_type,
+                           unknown_field,
+                           missing_field_type, wrong_fields_type, name_is_not_a_dataclass,
+                           dataclass_not_available, missing_dataclass_annotation)
+def ensure_dataclass(name, fields=None, root=None, compliment=False, **kwargs):
+    """
+    Ensures that the actual definition for the given class exists.
+    You can provide either a string and fields, or an instructor-defined version
+
+    Arguments:
+        name (str or dataclass): Either the name of the expected dataclass, or a
+            dataclass object (not an instance).
+        fields (dict):
+    """
+    if isinstance(name, str):
+        # Fields will be a dictionary or class
+        if fields is None:
+            fields = {}
+    # Or assume it is a dataclass provided by the instructor
+    else:
+        fields = {field.name: field.type for field in dataclasses.fields(name)}
+        name = name.__name__
+    # Inspect the code for the definition
+    report = kwargs.get('report', MAIN_REPORT)
+    root = root or parse_program(report=report)
+    defs = root.find_all('ClassDef')
+    defs = [a_def for a_def in defs if a_def._name == name]
+    if not defs:
+        return missing_dataclass(name, **kwargs)
+    if len(defs) > 1:
+        lines = [Location.from_ast(a_def) for a_def in defs]
+        return duplicate_dataclass_definition(name, lines, **kwargs)
+    definition = defs[0]
+    definition_fields = [line for line in definition.body
+                         if isinstance(line.ast_node, ast.AnnAssign) and line.simple]
+    # TODO: Support ast.Assign nodes for default values
+    # 1. Make sure import is present
+    missing_import = ensure_import('dataclasses')
+    if missing_import:
+        return missing_import
+    for decorator in definition.decorator_list:
+        # TODO: Support the @dataclasses.dataclass style too
+        if isinstance(decorator.ast_node, ast.Name) and decorator.id == 'dataclass':
+            break
+    else:
+        return missing_dataclass_annotation(name, **kwargs)
+    # 2. Confirm the number of fields
+    expected_arity = len(fields)
+    actual_arity = len(definition_fields)
+    if actual_arity < expected_arity:
+        return too_few_fields(name, actual_arity, expected_arity, **kwargs)
+    elif actual_arity > expected_arity:
+        return too_many_fields(name, actual_arity, expected_arity, **kwargs)
+    # 3. checks each field's name and type
+    for actual_field in definition_fields:
+        actual_field_name = actual_field.target.id
+        if actual_field_name not in fields:
+            return unknown_field(name, actual_field_name, **kwargs)
+        expected_field = fields[actual_field_name]
+        expected_field_type = normalize_type(expected_field, tifa_type_check).as_type()
+        if actual_field.annotation is None:
+            return missing_field_type(name, actual_field_name, expected_field_type, **kwargs)
+        try:
+            actual_field_type = normalize_type(actual_field.annotation.ast_node,
+                                               tifa_type_check).as_type()
+        except ValueError as e:
+            return invalid_field_type(name, actual_field_name, actual_field.annotation,
+                                      expected_field_type, **kwargs)
+        if not is_subtype(actual_field_type, expected_field_type):
+            return wrong_fields_type(name, actual_field_name, actual_field_type,
+                                     expected_field_type, **kwargs)
+    for actual_field, expected_field in zip(definition_fields, fields.keys()):
+        actual_field_name = actual_field.target.id
+        if actual_field_name != expected_field:
+            return wrong_field_order(name, actual_field_name, expected_field, **kwargs)
+    # Alternatively, returns positive FF?
+    if compliment:
+        if isinstance(compliment, str):
+            core_compliment(compliment, label="dataclass_defined", **kwargs)
+        elif compliment is True:
+            core_compliment(f"Defined {name}", label="dataclass_defined", **kwargs)
+    elif kwargs.get("score"):
+        give_partial(kwargs.pop("score"), label="dataclass_defined", **kwargs)
+
+    return None
+
 @CompositeFeedbackFunction(prevent_function_call, ensure_function_call)
 def ensure_prints_exactly(count, **kwargs):
     """
     DEPRECATED.
 
     Used to ensure that the student's code calls the print function a certain
     number of times.
```

### Comparing `pedal-2.3.8/pedal/assertions/unittest.py` & `pedal-2.4.0/pedal/assertions/unittest.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/cait/ast_helpers.py` & `pedal-2.4.0/pedal/cait/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/cait/ast_map.py` & `pedal-2.4.0/pedal/cait/ast_map.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/cait/cait_api.py` & `pedal-2.4.0/pedal/cait/cait_api.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/cait/cait_node.py` & `pedal-2.4.0/pedal/cait/cait_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/cait/find_node.py` & `pedal-2.4.0/pedal/cait/find_node.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/cait/stretchy_tree_matching.py` & `pedal-2.4.0/pedal/cait/stretchy_tree_matching.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/command_line/command_line.py` & `pedal-2.4.0/pedal/command_line/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     parser.add_argument('--skip_tifa', help="Skip using TIFA in the environment",
                         default=False, action='store_true')
     parser.add_argument('--skip_run', help="Skip automatically running student code in the environment",
                         default=False, action='store_true')
     parser.add_argument('--progsnap_events', help="Choose what level of event"
                                                   " to capture from Progsnap event"
                                                   " logs.",
-                        default='run', choices=['run', 'edit', 'last'])
+                        default='run', choices=['run', 'edit', 'last', 'compile'])
     parser.add_argument('--cache', help='Use the given directory to hold the cache.'
                                         ' You can use "./" to use the current directory.',
                         default=False)
     # TODO: Want to allow for multiple threads too to parallel process data (faster!)
     parser.add_argument('--threaded', help='Run the instructor script in a separate thread to avoid'
                                            ' timeout crashes.',
                         default=False)
```

### Comparing `pedal-2.3.8/pedal/command_line/mocks.py` & `pedal-2.4.0/pedal/command_line/mocks.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/command_line/modes.py` & `pedal-2.4.0/pedal/command_line/modes.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,21 +62,25 @@
     def __init__(self, data, output, error, resolution):
         self.data = data
         self.output = output
         self.error = error
         self.resolution = resolution
 
     def to_json(self):
+        resolution = self.resolution.copy() if self.resolution else {}
+        #if 'considered' in resolution:
+        #    for c in resolution['considered']:
+        #        if 'fields' in c:
+        #            del c['fields']
         return dict(
             output=self.output,
             error=self.error,
-            resolution=self.resolution.copy()
+            **resolution
         )
 
-
 class Bundle:
     def __init__(self, config, script, submission):
         self.config = config
         self.script = script
         self.submission = submission
         self.environment = None
         self.result = None
@@ -110,14 +114,16 @@
             MAIN_REPORT.contextualize(self.submission)
         with redirect_stdout(captured_output):
             with patch.object(sys, 'argv', ics_args):
                 try:
                     grader_exec = compile(self.script,
                                           self.submission.instructor_file, 'exec')
                     exec(grader_exec, global_data)
+                    #print(repr(self.script), file=x)
+                    #print(list(global_data.keys()), file=x)
                     if 'MAIN_REPORT' in global_data:
                         if not global_data['MAIN_REPORT'].resolves:
                             if resolver in global_data:
                                 resolution = global_data[resolver]()
                             # TODO: Need more elegance/configurability here
                             elif self.config.resolver == 'resolve':
                                 exec("from pedal.resolvers.simple import resolve", global_data)
@@ -209,14 +215,15 @@
                     instructor_file=script, load_error=load_error
                 )
                 self.submissions.append(Bundle(self.config, scripts_contents, new_submission))
             return load_error
 
     progsnap_events_map = {
         'run': 'Run.Program',
+        'compile': 'Compile',
         'edit': 'File.Edit',
         'last': 'File.Edit'
     }
 
     def load_progsnap(self, path, instructor_code=None):
         script_file_name, script_file_extension = os.path.splitext(path)
         if script_file_extension in ('.db',):
@@ -235,32 +242,39 @@
                         link_filters['Assignment']['X-URL'] = include_scripts[4:]
                     else:
                         link_filters['Assignment']['X-URL'] = include_scripts
                 event_type = self.progsnap_events_map[self.config.progsnap_events]
                 events = progsnap.get_events(event_filter={'EventType': event_type},
                                              link_filters=link_filters, limit=self.config.limit)
             if self.config.progsnap_events == 'last':
-                events = [e for e in {
-                    (event['student_email'], event['assignment_name']): event
-                    for event in sorted(events, key=lambda e: e['event_id'])}.values()]
+                runs_by_user_assign = {}
+                for event in sorted(events, key=lambda e: e['event_id']):
+                    key = (event[progsnap.PROFILES[progsnap.profile]['link_primary']['user']], event['assignment_name'])
+                    runs_by_user_assign[key] = event
+                events = list(runs_by_user_assign.values())
             for event in events:
                 if instructor_code is None:
-                    instructor_code = event['on_run']
+                    instructor_code_for_this_run = event['on_run']
+                else:
+                    instructor_code_for_this_run = instructor_code
+                link_selections = progsnap._merge('link_selections', {})
                 new_submission = Submission(
                     main_file='answer.py', main_code=event['submission_code'].decode('utf-8'),
                     instructor_file='instructor.py',
+                    #files={'cisc106.py': 'from bakery import *'},
                     execution=dict(client_timestamp=event['client_timestamp'],
                                    event_id=event['event_id']),
-                    user=dict(email=event['student_email'],
-                              first=event['student_first'],
-                              last=event['student_last']),
+                    #user=dict(email=event['student_email'],
+                    #          first=event['student_first'],
+                    #          last=event['student_last']),
+                    user={key: event[key] for key in link_selections['Subject'].values()},
                     assignment=dict(name=event['assignment_name'],
                                     url=event['assignment_url']),
                 )
-                self.submissions.append(Bundle(self.config, instructor_code, new_submission))
+                self.submissions.append(Bundle(self.config, instructor_code_for_this_run, new_submission))
             # raise ValueError("TODO: ProgSnap DB files not yet supported")
             # Progsnap Zip
         elif script_file_extension in ('.zip',):
             raise ValueError("TODO: Zip files not yet supported")
 
     def load_submissions(self):
         given_script = self.config.instructor
@@ -342,19 +356,20 @@
         for bundle in self.submissions:
             if bundle.result.error:
                 print(bundle.result.error)
                 errors += 1
             else:
                 final.append(bundle.to_json())
             total += 1
+        final = clean_json(final)
         if self.config.output is not None:
-            print(final)
+            #print(final)
             print("Total Processed:", total)
             print("Errors:", errors)
-            pedal_json_encoder = PedalJSONEncoder()
+            pedal_json_encoder = PedalJSONEncoder(indent=2, skipkeys=True)
             if self.config.output == 'stdout':
                 print(pedal_json_encoder.encode(final))
             else:
                 with open(self.config.output, 'w') as output_file:
                     print(pedal_json_encoder.encode(final), file=output_file)
         return StatReport(final)
 
@@ -370,14 +385,25 @@
         else:
             return super()._iterencode(o, markers)
 
     def default(self, obj):
         return '<not serializable>'
 
 
+def clean_json(obj):
+    if is_sandbox_result(obj):
+        return clean_json(obj._actual_value)
+    if isinstance(obj, dict):
+        return {clean_json(key): clean_json(value) for key, value in obj.items()}
+    elif isinstance(obj, (set, list, tuple)):
+        return [clean_json(value) for value in obj]
+    else:
+        return obj
+
+
 class VerifyPipeline(AbstractPipeline):
     def process_output(self):
         for bundle in self.submissions:
             bundle.run_ics_bundle(resolver=self.config.resolver, skip_tifa=self.config.skip_tifa,
                                   skip_run=self.config.skip_run)
             if bundle.result.error:
                 raise bundle.result.error
@@ -474,24 +500,27 @@
         if self.config.output == 'stdout':
             self.print_bundles(sys.stdout)
         else:
             with open(self.config.output, 'w') as output_file:
                 self.print_bundles(output_file)
 
     def print_bundles(self, target):
+        #print(len(self.submissions))
         for bundle in self.submissions:
             print(bundle.result.output, file=target)
             if bundle.result.error:
                 raise bundle.result.error
             # This info is not sent to the output target, just to stdout
             print(bundle.submission.instructor_file,
                   bundle.submission.main_file,
-                  bundle.result.data['MAIN_REPORT'].result.score *
-                  bundle.result.data['MAIN_REPORT'].result.success,
-                  sep=", ")
+                  bundle.submission.user.get('student_email') if bundle.submission.user else 'Unknown User',
+                  bundle.submission.assignment.get('name') if bundle.submission.assignment else 'Unknown Assignment',
+                  1 if bundle.result.resolution.success else
+                  bundle.result.resolution.score,
+                  sep=", ", end="")
 
 
 class SandboxPipeline(AbstractPipeline):
     """ Run the given script in a sandbox. """
 
     ICS = """from pedal import *
 verify()
@@ -536,28 +565,30 @@
                 output.append(sandbox.feedback.message)
             print("\n".join(output))
 
 
 class DebugPipeline(AbstractPipeline):
     def process_output(self):
         for bundle in self.submissions:
-            for bundle in self.submissions:
-                print(bundle.submission.instructor_file,
-                      bundle.submission.main_file)
-                if bundle.result.error:
-                    print(bundle.result.error)
-                else:
-                    print("Output:")
-                    print(indent(bundle.result.output, " " * 4))
-                    report = bundle.result.data['MAIN_REPORT']
-                    print("Feedback:")
-                    for feedback in report.feedback:
-                        print("\t", feedback, repr(feedback.fields))
-                    print("Final Feedback")
-                    pprint(report.result.to_json())
+            print(bundle.submission.instructor_file,
+                  bundle.submission.main_file)
+            print("****** Student Code:")
+            print(indent(bundle.submission.main_code, "    "))
+            print("****** Results")
+            if bundle.result.error:
+                print(bundle.result.error)
+            else:
+                print("Output:")
+                print(indent(bundle.result.output, " " * 4))
+                report = bundle.result.data['MAIN_REPORT']
+                print("Feedback:")
+                for feedback in report.feedback:
+                    print("\t", feedback, repr(feedback.fields))
+                print("Final Feedback")
+                pprint(report.result.to_json())
 
 
 class MODES:
     """
     The possible modes that Pedal can be run in.
     """
     # Runs the instructor control script and outputs all feedback
```

### Comparing `pedal-2.3.8/pedal/command_line/report.py` & `pedal-2.4.0/pedal/command_line/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,20 +77,20 @@
         if isinstance(item, str):
             return [r[item] for r in self._raw]
 
     def get_all_feedback(self, with_submissions=True):
         data = [dict(**e) if not with_submissions else
                 dict(**e, **flatten_nested_json('submission', r['submission']))
                 for r in self._raw
-                for e in r['result']['resolution']['considered']]
+                for e in r['result']['considered']]
         return data
 
     def get_final_feedback(self, with_submissions=True):
-        data = [dict(**r['result']['resolution']['final']) if not with_submissions else
-                dict(**r['result']['resolution']['final'],
+        data = [dict(**r['result']['final']) if not with_submissions else
+                dict(**r['result']['final'],
                      **flatten_nested_json('submission', r['submission']))
                 for r in self._raw]
         return data
 
     def get_errors(self):
         return [r['result']['error'] for r in self._raw if r['result']['error']]
```

### Comparing `pedal-2.3.8/pedal/command_line/verify.py` & `pedal-2.4.0/pedal/command_line/verify.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/core/commands.py` & `pedal-2.4.0/pedal/core/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Imperative style commands for constructing feedback in a convenient way.
 Uses a global report object (MAIN_REPORT).
 """
 
 __all__ = ['feedback', 'set_success', 'compliment', 'give_partial', 'explain',
            'gently', 'hide_correctness', 'suppress', 'log', 'debug',
            'system_error', 'clear_report', 'get_all_feedback', 'guidance',
-           'contextualize_report', 'Feedback']
+           'contextualize_report', 'Feedback', 'get_submission']
 
 from pedal.core.feedback import (Feedback, FeedbackKind, FeedbackCategory,
                                  FeedbackResponse)
 from pedal.core.report import MAIN_REPORT
 
 from pedal.core.submission import Submission
 
@@ -115,29 +115,31 @@
     Args:
         report (:py:class:`pedal.core.report.Report`): The report object to
             hide correctness on.
     """
     report.hide_correctness()
 
 
-def suppress(category=None, label=True, report=MAIN_REPORT):
+def suppress(category=None, label=True, fields=None, report=MAIN_REPORT):
     """
     Hides a given category or label within a category from being considered
     by the resolver.
 
     Args:
         category (str): The general feedback category to suppress within.
             Should be a member of
             :py:class:`pedal.core.feedback_category.FeedbackCategory`.
         label (str or bool): The specific feedback label to suppress, or
             True if all the labels within this category should be suppressed.
+        fields (dict): The fields that will be exactly matched to suppress a
+            given feedback. The keys should be strings.
         report (:py:class:`~pedal.core.report.Report`): The report object to
             suppress information within.
     """
-    report.suppress(category, label)
+    report.suppress(category, label, fields)
 
 
 def log(*items, sep=" ", **kwargs):
     """
     Attach logging information to the Report as a piece of feedback.
 
     Args:
@@ -213,14 +215,27 @@
     """
     if not isinstance(submission, Submission):
         submission = Submission(files={filename: submission})
     if clear:
         report.clear()
     report.contextualize(submission)
 
+def get_submission(report=MAIN_REPORT) -> Submission:
+    """
+    Get the current submission from the given report, or the default MAIN_REPORT.
+
+    Args:
+        report: The report to attach this feedback to (defaults to the
+            :py:data:`~pedal.core.report.MAIN_REPORT`).
+
+    Returns:
+        Submission: The current submission
+    """
+    return report.submission
+
 
 def get_all_feedback(report=MAIN_REPORT):
     """
     Gives access to the list of feedback from the report. Usually, you won't
     need this; but if you want to build on the results of earlier tools, it
     can be a useful mechanism.
 
@@ -246,7 +261,10 @@
     correctly. These will not usually be reported to the student.
     """
     title = "System Error"
     category = Feedback.CATEGORIES.SYSTEM
     kind = FeedbackKind.META
     valence = Feedback.NEUTRAL_VALENCE
     muted = True
+
+
+# TODO: set_line_offset(offset, filename='answer.py')
```

### Comparing `pedal-2.3.8/pedal/core/environment.py` & `pedal-2.4.0/pedal/core/environment.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/core/errors.py` & `pedal-2.4.0/pedal/core/errors.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/core/feedback.py` & `pedal-2.4.0/pedal/core/feedback.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,14 +34,17 @@
             more than one category.
         kind (str): The pedagogical role of this feedback, e.g., "misconception", "mistake",
             "hint", "constraint". Usually, a piece of Feedback is pointing out a mistake,
             but feedback can also be used for various other purposes.
         justification (str): An instructor-facing string briefly describing why this
             feedback was selected. Serves as a "TL;DR" for this feedback category, useful
             for debugging why a piece of feedback appeared.
+        justification_template (str): A markdown-formatted message template that will
+            be used if a ``justification`` is None. Any ``fields`` will be injected
+            into the template IF the ``condition`` is met.
         priority (str): An indication of how important this feedback is relative to other types
             of feedback in the same category. Might be "high/medium/low". Exactly how this
             gets used is up to the resolver, but typicaly it helps break ties.
         valence (int): Indicates whether this is negative, positive, or neutral feedback.
             Either 1, -1, or 0.
 
         title (str, optional): A formal, student-facing title for this feedback. If None, indicates
@@ -103,25 +106,32 @@
 
     POSITIVE_VALENCE = 1
     NEUTRAL_VALENCE = 0
     NEGATIVE_VALENCE = -1
     CATEGORIES = FeedbackCategory
     KINDS = FeedbackKind
 
+    DEFAULT_FEEDBACK_MESSAGE = "No feedback message provided"
+    DEFAULT_JUSTIFICATION_MESSAGE = "No justification provided"
+    DEFAULT_ELSE_MESSAGE = None
+
+
     label = None
     category = None
     justification = None
+    justification_template = None
     constant_fields = None
     fields = None
     field_names = None
     kind = None
     title = None
     message = None
     message_template = None
     else_message = None
+    else_message_template = None
     priority = None
     valence = None
     location = None
     score = None
     correct = None
     muted = None
     unscored = None
@@ -134,22 +144,25 @@
     activate: bool
     _status: str
     _exception: Exception or None
     _met_condition: bool
     _stored_args: tuple
     _stored_kwargs: dict
 
+    resolved_score = None
+    unused_message = None
+
     #MAIN_REPORT
 
     def __init__(self, *args, label=None,
                  category=None, justification=None,
                  fields=None, field_names=None,
                  kind=None, title=None,
                  message=None, message_template=None,
-                 else_message=None,
+                 else_message=None, else_message_template=None,
                  priority=None, valence=None,
                  location=None, score=None, correct=None,
                  muted=None, unscored=None,
                  tool=None, version=None, author=None,
                  tags=None, parent=None, report=MAIN_REPORT,
                  delay_condition=False, activate=True,
                  **kwargs):
@@ -189,14 +202,16 @@
             self.title = label
         if message is not None:
             self.message = message
         if message_template is not None:
             self.message_template = message_template
         if else_message is not None:
             self.else_message = else_message
+        if else_message_template is not None:
+            self.else_message_template = else_message_template
 
         # Locations
         if isinstance(location, int):
             location = Location(location)
         # TODO: Handle tuples (Line, Col) and (Filename, Line, Col), and
         #  possibly lists thereof
         if location is not None:
@@ -245,18 +260,25 @@
     def _handle_condition(self):
         """ Actually handle the condition check, updating message and report. """
         # Self-attach to a given report?
         self._exception = None
         try:
             self._met_condition = self.condition(*self._stored_args, **self._stored_kwargs)
             # Generate the message field as needed
+            self.justification = self._get_justification(self._met_condition)
             if self._met_condition:
                 self.message = self._get_message()
                 self._status = FeedbackStatus.ACTIVE
             else:
+                self.else_message = self._get_else_message()
+                self.message = self.else_message
+                try:
+                    self.unused_message = self._get_message()
+                except Exception:
+                    self.unused_message = ""
                 self._status = FeedbackStatus.INACTIVE
         except Exception as e:
             self._met_condition = False
             self._exception = e
             self._status = FeedbackStatus.ERROR
         if self.report is not None:
             if self._met_condition:
@@ -293,15 +315,67 @@
         """
         if self.message is not None:
             return self.message
         if self.message_template is not None:
             fields = {field: FeedbackFieldWrapper(field, value, self.report.format)
                       for field, value in self.fields.items()}
             return self.message_template.format(**fields)
-        return "No feedback message provided"
+        return self.DEFAULT_FEEDBACK_MESSAGE
+
+    def _get_else_message(self):
+        """
+        Determines the appropriate value for the else_message. It will attempt
+        to use this instance's else_message, but if it's not available then it will
+        try to generate one from the else_message_template. Then, it returns ``None``
+        instead (since usually we don't provide positive feedback).
+
+        You can override this to create a truly dynamic else_message, if you want.
+
+        Returns:
+            str: The else_message for this feedback.
+        """
+        if self.else_message is not None:
+            return self.else_message
+        if self.else_message_template is not None:
+            fields = {field: FeedbackFieldWrapper(field, value, self.report.format)
+                      for field, value in self.fields.items()}
+            return self.else_message_template.format(**fields)
+        return self.DEFAULT_ELSE_MESSAGE
+
+    def _get_justification(self, met_condition):
+        """
+        Determines the appropriate value for the justification. It first checks
+        if there is a `justification` already present, but if it's not available
+        then it will attempt to generate one from the `justification_template`. Then,
+        it returns a generic message.
+
+        You can override this to create a truly dynamic justification, if you want.
+
+        Returns:
+            str: The justification for this feedback.
+        """
+        if self.justification is not None:
+            if isinstance(self.justification, str):
+                if met_condition:
+                    return self.justification
+                else:
+                    return "The following condition was not met: " + self.justification
+            else:
+                met, unmet = self.justification
+                return met if met_condition else unmet
+        if self.justification_template is not None:
+            if isinstance(self.justification_template, str):
+                template = "The following condition was not met: " + self.justification_template
+            else:
+                met, unmet = self.justification_template
+                template = met if met_condition else unmet
+            fields = {field: FeedbackFieldWrapper(field, value, self.report.format)
+                      for field, value in self.fields.items()}
+            return template.format(**fields)
+        return self.DEFAULT_JUSTIFICATION_MESSAGE
 
     def _get_child_feedback(self, feedback, active):
         """ Callback function that Reports will call when a new piece of
         feedback is being considered. By default, does nothing. This is useful
         for :py:class:`pedal.core.group.FeedbackGroup`, most other feedbacks
         will just not care.
 
@@ -343,14 +417,16 @@
             metadata += ", tool=" + self.tool
         if self.category is not None:
             metadata += ", category=" + self.category
         if self.priority is not None:
             metadata += ", priority=" + self.priority
         if self.parent is not None:
             metadata += ", parent=" + str(self.parent.label)
+        if self.fields is not None:
+            metadata += ", " + ", ".join(f"{field}={value!r}" for field, value in self.fields.items())
         return "Feedback({}{})".format(self.label, metadata)
 
     def update_location(self, location):
         """ Updates both the fields and location attribute.
         TODO: Handle less information intelligently. """
         if isinstance(location, int):
             location = Location(location)
```

### Comparing `pedal-2.3.8/pedal/core/feedback_category.py` & `pedal-2.4.0/pedal/core/feedback_category.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/core/formatting.py` & `pedal-2.4.0/pedal/core/formatting.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,24 @@
     if format_spec.endswith(word):
         format_spec = format_spec[:-len(word)]
         if format_spec and format_spec[-1] == ':':
             format_spec = format_spec[:-1]
     return format_spec
 
 
+def escape_dunders(text):
+    if text[:2] == '__' and text[-2:] == '__':
+        return "\\_\\_" + text[2:-2] + "\\_\\_"
+    return text
+
+
+def escape_angles(text):
+    return text.replace("<", "&lt;").replace(">", "&gt;")
+
+
 class FeedbackFieldWrapper:
     """
     Wraps an individual field within a Feedback message.
 
     Args:
         key (str): The name of the field.
         value (Any): The value to interpolate into the message.
@@ -112,44 +122,48 @@
         result = []
         result.append(" | ".join(columns))
         for row in rows:
             result.append(" | ".join(row))
         return "\n" + ("\n".join(result))
 
     def check_mark(self):
+        # TODO: should be ✓, right?
         return " "
 
     def negative_mark(self):
         return "×"
 
+    def indent(self):
+        return "    "
+
 
 class HtmlFormatter(Formatter):
 
     def html_tag(self, tag, contents, classes=None):
         if classes is None:
             return f"<{tag}>{contents}</{tag}>"
         else:
             return f"<{tag} class='{classes}'>{contents}</{tag}>"
 
     def html_pre(self, text, classes=None):
-        return self.html_tag('pre', text, classes)
+        return self.html_tag('pre', escape_angles(text), classes)
 
     def html_div(self, contents, classes=None):
         return self.html_tag('div', contents, classes)
 
     def html_code(self, contents, classes=None):
-        return self.html_tag('code', contents, classes)
+        return self.html_tag('code', escape_dunders(contents), classes)
 
     def html_span(self, contents, classes=None):
         return self.html_tag('span', contents, classes)
 
     ############################################################################
 
     def python_code(self, code):
-        return self.html_pre(self.html_code(code), "pedal-python-code python")
+        return self.html_tag('pre', self.html_code(code), "pedal-python-code python")
 
     def python_expression(self, code):
         return self.html_code(code)
 
     def filename(self, filename):
         return self.html_code(filename, "pedal-filename")
 
@@ -213,14 +227,17 @@
             body.append(f"  <tr{row_class}>\n{row_text}\n  </tr>")
         body = "\n".join(body)
         return (f"\n<table{table_class}>"
                 f"   <tr{header_class}>\n{header}\n  </tr>"
                 f"   {body}"
                 f"</table>")
 
+    def indent(self):
+        return "&nbsp;"*4
+
     def check_mark(self):
         return self.html_span("&#10004;", "pedal-positive-mark")
 
     def negative_mark(self):
         return self.html_span("&#10060;", "pedal-negative-mark")
```

### Comparing `pedal-2.3.8/pedal/core/location.py` & `pedal-2.4.0/pedal/core/location.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,20 @@
                  filename=None):
         self.line = line
         self.col = col
         self.end_line = end_line
         self.end_col = end_col
         self.filename = filename
 
+    def __str__(self):
+        return f"<Location({self.line}, {self.col}, {self.filename})>"
+
+    def __repr__(self):
+        return str(self)
+
     @classmethod
     def from_ast(cls, node):
         """
         Creates a new Location object from the AST node. Should work
         for both built-in AST nodes and CaitNodes.
 
         Args:
```

### Comparing `pedal-2.3.8/pedal/core/report.py` & `pedal-2.4.0/pedal/core/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         """
         Creates a new Report instance.
         """
         self._tool_data = {}
         self.feedback = []
         self.ignored_feedback = []
         self.suppressions = {}
-        self.suppressed_labels = []
+        self.suppressed_labels = {}
         self.hiddens = set()
         self.groups = []
         self.group = None
         self.group_names = {}
         self.hooks = {}
         self.class_hooks = {}
         self.submission = None
@@ -155,35 +155,43 @@
             :py:class:`~pedal.core.feedback.Feedback`: The attached feedback.
         """
         self.ignored_feedback.append(feedback)
         if feedback.parent is not None:
             feedback.parent._get_child_feedback(feedback, False)
         return feedback
 
-    def suppress(self, category=None, label=True):
+    def suppress(self, category=None, label=True, fields=None):
         """
         Suggest that an entire category or label within a category ignored by
         the resolver.
         TODO: Currently, only global suppression is supported.
 
         Args:
             category (str): The category of feedback to suppress.
             label (bool or str): A specific label to match against and suppress.
+            fields (dict of key/values): The fields that will be matched exactly to
+                suppress.
         """
+        if fields is None:
+            fields = {}
         if category is None:
-            self.suppressed_labels.append(label)
+            if label not in self.suppressed_labels:
+                self.suppressed_labels[label] = []
+            self.suppressed_labels[label].append(fields)
         else:
             category = category.lower()
             if isinstance(label, str):
                 label = label.lower()
             if category in FeedbackCategory.ALIASES:
                 category = FeedbackCategory.ALIASES[category]
             if category not in self.suppressions:
-                self.suppressions[category] = []
-            self.suppressions[category].append(label)
+                self.suppressions[category] = {}
+            if label not in self.suppressions[category]:
+                self.suppressions[category][label] = []
+            self.suppressions[category][label].append(fields)
 
     def add_hook(self, event, function):
         """
         Register the `function` to be executed when the given `event` is
         triggered.
         
         Args:
```

### Comparing `pedal-2.3.8/pedal/core/resolver.py` & `pedal-2.4.0/pedal/core/resolver.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/core/scoring.py` & `pedal-2.4.0/pedal/core/scoring.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Class for managing custom score objects (e.g., "+20%").
 """
 import re
 
-SCORE_PATTERN = re.compile(r"(\!*)([\+\-\/\*])?([\d\.]+)(\%)?(.*)")
+SCORE_PATTERN = re.compile(r"(!*)([+\-/*])?([\d.]+)(%)?(.*)")
 
 class Score:
     def __init__(self, invert, operator, value, percentage, leftovers):
         self.invert = invert
         self.operator = operator
         self.value = value
         self.percentage = percentage
@@ -57,21 +57,27 @@
     def __str__(self):
         value = self.value
         if self.percentage:
             # TODO: Being careless with rounding here.
             value *= 100
         value = str(round(value))
         operator = self.operator
-        if operator is None:
+        if not operator:
             operator = "+"
         return (
             ("!" if self.invert else "")+operator+value +
             ("%" if self.percentage else "")+self.leftovers
         )
 
+    def to_percent_string(self):
+        value = self.value * 100
+        value = str(round(value))
+        operator = "+" if not self.operator else self.operator
+        return ("!" if self.invert else "") + operator + value + "%" + self.leftovers
+
     def add_to_current(self, current):
         if self.operator in ("+", None, "") and not self.invert:
             current += self.value
         elif self.operator == "-" and not self.invert:
             current -= self.value
         elif self.operator == "*" and not self.invert:
             current *= self.value
```

### Comparing `pedal-2.3.8/pedal/core/submission.py` & `pedal-2.4.0/pedal/core/submission.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/core/tool.py` & `pedal-2.4.0/pedal/core/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,19 +31,15 @@
 .. code-block:: python
 
     report[TOOL_NAME]['my field'] = False
 
 The ``__init__.py`` file for a Tool should use  ``__all__`` to expose any
 interesting teacher-level functions, classes, and data. That way, teachers can
 just consistently use ``from pedal.tool import *`` to instantly gain access to
-the interesting set of members. The big exception to this is
-:ref:`toolkit`, which is full of prototypical Tools organized
-into subsubmodules. If it's just a single function without much complexity, it
-probably belongs in the Toolkit; but as soon as complexity or multiple
-functions emerge with a theme, it can be promoted to a Tool.
+the interesting set of members.
 
 """
 
 __all__ = ['ToolRegistration']
 
 
 class ToolRegistration:
```

### Comparing `pedal-2.3.8/pedal/environments/__init__.py` & `pedal-2.4.0/pedal/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/environments/blockpy.py` & `pedal-2.4.0/pedal/environments/blockpy.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/environments/gradescope.py` & `pedal-2.4.0/pedal/environments/gradescope.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,21 @@
       {"name": "Accuracy", "value": .926},
       {"name": "Time", "value": 15.1, "order": "asc"},
       {"name": "Stars", "value": "*****"}
     ]
 }
 
 """
-import re
-import sys
 import json
-from html.parser import HTMLParser
 import tabulate
 
 from pedal import Score
 from pedal.core.final_feedback import parse_feedback
 from pedal.resolvers.core import make_resolver
 from pedal.source import verify, next_section as original_next_section
-from pedal.core.feedback import Feedback
 from pedal.core.environment import Environment
 from pedal.core.report import MAIN_REPORT
 from pedal.sandbox import run, get_sandbox, set_input, start_trace, get_output
 from pedal.source.sections import FeedbackSourceSection
 from pedal.tifa import tifa_analysis
 from pedal.resolvers.simple import resolve as simple_resolve, by_priority
 from pedal.resolvers.full import resolve as full_resolve
```

### Comparing `pedal-2.3.8/pedal/environments/jupyter.py` & `pedal-2.4.0/pedal/environments/jupyter.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/environments/nbgrader.py` & `pedal-2.4.0/pedal/environments/nbgrader.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/environments/sandbox.py` & `pedal-2.4.0/pedal/environments/sandbox.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/environments/standard.py` & `pedal-2.4.0/pedal/environments/standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pedal.cait import parse_program
 from pedal.sandbox.commands import run
 from pedal.resolvers import simple
 from pedal.sandbox import run, get_sandbox, set_input, start_trace
 from pedal.tifa import tifa_analysis
 from pedal.resolvers.simple import resolve
 
+
 def parse_argv():
     """ Retrieve fields from sys.argv """
     if len(sys.argv) == 2:
         main_file = sys.argv[1]
         with open(main_file) as main_file_handle:
             main_code = main_file_handle.read()
         return sys.argv[0], {main_file: main_code}, main_file, main_code, None, None, None, None
```

### Comparing `pedal-2.3.8/pedal/environments/vpl.py` & `pedal-2.4.0/pedal/environments/vpl.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/extensions/plotting.py` & `pedal-2.4.0/pedal/extensions/plotting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Extensions related to MatPlotLib.
 
 Mock module for Sandbox.
 
 Assertions.
 """
-from pedal import Feedback, CompositeFeedbackFunction
+from pedal import Feedback, CompositeFeedbackFunction, is_sandbox_result, Sandbox
 from pedal.assertions import ensure_function_call, prevent_function_call
 from pedal.core.feedback import FeedbackResponse
 from pedal.core.report import MAIN_REPORT
+from pedal.sandbox.data import format_contexts
 from pedal.types.builtin import BUILTIN_MODULES
-from pedal.types.definitions import ModuleType, FunctionType, NoneType
+from pedal.types.new_types import ModuleType, FunctionType, NoneType
 from pedal.cait.find_node import function_is_called
 from pedal.cait.cait_api import parse_program, def_use_error
 from pedal.sandbox.commands import get_sandbox
 
 PLOT_LABEL = {'plot': 'line plot',
               'hist': 'histogram',
               'scatter': 'scatter plot'}
@@ -97,31 +98,31 @@
                         "function, which actually creates the graph.")
     justification = "The show function was not found as a function call."
 
     def condition(self):
         return not function_is_called("show")
 
 
-def compare_data(plt_type, correct, given, special_comparion=None):
+def compare_data(plt_type, correct, given, special_comparison=None):
     """
     Determines whether the given data matches any of the data found in the
     correct data. This handles plots of different types: if a histogram
     was plotted with the expected data for a line plot, it will return True.
 
     Args:
         plt_type (str): The expected type of this plot
         correct (List of Int or List of List of Int): The expected data.
         given (Dict): The actual plotted data and information
-        special_comparion (callable): A special comparison function to use
+        special_comparison (callable): A special comparison function to use
             between the data. If None, then will use the ``==`` operator.
     Returns:
         bool: Whether the correct data was found in the given plot.
     """
-    if special_comparion is None:
-        def special_comparion(left, right):
+    if special_comparison is None:
+        def special_comparison(left, right):
             return left == right
 
     # Infer arguments
     if plt_type == 'hist':
         correct_xs = None
         correct_ys = correct
     elif not correct:
@@ -132,63 +133,100 @@
         correct_xs, correct_ys = correct
     else:
         # Assume it is a singular list
         correct_xs = list(range(len(correct)))
         correct_ys = correct
 
     if given['type'] == 'hist':
-        return special_comparion(correct_ys, given['values'])
+        return special_comparison(correct_ys, given['values'])
     elif plt_type == 'hist':
-        return special_comparion(correct_ys, given['y'])
+        return special_comparison(correct_ys, given['y'])
     else:
-        return (special_comparion(correct_xs, given['x']) and
-                special_comparion(correct_ys, given['y']))
+        return (special_comparison(correct_xs, given['x']) and
+                special_comparison(correct_ys, given['y']))
+
+
+def describe_data(given, with_x=False):
+    if given['type'] == 'hist':
+        return given['values']
+    elif given['type'] == 'line' and not with_x:
+        # TODO: Might need to know if we describe the x-axis too..?
+        return given['y']
+    else:
+        return [given['x'], given['y']]
 
 
 GRAPH_TYPES = {'line': 'line plot',
                'hist': 'histogram',
                'scatter': 'scatter plot'}
 
 
+def get_diff(expected, actual, format):
+    if isinstance(actual, bool):
+        return ("\nI expected the data to be:\n" +
+                format.python_value(repr(expected)))
+    if len(actual) == 1:
+        return ("\nI expected the data to be:\n" +
+                format.python_value(repr(expected)) +
+                "\nBut instead, the data was:\n" +
+                format.python_value(repr(actual[0])))
+    return ("\nI expected the data to be:\n" +
+            format.python_value(repr(expected)) +
+            f"\nBut instead, I found {len(actual)} plots, with this data:\n" +
+            "\n".join(format.python_value(repr(a)) for a in actual))
+
+
 class BadGraphFeedback(FeedbackResponse):
-    category = Feedback.CATEGORIES.INSTRUCTOR
-    def __init__(self, plt_type, expected, actual, **kwargs):
+    category = Feedback.CATEGORIES.SPECIFICATION
+    valence = Feedback.NEGATIVE_VALENCE
+    kind = Feedback.KINDS.CONSTRAINT
+
+    def __init__(self, plt_type, expected, actual, context=None, report=MAIN_REPORT, **kwargs):
         fields = kwargs.setdefault('fields', {})
         fields['plt_type'] = plt_type
         fields['expected'] = expected
         fields['actual'] = actual
-        super().__init__(plt_type, expected, actual, **kwargs)
+        fields['diff_message'] = get_diff(expected, actual, report.format)
+        fields['context'] = context
+        if is_sandbox_result(context):
+            context_id = context._actual_context_id
+            sandbox = context._actual_sandbox
+            actual_context = sandbox.get_context(context_id)
+            fields['context_message'] = "\n "+format_contexts([actual_context], report.format)
+        else:
+            fields['context_message'] = ""
+        super().__init__(plt_type, expected, actual, report=report, **kwargs)
 
 
 class other_plt(BadGraphFeedback):
     title = "Plotting Another Graph"
     message_template = ("You have created a {plt_type}, but it does not "
                         "have the right data. That data appears to have been "
-                        "plotted in another graph.")
+                        "plotted in another graph.{context_message}")
 
 
 class wrong_plt_data(BadGraphFeedback):
     title = "Plot Data Incorrect"
     message_template = ("You have created a {plt_type}, but it does not have "
-                        "the right data.")
+                        "the right data.{context_message}{diff_message}")
 
 
 class wrong_plt_type(BadGraphFeedback):
     title = "Wrong Plot Type"
     message_template = ("You have plotted the right data, but you appear to "
-                        "have not plotted it as a {plt_type}.")
+                        "have not plotted it as a {plt_type}.{context_message}")
 
 
 class no_plt(BadGraphFeedback):
     title = "Missing Plot"
-    message_template = "You have not created a {plt_type} with the proper data."
+    message_template = "You have not created a {plt_type} with the proper data.{context_message}"
 
 
 @CompositeFeedbackFunction(other_plt, wrong_plt_data, wrong_plt_type, no_plt)
-def assert_plot(plt_type, data, **kwargs):
+def assert_plot(plt_type, data, context=None, special_comparison=None, **kwargs):
     """
     Check whether a plot with the given ``plt_type`` and ``data`` exists.
     If the plot was found successfully, returns False.
     Otherwise, returns the feedback that was detected.
 
     Args:
         plt_type (str): Either 'line', 'hist', or 'scatter'
@@ -199,29 +237,31 @@
     # Allow instructor to use "plot" instead of "line" as type
     if plt_type == 'plot':
         plt_type = 'line'
     # Check the plots to see if there is a plot with the data
     type_found = False
     data_found = False
     plots = get_sandbox(report=report).modules.plotting.plots
+    appropriate_plots = []
     for graph in plots:
         for a_plot in graph['data']:
-            data_found_here = compare_data(plt_type, data, a_plot)
+            data_found_here = compare_data(plt_type, data, a_plot, special_comparison=special_comparison)
             if a_plot['type'] == plt_type and data_found_here:
                 return False
             if a_plot['type'] == plt_type:
                 type_found = True
+                appropriate_plots.append(describe_data(a_plot, not isinstance(data, (tuple, list))))
             if data_found_here:
                 data_found = data_found_here
     # Figure out what kind of mistake was made.
     plt_type = GRAPH_TYPES.get(plt_type, plt_type)
     if type_found and data_found:
         return other_plt(plt_type, data, data_found)
     elif type_found:
-        return wrong_plt_data(plt_type, data, data_found)
+        return wrong_plt_data(plt_type, data, appropriate_plots, context=context)
     elif data_found:
         return wrong_plt_type(plt_type, data, data_found)
     else:
         return no_plt(plt_type, data, data_found)
 
 
 def get_plots(report=MAIN_REPORT):
@@ -247,7 +287,10 @@
             }
         }
         # ...
         ]
     """
     return get_sandbox(report=report).modules.plotting.plots
 
+
+def clear_plots(report=MAIN_REPORT):
+    get_sandbox(report=report).modules.plotting._reset_plots()
```

### Comparing `pedal-2.3.8/pedal/questions/pool.py` & `pedal-2.4.0/pedal/questions/pool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 from pedal.core.commands import gently
 from pedal.core.report import MAIN_REPORT
 from pedal.questions import _name_hash, SETTING_SHOW_CASE_DETAILS, load_question
-from pedal.questions.questions import show_question
+from pedal.questions.feedbacks import show_question
 
 
 class Pool:
     """
 
     """
     _POOL_TRACKER = 0
+    _CURRENT = []
+    # TODO: Attach to report instead!
 
-    def __init__(self, name, choices, seed=None, report=MAIN_REPORT, position=None):
+    def __init__(self, name, choices=None, seed=None, report=MAIN_REPORT, position=None):
         self.name = name
-        self.choices = choices
+        self.choices = choices if choices else []
         self.seed = seed
         self.report = report
         if position is None:
             position = Pool._POOL_TRACKER
             Pool._POOL_TRACKER += 1
         self.position = position
 
+    def __enter__(self):
+        Pool._CURRENT.append(self)
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        Pool._CURRENT.pop()
+        self.ask()
+
+    @classmethod
+    def add_question_via_context(cls, question):
+        if cls._CURRENT:
+            cls._CURRENT[-1].choices.append(question)
+
     def choose(self, force=None):
         """
 
         Args:
             force:
 
         Returns:
@@ -37,14 +52,18 @@
                 # Assume iterable; could be check that throws better error
                 if not isinstance(force, int):
                     force = force[self.position]
             else:
                 force = self.seed
         return self.choices[force % len(self.choices)]
 
+    def ask(self):
+        question = self.choose()
+        return question.ask()
+
     @property
     def answered(self):
         """
 
         Returns:
 
         """
@@ -63,15 +82,15 @@
         force:
         seed:
         report:
     """
     # Choose a question
     if force is None:
         if seed is None:
-            force = MAIN_REPORT['questions']['seed']
+            force = report['questions']['seed']
             if isinstance(force, str):
                 force = _name_hash(force + name)
         else:
             force = seed
     elif isinstance(force, str):
         force = _name_hash(force + name)
     question = questions[force % len(questions)]
```

### Comparing `pedal-2.3.8/pedal/questions/setup.py` & `pedal-2.4.0/pedal/questions/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pedal.questions.constants import TOOL_NAME
 
 import hashlib
 
 
 def _name_hash(name: str) -> int:
     """ Turn a string name into a unique hashcode using MD5 """
+    name = ",".join(str(x) for x in bytes(name, 'utf-8'))
     return hashlib.md5(name.encode('utf8')).digest()[0]
 
 
 def reset(report=MAIN_REPORT):
     """
     Remove all settings for the Questions tool. Seed will be 0.
```

### Comparing `pedal-2.3.8/pedal/resolvers/__init__.py` & `pedal-2.4.0/pedal/resolvers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     Report all feedback, grouped by tool/category/priority/time.
 
 Full Summary
     Report all feedback but divided into frequencies of labels grouped by tool/category/priority/time.
 
 """
 
-from pedal.resolvers import simple
+from pedal.resolvers import simple as simple_resolver
 
 
 def print_resolve(*args, **kwargs):
     """
     Trivial formatter for resolver, just dumps the
     Title/Label/Score/Message. Any arguments are forwarded to
     :py:func:`pedal.resolvers.simple.resolve`
     """
-    result = simple.resolve(*args, **kwargs)
+    result = simple_resolver.resolve(*args, **kwargs)
     print("Title:", result.title)
     print("Label:", result.label)
     print("Score:", result.score)
     print("Message:", result.message)
     return result
```

### Comparing `pedal-2.3.8/pedal/resolvers/core.py` & `pedal-2.4.0/pedal/resolvers/core.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/resolvers/full.py` & `pedal-2.4.0/pedal/resolvers/full.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,33 +15,35 @@
     Feedback.CATEGORIES.POSITIVE,
     Feedback.CATEGORIES.UNKNOWN
 ]
 
 
 def resolve_feedback(feedback):
     """
+    This function is used to resolve a single feedback object into a string.
 
     Args:
-        feedback:
+        feedback: The feedback object to resolve.
 
     Returns:
-
+        str: The resolved feedback.
     """
     return "{title}\n{body}".format(title=feedback.title, body=feedback.message)
 
 
 @make_resolver
 def resolve(report=MAIN_REPORT, priority_key=by_priority):
     """
+    This function is used to resolve the feedback objects in the report into a FinalFeedback object.
 
     Args:
-        report:
+        report: The report to resolve.
 
     Returns:
-
+        FinalFeedback: The resolved feedback.
     """
 
     # Prepare feedbacks
     feedbacks = report.feedback + report.ignored_feedback
     feedbacks.sort(key=priority_key)
     # Create the initial final feedback
     final = FinalFeedback(success=True, score=0,
```

### Comparing `pedal-2.3.8/pedal/resolvers/sectional.py` & `pedal-2.4.0/pedal/resolvers/sectional.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
 A version of the resolver that still chooses one piece of feedback, but
 does so per section.
 """
 
-import sys
-
 from pedal.core.feedback import Feedback
-from pedal.core.final_feedback import parse_feedback, FinalFeedback
-from pedal.resolvers import simple
+from pedal.core.final_feedback import FinalFeedback
 from pedal.core.report import MAIN_REPORT
 from pedal.resolvers.core import make_resolver
 from pedal.resolvers.simple import by_priority
 
 
 @make_resolver
 def resolve(report=MAIN_REPORT, priority_key=by_priority):
```

### Comparing `pedal-2.3.8/pedal/resolvers/simple.py` & `pedal-2.4.0/pedal/resolvers/simple.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/resolvers/statistics.py` & `pedal-2.4.0/pedal/resolvers/statistics.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/sandbox/__init__.py` & `pedal-2.4.0/pedal/sandbox/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
     Resets (or initializes) the Sandbox instance for this report.
     Completely destroys the existing Sandbox instance attached to this report;
     if you want to just clear out its data, then instead use
     :py:func:`pedal.sandbox.commands.clear_sandbox`.
 
     Args:
-        report:
+        report: The report to reset the Sandbox for.
     """
     report[TOOL_NAME] = {
         'sandbox': Sandbox(report=report)
     }
 
 
 Report.register_tool(TOOL_NAME, reset)
```

### Comparing `pedal-2.3.8/pedal/sandbox/commands.py` & `pedal-2.4.0/pedal/sandbox/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     Args:
         code (str or :py:class:`~pedal.cait.cait_node.CaitNode` or None):
             The code to execute.
         filename (str or None): The filename to use for this code.
         inputs (list[str]): Optional inputs to be passed to
             :py:func:`~pedal.sandbox.Sandbox.set_input`.
-        threaded (bool): Whether or not to run this code in a threaded
+        threaded (bool): Whether to run this code in a threaded
             environment, which allows for timeouts.
         after (str): Code to run after this code (without a filename).
         before (str): Code to run before this code (without a filename).
         report (:py:class:`pedal.core.report.Report`): The report with the
             sandbox instance.
 
     Returns:
@@ -115,15 +115,20 @@
             returned instead.
     """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     return sandbox.evaluate(code, target=target, threaded=threaded)
 
 
 def clear_input(report=MAIN_REPORT):
-    """ Removes any existing inputs set up for the sandbox. """
+    """
+    Removes any existing inputs set up for the sandbox.
+
+    Args:
+        report (:py:class:`pedal.core.report.Report`): The report to clear inputs for
+    """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     sandbox.clear_input()
 
 
 def queue_input(*inputs, report=MAIN_REPORT):
     """
     Adds the given ``*inputs`` to be used as input during subsequent
@@ -175,35 +180,60 @@
             next student call of :py:func:`input`.
     """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     return sandbox.inputs
 
 
 def clear_output(report=MAIN_REPORT):
-    """ Removes any existing outputs associated with the sandbox. """
+    """
+    Removes any existing outputs associated with the sandbox.
+
+    Args:
+        report (:py:class:`pedal.core.report.Report`): The report to clear outputs for.
+    """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     sandbox.clear_output()
 
 
 def get_output(report=MAIN_REPORT):
-    """ Retrieves the current output (whatever the student has printed) since
-    execution began. """
+    """
+    Retrieves the current output (whatever the student has printed) since
+    execution began.
+
+    Args:
+        report (:py:class:`pedal.core.report.Report`): The report to get the output for.
+
+    Returns:
+        list[str]: The current output.
+    """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     return sandbox.output
 
 
 def get_exception(report=MAIN_REPORT):
-    """ Returns an exception if one occurred during the last execution,
-    otherwise returns None. """
+    """
+    Returns an exception if one occurred during the last execution,
+    otherwise returns None.
+
+    Args:
+        report (:py:class:`pedal.core.report.Report`): The report to get the exception for.
+    Returns:
+        Exception or None: The exception that occurred, or None if no exception
+    """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     return sandbox.exception
 
 
 def clear_student_data(report=MAIN_REPORT):
-    """ Removes any data in the student namespace. """
+    """
+    Removes any data in the student namespace.
+
+    Args:
+        report (:py:class:`pedal.core.report.Report`): The report to clear the data for.
+    """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     sandbox.clear_data()
 
 
 def get_student_data(report=MAIN_REPORT):
     """
     Retrieves the current data in the student namespace. Note that this is
@@ -254,16 +284,14 @@
 
     Returns:
         list[int]: The list of lines that have been executed in the student's
             code.
     """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     return sandbox.trace.lines
-    # Coverage version:
-    # return sandbox.trace.lines - sandbox.trace.missing
 
 
 def get_call_arguments(function_name, report=MAIN_REPORT):
     """
     Retrieves all the arguments that were passed into the given function when it
     was called.
 
@@ -371,14 +399,35 @@
 
 def allow_module(module_name, report=MAIN_REPORT):
     """ Explicitly allow students to use the given module. """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     sandbox.allow_module(module_name)
 
 
+def allow_real_io(report=MAIN_REPORT):
+    """
+    Allow the input() and print() functions to actually write to the real stdout.
+    By default, Pedal will block this kind of writing/reading normally (although students can
+    still use those functions).
+    """
+    sandbox: Sandbox = report[TOOL_NAME]['sandbox']
+    sandbox.allow_function('print')
+    sandbox.set_input(input)
+
+
+def block_real_io(report=MAIN_REPORT):
+    """
+    Explicitly block students from using the input() and print() functions to write/read
+    to the real stdout. This does not prevent them from using the functions, but it does
+    prevent the output from appearing in the real console.
+    """
+    sandbox: Sandbox = report[TOOL_NAME]['sandbox']
+    sandbox.clear_mocked_function('print')
+    sandbox.clear_input()
+
 def mock_module(module_name, new_version, friendly_name=None, report=MAIN_REPORT):
     """
     Provide an alternative version of the given module.
 
     Args:
         module_name (str): The importable name of the module.
         new_version (dict | :py:class:`pedal.sandbox.mocked.MockModule`): The
@@ -395,30 +444,44 @@
 
 def block_module(module_name, report=MAIN_REPORT):
     """ Cause an error if students use the given module. """
     sandbox: Sandbox = report[TOOL_NAME]['sandbox']
     sandbox.block_module(module_name)
 
 
+def get_module(module_name, report=MAIN_REPORT):
+    """ Loads the data for the given mocked module, if available (otherwise raises exception) """
+    sandbox: Sandbox = report[TOOL_NAME]['sandbox']
+    if hasattr(sandbox.modules, module_name):
+        return getattr(sandbox.modules, module_name)
+    raise ValueError(f"Unknown Sandbox Module: `{module_name}`")
+
+
 class CommandBlock:
     """
     Context Manager for creating instructor blocks of code that will
     be shown together to the student.
 
     TODO: What about named points where you can "rewind" the state to?
     """
 
     sandbox: Sandbox
 
     def __init__(self, report=MAIN_REPORT):
         self.sandbox = report[TOOL_NAME]['sandbox']
+        self.context_id = None
+        self.context = None
 
     def __enter__(self):
         self.sandbox.start_grouping_context()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.sandbox.stop_grouping_context()
+        self.context = self.sandbox.get_context()
+        self.context_id = self.sandbox.stop_grouping_context()
 
 
 # TODO: Deprecate these!
 reset_output = clear_output
+
+
+# TODO: Add function to get PREVIOUS inputs
```

### Comparing `pedal-2.3.8/pedal/sandbox/data.py` & `pedal-2.4.0/pedal/sandbox/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,18 +42,24 @@
     """ Enumeration of sandbox execution kind's. """
     RUN = 'run'
     EVAL = 'eval'
     CALL = 'call'
     GETITEM = 'getitem'
 
     @staticmethod
-    def describe_action(kind):
-        """ Produces the relevant Action message for the given kind
-        of context """
-        if kind == SandboxContextKind.EVAL:
+    def describe_action(context):
+        """
+        Produces the relevant Action message for the given kind of context.
+
+        Args:
+            context (SandboxContext): The context to describe.
+        Returns:
+            str: The description of the action.
+        """
+        if context.kind == SandboxContextKind.EVAL and context.target in ("", "_"):
             return 'I evaluated the expression'
         else:
             return 'I ran the code'
 
 
 class SandboxContext:
     """
@@ -95,48 +101,81 @@
         self.output = output
         self.exception = exception
         self.submission = submission
         self.called = called
         self.args = args
 
     def clone(self, context_id):
-        """ Create a separate copy of this item. Inputs will be deepcopied. """
+        """
+        Create a separate copy of this item. Inputs will be deep-copied.
+
+        Args:
+            context_id (int): The new context ID.
+        Returns:
+            SandboxContext: The new context, copied from the old one except with a new ID.
+        """
         return SandboxContext(context_id, self.code, self.filename,
                               self.kind, self.target, list(self.inputs),
                               self.output, self.exception, self.submission)
 
 
 class ExecutionTextHolder:
-    def __init__(self, format):
+    """
+    Helper class for formatting the text of an execution. Keeps track of the last action taken, the current body,
+    and the current formatter for this Report.
+
+    Args:
+        format (ReportFormatter): The formatter to use for this Report.
+    """
+    def __init__(self, report_format):
         self._result = []
         self._last_action = None
         self._current_body = []
-        self._format = format
+        self._format = report_format
 
     def add_message(self, action_message, body=None):
+        """
+        Add a message to the text of the execution.
+
+        Args:
+            action_message (str): The message to add.
+            body (str): The body of the message, if any.
+        """
         if action_message != self._last_action and self._last_action is not None:
             self._finish_body()
         if body:
             self._current_body.append(body)
         self._last_action = action_message
 
     def _finish_body(self):
+        """
+        Finish the current body, if any, and add it to the result.
+        """
         if self._current_body:
             code_message = self._format.python_code("\n".join(self._current_body))
             message = self._last_action + "\n"+code_message + "\n"
             self._result.append(message)
             self._current_body = []
         elif self._last_action:
             self._result.append(self._last_action+"\n")
 
     def get_lines(self):
+        """
+        Get the lines of the execution text, as a single string.
+
+        Returns:
+            str: The lines of the execution text.
+        """
         self._finish_body()
         return "".join(self._result)
 
 
+INPUT_MAXIMUM_LINES = 30
+
+
 def format_contexts(contexts, format):
     """
     Create a text string representation from a list of contexts.
 
     Args:
         contexts (list[list[SandboxContext]]): The list of list of sandbox
             executions. The inner list is because we could have a group of
@@ -148,25 +187,29 @@
         str: The string representation of the contexts.
     """
     execution_text = ExecutionTextHolder(format)
     inputs_text = []
     for context_group in contexts:
         for context in context_group:
             if context.filename in (None, context.submission.instructor_file):
-                action_message = SandboxContextKind.describe_action(context.kind)
+                action_message = SandboxContextKind.describe_action(context)
                 execution_text.add_message(action_message+":", context.code)
             elif context.filename in (context.submission.main_file, ):
                 execution_text.add_message(f"I ran your code.")
             else:
                 filename_message = format.filename(context.filename)
                 execution_text.add_message(f"I ran the file {filename_message}.")
             inputs_text.extend(context.inputs)
     final_text = [execution_text.get_lines()]
     if inputs_text:
-        inputs = "\n".join(inputs_text)
+        if len(inputs_text) > INPUT_MAXIMUM_LINES:
+            midpoint = int(INPUT_MAXIMUM_LINES / 2)
+            missed = len(inputs_text) - INPUT_MAXIMUM_LINES
+            inputs_text = inputs_text[:midpoint] + [f"... (Skipping {missed} other inputs) ..."] + inputs_text[-midpoint:]
+        inputs = "\n".join(inputs_text) + " "
         inputs_message = format.inputs(inputs)
         final_text.append(f"And I entered as input:{inputs_message}")
     return "\n".join(final_text)
 
 
 class SandboxModules:
     """
@@ -190,20 +233,22 @@
             friendly_name (str): The name to use when accessing this module's
                 data via attribute lookup.
 
         Returns:
             dict[str,:py:class:`types.ModuleType`]: The newly created modules
                 mapped by their imported path names.
         """
+        if isinstance(data, MockModule):
+            import_name = [import_name, *data.SUBMODULES]
         root, modules, target = create_module(import_name)
         if isinstance(data, dict):
             mocked_module = MockDictModule(data)
             mocked_module.add_to_module(target)
         elif isinstance(data, MockModule):
-            data.add_to_module(target)
+            data.add_to_module(target, modules)
         else:
             raise ValueError("Given data must be either MockModule or dict.")
         self._modules[friendly_name] = data
         return modules
 
     def __getattr__(self, name):
         return self._modules[name]
```

### Comparing `pedal-2.3.8/pedal/sandbox/exceptions.py` & `pedal-2.4.0/pedal/sandbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/sandbox/feedbacks.py` & `pedal-2.4.0/pedal/sandbox/feedbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from pedal.sandbox.data import format_contexts
 from pedal.utilities.exceptions import KeyError, get_exception_name
 from pedal.core.feedback import FeedbackResponse
 from pedal.sandbox import TOOL_NAME
 from pedal.utilities.text import add_indefinite_article
 
 RUNTIME_ERROR_MESSAGE_HEADER = (
+    "{context_message}\n"
     "{exception_name} occurred:\n\n"
     "{exception_message}\n\n"
-    "{context_message}\n"
-    "The traceback was:\n{traceback_message}\n"
+    "{traceback_message}\n"
 )
 
 
 class runtime_error(FeedbackResponse):
     """
     Used to create all runtime errors.
 
@@ -43,23 +43,28 @@
     version = '1.1.0'
     message_template = RUNTIME_ERROR_MESSAGE_HEADER
 
     def __init__(self, exception, context, traceback, location, **kwargs):
         report = kwargs.get('report', MAIN_REPORT)
         exception_name = get_exception_name(exception)
         exception_name_proper = add_indefinite_article(exception_name)
-        exception_message = str(exception).capitalize()
+        exception_message = str(exception)
+        exception_message = exception_message[0].upper() + exception_message[1:] if exception_message else ""
         if type(exception) not in EXCEPTION_FF_MAP:
             title = exception_name
         else:
             title = EXCEPTION_FF_MAP[type(exception)].title
         location = Location(location)
         traceback_stack = traceback.build_traceback()
         traceback_message = traceback.format_traceback(traceback_stack,
                                                        report.format)
+        if not traceback_message:
+            traceback_message = ""
+        else:
+            traceback_message = f"The traceback was:\n{traceback_message}"
         context_message = format_contexts(context, report.format)
         fields = {'exception': exception,
                   'exception_name': exception_name_proper,
                   'exception_message': report.format.exception(exception_message),
                   'location': location,
                   'traceback': traceback,
                   'traceback_stack': traceback_stack,
```

### Comparing `pedal-2.3.8/pedal/sandbox/result.py` & `pedal-2.4.0/pedal/sandbox/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,7 +425,8 @@
 def unwrap_value(value):
     """ Given either a SandboxResult or a regular value, make sure we have
     the actual value. """
     if is_sandbox_result(value):
         return value._actual_value
     else:
         return value
+
```

### Comparing `pedal-2.3.8/pedal/sandbox/sandbox.py` & `pedal-2.4.0/pedal/sandbox/sandbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 
 TODO: Handle sys.argv
 
 """
 
 import sys
 import io
+import types
 from itertools import zip_longest
 from unittest.mock import patch
 
 from pedal.core.feedback_category import FeedbackCategory
 from pedal.core.report import MAIN_REPORT
+from pedal.sandbox.mocked import PrintingStringIO
 from pedal.utilities.exceptions import ExpandedTraceback, improve_builtin_exceptions
 from pedal.sandbox.data import SandboxVariable, SandboxContextKind, \
     SandboxContext, SandboxModules
 from pedal.sandbox import mocked
 from pedal.sandbox.constants import TOOL_NAME
 from pedal.sandbox.feedbacks import runtime_error, EXCEPTION_FF_MAP
 from pedal.sandbox.exceptions import SandboxHasNoFunction, SandboxHasNoVariable
@@ -54,15 +56,16 @@
         _next_context_id (int): The ID of the next execution context.
         _current_patches (list[Patch]): A stack of patches that are currently
             being used. This allows recursive patching behavior.
         MAXIMUM_TEMPORARY_LENGTH (int): How long to allow arguments to be before
             turning them into temporary variables.
     """
 
-    MAXIMUM_TEMPORARY_LENGTH = 25
+    MAXIMUM_TEMPORARY_LENGTH = 200
+    MAXIMUM_INPUTS = 100000
 
     def __init__(self, report=MAIN_REPORT):
         self.report = report
         # Namespace
         self.data = {}
         self.result = None
         self.exception = None
@@ -100,14 +103,51 @@
         self.allowed_time = 3
         # Tracer Styles
         self.tracer_style = 'none'
 
     ############################################################################
     # Execution (run/call/eval)
 
+    def _import(self, code, module_name, filename, threaded, **meta):
+        """
+        Import the code as a new module. Requires prior `_execute` of some
+        manner to have already started (e.g., a `call`, `run`, or `evaluate`).
+        This does NOT reset the context, setup output capturing, or handle exceptions.
+        Instead, it relies on the existing infrastructure to do so.
+
+        Args:
+            code:
+            module_name:
+            threaded:
+            **meta:
+
+        Returns:
+
+        """
+        if threaded:
+            return timeout(self.allowed_time, self._import, code, module_name, filename, False, **meta)
+        # TODO: Skulpt doesn't support `module.__dict__` manipulation,
+        #   but once it does we don't need to manually copy over the attrs afterwards
+        imported_module = types.ModuleType(module_name)
+        # Patch the builtins using the same rules as `execute`
+        #    EXCEPT only the builtins, not the other stuff?
+        imported_module_data = {}
+        self._reset_builtins(imported_module_data)
+        builtins = self._module_overrides.get('__builtins__', {})
+        self._mock_builtins(imported_module_data, builtins)
+        # Compile and execute code
+        compiled_code = compile(code, filename, 'exec')
+        with self.trace.as_filename(filename, code):
+            exec(compiled_code, imported_module_data)
+        # Copy over data to module
+        for key, value in imported_module_data.items():
+            setattr(imported_module, key, value)
+        # And get them back the module
+        return imported_module
+
     def _execute_with_timeout(self, code, filename, kind, **meta):
         """
         Execute the given code, but stop after `self.allowed_time`.
         Args:
             code (str):
             filename (str):
             kind (:py:class:`pedal.sandbox.sandbox_mixins.SandboxContextKind`):
@@ -344,24 +384,24 @@
             else:
                 return self._context[self._context_group_start[-1]:]
         else:
             if not self._context_group_start:
                 return [self._context[context_id]]
             else:
                 for past_context_group_starts in self._context_group_start[::-1]:
-                    if past_context_group_starts < context_id+1:
-                        return self._context[past_context_group_starts:context_id+1]
-                return self._context[:context_id+1]
+                    if past_context_group_starts < context_id + 1:
+                        return self._context[past_context_group_starts:context_id + 1]
+                return self._context[:context_id + 1]
 
     def _guess_context(self, target_name):
         """
         Tries to figure out the best context for the given target_name, by
         first checking whether the target was ever used in a CALL or EVAL.
         If it fails to find it, then it uses the most recent RUN. Otherwise,
-        it just just returns None.
+        it just returns None.
 
         Returns:
             :py:class:`pedal.sandbox.data.SandboxContext` or None: The found
                 context, or None.
         """
         # Was it a target for a CALL or EVAL?
         for context in self._context[::-1]:
@@ -377,15 +417,15 @@
 
     def start_grouping_context(self):
         """ Any subsequent executions will be grouped. """
         self._context_group_start.append(self._next_context_id)
 
     def stop_grouping_context(self):
         """ Stop grouping subsequent executions. """
-        self._context_group_start.pop()
+        return self._context_group_start.pop()
 
     def clear_context(self):
         """ Removes the history of any previous executions. """
         self._context_group_start.clear()
         self._context.clear()
 
     ############################################################################
@@ -448,39 +488,50 @@
         """ Removes the latest exception information """
         self.exception = None
         self.feedback = None
 
     ############################################################################
     # Patching and Mocking
 
+    # TODO: Need to make this cover the `builtins` module, and look into best practices
+    #   for modern Python mocking, to prevent evil access.
+
+    def _mock_builtins(self, data: dict, builtins: dict):
+        builtins = builtins
+        for name, value in builtins.items():
+            if value is True:
+                data['__builtins__'][name] = mocked.ORIGINAL_BUILTINS[name]
+                data[name] = mocked.ORIGINAL_BUILTINS[name]
+            elif value is False:
+                data['__builtins__'][name] = mocked.disabled_builtin(name)
+                data[name] = mocked.disabled_builtin(name)
+            else:
+                data['__builtins__'][name] = value
+                data[name] = value
+
     def _start_mocking(self, context: SandboxContext):
         """ Mock input, output, builtins, and modules """
         # Handle input tracking
         self.mock_function('input', self._track_inputs(context.inputs))
         # Override builtin functions
-        self.reset_builtins()
+        self._reset_builtins(self.data)
         builtins = self._module_overrides.pop('__builtins__', {})
-        for name, value in builtins.items():
-            if value is True:
-                self.data['__builtins__'][name] = mocked.ORIGINAL_BUILTINS[name]
-                self.data[name] = mocked.ORIGINAL_BUILTINS[name]
-            elif value is False:
-                self.data['__builtins__'][name] = mocked.disabled_builtin(name)
-                self.data[name] = mocked.disabled_builtin(name)
-            else:
-                self.data['__builtins__'][name] = value
-                self.data[name] = value
+        self._mock_builtins(self.data, builtins)
         # Override sys modules
         overridden_modules = sys.modules.copy()
         for name, value in self._module_overrides.items():
             if value is not True:
                 overridden_modules[name] = value
         self._module_overrides['__builtins__'] = builtins
+        # Handle allowing *actual* printing to the real stdout console
+        if self._module_overrides['__builtins__'].get('print') is not True:
+            self._current_stdout.append(io.StringIO())
+        else:
+            self._current_stdout.append(PrintingStringIO())
         # And do the patches
-        self._current_stdout.append(io.StringIO())
         self._start_patches(
             patch.dict('sys.modules', overridden_modules),
             patch('sys.stdout', self._current_stdout[-1]),
             patch('time.sleep', return_value=None),
         )
 
     def _stop_mocking(self, context: SandboxContext):
@@ -500,19 +551,25 @@
         """ Helper function to end any tracked patches """
         if not self._current_patches:
             return
         patches = self._current_patches.pop()
         for a_patch in patches:
             a_patch.stop()
 
-    def clear_mocks(self):
-        """ Removes any module or builtin overrides currently in effect. """
+    def clear_mocks(self, reset_default_mocks=True):
+        """
+        Removes any module or builtin overrides currently in effect.
+
+        Args:
+            reset_default_mocks (bool): If True, also resets the default mocks (e.g., `open`, `__import__`).
+        """
         self._module_overrides.clear()
         self.modules.clear()
-        self.reset_default_overrides()
+        if reset_default_mocks:
+            self.reset_default_overrides()
 
     def reset_default_overrides(self):
         """
         Resets the list of blocked functions and modules to its starting
         state. This blocks ``compile``, ``eval``, ``exec``, ``globals``,
         and provides mocked versions of ``open`` and ``import`` that are
         more restricted. It also blocks the ``pedal`` module.
@@ -520,28 +577,39 @@
         self._module_overrides['__builtins__'] = {}
         self.block_function('compile')
         self.block_function('eval')
         self.block_function('exec')
         self.block_function('globals')
         self.block_function('exit')
         self.mock_function('open', mocked.create_open_function(self.report))
-        self.mock_function('__import__', mocked.create_import_function(self.report))
+        self.mock_function('__import__', mocked.create_import_function(self.report, self))
         self.block_module('pedal')
         self.mock_module('turtle', mocked.MockTurtle(), 'turtles')
         self.mock_module('matplotlib.pyplot', mocked.MockPlt(), 'plotting')
+        self.mock_module('designer', mocked.MockDesigner(), 'designer')
+        self.mock_module('microbit', mocked.MockMicrobit(), 'microbit')
 
     def mock_function(self, function_name, new_version):
         self._module_overrides['__builtins__'][function_name] = new_version
 
     def allow_function(self, function_name):
         self._module_overrides['__builtins__'][function_name] = True
 
     def block_function(self, function_name):
         self._module_overrides['__builtins__'][function_name] = False
 
+    def clear_mocked_function(self, function_name):
+        """
+        Removes the mocking associated with the given function name.
+
+        Args:
+            function_name (str): The name of the function to be mocked.
+        """
+        del self._module_overrides['__builtins__'][function_name]
+
     def allow_module(self, module_name):
         """
 
         Args:
             module_name (str):
 
         Returns:
@@ -556,26 +624,36 @@
             friendly_name = module_name
         mocked_modules = self.modules.new_module(new_version, module_name, friendly_name)
         for name, mocked_version in mocked_modules.items():
             if name not in self._module_overrides or not self._module_overrides[name]:
                 self._module_overrides[name] = mocked_version
         return self
 
-    def block_module(self, module_name):
+    def block_module(self, module_name, friendly_name=None):
         """
         Prevent the module from being loaded in student code.
+        Also unloads the module if it has been imported previously by
+        destroying the variable in the current student `data`.
 
         Args:
             module_name (str): The name of the module to prevent, as it would
                 be used by import (e.g., ``"matplotlib.pyplot"``).
 
         Returns:
             Sandbox: This sandbox.
         """
-        self._module_overrides[module_name] = mocked.BlockedModule(module_name)
+        if friendly_name is None:
+            friendly_name = module_name
+        mocked_modules = self.modules.new_module(mocked.BlockedModule(module_name), module_name, friendly_name)
+        for name, mocked_version in mocked_modules.items():
+            if name not in self._module_overrides or self._module_overrides[name] is True:
+                self._module_overrides[name] = mocked_version
+            if name in self.data:
+                del self.data[name]
+        # self._module_overrides[module_name] = mocked.BlockedModule(module_name)
         return self
 
     ############################################################################
     # Code generation
 
     def _construct_call(self, function, args, kwargs, args_locals, kwargs_locals,
                         target):
@@ -656,29 +734,37 @@
         current_addition = ""
         attempt_index = 2
         while name + current_addition in self.data:
             current_addition = "_{}".format(attempt_index)
             attempt_index += 1
         return name + current_addition
 
-
     ############################################################################
     # Data Namespace Management
 
     def clear_data(self):
         # Temporary data
         self.data.clear()
         self._temporary_variables.clear()
         self._backup_variables.clear()
-        self.reset_builtins()
+        self._reset_builtins(self.data)
+
+    @staticmethod
+    def _reset_builtins(data: dict):
+        """
+        Replace all the existing given `data` with the builtin mocked data.
+        Args:
+            data:
 
-    def reset_builtins(self):
-        self.data['__builtins__'] = {}
+        Returns:
+
+        """
+        data['__builtins__'] = {}
         for name, value in mocked._default_builtins.items():
-            self.data['__builtins__'][name] = value
+            data['__builtins__'][name] = value
 
     def set_student_data(self, new_data):
         """
         Overwrites the existing student data with the keys and values from
         the ``new_data``. This copies the data over, but does not modify the
         reference to ``data``'s dictionary.
 
@@ -780,15 +866,15 @@
             return self.result_proxy_class(value, context_id=context_id,
                                            sandbox=self)
         return value
 
     ############################################################################
     # Useful Dunders
 
-    #def __repr__(self):
+    # def __repr__(self):
     #    return "Sandbox({})".format()
 
     def __str__(self):
         return "Sandbox(contexts={context_count})".format(context_count=len(self._context))
 
     ############################################################################
     # Input Handling
@@ -816,28 +902,37 @@
             self.inputs = inputs
         return self
 
     def _track_inputs(self, context_inputs):
         """
         Wraps an input function with a tracker.
         """
+        self._called_inputs = 0
 
         def _input_tracker(*args, **kwargs):
             if args:
                 prompt = args[0]
             else:
                 prompt = ""
-            print(prompt)
-            if self.inputs:
+            if callable(self.inputs):
+                value_entered = self.inputs(prompt)
+            elif self.inputs:
+                print(prompt)
                 value_entered = self.inputs.pop(0)
             else:
                 # TODO: Make this smarter, more elegant in choosing IF we should repeat 0
+                print(prompt)
                 value_entered = '0'
             self._context[-1].inputs.append(value_entered)
-            #context_inputs.append(value_entered)
+            self._called_inputs += 1
+            if self.MAXIMUM_INPUTS is not None:
+                if self.MAXIMUM_INPUTS <= self._called_inputs:
+                    raise IOError(
+                        f"Asked for user input too many times ({self._called_inputs} times). Perhaps you have an infinite loop?")
+            # context_inputs.append(value_entered)
             return value_entered
 
         return _input_tracker
 
     ############################################################################
     # Output Handling
```

### Comparing `pedal-2.3.8/pedal/sandbox/timeout.py` & `pedal-2.4.0/pedal/sandbox/timeout.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/sandbox/tracer.py` & `pedal-2.4.0/pedal/sandbox/tracer.py`

 * *Files 20% similar despite different names*

```diff
@@ -109,14 +109,16 @@
     was something people wanted.
 
     TODO: Handle multiple submission files?
     """
     def __init__(self):
         super().__init__()
         self.calls = {}
+        self.returns = {}
+        self.call_stack = []
         self.lines = []
         self.old_tracer = None
         self.step_index = 1
 
     def __enter__(self):
         self.old_tracer = sys.gettrace()
         sys.settrace(self.tracer)
@@ -135,17 +137,27 @@
             self.lines.append(line)
             self.step_index += 1
         if event == 'call' and self.is_tracked_file(frame):
             called_function = frame.f_code.co_name
             if called_function != '<module>':
                 if called_function not in self.calls:
                     self.calls[called_function] = []
+                if called_function not in self.returns:
+                    self.returns[called_function] = []
                 arguments = {name: frame.f_locals[name] for name in frame.f_code.co_varnames
                              if name in frame.f_locals}
                 self.calls[called_function].append(arguments)
+                # Haha oh god why would you do this? Abusing mutable state!
+                placeholder = []
+                self.returns[called_function].append(placeholder)
+                self.call_stack.append(placeholder)
+        if event == 'return' and self.is_tracked_file(frame):
+            if self.call_stack:
+                placeholder = self.call_stack.pop()
+                placeholder.append(args)
         return self.tracer
 
 
 class SandboxCallTracer(SandboxBasicTracer, Bdb):
     """
 
     """
```

### Comparing `pedal-2.3.8/pedal/source/__init__.py` & `pedal-2.4.0/pedal/source/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 
 """
 
 from pedal.source.constants import TOOL_NAME
 from pedal.source.sections import (separate_into_sections, check_section_exists,
                                    stop_sections, next_section)
 from pedal.source.source import (verify, verify_section, set_source, set_source_file, get_program)
-
+#from pedal.source.rewrite import unparse
 
 __all__ = ['TOOL_NAME',
            'set_source', 'verify', 'set_source_file', 'get_program',
            'separate_into_sections',
            'check_section_exists', 'next_section', 'verify_section',
            ]
```

### Comparing `pedal-2.3.8/pedal/source/feedbacks.py` & `pedal-2.4.0/pedal/source/feedbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,23 +50,24 @@
     def __init__(self, name, sections, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         fields = {'name': name, 'sections': sections}
         group = 0 if sections else kwargs.get('group')
         super().__init__(fields=fields, group=group, **kwargs)
 
 
+
 class syntax_error(SourceFeedback):
     """ Generic feedback for any kind of syntax error. """
     muted = False
     title = "Syntax Error"
     message_template = ("Bad syntax on line {lineno:line}\n\n"
-                        "The traceback was:\n{traceback_message}\n\n"
+                        "{traceback_message}\n"
                         "Suggestion: Check line {lineno:line}, the line "
-                        "before it, and the line after it.")
-    version = '0.0.1'
+                        "before it, and the line after it. Remember to ignore blank lines.")
+    version = '0.0.2'
     justification = "Syntax error was triggered while calling ast.parse"
 
     def __init__(self, line, filename, code, col_offset,
                  exception, exc_info, **kwargs):
         report = kwargs.get('report', MAIN_REPORT)
         files = report.submission.get_files_lines()
         if filename not in files:
@@ -80,31 +81,47 @@
         line_offset = line_offsets.get(filename, 0)
         traceback = ExpandedTraceback(exception, exc_info, False,
                                       [report.submission.instructor_file],
                                       line_offsets, [filename], lines, files)
         traceback_stack = traceback.build_traceback()
         traceback_message = traceback.format_traceback(traceback_stack,
                                                        report.format)
+        if not traceback_message:
+            traceback_message = ""
+        else:
+            traceback_message = f"The traceback was:\n{traceback_message}"
         line_offset = line_offsets.get(filename, 0)
         fields = {'lineno': line+line_offset,
                   'filename': filename, 'offset': col_offset,
                   'exception': exception,
+                  'exception_message': str(exception),
                   'traceback': traceback,
                   'traceback_stack': traceback_stack,
                   'traceback_message': traceback_message}
         location = Location(line=line+line_offset, col=col_offset, filename=filename)
         super().__init__(fields=fields, location=location, **kwargs)
 
 
 class incorrect_number_of_sections(SourceFeedback):
     """ Incorrect number of sections """
     title = "Incorrect Number of Sections"
     message_template = ("Incorrect number of sections in your file. "
-                     "Expected {count}, but only found {found}")
+                        "Expected {count}, but only found {found}")
     justification = ""
 
     def __init__(self, count, found, **kwargs):
         fields = {'count': count, 'found': found}
         super().__init__(fields=fields, **kwargs)
 
-# TODO: IndentationError
 # TODO: TabError
+
+
+class indentation_error(syntax_error):
+    """ Generic feedback for indentation errors. """
+    title = "Indentation Error"
+    message_template = ("Bad indentation on line {lineno:line} or adjacent line.\n"
+                        "{exception_message:exception}\n\n"
+                        "{traceback_message}\n"
+                        "Suggestion: Check line {lineno:line}, the line "
+                        "before it, and the line after it. Remember to ignore blank lines.")
+    version = '0.0.1'
+    justification = "Indentation error was triggered while calling ast.parse"
```

### Comparing `pedal-2.3.8/pedal/source/sections.py` & `pedal-2.4.0/pedal/source/sections.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/source/source.py` & `pedal-2.4.0/pedal/source/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,23 @@
     :widths: 20, 20, 20, 40
 
     "substitutions", "List[Substitution]", "[]", "The history of previous source codes before the latest substitutions."
     "success", "bool", "None", "Whether the current file has been parsed successfully."
     "ast", "ast.Ast", "None", "The root node of the latest successfully parsed chunk of code."
 
 """
-import os
 import sys
 import ast
 
 from pedal.core.feedback import CompositeFeedbackFunction
 from pedal.core.report import Report, MAIN_REPORT
 from pedal.core.submission import Submission
 from pedal.source.constants import TOOL_NAME, DEFAULT_STUDENT_FILENAME
 from pedal.source.sections import separate_into_sections
-from pedal.source.feedbacks import blank_source, syntax_error, source_file_not_found
+from pedal.source.feedbacks import blank_source, syntax_error, source_file_not_found, indentation_error
 from pedal.source.substitutions import Substitution
 from pedal.utilities.files import find_possible_filenames
 
 
 def reset(report=MAIN_REPORT):
     """
     Resets the Source tool back to its initial configuration, removing any
@@ -103,15 +102,15 @@
     """
     if TOOL_NAME in report:
         old_submission = report[TOOL_NAME]['substitutions'].pop()
         report.submission.replace_main(old_submission.code, old_submission.filename)
         verify(report=report)
 
 
-@CompositeFeedbackFunction(blank_source, syntax_error)
+@CompositeFeedbackFunction(blank_source, syntax_error, indentation_error, source_file_not_found)
 def verify(code=None, filename=DEFAULT_STUDENT_FILENAME, report=MAIN_REPORT,
            muted=False):
     """
     Parses the given source code and checks for syntax errors; if no code is given, defaults to the
     current Main file of the submission.
 
     Args:
@@ -132,19 +131,25 @@
         return False
     if code.strip() == '':
         blank_source()
         report[TOOL_NAME]['success'] = False
     try:
         parsed = ast.parse(code, filename)
         report[TOOL_NAME]['ast'] = parsed
+    except IndentationError as e:
+        indentation_error(e.lineno, e.filename, code, e.offset, e,
+                     sys.exc_info(), report=report, muted=muted)
+        report[TOOL_NAME]['success'] = False
+        report[TOOL_NAME]['ast'] = ast.parse("")
     except SyntaxError as e:
         syntax_error(e.lineno, e.filename, code, e.offset, e,
                      sys.exc_info(), report=report, muted=muted)
         report[TOOL_NAME]['success'] = False
         report[TOOL_NAME]['ast'] = ast.parse("")
+        # TODO: Shouldn't this return early?
     report[TOOL_NAME]['success'] = True
     return report[TOOL_NAME]['success']
 
 
 # Legacy verify_section; now done by verify since its aware of sections
 verify_section = verify
```

### Comparing `pedal-2.3.8/pedal/tifa/__init__.py` & `pedal-2.4.0/pedal/tifa/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,30 +66,37 @@
         elements in an tuples.
 
     Name Map
         (Path x Fully Qualified Names) => States
 """
 from pedal.core.report import MAIN_REPORT, Report
 from pedal.tifa.constants import TOOL_NAME
+from pedal.tifa.settings import get_default_tifa_settings
 from pedal.tifa.tifa_visitor import Tifa
 from pedal.tifa.commands import *
+from pedal.types.new_types import reset_builtin_modules
 
 
 def reset(report=MAIN_REPORT):
     """
     Remove all the information associated with this tool.
 
     Args:
         report:
     """
     # TODO: Make it so we can reset TIFA through this, safely.
+    reset_builtin_modules()
     report[TOOL_NAME] = {
         'analyses': {},
         'latest': None,
-        'instance': Tifa(report=report)
+        'instance': Tifa(report=report),
+        'settings': get_default_tifa_settings(),
+        'types': {
+            'modules': {}
+        }
     }
     return report[TOOL_NAME]
 
 
 Report.register_tool(TOOL_NAME, reset)
```

### Comparing `pedal-2.3.8/pedal/tifa/commands.py` & `pedal-2.4.0/pedal/tifa/commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Commands related to navigating TIFA data.
 """
+import ast
 from pedal.core.report import MAIN_REPORT
 from pedal.tifa.constants import TOOL_NAME as TIFA_TOOL_NAME
+from pedal.types.new_types import ImpossibleType, ModuleType
 
 
 def tifa_analysis(code=None, report=MAIN_REPORT):
     """
     Perform the TIFA analysis and attach the results to the Report.
 
     Args:
@@ -24,14 +26,20 @@
         return report[TIFA_TOOL_NAME]['analyses'][code]
     result = report[TIFA_TOOL_NAME]['instance'].process_code(code)
     report[TIFA_TOOL_NAME]['analyses'][code] = result
     report[TIFA_TOOL_NAME]['latest'] = result
     return result
 
 
+def tifa_type_check(name: str, report=MAIN_REPORT):
+    tifa_instance = report[TIFA_TOOL_NAME]['instance']
+    variable = tifa_instance.find_variable_scope(name)
+    return variable.state.type if variable.exists else ImpossibleType()
+
+
 def get_issues(category, report=MAIN_REPORT):
     """
 
     Args:
         category (str or Feedback): The category of Issues to retrieve.
 
     Returns:
@@ -39,7 +47,23 @@
     """
     if not isinstance(category, str):
         category = category.__name__
     if not report[TIFA_TOOL_NAME]['latest']:
         tifa_analysis(report=report)
     latest = report[TIFA_TOOL_NAME]['latest']
     return latest.issues.get(category, [])
+
+
+def tifa_provide_module_type(name: str, fields, report=MAIN_REPORT):
+    """
+
+    Args:
+        name:
+        fields:
+
+    Returns:
+
+    """
+    if not isinstance(fields, ModuleType):
+        fields = ModuleType(name, fields)
+    report[TIFA_TOOL_NAME]['types']['modules'][name] = fields
+
```

### Comparing `pedal-2.3.8/pedal/tifa/contexts.py` & `pedal-2.4.0/pedal/tifa/contexts.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Context managers for dealing with paths and scopes.
 """
 
 
 class NewPath:
     """
     Context manager for entering and leaving execution paths (e.g., if
-    statements).)
+    statements).
 
     Args:
         tifa (Tifa): The tifa instance, so we can modify some of its
                      properties that track variables and paths.
         origin_path (int): The path ID parent to this one.
         name (str): The symbolic name of this path, typically 'i' for an IF
                     body and 'e' for ELSE body.
@@ -37,43 +37,47 @@
         self.tifa.path_names.pop()
         self.tifa.path_chain.pop(0)
 
 
 class NewScope:
     """
     Context manager for entering and leaving scopes (e.g., inside of
-    function calls).
+    function calls, class bodies).
 
     Args:
         tifa (Tifa): The tifa instance, so we can modify some of its
             properties that track variables and paths.
         definitions_scope_chain (list of int): The scope chain of the
             definition.
         class_type (ClassType): If this scope is a ClassType, then this
             will be available as a field.
     """
 
-    def __init__(self, tifa, definitions_scope_chain, class_type=None):
+    def __init__(self, tifa, definitions_scope_chain, class_type=None, is_module=False):
         self.tifa = tifa
         self.definitions_scope_chain = definitions_scope_chain
         self.class_type = class_type
+        self.is_module = is_module
 
     def __enter__(self):
         # Manage scope
         self.old_scope = self.tifa.scope_chain[:]
         # Move to the definition's scope chain
         self.tifa.scope_chain = self.definitions_scope_chain[:]
         # And then enter its body's new scope
         self.tifa.scope_id += 1
         self.tifa.scope_chain.insert(0, self.tifa.scope_id)
         # Register as class potentially
         if self.class_type is not None:
             self.class_type.scope_id = self.tifa.scope_id
             self.tifa.class_scopes[self.tifa.scope_id] = self.class_type
+        if self.is_module:
+            self.tifa.module_scopes[self.tifa.scope_id] = self.class_type
 
     def __exit__(self, exc_type, value, traceback):
         # Finish up the scope
-        self.tifa._finish_scope()
+        if not self.is_module:
+            self.tifa._finish_scope()
         # Leave the body
         self.tifa.scope_chain.pop(0)
         # Restore the scope
         self.tifa.scope_chain = self.old_scope
```

### Comparing `pedal-2.3.8/pedal/tifa/feedbacks.py` & `pedal-2.4.0/pedal/tifa/feedbacks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 All of the feedback responses generated by TIFA.
 """
+from pedal.types.new_types import ModuleType, FunctionType, ClassType
 from pedal.utilities.operators import OPERATION_DESCRIPTION
 from pedal.core.report import MAIN_REPORT
 from pedal.core.feedback import FeedbackResponse
 
 
 class TifaFeedback(FeedbackResponse):
     """ Base class for all TIFA feedback """
@@ -128,25 +129,30 @@
         super().__init__(location=location, name=name,
                          name_message=report.format.name(name), **kwargs)
 
 
 class unused_variable(TifaFeedback):
     """ Unused Variable """
     title = "Unused Variable"
-    message_template = ("The {kind} {name_message} was given a {initialization} on line "
+    message_template = ("The {kind} {name_message} was {initialization} on line "
                         "{location.line}, but was never used after that.")
     justification = ("TIFA stored a variable but it was not read any other time "
                      "in the program.")
 
     def __init__(self, location, name, variable_type, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
-        if variable_type.is_equal('function'):
-            kind, initialization = 'function', 'definition'
+        if isinstance(variable_type, ModuleType):
+            kind, initialization = 'module', 'imported'
+        elif isinstance(variable_type, FunctionType):
+            kind, initialization = 'function', 'given a definition'
+        elif isinstance(variable_type, ClassType):
+            kind, initialization = 'class', 'given a definition'
+        # TODO: Handle classes... anything else?
         else:
-            kind, initialization = 'variable', 'value'
+            kind, initialization = 'variable', 'given a value'
         fields = {'location': location, 'name': name, 'type': variable_type,
                   'name_message': report.format.name(name),
                   'kind': kind, 'initialization': initialization}
         if 'fields' in kwargs:
             fields.update(kwargs.pop('fields'))
         super().__init__(location=location, fields=fields, **kwargs)
 
@@ -249,34 +255,61 @@
                   'left_name': left_name, 'right_name': right_name}
         super().__init__(location=location, fields=fields, **kwargs)
 
 
 class parameter_type_mismatch(TifaFeedback):
     """ Parameter type mismatch """
     title = "Parameter Type Mismatch"
-    message_template = ("You defined the parameter {parameter_name_message} on line {location.line} "
-                        "as {parameter_type_name}. However, the argument passed to that parameter "
+    message_template = ("You defined the parameter {parameter_name_message} "
+                        "as {parameter_type_name}. However, the argument passed to that parameter on line {location.line} "
                         "was {argument_type_name}. The formal parameter type must match the argument's type."
                         )
     justification = "TIFA visited a function definition where a parameter type and argument type were not equal."
 
     def __init__(self, location, parameter_name, parameter, argument, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         parameter_type_name = parameter.singular_name
         argument_type_name = argument.singular_name
+        if parameter_type_name == argument_type_name:
+            argument_type_name = "a different kind of " + argument_type_name
         fields = {'location': location,
                   'parameter_name': parameter_name,
                   'parameter_name_message': report.format.name(parameter_name),
                   'parameter_type': parameter,
                   'argument_type': argument,
                   'parameter_type_name': parameter_type_name,
                   'argument_type_name': argument_type_name}
         super().__init__(location=location, fields=fields, **kwargs)
 
 
+class field_type_mismatch(TifaFeedback):
+    """ Field type mismatch """
+    title = "Field Type Mismatch"
+    message_template = ("You defined the field {field_name_message} "
+                        "as {field_type_name}. However, the argument passed to that field's parameter in the"
+                        " constructor function on line {location.line} was {argument_type_name}. The formal field"
+                        " type must match the argument's type."
+                        )
+    justification = "TIFA visited a constructor function call where a parameter type and argument type were not subtypes."
+
+    def __init__(self, location, field_name, field, argument, **kwargs):
+        report = kwargs.get("report", MAIN_REPORT)
+        field_type_name = field.singular_name
+        argument_type_name = argument.singular_name
+        if field_type_name == argument_type_name:
+            argument_type_name = "a different kind of " + argument_type_name
+        fields = {'location': location,
+                  'field_name': field_name,
+                  'field_name_message': report.format.name(field_name),
+                  'field_type': field,
+                  'field_type_name': field_type_name,
+                  'argument_type': argument,
+                  'argument_type_name': argument_type_name}
+        super().__init__(location=location, fields=fields, **kwargs)
+
 class read_out_of_scope(TifaFeedback):
     """ Read out of scope """
     title = "Read out of Scope"
     message_template = ("You attempted to read the variable {name_message} "
                         "from a different scope on line {location.line}. You "
                         "should only use variables inside the function they "
                         "were declared in."
@@ -302,14 +335,42 @@
         report = kwargs.get("report", MAIN_REPORT)
         fields = {'location': location, 'name': name,
                   'name_message': report.format.name(name),
                   'old': old, 'new': new}
         super().__init__(location=location, fields=fields, **kwargs)
 
 
+class attribute_type_change(TifaFeedback):
+    """ Type change on attribute """
+    title = "Attribute Type Change"
+    message_template = ("On line {location.line}, you attempted to assign a {new} to "
+                        "the attribute {attr_message}, which was supposed to be {old}.")
+    justification = ""
+    muted = False
+
+    def __init__(self, location, attr, old, new, **kwargs):
+        report = kwargs.get("report", MAIN_REPORT)
+        fields = {'location': location, 'attr': attr,
+                  'attr_message': report.format.name(attr),
+                  'old': old, 'new': new}
+        super().__init__(location=location, fields=fields, **kwargs)
+
+class type_change_append(TifaFeedback):
+    """ Type Change in an append Method """
+    title = "Type Change in Append"
+    message_template = ("You attempted to append a {new} to a list that was "
+                        "supposed to have {old} on line {location.line}.")
+    justification = ""
+    muted = True
+
+    def __init__(self, location, old, new, **kwargs):
+        fields = {'location': location, 'old': old, 'new': new}
+        super().__init__(location=location, fields=fields, **kwargs)
+
+
 class unnecessary_second_branch(TifaFeedback):
     """ Unnecessary second branch """
     title = "Unnecessary Second Branch"
     message_template = ("You have an `if` statement where one of the two branches"
                        " only has `pass` in its body, on line {location.line}."
                         " You shouldn't need an empty body.")
     justification = "There is an else or if statement who's body is just pass."
@@ -340,15 +401,15 @@
 
 
 class not_a_function(TifaFeedback):
     """ Not a function """
     title = "Not a Function"
     message_template = ("You attempted to call {name} as if it"
                         " was a function on line {location.line}. However,"
-                        " that expression was actually a {called_type}.")
+                        " that expression was actually {singular_name}.")
     justification = ""
     # TODO: Unmute?
     #muted = True
 
     def __init__(self, location, name, called_type, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
         singular_name = called_type.singular_name
@@ -357,22 +418,26 @@
                   'singular_name': singular_name}
         super().__init__(fields=fields, **kwargs)
 
 
 class incorrect_arity(TifaFeedback):
     """ Incorrect arity """
     title = "Incorrect Arity"
-    message_template = ("The function {function_name_message} was given the "
-                        "wrong number of arguments.")
+    message_template = ("The {function_type} {function_name_message} was given the "
+                        "wrong number of arguments. You should have had {expected_count} "
+                        "arguments, but instead you had {actual_count} arguments.")
     justification = ""
 
-    def __init__(self, location, function_name, **kwargs):
+    def __init__(self, location, function_name, expected_count, actual_count, is_constructor=False, **kwargs):
         report = kwargs.get("report", MAIN_REPORT)
+        function_type = 'constructor function' if is_constructor else 'function'
         super().__init__(location=location, function_name=function_name,
+                         expected_count=expected_count, actual_count=actual_count,
                          function_name_message=report.format.name(function_name),
+                         function_type=function_type,
                          **kwargs)
 
 
 class module_not_found(TifaFeedback):
     """ Module not found """
     title = "Module Not Found"
     message_template = "TODO"
@@ -451,8 +516,17 @@
 "Aliased built-in": [], #
 "Method not in Type": [], # A method was used that didn't exist for that type
 "Submodule not found": [],
 "Module not found": [],
 "Else on loop body": [], # Used an Else on a For or While
 '''
 
-# TODO: Equality instead of assignment
+
+# TODO: Add in all other names from this module
+FEEDBACK_BY_NAME = {'type_change_append': type_change_append,
+                    'incorrect_arity': incorrect_arity,
+                    'parameter_type_mismatch': parameter_type_mismatch,
+                    'field_type_mismatch': field_type_mismatch}
+
+
+def lookup_feedback(name):
+    return FEEDBACK_BY_NAME.get(name)
```

### Comparing `pedal-2.3.8/pedal/tifa/identifier.py` & `pedal-2.4.0/pedal/tifa/identifier.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/tifa/state.py` & `pedal-2.4.0/pedal/tifa/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Classes and functions for managing the State of a variable.
 """
+from pedal.types.new_types import is_subtype
 
 
 def check_trace(state):
     """
     Create a list of all the types that this given state ever took on.
 
     Args:
         state (:py:class:`pedal.tifa.state.State`): The state to check the trace
             history of.
 
     Returns:
-        list[:py:class:`pedal.types.definitions.Type`]: The list of all types
+        list[:py:class:`pedal.types.new_types.Type`]: The list of all types
             that this State ever took on.
     """
     past_types = [state.type]
     for past_state in state.trace:
         past_types.extend(check_trace(past_state))
     return past_types
 
@@ -85,9 +86,11 @@
         return str(self)
 
     def was_type(self, a_type):
         """
         Retrieve all the types that this variable took on over its entire
         trace.
         """
+        from pedal.types.normalize import normalize_type
+        a_type = normalize_type(a_type).as_type()
         past_types = check_trace(self)
-        return any(past_type.is_equal(a_type) for past_type in past_types)
+        return any(is_subtype(past_type, a_type) for past_type in past_types)
```

### Comparing `pedal-2.3.8/pedal/tifa/tifa_core.py` & `pedal-2.4.0/pedal/tifa/tifa_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,22 @@
 """
 Main TIFA visitor-based algorithm here.
 
 TODO: JoinedStr
 """
 
 import ast
-# TODO: FileType, DayType, TimeType,
-from pedal.core.commands import system_error
 from pedal.core.report import MAIN_REPORT
 from pedal.core.location import Location
-from pedal.types.definitions import (UnknownType,
-                                     FunctionType, ClassType, InstanceType,
-                                     NumType, NoneType, BoolType, TupleType,
-                                     ListType, StrType, GeneratorType,
-                                     DictType, ModuleType, SetType,
-                                     LiteralNum, LiteralBool,
-                                     LiteralNone, LiteralStr,
-                                     LiteralTuple, Type)
-from pedal.types.normalize import (get_pedal_type_from_json,
-                                   get_pedal_literal_from_pedal_type,
-                                   get_pedal_type_from_annotation,
-                                   get_pedal_type_from_value)
-from pedal.types.builtin import (get_builtin_module, get_builtin_function)
-from pedal.types.operations import (are_types_equal,
-                                    VALID_UNARYOP_TYPES, VALID_BINOP_TYPES,
-                                    ORDERABLE_TYPES, INDEXABLE_TYPES)
+from pedal.tifa.contexts import NewScope
+from pedal.types.normalize import (get_pedal_type_from_json)
+from pedal.types.builtin import (get_builtin_module)
+from pedal.types.new_types import (is_subtype, Type, AnyType, ImpossibleType, NoneType,
+                                   ListType, TupleType, ModuleType,
+                                   LiteralStr, LiteralInt, LiteralFloat, LiteralBool)
 from pedal.tifa.constants import TOOL_NAME
 from pedal.tifa.identifier import Identifier
 from pedal.tifa.state import State
 from pedal.tifa.feedbacks import (action_after_return, return_outside_function,
                                   write_out_of_scope, unconnected_blocks,
                                   iteration_problem, not_a_function,
                                   initialization_problem, unused_variable,
@@ -36,15 +24,16 @@
                                   iterating_over_empty_list, incompatible_types,
                                   parameter_type_mismatch, read_out_of_scope,
                                   type_changes, unnecessary_second_branch,
                                   recursive_call, multiple_return_types,
                                   possible_initialization_problem,
                                   incorrect_arity, else_on_loop_body,
                                   module_not_found, nested_function_definition,
-                                  unused_returned_value, invalid_indexing, append_to_non_list)
+                                  unused_returned_value, invalid_indexing, append_to_non_list,
+                                  lookup_feedback)
 
 __all__ = ['TifaCore', 'TifaAnalysis']
 
 
 class TifaAnalysis:
     """
     Container class for the results of running a Tifa Analysis.
@@ -77,16 +66,14 @@
     """
     TIFA Core, with methods for manipulating the TifaAnalysis data.
 
     Args:
         report (Report): The report object to store data and feedback in. If
                          left None, defaults to the global MAIN_REPORT.
     """
-    settings: dict
-
     path_id: int
     scope_id: int
     ast_id: int
 
     path_names: list
     scope_names: list
 
@@ -98,19 +85,23 @@
     # dict[paths, dict[names, State]]
     name_map: dict
     class_scopes: dict
     path_parents: dict
 
     final_node: ast.AST or None
 
+    line_offset: int
+
     def __init__(self, report=MAIN_REPORT):
         self.report = report
-        self.settings = {}
         self.analysis = None
 
+    def get_setting(self, setting_name):
+        return self.report[TOOL_NAME]['settings'][setting_name]
+
     def locate(self, node: ast.AST = None):
         """
         Return a dictionary representing the current location within the
         AST.
 
         Returns:
             Location: The line and column of the current or given node.
@@ -118,15 +109,19 @@
         if node is None:
             if self.node_chain:
                 node = self.node_chain[-1]
             else:
                 node = self.final_node
         return Location(node.lineno+self.line_offset, col=node.col_offset)
 
-    def _issue(self, feedback):
+    def _issue(self, *feedback):
+        if len(feedback) == 1:
+            feedback = feedback[0]
+        else:
+            feedback = lookup_feedback(feedback[0])(*feedback[1:])
         if feedback.label not in self.analysis.issues:
             self.analysis.issues[feedback.label] = []
         self.analysis.issues[feedback.label].append(feedback)
 
     def _collect_top_level_variables(self):
         """
         Walk through the variables and add any at the top level to the
@@ -158,14 +153,15 @@
         self.scope_chain = [self.scope_id]
         self.path_chain = [self.path_id]
         self.name_map = {self.path_id: {}}
         self.definition_chain = []
         self.path_parents = {}
         self.final_node = None
         self.class_scopes = {}
+        self.module_scopes = {}
 
     def find_variable_scope(self, name):
         """
         Walk through this scope and all enclosing scopes, finding the relevant
         identifier given by `name`.
 
         Args:
@@ -230,15 +226,15 @@
         path_id = self.path_chain[0]
         for name in self.name_map[path_id]:
             if self.in_scope(name, self.scope_chain):
                 state = self.name_map[path_id][name]
                 if state.over == 'yes':
                     position = state.over_position
                     self._issue(overwritten_variable(position, state.name))
-                if state.read == 'no':
+                if state.read == 'no' and state.name != '_':
                     self._issue(unused_variable(state.position, state.name, state.type, report=self.report))
 
     def _scope_chain_str(self, name=None):
         """
         Convert the current scope chain to a string representation (divided 
         by "/").
 
@@ -276,17 +272,18 @@
     def iterate_variable(self, name, position=None):
         """
         Update the variable by iterating through it - this doesn't do anything
         fancy yet.
         """
         return self.load_variable(name, position)
 
-    def store_iter_variable(self, name, new_type, position=None):
+    def store_read_variable(self, name, new_type, position=None):
         """
-        Record that the variable was iterated upon. This counts as a Read.
+        Record that the variable was iterated (or otherwise stored in a way that is safe
+        to not read later on) upon. This counts as a Read. Another use case is class variables.
 
         Args:
             name (str): The name of the variable.
             new_type (Type): The Tifa Type of the variable.
             position: The location where this iteration occurred.
 
         Returns:
@@ -346,18 +343,18 @@
         if not variable.exists or force_create:
             # Create a new instance of the variable on the current path
             new_state = State(name, [], store_type, 'store', position,
                               read='no', set='yes', over='no')
             self.name_map[current_path][full_name] = new_state
         else:
             new_state = self.trace_state(variable.state, "store", position)
-            if not variable.in_scope:
+            if not variable.in_scope and not self._in_module():
                 self._issue(write_out_of_scope(self.locate(), name, report=self.report))
             # Type change?
-            if not are_types_equal(store_type, variable.state.type):
+            if not is_subtype(store_type, variable.state.type):
                 self._issue(type_changes(position, name, variable.state.type, store_type))
             new_state.type = store_type
             # Overwritten?
             if variable.state.set == 'yes' and variable.state.read == 'no':
                 new_state.over_position = position
                 new_state.over = 'yes'
             else:
@@ -391,15 +388,15 @@
         if not variable.exists:
             out_of_scope_var = self.find_variable_out_of_scope(name)
             # Create a new instance of the variable on the current path
             if out_of_scope_var.exists:
                 self._issue(read_out_of_scope(self.locate(), name))
             else:
                 self._issue(initialization_problem(self.locate(), name))
-            new_state = State(name, [], UnknownType(), 'load', position,
+            new_state = State(name, [], AnyType(), 'load', position,
                               read='yes', set='no', over='no')
             self.name_map[current_path][full_name] = new_state
         else:
             new_state = self.trace_state(variable.state, "load", position)
             if variable.state.set == 'no':
                 self._issue(initialization_problem(self.locate(), name))
             if variable.state.set == 'maybe':
@@ -419,34 +416,63 @@
         Args:
             chain (str): A chain of module imports (e.g., "matplotlib.pyplot")
         Returns:
             ModuleType: The specific module with its members, or an empty
                         module type.
         """
         module_names = chain.split('.')
-        potential_module = get_builtin_module(module_names[0])
-        if not isinstance(potential_module, UnknownType):
-            base_module = potential_module
-            for module in module_names[1:]:
-                if (isinstance(base_module, ModuleType) and
-                        module in base_module.submodules):
-                    base_module = base_module.submodules[module]
-                else:
-                    self._issue(module_not_found(self.locate(), chain, False, None, report=self.report))
-            return base_module
-        else:
+        for potential_module in [self.report[TOOL_NAME]['types']['modules'].get(module_names[0]),
+                                 get_builtin_module(module_names[0])]:
+            if potential_module is not None:
+                base_module = potential_module
+                for module in module_names[1:]:
+                    if (isinstance(base_module, ModuleType) and
+                            module in base_module.submodules):
+                        base_module = base_module.submodules[module]
+                    else:
+                        # TODO: What if the module is partially overriding a builtin?
+                        self._issue(module_not_found(self.locate(), chain, False, None, report=self.report))
+                return base_module
+
+        # Non-student file, maybe it has _tifa_definitions?
+        error = None
+        try:
+            actual_module = __import__(chain, globals(), {},
+                                       ['_tifa_definitions'])
+            definitions = actual_module._tifa_definitions()
+            return get_pedal_type_from_json(definitions)
+        except Exception as e:
+            error = e
+        filename = chain.replace('.', '/') + ".py"
+        if self.report.submission and filename in self.report.submission.files:
+            # TODO: Try running TIFA over the code
+            code = self.report.submission.files[filename]
             try:
-                actual_module = __import__(chain, globals(), {},
-                                           ['_tifa_definitions'])
-                definitions = actual_module._tifa_definitions()
-                return get_pedal_type_from_json(definitions)
+                # TODO: Doesn't import toplevels as variables.
+                # TODO: Allow variables to be unused inside the file
+                self.report[TOOL_NAME]['types']['modules'][chain] = self._visit_module(chain, filename, code)
+                return self.report[TOOL_NAME]['types']['modules'][chain]
             except Exception as e:
-                #print(e)
-                self._issue(module_not_found(self.locate(), chain, True, e, report=self.report))
-                return ModuleType()
+                error = e
+        self._issue(module_not_found(self.locate(), chain, True, error, report=self.report))
+        return ModuleType(module_names[-1], {}, {})
+
+    def _visit_module(self, module_name, filename, code):
+        ast_tree = ast.parse(code, filename)
+        # TODO: Properly handle submodules
+        new_module = ModuleType(module_name, {}, {})
+        #self.store_variable(class_name, new_class_type)
+        definitions_scope = self.scope_chain[:]
+        class_scope = NewScope(self, definitions_scope, class_type=new_module, is_module=True)
+        with class_scope:
+            self.visit(ast_tree)
+        return new_module
+
+    def _in_module(self):
+        return any(scope_id in self.module_scopes for scope_id in self.scope_chain)
 
     def combine_states(self, left, right):
         """
 
         Args:
             left:
             right:
@@ -458,15 +484,15 @@
                       read=left.read, set=left.set, over=left.over,
                       over_position=left.over_position)
         if right is None:
             state.read = 'no' if left.read == 'no' else 'maybe'
             state.set = 'no' if left.set == 'no' else 'maybe'
             state.over = 'no' if left.over == 'no' else 'maybe'
         else:
-            if not are_types_equal(left.type, right.type):
+            if not is_subtype(left.type, right.type):
                 self._issue(type_changes(self.locate(), left.name, left.type, right.type))
             state.read = self.match_rso(left.read, right.read)
             state.set = self.match_rso(left.set, right.set)
             state.over = self.match_rso(left.over, right.over)
             if left.over == 'no':
                 state.over_position = right.over_position
             state.trace.append(right)
@@ -488,26 +514,38 @@
             left_state = self.name_map[left_path_id][left_name]
             right_identifier = self.find_path_parent(right_path_id, left_name)
             if right_identifier.exists:
                 # Was on both IF and ELSE path
                 right_state = right_identifier.state
             else:
                 # Was only on IF path, potentially on the parent path
-                right_state = self.name_map[parent_path_id].get(left_name)
+                right_state = self.search_parents(parent_path_id, left_name)
+                # right_state = self.name_map[parent_path_id].get(left_name)
             combined = self.combine_states(left_state, right_state)
             self.name_map[parent_path_id][left_name] = combined
         # Check for names that are on the ELSE path but not the IF path
         for right_name in self.name_map[right_path_id]:
             if right_name not in self.name_map[left_path_id]:
                 right_state = self.name_map[right_path_id][right_name]
                 # Potentially on the parent path
-                parent_state = self.name_map[parent_path_id].get(right_name)
+                #parent_state = self.name_map[parent_path_id].get(right_name)
+                parent_state = self.search_parents(parent_path_id, right_name)
                 combined = self.combine_states(right_state, parent_state)
                 self.name_map[parent_path_id][right_name] = combined
 
+    def search_parents(self, parent_id, seeking_name):
+        possible = self.name_map[parent_id]
+        if seeking_name in possible:
+            return possible[seeking_name]
+        elif parent_id in self.path_parents:
+            parent_id = self.path_parents[parent_id]
+            return self.search_parents(parent_id, seeking_name)
+        else:
+            return None
+
     @staticmethod
     def trace_state(state, method, position):
         """
         Makes a copy of the given state with the given method type.
 
         Args:
             state (State): The state to copy (as in, we trace a copy of it!)
@@ -558,29 +596,29 @@
         Args:
             node:
 
         Returns:
 
         """
         if isinstance(node, ast.Num):
-            return LiteralNum(node.n)
+            return LiteralInt(node.n) if isinstance(node.n, int) else LiteralFloat(node.n)
         elif isinstance(node, ast.Str):
             return LiteralStr(node.s)
         elif isinstance(node, ast.Tuple):
             values = []
             for elt in node.elts:
                 subvalue = self.get_literal(elt)
                 if subvalue is not None:
                     values.append(subvalue)
                 else:
                     return None
-            return LiteralTuple(values)
+            return TupleType(values)
         elif isinstance(node, ast.Name):
             if node.id == "None":
-                return LiteralNone(None)
+                return NoneType()
             elif node.id == "False":
                 return LiteralBool(False)
             elif node.id == "True":
                 return LiteralBool(True)
         return None
 
     def check_common_bad_lookups(self, left_type, attr, node):
```

### Comparing `pedal-2.3.8/pedal/tifa/tifa_visitor.py` & `pedal-2.4.0/pedal/tifa/tifa_visitor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,45 @@
 
-
-
 """
 Main TIFA visitor-based algorithm here.
 
 TODO: JoinedStr
 """
 
 import ast
 # TODO: FileType, DayType, TimeType,
 from pedal.core.commands import system_error
 from pedal.tifa.tifa_core import TifaCore, TifaAnalysis
-from pedal.types.definitions import (UnknownType,
-                                     FunctionType, ClassType, InstanceType,
-                                     NumType, NoneType, BoolType, TupleType,
-                                     ListType, StrType, GeneratorType,
-                                     DictType, ModuleType, SetType,
-                                     LiteralNum, LiteralBool,
-                                     LiteralNone, LiteralStr,
-                                     LiteralTuple, Type)
-from pedal.types.normalize import (get_pedal_type_from_json,
-                                   get_pedal_literal_from_pedal_type,
-                                   get_pedal_type_from_annotation,
-                                   get_pedal_type_from_value)
-from pedal.types.builtin import (get_builtin_module, get_builtin_function)
-from pedal.types.operations import (are_types_equal,
-                                    VALID_UNARYOP_TYPES, VALID_BINOP_TYPES,
-                                    ORDERABLE_TYPES, INDEXABLE_TYPES)
+from pedal.types.new_types import (Type, AnyType, ImpossibleType, FunctionType, GeneratorType,
+                                   IntType, FloatType, BoolType, TupleType,
+                                   ListType, StrType, SetType, DictType,
+                                   ClassType, InstanceType, BuiltinConstructorType, NumType, NoneType,
+                                   LiteralValue, LiteralInt, LiteralFloat, LiteralStr, LiteralBool,
+                                   TypeUnion, widen_type, widest_type)
+from pedal.types.new_types import is_subtype, specify_subtype
+from pedal.types.normalize import get_pedal_type_from_value
+from pedal.types.builtin import get_builtin_name
+from pedal.types.operations import (VALID_UNARYOP_TYPES, apply_binary_operation, apply_unary_operation)
 from pedal.tifa.constants import TOOL_NAME
 from pedal.tifa.contexts import NewPath, NewScope
-from pedal.tifa.identifier import Identifier
-from pedal.tifa.state import State
 from pedal.tifa.feedbacks import (action_after_return, return_outside_function,
                                   write_out_of_scope, unconnected_blocks,
                                   iteration_problem, not_a_function,
                                   initialization_problem, unused_variable,
                                   overwritten_variable, iterating_over_non_list,
                                   iterating_over_empty_list, incompatible_types,
                                   parameter_type_mismatch, read_out_of_scope,
                                   type_changes, unnecessary_second_branch,
                                   recursive_call, multiple_return_types,
                                   possible_initialization_problem,
                                   incorrect_arity, else_on_loop_body,
                                   module_not_found, nested_function_definition,
-                                  unused_returned_value, invalid_indexing)
-from pedal.utilities.system import IS_PYTHON_39
+                                  unused_returned_value, invalid_indexing,
+                                  attribute_type_change)
+from pedal.utilities.system import IS_PYTHON_39, IS_AT_LEAST_PYTHON_38
 
 
 class Tifa(TifaCore, ast.NodeVisitor):
     """
     TIFA subclass for traversing an AST and finding common issues.
     You can instantiate this class, manipulate settings, and then process
     some code or AST.
@@ -65,16 +56,16 @@
             reset (bool): Whether or not to reset the results from the
                 previous analysis before running this one.
         Returns:
             Report: The successful or successful report object
         """
         if reset or self.analysis is None:
             self.analysis = TifaAnalysis()
-        filename = filename or self.report.submission.main_file
-        self.line_offset = self.report.submission.line_offsets.get(filename, 0)
+        filename = filename or (self.report.submission.main_file if self.report.submission else 'student.py')
+        self.line_offset = self.report.submission.line_offsets.get(filename, 0) if self.report.submission else 0
 
         # Attempt parsing - might fail!
         try:
             ast_tree = ast.parse(code, filename)
         except Exception as error:
             self.analysis.fail(error)
             system_error(TOOL_NAME, "Could not parse code: " + str(error),
@@ -134,15 +125,15 @@
                                                     report=self.report))
 
         # No? All good, let's enter the node
         self.final_node = node
         result = ast.NodeVisitor.visit(self, node)
         # If a node failed to return something, return the UNKNOWN TYPE
         if result is None:
-            result = UnknownType()
+            result = AnyType()
         self.analysis.node_types[node] = result
 
         # Pop the node out of the chain
         self.ast_id -= 1
         self.node_chain.pop()
 
         return result
@@ -155,269 +146,239 @@
             nodes (list): A list of values, of which any AST nodes will be
                           visited.
         """
         for node in nodes:
             if isinstance(node, ast.AST):
                 self.visit(node)
 
-    @staticmethod
-    def walk_targets(targets, target_type, walker):
-        """
-        Iterate through the targets and call the given function on each one.
-
-        Args:
-            targets (list of Ast nodes): A list of potential targets to be
-                                         traversed.
-            target_type (Type): The given type to be unraveled and applied to the
-                         targets.
-            walker (Ast Node, Type -> None): A function that will process
-                                             each target and unravel the type.
-        """
-        for target in targets:
-            walker(target, target_type)
-
-    def _walk_target(self, target, target_type):
-        """
-        Recursively apply the type to the target
-
-        Args:
-            target (Ast): The current AST node to process
-            target_type (Type): The type to apply to this node
-        """
-        if isinstance(target, ast.Name):
-            self.store_iter_variable(target.id, target_type, self.locate(target))
-            return target.id
-        elif isinstance(target, (ast.Tuple, ast.List)):
-            result = None
-            for i, elt in enumerate(target.elts):
-                elt_type = target_type.iterate(LiteralNum(i))
-                potential_name = self._walk_target(elt, elt_type)
-                if potential_name is not None and result is None:
-                    result = potential_name
-            return result
-
-    # TODO: Properly handle assignments with subscripts
-    def assign_target(self, target, target_type):
-        """
-        Assign the type to the target, handling all kinds of assignment
-        statements, including Names, Tuples/Lists, Subscripts, and
-        Attributes.
-
-        Args:
-            target (ast.AST): The target AST Node.
-            target_type (Type): The TIFA type.
-
-        Returns:
-
-        """
-        if isinstance(target, ast.Name):
-            self.store_variable(target.id, target_type)
-        elif isinstance(target, (ast.Tuple, ast.List)):
-            for i, elt in enumerate(target.elts):
-                elt_type = target_type.iterate(LiteralNum(i))
-                self.assign_target(elt, elt_type)
-        elif isinstance(target, ast.Subscript):
-            left_hand_type = self.visit(target.value)
-            if isinstance(left_hand_type, ListType):
-                # TODO: Handle updating value in list
-                pass
-            elif isinstance(left_hand_type, DictType):
-                # TODO: Update this for Python 3.9, now that Slice notation has changed
-                if not isinstance(target.slice, ast.Index):
-                    # TODO: Can't subscript a dictionary assignment
-                    return None
-                literal = self.get_literal(target.slice.value)
-                if not literal:
-                    key_type = self.visit(target.slice.value)
-                    left_hand_type.empty = False
-                    left_hand_type.keys = [key_type.clone()]
-                    left_hand_type.values = [target_type.clone()]
-                elif left_hand_type.literals:
-                    original_type = left_hand_type.has_literal(literal)
-                    if not original_type:
-                        left_hand_type.update_key(literal, target_type.clone())
-                    elif not are_types_equal(original_type, target_type):
-                        # TODO: Fix "Dictionary" to be the name of the variable
-                        self._issue(type_changes(self.locate(), 'Dictionary', original_type, target_type))
-        elif isinstance(target, ast.Attribute):
-            left_hand_type = self.visit(target.value)
-            if isinstance(left_hand_type, InstanceType):
-                left_hand_type.add_attr(target.attr, target_type)
-            # TODO: Otherwise we attempted to assign to a non-instance
-            # TODO: Handle minor type changes (e.g., appending to an inner list)
-
     def _visit_collection_loop(self, node):
         was_empty = False
         # Handle the iteration list
         iter_list = node.iter
         iter_list_name = None
         if isinstance(iter_list, ast.Name):
             iter_list_name = iter_list.id
             if iter_list_name == "___":
                 self._issue(unconnected_blocks(self.locate(iter_list), report=self.report))
             state = self.iterate_variable(iter_list_name, self.locate(iter_list))
             iter_type = state.type
         else:
             iter_type = self.visit(iter_list)
 
-        if iter_type.is_empty():
+        if iter_type.is_empty:
             # TODO: It should check if its ONLY ever iterating over an empty list.
             # For now, only reports if we are NOT in a function
             was_empty = True
             if len(self.scope_chain) == 1:
                 self._issue(iterating_over_empty_list(self.locate(iter_list), iter_list_name))
 
-        if not isinstance(iter_type, INDEXABLE_TYPES):
+        iter_subtype = iter_type.iterate()
+        if isinstance(iter_subtype, ImpossibleType):
             self._issue(iterating_over_non_list(self.locate(iter_list), iter_list_name, report=self.report))
 
-        iter_subtype = iter_type.iterate(LiteralNum(0))
 
         # Handle the iteration variable
-        iter_variable_name = self._walk_target(node.target, iter_subtype)
+        self.assign_target(node.target, iter_subtype, store_with_read=True)
 
         # Check that the iteration list and variable are distinct
-        if iter_variable_name and iter_list_name:
-            if iter_variable_name == iter_list_name:
-                self._issue(iteration_problem(self.locate(node.target), iter_variable_name))
+        if isinstance(node.target, ast.Name) and node.target.id == iter_list_name:
+            self._issue(iteration_problem(self.locate(node.target), node.target.id))
 
         return was_empty
 
+    def break_starred(self, elements):
+        leading, starred, trailing = [], [], []
+        all_elements = iter(elements)
+        for elt in all_elements:
+            if isinstance(elt, ast.Starred):
+                starred.append(elt)
+                break
+            else:
+                leading.append(elt)
+        else:
+            return leading, starred, trailing
+        for elt in all_elements:
+            trailing.append(elt)
+        return leading, starred, trailing
+
+    # TODO: Properly handle assignments with subscripts
+    def assign_target(self, target, target_type, operation=None, store_with_read=False):
+        """
+        Assign the type to the target, handling all kinds of assignment
+        statements, including Names, Tuples/Lists, Subscripts, and
+        Attributes.
+
+        Args:
+            target (ast.AST): The target AST Node.
+            target_type (Type): The new TIFA type.
+            operation (None | ast.op): The AugAssign operation, if there is one
+
+        Returns:
+
+        """
+        if isinstance(target, ast.Name):
+            original_value_type = self.visit(target)
+            if operation:
+                new_target_type = apply_binary_operation(operation, original_value_type, target_type)
+                if isinstance(new_target_type, ImpossibleType):
+                    self._issue(incompatible_types(self.locate(), operation, original_value_type, target_type, report=self.report))
+            else:
+                new_target_type = target_type
+            if store_with_read:
+                self.store_read_variable(target.id, new_target_type)
+            else:
+                self.store_variable(target.id, new_target_type)
+        elif isinstance(target, (ast.Tuple, ast.List)):
+            original_type = self.visit(target)
+            leading, starred, trailing = self.break_starred(target.elts)
+            tt, ot = target_type.break_apart(), original_type.break_apart()
+            for elt, elt_type, old_type in zip(leading, tt, ot):
+                self.assign_target(elt, elt_type)
+            if starred:
+                # TODO: Handle starred node's type changes
+                # if not is_subtype(target_type, old_type):
+                    # self._issue(type_changes(self.locate(), 'an element of NODE', old_type.singular_name, elt_type.singular_name))
+                self.assign_target(starred[0], target_type)
+                for elt, elt_type, old_type in zip(trailing, tt, ot):
+                    # BUG: Any trailing elements will be incorrectly offset, so won't work with finite length stuff
+                    self.assign_target(elt, elt_type)
+        elif isinstance(target, ast.Subscript):
+            original_value_type = self.visit(target.value)
+            origin = self.identify_caller(target.value)
+            original_indexing_type = self.visit(target.slice)
+            original_type = original_value_type.index(original_indexing_type)
+            if operation:
+                new_target_type = apply_binary_operation(operation, original_type, target_type)
+                if isinstance(new_target_type, ImpossibleType):
+                    self._issue(incompatible_types(self.locate(), operation, original_type, target_type, report=self.report))
+            else:
+                new_target_type = target_type
+            original_type.set_index(original_indexing_type, new_target_type)
+            if origin:
+                origin_type = self.load_variable(origin)
+                self.store_variable(origin, origin_type.type)
+        elif isinstance(target, ast.Attribute):
+            original_type = self.visit(target.value)
+            origin = self.identify_caller(target.value)
+            if operation:
+                new_target_type = apply_binary_operation(operation, original_type, target_type)
+                if isinstance(new_target_type, ImpossibleType):
+                    self._issue(incompatible_types(self.locate(), operation, original_type, target_type, report=self.report))
+            else:
+                new_target_type = target_type
+            assigned_type = original_type.add_attr(target.attr, new_target_type)
+            if isinstance(assigned_type, ImpossibleType):
+                self._issue(attribute_type_change(self.locate(), target.attr, original_type, new_target_type, report=self.report))
+            if origin:
+                origin_type = self.load_variable(origin)
+                if origin_type:
+                    self.store_variable(origin, origin_type.type)
+
     def visit_AnnAssign(self, node):
         """
-        TODO: Implement!
+
+        Args:
+            node (ast.AnnAssign):
+
+        Returns:
+
         """
         # Name, Attribute, or SubScript
         target = node.target
         # Type
         annotation = node.annotation
+        annotation_type = self.evaluate_type(annotation)
+        was_class_attribute = False
         # Optional assigned value
         value = node.value
         # 0 or 1, with 1 indicating pure names (not expressions)
         simple = node.simple
+
         # If it's a class attribute, then build up the type!
         if simple:
-            self.visit(annotation)
-            annotation = get_pedal_type_from_annotation(annotation, self)
             current_scope = self.scope_chain[0]
             if current_scope in self.class_scopes:
-                # TODO: Treat it as a different kind of ClassType? TypedDict?
                 self.class_scopes[current_scope].add_attr(target.id, annotation)
-
-    def visit_Expr(self, node):
-        """
-        Any expression being used as a statement.
-
-        Args:
-            node (AST): An Expr node
-
-        Returns:
-
-        """
-        value = self.visit(node.value)
-        if isinstance(node.value, ast.Call) and not isinstance(value, NoneType):
-            # TODO: Helper function to get name with title ("append method")
-            if isinstance(node.value.func, ast.Name):
-                call_type = 'function'
-            else:
-                call_type = 'method'
-            name = self.identify_caller(node.value)
-            self._issue(unused_returned_value(self.locate(), name,
-                                              call_type, value))
+                was_class_attribute = True
+        # TODO: Allow setting for optional type coercion, or throw error
+        if value:
+            self.visit(value)
+            # self.assign_target(target, self.visit(value))
+        # Make local variable either way
+        self.assign_target(target, annotation_type, store_with_read=was_class_attribute)
 
     def visit_Assign(self, node):
         """
         Simple assignment statement:
         __targets__ = __value__
 
         Args:
-            node (AST): An Assign node
+            node (ast.Assign): An Assign node
         Returns:
             None
         """
         # Handle value
         value_type = self.visit(node.value)
-        # Handle targets
-        self._visit_nodes(node.targets)
-
-        self.walk_targets(node.targets, value_type, self.assign_target)
+        # Apply value to all targets
+        for target in node.targets:
+            self.assign_target(target, value_type)
 
     def visit_AugAssign(self, node):
         """
 
         Args:
-            node:
+            node (ast.AugAssign):
 
         Returns:
 
         """
         # Handle value
         right = self.visit(node.value)
-        # Handle target
-        left = self.visit(node.target)
-        # Target is always a Name, Subscript, or Attribute
-        name = self.identify_caller(node.target)
-
-        # Handle operation
-        self.load_variable(name)
-        if isinstance(left, UnknownType) or isinstance(right, UnknownType):
-            return UnknownType()
-        elif type(node.op) in VALID_BINOP_TYPES:
-            op_lookup = VALID_BINOP_TYPES[type(node.op)]
-            if type(left) in op_lookup:
-                op_lookup = op_lookup[type(left)]
-                if type(right) in op_lookup:
-                    op_lookup = op_lookup[type(right)]
-                    result_type = op_lookup(left, right)
-                    self.assign_target(node.target, result_type)
-                    return result_type
-        self._issue(incompatible_types(self.locate(), node.op, left, right, report=self.report))
+        if isinstance(node.target, ast.Name):
+            self.load_variable(self.identify_caller(node.target))
+        self.assign_target(node.target, right, node.op)
 
     def visit_Attribute(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
         # Handle value
         value_type = self.visit(node.value)
         self.check_common_bad_lookups(value_type, node.attr, node.value)
-        # Handle ctx
-        # TODO: Handling contexts
         # Handle attr
-        result = value_type.load_attr(node.attr)
+        result = value_type.get_attr(node.attr)
+        # Set up self if this was a function (because now it's a method!)
+        # TODO: Handle static/class functions differently I guess?
+        if isinstance(result, FunctionType):
+            result = result.as_method(value_type)
         return result
 
     def visit_BinOp(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
         # Handle left and right
         left = self.visit(node.left)
         right = self.visit(node.right)
+        operation = node.op
 
-        # Handle operation
-        if isinstance(left, UnknownType) or isinstance(right, UnknownType):
-            return UnknownType()
-        elif type(node.op) in VALID_BINOP_TYPES:
-            op_lookup = VALID_BINOP_TYPES[type(node.op)]
-            if type(left) in op_lookup:
-                op_lookup = op_lookup[type(left)]
-                if type(right) in op_lookup:
-                    op_lookup = op_lookup[type(right)]
-                    return op_lookup(left, right)
-        self._issue(incompatible_types(self.locate(), node.op, left, right, report=self.report))
-        return UnknownType()
+        new_target_type = apply_binary_operation(operation, left, right)
+        if isinstance(new_target_type, ImpossibleType):
+            self._issue(incompatible_types(self.locate(), operation, left, right, report=self.report))
+        return new_target_type
 
     def visit_Bool(self, node):
         """
         Visit a constant boolean value.
 
         Args:
             node (ast.AST): The boolean value Node.
@@ -433,89 +394,115 @@
         Args:
             node:
 
         Returns:
 
         """
         # Handle left and right
-        values = []
-        for value in node.values:
-            values.append(self.visit(value))
-
-        # TODO: Truthiness is not supported! Probably need a Union type
-        # TODO: Literals used as truthy value
-
+        values = [self.visit(value) for value in node.values]
         # Handle operation
-        return BoolType()
-
-    def visit_Call(self, node):
-        """
-
-        Args:
-            node:
+        # Actually, the operations are always the same behavior!
+        # Handle truthiness
+        if self.get_setting('truthiness_returns_booleans'):
+            return BoolType()
+        elif not values:
+            return ImpossibleType()
+        # All same type? Then return the first one!
+        elif all(is_subtype(values[0], other) for other in values[1:]):
+            return values[0]
+        # Oh no, type union is necessary!
+        else:
+            return TypeUnion(values)
 
-        Returns:
+    def load_root_variable(self, node, position=None):
+        root_name = self.identify_caller(node)
+        if root_name is not None:
+            variable = self.find_variable_scope(root_name)
+            if variable.exists:
+                return variable.state
+        return None
 
-        """
-        # Handle func part (Name or Attribute)
+    def visit_Call(self, node):
+        # Handle func part
         function_type = self.visit(node.func)
         # TODO: Need to grab the actual type in some situations
-        callee = self.identify_caller(node)
+        original_callee = self.load_root_variable(node)
 
         # Handle args
         arguments = [self.visit(arg) for arg in node.args] if node.args else []
+        keywords = [(kwarg.arg, self.visit(kwarg.value))
+                    for kwarg in node.keywords] if node.keywords else {}
 
         # Check special common mistakes
 
-        # TODO: Handle keywords
-        # TODO: Handle star args
-        # TODO: Handle kwargs
+        if isinstance(function_type, BuiltinConstructorType):
+            constructor = function_type.definition
+            return constructor(self, function_type, original_callee,
+                               arguments, keywords, self.locate())
         if isinstance(function_type, FunctionType):
             # Test if we have called this definition before
             if function_type.definition not in self.definition_chain:
                 self.definition_chain.append(function_type.definition)
                 # Function invocation
-                result = function_type.definition(self, function_type, callee,
-                                                  arguments, self.locate())
+                result = function_type.definition(self, function_type, original_callee,
+                                                  arguments, keywords, self.locate())
                 self.definition_chain.pop()
                 return result
             else:
-                self._issue(recursive_call(self.locate(), callee, report=self.report))
+                self._issue(recursive_call(self.locate(), original_callee, report=self.report))
         elif isinstance(function_type, ClassType):
             constructor = function_type.get_constructor().definition
             self.definition_chain.append(constructor)
-            result = constructor(self, constructor, callee, arguments, self.locate())
+            new_instance = constructor(self, constructor, original_callee, arguments, keywords, self.locate())
             self.definition_chain.pop()
             if '__init__' in function_type.fields:
-                initializer = function_type.fields['__init__']
+                initializer = function_type.fields['__init__'].as_method(new_instance)
                 if isinstance(initializer, FunctionType):
                     self.definition_chain.append(initializer)
-                    initializer.definition(self, initializer, result, [result] + arguments, self.locate())
+                    initializer.definition(self, initializer, new_instance, [new_instance] + arguments, keywords, self.locate())
                     self.definition_chain.pop()
-            return result
-        elif isinstance(function_type, (NumType, StrType, BoolType, NoneType)):
-            self._issue(not_a_function(self.locate(), callee, function_type, report=self.report))
-        return UnknownType()
+            return new_instance
+        elif isinstance(function_type, (IntType, FloatType, NumType, ListType,
+                                        DictType, SetType, TupleType, InstanceType,
+                                        StrType, BoolType, NoneType, LiteralValue)):
+            if original_callee is None:
+                self._issue(not_a_function(self.locate(), "a value", function_type, report=self.report))
+            else:
+                self._issue(not_a_function(self.locate(), original_callee.name, function_type, report=self.report))
+            return ImpossibleType()
+        return AnyType()
 
     def visit_ClassDef(self, node):
         """
 
         Args:
             node:
         """
         class_name = node.name
-        new_class_type = ClassType(class_name)
+        parents = [self.visit(base) for base in node.bases]
+        new_class_type = ClassType(class_name, {}, parents)
         self.store_variable(class_name, new_class_type)
-        # TODO: Define a new scope definition that executes the body
-        # TODO: find __init__, execute that
-        # TODO: handle Record subclasses
         definitions_scope = self.scope_chain[:]
         class_scope = NewScope(self, definitions_scope, class_type=new_class_type)
+        # TODO: Handle metaclass... somehow?
+        #self._visit_nodes(node.keywords)
         with class_scope:
-            self.generic_visit(node)
+            self._visit_nodes(node.body)
+        new_class_type = self.apply_decorators(class_name, new_class_type, node.decorator_list)
+        return new_class_type
+
+    def apply_decorators(self, new_name, new_type, decorators):
+        for decorator in reversed(decorators):
+            old_type = self.load_variable(new_name)
+            decorator_type = self.visit(decorator)
+            original_callee = self.load_root_variable(decorator)
+            new_type = decorator_type.definition(self, decorator_type, original_callee,
+                                                 [new_type], {}, self.locate())
+            self.store_variable(new_name, new_type)
+        return new_type
 
     def visit_Compare(self, node):
         """
 
         Args:
             node:
 
@@ -527,199 +514,266 @@
         comparators = [self.visit(compare) for compare in node.comparators]
 
         # Handle ops
         for op, right in zip(node.ops, comparators):
             if isinstance(op, (ast.Eq, ast.NotEq, ast.Is, ast.IsNot)):
                 continue
             elif isinstance(op, (ast.Lt, ast.LtE, ast.GtE, ast.Gt)):
-                if are_types_equal(left, right):
-                    if isinstance(left, ORDERABLE_TYPES):
-                        continue
+                if type(right) in left.orderable:
+                    continue
             elif isinstance(op, (ast.In, ast.NotIn)):
-                if isinstance(right, INDEXABLE_TYPES):
+                if right.allows_membership(left):
                     continue
             self._issue(incompatible_types(self.locate(), op, left, right, report=self.report))
         return BoolType()
 
     def visit_comprehension(self, node):
         """
 
         Args:
             node:
         """
+        self.fill_in_location(node, self.node_chain[-2])
         self._visit_collection_loop(node)
         # Handle ifs, unless they're blank (None in Skulpt :)
         if node.ifs:
             self.visit_statements(node.ifs)
 
+    def fill_in_location(self, node, source_node):
+        node.lineno = source_node.lineno
+        node.end_lineno = source_node.end_lineno
+        node.col_offset = source_node.col_offset
+        node.end_col_offset = source_node.end_col_offset
+
     def visit_Dict(self, node):
         """
         Three types of dictionaries
         - empty
         - uniform type
         - record
         TODO: Handle records appropriately
         """
-        result_type = DictType()
-        if not node.keys:
-            result_type.empty = True
+        items = [(self.visit(key), self.visit(value))
+                 for key, value in zip(node.keys, node.values) if key is not None]
+        # Unpack starred dictionaries
+        for key, value in zip(node.keys, node.values):
+            if key is None:
+                value_type = self.visit(value)
+                if isinstance(value_type, DictType):
+                    items.extend([
+                        (k, v) for k, v in value_type.element_types
+                    ])
+        # Empty dictionary
+        if not items:
+            return DictType([])
+        # All literal keys
+        if all(isinstance(k, LiteralValue) for k, _ in items):
+            return DictType([(k, v) for k, v in items])
+        # Find if all matched type
+        first_key = widest_type([key for key, value in items])
+        first_value = widest_type([value for key, value in items])
+        if first_key is not None and first_value is not None:
+            return DictType([(first_key, first_value)])
         else:
-            result_type.empty = False
-            all_literals = True
-            keys, values, literals = [], [], []
-            for key, value in zip(node.keys, node.values):
-                literal = self.get_literal(key)
-                key, value = self.visit(key), self.visit(value)
-                values.append(value)
-                keys.append(key)
-                if literal is not None:
-                    literals.append(literal)
-                else:
-                    all_literals = False
-
-            if all_literals:
-                result_type.literals = literals
-                result_type.values = values
-            else:
-                result_type.keys = node.keys[0]
-                result_type.values = node.values[0]
-        return result_type
+            # Resort to just matching the types?
+            return DictType([(k, v) for k, v in items])
 
     def visit_DictComp(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
-        # TODO: Handle comprehension scope
-        for generator in node.generators:
-            self.visit(generator)
-        keys = self.visit(node.key)
-        values = self.visit(node.value)
-        return DictType(keys=keys, values=values)
+        generator_scope = NewScope(self, self.scope_chain[:])
+        with generator_scope:
+            self._visit_nodes(node.generators)
+            keys = self.visit(node.key)
+            values = self.visit(node.value)
+            return DictType([(keys, values)])
+
+    def visit_Expr(self, node):
+        """
+        Any expression being used as a statement.
+
+        Args:
+            node (AST): An Expr node
+
+        Returns:
+
+        """
+        value = self.visit(node.value)
+        if isinstance(node.value, ast.Call) and not isinstance(value, NoneType):
+            # TODO: Helper function to get name with title ("append method")
+            if isinstance(node.value.func, ast.Name):
+                call_type = 'function'
+            else:
+                call_type = 'method'
+            name = self.identify_caller(node.value)
+            self._issue(unused_returned_value(self.locate(), name,
+                                              call_type, value))
 
     def visit_For(self, node):
         """
 
         Args:
             node:
         """
         was_empty = self._visit_collection_loop(node)
         # Handle the bodies
-        #if not was_empty:
-        #this_path_id = self.path_chain[0]
-        #non_empty_path = NewPath(self, this_path_id, "f")
-        #with non_empty_path:
+        # if not was_empty:
+        # this_path_id = self.path_chain[0]
+        # non_empty_path = NewPath(self, this_path_id, "f")
+        # with non_empty_path:
         self.visit_statements(node.body)
         self.visit_statements(node.orelse)
 
     def visit_FunctionDef(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
-        # Name
         function_name = node.name
         position = self.locate()
         definitions_scope = self.scope_chain[:]
+        definition = self.make_function(function_name, definitions_scope, position, node)
+        function = FunctionType(function_name, definition=definition)
+        self.store_variable(function_name, function)
+
+        if len(self.node_chain) > 2:
+            self._issue(nested_function_definition(self.locate(), function_name))
 
-        def definition(tifa, call_type, call_name, parameters, call_position):
-            """
+        return self.apply_decorators(function_name, function, node.decorator_list)
 
-            Args:
-                tifa:
-                call_type:
-                call_name:
-                parameters:
-                call_position:
+    def make_function(self, function_name, definitions_scope, position, node):
+        is_lambda = function_name is None
 
-            Returns:
+        class SkipType:
+            pass
+        # Pull apart args into a coherent set of data PRIOR to execution
+        args = node.args
+        pos_parameters = args.posonlyargs + args.args if IS_AT_LEAST_PYTHON_38 else args.args
+        none_padding = [SkipType] * (len(pos_parameters) - len(args.defaults))
+        pos_defaults = none_padding + [self.visit(d) for d in args.defaults]
+        kwarg_parameter = args.kwarg
+        vararg_parameter = args.vararg
+
+        # TODO: Finish kwargs
+        named_parameters = args.kwonlyargs
+        named_defaults = [self.visit(d) if d is not None else AnyType() for d in args.kw_defaults]
+        expected_returns = self.evaluate_type(node.returns) if not is_lambda and node.returns else None
 
-            """
+        def definition(tifa, function, callee_name, arguments, named_arguments, call_position):
             function_scope = NewScope(self, definitions_scope)
             with function_scope:
                 # Process arguments
-                args = node.args.args
-                if len(args) != len(parameters):
-                    self._issue(incorrect_arity(self.locate(), function_name, report=self.report))
-                # TODO: Handle special types of parameters
-                for arg, parameter in zip(args, parameters):
-                    name = arg.arg
-                    if arg.annotation:
-                        self.visit(arg.annotation)
-                        annotation = get_pedal_type_from_annotation(arg.annotation, self)
-                        # TODO: Use parameter information to "fill in" empty lists
-                        if isinstance(parameter, ListType) and isinstance(annotation, ListType):
-                            if isinstance(parameter.subtype, UnknownType):
-                                parameter.subtype = annotation.subtype
-                        # TODO: Check that arg.type and parameter type match!
-                        if not are_types_equal(annotation, parameter, True):
-                            self._issue(parameter_type_mismatch(self.locate(), name, annotation, parameter))
-                    if parameter is not None:
-                        parameter = parameter.clone_mutably()
-                        self.create_variable(name, parameter, position)
+                if len(arguments) + len(named_arguments) != len(pos_parameters) and not vararg_parameter:
+                    self._issue(incorrect_arity(self.locate(), function_name,
+                                                len(pos_parameters), len(arguments), report=self.report))
+                for parameter, default, argument in zip(pos_parameters, pos_defaults, arguments):
+                    parameter_name = parameter.arg
+                    if parameter.annotation:
+                        annotation = self.evaluate_type(parameter.annotation)
+                        if is_subtype(argument, annotation):
+                            specify_subtype(annotation, argument)
+                        else:
+                            self._issue(parameter_type_mismatch(self.locate(), parameter_name,
+                                                                annotation, argument))
+                    elif default is not SkipType:
+                        if is_subtype(argument, default):
+                            specify_subtype(default, argument)
+                        else:
+                            self._issue(parameter_type_mismatch(self.locate(), parameter_name,
+                                                                default, argument))
+                    if argument is not None:
+                        argument_type = argument.clone_mutably()
+                        self.create_variable(parameter_name, argument_type, position)
                 # Too many arguments
-                if len(args) < len(parameters):
-                    for undefined_parameter in parameters[len(args):]:
-                        self.create_variable(name, UnknownType(), position)
+                if len(pos_parameters) < len(arguments):
+                    if vararg_parameter:
+                        the_rest = arguments[len(pos_parameters):]
+                        self.create_variable(vararg_parameter.arg, TupleType(the_rest), position)
                 # Not enough arguments
-                if len(args) > len(parameters):
-                    for arg in args[len(parameters):]:
-                        if arg.annotation:
-                            self.visit(arg.annotation)
-                            annotation = get_pedal_type_from_annotation(arg.annotation, self)
+                if len(pos_parameters) > len(arguments):
+                    for parameter in pos_parameters[len(arguments):]:
+                        if parameter.annotation:
+                            annotation = self.evaluate_type(parameter.annotation)
                         else:
-                            annotation = UnknownType()
-                        self.create_variable(arg.arg, annotation, position)
+                            annotation = AnyType()
+                        self.create_variable(parameter.arg, annotation, position)
+                if is_lambda:
+                    return self.visit(node.body)
+
                 self.visit_statements(node.body)
                 return_state = self.find_variable_scope("*return")
                 return_value = NoneType()
                 # TODO: Figure out if we are not returning something when we should
                 # If the pseudo variable exists, we load it and get its type
                 if return_state.exists and return_state.in_scope:
                     return_state = self.load_variable("*return", call_position)
                     return_value = return_state.type
-                    if node.returns:
-                        # self.visit(node.returns)
-                        returns = get_pedal_type_from_annotation(node.returns, self)
-                        if not are_types_equal(return_value, returns, True):
+                    if expected_returns:
+                        if not is_subtype(return_value, expected_returns):
                             self._issue(multiple_return_types(return_state.position,
-                                                              returns.precise_description(),
-                                                              return_value.precise_description(),
+                                                              expected_returns.singular_name,
+                                                              return_value.singular_name,
                                                               report=self.report))
             return return_value
+        return definition
 
-        function = FunctionType(definition=definition, name=function_name)
-        self.store_variable(function_name, function)
-
-        if len(self.node_chain) > 2:
-            self._issue(nested_function_definition(self.locate(), function_name))
-
-        return function
+    def evaluate_type(self, node):
+        string_literal = False
+        if isinstance(node, ast.Str):
+            string_literal = node.s
+        elif isinstance(node, ast.Constant) and isinstance(node.value, str):
+            string_literal = node.value
+        if string_literal is not False:
+            if self.get_setting('evaluate_string_literal_types'):
+                # TODO: Handle string literal types properly!
+                pass
+            else:
+                return LiteralStr(string_literal)
+        elif isinstance(node, ast.List):
+            if node.elts:
+                return ListType(False, self.evaluate_type(node.elts[0]))
+            else:
+                return ListType(True)
+        elif isinstance(node, ast.Set) and node.elts:
+            return TypeUnion([self.evaluate_type(e) for e in node.elts])
+        elif isinstance(node, ast.Tuple) and node.elts:
+            return TupleType([self.evaluate_type(e) for e in node.elts])
+        elif isinstance(node, ast.Dict):
+            if node.keys and node.values:
+                return DictType([(self.evaluate_type(k), self.evaluate_type(v))
+                                 for k, v in zip(node.keys, node.values)])
+            else:
+                return DictType([])
+        else:
+            evaluated = self.visit(node)
+            return evaluated.as_type(self, self.locate(node))
 
     def visit_GeneratorExp(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
-        # TODO: Handle comprehension scope
-        for generator in node.generators:
-            self.visit(generator)
-        return GeneratorType(self.visit(node.elt))
+        generator_scope = NewScope(self, self.scope_chain[:])
+        with generator_scope:
+            self._visit_nodes(node.generators)
+            return GeneratorType(False, self.visit(node.elt))
 
     def visit_If(self, node):
         """
 
         Args:
             node:
         """
@@ -763,19 +817,19 @@
 
         # Visit the body
         body = self.visit(node.body)
 
         # Visit the orelse
         orelse = self.visit(node.orelse)
 
-        if are_types_equal(body, orelse):
+        if is_subtype(body, orelse):
             return body
 
         # TODO: Union type?
-        return UnknownType()
+        return TypeUnion([body, orelse])
 
     def visit_Import(self, node):
         """
 
         Args:
             node:
         """
@@ -789,115 +843,95 @@
         """
 
         Args:
             node:
         """
         # Handle names
         for alias in node.names:
-            if node.module is None:
-                asname = alias.asname or alias.name
-                module_type = self.load_module(alias.name)
+            if alias.name == '*':
+                module_type = self.load_module(node.module)
+                for field, value in module_type.fields.items():
+                    self.store_read_variable(field, value)
             else:
-                module_name = node.module
-                asname = alias.asname or alias.name
-                module_type = self.load_module(module_name)
-            name_type = module_type.load_attr(alias.name)
-            self.store_variable(asname, name_type)
+                if node.module is None:
+                    asname = alias.asname or alias.name
+                    module_type = self.load_module(alias.name)
+                else:
+                    module_name = node.module
+                    asname = alias.asname or alias.name
+                    module_type = self.load_module(module_name)
+                name_type = module_type.get_attr(alias.name)
+                self.store_variable(asname, name_type)
 
     def visit_Lambda(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
-        # Name
         position = self.locate()
         definitions_scope = self.scope_chain[:]
-
-        def definition(tifa, call_type, call_name, parameters, call_position):
-            """
-
-            Args:
-                tifa:
-                call_type:
-                call_name:
-                parameters:
-                call_position:
-
-            Returns:
-
-            """
-            function_scope = NewScope(self, definitions_scope)
-            with function_scope:
-                # Process arguments
-                args = node.args.args
-                if len(args) != len(parameters):
-                    self._issue(incorrect_arity(position, "lambda", report=self.report))
-                # TODO: Handle special types of parameters
-                for arg, parameter in zip(args, parameters):
-                    name = arg.arg
-                    if parameter is not None:
-                        parameter = parameter.clone_mutably()
-                        self.store_variable(name, parameter, position)
-                if len(args) < len(parameters):
-                    for undefined_parameter in parameters[len(args):]:
-                        self.store_variable(name, UnknownType(), position)
-                return_value = self.visit(node.body)
-            return return_value
-
-        return FunctionType(definition=definition)
+        definition = self.make_function(None, definitions_scope, position, node)
+        return FunctionType("*lambda", definition=definition)
 
     def visit_List(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
-        result_type = ListType()
-        if node.elts:
-            result_type.empty = False
-            # TODO: confirm homogenous subtype
-            for elt in node.elts:
-                result_type.subtype = self.visit(elt)
+        if not node.elts:
+            return ListType(True)
+
+        # All literal keys
+        elements = [self.visit(v) for v in node.elts]
+        if all(isinstance(v, LiteralValue) for v in elements):
+            # TODO: Allow type union instead?
+            return ListType(False, elements[0].promote())
+        # Find if all matched type
+        first_value = widest_type(elements)
+        if first_value is not None:
+            return ListType(False, first_value)
         else:
-            result_type.empty = True
-        return result_type
+            # Resort to just matching the types?
+            return ListType(False, TypeUnion(elements))
 
     def visit_ListComp(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
         # TODO: Handle comprehension scope
-        for generator in node.generators:
-            self.visit(generator)
-        return ListType(self.visit(node.elt))
+        generator_scope = NewScope(self, self.scope_chain[:])
+        with generator_scope:
+            self._visit_nodes(node.generators)
+            return ListType(False, self.visit(node.elt))
 
     def visit_NameConstant(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
         value = node.value
         if isinstance(value, bool):
-            return BoolType()
+            return LiteralBool(value)
         else:
             return NoneType()
 
     def visit_Name(self, node):
         """
 
         Args:
@@ -907,46 +941,46 @@
 
         """
         name = node.id
         if name == "___":
             self._issue(unconnected_blocks(self.locate()))
         if isinstance(node.ctx, ast.Load):
             if name == "True" or name == "False":
-                return BoolType()
+                return LiteralBool(name == "True")
             elif name == "None":
                 return NoneType()
             else:
                 variable = self.find_variable_scope(name)
-                builtin = get_builtin_function(name)
+                builtin = get_builtin_name(name)
                 if not variable.exists and builtin:
                     return builtin
                 else:
                     state = self.load_variable(name)
                     return state.type
         else:
             variable = self.find_variable_scope(name)
             if variable.exists:
                 return variable.state.type
             else:
-                return UnknownType()
+                return AnyType()
 
     def visit_Num(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
-        return NumType()
+        return LiteralInt(node.n) if isinstance(node.n, int) else LiteralFloat(node.n)
 
     def visit_Constant(self, node) -> Type:
         """ Handle new 3.8's Constant node """
-        return get_pedal_type_from_value(node.value)
+        return get_pedal_type_from_value(node.value, self.evaluate_type)
 
     def visit_Return(self, node):
         """
 
         Args:
             node:
         """
@@ -956,29 +990,44 @@
         if node.value is not None:
             self.return_variable(self.visit(node.value))
         else:
             self.return_variable(NoneType())
 
     def visit_Set(self, node):
         # Fun fact, it's impossible to make a literal empty set
-        return SetType(subtype=self.visit(node.elts[0]), empty=False)
+        if not node.elts:
+            return SetType(True)
+
+        # All literal keys
+        elements = [self.visit(v) for v in node.elts]
+        if all(isinstance(v, LiteralValue) for v in elements):
+            # TODO: Allow type union instead?
+            return SetType(False, elements[0].promote())
+        # Find if all matched type
+        first_value = widest_type(elements)
+        if first_value is not None:
+            return SetType(False, first_value)
+        else:
+            # Resort to just matching the types?
+            return SetType(False, TypeUnion(elements))
 
     def visit_SetComp(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
         # TODO: Handle comprehension scope
-        for generator in node.generators:
-            self.visit(generator)
-        return SetType(subtype=self.visit(node.elt))
+        generator_scope = NewScope(self, self.scope_chain[:])
+        with generator_scope:
+            self._visit_nodes(node.generators)
+            return SetType(False, self.visit(node.elt))
 
     def visit_statements(self, nodes):
         """
 
         Args:
             nodes:
 
@@ -995,112 +1044,89 @@
 
         Args:
             node:
 
         Returns:
 
         """
-        if node.s == "":
-            return StrType(True)
-        else:
-            return StrType(False)
+        return LiteralStr(node.s)
 
     def visit_JoinedStr(self, node):
         values = [self.visit(expr) for expr in node.values]
         # The result will be all StrType
-        return StrType(empty=all(n.empty for n in values))
+        return StrType(is_empty=all(isinstance(n, (StrType, LiteralStr)) and n.is_empty
+                                    for n in values))
 
     def visit_FormattedValue(self, node):
         value = self.visit(node.value)
         if isinstance(value, StrType):
             return value
         else:
-            return StrType(empty=False)
+            return StrType(is_empty=False)
 
     def visit_Subscript(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
         # Handle value
         value_type = self.visit(node.value)
-        # Handle slice
-        if IS_PYTHON_39 and isinstance(node.slice, ast.Tuple):
-            # TODO: Do something about extslices (especially since students stumble into this accidentally)
-            pass
-        elif not IS_PYTHON_39 and isinstance(node.slice, ast.ExtSlice):
-            # TODO: Do something about extslices (especially since students stumble into this accidentally)
-            pass
-        elif isinstance(node.slice, ast.Slice):
-            self.visit_Slice(node.slice)
-            return value_type
+        slice_type = self.visit(node.slice)
+        result = value_type.index(slice_type)
+        if isinstance(result, ImpossibleType):
+            self._issue(invalid_indexing(self.locate(), value_type, slice_type))
+        if isinstance(node.slice, ast.Slice):
+            return value_type.shallow_clone()
         else:
-            if IS_PYTHON_39:
-                slice = node.slice
-            else:
-                slice = node.slice.value
-            literal = self.get_literal(slice)
-            if literal is None:
-                literal = get_pedal_literal_from_pedal_type(self.visit(slice))
-            result = value_type.index(literal)
-            # TODO: Is this sufficient? Maybe we should be throwing?
-            if isinstance(result, UnknownType):
-                self._issue(invalid_indexing(self.locate(), value_type,
-                                             literal.type()))
-            else:
-                return result
+            return result
 
     def visit_Slice(self, node):
         """ Handles a slice by visiting its components; cannot return a value
         because the slice is always the same type as its value, which is
         not available on the Slice node itself. """
         if node.lower is not None:
             self.visit(node.lower)
         if node.upper is not None:
             self.visit(node.upper)
         if node.step is not None:
             self.visit(node.step)
 
+    def visit_Index(self, node):
+        return self.visit(node.value)
+
+    def visit_ExtSlice(self, node):
+        return TupleType([self.visit(d) for d in node.dims])
+
+    def visit_Starred(self, node):
+        return self.visit(node.value).break_apart()
+
     def visit_Tuple(self, node) -> TupleType:
-        """ Handle Tuple literal """
-        result_type = TupleType()
+        # Fun fact, it's impossible to make a literal empty set
         if not node.elts:
-            result_type.empty = True
-            result_type.subtypes = []
-        else:
-            result_type.empty = False
-            # TODO: confirm homogenous subtype
-            result_type.subtypes = [self.visit(elt) for elt in node.elts]
-        return result_type
+            return TupleType(True)
+
+        # All literal keys
+        return TupleType([self.visit(v) for v in node.elts])
 
     def visit_UnaryOp(self, node):
         """
 
         Args:
             node:
 
         Returns:
 
         """
         # Handle operand
-        operand = self.visit(node.operand)
-
-        if isinstance(node.op, ast.Not):
-            return BoolType()
-        elif isinstance(operand, UnknownType):
-            return UnknownType()
-        elif type(node.op) in VALID_UNARYOP_TYPES:
-            op_lookup = VALID_UNARYOP_TYPES[type(node.op)]
-            if type(operand) in op_lookup:
-                return op_lookup[type(operand)]()
-        return UnknownType()
+        operand_type = self.visit(node.operand)
+        return apply_unary_operation(node.op, operand_type)
 
     def visit_While(self, node):
         """
 
         Args:
             node:
         """
@@ -1134,11 +1160,11 @@
         """
 
         Args:
             node:
         """
         for item in node.items:
             type_value = self.visit(item.context_expr)
-            self.visit(item.optional_vars)
-            self._walk_target(item.optional_vars, type_value)
+            if item.optional_vars is not None:
+                self.assign_target(item.optional_vars, type_value)
         # Handle the bodies
         self.visit_statements(node.body)
```

### Comparing `pedal-2.3.8/pedal/utilities/__init__.py` & `pedal-2.4.0/pedal/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/utilities/ast_tools.py` & `pedal-2.4.0/pedal/utilities/ast_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "And": "a boolean AND operator",
     "AnnAssign": "an annotated assignment",
     "Assert": "an assert statement",
     "Assign": "an assignment statement",
     "AsyncFor": "an asychronous for loop",
     "AsyncFunctionDef": "an asychronous function definition",
     "AsyncWith": "an asychronous with statement",
-    "Attribute": "an attribute lookup",
+    "Attribute": "an attribute lookup (access a field)",
     "AugAssign": "an augmented assignment",
     "AugLoad": "an augmented load",
     "AugStore": "an augmented store",
     "Await": "an await statement",
     "BinOp": "a binary operator",
     "BitAnd": "a bitwise AND operator",
     "BitOr": "a bitwise OR operator",
```

### Comparing `pedal-2.3.8/pedal/utilities/comparisons.py` & `pedal-2.4.0/pedal/utilities/comparisons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import string
 import re
 
 # Number encapsulates bool, int, float, complex, decimal.Decimal, etc.
 try:
+    from dataclasses import is_dataclass, fields
+except ImportError:
+    is_dataclass = lambda value: False
+
+try:
     from numbers import Number
 except:
     Number = (bool, int, float, complex)
 
 try:
     bytes
 except NameError:
@@ -121,15 +126,15 @@
     if isinstance(actual, LIST_GENERATOR_TYPES):
         actual = list(actual)
     elif isinstance(actual, SET_GENERATOR_TYPES):
         actual = set(actual)
 
     # Float comparison
     if isinstance(expected, float) and isinstance(actual, (float, int)):
-        error = 10 ** (-_delta)
+        error = _delta
         return abs(expected - actual) < error
     # Other numerics
     elif isinstance(expected, Number) and isinstance(actual, Number) and isinstance(expected, type(actual)):
         return expected == actual
     # String comparisons
     elif ((isinstance(expected, str) and isinstance(actual, str)) or
           (isinstance(expected, bytes) and isinstance(actual, bytes))):
@@ -153,14 +158,19 @@
         primary_keys = set(expected.keys())
         if not _are_sets_equal(primary_keys, set(actual.keys()), _exact_strings, _delta):
             return False
         for key in primary_keys:
             if not equality_test(expected[key], actual[key], _exact_strings, _delta):
                 return False
         return True
+    # Two dataclasses
+    elif is_dataclass(expected) and is_dataclass(actual):
+        return (expected.__name__ == actual.__name__ and
+                all(e.name == a.name and equality_test(e.type, a.type, _exact_strings, _delta)
+                    for e, a in zip(fields(expected), fields(actual))))
     # Else
     return False
 
 
 def _are_sequences_equal(x, y, _exact_strings, _delta):
     """
     For sequences that support __len__, __iter__, and should have the same
```

### Comparing `pedal-2.3.8/pedal/utilities/dictionaries.py` & `pedal-2.4.0/pedal/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/utilities/exceptions.py` & `pedal-2.4.0/pedal/utilities/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,11 +229,13 @@
         """
         traceback_message = "\n".join([
             (f"Line {formatter.line(frame.lineno)}"
              f" of file {formatter.filename(frame.filename)}" +
              (f" in {formatter.frame(frame.name)}\n"
               if frame.name != "<module>" and frame.name is not None
               else "\n") +
-             f"{formatter.python_code(frame.line)}\n")
+             f"{formatter.python_code(frame.line if frame.line is not None else '')}\n")
             for frame in traceback_stack
         ])
+        if not traceback_message:
+            return None
         return formatter.traceback(traceback_message)
```

### Comparing `pedal-2.3.8/pedal/utilities/files.py` & `pedal-2.4.0/pedal/utilities/files.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/utilities/operators.py` & `pedal-2.4.0/pedal/utilities/operators.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/utilities/progsnap.py` & `pedal-2.4.0/pedal/utilities/progsnap.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,31 +55,41 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
 
 class SqlProgSnap2(BaseProgSnap2):
     PROFILES = {
-        'blockpy': dict(link_filters={
-            'Subject': {
-                'X-IsStaff': "False",
+        'blockpy': dict(
+            link_filters={
+                'Subject': {
+                    'X-IsStaff': "False",
+                },
+                "Assignment": {
+                    #"X-Name": "Midterm 2.4"
+                #    "X-Course.Id": "4"
+                }
             },
-        },
             link_selections={
                 'Subject': {
+                    #'X-Pokemon': 'student_pokemon',
                     'X-Email': 'student_email',
                     'X-Name.First': 'student_first',
                     'X-Name.Last': 'student_last',
                 },
                 'Assignment': {
                     'X-Name': 'assignment_name',
                     'X-URL': 'assignment_url',
                     'X-Code.OnRun': 'on_run'
                 }
-            })
+            },
+            link_primary={
+                'user': 'student_email'
+            },
+        ),
     }
 
     def set_profile(self, profile):
         if profile not in self.PROFILES:
             raise ValueError(f"Unknown ProgSnap Profile specified: {profile}")
         self.profile = profile
```

### Comparing `pedal-2.3.8/pedal/utilities/sorting.py` & `pedal-2.4.0/pedal/utilities/sorting.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/pedal/utilities/text.py` & `pedal-2.4.0/pedal/utilities/text.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 
 def add_indefinite_article(phrase):
     """
     Given a word, choose the appropriate indefinite article (e.g., "a" or "an")
     and add it the front of the word. Matches the original word's
     capitalization.
 
+
     Args:
         phrase (str): The phrase to get the appropriate definite article
             for.
 
     Returns:
         str: Either "an" or "a".
     """
-    if phrase[0] in "aeiou":
+    # Note: Must cast to string because it could be a SandboxResult
+    if str(phrase[0]) in "aeiou":
         return "an "+phrase
-    elif phrase[0] in "AEIOU":
+    elif str(phrase[0]) in "AEIOU":
         return "An "+phrase
     elif phrase[0].lower() == phrase[0]:
         return "a "+phrase
     else:
         return "A "+phrase
 
 
@@ -59,7 +61,21 @@
     if not text:
         return text
     if text[-2:] == '\n\r':
         return text[:-2]
     if text[-1] == '\n':
         return text[:-1]
     return text
+
+
+def join_list_with_and(items):
+    """ Properly format the string with commas (oxford-style) and the word `and`."""
+    items = list(items)
+    if len(items) < 1:
+        return ""
+    elif len(items) == 1:
+        return items[0]
+    elif len(items) == 2:
+        return f"{items[0]} and {items[1]}"
+    else:
+        pre = ", ".join(items[:-1])
+        return f"{pre}, and {items[-1]}"
```

### Comparing `pedal-2.3.8/pedal/utilities/types.py` & `pedal-2.4.0/pedal/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pedal-2.3.8/setup.py` & `pedal-2.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name='pedal',
-    version='2.3.8',
+    version='2.4.0',
     python_requires='>=3.6',
     author='acbart,lukesg08',
     author_email='acbart@udel.edu',
     description='Tools to provide feedback on student code.',
     keywords='feedback education teaching program analysis tifa cait sandbox pedal grading grader grade',
     packages=['pedal', 'pedal.core', 'pedal.utilities', 'pedal.environments',
               'pedal.resolvers', 'pedal.command_line',
               'pedal.source', 'pedal.cait', 'pedal.tifa',
-              'pedal.sandbox', 'pedal.assertions',
-              'pedal.questions', 'pedal.extensions', 'pedal.types'
+              'pedal.sandbox', 'pedal.sandbox.library', 'pedal.assertions',
+              'pedal.questions', 'pedal.extensions', 'pedal.types', 'pedal.types.library'
               ],
     license='Creative Commons Attribution-Noncommercial-Share Alike license',
     long_description=open('README.rst').read(),
     install_requires=["tabulate"],
     entry_points={
           'console_scripts': [
               'pedal = pedal.command_line.command_line:main'
```

