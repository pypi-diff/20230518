# Comparing `tmp/Phasor Noise-1.0.1.dev48.tar.gz` & `tmp/Phasor Noise-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Phasor Noise-1.0.1.dev48.tar", last modified: Wed May 17 21:01:55 2023, max compression
+gzip compressed data, was "Phasor Noise-1.3.0.tar", last modified: Thu May 18 19:41:37 2023, max compression
```

## Comparing `Phasor Noise-1.0.1.dev48.tar` & `Phasor Noise-1.3.0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.246921 Phasor Noise-1.0.1.dev48/
--rw-rw-rw-   0        0        0      284 2023-05-17 21:01:54.000000 Phasor Noise-1.0.1.dev48/AUTHORS
--rw-rw-rw-   0        0        0    35869 2023-05-16 20:15:41.000000 Phasor Noise-1.0.1.dev48/LICENSE
--rw-rw-rw-   0        0        0      156 2023-05-17 20:37:44.000000 Phasor Noise-1.0.1.dev48/Makefile
--rw-rw-rw-   0        0        0     1026 2023-05-17 21:01:55.246921 Phasor Noise-1.0.1.dev48/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-05-17 19:58:29.000000 Phasor Noise-1.0.1.dev48/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.215664 Phasor Noise-1.0.1.dev48/docs/
--rw-rw-rw-   0        0        0      603 2023-05-17 18:17:17.000000 Phasor Noise-1.0.1.dev48/docs/Makefile
--rw-rw-rw-   0        0        0        0 2023-05-17 13:34:47.000000 Phasor Noise-1.0.1.dev48/docs/README.rst
--rwxrwxrwx   0        0        0      827 2023-05-17 18:16:47.000000 Phasor Noise-1.0.1.dev48/docs/make.bat
--rw-rw-rw-   0        0        0       24 2023-05-17 18:51:28.000000 Phasor Noise-1.0.1.dev48/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.215664 Phasor Noise-1.0.1.dev48/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.215664 Phasor Noise-1.0.1.dev48/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.215664 Phasor Noise-1.0.1.dev48/docs/source/api/GUI/
--rw-rw-rw-   0        0        0      131 2023-05-17 20:04:06.000000 Phasor Noise-1.0.1.dev48/docs/source/api/GUI/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.215664 Phasor Noise-1.0.1.dev48/docs/source/api/analysis/
--rw-rw-rw-   0        0        0      175 2023-05-17 20:03:35.000000 Phasor Noise-1.0.1.dev48/docs/source/api/analysis/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.231296 Phasor Noise-1.0.1.dev48/docs/source/api/generator/
--rw-rw-rw-   0        0        0      203 2023-05-17 20:03:35.000000 Phasor Noise-1.0.1.dev48/docs/source/api/generator/index.rst
--rw-rw-rw-   0        0        0      248 2023-05-17 20:58:47.000000 Phasor Noise-1.0.1.dev48/docs/source/api/index.rst
--rw-rw-rw-   0        0        0     9197 2023-05-17 20:21:39.000000 Phasor Noise-1.0.1.dev48/docs/source/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.231296 Phasor Noise-1.0.1.dev48/docs/source/getting_started/
--rw-rw-rw-   0        0        0      196 2023-05-17 18:55:41.000000 Phasor Noise-1.0.1.dev48/docs/source/getting_started/index.rst
--rw-rw-rw-   0        0        0      193 2023-05-17 20:58:03.000000 Phasor Noise-1.0.1.dev48/docs/source/getting_started/installation.rst
--rw-rw-rw-   0        0        0      701 2023-05-17 19:12:49.000000 Phasor Noise-1.0.1.dev48/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.231296 Phasor Noise-1.0.1.dev48/docs/source/user_guide/
--rw-rw-rw-   0        0        0       99 2023-05-17 14:58:13.000000 Phasor Noise-1.0.1.dev48/docs/source/user_guide/index.rst
--rw-rw-rw-   0        0        0       89 2023-05-17 19:39:21.000000 Phasor Noise-1.0.1.dev48/requirements.txt
--rw-rw-rw-   0        0        0      637 2023-05-17 21:01:55.262546 Phasor Noise-1.0.1.dev48/setup.cfg
--rw-rw-rw-   0        0        0      181 2023-05-17 18:14:41.000000 Phasor Noise-1.0.1.dev48/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.231296 Phasor Noise-1.0.1.dev48/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.246921 Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/
--rw-rw-rw-   0        0        0     1026 2023-05-17 21:01:55.000000 Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-05-17 21:01:55.000000 Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 21:01:55.000000 Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 21:01:55.000000 Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-05-17 21:01:55.000000 Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/pbr.json
--rw-rw-rw-   0        0        0       86 2023-05-17 21:01:55.000000 Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 21:01:55.000000 Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      165 2023-05-16 20:15:41.000000 Phasor Noise-1.0.1.dev48/src/config.json
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.231296 Phasor Noise-1.0.1.dev48/src/phasor_noise/
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.231296 Phasor Noise-1.0.1.dev48/src/phasor_noise/GUI/
--rw-rw-rw-   0        0        0    21251 2023-05-17 20:36:54.000000 Phasor Noise-1.0.1.dev48/src/phasor_noise/GUI/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-05-16 20:15:41.000000 Phasor Noise-1.0.1.dev48/src/phasor_noise/GUI/menu.py
--rw-rw-rw-   0        0        0      380 2023-05-17 20:33:11.000000 Phasor Noise-1.0.1.dev48/src/phasor_noise/GUI/platform_specific.py
--rw-rw-rw-   0        0        0      464 2023-05-17 19:00:05.000000 Phasor Noise-1.0.1.dev48/src/phasor_noise/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.231296 Phasor Noise-1.0.1.dev48/src/phasor_noise/analysis/
--rw-rw-rw-   0        0        0      797 2023-05-17 20:05:56.000000 Phasor Noise-1.0.1.dev48/src/phasor_noise/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:55.246921 Phasor Noise-1.0.1.dev48/src/phasor_noise/phasor_noise_generator/
--rw-rw-rw-   0        0        0     5509 2023-05-16 20:24:18.000000 Phasor Noise-1.0.1.dev48/src/phasor_noise/phasor_noise_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.659980 Phasor Noise-1.3.0/
+-rw-rw-rw-   0        0        0      284 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/AUTHORS
+-rw-rw-rw-   0        0        0    35869 2023-05-16 20:15:41.000000 Phasor Noise-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      157 2023-05-18 19:39:39.000000 Phasor Noise-1.3.0/Makefile
+-rw-rw-rw-   0        0        0     1119 2023-05-18 19:41:37.659980 Phasor Noise-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-05-18 19:41:02.000000 Phasor Noise-1.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.611051 Phasor Noise-1.3.0/docs/
+-rw-rw-rw-   0        0        0      603 2023-05-17 18:17:17.000000 Phasor Noise-1.3.0/docs/Makefile
+-rw-rw-rw-   0        0        0        0 2023-05-17 13:34:47.000000 Phasor Noise-1.3.0/docs/README.rst
+-rwxrwxrwx   0        0        0      827 2023-05-17 18:16:47.000000 Phasor Noise-1.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0       24 2023-05-17 18:51:28.000000 Phasor Noise-1.3.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/api/GUI/
+-rw-rw-rw-   0        0        0      131 2023-05-17 20:04:06.000000 Phasor Noise-1.3.0/docs/source/api/GUI/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/api/analysis/
+-rw-rw-rw-   0        0        0      175 2023-05-17 20:03:35.000000 Phasor Noise-1.3.0/docs/source/api/analysis/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/api/generator/
+-rw-rw-rw-   0        0        0      203 2023-05-17 20:03:35.000000 Phasor Noise-1.3.0/docs/source/api/generator/index.rst
+-rw-rw-rw-   0        0        0      248 2023-05-17 20:58:47.000000 Phasor Noise-1.3.0/docs/source/api/index.rst
+-rw-rw-rw-   0        0        0     9189 2023-05-18 16:10:27.000000 Phasor Noise-1.3.0/docs/source/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/getting_started/
+-rw-rw-rw-   0        0        0      196 2023-05-17 18:55:41.000000 Phasor Noise-1.3.0/docs/source/getting_started/index.rst
+-rw-rw-rw-   0        0        0      193 2023-05-17 20:58:03.000000 Phasor Noise-1.3.0/docs/source/getting_started/installation.rst
+-rw-rw-rw-   0        0        0      668 2023-05-18 15:29:52.000000 Phasor Noise-1.3.0/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.626747 Phasor Noise-1.3.0/docs/source/user_guide/
+-rw-rw-rw-   0        0        0       99 2023-05-17 14:58:13.000000 Phasor Noise-1.3.0/docs/source/user_guide/index.rst
+-rw-rw-rw-   0        0        0       89 2023-05-17 19:39:21.000000 Phasor Noise-1.3.0/requirements.txt
+-rw-rw-rw-   0        0        0      652 2023-05-18 19:41:37.659980 Phasor Noise-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      181 2023-05-17 18:14:41.000000 Phasor Noise-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.595433 Phasor Noise-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.659980 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/
+-rw-rw-rw-   0        0        0     1119 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 21:01:55.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/pbr.json
+-rw-rw-rw-   0        0        0       86 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-18 19:41:37.000000 Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.642369 Phasor Noise-1.3.0/src/phasor_noise/
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.642369 Phasor Noise-1.3.0/src/phasor_noise/GUI/
+-rw-rw-rw-   0        0        0    22725 2023-05-18 16:04:17.000000 Phasor Noise-1.3.0/src/phasor_noise/GUI/__init__.py
+-rw-rw-rw-   0        0        0     1436 2023-05-18 16:04:17.000000 Phasor Noise-1.3.0/src/phasor_noise/GUI/menu.py
+-rw-rw-rw-   0        0        0      535 2023-05-18 16:04:17.000000 Phasor Noise-1.3.0/src/phasor_noise/GUI/platform_specific.py
+-rw-rw-rw-   0        0        0      546 2023-05-18 16:04:17.000000 Phasor Noise-1.3.0/src/phasor_noise/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.642369 Phasor Noise-1.3.0/src/phasor_noise/analysis/
+-rw-rw-rw-   0        0        0      777 2023-05-18 15:41:41.000000 Phasor Noise-1.3.0/src/phasor_noise/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:41:37.642369 Phasor Noise-1.3.0/src/phasor_noise/generator/
+-rw-rw-rw-   0        0        0     5325 2023-05-18 15:37:46.000000 Phasor Noise-1.3.0/src/phasor_noise/generator/__init__.py
```

### Comparing `Phasor Noise-1.0.1.dev48/LICENSE` & `Phasor Noise-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.0.1.dev48/PKG-INFO` & `Phasor Noise-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Phasor Noise
-Version: 1.0.1.dev48
+Version: 1.3.0
 Home-page: https://github.com/etachouzin/phasor_noise
 Author: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
 Author-email: phasor_noise_dev@outlook.fr
 Maintainer: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
 Maintainer-email: phasor_noise_dev@outlook.fr
 License: GNU
 Keywords: phasor_noise,generator
