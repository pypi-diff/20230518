# Comparing `tmp/avcv-0.0.6.tar.gz` & `tmp/avcv-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/avcv-0.0.6.tar", last modified: Thu Jul 29 18:15:50 2021, max compression
+gzip compressed data, was "avcv-0.0.7.tar", last modified: Sat Aug  7 05:47:32 2021, max compression
```

## Comparing `avcv-0.0.6.tar` & `avcv-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bi         (502) staff       (20)        0 2021-07-29 18:15:50.059057 avcv-0.0.6/
--rw-r--r--   0 bi         (502) staff       (20)     2348 2021-07-17 13:18:46.000000 avcv-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 bi         (502) staff       (20)    11357 2021-07-17 13:18:46.000000 avcv-0.0.6/LICENSE
--rw-r--r--   0 bi         (502) staff       (20)      111 2021-07-17 13:18:46.000000 avcv-0.0.6/MANIFEST.in
--rw-r--r--   0 bi         (502) staff       (20)      912 2021-07-29 18:15:50.058794 avcv-0.0.6/PKG-INFO
--rw-r--r--   0 bi         (502) staff       (20)      130 2021-07-29 18:15:29.000000 avcv-0.0.6/README.md
-drwxr-xr-x   0 bi         (502) staff       (20)        0 2021-07-29 18:15:50.056355 avcv-0.0.6/avcv/
--rw-r--r--   0 bi         (502) staff       (20)       22 2021-07-29 18:15:23.000000 avcv-0.0.6/avcv/__init__.py
--rw-r--r--   0 bi         (502) staff       (20)      878 2021-07-29 18:15:23.000000 avcv-0.0.6/avcv/_nbdev.py
--rw-r--r--   0 bi         (502) staff       (20)     1855 2021-07-29 18:15:23.000000 avcv-0.0.6/avcv/debug.py
--rw-r--r--   0 bi         (502) staff       (20)     1209 2021-07-29 18:15:23.000000 avcv-0.0.6/avcv/process.py
--rw-r--r--   0 bi         (502) staff       (20)     5514 2021-07-29 18:15:23.000000 avcv-0.0.6/avcv/utils.py
--rw-r--r--   0 bi         (502) staff       (20)     4430 2021-07-29 18:15:23.000000 avcv-0.0.6/avcv/visualize.py
-drwxr-xr-x   0 bi         (502) staff       (20)        0 2021-07-29 18:15:50.058432 avcv-0.0.6/avcv.egg-info/
--rw-r--r--   0 bi         (502) staff       (20)      912 2021-07-29 18:15:49.000000 avcv-0.0.6/avcv.egg-info/PKG-INFO
--rw-r--r--   0 bi         (502) staff       (20)      358 2021-07-29 18:15:49.000000 avcv-0.0.6/avcv.egg-info/SOURCES.txt
--rw-r--r--   0 bi         (502) staff       (20)        1 2021-07-29 18:15:49.000000 avcv-0.0.6/avcv.egg-info/dependency_links.txt
--rw-r--r--   0 bi         (502) staff       (20)      190 2021-07-29 18:15:49.000000 avcv-0.0.6/avcv.egg-info/entry_points.txt
--rw-r--r--   0 bi         (502) staff       (20)        1 2021-07-17 13:46:30.000000 avcv-0.0.6/avcv.egg-info/not-zip-safe
--rw-r--r--   0 bi         (502) staff       (20)       88 2021-07-29 18:15:49.000000 avcv-0.0.6/avcv.egg-info/requires.txt
--rw-r--r--   0 bi         (502) staff       (20)        5 2021-07-29 18:15:49.000000 avcv-0.0.6/avcv.egg-info/top_level.txt
--rw-r--r--   0 bi         (502) staff       (20)      853 2021-07-29 18:13:27.000000 avcv-0.0.6/settings.ini
--rw-r--r--   0 bi         (502) staff       (20)       38 2021-07-29 18:15:50.059136 avcv-0.0.6/setup.cfg
--rw-r--r--   0 bi         (502) staff       (20)     2300 2021-07-17 13:18:46.000000 avcv-0.0.6/setup.py
+drwxrwxr-x   0 av        (1002) av        (1002)        0 2021-08-07 05:47:32.672964 avcv-0.0.7/
+-rw-rw-r--   0 av        (1002) av        (1002)     2348 2021-08-07 05:39:31.000000 avcv-0.0.7/CONTRIBUTING.md
+-rw-rw-r--   0 av        (1002) av        (1002)    11357 2021-08-07 05:39:31.000000 avcv-0.0.7/LICENSE
+-rw-rw-r--   0 av        (1002) av        (1002)      111 2021-08-07 05:39:31.000000 avcv-0.0.7/MANIFEST.in
+-rw-rw-r--   0 av        (1002) av        (1002)      912 2021-08-07 05:47:32.672964 avcv-0.0.7/PKG-INFO
+-rw-rw-r--   0 av        (1002) av        (1002)      130 2021-08-07 05:39:31.000000 avcv-0.0.7/README.md
+drwxrwxr-x   0 av        (1002) av        (1002)        0 2021-08-07 05:47:32.668964 avcv-0.0.7/avcv/
+-rw-rw-r--   0 av        (1002) av        (1002)       22 2021-08-07 05:47:01.000000 avcv-0.0.7/avcv/__init__.py
+-rw-rw-r--   0 av        (1002) av        (1002)      962 2021-08-07 05:47:01.000000 avcv-0.0.7/avcv/_nbdev.py
+-rw-rw-r--   0 av        (1002) av        (1002)     2974 2021-08-07 05:47:01.000000 avcv-0.0.7/avcv/debug.py
+-rw-rw-r--   0 av        (1002) av        (1002)     1209 2021-08-07 05:47:01.000000 avcv-0.0.7/avcv/process.py
+-rw-rw-r--   0 av        (1002) av        (1002)     5514 2021-08-07 05:47:01.000000 avcv-0.0.7/avcv/utils.py
+-rw-rw-r--   0 av        (1002) av        (1002)     2969 2021-08-07 05:47:01.000000 avcv-0.0.7/avcv/visualize.py
+drwxrwxr-x   0 av        (1002) av        (1002)        0 2021-08-07 05:47:32.672964 avcv-0.0.7/avcv.egg-info/
+-rw-rw-r--   0 av        (1002) av        (1002)      912 2021-08-07 05:47:32.000000 avcv-0.0.7/avcv.egg-info/PKG-INFO
+-rw-rw-r--   0 av        (1002) av        (1002)      358 2021-08-07 05:47:32.000000 avcv-0.0.7/avcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 av        (1002) av        (1002)        1 2021-08-07 05:47:32.000000 avcv-0.0.7/avcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 av        (1002) av        (1002)      231 2021-08-07 05:47:32.000000 avcv-0.0.7/avcv.egg-info/entry_points.txt
+-rw-rw-r--   0 av        (1002) av        (1002)        1 2021-08-07 05:41:54.000000 avcv-0.0.7/avcv.egg-info/not-zip-safe
+-rw-rw-r--   0 av        (1002) av        (1002)       97 2021-08-07 05:47:32.000000 avcv-0.0.7/avcv.egg-info/requires.txt
+-rw-rw-r--   0 av        (1002) av        (1002)        5 2021-08-07 05:47:32.000000 avcv-0.0.7/avcv.egg-info/top_level.txt
+-rw-rw-r--   0 av        (1002) av        (1002)      902 2021-08-07 05:39:31.000000 avcv-0.0.7/settings.ini
+-rw-rw-r--   0 av        (1002) av        (1002)       38 2021-08-07 05:47:32.672964 avcv-0.0.7/setup.cfg
+-rw-rw-r--   0 av        (1002) av        (1002)     2300 2021-08-07 05:39:31.000000 avcv-0.0.7/setup.py
```

### Comparing `avcv-0.0.6/CONTRIBUTING.md` & `avcv-0.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `avcv-0.0.6/LICENSE` & `avcv-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `avcv-0.0.6/PKG-INFO` & `avcv-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avcv
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package utils for computer vision
 Home-page: https://github.com/anhvth/avcv/tree/nbdev-convert/
 Author: Hai Anh
 Author-email: anhvth.226@gmail.com
 License: Apache Software License 2.0
 Description: # AVCV
         > Optimized functions for vision problems
