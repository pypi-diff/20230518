# Comparing `tmp/tusuan-0.0.5.3.tar.gz` & `tmp/tusuan-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tusuan-0.0.5.3.tar", last modified: Mon May  8 18:14:27 2023, max compression
+gzip compressed data, was "tusuan-0.0.6.1.tar", last modified: Thu May 18 10:11:10 2023, max compression
```

## Comparing `tusuan-0.0.5.3.tar` & `tusuan-0.0.6.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-08 18:14:27.744439 tusuan-0.0.5.3/
--rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.5.3/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-08 18:14:27.744319 tusuan-0.0.5.3/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.5.3/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)       84 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-05-08 18:14:27.744480 tusuan-0.0.5.3/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1648 2023-05-08 18:14:20.000000 tusuan-0.0.5.3/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-08 18:14:27.743037 tusuan-0.0.5.3/tusuan/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.5.3/tusuan/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.5.3/tusuan/file_function.py
--rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.5.3/tusuan/hello.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-08 18:14:27.744153 tusuan-0.0.5.3/tusuan/image_video_utils/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.5.3/tusuan/image_video_utils/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2137 2023-05-08 05:08:27.000000 tusuan-0.0.5.3/tusuan/image_video_utils/croppers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1163 2023-05-07 17:43:48.000000 tusuan-0.0.5.3/tusuan/image_video_utils/display.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.5.3/tusuan/image_video_utils/image_visual_selector.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     4013 2023-05-08 05:14:00.000000 tusuan-0.0.5.3/tusuan/image_video_utils/readers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2583 2023-05-08 18:11:39.000000 tusuan-0.0.5.3/tusuan/image_video_utils/writers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.5.3/tusuan/path_utils.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-08 18:14:27.743489 tusuan-0.0.5.3/tusuan.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      508 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       84 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-05-08 18:14:27.000000 tusuan-0.0.5.3/tusuan.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.576080 tusuan-0.0.6.1/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.6.1/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-18 10:11:10.575965 tusuan-0.0.6.1/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.6.1/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 10:11:09.000000 tusuan-0.0.6.1/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-05-18 10:11:10.576122 tusuan-0.0.6.1/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1648 2023-05-18 10:10:58.000000 tusuan-0.0.6.1/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.574527 tusuan-0.0.6.1/tusuan/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.6.1/tusuan/__init__.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.575257 tusuan-0.0.6.1/tusuan/datasets/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-05-18 04:55:21.000000 tusuan-0.0.6.1/tusuan/datasets/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     4327 2023-05-18 08:45:26.000000 tusuan-0.0.6.1/tusuan/datasets/imagenet.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.6.1/tusuan/file_function.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.6.1/tusuan/hello.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.575825 tusuan-0.0.6.1/tusuan/image_video_utils/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.6.1/tusuan/image_video_utils/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2137 2023-05-08 05:08:27.000000 tusuan-0.0.6.1/tusuan/image_video_utils/croppers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1163 2023-05-07 17:43:48.000000 tusuan-0.0.6.1/tusuan/image_video_utils/display.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.6.1/tusuan/image_video_utils/image_visual_selector.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     4013 2023-05-08 05:14:00.000000 tusuan-0.0.6.1/tusuan/image_video_utils/readers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2583 2023-05-08 18:11:39.000000 tusuan-0.0.6.1/tusuan/image_video_utils/writers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.6.1/tusuan/path_utils.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       97 2023-05-14 11:47:37.000000 tusuan-0.0.6.1/tusuan/time_utils.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.575071 tusuan-0.0.6.1/tusuan.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      585 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/top_level.txt
```

### Comparing `tusuan-0.0.5.3/PKG-INFO` & `tusuan-0.0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.5.3
+Version: 0.0.6.1
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

### Comparing `tusuan-0.0.5.3/setup.py` & `tusuan-0.0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from read import read
 from setuptools import setup, find_packages
 
 setup(name='tusuan',  # 包名
       python_requires='>=3.8.0',  # python环境
-      version='0.0.5.3',  # 包的版本
+      version='0.0.6.1',  # 包的版本
       description="useful functions.",  # 包简介，显示在PyPI上
 
       long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
       long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
       author="tusuan",  # 作者相关信息
       author_email='btk@qq.com',
```

### Comparing `tusuan-0.0.5.3/tusuan/file_function.py` & `tusuan-0.0.6.1/tusuan/file_function.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.5.3/tusuan/image_video_utils/croppers.py` & `tusuan-0.0.6.1/tusuan/image_video_utils/croppers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.5.3/tusuan/image_video_utils/display.py` & `tusuan-0.0.6.1/tusuan/image_video_utils/display.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.5.3/tusuan/image_video_utils/image_visual_selector.py` & `tusuan-0.0.6.1/tusuan/image_video_utils/image_visual_selector.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.5.3/tusuan/image_video_utils/readers.py` & `tusuan-0.0.6.1/tusuan/image_video_utils/readers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.5.3/tusuan/image_video_utils/writers.py` & `tusuan-0.0.6.1/tusuan/image_video_utils/writers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.5.3/tusuan.egg-info/PKG-INFO` & `tusuan-0.0.6.1/tusuan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.5.3
+Version: 0.0.6.1
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

