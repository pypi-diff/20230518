# Comparing `tmp/wordcloud-1.9.1.1.tar.gz` & `tmp/wordcloud-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordcloud-1.9.1.1.tar", last modified: Thu Apr 27 20:34:02 2023, max compression
+gzip compressed data, was "wordcloud-1.9.2.tar", last modified: Thu May 18 17:57:26 2023, max compression
```

## Comparing `wordcloud-1.9.1.1.tar` & `wordcloud-1.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:34:02.912752 wordcloud-1.9.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-27 20:34:02.912752 wordcloud-1.9.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-27 20:34:02.912752 wordcloud-1.9.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:34:02.908752 wordcloud-1.9.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/test/test_wordcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/test/test_wordcloud_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    68612 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:34:02.912752 wordcloud-1.9.1.1/wordcloud/
--rw-r--r--   0 runner    (1001) docker     (123)   119380 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/DroidSansMono.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 20:34:02.912752 wordcloud-1.9.1.1/wordcloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/color_from_image.py
--rw-r--r--   0 runner    (1001) docker     (123)   790205 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/query_integral_image.c
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/stopwords
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)    38158 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/wordcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-04-27 20:33:48.000000 wordcloud-1.9.1.1/wordcloud/wordcloud_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:34:02.912752 wordcloud-1.9.1.1/wordcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-27 20:34:02.000000 wordcloud-1.9.1.1/wordcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-27 20:34:02.000000 wordcloud-1.9.1.1/wordcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:34:02.000000 wordcloud-1.9.1.1/wordcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 20:34:02.000000 wordcloud-1.9.1.1/wordcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 20:34:02.000000 wordcloud-1.9.1.1/wordcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 20:34:02.000000 wordcloud-1.9.1.1/wordcloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:26.378554 wordcloud-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 17:57:13.000000 wordcloud-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-18 17:57:13.000000 wordcloud-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-18 17:57:26.378554 wordcloud-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-18 17:57:13.000000 wordcloud-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-18 17:57:26.378554 wordcloud-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-18 17:57:13.000000 wordcloud-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:26.374554 wordcloud-1.9.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-18 17:57:13.000000 wordcloud-1.9.2/test/test_wordcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-05-18 17:57:13.000000 wordcloud-1.9.2/test/test_wordcloud_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68612 2023-05-18 17:57:13.000000 wordcloud-1.9.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:26.378554 wordcloud-1.9.2/wordcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)   119380 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/DroidSansMono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-18 17:57:26.378554 wordcloud-1.9.2/wordcloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/color_from_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   790205 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/query_integral_image.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/stopwords
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38158 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/wordcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-05-18 17:57:13.000000 wordcloud-1.9.2/wordcloud/wordcloud_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:57:26.378554 wordcloud-1.9.2/wordcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-18 17:57:26.000000 wordcloud-1.9.2/wordcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-18 17:57:26.000000 wordcloud-1.9.2/wordcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:57:26.000000 wordcloud-1.9.2/wordcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 17:57:26.000000 wordcloud-1.9.2/wordcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 17:57:26.000000 wordcloud-1.9.2/wordcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 17:57:26.000000 wordcloud-1.9.2/wordcloud.egg-info/top_level.txt
```

### Comparing `wordcloud-1.9.1.1/LICENSE` & `wordcloud-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/PKG-INFO` & `wordcloud-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordcloud
-Version: 1.9.1.1
+Version: 1.9.2
 Summary: A little word cloud generator
 Home-page: https://github.com/amueller/word_cloud
 Author: Andreas Mueller
 Author-email: t3kcit+wordcloud@gmail.com
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
```

### Comparing `wordcloud-1.9.1.1/README.md` & `wordcloud-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/setup.cfg` & `wordcloud-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/setup.py` & `wordcloud-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/test/test_wordcloud.py` & `wordcloud-1.9.2/test/test_wordcloud.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/test/test_wordcloud_cli.py` & `wordcloud-1.9.2/test/test_wordcloud_cli.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/versioneer.py` & `wordcloud-1.9.2/versioneer.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud/DroidSansMono.ttf` & `wordcloud-1.9.2/wordcloud/DroidSansMono.ttf`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud/__main__.py` & `wordcloud-1.9.2/wordcloud/__main__.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud/color_from_image.py` & `wordcloud-1.9.2/wordcloud/color_from_image.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud/query_integral_image.c` & `wordcloud-1.9.2/wordcloud/query_integral_image.c`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud/stopwords` & `wordcloud-1.9.2/wordcloud/stopwords`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud/tokenization.py` & `wordcloud-1.9.2/wordcloud/tokenization.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud/wordcloud.py` & `wordcloud-1.9.2/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud/wordcloud_cli.py` & `wordcloud-1.9.2/wordcloud/wordcloud_cli.py`

 * *Files identical despite different names*

### Comparing `wordcloud-1.9.1.1/wordcloud.egg-info/PKG-INFO` & `wordcloud-1.9.2/wordcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordcloud
-Version: 1.9.1.1
+Version: 1.9.2
 Summary: A little word cloud generator
 Home-page: https://github.com/amueller/word_cloud
 Author: Andreas Mueller
 Author-email: t3kcit+wordcloud@gmail.com
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
```

### Comparing `wordcloud-1.9.1.1/wordcloud.egg-info/SOURCES.txt` & `wordcloud-1.9.2/wordcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

