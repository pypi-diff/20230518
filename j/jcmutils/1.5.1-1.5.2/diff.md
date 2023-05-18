# Comparing `tmp/jcmutils-1.5.1.tar.gz` & `tmp/jcmutils-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.5.1.tar", last modified: Thu May 18 07:54:50 2023, max compression
+gzip compressed data, was "jcmutils-1.5.2.tar", last modified: Thu May 18 08:26:49 2023, max compression
```

## Comparing `jcmutils-1.5.1.tar` & `jcmutils-1.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 07:54:50.941615 jcmutils-1.5.1/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.1/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 07:54:50.941615 jcmutils-1.5.1/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.1/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 07:54:50.941615 jcmutils-1.5.1/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.1/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    11234 2023-05-18 07:54:19.000000 jcmutils-1.5.1/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.1/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.1/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.1/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 07:54:50.941615 jcmutils-1.5.1/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 07:54:50.000000 jcmutils-1.5.1/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-18 07:54:50.000000 jcmutils-1.5.1/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-18 07:54:50.000000 jcmutils-1.5.1/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 07:54:50.000000 jcmutils-1.5.1/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-18 07:54:50.000000 jcmutils-1.5.1/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 07:54:50.941615 jcmutils-1.5.1/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-18 07:54:28.000000 jcmutils-1.5.1/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:26:49.785235 jcmutils-1.5.2/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.5.2/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:26:49.785235 jcmutils-1.5.2/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.5.2/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:26:49.785235 jcmutils-1.5.2/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.5.2/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    11234 2023-05-18 08:26:27.000000 jcmutils-1.5.2/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.5.2/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.5.2/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.5.2/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-18 08:26:49.785235 jcmutils-1.5.2/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-18 08:26:49.000000 jcmutils-1.5.2/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-18 08:26:49.785235 jcmutils-1.5.2/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-18 08:26:36.000000 jcmutils-1.5.2/setup.py
```

### Comparing `jcmutils-1.5.1/LICENSE` & `jcmutils-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.1/README.md` & `jcmutils-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.1/jcmutils/dataset_utils.py` & `jcmutils-1.5.2/jcmutils/dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                     min_distance = min(distances)
                     min_distance2 = min(distances2)
                     # output_img[j,i] = 255
                     output_img[j,i] += diff_img[j,i]* (min_distance2)/(min_distance + min_distance2)
         xpos = (x + w/2)/image_shape[1]
         ypos = (y + h/2)/image_shape[0]
         width = w/image_shape[1]
-        height = y/image_shape[1]
+        height = h/image_shape[1]
         return (output_img,(xpos,ypos,width,height))
 
     # def export_database_old(self, num_of_result, source_density, target_density,target_filename, vmax, is_light_intense=True, is_symmetry=False):
     #     # 开始提取
     #     # 先确定total_result的形状
     #     temp_result = self.resultbag.get_result(self.keys[0])
     #     field = (temp_result[num_of_result]['field'][0].conj() *
```

### Comparing `jcmutils-1.5.1/jcmutils/gen_sources.py` & `jcmutils-1.5.2/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.1/jcmutils/logger.py` & `jcmutils-1.5.2/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.1/jcmutils/solver.py` & `jcmutils-1.5.2/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.5.1/setup.py` & `jcmutils-1.5.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.5.1'
+VERSION = '1.5.2'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

