# Comparing `tmp/exn-0.0.6.tar.gz` & `tmp/exn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exn-0.0.6.tar", last modified: Sat Feb 25 02:28:54 2023, max compression
+gzip compressed data, was "dist/exn-0.0.7.tar", last modified: Thu May 18 18:01:34 2023, max compression
```

## Comparing `exn-0.0.6.tar` & `exn-0.0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.401833 exn-0.0.6/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2023-01-27 15:41:30.000000 exn-0.0.6/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       65 2022-05-20 19:28:46.000000 exn-0.0.6/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)    13694 2023-02-25 02:28:54.401833 exn-0.0.6/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)    13136 2023-02-25 02:27:18.000000 exn-0.0.6/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2023-02-25 02:22:28.000000 exn-0.0.6/VERSION
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.365849 exn-0.0.6/exn/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-12-13 20:40:48.000000 exn-0.0.6/exn/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     3085 2023-02-22 20:15:04.000000 exn-0.0.6/exn/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.369847 exn-0.0.6/exn/constant/
--rw-rw-r--   0 alex      (1002) alex      (1003)      225 2023-02-25 00:54:34.000000 exn-0.0.6/exn/constant/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.369847 exn-0.0.6/exn/dao/
--rw-rw-r--   0 alex      (1002) alex      (1003)     3272 2023-02-22 19:11:30.000000 exn-0.0.6/exn/dao/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.369847 exn-0.0.6/exn/dto/
--rw-rw-r--   0 alex      (1002) alex      (1003)      274 2022-12-16 11:07:37.000000 exn-0.0.6/exn/dto/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.369847 exn-0.0.6/exn/manager/
--rw-rw-r--   0 alex      (1002) alex      (1003)     5296 2023-02-22 20:05:35.000000 exn-0.0.6/exn/manager/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.369847 exn-0.0.6/exn/theme/
--rw-rw-r--   0 alex      (1002) alex      (1003)    27587 2023-02-22 20:05:35.000000 exn-0.0.6/exn/theme/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.369847 exn-0.0.6/exn/utils/
--rw-rw-r--   0 alex      (1002) alex      (1003)     4215 2023-02-22 20:15:03.000000 exn-0.0.6/exn/utils/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.401833 exn-0.0.6/exn/view/
--rw-rw-r--   0 alex      (1002) alex      (1003)      180 2023-01-07 08:25:20.000000 exn-0.0.6/exn/view/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2394 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/about.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     3909 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/board.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    13643 2023-02-19 13:35:55.000000 exn-0.0.6/exn/view/footer.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     3948 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/front.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4455 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/goto.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4912 2023-02-22 20:20:26.000000 exn-0.0.6/exn/view/info.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2128 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/past.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    15821 2023-02-22 20:20:03.000000 exn-0.0.6/exn/view/roll.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     9903 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/search.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2844 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/switcher.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     6450 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/toc.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     5880 2023-02-22 20:15:03.000000 exn-0.0.6/exn/view/top.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      690 2023-02-19 16:05:49.000000 exn-0.0.6/exn/view/util.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.369847 exn-0.0.6/exn.egg-info/
--rw-rw-r--   0 alex      (1002) alex      (1003)    13694 2023-02-25 02:28:54.000000 exn-0.0.6/exn.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)      695 2023-02-25 02:28:54.000000 exn-0.0.6/exn.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-02-25 02:28:54.000000 exn-0.0.6/exn.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       43 2023-02-25 02:28:54.000000 exn-0.0.6/exn.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-02-25 02:18:23.000000 exn-0.0.6/exn.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)       59 2023-02-25 02:28:54.000000 exn-0.0.6/exn.egg-info/requires.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       10 2023-02-25 02:28:54.000000 exn-0.0.6/exn.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:28:46.000000 exn-0.0.6/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      813 2023-02-25 02:28:54.405831 exn-0.0.6/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:28:46.000000 exn-0.0.6/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-02-25 02:28:54.401833 exn-0.0.6/tests/
--rw-rw-r--   0 alex      (1002) alex      (1003)        8 2023-02-20 09:02:12.000000 exn-0.0.6/tests/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.853100 exn-0.0.7/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2023-01-27 15:41:30.000000 exn-0.0.7/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       65 2022-05-20 19:28:46.000000 exn-0.0.7/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15602 2023-05-18 18:01:34.857100 exn-0.0.7/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15044 2023-02-28 20:51:27.000000 exn-0.0.7/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2023-02-25 02:28:54.000000 exn-0.0.7/VERSION
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.657099 exn-0.0.7/exn/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-12-13 20:40:48.000000 exn-0.0.7/exn/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3085 2023-02-22 20:15:04.000000 exn-0.0.7/exn/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.685099 exn-0.0.7/exn/constant/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      225 2023-02-25 00:54:34.000000 exn-0.0.7/exn/constant/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.709099 exn-0.0.7/exn/dao/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3287 2023-03-12 15:15:50.000000 exn-0.0.7/exn/dao/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.709099 exn-0.0.7/exn/dto/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      274 2022-12-16 11:07:37.000000 exn-0.0.7/exn/dto/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.717099 exn-0.0.7/exn/manager/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     5296 2023-02-22 20:05:35.000000 exn-0.0.7/exn/manager/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.725099 exn-0.0.7/exn/theme/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    27587 2023-02-22 20:05:35.000000 exn-0.0.7/exn/theme/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.733099 exn-0.0.7/exn/utils/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4215 2023-02-22 20:15:03.000000 exn-0.0.7/exn/utils/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.825100 exn-0.0.7/exn/view/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      180 2023-01-07 08:25:20.000000 exn-0.0.7/exn/view/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2394 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/about.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3909 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/board.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    13643 2023-02-19 13:35:55.000000 exn-0.0.7/exn/view/footer.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3948 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/front.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4455 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/goto.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4912 2023-02-22 20:20:26.000000 exn-0.0.7/exn/view/info.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2128 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/past.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15821 2023-02-22 20:20:03.000000 exn-0.0.7/exn/view/roll.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     9903 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/search.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2844 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/switcher.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     6450 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/toc.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     5880 2023-02-22 20:15:03.000000 exn-0.0.7/exn/view/top.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      690 2023-02-19 16:05:49.000000 exn-0.0.7/exn/view/util.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.685099 exn-0.0.7/exn.egg-info/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15602 2023-05-18 18:01:34.000000 exn-0.0.7/exn.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      695 2023-05-18 18:01:34.000000 exn-0.0.7/exn.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-05-18 18:01:34.000000 exn-0.0.7/exn.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       43 2023-05-18 18:01:34.000000 exn-0.0.7/exn.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-02-25 02:18:23.000000 exn-0.0.7/exn.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       59 2023-05-18 18:01:34.000000 exn-0.0.7/exn.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       10 2023-05-18 18:01:34.000000 exn-0.0.7/exn.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:28:46.000000 exn-0.0.7/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      813 2023-05-18 18:01:34.857100 exn-0.0.7/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:28:46.000000 exn-0.0.7/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:01:34.837100 exn-0.0.7/tests/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        8 2023-02-20 09:02:12.000000 exn-0.0.7/tests/__init__.py
```

### Comparing `exn-0.0.6/LICENSE` & `exn-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/PKG-INFO` & `exn-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exn
-Version: 0.0.6
+Version: 0.0.7
 Summary: Browse a dossier of exonotes
 Home-page: https://github.com/pyrustic/exn
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
@@ -15,81 +15,95 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- Cover -->
 <div align="center">
-    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/cover.png" alt="Demo" width="683">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/cover.png" alt="Demo" width="500">
     <p align="center">
-    Exn <a href="https://github.com/pyrustic/exn-demo">demo</a>
+    <a href="https://github.com/pyrustic/exn-demo/blob/master/home.exn">Home.exn</a> from the <a href="https://github.com/pyrustic/exn-demo">demo</a> dossier
     </p>
 </div>
 