@@ -18,20 +18,24 @@
 Installation
 -------------
 
 1. Install from PyPI
 
 .. code:: console
 
-   pip install phasor_noise
+   pip install Phasor-Noise
 
 Usage
 ---------
-You can now use our Phasor noise generator. 
+You can now use Phasor-Noise and launch the default window setup.
 
+.. code:: python
+
+   import phasor_noise
+   phasor_noise.default_window()
 
 
 
 License
 -----------
 
 Distributed under the GNU License.
```

### Comparing `Phasor Noise-1.0.1.dev48/docs/Makefile` & `Phasor Noise-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.0.1.dev48/docs/make.bat` & `Phasor Noise-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Phasor Noise-1.0.1.dev48/docs/source/conf.py` & `Phasor Noise-1.3.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 author = 'Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = release = "1.0.1.dev14"
+version = release = "1.3"
 # The full version, including alpha/beta/rc tags.
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
```

### Comparing `Phasor Noise-1.0.1.dev48/docs/source/index.rst` & `Phasor Noise-1.3.0/docs/source/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -26,10 +26,7 @@
 * Guillaume Hisleur
 * Paul Martin
 
 About the project
 -----------------
 Phasor noise is a package providing a generator of procedural phasor noise. |br|
 It claims a graphical interface to visualize how parameters change the noise created.
-
-Project Index
---------------
```

### Comparing `Phasor Noise-1.0.1.dev48/setup.cfg` & `Phasor Noise-1.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 00000130: 7574 6c6f 6f6b 2e66 720d 0a64 6573 6372  utlook.fr..descr
 00000140: 6970 7469 6f6e 5f66 696c 6520 3d20 5245  iption_file = RE
 00000150: 4144 4d45 2e72 7374 0d0a 686f 6d65 5f70  ADME.rst..home_p
 00000160: 6167 6520 3d20 6874 7470 733a 2f2f 6769  age = https://gi
 00000170: 7468 7562 2e63 6f6d 2f65 7461 6368 6f75  thub.com/etachou
 00000180: 7a69 6e2f 7068 6173 6f72 5f6e 6f69 7365  zin/phasor_noise
 00000190: 0d0a 6c69 6365 6e73 6520 3d20 474e 550d  ..license = GNU.
