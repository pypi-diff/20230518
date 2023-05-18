# Comparing `tmp/jcmutils-1.5.3.tar.gz` & `tmp/jcmutils-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.5.3.tar", last modified: Thu May 18 08:41:29 2023, max compression
+gzip compressed data, was "jcmutils-1.5.4.tar", last modified: Thu May 18 08:47:25 2023, max compression
```

## Comparing `jcmutils-1.5.3.tar` & `jcmutils-1.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:41:29.316414 jcmutils-1.5.3/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.3/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:41:29.316414 jcmutils-1.5.3/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.3/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:41:29.316414 jcmutils-1.5.3/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.3/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    11233 2023-05-18 08:41:02.000000 jcmutils-1.5.3/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.3/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.3/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.3/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:41:29.316414 jcmutils-1.5.3/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-18 08:41:29.000000 jcmutils-1.5.3/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:41:29.316414 jcmutils-1.5.3/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-18 08:40:39.000000 jcmutils-1.5.3/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:47:25.269401 jcmutils-1.5.4/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.4/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:47:25.269401 jcmutils-1.5.4/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.4/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:47:25.269401 jcmutils-1.5.4/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.4/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    11241 2023-05-18 08:47:00.000000 jcmutils-1.5.4/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.4/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.4/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.4/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:47:25.269401 jcmutils-1.5.4/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:47:25.000000 jcmutils-1.5.4/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-18 08:47:25.000000 jcmutils-1.5.4/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-18 08:47:25.000000 jcmutils-1.5.4/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:47:25.000000 jcmutils-1.5.4/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-18 08:47:25.000000 jcmutils-1.5.4/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:47:25.269401 jcmutils-1.5.4/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-18 08:47:05.000000 jcmutils-1.5.4/setup.py
```

### Comparing `jcmutils-1.5.3/LICENSE` & `jcmutils-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.3/README.md` & `jcmutils-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.3/jcmutils/dataset_utils.py` & `jcmutils-1.5.4/jcmutils/dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,16 +170,16 @@
                         (x+w+gap_length,y+h+gap_length),
                         (x-gap_length,y+h+gap_length)]
 
         output_img = template_img
         output_img[y:y+h,x:x+w] = defect_img[y:y+h,x:x+w]
 
         diff_img = diff_img
-        for i in range(x-gap_length,x+w+gap_length):
-            for j in range(y- gap_length,y+h+gap_length):
+        for i in range(x-gap_length,x+w+gap_length - 1):
+            for j in range(y- gap_length,y+h+gap_length - 1):
                 if not (np.abs(i - x - w/2 + 0.5) < w/2 and np.abs(j - y - h/2 +0.5) < h/2):
                     # 计算点到矩形边界的距离
                     distances = []
                     distances2 = []
                     for k in range(4):
                         # 获取当前边的起点和终点
                         p1 = rect_points[k]
```

### Comparing `jcmutils-1.5.3/jcmutils/gen_sources.py` & `jcmutils-1.5.4/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.3/jcmutils/logger.py` & `jcmutils-1.5.4/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.3/jcmutils/solver.py` & `jcmutils-1.5.4/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.3/setup.py` & `jcmutils-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.5.3'
+VERSION = '1.5.4'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

