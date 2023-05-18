# Comparing `tmp/data2latex-1.0.4.tar.gz` & `tmp/data2latex-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2latex-1.0.4.tar", last modified: Tue May 16 08:23:16 2023, max compression
+gzip compressed data, was "data2latex-1.0.5.tar", last modified: Thu May 18 11:21:42 2023, max compression
```

## Comparing `data2latex-1.0.4.tar` & `data2latex-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:23:16.401973 data2latex-1.0.4/
--rw-rw-rw-   0        0        0     1094 2023-05-14 10:51:18.000000 data2latex-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4923 2023-05-16 08:23:16.400974 data2latex-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2528 2023-05-16 08:12:54.000000 data2latex-1.0.4/README.md
--rw-rw-rw-   0        0        0     1824 2023-05-16 08:15:25.000000 data2latex-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 08:23:16.401973 data2latex-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 08:23:16.372974 data2latex-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 08:23:16.387008 data2latex-1.0.4/src/data2latex/
--rw-rw-rw-   0        0        0      266 2023-05-11 19:09:04.000000 data2latex-1.0.4/src/data2latex/__init__.py
--rw-rw-rw-   0        0        0     8454 2023-05-14 20:33:59.000000 data2latex-1.0.4/src/data2latex/dm.py
--rw-rw-rw-   0        0        0     7494 2023-05-14 20:34:47.000000 data2latex-1.0.4/src/data2latex/environments.py
--rw-rw-rw-   0        0        0    10016 2023-05-14 20:34:10.000000 data2latex-1.0.4/src/data2latex/features.py
--rw-rw-rw-   0        0        0     7658 2023-05-14 14:44:36.000000 data2latex-1.0.4/src/data2latex/iter_protocols.py
--rw-rw-rw-   0        0        0    30916 2023-05-14 14:44:36.000000 data2latex-1.0.4/src/data2latex/plot.py
--rw-rw-rw-   0        0        0    18502 2023-05-13 21:52:50.000000 data2latex-1.0.4/src/data2latex/table.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:23:16.399975 data2latex-1.0.4/src/data2latex.egg-info/
--rw-rw-rw-   0        0        0     4923 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 11:21:42.710700 data2latex-1.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-05-14 10:51:18.000000 data2latex-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4923 2023-05-18 11:21:42.709695 data2latex-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2528 2023-05-16 08:12:54.000000 data2latex-1.0.5/README.md
+-rw-rw-rw-   0        0        0     1824 2023-05-18 11:19:58.000000 data2latex-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 11:21:42.710700 data2latex-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 11:21:42.673695 data2latex-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 11:21:42.687731 data2latex-1.0.5/src/data2latex/
+-rw-rw-rw-   0        0        0      266 2023-05-11 19:09:04.000000 data2latex-1.0.5/src/data2latex/__init__.py
+-rw-rw-rw-   0        0        0     8454 2023-05-14 20:33:59.000000 data2latex-1.0.5/src/data2latex/dm.py
+-rw-rw-rw-   0        0        0     7494 2023-05-14 20:34:47.000000 data2latex-1.0.5/src/data2latex/environments.py
+-rw-rw-rw-   0        0        0    10016 2023-05-14 20:34:10.000000 data2latex-1.0.5/src/data2latex/features.py
+-rw-rw-rw-   0        0        0     7658 2023-05-14 14:44:36.000000 data2latex-1.0.5/src/data2latex/iter_protocols.py
+-rw-rw-rw-   0        0        0    30923 2023-05-18 11:19:17.000000 data2latex-1.0.5/src/data2latex/plot.py
+-rw-rw-rw-   0        0        0    18502 2023-05-13 21:52:50.000000 data2latex-1.0.5/src/data2latex/table.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:21:42.708695 data2latex-1.0.5/src/data2latex.egg-info/
+-rw-rw-rw-   0        0        0     4923 2023-05-18 11:21:42.000000 data2latex-1.0.5/src/data2latex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-05-18 11:21:42.000000 data2latex-1.0.5/src/data2latex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 11:21:42.000000 data2latex-1.0.5/src/data2latex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-05-18 11:21:42.000000 data2latex-1.0.5/src/data2latex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 11:21:42.000000 data2latex-1.0.5/src/data2latex.egg-info/top_level.txt
```

### Comparing `data2latex-1.0.4/LICENSE` & `data2latex-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.4/PKG-INFO` & `data2latex-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2latex
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document.
 Author-email: Richard Kokštein <richard.Kokstein@fs.cvut.cz>
 License: MIT License
         
         Copyright (c) 2023 Richard Kokstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `data2latex-1.0.4/README.md` & `data2latex-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.4/pyproject.toml` & `data2latex-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data2latex"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Richard Kokštein", email="richard.Kokstein@fs.cvut.cz" },
 ]
 description = "Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document."
 keywords = ["generation", "latex", "table", "plot", "graph", "array", "datatable"]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
```

