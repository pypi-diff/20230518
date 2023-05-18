# Comparing `tmp/types_wxpython-0.6.1.tar.gz` & `tmp/types_wxpython-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_wxpython-0.6.1.tar", max compression
+gzip compressed data, was "types_wxpython-0.7.0.tar", max compression
```

## Comparing `types_wxpython-0.6.1.tar` & `types_wxpython-0.7.0.tar`

### file list

```diff
@@ -1,73 +1,82 @@
--rw-r--r--   0        0        0    35149 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/LICENSE
--rw-r--r--   0        0        0      725 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/README.md
--rw-r--r--   0        0        0     1136 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/DateTime/__init__.py
--rw-r--r--   0        0        0     2234 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/DateTime/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/FileType/__init__.py
--rw-r--r--   0        0        0     1048 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/FileType/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/Image/__init__.py
--rw-r--r--   0        0        0     1289 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/Image/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/TopLevelWindow/__init__.py
--rw-r--r--   0        0        0      266 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/TopLevelWindow/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/Window/__init__.py
--rw-r--r--   0        0        0      504 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/Window/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.366032 types_wxpython-0.6.1/wx-stubs/__init__.py
--rw-r--r--   0        0        0  1392740 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/adv/__init__.py
--rw-r--r--   0        0        0   113754 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/adv/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/aui/__init__.py
--rw-r--r--   0        0        0   103225 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/aui/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/dataview/__init__.py
--rw-r--r--   0        0        0   102538 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/dataview/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/glcanvas/__init__.py
--rw-r--r--   0        0        0    11748 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/glcanvas/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/grid/GridBlocks/__init__.py
--rw-r--r--   0        0        0      224 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/grid/GridBlocks/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.374032 types_wxpython-0.6.1/wx-stubs/grid/__init__.py
--rw-r--r--   0        0        0   136022 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/grid/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/html/__init__.py
--rw-r--r--   0        0        0    79713 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/html/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/html2/__init__.py
--rw-r--r--   0        0        0    21475 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/html2/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/agw/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/buttonbar/__init__.py
--rw-r--r--   0        0        0     1041 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/buttonbar/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/gallery/__init__.py
--rw-r--r--   0        0        0     1940 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/gallery/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/toolbar/__init__.py
--rw-r--r--   0        0        0      507 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/toolbar/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/analogclock/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.378032 types_wxpython-0.6.1/wx-stubs/lib/analogclock/lib_setup/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.py
--rw-r--r--   0        0        0      985 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/buttons/__init__.py
--rw-r--r--   0        0        0    16016 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/buttons/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/calendar/__init__.py
--rw-r--r--   0        0        0    15899 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/calendar/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/colourselect/__init__.py
--rw-r--r--   0        0        0     4240 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/colourselect/__init__.pyi
--rw-r--r--   0        0        0     2359 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/dialogs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/newevent/__init__.py
--rw-r--r--   0        0        0      452 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/newevent/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/scrolledpanel/__init__.py
--rw-r--r--   0        0        0     1746 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/scrolledpanel/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/wxpTag/__init__.py
--rw-r--r--   0        0        0     1060 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/lib/wxpTag/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/media/__init__.py
--rw-r--r--   0        0        0     6253 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/media/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/propgrid/__init__.py
--rw-r--r--   0        0        0   188688 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/propgrid/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.382032 types_wxpython-0.6.1/wx-stubs/ribbon/__init__.py
--rw-r--r--   0        0        0    80698 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/ribbon/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/richtext/__init__.py
--rw-r--r--   0        0        0   359303 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/richtext/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/stc/__init__.py
--rw-r--r--   0        0        0   182036 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/stc/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/xml/__init__.py
--rw-r--r--   0        0        0    14147 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/xml/__init__.pyi
--rw-r--r--   0        0        0        0 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/xrc/__init__.py
--rw-r--r--   0        0        0    18939 2023-03-29 11:17:09.386032 types_wxpython-0.6.1/wx-stubs/xrc/__init__.pyi
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 types_wxpython-0.6.1/setup.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 types_wxpython-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-01 15:52:26.763638 types_wxpython-0.7.0/LICENSE
+-rw-r--r--   0        0        0      725 2023-04-01 15:52:26.763638 types_wxpython-0.7.0/README.md
+-rw-r--r--   0        0        0     1136 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/ActivateEvent/__init__.pyi
+-rw-r--r--   0        0        0      120 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/ConfigBase/__init__.pyi
+-rw-r--r--   0        0        0      135 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/DataObject/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/DateTime/__init__.py
+-rw-r--r--   0        0        0     2371 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/DateTime/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/FileType/__init__.py
+-rw-r--r--   0        0        0     1059 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/FileType/__init__.pyi
+-rw-r--r--   0        0        0      132 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/HelpEvent/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/Image/__init__.py
+-rw-r--r--   0        0        0     1300 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/Image/__init__.pyi
+-rw-r--r--   0        0        0      173 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/StandardPaths/__init__.pyi
+-rw-r--r--   0        0        0      135 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/StaticBitmap/__init__.pyi
+-rw-r--r--   0        0        0      130 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/StockPreferencesPage/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/TopLevelWindow/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/TopLevelWindow/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/Window/__init__.py
+-rw-r--r--   0        0        0      515 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/Window/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.767638 types_wxpython-0.7.0/wx-stubs/__init__.py
+-rw-r--r--   0        0        0  1400871 2023-04-01 15:52:26.771638 types_wxpython-0.7.0/wx-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.771638 types_wxpython-0.7.0/wx-stubs/adv/__init__.py
+-rw-r--r--   0        0        0   114383 2023-04-01 15:52:26.775638 types_wxpython-0.7.0/wx-stubs/adv/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.775638 types_wxpython-0.7.0/wx-stubs/aui/__init__.py
+-rw-r--r--   0        0        0   103369 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/aui/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/dataview/__init__.py
+-rw-r--r--   0        0        0   102847 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/dataview/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/glcanvas/__init__.py
+-rw-r--r--   0        0        0    11759 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/glcanvas/__init__.pyi
+-rw-r--r--   0        0        0      134 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/grid/Grid/__init__.pyi
+-rw-r--r--   0        0        0      132 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/grid/GridActivationSource/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/grid/GridBlocks/__init__.py
+-rw-r--r--   0        0        0      235 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/grid/GridBlocks/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/grid/__init__.py
+-rw-r--r--   0        0        0   136304 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/grid/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/html/__init__.py
+-rw-r--r--   0        0        0    80110 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/html/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/html2/__init__.py
+-rw-r--r--   0        0        0    21938 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/html2/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/agw/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/buttonbar/__init__.py
+-rw-r--r--   0        0        0     1052 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/buttonbar/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/gallery/__init__.py
+-rw-r--r--   0        0        0     1951 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/gallery/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/toolbar/__init__.py
+-rw-r--r--   0        0        0      518 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/toolbar/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/analogclock/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/analogclock/lib_setup/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.py
+-rw-r--r--   0        0        0      996 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/buttons/__init__.py
+-rw-r--r--   0        0        0    16019 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/buttons/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/calendar/__init__.py
+-rw-r--r--   0        0        0    15906 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/calendar/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/colourselect/__init__.py
+-rw-r--r--   0        0        0     4270 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/colourselect/__init__.pyi
+-rw-r--r--   0        0        0     2370 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/dialogs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/newevent/__init__.py
+-rw-r--r--   0        0        0      463 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/newevent/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/scrolledpanel/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/scrolledpanel/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/wxpTag/__init__.py
+-rw-r--r--   0        0        0     1071 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/lib/wxpTag/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/media/__init__.py
+-rw-r--r--   0        0        0     6369 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/media/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/propgrid/__init__.py
+-rw-r--r--   0        0        0   189238 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/propgrid/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/ribbon/__init__.py
+-rw-r--r--   0        0        0    81621 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/ribbon/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.779638 types_wxpython-0.7.0/wx-stubs/richtext/__init__.py
+-rw-r--r--   0        0        0   360498 2023-04-01 15:52:26.783639 types_wxpython-0.7.0/wx-stubs/richtext/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.783639 types_wxpython-0.7.0/wx-stubs/stc/__init__.py
+-rw-r--r--   0        0        0   182064 2023-04-01 15:52:26.783639 types_wxpython-0.7.0/wx-stubs/stc/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.783639 types_wxpython-0.7.0/wx-stubs/xml/__init__.py
+-rw-r--r--   0        0        0    14211 2023-04-01 15:52:26.783639 types_wxpython-0.7.0/wx-stubs/xml/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-01 15:52:26.783639 types_wxpython-0.7.0/wx-stubs/xrc/__init__.py
+-rw-r--r--   0        0        0    19060 2023-04-01 15:52:26.783639 types_wxpython-0.7.0/wx-stubs/xrc/__init__.pyi
+-rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 types_wxpython-0.7.0/setup.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 types_wxpython-0.7.0/PKG-INFO
```

### Comparing `types_wxpython-0.6.1/LICENSE` & `types_wxpython-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.6.1/README.md` & `types_wxpython-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `types_wxpython-0.6.1/pyproject.toml` & `types_wxpython-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "types-wxpython"
-version = "0.6.1"
+version = "0.7.0"
 description = "Typing stubs for wxPython"
 authors = ["Alexion Software <info@alexion.nl>"]
 homepage = "https://github.com/AlexionSoftware/types-wxpython"
 repository = "https://github.com/AlexionSoftware/types-wxpython"
 keywords = ["wxPython", "typing", "stubs", "wx"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `types_wxpython-0.6.1/wx-stubs/DateTime/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/DateTime/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class TimeZone:
     """ Class representing a time zone.
 
         Source: https://docs.wxpython.org/wx.DateTime.TimeZone.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -36,31 +36,39 @@
 
 
 class Tm:
     """ Contains broken down date-time representation.
 
         Source: https://docs.wxpython.org/wx.DateTime.Tm.html
     """
-    def GetWeekDay(self) -> 'DateTime.WeekDay':
+    def GetWeekDay(self) -> 'WeekDay':
         """ Return the week day corresponding to this date.
 
             Source: https://docs.wxpython.org/wx.DateTime.Tm.html
         """
 
     def IsValid(self) -> bool:
         """ Check if the given date/time is valid (in Gregorian calendar).
 
             Source: https://docs.wxpython.org/wx.DateTime.Tm.html
         """
 
-    WeekDay: 'DateTime.WeekDay'  # See GetWeekDay
+    WeekDay: 'WeekDay'  # See GetWeekDay
     hour: Any  # A public C++ attribute of type int. Hours since midnight in 0..23 range.
     mday: Any  # A public C++ attribute of type int. Day of the month in 1..31 range.
     min: Any  # A public C++ attribute of type int. Minutes in 0..59 range.
     mon: Any  # A public C++ attribute of type DateTime.Month. Month, as an enumerated constant.
     msec: Any  # A public C++ attribute of type int. Number of milliseconds.
     sec: Any  # A public C++ attribute of type int. Seconds in 0..59 (60 with leap seconds) range.
     yday: Any  # A public C++ attribute of type int. Day of the year in 0..365 range.
     year: Any  # A public C++ attribute of type int. Year.
 
 
 
+Country: TypeAlias = int  # Enumeration
+
+WeekFlags: TypeAlias = int  # Enumeration
+
+Month: TypeAlias = Any  # Enumeration
+
+TZ: TypeAlias = Any
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/FileType/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/FileType/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class MessageParameters:
     """ Class representing message parameters.
 
         Source: https://docs.wxpython.org/wx.FileType.MessageParameters.html
     """
     def __init__(self, *args, **kw) -> None:
```

### Comparing `types_wxpython-0.6.1/wx-stubs/Image/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/Image/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class HSVValue:
     """ A simple class which stores hue, saturation and value as doubles in
 the range 0.0-1.0.
 
         Source: https://docs.wxpython.org/wx.Image.HSVValue.html
     """
```

### Comparing `types_wxpython-0.6.1/wx-stubs/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
+
+FontFamily: TypeAlias = int  # Enumeration
 
 FONTFAMILY_DEFAULT: int
 
 FONTFAMILY_DECORATIVE: int
 
 FONTFAMILY_ROMAN: int
 
@@ -15,14 +17,16 @@
 
 FONTFAMILY_TELETYPE: int
 
 FONTFAMILY_MAX: int
 
 FONTFAMILY_UNKNOWN: int
 
+FontWeight: TypeAlias = int  # Enumeration
+
 FONTWEIGHT_INVALID: int
 
 FONTWEIGHT_THIN: int
 
 FONTWEIGHT_EXTRALIGHT: int
 
 FONTWEIGHT_LIGHT: int
@@ -39,14 +43,16 @@
 
 FONTWEIGHT_HEAVY: int
 
 FONTWEIGHT_EXTRAHEAVY: int
 
 FONTWEIGHT_MAX: int
 
+StockCursor: TypeAlias = int  # Enumeration
+
 CURSOR_NONE: int
 
 CURSOR_ARROW: int
 
 CURSOR_RIGHT_ARROW: int
 
 CURSOR_BULLSEYE: int
@@ -101,14 +107,16 @@
 
 CURSOR_COPY_ARROW: int
 
 CURSOR_ARROWWAIT: int
 
 CURSOR_MAX: int
 
+StandardID: TypeAlias = int  # Enumeration
+
 ID_AUTO_LOWEST: int
 
 ID_ANY: int
 
 ID_AUTO_HIGHEST: int
 
 ID_NONE: int
@@ -373,14 +381,16 @@
 
 ID_FILEDLGG: int
 
 ID_FILECTRL: int
 
 ID_HIGHEST: int
 
+FontEncoding: TypeAlias = int  # Enumeration
+
 FONTENCODING_SYSTEM: int
 
 FONTENCODING_DEFAULT: int
 
 FONTENCODING_ISO8859_1: int
 
 FONTENCODING_ISO8859_2: int
@@ -579,14 +589,16 @@
 
 FONTENCODING_EUC_KR: int
 
 FONTENCODING_JOHAB: int
 
 FONTENCODING_VIETNAMESE: int
 
+FontStyle: TypeAlias = int  # Enumeration
+
 FONTSTYLE_NORMAL: int
 
 FONTSTYLE_ITALIC: int
 
 FONTSTYLE_SLANT: int
 
 FONTSTYLE_MAX: int
@@ -1087,15 +1099,15 @@
 def GetTopLevelParent(window: 'Window') -> 'Window':
     """ Returns the first top level parent of the given window, or in other words, the frame or dialog containing it, or None.
 
         Source: https://docs.wxpython.org/wx.functions.html
     """
 
 
-def GetTopLevelWindows() -> WindowList:
+def GetTopLevelWindows() -> 'WindowList':
     """ Returns a list-like object of the the applicationâs top-level windows, (frames,dialogs, etc.)
 
         Source: https://docs.wxpython.org/wx.functions.html
     """
 
 
 def GetTranslation(*args, **kw) -> str:
@@ -1584,14 +1596,16 @@
 
 FD_MULTIPLE: int
 
 OK: int
 
 KILL_NOCHILDREN: int
 
+_MenuItem: TypeAlias = MenuItem
+
 class AcceleratorEntry:
     """ An object used by an application wishing to create an accelerator
 table (see AcceleratorTable).
 
         Source: https://docs.wxpython.org/wx.AcceleratorEntry.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -1665,15 +1679,15 @@
 
             Source: https://docs.wxpython.org/wx.AcceleratorEntry.html
         """
 
     Command: int  # See GetCommand
     Flags: int  # See GetFlags
     KeyCode: int  # See GetKeyCode
-    MenuItem: 'MenuItem'  # See GetMenuItem
+    MenuItem: '_MenuItem'  # See GetMenuItem
 
 
 
 class AcceleratorTable(Object):
     """ An accelerator table allows the application to specify a table of
 keyboard shortcuts for menu or button commands.
 
@@ -1689,14 +1703,16 @@
         """ Returns True if the accelerator table is valid.
 
             Source: https://docs.wxpython.org/wx.AcceleratorTable.html
         """
 
 
 
+_Window: TypeAlias = Window
+
 class Accessible(Object):
     """ The Accessible class allows wxWidgets applications, and wxWidgets
 itself, to return extended information about user interface elements
 to client applications such as screen readers.
 
         Source: https://docs.wxpython.org/wx.Accessible.html
     """
@@ -1829,15 +1845,15 @@
 
     def SetWindow(self, window: 'Window') -> None:
         """ Sets the window associated with this object.
 
             Source: https://docs.wxpython.org/wx.Accessible.html
         """
 
-    Window: 'Window'  # See GetWindow and SetWindow
+    Window: '_Window'  # See GetWindow and SetWindow
 
 
 
 ACC_NOT_SUPPORTED: int
 
 ACC_OK: int
 
@@ -1981,21 +1997,21 @@
 
     def Set(self, mat2D, tr) -> None:
         """ Set all elements of this matrix.
 
             Source: https://docs.wxpython.org/wx.AffineMatrix2D.html
         """
 
-    def TransformDistance(self, *args, **kw) -> Point2DDouble:
+    def TransformDistance(self, *args, **kw) -> 'Point2DDouble':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.AffineMatrix2D.html
         """
 
-    def TransformPoint(self, *args, **kw) -> Point2DDouble:
+    def TransformPoint(self, *args, **kw) -> 'Point2DDouble':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.AffineMatrix2D.html
         """
 
     def Translate(self, dx, dy) -> None:
         """ Add the translation to this matrix.
@@ -2084,21 +2100,21 @@
 
     def Set(self, mat2D, tr) -> None:
         """ Set all elements of this matrix.
 
             Source: https://docs.wxpython.org/wx.AffineMatrix2DBase.html
         """
 
-    def TransformDistance(self, *args, **kw) -> Point2DDouble:
+    def TransformDistance(self, *args, **kw) -> 'Point2DDouble':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.AffineMatrix2DBase.html
         """
 
-    def TransformPoint(self, *args, **kw) -> Point2DDouble:
+    def TransformPoint(self, *args, **kw) -> 'Point2DDouble':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.AffineMatrix2DBase.html
         """
 
     def Translate(self, dx, dy) -> None:
         """ Add the translation to this matrix.
@@ -2150,14 +2166,20 @@
             Source: https://docs.wxpython.org/wx.AlphaPixelData.html
         """
 
     Pixels: 'AlphaPixelData_Accessor'  # See GetPixels
 
 
 
+_Mask: TypeAlias = Mask
+
+_Palette: TypeAlias = Palette
+
+_Size: TypeAlias = Size
+
 class Bitmap(GDIObject):
     """ This class encapsulates the concept of a platform-dependent bitmap,
 either monochrome or colour or colour with alpha channel support.
 
         Source: https://docs.wxpython.org/wx.Bitmap.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -2486,21 +2508,21 @@
     DIPSize: 'Size'  # See GetDIPSize
     Depth: int  # See GetDepth and SetDepth
     Handle: int  # See GetHandle and SetHandle
     Height: int  # See GetHeight and SetHeight
     LogicalHeight: float  # See GetLogicalHeight
     LogicalSize: 'Size'  # See GetLogicalSize
     LogicalWidth: float  # See GetLogicalWidth
-    Mask: 'Mask'  # See GetMask and SetMask
-    Palette: 'Palette'  # See GetPalette and SetPalette
+    Mask: '_Mask'  # See GetMask and SetMask
+    Palette: '_Palette'  # See GetPalette and SetPalette
     ScaleFactor: float  # See GetScaleFactor and SetScaleFactor
     ScaledHeight: float  # See GetScaledHeight
     ScaledSize: 'Size'  # See GetScaledSize
     ScaledWidth: float  # See GetScaledWidth
-    Size: 'Size'  # See GetSize and SetSize
+    Size: '_Size'  # See GetSize and SetSize
     Width: int  # See GetWidth and SetWidth
 
 
 
 ALPHA_OPAQUE: int
 
 class AlphaPixelData_Accessor:
@@ -2578,14 +2600,16 @@
         """ 
 
             Source: https://docs.wxpython.org/wx.AlphaPixelData_Accessor.html
         """
 
 
 
+_Bitmap: TypeAlias = Bitmap
+
 class AnyButton(Control):
     """ A class for common button functionality used as the base for the
 various button classes.
 
         Source: https://docs.wxpython.org/wx.AnyButton.html
     """
     def __init__(self) -> None:
@@ -2680,21 +2704,21 @@
 
     def SetBitmapPressed(self, bitmap: 'BitmapBundle') -> None:
         """ Sets the bitmap for the selected (depressed) button appearance.
 
             Source: https://docs.wxpython.org/wx.AnyButton.html
         """
 
-    Bitmap: 'Bitmap'  # See GetBitmap and SetBitmap
-    BitmapCurrent: 'BitmapBundle'  # See GetBitmapCurrent and SetBitmapCurrent
-    BitmapDisabled: 'BitmapBundle'  # See GetBitmapDisabled and SetBitmapDisabled
-    BitmapFocus: 'BitmapBundle'  # See GetBitmapFocus and SetBitmapFocus
-    BitmapLabel: 'BitmapBundle'  # See GetBitmapLabel and SetBitmapLabel
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
+    BitmapCurrent: 'Bitmap'  # See GetBitmapCurrent and SetBitmapCurrent
+    BitmapDisabled: 'Bitmap'  # See GetBitmapDisabled and SetBitmapDisabled
+    BitmapFocus: 'Bitmap'  # See GetBitmapFocus and SetBitmapFocus
+    BitmapLabel: 'Bitmap'  # See GetBitmapLabel and SetBitmapLabel
     BitmapMargins: 'Size'  # See GetBitmapMargins and SetBitmapMargins
-    BitmapPressed: 'BitmapBundle'  # See GetBitmapPressed and SetBitmapPressed
+    BitmapPressed: 'Bitmap'  # See GetBitmapPressed and SetBitmapPressed
 
 
 
 RIGHT: int
 
 TOP: int
 
@@ -2971,15 +2995,15 @@
 
     def SetUseBestVisual(self, flag, forceTrueColour=False) -> None:
         """ Allows the programmer to specify whether the application will use the best visual on systems that support several visual on the same display.
 
             Source: https://docs.wxpython.org/wx.PyApp.html
         """
 
-    AssertMode: AppAssertMode  # See GetAssertMode and SetAssertMode
+    AssertMode: 'AppAssertMode'  # See GetAssertMode and SetAssertMode
     DisplayMode: 'VideoMode'  # See GetDisplayMode and SetDisplayMode
     ExitOnFrameDelete: bool  # See GetExitOnFrameDelete and SetExitOnFrameDelete
     LayoutDirection: int  # See GetLayoutDirection
     TopWindow: 'Window'  # See GetTopWindow and SetTopWindow
     UseBestVisual: bool  # See GetUseBestVisual and SetUseBestVisual
 
 
@@ -3196,14 +3220,16 @@
     ClassName: str  # See GetClassName and SetClassName
     Traits: 'AppTraits'  # See GetTraits
     VendorDisplayName: str  # See GetVendorDisplayName and SetVendorDisplayName
     VendorName: str  # See GetVendorName and SetVendorName
 
 
 
+_StandardPaths: TypeAlias = StandardPaths
+
 class AppTraits:
     """ The AppTraits class defines various configurable aspects of a App.
 
         Source: https://docs.wxpython.org/wx.AppTraits.html
     """
     def CreateConfig(self) -> 'ConfigBase':
         """ Called by wxWidgets to create the default configuration object for the application.
@@ -3269,15 +3295,15 @@
         """ Shows the assert dialog with the specified message in GUI mode or just prints the string to stderr in console mode.
 
             Source: https://docs.wxpython.org/wx.AppTraits.html
         """
 
     AssertStackTrace: str  # See GetAssertStackTrace
     DesktopEnvironment: str  # See GetDesktopEnvironment
-    StandardPaths: 'StandardPaths'  # See GetStandardPaths
+    StandardPaths: '_StandardPaths'  # See GetStandardPaths
     ToolkitVersion: tuple  # See GetToolkitVersion
 
 
 
 PORT_GTK: int
 
 class ArchiveFSHandler(FileSystemHandler):
@@ -3551,14 +3577,24 @@
             Source: https://docs.wxpython.org/wx.AutoBufferedPaintDC.html
         """
 
 
 
 BG_STYLE_PAINT: int
 
+_Brush: TypeAlias = Brush
+
+_Font: TypeAlias = Font
+
+_FontMetrics: TypeAlias = FontMetrics
+
+_GraphicsContext: TypeAlias = GraphicsContext
+
+_Pen: TypeAlias = Pen
+
 class DC(Object):
     """ A DC is a âdevice contextâ onto which graphics and text can be
 drawn.
 
         Source: https://docs.wxpython.org/wx.DC.html
     """
     def Blit(self, xdest, ydest, width, height, source, xsrc, ysrc, logicalFunc=COPY, useMask=False, xsrcMask=DefaultCoord, ysrcMask=DefaultCoord) -> bool:
@@ -3847,15 +3883,15 @@
 
     def GetBrush(self) -> 'Brush':
         """ Gets the current brush.
 
             Source: https://docs.wxpython.org/wx.DC.html
         """
 
-    def GetCGContext(self) -> 'UIntPtr':
+    def GetCGContext(self) -> int:
         """ wx.UIntPtr
 
             Source: https://docs.wxpython.org/wx.DC.html
         """
 
     def GetCharHeight(self) -> 'Coord':
         """ Gets the character height of the currently set font.
@@ -3907,15 +3943,15 @@
 
     def GetFontMetrics(self) -> 'FontMetrics':
         """ Returns the various font characteristics.
 
             Source: https://docs.wxpython.org/wx.DC.html
         """
 
-    def GetGdkDrawable(self) -> 'UIntPtr':
+    def GetGdkDrawable(self) -> int:
         """ wx.UIntPtr
 
             Source: https://docs.wxpython.org/wx.DC.html
         """
 
     def GetGraphicsContext(self) -> 'GraphicsContext':
         """ If supported by the platform and the  `   wx.DC `   implementation, this method will return the  `   wx.GraphicsContext `   associated with the DC.
@@ -3925,15 +3961,15 @@
 
     def GetHDC(self) -> int:
         """ long
 
             Source: https://docs.wxpython.org/wx.DC.html
         """
 
-    def GetHandle(self) -> 'UIntPtr':
+    def GetHandle(self) -> int:
         """ Returns a value that can be used as a handle to the native drawing context, if this   wx.DC  has something that could be thought of in that way.
 
             Source: https://docs.wxpython.org/wx.DC.html
         """
 
     def GetLayoutDirection(self) -> int:
         """ Gets the current layout direction of the device context.
@@ -4352,40 +4388,40 @@
             Source: https://docs.wxpython.org/wx.DC.html
         """
 
     AsBitmap: 'Bitmap'  # See GetAsBitmap
     Background: 'Brush'  # See GetBackground and SetBackground
     BackgroundMode: int  # See GetBackgroundMode and SetBackgroundMode
     BoundingBox: None  # See GetBoundingBox
-    Brush: 'Brush'  # See GetBrush and SetBrush
-    CGContext: 'UIntPtr'  # See GetCGContext
+    Brush: '_Brush'  # See GetBrush and SetBrush
+    CGContext: int  # See GetCGContext
     CharHeight: 'Coord'  # See GetCharHeight
     CharWidth: 'Coord'  # See GetCharWidth
     ClippingRect: None  # See GetClippingRect
     ContentScaleFactor: float  # See GetContentScaleFactor
     Depth: int  # See GetDepth
     DeviceOrigin: 'Point'  # See GetDeviceOrigin and SetDeviceOrigin
-    Font: 'Font'  # See GetFont and SetFont
-    FontMetrics: 'FontMetrics'  # See GetFontMetrics
-    GdkDrawable: 'UIntPtr'  # See GetGdkDrawable
-    GraphicsContext: 'GraphicsContext'  # See GetGraphicsContext and SetGraphicsContext
+    Font: '_Font'  # See GetFont and SetFont
+    FontMetrics: '_FontMetrics'  # See GetFontMetrics
+    GdkDrawable: int  # See GetGdkDrawable
+    GraphicsContext: '_GraphicsContext'  # See GetGraphicsContext and SetGraphicsContext
     HDC: int  # See GetHDC
-    Handle: 'UIntPtr'  # See GetHandle
+    Handle: int  # See GetHandle
     LayoutDirection: int  # See GetLayoutDirection and SetLayoutDirection
-    LogicalFunction: RasterOperationMode  # See GetLogicalFunction and SetLogicalFunction
-    MapMode: MappingMode  # See GetMapMode and SetMapMode
+    LogicalFunction: 'RasterOperationMode'  # See GetLogicalFunction and SetLogicalFunction
+    MapMode: 'MappingMode'  # See GetMapMode and SetMapMode
     MultiLineTextExtent: None  # See GetMultiLineTextExtent
     PPI: 'Size'  # See GetPPI
-    Pen: 'Pen'  # See GetPen and SetPen
+    Pen: '_Pen'  # See GetPen and SetPen
     Pixel: 'Colour'  # See GetPixel
-    Size: 'Size'  # See GetSize
+    Size: '_Size'  # See GetSize
     SizeMM: 'Size'  # See GetSizeMM
-    TextBackground: Union[int, str, 'Colour']  # See GetTextBackground and SetTextBackground
+    TextBackground: 'Colour'  # See GetTextBackground and SetTextBackground
     TextExtent: None  # See GetTextExtent
-    TextForeground: Union[int, str, 'Colour']  # See GetTextForeground and SetTextForeground
+    TextForeground: 'Colour'  # See GetTextForeground and SetTextForeground
     TransformMatrix: 'AffineMatrix2D'  # See GetTransformMatrix and SetTransformMatrix
 
 
 
 BLACK: int
 
 WHITE: int
@@ -4730,15 +4766,15 @@
     def SetData(self, format, buf) -> bool:
         """ bool
 
             Source: https://docs.wxpython.org/wx.BitmapDataObject.html
         """
 
     AllFormats: None  # See GetAllFormats
-    Bitmap: 'Bitmap'  # See GetBitmap and SetBitmap
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
 
 
 
 class DataObject:
     """ A DataObject represents data that can be copied to or from the
 clipboard, or dragged and dropped.
 
@@ -5182,14 +5218,16 @@
 
 EVT_NOTEBOOK_PAGE_CHANGED: int  # The page selection was changed. Processes a  wxEVT_NOTEBOOK_PAGE_CHANGED   event.
 
 EVT_NOTEBOOK_PAGE_CHANGING: int  # The page selection is about to be changed. Processes a  wxEVT_NOTEBOOK_PAGE_CHANGING   event. This event can be vetoed. ^^
 
 CLIP_CHILDREN: int
 
+_ListView: TypeAlias = ListView
+
 class Listbook(BookCtrlBase):
     """ Listbook is a class similar to Notebook but which uses a
 ListCtrl to show the labels instead of the tabs.
 
         Source: https://docs.wxpython.org/wx.Listbook.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -5213,15 +5251,15 @@
 
     def GetListView(self, *args, **kw) -> 'ListView':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.Listbook.html
         """
 
-    ListView: 'ListView'  # See GetListView
+    ListView: '_ListView'  # See GetListView
 
 
 
 LB_DEFAULT: int  # Choose the default location for the labels depending on the current platform (left everywhere except Mac where it is top).
 
 LB_TOP: int  # Place labels above the page area.
 
@@ -5280,14 +5318,16 @@
 
 CHB_BOTTOM: int  # Place labels below the page area. ^^
 
 EVT_CHOICEBOOK_PAGE_CHANGED: int  # The page selection was changed. Processes a  wxEVT_CHOICEBOOK_PAGE_CHANGED   event.
 
 EVT_CHOICEBOOK_PAGE_CHANGING: int  # The page selection is about to be changed. Processes a  wxEVT_CHOICEBOOK_PAGE_CHANGING   event. This event can be vetoed (using  wx.NotifyEvent.Veto ). ^^
 
+_TreeCtrl: TypeAlias = TreeCtrl
+
 class Treebook(BookCtrlBase):
     """ This class is an extension of the Notebook class that allows a tree
 structured set of pages to be shown in a control.
 
         Source: https://docs.wxpython.org/wx.Treebook.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -5372,15 +5412,15 @@
     def IsNodeExpanded(self, pageId: int) -> bool:
         """ Returns True if the page represented by pageId  is expanded.
 
             Source: https://docs.wxpython.org/wx.Treebook.html
         """
 
     Selection: int  # See GetSelection
-    TreeCtrl: 'TreeCtrl'  # See GetTreeCtrl
+    TreeCtrl: '_TreeCtrl'  # See GetTreeCtrl
 
 
 
 EVT_TREEBOOK_PAGE_CHANGED: int  # The page selection was changed. Processes a  wxEVT_TREEBOOK_PAGE_CHANGED   event.
 
 EVT_TREEBOOK_PAGE_CHANGING: int  # The page selection is about to be changed. Processes a  wxEVT_TREEBOOK_PAGE_CHANGING   event. This event can be  vetoed.
 
@@ -5431,14 +5471,16 @@
             Source: https://docs.wxpython.org/wx.BoxSizer.html
         """
 
     Orientation: int  # See GetOrientation and SetOrientation
 
 
 
+_Colour: TypeAlias = Colour
+
 class Brush(GDIObject):
     """ A brush is a drawing tool for filling in areas.
 
         Source: https://docs.wxpython.org/wx.Brush.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -5538,17 +5580,17 @@
 
     def __eq__(self, item: Any) -> bool:
         """ Equality operator.
 
             Source: https://docs.wxpython.org/wx.Brush.html
         """
 
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
     Stipple: 'Bitmap'  # See GetStipple and SetStipple
-    Style: BrushStyle  # See GetStyle and SetStyle
+    Style: 'BrushStyle'  # See GetStyle and SetStyle
 
 
 
 BRUSHSTYLE_TRANSPARENT: int
 
 class BrushList:
     """ A brush list is a list containing all brushes which have been created.
@@ -6075,15 +6117,15 @@
         """ int
 
             Source: https://docs.wxpython.org/wx.Caret.html
         """
 
     Position: None  # See GetPosition
     Size: None  # See GetSize and SetSize
-    Window: 'Window'  # See GetWindow
+    Window: '_Window'  # See GetWindow
 
 
 
 class CheckBox(Control):
     """ A checkbox is a labelled box which by default is either on (checkmark
 is visible) or off (no checkmark).
 
@@ -6442,15 +6484,15 @@
 
     def GetWindow(self) -> 'Window':
         """ Returns the direct child which receives the focus, or a (grand-)parent of the control receiving the focus.
 
             Source: https://docs.wxpython.org/wx.ChildFocusEvent.html
         """
 
-    Window: 'Window'  # See GetWindow
+    Window: '_Window'  # See GetWindow
 
 
 
 EVT_CHILD_FOCUS: int  # Process a  wxEVT_CHILD_FOCUS   event. ^^
 
 class Choice(Control,ItemContainer):
     """ A choice item is used to select one of a list of strings.
@@ -6604,27 +6646,29 @@
     BaseClassName1: 'Char'  # See GetBaseClassName1
     BaseClassName2: 'Char'  # See GetBaseClassName2
     ClassName: 'Char'  # See GetClassName
     Size: int  # See GetSize
 
 
 
+_ClientData: TypeAlias = ClientData
+
 class ClientDataContainer:
     """ This class is a mixin that provides storage and management of âclient
 dataâ.
 
         Source: https://docs.wxpython.org/wx.ClientDataContainer.html
     """
     def __init__(self) -> None:
         """ Default constructor.
 
             Source: https://docs.wxpython.org/wx.ClientDataContainer.html
         """
 
-    def GetClientData(self) -> ClientData:
+    def GetClientData(self) -> 'ClientData':
         """ Get a pointer to the client data object.
 
             Source: https://docs.wxpython.org/wx.ClientDataContainer.html
         """
 
     def GetClientObject(self) -> Any:
         """ Alias for GetClientData
@@ -6640,15 +6684,15 @@
 
     def SetClientObject(self, data) -> Any:
         """ Alias for SetClientData
 
             Source: https://docs.wxpython.org/wx.ClientDataContainer.html
         """
 
-    ClientData: ClientData  # See GetClientData and SetClientData
+    ClientData: '_ClientData'  # See GetClientData and SetClientData
 
 
 
 class ClientDC(WindowDC):
     """ ClientDC is primarily useful for obtaining information about the
 window from outside EVT_PAINT() handler.
 
@@ -7315,27 +7359,27 @@
 
     def GetLuminance(self) -> float:
         """ Return the perceived brightness of the colour.
 
             Source: https://docs.wxpython.org/wx.Colour.html
         """
 
-    def GetPixel(self) -> 'IntPtr':
+    def GetPixel(self) -> int:
         """ wx.IntPtr
 
             Source: https://docs.wxpython.org/wx.Colour.html
         """
 
-    def GetRGB(self) -> 'int':
+    def GetRGB(self) -> int:
         """ Gets the RGB or RGBA colour values as a single 32 bit value.
 
             Source: https://docs.wxpython.org/wx.Colour.html
         """
 
-    def GetRGBA(self) -> 'int':
+    def GetRGBA(self) -> int:
         """ Gets the RGB or RGBA colour values as a single 32 bit value.
 
             Source: https://docs.wxpython.org/wx.Colour.html
         """
 
     def GetRed(self) -> int:
         """ Returns the red intensity as  int.
@@ -7467,17 +7511,17 @@
 
     def __eq__(self, item: Any) -> bool:
         """ Tests the equality of two colours by comparing individual red, green, blue intensities and alpha values.
 
             Source: https://docs.wxpython.org/wx.Colour.html
         """
 
-    Pixel: 'IntPtr'  # See GetPixel
-    RGB: 'int'  # See GetRGB and SetRGB
-    RGBA: 'int'  # See GetRGBA and SetRGBA
+    Pixel: int  # See GetPixel
+    RGB: int  # See GetRGB and SetRGB
+    RGBA: int  # See GetRGBA and SetRGBA
     alpha: Any  # See Alpha
     blue: Any  # See Blue
     green: Any  # See Green
     red: Any  # See Red
 
 
 
@@ -7550,15 +7594,15 @@
         """ Converts the colours saved in this class in a string form, separating the various colours with a comma.
 
             Source: https://docs.wxpython.org/wx.ColourData.html
         """
 
     ChooseAlpha: bool  # See GetChooseAlpha and SetChooseAlpha
     ChooseFull: bool  # See GetChooseFull and SetChooseFull
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
 
 
 
 class ColourDatabase:
     """ wxWidgets maintains a database of standard RGB colours for a
 predefined set of named colours.
 
@@ -7592,14 +7636,16 @@
         """ Finds a colour name given the colour.
 
             Source: https://docs.wxpython.org/wx.ColourDatabase.html
         """
 
 
 
+_ColourData: TypeAlias = ColourData
+
 class ColourDialog(Dialog):
     """ This class represents the colour chooser dialog.
 
         Source: https://docs.wxpython.org/wx.ColourDialog.html
     """
     def __init__(self, parent, data=None) -> None:
         """ Constructor.
@@ -7628,15 +7674,15 @@
 
     def ShowModal(self) -> int:
         """ Shows the dialog, returning wx.ID_OK if the user pressed wx.OK, and wx.ID_CANCEL otherwise.
 
             Source: https://docs.wxpython.org/wx.ColourDialog.html
         """
 
-    ColourData: 'ColourData'  # See GetColourData
+    ColourData: '_ColourData'  # See GetColourData
 
 
 
 class ColourDialogEvent(CommandEvent):
     """ This event class is used for the events generated by ColourDialog.
 
         Source: https://docs.wxpython.org/wx.ColourDialogEvent.html
@@ -7655,15 +7701,15 @@
 
     def SetColour(self, colour: Union[int, str, 'Colour']) -> None:
         """ Set the colour to be sent with the event.
 
             Source: https://docs.wxpython.org/wx.ColourDialogEvent.html
         """
 
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
 
 
 
 EVT_COLOUR_CHANGED: int  # Generated whenever the currently selected colour in the dialog changes. This event is currently only implemented in wxMSW. ^^
 
 class ColourPickerCtrl(PickerBase):
     """ This control allows the user to select a colour.
@@ -7697,15 +7743,15 @@
 
     def SetColour(self, *args, **kw) -> None:
         """ Sets the currently selected colour.
 
             Source: https://docs.wxpython.org/wx.ColourPickerCtrl.html
         """
 
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
 
 
 
 CLRP_DEFAULT_STYLE: int  # The default style: 0.
 
 CLRP_USE_TEXTCTRL: int  # Creates a text control to the left of the picker button which is completely managed by the   wx.ColourPickerCtrl  and which can be used by the user to specify a colour (see SetColour). The text control is automatically synchronized with buttonâs value. Use functions defined in   wx.PickerBase  to modify the text control.
 
@@ -7739,15 +7785,15 @@
 
     def SetColour(self, pos: Union[int, str, 'Colour']) -> None:
         """ Set the colour associated with the event.
 
             Source: https://docs.wxpython.org/wx.ColourPickerEvent.html
         """
 
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
 
 
 
 class ComboBox(Control,ItemContainer,TextEntry):
     """ A combobox is like a combination of an edit control and a listbox.
 
         Source: https://docs.wxpython.org/wx.ComboBox.html
@@ -7881,14 +7927,16 @@
 
 EVT_COMBOBOX: int  # Process a  wxEVT_COMBOBOX   event, when an item on the list is selected. Note that calling  GetValue  returns the new value of selection.
 
 EVT_COMBOBOX_DROPDOWN: int  # Process a  wxEVT_COMBOBOX_DROPDOWN   event, which is generated when the list box part of the combo box is shown (drops down). Notice that this event is only supported by wxMSW, wxGTK with GTK+ 2.10 or later, and OSX/Cocoa.
 
 EVT_COMBOBOX_CLOSEUP: int  # Process a  wxEVT_COMBOBOX_CLOSEUP   event, which is generated when the list box of the combo box disappears (closes up). This event is only generated for the same platforms as   wxEVT_COMBOBOX_DROPDOWN   above. ^^
 
+_TextCtrl: TypeAlias = TextCtrl
+
 class ComboCtrl(Control,TextEntry):
     """ A combo control is a generic combobox that allows totally custom
 popup.
 
         Source: https://docs.wxpython.org/wx.ComboCtrl.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -8249,15 +8297,15 @@
     CustomPaintWidth: int  # See GetCustomPaintWidth and SetCustomPaintWidth
     Hint: str  # See GetHint and SetHint
     InsertionPoint: int  # See GetInsertionPoint and SetInsertionPoint
     LastPosition: int  # See GetLastPosition
     Margins: 'Point'  # See GetMargins and SetMargins
     PopupControl: 'ComboPopup'  # See GetPopupControl and SetPopupControl
     PopupWindow: 'Window'  # See GetPopupWindow
-    TextCtrl: 'TextCtrl'  # See GetTextCtrl
+    TextCtrl: '_TextCtrl'  # See GetTextCtrl
     TextRect: 'Rect'  # See GetTextRect
     Value: str  # See GetValue and SetValue
 
 
 
 CC_SPECIAL_DCLICK: int  # Double-clicking triggers a call to popupâs OnComboDoubleClick. Actual behaviour is defined by a derived class. For instance,   wx.adv.OwnerDrawnComboBox  will cycle an item. This style only applies if wx.CB_READONLY is used as well.
 
@@ -8272,14 +8320,16 @@
 class ComboCtrlFeatures:
     """ Features enabled for ComboCtrl.
 
         Source: https://docs.wxpython.org/wx.ComboCtrlFeatures.html
     """
 
 
+_ComboCtrl: TypeAlias = ComboCtrl
+
 class ComboPopup:
     """ In order to use a custom popup with ComboCtrl, an interface class
 must be derived from ComboPopup.
 
         Source: https://docs.wxpython.org/wx.ComboPopup.html
     """
     def __init__(self) -> None:
@@ -8386,15 +8436,15 @@
 
     def SetStringValue(self, value: str) -> None:
         """ The derived class must implement this to receive string value changes from   wx.ComboCtrl.
 
             Source: https://docs.wxpython.org/wx.ComboPopup.html
         """
 
-    ComboCtrl: 'ComboCtrl'  # See GetComboCtrl
+    ComboCtrl: '_ComboCtrl'  # See GetComboCtrl
     Control: 'Window'  # See GetControl
     StringValue: str  # See GetStringValue and SetStringValue
 
 
 
 class Command(Object):
     """ Command is a base class for modelling an application command, which
@@ -8446,15 +8496,15 @@
     """
     def __init__(self, commandEventType=wxEVT_NULL, id=0) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.CommandEvent.html
         """
 
-    def GetClientData(self) -> ClientData:
+    def GetClientData(self) -> 'ClientData':
         """ Returns client object pointer for a listbox or choice selection event (not valid for a deselection).
 
             Source: https://docs.wxpython.org/wx.CommandEvent.html
         """
 
     def GetClientObject(self) -> Any:
         """ Alias for GetClientData
@@ -8524,15 +8574,15 @@
 
     def SetString(self, string: str) -> None:
         """ Sets the m_commandString  member.
 
             Source: https://docs.wxpython.org/wx.CommandEvent.html
         """
 
-    ClientData: ClientData  # See GetClientData and SetClientData
+    ClientData: '_ClientData'  # See GetClientData and SetClientData
     ExtraLong: int  # See GetExtraLong and SetExtraLong
     Int: int  # See GetInt and SetInt
     Selection: int  # See GetSelection
     String: str  # See GetString and SetString
 
 
 
@@ -8602,15 +8652,15 @@
 
     def ClearCommands(self) -> None:
         """ Deletes all commands in the list and sets the current command pointer to None.
 
             Source: https://docs.wxpython.org/wx.CommandProcessor.html
         """
 
-    def GetCommands(self) -> CommandList:
+    def GetCommands(self) -> 'CommandList':
         """ Returns the list of commands.
 
             Source: https://docs.wxpython.org/wx.CommandProcessor.html
         """
 
     def GetCurrentCommand(self) -> 'Command':
         """ Returns the current command.
@@ -8716,15 +8766,15 @@
 
     def Undo(self) -> bool:
         """ Undoes the last command executed.
 
             Source: https://docs.wxpython.org/wx.CommandProcessor.html
         """
 
-    Commands: CommandList  # See GetCommands
+    Commands: 'CommandList'  # See GetCommands
     CurrentCommand: 'Command'  # See GetCurrentCommand
     EditMenu: 'Menu'  # See GetEditMenu and SetEditMenu
     MaxCommands: int  # See GetMaxCommands
     RedoAccelerator: str  # See GetRedoAccelerator and SetRedoAccelerator
     RedoMenuLabel: str  # See GetRedoMenuLabel
     UndoAccelerator: str  # See GetUndoAccelerator and SetUndoAccelerator
     UndoMenuLabel: str  # See GetUndoMenuLabel
@@ -8909,15 +8959,15 @@
 
     def ReadLong(self, key, defaultVal) -> int:
         """ Reads a long value from the key and returns it.
 
             Source: https://docs.wxpython.org/wx.ConfigBase.html
         """
 
-    def ReadLongLong(self, key, defaultVal) -> LongLong_t:
+    def ReadLongLong(self, key, defaultVal) -> 'LongLong_t':
         """ Reads a 64-bit long long value from the key and returns it.
 
             Source: https://docs.wxpython.org/wx.ConfigBase.html
         """
 
     def RenameEntry(self, oldName, newName) -> bool:
         """ Renames an entry in the current group.
@@ -9105,17 +9155,37 @@
 
     def SetPosition(self, point: Union[tuple[int, int], 'Point']) -> None:
         """ Sets the position at which the menu should be shown.
 
             Source: https://docs.wxpython.org/wx.ContextMenuEvent.html
         """
 
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
+    Position: 'Point'  # See GetPosition and SetPosition
+
+
+
+_AcceleratorTable: TypeAlias = AcceleratorTable
+
+_BackgroundStyle: TypeAlias = BackgroundStyle
+
+_Border: TypeAlias = Border
 
+_Caret: TypeAlias = Caret
 
+_Cursor: TypeAlias = Cursor
+
+_DropTarget: TypeAlias = DropTarget
+
+_Rect: TypeAlias = Rect
+
+_Sizer: TypeAlias = Sizer
+
+_ToolTip: TypeAlias = ToolTip
+
+_Validator: TypeAlias = Validator
 
 class Window(EvtHandler):
     """ Window is the base class for all windows and represents any visible
 object on screen.
 
         Source: https://docs.wxpython.org/wx.Window.html
     """
@@ -9510,15 +9580,15 @@
 
     def GetCharWidth(self) -> int:
         """ Returns the average character width for this window.
 
             Source: https://docs.wxpython.org/wx.Window.html
         """
 
-    def GetChildren(self) -> WindowList:
+    def GetChildren(self) -> 'WindowList':
         """ Returns a reference to the list of the windowâs children.
 
             Source: https://docs.wxpython.org/wx.Window.html
         """
 
     @staticmethod
     def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
@@ -10750,69 +10820,69 @@
     def __nonzero__(self) -> None:
         """ Can be used to test if the C++ part of the window still exists, with
 code like this:
 
             Source: https://docs.wxpython.org/wx.Window.html
         """
 
-    AcceleratorTable: 'AcceleratorTable'  # See GetAcceleratorTable and SetAcceleratorTable
+    AcceleratorTable: '_AcceleratorTable'  # See GetAcceleratorTable and SetAcceleratorTable
     AutoLayout: bool  # See GetAutoLayout and SetAutoLayout
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
-    BackgroundStyle: BackgroundStyle  # See GetBackgroundStyle and SetBackgroundStyle
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
+    BackgroundStyle: '_BackgroundStyle'  # See GetBackgroundStyle and SetBackgroundStyle
     BestSize: 'Size'  # See GetBestSize
     BestVirtualSize: 'Size'  # See GetBestVirtualSize
-    Border: 'Border'  # See GetBorder
-    Caret: 'Caret'  # See GetCaret and SetCaret
+    Border: '_Border'  # See GetBorder
+    Caret: '_Caret'  # See GetCaret and SetCaret
     CharHeight: int  # See GetCharHeight
     CharWidth: int  # See GetCharWidth
-    Children: WindowList  # See GetChildren
+    Children: 'WindowList'  # See GetChildren
     ClientAreaOrigin: 'Point'  # See GetClientAreaOrigin
     ClientRect: 'Rect'  # See GetClientRect and SetClientRect
     ClientSize: None  # See GetClientSize and SetClientSize
     Constraints: 'LayoutConstraints'  # See GetConstraints and SetConstraints
     ContainingSizer: 'Sizer'  # See GetContainingSizer and SetContainingSizer
-    Cursor: 'Cursor'  # See GetCursor and SetCursor
+    Cursor: '_Cursor'  # See GetCursor and SetCursor
     DefaultAttributes: 'VisualAttributes'  # See GetDefaultAttributes
-    DropTarget: 'DropTarget'  # See GetDropTarget and SetDropTarget
+    DropTarget: '_DropTarget'  # See GetDropTarget and SetDropTarget
     EffectiveMinSize: 'Size'  # See GetEffectiveMinSize
     Enabled: Any  # See IsEnabled and Enable
     EventHandler: 'EvtHandler'  # See GetEventHandler and SetEventHandler
     ExtraStyle: int  # See GetExtraStyle and SetExtraStyle
-    Font: 'Font'  # See GetFont and SetFont
-    ForegroundColour: Union[int, str, 'Colour']  # See GetForegroundColour and SetForegroundColour
+    Font: '_Font'  # See GetFont and SetFont
+    ForegroundColour: 'Colour'  # See GetForegroundColour and SetForegroundColour
     GrandParent: 'Window'  # See GetGrandParent
     Handle: None  # See GetHandle
     HelpText: str  # See GetHelpText and SetHelpText
     Id: int  # See GetId and SetId
     Label: str  # See GetLabel and SetLabel
     LayoutDirection: int  # See GetLayoutDirection and SetLayoutDirection
-    MaxClientSize: Union[tuple[int, int], 'Size']  # See GetMaxClientSize and SetMaxClientSize
+    MaxClientSize: 'Size'  # See GetMaxClientSize and SetMaxClientSize
     MaxHeight: int  # See GetMaxHeight
-    MaxSize: Union[tuple[int, int], 'Size']  # See GetMaxSize and SetMaxSize
+    MaxSize: 'Size'  # See GetMaxSize and SetMaxSize
     MaxWidth: int  # See GetMaxWidth
-    MinClientSize: Union[tuple[int, int], 'Size']  # See GetMinClientSize and SetMinClientSize
+    MinClientSize: 'Size'  # See GetMinClientSize and SetMinClientSize
     MinHeight: int  # See GetMinHeight
-    MinSize: Union[tuple[int, int], 'Size']  # See GetMinSize and SetMinSize
+    MinSize: 'Size'  # See GetMinSize and SetMinSize
     MinWidth: int  # See GetMinWidth
     Name: str  # See GetName and SetName
     Parent: 'Window'  # See GetParent
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
-    Rect: 'Rect'  # See GetRect and SetRect
+    Position: 'Point'  # See GetPosition and SetPosition
+    Rect: '_Rect'  # See GetRect and SetRect
     ScreenPosition: 'Point'  # See GetScreenPosition
     ScreenRect: 'Rect'  # See GetScreenRect
     Shown: Any  # See IsShown and Show
-    Size: 'Size'  # See GetSize and SetSize
-    Sizer: 'Sizer'  # See GetSizer and SetSizer
+    Size: '_Size'  # See GetSize and SetSize
+    Sizer: '_Sizer'  # See GetSizer and SetSizer
     ThemeEnabled: bool  # See GetThemeEnabled and SetThemeEnabled
-    ToolTip: str  # See GetToolTip and SetToolTip
+    ToolTip: '_ToolTip'  # See GetToolTip and SetToolTip
     TopLevel: Any  # See IsTopLevel
     TopLevelParent: 'Window'  # See GetTopLevelParent
     UpdateClientRect: 'Rect'  # See GetUpdateClientRect
     UpdateRegion: 'Region'  # See GetUpdateRegion
-    Validator: 'Validator'  # See GetValidator and SetValidator
+    Validator: '_Validator'  # See GetValidator and SetValidator
     VirtualSize: 'Size'  # See GetVirtualSize and SetVirtualSize
     WindowStyle: int  # See GetWindowStyle and SetWindowStyle
     WindowStyleFlag: int  # See GetWindowStyleFlag and SetWindowStyleFlag
     WindowVariant: int  # See GetWindowVariant and SetWindowVariant
 
 
 
@@ -11045,21 +11115,21 @@
 
     def Delete(self, n: int) -> None:
         """ Deletes an item from the control.
 
             Source: https://docs.wxpython.org/wx.ItemContainer.html
         """
 
-    def DetachClientObject(self, n: int) -> ClientData:
+    def DetachClientObject(self, n: int) -> 'ClientData':
         """ Returns the client object associated with the given item and transfers its ownership to the caller.
 
             Source: https://docs.wxpython.org/wx.ItemContainer.html
         """
 
-    def GetClientData(self, n: int) -> ClientData:
+    def GetClientData(self, n: int) -> 'ClientData':
         """ Returns a pointer to the client data associated with the given item (if any).
 
             Source: https://docs.wxpython.org/wx.ItemContainer.html
         """
 
     def GetClientObject(self, n) -> Any:
         """ Alias for GetClientData
@@ -11331,15 +11401,15 @@
     def __eq__(self, item: Any) -> bool:
         """ Returns True if the formats are equal.
 
             Source: https://docs.wxpython.org/wx.DataFormat.html
         """
 
     Id: str  # See GetId and SetId
-    Type: DataFormatId  # See GetType and SetType
+    Type: 'DataFormatId'  # See GetType and SetType
 
 
 
 DF_INVALID: int
 
 DF_TEXT: int
 
@@ -11716,21 +11786,21 @@
 
     def GetDateOnly(self) -> 'DateTime':
         """ Returns the object having the same date component as this one but time of 00:00:00.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetDay(self, tz: 'DateTime.TimeZone'=Local) -> intshort:
+    def GetDay(self, tz: 'DateTime.TimeZone'=Local) -> 'intshort':
         """ Returns the day in the given timezone (local one by default).
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetDayOfYear(self, tz: 'DateTime.TimeZone'=Local) -> intshort:
+    def GetDayOfYear(self, tz: 'DateTime.TimeZone'=Local) -> 'intshort':
         """ Returns the day of the year (in 1-366 range) in the given timezone (local one by default).
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     @staticmethod
     def GetEndDST(year=Inv_Year, country=Country_Default) -> 'DateTime':
@@ -11756,15 +11826,15 @@
     @staticmethod
     def GetFirstWeekDay(firstDay: WeekDay) -> bool:
         """ Acquires the first weekday of a week based on locale and/or OS settings.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetHour(self, tz: 'DateTime.TimeZone'=Local) -> intshort:
+    def GetHour(self, tz: 'DateTime.TimeZone'=Local) -> 'intshort':
         """ Returns the hour in the given timezone (local one by default).
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     def GetJDN(self) -> float:
         """ Synonym for GetJulianDayNumber .
@@ -11792,21 +11862,21 @@
 
     def GetMJD(self) -> float:
         """ Synonym for GetModifiedJulianDayNumber .
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetMillisecond(self, tz: 'DateTime.TimeZone'=Local) -> intshort:
+    def GetMillisecond(self, tz: 'DateTime.TimeZone'=Local) -> 'intshort':
         """ Returns the milliseconds in the given timezone (local one by default).
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetMinute(self, tz: 'DateTime.TimeZone'=Local) -> intshort:
+    def GetMinute(self, tz: 'DateTime.TimeZone'=Local) -> 'intshort':
         """ Returns the minute in the given timezone (local one by default).
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     def GetModifiedJulianDayNumber(self) -> float:
         """ Returns the âModified Julian Day Numberâ  (MJD) which is, by definition, is equal to JDN - 2400000.5.
@@ -11830,15 +11900,15 @@
     def GetNextWeekDay(self, weekday: DateTime.WeekDay) -> 'DateTime':
         """ Returns the copy of this object to which SetToNextWeekDay   was applied.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     @staticmethod
-    def GetNumberOfDays(month, year=Inv_Year, cal=Gregorian) -> intshort:
+    def GetNumberOfDays(month, year=Inv_Year, cal=Gregorian) -> 'intshort':
         """ Returns the number of days in the given month of the given year.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     def GetPrevWeekDay(self, weekday: DateTime.WeekDay) -> 'DateTime':
         """ Returns the copy of this object to which SetToPrevWeekDay   was applied.
@@ -11848,15 +11918,15 @@
 
     def GetRataDie(self) -> float:
         """ Return the Rata  Die number of this date.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetSecond(self, tz: 'DateTime.TimeZone'=Local) -> intshort:
+    def GetSecond(self, tz: 'DateTime.TimeZone'=Local) -> 'intshort':
         """ Returns the seconds in the given timezone (local one by default).
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     def GetTicks(self) -> int:
         """ Returns the number of seconds since Jan 1, 1970 UTC.
@@ -11885,15 +11955,15 @@
 
     def GetWeekBasedYear(self, tz: 'DateTime.TimeZone') -> int:
         """ Returns the year to which the week containing this date belongs.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetWeekDay(self, *args, **kw) -> 'DateTime.WeekDay':
+    def GetWeekDay(self, *args, **kw) -> 'WeekDay':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     def GetWeekDayInSameWeek(self, weekday, flags=Monday_First) -> 'DateTime':
         """ Returns the copy of this object to which SetToWeekDayInSameWeek   was applied.
@@ -11904,21 +11974,21 @@
     @staticmethod
     def GetWeekDayName(weekday, flags=Name_Full) -> str:
         """ Gets the full (default) or abbreviated name of the given week day.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetWeekOfMonth(self, flags=Monday_First, tz=Local) -> intshort:
+    def GetWeekOfMonth(self, flags=Monday_First, tz=Local) -> 'intshort':
         """ Returns the ordinal number of the week in the month (in 1-5 range).
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    def GetWeekOfYear(self, flags=Monday_First, tz=Local) -> intshort:
+    def GetWeekOfYear(self, flags=Monday_First, tz=Local) -> 'intshort':
         """ Returns the number of the week of the year this date is in.
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
     def GetYear(self, tz: 'DateTime.TimeZone'=Local) -> int:
         """ Returns the year in the given timezone (local one by default).
@@ -12278,24 +12348,24 @@
 
     def __str__(self) -> None:
         """ 
 
             Source: https://docs.wxpython.org/wx.DateTime.html
         """
 
-    DayOfYear: intshort  # See GetDayOfYear
+    DayOfYear: 'intshort'  # See GetDayOfYear
     JDN: float  # See GetJDN and SetJDN
     JulianDayNumber: float  # See GetJulianDayNumber
     LastMonthDay: 'DateTime'  # See GetLastMonthDay
     MJD: float  # See GetMJD
     ModifiedJulianDayNumber: float  # See GetModifiedJulianDayNumber
     RataDie: float  # See GetRataDie
     Ticks: int  # See GetTicks
-    WeekOfMonth: intshort  # See GetWeekOfMonth
-    WeekOfYear: intshort  # See GetWeekOfYear
+    WeekOfMonth: 'intshort'  # See GetWeekOfMonth
+    WeekOfYear: 'intshort'  # See GetWeekOfYear
     day: Any  # See GetDay and SetDay
     hour: Any  # See GetHour and SetHour
     millisecond: Any  # See GetMillisecond and SetMillisecond
     minute: Any  # See GetMinute and SetMinute
     month: Any  # See GetMonth and SetMonth
     second: Any  # See GetSecond and SetSecond
     year: Any  # See GetYear and SetYear
@@ -13135,15 +13205,15 @@
         """
 
     AffirmativeId: int  # See GetAffirmativeId and SetAffirmativeId
     ContentWindow: 'Window'  # See GetContentWindow
     EscapeId: int  # See GetEscapeId and SetEscapeId
     LayoutAdaptationDone: bool  # See GetLayoutAdaptationDone and SetLayoutAdaptationDone
     LayoutAdaptationLevel: int  # See GetLayoutAdaptationLevel and SetLayoutAdaptationLevel
-    LayoutAdaptationMode: DialogLayoutAdaptationMode  # See GetLayoutAdaptationMode and SetLayoutAdaptationMode
+    LayoutAdaptationMode: 'DialogLayoutAdaptationMode'  # See GetLayoutAdaptationMode and SetLayoutAdaptationMode
     MainButtonIds: list[int]  # See GetMainButtonIds
     ReturnCode: int  # See GetReturnCode and SetReturnCode
 
 
 
 CAPTION: int  # Puts a caption on the dialog box.
 
@@ -13422,15 +13492,15 @@
 
     def GetGeometry(self) -> 'Rect':
         """ Returns the bounding rectangle of the display whose index was passed to the constructor.
 
             Source: https://docs.wxpython.org/wx.Display.html
         """
 
-    def GetModes(self, mode: 'VideoMode'=DefaultVideoMode) -> ArrayVideoModes:
+    def GetModes(self, mode: 'VideoMode'=DefaultVideoMode) -> 'ArrayVideoModes':
         """ Fills and returns an array with all the video modes that are supported by this display, or video modes that are supported by this display and match the mode parameter (if mode is not DefaultVideoMode).
 
             Source: https://docs.wxpython.org/wx.Display.html
         """
 
     def GetName(self) -> str:
         """ Returns the displayâs name.
@@ -13612,14 +13682,16 @@
 
     Files: Any  # See GetFiles
     NumberOfFiles: int  # See GetNumberOfFiles
     Position: 'Point'  # See GetPosition
 
 
 
+_DataObject: TypeAlias = DataObject
+
 class DropSource:
     """ This class represents a source for a drag and drop operation.
 
         Source: https://docs.wxpython.org/wx.DropSource.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -13659,15 +13731,15 @@
 
     def SetIcon(self, res, icon) -> None:
         """ Set the icon to use for a certain drag result.
 
             Source: https://docs.wxpython.org/wx.DropSource.html
         """
 
-    DataObject: 'DataObject'  # See GetDataObject
+    DataObject: '_DataObject'  # See GetDataObject
 
 
 
 class DropTarget:
     """ This class represents a target for a drag and drop operation.
 
         Source: https://docs.wxpython.org/wx.DropTarget.html
@@ -13735,19 +13807,21 @@
     def SetDefaultAction(self, action: DragResult) -> None:
         """ Sets the default action for drag and drop.
 
             Source: https://docs.wxpython.org/wx.DropTarget.html
         """
 
     Data: bool  # See GetData
-    DataObject: 'DataObject'  # See GetDataObject and SetDataObject
-    DefaultAction: DragResult  # See GetDefaultAction and SetDefaultAction
+    DataObject: '_DataObject'  # See GetDataObject and SetDataObject
+    DefaultAction: 'DragResult'  # See GetDefaultAction and SetDefaultAction
 
 
 
+_DC: TypeAlias = DC
+
 class EraseEvent(Event):
     """ An erase event is sent when a windowâs background needs to be
 repainted.
 
         Source: https://docs.wxpython.org/wx.EraseEvent.html
     """
     def __init__(self, id=0, dc=None) -> None:
@@ -13758,15 +13832,15 @@
 
     def GetDC(self) -> 'DC':
         """ Returns the device context associated with the erase event to draw on.
 
             Source: https://docs.wxpython.org/wx.EraseEvent.html
         """
 
-    DC: 'DC'  # See GetDC
+    DC: '_DC'  # See GetDC
 
 
 
 class Event(Object):
     """ An event is a structure holding information about an event passed to a
 callback or member function.
 
@@ -13870,15 +13944,15 @@
 
     def StopPropagation(self) -> int:
         """ Stop the event from propagating to its parent window.
 
             Source: https://docs.wxpython.org/wx.Event.html
         """
 
-    EventObject: 'Object'  # See GetEventObject and SetEventObject
+    EventObject: 'Window'  # See GetEventObject and SetEventObject
     EventType: int  # See GetEventType and SetEventType
     Id: int  # See GetId and SetId
     Skipped: bool  # See GetSkipped
     Timestamp: int  # See GetTimestamp and SetTimestamp
 
 
 
@@ -15137,15 +15211,15 @@
 
     def GetMenuPathStyle(self) -> 'FileHistoryMenuPathStyle':
         """ Get the current style of the menu item labels.
 
             Source: https://docs.wxpython.org/wx.FileHistory.html
         """
 
-    def GetMenus(self) -> FileHistoryMenuList:
+    def GetMenus(self) -> 'FileHistoryMenuList':
         """ Returns the list of menus that are managed by this file history object.
 
             Source: https://docs.wxpython.org/wx.FileHistory.html
         """
 
     def Load(self, config: 'ConfigBase') -> None:
         """ Loads the file history from the given config object.
@@ -15188,16 +15262,16 @@
 
             Source: https://docs.wxpython.org/wx.FileHistory.html
         """
 
     BaseId: int  # See GetBaseId and SetBaseId
     Count: int  # See GetCount
     MaxFiles: int  # See GetMaxFiles
-    MenuPathStyle: FileHistoryMenuPathStyle  # See GetMenuPathStyle and SetMenuPathStyle
-    Menus: FileHistoryMenuList  # See GetMenus
+    MenuPathStyle: 'FileHistoryMenuPathStyle'  # See GetMenuPathStyle and SetMenuPathStyle
+    Menus: 'FileHistoryMenuList'  # See GetMenus
 
 
 
 class FileSystem(Object):
     """ This class provides an interface for opening files on different file
 systems.
 
@@ -15519,22 +15593,26 @@
 
     def GetAvailableTranslations(self, domain: str) -> list[str]:
         """ Implements wx.Translations.GetAvailableTranslations .
 
             Source: https://docs.wxpython.org/wx.TranslationsLoader.html
         """
 
-    def LoadCatalog(self, domain, lang) -> MsgCatalog:
+    def LoadCatalog(self, domain, lang) -> 'MsgCatalog':
         """ Called to load requested catalog.
 
             Source: https://docs.wxpython.org/wx.TranslationsLoader.html
         """
 
 
 
+_Icon: TypeAlias = Icon
+
+_IconLocation: TypeAlias = IconLocation
+
 class FileType:
     """ This class holds information about a given file type.
 
         Source: https://docs.wxpython.org/wx.FileType.html
     """
     def __init__(self, ftInfo: 'FileTypeInfo') -> None:
         """ Copy constructor.
@@ -15622,17 +15700,17 @@
 the MessageParameters class.
 
             Source: https://docs.wxpython.org/wx.FileType.html
         """
 
     Description: str  # See GetDescription
     Extensions: list[str]  # See GetExtensions
-    Icon: 'Icon'  # See GetIcon
+    Icon: '_Icon'  # See GetIcon
     IconInfo: Any  # See GetIconInfo
-    IconLocation: 'IconLocation'  # See GetIconLocation
+    IconLocation: '_IconLocation'  # See GetIconLocation
     MimeType: str  # See GetMimeType
     MimeTypes: list[str]  # See GetMimeTypes
     OpenCommand: str  # See GetOpenCommand
     PrintCommand: str  # See GetPrintCommand
 
 
 
@@ -15894,15 +15972,15 @@
     def SetReplaceString(self, str: str) -> None:
         """ Set the replacement string (used as initial value by the dialog).
 
             Source: https://docs.wxpython.org/wx.FindReplaceData.html
         """
 
     FindString: str  # See GetFindString and SetFindString
-    Flags: 'int'  # See GetFlags and SetFlags
+    Flags: int  # See GetFlags and SetFlags
     ReplaceString: str  # See GetReplaceString and SetReplaceString
 
 
 
 class FlexGridSizer(GridSizer):
     """ A flex grid sizer is a sizer which lays out its children in a two-
 dimensional table with all table fields in one row having the same
@@ -16000,15 +16078,15 @@
         """ Specifies how the sizer should grow in the non-flexible direction if there is one (so SetFlexibleDirection   must have been called previously).
 
             Source: https://docs.wxpython.org/wx.FlexGridSizer.html
         """
 
     ColWidths: list[int]  # See GetColWidths
     FlexibleDirection: int  # See GetFlexibleDirection and SetFlexibleDirection
-    NonFlexibleGrowMode: FlexSizerGrowMode  # See GetNonFlexibleGrowMode and SetNonFlexibleGrowMode
+    NonFlexibleGrowMode: 'FlexSizerGrowMode'  # See GetNonFlexibleGrowMode and SetNonFlexibleGrowMode
     RowHeights: list[int]  # See GetRowHeights
 
 
 
 FLEX_GROWMODE_NONE: int
 
 FLEX_GROWMODE_SPECIFIED: int
@@ -16135,15 +16213,15 @@
 
     def SetWindow(self, win: 'Window') -> None:
         """ win (wx.Window) â
 
             Source: https://docs.wxpython.org/wx.FocusEvent.html
         """
 
-    Window: 'Window'  # See GetWindow and SetWindow
+    Window: '_Window'  # See GetWindow and SetWindow
 
 
 
 class Font(GDIObject):
     """ A font is an object which determines the appearance of text.
 
         Source: https://docs.wxpython.org/wx.Font.html
@@ -16521,15 +16599,15 @@
         """
 
     Encoding: int  # See GetEncoding and SetEncoding
     FaceName: str  # See GetFaceName and SetFaceName
     Family: int  # See GetFamily and SetFamily
     NativeFontInfoDesc: str  # See GetNativeFontInfoDesc and SetNativeFontInfo
     NativeFontInfoUserDesc: str  # See GetNativeFontInfoUserDesc and SetNativeFontInfoUserDesc
-    PixelSize: Union[tuple[int, int], 'Size']  # See GetPixelSize and SetPixelSize
+    PixelSize: 'Size'  # See GetPixelSize and SetPixelSize
     PointSize: int  # See GetPointSize and SetPointSize
     Style: int  # See GetStyle and SetStyle
     Weight: int  # See GetWeight and SetWeight
 
 
 
 class FontData(Object):
@@ -16631,20 +16709,22 @@
         """ Determines whether the Help button will be displayed in the font dialog (Windows only).
 
             Source: https://docs.wxpython.org/wx.FontData.html
         """
 
     AllowSymbols: bool  # See GetAllowSymbols and SetAllowSymbols
     ChosenFont: 'Font'  # See GetChosenFont and SetChosenFont
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
     InitialFont: 'Font'  # See GetInitialFont and SetInitialFont
     ShowHelp: bool  # See GetShowHelp and SetShowHelp
 
 
 
+_FontData: TypeAlias = FontData
+
 class FontDialog(Dialog):
     """ This class represents the font chooser dialog.
 
         Source: https://docs.wxpython.org/wx.FontDialog.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -16673,15 +16753,15 @@
 
     def ShowModal(self) -> int:
         """ Shows the dialog, returning  ID_OK   if the user pressed Ok, and   ID_CANCEL   otherwise.
 
             Source: https://docs.wxpython.org/wx.FontDialog.html
         """
 
-    FontData: 'FontData'  # See GetFontData
+    FontData: '_FontData'  # See GetFontData
 
 
 
 class FontEnumerator:
     """ FontEnumerator enumerates either all available fonts on the system
 or only the ones with given attributes - either only fixed-width
 (suited for use in programs such as terminal emulators and the like)
@@ -17067,15 +17147,15 @@
         """ Sets the currently selected font.
 
             Source: https://docs.wxpython.org/wx.FontPickerCtrl.html
         """
 
     MaxPointSize: int  # See GetMaxPointSize and SetMaxPointSize
     MinPointSize: int  # See GetMinPointSize and SetMinPointSize
-    SelectedColour: Union[int, str, 'Colour']  # See GetSelectedColour and SetSelectedColour
+    SelectedColour: 'Colour'  # See GetSelectedColour and SetSelectedColour
     SelectedFont: 'Font'  # See GetSelectedFont and SetSelectedFont
 
 
 
 FNTP_DEFAULT_STYLE: int  # The default style: wx.FNTP_FONTDESC_AS_LABEL | wx.FNTP_USEFONT_FOR_LABEL.
 
 FNTP_USE_TEXTCTRL: int  # Creates a text control to the left of the picker button which is completely managed by the   wx.FontPickerCtrl  and which can be used by the user to specify a font (see SetSelectedFont). The text control is automatically synchronized with buttonâs value. Use functions defined in   wx.PickerBase  to modify the text control.
@@ -17105,17 +17185,23 @@
 
     def SetFont(self: 'Font', f) -> None:
         """ Set the font associated with the event.
 
             Source: https://docs.wxpython.org/wx.FontPickerEvent.html
         """
 
-    Font: 'Font'  # See GetFont and SetFont
+    Font: '_Font'  # See GetFont and SetFont
+
 
 
+_MenuBar: TypeAlias = MenuBar
+
+_StatusBar: TypeAlias = StatusBar
+
+_ToolBar: TypeAlias = ToolBar
 
 class Frame(TopLevelWindow):
     """ A frame is a window whose size and position can (usually) be changed
 by the user.
 
         Source: https://docs.wxpython.org/wx.Frame.html
     """
@@ -17254,18 +17340,18 @@
 
     def SetToolBar(self, toolBar: 'ToolBar') -> None:
         """ Associates a toolbar with the frame.
 
             Source: https://docs.wxpython.org/wx.Frame.html
         """
 
-    MenuBar: 'MenuBar'  # See GetMenuBar and SetMenuBar
-    StatusBar: 'StatusBar'  # See GetStatusBar and SetStatusBar
+    MenuBar: '_MenuBar'  # See GetMenuBar and SetMenuBar
+    StatusBar: '_StatusBar'  # See GetStatusBar and SetStatusBar
     StatusBarPane: int  # See GetStatusBarPane and SetStatusBarPane
-    ToolBar: 'ToolBar'  # See GetToolBar and SetToolBar
+    ToolBar: '_ToolBar'  # See GetToolBar and SetToolBar
 
 
 
 DEFAULT_FRAME_STYLE: int  # Defined as wx.MINIMIZE_BOX | wx.MAXIMIZE_BOX | wx.RESIZE_BORDER | wx.SYSTEM_MENU | wx.CAPTION | wx.CLOSE_BOX | wx.CLIP_CHILDREN.
 
 ICONIZE: int  # Display the frame iconized (minimized). Windows only.
 
@@ -17668,15 +17754,15 @@
 
     def SetItemSpan(self, *args, **kw) -> bool:
         """ Set the row/col spanning of the specified item.
 
             Source: https://docs.wxpython.org/wx.GridBagSizer.html
         """
 
-    EmptyCellSize: Union[tuple[int, int], 'Size']  # See GetEmptyCellSize and SetEmptyCellSize
+    EmptyCellSize: 'Size'  # See GetEmptyCellSize and SetEmptyCellSize
 
 
 
 class GBSizerItem(SizerItem):
     """ The GBSizerItem class is used by the GridBagSizer for tracking the
 items in the sizer.
 
@@ -17882,17 +17968,23 @@
 
     def SetGraphicsContext(self, context: 'GraphicsContext') -> None:
         """ Set the graphics context to be used for this   wx.GCDC.
 
             Source: https://docs.wxpython.org/wx.GCDC.html
         """
 
-    GraphicsContext: 'GraphicsContext'  # See GetGraphicsContext and SetGraphicsContext
+    GraphicsContext: '_GraphicsContext'  # See GetGraphicsContext and SetGraphicsContext
+
+
 
+_AntialiasMode: TypeAlias = AntialiasMode
 
+_CompositionMode: TypeAlias = CompositionMode
+
+_InterpolationQuality: TypeAlias = InterpolationQuality
 
 class GraphicsContext(GraphicsObject):
     """ A GraphicsContext instance is the object that is drawn upon.
 
         Source: https://docs.wxpython.org/wx.GraphicsContext.html
     """
     def BeginLayer(self, opacity: 'Double') -> None:
@@ -18291,21 +18383,21 @@
 
     def Translate(self, dx, dy) -> None:
         """ Translates the current transformation matrix.
 
             Source: https://docs.wxpython.org/wx.GraphicsContext.html
         """
 
-    AntialiasMode: AntialiasMode  # See GetAntialiasMode and SetAntialiasMode
-    CompositionMode: CompositionMode  # See GetCompositionMode and SetCompositionMode
-    InterpolationQuality: InterpolationQuality  # See GetInterpolationQuality and SetInterpolationQuality
+    AntialiasMode: '_AntialiasMode'  # See GetAntialiasMode and SetAntialiasMode
+    CompositionMode: '_CompositionMode'  # See GetCompositionMode and SetCompositionMode
+    InterpolationQuality: '_InterpolationQuality'  # See GetInterpolationQuality and SetInterpolationQuality
     NativeContext: None  # See GetNativeContext
     TextExtent: Any  # See GetTextExtent
     Transform: 'GraphicsMatrix'  # See GetTransform and SetTransform
-    Window: 'Window'  # See GetWindow
+    Window: '_Window'  # See GetWindow
 
 
 
 class GDIObject(Object):
     """ This class allows platforms to implement functionality to optimise GDI
 objects, such as Pen, Brush and Font.
 
@@ -18458,21 +18550,21 @@
 
     def __eq__(self, item: Any) -> bool:
         """ Equality operator.
 
             Source: https://docs.wxpython.org/wx.Pen.html
         """
 
-    Cap: PenCap  # See GetCap and SetCap
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Cap: 'PenCap'  # See GetCap and SetCap
+    Colour: '_Colour'  # See GetColour and SetColour
     Dashes: list[int]  # See GetDashes and SetDashes
-    Join: PenJoin  # See GetJoin and SetJoin
-    Quality: PenQuality  # See GetQuality and SetQuality
+    Join: 'PenJoin'  # See GetJoin and SetJoin
+    Quality: 'PenQuality'  # See GetQuality and SetQuality
     Stipple: 'Bitmap'  # See GetStipple and SetStipple
-    Style: PenStyle  # See GetStyle and SetStyle
+    Style: 'PenStyle'  # See GetStyle and SetStyle
     Width: int  # See GetWidth and SetWidth
 
 
 
 PENSTYLE_TRANSPARENT: int
 
 class GenericDirCtrl(Control):
@@ -18642,15 +18734,15 @@
     FilePath: str  # See GetFilePath
     Filter: str  # See GetFilter and SetFilter
     FilterIndex: int  # See GetFilterIndex and SetFilterIndex
     FilterListCtrl: 'DirFilterListCtrl'  # See GetFilterListCtrl
     Path: str  # See GetPath and SetPath
     Paths: list  # See GetPaths
     RootId: 'TreeItemId'  # See GetRootId
-    TreeCtrl: 'TreeCtrl'  # See GetTreeCtrl
+    TreeCtrl: '_TreeCtrl'  # See GetTreeCtrl
 
 
 
 DIRCTRL_DIR_ONLY: int  # Only show directories, and not files.
 
 DIRCTRL_3D_INTERNAL: int  # Use 3D borders for internal controls. This is the default.
 
@@ -18873,19 +18965,19 @@
             Source: https://docs.wxpython.org/wx.GenericMessageDialog.html
         """
 
     CancelLabel: str  # See GetCancelLabel
     Caption: str  # See GetCaption
     EffectiveIcon: int  # See GetEffectiveIcon
     ExtendedMessage: str  # See GetExtendedMessage and SetExtendedMessage
-    HelpLabel: MessageDialogButtonLabel  # See GetHelpLabel and SetHelpLabel
+    HelpLabel: str  # See GetHelpLabel and SetHelpLabel
     Message: str  # See GetMessage and SetMessage
     MessageDialogStyle: int  # See GetMessageDialogStyle
     NoLabel: str  # See GetNoLabel
-    OKLabel: MessageDialogButtonLabel  # See GetOKLabel and SetOKLabel
+    OKLabel: str  # See GetOKLabel and SetOKLabel
     YesLabel: str  # See GetYesLabel
 
 
 
 YES_NO: int  # Puts Yes and No buttons in the message box. It is recommended to always use  CANCEL   with this style as otherwise the message box wonât have a close button under wxMSW and the user will be forced to answer it.
 
 CANCEL_DEFAULT: int  # Makes the âCancelâ button default, can only be used with  CANCEL . This style is currently not supported (and ignored) in wxOSX.
@@ -19050,15 +19142,15 @@
 
     def SetPosition(self, pos: Union[tuple[int, int], 'Point']) -> None:
         """ Sets the position where the event took effect, in client coordinates: position of Pan event, center of zoom for Zoom event, center of rotation for Rotate event.
 
             Source: https://docs.wxpython.org/wx.GestureEvent.html
         """
 
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
+    Position: 'Point'  # See GetPosition and SetPosition
 
 
 
 class GIFHandler(ImageHandler):
     """ This is the image handler for the GIF format.
 
         Source: https://docs.wxpython.org/wx.GIFHandler.html
@@ -19168,15 +19260,15 @@
 
     def SetPosition(self, pos: float) -> None:
         """ Change the stop position.
 
             Source: https://docs.wxpython.org/wx.GraphicsGradientStop.html
         """
 
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
     Position: float  # See GetPosition and SetPosition
 
 
 
 class GraphicsGradientStops:
     """ Represents a collection of GraphicGradientStop values for use with
 CreateLinearGradientBrush and CreateRadialGradientBrush.
@@ -19233,23 +19325,23 @@
 
     def __getitem__(self, n) -> None:
         """ 
 
             Source: https://docs.wxpython.org/wx.GraphicsGradientStops.html
         """
 
-    def __len__(self) -> SIP_SSIZE_T:
+    def __len__(self) -> 'SIP_SSIZE_T':
         """ SIP_SSIZE_T
 
             Source: https://docs.wxpython.org/wx.GraphicsGradientStops.html
         """
 
     Count: int  # See GetCount
-    EndColour: Union[int, str, 'Colour']  # See GetEndColour and SetEndColour
-    StartColour: Union[int, str, 'Colour']  # See GetStartColour and SetStartColour
+    EndColour: 'Colour'  # See GetEndColour and SetEndColour
+    StartColour: 'Colour'  # See GetStartColour and SetStartColour
 
 
 
 class GraphicsMatrix(GraphicsObject):
     """ A GraphicsMatrix is a native representation of an affine matrix.
 
         Source: https://docs.wxpython.org/wx.GraphicsMatrix.html
@@ -19491,14 +19583,16 @@
 class GraphicsPen(GraphicsObject):
     """ A GraphicsPen is a native representation of a pen.
 
         Source: https://docs.wxpython.org/wx.GraphicsPen.html
     """
 
 
+_GradientType: TypeAlias = GradientType
+
 class GraphicsPenInfo:
     """ This class is a helper used for GraphicsPen creation using named
 parameter idiom: it allows specifying various GraphicsPen attributes
 using the chained calls to its clearly named methods instead of
 passing them in the fixed order to GraphicsPen constructors.
 
         Source: https://docs.wxpython.org/wx.GraphicsPenInfo.html
@@ -19663,15 +19757,15 @@
         """ width (wx.Double) â
 
             Source: https://docs.wxpython.org/wx.GraphicsPenInfo.html
         """
 
     EndX: 'Double'  # See GetEndX
     EndY: 'Double'  # See GetEndY
-    GradientType: 'GradientType'  # See GetGradientType
+    GradientType: '_GradientType'  # See GetGradientType
     Radius: 'Double'  # See GetRadius
     StartX: 'Double'  # See GetStartX
     StartY: 'Double'  # See GetStartY
     Stops: 'GraphicsGradientStops'  # See GetStops
     X1: 'Double'  # See GetX1
     X2: 'Double'  # See GetX2
     Y1: 'Double'  # See GetY1
@@ -19927,15 +20021,15 @@
 
     def FitInside(self, window: 'Window') -> None:
         """ Tell the sizer to resize the virtual size of the window  to match the sizerâs minimal size.
 
             Source: https://docs.wxpython.org/wx.Sizer.html
         """
 
-    def GetChildren(self) -> SizerItemList:
+    def GetChildren(self) -> 'SizerItemList':
         """ Returns the list of the items in this sizer.
 
             Source: https://docs.wxpython.org/wx.Sizer.html
         """
 
     def GetContainingWindow(self) -> 'Window':
         """ Returns the window this sizer is used in or None if none.
@@ -20120,20 +20214,20 @@
     def __nonzero__(self) -> None:
         """ Can be used to test if the C++ part of the sizer still exists, with
 code like this:
 
             Source: https://docs.wxpython.org/wx.Sizer.html
         """
 
-    Children: SizerItemList  # See GetChildren
+    Children: 'SizerItemList'  # See GetChildren
     ContainingWindow: 'Window'  # See GetContainingWindow and SetContainingWindow
     ItemCount: int  # See GetItemCount
-    MinSize: Union[tuple[int, int], 'Size']  # See GetMinSize and SetMinSize
+    MinSize: 'Size'  # See GetMinSize and SetMinSize
     Position: 'Point'  # See GetPosition
-    Size: 'Size'  # See GetSize
+    Size: '_Size'  # See GetSize
 
 
 
 ALL: int
 
 EXPAND: int
 
@@ -20193,14 +20287,16 @@
     m_labelColour: Any  # A public C++ attribute of type Colour     .
     m_labelFont: Any  # A public C++ attribute of type Font     .
     m_labelText: Any  # A public C++ attribute of type string.
     m_selectionColour: Any  # A public C++ attribute of type Colour     .
 
 
 
+_BitmapBundle: TypeAlias = BitmapBundle
+
 class HeaderColumn:
     """ Represents a column header in controls displaying tabular data such as
 DataViewCtrl or Grid.
 
         Source: https://docs.wxpython.org/wx.HeaderColumn.html
     """
     def GetAlignment(self) -> int:
@@ -20290,16 +20386,16 @@
     def IsSortable(self) -> bool:
         """ Returns True if the column can be clicked by user to sort the control contents by the field in this column.
 
             Source: https://docs.wxpython.org/wx.HeaderColumn.html
         """
 
     Alignment: int  # See GetAlignment
-    Bitmap: 'Bitmap'  # See GetBitmap
-    BitmapBundle: 'BitmapBundle'  # See GetBitmapBundle
+    Bitmap: '_Bitmap'  # See GetBitmap
+    BitmapBundle: '_BitmapBundle'  # See GetBitmapBundle
     Flags: int  # See GetFlags
     Hidden: Any  # See IsHidden
     MinWidth: int  # See GetMinWidth
     Reorderable: Any  # See IsReorderable
     Resizeable: Any  # See IsResizeable
     Shown: Any  # See IsShown
     SortKey: Any  # See IsSortKey
@@ -20424,16 +20520,16 @@
     def SetWidth(self, width: int) -> None:
         """ Trivial implementations of the base class pure virtual functions.
 
             Source: https://docs.wxpython.org/wx.HeaderColumnSimple.html
         """
 
     Alignment: int  # See GetAlignment and SetAlignment
-    Bitmap: 'BitmapBundle'  # See GetBitmap and SetBitmap
-    BitmapBundle: 'BitmapBundle'  # See GetBitmapBundle
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
+    BitmapBundle: '_BitmapBundle'  # See GetBitmapBundle
     Flags: int  # See GetFlags and SetFlags
     MinWidth: int  # See GetMinWidth and SetMinWidth
     Title: str  # See GetTitle and SetTitle
     Width: int  # See GetWidth and SetWidth
 
 
 
@@ -20960,15 +21056,15 @@
 
     def SetPosition(self, pt: Union[tuple[int, int], 'Point']) -> None:
         """ Sets the left-click position of the mouse, in screen coordinates.
 
             Source: https://docs.wxpython.org/wx.HelpEvent.html
         """
 
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
+    Position: 'Point'  # See GetPosition and SetPosition
 
 
 
 class HScrolledWindow(Panel,VarHScrollHelper):
     """ In the name of this class, âHâ stands for âhorizontalâ because it can
 be used for scrolling columns of variable widths.
 
@@ -21192,15 +21288,15 @@
     Depth: int  # See GetDepth and SetDepth
     Handle: int  # See GetHandle and SetHandle
     Height: int  # See GetHeight and SetHeight
     LogicalHeight: float  # See GetLogicalHeight
     LogicalSize: 'Size'  # See GetLogicalSize
     LogicalWidth: float  # See GetLogicalWidth
     ScaleFactor: float  # See GetScaleFactor
-    Size: 'Size'  # See GetSize
+    Size: '_Size'  # See GetSize
     Width: int  # See GetWidth and SetWidth
 
 
 
 class IconBundle(GDIObject):
     """ This class contains multiple copies of an icon in different sizes.
 
@@ -21244,15 +21340,15 @@
 
     def IsEmpty(self) -> bool:
         """ Returns True if the bundle doesnât contain any icons, False otherwise (in which case a call to GetIcon   with default parameter should return a valid icon).
 
             Source: https://docs.wxpython.org/wx.IconBundle.html
         """
 
-    Icon: 'Icon'  # See GetIcon
+    Icon: '_Icon'  # See GetIcon
     IconCount: int  # See GetIconCount
 
 
 
 class IconizeEvent(Event):
     """ An event being sent when the frame is iconized (minimized) or
 restored.
@@ -21752,15 +21848,15 @@
     def GetWidth(self) -> int:
         """ Gets the width of the image in pixels.
 
             Source: https://docs.wxpython.org/wx.Image.html
         """
 
     @staticmethod
-    def HSVtoRGB(hsv: HSVValue) -> RGBValue:
+    def HSVtoRGB(hsv: HSVValue) -> 'RGBValue':
         """ Converts a color in HSV color space to RGB color space.
 
             Source: https://docs.wxpython.org/wx.Image.html
         """
 
     def HasAlpha(self) -> bool:
         """ Returns True if this image has alpha channel, False otherwise.
@@ -21827,15 +21923,15 @@
     def Paste(self, image, x, y, alphaBlend=IMAGE_ALPHA_BLEND_OVER) -> None:
         """ Copy the data of the given image  to the specified position in this image.
 
             Source: https://docs.wxpython.org/wx.Image.html
         """
 
     @staticmethod
-    def RGBtoHSV(rgb: RGBValue) -> HSVValue:
+    def RGBtoHSV(rgb: RGBValue) -> 'HSVValue':
         """ Converts a color in RGB color space to HSV color space.
 
             Source: https://docs.wxpython.org/wx.Image.html
         """
 
     @staticmethod
     def RemoveHandler(name: str) -> bool:
@@ -22001,15 +22097,15 @@
             Source: https://docs.wxpython.org/wx.Image.html
         """
 
     Height: int  # See GetHeight
     MaskBlue: int  # See GetMaskBlue
     MaskGreen: int  # See GetMaskGreen
     MaskRed: int  # See GetMaskRed
-    Type: BitmapType  # See GetType and SetType
+    Type: 'BitmapType'  # See GetType and SetType
     Width: int  # See GetWidth
 
 
 
 BITMAP_TYPE_BMP: int
 
 BITMAP_TYPE_GIF: int
@@ -22032,14 +22128,16 @@
 
 BITMAP_TYPE_CUR: int
 
 BITMAP_TYPE_ANI: int
 
 BITMAP_TYPE_ANY: int
 
+_Image: TypeAlias = Image
+
 class ImageDataObject(CustomDataObject):
     """ ImageDataObject is a specialization of DataObject for image data.
 
         Source: https://docs.wxpython.org/wx.ImageDataObject.html
     """
     def __init__(self, image: 'Image'=NullImage) -> None:
         """ Constructor, optionally passing an image (otherwise use SetImage   later).
@@ -22069,15 +22167,15 @@
     def SetImage(self, image: 'Image') -> None:
         """ Sets the image stored by the data object.
 
             Source: https://docs.wxpython.org/wx.ImageDataObject.html
         """
 
     AllFormats: None  # See GetAllFormats
-    Image: 'Image'  # See GetImage and SetImage
+    Image: '_Image'  # See GetImage and SetImage
 
 
 
 class ImageHandler(Object):
     """ This is the base class for implementing image file loading/saving, and
 image creation from data.
 
@@ -22185,15 +22283,15 @@
             Source: https://docs.wxpython.org/wx.ImageHandler.html
         """
 
     AltExtensions: list[str]  # See GetAltExtensions and SetAltExtensions
     Extension: str  # See GetExtension and SetExtension
     MimeType: str  # See GetMimeType and SetMimeType
     Name: str  # See GetName and SetName
-    Type: BitmapType  # See GetType and SetType
+    Type: 'BitmapType'  # See GetType and SetType
 
 
 
 class ImageHistogram:
     """ startR (int) â 
 
         Source: https://docs.wxpython.org/wx.ImageHistogram.html
@@ -22306,14 +22404,16 @@
 
 IMAGELIST_DRAW_TRANSPARENT: int
 
 IMAGELIST_DRAW_SELECTED: int
 
 IMAGELIST_DRAW_FOCUSED: int
 
+_Relationship: TypeAlias = Relationship
+
 class IndividualLayoutConstraint(Object):
     """ sibling (wx.Window) â 
 
         Source: https://docs.wxpython.org/wx.IndividualLayoutConstraint.html
     """
     def __init__(self) -> None:
         """ 
@@ -22479,19 +22579,21 @@
 
     Done: bool  # See GetDone and SetDone
     Margin: int  # See GetMargin and SetMargin
     MyEdge: 'Edge'  # See GetMyEdge
     OtherEdge: int  # See GetOtherEdge
     OtherWindow: 'Window'  # See GetOtherWindow
     Percent: int  # See GetPercent
-    Relationship: Relationship  # See GetRelationship and SetRelationship
+    Relationship: '_Relationship'  # See GetRelationship and SetRelationship
     Value: int  # See GetValue and SetValue
 
 
 
+_ShowEffect: TypeAlias = ShowEffect
+
 class InfoBar(Control):
     """ An info bar is a transient window shown at top or bottom of its parent
 window to display non-critical information to the user.
 
         Source: https://docs.wxpython.org/wx.InfoBar.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -22590,15 +22692,15 @@
 
             Source: https://docs.wxpython.org/wx.InfoBar.html
         """
 
     ButtonCount: int  # See GetButtonCount
     EffectDuration: int  # See GetEffectDuration and SetEffectDuration
     HideEffect: 'ShowEffect'  # See GetHideEffect
-    ShowEffect: 'ShowEffect'  # See GetShowEffect
+    ShowEffect: '_ShowEffect'  # See GetShowEffect
 
 
 
 SHOW_EFFECT_NONE: int
 
 SHOW_EFFECT_SLIDE_TO_BOTTOM: int
 
@@ -22840,17 +22942,17 @@
 
     def __eq__(self, item: Any) -> bool:
         """ Compare two item attributes for equality.
 
             Source: https://docs.wxpython.org/wx.ItemAttr.html
         """
 
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
-    Font: 'Font'  # See GetFont and SetFont
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
+    Font: '_Font'  # See GetFont and SetFont
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
 
 
 
 class ItemContainerImmutable:
     """ ItemContainer defines an interface which is implemented by all
 controls which have string subitems each of which may be selected.
 
@@ -23210,21 +23312,21 @@
 
     def GetPosition(self) -> 'Point':
         """ Obtains the position (in client coordinates) at which the key was pressed.
 
             Source: https://docs.wxpython.org/wx.KeyEvent.html
         """
 
-    def GetRawKeyCode(self) -> 'int':
+    def GetRawKeyCode(self) -> int:
         """ Returns the raw key code for this event.
 
             Source: https://docs.wxpython.org/wx.KeyEvent.html
         """
 
-    def GetRawKeyFlags(self) -> 'int':
+    def GetRawKeyFlags(self) -> int:
         """ Returns the low level key flags for this event.
 
             Source: https://docs.wxpython.org/wx.KeyEvent.html
         """
 
     def GetUnicodeKey(self) -> int:
         """ Returns the Unicode character corresponding to this key event.
@@ -23284,16 +23386,16 @@
         """ 
 
             Source: https://docs.wxpython.org/wx.KeyEvent.html
         """
 
     KeyCode: int  # See GetKeyCode and SetKeyCode
     Position: 'Point'  # See GetPosition
-    RawKeyCode: 'int'  # See GetRawKeyCode and SetRawKeyCode
-    RawKeyFlags: 'int'  # See GetRawKeyFlags and SetRawKeyFlags
+    RawKeyCode: int  # See GetRawKeyCode and SetRawKeyCode
+    RawKeyFlags: int  # See GetRawKeyFlags and SetRawKeyFlags
     UnicodeKey: int  # See GetUnicodeKey and SetUnicodeKey
     X: 'Coord'  # See GetX
     Y: 'Coord'  # See GetY
 
 
 
 class LanguageInfo:
@@ -23322,14 +23424,16 @@
     Language: Any  # A public C++ attribute of type int.   wx.Language  id.
     LayoutDirection: Any  # A public C++ attribute of type LayoutDirection     . The layout direction used for this language.
     LocaleName: str  # See GetLocaleName
     LocaleTag: Any  # A public C++ attribute of type string. Tag for locale in BCP 47-like notation.
 
 
 
+Language: TypeAlias = int  # Enumeration
+
 LANGUAGE_DEFAULT: int
 
 LANGUAGE_UNKNOWN: int
 
 LANGUAGE_ABKHAZIAN: int
 
 LANGUAGE_AFAR: int
@@ -25812,30 +25916,30 @@
 
     def SortItems(self, fnSortCallBack) -> None:
         """ Call this function to sort the items in the list control.
 
             Source: https://docs.wxpython.org/wx.ListCtrl.html
         """
 
-    AlternateRowColour: Union[int, str, 'Colour']  # See GetAlternateRowColour and SetAlternateRowColour
+    AlternateRowColour: 'Colour'  # See GetAlternateRowColour and SetAlternateRowColour
     Column: 'ListItem'  # See GetColumn and SetColumn
     ColumnCount: int  # See GetColumnCount
     ColumnsOrder: list[int]  # See GetColumnsOrder and SetColumnsOrder
     CountPerPage: int  # See GetCountPerPage
     EditControl: 'TextCtrl'  # See GetEditControl
     FocusedItem: None  # See GetFocusedItem
     Item: 'ListItem'  # See GetItem and SetItem
     ItemCount: int  # See GetItemCount and SetItemCount
     ItemPosition: 'Point'  # See GetItemPosition and SetItemPosition
     ItemRect: 'Rect'  # See GetItemRect
     ItemSpacing: 'Size'  # See GetItemSpacing
     MainWindow: 'Window'  # See GetMainWindow
     SelectedItemCount: int  # See GetSelectedItemCount
     SortIndicator: int  # See GetSortIndicator
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
     TopItem: int  # See GetTopItem
     ViewRect: 'Rect'  # See GetViewRect
 
 
 
 LC_LIST: int  # Multicolumn list view, with optional small icons. Columns are computed automatically, i.e. you donât set columns as in  LC_REPORT . In other words, the list wraps, unlike a    wx.ListBox.
 
@@ -25959,14 +26063,16 @@
 
 LIST_HITTEST_ONITEMLABEL: int
 
 LIST_HITTEST_ONITEMSTATEICON: int
 
 LIST_HITTEST_ONITEM: int
 
+_Point: TypeAlias = Point
+
 class ListEvent(NotifyEvent):
     """ A list event holds information about events associated with ListCtrl
 objects.
 
         Source: https://docs.wxpython.org/wx.ListEvent.html
     """
     def __init__(self, commandType=wxEVT_NULL, id=0) -> None:
@@ -25989,15 +26095,15 @@
 
     def GetColumn(self) -> int:
         """ The column position: it is only used with  COL   events.
 
             Source: https://docs.wxpython.org/wx.ListEvent.html
         """
 
-    def GetData(self) -> 'UIntPtr':
+    def GetData(self) -> int:
         """ The data.
 
             Source: https://docs.wxpython.org/wx.ListEvent.html
         """
 
     def GetImage(self) -> int:
         """ The image.
@@ -26094,22 +26200,22 @@
 
             Source: https://docs.wxpython.org/wx.ListEvent.html
         """
 
     CacheFrom: int  # See GetCacheFrom and SetCacheFrom
     CacheTo: int  # See GetCacheTo and SetCacheTo
     Column: int  # See GetColumn and SetColumn
-    Data: 'UIntPtr'  # See GetData
+    Data: int  # See GetData
     Image: int  # See GetImage
     Index: int  # See GetIndex and SetIndex
     Item: 'ListItem'  # See GetItem and SetItem
     KeyCode: int  # See GetKeyCode and SetKeyCode
     Label: str  # See GetLabel
     Mask: int  # See GetMask
-    Point: Union[tuple[int, int], 'Point']  # See GetPoint and SetPoint
+    Point: '_Point'  # See GetPoint and SetPoint
     Text: str  # See GetText
 
 
 
 class ListItem(Object):
     """ This class stores information about a ListCtrl item or column.
 
@@ -26273,25 +26379,25 @@
 
     def SetWidth(self, width: int) -> None:
         """ Meaningful only for column headers in report mode.
 
             Source: https://docs.wxpython.org/wx.ListItem.html
         """
 
-    Align: ListColumnFormat  # See GetAlign and SetAlign
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
+    Align: 'ListColumnFormat'  # See GetAlign and SetAlign
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
     Column: int  # See GetColumn and SetColumn
     Data: int  # See GetData and SetData
-    Font: 'Font'  # See GetFont and SetFont
+    Font: '_Font'  # See GetFont and SetFont
     Id: int  # See GetId and SetId
     Image: int  # See GetImage and SetImage
     Mask: int  # See GetMask and SetMask
     State: int  # See GetState and SetState
     Text: str  # See GetText and SetText
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
     Width: int  # See GetWidth and SetWidth
 
 
 
 LIST_MASK_STATE: int
 
 LIST_MASK_TEXT: int
@@ -26999,14 +27105,16 @@
         """ Constructs a log target which sends all the log messages to the given text control.
 
             Source: https://docs.wxpython.org/wx.LogTextCtrl.html
         """
 
 
 
+_Frame: TypeAlias = Frame
+
 class LogWindow(LogInterposer):
     """ This class represents a background log window: to be precise, it
 collects all log messages in the log frame which it manages but also
 passes them on to the log target which was active at the moment of its
 creation.
 
         Source: https://docs.wxpython.org/wx.LogWindow.html
@@ -27037,15 +27145,15 @@
 
     def Show(self, show: bool=True) -> None:
         """ Shows or hides the frame.
 
             Source: https://docs.wxpython.org/wx.LogWindow.html
         """
 
-    Frame: 'Frame'  # See GetFrame
+    Frame: '_Frame'  # See GetFrame
 
 
 
 class LongPressEvent(GestureEvent):
     """ This event is generated when one finger touches the surface and
 remains stationary.
 
@@ -27075,15 +27183,15 @@
 
     def GetBitmap(self) -> 'Bitmap':
         """ Returns the mask as a monochrome bitmap.
 
             Source: https://docs.wxpython.org/wx.Mask.html
         """
 
-    Bitmap: 'Bitmap'  # See GetBitmap
+    Bitmap: '_Bitmap'  # See GetBitmap
 
 
 
 class Matrix2D:
     """ A simple container for 2x2 matrix.
 
         Source: https://docs.wxpython.org/wx.Matrix2D.html
@@ -27507,15 +27615,15 @@
 
     def GetMenuItemCount(self) -> int:
         """ Returns the number of items in the menu.
 
             Source: https://docs.wxpython.org/wx.Menu.html
         """
 
-    def GetMenuItems(self) -> MenuItemList:
+    def GetMenuItems(self) -> 'MenuItemList':
         """ Returns the list of items in the menu.
 
             Source: https://docs.wxpython.org/wx.Menu.html
         """
 
     def GetParent(self) -> 'Menu':
         """ wx.Menu
@@ -27647,19 +27755,19 @@
         """ Update the state of all menu items, recursively, by generating  wxEVT_UPDATE_UI   events for them.
 
             Source: https://docs.wxpython.org/wx.Menu.html
         """
 
     InvokingWindow: 'Window'  # See GetInvokingWindow and SetInvokingWindow
     MenuItemCount: int  # See GetMenuItemCount
-    MenuItems: MenuItemList  # See GetMenuItems
+    MenuItems: 'MenuItemList'  # See GetMenuItems
     Parent: 'Menu'  # See GetParent and SetParent
     Style: int  # See GetStyle
     Title: str  # See GetTitle and SetTitle
-    Window: 'Window'  # See GetWindow
+    Window: '_Window'  # See GetWindow
 
 
 
 MENU_TEAROFF: int
 
 class MenuBar(Window):
     """ A menu bar is a series of menus accessible from the top of a frame.
@@ -27874,14 +27982,16 @@
 
     Menus: None  # See GetMenus and SetMenus
 
 
 
 MB_DOCKABLE: int
 
+_Menu: TypeAlias = Menu
+
 class MenuEvent(Event):
     """ This class is used for a variety of menu-related events.
 
         Source: https://docs.wxpython.org/wx.MenuEvent.html
     """
     def __init__(self, type=wxEVT_NULL, id=0, menu=None) -> None:
         """ Constructor.
@@ -27903,15 +28013,15 @@
 
     def IsPopup(self) -> bool:
         """ Returns True if the menu which is being opened or closed is a popup menu, False if it is a normal one.
 
             Source: https://docs.wxpython.org/wx.MenuEvent.html
         """
 
-    Menu: 'Menu'  # See GetMenu
+    Menu: '_Menu'  # See GetMenu
     MenuId: int  # See GetMenuId
 
 
 
 class MenuItem(Object):
     """ A menu item represents an item in a menu.
 
@@ -28155,29 +28265,29 @@
     def SetTextColour(self, colour: Union[int, str, 'Colour']) -> None:
         """ Sets the text colour associated with the menu item.
 
             Source: https://docs.wxpython.org/wx.MenuItem.html
         """
 
     Accel: 'AcceleratorEntry'  # See GetAccel and SetAccel
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
-    Bitmap: 'BitmapBundle'  # See GetBitmap and SetBitmap
-    BitmapBundle: 'BitmapBundle'  # See GetBitmapBundle
-    DisabledBitmap: 'BitmapBundle'  # See GetDisabledBitmap and SetDisabledBitmap
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
+    BitmapBundle: '_BitmapBundle'  # See GetBitmapBundle
+    DisabledBitmap: 'Bitmap'  # See GetDisabledBitmap and SetDisabledBitmap
     Enabled: Any  # See IsEnabled and Enable
-    Font: 'Font'  # See GetFont and SetFont
+    Font: '_Font'  # See GetFont and SetFont
     Help: str  # See GetHelp and SetHelp
     Id: int  # See GetId
     ItemLabel: str  # See GetItemLabel and SetItemLabel
     ItemLabelText: str  # See GetItemLabelText
     Kind: 'ItemKind'  # See GetKind
     MarginWidth: int  # See GetMarginWidth and SetMarginWidth
-    Menu: 'Menu'  # See GetMenu and SetMenu
+    Menu: '_Menu'  # See GetMenu and SetMenu
     SubMenu: 'Menu'  # See GetSubMenu and SetSubMenu
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
 
 
 
 WXK_DELETE: int
 
 WXK_BACK: int
 
@@ -28428,19 +28538,19 @@
             Source: https://docs.wxpython.org/wx.MessageDialog.html
         """
 
     CancelLabel: str  # See GetCancelLabel
     Caption: str  # See GetCaption
     EffectiveIcon: int  # See GetEffectiveIcon
     ExtendedMessage: str  # See GetExtendedMessage and SetExtendedMessage
-    HelpLabel: MessageDialogButtonLabel  # See GetHelpLabel and SetHelpLabel
+    HelpLabel: str  # See GetHelpLabel and SetHelpLabel
     Message: str  # See GetMessage and SetMessage
     MessageDialogStyle: int  # See GetMessageDialogStyle
     NoLabel: str  # See GetNoLabel
-    OKLabel: MessageDialogButtonLabel  # See GetOKLabel and SetOKLabel
+    OKLabel: str  # See GetOKLabel and SetOKLabel
     YesLabel: str  # See GetYesLabel
 
 
 
 class Metafile(Object):
     """ A Metafile represents the MS Windows metafile object, so metafile
 operations have no effect in X.
@@ -29141,17 +29251,17 @@
 
     def SetY(self, y: int) -> None:
         """ y (int) â
 
             Source: https://docs.wxpython.org/wx.MouseState.html
         """
 
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
-    X: int  # See GetX and SetX
-    Y: int  # See GetY and SetY
+    Position: 'Point'  # See GetPosition and SetPosition
+    X: 'Coord'  # See GetX and SetX
+    Y: 'Coord'  # See GetY and SetY
     aux1IsDown: Any  # See Aux1IsDown and SetAux1Down
     aux2IsDown: Any  # See Aux2IsDown and SetAux2Down
     leftIsDown: Any  # See LeftIsDown and SetLeftDown
     middleIsDown: Any  # See MiddleIsDown and SetMiddleDown
     rightIsDown: Any  # See RightIsDown and SetRightDown
     x: Any  # See GetX and SetX
     y: Any  # See GetY and SetY
@@ -29189,16 +29299,16 @@
 
     def SetRect(self, rect: 'Rect') -> None:
         """ rect (wx.Rect) â
 
             Source: https://docs.wxpython.org/wx.MoveEvent.html
         """
 
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
-    Rect: 'Rect'  # See GetRect and SetRect
+    Position: 'Point'  # See GetPosition and SetPosition
+    Rect: '_Rect'  # See GetRect and SetRect
 
 
 
 EVT_MOVE: int  # Process a  wxEVT_MOVE   event, which is generated when a window is moved.
 
 EVT_MOVE_START: int  # Process a  wxEVT_MOVE_START   event, which is generated when the user starts to move or size a window. wxMSW only.
 
@@ -29684,14 +29794,16 @@
             Source: https://docs.wxpython.org/wx.NumberEntryDialog.html
         """
 
     Value: int  # See GetValue
 
 
 
+_ClassInfo: TypeAlias = ClassInfo
+
 class Object:
     """ This is the root class of many of the wxWidgets classes.
 
         Source: https://docs.wxpython.org/wx.Object.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -29749,15 +29861,15 @@
 
     def UnShare(self) -> None:
         """ This is the same of AllocExclusive   but this method is public.
 
             Source: https://docs.wxpython.org/wx.Object.html
         """
 
-    ClassInfo: 'ClassInfo'  # See GetClassInfo
+    ClassInfo: '_ClassInfo'  # See GetClassInfo
     ClassName: 'Char'  # See GetClassName
     RefData: 'ObjectRefData'  # See GetRefData and SetRefData
 
 
 
 class OutputStream(StreamBase):
     """ OutputStream is an abstract base class which may not be used
@@ -29894,14 +30006,16 @@
             Source: https://docs.wxpython.org/wx.PageSetupDialog.html
         """
 
     PageSetupData: 'PageSetupDialogData'  # See GetPageSetupData
 
 
 
+_PrintData: TypeAlias = PrintData
+
 class PageSetupDialogData(Object):
     """ This class holds a variety of information related to
 PageSetupDialog.
 
         Source: https://docs.wxpython.org/wx.PageSetupDialogData.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -30092,21 +30206,21 @@
 
     def __nonzero__(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.PageSetupDialogData.html
         """
 
-    MarginBottomRight: Union[tuple[int, int], 'Point']  # See GetMarginBottomRight and SetMarginBottomRight
-    MarginTopLeft: Union[tuple[int, int], 'Point']  # See GetMarginTopLeft and SetMarginTopLeft
-    MinMarginBottomRight: Union[tuple[int, int], 'Point']  # See GetMinMarginBottomRight and SetMinMarginBottomRight
-    MinMarginTopLeft: Union[tuple[int, int], 'Point']  # See GetMinMarginTopLeft and SetMinMarginTopLeft
-    PaperId: PaperSize  # See GetPaperId and SetPaperId
-    PaperSize: Union[tuple[int, int], 'Size']  # See GetPaperSize and SetPaperSize
-    PrintData: 'PrintData'  # See GetPrintData and SetPrintData
+    MarginBottomRight: 'Point'  # See GetMarginBottomRight and SetMarginBottomRight
+    MarginTopLeft: 'Point'  # See GetMarginTopLeft and SetMarginTopLeft
+    MinMarginBottomRight: 'Point'  # See GetMinMarginBottomRight and SetMinMarginBottomRight
+    MinMarginTopLeft: 'Point'  # See GetMinMarginTopLeft and SetMinMarginTopLeft
+    PaperId: 'PaperSize'  # See GetPaperId and SetPaperId
+    PaperSize: 'Size'  # See GetPaperSize and SetPaperSize
+    PrintData: '_PrintData'  # See GetPrintData and SetPrintData
 
 
 
 class PaintEvent(Event):
     """ A paint event is sent when a windowâs contents needs to be repainted.
 
         Source: https://docs.wxpython.org/wx.PaintEvent.html
@@ -30267,15 +30381,15 @@
 
     def SetDelta(self, delta: Union[tuple[int, int], 'Point']) -> None:
         """ Sets the distance covered since the previous panning event.
 
             Source: https://docs.wxpython.org/wx.PanGestureEvent.html
         """
 
-    Delta: Union[tuple[int, int], 'Point']  # See GetDelta and SetDelta
+    Delta: 'Point'  # See GetDelta and SetDelta
 
 
 
 EVT_GESTURE_PAN: int  # Process a  wxEVT_GESTURE_PAN . ^^
 
 class PasswordEntryDialog(TextEntryDialog):
     """ This class represents a dialog that requests a one-line password
@@ -30603,15 +30717,15 @@
 
             Source: https://docs.wxpython.org/wx.PickerBase.html
         """
 
     InternalMargin: int  # See GetInternalMargin and SetInternalMargin
     PickerCtrl: 'Control'  # See GetPickerCtrl and SetPickerCtrl
     PickerCtrlProportion: int  # See GetPickerCtrlProportion and SetPickerCtrlProportion
-    TextCtrl: 'TextCtrl'  # See GetTextCtrl and SetTextCtrl
+    TextCtrl: '_TextCtrl'  # See GetTextCtrl and SetTextCtrl
     TextCtrlProportion: int  # See GetTextCtrlProportion and SetTextCtrlProportion
 
 
 
 PB_USE_TEXTCTRL: int  # Creates a text control to the left of the picker which is completely managed by this   wx.PickerBase  class. ^^
 
 class PixelDataBase:
@@ -30661,26 +30775,38 @@
 
             Source: https://docs.wxpython.org/wx.PixelDataBase.html
         """
 
     Height: int  # See GetHeight
     Origin: 'Point'  # See GetOrigin
     RowStride: int  # See GetRowStride
-    Size: 'Size'  # See GetSize
+    Size: '_Size'  # See GetSize
     Width: int  # See GetWidth
 
 
 
 class PlatformId:
     """ Defines a very broad platform categorization.
 
         Source: https://docs.wxpython.org/wx.PlatformId.html
     """
 
 
+_Architecture: TypeAlias = Architecture
+
+_Bitness: TypeAlias = Bitness
+
+_Endianness: TypeAlias = Endianness
+
+_LinuxDistributionInfo: TypeAlias = LinuxDistributionInfo
+
+_OperatingSystemId: TypeAlias = OperatingSystemId
+
+_PortId: TypeAlias = PortId
+
 class PlatformInformation:
     """ PlatformInfo()
 PlatformInfo(pid, tkMajor=-1, tkMinor=-1, id=OS_UNKNOWN, osMajor=-1, osMinor=-1, bitness=BITNESS_INVALID, endian=ENDIAN_INVALID)
 
         Source: https://docs.wxpython.org/wx.PlatformInformation.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -30698,15 +30824,15 @@
     def CheckToolkitVersion(self, major, minor, micro=0) -> bool:
         """ Returns True if the toolkit version is at least  major.minor.micro .
 
             Source: https://docs.wxpython.org/wx.PlatformInformation.html
         """
 
     @staticmethod
-    def Get() -> PlatformInfo:
+    def Get() -> 'PlatformInfo':
         """ Returns the global PlatformInfo       object, initialized with the values for the currently running platform.
 
             Source: https://docs.wxpython.org/wx.PlatformInformation.html
         """
 
     @staticmethod
     def GetArch(arch: str) -> 'Architecture':
@@ -30942,31 +31068,31 @@
     def __eq__(self, item: Any) -> bool:
         """ Equality operator.
 
             Source: https://docs.wxpython.org/wx.PlatformInformation.html
         """
 
     ArchName: str  # See GetArchName
-    Architecture: Architecture  # See GetArchitecture and SetArchitecture
-    Bitness: Bitness  # See GetBitness and SetBitness
+    Architecture: '_Architecture'  # See GetArchitecture and SetArchitecture
+    Bitness: '_Bitness'  # See GetBitness and SetBitness
     BitnessName: str  # See GetBitnessName
     CpuArchitectureName: str  # See GetCpuArchitectureName
     DesktopEnvironment: str  # See GetDesktopEnvironment and SetDesktopEnvironment
-    Endianness: Endianness  # See GetEndianness and SetEndianness
+    Endianness: '_Endianness'  # See GetEndianness and SetEndianness
     EndiannessName: str  # See GetEndiannessName
-    LinuxDistributionInfo: 'LinuxDistributionInfo'  # See GetLinuxDistributionInfo and SetLinuxDistributionInfo
+    LinuxDistributionInfo: '_LinuxDistributionInfo'  # See GetLinuxDistributionInfo and SetLinuxDistributionInfo
     NativeCpuArchitectureName: str  # See GetNativeCpuArchitectureName
     OSMajorVersion: int  # See GetOSMajorVersion
     OSMicroVersion: int  # See GetOSMicroVersion
     OSMinorVersion: int  # See GetOSMinorVersion
     OperatingSystemDescription: str  # See GetOperatingSystemDescription and SetOperatingSystemDescription
     OperatingSystemFamilyName: str  # See GetOperatingSystemFamilyName
-    OperatingSystemId: OperatingSystemId  # See GetOperatingSystemId and SetOperatingSystemId
+    OperatingSystemId: '_OperatingSystemId'  # See GetOperatingSystemId and SetOperatingSystemId
     OperatingSystemIdName: str  # See GetOperatingSystemIdName
-    PortId: PortId  # See GetPortId and SetPortId
+    PortId: '_PortId'  # See GetPortId and SetPortId
     PortIdName: str  # See GetPortIdName
     PortIdShortName: str  # See GetPortIdShortName
     ToolkitMajorVersion: int  # See GetToolkitMajorVersion
     ToolkitMicroVersion: int  # See GetToolkitMicroVersion
     ToolkitMinorVersion: int  # See GetToolkitMinorVersion
 
 
@@ -31763,14 +31889,16 @@
         """ Calls wx.PrintPreview.PaintPage   to refresh the canvas.
 
             Source: https://docs.wxpython.org/wx.PreviewCanvas.html
         """
 
 
 
+_PrintPreview: TypeAlias = PrintPreview
+
 class PreviewControlBar(Panel):
     """ This is the default implementation of the preview control bar, a panel
 with buttons and a zoom control.
 
         Source: https://docs.wxpython.org/wx.PreviewControlBar.html
     """
     def __init__(self, preview, buttons, parent, pos=DefaultPosition, size=DefaultSize, style=0, name="panel") -> None:
@@ -31806,15 +31934,15 @@
 
     def SetZoomControl(self, percent: int) -> None:
         """ Sets the zoom control.
 
             Source: https://docs.wxpython.org/wx.PreviewControlBar.html
         """
 
-    PrintPreview: 'PrintPreview'  # See GetPrintPreview
+    PrintPreview: '_PrintPreview'  # See GetPrintPreview
     ZoomControl: int  # See GetZoomControl and SetZoomControl
 
 
 
 PREVIEW_PRINT: int
 
 PREVIEW_NEXT: int
@@ -31899,14 +32027,16 @@
         """ currentPage (int) â
 
             Source: https://docs.wxpython.org/wx.PrintAbortDialog.html
         """
 
 
 
+_PrintMode: TypeAlias = PrintMode
+
 class PrintData(Object):
     """ This class holds a variety of information related to printers and
 printer device contexts.
 
         Source: https://docs.wxpython.org/wx.PrintData.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -32085,24 +32215,24 @@
 
     def __nonzero__(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.PrintData.html
         """
 
-    Bin: PrintBin  # See GetBin and SetBin
+    Bin: 'PrintBin'  # See GetBin and SetBin
     Collate: bool  # See GetCollate and SetCollate
     Colour: bool  # See GetColour and SetColour
-    Duplex: DuplexMode  # See GetDuplex and SetDuplex
+    Duplex: 'DuplexMode'  # See GetDuplex and SetDuplex
     Filename: str  # See GetFilename and SetFilename
     NoCopies: int  # See GetNoCopies and SetNoCopies
-    Orientation: PrintOrientation  # See GetOrientation and SetOrientation
-    PaperId: PaperSize  # See GetPaperId and SetPaperId
-    PaperSize: Union[tuple[int, int], 'Size']  # See GetPaperSize and SetPaperSize
-    PrintMode: PrintMode  # See GetPrintMode and SetPrintMode
+    Orientation: 'PrintOrientation'  # See GetOrientation and SetOrientation
+    PaperId: 'PaperSize'  # See GetPaperId and SetPaperId
+    PaperSize: 'Size'  # See GetPaperSize and SetPaperSize
+    PrintMode: '_PrintMode'  # See GetPrintMode and SetPrintMode
     PrinterName: str  # See GetPrinterName and SetPrinterName
     PrivData: Any  # See GetPrivData and SetPrivData
     Quality: 'PrintQuality'  # See GetQuality and SetQuality
 
 
 
 DUPLEX_SIMPLEX: int
@@ -32119,14 +32249,16 @@
 
 PRINT_QUALITY_MEDIUM: int
 
 PRINT_QUALITY_LOW: int
 
 PRINT_QUALITY_DRAFT: int
 
+_PrintDialogData: TypeAlias = PrintDialogData
+
 class PrintDialog(Object):
     """ This class represents the print and print setup common dialogs.
 
         Source: https://docs.wxpython.org/wx.PrintDialog.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -32155,16 +32287,16 @@
     def ShowModal(self) -> int:
         """ Shows the dialog, returning  ID_OK   if the user pressed wx.OK, and   ID_CANCEL   otherwise.
 
             Source: https://docs.wxpython.org/wx.PrintDialog.html
         """
 
     PrintDC: 'DC'  # See GetPrintDC
-    PrintData: 'PrintData'  # See GetPrintData
-    PrintDialogData: 'PrintDialogData'  # See GetPrintDialogData
+    PrintData: '_PrintData'  # See GetPrintData
+    PrintDialogData: '_PrintDialogData'  # See GetPrintDialogData
 
 
 
 class PrintDialogData(Object):
     """ This class holds information related to the visual characteristics of
 PrintDialog.
 
@@ -32334,15 +32466,15 @@
 
     AllPages: bool  # See GetAllPages
     Collate: bool  # See GetCollate and SetCollate
     FromPage: int  # See GetFromPage and SetFromPage
     MaxPage: int  # See GetMaxPage and SetMaxPage
     MinPage: int  # See GetMinPage and SetMinPage
     NoCopies: int  # See GetNoCopies and SetNoCopies
-    PrintData: 'PrintData'  # See GetPrintData and SetPrintData
+    PrintData: '_PrintData'  # See GetPrintData and SetPrintData
     PrintToFile: bool  # See GetPrintToFile and SetPrintToFile
     Selection: bool  # See GetSelection and SetSelection
     ToPage: int  # See GetToPage and SetToPage
 
 
 
 class Printer(Object):
@@ -32403,15 +32535,15 @@
     def Setup(self, parent: 'Window') -> bool:
         """ Invokes the print setup dialog.
 
             Source: https://docs.wxpython.org/wx.Printer.html
         """
 
     Abort: bool  # See GetAbort
-    PrintDialogData: 'PrintDialogData'  # See GetPrintDialogData
+    PrintDialogData: '_PrintDialogData'  # See GetPrintDialogData
 
 
 
 PRINTER_NO_ERROR: int
 
 PRINTER_CANCELLED: int
 
@@ -32621,23 +32753,25 @@
 
     def SetLogicalOrigin(self, x, y) -> None:
         """ Set the device origin of the associated   wx.DC  so that the current logical point becomes the new logical origin.
 
             Source: https://docs.wxpython.org/wx.Printout.html
         """
 
-    DC: 'DC'  # See GetDC
+    DC: '_DC'  # See GetDC
     LogicalPageRect: 'Rect'  # See GetLogicalPageRect
     LogicalPaperRect: 'Rect'  # See GetLogicalPaperRect
     PaperRectPixels: 'Rect'  # See GetPaperRectPixels
     Preview: 'PrintPreview'  # See GetPreview
     Title: str  # See GetTitle
 
 
 
+_Printout: TypeAlias = Printout
+
 class PrintPreview(Object):
     """ Objects of this class manage the print preview process.
 
         Source: https://docs.wxpython.org/wx.PrintPreview.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -32751,22 +32885,26 @@
         """ int
 
             Source: https://docs.wxpython.org/wx.PrintPreview.html
         """
 
     Canvas: 'PreviewCanvas'  # See GetCanvas and SetCanvas
     CurrentPage: int  # See GetCurrentPage and SetCurrentPage
-    Frame: 'Frame'  # See GetFrame and SetFrame
+    Frame: '_Frame'  # See GetFrame and SetFrame
     MaxPage: int  # See GetMaxPage
     MinPage: int  # See GetMinPage
-    Printout: 'Printout'  # See GetPrintout and SetPrintout
+    Printout: '_Printout'  # See GetPrintout and SetPrintout
     PrintoutForPrinting: 'Printout'  # See GetPrintoutForPrinting
 
 
 
+_InputStream: TypeAlias = InputStream
+
+_OutputStream: TypeAlias = OutputStream
+
 class Process(EvtHandler):
     """ The objects of this class are used in conjunction with the Execute()
 function.
 
         Source: https://docs.wxpython.org/wx.Process.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -32871,16 +33009,16 @@
     def SetPriority(self, priority: Any) -> None:
         """ Sets the priority of the process, between 0 (lowest) and 100 (highest).
 
             Source: https://docs.wxpython.org/wx.Process.html
         """
 
     ErrorStream: 'InputStream'  # See GetErrorStream
-    InputStream: 'InputStream'  # See GetInputStream
-    OutputStream: 'OutputStream'  # See GetOutputStream
+    InputStream: '_InputStream'  # See GetInputStream
+    OutputStream: '_OutputStream'  # See GetOutputStream
     Pid: int  # See GetPid
 
 
 
 EVT_END_PROCESS: int  # Process a  wxEVT_END_PROCESS   event, sent by  wx.Process.OnTerminate   upon the external process termination. ^^
 
 class ProcessEvent(Event):
@@ -34075,24 +34213,24 @@
     def __iadd__(self) -> None:
         """ Like Union , but doesnât treat empty rectangles specially.
 
             Source: https://docs.wxpython.org/wx.Rect.html
         """
 
     Bottom: int  # See GetBottom and SetBottom
-    BottomLeft: Union[tuple[int, int], 'Point']  # See GetBottomLeft and SetBottomLeft
-    BottomRight: Union[tuple[int, int], 'Point']  # See GetBottomRight and SetBottomRight
+    BottomLeft: 'Point'  # See GetBottomLeft and SetBottomLeft
+    BottomRight: 'Point'  # See GetBottomRight and SetBottomRight
     Height: int  # See GetHeight and SetHeight
     Left: int  # See GetLeft and SetLeft
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
+    Position: 'Point'  # See GetPosition and SetPosition
     Right: int  # See GetRight and SetRight
-    Size: Union[tuple[int, int], 'Size']  # See GetSize and SetSize
+    Size: '_Size'  # See GetSize and SetSize
     Top: int  # See GetTop and SetTop
-    TopLeft: Union[tuple[int, int], 'Point']  # See GetTopLeft and SetTopLeft
-    TopRight: Union[tuple[int, int], 'Point']  # See GetTopRight and SetTopRight
+    TopLeft: 'Point'  # See GetTopLeft and SetTopLeft
+    TopRight: 'Point'  # See GetTopRight and SetTopRight
     Width: int  # See GetWidth and SetWidth
     X: int  # See GetX and SetX
     Y: int  # See GetY and SetY
     bottom: Any  # See GetBottom and SetBottom
     bottomLeft: Any  # See GetBottomLeft and SetBottomLeft
     bottomRight: Any  # See GetBottomRight and SetBottomRight
     height: Any  # A public C++ attribute of type int. Height member.
@@ -34126,21 +34264,21 @@
 
     def Contains(self, *args, **kw) -> bool:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def CreateIntersection(self, otherRect: Rect2DDouble) -> Rect2DDouble:
+    def CreateIntersection(self, otherRect: Rect2DDouble) -> 'Rect2DDouble':
         """ otherRect (Rect2DDouble) â
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def CreateUnion(self, otherRect: Rect2DDouble) -> Rect2DDouble:
+    def CreateUnion(self, otherRect: Rect2DDouble) -> 'Rect2DDouble':
         """ otherRect (Rect2DDouble) â
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
     def Get(self) -> Any:
         """ Get() . (x, y, width, height)
@@ -34150,15 +34288,15 @@
 
     def GetBottom(self) -> 'Double':
         """ wx.Double
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def GetCentre(self) -> Point2DDouble:
+    def GetCentre(self) -> 'Point2DDouble':
         """ Point2DDouble
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
     def GetIM(self) -> None:
         """ Returns an immutable representation of the wx.Rect2D object, based on namedtuple.
@@ -34168,21 +34306,21 @@
 
     def GetLeft(self) -> 'Double':
         """ wx.Double
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def GetLeftBottom(self) -> Point2DDouble:
+    def GetLeftBottom(self) -> 'Point2DDouble':
         """ Point2DDouble
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def GetLeftTop(self) -> Point2DDouble:
+    def GetLeftTop(self) -> 'Point2DDouble':
         """ Point2DDouble
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
     def GetOutCode(self, pt: Point2DDouble) -> 'OutCode':
         """ pt (Point2DDouble) â
@@ -34192,33 +34330,33 @@
 
     def GetOutcode(self, pt: Point2DDouble) -> 'OutCode':
         """ pt (Point2DDouble) â
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def GetPosition(self) -> Point2DDouble:
+    def GetPosition(self) -> 'Point2DDouble':
         """ Point2DDouble
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
     def GetRight(self) -> 'Double':
         """ wx.Double
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def GetRightBottom(self) -> Point2DDouble:
+    def GetRightBottom(self) -> 'Point2DDouble':
         """ Point2DDouble
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def GetRightTop(self) -> Point2DDouble:
+    def GetRightTop(self) -> 'Point2DDouble':
         """ Point2DDouble
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
     def GetSize(self) -> 'Size':
         """ wx.Size
@@ -34240,15 +34378,15 @@
 
     def Inset(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
-    def Interpolate(self, widthfactor, heightfactor) -> Point2DDouble:
+    def Interpolate(self, widthfactor, heightfactor) -> 'Point2DDouble':
         """ widthfactor (wx.int) â
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
     def Intersect(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -34451,24 +34589,24 @@
     def __eq__(self, item: Any) -> bool:
         """ rect (Rect2DDouble) â
 
             Source: https://docs.wxpython.org/wx.Rect2D.html
         """
 
     Bottom: 'Double'  # See GetBottom and SetBottom
-    Centre: Point2DDouble  # See GetCentre and SetCentre
+    Centre: 'Point2DDouble'  # See GetCentre and SetCentre
     IM: None  # See GetIM
     Left: 'Double'  # See GetLeft and SetLeft
-    LeftBottom: Point2DDouble  # See GetLeftBottom and SetLeftBottom
-    LeftTop: Point2DDouble  # See GetLeftTop and SetLeftTop
-    Position: Point2DDouble  # See GetPosition
+    LeftBottom: 'Point2DDouble'  # See GetLeftBottom and SetLeftBottom
+    LeftTop: 'Point2DDouble'  # See GetLeftTop and SetLeftTop
+    Position: 'Point2DDouble'  # See GetPosition
     Right: 'Double'  # See GetRight and SetRight
-    RightBottom: Point2DDouble  # See GetRightBottom and SetRightBottom
-    RightTop: Point2DDouble  # See GetRightTop and SetRightTop
-    Size: 'Size'  # See GetSize
+    RightBottom: 'Point2DDouble'  # See GetRightBottom and SetRightBottom
+    RightTop: 'Point2DDouble'  # See GetRightTop and SetRightTop
+    Size: '_Size'  # See GetSize
     Top: 'Double'  # See GetTop and SetTop
     m_height: Any  # A public C++ attribute of type Double     .
     m_width: Any  # A public C++ attribute of type Double     .
     m_x: Any  # A public C++ attribute of type Double     .
     m_y: Any  # A public C++ attribute of type Double     .
 
 
@@ -34679,15 +34817,15 @@
         """ Returns True while there are still rectangles available in the iteration.
 
             Source: https://docs.wxpython.org/wx.RegionIterator.html
         """
 
     H: 'Coord'  # See GetH
     Height: 'Coord'  # See GetHeight
-    Rect: 'Rect'  # See GetRect
+    Rect: '_Rect'  # See GetRect
     W: 'Coord'  # See GetW
     Width: 'Coord'  # See GetWidth
     X: 'Coord'  # See GetX
     Y: 'Coord'  # See GetY
 
 
 
@@ -35865,15 +36003,15 @@
 
     CancelButtonVisible: Any  # See IsCancelButtonVisible and ShowCancelButton
     DescriptiveText: str  # See GetDescriptiveText and SetDescriptiveText
     Hint: str  # See GetHint and SetHint
     InsertionPoint: int  # See GetInsertionPoint and SetInsertionPoint
     LastPosition: 'TextPos'  # See GetLastPosition
     Margins: 'Point'  # See GetMargins and SetMargins
-    Menu: 'Menu'  # See GetMenu and SetMenu
+    Menu: '_Menu'  # See GetMenu and SetMenu
     SearchButtonVisible: Any  # See IsSearchButtonVisible and ShowSearchButton
     StringSelection: str  # See GetStringSelection
     Value: str  # See GetValue and SetValue
 
 
 
 EVT_SEARCH: int  # Respond to a  wxEVT_SEARCH   event, generated when the search button is clicked. Note that this does not initiate a search on its own, you need to perform the appropriate action in your event handler. You may use:
@@ -35918,15 +36056,15 @@
 
     def SetCursor(self, cursor: 'Cursor') -> None:
         """ Sets the cursor associated with this event.
 
             Source: https://docs.wxpython.org/wx.SetCursorEvent.html
         """
 
-    Cursor: 'Cursor'  # See GetCursor and SetCursor
+    Cursor: '_Cursor'  # See GetCursor and SetCursor
     X: 'Coord'  # See GetX
     Y: 'Coord'  # See GetY
 
 
 
 class SettableHeaderColumn(HeaderColumn):
     """ Adds methods to set the column attributes to HeaderColumn.
@@ -36031,24 +36169,24 @@
 
     def UnsetAsSortKey(self) -> None:
         """ Donât use this column for sorting.
 
             Source: https://docs.wxpython.org/wx.SettableHeaderColumn.html
         """
 
-    Alignment: int  # See GetAlignment and SetAlignment
-    Bitmap: 'BitmapBundle'  # See GetBitmap and SetBitmap
-    Flags: int  # See GetFlags and SetFlags
-    Hidden: bool  # See IsHidden and SetHidden
-    MinWidth: int  # See GetMinWidth and SetMinWidth
-    Reorderable: bool  # See IsReorderable and SetReorderable
-    Resizeable: bool  # See IsResizeable and SetResizeable
-    Sortable: bool  # See IsSortable and SetSortable
-    Title: str  # See GetTitle and SetTitle
-    Width: int  # See GetWidth and SetWidth
+    Alignment: Any  # See GetAlignment and SetAlignment
+    Bitmap: Any  # See GetBitmap and SetBitmap
+    Flags: Any  # See GetFlags and SetFlags
+    Hidden: Any  # See IsHidden and SetHidden
+    MinWidth: Any  # See GetMinWidth and SetMinWidth
+    Reorderable: Any  # See IsReorderable and SetReorderable
+    Resizeable: Any  # See IsResizeable and SetResizeable
+    Sortable: Any  # See IsSortable and SetSortable
+    Title: Any  # See GetTitle and SetTitle
+    Width: Any  # See GetWidth and SetWidth
 
 
 
 ALIGN_NOT: int
 
 COL_RESIZABLE: int
 
@@ -36061,15 +36199,15 @@
     """
     def GetClientData(self) -> None:
         """ Get the untyped client data.
 
             Source: https://docs.wxpython.org/wx.SharedClientDataContainer.html
         """
 
-    def GetClientObject(self) -> ClientData:
+    def GetClientObject(self) -> 'ClientData':
         """ Get a pointer to the client data object.
 
             Source: https://docs.wxpython.org/wx.SharedClientDataContainer.html
         """
 
     def SetClientData(self, data: Any) -> None:
         """ Set the untyped client data.
@@ -36079,16 +36217,16 @@
 
     def SetClientObject(self, data: ClientData) -> None:
         """ Set the client data object.
 
             Source: https://docs.wxpython.org/wx.SharedClientDataContainer.html
         """
 
-    ClientData: Any  # See GetClientData and SetClientData
-    ClientObject: ClientData  # See GetClientObject and SetClientObject
+    ClientData: None  # See GetClientData and SetClientData
+    ClientObject: 'ClientData'  # See GetClientObject and SetClientObject
 
 
 
 class ShowEvent(Event):
     """ An event being sent when the window is shown or hidden.
 
         Source: https://docs.wxpython.org/wx.ShowEvent.html
@@ -36107,15 +36245,15 @@
 
     def SetShow(self, show: bool) -> None:
         """ Set whether the windows was shown or hidden.
 
             Source: https://docs.wxpython.org/wx.ShowEvent.html
         """
 
-    Show: bool  # See IsShown and SetShow
+    Show: Any  # See IsShown and SetShow
 
 
 
 EVT_SHOW: int  # Process a  wxEVT_SHOW   event. ^^
 
 class Simplebook(BookCtrlBase):
     """ Simplebook is a control showing exactly one of its several pages.
@@ -36486,16 +36624,16 @@
 
     def SetSize(self, size: Union[tuple[int, int], 'Size']) -> None:
         """ size (wx.Size) â
 
             Source: https://docs.wxpython.org/wx.SizeEvent.html
         """
 
-    Rect: 'Rect'  # See GetRect and SetRect
-    Size: Union[tuple[int, int], 'Size']  # See GetSize and SetSize
+    Rect: '_Rect'  # See GetRect and SetRect
+    Size: '_Size'  # See GetSize and SetSize
 
 
 
 class SizerFlags:
     """ Container for sizer items flags providing readable names for them.
 
         Source: https://docs.wxpython.org/wx.SizerFlags.html
@@ -36759,15 +36897,15 @@
 
     def GetSpacer(self) -> 'Size':
         """ If this item is tracking a spacer, return its size.
 
             Source: https://docs.wxpython.org/wx.SizerItem.html
         """
 
-    def GetUserData(self) -> PyUserData:
+    def GetUserData(self) -> 'PyUserData':
         """ Get the userData item attribute.
 
             Source: https://docs.wxpython.org/wx.SizerItem.html
         """
 
     def GetWindow(self) -> 'Window':
         """ If this item is tracking a window then return it.
@@ -36858,24 +36996,24 @@
 
             Source: https://docs.wxpython.org/wx.SizerItem.html
         """
 
     Border: int  # See GetBorder and SetBorder
     Flag: int  # See GetFlag and SetFlag
     Id: int  # See GetId and SetId
-    MinSize: Union[tuple[int, int], 'Size']  # See GetMinSize and SetMinSize
+    MinSize: 'Size'  # See GetMinSize and SetMinSize
     Position: 'Point'  # See GetPosition
     Proportion: int  # See GetProportion and SetProportion
     Ratio: float  # See GetRatio and SetRatio
-    Rect: 'Rect'  # See GetRect
-    Size: 'Size'  # See GetSize
-    Sizer: 'Sizer'  # See GetSizer
+    Rect: '_Rect'  # See GetRect
+    Size: '_Size'  # See GetSize
+    Sizer: '_Sizer'  # See GetSizer
     Spacer: 'Size'  # See GetSpacer
-    UserData: PyUserData  # See GetUserData and SetUserData
-    Window: 'Window'  # See GetWindow
+    UserData: 'PyUserData'  # See GetUserData and SetUserData
+    Window: '_Window'  # See GetWindow
 
 
 
 class SpinButton(Control):
     """ A SpinButton has two small up and down (or left and right) arrow
 buttons.
 
@@ -37096,15 +37234,15 @@
 
     Base: int  # See GetBase and SetBase
     Increment: int  # See GetIncrement and SetIncrement
     Max: int  # See GetMax and SetMax
     Min: int  # See GetMin and SetMin
     Range: None  # See GetRange
     TextValue: str  # See GetTextValue
-    Value: str  # See GetValue and SetValue
+    Value: int  # See GetValue and SetValue
 
 
 
 EVT_SPINCTRL: int  # Process a wxEVT_SPINCTRL event, which is generated whenever the numeric value of the spin control is updated. ^^
 
 class SpinCtrlDouble(Control):
     """ SpinCtrlDouble combines TextCtrl and SpinButton in one control
@@ -37211,15 +37349,15 @@
 
     Digits: int  # See GetDigits and SetDigits
     Increment: float  # See GetIncrement and SetIncrement
     Max: float  # See GetMax and SetMax
     Min: float  # See GetMin and SetMin
     Range: None  # See GetRange
     TextValue: str  # See GetTextValue
-    Value: str  # See GetValue and SetValue
+    Value: float  # See GetValue and SetValue
 
 
 
 EVT_SPINCTRLDOUBLE: int  # Generated whenever the numeric value of the spin control is changed, that is, when the up/down spin button is clicked, when ENTER is pressed, or the control loses focus and the new value is different from the last. See   wx.SpinDoubleEvent. ^^
 
 class SpinDoubleEvent(NotifyEvent):
     """ This event class is used for the events generated by SpinCtrlDouble.
@@ -37359,14 +37497,16 @@
 
     border: Any  # A public C++ attribute of type int. The width of the border drawn by the splitter inside it, may be 0.
     isHotSensitive: Any  # A public C++ attribute of type bool. True if the sash changes appearance when the mouse passes over it, False otherwise.
     widthSash: Any  # A public C++ attribute of type int. The width of the splitter sash.
 
 
 
+_SplitMode: TypeAlias = SplitMode
+
 class SplitterWindow(Window):
     """ This class manages up to two subwindows.
 
         Source: https://docs.wxpython.org/wx.SplitterWindow.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -37512,18 +37652,18 @@
 
             Source: https://docs.wxpython.org/wx.SplitterWindow.html
         """
 
     DefaultSashSize: int  # See GetDefaultSashSize
     MinimumPaneSize: int  # See GetMinimumPaneSize and SetMinimumPaneSize
     SashGravity: float  # See GetSashGravity and SetSashGravity
-    SashInvisible: bool  # See IsSashInvisible and SetSashInvisible
+    SashInvisible: Any  # See IsSashInvisible and SetSashInvisible
     SashPosition: int  # See GetSashPosition and SetSashPosition
     SashSize: int  # See GetSashSize
-    SplitMode: int  # See GetSplitMode and SetSplitMode
+    SplitMode: '_SplitMode'  # See GetSplitMode and SetSplitMode
     Window1: 'Window'  # See GetWindow1
     Window2: 'Window'  # See GetWindow2
 
 
 
 SP_3D: int  # Draws a 3D effect border and sash.
 
@@ -37770,16 +37910,16 @@
 
     def SetScaleMode(self, scaleMode: ScaleMode) -> None:
         """ Sets the scale mode.
 
             Source: https://docs.wxpython.org/wx.StaticBitmap.html
         """
 
-    Bitmap: 'BitmapBundle'  # See GetBitmap and SetBitmap
-    Icon: 'Icon'  # See GetIcon and SetIcon
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
+    Icon: '_Icon'  # See GetIcon and SetIcon
 
 
 
 class StaticBox(Control):
     """ A static box is a rectangle drawn around other windows to denote a
 logical grouping of items.
 
@@ -37814,14 +37954,16 @@
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.StaticBox.html
         """
 
 
 
+_StaticBox: TypeAlias = StaticBox
+
 class StaticBoxSizer(BoxSizer):
     """ StaticBoxSizer is a sizer derived from BoxSizer but adds a static
 box around the sizer.
 
         Source: https://docs.wxpython.org/wx.StaticBoxSizer.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -37844,15 +37986,15 @@
 
     def RepositionChildren(self, minSize: Union[tuple[int, int], 'Size']) -> None:
         """ Method which must be overridden in the derived sizer classes.
 
             Source: https://docs.wxpython.org/wx.StaticBoxSizer.html
         """
 
-    StaticBox: 'StaticBox'  # See GetStaticBox
+    StaticBox: '_StaticBox'  # See GetStaticBox
 
 
 
 class StaticLine(Control):
     """ A static line is just a line which may be used in a dialog to separate
 the groups of controls.
 
@@ -38445,15 +38587,15 @@
     def StartPage(self) -> None:
         """ Function not implemented in this DC class.
 
             Source: https://docs.wxpython.org/wx.SVGFileDC.html
         """
 
     Depth: int  # See GetDepth
-    LogicalFunction: RasterOperationMode  # See GetLogicalFunction and SetLogicalFunction
+    LogicalFunction: 'RasterOperationMode'  # See GetLogicalFunction and SetLogicalFunction
 
 
 
 SVG_SHAPE_RENDERING_AUTO: int
 
 class SysColourChangedEvent(Event):
     """ This class is used for system colour change events, which are
@@ -39247,23 +39389,23 @@
     def SetURL(self, url: str) -> None:
         """ Sets the URL for the content.
 
             Source: https://docs.wxpython.org/wx.TextAttr.html
         """
 
     Alignment: int  # See GetAlignment and SetAlignment
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
     BulletFont: str  # See GetBulletFont and SetBulletFont
     BulletName: str  # See GetBulletName and SetBulletName
     BulletNumber: int  # See GetBulletNumber and SetBulletNumber
     BulletStyle: int  # See GetBulletStyle and SetBulletStyle
     BulletText: str  # See GetBulletText and SetBulletText
     CharacterStyleName: str  # See GetCharacterStyleName and SetCharacterStyleName
     Flags: int  # See GetFlags and SetFlags
-    Font: 'Font'  # See GetFont and SetFont
+    Font: '_Font'  # See GetFont and SetFont
     FontEncoding: int  # See GetFontEncoding and SetFontEncoding
     FontFaceName: str  # See GetFontFaceName and SetFontFaceName
     FontFamily: int  # See GetFontFamily and SetFontFamily
     FontSize: int  # See GetFontSize and SetFontSize
     FontStyle: int  # See GetFontStyle and SetFontStyle
     FontUnderlined: bool  # See GetFontUnderlined and SetFontUnderlined
     FontWeight: int  # See GetFontWeight and SetFontWeight
@@ -39273,15 +39415,15 @@
     ListStyleName: str  # See GetListStyleName and SetListStyleName
     OutlineLevel: int  # See GetOutlineLevel and SetOutlineLevel
     ParagraphSpacingAfter: int  # See GetParagraphSpacingAfter and SetParagraphSpacingAfter
     ParagraphSpacingBefore: int  # See GetParagraphSpacingBefore and SetParagraphSpacingBefore
     ParagraphStyleName: str  # See GetParagraphStyleName and SetParagraphStyleName
     RightIndent: int  # See GetRightIndent and SetRightIndent
     Tabs: list[int]  # See GetTabs and SetTabs
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
     TextEffectFlags: int  # See GetTextEffectFlags and SetTextEffectFlags
     TextEffects: int  # See GetTextEffects and SetTextEffects
     URL: str  # See GetURL and SetURL
     UnderlineColour: 'Colour'  # See GetUnderlineColour
     UnderlineType: 'TextAttrUnderlineType'  # See GetUnderlineType
 
 
@@ -39306,14 +39448,16 @@
 
 TEXT_ATTR_EFFECT_STRIKETHROUGH: int
 
 TEXT_ATTR_EFFECT_SUPERSCRIPT: int
 
 TEXT_ATTR_EFFECT_SUBSCRIPT: int
 
+_CommandProcessor: TypeAlias = CommandProcessor
+
 class TextCompleter:
     """ Base class for custom text completer objects.
 
         Source: https://docs.wxpython.org/wx.TextCompleter.html
     """
     def GetNext(self) -> str:
         """ Called to retrieve the next completion.
@@ -39332,15 +39476,15 @@
 
 
 class TextCompleterSimple(TextCompleter):
     """ A simpler base class for custom completer objects.
 
         Source: https://docs.wxpython.org/wx.TextCompleterSimple.html
     """
-    def GetCompletions(self, prefix: str) -> res:
+    def GetCompletions(self, prefix: str) -> 'res':
         """ Pure virtual method returning all possible completions for the given prefix.
 
             Source: https://docs.wxpython.org/wx.TextCompleterSimple.html
         """
 
     def GetNext(self) -> str:
         """ Called to retrieve the next completion.
@@ -39755,14 +39899,16 @@
             Source: https://docs.wxpython.org/wx.TextEntryDialog.html
         """
 
     Value: str  # See GetValue and SetValue
 
 
 
+_MouseEvent: TypeAlias = MouseEvent
+
 class TextUrlEvent(CommandEvent):
     """  Overloaded Implementations:
 
         Source: https://docs.wxpython.org/wx.TextUrlEvent.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -39790,15 +39936,15 @@
 
     def GetURLStart(self) -> int:
         """ long
 
             Source: https://docs.wxpython.org/wx.TextUrlEvent.html
         """
 
-    MouseEvent: 'MouseEvent'  # See GetMouseEvent
+    MouseEvent: '_MouseEvent'  # See GetMouseEvent
     URLEnd: int  # See GetURLEnd
     URLStart: int  # See GetURLStart
 
 
 
 class TGAHandler(ImageHandler):
     """ This is the image handler for the TGA format.
@@ -39852,14 +39998,16 @@
         """ Loads an image from a stream, putting the resulting data into image.
 
             Source: https://docs.wxpython.org/wx.TIFFHandler.html
         """
 
 
 
+_Timer: TypeAlias = Timer
+
 class TimerEvent(Event):
     """ TimerEvent object is passed to the event handler of timer events
 (see Timer.SetOwner).
 
         Source: https://docs.wxpython.org/wx.TimerEvent.html
     """
     def __init__(self, timer: 'Timer') -> None:
@@ -39877,15 +40025,15 @@
     def GetTimer(self) -> 'Timer':
         """ Returns the timer object which generated this event.
 
             Source: https://docs.wxpython.org/wx.TimerEvent.html
         """
 
     Interval: int  # See GetInterval
-    Timer: 'Timer'  # See GetTimer
+    Timer: '_Timer'  # See GetTimer
 
 
 
 class TimerRunner:
     """ Starts the timer in its constructor, stops in the dtor.
 
         Source: https://docs.wxpython.org/wx.TimerRunner.html
@@ -40282,15 +40430,15 @@
 
     def GetToolByPos(self, pos: int) -> 'ToolBarToolBase':
         """ Returns a pointer to the tool at ordinal position pos.
 
             Source: https://docs.wxpython.org/wx.ToolBar.html
         """
 
-    def GetToolClientData(self, toolId: int) -> PyUserData:
+    def GetToolClientData(self, toolId: int) -> 'PyUserData':
         """ Get any client data associated with the tool.
 
             Source: https://docs.wxpython.org/wx.ToolBar.html
         """
 
     def GetToolEnabled(self, toolId: int) -> bool:
         """ Called to determine whether a tool is enabled (responds to user input).
@@ -40457,15 +40605,15 @@
     def ToggleTool(self, toolId, toggle) -> None:
         """ Toggles a tool on or off.
 
             Source: https://docs.wxpython.org/wx.ToolBar.html
         """
 
     Margins: 'Size'  # See GetMargins and SetMargins
-    ToolBitmapSize: Union[tuple[int, int], 'Size']  # See GetToolBitmapSize and SetToolBitmapSize
+    ToolBitmapSize: 'Size'  # See GetToolBitmapSize and SetToolBitmapSize
     ToolPacking: int  # See GetToolPacking and SetToolPacking
     ToolSeparation: int  # See GetToolSeparation and SetToolSeparation
     ToolSize: 'Size'  # See GetToolSize
     ToolsCount: int  # See GetToolsCount
 
 
 
@@ -40495,14 +40643,16 @@
 
 TB_RIGHT: int  # Align the toolbar at the right side of parent window.
 
 TB_DEFAULT_STYLE: int  # The  TB_HORIZONTAL   style. This style is new since wxWidgets 2.9.5. ^^
 
 EVT_TOOL_DROPDOWN: int  # Process a  wxEVT_TOOL_DROPDOWN   event. If unhandled, displays the default dropdown menu set using  wx.ToolBar.SetDropdownMenu . ^^
 
+_Control: TypeAlias = Control
+
 class ToolBarToolBase(Object):
     """ A toolbar tool represents one item on the toolbar.
 
         Source: https://docs.wxpython.org/wx.ToolBarToolBase.html
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
@@ -40536,15 +40686,15 @@
 
     def GetBitmap(self) -> 'Bitmap':
         """ wx.Bitmap
 
             Source: https://docs.wxpython.org/wx.ToolBarToolBase.html
         """
 
-    def GetClientData(self) -> PyUserData:
+    def GetClientData(self) -> 'PyUserData':
         """ PyUserData
 
             Source: https://docs.wxpython.org/wx.ToolBarToolBase.html
         """
 
     def GetControl(self) -> 'Control':
         """ wx.Control
@@ -40722,29 +40872,29 @@
 
     def Toggle(self, *args, **kw) -> bool:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ToolBarToolBase.html
         """
 
-    Bitmap: 'Bitmap'  # See GetBitmap
-    ClientData: PyUserData  # See GetClientData and SetClientData
-    Control: 'Control'  # See GetControl
-    DisabledBitmap: 'BitmapBundle'  # See GetDisabledBitmap and SetDisabledBitmap
+    Bitmap: '_Bitmap'  # See GetBitmap
+    ClientData: 'PyUserData'  # See GetClientData and SetClientData
+    Control: '_Control'  # See GetControl
+    DisabledBitmap: 'Bitmap'  # See GetDisabledBitmap and SetDisabledBitmap
     DisabledBitmapBundle: 'BitmapBundle'  # See GetDisabledBitmapBundle
     DropdownMenu: 'Menu'  # See GetDropdownMenu and SetDropdownMenu
     Id: int  # See GetId
     Kind: 'ItemKind'  # See GetKind
     Label: str  # See GetLabel and SetLabel
     LongHelp: str  # See GetLongHelp and SetLongHelp
-    NormalBitmap: 'BitmapBundle'  # See GetNormalBitmap and SetNormalBitmap
+    NormalBitmap: 'Bitmap'  # See GetNormalBitmap and SetNormalBitmap
     NormalBitmapBundle: 'BitmapBundle'  # See GetNormalBitmapBundle
     ShortHelp: str  # See GetShortHelp and SetShortHelp
     Style: int  # See GetStyle
-    ToolBar: 'ToolBar'  # See GetToolBar
+    ToolBar: '_ToolBar'  # See GetToolBar
 
 
 
 class Toolbook(BookCtrlBase):
     """ Toolbook is a class similar to Notebook but which uses a ToolBar
 to show the labels instead of the tabs.
 
@@ -40777,15 +40927,15 @@
 
     def GetToolBar(self) -> 'ToolBar':
         """ Return the toolbar used for page selection.
 
             Source: https://docs.wxpython.org/wx.Toolbook.html
         """
 
-    ToolBar: 'ToolBar'  # See GetToolBar
+    ToolBar: '_ToolBar'  # See GetToolBar
 
 
 
 TBK_BUTTONBAR: int  # Use ButtonToolBar-based implementation under macOS (ignored under other platforms).
 
 TBK_HORZ_LAYOUT: int  # Shows the text and the icons alongside, not vertically stacked (only implement under Windows and GTK 2 platforms as it relies on  TB_HORZ_LAYOUT   flag support). ^^
 
@@ -40855,15 +41005,15 @@
     def SetTip(self, tip: str) -> None:
         """ Set the tooltip text.
 
             Source: https://docs.wxpython.org/wx.ToolTip.html
         """
 
     Tip: str  # See GetTip and SetTip
-    Window: 'Window'  # See GetWindow
+    Window: '_Window'  # See GetWindow
 
 
 
 class TopLevelWindow(NonOwnedWindow):
     """ TopLevelWindow is a common base class for Dialog and Frame.
 
         Source: https://docs.wxpython.org/wx.TopLevelWindow.html
@@ -41161,15 +41311,15 @@
     def ShowWithoutActivating(self) -> None:
         """ Show the   wx.TopLevelWindow, but do not give it keyboard focus.
 
             Source: https://docs.wxpython.org/wx.TopLevelWindow.html
         """
 
     DefaultItem: 'Window'  # See GetDefaultItem and SetDefaultItem
-    Icon: 'Icon'  # See GetIcon and SetIcon
+    Icon: '_Icon'  # See GetIcon and SetIcon
     MacMetalAppearance: Any  # See MacGetMetalAppearance and MacSetMetalAppearance
     OSXModified: Any  # See OSXIsModified and OSXSetModified
     Title: str  # See GetTitle and SetTitle
     TmpDefaultItem: 'Window'  # See GetTmpDefaultItem and SetTmpDefaultItem
 
 
 
@@ -41861,14 +42011,16 @@
 
 EVT_TREE_ITEM_GETTOOLTIP: int  # The opportunity to set the item tooltip is being given to the application (call wx.TreeEvent.SetToolTip ). Windows only. Processes a  wxEVT_TREE_ITEM_GETTOOLTIP   event type.
 
 EVT_TREE_ITEM_MENU: int  # The context menu for the selected item has been requested, either by a right click or by using the menu key. Notice that these events always carry a valid tree item and so are not generated when (right) clicking outside of the items area. If you need to handle such events, consider using  wxEVT_CONTEXT_MENU   instead. Processes a   wxEVT_TREE_ITEM_MENU   event type.
 
 EVT_TREE_STATE_IMAGE_CLICK: int  # The state image has been clicked. Processes a  wxEVT_TREE_STATE_IMAGE_CLICK   event type. ^^
 
+_KeyEvent: TypeAlias = KeyEvent
+
 class TreeEvent(NotifyEvent):
     """ A tree event holds information about events associated with TreeCtrl
 objects.
 
         Source: https://docs.wxpython.org/wx.TreeEvent.html
     """
     def __init__(*args, **kwargs) -> None:
@@ -41923,18 +42075,18 @@
         """ Set the tooltip for the item (valid for  EVT_TREE_ITEM_GETTOOLTIP   events).
 
             Source: https://docs.wxpython.org/wx.TreeEvent.html
         """
 
     Item: 'TreeItemId'  # See GetItem
     KeyCode: int  # See GetKeyCode
-    KeyEvent: 'KeyEvent'  # See GetKeyEvent
+    KeyEvent: '_KeyEvent'  # See GetKeyEvent
     Label: str  # See GetLabel
     OldItem: 'TreeItemId'  # See GetOldItem
-    Point: 'Point'  # See GetPoint
+    Point: '_Point'  # See GetPoint
 
 
 
 class TreeItemId:
     """ An opaque reference to a tree item.
 
         Source: https://docs.wxpython.org/wx.TreeItemId.html
@@ -42106,15 +42258,15 @@
 
     def GetAsChar(self, c: int) -> bool:
         """ Returns True if the character is representable as a single byte in the current locale encoding.
 
             Source: https://docs.wxpython.org/wx.UniChar.html
         """
 
-    def GetValue(self) -> value_type:
+    def GetValue(self) -> 'value_type':
         """ Returns Unicode code point value of the character.
 
             Source: https://docs.wxpython.org/wx.UniChar.html
         """
 
     def HighSurrogate(self, *args, **kw) -> 'Uint16':
         """ Overloaded Implementations:
@@ -42142,15 +42294,15 @@
 
     def LowSurrogate(self, *args, **kw) -> 'Uint16':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.UniChar.html
         """
 
-    Value: value_type  # See GetValue
+    Value: 'value_type'  # See GetValue
 
 
 
 class UpdateUIEvent(CommandEvent):
     """ This class is used for pseudo-events which are called by wxWidgets to
 give an application the chance to update various user interface
 elements.
@@ -42398,15 +42550,15 @@
 
     def Validate(self, parent: 'Window') -> bool:
         """ This overridable function is called when the value in the associated window must be validated.
 
             Source: https://docs.wxpython.org/wx.Validator.html
         """
 
-    Window: 'Window'  # See GetWindow and SetWindow
+    Window: '_Window'  # See GetWindow and SetWindow
 
 
 
 class VarHScrollHelper(VarScrollHelperBase):
     """ This class provides functions wrapping the VarScrollHelperBase
 class, targeted for horizontal-specific scrolling.
 
@@ -42498,14 +42650,16 @@
 
     ColumnCount: int  # See GetColumnCount and SetColumnCount
     VisibleColumnsBegin: int  # See GetVisibleColumnsBegin
     VisibleColumnsEnd: int  # See GetVisibleColumnsEnd
 
 
 
+_Orientation: TypeAlias = Orientation
+
 class VarScrollHelperBase:
     """ This class provides all common base functionality for scroll
 calculations shared among all variable scrolled window implementations
 as well as automatic scrollbar functionality, saved scroll positions,
 controlling target windows to be scrolled, as well as defining all
 required virtual functions that need to be implemented for any
 orientation specific work.
@@ -42617,15 +42771,15 @@
     def VirtualHitTest(self, coord: int) -> int:
         """ Returns the virtual scroll unit under the device unit given accounting for scroll position or  NOT_FOUND   if none (i.e.
 
             Source: https://docs.wxpython.org/wx.VarScrollHelperBase.html
         """
 
     NonOrientationTargetSize: int  # See GetNonOrientationTargetSize
-    Orientation: 'Orientation'  # See GetOrientation
+    Orientation: '_Orientation'  # See GetOrientation
     OrientationTargetSize: int  # See GetOrientationTargetSize
     TargetWindow: 'Window'  # See GetTargetWindow and SetTargetWindow
     VisibleBegin: int  # See GetVisibleBegin
     VisibleEnd: int  # See GetVisibleEnd
 
 
 
@@ -43155,18 +43309,18 @@
     def Toggle(self, item: int) -> None:
         """ Toggles the state of the specified item, i.e. selects it if it was unselected and deselects it if it was selected.
 
             Source: https://docs.wxpython.org/wx.VListBox.html
         """
 
     ItemCount: int  # See GetItemCount and SetItemCount
-    Margins: Union[tuple[int, int], 'Point']  # See GetMargins and SetMargins
+    Margins: 'Point'  # See GetMargins and SetMargins
     SelectedCount: int  # See GetSelectedCount
     Selection: int  # See GetSelection and SetSelection
-    SelectionBackground: Union[int, str, 'Colour']  # See GetSelectionBackground and SetSelectionBackground
+    SelectionBackground: 'Colour'  # See GetSelectionBackground and SetSelectionBackground
 
 
 
 class VScrolledWindow(Panel,VarVScrollHelper):
     """ In the name of this class, âVâ may stand for âvariableâ because it can
 be used for scrolling rows of variable heights; âvirtualâ, because it
 is not necessary to know the heights of all rows in advance  only
@@ -43293,15 +43447,15 @@
 
     def GetWindow(self) -> 'Window':
         """ Return the window being created.
 
             Source: https://docs.wxpython.org/wx.WindowCreateEvent.html
         """
 
-    Window: 'Window'  # See GetWindow
+    Window: '_Window'  # See GetWindow
 
 
 
 EVT_WINDOW_CREATE: int  # Process a  wxEVT_CREATE   event. ^^
 
 class WindowDC(DC):
     """ A WindowDC must be constructed if an application wishes to paint on
@@ -43331,15 +43485,15 @@
 
     def GetWindow(self) -> 'Window':
         """ Return the window being destroyed.
 
             Source: https://docs.wxpython.org/wx.WindowDestroyEvent.html
         """
 
-    Window: 'Window'  # See GetWindow
+    Window: '_Window'  # See GetWindow
 
 
 
 class WindowDisabler:
     """ This class disables all top level windows of the application (maybe
 with the exception of one of them) in its constructor and enables them
 back in its destructor.
@@ -43451,14 +43605,16 @@
         """
 
     Id: int  # See GetId
     Value: int  # See GetValue
 
 
 
+_Dialog: TypeAlias = Dialog
+
 class WindowModalDialogEvent(CommandEvent):
     """ Event sent by Dialog.ShowWindowModal() when the dialog closes.
 
         Source: https://docs.wxpython.org/wx.WindowModalDialogEvent.html
     """
     def __init__(self, commandType=wxEVT_NULL, id=0) -> None:
         """ Constructor.
@@ -43480,19 +43636,21 @@
 
     def GetReturnCode(self) -> int:
         """ Return the dialogâs return code.
 
             Source: https://docs.wxpython.org/wx.WindowModalDialogEvent.html
         """
 
-    Dialog: 'Dialog'  # See GetDialog
+    Dialog: '_Dialog'  # See GetDialog
     ReturnCode: int  # See GetReturnCode
 
 
 
+_ImageList: TypeAlias = ImageList
+
 class WithImages:
     """ A mixin class to be used with other classes that use a ImageList.
 
         Source: https://docs.wxpython.org/wx.WithImages.html
     """
     def __init__(self) -> None:
         """ 
@@ -43539,15 +43697,15 @@
     def SetImages(self, images: Vector) -> None:
         """ Set the images to use for the items in the control.
 
             Source: https://docs.wxpython.org/wx.WithImages.html
         """
 
     ImageCount: int  # See GetImageCount
-    ImageList: 'ImageList'  # See GetImageList and SetImageList
+    ImageList: '_ImageList'  # See GetImageList and SetImageList
 
 
 
 NO_IMAGE: int
 
 class WrapSizer(BoxSizer):
     """ A wrap sizer lays out its items in a single line, like a box sizer  as
@@ -43644,24 +43802,28 @@
 
     ZoomFactor: float  # See GetZoomFactor and SetZoomFactor
 
 
 
 EVT_GESTURE_ZOOM: int  # Process a  wxEVT_GESTURE_ZOOM . ^^
 
+BatteryState: TypeAlias = int  # Enumeration
+
 BATTERY_NORMAL_STATE: int
 
 BATTERY_LOW_STATE: int
 
 BATTERY_CRITICAL_STATE: int
 
 BATTERY_SHUTDOWN_STATE: int
 
 BATTERY_UNKNOWN_STATE: int
 
+KeyCode: TypeAlias = int  # Enumeration
+
 WXK_NONE: int
 
 WXK_CONTROL_A: int
 
 WXK_CONTROL_B: int
 
 WXK_CONTROL_C: int
@@ -43904,14 +44066,16 @@
 
 WXK_LAUNCH_D: int
 
 WXK_LAUNCH_E: int
 
 WXK_LAUNCH_F: int
 
+OperatingSystemId: TypeAlias = int  # Enumeration
+
 OS_UNKNOWN: int
 
 OS_MAC_OS: int
 
 OS_MAC_OSX_DARWIN: int
 
 OS_MAC: int
@@ -43932,20 +44096,26 @@
 
 OS_UNIX_AIX: int
 
 OS_UNIX_HPUX: int
 
 OS_UNIX: int
 
+PowerType: TypeAlias = int  # Enumeration
+
 POWER_SOCKET: int
 
 POWER_BATTERY: int
 
 POWER_UNKNOWN: int
 
+DragResult: TypeAlias = int  # Enumeration
+
+Signal: TypeAlias = int  # Enumeration
+
 SIGNONE: int
 
 SIGHUP: int
 
 SIGINT: int
 
 SIGQUIT: int
@@ -43970,44 +44140,52 @@
 
 SIGPIPE: int
 
 SIGALRM: int
 
 SIGTERM: int
 
+KillError: TypeAlias = int  # Enumeration
+
 KILL_OK: int
 
 KILL_BAD_SIGNAL: int
 
 KILL_ACCESS_DENIED: int
 
 KILL_NO_PROCESS: int
 
 KILL_ERROR: int
 
+AcceleratorEntryFlags: TypeAlias = int  # Enumeration
+
 ACCEL_NORMAL: int
 
 ACCEL_ALT: int
 
 ACCEL_CTRL: int
 
 ACCEL_SHIFT: int
 
 ACCEL_RAW_CTRL: int
 
 ACCEL_CMD: int
 
+AccStatus: TypeAlias = int  # Enumeration
+
 ACC_FAIL: int
 
 ACC_FALSE: int
 
 ACC_NOT_IMPLEMENTED: int
 
 ACC_INVALID_ARG: int
 
+NavDir: TypeAlias = int  # Enumeration
+
 NAVDIR_FIRSTCHILD: int
 
 NAVDIR_LASTCHILD: int
 
 NAVDIR_DOWN: int
 
 NAVDIR_LEFT: int
@@ -44016,14 +44194,16 @@
 
 NAVDIR_PREVIOUS: int
 
 NAVDIR_RIGHT: int
 
 NAVDIR_UP: int
 
+AccObject: TypeAlias = int  # Enumeration
+
 OBJID_WINDOW: int
 
 OBJID_SYSMENU: int
 
 OBJID_TITLEBAR: int
 
 OBJID_MENU: int
@@ -44040,14 +44220,16 @@
 
 OBJID_CURSOR: int
 
 OBJID_ALERT: int
 
 OBJID_SOUND: int
 
+AccSelectionFlags: TypeAlias = int  # Enumeration
+
 ACC_SEL_NONE: int
 
 ACC_SEL_TAKEFOCUS: int
 
 ACC_SEL_TAKESELECTION: int
 
 ACC_SEL_EXTENDSELECTION: int
@@ -44062,24 +44244,28 @@
 
 ID_ANY: int
 
 ID_HIGHEST: int
 
 ID_LOWEST: int
 
+WindowVariant: TypeAlias = int  # Enumeration
+
 WINDOW_VARIANT_NORMAL: int
 
 WINDOW_VARIANT_SMALL: int
 
 WINDOW_VARIANT_MINI: int
 
 WINDOW_VARIANT_LARGE: int
 
 WINDOW_VARIANT_MAX: int
 
+BitmapType: TypeAlias = int  # Enumeration
+
 BITMAP_TYPE_INVALID: int
 
 BITMAP_TYPE_XBM: int
 
 BITMAP_TYPE_XBM_DATA: int
 
 BITMAP_TYPE_XPM_DATA: int
@@ -44106,14 +44292,16 @@
 
 BITMAP_TYPE_ICO: int
 
 BITMAP_TYPE_CUR_RESOURCE: int
 
 BITMAP_TYPE_CUR: int
 
+PortId: TypeAlias = int  # Enumeration
+
 PORT_UNKNOWN: int
 
 PORT_BASE: int
 
 PORT_MSW: int
 
 PORT_MOTIF: int
@@ -44266,14 +44454,16 @@
 
 ID_ZOOM_FIT: int
 
 ID_ZOOM_IN: int
 
 ID_ZOOM_OUT: int
 
+RasterOperationMode: TypeAlias = int  # Enumeration
+
 CLEAR: int
 
 INVERT: int
 
 OR_REVERSE: int
 
 OR: int
@@ -44294,24 +44484,30 @@
 
 OR_INVERT: int
 
 NAND: int
 
 SET: int
 
+FloodFillStyle: TypeAlias = int  # Enumeration
+
+MappingMode: TypeAlias = int  # Enumeration
+
 MM_TEXT: int
 
 MM_METRIC: int
 
 MM_LOMETRIC: int
 
 MM_TWIPS: int
 
 MM_POINTS: int
 
+Direction: TypeAlias = int  # Enumeration
+
 NORTH: int
 
 SOUTH: int
 
 WEST: int
 
 EAST: int
@@ -44379,14 +44575,16 @@
 
 GROW: int
 
 NORTH: int
 
 WEST: int
 
+BrushStyle: TypeAlias = int  # Enumeration
+
 BRUSHSTYLE_INVALID: int
 
 BRUSHSTYLE_SOLID: int
 
 BRUSHSTYLE_STIPPLE_MASK_OPAQUE: int
 
 BRUSHSTYLE_STIPPLE_MASK: int
@@ -44405,18 +44603,24 @@
 
 BRUSHSTYLE_VERTICAL_HATCH: int
 
 BRUSHSTYLE_FIRST_HATCH: int
 
 BRUSHSTYLE_LAST_HATCH: int
 
+CheckBoxState: TypeAlias = int  # Enumeration
+
 CHK_UNCHECKED: int
 
 CHK_CHECKED: int
 
+_ListCtrl: TypeAlias = ListCtrl
+
+HitTest: TypeAlias = int  # Enumeration
+
 HT_NOWHERE: int
 
 HT_SCROLLBAR_FIRST: int
 
 HT_SCROLLBAR_ARROW_LINE_1: int
 
 HT_SCROLLBAR_ARROW_LINE_2: int
@@ -44461,26 +44665,34 @@
 
 FD_CHANGE_DIR: int
 
 ID_FILE1: int
 
 ID_FILE9: int
 
+_DragResult: TypeAlias = DragResult
+
 EVT_PAINT: int
 
 DefaultSize: int
 
 EVT_SIZE: int
 
+BackgroundStyle: TypeAlias = int  # Enumeration
+
 BG_STYLE_ERASE: int
 
 BG_STYLE_SYSTEM: int
 
 BG_STYLE_TRANSPARENT: int
 
+Border: TypeAlias = int  # Enumeration
+
+ShowEffect: TypeAlias = int  # Enumeration
+
 SHOW_EFFECT_ROLL_TO_LEFT: int
 
 SHOW_EFFECT_ROLL_TO_RIGHT: int
 
 SHOW_EFFECT_ROLL_TO_TOP: int
 
 SHOW_EFFECT_ROLL_TO_BOTTOM: int
@@ -44495,34 +44707,42 @@
 
 SHOW_EFFECT_MAX: int
 
 VERTICAL: int
 
 HORIZONTAL: int
 
+UpdateUI: TypeAlias = int  # Enumeration
+
 UPDATE_UI_NONE: int
 
 UPDATE_UI_RECURSE: int
 
+EllipsizeMode: TypeAlias = int  # Enumeration
+
 ELLIPSIZE_NONE: int
 
 ELLIPSIZE_START: int
 
 ELLIPSIZE_MIDDLE: int
 
 ELLIPSIZE_END: int
 
+EllipsizeFlags: TypeAlias = int  # Enumeration
+
 ELLIPSIZE_FLAGS_NONE: int
 
 ELLIPSIZE_FLAGS_PROCESS_MNEMONICS: int
 
 ELLIPSIZE_FLAGS_EXPAND_TABS: int
 
 ELLIPSIZE_FLAGS_DEFAULT: int
 
+DataFormatId: TypeAlias = int  # Enumeration
+
 DF_SYLK: int
 
 DF_DIF: int
 
 DF_TIFF: int
 
 DF_OEMTEXT: int
@@ -44541,52 +44761,70 @@
 
 DF_LOCALE: int
 
 DF_PRIVATE: int
 
 DF_MAX: int
 
+HeaderSortIconType: TypeAlias = int  # Enumeration
+
 HDR_SORT_ICON_NONE: int
 
 HDR_SORT_ICON_UP: int
 
 HDR_SORT_ICON_DOWN: int
 
+Orientation: TypeAlias = int  # Enumeration
+
 ORIENTATION_MASK: int
 
 DIALOG_ADAPTATION_MODE_DEFAULT: int
 
 DIALOG_ADAPTATION_MODE_ENABLED: int
 
 DIALOG_ADAPTATION_MODE_DISABLED: int
 
+DialogLayoutAdaptationMode: TypeAlias = int  # Enumeration
+
 DIALOG_ADAPTATION_MODE_DEFAULT: int
 
 DIALOG_ADAPTATION_MODE_ENABLED: int
 
 DIALOG_ADAPTATION_MODE_DISABLED: int
 
+EventCategory: TypeAlias = int  # Enumeration
+
+FileHistoryMenuPathStyle: TypeAlias = int  # Enumeration
+
 FH_PATH_SHOW_IF_DIFFERENT: int
 
 FH_PATH_SHOW_NEVER: int
 
 FH_PATH_SHOW_ALWAYS: int
 
+FileSystemOpenFlags: TypeAlias = int  # Enumeration
+
+FSWWarningType: TypeAlias = int  # Enumeration
+
 FSW_WARNING_NONE: int
 
 FSW_WARNING_GENERAL: int
 
 FSW_WARNING_OVERFLOW: int
 
+FindReplaceFlags: TypeAlias = int  # Enumeration
+
 FR_DOWN: int
 
 FR_WHOLEWORD: int
 
 FR_MATCHCASE: int
 
+FlexSizerGrowMode: TypeAlias = int  # Enumeration
+
 DEFAULT: int
 
 DECORATIVE: int
 
 ROMAN: int
 
 SCRIPT: int
@@ -44617,28 +44855,32 @@
 
 FONTENCODING_CP1251: int
 
 FONTENCODING_CP1250: int
 
 FONTENCODING_CP1252: int
 
+FontSymbolicSize: TypeAlias = int  # Enumeration
+
 FONTSIZE_XX_SMALL: int
 
 FONTSIZE_X_SMALL: int
 
 FONTSIZE_SMALL: int
 
 FONTSIZE_MEDIUM: int
 
 FONTSIZE_LARGE: int
 
 FONTSIZE_X_LARGE: int
 
 FONTSIZE_XX_LARGE: int
 
+FontFlag: TypeAlias = int  # Enumeration
+
 FONTFLAG_DEFAULT: int
 
 FONTFLAG_ITALIC: int
 
 FONTFLAG_SLANT: int
 
 FONTFLAG_LIGHT: int
@@ -44651,18 +44893,24 @@
 
 FONTFLAG_UNDERLINED: int
 
 FONTFLAG_STRIKETHROUGH: int
 
 FONTFLAG_MASK: int
 
+PolygonFillMode: TypeAlias = int  # Enumeration
+
+AntialiasMode: TypeAlias = int  # Enumeration
+
 ANTIALIAS_NONE: int
 
 ANTIALIAS_DEFAULT: int
 
+CompositionMode: TypeAlias = int  # Enumeration
+
 COMPOSITION_INVALID: int
 
 COMPOSITION_CLEAR: int
 
 COMPOSITION_SOURCE: int
 
 COMPOSITION_OVER: int
@@ -44685,24 +44933,28 @@
 
 COMPOSITION_XOR: int
 
 COMPOSITION_ADD: int
 
 COMPOSITION_DIFF: int
 
+InterpolationQuality: TypeAlias = int  # Enumeration
+
 INTERPOLATION_DEFAULT: int
 
 INTERPOLATION_NONE: int
 
 INTERPOLATION_FAST: int
 
 INTERPOLATION_GOOD: int
 
 INTERPOLATION_BEST: int
 
+PenStyle: TypeAlias = int  # Enumeration
+
 PENSTYLE_INVALID: int
 
 PENSTYLE_SOLID: int
 
 PENSTYLE_DOT: int
 
 PENSTYLE_LONG_DASH: int
@@ -44731,128 +44983,164 @@
 
 PENSTYLE_VERTICAL_HATCH: int
 
 PENSTYLE_FIRST_HATCH: int
 
 PENSTYLE_LAST_HATCH: int
 
+PenCap: TypeAlias = int  # Enumeration
+
 CAP_INVALID: int
 
 CAP_ROUND: int
 
 CAP_PROJECTING: int
 
 CAP_BUTT: int
 
+PenJoin: TypeAlias = int  # Enumeration
+
 JOIN_INVALID: int
 
 JOIN_BEVEL: int
 
 JOIN_MITER: int
 
 JOIN_ROUND: int
 
+PenQuality: TypeAlias = int  # Enumeration
+
 PEN_QUALITY_DEFAULT: int
 
 PEN_QUALITY_LOW: int
 
 PEN_QUALITY_HIGH: int
 
+GradientType: TypeAlias = int  # Enumeration
+
 GRADIENT_NONE: int
 
 GRADIENT_LINEAR: int
 
 GRADIENT_RADIAL: int
 
+Alignment: TypeAlias = int  # Enumeration
+
 ALIGN_INVALID: int
 
 ALIGN_MASK: int
 
+_EllipsizeMode: TypeAlias = EllipsizeMode
+
+_DataFormat: TypeAlias = DataFormat
+
+HelpSearchMode: TypeAlias = int  # Enumeration
+
 HELP_SEARCH_INDEX: int
 
 HELP_SEARCH_ALL: int
 
+IdleMode: TypeAlias = int  # Enumeration
+
+ImageAlphaBlendMode: TypeAlias = int  # Enumeration
+
 IMAGE_ALPHA_BLEND_OVER: int
 
 IMAGE_ALPHA_BLEND_COMPOSE: int
 
+ImageResizeQuality: TypeAlias = int  # Enumeration
+
 IMAGE_QUALITY_NEAREST: int
 
 IMAGE_QUALITY_BILINEAR: int
 
 IMAGE_QUALITY_BICUBIC: int
 
 IMAGE_QUALITY_BOX_AVERAGE: int
 
 IMAGE_QUALITY_NORMAL: int
 
 IMAGE_QUALITY_HIGH: int
 
+KeyModifier: TypeAlias = int  # Enumeration
+
 MOD_NONE: int
 
 MOD_ALTGR: int
 
 MOD_META: int
 
 MOD_RAW_CONTROL: int
 
 MOD_CMD: int
 
 MOD_ALL: int
 
+KeyCategoryFlags: TypeAlias = int  # Enumeration
+
 WXK_CATEGORY_ARROW: int
 
 WXK_CATEGORY_PAGING: int
 
 WXK_CATEGORY_JUMP: int
 
 WXK_CATEGORY_TAB: int
 
 WXK_CATEGORY_CUT: int
 
 WXK_CATEGORY_NAVIGATION: int
 
+ListColumnFormat: TypeAlias = int  # Enumeration
+
 LIST_FORMAT_LEFT: int
 
 LIST_FORMAT_RIGHT: int
 
 LIST_FORMAT_CENTRE: int
 
 LIST_FORMAT_CENTER: int
 
+LocaleInfo: TypeAlias = int  # Enumeration
+
 LOCALE_THOUSANDS_SEP: int
 
 LOCALE_DECIMAL_POINT: int
 
 LOCALE_SHORT_DATE_FMT: int
 
 LOCALE_LONG_DATE_FMT: int
 
 LOCALE_DATE_TIME_FMT: int
 
 LOCALE_TIME_FMT: int
 
+LocaleCategory: TypeAlias = int  # Enumeration
+
 LOCALE_CAT_NUMBER: int
 
 LOCALE_CAT_DATE: int
 
 LOCALE_CAT_MONEY: int
 
+ItemKind: TypeAlias = int  # Enumeration
+
 ITEM_SEPARATOR: int
 
 ITEM_NORMAL: int
 
 ITEM_CHECK: int
 
 ITEM_RADIO: int
 
 ITEM_DROPDOWN: int
 
 ITEM_MAX: int
 
+MouseButton: TypeAlias = int  # Enumeration
+
 MOUSE_BTN_ANY: int
 
 MOUSE_BTN_NONE: int
 
 MOUSE_BTN_LEFT: int
 
 MOUSE_BTN_MIDDLE: int
@@ -44861,18 +45149,24 @@
 
 MOUSE_BTN_AUX1: int
 
 MOUSE_BTN_AUX2: int
 
 MOUSE_BTN_MAX: int
 
+MouseWheelAxis: TypeAlias = int  # Enumeration
+
 MOUSE_WHEEL_VERTICAL: int
 
 MOUSE_WHEEL_HORIZONTAL: int
 
+_VersionInfo: TypeAlias = VersionInfo
+
+PaperSize: TypeAlias = int  # Enumeration
+
 PAPER_10X11: int
 
 PAPER_10X14: int
 
 PAPER_11X17: int
 
 PAPER_12X11: int
@@ -45099,44 +45393,54 @@
 
 PAPER_STATEMENT: int
 
 PAPER_TABLOID: int
 
 PAPER_TABLOID_EXTRA: int
 
+Bitness: TypeAlias = int  # Enumeration
+
 BITNESS_INVALID: int
 
 BITNESS_32: int
 
 BITNESS_64: int
 
 BITNESS_MAX: int
 
+Endianness: TypeAlias = int  # Enumeration
+
 ENDIAN_INVALID: int
 
 ENDIAN_BIG: int
 
 ENDIAN_LITTLE: int
 
 ENDIAN_PDP: int
 
 ENDIAN_MAX: int
 
+Architecture: TypeAlias = int  # Enumeration
+
 ARCH_INVALID: int
 
 ARCH_32: int
 
 ARCH_64: int
 
 ARCH_MAX: int
 
+PowerResourceKind: TypeAlias = int  # Enumeration
+
 POWER_RESOURCE_SCREEN: int
 
 POWER_RESOURCE_SYSTEM: int
 
+PrintBin: TypeAlias = int  # Enumeration
+
 PRINTBIN_DEFAULT: int
 
 PRINTBIN_ONLYONE: int
 
 PRINTBIN_LOWER: int
 
 PRINTBIN_MIDDLE: int
@@ -45159,50 +45463,70 @@
 
 PRINTBIN_CASSETTE: int
 
 PRINTBIN_FORMSOURCE: int
 
 PRINTBIN_USER: int
 
+DuplexMode: TypeAlias = int  # Enumeration
+
+PrintOrientation: TypeAlias = int  # Enumeration
+
+PrintMode: TypeAlias = int  # Enumeration
+
 PRINT_MODE_NONE: int
 
 PRINT_MODE_PREVIEW: int
 
 PRINT_MODE_FILE: int
 
 PRINT_MODE_PRINTER: int
 
 PRINT_MODE_STREAM: int
 
+PrinterError: TypeAlias = int  # Enumeration
+
+AppAssertMode: TypeAlias = int  # Enumeration
+
 APP_ASSERT_SUPPRESS: int
 
 APP_ASSERT_EXCEPTION: int
 
 APP_ASSERT_DIALOG: int
 
 APP_ASSERT_LOG: int
 
+ScrollbarVisibility: TypeAlias = int  # Enumeration
+
 SP_3D: int
 
+SplitMode: TypeAlias = int  # Enumeration
+
+StreamError: TypeAlias = int  # Enumeration
+
 STREAM_NO_ERROR: int
 
 STREAM_EOF: int
 
 STREAM_WRITE_ERROR: int
 
 STREAM_READ_ERROR: int
 
+SVGShapeRenderingMode: TypeAlias = int  # Enumeration
+
 SVG_SHAPE_RENDERING_OPTIMIZE_SPEED: int
 
 SVG_SHAPE_RENDERING_CRISP_EDGES: int
 
 SVG_SHAPE_RENDERING_GEOMETRIC_PRECISION: int
 
 SVG_SHAPE_RENDERING_OPTIMISE_SPEED: int
 
+SystemColour: TypeAlias = int  # Enumeration
+
 SYS_COLOUR_SCROLLBAR: int
 
 SYS_COLOUR_DESKTOP: int
 
 SYS_COLOUR_ACTIVECAPTION: int
 
 SYS_COLOUR_INACTIVECAPTION: int
@@ -45275,26 +45599,30 @@
 
 SYS_COLOUR_3DHIGHLIGHT: int
 
 SYS_COLOUR_3DHILIGHT: int
 
 SYS_COLOUR_FRAMEBK: int
 
+SystemFont: TypeAlias = int  # Enumeration
+
 SYS_OEM_FIXED_FONT: int
 
 SYS_ANSI_FIXED_FONT: int
 
 SYS_ANSI_VAR_FONT: int
 
 SYS_SYSTEM_FONT: int
 
 SYS_DEVICE_DEFAULT_FONT: int
 
 SYS_DEFAULT_GUI_FONT: int
 
+SystemMetric: TypeAlias = int  # Enumeration
+
 SYS_MOUSE_BUTTONS: int
 
 SYS_BORDER_X: int
 
 SYS_BORDER_Y: int
 
 SYS_CURSOR_Y: int
@@ -45365,46 +45693,56 @@
 
 SYS_CARET_ON_MSEC: int
 
 SYS_CARET_OFF_MSEC: int
 
 SYS_CARET_TIMEOUT_MSEC: int
 
+SystemScreenType: TypeAlias = int  # Enumeration
+
 SYS_SCREEN_NONE: int
 
 SYS_SCREEN_TINY: int
 
 SYS_SCREEN_PDA: int
 
 SYS_SCREEN_SMALL: int
 
 SYS_SCREEN_DESKTOP: int
 
+SystemFeature: TypeAlias = int  # Enumeration
+
 SYS_CAN_DRAW_FRAME_DECORATIONS: int
 
 SYS_CAN_ICONIZE_FRAME: int
 
 SYS_TABLET_PRESENT: int
 
+TextAttrLineSpacing: TypeAlias = int  # Enumeration
+
 TEXT_ATTR_LINE_SPACING_NORMAL: int
 
 TEXT_ATTR_LINE_SPACING_HALF: int
 
 TEXT_ATTR_LINE_SPACING_TWICE: int
 
+TextAttrAlignment: TypeAlias = int  # Enumeration
+
 TEXT_ALIGNMENT_DEFAULT: int
 
 TEXT_ALIGNMENT_LEFT: int
 
 TEXT_ALIGNMENT_CENTRE: int
 
 TEXT_ALIGNMENT_CENTER: int
 
 TEXT_ALIGNMENT_RIGHT: int
 
+TextAttrBulletStyle: TypeAlias = int  # Enumeration
+
 TEXT_ATTR_BULLET_STYLE_NONE: int
 
 TEXT_ATTR_BULLET_STYLE_ARABIC: int
 
 TEXT_ATTR_BULLET_STYLE_LETTERS_UPPER: int
 
 TEXT_ATTR_BULLET_STYLE_LETTERS_LOWER: int
@@ -45427,16 +45765,20 @@
 
 TEXT_ATTR_BULLET_STYLE_ALIGN_RIGHT: int
 
 TEXT_ATTR_BULLET_STYLE_ALIGN_CENTRE: int
 
 TEXT_ATTR_BULLET_STYLE_CONTINUATION: int
 
+TextAttrUnderlineType: TypeAlias = int  # Enumeration
+
 TEXT_ATTR_UNDERLINE_NONE: int
 
+TextAttrFlags: TypeAlias = int  # Enumeration
+
 TEXT_ATTR_TEXT_COLOUR: int
 
 TEXT_ATTR_BACKGROUND_COLOUR: int
 
 TEXT_ATTR_FONT_FACE: int
 
 TEXT_ATTR_FONT_POINT_SIZE: int
@@ -45499,14 +45841,16 @@
 
 TEXT_ATTR_CHARACTER: int
 
 TEXT_ATTR_PARAGRAPH: int
 
 TEXT_ATTR_ALL: int
 
+TextAttrEffects: TypeAlias = int  # Enumeration
+
 TEXT_ATTR_EFFECT_NONE: int
 
 TEXT_ATTR_EFFECT_SMALL_CAPITALS: int
 
 TEXT_ATTR_EFFECT_DOUBLE_STRIKETHROUGH: int
 
 TEXT_ATTR_EFFECT_SHADOW: int
@@ -45517,39 +45861,147 @@
 
 TEXT_ATTR_EFFECT_ENGRAVE: int
 
 TEXT_ATTR_EFFECT_RTL: int
 
 TEXT_ATTR_EFFECT_SUPPRESS_HYPHENATION: int
 
+TextCtrlHitTestResult: TypeAlias = int  # Enumeration
+
 TE_HT_UNKNOWN: int
 
 TE_HT_BEFORE: int
 
 TE_HT_ON_TEXT: int
 
 TE_HT_BELOW: int
 
 TE_HT_BEYOND: int
 
+ContentProtection: TypeAlias = int  # Enumeration
+
 CONTENT_PROTECTION_NONE: int
 
 CONTENT_PROTECTION_ENABLED: int
 
 EVT_TREE_ITEM_EXPANDING: int
 
+UpdateUIMode: TypeAlias = int  # Enumeration
+
+_FileSystem: TypeAlias = FileSystem
+
 ID_NONE: int
 
+_SizerItem: TypeAlias = SizerItem
+
+TextFileType: TypeAlias = int  # Enumeration
+
 def HtmlWinParser_AddTagHandler(tagHandlerClass) -> None:
     """ 
 
         Source: https://docs.wxpython.org/wx.html.functions.html
     """
 
 
+Coord: TypeAlias = Any
+
+Char: TypeAlias = Any
+
+Double: TypeAlias = Any
+
+CommandList: TypeAlias = Any
+
+WindowList: TypeAlias = list['Window']  # WindowList is a type-safe List-like class whose elements are of type Window* .
+
+intshort: TypeAlias = int
+
+FileHistoryMenuList: TypeAlias = 'Menu'
+
+MessageDialogButtonLabel: TypeAlias = str
+
+SizerItemList: TypeAlias = list['SizerItem']
+
+Edge: TypeAlias = int
+
+MenuItemList: TypeAlias = list['MenuItem']
+
+ObjectRefData: TypeAlias = Any
+
+PrintQuality: TypeAlias = int
+
+Point2DDouble: TypeAlias = Any
+
+TextPos: TypeAlias = int
+
+ClientData: TypeAlias = Any
+
+PyUserData: TypeAlias = Any
+
+FileOffset: TypeAlias = int
+
+WeekDay: TypeAlias = int
+
+value_type: TypeAlias = bytes
+
+Byte: TypeAlias = bytes
+
+Reason: TypeAlias = int
+
+ArtClient: TypeAlias = Any
+
+Vector: TypeAlias = Any
+
+EntryType: TypeAlias = int
+
+LongLong_t: TypeAlias = Any
+
+Country: TypeAlias = wx.DateTime.Country  # Enumeration
+
+ArrayVideoModes: TypeAlias = list['VideoMode']
+
+MsgCatalog: TypeAlias = Any
+
+SIP_SSIZE_T: TypeAlias = int
+
+RGBValue: TypeAlias = 'Image.RGBValue'
+
+HSVValue: TypeAlias = 'Image.HSVValue'
+
+Relationship: TypeAlias = int  # Enumeration
+
+LogLevel: TypeAlias = int  # Enumeration
+
+PlatformInfo: TypeAlias = PlatformInformation
+
+PreviewFrameModalityKind: TypeAlias = int  # Enumeration
+
+Rect2DDouble: TypeAlias = Any
+
+OutCode: TypeAlias = int  # Enumeration
+
+RegionContain: TypeAlias = int  # Enumeration
+
+Dir: TypeAlias = 'StandardPaths.Dir'  # Enumeration
+
+FileLayout: TypeAlias = 'StandardPaths.FileLayout'  # Enumeration
+
+ScaleMode: TypeAlias = 'StaticBitmap.ScaleMode'  # Enumeration
+
+Kind: TypeAlias = 'StockPreferencesPage.Kind'  # Enumeration
+
+res: TypeAlias = Any
+
+void: TypeAlias = Any
+
+Uint16: TypeAlias = int
+
+MemoryBuffer: TypeAlias = Any
+
+Calendar: TypeAlias = int  # Enumeration
+
 GROW: int  # Synonym of wx.EXPAND
 
 RA_HORIZONTAL: int  # Synonym of wx.HORIZONTAL
 
 RA_VERTICAL: int  # Synonym of wx.VERTICAL
 
 NORMAL: int
@@ -45558,18 +46010,14 @@
 
 wxEVT_COMMAND_BUTTON_CLICKED: int
 
 RED: int
 
 YELLOW: int
 
-BLACK: int
-
-WHITE: int
-
 BLUE: int
 
 GREEN: int
 
 CYAN: int
 
 OPEN: int
```

### Comparing `types_wxpython-0.6.1/wx-stubs/adv/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/adv/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class CommandLinkButton(Button):
     """ Objects of this class are similar in appearance to the normal
 Buttons but are similar to the links in a web page in functionality.
 
         Source: https://docs.wxpython.org/wx.adv.CommandLinkButton.html
     """
@@ -16,15 +16,15 @@
     def Create(self, parent, id=ID_ANY, mainLabel="", note="", pos=DefaultPosition, size=DefaultSize, style=0, validator=DefaultValidator, name=ButtonNameStr) -> bool:
         """ Button creation function for two-step creation.
 
             Source: https://docs.wxpython.org/wx.adv.CommandLinkButton.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.CommandLinkButton.html
         """
 
     def GetLabel(self) -> str:
         """ Returns the string label for the button.
@@ -91,75 +91,75 @@
     def Create(self, parent, id=ID_ANY, label="", pos=DefaultPosition, size=DefaultSize, style=EL_DEFAULT_STYLE, name=EditableListBoxNameStr) -> bool:
         """ Creates the editable listbox for two-step construction.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
-    def GetDelButton(self) -> BitmapButton:
+    def GetDelButton(self) -> 'BitmapButton':
         """ Returns a reference to the delete button used in the EditableListBox.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
-    def GetDownButton(self) -> BitmapButton:
+    def GetDownButton(self) -> 'BitmapButton':
         """ Returns a reference to the down button used in the EditableListBox.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
-    def GetEditButton(self) -> BitmapButton:
+    def GetEditButton(self) -> 'BitmapButton':
         """ Returns a reference to the edit button used in the EditableListBox.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
-    def GetListCtrl(self) -> ListCtrl:
+    def GetListCtrl(self) -> 'ListCtrl':
         """ Returns a reference to the listctrl used in the EditableListBox.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
-    def GetNewButton(self) -> BitmapButton:
+    def GetNewButton(self) -> 'BitmapButton':
         """ Returns a reference to the new button used in the EditableListBox.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
     def GetStrings(self) -> list[str]:
         """ Returns a list of the current contents of the control.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
-    def GetUpButton(self) -> BitmapButton:
+    def GetUpButton(self) -> 'BitmapButton':
         """ Returns a reference to the up button used in the EditableListBox.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
     def SetStrings(self, strings: list[str]) -> None:
         """ Replaces current contents with given strings.
 
             Source: https://docs.wxpython.org/wx.adv.EditableListBox.html
         """
 
-    DelButton: BitmapButton  # See GetDelButton
-    DownButton: BitmapButton  # See GetDownButton
-    EditButton: BitmapButton  # See GetEditButton
-    ListCtrl: ListCtrl  # See GetListCtrl
-    NewButton: BitmapButton  # See GetNewButton
+    DelButton: 'BitmapButton'  # See GetDelButton
+    DownButton: 'BitmapButton'  # See GetDownButton
+    EditButton: 'BitmapButton'  # See GetEditButton
+    ListCtrl: '_ListCtrl'  # See GetListCtrl
+    NewButton: 'BitmapButton'  # See GetNewButton
     Strings: list[str]  # See GetStrings and SetStrings
-    UpButton: BitmapButton  # See GetUpButton
+    UpButton: 'BitmapButton'  # See GetUpButton
 
 
 
 EL_ALLOW_NEW: int  # Allows the user to enter new strings.
 
 EL_ALLOW_EDIT: int  # Allows the user to edit existing strings.
 
@@ -183,15 +183,15 @@
     def Create(self, parent, id=ID_ANY, value="", pos=DefaultPosition, size=DefaultSize, choices=[], style=0, validator=DefaultValidator, name=ComboBoxNameStr) -> bool:
         """ Creates the combobox for two-step construction.
 
             Source: https://docs.wxpython.org/wx.adv.OwnerDrawnComboBox.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.OwnerDrawnComboBox.html
         """
 
     def GetWidestItem(self) -> int:
         """ Returns index to the widest item in the list.
@@ -287,22 +287,22 @@
 
     def FindString(self, string, caseSensitive=False) -> int:
         """ Finds an item whose label matches the given string.
 
             Source: https://docs.wxpython.org/wx.adv.BitmapComboBox.html
         """
 
-    def GetBitmapSize(self) -> Size:
+    def GetBitmapSize(self) -> 'Size':
         """ Returns the size of the bitmaps used in the combo box.
 
             Source: https://docs.wxpython.org/wx.adv.BitmapComboBox.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.BitmapComboBox.html
         """
 
     def GetCount(self) -> int:
         """ Returns the number of items in the control.
@@ -312,15 +312,15 @@
 
     def GetInsertionPoint(self) -> int:
         """ Same as wx.TextEntry.GetInsertionPoint .
 
             Source: https://docs.wxpython.org/wx.adv.BitmapComboBox.html
         """
 
-    def GetItemBitmap(self, n: int) -> Bitmap:
+    def GetItemBitmap(self, n: int) -> 'Bitmap':
         """ Returns the bitmap of the item with the given index.
 
             Source: https://docs.wxpython.org/wx.adv.BitmapComboBox.html
         """
 
     def GetSelection(self) -> int:
         """ Returns the index of the selected item or  NOT_FOUND   if no item is selected.
@@ -390,15 +390,15 @@
 
     def SetValue(self, text: str) -> None:
         """ Sets the text for the combobox text field.
 
             Source: https://docs.wxpython.org/wx.adv.BitmapComboBox.html
         """
 
-    BitmapSize: Size  # See GetBitmapSize
+    BitmapSize: 'Size'  # See GetBitmapSize
     Count: int  # See GetCount
     InsertionPoint: int  # See GetInsertionPoint
     Selection: int  # See GetSelection and SetSelection
 
 
 
 CB_SORT: int  # Sorts the entries in the list alphabetically.
@@ -419,15 +419,15 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.adv.DateEvent.html
         """
 
-    def GetDate(self) -> DateTime:
+    def GetDate(self) -> 'DateTime':
         """ Returns the date.
 
             Source: https://docs.wxpython.org/wx.adv.DateEvent.html
         """
 
     def PyGetDate(self) -> None:
         """ Return the date as a Python datetime.date object.
@@ -482,15 +482,15 @@
     """
     def __init__(self, id=0, edge=SASH_NONE) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.adv.SashEvent.html
         """
 
-    def GetDragRect(self) -> Rect:
+    def GetDragRect(self) -> 'Rect':
         """ Returns the rectangle representing the new size the window would be if the resize was applied.
 
             Source: https://docs.wxpython.org/wx.adv.SashEvent.html
         """
 
     def GetDragStatus(self) -> 'adv.SashDragStatus':
         """ Returns the status of the sash: one of wx.adv.SASH_STATUS_OK, wx.adv.SASH_STATUS_OUT_OF_RANGE.
@@ -519,16 +519,16 @@
     def SetEdge(self, edge: SashEdgePosition) -> None:
         """ edge (SashEdgePosition) â
 
             Source: https://docs.wxpython.org/wx.adv.SashEvent.html
         """
 
     DragRect: 'Rect'  # See GetDragRect and SetDragRect
-    DragStatus: SashDragStatus  # See GetDragStatus and SetDragStatus
-    Edge: SashEdgePosition  # See GetEdge and SetEdge
+    DragStatus: 'adv.SashDragStatus'  # See GetDragStatus and SetDragStatus
+    Edge: 'adv.SashEdgePosition'  # See GetEdge and SetEdge
 
 
 
 EVT_SASH_DRAGGED: int  # Process a  wxEVT_SASH_DRAGGED   event, when the user has finished dragging a sash.
 
 EVT_SASH_DRAGGED_RANGE: int  # Process a  wxEVT_SASH_DRAGGED_RANGE   event, when the user has finished dragging a sash. The event handler is called when windows with ids in the given range have their sashes dragged. ^^
 
@@ -560,15 +560,15 @@
     def Create(self, parent, winid=ID_ANY, dir=LEFT, pos=DefaultPosition, size=DefaultSize, style=0, name=BannerWindowNameStr) -> bool:
         """ Really create the banner window for the objects created using the default constructor.
 
             Source: https://docs.wxpython.org/wx.adv.BannerWindow.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.BannerWindow.html
         """
 
     def SetBitmap(self, bmp: 'BitmapBundle') -> None:
         """ Provide the bitmap to use as background.
@@ -607,15 +607,15 @@
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.adv.SashWindow.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.SashWindow.html
         """
 
     def GetDefaultBorderSize(self) -> int:
         """ Gets the default sash border size.
@@ -769,21 +769,21 @@
     def GetAnimation(self) -> 'adv.Animation':
         """ Returns the animation associated with this control.
 
             Source: https://docs.wxpython.org/wx.adv.AnimationCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.AnimationCtrl.html
         """
 
-    def GetInactiveBitmap(self) -> Bitmap:
+    def GetInactiveBitmap(self) -> 'Bitmap':
         """ Returns the inactive bitmap shown in this control when the; see SetInactiveBitmap   for more info.
 
             Source: https://docs.wxpython.org/wx.adv.AnimationCtrl.html
         """
 
     def IsPlaying(self) -> bool:
         """ Returns True if the animation is being played.
@@ -824,15 +824,15 @@
     def Stop(self) -> None:
         """ Stops playing the animation.
 
             Source: https://docs.wxpython.org/wx.adv.AnimationCtrl.html
         """
 
     Animation: 'adv.Animation'  # See GetAnimation and SetAnimation
-    InactiveBitmap: 'BitmapBundle'  # See GetInactiveBitmap and SetInactiveBitmap
+    InactiveBitmap: 'Bitmap'  # See GetInactiveBitmap and SetInactiveBitmap
 
 
 
 AC_DEFAULT_STYLE: int  # The default style: wx.BORDER_NONE.
 
 AC_NO_AUTORESIZE: int  # By default, the control will adjust its size to exactly fit to the size of the animation when SetAnimation is called. If this style flag is given, the control will not change its size ^^
 
@@ -870,63 +870,63 @@
     def GetAttr(self, day: int) -> 'adv.CalendarDateAttr':
         """ Returns the attribute for the given date (should be in the range 1â¦31).
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
-    def GetDate(self) -> DateTime:
+    def GetDate(self) -> 'DateTime':
         """ Gets the currently selected date.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
     def GetDateRange(self) -> tuple:
         """ Returns the limits currently being used.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
-    def GetHeaderColourBg(self) -> Colour:
+    def GetHeaderColourBg(self) -> 'Colour':
         """ Gets the background colour of the header part of the calendar window.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
-    def GetHeaderColourFg(self) -> Colour:
+    def GetHeaderColourFg(self) -> 'Colour':
         """ Gets the foreground colour of the header part of the calendar window.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
-    def GetHighlightColourBg(self) -> Colour:
+    def GetHighlightColourBg(self) -> 'Colour':
         """ Gets the background highlight colour.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
-    def GetHighlightColourFg(self) -> Colour:
+    def GetHighlightColourFg(self) -> 'Colour':
         """ Gets the foreground highlight colour.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
-    def GetHolidayColourBg(self) -> Colour:
+    def GetHolidayColourBg(self) -> 'Colour':
         """ Return the background colour currently used for holiday highlighting.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
-    def GetHolidayColourFg(self) -> Colour:
+    def GetHolidayColourFg(self) -> 'Colour':
         """ Return the foreground colour currently used for holiday highlighting.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
     def HitTest(self, pos: Union[tuple[int, int], 'Point']) -> tuple:
         """ Returns one of CalendarHitTestResult constants and fills either date  or wd  pointer with the corresponding value depending on the hit test code.
@@ -992,20 +992,20 @@
         """ Sets the colours to be used for the holidays highlighting.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarCtrl.html
         """
 
     Date: 'DateTime'  # See GetDate and SetDate
     DateRange: tuple  # See GetDateRange and SetDateRange
-    HeaderColourBg: Colour  # See GetHeaderColourBg
-    HeaderColourFg: Colour  # See GetHeaderColourFg
-    HighlightColourBg: Colour  # See GetHighlightColourBg
-    HighlightColourFg: Colour  # See GetHighlightColourFg
-    HolidayColourBg: Colour  # See GetHolidayColourBg
-    HolidayColourFg: Colour  # See GetHolidayColourFg
+    HeaderColourBg: 'Colour'  # See GetHeaderColourBg
+    HeaderColourFg: 'Colour'  # See GetHeaderColourFg
+    HighlightColourBg: 'Colour'  # See GetHighlightColourBg
+    HighlightColourFg: 'Colour'  # See GetHighlightColourFg
+    HolidayColourBg: 'Colour'  # See GetHolidayColourBg
+    HolidayColourFg: 'Colour'  # See GetHolidayColourFg
 
 
 
 CAL_SUNDAY_FIRST: int  # Show Sunday as the first day in the week (not in wxGTK)
 
 CAL_MONDAY_FIRST: int  # Show Monday as the first day in the week (not in wxGTK)
 
@@ -1045,27 +1045,27 @@
     def Create(self, parent, id=ID_ANY, dt=DefaultDateTime, pos=DefaultPosition, size=DefaultSize, style=DP_DEFAULT|DP_SHOWCENTURY, validator=DefaultValidator, name="datectrl") -> bool:
         """ Create the control window.
 
             Source: https://docs.wxpython.org/wx.adv.DatePickerCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.DatePickerCtrl.html
         """
 
     def GetRange(self) -> tuple:
         """ If the control had been previously limited to a range of dates using SetRange , returns the lower and upper bounds of this range.
 
             Source: https://docs.wxpython.org/wx.adv.DatePickerCtrl.html
         """
 
-    def GetValue(self) -> DateTime:
+    def GetValue(self) -> 'DateTime':
         """ Returns the currently entered date.
 
             Source: https://docs.wxpython.org/wx.adv.DatePickerCtrl.html
         """
 
     def SetNullText(self, text: str) -> None:
         """ Set the text to show when there is no valid value.
@@ -1115,27 +1115,27 @@
     def Create(self, parent, id=ID_ANY, label="", url="", pos=DefaultPosition, size=DefaultSize, style=HL_DEFAULT_STYLE, name=HyperlinkCtrlNameStr) -> bool:
         """ Creates the hyperlink control.
 
             Source: https://docs.wxpython.org/wx.adv.HyperlinkCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.HyperlinkCtrl.html
         """
 
-    def GetHoverColour(self) -> Colour:
+    def GetHoverColour(self) -> 'Colour':
         """ Returns the colour used to print the label of the hyperlink when the mouse is over the control.
 
             Source: https://docs.wxpython.org/wx.adv.HyperlinkCtrl.html
         """
 
-    def GetNormalColour(self) -> Colour:
+    def GetNormalColour(self) -> 'Colour':
         """ Returns the colour used to print the label when the link has never been clicked before (i.e. the link has not been visited) and the mouse is not over the control.
 
             Source: https://docs.wxpython.org/wx.adv.HyperlinkCtrl.html
         """
 
     def GetURL(self) -> str:
         """ Returns the URL associated with the hyperlink.
@@ -1145,15 +1145,15 @@
 
     def GetVisited(self) -> bool:
         """ Returns True if the hyperlink has already been clicked by the user at least one time.
 
             Source: https://docs.wxpython.org/wx.adv.HyperlinkCtrl.html
         """
 
-    def GetVisitedColour(self) -> Colour:
+    def GetVisitedColour(self) -> 'Colour':
         """ Returns the colour used to print the label when the mouse is not over the control and the link has already been clicked before (i.e. the link has been visited).
 
             Source: https://docs.wxpython.org/wx.adv.HyperlinkCtrl.html
         """
 
     def SetHoverColour(self, colour: Union[int, str, 'Colour']) -> None:
         """ Sets the colour used to print the label of the hyperlink when the mouse is over the control.
@@ -1181,19 +1181,19 @@
 
     def SetVisitedColour(self, colour: Union[int, str, 'Colour']) -> None:
         """ Sets the colour used to print the label when the mouse is not over the control and the link has already been clicked before (i.e. the link has been visited).
 
             Source: https://docs.wxpython.org/wx.adv.HyperlinkCtrl.html
         """
 
-    HoverColour: Union[int, str, 'Colour']  # See GetHoverColour and SetHoverColour
-    NormalColour: Union[int, str, 'Colour']  # See GetNormalColour and SetNormalColour
+    HoverColour: 'Colour'  # See GetHoverColour and SetHoverColour
+    NormalColour: 'Colour'  # See GetNormalColour and SetNormalColour
     URL: str  # See GetURL and SetURL
     Visited: bool  # See GetVisited and SetVisited
-    VisitedColour: Union[int, str, 'Colour']  # See GetVisitedColour and SetVisitedColour
+    VisitedColour: 'Colour'  # See GetVisitedColour and SetVisitedColour
 
 
 
 HL_ALIGN_LEFT: int  # Align the text to the left.
 
 HL_ALIGN_RIGHT: int  # Align the text to the right. This style is not supported under Windows.
 
@@ -1217,27 +1217,27 @@
     def Create(self, parent, id=ID_ANY, dt=DefaultDateTime, pos=DefaultPosition, size=DefaultSize, style=TP_DEFAULT, validator=DefaultValidator, name=TimePickerCtrlNameStr) -> bool:
         """ Create the control window.
 
             Source: https://docs.wxpython.org/wx.adv.TimePickerCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.TimePickerCtrl.html
         """
 
     def GetTime(self) -> tuple:
         """ Returns the currently entered time as hours, minutes and seconds.
 
             Source: https://docs.wxpython.org/wx.adv.TimePickerCtrl.html
         """
 
-    def GetValue(self) -> DateTime:
+    def GetValue(self) -> 'DateTime':
         """ Returns the currently entered time.
 
             Source: https://docs.wxpython.org/wx.adv.TimePickerCtrl.html
         """
 
     def SetTime(self, hour, min, sec) -> bool:
         """ Changes the current time of the control.
@@ -1277,46 +1277,46 @@
 
     def Create(self, parent, id=ID_ANY, title="", pos=DefaultPosition, size=DefaultSize, style=DEFAULT_DIALOG_STYLE, name=DialogNameStr) -> bool:
         """ Call this from your own Create function, before adding buttons and pages.
 
             Source: https://docs.wxpython.org/wx.adv.PropertySheetDialog.html
         """
 
-    def CreateBookCtrl(self) -> BookCtrlBase:
+    def CreateBookCtrl(self) -> 'BookCtrlBase':
         """ Override this if you wish to create a different kind of book control; by default, the value passed to SetSheetStyle   is used to determine the control.
 
             Source: https://docs.wxpython.org/wx.adv.PropertySheetDialog.html
         """
 
     def CreateButtons(self, flags: int=OK|CANCEL) -> None:
         """ Call this to create the buttons for the dialog.
 
             Source: https://docs.wxpython.org/wx.adv.PropertySheetDialog.html
         """
 
-    def GetBookCtrl(self) -> BookCtrlBase:
+    def GetBookCtrl(self) -> 'BookCtrlBase':
         """ Returns the book control that will contain your settings pages.
 
             Source: https://docs.wxpython.org/wx.adv.PropertySheetDialog.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.PropertySheetDialog.html
         """
 
-    def GetContentWindow(self) -> Window:
+    def GetContentWindow(self) -> 'Window':
         """ Override this to return a window containing the main content of the dialog.
 
             Source: https://docs.wxpython.org/wx.adv.PropertySheetDialog.html
         """
 
-    def GetInnerSizer(self) -> Sizer:
+    def GetInnerSizer(self) -> 'Sizer':
         """ Returns the inner sizer that contains the book control and button sizer.
 
             Source: https://docs.wxpython.org/wx.adv.PropertySheetDialog.html
         """
 
     def GetSheetInnerBorder(self) -> int:
         """ Returns the border around the book control only.
@@ -1369,15 +1369,15 @@
     def SetSheetStyle(self, style: int) -> None:
         """ You can customize the look and feel of the dialog by setting the sheet style.
 
             Source: https://docs.wxpython.org/wx.adv.PropertySheetDialog.html
         """
 
     BookCtrl: 'BookCtrlBase'  # See GetBookCtrl and SetBookCtrl
-    ContentWindow: Window  # See GetContentWindow
+    ContentWindow: 'Window'  # See GetContentWindow
     InnerSizer: 'Sizer'  # See GetInnerSizer and SetInnerSizer
     SheetInnerBorder: int  # See GetSheetInnerBorder and SetSheetInnerBorder
     SheetOuterBorder: int  # See GetSheetOuterBorder and SetSheetOuterBorder
     SheetStyle: int  # See GetSheetStyle and SetSheetStyle
 
 
 
@@ -1400,34 +1400,34 @@
 
     def FitToPage(self, firstPage: 'adv.WizardPage') -> None:
         """ This method is obsolete, use GetPageAreaSizer   instead.
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
-    def GetBitmap(self) -> Bitmap:
+    def GetBitmap(self) -> 'Bitmap':
         """ Returns the bitmap used for the wizard.
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
-    def GetBitmapBackgroundColour(self) -> Colour:
+    def GetBitmapBackgroundColour(self) -> 'Colour':
         """ Returns the colour that should be used to fill the area not taken up by the wizard or page bitmap, if a non-zero bitmap placement flag has been set.
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
     def GetBitmapPlacement(self) -> int:
         """ Returns the flags indicating how the wizard or page bitmap should be expanded and positioned to fit the page height.
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
     def GetCurrentPage(self) -> 'adv.WizardPage':
         """ Get the current page while the wizard is running.
@@ -1437,21 +1437,21 @@
 
     def GetMinimumBitmapWidth(self) -> int:
         """ Returns the minimum width for the bitmap that will be constructed to contain the actual wizard or page bitmap if a non-zero bitmap placement flag has been set.
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
-    def GetPageAreaSizer(self) -> Sizer:
+    def GetPageAreaSizer(self) -> 'Sizer':
         """ Returns pointer to page area sizer.
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
-    def GetPageSize(self) -> Size:
+    def GetPageSize(self) -> 'Size':
         """ Returns the size available for the pages.
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
     def HasNextPage(self, page: 'adv.WizardPage') -> bool:
         """ Return True if this page is not the last one in the wizard.
@@ -1515,21 +1515,21 @@
 
     def ShowPage(self, page, goingForward=True) -> bool:
         """ Show the given wizard page.
 
             Source: https://docs.wxpython.org/wx.adv.Wizard.html
         """
 
-    Bitmap: 'BitmapBundle'  # See GetBitmap and SetBitmap
-    BitmapBackgroundColour: Union[int, str, 'Colour']  # See GetBitmapBackgroundColour and SetBitmapBackgroundColour
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
+    BitmapBackgroundColour: 'Colour'  # See GetBitmapBackgroundColour and SetBitmapBackgroundColour
     BitmapPlacement: int  # See GetBitmapPlacement and SetBitmapPlacement
     CurrentPage: 'adv.WizardPage'  # See GetCurrentPage
     MinimumBitmapWidth: int  # See GetMinimumBitmapWidth and SetMinimumBitmapWidth
-    PageAreaSizer: Sizer  # See GetPageAreaSizer
-    PageSize: Union[tuple[int, int], 'Size']  # See GetPageSize and SetPageSize
+    PageAreaSizer: 'Sizer'  # See GetPageAreaSizer
+    PageSize: 'Size'  # See GetPageSize and SetPageSize
 
 
 
 EVT_WIZARD_PAGE_CHANGED: int  # The page has just been changed (this event cannot be vetoed).
 
 EVT_WIZARD_PAGE_CHANGING: int  # The page is being changed (this event can be vetoed).
 
@@ -1575,15 +1575,15 @@
 
     def GetFlags(self) -> int:
         """ Returns the flags associated with this event.
 
             Source: https://docs.wxpython.org/wx.adv.CalculateLayoutEvent.html
         """
 
-    def GetRect(self) -> Rect:
+    def GetRect(self) -> 'Rect':
         """ Before the event handler is entered, returns the remaining parent client area that the window could occupy.
 
             Source: https://docs.wxpython.org/wx.adv.CalculateLayoutEvent.html
         """
 
     def SetFlags(self, flags: int) -> None:
         """ Sets the flags associated with this event.
@@ -1594,15 +1594,15 @@
     def SetRect(self, rect: 'Rect') -> None:
         """ Call this to specify the new remaining parent client area, after the space occupied by the window has been subtracted.
 
             Source: https://docs.wxpython.org/wx.adv.CalculateLayoutEvent.html
         """
 
     Flags: int  # See GetFlags and SetFlags
-    Rect: 'Rect'  # See GetRect and SetRect
+    Rect: '_Rect'  # See GetRect and SetRect
 
 
 
 EVT_CALCULATE_LAYOUT: int  # Process a  wxEVT_CALCULATE_LAYOUT   event, which asks the window to take a âbiteâ out of a rectangle provided by the algorithm. ^^
 
 class QueryLayoutInfoEvent(Event):
     """ This event is sent when LayoutAlgorithm wishes to get the size,
@@ -1636,15 +1636,15 @@
 
     def GetRequestedLength(self) -> int:
         """ Returns the requested length of the window in the direction of the window orientation.
 
             Source: https://docs.wxpython.org/wx.adv.QueryLayoutInfoEvent.html
         """
 
-    def GetSize(self) -> Size:
+    def GetSize(self) -> 'Size':
         """ Returns the size that the event handler specified to the event object as being the requested size of the window.
 
             Source: https://docs.wxpython.org/wx.adv.QueryLayoutInfoEvent.html
         """
 
     def SetAlignment(self, alignment: int) -> None:
         """ Call this to specify the alignment of the window (which side of the remaining parent client area the window sticks to).
@@ -1674,17 +1674,17 @@
         """ Call this to let the calling code know what the size of the window is.
 
             Source: https://docs.wxpython.org/wx.adv.QueryLayoutInfoEvent.html
         """
 
     Alignment: int  # See GetAlignment and SetAlignment
     Flags: int  # See GetFlags and SetFlags
-    Orientation: LayoutOrientation  # See GetOrientation and SetOrientation
+    Orientation: 'adv.LayoutOrientation'  # See GetOrientation and SetOrientation
     RequestedLength: int  # See GetRequestedLength and SetRequestedLength
-    Size: Union[tuple[int, int], 'Size']  # See GetSize and SetSize
+    Size: '_Size'  # See GetSize and SetSize
 
 
 
 EVT_QUERY_LAYOUT_INFO: int  # Process a  wxEVT_QUERY_LAYOUT_INFO   event, to get size, orientation and alignment from a window. ^^
 
 LAYOUT_TOP: int
 
@@ -1799,27 +1799,27 @@
     """
     def __init__(self, iconType: TaskBarIconType=TBI_DEFAULT_TYPE) -> None:
         """ Default constructor.
 
             Source: https://docs.wxpython.org/wx.adv.TaskBarIcon.html
         """
 
-    def CreatePopupMenu(self) -> Menu:
+    def CreatePopupMenu(self) -> 'Menu':
         """ Called by the library when the user requests popup menu if GetPopupMenu   is not overridden.
 
             Source: https://docs.wxpython.org/wx.adv.TaskBarIcon.html
         """
 
     def Destroy(self) -> None:
         """ This method is similar to wx.Window.Destroy   and can be used to schedule the task bar icon object for the delayed destruction: it will be deleted during the next event loop iteration, which allows the task bar icon to process any pending events for it before being destroyed.
 
             Source: https://docs.wxpython.org/wx.adv.TaskBarIcon.html
         """
 
-    def GetPopupMenu(self) -> Menu:
+    def GetPopupMenu(self) -> 'Menu':
         """ Called by the library when the user requests popup menu.
 
             Source: https://docs.wxpython.org/wx.adv.TaskBarIcon.html
         """
 
     @staticmethod
     def IsAvailable() -> bool:
@@ -1893,22 +1893,22 @@
     """
     def __init__(self, bitmap, splashStyle, milliseconds, parent, id=ID_ANY, pos=DefaultPosition, size=DefaultSize, style=BORDER_SIMPLE|FRAME_NO_TASKBAR|STAY_ON_TOP) -> None:
         """ Construct the splash screen passing a bitmap, a style, a timeout, a window id, optional position and size, and a window style.
 
             Source: https://docs.wxpython.org/wx.adv.SplashScreen.html
         """
 
-    def GetBitmap(self) -> Bitmap:
+    def GetBitmap(self) -> 'Bitmap':
         """ Get the spash screenâs bitmap
 
             Source: https://docs.wxpython.org/wx.adv.SplashScreen.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.SplashScreen.html
         """
 
     def GetSplashStyle(self) -> int:
         """ Returns the splash style (see   wx.adv.SplashScreen  for details).
@@ -1924,15 +1924,15 @@
 
     def SetBitmap(self, bitmap) -> None:
         """ Set a new bitmap for the splash screen.
 
             Source: https://docs.wxpython.org/wx.adv.SplashScreen.html
         """
 
-    Bitmap: Bitmap  # See GetBitmap and SetBitmap
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
     SplashStyle: int  # See GetSplashStyle
     Timeout: int  # See GetTimeout
 
 
 
 SPLASH_CENTRE_ON_PARENT: int
 
@@ -1975,15 +1975,15 @@
 
     def DisplaySection(self, *args, **kw) -> bool:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.adv.ExtHelpController.html
         """
 
-    def GetFrameParameters(self, size=None, pos=None, newFrameEachTime=None) -> Frame:
+    def GetFrameParameters(self, size=None, pos=None, newFrameEachTime=None) -> 'Frame':
         """ Obtains the latest settings used by the help frame and the help frame.
 
             Source: https://docs.wxpython.org/wx.adv.ExtHelpController.html
         """
 
     def Initialize(self, dir: str) -> bool:
         """ This must be called to tell the controller where to find the documentation.
@@ -2023,15 +2023,15 @@
 
     def SetViewer(self, viewer="", flags=HELP_NETSCAPE) -> None:
         """ Tell it which browser to use.
 
             Source: https://docs.wxpython.org/wx.adv.ExtHelpController.html
         """
 
-    FrameParameters: Frame  # See GetFrameParameters
+    FrameParameters: 'Frame'  # See GetFrameParameters
 
 
 
 HELP_NETSCAPE: int
 
 class Joystick(Object):
     """ Joystick allows an application to control one or more joysticks.
@@ -2113,15 +2113,15 @@
 
     def GetPollingMin(self) -> int:
         """ Returns the minimum polling frequency.
 
             Source: https://docs.wxpython.org/wx.adv.Joystick.html
         """
 
-    def GetPosition(self, *args, **kw) -> Point:
+    def GetPosition(self, *args, **kw) -> 'Point':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.adv.Joystick.html
         """
 
     def GetProductId(self) -> int:
         """ Returns the product id for the joystick.
@@ -2304,15 +2304,15 @@
     MovementThreshold: int  # See GetMovementThreshold and SetMovementThreshold
     NumberAxes: int  # See GetNumberAxes
     NumberButtons: int  # See GetNumberButtons
     POVCTSPosition: int  # See GetPOVCTSPosition
     POVPosition: int  # See GetPOVPosition
     PollingMax: int  # See GetPollingMax
     PollingMin: int  # See GetPollingMin
-    Position: Point  # See GetPosition
+    Position: 'Point'  # See GetPosition
     ProductId: int  # See GetProductId
     ProductName: str  # See GetProductName
     RudderMax: int  # See GetRudderMax
     RudderMin: int  # See GetRudderMin
     RudderPosition: int  # See GetRudderPosition
     UMax: int  # See GetUMax
     UMin: int  # See GetUMin
@@ -2399,34 +2399,34 @@
 
     def GetDelay(self, frame: int) -> int:
         """ Returns the delay for the i-th frame in milliseconds.
 
             Source: https://docs.wxpython.org/wx.adv.Animation.html
         """
 
-    def GetFrame(self, frame: int) -> Image:
+    def GetFrame(self, frame: int) -> 'Image':
         """ Returns the i-th frame as a   wx.Image.
 
             Source: https://docs.wxpython.org/wx.adv.Animation.html
         """
 
     def GetFrameCount(self) -> int:
         """ Returns the number of frames for this animation.
 
             Source: https://docs.wxpython.org/wx.adv.Animation.html
         """
 
     @staticmethod
-    def GetHandlers() -> AnimationDecoderList:
+    def GetHandlers() -> list['adv.AnimationHandler']:
         """ Returns the list of animation decoders used by the generic animation and    wx.adv.GenericAnimationCtrl.
 
             Source: https://docs.wxpython.org/wx.adv.Animation.html
         """
 
-    def GetSize(self) -> Size:
+    def GetSize(self) -> 'Size':
         """ Returns the size of the animation.
 
             Source: https://docs.wxpython.org/wx.adv.Animation.html
         """
 
     @staticmethod
     def InitStandardHandlers() -> None:
@@ -2463,15 +2463,15 @@
     def LoadFile(self, name, type=ANIMATION_TYPE_ANY) -> bool:
         """ Loads an animation from a file.
 
             Source: https://docs.wxpython.org/wx.adv.Animation.html
         """
 
     FrameCount: int  # See GetFrameCount
-    Size: Size  # See GetSize
+    Size: '_Size'  # See GetSize
 
 
 
 ANIMATION_TYPE_ANY: int
 
 class LayoutAlgorithm(Object):
     """ LayoutAlgorithm implements layout of subwindows in MDI or SDI
@@ -2588,22 +2588,22 @@
 
     def Create(*args, **kwargs) -> bool:
         """ Creates the wizard page.
 
             Source: https://docs.wxpython.org/wx.adv.WizardPage.html
         """
 
-    def GetBitmap(self) -> Bitmap:
+    def GetBitmap(self) -> 'Bitmap':
         """ This method is called by   wx.adv.Wizard  to get the bitmap to display alongside the page.
 
             Source: https://docs.wxpython.org/wx.adv.WizardPage.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.WizardPage.html
         """
 
     def GetNext(self) -> 'adv.WizardPage':
         """ Get the page which should be shown when the user chooses the  "Next"   button: if None is returned, this button will be disabled.
@@ -2613,20 +2613,22 @@
 
     def GetPrev(self) -> 'adv.WizardPage':
         """ Get the page which should be shown when the user chooses the  "Back"   button: if None is returned, this button will be disabled.
 
             Source: https://docs.wxpython.org/wx.adv.WizardPage.html
         """
 
-    Bitmap: Bitmap  # See GetBitmap
+    Bitmap: '_Bitmap'  # See GetBitmap
     Next: 'adv.WizardPage'  # See GetNext
     Prev: 'adv.WizardPage'  # See GetPrev
 
 
 
+OwnerDrawnComboBoxPaintingFlags: TypeAlias = int  # Enumeration
+
 ODCB_PAINTING_CONTROL: int
 
 ODCB_PAINTING_SELECTED: int
 
 class CalendarEvent(DateEvent):
     """ The CalendarEvent class is used together with CalendarCtrl.
 
@@ -2634,32 +2636,36 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.adv.CalendarEvent.html
         """
 
-    def GetWeekDay(self) -> 'DateTime.WeekDay':
+    def GetWeekDay(self) -> 'WeekDay':
         """ Returns the week day on which the user clicked in  EVT_CALENDAR_WEEKDAY_CLICKED   handler.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarEvent.html
         """
 
     def SetWeekDay(self, day: DateTime.WeekDay) -> None:
         """ Sets the week day carried by the event, normally only used by the library internally.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarEvent.html
         """
 
-    WeekDay: DateTime.WeekDay  # See GetWeekDay and SetWeekDay
+    WeekDay: 'WeekDay'  # See GetWeekDay and SetWeekDay
+
 
 
+SashEdgePosition: TypeAlias = int  # Enumeration
 
 SASH_NONE: int
 
+SashDragStatus: TypeAlias = int  # Enumeration
+
 class SashLayoutWindow(SashWindow):
     """ SashLayoutWindow responds to OnCalculateLayout events generated by
 LayoutAlgorithm.
 
         Source: https://docs.wxpython.org/wx.adv.SashLayoutWindow.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -2677,15 +2683,15 @@
     def GetAlignment(self) -> int:
         """ Returns the alignment of the window: one of wx.adv.LAYOUT_TOP, wx.adv.LAYOUT_LEFT, wx.adv.LAYOUT_RIGHT, wx.adv.LAYOUT_BOTTOM.
 
             Source: https://docs.wxpython.org/wx.adv.SashLayoutWindow.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.SashLayoutWindow.html
         """
 
     def GetOrientation(self) -> 'adv.LayoutOrientation':
         """ Returns the orientation of the window: one of wx.adv.LAYOUT_HORIZONTAL, wx.adv.LAYOUT_VERTICAL.
@@ -2720,15 +2726,15 @@
     def SetOrientation(self, orientation: LayoutOrientation) -> None:
         """ Sets the orientation of the window (the direction the window will stretch in, to fill the available parent client area).
 
             Source: https://docs.wxpython.org/wx.adv.SashLayoutWindow.html
         """
 
     Alignment: int  # See GetAlignment and SetAlignment
-    Orientation: LayoutOrientation  # See GetOrientation and SetOrientation
+    Orientation: 'adv.LayoutOrientation'  # See GetOrientation and SetOrientation
 
 
 
 class GenericAnimationCtrl(AnimationCtrl):
     """ Generic implementation of AnimationCtrl interface.
 
         Source: https://docs.wxpython.org/wx.adv.GenericAnimationCtrl.html
@@ -2766,28 +2772,28 @@
 
     def GetAnimation(self) -> 'adv.Animation':
         """ Returns the animation associated with this control.
 
             Source: https://docs.wxpython.org/wx.adv.GenericAnimationCtrl.html
         """
 
-    def GetBackingStore(self) -> Bitmap:
+    def GetBackingStore(self) -> 'Bitmap':
         """ Returns a   wx.Bitmap  with the current frame drawn in it.
 
             Source: https://docs.wxpython.org/wx.adv.GenericAnimationCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.GenericAnimationCtrl.html
         """
 
-    def GetInactiveBitmap(self) -> Bitmap:
+    def GetInactiveBitmap(self) -> 'Bitmap':
         """ Returns the inactive bitmap shown in this control when the; see SetInactiveBitmap   for more info.
 
             Source: https://docs.wxpython.org/wx.adv.GenericAnimationCtrl.html
         """
 
     def IsPlaying(self) -> bool:
         """ Returns True if the animation is being played.
@@ -2840,19 +2846,21 @@
     def Stop(self) -> None:
         """ Stops playing the animation.
 
             Source: https://docs.wxpython.org/wx.adv.GenericAnimationCtrl.html
         """
 
     Animation: 'adv.Animation'  # See GetAnimation and SetAnimation
-    BackingStore: Bitmap  # See GetBackingStore
-    InactiveBitmap: 'BitmapBundle'  # See GetInactiveBitmap and SetInactiveBitmap
+    BackingStore: 'Bitmap'  # See GetBackingStore
+    InactiveBitmap: 'Bitmap'  # See GetInactiveBitmap and SetInactiveBitmap
 
 
 
+AnimationType: TypeAlias = int  # Enumeration
+
 ANIMATION_TYPE_INVALID: int
 
 ANIMATION_TYPE_GIF: int
 
 ANIMATION_TYPE_ANI: int
 
 class CalendarDateAttr:
@@ -2862,46 +2870,46 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.adv.CalendarDateAttr.html
         """
 
-    def GetBackgroundColour(self) -> Colour:
+    def GetBackgroundColour(self) -> 'Colour':
         """ Returns the background colour set for the calendar date.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarDateAttr.html
         """
 
     def GetBorder(self) -> 'adv.CalendarDateBorder':
         """ Returns the border set for the calendar date.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarDateAttr.html
         """
 
-    def GetBorderColour(self) -> Colour:
+    def GetBorderColour(self) -> 'Colour':
         """ Returns the border colour set for the calendar date.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarDateAttr.html
         """
 
-    def GetFont(self) -> Font:
+    def GetFont(self) -> 'Font':
         """ Returns the font set for the calendar date.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarDateAttr.html
         """
 
     @staticmethod
     def GetMark() -> 'adv.CalendarDateAttr':
         """ Used (internally) by the generic wx.adv.CalendarCtrl.Mark .
 
             Source: https://docs.wxpython.org/wx.adv.CalendarDateAttr.html
         """
 
-    def GetTextColour(self) -> Colour:
+    def GetTextColour(self) -> 'Colour':
         """ Returns the text colour set for the calendar date.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarDateAttr.html
         """
 
     def HasBackgroundColour(self) -> bool:
         """ Returns True if a non-default text background colour is set.
@@ -2978,21 +2986,23 @@
 
     def SetTextColour(self, colText: Union[int, str, 'Colour']) -> None:
         """ Sets the text (foreground) colour to use.
 
             Source: https://docs.wxpython.org/wx.adv.CalendarDateAttr.html
         """
 
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
-    Border: CalendarDateBorder  # See GetBorder and SetBorder
-    BorderColour: Union[int, str, 'Colour']  # See GetBorderColour and SetBorderColour
-    Font: 'Font'  # See GetFont and SetFont
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
+    Border: 'adv.CalendarDateBorder'  # See GetBorder and SetBorder
+    BorderColour: 'Colour'  # See GetBorderColour and SetBorderColour
+    Font: '_Font'  # See GetFont and SetFont
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
+
 
 
+CalendarHitTestResult: TypeAlias = int  # Enumeration
 
 CAL_HITTEST_NOWHERE: int
 
 CAL_HITTEST_HEADER: int
 
 CAL_HITTEST_DAY: int
 
@@ -3000,14 +3010,16 @@
 
 CAL_HITTEST_DECMONTH: int
 
 CAL_HITTEST_SURROUNDING_WEEK: int
 
 CAL_HITTEST_WEEK: int
 
+PropertySheetDialogFlags: TypeAlias = int  # Enumeration
+
 PROPSHEET_DEFAULT: int
 
 PROPSHEET_NOTEBOOK: int
 
 PROPSHEET_TOOLBOOK: int
 
 PROPSHEET_CHOICEBOOK: int
@@ -3016,16 +3028,22 @@
 
 PROPSHEET_BUTTONTOOLBOOK: int
 
 PROPSHEET_TREEBOOK: int
 
 PROPSHEET_SHRINKTOFIT: int
 
+LayoutAlignment: TypeAlias = int  # Enumeration
+
 LAYOUT_NONE: int
 
+LayoutOrientation: TypeAlias = int  # Enumeration
+
+TaskBarIconType: TypeAlias = int  # Enumeration
+
 TBI_DOCK: int
 
 TBI_CUSTOM_STATUSITEM: int
 
 TBI_DEFAULT_TYPE: int
 
 class AnimationDecoder(ObjectRefData):
@@ -3060,21 +3078,21 @@
 
     def DoCanRead(self, stream: 'InputStream') -> bool:
         """ Checks the signature of the data in the given stream and returns True if it appears to be a valid animation format recognized by the animation decoder; this function should modify the stream current position without taking care of restoring it since  CanRead   will do it.
 
             Source: https://docs.wxpython.org/wx.adv.AnimationDecoder.html
         """
 
-    def GetAnimationSize(self) -> Size:
+    def GetAnimationSize(self) -> 'Size':
         """ Size
 
             Source: https://docs.wxpython.org/wx.adv.AnimationDecoder.html
         """
 
-    def GetBackgroundColour(self) -> Colour:
+    def GetBackgroundColour(self) -> 'Colour':
         """ Colour
 
             Source: https://docs.wxpython.org/wx.adv.AnimationDecoder.html
         """
 
     def GetDelay(self, frame: int) -> int:
         """ Return the number of milliseconds this frame should be displayed.
@@ -3090,27 +3108,27 @@
 
     def GetFrameCount(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.adv.AnimationDecoder.html
         """
 
-    def GetFramePosition(self, frame: int) -> Point:
+    def GetFramePosition(self, frame: int) -> 'Point':
         """ frame (int) â
 
             Source: https://docs.wxpython.org/wx.adv.AnimationDecoder.html
         """
 
-    def GetFrameSize(self, frame: int) -> Size:
+    def GetFrameSize(self, frame: int) -> 'Size':
         """ frame (int) â
 
             Source: https://docs.wxpython.org/wx.adv.AnimationDecoder.html
         """
 
-    def GetTransparentColour(self, frame: int) -> Colour:
+    def GetTransparentColour(self, frame: int) -> 'Colour':
         """ The transparent colour for this frame, if any, or  NullColour .
 
             Source: https://docs.wxpython.org/wx.adv.AnimationDecoder.html
         """
 
     def GetType(self) -> 'adv.AnimationType':
         """ Return the animation type this decoder implements.
@@ -3120,16 +3138,16 @@
 
     def Load(self, stream: 'InputStream') -> bool:
         """ Load the animation image frames from the given stream.
 
             Source: https://docs.wxpython.org/wx.adv.AnimationDecoder.html
         """
 
-    AnimationSize: Size  # See GetAnimationSize
-    BackgroundColour: Colour  # See GetBackgroundColour
+    AnimationSize: 'Size'  # See GetAnimationSize
+    BackgroundColour: 'Colour'  # See GetBackgroundColour
     FrameCount: int  # See GetFrameCount
     Type: 'adv.AnimationType'  # See GetType
 
 
 
 class WizardPageSimple(WizardPage):
     """ WizardPageSimple is the simplest possible WizardPage
@@ -3153,15 +3171,15 @@
     def Create(*args, **kwargs) -> bool:
         """ Creates the wizard page.
 
             Source: https://docs.wxpython.org/wx.adv.WizardPageSimple.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.adv.WizardPageSimple.html
         """
 
     def SetNext(self, next: 'adv.WizardPage') -> None:
         """ Sets the next page.
@@ -3173,14 +3191,16 @@
         """ Sets the previous page.
 
             Source: https://docs.wxpython.org/wx.adv.WizardPageSimple.html
         """
 
 
 
+CalendarDateBorder: TypeAlias = int  # Enumeration
+
 CAL_BORDER_NONE: int
 
 CAL_BORDER_SQUARE: int
 
 CAL_BORDER_ROUND: int
 
 class ANIDecoder(AnimationDecoder):
@@ -3220,27 +3240,27 @@
 
     def GetDisposalMethod(self, frame: int) -> 'adv.AnimationDisposal':
         """ What should be done after displaying this frame.
 
             Source: https://docs.wxpython.org/wx.adv.ANIDecoder.html
         """
 
-    def GetFramePosition(self, frame: int) -> Point:
+    def GetFramePosition(self, frame: int) -> 'Point':
         """ frame (int) â
 
             Source: https://docs.wxpython.org/wx.adv.ANIDecoder.html
         """
 
-    def GetFrameSize(self, frame: int) -> Size:
+    def GetFrameSize(self, frame: int) -> 'Size':
         """ frame (int) â
 
             Source: https://docs.wxpython.org/wx.adv.ANIDecoder.html
         """
 
-    def GetTransparentColour(self, frame: int) -> Colour:
+    def GetTransparentColour(self, frame: int) -> 'Colour':
         """ The transparent colour for this frame, if any, or  NullColour .
 
             Source: https://docs.wxpython.org/wx.adv.ANIDecoder.html
         """
 
     def GetType(self) -> 'adv.AnimationType':
         """ Return the animation type this decoder implements.
@@ -3295,27 +3315,27 @@
 
     def GetDisposalMethod(self, frame: int) -> 'adv.AnimationDisposal':
         """ What should be done after displaying this frame.
 
             Source: https://docs.wxpython.org/wx.adv.GIFDecoder.html
         """
 
-    def GetFramePosition(self, frame: int) -> Point:
+    def GetFramePosition(self, frame: int) -> 'Point':
         """ frame (int) â
 
             Source: https://docs.wxpython.org/wx.adv.GIFDecoder.html
         """
 
-    def GetFrameSize(self, frame: int) -> Size:
+    def GetFrameSize(self, frame: int) -> 'Size':
         """ frame (int) â
 
             Source: https://docs.wxpython.org/wx.adv.GIFDecoder.html
         """
 
-    def GetTransparentColour(self, frame: int) -> Colour:
+    def GetTransparentColour(self, frame: int) -> 'Colour':
         """ The transparent colour for this frame, if any, or  NullColour .
 
             Source: https://docs.wxpython.org/wx.adv.GIFDecoder.html
         """
 
     def GetType(self) -> 'adv.AnimationType':
         """ Return the animation type this decoder implements.
@@ -3329,14 +3349,16 @@
             Source: https://docs.wxpython.org/wx.adv.GIFDecoder.html
         """
 
     Type: 'adv.AnimationType'  # See GetType
 
 
 
+AnimationDisposal: TypeAlias = int  # Enumeration
+
 ANIM_UNSPECIFIED: int
 
 ANIM_DONOTREMOVE: int
 
 ANIM_TOBACKGROUND: int
 
 ANIM_TOPREVIOUS: int
```

### Comparing `types_wxpython-0.6.1/wx-stubs/aui/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/aui/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class AuiNotebook(BookCtrlBase):
     """ AuiNotebook is part of the AUI class framework, which represents a
 notebook control, managing multiple windows with associated tabs.
 
         Source: https://docs.wxpython.org/wx.aui.AuiNotebook.html
     """
@@ -64,39 +64,39 @@
     def GetArtProvider(self) -> 'aui.AuiTabArt':
         """ Returns the associated art provider.
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebook.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebook.html
         """
 
-    def GetCurrentPage(self) -> Window:
+    def GetCurrentPage(self) -> 'Window':
         """ Returns the currently selected page or None.
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebook.html
         """
 
     def GetHeightForPageHeight(self, pageHeight: int) -> int:
         """ Returns the desired height of the notebook for the given page height.
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebook.html
         """
 
-    def GetPage(self, page_idx: int) -> Window:
+    def GetPage(self, page_idx: int) -> 'Window':
         """ Returns the page specified by the given index.
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebook.html
         """
 
-    def GetPageBitmap(self, page: int) -> Bitmap:
+    def GetPageBitmap(self, page: int) -> 'Bitmap':
         """ Returns the tab bitmap for the page.
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebook.html
         """
 
     def GetPageCount(self) -> int:
         """ Returns the number of pages in the notebook.
@@ -240,15 +240,15 @@
         """ Split performs a split operation programmatically.
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebook.html
         """
 
     ActiveTabCtrl: 'aui.AuiTabCtrl'  # See GetActiveTabCtrl
     ArtProvider: 'aui.AuiTabArt'  # See GetArtProvider and SetArtProvider
-    CurrentPage: Window  # See GetCurrentPage
+    CurrentPage: 'Window'  # See GetCurrentPage
     PageCount: int  # See GetPageCount
     Selection: int  # See GetSelection and SetSelection
     TabCtrlHeight: int  # See GetTabCtrlHeight and SetTabCtrlHeight
 
 
 
 AUI_NB_DEFAULT_STYLE: int  # Defined as wx.aui.AUI_NB_TOP | wx.aui.AUI_NB_TAB_SPLIT | wx.aui.AUI_NB_TAB_MOVE | wx.aui.AUI_NB_SCROLL_BUTTONS | wx.aui.AUI_NB_CLOSE_ON_ACTIVE_TAB | wx.aui.AUI_NB_MIDDLE_CLICK_CLOSE.
@@ -324,15 +324,15 @@
     """
     def __init__(self, command_type=wxEVT_NULL, win_id=0) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebookEvent.html
         """
 
-    def Clone(self) -> Event:
+    def Clone(self) -> 'Event':
         """ Event
 
             Source: https://docs.wxpython.org/wx.aui.AuiNotebookEvent.html
         """
 
 
 
@@ -379,15 +379,15 @@
 
     def GetIndentSize(self) -> int:
         """ Returns the indent size.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultTabArt.html
         """
 
-    def GetTabSize(self, dc, wnd, caption, bitmap, active, close_button_state, x_extent) -> Size:
+    def GetTabSize(self, dc, wnd, caption, bitmap, active, close_button_state, x_extent) -> 'Size':
         """ Returns the tab size for the given caption, bitmap and state.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultTabArt.html
         """
 
     def SetActiveColour(self, colour: Union[int, str, 'Colour']) -> None:
         """ Sets the colour of the selected tab.
@@ -461,15 +461,15 @@
     def GetActiveChild(self) -> 'aui.AuiMDIChildFrame':
         """ wx.aui.AuiMDIChildFrame
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIClientWindow.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIClientWindow.html
         """
 
     def SetActiveChild(self, pChildFrame: 'aui.AuiMDIChildFrame') -> None:
         """ pChildFrame (wx.aui.AuiMDIChildFrame) â
@@ -495,15 +495,15 @@
     def __init__(self, parent, id=ID_ANY, pos=DefaultPosition, size=DefaultSize, style=0) -> None:
         """ parent (wx.Window) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiTabCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiTabCtrl.html
         """
 
     def IsDragging(self) -> bool:
         """ bool
@@ -557,15 +557,15 @@
 
     def GetIndentSize(self) -> int:
         """ Returns the indent size.
 
             Source: https://docs.wxpython.org/wx.aui.AuiTabArt.html
         """
 
-    def GetTabSize(self, dc, wnd, caption, bitmap, active, close_button_state, x_extent) -> Size:
+    def GetTabSize(self, dc, wnd, caption, bitmap, active, close_button_state, x_extent) -> 'Size':
         """ Returns the tab size for the given caption, bitmap and state.
 
             Source: https://docs.wxpython.org/wx.aui.AuiTabArt.html
         """
 
     def SetActiveColour(self, colour: Union[int, str, 'Colour']) -> None:
         """ Sets the colour of the selected tab.
@@ -704,15 +704,15 @@
 
     def EnableTool(self, toolId, state) -> None:
         """ toolId (int) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
-    def FindControl(self, window_id: int) -> Control:
+    def FindControl(self, window_id: int) -> 'Control':
         """ window_id (int) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
     def FindTool(self, toolId: int) -> 'aui.AuiToolBarItem':
         """ toolId (int) â
@@ -735,27 +735,27 @@
     def GetArtProvider(self) -> 'aui.AuiToolBarArt':
         """ wx.aui.AuiToolBarArt
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
     def GetGripperVisible(self) -> bool:
         """ bool
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
-    def GetHintSize(self, dock_direction: int) -> Size:
+    def GetHintSize(self, dock_direction: int) -> 'Size':
         """ get size of hint rectangle for a particular dock location
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
     def GetOverflowVisible(self) -> bool:
         """ bool
@@ -765,21 +765,21 @@
 
     def GetToolBarFits(self) -> bool:
         """ bool
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
-    def GetToolBitmap(self, toolId: int) -> Bitmap:
+    def GetToolBitmap(self, toolId: int) -> 'Bitmap':
         """ toolId (int) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
-    def GetToolBitmapSize(self) -> Size:
+    def GetToolBitmapSize(self) -> 'Size':
         """ Size
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
     def GetToolBorderPadding(self) -> int:
         """ int
@@ -849,15 +849,15 @@
 
     def GetToolProportion(self, toolId: int) -> int:
         """ toolId (int) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
-    def GetToolRect(self, toolId: int) -> Rect:
+    def GetToolRect(self, toolId: int) -> 'Rect':
         """ toolId (int) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
     def GetToolSeparation(self) -> int:
         """ int
@@ -1027,15 +1027,15 @@
             Source: https://docs.wxpython.org/wx.aui.AuiToolBar.html
         """
 
     ArtProvider: 'aui.AuiToolBarArt'  # See GetArtProvider and SetArtProvider
     GripperVisible: bool  # See GetGripperVisible and SetGripperVisible
     OverflowVisible: bool  # See GetOverflowVisible and SetOverflowVisible
     ToolBarFits: bool  # See GetToolBarFits
-    ToolBitmapSize: Union[tuple[int, int], 'Size']  # See GetToolBitmapSize and SetToolBitmapSize
+    ToolBitmapSize: 'Size'  # See GetToolBitmapSize and SetToolBitmapSize
     ToolBorderPadding: int  # See GetToolBorderPadding and SetToolBorderPadding
     ToolCount: int  # See GetToolCount
     ToolPacking: int  # See GetToolPacking and SetToolPacking
     ToolSeparation: int  # See GetToolSeparation and SetToolSeparation
     ToolTextOrientation: int  # See GetToolTextOrientation and SetToolTextOrientation
     WindowStyleFlag: int  # See GetWindowStyleFlag and SetWindowStyleFlag
 
@@ -1094,15 +1094,15 @@
 
     def GetButton(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.aui.AuiManagerEvent.html
         """
 
-    def GetDC(self) -> DC:
+    def GetDC(self) -> 'DC':
         """ DC
 
             Source: https://docs.wxpython.org/wx.aui.AuiManagerEvent.html
         """
 
     def GetManager(self) -> 'aui.AuiManager':
         """ wx.aui.AuiManager
@@ -1155,15 +1155,15 @@
     def Veto(self, veto: bool=True) -> None:
         """ Cancels the action indicated by this event if CanVeto   is True.
 
             Source: https://docs.wxpython.org/wx.aui.AuiManagerEvent.html
         """
 
     Button: int  # See GetButton and SetButton
-    DC: 'DC'  # See GetDC and SetDC
+    DC: '_DC'  # See GetDC and SetDC
     Manager: 'aui.AuiManager'  # See GetManager and SetManager
     Pane: 'aui.AuiPaneInfo'  # See GetPane and SetPane
 
 
 
 EVT_AUI_PANE_BUTTON: int  # Triggered when any button is pressed for any docked panes.
 
@@ -1197,15 +1197,15 @@
     @staticmethod
     def AlwaysUsesLiveResize() -> bool:
         """ Returns True if live resize is always used on the current platform.
 
             Source: https://docs.wxpython.org/wx.aui.AuiManager.html
         """
 
-    def CalculateHintRect(self, paneWindow, pt, offset) -> Rect:
+    def CalculateHintRect(self, paneWindow, pt, offset) -> 'Rect':
         """ This function is used by controls to calculate the drop hint rectangle.
 
             Source: https://docs.wxpython.org/wx.aui.AuiManager.html
         """
 
     def CanDockPanel(self, p: 'aui.AuiPaneInfo') -> bool:
         """ Check if a key modifier is pressed (actually   or ) while dragging the frame to not dock the window.
@@ -1233,15 +1233,15 @@
 
     def DrawHintRect(self, paneWindow, pt, offset) -> None:
         """ This function is used by controls to draw the hint window.
 
             Source: https://docs.wxpython.org/wx.aui.AuiManager.html
         """
 
-    def GetAllPanes(self) -> AuiPaneInfoArray:
+    def GetAllPanes(self) -> 'aui.AuiPaneInfoArray':
         """ Returns an array of all panes managed by the frame manager.
 
             Source: https://docs.wxpython.org/wx.aui.AuiManager.html
         """
 
     def GetArtProvider(self) -> 'aui.AuiDockArt':
         """ Returns the current art provider being used.
@@ -1257,15 +1257,15 @@
 
     def GetFlags(self) -> int:
         """ Returns the current   wx.aui.AuiManagerOptionâs flags.
 
             Source: https://docs.wxpython.org/wx.aui.AuiManager.html
         """
 
-    def GetManagedWindow(self) -> Window:
+    def GetManagedWindow(self) -> 'Window':
         """ Returns the frame currently being managed by   wx.aui.AuiManager.
 
             Source: https://docs.wxpython.org/wx.aui.AuiManager.html
         """
 
     @staticmethod
     def GetManager(window: 'Window') -> 'aui.AuiManager':
@@ -1390,15 +1390,15 @@
 
     def Update(self) -> None:
         """ This method is called after any number of changes are made to any of the managed panes.
 
             Source: https://docs.wxpython.org/wx.aui.AuiManager.html
         """
 
-    AllPanes: AuiPaneInfoArray  # See GetAllPanes
+    AllPanes: 'aui.AuiPaneInfoArray'  # See GetAllPanes
     ArtProvider: 'aui.AuiDockArt'  # See GetArtProvider and SetArtProvider
     Flags: int  # See GetFlags and SetFlags
     ManagedWindow: 'Window'  # See GetManagedWindow and SetManagedWindow
 
 
 
 AUI_MGR_ALLOW_FLOATING: int  # Allow a pane to be undocked to take the form of a   wx.MiniFrame.
@@ -1505,15 +1505,15 @@
     def GetArtProvider(self) -> 'aui.AuiTabArt':
         """ wx.aui.AuiTabArt
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIParentFrame.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIParentFrame.html
         """
 
     def GetClientWindow(self) -> 'aui.AuiMDIClientWindow':
         """ wx.aui.AuiMDIClientWindow
@@ -1523,15 +1523,15 @@
 
     def GetNotebook(self) -> 'aui.AuiNotebook':
         """ wx.aui.AuiNotebook
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIParentFrame.html
         """
 
-    def GetWindowMenu(self) -> Menu:
+    def GetWindowMenu(self) -> 'Menu':
         """ Menu
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIParentFrame.html
         """
 
     def OnCreateClient(self) -> 'aui.AuiMDIClientWindow':
         """ wx.aui.AuiMDIClientWindow
@@ -1590,21 +1590,21 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarEvent.html
         """
 
-    def GetClickPoint(self) -> Point:
+    def GetClickPoint(self) -> 'Point':
         """ Returns the point where the user clicked with the mouse.
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarEvent.html
         """
 
-    def GetItemRect(self) -> Rect:
+    def GetItemRect(self) -> 'Rect':
         """ Returns the   wx.aui.AuiToolBarItem  rectangle bounding the mouse click point.
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarEvent.html
         """
 
     def GetToolId(self) -> int:
         """ Returns the   wx.aui.AuiToolBarItem  identifier.
@@ -1638,15 +1638,15 @@
 
     def SetToolId(self, toolId: int) -> None:
         """ toolId (int) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarEvent.html
         """
 
-    ClickPoint: Union[tuple[int, int], 'Point']  # See GetClickPoint and SetClickPoint
+    ClickPoint: 'Point'  # See GetClickPoint and SetClickPoint
     ItemRect: 'Rect'  # See GetItemRect and SetItemRect
     ToolId: int  # See GetToolId and SetToolId
 
 
 
 class AuiMDIChildFrame(Panel):
     """  Overloaded Implementations:
@@ -1667,76 +1667,76 @@
 
     def Create(self, parent, winid=ID_ANY, title="", pos=DefaultPosition, size=DefaultSize, style=DEFAULT_FRAME_STYLE, name=FrameNameStr) -> bool:
         """ parent (wx.aui.AuiMDIParentFrame) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
-    def CreateStatusBar(self, number=1, style=1, winid=1, name="") -> StatusBar:
+    def CreateStatusBar(self, number=1, style=1, winid=1, name="") -> 'StatusBar':
         """ number (int) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
-    def CreateToolBar(self, style, winid, name) -> ToolBar:
+    def CreateToolBar(self, style, winid, name) -> 'ToolBar':
         """ style (long) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
     def Destroy(self) -> bool:
         """ Destroys the window safely.
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
-    def GetIcon(self) -> Icon:
+    def GetIcon(self) -> 'Icon':
         """ Icon
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
-    def GetIcons(self) -> IconBundle:
+    def GetIcons(self) -> 'IconBundle':
         """ IconBundle
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
     def GetMDIParentFrame(self) -> 'aui.AuiMDIParentFrame':
         """ wx.aui.AuiMDIParentFrame
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
-    def GetMenuBar(self) -> MenuBar:
+    def GetMenuBar(self) -> 'MenuBar':
         """ MenuBar
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
-    def GetStatusBar(self) -> StatusBar:
+    def GetStatusBar(self) -> 'StatusBar':
         """ StatusBar
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
     def GetTitle(self) -> str:
         """ string
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
-    def GetToolBar(self) -> ToolBar:
+    def GetToolBar(self) -> 'ToolBar':
         """ ToolBar
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
     def Iconize(self, iconize: bool=True) -> None:
         """ iconize (bool) â
@@ -1830,21 +1830,21 @@
 
     def ShowFullScreen(self, show, style) -> bool:
         """ show (bool) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiMDIChildFrame.html
         """
 
-    Icon: 'Icon'  # See GetIcon and SetIcon
+    Icon: '_Icon'  # See GetIcon and SetIcon
     Icons: 'IconBundle'  # See GetIcons and SetIcons
     MDIParentFrame: 'aui.AuiMDIParentFrame'  # See GetMDIParentFrame and SetMDIParentFrame
-    MenuBar: 'MenuBar'  # See GetMenuBar and SetMenuBar
-    StatusBar: StatusBar  # See GetStatusBar
+    MenuBar: '_MenuBar'  # See GetMenuBar and SetMenuBar
+    StatusBar: '_StatusBar'  # See GetStatusBar
     Title: str  # See GetTitle and SetTitle
-    ToolBar: ToolBar  # See GetToolBar
+    ToolBar: '_ToolBar'  # See GetToolBar
 
 
 
 class AuiNotebookPage:
     """ A simple class which holds information about the notebookâs pages and
 their state.
 
@@ -1902,15 +1902,15 @@
 
     def GetIndentSize(self) -> int:
         """ Returns the indent size.
 
             Source: https://docs.wxpython.org/wx.aui.AuiSimpleTabArt.html
         """
 
-    def GetTabSize(self, dc, wnd, caption, bitmap, active, closeButtonState, xExtent) -> Size:
+    def GetTabSize(self, dc, wnd, caption, bitmap, active, closeButtonState, xExtent) -> 'Size':
         """ dc (wx.DC) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiSimpleTabArt.html
         """
 
     def SetActiveColour(self, colour: Union[int, str, 'Colour']) -> None:
         """ Sets the colour of the selected tab.
@@ -1990,27 +1990,27 @@
 
     def GetAlignment(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
-    def GetBitmap(self) -> Bitmap:
+    def GetBitmap(self) -> 'Bitmap':
         """ Bitmap
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
-    def GetDisabledBitmap(self) -> Bitmap:
+    def GetDisabledBitmap(self) -> 'Bitmap':
         """ Bitmap
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
-    def GetHoverBitmap(self) -> Bitmap:
+    def GetHoverBitmap(self) -> 'Bitmap':
         """ Bitmap
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
     def GetId(self) -> int:
         """ Returns the toolbar item identifier.
@@ -2032,15 +2032,15 @@
 
     def GetLongHelp(self) -> str:
         """ string
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
-    def GetMinSize(self) -> Size:
+    def GetMinSize(self) -> 'Size':
         """ Size
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
     def GetProportion(self) -> int:
         """ int
@@ -2050,15 +2050,15 @@
 
     def GetShortHelp(self) -> str:
         """ string
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
-    def GetSizerItem(self) -> SizerItem:
+    def GetSizerItem(self) -> 'SizerItem':
         """ SizerItem
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
     def GetSpacerPixels(self) -> int:
         """ int
@@ -2074,15 +2074,15 @@
 
     def GetUserData(self) -> int:
         """ long
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
-    def GetWindow(self) -> Window:
+    def GetWindow(self) -> 'Window':
         """ Returns the Window associated to the toolbar item.
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
     def HasDropDown(self) -> bool:
         """ Returns whether the toolbar item has an associated drop down button.
@@ -2213,29 +2213,29 @@
     def SetWindow(self, w: 'Window') -> None:
         """ Assigns a window to the toolbar item.
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarItem.html
         """
 
     Alignment: int  # See GetAlignment and SetAlignment
-    Bitmap: 'BitmapBundle'  # See GetBitmap and SetBitmap
-    DisabledBitmap: 'BitmapBundle'  # See GetDisabledBitmap and SetDisabledBitmap
-    HoverBitmap: 'BitmapBundle'  # See GetHoverBitmap and SetHoverBitmap
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
+    DisabledBitmap: 'Bitmap'  # See GetDisabledBitmap and SetDisabledBitmap
+    HoverBitmap: 'Bitmap'  # See GetHoverBitmap and SetHoverBitmap
     Id: int  # See GetId and SetId
     Kind: int  # See GetKind and SetKind
     Label: str  # See GetLabel and SetLabel
     LongHelp: str  # See GetLongHelp and SetLongHelp
-    MinSize: Union[tuple[int, int], 'Size']  # See GetMinSize and SetMinSize
+    MinSize: 'Size'  # See GetMinSize and SetMinSize
     Proportion: int  # See GetProportion and SetProportion
     ShortHelp: str  # See GetShortHelp and SetShortHelp
-    SizerItem: 'SizerItem'  # See GetSizerItem and SetSizerItem
+    SizerItem: '_SizerItem'  # See GetSizerItem and SetSizerItem
     SpacerPixels: int  # See GetSpacerPixels and SetSpacerPixels
     State: int  # See GetState and SetState
     UserData: int  # See GetUserData and SetUserData
-    Window: 'Window'  # See GetWindow and SetWindow
+    Window: '_Window'  # See GetWindow and SetWindow
 
 
 
 class AuiToolBarArt:
     """ AuiToolBarArt is part of the AUI class framework.
 
         Source: https://docs.wxpython.org/wx.aui.AuiToolBarArt.html
@@ -2314,33 +2314,33 @@
 
     def GetFlags(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarArt.html
         """
 
-    def GetFont(self) -> Font:
+    def GetFont(self) -> 'Font':
         """ Font
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarArt.html
         """
 
-    def GetLabelSize(self, dc, wnd, item) -> Size:
+    def GetLabelSize(self, dc, wnd, item) -> 'Size':
         """ dc (wx.DC) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarArt.html
         """
 
     def GetTextOrientation(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarArt.html
         """
 
-    def GetToolSize(self, dc, wnd, item) -> Size:
+    def GetToolSize(self, dc, wnd, item) -> 'Size':
         """ dc (wx.DC) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarArt.html
         """
 
     def SetElementSize(self, element_id, size) -> None:
         """ element_id (int) â
@@ -2369,15 +2369,15 @@
     def ShowDropDown(self, wnd, items) -> int:
         """ wnd (wx.Window) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiToolBarArt.html
         """
 
     Flags: int  # See GetFlags and SetFlags
-    Font: 'Font'  # See GetFont and SetFont
+    Font: '_Font'  # See GetFont and SetFont
     TextOrientation: int  # See GetTextOrientation and SetTextOrientation
 
 
 
 class AuiPaneInfo:
     """ AuiPaneInfo is part of the AUI class framework.
 
@@ -2890,21 +2890,21 @@
 
     def DrawSash(self, dc, window, orientation, rect) -> None:
         """ Draws a sash between two windows.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDockArt.html
         """
 
-    def GetColour(self, id: int) -> Colour:
+    def GetColour(self, id: int) -> 'Colour':
         """ Get the colour of a certain setting.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDockArt.html
         """
 
-    def GetFont(self, id: int) -> Font:
+    def GetFont(self, id: int) -> 'Font':
         """ Get a font setting.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDockArt.html
         """
 
     def GetMetric(self, id: int) -> int:
         """ Get the value of a certain setting.
@@ -2928,14 +2928,16 @@
         """ Set a certain setting with the value new_val.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDockArt.html
         """
 
 
 
+AuiManagerOption: TypeAlias = int  # Enumeration
+
 class AuiDefaultToolBarArt(AuiToolBarArt):
     """ AuiDefaultToolBarArt is part of the AUI class framework.
 
         Source: https://docs.wxpython.org/wx.aui.AuiDefaultToolBarArt.html
     """
     def __init__(self) -> None:
         """ 
@@ -3011,33 +3013,33 @@
 
     def GetFlags(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultToolBarArt.html
         """
 
-    def GetFont(self) -> Font:
+    def GetFont(self) -> 'Font':
         """ Font
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultToolBarArt.html
         """
 
-    def GetLabelSize(self, dc, wnd, item) -> Size:
+    def GetLabelSize(self, dc, wnd, item) -> 'Size':
         """ dc (wx.DC) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultToolBarArt.html
         """
 
     def GetTextOrientation(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultToolBarArt.html
         """
 
-    def GetToolSize(self, dc, wnd, item) -> Size:
+    def GetToolSize(self, dc, wnd, item) -> 'Size':
         """ dc (wx.DC) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultToolBarArt.html
         """
 
     def SetElementSize(self, element_id, size) -> None:
         """ element_id (int) â
@@ -3066,15 +3068,15 @@
     def ShowDropDown(self, wnd, items) -> int:
         """ wnd (wx.Window) â
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultToolBarArt.html
         """
 
     Flags: int  # See GetFlags and SetFlags
-    Font: 'Font'  # See GetFont and SetFont
+    Font: '_Font'  # See GetFont and SetFont
     TextOrientation: int  # See GetTextOrientation and SetTextOrientation
 
 
 
 class AuiDefaultDockArt(AuiDockArt):
     """ This is the default art provider for AuiManager.
 
@@ -3130,21 +3132,21 @@
 
     def DrawSash(self, dc, window, orientation, rect) -> None:
         """ Draws a sash between two windows.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultDockArt.html
         """
 
-    def GetColour(self, id: int) -> Colour:
+    def GetColour(self, id: int) -> 'Colour':
         """ Get the colour of a certain setting.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultDockArt.html
         """
 
-    def GetFont(self, id: int) -> Font:
+    def GetFont(self, id: int) -> 'Font':
         """ Get a font setting.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultDockArt.html
         """
 
     def GetMetric(self, id: int) -> int:
         """ Get the value of a certain setting.
@@ -3168,7 +3170,9 @@
         """ Set a certain setting with the value new_val.
 
             Source: https://docs.wxpython.org/wx.aui.AuiDefaultDockArt.html
         """
 
 
 
+AuiPaneInfoArray: TypeAlias = list['AuiPaneInfo']
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/dataview/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/dataview/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class DataViewCtrl(Control):
     """ DataViewCtrl is a control to display data either in a tree like
 fashion or in a tabular form or both.
 
         Source: https://docs.wxpython.org/wx.dataview.DataViewCtrl.html
     """
@@ -150,15 +150,15 @@
     def ExpandChildren(self, item: 'dataview.DataViewItem') -> None:
         """ Expand all children of the given item recursively.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCtrl.html
         """
 
     def GetColumn(self, pos: int) -> 'dataview.DataViewColumn':
         """ Returns pointer to the column.
@@ -210,21 +210,21 @@
 
     def GetIndent(self) -> int:
         """ Returns indentation.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCtrl.html
         """
 
-    def GetItemRect(self, item, col=None) -> Rect:
+    def GetItemRect(self, item, col=None) -> 'Rect':
         """ Returns item rectangle.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCtrl.html
         """
 
-    def GetMainWindow(self) -> Window:
+    def GetMainWindow(self) -> 'Window':
         """ Returns the window corresponding to the main area of the control.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCtrl.html
         """
 
     def GetModel(self) -> 'dataview.DataViewModel':
         """ Returns pointer to the data model associated with the control (if any).
@@ -240,15 +240,15 @@
 
     def GetSelection(self) -> 'dataview.DataViewItem':
         """ Returns first selected item or an invalid item if none is selected.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCtrl.html
         """
 
-    def GetSelections(self) -> DataViewItemArray:
+    def GetSelections(self) -> 'dataview.DataViewItemArray':
         """ Returns a list of the currently selected items.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCtrl.html
         """
 
     def GetSortingColumn(self) -> 'dataview.DataViewColumn':
         """ Returns the   wx.dataview.DataViewColumn  currently responsible for sorting or None if none has been selected.
@@ -415,19 +415,19 @@
     ColumnCount: int  # See GetColumnCount
     Columns: None  # See GetColumns
     CountPerPage: int  # See GetCountPerPage
     CurrentColumn: 'dataview.DataViewColumn'  # See GetCurrentColumn
     CurrentItem: 'dataview.DataViewItem'  # See GetCurrentItem and SetCurrentItem
     ExpanderColumn: 'dataview.DataViewColumn'  # See GetExpanderColumn and SetExpanderColumn
     Indent: int  # See GetIndent and SetIndent
-    MainWindow: Window  # See GetMainWindow
+    MainWindow: 'Window'  # See GetMainWindow
     Model: 'dataview.DataViewModel'  # See GetModel
     SelectedItemsCount: int  # See GetSelectedItemsCount
     Selection: 'dataview.DataViewItem'  # See GetSelection
-    Selections: DataViewItemArray  # See GetSelections and SetSelections
+    Selections: 'dataview.DataViewItemArray'  # See GetSelections and SetSelections
     SortingColumn: 'dataview.DataViewColumn'  # See GetSortingColumn
     TopItem: 'dataview.DataViewItem'  # See GetTopItem
 
 
 
 DV_SINGLE: int  # Single selection mode. This is the default.
 
@@ -548,15 +548,15 @@
 
     def DeleteAllItems(self) -> None:
         """ Delete all tree items.
 
             Source: https://docs.wxpython.org/wx.dataview.TreeListCtrl.html
         """
 
-    def DeleteColumn(self, col: GetColumnCount) -> bool:
+    def DeleteColumn(self, col: int) -> bool:
         """ Delete the column with the given index.
 
             Source: https://docs.wxpython.org/wx.dataview.TreeListCtrl.html
         """
 
     def DeleteItem(self, item: 'dataview.TreeListItem') -> None:
         """ Delete the specified item.
@@ -579,15 +579,15 @@
     def GetCheckedState(self, item: 'dataview.TreeListItem') -> 'CheckBoxState':
         """ Return the checked state of the item.
 
             Source: https://docs.wxpython.org/wx.dataview.TreeListCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.dataview.TreeListCtrl.html
         """
 
     def GetColumnCount(self) -> None:
         """ Return the total number of columns.
@@ -615,15 +615,15 @@
 
     def GetFirstItem(self) -> 'dataview.TreeListItem':
         """ Return the first item in the tree.
 
             Source: https://docs.wxpython.org/wx.dataview.TreeListCtrl.html
         """
 
-    def GetItemData(self, item: 'dataview.TreeListItem') -> ClientData:
+    def GetItemData(self, item: 'dataview.TreeListItem') -> 'ClientData':
         """ Get the data associated with the given item.
 
             Source: https://docs.wxpython.org/wx.dataview.TreeListCtrl.html
         """
 
     def GetItemParent(self, item: 'dataview.TreeListItem') -> 'dataview.TreeListItem':
         """ Return the parent of the given item.
@@ -670,15 +670,15 @@
 
     def GetSortColumn(self) -> tuple:
         """ Return the column currently used for sorting, if any.
 
             Source: https://docs.wxpython.org/wx.dataview.TreeListCtrl.html
         """
 
-    def GetView(self) -> Window:
+    def GetView(self) -> 'Window':
         """ Return the view part of this control as a   wx.Window.
 
             Source: https://docs.wxpython.org/wx.dataview.TreeListCtrl.html
         """
 
     def InsertItem(self, parent, previous, text, imageClosed=-1, imageOpened=-1, data=None) -> 'dataview.TreeListItem':
         """ Insert a new item into the tree.
@@ -792,15 +792,15 @@
     DataView: 'dataview.DataViewCtrl'  # See GetDataView
     FirstItem: 'dataview.TreeListItem'  # See GetFirstItem
     NO_IMAGE: Any  # A public C++ attribute of type int. A constant indicating that no image should be used for an item.
     RootItem: 'dataview.TreeListItem'  # See GetRootItem
     Selection: 'dataview.TreeListItem'  # See GetSelection
     Selections: Any  # See GetSelections
     SortColumn: tuple  # See GetSortColumn and SetSortColumn
-    View: Window  # See GetView
+    View: 'Window'  # See GetView
 
 
 
 TL_SINGLE: int  # Single selection, this is the default.
 
 TL_MULTIPLE: int  # Allow multiple selection, see GetSelections.
 
@@ -897,39 +897,39 @@
     def GetChildCount(self, parent: 'dataview.DataViewItem') -> int:
         """ Calls the identical method from   wx.dataview.DataViewTreeStore.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeCtrl.html
         """
 
-    def GetImageList(self) -> ImageList:
+    def GetImageList(self) -> 'ImageList':
         """ Returns the image list.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeCtrl.html
         """
 
-    def GetItemData(self, item: 'dataview.DataViewItem') -> ClientData:
+    def GetItemData(self, item: 'dataview.DataViewItem') -> 'ClientData':
         """ Calls the identical method from   wx.dataview.DataViewTreeStore.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeCtrl.html
         """
 
-    def GetItemExpandedIcon(self, item: 'dataview.DataViewItem') -> Icon:
+    def GetItemExpandedIcon(self, item: 'dataview.DataViewItem') -> 'Icon':
         """ Calls the identical method from   wx.dataview.DataViewTreeStore.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeCtrl.html
         """
 
-    def GetItemIcon(self, item: 'dataview.DataViewItem') -> Icon:
+    def GetItemIcon(self, item: 'dataview.DataViewItem') -> 'Icon':
         """ Calls the identical method from   wx.dataview.DataViewTreeStore.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeCtrl.html
         """
 
     def GetItemParent(self, item: 'dataview.DataViewItem') -> 'dataview.DataViewItem':
         """ Returns the itemâs parent.
@@ -1011,15 +1011,15 @@
 
     def SetItemText(self, item, text) -> None:
         """ Calls the identical method from   wx.dataview.DataViewTreeStore.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeCtrl.html
         """
 
-    ImageList: 'ImageList'  # See GetImageList and SetImageList
+    ImageList: '_ImageList'  # See GetImageList and SetImageList
     Store: 'dataview.DataViewTreeStore'  # See GetStore
 
 
 
 class DataViewListCtrl(DataViewCtrl):
     """ This class is a DataViewCtrl which internally uses a
 DataViewListStore and forwards most of its API to that class.
@@ -1083,27 +1083,27 @@
     def DeleteItem(self, row: Any) -> None:
         """ Delete the row at position row.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListCtrl.html
         """
 
     def GetItemCount(self) -> int:
         """ Returns the number of items (=rows) in the control.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListCtrl.html
         """
 
-    def GetItemData(self, item: 'dataview.DataViewItem') -> 'UIntPtr':
+    def GetItemData(self, item: 'dataview.DataViewItem') -> int:
         """ Returns the client data associated with the item.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListCtrl.html
         """
 
     def GetSelectedRow(self) -> int:
         """ Returns index of the selected row or wx.NOT_FOUND.
@@ -1125,15 +1125,15 @@
 
     def GetToggleValue(self, row, col) -> bool:
         """ Returns the value from the store.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListCtrl.html
         """
 
-    def GetValue(self, row, col) -> value:
+    def GetValue(self, row, col) -> Any:
         """ Returns the value from the store.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListCtrl.html
         """
 
     def InsertColumn(self, *args, **kw) -> bool:
         """ Overloaded Implementations:
@@ -1271,15 +1271,15 @@
 
     def GetParent(self, item: 'dataview.DataViewItem') -> 'dataview.DataViewItem':
         """ Override this to indicate which   wx.dataview.DataViewItem  representing the parent of item  or an invalid   wx.dataview.DataViewItem  if the root item is the parent item.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewModel.html
         """
 
-    def GetValue(self, item, col) -> variant:
+    def GetValue(self, item, col) -> Any:
         """ Override this to indicate the value of item.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewModel.html
         """
 
     def HasContainerColumns(self, item: 'dataview.DataViewItem') -> bool:
         """ Override this method to indicate if a container item merely acts as a headline (or for categorisation) or if it also acts a normal item with entries for further columns.
@@ -1498,15 +1498,15 @@
 
     def CancelEditing(self) -> None:
         """ 
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewRenderer.html
         """
 
-    def CreateEditorCtrl(self, parent, labelRect, value) -> Window:
+    def CreateEditorCtrl(self, parent, labelRect, value) -> 'Window':
         """ parent (wx.Window) â
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewRenderer.html
         """
 
     def DisableEllipsize(self) -> None:
         """ Disable replacing parts of the item text with ellipsis.
@@ -1528,15 +1528,15 @@
 
     def GetAlignment(self) -> int:
         """ Returns the alignment.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewRenderer.html
         """
 
-    def GetEditorCtrl(self) -> Window:
+    def GetEditorCtrl(self) -> 'Window':
         """ Window
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewRenderer.html
         """
 
     def GetEllipsizeMode(self) -> 'EllipsizeMode':
         """ Returns the ellipsize mode used by the renderer.
@@ -1552,21 +1552,21 @@
 
     def GetOwner(self) -> 'dataview.DataViewColumn':
         """ Returns pointer to the owning   wx.dataview.DataViewColumn.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewRenderer.html
         """
 
-    def GetValue(self) -> value:
+    def GetValue(self) -> Any:
         """ This methods retrieves the value from the renderer in order to transfer the value back to the data model.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewRenderer.html
         """
 
-    def GetValueFromEditorCtrl(self, editor: 'Window') -> value:
+    def GetValueFromEditorCtrl(self, editor: 'Window') -> Any:
         """ editor (wx.Window) â
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewRenderer.html
         """
 
     def GetVariantType(self) -> str:
         """ Returns a string with the type of the Variant       supported by this renderer.
@@ -1625,16 +1625,16 @@
     def Validate(self, value: DVCVariant) -> bool:
         """ Before data is committed to the data model, it is passed to this method where it can be checked for validity.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewRenderer.html
         """
 
     Alignment: int  # See GetAlignment and SetAlignment
-    EditorCtrl: Window  # See GetEditorCtrl
-    EllipsizeMode: 'EllipsizeMode'  # See GetEllipsizeMode
+    EditorCtrl: 'Window'  # See GetEditorCtrl
+    EllipsizeMode: '_EllipsizeMode'  # See GetEllipsizeMode
     Mode: 'dataview.DataViewCellMode'  # See GetMode
     Owner: 'dataview.DataViewColumn'  # See GetOwner and SetOwner
     VariantType: str  # See GetVariantType
     View: 'dataview.DataViewCtrl'  # See GetView
 
 
 
@@ -1662,15 +1662,15 @@
 
     def ActivateCell(self, cell, model, item, col, mouseEvent) -> bool:
         """ Override this to react to cell activation.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCustomRenderer.html
         """
 
-    def CreateEditorCtrl(self, parent, labelRect, value) -> Window:
+    def CreateEditorCtrl(self, parent, labelRect, value) -> 'Window':
         """ Override this to create the actual editor control once editing is about to start.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCustomRenderer.html
         """
 
     def GetAttr(self) -> 'dataview.DataViewItemAttr':
         """ Return the attribute to be used for rendering.
@@ -1681,27 +1681,27 @@
     @staticmethod
     def GetDefaultType() -> str:
         """ Returns the Variant       type used with this renderer.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCustomRenderer.html
         """
 
-    def GetSize(self) -> Size:
+    def GetSize(self) -> 'Size':
         """ Return size required to show content.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCustomRenderer.html
         """
 
-    def GetTextExtent(self, str: str) -> Size:
+    def GetTextExtent(self, str: str) -> 'Size':
         """ Helper for GetSize   implementations, respects attributes.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCustomRenderer.html
         """
 
-    def GetValueFromEditorCtrl(self, editor: 'Window') -> value:
+    def GetValueFromEditorCtrl(self, editor: 'Window') -> Any:
         """ Override this so that the renderer can get the value from the editor control (pointed to by editor):
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCustomRenderer.html
         """
 
     def HasEditorCtrl(self) -> bool:
         """ Override this and make it return True in order to indicate that this renderer supports in-place editing.
@@ -1730,15 +1730,15 @@
     def StartDrag(self, cursor, cell, model, item, col) -> bool:
         """ Override this to start a drag operation.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewCustomRenderer.html
         """
 
     Attr: 'dataview.DataViewItemAttr'  # See GetAttr
-    Size: Size  # See GetSize
+    Size: '_Size'  # See GetSize
 
 
 
 DATAVIEW_CELL_ACTIVATABLE: int
 
 DATAVIEW_CELL_EDITABLE: int
 
@@ -1773,21 +1773,21 @@
 
     def GetDataBuffer(self) -> Any:
         """ Gets the data buffer for a drop data transfer
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewEvent.html
         """
 
-    def GetDataFormat(self) -> DataFormat:
+    def GetDataFormat(self) -> 'DataFormat':
         """ Gets the   wx.DataFormat  during a drop operation.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewEvent.html
         """
 
-    def GetDataObject(self) -> DataObject:
+    def GetDataObject(self) -> 'DataObject':
         """ DataObject
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewEvent.html
         """
 
     def GetDataSize(self) -> int:
         """ Gets the data size for a drop data transfer.
@@ -1821,27 +1821,27 @@
 
     def GetModel(self) -> 'dataview.DataViewModel':
         """ Returns the   wx.dataview.DataViewModel  associated with the event.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewEvent.html
         """
 
-    def GetPosition(self) -> Point:
+    def GetPosition(self) -> 'Point':
         """ Returns the position of a context menu event in client coordinates.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewEvent.html
         """
 
     def GetProposedDropIndex(self) -> int:
         """ Returns the index of the child item at which an item currently being dragged would be dropped.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewEvent.html
         """
 
-    def GetValue(self) -> DVCVariant:
+    def GetValue(self) -> 'dataview.DVCVariant':
         """ Returns a reference to a value.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewEvent.html
         """
 
     def IsEditCancelled(self) -> bool:
         """ Can be used to determine whether the new value is going to be accepted in wxEVT_DATAVIEW_ITEM_EDITING_DONE handler.
@@ -1927,30 +1927,32 @@
             Source: https://docs.wxpython.org/wx.dataview.DataViewEvent.html
         """
 
     CacheFrom: int  # See GetCacheFrom
     CacheTo: int  # See GetCacheTo
     Column: int  # See GetColumn and SetColumn
     DataBuffer: Any  # See GetDataBuffer and SetDataBuffer
-    DataFormat: 'DataFormat'  # See GetDataFormat and SetDataFormat
-    DataObject: 'DataObject'  # See GetDataObject and SetDataObject
+    DataFormat: '_DataFormat'  # See GetDataFormat and SetDataFormat
+    DataObject: '_DataObject'  # See GetDataObject and SetDataObject
     DataSize: int  # See GetDataSize and SetDataSize
     DataViewColumn: 'dataview.DataViewColumn'  # See GetDataViewColumn and SetDataViewColumn
     DragFlags: int  # See GetDragFlags and SetDragFlags
-    DropEffect: DragResult  # See GetDropEffect and SetDropEffect
+    DropEffect: 'DragResult'  # See GetDropEffect and SetDropEffect
     Item: 'dataview.DataViewItem'  # See GetItem and SetItem
     Model: 'dataview.DataViewModel'  # See GetModel and SetModel
-    Position: Point  # See GetPosition and SetPosition
+    Position: 'Point'  # See GetPosition and SetPosition
     ProposedDropIndex: int  # See GetProposedDropIndex
-    Value: DVCVariant  # See GetValue and SetValue
+    Value: 'dataview.DVCVariant'  # See GetValue and SetValue
 
 
 
 EVT_DATAVIEW_CACHE_HINT: int  # Process a  wxEVT_DATAVIEW_CACHE_HINT   event. ^^
 
+DataViewCellMode: TypeAlias = int  # Enumeration
+
 DATAVIEW_CELL_INERT: int
 
 class DataViewIconTextRenderer(DataViewRenderer):
     """ The DataViewIconTextRenderer class is used to display text with a
 small icon next to it as it is typically done in a file manager.
 
         Source: https://docs.wxpython.org/wx.dataview.DataViewIconTextRenderer.html
@@ -2013,21 +2015,21 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewIconText.html
         """
 
-    def GetBitmapBundle(self) -> BitmapBundle:
+    def GetBitmapBundle(self) -> 'BitmapBundle':
         """ Gets the associated image.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewIconText.html
         """
 
-    def GetIcon(self) -> Icon:
+    def GetIcon(self) -> 'Icon':
         """ Gets the icon.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewIconText.html
         """
 
     def GetText(self) -> str:
         """ Gets the text.
@@ -2049,16 +2051,16 @@
 
     def SetText(self, text: str) -> None:
         """ Set the text.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewIconText.html
         """
 
-    BitmapBundle: 'BitmapBundle'  # See GetBitmapBundle and SetBitmapBundle
-    Icon: 'Icon'  # See GetIcon and SetIcon
+    BitmapBundle: '_BitmapBundle'  # See GetBitmapBundle and SetBitmapBundle
+    Icon: '_Icon'  # See GetIcon and SetIcon
     Text: str  # See GetText and SetText
 
 
 
 class TreeListItem:
     """ Unique identifier of an item in TreeListCtrl.
 
@@ -2172,27 +2174,27 @@
 
     def GetChildCount(self, parent: 'dataview.DataViewItem') -> int:
         """ Return the number of children of item.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeStore.html
         """
 
-    def GetItemData(self, item: 'dataview.DataViewItem') -> ClientData:
+    def GetItemData(self, item: 'dataview.DataViewItem') -> 'ClientData':
         """ Returns the client data associated with the item.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeStore.html
         """
 
-    def GetItemExpandedIcon(self, item: 'dataview.DataViewItem') -> Icon:
+    def GetItemExpandedIcon(self, item: 'dataview.DataViewItem') -> 'Icon':
         """ Returns the icon to display in expanded containers.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeStore.html
         """
 
-    def GetItemIcon(self, item: 'dataview.DataViewItem') -> Icon:
+    def GetItemIcon(self, item: 'dataview.DataViewItem') -> 'Icon':
         """ Returns the icon of the item.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewTreeStore.html
         """
 
     def GetItemText(self, item: 'dataview.DataViewItem') -> str:
         """ Returns the text of the item.
@@ -2288,21 +2290,21 @@
 
     def GetItemCount(self) -> int:
         """ Returns the number of items (=rows) in the control.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListStore.html
         """
 
-    def GetItemData(self, item: 'dataview.DataViewItem') -> 'UIntPtr':
+    def GetItemData(self, item: 'dataview.DataViewItem') -> int:
         """ Returns the client data associated with the item.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListStore.html
         """
 
-    def GetValueByRow(self, row, col) -> value:
+    def GetValueByRow(self, row, col) -> Any:
         """ Overridden from   wx.dataview.DataViewIndexListModel.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListStore.html
         """
 
     def InsertColumn(self, pos, varianttype) -> None:
         """ Inserts a data column before pos.
@@ -2591,15 +2593,15 @@
 
     def GetRow(self, item: 'dataview.DataViewItem') -> int:
         """ Returns the position of given item.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListModel.html
         """
 
-    def GetValueByRow(self, row, col) -> variant:
+    def GetValueByRow(self, row, col) -> Any:
         """ Override this to allow getting values from the model.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewListModel.html
         """
 
     def IsEnabledByRow(self, row, col) -> bool:
         """ Override this if you want to disable specific items.
@@ -2625,33 +2627,33 @@
     """
     def __init__(self) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewItemAttr.html
         """
 
-    def GetBackgroundColour(self) -> Colour:
+    def GetBackgroundColour(self) -> 'Colour':
         """ Returns the colour to be used for the background.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewItemAttr.html
         """
 
     def GetBold(self) -> bool:
         """ Returns value of the bold property.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewItemAttr.html
         """
 
-    def GetColour(self) -> Colour:
+    def GetColour(self) -> 'Colour':
         """ Returns this attributeâs colour.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewItemAttr.html
         """
 
-    def GetEffectiveFont(self, font: 'Font') -> Font:
+    def GetEffectiveFont(self, font: 'Font') -> 'Font':
         """ Return the font based on the given one with this attribute applied to it.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewItemAttr.html
         """
 
     def GetItalic(self) -> bool:
         """ Returns value of the italics property.
@@ -2709,17 +2711,17 @@
 
     def SetStrikethrough(self, set: bool) -> None:
         """ Call this to indicate that the item shall be displayed in strikethrough text.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewItemAttr.html
         """
 
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
     Bold: bool  # See GetBold and SetBold
-    Colour: Union[int, str, 'Colour']  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
     Italic: bool  # See GetItalic and SetItalic
 
 
 
 class DataViewToggleRenderer(DataViewRenderer):
     """ This class is used by DataViewCtrl to render toggle controls.
 
@@ -2742,14 +2744,16 @@
         """ Switch to using radiobutton-like appearance instead of the default checkbox-like one.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewToggleRenderer.html
         """
 
 
 
+DataViewColumnFlags: TypeAlias = int  # Enumeration
+
 DATAVIEW_COL_RESIZABLE: int
 
 DATAVIEW_COL_SORTABLE: int
 
 DATAVIEW_COL_REORDERABLE: int
 
 DATAVIEW_COL_HIDDEN: int
@@ -2905,29 +2909,35 @@
             Source: https://docs.wxpython.org/wx.dataview.DataViewChoiceRenderer.html
         """
 
     Choices: list[str]  # See GetChoices
 
 
 
+DataViewCellRenderState: TypeAlias = int  # Enumeration
+
 DATAVIEW_CELL_SELECTED: int
 
 DATAVIEW_CELL_PRELIT: int
 
 DATAVIEW_CELL_INSENSITIVE: int
 
 DATAVIEW_CELL_FOCUSED: int
 
 class DataViewValueAdjuster:
     """ This class can be used with DataViewRenderer.SetValueAdjuster() to
 customize rendering of model values with standard renderers.
 
         Source: https://docs.wxpython.org/wx.dataview.DataViewValueAdjuster.html
     """
-    def MakeHighlighted(self, value: DVCVariant) -> DVCVariant:
+    def MakeHighlighted(self, value: DVCVariant) -> 'dataview.DVCVariant':
         """ Change value for rendering when highlighted.
 
             Source: https://docs.wxpython.org/wx.dataview.DataViewValueAdjuster.html
         """
 
 
 
+DataViewItemArray: TypeAlias = list['DataViewItem']
+
+DVCVariant: TypeAlias = Any
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/glcanvas/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/glcanvas/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class GLCanvas(Window):
     """ GLCanvas is a class for displaying OpenGL graphics.
 
         Source: https://docs.wxpython.org/wx.glcanvas.GLCanvas.html
     """
     def __init__(self, *args, **kw) -> None:
```

### Comparing `types_wxpython-0.6.1/wx-stubs/grid/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/grid/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class Grid(Scrolled):
     """ Grid and its related classes are used for displaying and editing
 tabular data.
 
         Source: https://docs.wxpython.org/wx.grid.Grid.html
     """
@@ -87,21 +87,21 @@
 
     def BeginBatch(self) -> None:
         """ Increments the gridâs batch count.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def BlockToDeviceRect(self, topLeft, bottomRight, gridWindow=None) -> Rect:
+    def BlockToDeviceRect(self, topLeft, bottomRight, gridWindow=None) -> 'Rect':
         """ Convert grid cell coordinates to grid window pixel coordinates.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def CalcCellsExposed(self, reg, gridWindow=None) -> GridCellCoordsArray:
+    def CalcCellsExposed(self, reg, gridWindow=None) -> 'grid.GridCellCoordsArray':
         """ Appends one or more new columns to the right of the grid.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def CalcColLabelsExposed(self, reg, gridWindow=None) -> list[int]:
         """ Appends one or more new columns to the right of the grid.
@@ -195,15 +195,15 @@
 
     def CellToGridWindow(self, *args, **kw) -> 'grid.GridWindow':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def CellToRect(self, *args, **kw) -> Rect:
+    def CellToRect(self, *args, **kw) -> 'Rect':
         """ Return the rectangle corresponding to the grid cellâs size and position in logical coordinates.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def ClearGrid(self) -> None:
         """ Clears all data in the underlying grid table and repaints the grid.
@@ -465,15 +465,15 @@
 
     def GetCellAlignment(self, row, col) -> tuple:
         """ Sets the arguments to the horizontal and vertical text alignment values for the grid cell at the specified location.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetCellBackgroundColour(self, row, col) -> Colour:
+    def GetCellBackgroundColour(self, row, col) -> 'Colour':
         """ Returns the background colour of the cell at the specified location.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetCellEditor(self, row, col) -> 'grid.GridCellEditor':
         """ Returns a pointer to the editor for the cell at the specified location.
@@ -483,21 +483,21 @@
 
     def GetCellFitMode(self, row, col) -> 'grid.GridFitMode':
         """ Returns the cell fitting mode.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetCellFont(self, row, col) -> Font:
+    def GetCellFont(self, row, col) -> 'Font':
         """ Returns the font for text in the grid cell at the specified location.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetCellHighlightColour(self) -> Colour:
+    def GetCellHighlightColour(self) -> 'Colour':
         """ Colour
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetCellHighlightPenWidth(self) -> int:
         """ int
@@ -525,40 +525,40 @@
 
     def GetCellSize(self, *args, **kw) -> 'grid.Grid.CellSpan':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetCellTextColour(self, row, col) -> Colour:
+    def GetCellTextColour(self, row, col) -> 'Colour':
         """ Returns the text colour for the grid cell at the specified location.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetCellValue(self, *args, **kw) -> str:
         """ Returns the string contained in the cell at the specified location.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetColAt(self, colPos: int) -> int:
         """ Returns the column ID of the specified column position.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetColGridLinePen(self, col: int) -> Pen:
+    def GetColGridLinePen(self, col: int) -> 'Pen':
         """ Returns the pen used for vertical grid lines.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetColLabelAlignment(self) -> tuple:
         """ Sets the arguments to the current column label alignment values.
@@ -646,39 +646,39 @@
 
     def GetDefaultCellAlignment(self) -> tuple:
         """ Returns the default cell alignment.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetDefaultCellBackgroundColour(self) -> Colour:
+    def GetDefaultCellBackgroundColour(self) -> 'Colour':
         """ Returns the current default background colour for grid cells.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetDefaultCellFitMode(self) -> 'grid.GridFitMode':
         """ Returns the default cell fitting mode.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetDefaultCellFont(self) -> Font:
+    def GetDefaultCellFont(self) -> 'Font':
         """ Returns the current default font for grid cell text.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetDefaultCellOverflow(self) -> bool:
         """ Returns True if the cells can overflow by default.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetDefaultCellTextColour(self) -> Colour:
+    def GetDefaultCellTextColour(self) -> 'Colour':
         """ Returns the current default colour for grid cell text.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetDefaultColLabelSize(self) -> int:
         """ Returns the default height for column labels.
@@ -706,15 +706,15 @@
 
     def GetDefaultEditorForType(self, typeName: str) -> 'grid.GridCellEditor':
         """ Returns the default editor for the cells containing values of the given type.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetDefaultGridLinePen(self) -> Pen:
+    def GetDefaultGridLinePen(self) -> 'Pen':
         """ Returns the pen used for grid lines.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetDefaultRenderer(self) -> 'grid.GridCellRenderer':
         """ Returns a pointer to the current default grid cell renderer.
@@ -754,45 +754,45 @@
 
     def GetFirstFullyVisibleRow(self) -> int:
         """ Returns the topmost row of the current visible area.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetFrozenColGridWindow(self) -> Window:
+    def GetFrozenColGridWindow(self) -> 'Window':
         """ Return the columns grid window containing column frozen cells.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetFrozenCornerGridWindow(self) -> Window:
+    def GetFrozenCornerGridWindow(self) -> 'Window':
         """ Return the corner grid window containing frozen cells.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetFrozenRowGridWindow(self) -> Window:
+    def GetFrozenRowGridWindow(self) -> 'Window':
         """ Return the rows grid window containing row frozen cells.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetGridColHeader(self) -> HeaderCtrl:
+    def GetGridColHeader(self) -> 'HeaderCtrl':
         """ Return the header control used for column labels display.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetGridColLabelWindow(self) -> Window:
+    def GetGridColLabelWindow(self) -> 'Window':
         """ Return the column labels window.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetGridCornerLabelWindow(self) -> Window:
+    def GetGridCornerLabelWindow(self) -> 'Window':
         """ Return the window in the top left grid corner.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetGridCursorCol(self) -> int:
         """ Returns the current grid cell column position.
@@ -808,51 +808,51 @@
 
     def GetGridCursorRow(self) -> int:
         """ Returns the current grid cell row position.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetGridLineColour(self) -> Colour:
+    def GetGridLineColour(self) -> 'Colour':
         """ Returns the colour used for grid lines.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetGridRowLabelWindow(self) -> Window:
+    def GetGridRowLabelWindow(self) -> 'Window':
         """ Return the row labels window.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetGridWindow(self) -> Window:
+    def GetGridWindow(self) -> 'Window':
         """ Return the main grid window containing the grid cells.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetGridWindowOffset(self, gridWindow: 'grid.GridWindow') -> Point:
+    def GetGridWindowOffset(self, gridWindow: 'grid.GridWindow') -> 'Point':
         """ This is an overloaded member function, provided for convenience. It differs from the above function only in what argument(s) it accepts.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetLabelBackgroundColour(self) -> Colour:
+    def GetLabelBackgroundColour(self) -> 'Colour':
         """ Returns the colour used for the background of row and column labels.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetLabelFont(self) -> Font:
+    def GetLabelFont(self) -> 'Font':
         """ Returns the font used for row and column labels.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetLabelTextColour(self) -> Colour:
+    def GetLabelTextColour(self) -> 'Colour':
         """ Returns the colour used for row and column label text.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetNumberCols(self) -> int:
         """ Returns the total number of grid columns.
@@ -892,15 +892,15 @@
 
     def GetRowAt(self, rowPos: int) -> int:
         """ Returns the row ID of the specified row position.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetRowGridLinePen(self, row: int) -> Pen:
+    def GetRowGridLinePen(self, row: int) -> 'Pen':
         """ Returns the pen used for horizontal grid lines.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetRowLabelAlignment(self) -> tuple:
         """ Returns the alignment used for row labels.
@@ -964,15 +964,15 @@
 
     def GetSelectedBlocks(self) -> 'grid.GridBlocks':
         """ Returns a range of grid selection blocks.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetSelectedCells(self) -> GridCellCoordsArray:
+    def GetSelectedCells(self) -> 'grid.GridCellCoordsArray':
         """ Returns an array of individually selected cells.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetSelectedColBlocks(self) -> Any:
         """ Returns an ordered range of non-overlapping selected columns.
@@ -994,39 +994,39 @@
 
     def GetSelectedRows(self) -> list[int]:
         """ Returns an array of selected rows.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetSelectionBackground(self) -> Colour:
+    def GetSelectionBackground(self) -> 'Colour':
         """ Returns the colour used for drawing the selection background.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetSelectionBlockBottomRight(self) -> GridCellCoordsArray:
+    def GetSelectionBlockBottomRight(self) -> 'grid.GridCellCoordsArray':
         """ Returns an array of the bottom right corners of blocks of selected cells.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetSelectionBlockTopLeft(self) -> GridCellCoordsArray:
+    def GetSelectionBlockTopLeft(self) -> 'grid.GridCellCoordsArray':
         """ Returns an array of the top left corners of blocks of selected cells.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetSelectionForeground(self) -> Colour:
+    def GetSelectionForeground(self) -> 'Colour':
         """ Returns the colour used for drawing the selection foreground.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
-    def GetSelectionMode(self) -> 'grid.Grid.GridSelectionModes':
+    def GetSelectionMode(self) -> 'grid.GridSelectionModes':
         """ Returns the current selection mode.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     def GetSortingColumn(self) -> int:
         """ Return the column in which the sorting indicator is currently displayed.
@@ -1793,72 +1793,72 @@
     def YToRow(self, y, clipToMinMax=False, gridWindow=None) -> int:
         """ Returns the grid row that corresponds to the logical y  coordinate.
 
             Source: https://docs.wxpython.org/wx.grid.Grid.html
         """
 
     BatchCount: int  # See GetBatchCount
-    CellHighlightColour: Union[int, str, 'Colour']  # See GetCellHighlightColour and SetCellHighlightColour
+    CellHighlightColour: 'Colour'  # See GetCellHighlightColour and SetCellHighlightColour
     CellHighlightPenWidth: int  # See GetCellHighlightPenWidth and SetCellHighlightPenWidth
     CellHighlightROPenWidth: int  # See GetCellHighlightROPenWidth and SetCellHighlightROPenWidth
     ColLabelSize: int  # See GetColLabelSize and SetColLabelSize
     ColLabelTextOrientation: int  # See GetColLabelTextOrientation and SetColLabelTextOrientation
     ColMinimalAcceptableWidth: int  # See GetColMinimalAcceptableWidth and SetColMinimalAcceptableWidth
     ColSizes: 'grid.GridSizesInfo'  # See GetColSizes and SetColSizes
     CornerLabelTextOrientation: int  # See GetCornerLabelTextOrientation and SetCornerLabelTextOrientation
     CornerLabelValue: str  # See GetCornerLabelValue and SetCornerLabelValue
-    DefaultCellBackgroundColour: Union[int, str, 'Colour']  # See GetDefaultCellBackgroundColour and SetDefaultCellBackgroundColour
+    DefaultCellBackgroundColour: 'Colour'  # See GetDefaultCellBackgroundColour and SetDefaultCellBackgroundColour
     DefaultCellFitMode: 'grid.GridFitMode'  # See GetDefaultCellFitMode and SetDefaultCellFitMode
     DefaultCellFont: 'Font'  # See GetDefaultCellFont and SetDefaultCellFont
     DefaultCellOverflow: bool  # See GetDefaultCellOverflow and SetDefaultCellOverflow
-    DefaultCellTextColour: Union[int, str, 'Colour']  # See GetDefaultCellTextColour and SetDefaultCellTextColour
+    DefaultCellTextColour: 'Colour'  # See GetDefaultCellTextColour and SetDefaultCellTextColour
     DefaultColLabelSize: int  # See GetDefaultColLabelSize
     DefaultColSize: int  # See GetDefaultColSize and SetDefaultColSize
     DefaultEditor: 'grid.GridCellEditor'  # See GetDefaultEditor and SetDefaultEditor
-    DefaultGridLinePen: Pen  # See GetDefaultGridLinePen
+    DefaultGridLinePen: 'Pen'  # See GetDefaultGridLinePen
     DefaultRenderer: 'grid.GridCellRenderer'  # See GetDefaultRenderer and SetDefaultRenderer
     DefaultRowLabelSize: int  # See GetDefaultRowLabelSize
     DefaultRowSize: int  # See GetDefaultRowSize and SetDefaultRowSize
     FirstFullyVisibleColumn: int  # See GetFirstFullyVisibleColumn
     FirstFullyVisibleRow: int  # See GetFirstFullyVisibleRow
-    FrozenColGridWindow: Window  # See GetFrozenColGridWindow
-    FrozenCornerGridWindow: Window  # See GetFrozenCornerGridWindow
-    FrozenRowGridWindow: Window  # See GetFrozenRowGridWindow
-    GridColHeader: HeaderCtrl  # See GetGridColHeader
-    GridColLabelWindow: Window  # See GetGridColLabelWindow
-    GridCornerLabelWindow: Window  # See GetGridCornerLabelWindow
+    FrozenColGridWindow: 'Window'  # See GetFrozenColGridWindow
+    FrozenCornerGridWindow: 'Window'  # See GetFrozenCornerGridWindow
+    FrozenRowGridWindow: 'Window'  # See GetFrozenRowGridWindow
+    GridColHeader: 'HeaderCtrl'  # See GetGridColHeader
+    GridColLabelWindow: 'Window'  # See GetGridColLabelWindow
+    GridCornerLabelWindow: 'Window'  # See GetGridCornerLabelWindow
     GridCursorCol: int  # See GetGridCursorCol
     GridCursorCoords: 'grid.GridCellCoords'  # See GetGridCursorCoords
     GridCursorRow: int  # See GetGridCursorRow
-    GridLineColour: Union[int, str, 'Colour']  # See GetGridLineColour and SetGridLineColour
-    GridRowLabelWindow: Window  # See GetGridRowLabelWindow
-    GridWindow: Window  # See GetGridWindow
-    LabelBackgroundColour: Union[int, str, 'Colour']  # See GetLabelBackgroundColour and SetLabelBackgroundColour
+    GridLineColour: 'Colour'  # See GetGridLineColour and SetGridLineColour
+    GridRowLabelWindow: 'Window'  # See GetGridRowLabelWindow
+    GridWindow: 'Window'  # See GetGridWindow
+    LabelBackgroundColour: 'Colour'  # See GetLabelBackgroundColour and SetLabelBackgroundColour
     LabelFont: 'Font'  # See GetLabelFont and SetLabelFont
-    LabelTextColour: Union[int, str, 'Colour']  # See GetLabelTextColour and SetLabelTextColour
+    LabelTextColour: 'Colour'  # See GetLabelTextColour and SetLabelTextColour
     NumberCols: int  # See GetNumberCols
     NumberFrozenCols: int  # See GetNumberFrozenCols
     NumberFrozenRows: int  # See GetNumberFrozenRows
     NumberRows: int  # See GetNumberRows
     RowLabelSize: int  # See GetRowLabelSize and SetRowLabelSize
     RowMinimalAcceptableHeight: int  # See GetRowMinimalAcceptableHeight and SetRowMinimalAcceptableHeight
     RowSizes: 'grid.GridSizesInfo'  # See GetRowSizes and SetRowSizes
     ScrollLineX: int  # See GetScrollLineX and SetScrollLineX
     ScrollLineY: int  # See GetScrollLineY and SetScrollLineY
     SelectedBlocks: 'grid.GridBlocks'  # See GetSelectedBlocks
-    SelectedCells: GridCellCoordsArray  # See GetSelectedCells
+    SelectedCells: 'grid.GridCellCoordsArray'  # See GetSelectedCells
     SelectedColBlocks: Any  # See GetSelectedColBlocks
     SelectedCols: list[int]  # See GetSelectedCols
     SelectedRowBlocks: Any  # See GetSelectedRowBlocks
     SelectedRows: list[int]  # See GetSelectedRows
-    SelectionBackground: Union[int, str, 'Colour']  # See GetSelectionBackground and SetSelectionBackground
-    SelectionBlockBottomRight: GridCellCoordsArray  # See GetSelectionBlockBottomRight
-    SelectionBlockTopLeft: GridCellCoordsArray  # See GetSelectionBlockTopLeft
-    SelectionForeground: Union[int, str, 'Colour']  # See GetSelectionForeground and SetSelectionForeground
-    SelectionMode: GridSelectionModes  # See GetSelectionMode and SetSelectionMode
+    SelectionBackground: 'Colour'  # See GetSelectionBackground and SetSelectionBackground
+    SelectionBlockBottomRight: 'grid.GridCellCoordsArray'  # See GetSelectionBlockBottomRight
+    SelectionBlockTopLeft: 'grid.GridCellCoordsArray'  # See GetSelectionBlockTopLeft
+    SelectionForeground: 'Colour'  # See GetSelectionForeground and SetSelectionForeground
+    SelectionMode: 'grid.GridSelectionModes'  # See GetSelectionMode and SetSelectionMode
     SortingColumn: int  # See GetSortingColumn and SetSortingColumn
     Table: 'grid.GridTableBase'  # See GetTable and SetTable
 
 
 
 class GridCellAttrProvider(ClientDataContainer):
     """ Class providing attributes to be used for the grid cells.
@@ -1936,27 +1936,27 @@
 
     def GetCol(self) -> int:
         """ Returns the column at which the event occurred.
 
             Source: https://docs.wxpython.org/wx.grid.GridEditorCreatedEvent.html
         """
 
-    def GetControl(self) -> Control:
+    def GetControl(self) -> 'Control':
         """ Returns the edit control.
 
             Source: https://docs.wxpython.org/wx.grid.GridEditorCreatedEvent.html
         """
 
     def GetRow(self) -> int:
         """ Returns the row at which the event occurred.
 
             Source: https://docs.wxpython.org/wx.grid.GridEditorCreatedEvent.html
         """
 
-    def GetWindow(self) -> Window:
+    def GetWindow(self) -> 'Window':
         """ Returns the edit window.
 
             Source: https://docs.wxpython.org/wx.grid.GridEditorCreatedEvent.html
         """
 
     def SetCol(self, col: int) -> None:
         """ Sets the column at which the event occurred.
@@ -1979,17 +1979,17 @@
     def SetWindow(self, window: 'Window') -> None:
         """ Sets the edit window.
 
             Source: https://docs.wxpython.org/wx.grid.GridEditorCreatedEvent.html
         """
 
     Col: int  # See GetCol and SetCol
-    Control: 'Control'  # See GetControl and SetControl
+    Control: '_Control'  # See GetControl and SetControl
     Row: int  # See GetRow and SetRow
-    Window: 'Window'  # See GetWindow and SetWindow
+    Window: '_Window'  # See GetWindow and SetWindow
 
 
 
 EVT_GRID_EDITOR_CREATED: int  # The editor for a cell was created. Processes a  wxEVT_GRID_EDITOR_CREATED   event type.
 
 EVT_GRID_CMD_EDITOR_CREATED: int  # The editor for a cell was created; variant taking a window identifier. Processes a  wxEVT_GRID_EDITOR_CREATED   event type. ^^
 
@@ -2405,27 +2405,27 @@
 
     def GetBestHeight(self, grid, attr, dc, row, col, width) -> int:
         """ Get the preferred height of the cell at the given width.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellRenderer.html
         """
 
-    def GetBestSize(self, grid, attr, dc, row, col) -> Size:
+    def GetBestSize(self, grid, attr, dc, row, col) -> 'Size':
         """ Get the preferred size of the cell for its contents.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellRenderer.html
         """
 
     def GetBestWidth(self, grid, attr, dc, row, col, height) -> int:
         """ Get the preferred width of the cell at the given height.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellRenderer.html
         """
 
-    def GetMaxBestSize(self, grid, attr, dc) -> Size:
+    def GetMaxBestSize(self, grid, attr, dc) -> 'Size':
         """ Get the maximum possible size for a cell using this renderer, if possible.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellRenderer.html
         """
 
 
 
@@ -2592,45 +2592,45 @@
 
     def GetAlignment(self) -> tuple:
         """ Get the alignment to use for the cell with the given attribute.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
-    def GetBackgroundColour(self) -> Colour:
+    def GetBackgroundColour(self) -> 'Colour':
         """ Returns the background colour.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
     def GetEditor(self, grid, row, col) -> 'grid.GridCellEditor':
         """ Returns the cell editor.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
-    def GetEditorPtr(self, grid, row, col) -> 'grid.GridCellEditorPtr':
+    def GetEditorPtr(self, grid, row, col) -> 'grid.GridCellEditor':
         """ Returns the cell editor.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
     def GetFitMode(self) -> 'grid.GridFitMode':
         """ Returns the fitting mode for the cells using this attribute.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
-    def GetFont(self) -> Font:
+    def GetFont(self) -> 'Font':
         """ Returns the font.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
-    def GetKind(self) -> 'grid.GridCellAttr.AttrKind':
+    def GetKind(self) -> 'grid.AttrKind':
         """ wx.grid.GridCellAttr.AttrKind
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
     def GetNonDefaultAlignment(self) -> tuple:
         """ Get the alignment defined by this attribute.
@@ -2652,15 +2652,15 @@
 
     def GetSize(self) -> tuple:
         """ tuple
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
-    def GetTextColour(self) -> Colour:
+    def GetTextColour(self) -> 'Colour':
         """ Returns the text colour.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
     def HasAlignment(self) -> bool:
         """ Returns True if this attribute has a valid alignment set.
@@ -2802,20 +2802,20 @@
 
     def SetTextColour(self, colText: Union[int, str, 'Colour']) -> None:
         """ Sets the text colour.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellAttr.html
         """
 
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
     FitMode: 'grid.GridFitMode'  # See GetFitMode and SetFitMode
-    Font: 'Font'  # See GetFont and SetFont
-    Kind: AttrKind  # See GetKind and SetKind
+    Font: '_Font'  # See GetFont and SetFont
+    Kind: 'grid.AttrKind'  # See GetKind and SetKind
     Overflow: bool  # See GetOverflow and SetOverflow
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
 
 
 
 ALIGN_LEFT: int
 
 ALIGN_INVALID: int
 
@@ -2869,27 +2869,27 @@
 
     def EndEdit(self, row, col, grid, oldval) -> None:
         """ End editing the cell.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellEditor.html
         """
 
-    def GetControl(self) -> Control:
+    def GetControl(self) -> 'Control':
         """ Get the   wx.Control  used by this editor.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellEditor.html
         """
 
     def GetValue(self) -> str:
         """ Returns the value currently in the editor control.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellEditor.html
         """
 
-    def GetWindow(self) -> Window:
+    def GetWindow(self) -> 'Window':
         """ Get the edit window used by this editor.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellEditor.html
         """
 
     def HandleReturn(self, event: 'KeyEvent') -> None:
         """ Some types of controls on some platforms may need some help with the Return key.
@@ -2959,17 +2959,17 @@
 
     def TryActivate(self, row, col, grid, actSource) -> 'grid.GridActivationResult':
         """ Function allowing to create an âactivatableâ editor.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellEditor.html
         """
 
-    Control: 'Control'  # See GetControl and SetControl
+    Control: '_Control'  # See GetControl and SetControl
     Value: str  # See GetValue
-    Window: 'Window'  # See GetWindow and SetWindow
+    Window: '_Window'  # See GetWindow and SetWindow
 
 
 
 class GridCellBoolEditor(GridCellEditor):
     """ Grid cell editor for boolean data.
 
         Source: https://docs.wxpython.org/wx.grid.GridCellBoolEditor.html
@@ -3153,15 +3153,15 @@
 
     def GetCol(self) -> int:
         """ Column at which the event occurred.
 
             Source: https://docs.wxpython.org/wx.grid.GridEvent.html
         """
 
-    def GetPosition(self) -> Point:
+    def GetPosition(self) -> 'Point':
         """ Position in pixels at which the event occurred.
 
             Source: https://docs.wxpython.org/wx.grid.GridEvent.html
         """
 
     def GetRow(self) -> int:
         """ Row at which the event occurred.
@@ -3184,15 +3184,15 @@
     def ShiftDown(self) -> bool:
         """ Returns True if the Shift key was down at the time of the event.
 
             Source: https://docs.wxpython.org/wx.grid.GridEvent.html
         """
 
     Col: int  # See GetCol
-    Position: Point  # See GetPosition
+    Position: 'Point'  # See GetPosition
     Row: int  # See GetRow
 
 
 
 EVT_GRID_CELL_CHANGING: int  # The user is about to change the data in a cell. The new cell value as string is available from GetString  event object method. This event can be vetoed if the change is not allowed. Processes a  wxEVT_GRID_CELL_CHANGING   event type.
 
 EVT_GRID_CELL_CHANGED: int  # The user changed the data in a cell. The old cell value as string is available from GetString  event object method. Notice that vetoing this event still works for backwards compatibility reasons but any new code should only veto EVT_GRID_CELL_CHANGING event and not this one. Processes a  wxEVT_GRID_CELL_CHANGED   event type.
@@ -3246,15 +3246,15 @@
 
     def ControlDown(self) -> bool:
         """ Returns True if the Control key was down at the time of the event.
 
             Source: https://docs.wxpython.org/wx.grid.GridSizeEvent.html
         """
 
-    def GetPosition(self) -> Point:
+    def GetPosition(self) -> 'Point':
         """ Position in pixels at which the event occurred.
 
             Source: https://docs.wxpython.org/wx.grid.GridSizeEvent.html
         """
 
     def GetRowOrCol(self) -> int:
         """ Row or column at that was resized.
@@ -3270,15 +3270,15 @@
 
     def ShiftDown(self) -> bool:
         """ Returns True if the Shift key was down at the time of the event.
 
             Source: https://docs.wxpython.org/wx.grid.GridSizeEvent.html
         """
 
-    Position: Point  # See GetPosition
+    Position: 'Point'  # See GetPosition
     RowOrCol: int  # See GetRowOrCol
 
 
 
 EVT_GRID_CMD_COL_SIZE: int  # The user resized a column, corresponds to  wxEVT_GRID_COL_SIZE   event type.
 
 EVT_GRID_CMD_ROW_SIZE: int  # The user resized a row, corresponds to  wxEVT_GRID_ROW_SIZE   event type.
@@ -3589,15 +3589,15 @@
     @staticmethod
     def Overflow() -> 'grid.GridFitMode':
         """ Pseudo-constructor for object specifying overflow behaviour.
 
             Source: https://docs.wxpython.org/wx.grid.GridFitMode.html
         """
 
-    EllipsizeMode: 'EllipsizeMode'  # See GetEllipsizeMode
+    EllipsizeMode: '_EllipsizeMode'  # See GetEllipsizeMode
 
 
 
 class GridSizesInfo:
     """ GridSizesInfo stores information about sizes of all Grid rows or
 columns.
 
@@ -3800,14 +3800,16 @@
         """ Sets the comma separated string content of the enum.
 
             Source: https://docs.wxpython.org/wx.grid.GridCellEnumRenderer.html
         """
 
 
 
+GridCellFloatFormat: TypeAlias = int  # Enumeration
+
 GRID_FLOAT_FORMAT_FIXED: int
 
 GRID_FLOAT_FORMAT_SCIENTIFIC: int
 
 GRID_FLOAT_FORMAT_COMPACT: int
 
 GRID_FLOAT_FORMAT_UPPER: int
@@ -3874,34 +3876,34 @@
 
 class GridActivationSource:
     """ Represents a source of cell activation, which may be either a user
 event (mouse or keyboard) or the program itself.
 
         Source: https://docs.wxpython.org/wx.grid.GridActivationSource.html
     """
-    def GetKeyEvent(self) -> KeyEvent:
+    def GetKeyEvent(self) -> 'KeyEvent':
         """ Get the key event corresponding to the key press activating the cell.
 
             Source: https://docs.wxpython.org/wx.grid.GridActivationSource.html
         """
 
-    def GetMouseEvent(self) -> MouseEvent:
+    def GetMouseEvent(self) -> 'MouseEvent':
         """ Get the mouse event corresponding to the click activating the cell.
 
             Source: https://docs.wxpython.org/wx.grid.GridActivationSource.html
         """
 
     def GetOrigin(self) -> 'grid.GridActivationSource.Origin':
         """ Get the origin of the activation.
 
             Source: https://docs.wxpython.org/wx.grid.GridActivationSource.html
         """
 
-    KeyEvent: KeyEvent  # See GetKeyEvent
-    MouseEvent: MouseEvent  # See GetMouseEvent
+    KeyEvent: '_KeyEvent'  # See GetKeyEvent
+    MouseEvent: '_MouseEvent'  # See GetMouseEvent
 
 
 
 class GridActivationResult:
     """ Represents the result of GridCellEditor.TryActivate().
 
         Source: https://docs.wxpython.org/wx.grid.GridActivationResult.html
@@ -3944,7 +3946,19 @@
         """ Called by the grid to draw the specified label.
 
             Source: https://docs.wxpython.org/wx.grid.GridHeaderLabelsRenderer.html
         """
 
 
 
+GridCellCoordsArray: TypeAlias = list['GridCellCoords']
+
+GridSelectionModes: TypeAlias = int
+
+AttrKind: TypeAlias = int
+
+GridWindow: TypeAlias = Any
+
+GridCellAttrPtr: TypeAlias = Any
+
+TabBehaviour: TypeAlias = int  # Enumeration
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/html/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/html/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class HtmlCellEvent(CommandEvent):
     """ This event class is used for the events generated by HtmlWindow.
 
         Source: https://docs.wxpython.org/wx.html.HtmlCellEvent.html
     """
     def __init__(self, commandType, id, cell, point, ev) -> None:
@@ -20,36 +20,36 @@
 
     def GetLinkClicked(self) -> bool:
         """ Returns True if SetLinkClicked(true) has previously been called; False otherwise.
 
             Source: https://docs.wxpython.org/wx.html.HtmlCellEvent.html
         """
 
-    def GetMouseEvent(self) -> MouseEvent:
+    def GetMouseEvent(self) -> 'MouseEvent':
         """ Returns the   wx.MouseEvent  associated with the event.
 
             Source: https://docs.wxpython.org/wx.html.HtmlCellEvent.html
         """
 
-    def GetPoint(self) -> Point:
+    def GetPoint(self) -> 'Point':
         """ Returns the   wx.Point  associated with the event.
 
             Source: https://docs.wxpython.org/wx.html.HtmlCellEvent.html
         """
 
     def SetLinkClicked(self, linkclicked: bool) -> None:
         """ Call this function with linkclicked  set to True if the cell which has been clicked contained a link or False otherwise (which is the default).
 
             Source: https://docs.wxpython.org/wx.html.HtmlCellEvent.html
         """
 
     Cell: 'html.HtmlCell'  # See GetCell
     LinkClicked: bool  # See GetLinkClicked and SetLinkClicked
-    MouseEvent: MouseEvent  # See GetMouseEvent
-    Point: Point  # See GetPoint
+    MouseEvent: '_MouseEvent'  # See GetMouseEvent
+    Point: '_Point'  # See GetPoint
 
 
 
 EVT_HTML_CELL_HOVER: int  # User moved the mouse over a   wx.html.HtmlCell.
 
 EVT_HTML_CELL_CLICKED: int  # User clicked on a   wx.html.HtmlCell. When handling this event, remember to use HtmlCell.SetLinkClicked(true) if the cell contains a link. ^^
 
@@ -134,15 +134,15 @@
     def DisplayIndex(self) -> bool:
         """ Displays index panel.
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpWindow.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpWindow.html
         """
 
     def GetController(self) -> 'html.HtmlHelpController':
         """ wx.html.HtmlHelpController
@@ -214,15 +214,15 @@
     def Create(self, parent, id=ID_ANY, pos=DefaultPosition, size=DefaultSize, choices=[], style=HLB_DEFAULT_STYLE, validator=DefaultValidator, name=SimpleHtmlListBoxNameStr) -> bool:
         """ Creates the HTML listbox for two-step construction.
 
             Source: https://docs.wxpython.org/wx.html.SimpleHtmlListBox.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.html.SimpleHtmlListBox.html
         """
 
 
 
@@ -256,15 +256,15 @@
     def Create(self, parent, id=ID_ANY, title="", style=HF_DEFAULT_STYLE) -> bool:
         """ Creates the dialog.
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpDialog.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpDialog.html
         """
 
     def GetController(self) -> 'html.HtmlHelpController':
         """ Returns the help controller associated with the dialog.
@@ -308,15 +308,15 @@
     def Create(self, parent, id=ID_ANY, title="", style=HF_DEFAULT_STYLE, config=None, rootpath="") -> bool:
         """ Creates the frame.
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpFrame.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpFrame.html
         """
 
     def GetController(self) -> 'html.HtmlHelpController':
         """ Returns the help controller associated with the frame.
@@ -535,15 +535,15 @@
 
     def FindCellByPos(self, x, y, flags=HTML_FIND_EXACT) -> 'html.HtmlCell':
         """ Find a cell inside this cell positioned at the given coordinates (relative to thisâs positions).
 
             Source: https://docs.wxpython.org/wx.html.HtmlCell.html
         """
 
-    def GetAbsPos(self, rootCell: Optional['html.HtmlCell']=None) -> Point:
+    def GetAbsPos(self, rootCell: Optional['html.HtmlCell']=None) -> 'Point':
         """ rootCell (wx.html.HtmlCell) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlCell.html
         """
 
     def GetDescent(self) -> int:
         """ Returns descent value of the cell (m_Descent member).
@@ -571,21 +571,21 @@
 
     def GetLink(self, x=0, y=0) -> 'html.HtmlLinkInfo':
         """ Returns hypertext link if associated with this cell or None otherwise.
 
             Source: https://docs.wxpython.org/wx.html.HtmlCell.html
         """
 
-    def GetMouseCursor(self, window: 'html.HtmlWindowInterface') -> Cursor:
+    def GetMouseCursor(self, window: 'html.HtmlWindowInterface') -> 'Cursor':
         """ Returns cursor to show when mouse pointer is over the cell.
 
             Source: https://docs.wxpython.org/wx.html.HtmlCell.html
         """
 
-    def GetMouseCursorAt(self, window, rePos) -> Cursor:
+    def GetMouseCursorAt(self, window, rePos) -> 'Cursor':
         """ Returns cursor to show when mouse pointer is over the specified point.
 
             Source: https://docs.wxpython.org/wx.html.HtmlCell.html
         """
 
     def GetNext(self) -> 'html.HtmlCell':
         """ Returns pointer to the next cell in list (see htmlcell.h       if youâre interested in details).
@@ -661,15 +661,15 @@
 
     def SetPos(self, x, y) -> None:
         """ Sets the cellâs position within parent container.
 
             Source: https://docs.wxpython.org/wx.html.HtmlCell.html
         """
 
-    AbsPos: Point  # See GetAbsPos
+    AbsPos: 'Point'  # See GetAbsPos
     Descent: int  # See GetDescent
     FirstChild: 'html.HtmlCell'  # See GetFirstChild
     Height: int  # See GetHeight
     Id: str  # See GetId and SetId
     Link: 'html.HtmlLinkInfo'  # See GetLink and SetLink
     Next: 'html.HtmlCell'  # See GetNext and SetNext
     Parent: 'html.HtmlContainerCell'  # See GetParent and SetParent
@@ -771,27 +771,27 @@
 
     def GetName(self) -> str:
         """ Returns the current name being used for preview frames and setup dialogs.
 
             Source: https://docs.wxpython.org/wx.html.HtmlEasyPrinting.html
         """
 
-    def GetPageSetupData(self) -> PageSetupDialogData:
+    def GetPageSetupData(self) -> 'PageSetupDialogData':
         """ Returns a pointer to   wx.PageSetupDialogData  instance used by this class.
 
             Source: https://docs.wxpython.org/wx.html.HtmlEasyPrinting.html
         """
 
-    def GetParentWindow(self) -> Window:
+    def GetParentWindow(self) -> 'Window':
         """ Gets the parent window for dialogs.
 
             Source: https://docs.wxpython.org/wx.html.HtmlEasyPrinting.html
         """
 
-    def GetPrintData(self) -> PrintData:
+    def GetPrintData(self) -> 'PrintData':
         """ Returns pointer to   wx.PrintData  instance used by this class.
 
             Source: https://docs.wxpython.org/wx.html.HtmlEasyPrinting.html
         """
 
     def PageSetup(self) -> None:
         """ Display page setup dialog and allows the user to modify settings.
@@ -862,17 +862,17 @@
     def SetStandardFonts(self, size=-1, normal_face="", fixed_face="") -> None:
         """ Sets default font sizes and/or default font size.
 
             Source: https://docs.wxpython.org/wx.html.HtmlEasyPrinting.html
         """
 
     Name: str  # See GetName and SetName
-    PageSetupData: PageSetupDialogData  # See GetPageSetupData
+    PageSetupData: 'PageSetupDialogData'  # See GetPageSetupData
     ParentWindow: 'Window'  # See GetParentWindow and SetParentWindow
-    PrintData: PrintData  # See GetPrintData
+    PrintData: '_PrintData'  # See GetPrintData
 
 
 
 PAGE_ODD: int
 
 PAGE_EVEN: int
 
@@ -929,41 +929,41 @@
 
     def FindPageByName(self, page: str) -> str:
         """ Returns pageâs URL based on its (file)name.
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpData.html
         """
 
-    def GetBookRecArray(self) -> HtmlBookRecArray:
+    def GetBookRecArray(self) -> 'html.HtmlBookRecArray':
         """ Returns array with help books info.
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpData.html
         """
 
-    def GetContentsArray(self) -> HtmlHelpDataItems:
+    def GetContentsArray(self) -> 'html.HtmlHelpDataItems':
         """ Returns reference to array with contents entries.
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpData.html
         """
 
-    def GetIndexArray(self) -> HtmlHelpDataItems:
+    def GetIndexArray(self) -> 'html.HtmlHelpDataItems':
         """ Returns reference to array with index entries.
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpData.html
         """
 
     def SetTempDir(self, path: str) -> None:
         """ Sets the temporary directory where binary cached versions of MS HTML Workshop files will be stored.
 
             Source: https://docs.wxpython.org/wx.html.HtmlHelpData.html
         """
 
-    BookRecArray: HtmlBookRecArray  # See GetBookRecArray
-    ContentsArray: HtmlHelpDataItems  # See GetContentsArray
-    IndexArray: HtmlHelpDataItems  # See GetIndexArray
+    BookRecArray: 'html.HtmlBookRecArray'  # See GetBookRecArray
+    ContentsArray: 'html.HtmlHelpDataItems'  # See GetContentsArray
+    IndexArray: 'html.HtmlHelpDataItems'  # See GetIndexArray
 
 
 
 class HtmlLinkInfo(Object):
     """ This class stores all necessary information about hypertext links (as
 represented by <A> tag in HTML documents).
 
@@ -971,15 +971,15 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.html.HtmlLinkInfo.html
         """
 
-    def GetEvent(self) -> MouseEvent:
+    def GetEvent(self) -> 'MouseEvent':
         """ Return pointer to event that generated OnLinkClicked() event.
 
             Source: https://docs.wxpython.org/wx.html.HtmlLinkInfo.html
         """
 
     def GetHref(self) -> str:
         """ Return HREF  value of the <A> tag.
@@ -995,15 +995,15 @@
 
     def GetTarget(self) -> str:
         """ Return TARGET  value of the <A> tag (this value is used to specify in which frame should be the page pointed by GetHref   Href opened).
 
             Source: https://docs.wxpython.org/wx.html.HtmlLinkInfo.html
         """
 
-    Event: MouseEvent  # See GetEvent
+    Event: 'MouseEvent'  # See GetEvent
     Href: str  # See GetHref
     HtmlCell: 'html.HtmlCell'  # See GetHtmlCell
     Target: str  # See GetTarget
 
 
 
 class HtmlTagHandler(Object):
@@ -1137,22 +1137,22 @@
     def AppendToPage(self, source: str) -> bool:
         """ Appends HTML fragment to currently displayed text and refreshes the window.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindow.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindow.html
         """
 
     @staticmethod
-    def GetDefaultHTMLCursor(type: HTMLCursor) -> Cursor:
+    def GetDefaultHTMLCursor(type: HTMLCursor) -> 'Cursor':
         """ Retrieves the default cursor for a given HTMLCursor type.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindow.html
         """
 
     def GetInternalRepresentation(self) -> 'html.HtmlContainerCell':
         """ Returns pointer to the top-level container.
@@ -1180,15 +1180,15 @@
 
     def GetParser(self) -> 'html.HtmlWinParser':
         """ Returns a pointer to the current parser.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindow.html
         """
 
-    def GetRelatedFrame(self) -> Frame:
+    def GetRelatedFrame(self) -> 'Frame':
         """ Returns the related frame.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindow.html
         """
 
     def HistoryBack(self) -> bool:
         """ Moves back to the previous page.
@@ -1354,15 +1354,15 @@
         """
 
     InternalRepresentation: 'html.HtmlContainerCell'  # See GetInternalRepresentation
     OpenedAnchor: str  # See GetOpenedAnchor
     OpenedPage: str  # See GetOpenedPage
     OpenedPageTitle: str  # See GetOpenedPageTitle
     Parser: 'html.HtmlWinParser'  # See GetParser
-    RelatedFrame: Frame  # See GetRelatedFrame and SetRelatedFrame
+    RelatedFrame: 'Frame'  # See GetRelatedFrame and SetRelatedFrame
 
 
 
 HW_SCROLLBAR_NEVER: int  # Never display scrollbars, not even when the page is larger than the window.
 
 HW_SCROLLBAR_AUTO: int  # Display scrollbars only if pageâs size exceeds windowâs size.
 
@@ -1395,33 +1395,33 @@
     def Create(self, parent, id=ID_ANY, pos=DefaultPosition, size=DefaultSize, style=0, name=HtmlListBoxNameStr) -> bool:
         """ Creates the control and optionally sets the initial number of items in it (it may also be set or changed later with wx.VListBox.SetItemCount ).
 
             Source: https://docs.wxpython.org/wx.html.HtmlListBox.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlListBox.html
         """
 
-    def GetFileSystem(self) -> FileSystem:
+    def GetFileSystem(self) -> 'FileSystem':
         """ Returns the   wx.FileSystem  used by the HTML parser of this object.
 
             Source: https://docs.wxpython.org/wx.html.HtmlListBox.html
         """
 
-    def GetSelectedTextBgColour(self, colBg: Union[int, str, 'Colour']) -> Colour:
+    def GetSelectedTextBgColour(self, colBg: Union[int, str, 'Colour']) -> 'Colour':
         """ This virtual function may be overridden to change the appearance of the background of the selected cells in the same way as GetSelectedTextColour .
 
             Source: https://docs.wxpython.org/wx.html.HtmlListBox.html
         """
 
-    def GetSelectedTextColour(self, colFg: Union[int, str, 'Colour']) -> Colour:
+    def GetSelectedTextColour(self, colFg: Union[int, str, 'Colour']) -> 'Colour':
         """ This virtual function may be overridden to customize the appearance of the selected cells.
 
             Source: https://docs.wxpython.org/wx.html.HtmlListBox.html
         """
 
     def OnGetItem(self, n: int) -> str:
         """ This method must be implemented in the derived class and should return the body (i.e. without  html   nor   body   tags) of the HTML fragment for the given item.
@@ -1437,15 +1437,15 @@
 
     def OnLinkClicked(self, n, link) -> None:
         """ Called when the user clicks on hypertext link.
 
             Source: https://docs.wxpython.org/wx.html.HtmlListBox.html
         """
 
-    FileSystem: FileSystem  # See GetFileSystem
+    FileSystem: '_FileSystem'  # See GetFileSystem
 
 
 
 class HtmlModalHelp:
     """ This class uses HtmlHelpController to display help in a modal
 dialog.
 
@@ -1493,21 +1493,21 @@
 
     def DoneParser(self) -> None:
         """ This must be called after DoParsing .
 
             Source: https://docs.wxpython.org/wx.html.HtmlParser.html
         """
 
-    def GetFS(self) -> FileSystem:
+    def GetFS(self) -> 'FileSystem':
         """ Returns pointer to the file system.
 
             Source: https://docs.wxpython.org/wx.html.HtmlParser.html
         """
 
-    def GetProduct(self) -> Object:
+    def GetProduct(self) -> 'Object':
         """ Returns product of parsing.
 
             Source: https://docs.wxpython.org/wx.html.HtmlParser.html
         """
 
     def GetSource(self) -> str:
         """ Returns pointer to the source being parsed.
@@ -1517,21 +1517,21 @@
 
     def InitParser(self, source: str) -> None:
         """ Setups the parser for parsing the source  string.
 
             Source: https://docs.wxpython.org/wx.html.HtmlParser.html
         """
 
-    def OpenURL(self, type, url) -> FSFile:
+    def OpenURL(self, type, url) -> 'FSFile':
         """ Opens given URL and returns    wx.FSFile  object that can be used to read data from it.
 
             Source: https://docs.wxpython.org/wx.html.HtmlParser.html
         """
 
-    def Parse(self, source: str) -> Object:
+    def Parse(self, source: str) -> 'Object':
         """ Proceeds parsing of the document.
 
             Source: https://docs.wxpython.org/wx.html.HtmlParser.html
         """
 
     def PopTagHandler(self) -> None:
         """ Restores parserâs state before last call to PushTagHandler .
@@ -1554,15 +1554,15 @@
     def StopParsing(self) -> None:
         """ Call this function to interrupt parsing from a tag handler.
 
             Source: https://docs.wxpython.org/wx.html.HtmlParser.html
         """
 
     FS: 'FileSystem'  # See GetFS and SetFS
-    Product: Object  # See GetProduct
+    Product: 'Object'  # See GetProduct
     Source: str  # See GetSource
 
 
 
 class HtmlWinParser(HtmlParser):
     """ This class is derived from HtmlParser and its main goal is to parse
 HTML input so that it can be displayed in HtmlWindow.
@@ -1577,21 +1577,21 @@
 
     def CloseContainer(self) -> 'html.HtmlContainerCell':
         """ Closes the container, sets actual container to the parent one and returns pointer to it (see Cells and Containers).
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinParser.html
         """
 
-    def CreateCurrentFont(self) -> Font:
+    def CreateCurrentFont(self) -> 'Font':
         """ Creates font based on current setting (see SetFontSize , SetFontBold , SetFontItalic , SetFontFixed , wx.html.HtmlWinParser.SetFontUnderlined ) and returns pointer to it.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinParser.html
         """
 
-    def GetActualColor(self) -> Colour:
+    def GetActualColor(self) -> 'Colour':
         """ Returns actual text colour.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinParser.html
         """
 
     def GetAlign(self) -> int:
         """ Returns default horizontal alignment.
@@ -1613,15 +1613,15 @@
 
     def GetContainer(self) -> 'html.HtmlContainerCell':
         """ Returns pointer to the currently opened container (see Cells and Containers).
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinParser.html
         """
 
-    def GetDC(self) -> DC:
+    def GetDC(self) -> 'DC':
         """ Returns pointer to the DC used during parsing.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinParser.html
         """
 
     def GetFontBold(self) -> int:
         """ Returns True if actual font is bold, False otherwise.
@@ -1661,15 +1661,15 @@
 
     def GetLink(self) -> 'html.HtmlLinkInfo':
         """ Returns actual hypertext link.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinParser.html
         """
 
-    def GetLinkColor(self) -> Colour:
+    def GetLinkColor(self) -> 'Colour':
         """ Returns the colour of hypertext link text.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinParser.html
         """
 
     def GetWindowInterface(self) -> 'html.HtmlWindowInterface':
         """ Returns associated window (  wx.html.HtmlWindow).
@@ -1757,28 +1757,28 @@
 
     def SetLinkColor(self, clr: Union[int, str, 'Colour']) -> None:
         """ Sets colour of hypertext link.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinParser.html
         """
 
-    ActualColor: Union[int, str, 'Colour']  # See GetActualColor and SetActualColor
+    ActualColor: 'Colour'  # See GetActualColor and SetActualColor
     Align: int  # See GetAlign and SetAlign
     CharHeight: int  # See GetCharHeight
     CharWidth: int  # See GetCharWidth
     Container: 'html.HtmlContainerCell'  # See GetContainer and SetContainer
-    DC: DC  # See GetDC and SetDC
+    DC: '_DC'  # See GetDC and SetDC
     FontBold: int  # See GetFontBold and SetFontBold
     FontFace: str  # See GetFontFace and SetFontFace
     FontFixed: int  # See GetFontFixed and SetFontFixed
     FontItalic: int  # See GetFontItalic and SetFontItalic
     FontSize: int  # See GetFontSize and SetFontSize
     FontUnderlined: int  # See GetFontUnderlined and SetFontUnderlined
     Link: 'html.HtmlLinkInfo'  # See GetLink and SetLink
-    LinkColor: Union[int, str, 'Colour']  # See GetLinkColor and SetLinkColor
+    LinkColor: 'Colour'  # See GetLinkColor and SetLinkColor
     WindowInterface: 'html.HtmlWindowInterface'  # See GetWindowInterface
 
 
 
 class HtmlContainerCell(HtmlCell):
     """ The HtmlContainerCell class is an implementation of a cell that may
 contain more cells in it.
@@ -1805,15 +1805,15 @@
 
     def GetAlignVer(self) -> int:
         """ Returns containerâs vertical alignment.
 
             Source: https://docs.wxpython.org/wx.html.HtmlContainerCell.html
         """
 
-    def GetBackgroundColour(self) -> Colour:
+    def GetBackgroundColour(self) -> 'Colour':
         """ Returns the background colour of the container or  NullColour   if no background colour is set.
 
             Source: https://docs.wxpython.org/wx.html.HtmlContainerCell.html
         """
 
     def GetIndent(self, ind: int) -> int:
         """ Returns the indentation.
@@ -1879,15 +1879,15 @@
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.html.HtmlContainerCell.html
         """
 
     AlignHor: int  # See GetAlignHor and SetAlignHor
     AlignVer: int  # See GetAlignVer and SetAlignVer
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
 
 
 
 HTML_ALIGN_LEFT: int
 
 HTML_ALIGN_JUSTIFY: int
 
@@ -1940,15 +1940,15 @@
 
     def SetParser(self, parser: 'html.HtmlParser') -> None:
         """ Assigns parser  to this handler.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWinTagHandler.html
         """
 
-    Parser: 'html.HtmlParser'  # See GetParser and SetParser
+    Parser: 'html.HtmlWinParser'  # See GetParser and SetParser
 
 
 
 class HtmlColourCell(HtmlCell):
     """ This cell changes the colour of either the background or the
 foreground.
 
@@ -2038,15 +2038,15 @@
 
     def GetFromCharacterPos(self) -> 'Coord':
         """ wx.Coord
 
             Source: https://docs.wxpython.org/wx.html.HtmlSelection.html
         """
 
-    def GetFromPos(self) -> Point:
+    def GetFromPos(self) -> 'Point':
         """ Point
 
             Source: https://docs.wxpython.org/wx.html.HtmlSelection.html
         """
 
     def GetToCell(self) -> 'html.HtmlCell':
         """ wx.html.HtmlCell
@@ -2056,15 +2056,15 @@
 
     def GetToCharacterPos(self) -> 'Coord':
         """ wx.Coord
 
             Source: https://docs.wxpython.org/wx.html.HtmlSelection.html
         """
 
-    def GetToPos(self) -> Point:
+    def GetToPos(self) -> 'Point':
         """ Point
 
             Source: https://docs.wxpython.org/wx.html.HtmlSelection.html
         """
 
     def IsEmpty(self) -> bool:
         """ bool
@@ -2087,19 +2087,19 @@
     def SetToCharacterPos(self, pos: int) -> None:
         """ pos (int) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlSelection.html
         """
 
     FromCell: 'html.HtmlCell'  # See GetFromCell
-    FromCharacterPos: int  # See GetFromCharacterPos and SetFromCharacterPos
-    FromPos: Point  # See GetFromPos
+    FromCharacterPos: 'Coord'  # See GetFromCharacterPos and SetFromCharacterPos
+    FromPos: 'Point'  # See GetFromPos
     ToCell: 'html.HtmlCell'  # See GetToCell
-    ToCharacterPos: int  # See GetToCharacterPos and SetToCharacterPos
-    ToPos: Point  # See GetToPos
+    ToCharacterPos: 'Coord'  # See GetToCharacterPos and SetToCharacterPos
+    ToPos: 'Point'  # See GetToPos
 
 
 
 class HtmlRenderingInfo:
     """ This class contains information given to cells when drawing them.
 
         Source: https://docs.wxpython.org/wx.html.HtmlRenderingInfo.html
@@ -2154,33 +2154,33 @@
     """
     def __init__(self) -> None:
         """ Ctor.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindowInterface.html
         """
 
-    def GetHTMLBackgroundColour(self) -> Colour:
+    def GetHTMLBackgroundColour(self) -> 'Colour':
         """ Returns background colour to use by default.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindowInterface.html
         """
 
-    def GetHTMLCursor(self, type: HtmlWindowInterface.HTMLCursor) -> Cursor:
+    def GetHTMLCursor(self, type: HtmlWindowInterface.HTMLCursor) -> 'Cursor':
         """ Returns mouse cursor of given type.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindowInterface.html
         """
 
-    def GetHTMLWindow(self) -> Window:
+    def GetHTMLWindow(self) -> 'Window':
         """ Returns the window used for rendering (may be None).
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindowInterface.html
         """
 
-    def HTMLCoordsToWindow(self, cell, pos) -> Point:
+    def HTMLCoordsToWindow(self, cell, pos) -> 'Point':
         """ Converts coordinates pos  relative to given cell  to physical coordinates in the window.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindowInterface.html
         """
 
     def OnHTMLLinkClicked(self, link: 'html.HtmlLinkInfo') -> None:
         """ Called when a link is clicked.
@@ -2214,16 +2214,16 @@
 
     def SetHTMLWindowTitle(self, title: str) -> None:
         """ Called by the parser to set windowâs title to given text.
 
             Source: https://docs.wxpython.org/wx.html.HtmlWindowInterface.html
         """
 
-    HTMLBackgroundColour: Union[int, str, 'Colour']  # See GetHTMLBackgroundColour and SetHTMLBackgroundColour
-    HTMLWindow: Window  # See GetHTMLWindow
+    HTMLBackgroundColour: 'Colour'  # See GetHTMLBackgroundColour and SetHTMLBackgroundColour
+    HTMLWindow: 'Window'  # See GetHTMLWindow
 
 
 
 class HtmlTag:
     """ This class represents a single HTML tag.
 
         Source: https://docs.wxpython.org/wx.html.HtmlTag.html
@@ -2284,14 +2284,18 @@
         """
 
     AllParams: str  # See GetAllParams
     Name: str  # See GetName
 
 
 
+HtmlURLType: TypeAlias = int  # Enumeration
+
+HtmlOpeningStatus: TypeAlias = int  # Enumeration
+
 class HtmlBookRecord:
     """ Helper class for HtmlHelpData.
 
         Source: https://docs.wxpython.org/wx.html.HtmlBookRecord.html
     """
     def __init__(self, bookfile, basepath, title, start) -> None:
         """ bookfile (string) â
@@ -2416,27 +2420,27 @@
     """
     def __init__(self) -> None:
         """ 
 
             Source: https://docs.wxpython.org/wx.html.HtmlRenderingState.html
         """
 
-    def GetBgColour(self) -> Colour:
+    def GetBgColour(self) -> 'Colour':
         """ Colour
 
             Source: https://docs.wxpython.org/wx.html.HtmlRenderingState.html
         """
 
     def GetBgMode(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.html.HtmlRenderingState.html
         """
 
-    def GetFgColour(self) -> Colour:
+    def GetFgColour(self) -> 'Colour':
         """ Colour
 
             Source: https://docs.wxpython.org/wx.html.HtmlRenderingState.html
         """
 
     def GetSelectionState(self) -> 'html.HtmlSelectionState':
         """ wx.html.HtmlSelectionState
@@ -2464,33 +2468,33 @@
 
     def SetSelectionState(self, s: HtmlSelectionState) -> None:
         """ s (HtmlSelectionState) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlRenderingState.html
         """
 
-    BgColour: Union[int, str, 'Colour']  # See GetBgColour and SetBgColour
+    BgColour: 'Colour'  # See GetBgColour and SetBgColour
     BgMode: int  # See GetBgMode and SetBgMode
-    FgColour: Union[int, str, 'Colour']  # See GetFgColour and SetFgColour
-    SelectionState: HtmlSelectionState  # See GetSelectionState and SetSelectionState
+    FgColour: 'Colour'  # See GetFgColour and SetFgColour
+    SelectionState: 'html.HtmlSelectionState'  # See GetSelectionState and SetSelectionState
 
 
 
 class HtmlRenderingStyle:
     """ HtmlSelection is data holder with information about text selection.
 
         Source: https://docs.wxpython.org/wx.html.HtmlRenderingStyle.html
     """
-    def GetSelectedTextBgColour(self, clr: Union[int, str, 'Colour']) -> Colour:
+    def GetSelectedTextBgColour(self, clr: Union[int, str, 'Colour']) -> 'Colour':
         """ Returns the colour to use for the selected textâs background.
 
             Source: https://docs.wxpython.org/wx.html.HtmlRenderingStyle.html
         """
 
-    def GetSelectedTextColour(self, clr: Union[int, str, 'Colour']) -> Colour:
+    def GetSelectedTextColour(self, clr: Union[int, str, 'Colour']) -> 'Colour':
         """ Returns the colour to use for the selected text.
 
             Source: https://docs.wxpython.org/wx.html.HtmlRenderingStyle.html
         """
 
 
 
@@ -2504,13 +2508,23 @@
         """ word (string) â
 
             Source: https://docs.wxpython.org/wx.html.HtmlWordWithTabsCell.html
         """
 
 
 
+HtmlSelectionState: TypeAlias = int  # Enumeration
+
 HTML_SEL_OUT: int
 
 HTML_SEL_IN: int
 
 HTML_SEL_CHANGING: int
 
+HtmlBookRecArray: TypeAlias = list[Any]
+
+HtmlHelpDataItems: TypeAlias = list[Any]
+
+PromptMode: TypeAlias = int  # Enumeration
+
+HTMLCursor: TypeAlias = int  # Enumeration
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/html2/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/html2/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class WebView(Control):
     """ This control may be used to render web (HTML / CSS / javascript)
 documents.
 
         Source: https://docs.wxpython.org/wx.html2.WebView.html
     """
@@ -124,28 +124,28 @@
     def Find(self, text, flags=WEBVIEW_FIND_DEFAULT) -> int:
         """ Finds a phrase on the current page and if found, the control will scroll the phrase into view and select it.
 
             Source: https://docs.wxpython.org/wx.html2.WebView.html
         """
 
     @staticmethod
-    def GetBackendVersionInfo(backend: str=WebViewBackendDefault) -> VersionInfo:
+    def GetBackendVersionInfo(backend: str=WebViewBackendDefault) -> 'VersionInfo':
         """ Retrieve the version information about the backend implementation.
 
             Source: https://docs.wxpython.org/wx.html2.WebView.html
         """
 
     def GetBackwardHistory(self) -> Any:
         """ Returns a list of items in the back history.
 
             Source: https://docs.wxpython.org/wx.html2.WebView.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.html2.WebView.html
         """
 
     def GetCurrentTitle(self) -> str:
         """ Get the title of the current web page, or its URL/path if title is not available.
@@ -416,17 +416,17 @@
     ForwardHistory: Any  # See GetForwardHistory
     NativeBackend: None  # See GetNativeBackend
     PageSource: str  # See GetPageSource
     PageText: str  # See GetPageText
     SelectedSource: str  # See GetSelectedSource
     SelectedText: str  # See GetSelectedText
     UserAgent: str  # See GetUserAgent and SetUserAgent
-    Zoom: WebViewZoom  # See GetZoom and SetZoom
+    Zoom: 'html2.WebViewZoom'  # See GetZoom and SetZoom
     ZoomFactor: float  # See GetZoomFactor and SetZoomFactor
-    ZoomType: WebViewZoomType  # See GetZoomType and SetZoomType
+    ZoomType: 'html2.WebViewZoomType'  # See GetZoomType and SetZoomType
 
 
 
 EVT_WEBVIEW_NAVIGATING: int  # Process a  wxEVT_WEBVIEW_NAVIGATING   event, generated before trying to get a resource. This event may be vetoed to prevent navigating to this resource. Note that if the displayed HTML document has several frames, one such event will be generated per frame.
 
 EVT_WEBVIEW_NAVIGATED: int  # Process a  wxEVT_WEBVIEW_NAVIGATED   event generated after it was confirmed that a resource would be requested. This event may not be vetoed. Note that if the displayed HTML document has several frames, one such event will be generated per frame.
 
@@ -502,27 +502,27 @@
     """
     def Create(self, *args, **kw) -> 'html2.WebView':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.html2.WebViewFactory.html
         """
 
-    def GetVersionInfo(self) -> VersionInfo:
+    def GetVersionInfo(self) -> 'VersionInfo':
         """ Retrieve the version information about this backend implementation.
 
             Source: https://docs.wxpython.org/wx.html2.WebViewFactory.html
         """
 
     def IsAvailable(self) -> bool:
         """ Function to check if the backend is available at runtime.
 
             Source: https://docs.wxpython.org/wx.html2.WebViewFactory.html
         """
 
-    VersionInfo: VersionInfo  # See GetVersionInfo
+    VersionInfo: '_VersionInfo'  # See GetVersionInfo
 
 
 
 class WebViewHandler:
     """ The base class for handling custom schemes in WebView, for example
 to allow virtual file system support.
 
@@ -530,15 +530,15 @@
     """
     def __init__(self, scheme: str) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.html2.WebViewHandler.html
         """
 
-    def GetFile(self, uri: str) -> FSFile:
+    def GetFile(self, uri: str) -> 'FSFile':
         """ uri (string) â
 
             Source: https://docs.wxpython.org/wx.html2.WebViewHandler.html
         """
 
     def GetName(self) -> str:
         """ string
@@ -572,15 +572,15 @@
     """
     def __init__(self, scheme: str) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.html2.WebViewFSHandler.html
         """
 
-    def GetFile(self, uri: str) -> FSFile:
+    def GetFile(self, uri: str) -> 'FSFile':
         """ uri (string) â
 
             Source: https://docs.wxpython.org/wx.html2.WebViewFSHandler.html
         """
 
 
 
@@ -592,40 +592,48 @@
     """
     def __init__(self, scheme: str) -> None:
         """ Constructor.
 
             Source: https://docs.wxpython.org/wx.html2.WebViewArchiveHandler.html
         """
 
-    def GetFile(self, uri: str) -> FSFile:
+    def GetFile(self, uri: str) -> 'FSFile':
         """ uri (string) â
 
             Source: https://docs.wxpython.org/wx.html2.WebViewArchiveHandler.html
         """
 
 
 
+WebViewUserScriptInjectionTime: TypeAlias = int  # Enumeration
+
 WEBVIEW_INJECT_AT_DOCUMENT_END: int
 
+WebViewZoomType: TypeAlias = int  # Enumeration
+
 WEBVIEW_ZOOM_TYPE_LAYOUT: int
 
 WEBVIEW_ZOOM_TYPE_TEXT: int
 
+WebViewFindFlags: TypeAlias = int  # Enumeration
+
 WEBVIEW_FIND_WRAP: int
 
 WEBVIEW_FIND_ENTIRE_WORD: int
 
 WEBVIEW_FIND_MATCH_CASE: int
 
 WEBVIEW_FIND_HIGHLIGHT_RESULT: int
 
 WEBVIEW_FIND_BACKWARDS: int
 
 WEBVIEW_FIND_DEFAULT: int
 
+WebViewZoom: TypeAlias = int  # Enumeration
+
 WEBVIEW_ZOOM_TINY: int
 
 WEBVIEW_ZOOM_SMALL: int
 
 WEBVIEW_ZOOM_MEDIUM: int
 
 WEBVIEW_ZOOM_LARGE: int
@@ -648,18 +656,22 @@
 
 WEBVIEWIE_EMU_IE10_FORCE: int
 
 WEBVIEWIE_EMU_IE11: int
 
 WEBVIEWIE_EMU_IE11_FORCE: int
 
+WebViewReloadFlags: TypeAlias = int  # Enumeration
+
 WEBVIEW_RELOAD_DEFAULT: int
 
 WEBVIEW_RELOAD_NO_CACHE: int
 
+WebViewNavigationError: TypeAlias = int  # Enumeration
+
 WEBVIEW_NAV_ERR_CONNECTION: int
 
 WEBVIEW_NAV_ERR_CERTIFICATE: int
 
 WEBVIEW_NAV_ERR_AUTH: int
 
 WEBVIEW_NAV_ERR_SECURITY: int
@@ -668,13 +680,17 @@
 
 WEBVIEW_NAV_ERR_REQUEST: int
 
 WEBVIEW_NAV_ERR_USER_CANCELLED: int
 
 WEBVIEW_NAV_ERR_OTHER: int
 
+WebViewNavigationActionFlags: TypeAlias = int  # Enumeration
+
 WEBVIEW_NAV_ACTION_NONE: int
 
 WEBVIEW_NAV_ACTION_USER: int
 
 WEBVIEW_NAV_ACTION_OTHER: int
 
+WebViewIE_EmulationLevel: TypeAlias = int
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/buttonbar/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/buttonbar/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class RibbonButtonBarButtonBase:
     """ Initialize self.  See help(type(self)) for accurate signature.
 
         Source: https://docs.wxpython.org/wx.lib.agw.ribbon.buttonbar.RibbonButtonBarButtonBase.html
     """
     def __init__(self) -> None:
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/agw/ribbon/gallery/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/agw/ribbon/gallery/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class RibbonGalleryItem:
     """ Initialize self.  See help(type(self)) for accurate signature.
 
         Source: https://docs.wxpython.org/wx.lib.agw.ribbon.gallery.RibbonGalleryItem.html
     """
     def __init__(self) -> None:
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/analogclock/lib_setup/fontselect/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class FontSelect(GenButton):
     """ A generic button, and base class for the other generic buttons.
 
         Source: https://docs.wxpython.org/wx.lib.analogclock.lib_setup.fontselect.FontSelect.html
     """
     def __init__(*args, **kwargs) -> None:
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/buttons/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/buttons/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class __ThemedMixin:
     """ Uses the native renderer to draw the bezel, also handle mouse-overs.
 
         Source: https://docs.wxpython.org/wx.lib.buttons.__ThemedMixin.html
     """
     def DrawBezel(self, dc, x1, y1, x2, y2) -> None:
@@ -141,15 +141,15 @@
 
     def GetBackgroundBrush(self, dc: 'DC') -> None:
         """ Returns the current wx.Brush to be used to draw the button background.
 
             Source: https://docs.wxpython.org/wx.lib.buttons.GenButton.html
         """
 
-    def GetBezelWidth(self) -> integer:
+    def GetBezelWidth(self) -> int:
         """ Returns the width of the 3D effect, in pixels.
 
             Source: https://docs.wxpython.org/wx.lib.buttons.GenButton.html
         """
 
     def GetDefaultAttributes(self) -> None:
         """ Overridden base class virtual. By default we should use
@@ -248,15 +248,15 @@
 
     def SetBackgroundColour(self, colour: Union[int, str, 'Colour']) -> None:
         """ Sets the GenButton background colour.
 
             Source: https://docs.wxpython.org/wx.lib.buttons.GenButton.html
         """
 
-    def SetBezelWidth(self, width: integer) -> None:
+    def SetBezelWidth(self, width: int) -> None:
         """ Sets the width of the 3D effect.
 
             Source: https://docs.wxpython.org/wx.lib.buttons.GenButton.html
         """
 
     def SetDefault(self) -> None:
         """ This sets the GenButton to be the default item for
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/calendar/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/calendar/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class CalDraw:
     """ A class to draw a calendar.
 
         Source: https://docs.wxpython.org/wx.lib.calendar.CalDraw.html
     """
     def __init__(self, parent: 'Window') -> None:
@@ -225,15 +225,15 @@
 
     def DrawRectOrg(self, key, fgcolor='BLACK', width=0) -> None:
         """ Draw a rectangle.
 
             Source: https://docs.wxpython.org/wx.lib.calendar.Calendar.html
         """
 
-    def GetColor(self, name: SetColor) -> None:
+    def GetColor(self, color: str) -> None:
         """ Get a color.
 
             Source: https://docs.wxpython.org/wx.lib.calendar.Calendar.html
         """
 
     def GetDate(self) -> None:
         """ Get the set calendar date.
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/colourselect/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/colourselect/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class ColourSelect(GenBitmapButton):
     """ A subclass of wx.lib.buttons.GenBitmapButton that,
 when clicked, will display a colour selection dialog.
 
         Source: https://docs.wxpython.org/wx.lib.colourselect.ColourSelect.html
     """
@@ -15,15 +15,15 @@
 
     def GetColour(self) -> 'Colour':
         """ Returns the current colour set for the ColourSelect.
 
             Source: https://docs.wxpython.org/wx.lib.colourselect.ColourSelect.html
         """
 
-    def GetCustomColours(self) -> CustomColourData:
+    def GetCustomColours(self) -> 'lib.colourselect.CustomColourData':
         """ Returns the current set of custom colour values to be shown in the
 colour dialog, if supported.
 
             Source: https://docs.wxpython.org/wx.lib.colourselect.ColourSelect.html
         """
 
     def GetLabel(self) -> str:
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/dialogs/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/dialogs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class MultiMessageDialog(Dialog):
     """ A dialog like wx.MessageDialog, but with an optional 2nd message string
 that is shown in a scrolled window, and also allows passing in the icon to
 be shown instead of the stock error, question, etc. icons. The btnLabels
 can be used if youâd like to change the stock labels on the buttons, itâs
 a dictionary mapping stock IDs to label strings.
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/scrolledpanel/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/scrolledpanel/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class ScrolledPanel(ScrolledWindow):
     """ ScrolledPanel fills a âholeâ in the implementation of
 ScrolledWindow, providing automatic scrollbar and scrolling
 behavior and the tab traversal management that ScrolledWindow lacks.
 
         Source: https://docs.wxpython.org/wx.lib.scrolledpanel.ScrolledPanel.html
```

### Comparing `types_wxpython-0.6.1/wx-stubs/lib/wxpTag/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/lib/wxpTag/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class wxpTagHandler(Object):
     """ HtmlWinTagHandler()
 
         Source: https://docs.wxpython.org/wx.lib.wxpTag.wxpTagHandler.html
     """
     def __init__(self) -> None:
```

### Comparing `types_wxpython-0.6.1/wx-stubs/media/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/media/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class MediaCtrl(Control):
     """ MediaCtrl is a class for displaying various types of media, such as
 videos, audio files, natively through native codecs.
 
         Source: https://docs.wxpython.org/wx.media.MediaCtrl.html
     """
@@ -15,15 +15,15 @@
 
     def Create(self, parent, id=-1, fileName="", pos=DefaultPosition, size=DefaultSize, style=0, szBackend="", validator=DefaultValidator, name="mediaCtrl") -> bool:
         """ Creates this control.
 
             Source: https://docs.wxpython.org/wx.media.MediaCtrl.html
         """
 
-    def GetBestSize(self) -> Size:
+    def GetBestSize(self) -> 'Size':
         """ Obtains the best size relative to the original/natural size of the video, if there is any.
 
             Source: https://docs.wxpython.org/wx.media.MediaCtrl.html
         """
 
     def GetPlaybackRate(self) -> float:
         """ Obtains the playback rate, or speed of the media.
@@ -111,15 +111,15 @@
 
     def Tell(self) -> 'FileOffset':
         """ Obtains the current position in time within the media in milliseconds.
 
             Source: https://docs.wxpython.org/wx.media.MediaCtrl.html
         """
 
-    BestSize: Size  # See GetBestSize
+    BestSize: 'Size'  # See GetBestSize
     PlaybackRate: float  # See GetPlaybackRate and SetPlaybackRate
     State: 'media.MediaState'  # See GetState
     Volume: float  # See GetVolume and SetVolume
 
 
 
 MC_NO_AUTORESIZE: int  # By default, the control will automatically adjust its size to exactly fit the size of a loaded video as soon as a video is loaded. If this flag is given, the control will not change its size automatically and it must be done manually (if desired) using Layout. It is strongly recommended to use this flag and handle control resizing manually (note that this style is only available in wxWidgets 3.1.6, so it is only possible to do it when using this or later version). ^^
@@ -151,14 +151,18 @@
 
 EVT_MEDIA_STATECHANGED: int  # Sent when a media has switched its state (from any media state). Processes a  wxEVT_MEDIA_STATECHANGED   event type.
 
 EVT_MEDIA_PLAY: int  # Sent when a media has switched to the  MEDIASTATE_PLAYING   state. Processes a   wxEVT_MEDIA_PLAY   event type.
 
 EVT_MEDIA_PAUSE: int  # Sent when a media has switched to the  MEDIASTATE_PAUSED   state. Processes a   wxEVT_MEDIA_PAUSE   event type. ^^
 
+MediaState: TypeAlias = int  # Enumeration
+
+MediaCtrlPlayerControls: TypeAlias = int  # Enumeration
+
 MEDIACTRLPLAYERCONTROLS_NONE: int
 
 MEDIACTRLPLAYERCONTROLS_STEP: int
 
 MEDIACTRLPLAYERCONTROLS_VOLUME: int
 
 MEDIACTRLPLAYERCONTROLS_DEFAULT: int
```

### Comparing `types_wxpython-0.6.1/wx-stubs/propgrid/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/propgrid/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class PropertyGridEvent(CommandEvent):
     """ A property grid event holds information about events associated with
 PropertyGrid objects.
 
         Source: https://docs.wxpython.org/wx.propgrid.PropertyGridEvent.html
     """
@@ -39,27 +39,27 @@
 
     def GetPropertyName(self) -> str:
         """ Returns name of the associated property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridEvent.html
         """
 
-    def GetPropertyValue(self) -> PGVariant:
+    def GetPropertyValue(self) -> 'propgrid.PGVariant':
         """ Returns value of the associated property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridEvent.html
         """
 
-    def GetValidationFailureBehavior(self) -> 'byte':
+    def GetValidationFailureBehavior(self) -> 'propgrid.byte':
         """ Returns current validation failure flags.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridEvent.html
         """
 
-    def GetValue(self) -> PGVariant:
+    def GetValue(self) -> 'propgrid.PGVariant':
         """ Returns value of the associated property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridEvent.html
         """
 
     def SetCanVeto(self, canVeto: bool) -> None:
         """ Set if event can be vetoed.
@@ -97,17 +97,17 @@
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridEvent.html
         """
 
     Column: int  # See GetColumn
     MainParent: 'propgrid.PGProperty'  # See GetMainParent
     Property: 'propgrid.PGProperty'  # See GetProperty and SetProperty
     PropertyName: str  # See GetPropertyName
-    PropertyValue: PGVariant  # See GetPropertyValue
-    ValidationFailureBehavior: 'byte'  # See GetValidationFailureBehavior and SetValidationFailureBehavior
-    Value: PGVariant  # See GetValue
+    PropertyValue: 'propgrid.PGVariant'  # See GetPropertyValue
+    ValidationFailureBehavior: 'propgrid.byte'  # See GetValidationFailureBehavior and SetValidationFailureBehavior
+    Value: 'propgrid.PGVariant'  # See GetValue
 
 
 
 EVT_PG_SELECTED : int  # Respond to  wxEVT_PG_SELECTED   event, generated when a property selection has been changed, either by user action or by indirect program function. For instance, collapsing a parent property programmatically causes any selected child property to become unselected, and may therefore cause this event to be generated.
 
 EVT_PG_CHANGED: int  # Respond to  wxEVT_PG_CHANGED   event, generated when property value has been changed by the user.
 
@@ -164,47 +164,47 @@
 
     def Finalize(self, propGrid, pos) -> None:
         """ Call this in CreateControls() of your custom editor class after all buttons have been added.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGMultiButton.html
         """
 
-    def GetButton(self, i: int) -> Window:
+    def GetButton(self, i: int) -> 'Window':
         """ Returns pointer to one of the buttons.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGMultiButton.html
         """
 
     def GetButtonId(self, i: int) -> int:
         """ Returns Id of one of the buttons.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGMultiButton.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGMultiButton.html
         """
 
     def GetCount(self) -> int:
         """ Returns number of buttons.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGMultiButton.html
         """
 
-    def GetPrimarySize(self) -> Size:
+    def GetPrimarySize(self) -> 'Size':
         """ Returns size of primary editor control, as appropriately reduced by number of buttons present.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGMultiButton.html
         """
 
     Count: int  # See GetCount
-    PrimarySize: Size  # See GetPrimarySize
+    PrimarySize: 'Size'  # See GetPrimarySize
 
 
 
 class PGArrayEditorDialog(Dialog):
     """ index (int) â 
 
         Source: https://docs.wxpython.org/wx.propgrid.PGArrayEditorDialog.html
@@ -260,33 +260,33 @@
     def EnableCustomNewAction(self) -> None:
         """ 
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayEditorDialog.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayEditorDialog.html
         """
 
-    def GetDialogValue(self) -> PGVariant:
+    def GetDialogValue(self) -> 'propgrid.PGVariant':
         """ Return value modified by dialog.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayEditorDialog.html
         """
 
     def GetSelection(self) -> int:
         """ int
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayEditorDialog.html
         """
 
-    def GetTextCtrlValidator(self) -> Validator:
+    def GetTextCtrlValidator(self) -> 'Validator':
         """ Override to return   wx.Validator  to be used with the   wx.TextCtrl  in dialog.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayEditorDialog.html
         """
 
     def Init(self) -> None:
         """ 
@@ -314,17 +314,17 @@
 
     def SetNewButtonText(self, text: str) -> None:
         """ Sets tooltip text for button allowing the user to enter new string.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayEditorDialog.html
         """
 
-    DialogValue: PGVariant  # See GetDialogValue and SetDialogValue
+    DialogValue: 'propgrid.PGVariant'  # See GetDialogValue and SetDialogValue
     Selection: int  # See GetSelection
-    TextCtrlValidator: Validator  # See GetTextCtrlValidator
+    TextCtrlValidator: 'Validator'  # See GetTextCtrlValidator
 
 
 
 class PropertyGridPage(EvtHandler,PropertyGridInterface,PropertyGridPageState):
     """ Holder of property grid page information.
 
         Source: https://docs.wxpython.org/wx.propgrid.PropertyGridPage.html
@@ -337,15 +337,15 @@
 
     def Clear(self) -> None:
         """ Deletes all properties on page.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridPage.html
         """
 
-    def FitColumns(self) -> Size:
+    def FitColumns(self) -> 'Size':
         """ Reduces column sizes to minimum possible that contents are still visibly (naturally some margin space will be applied as well).
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridPage.html
         """
 
     def GetIndex(self) -> int:
         """ Returns page index in manager;.
@@ -446,39 +446,39 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCell.html
         """
 
-    def GetBgCol(self) -> Colour:
+    def GetBgCol(self) -> 'Colour':
         """ Colour
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCell.html
         """
 
-    def GetBitmap(self) -> BitmapBundle:
+    def GetBitmap(self) -> 'BitmapBundle':
         """ BitmapBundle
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCell.html
         """
 
     def GetData(self) -> 'propgrid.PGCellData':
         """ wx.propgrid.PGCellData
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCell.html
         """
 
-    def GetFgCol(self) -> Colour:
+    def GetFgCol(self) -> 'Colour':
         """ Colour
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCell.html
         """
 
-    def GetFont(self) -> Font:
+    def GetFont(self) -> 'Font':
         """ Returns font of the cell.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCell.html
         """
 
     def GetText(self) -> str:
         """ string
@@ -530,19 +530,19 @@
 
     def SetText(self, text: str) -> None:
         """ text (string) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCell.html
         """
 
-    BgCol: Union[int, str, 'Colour']  # See GetBgCol and SetBgCol
+    BgCol: 'Colour'  # See GetBgCol and SetBgCol
     Bitmap: 'BitmapBundle'  # See GetBitmap and SetBitmap
     Data: 'propgrid.PGCellData'  # See GetData
-    FgCol: Union[int, str, 'Colour']  # See GetFgCol and SetFgCol
-    Font: 'Font'  # See GetFont and SetFont
+    FgCol: 'Colour'  # See GetFgCol and SetFgCol
+    Font: '_Font'  # See GetFont and SetFont
     Text: str  # See GetText and SetText
 
 
 
 class PGEditor(Object):
     """ Base class for custom PropertyGrid editors.
 
@@ -657,15 +657,15 @@
 
     def DoShowDialog(self, propGrid, property) -> bool:
         """ propGrid (wx.propgrid.PropertyGrid) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGEditorDialogAdapter.html
         """
 
-    def GetValue(self) -> PGVariant:
+    def GetValue(self) -> 'propgrid.PGVariant':
         """ This method is typically only used if deriving class from existing adapter with value conversion purposes.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGEditorDialogAdapter.html
         """
 
     def SetValue(self, value: PGVariant) -> None:
         """ value (PGVariant) â
@@ -675,15 +675,15 @@
 
     def ShowDialog(self, propGrid, property) -> bool:
         """ propGrid (wx.propgrid.PropertyGrid) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGEditorDialogAdapter.html
         """
 
-    Value: PGVariant  # See GetValue and SetValue
+    Value: 'propgrid.PGVariant'  # See GetValue and SetValue
     m_clientData: Any  # A public C++ attribute of type ````.
 
 
 
 class PGProperty(Object):
     """ PGProperty is base class for all PropertyGrid properties and as
 such it is not intended to be instantiated directly.
@@ -728,15 +728,15 @@
 
     def ChangeFlag(self, flag, set) -> None:
         """ Sets or clears given property flag.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def ChildChanged(self, thisValue, childIndex, childValue) -> PGVariant:
+    def ChildChanged(self, thisValue, childIndex, childValue) -> 'propgrid.PGVariant':
         """ Called after value of a child property has been altered.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def DeleteChildren(self) -> None:
         """ Deletes children of the property.
@@ -746,33 +746,33 @@
 
     def DeleteChoice(self, index: int) -> None:
         """ Removes entry from propertyâs   wx.propgrid.PGChoices  and editor control (if it is active).
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def DoGetAttribute(self, name: str) -> PGVariant:
+    def DoGetAttribute(self, name: str) -> 'propgrid.PGVariant':
         """ Returns value of an attribute.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def DoGetEditorClass(self) -> 'propgrid.PGEditor':
         """ Returns pointer to an instance of used editor.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def DoGetValidator(self) -> Validator:
+    def DoGetValidator(self) -> 'Validator':
         """ Returns pointer to the   wx.Validator  that should be used with the editor of this property (None for no validator).
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def DoGetValue(self) -> PGVariant:
+    def DoGetValue(self) -> 'propgrid.PGVariant':
         """ Override this to return something else than m_value as the value.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def DoSetAttribute(self, name, value) -> bool:
         """ Reimplement this member function to add special handling for attributes of this property.
@@ -794,15 +794,15 @@
 
     def GenerateComposedValue(self) -> str:
         """ Composes text from values of child properties.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def GetAttribute(self, *args, **kw) -> PGVariant:
+    def GetAttribute(self, *args, **kw) -> 'propgrid.PGVariant':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def GetAttributeAsDouble(self, name, defVal) -> float:
         """ Returns named attribute, as double, if found.
@@ -818,15 +818,15 @@
 
     def GetAttributes(self) -> Any:
         """ Returns map-like storage of propertyâs attributes.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def GetAttributesAsList(self) -> PGVariant:
+    def GetAttributesAsList(self) -> 'propgrid.PGVariant':
         """ Returns attributes as list Variant     .
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def GetBaseName(self) -> str:
         """ Returns propertyâs base name (i.e.
@@ -866,15 +866,15 @@
 
     def GetChoices(self) -> 'propgrid.PGChoices':
         """ Returns read-only reference to propertyâs list of choices.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def GetClientData(self) -> ClientData:
+    def GetClientData(self) -> 'ClientData':
         """ Gets managed client object of a property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def GetClientObject(self, n) -> Any:
         """ Alias for GetClientData
@@ -890,15 +890,15 @@
 
     def GetCommonValue(self) -> int:
         """ Returns common value selected for this property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def GetDefaultValue(self) -> PGVariant:
+    def GetDefaultValue(self) -> 'propgrid.PGVariant':
         """ Returns propertyâs default value.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def GetDepth(self) -> int:
         """ int
@@ -1022,33 +1022,33 @@
 
     def GetPropertyByName(self, name: str) -> 'propgrid.PGProperty':
         """ Returns (direct) child property with given name (or None if not found).
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def GetValidator(self) -> Validator:
+    def GetValidator(self) -> 'Validator':
         """ Gets assignable version of propertyâs validator.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def GetValue(self) -> PGVariant:
+    def GetValue(self) -> 'propgrid.PGVariant':
         """ Returns propertyâs value.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def GetValueAsString(self, argFlags: int=0) -> str:
         """ Returns text representation of propertyâs value.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def GetValueImage(self) -> Bitmap:
+    def GetValueImage(self) -> 'Bitmap':
         """ Returns bitmap that appears next to value text.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def GetValueType(self) -> str:
         """ Returns value type used by this property.
@@ -1184,15 +1184,15 @@
 
     def OnEvent(self, propgrid, wnd_primary, event) -> None:
         """ Events received by editor widgets are processed here.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
-    def OnMeasureImage(self, item: int=-1) -> Size:
+    def OnMeasureImage(self, item: int=-1) -> 'Size':
         """ Returns size of the custom painted image in front of property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGProperty.html
         """
 
     def OnSetValue(self) -> None:
         """ This virtual function is called after m_value has been set.
@@ -1511,15 +1511,15 @@
     def EnsureVisible(self, id: 'propgrid.PGPropArgCls') -> bool:
         """ Selects page, scrolls and/or expands items to ensure that the given item is visible.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridManager.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridManager.html
         """
 
     def GetColumnCount(self, page: int=-1) -> int:
         """ Returns number of columns on given page.
@@ -1595,15 +1595,15 @@
 
     def GetSelection(self) -> 'propgrid.PGProperty':
         """ Shortcut for GetGrid . GetSelection .
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridManager.html
         """
 
-    def GetToolBar(self) -> ToolBar:
+    def GetToolBar(self) -> 'ToolBar':
         """ Returns a pointer to the toolbar currently associated with the   wx.propgrid.PropertyGridManager  (if any).
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridManager.html
         """
 
     def GetVIterator(self, flags: int) -> 'propgrid.PGVIterator':
         """ Similar to GetIterator , but instead returns   wx.propgrid.PGVIterator  instance, which can be useful for forward-iterating through arbitrary property containers.
@@ -1711,15 +1711,15 @@
     CurrentPage: 'propgrid.PropertyGridPage'  # See GetCurrentPage
     DescBoxHeight: int  # See GetDescBoxHeight and SetDescBoxHeight
     Grid: 'propgrid.PropertyGrid'  # See GetGrid
     PageCount: int  # See GetPageCount
     SelectedPage: int  # See GetSelectedPage
     SelectedProperty: 'propgrid.PGProperty'  # See GetSelectedProperty
     Selection: 'propgrid.PGProperty'  # See GetSelection
-    ToolBar: ToolBar  # See GetToolBar
+    ToolBar: '_ToolBar'  # See GetToolBar
 
 
 
 class PropertyGrid(Scrolled,PropertyGridInterface):
     """ PropertyGrid is a specialized grid for editing properties - in other
 words name = value pairs.
 
@@ -1897,76 +1897,76 @@
 
     def EnsureVisible(self, id: 'propgrid.PGPropArgCls') -> bool:
         """ Scrolls and/or expands items to ensure that the given item is visible.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def FitColumns(self) -> Size:
+    def FitColumns(self) -> 'Size':
         """ Reduces column sizes to minimum possible, while still retaining fully visible grid contents (labels, images).
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetCaptionBackgroundColour(self) -> Colour:
+    def GetCaptionBackgroundColour(self) -> 'Colour':
         """ Returns current category caption background colour.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetCaptionFont(self) -> Font:
+    def GetCaptionFont(self) -> 'Font':
         """ Returns current category caption font.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetCaptionForegroundColour(self) -> Colour:
+    def GetCaptionForegroundColour(self) -> 'Colour':
         """ Returns current category caption text colour.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetCellBackgroundColour(self) -> Colour:
+    def GetCellBackgroundColour(self) -> 'Colour':
         """ Returns current cell background colour.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetCellDisabledTextColour(self) -> Colour:
+    def GetCellDisabledTextColour(self) -> 'Colour':
         """ Returns current cell text colour when disabled.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetCellTextColour(self) -> Colour:
+    def GetCellTextColour(self) -> 'Colour':
         """ Returns current cell text colour.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     def GetColumnCount(self) -> int:
         """ Returns number of columns currently on grid.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetEditorTextCtrl(self) -> TextCtrl:
+    def GetEditorTextCtrl(self) -> 'TextCtrl':
         """ Returns   wx.TextCtrl  active in currently selected property, if any.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetEmptySpaceColour(self) -> Colour:
+    def GetEmptySpaceColour(self) -> 'Colour':
         """ Returns colour of empty space below properties.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     def GetFontHeight(self) -> int:
         """ Returns height of highest characters of used font.
@@ -1976,57 +1976,57 @@
 
     def GetGrid(self) -> 'propgrid.PropertyGrid':
         """ Returns pointer to itself.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetImageRect(self, property, item) -> Rect:
+    def GetImageRect(self, property, item) -> 'Rect':
         """ Returns rectangle of custom paint image.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetImageSize(self, property=None, item=-1) -> Size:
+    def GetImageSize(self, property=None, item=-1) -> 'Size':
         """ Returns size of the custom paint image in front of property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetLabelEditor(self) -> TextCtrl:
+    def GetLabelEditor(self) -> 'TextCtrl':
         """ Returns currently active label editor, None if none.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     def GetLastItem(self, flags: int=PG_ITERATE_DEFAULT) -> 'propgrid.PGProperty':
         """ Returns last item which could be iterated using given flags.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetLineColour(self) -> Colour:
+    def GetLineColour(self) -> 'Colour':
         """ Returns colour of lines between cells.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetMarginColour(self) -> Colour:
+    def GetMarginColour(self) -> 'Colour':
         """ Returns background colour of margin.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     def GetMarginWidth(self) -> int:
         """ Returns margin width.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetPanel(self) -> Window:
+    def GetPanel(self) -> 'Window':
         """ Returns   wx.Window  that the properties are painted on, and which should be used as the parent for editor controls.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     def GetRoot(self) -> 'propgrid.PGProperty':
         """ Returns âroot propertyâ.
@@ -2078,21 +2078,21 @@
 
     def GetSelection(self) -> 'propgrid.PGProperty':
         """ Returns currently selected property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetSelectionBackgroundColour(self) -> Colour:
+    def GetSelectionBackgroundColour(self) -> 'Colour':
         """ Returns current selection background colour.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetSelectionForegroundColour(self) -> Colour:
+    def GetSelectionForegroundColour(self) -> 'Colour':
         """ Returns current selection text colour.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     def GetSizeAvailableForScrollTarget(self, size: Union[tuple[int, int], 'Size']) -> 'Size':
         """ Function which must be overridden to implement the size available for the scroll target for the given size of the main window.
@@ -2102,15 +2102,15 @@
 
     def GetSplitterPosition(self, splitterIndex: int=0) -> int:
         """ Returns current splitter x position.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetStatusBar(self) -> StatusBar:
+    def GetStatusBar(self) -> 'StatusBar':
         """ Return   wx.StatusBar  that is used by this   wx.propgrid.PropertyGrid.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     def GetTargetRect(self) -> 'Rect':
         """ wx.Rect
@@ -2120,15 +2120,15 @@
 
     def GetTargetWindow(self) -> 'Window':
         """ wx.Window
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    def GetUncommittedPropertyValue(self) -> PGVariant:
+    def GetUncommittedPropertyValue(self) -> 'propgrid.PGVariant':
         """ Returns most up-to-date value of selected property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
     def GetUnspecifiedValueAppearance(self) -> 'propgrid.PGCell':
         """ Returns current appearance of unspecified value cells.
@@ -2463,45 +2463,45 @@
 
     def WasValueChangedInEvent(self) -> bool:
         """ You can use this member function, for instance, to detect in wx.propgrid.PGProperty.OnEvent   if wx.propgrid.PGProperty.SetValueInEvent   was already called in wx.propgrid.PGEditor.OnEvent .
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGrid.html
         """
 
-    CaptionBackgroundColour: Union[int, str, 'Colour']  # See GetCaptionBackgroundColour and SetCaptionBackgroundColour
-    CaptionFont: Font  # See GetCaptionFont
-    CaptionForegroundColour: Colour  # See GetCaptionForegroundColour
-    CellBackgroundColour: Union[int, str, 'Colour']  # See GetCellBackgroundColour and SetCellBackgroundColour
-    CellDisabledTextColour: Union[int, str, 'Colour']  # See GetCellDisabledTextColour and SetCellDisabledTextColour
-    CellTextColour: Union[int, str, 'Colour']  # See GetCellTextColour and SetCellTextColour
+    CaptionBackgroundColour: 'Colour'  # See GetCaptionBackgroundColour and SetCaptionBackgroundColour
+    CaptionFont: 'Font'  # See GetCaptionFont
+    CaptionForegroundColour: 'Colour'  # See GetCaptionForegroundColour
+    CellBackgroundColour: 'Colour'  # See GetCellBackgroundColour and SetCellBackgroundColour
+    CellDisabledTextColour: 'Colour'  # See GetCellDisabledTextColour and SetCellDisabledTextColour
+    CellTextColour: 'Colour'  # See GetCellTextColour and SetCellTextColour
     ColumnCount: int  # See GetColumnCount and SetColumnCount
-    EditorTextCtrl: TextCtrl  # See GetEditorTextCtrl
-    EmptySpaceColour: Union[int, str, 'Colour']  # See GetEmptySpaceColour and SetEmptySpaceColour
+    EditorTextCtrl: 'TextCtrl'  # See GetEditorTextCtrl
+    EmptySpaceColour: 'Colour'  # See GetEmptySpaceColour and SetEmptySpaceColour
     FontHeight: int  # See GetFontHeight
     Grid: 'propgrid.PropertyGrid'  # See GetGrid
-    ImageSize: Size  # See GetImageSize
-    LabelEditor: TextCtrl  # See GetLabelEditor
+    ImageSize: 'Size'  # See GetImageSize
+    LabelEditor: 'TextCtrl'  # See GetLabelEditor
     LastItem: 'propgrid.PGProperty'  # See GetLastItem
-    LineColour: Union[int, str, 'Colour']  # See GetLineColour and SetLineColour
-    MarginColour: Union[int, str, 'Colour']  # See GetMarginColour and SetMarginColour
+    LineColour: 'Colour'  # See GetLineColour and SetLineColour
+    MarginColour: 'Colour'  # See GetMarginColour and SetMarginColour
     MarginWidth: int  # See GetMarginWidth
-    Panel: Window  # See GetPanel
+    Panel: 'Window'  # See GetPanel
     Root: 'propgrid.PGProperty'  # See GetRoot
     RowHeight: int  # See GetRowHeight
     ScaleX: float  # See GetScaleX
     ScaleY: float  # See GetScaleY
     SelectedProperty: 'propgrid.PGProperty'  # See GetSelectedProperty
-    Selection: ArrayPGProperty  # See GetSelection and SetSelection
-    SelectionBackgroundColour: Union[int, str, 'Colour']  # See GetSelectionBackgroundColour and SetSelectionBackgroundColour
-    SelectionForegroundColour: Colour  # See GetSelectionForegroundColour
+    Selection: 'propgrid.PGProperty'  # See GetSelection and SetSelection
+    SelectionBackgroundColour: 'Colour'  # See GetSelectionBackgroundColour and SetSelectionBackgroundColour
+    SelectionForegroundColour: 'Colour'  # See GetSelectionForegroundColour
     SplitterPosition: int  # See GetSplitterPosition and SetSplitterPosition
-    StatusBar: StatusBar  # See GetStatusBar
+    StatusBar: '_StatusBar'  # See GetStatusBar
     TargetRect: 'Rect'  # See GetTargetRect and SetTargetRect
     TargetWindow: 'Window'  # See GetTargetWindow and SetTargetWindow
-    UncommittedPropertyValue: PGVariant  # See GetUncommittedPropertyValue
+    UncommittedPropertyValue: 'propgrid.PGVariant'  # See GetUncommittedPropertyValue
     UnspecifiedValueAppearance: 'propgrid.PGCell'  # See GetUnspecifiedValueAppearance and SetUnspecifiedValueAppearance
     UnspecifiedValueText: str  # See GetUnspecifiedValueText
     VerticalSpacing: int  # See GetVerticalSpacing and SetVerticalSpacing
 
 
 
 SHOW_SB_ALWAYS: int
@@ -2517,33 +2517,33 @@
     """
     def __init__(self, primary, secondary=None) -> None:
         """ primary (wx.Window) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGWindowList.html
         """
 
-    def GetPrimary(self) -> Window:
+    def GetPrimary(self) -> 'Window':
         """ Gets window of primary editor.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGWindowList.html
         """
 
-    def GetSecondary(self) -> Window:
+    def GetSecondary(self) -> 'Window':
         """ Gets window of secondary editor.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGWindowList.html
         """
 
     def SetSecondary(self, secondary: 'Window') -> None:
         """ secondary (wx.Window) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGWindowList.html
         """
 
-    Primary: Window  # See GetPrimary
+    Primary: 'Window'  # See GetPrimary
     Secondary: 'Window'  # See GetSecondary and SetSecondary
 
 
 
 class PGArrayStringEditorDialog(PGArrayEditorDialog):
     """ index (int) â 
 
@@ -2588,21 +2588,21 @@
     def ArraySwap(self, first, second) -> None:
         """ first (int) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayStringEditorDialog.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayStringEditorDialog.html
         """
 
-    def GetDialogValue(self) -> PGVariant:
+    def GetDialogValue(self) -> 'propgrid.PGVariant':
         """ Return value modified by dialog.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayStringEditorDialog.html
         """
 
     def Init(self) -> None:
         """ 
@@ -2624,15 +2624,15 @@
 
     def SetDialogValue(self, value: PGVariant) -> None:
         """ Set value modified by dialog.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGArrayStringEditorDialog.html
         """
 
-    DialogValue: PGVariant  # See GetDialogValue and SetDialogValue
+    DialogValue: 'propgrid.PGVariant'  # See GetDialogValue and SetDialogValue
 
 
 
 class PropertyGridInterface:
     """ Most of the shared property manipulation interface shared by
 PropertyGrid, PropertyGridPage, and PropertyGridManager is
 defined in this class.
@@ -2793,27 +2793,27 @@
 
     def GetProperty(self, name: str) -> 'propgrid.PGProperty':
         """ Returns pointer to a property with given name (case-sensitive).
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyAttribute(self, id, attrName) -> PGVariant:
+    def GetPropertyAttribute(self, id, attrName) -> 'propgrid.PGVariant':
         """ Returns value of given attribute.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
     def GetPropertyAttributes(self, id: 'propgrid.PGPropArgCls') -> 'propgrid.PGAttributeStorage':
         """ Returns map-like storage of propertyâs attributes.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyBackgroundColour(self, id: 'propgrid.PGPropArgCls') -> Colour:
+    def GetPropertyBackgroundColour(self, id: 'propgrid.PGPropArgCls') -> 'Colour':
         """ Returns background colour of first cell of a property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
     def GetPropertyByLabel(self, label: str) -> 'propgrid.PGProperty':
         """ Returns first property which label matches given string.
@@ -2853,15 +2853,15 @@
 
     def GetPropertyHelpString(self, id: 'propgrid.PGPropArgCls') -> str:
         """ Returns help string associated with a property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyImage(self, id: 'propgrid.PGPropArgCls') -> Bitmap:
+    def GetPropertyImage(self, id: 'propgrid.PGPropArgCls') -> 'Bitmap':
         """ Returns propertyâs custom value image (None of none).
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
     def GetPropertyLabel(self, id: 'propgrid.PGPropArgCls') -> str:
         """ Returns label of a property.
@@ -2877,27 +2877,27 @@
 
     def GetPropertyParent(self, id: 'propgrid.PGPropArgCls') -> 'propgrid.PGProperty':
         """ Returns parent item of a property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyTextColour(self, id: 'propgrid.PGPropArgCls') -> Colour:
+    def GetPropertyTextColour(self, id: 'propgrid.PGPropArgCls') -> 'Colour':
         """ Returns text colour of first cell of a property.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyValidator(self, id: 'propgrid.PGPropArgCls') -> Validator:
+    def GetPropertyValidator(self, id: 'propgrid.PGPropArgCls') -> 'Validator':
         """ Returns validator of a property as a reference, which you can pass to any number of SetPropertyValidator.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyValue(self, id: 'propgrid.PGPropArgCls') -> PGVariant:
+    def GetPropertyValue(self, id: 'propgrid.PGPropArgCls') -> 'propgrid.PGVariant':
         """ Returns propertyâs value as Variant     .
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
     def GetPropertyValueAsArrayInt(self, id: 'propgrid.PGPropArgCls') -> list[int]:
         """ Returnâs propertyâs value as ArrayInt.
@@ -2913,15 +2913,15 @@
 
     def GetPropertyValueAsBool(self, id: 'propgrid.PGPropArgCls') -> bool:
         """ Returns propertyâs value as bool.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyValueAsDateTime(self, id: 'propgrid.PGPropArgCls') -> DateTime:
+    def GetPropertyValueAsDateTime(self, id: 'propgrid.PGPropArgCls') -> 'DateTime':
         """ Returnâs propertyâs value as   wx.DateTime.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
     def GetPropertyValueAsDouble(self, id: 'propgrid.PGPropArgCls') -> float:
         """ Returns propertyâs value as double-precision floating point number.
@@ -2937,15 +2937,15 @@
 
     def GetPropertyValueAsLong(self, id: 'propgrid.PGPropArgCls') -> int:
         """ Returns propertyâs value as integer.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyValueAsLongLong(self, id: 'propgrid.PGPropArgCls') -> LongLong_t:
+    def GetPropertyValueAsLongLong(self, id: 'propgrid.PGPropArgCls') -> 'LongLong_t':
         """ Returns propertyâs value as native signed 64-bit integer.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
     def GetPropertyValueAsString(self, id: 'propgrid.PGPropArgCls') -> str:
         """ Returns propertyâs value as String     .
@@ -2955,15 +2955,15 @@
 
     def GetPropertyValueAsULong(self, id: 'propgrid.PGPropArgCls') -> int:
         """ Returns propertyâs value as  integer.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetPropertyValueAsULongLong(self, id: 'propgrid.PGPropArgCls') -> ULongLong_t:
+    def GetPropertyValueAsULongLong(self, id: 'propgrid.PGPropArgCls') -> int:
         """ Returns propertyâs value as native  64-bit integer.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
     def GetPropertyValues(self, dict_=None, as_strings=False, inc_attributes=False, flags=PG_ITERATE_PROPERTIES) -> None:
         """ Returns all property values in the grid.
@@ -2981,15 +2981,15 @@
 
     def GetPyVIterator(self, flags=PG_ITERATE_DEFAULT) -> None:
         """ Similar to GetVIterator      but returns a pythonic iterator.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
-    def GetSelectedProperties(self) -> ArrayPGProperty:
+    def GetSelectedProperties(self) -> 'propgrid.ArrayPGProperty':
         """ Returns list of currently selected properties.
 
             Source: https://docs.wxpython.org/wx.propgrid.PropertyGridInterface.html
         """
 
     def GetSelection(self) -> 'propgrid.PGProperty':
         """ Returns currently selected property.
@@ -3500,15 +3500,15 @@
 
     def DoSetAttribute(self, name, value) -> bool:
         """ Reimplement this member function to add special handling for attributes of this property.
 
             Source: https://docs.wxpython.org/wx.propgrid.SystemColourProperty.html
         """
 
-    def GetColour(self, index: int) -> Colour:
+    def GetColour(self, index: int) -> 'Colour':
         """ Default is to use SystemSettings.GetColour(index).
 
             Source: https://docs.wxpython.org/wx.propgrid.SystemColourProperty.html
         """
 
     def GetCustomColourIndex(self) -> int:
         """ Returns index of entry that triggers colour picker dialog (default is last).
@@ -3536,15 +3536,15 @@
 
     def OnEvent(self, propgrid, wnd_primary, event) -> None:
         """ Events received by editor widgets are processed here.
 
             Source: https://docs.wxpython.org/wx.propgrid.SystemColourProperty.html
         """
 
-    def OnMeasureImage(self, item: int) -> Size:
+    def OnMeasureImage(self, item: int) -> 'Size':
         """ Returns size of the custom painted image in front of property.
 
             Source: https://docs.wxpython.org/wx.propgrid.SystemColourProperty.html
         """
 
     def OnSetValue(self) -> None:
         """ This virtual function is called after m_value has been set.
@@ -3727,15 +3727,15 @@
 
     def CreateControls(self, propgrid, property, pos, size) -> 'propgrid.PGWindowList':
         """ Instantiates editor controls.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGChoiceEditor.html
         """
 
-    def CreateControlsBase(self, propgrid, property, pos, sz, extraStyle) -> Window:
+    def CreateControlsBase(self, propgrid, property, pos, sz, extraStyle) -> 'Window':
         """ propgrid (wx.propgrid.PropertyGrid) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGChoiceEditor.html
         """
 
     def DeleteItem(self, ctrl, index) -> None:
         """ Deletes item from existing control.
@@ -3984,15 +3984,15 @@
     """
     def __init__(self, label=PG_LABEL, name=PG_LABEL, value=WHITE) -> None:
         """ label (string) â
 
             Source: https://docs.wxpython.org/wx.propgrid.ColourProperty.html
         """
 
-    def GetColour(self, index: int) -> Colour:
+    def GetColour(self, index: int) -> 'Colour':
         """ Default is to use SystemSettings.GetColour(index).
 
             Source: https://docs.wxpython.org/wx.propgrid.ColourProperty.html
         """
 
     def ValueToString(self, value, argFlags=0) -> str:
         """ Converts property value into a text representation.
@@ -4015,15 +4015,15 @@
 
     def OnCustomPaint(self, dc, rect, paintdata) -> None:
         """ Override to paint an image in front of the property value text or drop-down list item (but only if wx.propgrid.PGProperty.OnMeasureImage   is overridden as well).
 
             Source: https://docs.wxpython.org/wx.propgrid.CursorProperty.html
         """
 
-    def OnMeasureImage(self, item: int) -> Size:
+    def OnMeasureImage(self, item: int) -> 'Size':
         """ Returns size of the custom painted image in front of property.
 
             Source: https://docs.wxpython.org/wx.propgrid.CursorProperty.html
         """
 
 
 
@@ -4046,15 +4046,15 @@
 
     def GetDatePickerStyle(self) -> int:
         """ long
 
             Source: https://docs.wxpython.org/wx.propgrid.DateProperty.html
         """
 
-    def GetDateValue(self) -> DateTime:
+    def GetDateValue(self) -> 'DateTime':
         """ DateTime
 
             Source: https://docs.wxpython.org/wx.propgrid.DateProperty.html
         """
 
     def GetFormat(self) -> str:
         """ string
@@ -4112,15 +4112,15 @@
 
     def DisplayEditorDialog(self, pg, value) -> tuple:
         """ Shows editor dialog.
 
             Source: https://docs.wxpython.org/wx.propgrid.DirProperty.html
         """
 
-    def DoGetValidator(self) -> Validator:
+    def DoGetValidator(self) -> 'Validator':
         """ Returns pointer to the   wx.Validator  that should be used with the editor of this property (None for no validator).
 
             Source: https://docs.wxpython.org/wx.propgrid.DirProperty.html
         """
 
     def StringToValue(self, text, argFlags=0) -> tuple:
         """ Converts text into Variant       value appropriate for this property.
@@ -4227,28 +4227,28 @@
 
     def DisplayEditorDialog(self, pg, value) -> tuple:
         """ Shows editor dialog.
 
             Source: https://docs.wxpython.org/wx.propgrid.FileProperty.html
         """
 
-    def DoGetValidator(self) -> Validator:
+    def DoGetValidator(self) -> 'Validator':
         """ Returns pointer to the   wx.Validator  that should be used with the editor of this property (None for no validator).
 
             Source: https://docs.wxpython.org/wx.propgrid.FileProperty.html
         """
 
     def DoSetAttribute(self, name, value) -> bool:
         """ Reimplement this member function to add special handling for attributes of this property.
 
             Source: https://docs.wxpython.org/wx.propgrid.FileProperty.html
         """
 
     @staticmethod
-    def GetClassValidator() -> Validator:
+    def GetClassValidator() -> 'Validator':
         """ Validator
 
             Source: https://docs.wxpython.org/wx.propgrid.FileProperty.html
         """
 
     def GetFileName(self) -> str:
         """ Returns filename to file represented by current value.
@@ -4285,15 +4285,15 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.propgrid.FlagsProperty.html
         """
 
-    def ChildChanged(self, thisValue, childIndex, childValue) -> PGVariant:
+    def ChildChanged(self, thisValue, childIndex, childValue) -> 'propgrid.PGVariant':
         """ Called after value of a child property has been altered.
 
             Source: https://docs.wxpython.org/wx.propgrid.FlagsProperty.html
         """
 
     def DoSetAttribute(self, name, value) -> bool:
         """ Reimplement this member function to add special handling for attributes of this property.
@@ -4355,34 +4355,34 @@
     """
     def __init__(self, label=PG_LABEL, name=PG_LABEL, value=0.0) -> None:
         """ label (string) â
 
             Source: https://docs.wxpython.org/wx.propgrid.FloatProperty.html
         """
 
-    def AddSpinStepValue(self, stepScale: int) -> PGVariant:
+    def AddSpinStepValue(self, stepScale: int) -> 'propgrid.PGVariant':
         """ Returns what would be the new value of the property after adding SpinCtrl editor step to the current value.
 
             Source: https://docs.wxpython.org/wx.propgrid.FloatProperty.html
         """
 
-    def DoGetValidator(self) -> Validator:
+    def DoGetValidator(self) -> 'Validator':
         """ Returns pointer to the   wx.Validator  that should be used with the editor of this property (None for no validator).
 
             Source: https://docs.wxpython.org/wx.propgrid.FloatProperty.html
         """
 
     def DoSetAttribute(self, name, value) -> bool:
         """ Reimplement this member function to add special handling for attributes of this property.
 
             Source: https://docs.wxpython.org/wx.propgrid.FloatProperty.html
         """
 
     @staticmethod
-    def GetClassValidator() -> Validator:
+    def GetClassValidator() -> 'Validator':
         """ Validator
 
             Source: https://docs.wxpython.org/wx.propgrid.FloatProperty.html
         """
 
     def StringToValue(self, text, argFlags=0) -> tuple:
         """ Converts text into Variant       value appropriate for this property.
@@ -4411,15 +4411,15 @@
     """
     def __init__(*args, **kwargs) -> None:
         """ label (string) â
 
             Source: https://docs.wxpython.org/wx.propgrid.FontProperty.html
         """
 
-    def ChildChanged(self, thisValue, childIndex, childValue) -> PGVariant:
+    def ChildChanged(self, thisValue, childIndex, childValue) -> 'propgrid.PGVariant':
         """ Called after value of a child property has been altered.
 
             Source: https://docs.wxpython.org/wx.propgrid.FontProperty.html
         """
 
     def DisplayEditorDialog(self, pg, value) -> tuple:
         """ Shows editor dialog.
@@ -4460,15 +4460,15 @@
 
     def OnCustomPaint(self, dc, rect, paintdata) -> None:
         """ Override to paint an image in front of the property value text or drop-down list item (but only if wx.propgrid.PGProperty.OnMeasureImage   is overridden as well).
 
             Source: https://docs.wxpython.org/wx.propgrid.ImageFileProperty.html
         """
 
-    def OnMeasureImage(self, item: int) -> Size:
+    def OnMeasureImage(self, item: int) -> 'Size':
         """ Returns size of the custom painted image in front of property.
 
             Source: https://docs.wxpython.org/wx.propgrid.ImageFileProperty.html
         """
 
     def OnSetValue(self) -> None:
         """ This virtual function is called after m_value has been set.
@@ -4485,28 +4485,28 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.propgrid.IntProperty.html
         """
 
-    def AddSpinStepValue(self, stepScale: int) -> PGVariant:
+    def AddSpinStepValue(self, stepScale: int) -> 'propgrid.PGVariant':
         """ Returns what would be the new value of the property after adding SpinCtrl editor step to the current value.
 
             Source: https://docs.wxpython.org/wx.propgrid.IntProperty.html
         """
 
-    def DoGetValidator(self) -> Validator:
+    def DoGetValidator(self) -> 'Validator':
         """ Returns pointer to the   wx.Validator  that should be used with the editor of this property (None for no validator).
 
             Source: https://docs.wxpython.org/wx.propgrid.IntProperty.html
         """
 
     @staticmethod
-    def GetClassValidator() -> Validator:
+    def GetClassValidator() -> 'Validator':
         """ Validator
 
             Source: https://docs.wxpython.org/wx.propgrid.IntProperty.html
         """
 
     def IntToValue(self, number, argFlags=0) -> tuple:
         """ Converts integer (possibly a choice selection) into Variant       value appropriate for this property.
@@ -4688,21 +4688,21 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.propgrid.UIntProperty.html
         """
 
-    def AddSpinStepValue(self, stepScale: int) -> PGVariant:
+    def AddSpinStepValue(self, stepScale: int) -> 'propgrid.PGVariant':
         """ Returns what would be the new value of the property after adding SpinCtrl editor step to the current value.
 
             Source: https://docs.wxpython.org/wx.propgrid.UIntProperty.html
         """
 
-    def DoGetValidator(self) -> Validator:
+    def DoGetValidator(self) -> 'Validator':
         """ Returns pointer to the   wx.Validator  that should be used with the editor of this property (None for no validator).
 
             Source: https://docs.wxpython.org/wx.propgrid.UIntProperty.html
         """
 
     def DoSetAttribute(self, name, value) -> bool:
         """ Reimplement this member function to add special handling for attributes of this property.
@@ -4738,15 +4738,15 @@
 
 class NumericProperty(PGProperty):
     """ This is an abstract class which serves as a base class for numeric
 properties, like IntProperty, UIntProperty, FloatProperty.
 
         Source: https://docs.wxpython.org/wx.propgrid.NumericProperty.html
     """
-    def AddSpinStepValue(self, stepScale: int) -> PGVariant:
+    def AddSpinStepValue(self, stepScale: int) -> 'propgrid.PGVariant':
         """ Returns what would be the new value of the property after adding SpinCtrl editor step to the current value.
 
             Source: https://docs.wxpython.org/wx.propgrid.NumericProperty.html
         """
 
     def DoSetAttribute(self, name, value) -> bool:
         """ Reimplement this member function to add special handling for attributes of this property.
@@ -4881,15 +4881,15 @@
 
     def GetDataPtr(self) -> 'propgrid.PGChoicesData':
         """ Returns plain data ptr - no refcounting stuff is done.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGChoices.html
         """
 
-    def GetId(self) -> 'IntPtr':
+    def GetId(self) -> int:
         """ Gets an  number identifying this list.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGChoices.html
         """
 
     def GetIndicesForStrings(self, strings, unmatched=None) -> list[int]:
         """ Returns array of indices matching given strings.
@@ -4968,15 +4968,15 @@
 
             Source: https://docs.wxpython.org/wx.propgrid.PGChoices.html
         """
 
     Count: int  # See GetCount
     Data: 'propgrid.PGChoicesData'  # See GetData
     DataPtr: 'propgrid.PGChoicesData'  # See GetDataPtr
-    Id: 'IntPtr'  # See GetId
+    Id: int  # See GetId
     Labels: list[str]  # See GetLabels
 
 
 
 class PGCellRenderer(ObjectRefData):
     """ Base class for PropertyGrid cell renderers.
 
@@ -5002,15 +5002,15 @@
 
     def DrawText(self, dc, rect, imageWidth, text) -> None:
         """ Utility to draw vertically centered text.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCellRenderer.html
         """
 
-    def GetImageSize(self, property, column, item) -> Size:
+    def GetImageSize(self, property, column, item) -> 'Size':
         """ Returns size of the image in front of the editable area.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCellRenderer.html
         """
 
     def PostDrawCell(self, dc, propGrid, cell, flags) -> None:
         """ Utility to be called after drawing is done, to revert whatever changes PreDrawCell   did.
@@ -5028,14 +5028,16 @@
         """ Returns True if rendered something in the foreground (text or bitmap).
 
             Source: https://docs.wxpython.org/wx.propgrid.PGCellRenderer.html
         """
 
 
 
+PGPropertyFlags: TypeAlias = int  # Enumeration
+
 PG_PROP_MODIFIED: int
 
 PG_PROP_DISABLED: int
 
 PG_PROP_HIDDEN: int
 
 PG_PROP_CUSTOMIMAGE: int
@@ -5086,27 +5088,27 @@
 
 class PGValidationInfo:
     """ Used to convey validation information to and from functions that
 actually perform validation.
 
         Source: https://docs.wxpython.org/wx.propgrid.PGValidationInfo.html
     """
-    def GetFailureBehavior(self) -> 'byte':
+    def GetFailureBehavior(self) -> 'propgrid.byte':
         """ wx.byte
 
             Source: https://docs.wxpython.org/wx.propgrid.PGValidationInfo.html
         """
 
     def GetFailureMessage(self) -> str:
         """ Returns current failure message.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGValidationInfo.html
         """
 
-    def GetValue(self) -> PGVariant:
+    def GetValue(self) -> 'propgrid.PGVariant':
         """ Returns reference to pending value.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGValidationInfo.html
         """
 
     def SetFailureBehavior(self, failureBehavior: 'byte') -> None:
         """ Set validation failure behaviour.
@@ -5116,17 +5118,17 @@
 
     def SetFailureMessage(self, message: str) -> None:
         """ Set current failure message.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGValidationInfo.html
         """
 
-    FailureBehavior: 'byte'  # See GetFailureBehavior and SetFailureBehavior
+    FailureBehavior: 'propgrid.byte'  # See GetFailureBehavior and SetFailureBehavior
     FailureMessage: str  # See GetFailureMessage and SetFailureMessage
-    Value: PGVariant  # See GetValue
+    Value: 'propgrid.PGVariant'  # See GetValue
 
 
 
 class PGVIterator:
     """  Overloaded Implementations:
 
         Source: https://docs.wxpython.org/wx.propgrid.PGVIterator.html
@@ -5293,15 +5295,15 @@
     """
     def __init__(self) -> None:
         """ 
 
             Source: https://docs.wxpython.org/wx.propgrid.PGAttributeStorage.html
         """
 
-    def FindValue(self, name: str) -> PGVariant:
+    def FindValue(self, name: str) -> 'propgrid.PGVariant':
         """ name (string) â
 
             Source: https://docs.wxpython.org/wx.propgrid.PGAttributeStorage.html
         """
 
     def GetCount(self) -> int:
         """ int
@@ -5497,21 +5499,29 @@
 
 
 class PGDefaultRenderer(PGCellRenderer):
     """ Default cell renderer, that can handles the common scenarios.
 
         Source: https://docs.wxpython.org/wx.propgrid.PGDefaultRenderer.html
     """
-    def GetImageSize(self, property, column, item) -> Size:
+    def GetImageSize(self, property, column, item) -> 'Size':
         """ Returns size of the image in front of the editable area.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGDefaultRenderer.html
         """
 
     def Render(self, dc, rect, propertyGrid, property, column, item, flags) -> bool:
         """ Returns True if rendered something in the foreground (text or bitmap.
 
             Source: https://docs.wxpython.org/wx.propgrid.PGDefaultRenderer.html
         """
 
 
 
+PGVariant: TypeAlias = Any
+
+byte: TypeAlias = bytes
+
+ArrayPGProperty: TypeAlias = list['PGProperty']
+
+FlagType: TypeAlias = int  # Enumeration
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/ribbon/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/ribbon/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class RibbonButtonBarEvent(CommandEvent):
     """ Event used to indicate various actions relating to a button on a
 RibbonButtonBar.
 
         Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBarEvent.html
     """
@@ -15,15 +15,15 @@
 
     def GetBar(self) -> 'ribbon.RibbonButtonBar':
         """ Returns the bar which contains the button which the event relates to.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBarEvent.html
         """
 
-    def GetButton(self) -> RibbonButtonBarButtonBase:
+    def GetButton(self) -> 'ribbon.RibbonButtonBarButtonBase':
         """ Returns the button which the event relates to.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBarEvent.html
         """
 
     def PopupMenu(self, menu: 'Menu') -> bool:
         """ Display a popup menu as a result of this (dropdown clicked) event.
@@ -40,15 +40,15 @@
     def SetButton(self, bar: RibbonButtonBarButtonBase) -> None:
         """ Sets the button relating to this event.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBarEvent.html
         """
 
     Bar: 'ribbon.RibbonButtonBar'  # See GetBar and SetBar
-    Button: RibbonButtonBarButtonBase  # See GetButton and SetButton
+    Button: 'ribbon.RibbonButtonBarButtonBase'  # See GetButton and SetButton
 
 
 
 class RibbonGalleryEvent(CommandEvent):
     """ Constructor.
 
         Source: https://docs.wxpython.org/wx.ribbon.RibbonGalleryEvent.html
@@ -61,15 +61,15 @@
 
     def GetGallery(self) -> 'ribbon.RibbonGallery':
         """ Returns the gallery which the event relates to.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGalleryEvent.html
         """
 
-    def GetGalleryItem(self) -> RibbonGalleryItem:
+    def GetGalleryItem(self) -> 'ribbon.RibbonGalleryItem':
         """ Returns the gallery item which the event relates to, or None if it does not relate to an item.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGalleryEvent.html
         """
 
     def SetGallery(self, gallery: 'ribbon.RibbonGallery') -> None:
         """ Sets the gallery relating to this event.
@@ -80,15 +80,15 @@
     def SetGalleryItem(self, item: RibbonGalleryItem) -> None:
         """ Sets the gallery item relating to this event.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGalleryEvent.html
         """
 
     Gallery: 'ribbon.RibbonGallery'  # See GetGallery and SetGallery
-    GalleryItem: RibbonGalleryItem  # See GetGalleryItem and SetGalleryItem
+    GalleryItem: 'ribbon.RibbonGalleryItem'  # See GetGalleryItem and SetGalleryItem
 
 
 
 class RibbonPanelEvent(CommandEvent):
     """ Event used to indicate various actions relating to a RibbonPanel.
 
         Source: https://docs.wxpython.org/wx.ribbon.RibbonPanelEvent.html
@@ -157,21 +157,21 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonControl.html
         """
 
-    def DoGetNextLargerSize(self, direction, relative_to) -> Size:
+    def DoGetNextLargerSize(self, direction, relative_to) -> 'Size':
         """ Implementation of GetNextLargerSize .
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonControl.html
         """
 
-    def DoGetNextSmallerSize(self, direction, relative_to) -> Size:
+    def DoGetNextSmallerSize(self, direction, relative_to) -> 'Size':
         """ Implementation of GetNextSmallerSize .
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonControl.html
         """
 
     def GetAncestorRibbonBar(self) -> 'ribbon.RibbonBar':
         """ Get the first ancestor which is a   wx.ribbon.RibbonBar  (or derived) or None if not having such parent.
@@ -181,34 +181,34 @@
 
     def GetArtProvider(self) -> 'ribbon.RibbonArtProvider':
         """ Get the art provider to be used.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonControl.html
         """
 
-    def GetBestSizeForParentSize(self, parentSize: Union[tuple[int, int], 'Size']) -> Size:
+    def GetBestSizeForParentSize(self, parentSize: Union[tuple[int, int], 'Size']) -> 'Size':
         """ Finds the best width and height given the parentâs width and height.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonControl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonControl.html
         """
 
-    def GetNextLargerSize(self, *args, **kw) -> Size:
+    def GetNextLargerSize(self, *args, **kw) -> 'Size':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonControl.html
         """
 
-    def GetNextSmallerSize(self, *args, **kw) -> Size:
+    def GetNextSmallerSize(self, *args, **kw) -> 'Size':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonControl.html
         """
 
     def IsSizingContinuous(self) -> bool:
         """ bool
@@ -275,33 +275,33 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def AddButton(self, *args, **kw) -> RibbonButtonBarButtonBase:
+    def AddButton(self, *args, **kw) -> 'ribbon.RibbonButtonBarButtonBase':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def AddDropdownButton(self, button_id, label, bitmap, help_string="") -> RibbonButtonBarButtonBase:
+    def AddDropdownButton(self, button_id, label, bitmap, help_string="") -> 'ribbon.RibbonButtonBarButtonBase':
         """ Add a dropdown button to the button bar (simple version).
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def AddHybridButton(self, button_id, label, bitmap, help_string="") -> RibbonButtonBarButtonBase:
+    def AddHybridButton(self, button_id, label, bitmap, help_string="") -> 'ribbon.RibbonButtonBarButtonBase':
         """ Add a hybrid button to the button bar (simple version).
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def AddToggleButton(self, button_id, label, bitmap, help_string="") -> RibbonButtonBarButtonBase:
+    def AddToggleButton(self, button_id, label, bitmap, help_string="") -> 'ribbon.RibbonButtonBarButtonBase':
         """ Add a toggle button to the button bar (simple version).
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
     def ClearButtons(self) -> None:
         """ Delete all buttons from the button bar.
@@ -323,94 +323,94 @@
 
     def EnableButton(self, button_id, enable=True) -> None:
         """ Enable or disable a single button on the bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def GetActiveItem(self) -> RibbonButtonBarButtonBase:
+    def GetActiveItem(self) -> 'ribbon.RibbonButtonBarButtonBase':
         """ Returns the active item of the button bar or None if there is none.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
     def GetButtonCount(self) -> int:
         """ Returns the number of buttons in this button bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def GetHoveredItem(self) -> RibbonButtonBarButtonBase:
+    def GetHoveredItem(self) -> 'ribbon.RibbonButtonBarButtonBase':
         """ Returns the hovered item of the button bar or None if there is none.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def GetItem(self, n: int) -> RibbonButtonBarButtonBase:
+    def GetItem(self, n: int) -> 'ribbon.RibbonButtonBarButtonBase':
         """ Returns the N-th button of the bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def GetItemById(self, id: int) -> RibbonButtonBarButtonBase:
+    def GetItemById(self, id: int) -> 'ribbon.RibbonButtonBarButtonBase':
         """ Returns the first button having a given id or None if none matches.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def GetItemClientData(self, item: RibbonButtonBarButtonBase) -> ClientData:
+    def GetItemClientData(self, item: RibbonButtonBarButtonBase) -> 'ClientData':
         """ Get the client object associated with a button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
     def GetItemId(self, item: RibbonButtonBarButtonBase) -> int:
         """ Returns the id of a button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def GetItemRect(self, button_id: int) -> Rect:
+    def GetItemRect(self, button_id: int) -> 'Rect':
         """ Returns the itemsâs rect with coordinates relative to the button barâs parent, or a default-constructed rect if the tool is not found.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
     def GetShowToolTipsForDisabled(self) -> bool:
         """ Sets whether tooltips should be shown for disabled buttons or not.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def InsertButton(self, *args, **kw) -> RibbonButtonBarButtonBase:
+    def InsertButton(self, *args, **kw) -> 'ribbon.RibbonButtonBarButtonBase':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def InsertDropdownButton(self, pos, button_id, label, bitmap, help_string="") -> RibbonButtonBarButtonBase:
+    def InsertDropdownButton(self, pos, button_id, label, bitmap, help_string="") -> 'ribbon.RibbonButtonBarButtonBase':
         """ Inserts a dropdown button to the button bar (simple version) at the given position.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def InsertHybridButton(self, pos, button_id, label, bitmap, help_string="") -> RibbonButtonBarButtonBase:
+    def InsertHybridButton(self, pos, button_id, label, bitmap, help_string="") -> 'ribbon.RibbonButtonBarButtonBase':
         """ Inserts a hybrid button to the button bar (simple version) at the given position.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    def InsertToggleButton(self, pos, button_id, label, bitmap, help_string="") -> RibbonButtonBarButtonBase:
+    def InsertToggleButton(self, pos, button_id, label, bitmap, help_string="") -> 'ribbon.RibbonButtonBarButtonBase':
         """ Inserts a toggle button to the button bar (simple version) at the given position.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
     def Realize(self) -> bool:
         """ Calculate button layouts and positions.
@@ -462,17 +462,17 @@
 
     def ToggleButton(self, button_id, checked) -> None:
         """ Set a toggle button to the checked or unchecked state.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonButtonBar.html
         """
 
-    ActiveItem: RibbonButtonBarButtonBase  # See GetActiveItem
+    ActiveItem: 'ribbon.RibbonButtonBarButtonBase'  # See GetActiveItem
     ButtonCount: int  # See GetButtonCount
-    HoveredItem: RibbonButtonBarButtonBase  # See GetHoveredItem
+    HoveredItem: 'ribbon.RibbonButtonBarButtonBase'  # See GetHoveredItem
     ShowToolTipsForDisabled: bool  # See GetShowToolTipsForDisabled and SetShowToolTipsForDisabled
 
 
 
 EVT_RIBBONBUTTONBAR_CLICKED: int  # Triggered when the normal (non-dropdown) region of a button on the button bar is clicked.
 
 EVT_RIBBONBUTTONBAR_DROPDOWN_CLICKED: int  # Triggered when the dropdown region of a button on the button bar is clicked. wx.ribbon.RibbonButtonBarEvent.PopupMenu   should be called by the event handler if it wants to display a popup menu (which is what most dropdown buttons should be doing). ^^
@@ -533,15 +533,15 @@
     def GetActivePage(self) -> int:
         """ Get the index of the active page.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonBar.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonBar.html
         """
 
     def GetDisplayMode(self) -> 'ribbon.RibbonDisplayMode':
         """ Returns the current display mode of the panel area.
@@ -685,15 +685,15 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
-    def Append(self, *args, **kw) -> RibbonGalleryItem:
+    def Append(self, *args, **kw) -> 'ribbon.RibbonGalleryItem':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
     def Clear(self) -> None:
         """ Remove all items from the gallery.
@@ -709,22 +709,22 @@
 
     def EnsureVisible(self, item: RibbonGalleryItem) -> None:
         """ Scroll the gallery to ensure that the given item is visible.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
-    def GetActiveItem(self) -> RibbonGalleryItem:
+    def GetActiveItem(self) -> 'ribbon.RibbonGalleryItem':
         """ Get the currently active item, or None if there is none.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
     def GetCount(self) -> int:
         """ Get the number of items in the gallery.
@@ -740,33 +740,33 @@
 
     def GetExtensionButtonState(self) -> 'ribbon.RibbonGalleryButtonState':
         """ Get the state of the âextensionâ button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
-    def GetHoveredItem(self) -> RibbonGalleryItem:
+    def GetHoveredItem(self) -> 'ribbon.RibbonGalleryItem':
         """ Get the currently hovered item, or None if there is none.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
-    def GetItem(self, n: int) -> RibbonGalleryItem:
+    def GetItem(self, n: int) -> 'ribbon.RibbonGalleryItem':
         """ Get an item by index.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
-    def GetItemClientData(self, item: RibbonGalleryItem) -> ClientData:
+    def GetItemClientData(self, item: RibbonGalleryItem) -> 'ClientData':
         """ Get the client object associated with a gallery item.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
-    def GetSelection(self) -> RibbonGalleryItem:
+    def GetSelection(self) -> 'ribbon.RibbonGalleryItem':
         """ Get the currently selected item, or None if there is none.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
     def GetUpButtonState(self) -> 'ribbon.RibbonGalleryButtonState':
         """ Get the state of the scroll up button.
@@ -806,20 +806,20 @@
 
     def SetSelection(self, item: RibbonGalleryItem) -> None:
         """ Set the selection to the given item, or removes the selection if item  == None.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonGallery.html
         """
 
-    ActiveItem: RibbonGalleryItem  # See GetActiveItem
+    ActiveItem: 'ribbon.RibbonGalleryItem'  # See GetActiveItem
     Count: int  # See GetCount
     DownButtonState: 'ribbon.RibbonGalleryButtonState'  # See GetDownButtonState
     ExtensionButtonState: 'ribbon.RibbonGalleryButtonState'  # See GetExtensionButtonState
-    HoveredItem: RibbonGalleryItem  # See GetHoveredItem
-    Selection: RibbonGalleryItem  # See GetSelection and SetSelection
+    HoveredItem: 'ribbon.RibbonGalleryItem'  # See GetHoveredItem
+    Selection: 'ribbon.RibbonGalleryItem'  # See GetSelection and SetSelection
     UpButtonState: 'ribbon.RibbonGalleryButtonState'  # See GetUpButtonState
 
 
 
 EVT_RIBBONGALLERY_SELECTED: int  # Triggered when the user selects an item from the gallery. Note that the ID is that of the gallery, not of the item.
 
 EVT_RIBBONGALLERY_CLICKED: int  # Similar to EVT_RIBBONGALLERY_SELECTED but triggered every time a gallery item is clicked, even if it is already selected. Note that the ID of the event is that of the gallery, not of the item, just as above. This event is available since wxWidgets 2.9.2.
@@ -846,15 +846,15 @@
     def Create(self, parent, id=ID_ANY, label="", icon=NullBitmap, pos=DefaultPosition, size=DefaultSize, style=RIBBON_PANEL_DEFAULT_STYLE) -> bool:
         """ Create a ribbon panel in two-step ribbon panel construction.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPanel.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPanel.html
         """
 
     def GetExpandedDummy(self) -> 'ribbon.RibbonPanel':
         """ Get the dummy panel of an expanded panel.
@@ -864,15 +864,15 @@
 
     def GetExpandedPanel(self) -> 'ribbon.RibbonPanel':
         """ Get the expanded panel of a dummy panel.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPanel.html
         """
 
-    def GetMinimisedIcon(self) -> Bitmap:
+    def GetMinimisedIcon(self) -> 'Bitmap':
         """ Get the bitmap to be used in place of the panel children when it is minimised.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPanel.html
         """
 
     def HasExtButton(self) -> bool:
         """ Test if the panel has an extension button.
@@ -920,15 +920,15 @@
         """ Show the panel externally expanded.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPanel.html
         """
 
     ExpandedDummy: 'ribbon.RibbonPanel'  # See GetExpandedDummy
     ExpandedPanel: 'ribbon.RibbonPanel'  # See GetExpandedPanel
-    MinimisedIcon: Bitmap  # See GetMinimisedIcon
+    MinimisedIcon: 'Bitmap'  # See GetMinimisedIcon
 
 
 
 RIBBON_PANEL_DEFAULT_STYLE: int  # Defined as no other flags set.
 
 RIBBON_PANEL_NO_AUTO_MINIMISE: int  # Prevents the panel from automatically minimising to conserve screen space.
 
@@ -948,39 +948,39 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def AddDropdownTool(self, tool_id, bitmap, help_string="") -> RibbonToolBarToolBase:
+    def AddDropdownTool(self, tool_id, bitmap, help_string="") -> 'ribbon.RibbonToolBarToolBase':
         """ Add a dropdown tool to the tool bar (simple version).
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def AddHybridTool(self, tool_id, bitmap, help_string="") -> RibbonToolBarToolBase:
+    def AddHybridTool(self, tool_id, bitmap, help_string="") -> 'ribbon.RibbonToolBarToolBase':
         """ Add a hybrid tool to the tool bar (simple version).
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def AddSeparator(self) -> RibbonToolBarToolBase:
+    def AddSeparator(self) -> 'ribbon.RibbonToolBarToolBase':
         """ Add a separator to the tool bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def AddToggleTool(self, tool_id, bitmap, help_string) -> RibbonToolBarToolBase:
+    def AddToggleTool(self, tool_id, bitmap, help_string) -> 'ribbon.RibbonToolBarToolBase':
         """ Add a toggle tool to the tool bar (simple version).
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def AddTool(self, *args, **kw) -> RibbonToolBarToolBase:
+    def AddTool(self, *args, **kw) -> 'ribbon.RibbonToolBarToolBase':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
     def ClearTools(self) -> None:
         """ Deletes all the tools in the toolbar.
@@ -1008,40 +1008,40 @@
 
     def EnableTool(self, tool_id, enable=True) -> None:
         """ Enable or disable a single tool on the bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def FindById(self, tool_id: int) -> RibbonToolBarToolBase:
+    def FindById(self, tool_id: int) -> 'ribbon.RibbonToolBarToolBase':
         """ Returns a pointer to the tool opaque structure by id  or None if no corresponding tool is found.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def GetActiveTool(self) -> RibbonToolBarToolBase:
+    def GetActiveTool(self) -> 'ribbon.RibbonToolBarToolBase':
         """ Returns the active item of the tool bar or None if there is none.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def GetToolByPos(self, *args, **kw) -> RibbonToolBarToolBase:
+    def GetToolByPos(self, *args, **kw) -> 'ribbon.RibbonToolBarToolBase':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def GetToolClientData(self, tool_id: int) -> PyUserData:
+    def GetToolClientData(self, tool_id: int) -> 'PyUserData':
         """ Get any client data associated with the tool.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
     def GetToolCount(self) -> int:
         """ Returns the number of tools in the toolbar.
@@ -1075,51 +1075,51 @@
 
     def GetToolPos(self, tool_id: int) -> int:
         """ Returns the tool position in the toolbar, or  NOT_FOUND   if the tool is not found.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def GetToolRect(self, tool_id: int) -> Rect:
+    def GetToolRect(self, tool_id: int) -> 'Rect':
         """ Returns the toolâs rect with coordinates relative to the toolbarâs parent, or a default-constructed rect if the tool is not found.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
     def GetToolState(self, tool_id: int) -> bool:
         """ Gets the on/off state of a toggle tool.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def InsertDropdownTool(self, pos, tool_id, bitmap, help_string="") -> RibbonToolBarToolBase:
+    def InsertDropdownTool(self, pos, tool_id, bitmap, help_string="") -> 'ribbon.RibbonToolBarToolBase':
         """ Insert a dropdown tool to the tool bar (simple version) as the specified position.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def InsertHybridTool(self, pos, tool_id, bitmap, help_string="") -> RibbonToolBarToolBase:
+    def InsertHybridTool(self, pos, tool_id, bitmap, help_string="") -> 'ribbon.RibbonToolBarToolBase':
         """ Insert a hybrid tool to the tool bar (simple version) as the specified position.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def InsertSeparator(self, pos: int) -> RibbonToolBarToolBase:
+    def InsertSeparator(self, pos: int) -> 'ribbon.RibbonToolBarToolBase':
         """ Insert a separator to the tool bar at the specified position.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def InsertToggleTool(self, pos, tool_id, bitmap, help_string="") -> RibbonToolBarToolBase:
+    def InsertToggleTool(self, pos, tool_id, bitmap, help_string="") -> 'ribbon.RibbonToolBarToolBase':
         """ Insert a toggle tool to the tool bar (simple version) as the specified position.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    def InsertTool(self, *args, **kw) -> RibbonToolBarToolBase:
+    def InsertTool(self, *args, **kw) -> 'ribbon.RibbonToolBarToolBase':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
     def Realize(self) -> bool:
         """ Calculate tool layouts and positions.
@@ -1159,15 +1159,15 @@
 
     def ToggleTool(self, tool_id, checked) -> None:
         """ Set a toggle tool to the checked or unchecked state.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonToolBar.html
         """
 
-    ActiveTool: RibbonToolBarToolBase  # See GetActiveTool
+    ActiveTool: 'ribbon.RibbonToolBarToolBase'  # See GetActiveTool
     ToolCount: int  # See GetToolCount
 
 
 
 EVT_RIBBONTOOLBAR_CLICKED: int  # Triggered when the normal (non-dropdown) region of a tool on the tool bar is clicked.
 
 EVT_RIBBONTOOLBAR_DROPDOWN_CLICKED: int  # Triggered when the dropdown region of a tool on the tool bar is clicked. wx.ribbon.RibbonToolBarEvent.PopupMenu   should be called by the event handler if it wants to display a popup menu (which is what most dropdown tools should be doing). ^^
@@ -1288,15 +1288,15 @@
 
     def GetBarTabWidth(self, dc, wnd, label, bitmap, ideal, small_begin_need_separator, small_must_have_separator, minimum) -> None:
         """ Calculate the ideal and minimum width (in pixels) of a tab in a ribbon bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetBarToggleButtonArea(self, rect: 'Rect') -> Rect:
+    def GetBarToggleButtonArea(self, rect: 'Rect') -> 'Rect':
         """ Calculate the position and size of the ribbonâs toggle button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
     def GetButtonBarButtonSize(self, dc, wnd, kind, size, label, text_min_width, bitmap_size_large, bitmap_size_small, button_size, normal_region, dropdown_region) -> bool:
         """ Calculate the size of a button within a   wx.ribbon.RibbonButtonBar.
@@ -1306,21 +1306,21 @@
 
     def GetButtonBarButtonTextWidth(self, dc, label, kind, size) -> 'Coord':
         """ Gets the width of the string if it is used as a   wx.ribbon.RibbonButtonBar  button label.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetColor(self, id: int) -> Colour:
+    def GetColor(self, id: int) -> 'Colour':
         """ id (int) â
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetColour(self, id: int) -> Colour:
+    def GetColour(self, id: int) -> 'Colour':
         """ Get the value of a certain colour setting.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
     def GetColourScheme(self) -> tuple:
         """ Get the current colour scheme.
@@ -1330,87 +1330,87 @@
 
     def GetFlags(self) -> int:
         """ Get the previously set style flags.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetFont(self, id: int) -> Font:
+    def GetFont(self, id: int) -> 'Font':
         """ Get the value of a certain font setting.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetGalleryClientSize(self, dc, wnd, size, client_offset, scroll_up_button, scroll_down_button, extension_button) -> Size:
+    def GetGalleryClientSize(self, dc, wnd, size, client_offset, scroll_up_button, scroll_down_button, extension_button) -> 'Size':
         """ Calculate the client size of a   wx.ribbon.RibbonGallery  control for a given size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetGallerySize(self, dc, wnd, client_size) -> Size:
+    def GetGallerySize(self, dc, wnd, client_size) -> 'Size':
         """ Calculate the size of a   wx.ribbon.RibbonGallery  control for a given client size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
     def GetMetric(self, id: int) -> int:
         """ Get the value of a certain integer setting.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetMinimisedPanelMinimumSize(self, dc, wnd, desired_bitmap_size, expanded_panel_direction) -> Size:
+    def GetMinimisedPanelMinimumSize(self, dc, wnd, desired_bitmap_size, expanded_panel_direction) -> 'Size':
         """ Calculate the size of a minimised ribbon panel.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetPageBackgroundRedrawArea(self, dc, wnd, page_old_size, page_new_size) -> Rect:
+    def GetPageBackgroundRedrawArea(self, dc, wnd, page_old_size, page_new_size) -> 'Rect':
         """ Calculate the portion of a page background which needs to be redrawn when a page is resized.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetPanelClientSize(self, dc, wnd, size, client_offset) -> Size:
+    def GetPanelClientSize(self, dc, wnd, size, client_offset) -> 'Size':
         """ Calculate the client size of a panel for a given overall size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetPanelExtButtonArea(self, dc, wnd, rect) -> Rect:
+    def GetPanelExtButtonArea(self, dc, wnd, rect) -> 'Rect':
         """ Calculate the position and size of the panel extension button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetPanelSize(self, dc, wnd, client_size, client_offset) -> Size:
+    def GetPanelSize(self, dc, wnd, client_size, client_offset) -> 'Size':
         """ Calculate the size of a panel for a given client size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetRibbonHelpButtonArea(self, rect: 'Rect') -> Rect:
+    def GetRibbonHelpButtonArea(self, rect: 'Rect') -> 'Rect':
         """ Calculate the position and size of the ribbonâs help button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetScrollButtonMinimumSize(self, dc, wnd, style) -> Size:
+    def GetScrollButtonMinimumSize(self, dc, wnd, style) -> 'Size':
         """ Calculate the minimum size (in pixels) of a scroll button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
     def GetTabCtrlHeight(self, dc, wnd, pages) -> int:
         """ Calculate the height (in pixels) of the tab region of a ribbon bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
-    def GetToolSize(self, dc, wnd, bitmap_size, kind, is_first, is_last, dropdown_region) -> Size:
+    def GetToolSize(self, dc, wnd, bitmap_size, kind, is_first, is_last, dropdown_region) -> 'Size':
         """ Calculate the size of a tool within a   wx.ribbon.RibbonToolBar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonArtProvider.html
         """
 
     def SetColor(self, id, color) -> None:
         """ id (int) â
@@ -1486,21 +1486,21 @@
     def DismissExpandedPanel(self) -> bool:
         """ Dismiss the current externally expanded panel, if there is one.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPage.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPage.html
         """
 
-    def GetIcon(self) -> Bitmap:
+    def GetIcon(self) -> 'Bitmap':
         """ Get the icon used for the page in the ribbon bar tab area (only displayed if the ribbon bar is actually showing icons).
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPage.html
         """
 
     def GetMajorAxis(self) -> 'Orientation':
         """ Get the direction in which ribbon panels are stacked within the page.
@@ -1540,33 +1540,37 @@
 
     def SetSizeWithScrollButtonAdjustment(self, x, y, width, height) -> None:
         """ Set the size of the page and the external scroll buttons (if any).
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonPage.html
         """
 
-    Icon: Bitmap  # See GetIcon
+    Icon: 'Bitmap'  # See GetIcon
     MajorAxis: 'Orientation'  # See GetMajorAxis
 
 
 
 HORIZONTAL: int
 
 VERTICAL: int
 
 BOTH: int
 
+RibbonButtonKind: TypeAlias = int  # Enumeration
+
 RIBBON_BUTTON_NORMAL: int
 
 RIBBON_BUTTON_DROPDOWN: int
 
 RIBBON_BUTTON_HYBRID: int
 
 RIBBON_BUTTON_TOGGLE: int
 
+RibbonButtonBarButtonState: TypeAlias = int  # Enumeration
+
 RIBBON_BUTTONBAR_BUTTON_SIZE_MASK: int
 
 RIBBON_BUTTONBAR_BUTTON_NORMAL_HOVERED: int
 
 RIBBON_BUTTONBAR_BUTTON_DROPDOWN_HOVERED: int
 
 RIBBON_BUTTONBAR_BUTTON_HOVER_MASK: int
@@ -1577,20 +1581,24 @@
 
 RIBBON_BUTTONBAR_BUTTON_ACTIVE_MASK: int
 
 RIBBON_BUTTONBAR_BUTTON_TOGGLED: int
 
 RIBBON_BUTTONBAR_BUTTON_STATE_MASK: int
 
+RibbonDisplayMode: TypeAlias = int  # Enumeration
+
 RIBBON_BAR_PINNED: int
 
 RIBBON_BAR_MINIMIZED: int
 
 RIBBON_BAR_EXPANDED: int
 
+RibbonGalleryButtonState: TypeAlias = int  # Enumeration
+
 RIBBON_GALLERY_BUTTON_NORMAL: int
 
 RIBBON_GALLERY_BUTTON_HOVERED: int
 
 RIBBON_GALLERY_BUTTON_ACTIVE: int
 
 RIBBON_GALLERY_BUTTON_DISABLED: int
@@ -1698,39 +1706,39 @@
 
     def GetBarTabWidth(self, dc, wnd, label, bitmap, ideal, small_begin_need_separator, small_must_have_separator, minimum) -> None:
         """ Calculate the ideal and minimum width (in pixels) of a tab in a ribbon bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonAUIArtProvider.html
         """
 
-    def GetColour(self, id: int) -> Colour:
+    def GetColour(self, id: int) -> 'Colour':
         """ Get the value of a certain colour setting.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonAUIArtProvider.html
         """
 
-    def GetPanelClientSize(self, dc, wnd, size, client_offset) -> Size:
+    def GetPanelClientSize(self, dc, wnd, size, client_offset) -> 'Size':
         """ Calculate the client size of a panel for a given overall size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonAUIArtProvider.html
         """
 
-    def GetPanelExtButtonArea(self, dc, wnd, rect) -> Rect:
+    def GetPanelExtButtonArea(self, dc, wnd, rect) -> 'Rect':
         """ Calculate the position and size of the panel extension button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonAUIArtProvider.html
         """
 
-    def GetPanelSize(self, dc, wnd, client_size, client_offset) -> Size:
+    def GetPanelSize(self, dc, wnd, client_size, client_offset) -> 'Size':
         """ Calculate the size of a panel for a given client size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonAUIArtProvider.html
         """
 
-    def GetScrollButtonMinimumSize(self, dc, wnd, style) -> Size:
+    def GetScrollButtonMinimumSize(self, dc, wnd, style) -> 'Size':
         """ Calculate the minimum size (in pixels) of a scroll button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonAUIArtProvider.html
         """
 
     def GetTabCtrlHeight(self, dc, wnd, pages) -> int:
         """ Calculate the height (in pixels) of the tab region of a ribbon bar.
@@ -1873,15 +1881,15 @@
 
     def GetBarTabWidth(self, dc, wnd, label, bitmap, ideal, small_begin_need_separator, small_must_have_separator, minimum) -> None:
         """ Calculate the ideal and minimum width (in pixels) of a tab in a ribbon bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetBarToggleButtonArea(self, rect: 'Rect') -> Rect:
+    def GetBarToggleButtonArea(self, rect: 'Rect') -> 'Rect':
         """ Calculate the position and size of the ribbonâs toggle button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
     def GetButtonBarButtonSize(self, dc, wnd, kind, size, label, text_min_width, bitmap_size_large, bitmap_size_small, button_size, normal_region, dropdown_region) -> bool:
         """ Calculate the size of a button within a   wx.ribbon.RibbonButtonBar.
@@ -1891,15 +1899,15 @@
 
     def GetButtonBarButtonTextWidth(self, dc, label, kind, size) -> 'Coord':
         """ Gets the width of the string if it is used as a   wx.ribbon.RibbonButtonBar  button label.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetColour(self, id: int) -> Colour:
+    def GetColour(self, id: int) -> 'Colour':
         """ Get the value of a certain colour setting.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
     def GetColourScheme(self) -> tuple:
         """ Get the current colour scheme.
@@ -1909,87 +1917,87 @@
 
     def GetFlags(self) -> int:
         """ Get the previously set style flags.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetFont(self, id: int) -> Font:
+    def GetFont(self, id: int) -> 'Font':
         """ Get the value of a certain font setting.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetGalleryClientSize(self, dc, wnd, size, client_offset, scroll_up_button, scroll_down_button, extension_button) -> Size:
+    def GetGalleryClientSize(self, dc, wnd, size, client_offset, scroll_up_button, scroll_down_button, extension_button) -> 'Size':
         """ Calculate the client size of a   wx.ribbon.RibbonGallery  control for a given size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetGallerySize(self, dc, wnd, client_size) -> Size:
+    def GetGallerySize(self, dc, wnd, client_size) -> 'Size':
         """ Calculate the size of a   wx.ribbon.RibbonGallery  control for a given client size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
     def GetMetric(self, id: int) -> int:
         """ Get the value of a certain integer setting.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetMinimisedPanelMinimumSize(self, dc, wnd, desired_bitmap_size, expanded_panel_direction) -> Size:
+    def GetMinimisedPanelMinimumSize(self, dc, wnd, desired_bitmap_size, expanded_panel_direction) -> 'Size':
         """ Calculate the size of a minimised ribbon panel.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetPageBackgroundRedrawArea(self, dc, wnd, page_old_size, page_new_size) -> Rect:
+    def GetPageBackgroundRedrawArea(self, dc, wnd, page_old_size, page_new_size) -> 'Rect':
         """ Calculate the portion of a page background which needs to be redrawn when a page is resized.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetPanelClientSize(self, dc, wnd, size, client_offset) -> Size:
+    def GetPanelClientSize(self, dc, wnd, size, client_offset) -> 'Size':
         """ Calculate the client size of a panel for a given overall size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetPanelExtButtonArea(self, dc, wnd, rect) -> Rect:
+    def GetPanelExtButtonArea(self, dc, wnd, rect) -> 'Rect':
         """ Calculate the position and size of the panel extension button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetPanelSize(self, dc, wnd, client_size, client_offset) -> Size:
+    def GetPanelSize(self, dc, wnd, client_size, client_offset) -> 'Size':
         """ Calculate the size of a panel for a given client size.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetRibbonHelpButtonArea(self, rect: 'Rect') -> Rect:
+    def GetRibbonHelpButtonArea(self, rect: 'Rect') -> 'Rect':
         """ Calculate the position and size of the ribbonâs help button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetScrollButtonMinimumSize(self, dc, wnd, style) -> Size:
+    def GetScrollButtonMinimumSize(self, dc, wnd, style) -> 'Size':
         """ Calculate the minimum size (in pixels) of a scroll button.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
     def GetTabCtrlHeight(self, dc, wnd, pages) -> int:
         """ Calculate the height (in pixels) of the tab region of a ribbon bar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
-    def GetToolSize(self, dc, wnd, bitmap_size, kind, is_first, is_last, dropdown_region) -> Size:
+    def GetToolSize(self, dc, wnd, bitmap_size, kind, is_first, is_last, dropdown_region) -> 'Size':
         """ Calculate the size of a tool within a   wx.ribbon.RibbonToolBar.
 
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
     def SetColour(self, id, colour) -> None:
         """ Set the value of a certain colour setting to the value colour.
@@ -2021,14 +2029,16 @@
             Source: https://docs.wxpython.org/wx.ribbon.RibbonMSWArtProvider.html
         """
 
     Flags: int  # See GetFlags and SetFlags
 
 
 
+RibbonScrollButtonStyle: TypeAlias = int  # Enumeration
+
 RIBBON_SCROLL_BTN_LEFT: int
 
 RIBBON_SCROLL_BTN_RIGHT: int
 
 RIBBON_SCROLL_BTN_UP: int
 
 RIBBON_SCROLL_BTN_DOWN: int
@@ -2065,14 +2075,16 @@
     rect: Any  # A public C++ attribute of type Rect     .
     shown: Any  # A public C++ attribute of type bool.
     small_begin_need_separator_width: Any  # A public C++ attribute of type int.
     small_must_have_separator_width: Any  # A public C++ attribute of type int.
 
 
 
+RibbonArtSetting: TypeAlias = int  # Enumeration
+
 RIBBON_ART_TAB_SEPARATION_SIZE: int
 
 RIBBON_ART_PAGE_BORDER_LEFT_SIZE: int
 
 RIBBON_ART_PAGE_BORDER_TOP_SIZE: int
 
 RIBBON_ART_PAGE_BORDER_RIGHT_SIZE: int
@@ -2273,7 +2285,13 @@
 
 RIBBON_ART_BUTTON_BAR_LABEL_HIGHLIGHT_GRADIENT_COLOUR: int
 
 RIBBON_ART_BUTTON_BAR_LABEL_HIGHLIGHT_TOP_COLOUR: int
 
 RIBBON_ART_BUTTON_BAR_LABEL_HIGHLIGHT_GRADIENT_TOP_COLOUR: int
 
+RibbonButtonBarButtonBase: TypeAlias = Any
+
+RibbonToolBarToolBase: TypeAlias = Any
+
+RibbonGalleryItem: TypeAlias = Any
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/richtext/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/richtext/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class RichTextCtrl(Control):
     """ RichTextCtrl provides a generic, ground-up implementation of a text
 control capable of showing multiple styles and images.
 
         Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
     """
@@ -346,15 +346,15 @@
 
     def DiscardEdits(self) -> None:
         """ Sets the bufferâs modified status to False, and clears the bufferâs command history.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def DoGetBestSize(self) -> Size:
+    def DoGetBestSize(self) -> 'Size':
         """ Currently this simply returns    wx.Size.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def DoGetValue(self) -> str:
         """ string
@@ -654,27 +654,27 @@
     def GetCaretPositionForIndex(self, position, rect, container=None) -> None:
         """ Returns the caret height and position for the given character position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetCommandProcessor(self) -> CommandProcessor:
+    def GetCommandProcessor(self) -> 'CommandProcessor':
         """ Gets the command processor associated with the controlâs buffer.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetContextMenu(self) -> Menu:
+    def GetContextMenu(self) -> 'Menu':
         """ Returns the current context menu.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def GetContextMenuPropertiesInfo(self) -> 'richtext.RichTextContextMenuPropertiesInfo':
         """ Returns an object that stores information about context menu property item(s), in order to communicate between the context menu event handler and the code that responds to it.
@@ -714,21 +714,21 @@
 
     def GetDimensionScale(self) -> float:
         """ Returns the scale factor for displaying certain dimensions such as indentation and inter-paragraph spacing.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetDragStartPoint(self) -> Point:
+    def GetDragStartPoint(self) -> 'Point':
         """ Get the possible DragânâDrop start point.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetDragStartTime(self) -> DateTime:
+    def GetDragStartTime(self) -> 'DateTime':
         """ Get the possible DragânâDrop start time.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def GetDragging(self) -> bool:
         """ Returns True if we are extending a selection.
@@ -738,15 +738,15 @@
 
     def GetFilename(self) -> str:
         """ Gets the current filename associated with the control.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetFirstVisiblePoint(self) -> Point:
+    def GetFirstVisiblePoint(self) -> 'Point':
         """ Returns the first visible point in the window.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def GetFirstVisiblePosition(self) -> int:
         """ Returns the first visible position in the current view.
@@ -828,15 +828,15 @@
 
     def GetLineText(self, lineNo: int) -> str:
         """ Returns the text for the given line.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetLogicalPoint(self, ptPhysical: Union[tuple[int, int], 'Point']) -> Point:
+    def GetLogicalPoint(self, ptPhysical: Union[tuple[int, int], 'Point']) -> 'Point':
         """ Transforms physical window position to logical (unscrolled) position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def GetMargins(self) -> 'Point':
         """ Returns the margins used by the control.
@@ -846,15 +846,15 @@
 
     def GetNumberOfLines(self) -> int:
         """ Returns the number of lines in the buffer.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetPhysicalPoint(self, ptLogical: Union[tuple[int, int], 'Point']) -> Point:
+    def GetPhysicalPoint(self, ptLogical: Union[tuple[int, int], 'Point']) -> 'Point':
         """ Transforms logical (unscrolled) position to physical window position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def GetPreDrag(self) -> bool:
         """ Are we trying to start DragânâDrop?
@@ -876,27 +876,27 @@
 
     def GetScale(self) -> float:
         """ Returns an overall scale factor for displaying and editing the content.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetScaledPoint(self, pt: Union[tuple[int, int], 'Point']) -> Point:
+    def GetScaledPoint(self, pt: Union[tuple[int, int], 'Point']) -> 'Point':
         """ Returns a scaled point.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetScaledRect(self, rect: 'Rect') -> Rect:
+    def GetScaledRect(self, rect: 'Rect') -> 'Rect':
         """ Returns a scaled rectangle.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetScaledSize(self, sz: Union[tuple[int, int], 'Size']) -> Size:
+    def GetScaledSize(self, sz: Union[tuple[int, int], 'Size']) -> 'Size':
         """ Returns a scaled size.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def GetSelection(self) -> 'richtext.RichTextSelection':
         """ Returns the range of the current selection.
@@ -942,45 +942,45 @@
 
     def GetStyleSheet(self) -> 'richtext.RichTextStyleSheet':
         """ Returns the style sheet associated with the control, if any.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetTextCursor(self) -> Cursor:
+    def GetTextCursor(self) -> 'Cursor':
         """ Returns the text (normal) cursor.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetURLCursor(self) -> Cursor:
+    def GetURLCursor(self) -> 'Cursor':
         """ Returns the cursor to be used over URLs.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def GetUncombinedStyle(self, *args, **kw) -> None:
         """ Gets the attributes at the given position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetUnscaledPoint(self, pt: Union[tuple[int, int], 'Point']) -> Point:
+    def GetUnscaledPoint(self, pt: Union[tuple[int, int], 'Point']) -> 'Point':
         """ Returns an unscaled point.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetUnscaledRect(self, rect: 'Rect') -> Rect:
+    def GetUnscaledRect(self, rect: 'Rect') -> 'Rect':
         """ Returns an unscaled rectangle.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
-    def GetUnscaledSize(self, sz: Union[tuple[int, int], 'Size']) -> Size:
+    def GetUnscaledSize(self, sz: Union[tuple[int, int], 'Size']) -> 'Size':
         """ Returns an unscaled size.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCtrl.html
         """
 
     def GetValue(self) -> str:
         """ Returns the content of the entire control as a string.
@@ -1973,29 +1973,29 @@
         """
 
     BasicStyle: 'richtext.RichTextAttr'  # See GetBasicStyle and SetBasicStyle
     Buffer: 'richtext.RichTextBuffer'  # See GetBuffer
     CaretAtLineStart: bool  # See GetCaretAtLineStart and SetCaretAtLineStart
     CaretPosition: int  # See GetCaretPosition and SetCaretPosition
     CaretPositionForDefaultStyle: int  # See GetCaretPositionForDefaultStyle and SetCaretPositionForDefaultStyle
-    CommandProcessor: CommandProcessor  # See GetCommandProcessor
+    CommandProcessor: '_CommandProcessor'  # See GetCommandProcessor
     ContextMenu: 'Menu'  # See GetContextMenu and SetContextMenu
     ContextMenuPropertiesInfo: 'richtext.RichTextContextMenuPropertiesInfo'  # See GetContextMenuPropertiesInfo
-    DefaultStyle: 'TextAttr'  # See GetDefaultStyle and SetDefaultStyle
+    DefaultStyle: Any  # See GetDefaultStyle and SetDefaultStyle
     DefaultStyleEx: 'richtext.RichTextAttr'  # See GetDefaultStyleEx
     DelayedImageLoading: bool  # See GetDelayedImageLoading
     DelayedImageProcessingRequired: bool  # See GetDelayedImageProcessingRequired and SetDelayedImageProcessingRequired
     DelayedImageProcessingTime: int  # See GetDelayedImageProcessingTime and SetDelayedImageProcessingTime
     DelayedLayoutThreshold: int  # See GetDelayedLayoutThreshold and SetDelayedLayoutThreshold
     DimensionScale: float  # See GetDimensionScale and SetDimensionScale
-    DragStartPoint: Union[tuple[int, int], 'Point']  # See GetDragStartPoint and SetDragStartPoint
+    DragStartPoint: 'Point'  # See GetDragStartPoint and SetDragStartPoint
     DragStartTime: 'DateTime'  # See GetDragStartTime and SetDragStartTime
     Dragging: bool  # See GetDragging and SetDragging
     Filename: str  # See GetFilename and SetFilename
-    FirstVisiblePoint: Point  # See GetFirstVisiblePoint
+    FirstVisiblePoint: 'Point'  # See GetFirstVisiblePoint
     FirstVisiblePosition: int  # See GetFirstVisiblePosition
     FocusObject: 'richtext.RichTextParagraphLayoutBox'  # See GetFocusObject and SetFocusObject
     FontScale: float  # See GetFontScale and SetFontScale
     FullLayoutRequired: bool  # See GetFullLayoutRequired and SetFullLayoutRequired
     FullLayoutSavedPosition: int  # See GetFullLayoutSavedPosition and SetFullLayoutSavedPosition
     FullLayoutTime: int  # See GetFullLayoutTime and SetFullLayoutTime
     HandlerFlags: int  # See GetHandlerFlags and SetHandlerFlags
@@ -2092,15 +2092,15 @@
     def Create(self, parent, id=ID_ANY, pos=DefaultPosition, size=DefaultSize, style=0) -> bool:
         """ Creates the windows.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleComboCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleComboCtrl.html
         """
 
     def GetRichTextCtrl(self) -> 'richtext.RichTextCtrl':
         """ Returns the   wx.richtext.RichTextCtrl  associated with this control.
@@ -2162,27 +2162,27 @@
 
     def Do(self) -> bool:
         """ Performs the command.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCommand.html
         """
 
-    def GetActions(self) -> RichTextActionList:
+    def GetActions(self) -> 'richtext.RichTextActionList':
         """ Returns the action list.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCommand.html
         """
 
     def Undo(self) -> bool:
         """ Undoes the command.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCommand.html
         """
 
-    Actions: RichTextActionList  # See GetActions
+    Actions: 'richtext.RichTextActionList'  # See GetActions
 
 
 
 class RichTextStyleListCtrl(Control):
     """ This class incorporates a RichTextStyleListBox and a choice control
 that allows the user to select the category of style to view.
 
@@ -2197,27 +2197,27 @@
     def Create(self, parent, id=ID_ANY, pos=DefaultPosition, size=DefaultSize, style=0) -> bool:
         """ Creates the windows.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListCtrl.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListCtrl.html
         """
 
     def GetRichTextCtrl(self) -> 'richtext.RichTextCtrl':
         """ Returns the associated rich text control, if any.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListCtrl.html
         """
 
-    def GetStyleChoice(self) -> Choice:
+    def GetStyleChoice(self) -> 'Choice':
         """ Returns the   wx.Choice  control used for selecting the style category.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListCtrl.html
         """
 
     def GetStyleListBox(self) -> 'richtext.RichTextStyleListBox':
         """ Returns the   wx.ListBox  control used to view the style list.
@@ -2227,15 +2227,15 @@
 
     def GetStyleSheet(self) -> 'richtext.RichTextStyleSheet':
         """ Returns the associated style sheet, if any.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListCtrl.html
         """
 
-    def GetStyleType(self) -> 'richtext.RichTextStyleListBox.wxRichTextStyleType':
+    def GetStyleType(self) -> 'richtext.wxRichTextStyleType':
         """ Returns the type of style to show in the list box.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListCtrl.html
         """
 
     def SetRichTextCtrl(self, ctrl: 'richtext.RichTextCtrl') -> None:
         """ Associates the control with a   wx.richtext.RichTextCtrl.
@@ -2258,18 +2258,18 @@
     def UpdateStyles(self) -> None:
         """ Updates the style list box.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListCtrl.html
         """
 
     RichTextCtrl: 'richtext.RichTextCtrl'  # See GetRichTextCtrl and SetRichTextCtrl
-    StyleChoice: Choice  # See GetStyleChoice
+    StyleChoice: 'Choice'  # See GetStyleChoice
     StyleListBox: 'richtext.RichTextStyleListBox'  # See GetStyleListBox
     StyleSheet: 'richtext.RichTextStyleSheet'  # See GetStyleSheet and SetStyleSheet
-    StyleType: RichTextStyleListBox.wxRichTextStyleType  # See GetStyleType and SetStyleType
+    StyleType: 'richtext.wxRichTextStyleType'  # See GetStyleType and SetStyleType
 
 
 
 RICHTEXTSTYLELIST_HIDE_TYPE_SELECTOR: int  # This style hides the category selection control. ^^
 
 class RichTextBufferDataObject(DataObjectSimple):
     """ Implements a rich text data object for clipboard transfer.
@@ -2290,15 +2290,15 @@
 
     def GetDataSize(self, *args, **kw) -> int:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBufferDataObject.html
         """
 
-    def GetPreferredFormat(self, dir: int) -> DataFormat:
+    def GetPreferredFormat(self, dir: int) -> 'DataFormat':
         """ Returns the preferred format for either rendering the data (if dir  is  Get , its default value) or for setting it.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBufferDataObject.html
         """
 
     def GetRichTextBuffer(self) -> 'richtext.RichTextBuffer':
         """ After a call to this function, the buffer is owned by the caller and it is responsible for deleting it.
@@ -2345,15 +2345,15 @@
     def Create(*args, **kwargs) -> bool:
         """ Creates the dialog.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleOrganiserDialog.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleOrganiserDialog.html
         """
 
     def GetFlags(self) -> int:
         """ Returns the flags used to control the interface presented to the user.
@@ -2476,15 +2476,15 @@
     def Create(*args, **kwargs) -> bool:
         """ Creation: see the constructor  for details about the parameters.
 
             Source: https://docs.wxpython.org/wx.richtext.SymbolPickerDialog.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.richtext.SymbolPickerDialog.html
         """
 
     def GetFontName(self) -> str:
         """ Returns the font name (the font reflected in the font list).
@@ -2573,15 +2573,15 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextEvent.html
         """
 
-    def Clone(self) -> Event:
+    def Clone(self) -> 'Event':
         """ Returns a copy of the event.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextEvent.html
         """
 
     def GetCharacter(self) -> 'Char':
         """ Returns the character pressed, within a  wxEVT_RICHTEXT_CHARACTER   event.
@@ -3299,15 +3299,15 @@
 
     def Clear(self) -> None:
         """ Clears the font table.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFontTable.html
         """
 
-    def FindFont(self, fontSpec: 'richtext.RichTextAttr') -> Font:
+    def FindFont(self, fontSpec: 'richtext.RichTextAttr') -> 'Font':
         """ Finds a font for the given attribute object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFontTable.html
         """
 
     def IsOk(self) -> bool:
         """ Returns True if the font table is valid.
@@ -3349,15 +3349,15 @@
 
     def CreateButtons(self, dialog: 'richtext.RichTextFormattingDialog') -> bool:
         """ Creates the main dialog buttons.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialogFactory.html
         """
 
-    def CreatePage(self, page, title, dialog) -> Panel:
+    def CreatePage(self, page, title, dialog) -> 'Panel':
         """ Creates a page, given a page identifier.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialogFactory.html
         """
 
     def CreatePages(self, pages, dialog) -> bool:
         """ Creates all pages under the dialogâs book control, also calling AddPage().
@@ -3419,15 +3419,15 @@
 
     def Copy(self, data: 'richtext.RichTextHeaderFooterData') -> None:
         """ Copies the data.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextHeaderFooterData.html
         """
 
-    def GetFont(self) -> Font:
+    def GetFont(self) -> 'Font':
         """ Returns the font specified for printing the header and footer.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextHeaderFooterData.html
         """
 
     def GetFooterMargin(self) -> int:
         """ Returns the margin between the text and the footer.
@@ -3461,15 +3461,15 @@
 
     def GetText(self, headerFooter, page, location) -> str:
         """ Helper function for getting the header or footer text, odd or even pages, and at a given position on the page (left, centre or right).
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextHeaderFooterData.html
         """
 
-    def GetTextColour(self) -> Colour:
+    def GetTextColour(self) -> 'Colour':
         """ Returns the text colour for drawing the header and footer.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextHeaderFooterData.html
         """
 
     def Init(self) -> None:
         """ Initialises the object.
@@ -3515,21 +3515,21 @@
 
     def SetTextColour(self, col: Union[int, str, 'Colour']) -> None:
         """ Sets the text colour for drawing the header and footer.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextHeaderFooterData.html
         """
 
-    Font: 'Font'  # See GetFont and SetFont
+    Font: '_Font'  # See GetFont and SetFont
     FooterMargin: int  # See GetFooterMargin
     FooterText: str  # See GetFooterText and SetFooterText
     HeaderMargin: int  # See GetHeaderMargin
     HeaderText: str  # See GetHeaderText and SetHeaderText
     ShowOnFirstPage: bool  # See GetShowOnFirstPage and SetShowOnFirstPage
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
 
 
 
 class RichTextImageBlock(Object):
     """ This class stores information about an image, in binary in-memory
 form.
 
@@ -3668,15 +3668,15 @@
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextImageBlock.html
         """
 
     Data: int  # See GetData and SetData
     DataSize: int  # See GetDataSize and SetDataSize
     Extension: str  # See GetExtension
-    ImageType: BitmapType  # See GetImageType and SetImageType
+    ImageType: 'BitmapType'  # See GetImageType and SetImageType
 
 
 
 class RichTextObject(Object):
     """ This is the base for drawable rich text objects.
 
         Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
@@ -3696,21 +3696,21 @@
     def AdjustAttributes(self, attr, context) -> bool:
         """ Adjusts the attributes for virtual attribute provision, collapsed borders, etc.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
     @staticmethod
-    def AdjustAvailableSpace(dc, buffer, parentAttr, childAttr, availableParentSpace, availableContainerSpace) -> Rect:
+    def AdjustAvailableSpace(dc, buffer, parentAttr, childAttr, availableParentSpace, availableContainerSpace) -> 'Rect':
         """ Returns the rectangle which the child has available to it given restrictions specified in the child attribute, e.g.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def CalculateRange(self, start: int) -> end:
+    def CalculateRange(self, start: int) -> None:
         """ Calculates the range of the object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
     def CanEditProperties(self) -> bool:
         """ Returns True if we can edit the objectâs properties via a GUI.
@@ -3800,33 +3800,33 @@
 
     def FindPosition(self, dc, context, index, forceLineStart) -> tuple:
         """ Finds the absolute position and row height for the given character position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def GetAbsolutePosition(self) -> Point:
+    def GetAbsolutePosition(self) -> 'Point':
         """ Returns the absolute object position, by traversing up the child/parent hierarchy.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
     def GetAttributes(self) -> 'richtext.RichTextAttr':
         """ Returns the objectâs attributes.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def GetAvailableContentArea(self, dc, context, outerRect) -> Rect:
+    def GetAvailableContentArea(self, dc, context, outerRect) -> 'Rect':
         """ Calculates the available content space in the given rectangle, given the margins, border and padding specified in the objectâs attributes.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def GetBestSize(self) -> Size:
+    def GetBestSize(self) -> 'Size':
         """ Returns the best size, i.e. the ideal starting size for this object irrespective of available space.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
     def GetBottomMargin(self) -> int:
         """ Returns the bottom margin of the object, in pixels.
@@ -3843,15 +3843,15 @@
 
     def GetBuffer(self) -> 'richtext.RichTextBuffer':
         """ Returns the containing buffer.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def GetCachedSize(self) -> Size:
+    def GetCachedSize(self) -> 'Size':
         """ Gets the cached object size as calculated by Layout.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
     def GetContainer(self) -> 'richtext.RichTextParagraphLayoutBox':
         """ Returns the top-level container of this object.
@@ -3873,21 +3873,21 @@
 
     def GetLeftMargin(self) -> int:
         """ Returns the left margin of the object, in pixels.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def GetMaxSize(self) -> Size:
+    def GetMaxSize(self) -> 'Size':
         """ Gets the maximum object size as calculated by Layout.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def GetMinSize(self) -> Size:
+    def GetMinSize(self) -> 'Size':
         """ Gets the minimum object size as calculated by Layout.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
     def GetName(self) -> str:
         """ Returns the identifying name for this object from the properties, using the ânameâ key.
@@ -3921,15 +3921,15 @@
 
     def GetParentContainer(self) -> 'richtext.RichTextParagraphLayoutBox':
         """ Returns the top-level container of this object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def GetPosition(self) -> Point:
+    def GetPosition(self) -> 'Point':
         """ Returns the object position in pixels.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
     def GetProperties(self) -> 'richtext.RichTextProperties':
         """ Returns the objectâs properties.
@@ -3951,15 +3951,15 @@
 
     def GetRangeSize(*args, **kwargs) -> bool:
         """ Returns the object size for the given range.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    def GetRect(self) -> Rect:
+    def GetRect(self) -> 'Rect':
         """ Returns the rectangle enclosing the object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
     def GetRightMargin(self) -> int:
         """ Returns the right margin of the object, in pixels.
@@ -4180,37 +4180,37 @@
 
     def UsesParagraphAttributes(self) -> bool:
         """ Returns True if this object takes note of paragraph attributes (text and image objects donât).
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextObject.html
         """
 
-    AbsolutePosition: Point  # See GetAbsolutePosition
+    AbsolutePosition: 'Point'  # See GetAbsolutePosition
     Attributes: 'richtext.RichTextAttr'  # See GetAttributes and SetAttributes
-    BestSize: Size  # See GetBestSize
+    BestSize: 'Size'  # See GetBestSize
     BottomMargin: int  # See GetBottomMargin
     Buffer: 'richtext.RichTextBuffer'  # See GetBuffer
-    CachedSize: Union[tuple[int, int], 'Size']  # See GetCachedSize and SetCachedSize
+    CachedSize: 'Size'  # See GetCachedSize and SetCachedSize
     Container: 'richtext.RichTextParagraphLayoutBox'  # See GetContainer
     Descent: int  # See GetDescent and SetDescent
     FloatDirection: int  # See GetFloatDirection
     LeftMargin: int  # See GetLeftMargin
-    MaxSize: Union[tuple[int, int], 'Size']  # See GetMaxSize and SetMaxSize
-    MinSize: Union[tuple[int, int], 'Size']  # See GetMinSize and SetMinSize
+    MaxSize: 'Size'  # See GetMaxSize and SetMaxSize
+    MinSize: 'Size'  # See GetMinSize and SetMinSize
     Name: str  # See GetName and SetName
     NaturalSize: 'richtext.TextAttrSize'  # See GetNaturalSize
     OwnRange: 'richtext.RichTextRange'  # See GetOwnRange and SetOwnRange
     OwnRangeIfTopLevel: 'richtext.RichTextRange'  # See GetOwnRangeIfTopLevel
     Parent: 'richtext.RichTextObject'  # See GetParent and SetParent
     ParentContainer: 'richtext.RichTextParagraphLayoutBox'  # See GetParentContainer
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
+    Position: 'Point'  # See GetPosition and SetPosition
     Properties: 'richtext.RichTextProperties'  # See GetProperties and SetProperties
     PropertiesMenuLabel: str  # See GetPropertiesMenuLabel
     Range: 'richtext.RichTextRange'  # See GetRange and SetRange
-    Rect: Rect  # See GetRect
+    Rect: '_Rect'  # See GetRect
     RightMargin: int  # See GetRightMargin
     TopMargin: int  # See GetTopMargin
     XMLNodeName: str  # See GetXMLNodeName
 
 
 
 class RichTextPrinting(Object):
@@ -4239,33 +4239,33 @@
 
     def GetHeaderText(self, page=RICHTEXT_PAGE_EVEN, location=RICHTEXT_PAGE_CENTRE) -> str:
         """ A convenience function to get the header text.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextPrinting.html
         """
 
-    def GetPageSetupData(self) -> PageSetupDialogData:
+    def GetPageSetupData(self) -> 'PageSetupDialogData':
         """ Returns a pointer to the internal page setup data.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextPrinting.html
         """
 
-    def GetParentWindow(self) -> Window:
+    def GetParentWindow(self) -> 'Window':
         """ Returns the parent window to be used for the preview window and printing wait dialog.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextPrinting.html
         """
 
-    def GetPreviewRect(self) -> Rect:
+    def GetPreviewRect(self) -> 'Rect':
         """ Returns the dimensions to be used for the preview window.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextPrinting.html
         """
 
-    def GetPrintData(self) -> PrintData:
+    def GetPrintData(self) -> 'PrintData':
         """ Returns a pointer to the internal print data.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextPrinting.html
         """
 
     def GetTitle(self) -> str:
         """ Returns the title of the preview window or printing wait caption.
@@ -4371,15 +4371,15 @@
 
     FooterText: str  # See GetFooterText and SetFooterText
     HeaderFooterData: 'richtext.RichTextHeaderFooterData'  # See GetHeaderFooterData and SetHeaderFooterData
     HeaderText: str  # See GetHeaderText and SetHeaderText
     PageSetupData: 'PageSetupDialogData'  # See GetPageSetupData and SetPageSetupData
     ParentWindow: 'Window'  # See GetParentWindow and SetParentWindow
     PreviewRect: 'Rect'  # See GetPreviewRect and SetPreviewRect
-    PrintData: 'PrintData'  # See GetPrintData and SetPrintData
+    PrintData: '_PrintData'  # See GetPrintData and SetPrintData
     Title: str  # See GetTitle and SetTitle
 
 
 
 class RichTextProperties(Object):
     """ A simple property class using Variants.
 
@@ -4405,33 +4405,33 @@
 
     def Find(self, name: str) -> int:
         """ Finds the given property.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextProperties.html
         """
 
-    def FindOrCreateProperty(self, name: str) -> Variant:
+    def FindOrCreateProperty(self, name: str) -> Any:
         """ Finds or creates a property with the given name, returning a pointer to the variant.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextProperties.html
         """
 
     def GetCount(self) -> int:
         """ Returns a count of the properties.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextProperties.html
         """
 
-    def GetProperties(self) -> RichTextVariantArray:
+    def GetProperties(self) -> 'richtext.RichTextVariantArray':
         """ Returns the array of variants implementing the properties.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextProperties.html
         """
 
-    def GetProperty(self, name: str) -> Variant:
+    def GetProperty(self, name: str) -> Any:
         """ Gets the property variant by name.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextProperties.html
         """
 
     def GetPropertyBool(self, name: str) -> bool:
         """ Gets the value of the named property as a boolean.
@@ -4489,28 +4489,28 @@
 
     def SetProperties(self, props: RichTextVariantArray) -> None:
         """ Sets the array of variants.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextProperties.html
         """
 
-    def SetProperty(self, *args, **kw) -> None:
+    def SetProperty(self, props: Any) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextProperties.html
         """
 
     def __eq__(self, item: Any) -> bool:
         """ Equality operator.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextProperties.html
         """
 
     Count: int  # See GetCount
-    Properties: RichTextVariantArray  # See GetProperties and SetProperties
+    Properties: 'richtext.RichTextVariantArray'  # See GetProperties and SetProperties
     PropertyNames: list[str]  # See GetPropertyNames
 
 
 
 class RichTextRenderer(Object):
     """ This class isolates some common drawing functionality.
 
@@ -5430,28 +5430,28 @@
     @staticmethod
     def GetBulletRightMargin() -> int:
         """ Returns the minimum margin between bullet and paragraph in 10ths of a mm.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBuffer.html
         """
 
-    def GetCommandProcessor(self) -> CommandProcessor:
+    def GetCommandProcessor(self) -> 'CommandProcessor':
         """ Returns the command processor.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBuffer.html
         """
 
     def GetDimensionScale(self) -> float:
         """ Returns the scale factor for displaying certain dimensions such as indentation and inter-paragraph spacing.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBuffer.html
         """
 
     @staticmethod
-    def GetDrawingHandlers() -> RichTextDrawingHandlerList:
+    def GetDrawingHandlers() -> list['richtext.RichTextDrawingHandler']:
         """ Returns the drawing handlers.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBuffer.html
         """
 
     @staticmethod
     def GetExtWildcard(combine=False, save=False) -> Any:
@@ -5484,15 +5484,15 @@
     def GetHandlerFlags(self) -> int:
         """ Gets the handler flags, controlling loading and saving.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBuffer.html
         """
 
     @staticmethod
-    def GetHandlers() -> RichTextFileHandlerList:
+    def GetHandlers() -> list['richtext.RichTextFileHandler']:
         """ Returns the file handlers.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBuffer.html
         """
 
     @staticmethod
     def GetRenderer() -> 'richtext.RichTextRenderer':
@@ -5742,15 +5742,15 @@
     def SuppressingUndo(self) -> bool:
         """ Are we suppressing undo??
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextBuffer.html
         """
 
     BatchedCommand: 'richtext.RichTextCommand'  # See GetBatchedCommand
-    CommandProcessor: CommandProcessor  # See GetCommandProcessor
+    CommandProcessor: '_CommandProcessor'  # See GetCommandProcessor
     DimensionScale: float  # See GetDimensionScale and SetDimensionScale
     FontScale: float  # See GetFontScale and SetFontScale
     FontTable: 'richtext.RichTextFontTable'  # See GetFontTable and SetFontTable
     HandlerFlags: int  # See GetHandlerFlags and SetHandlerFlags
     Scale: float  # See GetScale and SetScale
     StyleSheet: 'richtext.RichTextStyleSheet'  # See GetStyleSheet and SetStyleSheet
     StyleStackSize: int  # See GetStyleStackSize
@@ -6069,15 +6069,15 @@
 
     def GetDefaultStyle(self) -> 'richtext.RichTextAttr':
         """ Returns the current default style, affecting the style currently being applied (for example, setting the default style to bold will cause subsequently inserted text to be bold).
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraphLayoutBox.html
         """
 
-    def GetFloatCollector(self) -> RichTextFloatCollector:
+    def GetFloatCollector(self) -> 'richtext.RichTextFloatCollector':
         """ Returns the RichTextFloatCollector of this object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraphLayoutBox.html
         """
 
     def GetFloatingObjectCount(self) -> int:
         """ Returns the number of floating objects at this level.
@@ -6123,15 +6123,15 @@
 
     def GetLineForVisibleLineNumber(self, lineNumber: int) -> 'richtext.RichTextLine':
         """ Given a line number, returns the corresponding   wx.richtext.RichTextLine  object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraphLayoutBox.html
         """
 
-    def GetLineSizeAtPosition(self, pos, caretPosition=False) -> Size:
+    def GetLineSizeAtPosition(self, pos, caretPosition=False) -> 'Size':
         """ Returns the line size at the given position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraphLayoutBox.html
         """
 
     def GetParagraphAtLine(self, paragraphNumber: int) -> 'richtext.RichTextParagraph':
         """ Returns the paragraph by number.
@@ -6443,15 +6443,15 @@
         """ Converts zero-based line column and paragraph number to a position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraphLayoutBox.html
         """
 
     BasicStyle: 'richtext.RichTextAttr'  # See GetBasicStyle and SetBasicStyle
     DefaultStyle: 'richtext.RichTextAttr'  # See GetDefaultStyle and SetDefaultStyle
-    FloatCollector: RichTextFloatCollector  # See GetFloatCollector
+    FloatCollector: 'richtext.RichTextFloatCollector'  # See GetFloatCollector
     FloatingObjectCount: int  # See GetFloatingObjectCount
     InvalidRange: 'richtext.RichTextRange'  # See GetInvalidRange
     LineCount: int  # See GetLineCount
     ParagraphCount: int  # See GetParagraphCount
     PartialParagraph: bool  # See GetPartialParagraph and SetPartialParagraph
     RichTextCtrl: 'richtext.RichTextCtrl'  # See GetRichTextCtrl and SetRichTextCtrl
     StyleSheet: 'richtext.RichTextStyleSheet'  # See GetStyleSheet
@@ -6487,15 +6487,15 @@
 
     def AddRows(*args, **kwargs) -> bool:
         """ Adds rows from the given row position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextTable.html
         """
 
-    def CalculateRange(self, start: int) -> end:
+    def CalculateRange(self, start: int) -> None:
         """ Calculates the range of the object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextTable.html
         """
 
     def CanEditProperties(self) -> bool:
         """ Returns True if we can edit the objectâs properties via a GUI.
@@ -6571,27 +6571,27 @@
 
     def GetCellRowColumnPosition(self, pos, row, col) -> bool:
         """ Returns the row/column for a given character position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextTable.html
         """
 
-    def GetCells(self) -> RichTextObjectPtrArrayArray:
+    def GetCells(self) -> 'richtext.RichTextObjectPtrArrayArray':
         """ Returns the cells array.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextTable.html
         """
 
     def GetColumnCount(self) -> int:
         """ Returns the column count.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextTable.html
         """
 
-    def GetFocusedCell(self) -> Position:
+    def GetFocusedCell(self) -> 'Position':
         """ Returns the coordinates of the cell with keyboard focus, or (-1,-1) if none.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextTable.html
         """
 
     def GetPropertiesMenuLabel(self) -> str:
         """ Returns the label to be used for the properties context menu item.
@@ -6655,17 +6655,17 @@
 
     def SetCellStyle(self, selection, style, flags=RICHTEXT_SETSTYLE_WITH_UNDO) -> bool:
         """ Sets the attributes for the cells specified by the selection.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextTable.html
         """
 
-    Cells: RichTextObjectPtrArrayArray  # See GetCells
+    Cells: 'richtext.RichTextObjectPtrArrayArray'  # See GetCells
     ColumnCount: int  # See GetColumnCount
-    FocusedCell: Position  # See GetFocusedCell
+    FocusedCell: 'Position'  # See GetFocusedCell
     PropertiesMenuLabel: str  # See GetPropertiesMenuLabel
     RowCount: int  # See GetRowCount
     XMLNodeName: str  # See GetXMLNodeName
 
 
 
 class RichTextContextMenuPropertiesInfo:
@@ -6724,29 +6724,29 @@
 
     def GetObject(self, n: int) -> 'richtext.RichTextObject':
         """ Returns the nth object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextContextMenuPropertiesInfo.html
         """
 
-    def GetObjects(self) -> RichTextObjectPtrArray:
+    def GetObjects(self) -> 'richtext.RichTextObjectPtrArray':
         """ Returns the array of objects.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextContextMenuPropertiesInfo.html
         """
 
     def Init(self) -> None:
         """ Initialisation.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextContextMenuPropertiesInfo.html
         """
 
     Count: int  # See GetCount
     Labels: list[str]  # See GetLabels
-    Objects: RichTextObjectPtrArray  # See GetObjects
+    Objects: 'richtext.RichTextObjectPtrArray'  # See GetObjects
     m_labels: Any  # A public C++ attribute of type list of strings.
     m_objects: Any  # A public C++ attribute of type RichTextObjectPtrArray.
 
 
 
 class RichTextSelection:
     """ Stores selection information.
@@ -6785,21 +6785,21 @@
 
     def GetRange(self, *args, **kw) -> 'richtext.RichTextRange':
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextSelection.html
         """
 
-    def GetRanges(self) -> RichTextRangeArray:
+    def GetRanges(self) -> 'richtext.RichTextRangeArray':
         """ Returns the selection ranges.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextSelection.html
         """
 
-    def GetSelectionForObject(self, obj: 'richtext.RichTextObject') -> RichTextRangeArray:
+    def GetSelectionForObject(self, obj: 'richtext.RichTextObject') -> 'richtext.RichTextRangeArray':
         """ Returns the selection appropriate to the specified object, if any; returns an empty array if none at the level of the objectâs container.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextSelection.html
         """
 
     def IsValid(self) -> bool:
         """ Returns True if the selection is valid.
@@ -6860,15 +6860,15 @@
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextSelection.html
         """
 
     Container: 'richtext.RichTextParagraphLayoutBox'  # See GetContainer and SetContainer
     Count: int  # See GetCount
     Range: 'richtext.RichTextRange'  # See GetRange and SetRange
-    Ranges: RichTextRangeArray  # See GetRanges and SetRanges
+    Ranges: 'richtext.RichTextRangeArray'  # See GetRanges and SetRanges
     m_container: Any  # A public C++ attribute of type RichTextParagraphLayoutBox     .
     m_ranges: Any  # A public C++ attribute of type RichTextRangeArray.
 
 
 
 RICHTEXT_NO_SELECTION: int
 
@@ -6893,15 +6893,15 @@
 
     def Copy(self, obj: 'richtext.RichTextLine') -> None:
         """ Copies from obj.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextLine.html
         """
 
-    def GetAbsolutePosition(self) -> Point:
+    def GetAbsolutePosition(self) -> 'Point':
         """ Returns the absolute object position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextLine.html
         """
 
     def GetAbsoluteRange(self) -> 'richtext.RichTextRange':
         """ Returns the absolute range.
@@ -6917,33 +6917,33 @@
 
     def GetParent(self) -> 'richtext.RichTextParagraph':
         """ Returns the parent paragraph.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextLine.html
         """
 
-    def GetPosition(self) -> Point:
+    def GetPosition(self) -> 'Point':
         """ Returns the object position relative to the parent.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextLine.html
         """
 
     def GetRange(self) -> 'richtext.RichTextRange':
         """ Returns the range.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextLine.html
         """
 
-    def GetRect(self) -> Rect:
+    def GetRect(self) -> 'Rect':
         """ Returns the rectangle enclosing the line.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextLine.html
         """
 
-    def GetSize(self) -> Size:
+    def GetSize(self) -> 'Size':
         """ Returns the line size as calculated by Layout.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextLine.html
         """
 
     def Init(self, parent: 'richtext.RichTextParagraph') -> None:
         """ Initialises the object.
@@ -6971,22 +6971,22 @@
 
     def SetSize(self, sz: Union[tuple[int, int], 'Size']) -> None:
         """ Sets the line size as calculated by Layout.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextLine.html
         """
 
-    AbsolutePosition: Point  # See GetAbsolutePosition
+    AbsolutePosition: 'Point'  # See GetAbsolutePosition
     AbsoluteRange: 'richtext.RichTextRange'  # See GetAbsoluteRange
     Descent: int  # See GetDescent and SetDescent
     Parent: 'richtext.RichTextParagraph'  # See GetParent
-    Position: Union[tuple[int, int], 'Point']  # See GetPosition and SetPosition
+    Position: 'Point'  # See GetPosition and SetPosition
     Range: 'richtext.RichTextRange'  # See GetRange and SetRange
-    Rect: Rect  # See GetRect
-    Size: Union[tuple[int, int], 'Size']  # See GetSize and SetSize
+    Rect: '_Rect'  # See GetRect
+    Size: '_Size'  # See GetSize and SetSize
 
 
 
 class RichTextListStyleDefinition(RichTextParagraphStyleDefinition):
     """ This class represents a list style definition, usually added to a
 RichTextStyleSheet.
 
@@ -7065,15 +7065,15 @@
 
     def AcceptsFocus(self) -> bool:
         """ Returns True if objects of this class can accept the focus, i.e. a call to SetFocusObject is possible.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextField.html
         """
 
-    def CalculateRange(self, start: int) -> end:
+    def CalculateRange(self, start: int) -> None:
         """ Calculates the range of the object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextField.html
         """
 
     def CanEditProperties(self) -> bool:
         """ Returns True if we can edit the objectâs properties via a GUI.
@@ -7192,39 +7192,39 @@
 
     def Draw(self, obj, dc, context, range, selection, rect, descent, style) -> bool:
         """ Draw the item, within the given range.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
-    def GetBackgroundColour(self) -> Colour:
+    def GetBackgroundColour(self) -> 'Colour':
         """ Gets the colour used for drawing the field background.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
-    def GetBitmap(self) -> Bitmap:
+    def GetBitmap(self) -> 'Bitmap':
         """ Gets the bitmap label for fields of this type.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
-    def GetBorderColour(self) -> Colour:
+    def GetBorderColour(self) -> 'Colour':
         """ Gets the colour used for drawing the field border.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
     def GetDisplayStyle(self) -> int:
         """ Gets the display style for fields of this type.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
-    def GetFont(self) -> Font:
+    def GetFont(self) -> 'Font':
         """ Gets the font used for drawing the text label.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
     def GetHorizontalMargin(self) -> int:
         """ Gets the horizontal margin surrounding the field object.
@@ -7246,21 +7246,21 @@
 
     def GetRangeSize(*args, **kwargs) -> bool:
         """ Returns the object size for the given range.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
-    def GetSize(self, obj, dc, context, style) -> Size:
+    def GetSize(self, obj, dc, context, style) -> 'Size':
         """ Get the size of the field, given the label, font size, and so on.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
-    def GetTextColour(self) -> Colour:
+    def GetTextColour(self) -> 'Colour':
         """ Gets the colour used for drawing the text label.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
     def GetVerticalMargin(self) -> int:
         """ Gets the vertical margin surrounding the field object.
@@ -7354,23 +7354,23 @@
 
     def SetVerticalPadding(self, padding: int) -> None:
         """ Sets the vertical padding (the distance between the border and the text).
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFieldTypeStandard.html
         """
 
-    BackgroundColour: Union[int, str, 'Colour']  # See GetBackgroundColour and SetBackgroundColour
-    Bitmap: 'Bitmap'  # See GetBitmap and SetBitmap
-    BorderColour: Union[int, str, 'Colour']  # See GetBorderColour and SetBorderColour
+    BackgroundColour: 'Colour'  # See GetBackgroundColour and SetBackgroundColour
+    Bitmap: '_Bitmap'  # See GetBitmap and SetBitmap
+    BorderColour: 'Colour'  # See GetBorderColour and SetBorderColour
     DisplayStyle: int  # See GetDisplayStyle and SetDisplayStyle
-    Font: 'Font'  # See GetFont and SetFont
+    Font: '_Font'  # See GetFont and SetFont
     HorizontalMargin: int  # See GetHorizontalMargin and SetHorizontalMargin
     HorizontalPadding: int  # See GetHorizontalPadding and SetHorizontalPadding
     Label: str  # See GetLabel and SetLabel
-    TextColour: Union[int, str, 'Colour']  # See GetTextColour and SetTextColour
+    TextColour: 'Colour'  # See GetTextColour and SetTextColour
     VerticalMargin: int  # See GetVerticalMargin and SetVerticalMargin
     VerticalPadding: int  # See GetVerticalPadding and SetVerticalPadding
 
 
 
 RICHTEXT_FIELD_STYLE_COMPOSITE: int  # Creates a composite field; you will probably need to derive a new class to implement UpdateField.
 
@@ -7481,15 +7481,15 @@
     def GetApplyOnSelection(self) -> bool:
         """ If the return value is True, clicking on a style name in the list will immediately apply the style to the associated rich text control.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListBox.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListBox.html
         """
 
     def GetRichTextCtrl(self) -> 'richtext.RichTextCtrl':
         """ Returns the   wx.richtext.RichTextCtrl  associated with this listbox.
@@ -7505,15 +7505,15 @@
 
     def GetStyleSheet(self) -> 'richtext.RichTextStyleSheet':
         """ Returns the style sheet associated with this listbox.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListBox.html
         """
 
-    def GetStyleType(self) -> 'richtext.RichTextStyleListBox.wxRichTextStyleType':
+    def GetStyleType(self) -> 'richtext.wxRichTextStyleType':
         """ Returns the type of style to show in the list box.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListBox.html
         """
 
     def OnGetItem(self, n: int) -> str:
         """ Returns the HTML for this item.
@@ -7556,18 +7556,20 @@
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextStyleListBox.html
         """
 
     ApplyOnSelection: bool  # See GetApplyOnSelection and SetApplyOnSelection
     RichTextCtrl: 'richtext.RichTextCtrl'  # See GetRichTextCtrl and SetRichTextCtrl
     StyleSheet: 'richtext.RichTextStyleSheet'  # See GetStyleSheet and SetStyleSheet
-    StyleType: RichTextStyleListBox.wxRichTextStyleType  # See GetStyleType and SetStyleType
+    StyleType: 'richtext.wxRichTextStyleType'  # See GetStyleType and SetStyleType
 
 
 
+RichTextCommandId: TypeAlias = int  # Enumeration
+
 RICHTEXT_INSERT: int
 
 RICHTEXT_DELETE: int
 
 RICHTEXT_CHANGE_ATTRIBUTES: int
 
 RICHTEXT_CHANGE_STYLE: int
@@ -7592,43 +7594,43 @@
 
     def Create(*args, **kwargs) -> bool:
         """ Creation: see   wx.richtext.RichTextFormattingDialog  âthe constructorâ for details about the parameters.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
-    def GetAttributes(self) -> TextAttr:
+    def GetAttributes(self) -> 'TextAttr':
         """ Gets the attributes being edited.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
     @staticmethod
-    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> VisualAttributes:
+    def GetClassDefaultAttributes(variant: int=WINDOW_VARIANT_NORMAL) -> 'VisualAttributes':
         """ variant (WindowVariant) â
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
     @staticmethod
-    def GetColourData() -> ColourData:
+    def GetColourData() -> 'ColourData':
         """ Returns the custom colour data for use by the colour dialog.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
     @staticmethod
     def GetDialog(win: 'Window') -> 'richtext.RichTextFormattingDialog':
         """ Helper for pages to get the top-level dialog.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
     @staticmethod
-    def GetDialogAttributes(win: 'Window') -> TextAttr:
+    def GetDialogAttributes(win: 'Window') -> 'TextAttr':
         """ Helper for pages to get the attributes.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
     @staticmethod
     def GetDialogStyleDefinition(win: 'Window') -> 'richtext.RichTextStyleDefinition':
@@ -7640,15 +7642,15 @@
     @staticmethod
     def GetFormattingDialogFactory() -> 'richtext.RichTextFormattingDialogFactory':
         """ Returns the object to be used to customize the dialog and provide pages.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
-    def GetImageList(self) -> ImageList:
+    def GetImageList(self) -> 'ImageList':
         """ Returns the image list associated with the dialog, used for example if showing the dialog as a toolbook.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
     @staticmethod
     def GetLastPage() -> int:
@@ -7755,15 +7757,15 @@
     def UpdateDisplay(self) -> bool:
         """ Updates the display.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextFormattingDialog.html
         """
 
     Attributes: 'TextAttr'  # See GetAttributes and SetAttributes
-    ImageList: 'ImageList'  # See GetImageList and SetImageList
+    ImageList: '_ImageList'  # See GetImageList and SetImageList
     Options: int  # See GetOptions and SetOptions
     StyleDefinition: 'richtext.RichTextStyleDefinition'  # See GetStyleDefinition and SetStyleDefinition
     StyleSheet: 'richtext.RichTextStyleSheet'  # See GetStyleSheet
 
 
 
 class RichTextObjectAddress:
@@ -7826,15 +7828,15 @@
     """
     def __init__(self, *args, **kw) -> None:
         """ Overloaded Implementations:
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextPlainText.html
         """
 
-    def CalculateRange(self, start: int) -> end:
+    def CalculateRange(self, start: int) -> None:
         """ Calculates the range of the object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextPlainText.html
         """
 
     def CanMerge(self, object, context) -> bool:
         """ Returns True if this object can merge itself with the given one.
@@ -8124,20 +8126,24 @@
             Source: https://docs.wxpython.org/wx.richtext.RichTextXMLHandler.html
         """
 
 
 
 RICHTEXT_HANDLER_INCLUDE_STYLESHEET: int
 
+RichTextOddEvenPage: TypeAlias = int  # Enumeration
+
 RICHTEXT_PAGE_ODD: int
 
 RICHTEXT_PAGE_EVEN: int
 
 RICHTEXT_PAGE_ALL: int
 
+RichTextPageLocation: TypeAlias = int  # Enumeration
+
 RICHTEXT_PAGE_LEFT: int
 
 RICHTEXT_PAGE_CENTRE: int
 
 RICHTEXT_PAGE_RIGHT: int
 
 class RichTextCompositeObject(RichTextObject):
@@ -8153,15 +8159,15 @@
 
     def AppendChild(self, child: 'richtext.RichTextObject') -> int:
         """ Appends a child, returning the position.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCompositeObject.html
         """
 
-    def CalculateRange(self, start: int) -> end:
+    def CalculateRange(self, start: int) -> None:
         """ Calculates the range of the object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCompositeObject.html
         """
 
     def Copy(self, obj: 'richtext.RichTextCompositeObject') -> None:
         """ obj (wx.richtext.RichTextCompositeObject) â
@@ -8207,15 +8213,15 @@
 
     def GetChildCount(self) -> int:
         """ Returns the number of children.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCompositeObject.html
         """
 
-    def GetChildren(self) -> RichTextObjectList:
+    def GetChildren(self) -> 'richtext.RichTextObjectList':
         """ Returns the children.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCompositeObject.html
         """
 
     def GetRangeSize(*args, **kwargs) -> bool:
         """ Returns the object size for the given range.
@@ -8274,15 +8280,15 @@
     def RemoveChild(self, child, deleteChild=False) -> bool:
         """ Removes and optionally deletes the specified child.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextCompositeObject.html
         """
 
     ChildCount: int  # See GetChildCount
-    Children: RichTextObjectList  # See GetChildren
+    Children: 'richtext.RichTextObjectList'  # See GetChildren
 
 
 
 class RichTextImage(RichTextObject):
     """ This class implements a graphic object.
 
         Source: https://docs.wxpython.org/wx.richtext.RichTextImage.html
@@ -8325,15 +8331,15 @@
 
     def GetImageBlock(self) -> 'richtext.RichTextImageBlock':
         """ Returns the image block containing the raw data.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextImage.html
         """
 
-    def GetImageCache(self) -> Bitmap:
+    def GetImageCache(self) -> 'Bitmap':
         """ Returns the image cache (a scaled bitmap).
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextImage.html
         """
 
     def GetImageState(self) -> int:
         """ Gets the image state.
@@ -8343,15 +8349,15 @@
 
     def GetNaturalSize(self) -> 'richtext.TextAttrSize':
         """ Returns the ânaturalâ size for this object - the image size.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextImage.html
         """
 
-    def GetOriginalImageSize(self) -> Size:
+    def GetOriginalImageSize(self) -> 'Size':
         """ Gets the original image size.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextImage.html
         """
 
     def GetPropertiesMenuLabel(self) -> str:
         """ Returns the label to be used for the properties context menu item.
@@ -8437,15 +8443,15 @@
             Source: https://docs.wxpython.org/wx.richtext.RichTextImage.html
         """
 
     ImageBlock: 'richtext.RichTextImageBlock'  # See GetImageBlock
     ImageCache: 'Bitmap'  # See GetImageCache and SetImageCache
     ImageState: int  # See GetImageState and SetImageState
     NaturalSize: 'richtext.TextAttrSize'  # See GetNaturalSize
-    OriginalImageSize: Union[tuple[int, int], 'Size']  # See GetOriginalImageSize and SetOriginalImageSize
+    OriginalImageSize: 'Size'  # See GetOriginalImageSize and SetOriginalImageSize
     PropertiesMenuLabel: str  # See GetPropertiesMenuLabel
     XMLNodeName: str  # See GetXMLNodeName
 
 
 
 class TextAttrBorders:
     """ A class representing a rich text objectâs borders.
@@ -8681,15 +8687,15 @@
 
     def ApplyParagraphStyle(self, line, attr, rect, dc) -> None:
         """ Applies paragraph styles such as centering to the wrapped lines.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraph.html
         """
 
-    def CalculateRange(self, start: int) -> end:
+    def CalculateRange(self, start: int) -> None:
         """ Calculates the range of the object.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraph.html
         """
 
     @staticmethod
     def ClearDefaultTabs() -> None:
@@ -8834,15 +8840,15 @@
 
     def LayoutFloat(self, dc, context, rect, parentRect, style, floatCollector) -> None:
         """ Lays out the floating objects.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraph.html
         """
 
-    def MoveFromList(self, list: RichTextObjectList_) -> None:
+    def MoveFromList(self, list: list['richtext.RichTextList']) -> None:
         """ Adds content back from a list.
 
             Source: https://docs.wxpython.org/wx.richtext.RichTextParagraph.html
         """
 
     def MoveToList(self, obj, list) -> None:
         """ Moves content to a list from this point.
@@ -9340,19 +9346,19 @@
     Border: 'richtext.TextAttrBorders'  # See GetBorder
     Bottom: 'richtext.TextAttrDimension'  # See GetBottom
     BottomBorder: 'richtext.TextAttrBorder'  # See GetBottomBorder
     BottomMargin: 'richtext.TextAttrDimension'  # See GetBottomMargin
     BottomOutline: 'richtext.TextAttrBorder'  # See GetBottomOutline
     BottomPadding: 'richtext.TextAttrDimension'  # See GetBottomPadding
     BoxStyleName: str  # See GetBoxStyleName and SetBoxStyleName
-    ClearMode: TextBoxAttrClearStyle  # See GetClearMode and SetClearMode
-    CollapseBorders: TextBoxAttrCollapseMode  # See GetCollapseBorders and SetCollapseBorders
+    ClearMode: 'richtext.TextBoxAttrClearStyle'  # See GetClearMode and SetClearMode
+    CollapseBorders: 'richtext.TextBoxAttrCollapseMode'  # See GetCollapseBorders and SetCollapseBorders
     CornerRadius: 'richtext.TextAttrDimension'  # See GetCornerRadius and SetCornerRadius
     Flags: int  # See GetFlags and SetFlags
-    FloatMode: TextBoxAttrFloatStyle  # See GetFloatMode and SetFloatMode
+    FloatMode: 'richtext.TextBoxAttrFloatStyle'  # See GetFloatMode and SetFloatMode
     Height: 'richtext.TextAttrDimension'  # See GetHeight
     Left: 'richtext.TextAttrDimension'  # See GetLeft
     LeftBorder: 'richtext.TextAttrBorder'  # See GetLeftBorder
     LeftMargin: 'richtext.TextAttrDimension'  # See GetLeftMargin
     LeftOutline: 'richtext.TextAttrBorder'  # See GetLeftOutline
     LeftPadding: 'richtext.TextAttrDimension'  # See GetLeftPadding
     Margins: 'richtext.TextAttrDimensions'  # See GetMargins
@@ -9370,15 +9376,15 @@
     Size: 'richtext.TextAttrSize'  # See GetSize and SetSize
     Top: 'richtext.TextAttrDimension'  # See GetTop
     TopBorder: 'richtext.TextAttrBorder'  # See GetTopBorder
     TopMargin: 'richtext.TextAttrDimension'  # See GetTopMargin
     TopOutline: 'richtext.TextAttrBorder'  # See GetTopOutline
     TopPadding: 'richtext.TextAttrDimension'  # See GetTopPadding
     VerticalAlignment: int  # See GetVerticalAlignment and SetVerticalAlignment
-    WhitespaceMode: TextBoxAttrWhitespaceMode  # See GetWhitespaceMode and SetWhitespaceMode
+    WhitespaceMode: 'richtext.TextBoxAttrWhitespaceMode'  # See GetWhitespaceMode and SetWhitespaceMode
     Width: 'richtext.TextAttrDimension'  # See GetWidth
     m_border: Any  # A public C++ attribute of type TextAttrBorders     .
     m_boxStyleName: Any  # A public C++ attribute of type string.
     m_clearMode: Any  # A public C++ attribute of type TextBoxAttrClearStyle     .
     m_collapseMode: Any  # A public C++ attribute of type TextBoxAttrCollapseMode     .
     m_cornerRadius: Any  # A public C++ attribute of type TextAttrDimension     .
     m_flags: Any  # A public C++ attribute of type int.
@@ -9392,14 +9398,16 @@
     m_shadow: Any  # A public C++ attribute of type TextAttrShadow     .
     m_size: Any  # A public C++ attribute of type TextAttrSize     .
     m_verticalAlignment: Any  # A public C++ attribute of type TextBoxAttrVerticalAlignment     .
     m_whitespaceMode: Any  # A public C++ attribute of type TextBoxAttrWhitespaceMode     .
 
 
 
+RichTextFileType: TypeAlias = int  # Enumeration
+
 RICHTEXT_TYPE_TEXT: int
 
 RICHTEXT_TYPE_XML: int
 
 RICHTEXT_TYPE_HTML: int
 
 RICHTEXT_TYPE_RTF: int
@@ -9527,15 +9535,15 @@
 
     def EqPartial(self, border, weakTest=True) -> bool:
         """ Partial equality test.
 
             Source: https://docs.wxpython.org/wx.richtext.TextAttrBorder.html
         """
 
-    def GetColour(self) -> Colour:
+    def GetColour(self) -> 'Colour':
         """ Gets the colour.
 
             Source: https://docs.wxpython.org/wx.richtext.TextAttrBorder.html
         """
 
     def GetColourLong(self) -> int:
         """ Gets the colour as a long.
@@ -9653,15 +9661,15 @@
 
     def __eq__(self, item: Any) -> bool:
         """ Equality operator.
 
             Source: https://docs.wxpython.org/wx.richtext.TextAttrBorder.html
         """
 
-    Colour: int  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
     ColourLong: int  # See GetColourLong
     Flags: int  # See GetFlags and SetFlags
     Style: int  # See GetStyle and SetStyle
     Width: 'richtext.TextAttrDimension'  # See GetWidth and SetWidth
     m_borderColour: Any  # A public C++ attribute of type long.
     m_borderStyle: Any  # A public C++ attribute of type int.
     m_borderWidth: Any  # A public C++ attribute of type TextAttrDimension     .
@@ -9792,23 +9800,25 @@
     def __eq__(self, item: Any) -> bool:
         """ Equality operator.
 
             Source: https://docs.wxpython.org/wx.richtext.TextAttrDimension.html
         """
 
     Flags: 'richtext.TextAttrDimensionFlags'  # See GetFlags and SetFlags
-    Position: TextBoxAttrPosition  # See GetPosition and SetPosition
-    Units: TextAttrUnits  # See GetUnits and SetUnits
+    Position: 'richtext.TextBoxAttrPosition'  # See GetPosition and SetPosition
+    Units: 'richtext.TextAttrUnits'  # See GetUnits and SetUnits
     Value: int  # See GetValue and SetValue
     ValueMM: float  # See GetValueMM and SetValueMM
     m_flags: Any  # A public C++ attribute of type TextAttrDimensionFlags     .
     m_value: Any  # A public C++ attribute of type int.
 
 
 
+TextAttrUnits: TypeAlias = int  # Enumeration
+
 TEXT_ATTR_UNITS_TENTHS_MM: int
 
 TEXT_ATTR_UNITS_PIXELS: int
 
 TEXT_ATTR_UNITS_PERCENTAGE: int
 
 TEXT_ATTR_UNITS_POINTS: int
@@ -9954,15 +9964,15 @@
 
     def GetBlurDistance(self) -> 'richtext.TextAttrDimension':
         """ Gets the shadow blur distance.
 
             Source: https://docs.wxpython.org/wx.richtext.TextAttrShadow.html
         """
 
-    def GetColour(self) -> Colour:
+    def GetColour(self) -> 'Colour':
         """ Gets the colour.
 
             Source: https://docs.wxpython.org/wx.richtext.TextAttrShadow.html
         """
 
     def GetColourLong(self) -> int:
         """ Gets the colour as a long.
@@ -10087,15 +10097,15 @@
     def __eq__(self, item: Any) -> bool:
         """ Equality operator.
 
             Source: https://docs.wxpython.org/wx.richtext.TextAttrShadow.html
         """
 
     BlurDistance: 'richtext.TextAttrDimension'  # See GetBlurDistance and SetBlurDistance
-    Colour: int  # See GetColour and SetColour
+    Colour: '_Colour'  # See GetColour and SetColour
     ColourLong: int  # See GetColourLong
     Flags: int  # See GetFlags and SetFlags
     OffsetX: 'richtext.TextAttrDimension'  # See GetOffsetX and SetOffsetX
     OffsetY: 'richtext.TextAttrDimension'  # See GetOffsetY and SetOffsetY
     Opacity: 'richtext.TextAttrDimension'  # See GetOpacity and SetOpacity
     Spread: 'richtext.TextAttrDimension'  # See GetSpread and SetSpread
     m_blurDistance: Any  # A public C++ attribute of type TextAttrDimension     .
@@ -10104,69 +10114,101 @@
     m_offsetY: Any  # A public C++ attribute of type TextAttrDimension     .
     m_opacity: Any  # A public C++ attribute of type TextAttrDimension     .
     m_shadowColour: Any  # A public C++ attribute of type long.
     m_spread: Any  # A public C++ attribute of type TextAttrDimension     .
 
 
 
+TextBoxAttrFlags: TypeAlias = int  # Enumeration
+
 TEXT_BOX_ATTR_FLOAT: int
 
 TEXT_BOX_ATTR_CLEAR: int
 
 TEXT_BOX_ATTR_COLLAPSE_BORDERS: int
 
 TEXT_BOX_ATTR_VERTICAL_ALIGNMENT: int
 
 TEXT_BOX_ATTR_BOX_STYLE_NAME: int
 
 TEXT_BOX_ATTR_WHITESPACE: int
 
 TEXT_BOX_ATTR_CORNER_RADIUS: int
 
+TextBoxAttrClearStyle: TypeAlias = int  # Enumeration
+
 TEXT_BOX_ATTR_CLEAR_NONE: int
 
 TEXT_BOX_ATTR_CLEAR_LEFT: int
 
 TEXT_BOX_ATTR_CLEAR_RIGHT: int
 
 TEXT_BOX_ATTR_CLEAR_BOTH: int
 
+TextBoxAttrCollapseMode: TypeAlias = int  # Enumeration
+
 TEXT_BOX_ATTR_COLLAPSE_NONE: int
 
 TEXT_BOX_ATTR_COLLAPSE_FULL: int
 
+TextBoxAttrFloatStyle: TypeAlias = int  # Enumeration
+
 TEXT_BOX_ATTR_FLOAT_NONE: int
 
 TEXT_BOX_ATTR_FLOAT_LEFT: int
 
 TEXT_BOX_ATTR_FLOAT_RIGHT: int
 
+TextBoxAttrVerticalAlignment: TypeAlias = int  # Enumeration
+
 TEXT_BOX_ATTR_VERTICAL_ALIGNMENT_NONE: int
 
 TEXT_BOX_ATTR_VERTICAL_ALIGNMENT_TOP: int
 
 TEXT_BOX_ATTR_VERTICAL_ALIGNMENT_CENTRE: int
 
 TEXT_BOX_ATTR_VERTICAL_ALIGNMENT_BOTTOM: int
 
+TextBoxAttrWhitespaceMode: TypeAlias = int  # Enumeration
+
 TEXT_BOX_ATTR_WHITESPACE_NONE: int
 
 TEXT_BOX_ATTR_WHITESPACE_NORMAL: int
 
 TEXT_BOX_ATTR_WHITESPACE_NO_WRAP: int
 
 TEXT_BOX_ATTR_WHITESPACE_PREFORMATTED: int
 
 TEXT_BOX_ATTR_WHITESPACE_PREFORMATTED_LINE: int
 
 TEXT_BOX_ATTR_WHITESPACE_PREFORMATTED_WRAP: int
 
+TextBoxAttrPosition: TypeAlias = int  # Enumeration
+
 TEXT_BOX_ATTR_POSITION_STATIC: int
 
 TEXT_BOX_ATTR_POSITION_RELATIVE: int
 
 TEXT_BOX_ATTR_POSITION_ABSOLUTE: int
 
 TEXT_BOX_ATTR_POSITION_FIXED: int
 
 TEXT_BOX_ATTR_POSITION_MASK: int
 
+RichTextActionList: TypeAlias = list['RichTextAction']
+
+wxRichTextStyleType: TypeAlias = int
+
+RichTextVariantArray: TypeAlias = list[Any]
+
+RichTextFloatCollector: TypeAlias = Any
+
+RichTextObjectPtrArrayArray: TypeAlias = list[Any]
+
+RichTextObjectPtrArray: TypeAlias = list[Any]
+
+RichTextRangeArray: TypeAlias = list['RichTextRange']
+
+RichTextObjectList: TypeAlias = list['RichTextObject']
+
+TextAttrDimensionFlags: TypeAlias = int
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/stc/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/stc/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class StyledTextEvent(CommandEvent):
     """ The type of events sent from StyledTextCtrl.
 
         Source: https://docs.wxpython.org/wx.stc.StyledTextEvent.html
     """
     def __init__(self, *args, **kw) -> None:
@@ -318,15 +318,15 @@
             Source: https://docs.wxpython.org/wx.stc.StyledTextEvent.html
         """
 
     Alt: bool  # See GetAlt
     AnnotationsLinesAdded: int  # See GetAnnotationsLinesAdded
     Control: bool  # See GetControl
     DragFlags: int  # See GetDragFlags and SetDragFlags
-    DragResult: DragResult  # See GetDragResult and SetDragResult
+    DragResult: '_DragResult'  # See GetDragResult and SetDragResult
     DragText: str  # See GetDragText and SetDragText
     FoldLevelNow: int  # See GetFoldLevelNow and SetFoldLevelNow
     FoldLevelPrev: int  # See GetFoldLevelPrev and SetFoldLevelPrev
     Key: int  # See GetKey and SetKey
     LParam: int  # See GetLParam and SetLParam
     Length: int  # See GetLength and SetLength
     Line: int  # See GetLine and SetLine
@@ -1855,15 +1855,15 @@
 
     def GetLineLength(self, lineNo: int) -> int:
         """ Gets the length of the specified line, not including any trailing newline character(s).
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
-    def GetLineRaw(self, line: int) -> CharBuffer:
+    def GetLineRaw(self, line: int) -> 'stc.CharBuffer':
         """ Retrieve the contents of a line.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
     def GetLineSelEndPosition(self, line: int) -> int:
         """ Retrieve the position of the end of the selection at the given line (wx``wx.stc.STC_INVALID_POSITION`` if no selection on this line).
@@ -2211,15 +2211,15 @@
 
     def GetSelectedText(self) -> str:
         """ Retrieve the selected text.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
-    def GetSelectedTextRaw(self) -> CharBuffer:
+    def GetSelectedTextRaw(self) -> 'stc.CharBuffer':
         """ Retrieve the selected text.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
     def GetSelection(self) -> tuple:
         """ Gets the current selection span.
@@ -2331,15 +2331,15 @@
 
     def GetStyleFromSubStyle(self, subStyle: int) -> int:
         """ For a sub style, return the base style, else return the argument.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
-    def GetStyledText(self, startPos, endPos) -> MemoryBuffer:
+    def GetStyledText(self, startPos, endPos) -> 'MemoryBuffer':
         """ Retrieve a buffer of cells.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
     def GetSubStyleBases(self) -> str:
         """ Get the set of base styles that can be extended with sub styles.
@@ -2397,15 +2397,15 @@
 
     def GetTargetText(self) -> str:
         """ Retrieve the text in the target.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
-    def GetTargetTextRaw(self) -> CharBuffer:
+    def GetTargetTextRaw(self) -> 'stc.CharBuffer':
         """ Retrieve the target text.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
     def GetTechnology(self) -> int:
         """ Get the tech.
@@ -2427,21 +2427,21 @@
 
     def GetTextRange(self, startPos, endPos) -> str:
         """ Retrieve a range of text.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
-    def GetTextRangeRaw(self, startPos, endPos) -> CharBuffer:
+    def GetTextRangeRaw(self, startPos, endPos) -> 'stc.CharBuffer':
         """ Retrieve a range of text.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
-    def GetTextRaw(self) -> CharBuffer:
+    def GetTextRaw(self) -> 'stc.CharBuffer':
         """ Retrieve all the text in the document.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
     def GetTwoPhaseDraw(self) -> bool:
         """ Is drawing done in two phases with backgrounds drawn before foregrounds?
@@ -3513,15 +3513,15 @@
 
     def SelectionIsRectangle(self) -> bool:
         """ Is the selection rectangular? The alternative is the more common stream selection.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
-    def SendMsg(self, msg, wp=0, lp=0) -> 'IntPtr':
+    def SendMsg(self, msg, wp=0, lp=0) -> int:
         """ Scintilla API call.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
     def SetAdditionalCaretForeground(self, fore: Union[int, str, 'Colour']) -> None:
         """ Set the foreground colour of additional carets.
@@ -5037,27 +5037,27 @@
 
     def write(self, text) -> None:
         """ Append text to the textctrl, for file-like compatibility.
 
             Source: https://docs.wxpython.org/wx.stc.StyledTextCtrl.html
         """
 
-    AdditionalCaretForeground: Union[int, str, 'Colour']  # See GetAdditionalCaretForeground and SetAdditionalCaretForeground
+    AdditionalCaretForeground: 'Colour'  # See GetAdditionalCaretForeground and SetAdditionalCaretForeground
     AdditionalCaretsBlink: bool  # See GetAdditionalCaretsBlink and SetAdditionalCaretsBlink
     AdditionalCaretsVisible: bool  # See GetAdditionalCaretsVisible and SetAdditionalCaretsVisible
     AdditionalSelAlpha: int  # See GetAdditionalSelAlpha and SetAdditionalSelAlpha
     AdditionalSelectionTyping: bool  # See GetAdditionalSelectionTyping and SetAdditionalSelectionTyping
     AllLinesVisible: bool  # See GetAllLinesVisible
     Anchor: int  # See GetAnchor and SetAnchor
     AutomaticFold: int  # See GetAutomaticFold and SetAutomaticFold
     BackSpaceUnIndents: bool  # See GetBackSpaceUnIndents and SetBackSpaceUnIndents
     BufferedDraw: bool  # See GetBufferedDraw and SetBufferedDraw
-    CaretForeground: Union[int, str, 'Colour']  # See GetCaretForeground and SetCaretForeground
+    CaretForeground: 'Colour'  # See GetCaretForeground and SetCaretForeground
     CaretLineBackAlpha: int  # See GetCaretLineBackAlpha and SetCaretLineBackAlpha
-    CaretLineBackground: Union[int, str, 'Colour']  # See GetCaretLineBackground and SetCaretLineBackground
+    CaretLineBackground: 'Colour'  # See GetCaretLineBackground and SetCaretLineBackground
     CaretLineVisible: bool  # See GetCaretLineVisible and SetCaretLineVisible
     CaretLineVisibleAlways: bool  # See GetCaretLineVisibleAlways and SetCaretLineVisibleAlways
     CaretPeriod: int  # See GetCaretPeriod and SetCaretPeriod
     CaretSticky: int  # See GetCaretSticky and SetCaretSticky
     CaretStyle: int  # See GetCaretStyle and SetCaretStyle
     CaretWidth: int  # See GetCaretWidth and SetCaretWidth
     CharacterPointer: Any  # See GetCharacterPointer
@@ -5066,17 +5066,17 @@
     CurLine: tuple  # See GetCurLine
     CurLineRaw: tuple  # See GetCurLineRaw
     CurrentLine: int  # See GetCurrentLine
     CurrentPos: int  # See GetCurrentPos and SetCurrentPos
     DefaultStyle: 'TextAttr'  # See GetDefaultStyle and SetDefaultStyle
     DirectFunction: None  # See GetDirectFunction
     DirectPointer: None  # See GetDirectPointer
-    DocPointer: Any  # See GetDocPointer and SetDocPointer
+    DocPointer: None  # See GetDocPointer and SetDocPointer
     EOLMode: int  # See GetEOLMode and SetEOLMode
-    EdgeColour: Union[int, str, 'Colour']  # See GetEdgeColour and SetEdgeColour
+    EdgeColour: 'Colour'  # See GetEdgeColour and SetEdgeColour
     EdgeColumn: int  # See GetEdgeColumn and SetEdgeColumn
     EdgeMode: int  # See GetEdgeMode and SetEdgeMode
     EndAtLastLine: bool  # See GetEndAtLastLine and SetEndAtLastLine
     EndStyled: int  # See GetEndStyled
     ExtraAscent: int  # See GetExtraAscent and SetExtraAscent
     ExtraDescent: int  # See GetExtraDescent and SetExtraDescent
     FirstVisibleLine: int  # See GetFirstVisibleLine and SetFirstVisibleLine
@@ -5141,15 +5141,15 @@
     STCFocus: bool  # See GetSTCFocus and SetSTCFocus
     ScrollWidth: int  # See GetScrollWidth and SetScrollWidth
     ScrollWidthTracking: bool  # See GetScrollWidthTracking and SetScrollWidthTracking
     SearchFlags: int  # See GetSearchFlags and SetSearchFlags
     SelAlpha: int  # See GetSelAlpha and SetSelAlpha
     SelEOLFilled: bool  # See GetSelEOLFilled and SetSelEOLFilled
     SelectedText: str  # See GetSelectedText
-    SelectedTextRaw: CharBuffer  # See GetSelectedTextRaw
+    SelectedTextRaw: 'stc.CharBuffer'  # See GetSelectedTextRaw
     SelectionEmpty: bool  # See GetSelectionEmpty
     SelectionEnd: int  # See GetSelectionEnd and SetSelectionEnd
     SelectionMode: int  # See GetSelectionMode and SetSelectionMode
     SelectionStart: int  # See GetSelectionStart and SetSelectionStart
     Selections: int  # See GetSelections
     Status: int  # See GetStatus and SetStatus
     StringSelection: str  # See GetStringSelection
@@ -5158,19 +5158,19 @@
     SubStyleBases: str  # See GetSubStyleBases
     TabDrawMode: int  # See GetTabDrawMode and SetTabDrawMode
     TabIndents: bool  # See GetTabIndents and SetTabIndents
     TabWidth: int  # See GetTabWidth and SetTabWidth
     TargetEnd: int  # See GetTargetEnd and SetTargetEnd
     TargetStart: int  # See GetTargetStart and SetTargetStart
     TargetText: str  # See GetTargetText
-    TargetTextRaw: CharBuffer  # See GetTargetTextRaw
+    TargetTextRaw: 'stc.CharBuffer'  # See GetTargetTextRaw
     Technology: int  # See GetTechnology and SetTechnology
     Text: str  # See GetText and SetText
     TextLength: int  # See GetTextLength
-    TextRaw: int  # See GetTextRaw and SetTextRaw
+    TextRaw: 'stc.CharBuffer'  # See GetTextRaw and SetTextRaw
     TwoPhaseDraw: bool  # See GetTwoPhaseDraw and SetTwoPhaseDraw
     UndoCollection: bool  # See GetUndoCollection and SetUndoCollection
     UseAntiAliasing: bool  # See GetUseAntiAliasing and SetUseAntiAliasing
     UseHorizontalScrollBar: bool  # See GetUseHorizontalScrollBar and SetUseHorizontalScrollBar
     UseTabs: bool  # See GetUseTabs and SetUseTabs
     UseVerticalScrollBar: bool  # See GetUseVerticalScrollBar and SetUseVerticalScrollBar
     Value: str  # See GetValue and SetValue
@@ -5230,7 +5230,9 @@
 
 STC_KEYMOD_SUPER: int
 
 STC_TECHNOLOGY_DEFAULT: int
 
 STC_POPUP_NEVER: int
 
+CharBuffer: TypeAlias = Any
+
```

### Comparing `types_wxpython-0.6.1/wx-stubs/xml/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/xml/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class XmlDocument(Object):
     """ This class holds XML data/document as parsed by XML parser in the root
 node.
 
         Source: https://docs.wxpython.org/wx.xml.XmlDocument.html
     """
@@ -134,15 +134,15 @@
             Source: https://docs.wxpython.org/wx.xml.XmlDocument.html
         """
 
     Doctype: 'xml.XmlDoctype'  # See GetDoctype and SetDoctype
     DocumentNode: 'xml.XmlNode'  # See GetDocumentNode and SetDocumentNode
     EOL: str  # See GetEOL
     FileEncoding: str  # See GetFileEncoding and SetFileEncoding
-    FileType: TextFileType  # See GetFileType and SetFileType
+    FileType: 'TextFileType'  # See GetFileType and SetFileType
     Root: 'xml.XmlNode'  # See GetRoot and SetRoot
     Version: str  # See GetVersion and SetVersion
 
 
 
 XMLDOC_KEEP_WHITESPACE_NODES: int
 
@@ -319,15 +319,15 @@
     Depth: int  # See GetDepth
     LineNumber: int  # See GetLineNumber
     Name: str  # See GetName and SetName
     Next: 'xml.XmlNode'  # See GetNext and SetNext
     NoConversion: bool  # See GetNoConversion and SetNoConversion
     NodeContent: str  # See GetNodeContent
     Parent: 'xml.XmlNode'  # See GetParent and SetParent
-    Type: XmlNodeType  # See GetType and SetType
+    Type: 'xml.XmlNodeType'  # See GetType and SetType
 
 
 
 class XmlAttribute:
     """ Represents a node attribute.
 
         Source: https://docs.wxpython.org/wx.xml.XmlAttribute.html
@@ -430,14 +430,16 @@
     FullString: str  # See GetFullString
     PublicId: str  # See GetPublicId
     RootName: str  # See GetRootName
     SystemId: str  # See GetSystemId
 
 
 
+XmlNodeType: TypeAlias = int  # Enumeration
+
 XML_ELEMENT_NODE: int
 
 XML_ATTRIBUTE_NODE: int
 
 XML_TEXT_NODE: int
 
 XML_CDATA_SECTION_NODE: int
```

### Comparing `types_wxpython-0.6.1/wx-stubs/xrc/__init__.pyi` & `types_wxpython-0.7.0/wx-stubs/xrc/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Any, ContextManager, Optional, Union
+from typing import Any, ContextManager, Optional, TypeAlias, Union
 
 class XmlResource(Object):
     """ This is the main class for interacting with the XML-based resource
 system.
 
         Source: https://docs.wxpython.org/wx.xrc.XmlResource.html
     """
@@ -66,15 +66,15 @@
 
     def GetFlags(self) -> int:
         """ Returns flags, which may be a bitlist of   wx.xrc.XmlResourceFlags  enumeration values.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResource.html
         """
 
-    def GetResourceNode(self, name: str) -> 'xml.XmlNode':
+    def GetResourceNode(self, name: str) -> 'xrc.XmlNode':
         """ Returns the   wx.xml.XmlNode  containing the definition of the object with the given name or None.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResource.html
         """
 
     def GetVersion(self) -> int:
         """ Returns version information (a.b.c.d = d + 256c + 2562b + 2563a).
@@ -278,15 +278,15 @@
 
     def DoCreateResource(self) -> 'Window':
         """ Called from CreateResource after variables were filled.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
-    def GetAnimation(self, param="animation", ctrl=None) -> 'adv.Animation':
+    def GetAnimation(self, param="animation", ctrl=None) -> 'xrc.Animation':
         """ Creates an animation (see   wx.adv.Animation) from the filename specified in param.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
     def GetBitmap(self, *args, **kw) -> 'Bitmap':
         """ Overloaded Implementations:
@@ -386,45 +386,45 @@
 
     def GetName(self) -> str:
         """ Returns the resource name.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
-    def GetNode(self) -> 'xml.XmlNode':
+    def GetNode(self) -> 'xrc.XmlNode':
         """ After CreateResource has been called this will return the XML node being processed.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
-    def GetNodeChildren(self, node: 'xml.XmlNode') -> 'xml.XmlNode':
+    def GetNodeChildren(self, node: 'xml.XmlNode') -> 'xrc.XmlNode':
         """ Gets the first child of the given node or None.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
     def GetNodeContent(self, node: 'xml.XmlNode') -> str:
         """ Gets node content from wx.xml.XML_ENTITY_NODE.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
-    def GetNodeNext(self, node: 'xml.XmlNode') -> 'xml.XmlNode':
+    def GetNodeNext(self, node: 'xml.XmlNode') -> 'xrc.XmlNode':
         """ Gets the next sibling node related to the given node, possibly None.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
-    def GetNodeParent(self, node: 'xml.XmlNode') -> 'xml.XmlNode':
+    def GetNodeParent(self, node: 'xml.XmlNode') -> 'xrc.XmlNode':
         """ Gets the parent of the node given.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
-    def GetParamNode(self, param: str) -> 'xml.XmlNode':
+    def GetParamNode(self, param: str) -> 'xrc.XmlNode':
         """ Finds the node or returns None.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
     def GetParamValue(self, *args, **kw) -> str:
         """ Overloaded Implementations:
@@ -512,39 +512,41 @@
 
     def SetupWindow(self, wnd: 'Window') -> None:
         """ Sets common window options.
 
             Source: https://docs.wxpython.org/wx.xrc.XmlResourceHandler.html
         """
 
-    Animation: 'adv.Animation'  # See GetAnimation
-    Bitmap: 'Bitmap'  # See GetBitmap
-    BitmapBundle: 'BitmapBundle'  # See GetBitmapBundle
+    Animation: 'xrc.Animation'  # See GetAnimation
+    Bitmap: '_Bitmap'  # See GetBitmap
+    BitmapBundle: '_BitmapBundle'  # See GetBitmapBundle
     Class: str  # See GetClass
     CurFileSystem: 'FileSystem'  # See GetCurFileSystem
-    Font: 'Font'  # See GetFont
+    Font: '_Font'  # See GetFont
     ID: int  # See GetID
-    Icon: 'Icon'  # See GetIcon
-    ImageList: 'ImageList'  # See GetImageList
+    Icon: '_Icon'  # See GetIcon
+    ImageList: '_ImageList'  # See GetImageList
     Instance: 'Window'  # See GetInstance
     Name: str  # See GetName
-    Node: 'xml.XmlNode'  # See GetNode
+    Node: 'xrc.XmlNode'  # See GetNode
     Parent: 'Window'  # See GetParent
     ParentAsWindow: 'Window'  # See GetParentAsWindow
     Position: 'Point'  # See GetPosition
     Resource: 'xrc.XmlResource'  # See GetResource
-    Size: 'Size'  # See GetSize
+    Size: '_Size'  # See GetSize
     Style: int  # See GetStyle
 
 
 
 XRCID: int
 
 XML_ENTITY_NODE: int
 
+XmlResourceFlags: TypeAlias = int  # Enumeration
+
 XRC_USE_LOCALE: int
 
 XRC_NO_SUBCLASSING: int
 
 XRC_NO_RELOADING: int
 
 XRC_USE_ENVVARS: int
@@ -564,7 +566,11 @@
         """ className (String) â
 
             Source: https://docs.wxpython.org/wx.xrc.XmlSubclassFactory.html
         """
 
 
 
+Animation: TypeAlias = Any
+
+XmlNode: TypeAlias = Any
+
```

### Comparing `types_wxpython-0.6.1/setup.py` & `types_wxpython-0.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,28 @@
  'wx-stubs.ribbon',
  'wx-stubs.richtext',
  'wx-stubs.stc',
  'wx-stubs.xml',
  'wx-stubs.xrc']
 
 package_data = \
-{'': ['*'], 'wx-stubs.lib': ['dialogs/*']}
+{'': ['*'],
+ 'wx-stubs': ['ActivateEvent/*',
+              'ConfigBase/*',
+              'DataObject/*',
+              'HelpEvent/*',
+              'StandardPaths/*',
+              'StaticBitmap/*',
+              'StockPreferencesPage/*'],
+ 'wx-stubs.grid': ['Grid/*', 'GridActivationSource/*'],
+ 'wx-stubs.lib': ['dialogs/*']}
 
 setup_kwargs = {
     'name': 'types-wxpython',
-    'version': '0.6.1',
+    'version': '0.7.0',
     'description': 'Typing stubs for wxPython',
     'long_description': '[![PyPI version](https://badge.fury.io/py/types-wxpython.svg)](https://badge.fury.io/py/types-wxpython)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-wxpython)\n![GitHub branch checks state](https://img.shields.io/github/checks-status/AlexionSoftware/types-wxpython/main)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/types-wxpython)\n![GitHub](https://img.shields.io/github/license/AlexionSoftware/types-wxpython)\n\n# Typing stubs for wxPython\nVersion: wxPython 4.2.0\n\nThis package contains typings stubs for [wxPython](https://pypi.org/project/wxPython/)\n\nThis package is not maintained by the maintainers of wxPython. This is made by users of wxPython.\n\nAny help is always welcome.\n',
     'author': 'Alexion Software',
     'author_email': 'info@alexion.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/AlexionSoftware/types-wxpython',
```

### Comparing `types_wxpython-0.6.1/PKG-INFO` & `types_wxpython-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-wxpython
-Version: 0.6.1
+Version: 0.7.0
 Summary: Typing stubs for wxPython
 Home-page: https://github.com/AlexionSoftware/types-wxpython
 License: MIT
 Keywords: wxPython,typing,stubs,wx
 Author: Alexion Software
 Author-email: info@alexion.nl
 Requires-Python: >=3.8.1,<4.0.0
```

