# Comparing `tmp/exn-0.0.8.tar.gz` & `tmp/exn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exn-0.0.8.tar", last modified: Thu May 18 18:31:48 2023, max compression
+gzip compressed data, was "dist/exn-0.0.9.tar", last modified: Thu May 18 19:16:02 2023, max compression
```

## Comparing `exn-0.0.8.tar` & `exn-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.798640 exn-0.0.8/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2023-01-27 15:41:30.000000 exn-0.0.8/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       65 2022-05-20 19:28:46.000000 exn-0.0.8/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)    15602 2023-05-18 18:31:48.798640 exn-0.0.8/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)    15044 2023-02-28 20:51:27.000000 exn-0.0.8/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2023-05-18 18:01:35.000000 exn-0.0.8/VERSION
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.794640 exn-0.0.8/exn/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-12-13 20:40:48.000000 exn-0.0.8/exn/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     3085 2023-02-22 20:15:04.000000 exn-0.0.8/exn/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.794640 exn-0.0.8/exn/constant/
--rw-rw-r--   0 alex      (1002) alex      (1003)      225 2023-02-25 00:54:34.000000 exn-0.0.8/exn/constant/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.794640 exn-0.0.8/exn/dao/
--rw-rw-r--   0 alex      (1002) alex      (1003)     3290 2023-05-18 18:20:24.000000 exn-0.0.8/exn/dao/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.794640 exn-0.0.8/exn/dto/
--rw-rw-r--   0 alex      (1002) alex      (1003)      274 2022-12-16 11:07:37.000000 exn-0.0.8/exn/dto/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.798640 exn-0.0.8/exn/manager/
--rw-rw-r--   0 alex      (1002) alex      (1003)     5296 2023-02-22 20:05:35.000000 exn-0.0.8/exn/manager/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.798640 exn-0.0.8/exn/theme/
--rw-rw-r--   0 alex      (1002) alex      (1003)    27587 2023-02-22 20:05:35.000000 exn-0.0.8/exn/theme/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.798640 exn-0.0.8/exn/utils/
--rw-rw-r--   0 alex      (1002) alex      (1003)     4241 2023-05-18 18:23:36.000000 exn-0.0.8/exn/utils/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.798640 exn-0.0.8/exn/view/
--rw-rw-r--   0 alex      (1002) alex      (1003)      180 2023-01-07 08:25:20.000000 exn-0.0.8/exn/view/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2394 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/about.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     3909 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/board.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    13643 2023-02-19 13:35:55.000000 exn-0.0.8/exn/view/footer.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     3948 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/front.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4455 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/goto.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4912 2023-02-22 20:20:26.000000 exn-0.0.8/exn/view/info.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2128 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/past.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    15821 2023-02-22 20:20:03.000000 exn-0.0.8/exn/view/roll.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     9903 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/search.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2844 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/switcher.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     6450 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/toc.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     5880 2023-02-22 20:15:03.000000 exn-0.0.8/exn/view/top.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      690 2023-02-19 16:05:49.000000 exn-0.0.8/exn/view/util.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.794640 exn-0.0.8/exn.egg-info/
--rw-rw-r--   0 alex      (1002) alex      (1003)    15602 2023-05-18 18:31:48.000000 exn-0.0.8/exn.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)      695 2023-05-18 18:31:48.000000 exn-0.0.8/exn.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-05-18 18:31:48.000000 exn-0.0.8/exn.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       43 2023-05-18 18:31:48.000000 exn-0.0.8/exn.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-02-25 02:18:23.000000 exn-0.0.8/exn.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)       59 2023-05-18 18:31:48.000000 exn-0.0.8/exn.egg-info/requires.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       10 2023-05-18 18:31:48.000000 exn-0.0.8/exn.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:28:46.000000 exn-0.0.8/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      813 2023-05-18 18:31:48.798640 exn-0.0.8/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:28:46.000000 exn-0.0.8/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 18:31:48.798640 exn-0.0.8/tests/
--rw-rw-r--   0 alex      (1002) alex      (1003)        8 2023-02-20 09:02:12.000000 exn-0.0.8/tests/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.844127 exn-0.0.9/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2023-01-27 15:41:30.000000 exn-0.0.9/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       65 2022-05-20 19:28:46.000000 exn-0.0.9/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15602 2023-05-18 19:16:02.844127 exn-0.0.9/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15044 2023-02-28 20:51:27.000000 exn-0.0.9/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2023-05-18 18:31:48.000000 exn-0.0.9/VERSION
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.840127 exn-0.0.9/exn/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2022-12-13 20:40:48.000000 exn-0.0.9/exn/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3086 2023-05-18 19:15:50.000000 exn-0.0.9/exn/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.840127 exn-0.0.9/exn/constant/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      225 2023-02-25 00:54:34.000000 exn-0.0.9/exn/constant/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.840127 exn-0.0.9/exn/dao/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3290 2023-05-18 19:13:45.000000 exn-0.0.9/exn/dao/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.840127 exn-0.0.9/exn/dto/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      274 2022-12-16 11:07:37.000000 exn-0.0.9/exn/dto/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.840127 exn-0.0.9/exn/manager/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     5296 2023-02-22 20:05:35.000000 exn-0.0.9/exn/manager/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.840127 exn-0.0.9/exn/theme/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    27587 2023-02-22 20:05:35.000000 exn-0.0.9/exn/theme/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.840127 exn-0.0.9/exn/utils/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4272 2023-05-18 19:15:50.000000 exn-0.0.9/exn/utils/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.844127 exn-0.0.9/exn/view/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      180 2023-01-07 08:25:20.000000 exn-0.0.9/exn/view/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2394 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/about.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3909 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/board.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    13643 2023-02-19 13:35:55.000000 exn-0.0.9/exn/view/footer.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3948 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/front.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4455 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/goto.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4912 2023-02-22 20:20:26.000000 exn-0.0.9/exn/view/info.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2128 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/past.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15821 2023-02-22 20:20:03.000000 exn-0.0.9/exn/view/roll.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     9903 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/search.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2844 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/switcher.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     6450 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/toc.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     5880 2023-02-22 20:15:03.000000 exn-0.0.9/exn/view/top.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      690 2023-02-19 16:05:49.000000 exn-0.0.9/exn/view/util.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.840127 exn-0.0.9/exn.egg-info/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15602 2023-05-18 19:16:02.000000 exn-0.0.9/exn.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      695 2023-05-18 19:16:02.000000 exn-0.0.9/exn.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-05-18 19:16:02.000000 exn-0.0.9/exn.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       43 2023-05-18 19:16:02.000000 exn-0.0.9/exn.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-02-25 02:18:23.000000 exn-0.0.9/exn.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       59 2023-05-18 19:16:02.000000 exn-0.0.9/exn.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       10 2023-05-18 19:16:02.000000 exn-0.0.9/exn.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:28:46.000000 exn-0.0.9/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      813 2023-05-18 19:16:02.844127 exn-0.0.9/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2022-05-20 19:28:46.000000 exn-0.0.9/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2023-05-18 19:16:02.844127 exn-0.0.9/tests/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        8 2023-02-20 09:02:12.000000 exn-0.0.9/tests/__init__.py
```

### Comparing `exn-0.0.8/LICENSE` & `exn-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/PKG-INFO` & `exn-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Browse a dossier of exonotes
 Home-page: https://github.com/pyrustic/exn
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exn Version: 0.0.8 Summary: Browse a dossier of
+Metadata-Version: 2.1 Name: exn Version: 0.0.9 Summary: Browse a dossier of
 exonotes Home-page: https://github.com/pyrustic/exn Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com Maintainer: Pyrustic Evangelist Maintainer-
 email: rusticalex@yahoo.com License: MIT Keywords: application,pyrustic
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.5 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `exn-0.0.8/README.md` & `exn-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/__main__.py` & `exn-0.0.9/exn/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     if target:
         target = update_target(target)
     dossier = os.getcwd()
     manager = Manager(dossier, restriction)
     manager.start(target)
 
 
+
 def build_index():
     dossier = os.getcwd()
     utils.IndexBuilder.build(dossier)
     print("Index successfully built !")
 
 
 def update_target(target):
```