-000001a0: 0a6b 6579 776f 7264 7320 3d20 0d0a 0970  .keywords = ...p
-000001b0: 6861 736f 725f 6e6f 6973 650d 0a09 6765  hasor_noise...ge
-000001c0: 6e65 7261 746f 720d 0a0d 0a5b 6f70 7469  nerator....[opti
-000001d0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-000001e0: 7220 3d20 0d0a 093d 7372 630d 0a0d 0a5b  r = ...=src....[
-000001f0: 6669 6c65 735d 0d0a 7061 636b 6167 6573  files]..packages
-00000200: 203d 200d 0a09 7068 6173 6f72 5f6e 6f69   = ...phasor_noi
-00000210: 7365 0d0a 0d0a 5b70 6272 5d0d 0a73 6b69  se....[pbr]..ski
-00000220: 705f 6368 616e 6765 6c6f 6720 3d20 310d  p_changelog = 1.
-00000230: 0a0d 0a5b 7364 6973 745f 7768 6565 6c5d  ...[sdist_wheel]
-00000240: 0d0a 756e 6976 6572 7361 6c20 3d20 310d  ..universal = 1.
-00000250: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000260: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000270: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000001a0: 0a76 6572 7369 6f6e 203d 2031 2e33 0d0a  .version = 1.3..
+000001b0: 6b65 7977 6f72 6473 203d 200d 0a09 7068  keywords = ...ph
+000001c0: 6173 6f72 5f6e 6f69 7365 0d0a 0967 656e  asor_noise...gen
+000001d0: 6572 6174 6f72 0d0a 0d0a 5b6f 7074 696f  erator....[optio
+000001e0: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+000001f0: 203d 200d 0a09 3d73 7263 0d0a 0d0a 5b66   = ...=src....[f
+00000200: 696c 6573 5d0d 0a70 6163 6b61 6765 7320  iles]..packages 
+00000210: 3d20 0d0a 0970 6861 736f 725f 6e6f 6973  = ...phasor_nois
+00000220: 650d 0a0d 0a5b 7062 725d 0d0a 736b 6970  e....[pbr]..skip
+00000230: 5f63 6861 6e67 656c 6f67 203d 2031 0d0a  _changelog = 1..
+00000240: 0d0a 5b73 6469 7374 5f77 6865 656c 5d0d  ..[sdist_wheel].
+00000250: 0a75 6e69 7665 7273 616c 203d 2031 0d0a  .universal = 1..
+00000260: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000270: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000280: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/PKG-INFO` & `Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Phasor-Noise
-Version: 1.0.1.dev48
+Version: 1.3.0
 Home-page: https://github.com/etachouzin/phasor_noise
 Author: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
 Author-email: phasor_noise_dev@outlook.fr
 Maintainer: Alexis Le Meur, Etienne Tachouzin, Paul Martin, Guillaume Hisleur, Paul Bedrossian
 Maintainer-email: phasor_noise_dev@outlook.fr
 License: GNU
 Keywords: phasor_noise,generator
@@ -18,20 +18,24 @@
 Installation
 -------------
 
 1. Install from PyPI
 
 .. code:: console
 
-   pip install phasor_noise
+   pip install Phasor-Noise
 
 Usage
 ---------
-You can now use our Phasor noise generator. 
+You can now use Phasor-Noise and launch the default window setup.
 
+.. code:: python
+
+   import phasor_noise
+   phasor_noise.default_window()
 
 
 
 License
 -----------
 
 Distributed under the GNU License.
```

### Comparing `Phasor Noise-1.0.1.dev48/src/Phasor_Noise.egg-info/SOURCES.txt` & `Phasor Noise-1.3.0/src/Phasor_Noise.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,27 +14,26 @@
 docs/source/api/index.rst
 docs/source/api/GUI/index.rst
 docs/source/api/analysis/index.rst
 docs/source/api/generator/index.rst
 docs/source/getting_started/index.rst
 docs/source/getting_started/installation.rst
 docs/source/user_guide/index.rst
-src/config.json
 src/phasor_noise/__init__.py
 src/phasor_noise/GUI/__init__.py
 src/phasor_noise/GUI/menu.py
 src/phasor_noise/GUI/platform_specific.py
 src/phasor_noise/analysis/__init__.py
-src/phasor_noise/phasor_noise_generator/__init__.py
+src/phasor_noise/generator/__init__.py
 src/Phasor_Noise.egg-info/PKG-INFO
 src/Phasor_Noise.egg-info/SOURCES.txt
 src/Phasor_Noise.egg-info/dependency_links.txt
 src/Phasor_Noise.egg-info/not-zip-safe
 src/Phasor_Noise.egg-info/pbr.json
 src/Phasor_Noise.egg-info/requires.txt
 src/Phasor_Noise.egg-info/top_level.txt
 src/phasor_noise/__init__.py
 src/phasor_noise/GUI/__init__.py
 src/phasor_noise/GUI/menu.py
 src/phasor_noise/GUI/platform_specific.py
 src/phasor_noise/analysis/__init__.py
-src/phasor_noise/phasor_noise_generator/__init__.py
+src/phasor_noise/generator/__init__.py
```

### Comparing `Phasor Noise-1.0.1.dev48/src/phasor_noise/GUI/__init__.py` & `Phasor Noise-1.3.0/src/phasor_noise/GUI/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,431 +8,488 @@
 from PIL import Image
 from PIL import ImageTk
 import json
 from skimage import exposure
 from copy import deepcopy
 from phasor_noise.GUI.platform_specific import *
 
-class Window():
-    def __init__(self, master, version = "Python") -> None:
+
+class Window:
+    """
+    Window GUI to manipulate the phasor noise and analyse it
+    """
+    def __init__(self, master, version="Python") -> None:
+        """
+        Initialization of the window with default configuration
+        Load a 1090x720 window with the homepage
+        """
         self.master = master
         self.visualize = tk.BooleanVar()
-        self.master.resizable(height = False, width = False)
+        self.master.resizable(height=False, width=False)
         self.master.title("Générateur de bruit Phasor - Version : " + version)
         self.master.geometry("1090x720")
         self.currentPage = 0
         self.gen_mode = version
         self.load_page()
         self.menu = phasor_noise.GUI.menu.Menu(self)
 
-    def save(self): #Save current configuration
+    def save(self):
+        """
+        Save current configuration
+        """
         new_config = {
             "x": self.img_size_x.get(),
             "y": self.img_size_y.get(),
             "nb_ker": self.img_nb_ker.get(),
             "min_freq": self.img_freq_min.get(),
             "max_freq": self.img_freq_max.get(),
             "min_angle": self.img_angle_min.get(),
             "max_angle": self.img_angle_max.get(),
             "min_bandwidth": self.img_bandwidth_min.get(),
             "max_bandwidth": self.img_bandwidth_max.get()
         }
         config_file = open(f"{config_directory()}/config.json", 'w')
         json.dump(new_config, config_file)
-    
-    def reload(self): #Reload the page
+
+    def reload(self):
+        """
+        Reload the page
+        """
         self.page.destroy()
-        config_file = open(f"{config_directory()}/config.json")
-        config = json.load(config_file)
+        path = f"{config_directory()}/config.json"
+        if os.path.exists(path):
+            config_file = open(f"{config_directory()}/config.json", "r")
+            config = json.load(config_file)
+        else:
+            config_file = open(f"{config_directory()}/config.json", "w")
+            config = {"x": "100", "y": "100", "nb_ker": "10", "min_freq": "1", "max_freq": "1", "min_angle": "-1.57",
+                      "max_angle": "1.57", "min_bandwidth": "0.1", "max_bandwidth": "0.1"}
+            json.dump(config, config_file)
         self.config = config
         self.load_page()
 
     def load_page(self):
+        """
+        Load page
+        """
         if self.currentPage == 0:
             self.page = tk.Frame(self.master)
-            self.title = tk.Label(self.page, text=(f"Générateur de bruit Phasor - {self.gen_mode}"), font=("Times", 25))
-            self.title.grid(row=0, column=0, columnspan=2, pady=(20,20))
+            self.title = tk.Label(self.page, text=f"Générateur de bruit Phasor - {self.gen_mode}", font=("Times", 25))
+            self.title.grid(row=0, column=0, columnspan=2, pady=(20, 20))
 
             self.one_image_button = tk.Button(self.page, text="Analyse d'un unique bruit", command=self.one_noise_mode)
-            self.one_image_button.grid(row=1, column=0, ipady=50, pady=(200,50))
+            self.one_image_button.grid(row=1, column=0, ipady=50, pady=(200, 50))
 
             self.multi_test_button = tk.Button(self.page, text="Test de performances", command=self.test_performance)
-            self.multi_test_button.grid(row=1, column=1, ipady=50, pady=(200,50))
+            self.multi_test_button.grid(row=1, column=1, ipady=50, pady=(200, 50))
 
             self.page.pack()
         elif self.currentPage == 1:
             self.page = tk.Frame(self.master)
             self.title = tk.Label(self.page, text=f"Analyse d'un unique bruit - {self.gen_mode}", font=("Times", 20))
-            self.title.grid(row=0, column=0, columnspan=2, pady=(20,70))
+            self.title.grid(row=0, column=0, columnspan=2, pady=(20, 70))
 
             self.visu_img = tk.Canvas(self.page, bg='white', height=500, width=500)
-            self.visu_img.grid(row=1,column=0, rowspan=2, padx=10, sticky="nswe")
+            self.visu_img.grid(row=1, column=0, rowspan=2, padx=10, sticky="nswe")
 
             self.config_img = tk.Frame(self.page, relief=tk.GROOVE, bd=3)
             self.config_img_title = tk.Label(self.config_img, text=f"Configuration du bruit", font=("Times", 15))
             self.config_img_title.grid(row=0, column=0, columnspan=4, ipady=10)
-            
+
             self.img_size_title = tk.Label(self.config_img, text=f"Taille de l'image :")
             self.img_size_title.grid(row=1, column=0)
             self.img_size_x = tk.Entry(self.config_img)
             self.img_size_x.insert(0, str(self.config["x"]))
             self.img_size_x.grid(row=1, column=1)
             self.img_size_label1 = tk.Label(self.config_img, text=f" x ")
-            self.img_size_label1.grid(row= 1, column=2)
+            self.img_size_label1.grid(row=1, column=2)
             self.img_size_y = tk.Entry(self.config_img)
             self.img_size_y.insert(0, str(self.config["y"]))
             self.img_size_y.grid(row=1, column=3)
-            
+
             self.img_nb_ker_title = tk.Label(self.config_img, text=f"Nombre de noyaux :")
             self.img_nb_ker_title.grid(row=2, column=0)
             self.img_nb_ker = tk.Entry(self.config_img)
             self.img_nb_ker.insert(0, str(self.config["nb_ker"]))
             self.img_nb_ker.grid(row=2, column=1)
-            
 
             self.img_freq_title = tk.Label(self.config_img, text=f"Fréquences :")
             self.img_freq_title.grid(row=3, column=0)
             self.img_freq_min = tk.Entry(self.config_img)
             self.img_freq_min.insert(0, str(self.config["min_freq"]))
             self.img_freq_min.grid(row=3, column=1)
             self.img_freq_label = tk.Label(self.config_img, text=f" < f < ")
-            self.img_freq_label.grid(row= 3, column=2)
+            self.img_freq_label.grid(row=3, column=2)
             self.img_freq_max = tk.Entry(self.config_img)
             self.img_freq_max.insert(0, str(self.config["max_freq"]))
             self.img_freq_max.grid(row=3, column=3)
 
             self.img_angle_title = tk.Label(self.config_img, text=f"Angles :")
             self.img_angle_title.grid(row=4, column=0)
             self.img_angle_min = tk.Entry(self.config_img)
             self.img_angle_min.insert(0, str(self.config["min_angle"]))
             self.img_angle_min.grid(row=4, column=1)
             self.img_angle_label = tk.Label(self.config_img, text=f" < a < ")
-            self.img_angle_label.grid(row= 4, column=2)
+            self.img_angle_label.grid(row=4, column=2)
             self.img_angle_max = tk.Entry(self.config_img)
             self.img_angle_max.insert(0, str(self.config["max_angle"]))
             self.img_angle_max.grid(row=4, column=3)
 
             self.img_bandwidth_title = tk.Label(self.config_img, text=f"Bandes :")
             self.img_bandwidth_title.grid(row=5, column=0)
             self.img_bandwidth_min = tk.Entry(self.config_img)
             self.img_bandwidth_min.insert(0, str(self.config["min_bandwidth"]))
             self.img_bandwidth_min.grid(row=5, column=1)
             self.img_bandwidth_label = tk.Label(self.config_img, text=f" < b < ")
-            self.img_bandwidth_label.grid(row= 5, column=2)
+            self.img_bandwidth_label.grid(row=5, column=2)
             self.img_bandwidth_max = tk.Entry(self.config_img)
             self.img_bandwidth_max.insert(0, str(self.config["max_bandwidth"]))
             self.img_bandwidth_max.grid(row=5, column=3)
 
             self.img_gen_button = tk.Button(self.config_img, text="Générer", command=self.validate_entry)
-            self.img_gen_button.grid(row=6, column=0, columnspan=4, pady=(20,0))
-
+            self.img_gen_button.grid(row=6, column=0, columnspan=4, pady=(20, 0))
 
-            self.config_img.grid(row=1,column=1, ipadx=10, ipady=10,  sticky="nwe", pady=(00,0))
+            self.config_img.grid(row=1, column=1, ipadx=10, ipady=10, sticky="nwe", pady=(00, 0))
 
             self.console_img = tk.Frame(self.page, relief=tk.GROOVE, bd=3)
-            
+
             self.console_img_title = tk.Label(self.console_img, text=f"Console", font=("Times", 15))
-            self.console_img_title.grid(row=0, column=0, ipadx=50, pady=(10,0), sticky="w")
-            
+            self.console_img_title.grid(row=0, column=0, ipadx=50, pady=(10, 0), sticky="w")
+
             self.console_text = tk.StringVar()
             self.console_text.set("En attente...")
             self.console_label = tk.Label(self.console_img, textvariable=self.console_text, justify="left")
-            self.console_label.grid(row=1,column=0, sticky="w")
-            self.console_img.grid(row=2, column=1,  sticky="nswe")
-            
+            self.console_label.grid(row=1, column=0, sticky="w")
+            self.console_img.grid(row=2, column=1, sticky="nswe")
+
             self.return_button = tk.Button(self.page, text="Retour", command=self.return_menu)
             self.return_button.grid(row=3, column=1, pady=50, sticky="e")
 
             self.button_chooser = tk.Frame(self.page, relief=tk.GROOVE, bd=3)
             self.img_button = tk.Button(self.button_chooser, text="Image", command=self.visu_mode_img)
             self.img_button.grid(column=0, row=0)
             self.histo_button = tk.Button(self.button_chooser, text="Histogramme", command=self.visu_mode_hist)
             self.histo_button.grid(column=1, row=0)
-            self.psd_button = tk.Button(self.button_chooser, text="Densité spect. de puissance", command=self.visu_mode_psd)
+            self.psd_button = tk.Button(self.button_chooser, text="Densité spect. de puissance",
+                                        command=self.visu_mode_psd)
             self.psd_button.grid(column=2, row=0)
 
             self.button_chooser.grid(row=3, column=0, sticky="n")
 
-
             self.page.pack()
 
         elif self.currentPage == 2:
             self.page = tk.Frame(self.master)
             self.title = tk.Label(self.page, text=f"Test de performances", font=("Times", 20))
-            self.title.grid(row=0, column=0, columnspan=2, pady=(20,70))
+            self.title.grid(row=0, column=0, columnspan=2, pady=(20, 70))
 
             self.visu_img = tk.Canvas(self.page, bg='white', height=500, width=500)
-            self.visu_img.grid(row=1,column=0, rowspan=2, padx=10, sticky="nswe")
+            self.visu_img.grid(row=1, column=0, rowspan=2, padx=10, sticky="nswe")
 
             self.config_img = tk.Frame(self.page, relief=tk.GROOVE, bd=3)
             self.config_img_title = tk.Label(self.config_img, text=f"Configuration des bruits", font=("Times", 15))
             self.config_img_title.grid(row=0, column=0, columnspan=4, ipady=10)
-            
+
             self.img_size_title = tk.Label(self.config_img, text=f"Taille des images :")
             self.img_size_title.grid(row=1, column=0)
             self.img_size_x = tk.Entry(self.config_img)
             self.img_size_x.insert(0, str(self.config["x"]))
             self.img_size_x.grid(row=1, column=1)
             self.img_size_label1 = tk.Label(self.config_img, text=f" x ")
-            self.img_size_label1.grid(row= 1, column=2)
+            self.img_size_label1.grid(row=1, column=2)
             self.img_size_y = tk.Entry(self.config_img)
             self.img_size_y.insert(0, str(self.config["y"]))
             self.img_size_y.grid(row=1, column=3)
-            
+
             self.img_nb_ker_title = tk.Label(self.config_img, text=f"Nombre de noyaux :")
             self.img_nb_ker_title.grid(row=2, column=0)
             self.img_nb_ker = tk.Entry(self.config_img)
             self.img_nb_ker.insert(0, str(self.config["nb_ker"]))
             self.img_nb_ker.grid(row=2, column=1)
-            
 
             self.img_freq_title = tk.Label(self.config_img, text=f"Fréquences :")
             self.img_freq_title.grid(row=3, column=0)
             self.img_freq_min = tk.Entry(self.config_img)
             self.img_freq_min.insert(0, str(self.config["min_freq"]))
             self.img_freq_min.grid(row=3, column=1)
             self.img_freq_label = tk.Label(self.config_img, text=f" < f < ")
-            self.img_freq_label.grid(row= 3, column=2)
+            self.img_freq_label.grid(row=3, column=2)
             self.img_freq_max = tk.Entry(self.config_img)
             self.img_freq_max.insert(0, str(self.config["max_freq"]))
             self.img_freq_max.grid(row=3, column=3)
 
             self.img_angle_title = tk.Label(self.config_img, text=f"Angles :")
             self.img_angle_title.grid(row=4, column=0)
             self.img_angle_min = tk.Entry(self.config_img)
             self.img_angle_min.insert(0, str(self.config["min_angle"]))
             self.img_angle_min.grid(row=4, column=1)
             self.img_angle_label = tk.Label(self.config_img, text=f" < a < ")
-            self.img_angle_label.grid(row= 4, column=2)
+            self.img_angle_label.grid(row=4, column=2)
             self.img_angle_max = tk.Entry(self.config_img)
             self.img_angle_max.insert(0, str(self.config["max_angle"]))
             self.img_angle_max.grid(row=4, column=3)
 
             self.img_bandwidth_title = tk.Label(self.config_img, text=f"Bandes :")
             self.img_bandwidth_title.grid(row=5, column=0)
             self.img_bandwidth_min = tk.Entry(self.config_img)
             self.img_bandwidth_min.insert(0, str(self.config["min_bandwidth"]))
             self.img_bandwidth_min.grid(row=5, column=1)
             self.img_bandwidth_label = tk.Label(self.config_img, text=f" < b < ")
-            self.img_bandwidth_label.grid(row= 5, column=2)
+            self.img_bandwidth_label.grid(row=5, column=2)
             self.img_bandwidth_max = tk.Entry(self.config_img)
             self.img_bandwidth_max.insert(0, str(self.config["max_bandwidth"]))
             self.img_bandwidth_max.grid(row=5, column=3)
             self.number_label = tk.Label(self.config_img, text=f"Occurences :")
-            self.number_label.grid(row= 6, column=0)
+            self.number_label.grid(row=6, column=0)
             self.number = tk.Entry(self.config_img)
             self.number.insert(0, str(self.config["max_bandwidth"]))
             self.number.grid(row=6, column=1)
 
             self.img_gen_button = tk.Button(self.config_img, text="Générer", command=self.validate_entry_performance)
-            self.img_gen_button.grid(row=7, column=0, columnspan=4, pady=(20,0))
-
+            self.img_gen_button.grid(row=7, column=0, columnspan=4, pady=(20, 0))
 
-            self.config_img.grid(row=1,column=1, ipadx=10, ipady=10,  sticky="nwe", pady=(00,0))
+            self.config_img.grid(row=1, column=1, ipadx=10, ipady=10, sticky="nwe", pady=(00, 0))
 
             self.console_img = tk.Frame(self.page, relief=tk.GROOVE, bd=3)
-            
+
             self.console_img_title = tk.Label(self.console_img, text=f"Console", font=("Times", 15))
-            self.console_img_title.grid(row=0, column=0, ipadx=50, pady=(10,0), sticky="w")
-            
+            self.console_img_title.grid(row=0, column=0, ipadx=50, pady=(10, 0), sticky="w")
+
             self.console_text = tk.StringVar()
             self.console_text.set("En attente...")
             self.console_label = tk.Label(self.console_img, textvariable=self.console_text, justify="left")
-            self.console_label.grid(row=1,column=0, sticky="w")
-            self.console_img.grid(row=2, column=1,  sticky="nswe")
-            
+            self.console_label.grid(row=1, column=0, sticky="w")
+            self.console_img.grid(row=2, column=1, sticky="nswe")
+
             self.return_button = tk.Button(self.page, text="Retour", command=self.return_menu)
             self.return_button.grid(row=3, column=1, pady=50, sticky="e")
 
-
             self.page.pack()
 
-        else: 
+        else:
             print("error")
 
     def visu_mode_img(self):
+        """
+        Show image
+        """
         try:
             self.visu_img.delete(self.noise)
         except:
             pass
         try:
             img = Image.open(f"{images_directory()}/noise.png")
-            img.thumbnail((500,500), Image.ANTIALIAS)
+            img.thumbnail((500, 500), Image.ANTIALIAS)
             img.save(f"{images_directory()}/noise_reshape.png")
             self.img = ImageTk.PhotoImage(Image.open(f"{images_directory()}/noise_reshape.png"))
             self.noise = self.visu_img.create_image(0, 0, image=self.img, anchor="nw", tags="IMG")
         except:
             self.console_text.set("Générer d'abord un nouveau bruit !")
 
     def visu_mode_psd(self):
+        """
+        Show power spectral density
+        """
         try:
             self.visu_img.delete(self.noise)
         except:
             pass
         try:
             img = Image.open(f"{images_directory()}/noise_psd.png")
-            img.thumbnail((500,500), Image.ANTIALIAS)
+            img.thumbnail((500, 500), Image.ANTIALIAS)
             img.save(f"{images_directory()}/noise_psd_reshape.png")
             self.img = ImageTk.PhotoImage(Image.open(f"{images_directory()}/noise_psd_reshape.png"))
             self.noise = self.visu_img.create_image(0, 0, image=self.img, anchor="nw", tags="IMG")
         except:
             self.console_text.set("Générer d'abord un nouveau bruit !")
 
     def visu_mode_hist(self):
+        """
+        Show histogram
+        """
         try:
             self.visu_img.delete(self.noise)
         except:
             pass
         try:
             img = Image.open(f"{images_directory()}/noise_hist.png")
-            img.thumbnail((500,500), Image.ANTIALIAS)
+            img.thumbnail((500, 500), Image.ANTIALIAS)
             img.save(f"{images_directory()}/noise_hist_reshape.png")
             self.img = ImageTk.PhotoImage(Image.open(f"{images_directory()}/noise_hist_reshape.png"))
             self.noise = self.visu_img.create_image(0, 0, image=self.img, anchor="nw", tags="IMG")
         except:
             self.console_text.set("Générer d'abord un nouveau bruit !")
 
     def return_menu(self):
+        """
+        Menu
+        """
         self.currentPage = 0
         self.reload()
 
     def validate_entry(self):
+        """
+        Parsing entry values
+        """
         try:
             x = int(self.img_size_x.get())
             y = int(self.img_size_x.get())
             nb_ker = int(self.img_nb_ker.get())
             freq_min = float(self.img_freq_min.get())
-            freq_max = float(self.img_freq_max.get())    
+            freq_max = float(self.img_freq_max.get())
             angle_min = float(self.img_angle_min.get())
             angle_max = float(self.img_angle_max.get())
             bandwidth_min = float(self.img_bandwidth_min.get())
             bandwidth_max = float(self.img_bandwidth_max.get())
             self.console_text.set("Génération du bruit...")
 
         except:
             self.console_text.set("Une erreur est survenu vérifier les valeurs entrées...")
 
-        self.gen_kernels([x,y], nb_ker, [freq_min,freq_max], [angle_min,angle_max], [bandwidth_min, bandwidth_max])
+        self.gen_kernels([x, y], nb_ker, [freq_min, freq_max], [angle_min, angle_max], [bandwidth_min, bandwidth_max])
         self.gen_noise()
 
     def validate_entry_performance(self):
+        """
+        Parsing entry performances values
+        """
         try:
             n = int(self.number.get())
             x = int(self.img_size_x.get())
             y = int(self.img_size_x.get())
             nb_ker = int(self.img_nb_ker.get())
             freq_min = float(self.img_freq_min.get())
-            freq_max = float(self.img_freq_max.get())    
+            freq_max = float(self.img_freq_max.get())
             angle_min = float(self.img_angle_min.get())
             angle_max = float(self.img_angle_max.get())
             bandwidth_min = float(self.img_bandwidth_min.get())
             bandwidth_max = float(self.img_bandwidth_max.get())
             self.console_text.set("Génération du bruit...")
 
         except:
             self.console_text.set("Une erreur est survenu vérifier les valeurs entrées...")
 
-        self.gen_kernels([x,y], nb_ker, [freq_min,freq_max], [angle_min,angle_max], [bandwidth_min, bandwidth_max])
+        self.gen_kernels([x, y], nb_ker, [freq_min, freq_max], [angle_min, angle_max], [bandwidth_min, bandwidth_max])
         self.gen_noise()
-        
 
     def gen_kernels(self, size, nb_ker, freq, angle, bandwidth):
+        """
+        Generation of a kernel
+        """
         self.size = size
         kernels = list()
         for i in range(nb_ker):
-            pos = [rd.randint(0,size[0]), rd.randint(0,size[1])]
+            pos = [rd.randint(0, size[0]), rd.randint(0, size[1])]
             ang = rd.uniform(angle[0], angle[1])
             dire = [np.cos(ang), np.sin(ang)]
             f = rd.uniform(freq[0], freq[1])
             b = rd.uniform(bandwidth[0], bandwidth[1])
-            kernels.append([pos,dire,f,b])
+            kernels.append([pos, dire, f, b])
         self.kernels = kernels
 
     def gen_noise(self):
         if self.gen_mode == "Python":
-            X = np.arange(0,self.size[0])
+            X = np.arange(0, self.size[0])
             Y = np.arange(0, self.size[1])
             X, Y = np.meshgrid(X, Y)
             self.results = phasor_noise.phasor_noise_generator.apply_noise_python(X, Y, self.kernels)
             plt.contourf(X, Y, self.results[0], cmap='Greys')
             plt.colorbar()
             plt.axis('off')
             if self.visualize.get() == 1:
                 for kernel in self.kernels:
-                    plt.plot(kernel[0][0],kernel[0][1], color="green", marker="o")
-                    plt.arrow(kernel[0][0],kernel[0][1], kernel[1][0]*5,kernel[1][1]*5 , width= 1,head_width=2, head_length=2, color="red")
+                    plt.plot(kernel[0][0], kernel[0][1], color="green", marker="o")
+                    plt.arrow(kernel[0][0], kernel[0][1], kernel[1][0] * 5, kernel[1][1] * 5, width=1, head_width=2,
+                              head_length=2, color="red")
             mean = analysis.mean(self.results[0])
             std_gap = analysis.std_gap(self.results[0])
-            self.console_text.set(f"Le bruit à bien été créé en {self.results[1]/10**6} ms ! \n Moyenne: {mean} \n Ecart-type: {std_gap}")
+            self.console_text.set(
+                f"Le bruit à bien été créé en {self.results[1] / 10 ** 6} ms ! \n Moyenne: {mean} \n Ecart-type: {std_gap}")
             plt.savefig(f"{images_directory()}/noise.png", bbox_inches='tight')
             plt.close()
-            
+
             mag = analysis.PSD(np.array(self.results[0]))
-            plt.contourf(X,Y,mag, cmap="Greys")
+            plt.contourf(X, Y, mag, cmap="Greys")
             plt.axis('off')
             plt.colorbar()
             plt.savefig(f"{images_directory()}/noise_psd.png", bbox_inches='tight')
             plt.close()
-        
 
             hist = exposure.histogram(np.array(self.results[0]))
             plt.plot(hist[1], hist[0])
 
             plt.savefig(f"{images_directory()}/noise_hist.png", bbox_inches='tight')
             self.visu_mode_img()
 
             plt.savefig(f"{images_directory()}/noise_hist.png", bbox_inches='tight')
             self.visu_mode_img()
-            
 
         elif self.gen_mode == "Numpy":
-            X = np.arange(0,self.size[0])
+            X = np.arange(0, self.size[0])
             Y = np.arange(0, self.size[1])
             X, Y = np.meshgrid(X, Y)
-            self.results = phasor_noise.phasor_noise_generator.apply_noise_numpy(X, Y, deepcopy(self.kernels), self.size)
+            self.results = phasor_noise.phasor_noise_generator.apply_noise_numpy(X, Y, deepcopy(self.kernels),
+                                                                                 self.size)
             plt.contourf(X, Y, self.results[0], cmap='Greys')
             plt.axis('off')
             plt.colorbar()
             if self.visualize.get() == 1:
                 for kernel in self.kernels:
-                    plt.plot(kernel[0][0],kernel[0][1], color="green", marker="o")
-                    plt.arrow(kernel[0][0],kernel[0][1], kernel[1][0]*5,kernel[1][1]*5 , width= 1,head_width=2, head_length=2, color="red")
+                    plt.plot(kernel[0][0], kernel[0][1], color="green", marker="o")
+                    plt.arrow(kernel[0][0], kernel[0][1], kernel[1][0] * 5, kernel[1][1] * 5, width=1, head_width=2,
+                              head_length=2, color="red")
             mean = analysis.mean(self.results[0])
             std_gap = analysis.std_gap(self.results[0])
-            self.console_text.set(f"Le bruit à bien été créé en {self.results[1]/10**6} ms !\n Moyenne: {mean}\nEcart-type: {std_gap}")
+            self.console_text.set(
+                f"Le bruit à bien été créé en {self.results[1] / 10 ** 6} ms !\n Moyenne: {mean}\nEcart-type: {std_gap}")
             plt.savefig(f"{images_directory()}/noise.png", bbox_inches='tight')
             plt.close()
 
             mag = analysis.PSD(np.array(self.results[0]))
-            plt.contourf(X,Y,mag, cmap='Greys')
+            plt.contourf(X, Y, mag, cmap='Greys')
             plt.axis('off')
             plt.colorbar()
             plt.savefig(f"{images_directory()}/noise_psd.png", bbox_inches='tight')
             plt.close()
-            
+
             hist = exposure.histogram(np.array(self.results[0]))
             plt.plot(hist[1], hist[0])
 
             plt.savefig(f"{images_directory()}/noise_hist.png", bbox_inches='tight')
             self.visu_mode_img()
 
         plt.close()
 
     def one_noise_mode(self):
+        """
+        One noise mode
+        """
         self.currentPage = 1
         self.reload()
-    
+
     def test_performance(self):
+        """
+        Testing performance
+        """
         self.currentPage = 2
         self.reload()
 
     def change_mode_python(self):
+        """
+        Set to builtins Python calculation
+        """
         self.gen_mode = "Python"
         self.reload()
 
     def change_mode_numpy(self):
+        """
+        Set to numpy calculation
+        """
         self.gen_mode = "Numpy"
         self.reload()
 
     def change_mode_jax(self):
-        self.gen_mode = "JAX"  
-        self.reload()  
+        """
+        Set to Jax calculation
+        """
+        self.gen_mode = "JAX"
+        self.reload()
```

### Comparing `Phasor Noise-1.0.1.dev48/src/phasor_noise/GUI/menu.py` & `Phasor Noise-1.3.0/src/phasor_noise/GUI/menu.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import tkinter as tk
 
-class Menu():
+
+class Menu:
+    """
+    Menu is class to create the different sections of the window
+    """
     def __init__(self, gui) -> None:
-        #Main top menu
-        mainmenu  = tk.Menu (relief=tk.RAISED, borderwidth=3)
+        """
+        Set the main menu on top and set the version with parameters and save and load it
+        """
+        mainmenu = tk.Menu(relief=tk.RAISED, borderwidth=3)
 
-        #Version chooser section
-        version= tk.Menu(mainmenu, tearoff=0)
-        mainmenu.add_cascade(label= "Version", menu = version)
+        version = tk.Menu(mainmenu, tearoff=0)
+        mainmenu.add_cascade(label="Version", menu=version)
         version.add_radiobutton(label="Python")
         version.add_radiobutton(label="Numpy")
         version.add_radiobutton(label="JAX")
         version.entryconfigure("Python", command=gui.change_mode_python)
         version.entryconfigure("Numpy", command=gui.change_mode_numpy)
         version.entryconfigure("JAX", command=gui.change_mode_jax)
 
-        #Parameters chooser section
         param = tk.Menu(mainmenu, tearoff=0)
-        mainmenu.add_cascade(label= "Paramètres", menu=param)
+        mainmenu.add_cascade(label="Paramètres", menu=param)
 
-        #Save configuration 
         save = tk.Menu(mainmenu, tearoff=0)
         param.add_cascade(label="Sauvegarde des données", menu=save)
         save.add_command(label="Sauvegarder la configuration", command=gui.save)
 
-        #Visualize options
-        visu= tk.Menu(mainmenu, tearoff=0)
+        visu = tk.Menu(mainmenu, tearoff=0)
         param.add_cascade(label="Visualisation", menu=visu)
         visu.add_separator()
         visu.add_checkbutton(label="Afficher les noyaux", onvalue=1, offvalue=0, variable=gui.visualize)
         visu.add_separator()
 
-        #Load the menu
-        gui.master.config(menu = mainmenu)
+        gui.master.config(menu=mainmenu)
```

### Comparing `Phasor Noise-1.0.1.dev48/src/phasor_noise/analysis/__init__.py` & `Phasor Noise-1.3.0/src/phasor_noise/analysis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import numpy as np
 
 
 def PSD(signal: list) -> np.array:
     """
-    The Power Spectral Density PSD is defined by :
-    P = |x̂(f)|² with x̂ the Fourier Transform of the Signal
-
-    PSD(signal) return the Power Spectral Density of a signal
-
-    plotPSD(X,Y,signal,ax) plot the Power Spectral Density on a 3D axis
+    PSD = |x̂(f)|² with x̂ the Fourier Transform of the Signal scale by the time of integration
+    :param signal : a ndarray or list containing the evaluated value by a function
+    return : the Power Spectral Density of a signal
     """
     f = np.fft.fft2(signal)
     f_s = np.fft.fftshift(f)
     resp = np.power(np.absolute(f_s), 2)
     return -resp
```

### Comparing `Phasor Noise-1.0.1.dev48/src/phasor_noise/phasor_noise_generator/__init__.py` & `Phasor Noise-1.3.0/src/phasor_noise/generator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,12 @@
-"""
-Nom :           phasor/phasor_py.py
-Decription :    Script d'application de bruit Phasor en utilisant uniquement python
-Date :          30/01/2023
-Auteur :        Alexis
-Statut :        Fonctionne en v1.0 (A faire relire par Alexis)
-"""
+"""Script d'application de bruit Phasor en utilisant uniquement python"""
 import math
 import numpy as np
 
 
-# Section des imports   
-
-# Section de définition des fonctions
-"""
-apply_function applique à une matrice la fonction de bruit Phasor avec les noyaux passés en arguments
-Matrice : X, Y -> np.meshgrid()
-Un noyau est défini par : [position, direction, frequence, largeur]
-"""
 class PhasorGenerator:
     """
     Classe inutilisable dans l'état doit redéfinir:
      -exp
      -sin
      -cos
      -atan2
@@ -67,51 +53,54 @@
 
     def vector_subtraction(self, vector1: list, vector2: list):
         """
         vector_subtraction retourne la soustraction de deux vecteurs (vector1 et vector2)
         """
         raise NotImplemented()
 
-    def gaussian(self, vector:list, bandwidth:float) -> float:
+    def gaussian(self, vector: list, bandwidth: float) -> float:
         """
         gaussian retourne le résultat du vecteur (vector) par la fonction gaussienne avec une largeur définie (bandwidth)
         """
-        return self.exp(-math.pi*(bandwidth**2)*self.dot(vector, vector))
+        return self.exp(-math.pi * (bandwidth ** 2) * self.dot(vector, vector))
 
     def polar_coordinates_coefficients(self, x: list, kernel_array: list) -> list:
         """
         polar_coordinates_coefficients retourne la somme des coordonnées polaires des vecteurs (A vérifier par Alexis)
         """
         return [self.gaussian(self.vector_subtraction(x, kernel[0]), kernel[3]) * self.sin(
             -self.dot(self.vector_subtraction(x, kernel[0]), kernel[1]) * kernel[2]) for kernel in kernel_array], \
-               [self.gaussian(self.vector_subtraction(x, kernel[0]), kernel[3]) * self.cos(
-                   -self.dot(self.vector_subtraction(x, kernel[0]), kernel[1]) * kernel[2]) for kernel in kernel_array]
+            [self.gaussian(self.vector_subtraction(x, kernel[0]), kernel[3]) * self.cos(
+                -self.dot(self.vector_subtraction(x, kernel[0]), kernel[1]) * kernel[2]) for kernel in kernel_array]
 
     def phase_func(self, x: list, kernel_array: list) -> float:
         """
         phase_func retourne la phase du bruit calculé
         """
         l1, l2 = self.polar_coordinates_coefficients(x, kernel_array)
         return self.atan2(sum(l1), sum(l2))
 
     def phasor_noise(self, x: list, kernel_array: list) -> float:
         """
             phasor_noise retourne le sinus de la phase du bruit calculé
         """
         return self.sin(self.phase_func(x, kernel_array))
 
+
 def timeperf(func):
     def inner(*args, **kargs):
         import time
         begin = time.perf_counter_ns()
         result = func(*args, **kargs)
         end = time.perf_counter_ns()
-        return result, end-begin
+        return result, end - begin
+
     return inner
 
+
 class PythonPhasorGenerator(PhasorGenerator):
 
     def exp(self, x):
         return math.exp(x)
 
     def sin(self, x):
         return math.sin(x)
@@ -119,18 +108,19 @@
     def cos(self, x):
         return math.cos(x)
 
     def atan2(self, x, y):
         return math.atan2(x, y)
 
     def dot(self, vector1, vector2):
-        return vector1[0]*vector2[0]+vector1[1]*vector2[1]
+        return vector1[0] * vector2[0] + vector1[1] * vector2[1]
 
     def vector_subtraction(self, vector1: list, vector2: list):
-        return [vector1[0]-vector2[0], vector1[1]-vector2[1]]
+        return [vector1[0] - vector2[0], vector1[1] - vector2[1]]
+
 
 class NumpyPhasorGenerator(PhasorGenerator):
 
     def exp(self, x):
         return np.exp(x)
 
     def sin(self, x):
@@ -139,37 +129,45 @@
     def cos(self, x):
         return np.cos(x)
 
     def atan2(self, x, y):
         return np.arctan2(x, y)
 
     def dot(self, vector1, vector2):
-        return vector1[0]*vector2[0]+vector1[1]*vector2[1]
+        return vector1[0] * vector2[0] + vector1[1] * vector2[1]
 
     def vector_subtraction(self, vector1: list, vector2: list):
-        return vector1-vector2
+        return vector1 - vector2
+
 
 @timeperf
-def apply_noise_python(X:list, Y:list, kernels:list) -> list:
+def apply_noise_python(x: list, y: list, kernels: list) -> list:
+    """
+    apply_function applique à une matrice la fonction de bruit Phasor avec les noyaux passés en arguments
+    Matrice : X, Y -> np.meshgrid()
+    Un noyau est défini par : [position, direction, frequence, largeur]
+    """
     Z = list()
     phasor_generator = PythonPhasorGenerator()
-    for i in range(len(X)):
+    for i in range(len(x)):
         Z.insert(i, [])
-        for j in range(len(Y)):
-            vector = X[i][j], Y[i][j]
-            Z[i].insert(j, phasor_generator.phasor_noise(vector, kernels)) # On redéfinit le pixel par la nouvelle valeur calculer avec le bruit Phasor
+        for j in range(len(y)):
+            vector = x[i][j], y[i][j]
+            Z[i].insert(j, phasor_generator.phasor_noise(vector,
+                                                         kernels))
     return Z
 
-def create_numpy_kernel(kernels, sizeX, sizeY):
+
+def create_numpy_kernel(kernels, size_x, size_y):
     for i in range(len(kernels)):
-        kernels[i][0] = np.array([np.full((sizeX, sizeY), kernels[i][0][0]),
-                               np.full((sizeX, sizeY), kernels[i][0][1])])
-        kernels[i][1] = np.array([np.full((sizeX, sizeY), kernels[i][1][0]),
-                               np.full((sizeX, sizeY), kernels[i][1][1])])
+        kernels[i][0] = np.array([np.full((size_x, size_y), kernels[i][0][0]),
+                                  np.full((size_x, size_y), kernels[i][0][1])])
+        kernels[i][1] = np.array([np.full((size_x, size_y), kernels[i][1][0]),
+                                  np.full((size_x, size_y), kernels[i][1][1])])
     return kernels
 
+
 @timeperf
-def apply_noise_numpy(X:list, Y:list, kernels:list, size:list) -> list:
+def apply_noise_numpy(x: list, y: list, kernels: list, size: list) -> list:
     kernels = create_numpy_kernel(kernels, size[0], size[1])
-    Z = NumpyPhasorGenerator().phasor_noise(np.array([X, Y]), kernels)
+    Z = NumpyPhasorGenerator().phasor_noise(np.array([x, y]), kernels)
     return Z
-
```