```

### Comparing `avcv-0.0.6/avcv/_nbdev.py` & `avcv-0.0.7/avcv/_nbdev.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # AUTOGENERATED BY NBDEV! DO NOT EDIT!
 
 __all__ = ["index", "modules", "custom_doc_links", "git_url"]
 
 index = {"plot_images": "00_visualize.ipynb",
          "show": "00_visualize.ipynb",
+         "tensor2imgs": "00_visualize.ipynb",
          "multi_thread": "01_process.ipynb",
          "get_name": "03_utils.ipynb",
          "find_contours": "03_utils.ipynb",
          "download_file_from_google_drive": "03_utils.ipynb",
          "mkdir": "03_utils.ipynb",
          "put_text": "03_utils.ipynb",
          "images_to_video": "03_utils.ipynb",
          "get_paths": "03_utils.ipynb",
          "video_to_images": "03_utils.ipynb",
-         "make_mini_coco": "04_debug.ipynb"}
+         "make_mini_coco": "04_debug.ipynb",
+         "dpython": "04_debug.ipynb"}
 
 modules = ["visualize.py",
            "process.py",
            "utils.py",
            "debug.py"]
 
 doc_url = "https://anhvth.github.io/avcv/"
```

### Comparing `avcv-0.0.6/avcv/debug.py` & `avcv-0.0.7/avcv/debug.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/04_debug.ipynb (unless otherwise specified).
 