### Comparing `data2latex-1.0.4/src/data2latex/dm.py` & `data2latex-1.0.5/src/data2latex/dm.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.4/src/data2latex/environments.py` & `data2latex-1.0.5/src/data2latex/environments.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.4/src/data2latex/features.py` & `data2latex-1.0.5/src/data2latex/features.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.4/src/data2latex/iter_protocols.py` & `data2latex-1.0.5/src/data2latex/iter_protocols.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.4/src/data2latex/plot.py` & `data2latex-1.0.5/src/data2latex/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,15 +448,15 @@
 
     :param mode: Axis scale: the first tuple element for x axis, the second one for y axis. If single value is given, it will be used for both axis. Defaults to ``("lin", "lin")``.
     :type mode: Union[AxisMode, Tuple[AxisMode, AxisMode]], optional
 
     :param legend: Legend entries: input ``None`` if dataset should not have an entry. Defaults to ``None``.
     :type legend: Union[None, str, List[Union[None, str]]], optional
 
-    :param legend_pos: Legend position: available string literals start with vertical position (e.g. top) followed by horizontal position (e.g. right). Defaults to "top right".
+    :param legend_pos: Legend position: available string literals start with vertical position (e.g. top) followed by horizontal position (e.g. right). Defaults to ``"top right"``.
     :type legend_pos: LegendPosition, optional
 
     :param legend_entry_align: Horizontal text alignment of legend entries, defaults to ``"c"``.
     :type legend_entry_align: Literal[``l``, ``c``, ``r``], optional
 
     :param width: Width of the plot with unit, defaults to ``None``.
     :type width: Optional[str], optional
@@ -469,21 +469,21 @@
 
     :param xlimits: Limits for x axis: either two numbers (min, max) in tuple or ``"exact"`` literal for setting the limits to minimum and maximum of the datasets. Defaults to ``None``.
     :type xlimits: Optional[Union[Tuple[Optional[float], Optional[float]], Literal[``exact``]]], optional
 
     :param ylimits: Limits for y axis: either two numbers (min, max) in tuple or ``"exact"`` literal for setting the limits to minimum and maximum of the datasets. Defaults to ``None``.
     :type ylimits: Optional[Union[Tuple[Optional[float], Optional[float]], Literal[``exact``]]], optional
 
-    :param precision: Precision of the displayed tick labels in the form of (x axis tick labels, y axis tick labels). Defaults to (2, 2).
+    :param precision: Precision of the displayed tick labels in the form of (x axis tick labels, y axis tick labels). Defaults to ``(2, 2)``.
     :type precision: Union[int, Tuple[int, int]], optional
 
     :param zerofill: ``True`` for padding decimal numbers (tick labels) with zeros to satisfy given precision, defaults to ``(False, False)``.
     :type zerofill: Union[bool, Tuple[bool, bool]], optional
 
-    :param label: Label for later referencing, use format ``"prefix:label"`` or just ``"label"`` with automatic prefix ``"table"``, defaults to ``None``.
+    :param label: Label for later referencing, use format ``"prefix:label"`` or just ``"label"`` with automatic prefix ``"plot"``, defaults to ``None``.
     :type label: Optional[str], optional
 
     :param caption_pos: Position caption above or below the table, defaults to ``"below"``.
     :type caption_pos: Literal[``above``, ``below``], optional
 
     :param escape_caption: ``True`` for escaping special LaTeX symbols in caption text, defaults to ``True``.
     :type escape_caption: bool, optional
```

### Comparing `data2latex-1.0.4/src/data2latex/table.py` & `data2latex-1.0.5/src/data2latex/table.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.4/src/data2latex.egg-info/PKG-INFO` & `data2latex-1.0.5/src/data2latex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2latex
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document.
 Author-email: Richard Kokštein <richard.Kokstein@fs.cvut.cz>
 License: MIT License
         
         Copyright (c) 2023 Richard Kokstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

