# Comparing `tmp/Lshengpackage-0.4.0.tar.gz` & `tmp/Lshengpackage-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.4.0.tar", last modified: Thu May 18 01:39:53 2023, max compression
+gzip compressed data, was "Lshengpackage-0.4.1.tar", last modified: Thu May 18 05:50:47 2023, max compression
```

## Comparing `Lshengpackage-0.4.0.tar` & `Lshengpackage-0.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.066005 Lshengpackage-0.4.0/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.0/License.md
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.018124 Lshengpackage-0.4.0/Lshengpackage/
--rw-rw-rw-   0        0        0      719 2023-05-17 13:46:03.000000 Lshengpackage-0.4.0/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.029637 Lshengpackage-0.4.0/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.032637 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     3318 2023-05-17 13:41:00.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.034637 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.038930 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/dingtalk/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/dingtalk/__init__.py
--rw-rw-rw-   0        0        0     8928 2023-05-18 01:38:58.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
--rw-rw-rw-   0        0        0  3646951 2023-05-17 12:12:22.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/dingtalk/image_data.py
--rw-rw-rw-   0        0        0     1629 2023-05-17 13:41:00.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/adb/re_Pic.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.053999 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.059040 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/mock_findFr.py
--rw-rw-rw-   0        0        0     2371 2023-05-14 10:04:42.000000 Lshengpackage-0.4.0/Lshengpackage/simulate/mock_findPic.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.065005 Lshengpackage-0.4.0/Lshengpackage/tools/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.0/Lshengpackage/tools/ChaoJiYing.py
--rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.4.0/Lshengpackage/tools/General.py
--rw-rw-rw-   0        0        0     1724 2023-05-17 12:59:31.000000 Lshengpackage-0.4.0/Lshengpackage/tools/Loading.py
--rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.4.0/Lshengpackage/tools/OperateFile.py
--rw-rw-rw-   0        0        0     2059 2023-05-14 04:52:50.000000 Lshengpackage-0.4.0/Lshengpackage/tools/SearchFile.py
--rw-rw-rw-   0        0        0       49 2023-05-14 09:58:14.000000 Lshengpackage-0.4.0/Lshengpackage/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:39:53.025637 Lshengpackage-0.4.0/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      858 2023-05-18 01:39:52.000000 Lshengpackage-0.4.0/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-18 01:39:52.000000 Lshengpackage-0.4.0/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:39:52.000000 Lshengpackage-0.4.0/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-18 01:39:52.000000 Lshengpackage-0.4.0/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-18 01:39:52.000000 Lshengpackage-0.4.0/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      299 2023-05-17 15:14:59.000000 Lshengpackage-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2023-05-18 01:39:53.067051 Lshengpackage-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.0/README.md
--rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-18 01:39:53.068005 Lshengpackage-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1987 2023-05-17 15:15:20.000000 Lshengpackage-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.849434 Lshengpackage-0.4.1/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.1/License.md
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.812837 Lshengpackage-0.4.1/Lshengpackage/
+-rw-rw-rw-   0        0        0      287 2023-05-18 05:38:59.000000 Lshengpackage-0.4.1/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.820916 Lshengpackage-0.4.1/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.824917 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     3318 2023-05-17 13:41:00.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.825918 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.828918 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/__init__.py
+-rw-rw-rw-   0        0        0     7389 2023-05-18 05:50:00.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
+-rw-rw-rw-   0        0        0  3646951 2023-05-17 12:12:22.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/image_data.py
+-rw-rw-rw-   0        0        0     1601 2023-05-18 05:50:00.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/re_Pic.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.836434 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4669 2023-05-18 05:50:00.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.843434 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2371 2023-05-14 10:04:42.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.849434 Lshengpackage-0.4.1/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.1/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.4.1/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0     1659 2023-05-18 05:50:00.000000 Lshengpackage-0.4.1/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.4.1/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.1/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       49 2023-05-14 09:58:14.000000 Lshengpackage-0.4.1/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.817916 Lshengpackage-0.4.1/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      299 2023-05-17 15:14:59.000000 Lshengpackage-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2023-05-18 05:50:47.850497 Lshengpackage-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.1/README.md
+-rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-18 05:50:47.851503 Lshengpackage-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1987 2023-05-18 05:50:24.000000 Lshengpackage-0.4.1/setup.py
```

### Comparing `Lshengpackage-0.4.0/LICENSE` & `Lshengpackage-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/License.md` & `Lshengpackage-0.4.1/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/adb/Command_adb.py` & `Lshengpackage-0.4.1/Lshengpackage/simulate/adb/Command_adb.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py` & `Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,14 @@
 # -*- coding: UTF-8 -*-
 import os
 import pickle
 from time import sleep
 