-__all__ = ['make_mini_coco']
+__all__ = ['make_mini_coco', 'dpython']
 
 # Cell
 import os
 import os.path as osp
 import matplotlib.pyplot as plt
 import numpy as np
 import mmcv
@@ -21,22 +21,22 @@
         Helper function for creating a mini-dataset ensembles it's father
     """
     from pycocotools.coco import COCO
     new_img_prefix = osp.join(out_dir, "images")
 
     out_json = os.path.join(out_dir, "annotations", "mini_json.json")
     if not osp.exists(out_json):
-        print("Making mini dataset", out_dir, "num images:", n)
+        print("Making mini dataset", out_dir, "num images:", num_samples)
         os.makedirs(os.path.join(out_dir, "images"), exist_ok=True)
         os.makedirs(os.path.join(out_dir, "annotations"), exist_ok=True)
         coco = COCO(json_path)
         # imgs = coco.imgs
         img_ids = list(coco.imgs.keys())
         np.random.seed(0)
-        selected_img_ids = np.random.choice(img_ids, n, replace=False)
+        selected_img_ids = np.random.choice(img_ids, num_samples, replace=False)
         imgs = coco.loadImgs(selected_img_ids)
         selected_ann_ids = coco.getAnnIds(selected_img_ids)
         anns = coco.loadAnns(selected_ann_ids)
         for i, ann in enumerate(anns):
             ann['iscrowd'] = False
             anns[i] = ann
         out_dict = dict(
@@ -49,7 +49,49 @@
             path = osp.join(image_prefix, img['file_name'])
             new_path = osp.join(new_img_prefix, img['file_name'])
             shutil.copy(path, new_path)
 
         mmcv.dump(out_dict, out_json)
     print(out_json, new_img_prefix)
     return out_json, new_img_prefix
+
+
+# Cell
+@call_parse
+def dpython(cmd: Param(type=str)):
+    for _ in range(3):
+        cmd = cmd.replace('  ', '')
+    i_split = cmd.index(".py")+4
+    file = cmd[:i_split].strip().split(' ')[1]
+
+    args = cmd[i_split:].split(' ')
+    cfg_name = os.environ.get("DNAME", "Latest-Generated")
+    cfg = {
+        "name": f"Python: {cfg_name}",
+        "type": "python",
+        "request": "launch",
+        "program": f"{file}",
+        "console": "integratedTerminal",
+        "args": args,
+    }
+    # pp(cfg)
+    mmcv.mkdir_or_exist(".vscode")
+    try:
+        lauch = read_json(".vscode/launch.json")
+    except:
+        lauch = {
+            "version": "0.2.0",
+            "configurations": [
+
+            ]
+        }
+    replace = False
+    for i, _cfg in enumerate(lauch['configurations']):
+        if _cfg["name"] == cfg["name"]:
+            lauch["configurations"][i] = cfg
+            replace = True
+    if not replace:
+        lauch["configurations"] += [cfg]
+#     with open(, 'w') as f:
+#         mmcv.dump(lauch, f, indent=4)
+        mmcv.dump(lauch, '.vscode/launch.json')
+
```

### Comparing `avcv-0.0.6/avcv/process.py` & `avcv-0.0.7/avcv/process.py`

 * *Files identical despite different names*

### Comparing `avcv-0.0.6/avcv/utils.py` & `avcv-0.0.7/avcv/utils.py`

 * *Files identical despite different names*

### Comparing `avcv-0.0.6/avcv.egg-info/PKG-INFO` & `avcv-0.0.7/avcv.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avcv
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package utils for computer vision
 Home-page: https://github.com/anhvth/avcv/tree/nbdev-convert/
 Author: Hai Anh
 Author-email: anhvth.226@gmail.com
 License: Apache Software License 2.0
 Description: # AVCV
         > Optimized functions for vision problems
```

### Comparing `avcv-0.0.6/setup.py` & `avcv-0.0.7/setup.py`

 * *Files identical despite different names*