### Comparing `exn-0.0.8/exn/dao/__init__.py` & `exn-0.0.9/exn/dao/__init__.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/manager/__init__.py` & `exn-0.0.9/exn/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/theme/__init__.py` & `exn-0.0.9/exn/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/utils/__init__.py` & `exn-0.0.9/exn/utils/__init__.py`

 * *Files identical despite different names*

```diff
@@ -113,14 +113,16 @@
         text = "\n\n".join(sections)
         with open(path, "w") as file:
             file.write(text)
 
 
 def read_style_file(path):
     doc = jesth.read(path)
+    if not doc:
+        return
     section = doc.get("")
     body = section.body if section else list()
     style_data = dict()
     if not body:
         return
     for line in body:
         if not line or line.startswith("#"):
```

### Comparing `exn-0.0.8/exn/view/about.py` & `exn-0.0.9/exn/view/about.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/board.py` & `exn-0.0.9/exn/view/board.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/footer.py` & `exn-0.0.9/exn/view/footer.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/front.py` & `exn-0.0.9/exn/view/front.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/goto.py` & `exn-0.0.9/exn/view/goto.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/info.py` & `exn-0.0.9/exn/view/info.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/past.py` & `exn-0.0.9/exn/view/past.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/roll.py` & `exn-0.0.9/exn/view/roll.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/search.py` & `exn-0.0.9/exn/view/search.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/switcher.py` & `exn-0.0.9/exn/view/switcher.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/toc.py` & `exn-0.0.9/exn/view/toc.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/top.py` & `exn-0.0.9/exn/view/top.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn/view/util.py` & `exn-0.0.9/exn/view/util.py`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/exn.egg-info/PKG-INFO` & `exn-0.0.9/exn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Browse a dossier of exonotes
 Home-page: https://github.com/pyrustic/exn
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exn Version: 0.0.8 Summary: Browse a dossier of
+Metadata-Version: 2.1 Name: exn Version: 0.0.9 Summary: Browse a dossier of
 exonotes Home-page: https://github.com/pyrustic/exn Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com Maintainer: Pyrustic Evangelist Maintainer-
 email: rusticalex@yahoo.com License: MIT Keywords: application,pyrustic
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.5 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `exn-0.0.8/exn.egg-info/SOURCES.txt` & `exn-0.0.9/exn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exn-0.0.8/setup.cfg` & `exn-0.0.9/setup.cfg`

 * *Files identical despite different names*