-from Lshengpackage.simulate.adb.Command_adb import command
-from Lshengpackage.simulate.mock_findPic import find_image
-from Lshengpackage.tools.Loading import load_click, load, insclick
-from PIL import Image
-
-
-def start_picdata(pypath):
-    global image_data
-    with open(pypath, 'rb') as f:
-        image_data = pickle.load(f)
-
-
-def read_img(path, img_name):
-    # 读取py的图片并缓存为临时文件
-    img_data = image_data[img_name][0]
-    img = Image.new(mode='RGB', size=(img_data['width'], img_data['height']))
-    img.putdata(img_data['pixel_values'])
-    img.save(path + 'public.png')
-
-
-def refind_image(fol_path, path, img_name, _system=None, int_x1=-1, int_y1=None, int_x2=None, int_y2=None):
-    read_img(path, img_name)
-    pub = find_image(fol_path, path + 'public.png', _system, int_x1, int_y1, int_x2, int_y2)
-    if pub is not None:
-        return pub
-
-
-def refiloadclick_image(fol_path, path, img_name, _system):
-    read_img(path, img_name)
-    pub = load_click(fol_path, path + 'public.png', _system)  # 退出当前页再找
-    if pub is True:
-        return True
-    else:
-        return False
-
-
-def refiload_image(fol_path, path, img_name, _system):
-    read_img(path, img_name)
-    pub = load(fol_path, path + 'public.png', _system)  # 退出当前页再找
-    if pub is not None:
-        return pub
-
-
-def refiinsclick_image(fol_path, path, img_name, _system):
-    read_img(path, img_name)
-    pub = insclick(fol_path, path + 'public.png', _system)  # 退出当前页再找
-    if pub is True:
-        return True
-    else:
-        return False
+from simulate.adb.Command_adb import command
+from simulate.adb.re_Pic import refind_image, refiinsclick_image, refiloadclick_image, refiload_image
 
 
 # 检测当前连接状态
 def connect_status_api():
     state = os.popen('adb get-state').read()  # ddddddddddd
     if state[0:7] == 'unknown':
         print('未检测到连接设备')
@@ -69,15 +21,14 @@
 
 
 # 连接adb
 def connect_api(ip):
     connect = os.system('adb connect {}'.format(ip))
     if connect == 0:
         txt = '连接设备{},成功'.format(ip)
-        # print(txt)
         return txt
 
 
 # 检测dingding当前界面
 def ding_current_api(fol_path, path, _system):
     # Lshengpackage.simulate.adb.Command_adb.command().tap_work(419,953)
     sleep(0.1)
@@ -169,19 +120,17 @@
     refiloadclick_image(fol_path, path, 'ose', _system)
 
 
 def _upup(fol_path, path, _system, a):
     while True:
 
         sh = refiload_image(fol_path, path, 'shouqi', _system)  # 加载
-        print(sh)
-        command().swip_work(int(sh[0]), int(sh[1]), int(sh[0]), int(sh[1] - 100))
 
+        command().swip_work(int(sh[0]), int(sh[1]), int(sh[0]), int(sh[1] - 100))
         pu = refind_image(fol_path, path, 'push', _system)  # 加载
-        print(pu)
         if pu is not None:
             return True
         else:
             if a == 5:
                 command().swip_work(int(sh[0]), int(sh[1]), int(sh[0]), int(sh[1] - 500))
                 return True