-> **Note to HN user**: I plan to make a Show HN soon ! ;)
-
 
 <!-- Intro Text -->
 # Exonote / Exn
 <b> Write and render rich, scriptable, and interactive notes </b>
     
 This project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
 > [Installation](#installation) &nbsp; &nbsp; [Demo](#demo) &nbsp; &nbsp; [Latest](https://github.com/pyrustic/exn/tags) &nbsp; &nbsp; [Modules](https://github.com/pyrustic/exn/tree/master/docs/modules#readme)
 
 
 ## Table of contents
 
-
-[Overview](#overview)
-    
-[Why use this project ?](#why-use-this-project-)
-
-[Demo](#demo)
-
-[Markup language](#markup-language)
-
-[Command line interface](#command-line-interface)
-
-[Scripting with Python](#scripting-with-Python)
-
-[Viewer API](#viewer-api)
-
-[Embedding GUI programs](#embedding-gui-programs)
-
-[Key bindings](#key-bindings)
-
-[Miscellaneous](#miscellaneous)
-
-[Installation](#installation)
+- [Overview](#overview)
+- [Why not org-mode ?](#why-not-org-mode-)
+- [Why use this project ?](#why-use-this-project-)
+- [Demo](#demo)
+- [Markup language](#markup-language)
+- [Command line interface](#command-line-interface)
+- [Scripting with Python](#scripting-with-Python)
+- [Viewer API](#viewer-api)
+- [Embedding GUI programs](#embedding-gui-programs)
+- [Miscellaneous](#miscellaneous)
+- [Installation](#installation)
 
 
 # Overview
-Exn is a lightweight Python application for browsing a dossier of exonotes. An exonote is **plain text** written with an [eponymous](https://github.com/pyrustic/exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://www.python.org/downloads/)).
+**Exn** is a lightweight Python application for browsing a dossier of exonotes. An **exonote** is **plain text** written with an [eponymous](https://github.com/pyrustic/exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://www.python.org/downloads/)).
 
 **Interactivity** can be added to an exonote by **embedding GUI programs** written in Python with Tkinter. Additionally, all or part of an exonote can be arbitrarily generated using **custom Python scripts**.
 
-This application is built with the Gaspium framework and uses [Shared](https://github.com/pyrustic/shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to manipulate data.
+This application is built with the [Gaspium](https://github.com/pyrustic/gaspium) framework and uses [Shared](https://github.com/pyrustic/shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to manipulate data.
+
+This project is built on top of [Exonote](https://github.com/pyrustic/exonote). Solving issues in **Exonote** means improving **Exn**. Check the [issues](https://github.com/pyrustic/exonote/issues) !
 
 ## Dossier of exonotes
-A dossier is a directory containing exonotes and resources such as attachments and Python source code. At the root of a dossier should be an index file containing an ordered list of exonotes filenames, titles, and their associated tags. The index file is generated automatically by the `--build` command in the command line (the order is based on the creation timestamp of the exonotes).
+A **dossier** is a directory containing exonotes and resources such as attachments and Python source code. At the root of a dossier should be an index file containing an ordered list of exonotes filenames, titles, and their associated tags. The index file is generated automatically by the `--build` command in the command line (the order is based on the creation timestamp of the exonotes).
 
 Exn treats each exonote with the `.exn` extension as the page of a virtual book, so the graphical user interface of Exn is a metaphor for a book with controls to move from one page to the next or to the previous one.
 
 ## The Search feature
 Exn has a search interface that allows the user to search for exonotes in the dossier by specifying tags, words or a phrase. The search mechanism has an optional [regular expression](https://en.wikipedia.org/wiki/Regular_expression) mode.
 
+<div align="center">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/search.png" alt="Search" width="300">
+    <p align="center">
+    <b>Search</b> interface
+    </p>
+</div>
+
 ## On security: run untrusted exonotes
 The command line interface exposes two options for running exonotes:
 
 |Option|Description|
 |---|---|
 |`-r`, `--restrict [<filename>]`| Open a note with low restriction, i.e., block the execution of embedded programs|
 |`-R`, `--Restrict [<filename>]`| Open a note with high restriction, i.e., block executable links and also the execution of embedded programs|
 
 
+# Why not org-mode ?
+Exonote supports codeblocks like in Markdown. Instead of providing the ability to execute codeblocks, which would lead to [literate programming](https://en.wikipedia.org/wiki/Literate_programming) like in [Emacs](https://en.wikipedia.org/wiki/Emacs)' [org-mode](https://orgmode.org/), Exonote would execute a program whose source code is **properly written** elsewhere by calling a function with arguments.
+
+By **properly written** source code, I mean a regular Python [package](https://python-course.eu/python-tutorial/packages.php) with tree structure, modularity, Python `.py` file extension, et cetera. Thus, with a **minimalist** syntax, one can embed not only a program whose source code is written in a directory inside an exonotes dossier, but also a program whose distributable package is installed in the current Python [virtual environment](https://docs.python.org/3/library/venv.html). 
+
+I thought it would be nice to separate prose and source code and embed a program by simply referencing it with a minimalist syntax the same way an image is embedded in Markdown.
+
+This is how an image is embedded in Exonote:
+
+```
+@[title](path/to/img.png)
+```
+
+This is how a program is embedded in Exonote:
+```
+${path.to.module:functionOrClass arg1 arg2 "foo bar"}
+```
+
 # Why use this project ?
 Despite the existence of interesting note-taking solutions and the storm of AI-powered projects, there are compelling arguments for adopting Exonote and Exn. Let's explore some characteristics and concrete examples.
 
 ## Characteristics
 Here are some characteristics and their consequences:
 
 |Characteristic|Consequence|
@@ -102,15 +116,15 @@
 ## Examples
 These are few concrete examples of what can be done with Exonote and Exn:
 
 - create interactive courses;
 - build programming puzzles with levels and backstory;
 - make a [proof of concept](https://www.malwarebytes.com/glossary/proof-of-concept);
 - use the `exonote.Viewer` class to make rich and/or interactive documentation inside another application. Exn itself uses the default viewer in the Exonote library.
-- Whistleblowing and and censorship bypass: Due to its nature, a dossier of exonotes is very convenient for disclosing information that can be easily replicated and consumed by people.
+- Whistleblowing and censorship bypass: Due to its nature, a dossier of exonotes is very convenient for disclosing information that can be easily replicated and consumed by people.
 - Decent alternative to a personal website: it is as simple as creating a GitHub repository, upload a dossier of exonote, share the link with readers, then regularly update the contents with `git commit`.
 
 > **Note**: you can define a `blocklist` file in `$dossier/.exn` to block access to a list of exonotes (filenames). This mechanism with the help of custom scripts, allows the implementation of a system of levels where certain conditions must be met before opening specific exonotes.
 
 # Demo
 A [demo](https://github.com/pyrustic/exn-demo) is available that you can play with. You will need to clone the demo repository, install Exn with [pip](https://en.wikipedia.org/wiki/Pip_(package_manager)) and then run it without any arguments. By default, it executes the last exonote opened or runs the home page (first exonote referenced in the index).
 
@@ -251,14 +265,17 @@
 # Miscellaneous
 
 ## Keymap
 For a smooth user experience, keyboard keys are mapped to certain functions in Exn. For example, pressing `F` would activate the `Find in Page` functionality. Pressing `H` would open the home page. Pressing `S` would open the search interface. Pressing `T` would open the table of contents. Pressing `F5` would refresh the page. Et cetera.
 
 > **Note:** `Ctrl+Tab` will open the **switcher** to allow you to go back to the previously opened exonote.
 
+## Quick-copy
+Quickly copy the contents of a codeblock or the address of a link with a right-click over it !
+
 ## Attachments
 For the moments only images are supported.
 
 ## Path separator
 The separator symbol inside the path to an exonote or asset is the slash `/` symbol. Also, a path must not start with a separator.
 
 ## Filenames
```

#### html2text {}

```diff
@@ -1,101 +1,124 @@
-Metadata-Version: 2.1 Name: exn Version: 0.0.6 Summary: Browse a dossier of
+Metadata-Version: 2.1 Name: exn Version: 0.0.7 Summary: Browse a dossier of
 exonotes Home-page: https://github.com/pyrustic/exn Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com Maintainer: Pyrustic Evangelist Maintainer-
 email: rusticalex@yahoo.com License: MIT Keywords: application,pyrustic
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.5 Description-Content-Type: text/markdown
 License-File: LICENSE
                                     [Demo]
-                                   Exn demo
-> **Note to HN user**: I plan to make a Show HN soon ! ;)  # Exonote / Exn
-Write and render rich, scriptable, and interactive notes This project is part
-of the [Pyrustic Open Ecosystem](https://pyrustic.github.io). > [Installation]
-(#installation)     [Demo](#demo)     [Latest](https://github.com/pyrustic/exn/
-tags)     [Modules](https://github.com/pyrustic/exn/tree/master/docs/
-modules#readme) ## Table of contents [Overview](#overview) [Why use this
-project ?](#why-use-this-project-) [Demo](#demo) [Markup language](#markup-
-language) [Command line interface](#command-line-interface) [Scripting with
-Python](#scripting-with-Python) [Viewer API](#viewer-api) [Embedding GUI
-programs](#embedding-gui-programs) [Key bindings](#key-bindings)
-[Miscellaneous](#miscellaneous) [Installation](#installation) # Overview Exn is
-a lightweight Python application for browsing a dossier of exonotes. An exonote
-is **plain text** written with an [eponymous](https://github.com/pyrustic/
-exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/
-Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter)
-(the default GUI library for [Python](https://www.python.org/downloads/)).
-**Interactivity** can be added to an exonote by **embedding GUI programs**
-written in Python with Tkinter. Additionally, all or part of an exonote can be
-arbitrarily generated using **custom Python scripts**. This application is
-built with the Gaspium framework and uses [Shared](https://github.com/pyrustic/
+                        Home.exn from the demo dossier
+ # Exonote / Exn Write and render rich, scriptable, and interactive notes This
+project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io). >
+[Installation](#installation)     [Demo](#demo)     [Latest](https://
+github.com/pyrustic/exn/tags)     [Modules](https://github.com/pyrustic/exn/
+tree/master/docs/modules#readme) ## Table of contents - [Overview](#overview) -
+[Why not org-mode ?](#why-not-org-mode-) - [Why use this project ?](#why-use-
+this-project-) - [Demo](#demo) - [Markup language](#markup-language) - [Command
+line interface](#command-line-interface) - [Scripting with Python](#scripting-
+with-Python) - [Viewer API](#viewer-api) - [Embedding GUI programs](#embedding-
+gui-programs) - [Miscellaneous](#miscellaneous) - [Installation](#installation)
+# Overview **Exn** is a lightweight Python application for browsing a dossier
+of exonotes. An **exonote** is **plain text** written with an [eponymous]
+(https://github.com/pyrustic/exonote) markup language inspired by [Markdown]
+(https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://
+en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://
+www.python.org/downloads/)). **Interactivity** can be added to an exonote by
+**embedding GUI programs** written in Python with Tkinter. Additionally, all or
+part of an exonote can be arbitrarily generated using **custom Python
+scripts**. This application is built with the [Gaspium](https://github.com/
+pyrustic/gaspium) framework and uses [Shared](https://github.com/pyrustic/
 shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to
-manipulate data. ## Dossier of exonotes A dossier is a directory containing
-exonotes and resources such as attachments and Python source code. At the root
-of a dossier should be an index file containing an ordered list of exonotes
-filenames, titles, and their associated tags. The index file is generated
-automatically by the `--build` command in the command line (the order is based
-on the creation timestamp of the exonotes). Exn treats each exonote with the
-`.exn` extension as the page of a virtual book, so the graphical user interface
-of Exn is a metaphor for a book with controls to move from one page to the next
-or to the previous one. ## The Search feature Exn has a search interface that
-allows the user to search for exonotes in the dossier by specifying tags, words
-or a phrase. The search mechanism has an optional [regular expression](https://
-en.wikipedia.org/wiki/Regular_expression) mode. ## On security: run untrusted
-exonotes The command line interface exposes two options for running exonotes:
-|Option|Description| |---|---| |`-r`, `--restrict []`| Open a note with low
-restriction, i.e., block the execution of embedded programs| |`-R`, `--Restrict
-[]`| Open a note with high restriction, i.e., block executable links and also
-the execution of embedded programs| # Why use this project ? Despite the
-existence of interesting note-taking solutions and the storm of AI-powered
-projects, there are compelling arguments for adopting Exonote and Exn. Let's
-explore some characteristics and concrete examples. ## Characteristics Here are
-some characteristics and their consequences: |Characteristic|Consequence| |---
-|---| |Plain old text file|Since an exonote is just plain text, you can always
-use your favorite text editor (Vim, Sublime Text, Visual Studio Code, et
-cetera) to write your notes. Exonotes are also de facto compatible with [VCS]
-(https://en.wikipedia.org/wiki/Version_control).| |Minimalism|Exonote's
-minimalist markup language specification made Tkinter a good candidate to
-render it, eliminating the need for web-based technology (browser, html, css,
-et cetera). Hence, we got Exn, a lightweight, cross-platform app to view
-exonotes.| |Scripting with Python|Python is one of the [most popular](https://
-www.wired.com/story/python-language-more-popular-than-ever/) programming
-languages in the world. Since people like to tinker with Python, it would be
-fun to write scripts with this language for personal exonotes.| |Embed GUI
-programs written with Tkinter|[Tcl/Tk](https://www.tcl.tk/) is one of the
-easiest GUI toolkits to use, unsurprisingly, it's the default solution for GUI
-programming in Python via Tkinter. In the demo, a working calculator was built
-with Tkinter and embedded into an exonote.| ## Examples These are few concrete
-examples of what can be done with Exonote and Exn: - create interactive
-courses; - build programming puzzles with levels and backstory; - make a [proof
-of concept](https://www.malwarebytes.com/glossary/proof-of-concept); - use the
-`exonote.Viewer` class to make rich and/or interactive documentation inside
-another application. Exn itself uses the default viewer in the Exonote library.
-- Whistleblowing and and censorship bypass: Due to its nature, a dossier of
-exonotes is very convenient for disclosing information that can be easily
-replicated and consumed by people. - Decent alternative to a personal website:
-it is as simple as creating a GitHub repository, upload a dossier of exonote,
-share the link with readers, then regularly update the contents with `git
-commit`. > **Note**: you can define a `blocklist` file in `$dossier/.exn` to
-block access to a list of exonotes (filenames). This mechanism with the help of
-custom scripts, allows the implementation of a system of levels where certain
-conditions must be met before opening specific exonotes. # Demo A [demo](https:
-//github.com/pyrustic/exn-demo) is available that you can play with. You will
-need to clone the demo repository, install Exn with [pip](https://
-en.wikipedia.org/wiki/Pip_(package_manager)) and then run it without any
-arguments. By default, it executes the last exonote opened or runs the home
-page (first exonote referenced in the index). ```bash # 1- clone the repository
-$ git clone https://github.com/pyrustic/exn-demo $ cd exn-demo # 2- install exn
-$ pip install exn # 3- run exn with zero restriction $ exn ``` You can still
-run Exn with restriction: ```bash # run exn with low restriction $ exn -r # run
-exn with high restriction $ exn -R ``` # Markup language |Element|Description|
-|---|---| |ANCHOR|Create an anchor in a specific location of an exonote that
-can be accessed when its name is appended to the filename of the exonote.
-Syntax: ``| |ATTACHMENT|Insert an asset like an image. Syntax: `@[optional
-text](path/to/assets/resource.png)`| |BOLD|Make a text bold. Syntax: `*bold*`|
+manipulate data. This project is built on top of [Exonote](https://github.com/
+pyrustic/exonote). Solving issues in **Exonote** means improving **Exn**. Check
+the [issues](https://github.com/pyrustic/exonote/issues) ! ## Dossier of
+exonotes A **dossier** is a directory containing exonotes and resources such as
+attachments and Python source code. At the root of a dossier should be an index
+file containing an ordered list of exonotes filenames, titles, and their
+associated tags. The index file is generated automatically by the `--build`
+command in the command line (the order is based on the creation timestamp of
+the exonotes). Exn treats each exonote with the `.exn` extension as the page of
+a virtual book, so the graphical user interface of Exn is a metaphor for a book
+with controls to move from one page to the next or to the previous one. ## The
+Search feature Exn has a search interface that allows the user to search for
+exonotes in the dossier by specifying tags, words or a phrase. The search
+mechanism has an optional [regular expression](https://en.wikipedia.org/wiki/
+Regular_expression) mode.
+                                   [Search]
+                               Search interface
+## On security: run untrusted exonotes The command line interface exposes two
+options for running exonotes: |Option|Description| |---|---| |`-r`, `--restrict
+[]`| Open a note with low restriction, i.e., block the execution of embedded
+programs| |`-R`, `--Restrict []`| Open a note with high restriction, i.e.,
+block executable links and also the execution of embedded programs| # Why not
+org-mode ? Exonote supports codeblocks like in Markdown. Instead of providing
+the ability to execute codeblocks, which would lead to [literate programming]
+(https://en.wikipedia.org/wiki/Literate_programming) like in [Emacs](https://
+en.wikipedia.org/wiki/Emacs)' [org-mode](https://orgmode.org/), Exonote would
+execute a program whose source code is **properly written** elsewhere by
+calling a function with arguments. By **properly written** source code, I mean
+a regular Python [package](https://python-course.eu/python-tutorial/
+packages.php) with tree structure, modularity, Python `.py` file extension, et
+cetera. Thus, with a **minimalist** syntax, one can embed not only a program
+whose source code is written in a directory inside an exonotes dossier, but
+also a program whose distributable package is installed in the current Python
+[virtual environment](https://docs.python.org/3/library/venv.html). I thought
+it would be nice to separate prose and source code and embed a program by
+simply referencing it with a minimalist syntax the same way an image is
+embedded in Markdown. This is how an image is embedded in Exonote: ``` @[title]
+(path/to/img.png) ``` This is how a program is embedded in Exonote: ``` $
+{path.to.module:functionOrClass arg1 arg2 "foo bar"} ``` # Why use this project
+? Despite the existence of interesting note-taking solutions and the storm of
+AI-powered projects, there are compelling arguments for adopting Exonote and
+Exn. Let's explore some characteristics and concrete examples. ##
+Characteristics Here are some characteristics and their consequences:
+|Characteristic|Consequence| |---|---| |Plain old text file|Since an exonote is
+just plain text, you can always use your favorite text editor (Vim, Sublime
+Text, Visual Studio Code, et cetera) to write your notes. Exonotes are also de
+facto compatible with [VCS](https://en.wikipedia.org/wiki/Version_control).|
+|Minimalism|Exonote's minimalist markup language specification made Tkinter a
+good candidate to render it, eliminating the need for web-based technology
+(browser, html, css, et cetera). Hence, we got Exn, a lightweight, cross-
+platform app to view exonotes.| |Scripting with Python|Python is one of the
+[most popular](https://www.wired.com/story/python-language-more-popular-than-
+ever/) programming languages in the world. Since people like to tinker with
+Python, it would be fun to write scripts with this language for personal
+exonotes.| |Embed GUI programs written with Tkinter|[Tcl/Tk](https://
+www.tcl.tk/) is one of the easiest GUI toolkits to use, unsurprisingly, it's
+the default solution for GUI programming in Python via Tkinter. In the demo, a
+working calculator was built with Tkinter and embedded into an exonote.| ##
+Examples These are few concrete examples of what can be done with Exonote and
+Exn: - create interactive courses; - build programming puzzles with levels and
+backstory; - make a [proof of concept](https://www.malwarebytes.com/glossary/
+proof-of-concept); - use the `exonote.Viewer` class to make rich and/or
+interactive documentation inside another application. Exn itself uses the
+default viewer in the Exonote library. - Whistleblowing and censorship bypass:
+Due to its nature, a dossier of exonotes is very convenient for disclosing
+information that can be easily replicated and consumed by people. - Decent
+alternative to a personal website: it is as simple as creating a GitHub
+repository, upload a dossier of exonote, share the link with readers, then
+regularly update the contents with `git commit`. > **Note**: you can define a
+`blocklist` file in `$dossier/.exn` to block access to a list of exonotes
+(filenames). This mechanism with the help of custom scripts, allows the
+implementation of a system of levels where certain conditions must be met
+before opening specific exonotes. # Demo A [demo](https://github.com/pyrustic/
+exn-demo) is available that you can play with. You will need to clone the demo
+repository, install Exn with [pip](https://en.wikipedia.org/wiki/Pip_
+(package_manager)) and then run it without any arguments. By default, it
+executes the last exonote opened or runs the home page (first exonote
+referenced in the index). ```bash # 1- clone the repository $ git clone https:/
+/github.com/pyrustic/exn-demo $ cd exn-demo # 2- install exn $ pip install exn
+# 3- run exn with zero restriction $ exn ``` You can still run Exn with
+restriction: ```bash # run exn with low restriction $ exn -r # run exn with
+high restriction $ exn -R ``` # Markup language |Element|Description| |---|---
+| |ANCHOR|Create an anchor in a specific location of an exonote that can be
+accessed when its name is appended to the filename of the exonote. Syntax: ``|
+|ATTACHMENT|Insert an asset like an image. Syntax: `@[optional text](path/to/
+assets/resource.png)`| |BOLD|Make a text bold. Syntax: `*bold*`|
 |CODE|Surrounding a word or phrase with double backticks will apply a monospace
 font to it and also a colored background.| |CODEBLOCK|Same as in Markdown|
 |DINKUS|Three asterisks at the start of a blank will be centered and bolded
 like a [dinkus](https://en.wikipedia.org/wiki/Dinkus).| |GAP|Leave at least one
 blank line between a group de sentences to create paragraphs.| |HEADING|An
 exonote is made up of sections, which are made up of paragraphs. A section
 title is the Heading and it a section can have an identifier (section id,
@@ -151,30 +174,31 @@
                                                                     Back_to_top
 # Miscellaneous ## Keymap For a smooth user experience, keyboard keys are
 mapped to certain functions in Exn. For example, pressing `F` would activate
 the `Find in Page` functionality. Pressing `H` would open the home page.
 Pressing `S` would open the search interface. Pressing `T` would open the table
 of contents. Pressing `F5` would refresh the page. Et cetera. > **Note:**
 `Ctrl+Tab` will open the **switcher** to allow you to go back to the previously
-opened exonote. ## Attachments For the moments only images are supported. ##
-Path separator The separator symbol inside the path to an exonote or asset is
-the slash `/` symbol. Also, a path must not start with a separator. ##
-Filenames Exn only recognizes files with the extension `.exn`. Also, to
-reference a specific filename as a link in an exonote, you must write its path
-relative to the root of the folder. Filename and Path can be used as synonyms.
-Example: ``` dossier exonote1.exn exonote2.exn folder exonote3.exn ``` The path
-to `exonote3.exn` is `folder/exonote3.exn` ## The context object The context
-object is a namedtuple instance whose fields are: - viewer: the
-`exonote.Viewer` instance which exposes the API to manipulate the
-representation of the currently displayed exonote; - arguments: list of
-arguments passed to this function in the exonote. ## ASCII Art The ASCII Art at
-the beginning of the CLI help text is made with [patorjk's TAAG](https://
-patorjk.com/software/taag/#p=display&f=Roman&t=E%20X%20N) # Installation
-**Exn** is **cross platform** and versions under **1.0.0** will be considered
-**Beta** at best. It is built on [Ubuntu](https://ubuntu.com/download/desktop)
-with [Python 3.8](https://www.python.org/downloads/) and should work on
-**Python 3.5** or **newer**. ## For the first time ```bash $ pip install exn
-``` ## Upgrade ```bash $ pip install exn --upgrade --upgrade-strategy eager ```
-
+opened exonote. ## Quick-copy Quickly copy the contents of a codeblock or the
+address of a link with a right-click over it ! ## Attachments For the moments
+only images are supported. ## Path separator The separator symbol inside the
+path to an exonote or asset is the slash `/` symbol. Also, a path must not
+start with a separator. ## Filenames Exn only recognizes files with the
+extension `.exn`. Also, to reference a specific filename as a link in an
+exonote, you must write its path relative to the root of the folder. Filename
+and Path can be used as synonyms. Example: ``` dossier exonote1.exn
+exonote2.exn folder exonote3.exn ``` The path to `exonote3.exn` is `folder/
+exonote3.exn` ## The context object The context object is a namedtuple instance
+whose fields are: - viewer: the `exonote.Viewer` instance which exposes the API
+to manipulate the representation of the currently displayed exonote; -
+arguments: list of arguments passed to this function in the exonote. ## ASCII
+Art The ASCII Art at the beginning of the CLI help text is made with [patorjk's
+TAAG](https://patorjk.com/software/taag/#p=display&f=Roman&t=E%20X%20N) #
+Installation **Exn** is **cross platform** and versions under **1.0.0** will be
+considered **Beta** at best. It is built on [Ubuntu](https://ubuntu.com/
+download/desktop) with [Python 3.8](https://www.python.org/downloads/) and
+should work on **Python 3.5** or **newer**. ## For the first time ```bash $ pip
+install exn ``` ## Upgrade ```bash $ pip install exn --upgrade --upgrade-
+strategy eager ```
 
 
 [Back to top](#readme)
```

### Comparing `exn-0.0.6/README.md` & `exn-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,90 @@
 <!-- Cover -->
 <div align="center">
-    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/cover.png" alt="Demo" width="683">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/cover.png" alt="Demo" width="500">
     <p align="center">
-    Exn <a href="https://github.com/pyrustic/exn-demo">demo</a>
+    <a href="https://github.com/pyrustic/exn-demo/blob/master/home.exn">Home.exn</a> from the <a href="https://github.com/pyrustic/exn-demo">demo</a> dossier
     </p>
 </div>
 
-> **Note to HN user**: I plan to make a Show HN soon ! ;)
-
 
 <!-- Intro Text -->
 # Exonote / Exn
 <b> Write and render rich, scriptable, and interactive notes </b>
     
 This project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
 > [Installation](#installation) &nbsp; &nbsp; [Demo](#demo) &nbsp; &nbsp; [Latest](https://github.com/pyrustic/exn/tags) &nbsp; &nbsp; [Modules](https://github.com/pyrustic/exn/tree/master/docs/modules#readme)
 
 
 ## Table of contents
 
-
-[Overview](#overview)
-    
-[Why use this project ?](#why-use-this-project-)
-
-[Demo](#demo)
-
-[Markup language](#markup-language)
-
-[Command line interface](#command-line-interface)
-
-[Scripting with Python](#scripting-with-Python)
-
-[Viewer API](#viewer-api)
-
-[Embedding GUI programs](#embedding-gui-programs)
-
-[Key bindings](#key-bindings)
-
-[Miscellaneous](#miscellaneous)
-
-[Installation](#installation)
+- [Overview](#overview)
+- [Why not org-mode ?](#why-not-org-mode-)
+- [Why use this project ?](#why-use-this-project-)
+- [Demo](#demo)
+- [Markup language](#markup-language)
+- [Command line interface](#command-line-interface)
+- [Scripting with Python](#scripting-with-Python)
+- [Viewer API](#viewer-api)
+- [Embedding GUI programs](#embedding-gui-programs)
+- [Miscellaneous](#miscellaneous)
+- [Installation](#installation)
 
 
 # Overview
-Exn is a lightweight Python application for browsing a dossier of exonotes. An exonote is **plain text** written with an [eponymous](https://github.com/pyrustic/exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://www.python.org/downloads/)).
+**Exn** is a lightweight Python application for browsing a dossier of exonotes. An **exonote** is **plain text** written with an [eponymous](https://github.com/pyrustic/exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://www.python.org/downloads/)).
 
 **Interactivity** can be added to an exonote by **embedding GUI programs** written in Python with Tkinter. Additionally, all or part of an exonote can be arbitrarily generated using **custom Python scripts**.
 
-This application is built with the Gaspium framework and uses [Shared](https://github.com/pyrustic/shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to manipulate data.
+This application is built with the [Gaspium](https://github.com/pyrustic/gaspium) framework and uses [Shared](https://github.com/pyrustic/shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to manipulate data.
+
+This project is built on top of [Exonote](https://github.com/pyrustic/exonote). Solving issues in **Exonote** means improving **Exn**. Check the [issues](https://github.com/pyrustic/exonote/issues) !
 
 ## Dossier of exonotes
-A dossier is a directory containing exonotes and resources such as attachments and Python source code. At the root of a dossier should be an index file containing an ordered list of exonotes filenames, titles, and their associated tags. The index file is generated automatically by the `--build` command in the command line (the order is based on the creation timestamp of the exonotes).
+A **dossier** is a directory containing exonotes and resources such as attachments and Python source code. At the root of a dossier should be an index file containing an ordered list of exonotes filenames, titles, and their associated tags. The index file is generated automatically by the `--build` command in the command line (the order is based on the creation timestamp of the exonotes).
 
 Exn treats each exonote with the `.exn` extension as the page of a virtual book, so the graphical user interface of Exn is a metaphor for a book with controls to move from one page to the next or to the previous one.
 
 ## The Search feature
 Exn has a search interface that allows the user to search for exonotes in the dossier by specifying tags, words or a phrase. The search mechanism has an optional [regular expression](https://en.wikipedia.org/wiki/Regular_expression) mode.
 
+<div align="center">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/search.png" alt="Search" width="300">
+    <p align="center">
+    <b>Search</b> interface
+    </p>
+</div>
+
 ## On security: run untrusted exonotes
 The command line interface exposes two options for running exonotes:
 
 |Option|Description|
 |---|---|
 |`-r`, `--restrict [<filename>]`| Open a note with low restriction, i.e., block the execution of embedded programs|
 |`-R`, `--Restrict [<filename>]`| Open a note with high restriction, i.e., block executable links and also the execution of embedded programs|
 
 
+# Why not org-mode ?
+Exonote supports codeblocks like in Markdown. Instead of providing the ability to execute codeblocks, which would lead to [literate programming](https://en.wikipedia.org/wiki/Literate_programming) like in [Emacs](https://en.wikipedia.org/wiki/Emacs)' [org-mode](https://orgmode.org/), Exonote would execute a program whose source code is **properly written** elsewhere by calling a function with arguments.
+
+By **properly written** source code, I mean a regular Python [package](https://python-course.eu/python-tutorial/packages.php) with tree structure, modularity, Python `.py` file extension, et cetera. Thus, with a **minimalist** syntax, one can embed not only a program whose source code is written in a directory inside an exonotes dossier, but also a program whose distributable package is installed in the current Python [virtual environment](https://docs.python.org/3/library/venv.html). 
+
+I thought it would be nice to separate prose and source code and embed a program by simply referencing it with a minimalist syntax the same way an image is embedded in Markdown.
+
+This is how an image is embedded in Exonote:
+
+```
+@[title](path/to/img.png)
+```
+
+This is how a program is embedded in Exonote:
+```
+${path.to.module:functionOrClass arg1 arg2 "foo bar"}
+```
+
 # Why use this project ?
 Despite the existence of interesting note-taking solutions and the storm of AI-powered projects, there are compelling arguments for adopting Exonote and Exn. Let's explore some characteristics and concrete examples.
 
 ## Characteristics
 Here are some characteristics and their consequences:
 
 |Characteristic|Consequence|
@@ -83,15 +97,15 @@
 ## Examples
 These are few concrete examples of what can be done with Exonote and Exn:
 
 - create interactive courses;
 - build programming puzzles with levels and backstory;
 - make a [proof of concept](https://www.malwarebytes.com/glossary/proof-of-concept);
 - use the `exonote.Viewer` class to make rich and/or interactive documentation inside another application. Exn itself uses the default viewer in the Exonote library.
-- Whistleblowing and and censorship bypass: Due to its nature, a dossier of exonotes is very convenient for disclosing information that can be easily replicated and consumed by people.
+- Whistleblowing and censorship bypass: Due to its nature, a dossier of exonotes is very convenient for disclosing information that can be easily replicated and consumed by people.
 - Decent alternative to a personal website: it is as simple as creating a GitHub repository, upload a dossier of exonote, share the link with readers, then regularly update the contents with `git commit`.
 
 > **Note**: you can define a `blocklist` file in `$dossier/.exn` to block access to a list of exonotes (filenames). This mechanism with the help of custom scripts, allows the implementation of a system of levels where certain conditions must be met before opening specific exonotes.
 
 # Demo
 A [demo](https://github.com/pyrustic/exn-demo) is available that you can play with. You will need to clone the demo repository, install Exn with [pip](https://en.wikipedia.org/wiki/Pip_(package_manager)) and then run it without any arguments. By default, it executes the last exonote opened or runs the home page (first exonote referenced in the index).
 
@@ -232,14 +246,17 @@
 # Miscellaneous
 
 ## Keymap
 For a smooth user experience, keyboard keys are mapped to certain functions in Exn. For example, pressing `F` would activate the `Find in Page` functionality. Pressing `H` would open the home page. Pressing `S` would open the search interface. Pressing `T` would open the table of contents. Pressing `F5` would refresh the page. Et cetera.
 
 > **Note:** `Ctrl+Tab` will open the **switcher** to allow you to go back to the previously opened exonote.
 
+## Quick-copy
+Quickly copy the contents of a codeblock or the address of a link with a right-click over it !
+
 ## Attachments
 For the moments only images are supported.
 
 ## Path separator
 The separator symbol inside the path to an exonote or asset is the slash `/` symbol. Also, a path must not start with a separator.
 
 ## Filenames
```

#### html2text {}

```diff
@@ -1,93 +1,116 @@
                                     [Demo]
-                                   Exn demo
-> **Note to HN user**: I plan to make a Show HN soon ! ;)  # Exonote / Exn
-Write and render rich, scriptable, and interactive notes This project is part
-of the [Pyrustic Open Ecosystem](https://pyrustic.github.io). > [Installation]
-(#installation)     [Demo](#demo)     [Latest](https://github.com/pyrustic/exn/
-tags)     [Modules](https://github.com/pyrustic/exn/tree/master/docs/
-modules#readme) ## Table of contents [Overview](#overview) [Why use this
-project ?](#why-use-this-project-) [Demo](#demo) [Markup language](#markup-
-language) [Command line interface](#command-line-interface) [Scripting with
-Python](#scripting-with-Python) [Viewer API](#viewer-api) [Embedding GUI
-programs](#embedding-gui-programs) [Key bindings](#key-bindings)
-[Miscellaneous](#miscellaneous) [Installation](#installation) # Overview Exn is
-a lightweight Python application for browsing a dossier of exonotes. An exonote
-is **plain text** written with an [eponymous](https://github.com/pyrustic/
-exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/
-Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter)
-(the default GUI library for [Python](https://www.python.org/downloads/)).
-**Interactivity** can be added to an exonote by **embedding GUI programs**
-written in Python with Tkinter. Additionally, all or part of an exonote can be
-arbitrarily generated using **custom Python scripts**. This application is
-built with the Gaspium framework and uses [Shared](https://github.com/pyrustic/
+                        Home.exn from the demo dossier
+ # Exonote / Exn Write and render rich, scriptable, and interactive notes This
+project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io). >
+[Installation](#installation)     [Demo](#demo)     [Latest](https://
+github.com/pyrustic/exn/tags)     [Modules](https://github.com/pyrustic/exn/
+tree/master/docs/modules#readme) ## Table of contents - [Overview](#overview) -
+[Why not org-mode ?](#why-not-org-mode-) - [Why use this project ?](#why-use-
+this-project-) - [Demo](#demo) - [Markup language](#markup-language) - [Command
+line interface](#command-line-interface) - [Scripting with Python](#scripting-
+with-Python) - [Viewer API](#viewer-api) - [Embedding GUI programs](#embedding-
+gui-programs) - [Miscellaneous](#miscellaneous) - [Installation](#installation)
+# Overview **Exn** is a lightweight Python application for browsing a dossier
+of exonotes. An **exonote** is **plain text** written with an [eponymous]
+(https://github.com/pyrustic/exonote) markup language inspired by [Markdown]
+(https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://
+en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://
+www.python.org/downloads/)). **Interactivity** can be added to an exonote by
+**embedding GUI programs** written in Python with Tkinter. Additionally, all or
+part of an exonote can be arbitrarily generated using **custom Python
+scripts**. This application is built with the [Gaspium](https://github.com/
+pyrustic/gaspium) framework and uses [Shared](https://github.com/pyrustic/
 shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to
-manipulate data. ## Dossier of exonotes A dossier is a directory containing
-exonotes and resources such as attachments and Python source code. At the root
-of a dossier should be an index file containing an ordered list of exonotes
-filenames, titles, and their associated tags. The index file is generated
-automatically by the `--build` command in the command line (the order is based
-on the creation timestamp of the exonotes). Exn treats each exonote with the
-`.exn` extension as the page of a virtual book, so the graphical user interface
-of Exn is a metaphor for a book with controls to move from one page to the next
-or to the previous one. ## The Search feature Exn has a search interface that
-allows the user to search for exonotes in the dossier by specifying tags, words
-or a phrase. The search mechanism has an optional [regular expression](https://
-en.wikipedia.org/wiki/Regular_expression) mode. ## On security: run untrusted
-exonotes The command line interface exposes two options for running exonotes:
-|Option|Description| |---|---| |`-r`, `--restrict []`| Open a note with low
-restriction, i.e., block the execution of embedded programs| |`-R`, `--Restrict
-[]`| Open a note with high restriction, i.e., block executable links and also
-the execution of embedded programs| # Why use this project ? Despite the
-existence of interesting note-taking solutions and the storm of AI-powered
-projects, there are compelling arguments for adopting Exonote and Exn. Let's
-explore some characteristics and concrete examples. ## Characteristics Here are
-some characteristics and their consequences: |Characteristic|Consequence| |---
-|---| |Plain old text file|Since an exonote is just plain text, you can always
-use your favorite text editor (Vim, Sublime Text, Visual Studio Code, et
-cetera) to write your notes. Exonotes are also de facto compatible with [VCS]
-(https://en.wikipedia.org/wiki/Version_control).| |Minimalism|Exonote's
-minimalist markup language specification made Tkinter a good candidate to
-render it, eliminating the need for web-based technology (browser, html, css,
-et cetera). Hence, we got Exn, a lightweight, cross-platform app to view
-exonotes.| |Scripting with Python|Python is one of the [most popular](https://
-www.wired.com/story/python-language-more-popular-than-ever/) programming
-languages in the world. Since people like to tinker with Python, it would be
-fun to write scripts with this language for personal exonotes.| |Embed GUI
-programs written with Tkinter|[Tcl/Tk](https://www.tcl.tk/) is one of the
-easiest GUI toolkits to use, unsurprisingly, it's the default solution for GUI
-programming in Python via Tkinter. In the demo, a working calculator was built
-with Tkinter and embedded into an exonote.| ## Examples These are few concrete
-examples of what can be done with Exonote and Exn: - create interactive
-courses; - build programming puzzles with levels and backstory; - make a [proof
-of concept](https://www.malwarebytes.com/glossary/proof-of-concept); - use the
-`exonote.Viewer` class to make rich and/or interactive documentation inside
-another application. Exn itself uses the default viewer in the Exonote library.
-- Whistleblowing and and censorship bypass: Due to its nature, a dossier of
-exonotes is very convenient for disclosing information that can be easily
-replicated and consumed by people. - Decent alternative to a personal website:
-it is as simple as creating a GitHub repository, upload a dossier of exonote,
-share the link with readers, then regularly update the contents with `git
-commit`. > **Note**: you can define a `blocklist` file in `$dossier/.exn` to
-block access to a list of exonotes (filenames). This mechanism with the help of
-custom scripts, allows the implementation of a system of levels where certain
-conditions must be met before opening specific exonotes. # Demo A [demo](https:
-//github.com/pyrustic/exn-demo) is available that you can play with. You will
-need to clone the demo repository, install Exn with [pip](https://
-en.wikipedia.org/wiki/Pip_(package_manager)) and then run it without any
-arguments. By default, it executes the last exonote opened or runs the home
-page (first exonote referenced in the index). ```bash # 1- clone the repository
-$ git clone https://github.com/pyrustic/exn-demo $ cd exn-demo # 2- install exn
-$ pip install exn # 3- run exn with zero restriction $ exn ``` You can still
-run Exn with restriction: ```bash # run exn with low restriction $ exn -r # run
-exn with high restriction $ exn -R ``` # Markup language |Element|Description|
-|---|---| |ANCHOR|Create an anchor in a specific location of an exonote that
-can be accessed when its name is appended to the filename of the exonote.
-Syntax: ``| |ATTACHMENT|Insert an asset like an image. Syntax: `@[optional
-text](path/to/assets/resource.png)`| |BOLD|Make a text bold. Syntax: `*bold*`|
+manipulate data. This project is built on top of [Exonote](https://github.com/
+pyrustic/exonote). Solving issues in **Exonote** means improving **Exn**. Check
+the [issues](https://github.com/pyrustic/exonote/issues) ! ## Dossier of
+exonotes A **dossier** is a directory containing exonotes and resources such as
+attachments and Python source code. At the root of a dossier should be an index
+file containing an ordered list of exonotes filenames, titles, and their
+associated tags. The index file is generated automatically by the `--build`
+command in the command line (the order is based on the creation timestamp of
+the exonotes). Exn treats each exonote with the `.exn` extension as the page of
+a virtual book, so the graphical user interface of Exn is a metaphor for a book
+with controls to move from one page to the next or to the previous one. ## The
+Search feature Exn has a search interface that allows the user to search for
+exonotes in the dossier by specifying tags, words or a phrase. The search
+mechanism has an optional [regular expression](https://en.wikipedia.org/wiki/
+Regular_expression) mode.
+                                   [Search]
+                               Search interface
+## On security: run untrusted exonotes The command line interface exposes two
+options for running exonotes: |Option|Description| |---|---| |`-r`, `--restrict
+[]`| Open a note with low restriction, i.e., block the execution of embedded
+programs| |`-R`, `--Restrict []`| Open a note with high restriction, i.e.,
+block executable links and also the execution of embedded programs| # Why not
+org-mode ? Exonote supports codeblocks like in Markdown. Instead of providing
+the ability to execute codeblocks, which would lead to [literate programming]
+(https://en.wikipedia.org/wiki/Literate_programming) like in [Emacs](https://
+en.wikipedia.org/wiki/Emacs)' [org-mode](https://orgmode.org/), Exonote would
+execute a program whose source code is **properly written** elsewhere by
+calling a function with arguments. By **properly written** source code, I mean
+a regular Python [package](https://python-course.eu/python-tutorial/
+packages.php) with tree structure, modularity, Python `.py` file extension, et
+cetera. Thus, with a **minimalist** syntax, one can embed not only a program
+whose source code is written in a directory inside an exonotes dossier, but
+also a program whose distributable package is installed in the current Python
+[virtual environment](https://docs.python.org/3/library/venv.html). I thought
+it would be nice to separate prose and source code and embed a program by
+simply referencing it with a minimalist syntax the same way an image is
+embedded in Markdown. This is how an image is embedded in Exonote: ``` @[title]
+(path/to/img.png) ``` This is how a program is embedded in Exonote: ``` $
+{path.to.module:functionOrClass arg1 arg2 "foo bar"} ``` # Why use this project
+? Despite the existence of interesting note-taking solutions and the storm of
+AI-powered projects, there are compelling arguments for adopting Exonote and
+Exn. Let's explore some characteristics and concrete examples. ##
+Characteristics Here are some characteristics and their consequences:
+|Characteristic|Consequence| |---|---| |Plain old text file|Since an exonote is
+just plain text, you can always use your favorite text editor (Vim, Sublime
+Text, Visual Studio Code, et cetera) to write your notes. Exonotes are also de
+facto compatible with [VCS](https://en.wikipedia.org/wiki/Version_control).|
+|Minimalism|Exonote's minimalist markup language specification made Tkinter a
+good candidate to render it, eliminating the need for web-based technology
+(browser, html, css, et cetera). Hence, we got Exn, a lightweight, cross-
+platform app to view exonotes.| |Scripting with Python|Python is one of the
+[most popular](https://www.wired.com/story/python-language-more-popular-than-
+ever/) programming languages in the world. Since people like to tinker with
+Python, it would be fun to write scripts with this language for personal
+exonotes.| |Embed GUI programs written with Tkinter|[Tcl/Tk](https://
+www.tcl.tk/) is one of the easiest GUI toolkits to use, unsurprisingly, it's
+the default solution for GUI programming in Python via Tkinter. In the demo, a
+working calculator was built with Tkinter and embedded into an exonote.| ##
+Examples These are few concrete examples of what can be done with Exonote and
+Exn: - create interactive courses; - build programming puzzles with levels and
+backstory; - make a [proof of concept](https://www.malwarebytes.com/glossary/
+proof-of-concept); - use the `exonote.Viewer` class to make rich and/or
+interactive documentation inside another application. Exn itself uses the
+default viewer in the Exonote library. - Whistleblowing and censorship bypass:
+Due to its nature, a dossier of exonotes is very convenient for disclosing
+information that can be easily replicated and consumed by people. - Decent
+alternative to a personal website: it is as simple as creating a GitHub
+repository, upload a dossier of exonote, share the link with readers, then
+regularly update the contents with `git commit`. > **Note**: you can define a
+`blocklist` file in `$dossier/.exn` to block access to a list of exonotes
+(filenames). This mechanism with the help of custom scripts, allows the
+implementation of a system of levels where certain conditions must be met
+before opening specific exonotes. # Demo A [demo](https://github.com/pyrustic/
+exn-demo) is available that you can play with. You will need to clone the demo
+repository, install Exn with [pip](https://en.wikipedia.org/wiki/Pip_
+(package_manager)) and then run it without any arguments. By default, it
+executes the last exonote opened or runs the home page (first exonote
+referenced in the index). ```bash # 1- clone the repository $ git clone https:/
+/github.com/pyrustic/exn-demo $ cd exn-demo # 2- install exn $ pip install exn
+# 3- run exn with zero restriction $ exn ``` You can still run Exn with
+restriction: ```bash # run exn with low restriction $ exn -r # run exn with
+high restriction $ exn -R ``` # Markup language |Element|Description| |---|---
+| |ANCHOR|Create an anchor in a specific location of an exonote that can be
+accessed when its name is appended to the filename of the exonote. Syntax: ``|
+|ATTACHMENT|Insert an asset like an image. Syntax: `@[optional text](path/to/
+assets/resource.png)`| |BOLD|Make a text bold. Syntax: `*bold*`|
 |CODE|Surrounding a word or phrase with double backticks will apply a monospace
 font to it and also a colored background.| |CODEBLOCK|Same as in Markdown|
 |DINKUS|Three asterisks at the start of a blank will be centered and bolded
 like a [dinkus](https://en.wikipedia.org/wiki/Dinkus).| |GAP|Leave at least one
 blank line between a group de sentences to create paragraphs.| |HEADING|An
 exonote is made up of sections, which are made up of paragraphs. A section
 title is the Heading and it a section can have an identifier (section id,
@@ -143,30 +166,31 @@
                                                                     Back_to_top
 # Miscellaneous ## Keymap For a smooth user experience, keyboard keys are
 mapped to certain functions in Exn. For example, pressing `F` would activate
 the `Find in Page` functionality. Pressing `H` would open the home page.
 Pressing `S` would open the search interface. Pressing `T` would open the table
 of contents. Pressing `F5` would refresh the page. Et cetera. > **Note:**
 `Ctrl+Tab` will open the **switcher** to allow you to go back to the previously
-opened exonote. ## Attachments For the moments only images are supported. ##
-Path separator The separator symbol inside the path to an exonote or asset is
-the slash `/` symbol. Also, a path must not start with a separator. ##
-Filenames Exn only recognizes files with the extension `.exn`. Also, to
-reference a specific filename as a link in an exonote, you must write its path
-relative to the root of the folder. Filename and Path can be used as synonyms.
-Example: ``` dossier exonote1.exn exonote2.exn folder exonote3.exn ``` The path
-to `exonote3.exn` is `folder/exonote3.exn` ## The context object The context
-object is a namedtuple instance whose fields are: - viewer: the
-`exonote.Viewer` instance which exposes the API to manipulate the
-representation of the currently displayed exonote; - arguments: list of
-arguments passed to this function in the exonote. ## ASCII Art The ASCII Art at
-the beginning of the CLI help text is made with [patorjk's TAAG](https://
-patorjk.com/software/taag/#p=display&f=Roman&t=E%20X%20N) # Installation
-**Exn** is **cross platform** and versions under **1.0.0** will be considered
-**Beta** at best. It is built on [Ubuntu](https://ubuntu.com/download/desktop)
-with [Python 3.8](https://www.python.org/downloads/) and should work on
-**Python 3.5** or **newer**. ## For the first time ```bash $ pip install exn
-``` ## Upgrade ```bash $ pip install exn --upgrade --upgrade-strategy eager ```
-
+opened exonote. ## Quick-copy Quickly copy the contents of a codeblock or the
+address of a link with a right-click over it ! ## Attachments For the moments
+only images are supported. ## Path separator The separator symbol inside the
+path to an exonote or asset is the slash `/` symbol. Also, a path must not
+start with a separator. ## Filenames Exn only recognizes files with the
+extension `.exn`. Also, to reference a specific filename as a link in an
+exonote, you must write its path relative to the root of the folder. Filename
+and Path can be used as synonyms. Example: ``` dossier exonote1.exn
+exonote2.exn folder exonote3.exn ``` The path to `exonote3.exn` is `folder/
+exonote3.exn` ## The context object The context object is a namedtuple instance
+whose fields are: - viewer: the `exonote.Viewer` instance which exposes the API
+to manipulate the representation of the currently displayed exonote; -
+arguments: list of arguments passed to this function in the exonote. ## ASCII
+Art The ASCII Art at the beginning of the CLI help text is made with [patorjk's
+TAAG](https://patorjk.com/software/taag/#p=display&f=Roman&t=E%20X%20N) #
+Installation **Exn** is **cross platform** and versions under **1.0.0** will be
+considered **Beta** at best. It is built on [Ubuntu](https://ubuntu.com/
+download/desktop) with [Python 3.8](https://www.python.org/downloads/) and
+should work on **Python 3.5** or **newer**. ## For the first time ```bash $ pip
+install exn ``` ## Upgrade ```bash $ pip install exn --upgrade --upgrade-
+strategy eager ```
 
 
 [Back to top](#readme)
```

### Comparing `exn-0.0.6/exn/__main__.py` & `exn-0.0.7/exn/__main__.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/dao/__init__.py` & `exn-0.0.7/exn/dao/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,23 +58,23 @@
         self._bookmarks_filename = os.path.join(self._dossier, ".exn", "bookmarks")
         self._blocklist_filename = os.path.join(self._dossier, ".exn", "blocklist")
         self._load_data()
         atexit.register(self._on_exit)
 
     def _load_data(self):
         if os.path.exists(self._history_filename):
-            cache = jesth.read(self._history_filename, compact=True)
+            cache = jesth.read(self._history_filename, compact_mode=True)
             if cache:
                 self._history_cache = cache.get("", list())
         if os.path.exists(self._bookmarks_filename):
-            cache = jesth.read(self._bookmarks_filename, compact=True)
+            cache = jesth.read(self._bookmarks_filename, compact_mode=True)
             if cache:
                 self._bookmarks_cache = cache.get("", list())
         if os.path.exists(self._blocklist_filename):
-            cache = jesth.read(self._blocklist_filename, compact=True)
+            cache = jesth.read(self._blocklist_filename, compact_mode=True)
             if cache:
                 self._blocklist = cache.get("", list())
 
     def _save_state(self):
         self._create_dotexn_folder()
         items = [(self._history_filename, self.get_history),
                  (self._bookmarks_filename, self.get_bookmarks)]
```

### Comparing `exn-0.0.6/exn/manager/__init__.py` & `exn-0.0.7/exn/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/theme/__init__.py` & `exn-0.0.7/exn/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/utils/__init__.py` & `exn-0.0.7/exn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/about.py` & `exn-0.0.7/exn/view/about.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/board.py` & `exn-0.0.7/exn/view/board.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/footer.py` & `exn-0.0.7/exn/view/footer.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/front.py` & `exn-0.0.7/exn/view/front.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/goto.py` & `exn-0.0.7/exn/view/goto.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/info.py` & `exn-0.0.7/exn/view/info.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/past.py` & `exn-0.0.7/exn/view/past.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/roll.py` & `exn-0.0.7/exn/view/roll.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/search.py` & `exn-0.0.7/exn/view/search.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/switcher.py` & `exn-0.0.7/exn/view/switcher.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/toc.py` & `exn-0.0.7/exn/view/toc.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/top.py` & `exn-0.0.7/exn/view/top.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn/view/util.py` & `exn-0.0.7/exn/view/util.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/exn.egg-info/PKG-INFO` & `exn-0.0.7/exn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exn
-Version: 0.0.6
+Version: 0.0.7
 Summary: Browse a dossier of exonotes
 Home-page: https://github.com/pyrustic/exn
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
@@ -15,81 +15,95 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- Cover -->
 <div align="center">
-    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/cover.png" alt="Demo" width="683">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/cover.png" alt="Demo" width="500">
     <p align="center">
-    Exn <a href="https://github.com/pyrustic/exn-demo">demo</a>
+    <a href="https://github.com/pyrustic/exn-demo/blob/master/home.exn">Home.exn</a> from the <a href="https://github.com/pyrustic/exn-demo">demo</a> dossier
     </p>
 </div>
 
-> **Note to HN user**: I plan to make a Show HN soon ! ;)
-
 
 <!-- Intro Text -->
 # Exonote / Exn
 <b> Write and render rich, scriptable, and interactive notes </b>
     
 This project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
 > [Installation](#installation) &nbsp; &nbsp; [Demo](#demo) &nbsp; &nbsp; [Latest](https://github.com/pyrustic/exn/tags) &nbsp; &nbsp; [Modules](https://github.com/pyrustic/exn/tree/master/docs/modules#readme)
 
 
 ## Table of contents
 
-
-[Overview](#overview)
-    
-[Why use this project ?](#why-use-this-project-)
-
-[Demo](#demo)
-
-[Markup language](#markup-language)
-
-[Command line interface](#command-line-interface)
-
-[Scripting with Python](#scripting-with-Python)
-
-[Viewer API](#viewer-api)
-
-[Embedding GUI programs](#embedding-gui-programs)
-
-[Key bindings](#key-bindings)
-
-[Miscellaneous](#miscellaneous)
-
-[Installation](#installation)
+- [Overview](#overview)
+- [Why not org-mode ?](#why-not-org-mode-)
+- [Why use this project ?](#why-use-this-project-)
+- [Demo](#demo)
+- [Markup language](#markup-language)
+- [Command line interface](#command-line-interface)
+- [Scripting with Python](#scripting-with-Python)
+- [Viewer API](#viewer-api)
+- [Embedding GUI programs](#embedding-gui-programs)
+- [Miscellaneous](#miscellaneous)
+- [Installation](#installation)
 
 
 # Overview
-Exn is a lightweight Python application for browsing a dossier of exonotes. An exonote is **plain text** written with an [eponymous](https://github.com/pyrustic/exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://www.python.org/downloads/)).
+**Exn** is a lightweight Python application for browsing a dossier of exonotes. An **exonote** is **plain text** written with an [eponymous](https://github.com/pyrustic/exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://www.python.org/downloads/)).
 
 **Interactivity** can be added to an exonote by **embedding GUI programs** written in Python with Tkinter. Additionally, all or part of an exonote can be arbitrarily generated using **custom Python scripts**.
 
-This application is built with the Gaspium framework and uses [Shared](https://github.com/pyrustic/shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to manipulate data.
+This application is built with the [Gaspium](https://github.com/pyrustic/gaspium) framework and uses [Shared](https://github.com/pyrustic/shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to manipulate data.
+
+This project is built on top of [Exonote](https://github.com/pyrustic/exonote). Solving issues in **Exonote** means improving **Exn**. Check the [issues](https://github.com/pyrustic/exonote/issues) !
 
 ## Dossier of exonotes
-A dossier is a directory containing exonotes and resources such as attachments and Python source code. At the root of a dossier should be an index file containing an ordered list of exonotes filenames, titles, and their associated tags. The index file is generated automatically by the `--build` command in the command line (the order is based on the creation timestamp of the exonotes).
+A **dossier** is a directory containing exonotes and resources such as attachments and Python source code. At the root of a dossier should be an index file containing an ordered list of exonotes filenames, titles, and their associated tags. The index file is generated automatically by the `--build` command in the command line (the order is based on the creation timestamp of the exonotes).
 
 Exn treats each exonote with the `.exn` extension as the page of a virtual book, so the graphical user interface of Exn is a metaphor for a book with controls to move from one page to the next or to the previous one.
 
 ## The Search feature
 Exn has a search interface that allows the user to search for exonotes in the dossier by specifying tags, words or a phrase. The search mechanism has an optional [regular expression](https://en.wikipedia.org/wiki/Regular_expression) mode.
 
+<div align="center">
+    <img src="https://raw.githubusercontent.com/pyrustic/misc/master/assets/exn/search.png" alt="Search" width="300">
+    <p align="center">
+    <b>Search</b> interface
+    </p>
+</div>
+
 ## On security: run untrusted exonotes
 The command line interface exposes two options for running exonotes:
 
 |Option|Description|
 |---|---|
 |`-r`, `--restrict [<filename>]`| Open a note with low restriction, i.e., block the execution of embedded programs|
 |`-R`, `--Restrict [<filename>]`| Open a note with high restriction, i.e., block executable links and also the execution of embedded programs|
 
 
+# Why not org-mode ?
+Exonote supports codeblocks like in Markdown. Instead of providing the ability to execute codeblocks, which would lead to [literate programming](https://en.wikipedia.org/wiki/Literate_programming) like in [Emacs](https://en.wikipedia.org/wiki/Emacs)' [org-mode](https://orgmode.org/), Exonote would execute a program whose source code is **properly written** elsewhere by calling a function with arguments.
+
+By **properly written** source code, I mean a regular Python [package](https://python-course.eu/python-tutorial/packages.php) with tree structure, modularity, Python `.py` file extension, et cetera. Thus, with a **minimalist** syntax, one can embed not only a program whose source code is written in a directory inside an exonotes dossier, but also a program whose distributable package is installed in the current Python [virtual environment](https://docs.python.org/3/library/venv.html). 
+
+I thought it would be nice to separate prose and source code and embed a program by simply referencing it with a minimalist syntax the same way an image is embedded in Markdown.
+
+This is how an image is embedded in Exonote:
+
+```
+@[title](path/to/img.png)
+```
+
+This is how a program is embedded in Exonote:
+```
+${path.to.module:functionOrClass arg1 arg2 "foo bar"}
+```
+
 # Why use this project ?
 Despite the existence of interesting note-taking solutions and the storm of AI-powered projects, there are compelling arguments for adopting Exonote and Exn. Let's explore some characteristics and concrete examples.
 
 ## Characteristics
 Here are some characteristics and their consequences:
 
 |Characteristic|Consequence|
@@ -102,15 +116,15 @@
 ## Examples
 These are few concrete examples of what can be done with Exonote and Exn:
 
 - create interactive courses;
 - build programming puzzles with levels and backstory;
 - make a [proof of concept](https://www.malwarebytes.com/glossary/proof-of-concept);
 - use the `exonote.Viewer` class to make rich and/or interactive documentation inside another application. Exn itself uses the default viewer in the Exonote library.
-- Whistleblowing and and censorship bypass: Due to its nature, a dossier of exonotes is very convenient for disclosing information that can be easily replicated and consumed by people.
+- Whistleblowing and censorship bypass: Due to its nature, a dossier of exonotes is very convenient for disclosing information that can be easily replicated and consumed by people.
 - Decent alternative to a personal website: it is as simple as creating a GitHub repository, upload a dossier of exonote, share the link with readers, then regularly update the contents with `git commit`.
 
 > **Note**: you can define a `blocklist` file in `$dossier/.exn` to block access to a list of exonotes (filenames). This mechanism with the help of custom scripts, allows the implementation of a system of levels where certain conditions must be met before opening specific exonotes.
 
 # Demo
 A [demo](https://github.com/pyrustic/exn-demo) is available that you can play with. You will need to clone the demo repository, install Exn with [pip](https://en.wikipedia.org/wiki/Pip_(package_manager)) and then run it without any arguments. By default, it executes the last exonote opened or runs the home page (first exonote referenced in the index).
 
@@ -251,14 +265,17 @@
 # Miscellaneous
 
 ## Keymap
 For a smooth user experience, keyboard keys are mapped to certain functions in Exn. For example, pressing `F` would activate the `Find in Page` functionality. Pressing `H` would open the home page. Pressing `S` would open the search interface. Pressing `T` would open the table of contents. Pressing `F5` would refresh the page. Et cetera.
 
 > **Note:** `Ctrl+Tab` will open the **switcher** to allow you to go back to the previously opened exonote.
 
+## Quick-copy
+Quickly copy the contents of a codeblock or the address of a link with a right-click over it !
+
 ## Attachments
 For the moments only images are supported.
 
 ## Path separator
 The separator symbol inside the path to an exonote or asset is the slash `/` symbol. Also, a path must not start with a separator.
 
 ## Filenames
```

#### html2text {}

```diff
@@ -1,101 +1,124 @@
-Metadata-Version: 2.1 Name: exn Version: 0.0.6 Summary: Browse a dossier of
+Metadata-Version: 2.1 Name: exn Version: 0.0.7 Summary: Browse a dossier of
 exonotes Home-page: https://github.com/pyrustic/exn Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com Maintainer: Pyrustic Evangelist Maintainer-
 email: rusticalex@yahoo.com License: MIT Keywords: application,pyrustic
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.5 Description-Content-Type: text/markdown
 License-File: LICENSE
                                     [Demo]
-                                   Exn demo
-> **Note to HN user**: I plan to make a Show HN soon ! ;)  # Exonote / Exn
-Write and render rich, scriptable, and interactive notes This project is part
-of the [Pyrustic Open Ecosystem](https://pyrustic.github.io). > [Installation]
-(#installation)     [Demo](#demo)     [Latest](https://github.com/pyrustic/exn/
-tags)     [Modules](https://github.com/pyrustic/exn/tree/master/docs/
-modules#readme) ## Table of contents [Overview](#overview) [Why use this
-project ?](#why-use-this-project-) [Demo](#demo) [Markup language](#markup-
-language) [Command line interface](#command-line-interface) [Scripting with
-Python](#scripting-with-Python) [Viewer API](#viewer-api) [Embedding GUI
-programs](#embedding-gui-programs) [Key bindings](#key-bindings)
-[Miscellaneous](#miscellaneous) [Installation](#installation) # Overview Exn is
-a lightweight Python application for browsing a dossier of exonotes. An exonote
-is **plain text** written with an [eponymous](https://github.com/pyrustic/
-exonote) markup language inspired by [Markdown](https://en.wikipedia.org/wiki/
-Markdown) and rendered with [Tkinter](https://en.wikipedia.org/wiki/Tkinter)
-(the default GUI library for [Python](https://www.python.org/downloads/)).
-**Interactivity** can be added to an exonote by **embedding GUI programs**
-written in Python with Tkinter. Additionally, all or part of an exonote can be
-arbitrarily generated using **custom Python scripts**. This application is
-built with the Gaspium framework and uses [Shared](https://github.com/pyrustic/
+                        Home.exn from the demo dossier
+ # Exonote / Exn Write and render rich, scriptable, and interactive notes This
+project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io). >
+[Installation](#installation)     [Demo](#demo)     [Latest](https://
+github.com/pyrustic/exn/tags)     [Modules](https://github.com/pyrustic/exn/
+tree/master/docs/modules#readme) ## Table of contents - [Overview](#overview) -
+[Why not org-mode ?](#why-not-org-mode-) - [Why use this project ?](#why-use-
+this-project-) - [Demo](#demo) - [Markup language](#markup-language) - [Command
+line interface](#command-line-interface) - [Scripting with Python](#scripting-
+with-Python) - [Viewer API](#viewer-api) - [Embedding GUI programs](#embedding-
+gui-programs) - [Miscellaneous](#miscellaneous) - [Installation](#installation)
+# Overview **Exn** is a lightweight Python application for browsing a dossier
+of exonotes. An **exonote** is **plain text** written with an [eponymous]
+(https://github.com/pyrustic/exonote) markup language inspired by [Markdown]
+(https://en.wikipedia.org/wiki/Markdown) and rendered with [Tkinter](https://
+en.wikipedia.org/wiki/Tkinter) (the default GUI library for [Python](https://
+www.python.org/downloads/)). **Interactivity** can be added to an exonote by
+**embedding GUI programs** written in Python with Tkinter. Additionally, all or
+part of an exonote can be arbitrarily generated using **custom Python
+scripts**. This application is built with the [Gaspium](https://github.com/
+pyrustic/gaspium) framework and uses [Shared](https://github.com/pyrustic/
 shared) and [Jesth](https://github.com/pyrustic/jesth) extensively to
-manipulate data. ## Dossier of exonotes A dossier is a directory containing
-exonotes and resources such as attachments and Python source code. At the root
-of a dossier should be an index file containing an ordered list of exonotes
-filenames, titles, and their associated tags. The index file is generated
-automatically by the `--build` command in the command line (the order is based
-on the creation timestamp of the exonotes). Exn treats each exonote with the
-`.exn` extension as the page of a virtual book, so the graphical user interface
-of Exn is a metaphor for a book with controls to move from one page to the next
-or to the previous one. ## The Search feature Exn has a search interface that
-allows the user to search for exonotes in the dossier by specifying tags, words
-or a phrase. The search mechanism has an optional [regular expression](https://
-en.wikipedia.org/wiki/Regular_expression) mode. ## On security: run untrusted
-exonotes The command line interface exposes two options for running exonotes:
-|Option|Description| |---|---| |`-r`, `--restrict []`| Open a note with low
-restriction, i.e., block the execution of embedded programs| |`-R`, `--Restrict
-[]`| Open a note with high restriction, i.e., block executable links and also
-the execution of embedded programs| # Why use this project ? Despite the
-existence of interesting note-taking solutions and the storm of AI-powered
-projects, there are compelling arguments for adopting Exonote and Exn. Let's
-explore some characteristics and concrete examples. ## Characteristics Here are
-some characteristics and their consequences: |Characteristic|Consequence| |---
-|---| |Plain old text file|Since an exonote is just plain text, you can always
-use your favorite text editor (Vim, Sublime Text, Visual Studio Code, et
-cetera) to write your notes. Exonotes are also de facto compatible with [VCS]
-(https://en.wikipedia.org/wiki/Version_control).| |Minimalism|Exonote's
-minimalist markup language specification made Tkinter a good candidate to
-render it, eliminating the need for web-based technology (browser, html, css,
-et cetera). Hence, we got Exn, a lightweight, cross-platform app to view
-exonotes.| |Scripting with Python|Python is one of the [most popular](https://
-www.wired.com/story/python-language-more-popular-than-ever/) programming
-languages in the world. Since people like to tinker with Python, it would be
-fun to write scripts with this language for personal exonotes.| |Embed GUI
-programs written with Tkinter|[Tcl/Tk](https://www.tcl.tk/) is one of the
-easiest GUI toolkits to use, unsurprisingly, it's the default solution for GUI
-programming in Python via Tkinter. In the demo, a working calculator was built
-with Tkinter and embedded into an exonote.| ## Examples These are few concrete
-examples of what can be done with Exonote and Exn: - create interactive
-courses; - build programming puzzles with levels and backstory; - make a [proof
-of concept](https://www.malwarebytes.com/glossary/proof-of-concept); - use the
-`exonote.Viewer` class to make rich and/or interactive documentation inside
-another application. Exn itself uses the default viewer in the Exonote library.
-- Whistleblowing and and censorship bypass: Due to its nature, a dossier of
-exonotes is very convenient for disclosing information that can be easily
-replicated and consumed by people. - Decent alternative to a personal website:
-it is as simple as creating a GitHub repository, upload a dossier of exonote,
-share the link with readers, then regularly update the contents with `git
-commit`. > **Note**: you can define a `blocklist` file in `$dossier/.exn` to
-block access to a list of exonotes (filenames). This mechanism with the help of
-custom scripts, allows the implementation of a system of levels where certain
-conditions must be met before opening specific exonotes. # Demo A [demo](https:
-//github.com/pyrustic/exn-demo) is available that you can play with. You will
-need to clone the demo repository, install Exn with [pip](https://
-en.wikipedia.org/wiki/Pip_(package_manager)) and then run it without any
-arguments. By default, it executes the last exonote opened or runs the home
-page (first exonote referenced in the index). ```bash # 1- clone the repository
-$ git clone https://github.com/pyrustic/exn-demo $ cd exn-demo # 2- install exn
-$ pip install exn # 3- run exn with zero restriction $ exn ``` You can still
-run Exn with restriction: ```bash # run exn with low restriction $ exn -r # run
-exn with high restriction $ exn -R ``` # Markup language |Element|Description|
-|---|---| |ANCHOR|Create an anchor in a specific location of an exonote that
-can be accessed when its name is appended to the filename of the exonote.
-Syntax: ``| |ATTACHMENT|Insert an asset like an image. Syntax: `@[optional
-text](path/to/assets/resource.png)`| |BOLD|Make a text bold. Syntax: `*bold*`|
+manipulate data. This project is built on top of [Exonote](https://github.com/
+pyrustic/exonote). Solving issues in **Exonote** means improving **Exn**. Check
+the [issues](https://github.com/pyrustic/exonote/issues) ! ## Dossier of
+exonotes A **dossier** is a directory containing exonotes and resources such as
+attachments and Python source code. At the root of a dossier should be an index
+file containing an ordered list of exonotes filenames, titles, and their
+associated tags. The index file is generated automatically by the `--build`
+command in the command line (the order is based on the creation timestamp of
+the exonotes). Exn treats each exonote with the `.exn` extension as the page of
+a virtual book, so the graphical user interface of Exn is a metaphor for a book
+with controls to move from one page to the next or to the previous one. ## The
+Search feature Exn has a search interface that allows the user to search for
+exonotes in the dossier by specifying tags, words or a phrase. The search
+mechanism has an optional [regular expression](https://en.wikipedia.org/wiki/
+Regular_expression) mode.
+                                   [Search]
+                               Search interface
+## On security: run untrusted exonotes The command line interface exposes two
+options for running exonotes: |Option|Description| |---|---| |`-r`, `--restrict
+[]`| Open a note with low restriction, i.e., block the execution of embedded
+programs| |`-R`, `--Restrict []`| Open a note with high restriction, i.e.,
+block executable links and also the execution of embedded programs| # Why not
+org-mode ? Exonote supports codeblocks like in Markdown. Instead of providing
+the ability to execute codeblocks, which would lead to [literate programming]
+(https://en.wikipedia.org/wiki/Literate_programming) like in [Emacs](https://
+en.wikipedia.org/wiki/Emacs)' [org-mode](https://orgmode.org/), Exonote would
+execute a program whose source code is **properly written** elsewhere by
+calling a function with arguments. By **properly written** source code, I mean
+a regular Python [package](https://python-course.eu/python-tutorial/
+packages.php) with tree structure, modularity, Python `.py` file extension, et
+cetera. Thus, with a **minimalist** syntax, one can embed not only a program
+whose source code is written in a directory inside an exonotes dossier, but
+also a program whose distributable package is installed in the current Python
+[virtual environment](https://docs.python.org/3/library/venv.html). I thought
+it would be nice to separate prose and source code and embed a program by
+simply referencing it with a minimalist syntax the same way an image is
+embedded in Markdown. This is how an image is embedded in Exonote: ``` @[title]
+(path/to/img.png) ``` This is how a program is embedded in Exonote: ``` $
+{path.to.module:functionOrClass arg1 arg2 "foo bar"} ``` # Why use this project
+? Despite the existence of interesting note-taking solutions and the storm of
+AI-powered projects, there are compelling arguments for adopting Exonote and
+Exn. Let's explore some characteristics and concrete examples. ##
+Characteristics Here are some characteristics and their consequences:
+|Characteristic|Consequence| |---|---| |Plain old text file|Since an exonote is
+just plain text, you can always use your favorite text editor (Vim, Sublime
+Text, Visual Studio Code, et cetera) to write your notes. Exonotes are also de
+facto compatible with [VCS](https://en.wikipedia.org/wiki/Version_control).|
+|Minimalism|Exonote's minimalist markup language specification made Tkinter a
+good candidate to render it, eliminating the need for web-based technology
+(browser, html, css, et cetera). Hence, we got Exn, a lightweight, cross-
+platform app to view exonotes.| |Scripting with Python|Python is one of the
+[most popular](https://www.wired.com/story/python-language-more-popular-than-
+ever/) programming languages in the world. Since people like to tinker with
+Python, it would be fun to write scripts with this language for personal
+exonotes.| |Embed GUI programs written with Tkinter|[Tcl/Tk](https://
+www.tcl.tk/) is one of the easiest GUI toolkits to use, unsurprisingly, it's
+the default solution for GUI programming in Python via Tkinter. In the demo, a
+working calculator was built with Tkinter and embedded into an exonote.| ##
+Examples These are few concrete examples of what can be done with Exonote and
+Exn: - create interactive courses; - build programming puzzles with levels and
+backstory; - make a [proof of concept](https://www.malwarebytes.com/glossary/
+proof-of-concept); - use the `exonote.Viewer` class to make rich and/or
+interactive documentation inside another application. Exn itself uses the
+default viewer in the Exonote library. - Whistleblowing and censorship bypass:
+Due to its nature, a dossier of exonotes is very convenient for disclosing
+information that can be easily replicated and consumed by people. - Decent
+alternative to a personal website: it is as simple as creating a GitHub
+repository, upload a dossier of exonote, share the link with readers, then
+regularly update the contents with `git commit`. > **Note**: you can define a
+`blocklist` file in `$dossier/.exn` to block access to a list of exonotes
+(filenames). This mechanism with the help of custom scripts, allows the
+implementation of a system of levels where certain conditions must be met
+before opening specific exonotes. # Demo A [demo](https://github.com/pyrustic/
+exn-demo) is available that you can play with. You will need to clone the demo
+repository, install Exn with [pip](https://en.wikipedia.org/wiki/Pip_
+(package_manager)) and then run it without any arguments. By default, it
+executes the last exonote opened or runs the home page (first exonote
+referenced in the index). ```bash # 1- clone the repository $ git clone https:/
+/github.com/pyrustic/exn-demo $ cd exn-demo # 2- install exn $ pip install exn
+# 3- run exn with zero restriction $ exn ``` You can still run Exn with
+restriction: ```bash # run exn with low restriction $ exn -r # run exn with
+high restriction $ exn -R ``` # Markup language |Element|Description| |---|---
+| |ANCHOR|Create an anchor in a specific location of an exonote that can be
+accessed when its name is appended to the filename of the exonote. Syntax: ``|
+|ATTACHMENT|Insert an asset like an image. Syntax: `@[optional text](path/to/
+assets/resource.png)`| |BOLD|Make a text bold. Syntax: `*bold*`|
 |CODE|Surrounding a word or phrase with double backticks will apply a monospace
 font to it and also a colored background.| |CODEBLOCK|Same as in Markdown|
 |DINKUS|Three asterisks at the start of a blank will be centered and bolded
 like a [dinkus](https://en.wikipedia.org/wiki/Dinkus).| |GAP|Leave at least one
 blank line between a group de sentences to create paragraphs.| |HEADING|An
 exonote is made up of sections, which are made up of paragraphs. A section
 title is the Heading and it a section can have an identifier (section id,
@@ -151,30 +174,31 @@
                                                                     Back_to_top
 # Miscellaneous ## Keymap For a smooth user experience, keyboard keys are
 mapped to certain functions in Exn. For example, pressing `F` would activate
 the `Find in Page` functionality. Pressing `H` would open the home page.
 Pressing `S` would open the search interface. Pressing `T` would open the table
 of contents. Pressing `F5` would refresh the page. Et cetera. > **Note:**
 `Ctrl+Tab` will open the **switcher** to allow you to go back to the previously
-opened exonote. ## Attachments For the moments only images are supported. ##
-Path separator The separator symbol inside the path to an exonote or asset is
-the slash `/` symbol. Also, a path must not start with a separator. ##
-Filenames Exn only recognizes files with the extension `.exn`. Also, to
-reference a specific filename as a link in an exonote, you must write its path
-relative to the root of the folder. Filename and Path can be used as synonyms.
-Example: ``` dossier exonote1.exn exonote2.exn folder exonote3.exn ``` The path
-to `exonote3.exn` is `folder/exonote3.exn` ## The context object The context
-object is a namedtuple instance whose fields are: - viewer: the
-`exonote.Viewer` instance which exposes the API to manipulate the
-representation of the currently displayed exonote; - arguments: list of
-arguments passed to this function in the exonote. ## ASCII Art The ASCII Art at
-the beginning of the CLI help text is made with [patorjk's TAAG](https://
-patorjk.com/software/taag/#p=display&f=Roman&t=E%20X%20N) # Installation
-**Exn** is **cross platform** and versions under **1.0.0** will be considered
-**Beta** at best. It is built on [Ubuntu](https://ubuntu.com/download/desktop)
-with [Python 3.8](https://www.python.org/downloads/) and should work on
-**Python 3.5** or **newer**. ## For the first time ```bash $ pip install exn
-``` ## Upgrade ```bash $ pip install exn --upgrade --upgrade-strategy eager ```
-
+opened exonote. ## Quick-copy Quickly copy the contents of a codeblock or the
+address of a link with a right-click over it ! ## Attachments For the moments
+only images are supported. ## Path separator The separator symbol inside the
+path to an exonote or asset is the slash `/` symbol. Also, a path must not
+start with a separator. ## Filenames Exn only recognizes files with the
+extension `.exn`. Also, to reference a specific filename as a link in an
+exonote, you must write its path relative to the root of the folder. Filename
+and Path can be used as synonyms. Example: ``` dossier exonote1.exn
+exonote2.exn folder exonote3.exn ``` The path to `exonote3.exn` is `folder/
+exonote3.exn` ## The context object The context object is a namedtuple instance
+whose fields are: - viewer: the `exonote.Viewer` instance which exposes the API
+to manipulate the representation of the currently displayed exonote; -
+arguments: list of arguments passed to this function in the exonote. ## ASCII
+Art The ASCII Art at the beginning of the CLI help text is made with [patorjk's
+TAAG](https://patorjk.com/software/taag/#p=display&f=Roman&t=E%20X%20N) #
+Installation **Exn** is **cross platform** and versions under **1.0.0** will be
+considered **Beta** at best. It is built on [Ubuntu](https://ubuntu.com/
+download/desktop) with [Python 3.8](https://www.python.org/downloads/) and
+should work on **Python 3.5** or **newer**. ## For the first time ```bash $ pip
+install exn ``` ## Upgrade ```bash $ pip install exn --upgrade --upgrade-
+strategy eager ```
 
 
 [Back to top](#readme)
```

### Comparing `exn-0.0.6/exn.egg-info/SOURCES.txt` & `exn-0.0.7/exn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exn-0.0.6/setup.cfg` & `exn-0.0.7/setup.cfg`

 * *Files identical despite different names*

