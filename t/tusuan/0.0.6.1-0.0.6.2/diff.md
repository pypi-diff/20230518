# Comparing `tmp/tusuan-0.0.6.1.tar.gz` & `tmp/tusuan-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tusuan-0.0.6.1.tar", last modified: Thu May 18 10:11:10 2023, max compression
+gzip compressed data, was "tusuan-0.0.6.2.tar", last modified: Thu May 18 16:04:22 2023, max compression
```

## Comparing `tusuan-0.0.6.1.tar` & `tusuan-0.0.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.576080 tusuan-0.0.6.1/
--rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.6.1/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-18 10:11:10.575965 tusuan-0.0.6.1/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.6.1/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 10:11:09.000000 tusuan-0.0.6.1/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-05-18 10:11:10.576122 tusuan-0.0.6.1/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1648 2023-05-18 10:10:58.000000 tusuan-0.0.6.1/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.574527 tusuan-0.0.6.1/tusuan/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.6.1/tusuan/__init__.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.575257 tusuan-0.0.6.1/tusuan/datasets/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-05-18 04:55:21.000000 tusuan-0.0.6.1/tusuan/datasets/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     4327 2023-05-18 08:45:26.000000 tusuan-0.0.6.1/tusuan/datasets/imagenet.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.6.1/tusuan/file_function.py
--rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.6.1/tusuan/hello.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.575825 tusuan-0.0.6.1/tusuan/image_video_utils/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.6.1/tusuan/image_video_utils/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2137 2023-05-08 05:08:27.000000 tusuan-0.0.6.1/tusuan/image_video_utils/croppers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1163 2023-05-07 17:43:48.000000 tusuan-0.0.6.1/tusuan/image_video_utils/display.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.6.1/tusuan/image_video_utils/image_visual_selector.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     4013 2023-05-08 05:14:00.000000 tusuan-0.0.6.1/tusuan/image_video_utils/readers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2583 2023-05-08 18:11:39.000000 tusuan-0.0.6.1/tusuan/image_video_utils/writers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.6.1/tusuan/path_utils.py
--rw-r--r--   0 xiangyang   (501) staff       (20)       97 2023-05-14 11:47:37.000000 tusuan-0.0.6.1/tusuan/time_utils.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 10:11:10.575071 tusuan-0.0.6.1/tusuan.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      585 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-05-18 10:11:10.000000 tusuan-0.0.6.1/tusuan.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.363945 tusuan-0.0.6.2/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.6.2/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-18 16:04:22.363806 tusuan-0.0.6.2/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.6.2/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 10:11:09.000000 tusuan-0.0.6.2/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-05-18 16:04:22.363995 tusuan-0.0.6.2/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1648 2023-05-18 16:03:36.000000 tusuan-0.0.6.2/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.360928 tusuan-0.0.6.2/tusuan/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.6.2/tusuan/__init__.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.361884 tusuan-0.0.6.2/tusuan/datasets/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-05-18 04:55:21.000000 tusuan-0.0.6.2/tusuan/datasets/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     4332 2023-05-18 16:03:26.000000 tusuan-0.0.6.2/tusuan/datasets/imagenet.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.6.2/tusuan/file_function.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.6.2/tusuan/hello.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.363413 tusuan-0.0.6.2/tusuan/image_video_utils/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.6.2/tusuan/image_video_utils/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2137 2023-05-08 05:08:27.000000 tusuan-0.0.6.2/tusuan/image_video_utils/croppers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1163 2023-05-07 17:43:48.000000 tusuan-0.0.6.2/tusuan/image_video_utils/display.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.6.2/tusuan/image_video_utils/image_visual_selector.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     4013 2023-05-08 05:14:00.000000 tusuan-0.0.6.2/tusuan/image_video_utils/readers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2583 2023-05-08 18:11:39.000000 tusuan-0.0.6.2/tusuan/image_video_utils/writers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.6.2/tusuan/path_utils.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       97 2023-05-14 11:47:37.000000 tusuan-0.0.6.2/tusuan/time_utils.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-05-18 16:04:22.361633 tusuan-0.0.6.2/tusuan.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      585 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       90 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-05-18 16:04:22.000000 tusuan-0.0.6.2/tusuan.egg-info/top_level.txt
```

### Comparing `tusuan-0.0.6.1/PKG-INFO` & `tusuan-0.0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