```

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/adb/dingtalk/image_data.py` & `Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/image_data.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/adb/re_Pic.py` & `Lshengpackage-0.4.1/Lshengpackage/simulate/adb/re_Pic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*coding:utf-8 -*-
 # !/usr/bin/env python
 import pickle
-from Lshengpackage.tools.Loading import load_click, load, insclick
-from Lshengpackage.simulate.mock_findPic import find_image
 from PIL import Image
+from simulate.mock_findPic import find_image
+from tools.Loading import load_click, insclick, load
 
 
 def start_picdata(pypath):
     global image_data
     with open(pypath, 'rb') as f:
         image_data = pickle.load(f)
```

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: UTF-8 -*-
-
-from Lshengpackage.Delay import Delay
+from tools.General import Delay
 
 
 class mouse:
     def __init__(self, dm_obj, start_time=0.3, end_time=0.7):
         self.__dm_obj = dm_obj
         self.start_time = start_time
         self.end_time = end_time
```

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc` & `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/simulate/mock_findPic.py` & `Lshengpackage-0.4.1/Lshengpackage/simulate/mock_findPic.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/tools/ChaoJiYing.py` & `Lshengpackage-0.4.1/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/tools/General.py` & `Lshengpackage-0.4.1/Lshengpackage/tools/General.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/tools/Loading.py` & `Lshengpackage-0.4.1/Lshengpackage/tools/Loading.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 # !/usr/bin/env python
 # -*- coding: UTF-8 -*-
 import os
 import sys
 import pyautogui
 from time import sleep
-from Lshengpackage.simulate.adb.Command_adb import command
-from Lshengpackage.simulate.mock_findPic import find_image
-from Lshengpackage.simulate.adb import Command_adb
+
+from simulate.adb.Command_adb import command
+from simulate.mock_findPic import find_image
+
+
 # 加载
-def load(fol_path, target_path,_system):
+def load(fol_path, target_path, _system):
     """
         :param img: 循环等待的值
         :type img: img
         :return: 鼠标(1,1),返回 'N'
         :rtype:
         """
     while True:
         sleep(0.1)
-        iocn = find_image(fol_path, target_path,_system)
+        iocn = find_image(fol_path, target_path, _system)
         if iocn is not None:
             sleep(0.1)
             return iocn
         x, y = pyautogui.position()
         if x & y == 0:
             sys.exit()
             # 暂时先这样结束进程
         else:
             pass
 
 
-def load_click(fol_path, target_path,_system):
+def load_click(fol_path, target_path, _system):
     """
     加载点击
     """
     sleep(0.1)
-    iocn = load(fol_path, target_path,_system)
+    iocn = load(fol_path, target_path, _system)
     print(iocn)
     if iocn is not None:
         if _system == 'adb':
             sleep(0.1)
             command().tap_work(int(iocn[0]), int(iocn[1]))
         else:
             sleep(0.1)
             pyautogui.click(int(iocn[0]), int(iocn[1]))
             return True
     else:
         return False
 
-def insclick(fol_path, target_path,_system):
+
+def insclick(fol_path, target_path, _system):
     """
     加载点击
     """
     sleep(0.1)
     iocn = find_image(fol_path, target_path, _system)
     if iocn is not None:
         sleep(0.1)
         if _system == 'adb':
             command().tap_work(int(iocn[0]), int(iocn[1]))
             return True
         else:
             pyautogui.click(int(iocn[0]), int(iocn[1]))
             return True
     else:
-        return False
+        return False
```

### Comparing `Lshengpackage-0.4.0/Lshengpackage/tools/OperateFile.py` & `Lshengpackage-0.4.1/Lshengpackage/tools/OperateFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/Lshengpackage/tools/SearchFile.py` & `Lshengpackage-0.4.1/Lshengpackage/tools/SearchFile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: UTF-8 -*-
 
 # 检索目录下文件
 import os
-
 import pandas as pd
-
 global road
 
 
 # 找文件
 def search_it(paths, filename):
     
     global road  # 表明这里的road是全局变量road
```

### Comparing `Lshengpackage-0.4.0/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.4.1/Lshengpackage.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.0
+Version: 0.4.1
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.4.0/Lshengpackage.egg-info/SOURCES.txt` & `Lshengpackage-0.4.1/Lshengpackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/PKG-INFO` & `Lshengpackage-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.0
+Version: 0.4.1
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.4.0/README.md` & `Lshengpackage-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.0/setup.py` & `Lshengpackage-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.4.0',  # Start with a small number and increase it with every change you make
+    version='0.4.1',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
     url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
```