### Comparing `tusuan-0.0.6.1/setup.py` & `tusuan-0.0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from read import read
 from setuptools import setup, find_packages
 
 setup(name='tusuan',  # 包名
       python_requires='>=3.8.0',  # python环境
-      version='0.0.6.1',  # 包的版本
+      version='0.0.6.2',  # 包的版本
       description="useful functions.",  # 包简介，显示在PyPI上
 
       long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
       long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
       author="tusuan",  # 作者相关信息
       author_email='btk@qq.com',
```

### Comparing `tusuan-0.0.6.1/tusuan/datasets/imagenet.py` & `tusuan-0.0.6.2/tusuan/datasets/imagenet.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,25 @@
         obj = pickle.load(fo)
     return obj
 
 
 def load_databatch(data_file, img_size=64):
     # data_file = os.path.join(data_folder, f'train_data_batch_{str(idn)}')
     d = unpickle(data_file)
-    x = numpy.array(d['data'], dtype="uint8")
+    x = numpy.array(d['data'], dtype="float32")
     y = numpy.array(d['labels'], dtype="int32")
-    mean = numpy.array(d['mean'])
+    # mean = numpy.array(d['mean'])
 
     # Labels are indexed from 1, shift it so that indexes start at 0
     y = y - 1
 
-    x = einops.rearrange(x, "b (c h w) -> b h w c", h=img_size, w=img_size)
-    mean = einops.rearrange(mean, "(c h w) -> h w c", h=img_size, w=img_size)
+    x = einops.rearrange(x, "b (c h w) -> b c h w", h=img_size, w=img_size)
+    # mean = einops.rearrange(mean, "(c h w) -> h w c", h=img_size, w=img_size)
 
-    return dict(x=x, y=y, mean=mean)
+    return dict(x=x, y=y)
 
 
 class ImageNet64(dataset.Dataset):
     BLOCK_CACHE_SIZE = 2
     DATA_CACHE_SIZE = 100_000
 
     def __init__(self, root, train=True):
@@ -67,31 +67,32 @@
             # print(self.index_block_map)
             self.data_length = sum(each_block_length)
 
             self.get_data = self.get_data_train
         else:
             if len(glob.glob(join(root, "val_data"))) != 1:
                 raise FileNotFoundError(f"val_data file not exists.")
-            self.data_list = load_databatch(join(root, "train_data_batch_*"))
-            self.data_length = len(self.data_list)
+            self.data_list = load_databatch(join(root, "val_data"))
+            self.data_length = len(self.data_list["y"])
 
             self.get_data = self.get_data_val
 
     @lru_cache(BLOCK_CACHE_SIZE)
     def get_data_block(self, block_idn):
+        # print(block_idn)
         return load_databatch(data_file=join(self.root, f'train_data_batch_{str(block_idn)}'))
 
     @lru_cache(DATA_CACHE_SIZE)
     def get_data_train(self, index):
         if index >= self.data_length or index < 0:
             raise IndexError(f"index {index} out of bounds for size [0, {self.data_length})")
 
         count_previous_blocks_length = 0
         for map_block_idn, map_interval in self.index_block_map:
-            print(map_block_idn)
+            # print(map_block_idn)
             if map_interval[0] <= index < map_interval[1]:
                 block_idn = map_block_idn
                 break
             else:
                 count_previous_blocks_length = map_interval[1]
         else:
             raise ValueError(f"没有找到{index}")
@@ -105,10 +106,7 @@
         return self.data_list["x"][index], self.data_list["y"][index]
 
     def __getitem__(self, index) -> Tuple[numpy.ndarray, int]:
         return self.get_data(index)
 
     def __len__(self):
         return self.data_length
-
-
-ImageNet64()
```

### Comparing `tusuan-0.0.6.1/tusuan/file_function.py` & `tusuan-0.0.6.2/tusuan/file_function.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.1/tusuan/image_video_utils/croppers.py` & `tusuan-0.0.6.2/tusuan/image_video_utils/croppers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.1/tusuan/image_video_utils/display.py` & `tusuan-0.0.6.2/tusuan/image_video_utils/display.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.1/tusuan/image_video_utils/image_visual_selector.py` & `tusuan-0.0.6.2/tusuan/image_video_utils/image_visual_selector.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.1/tusuan/image_video_utils/readers.py` & `tusuan-0.0.6.2/tusuan/image_video_utils/readers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.1/tusuan/image_video_utils/writers.py` & `tusuan-0.0.6.2/tusuan/image_video_utils/writers.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.6.1/tusuan.egg-info/PKG-INFO` & `tusuan-0.0.6.2/tusuan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

### Comparing `tusuan-0.0.6.1/tusuan.egg-info/SOURCES.txt` & `tusuan-0.0.6.2/tusuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

