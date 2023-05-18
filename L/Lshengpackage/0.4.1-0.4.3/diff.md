# Comparing `tmp/Lshengpackage-0.4.1.tar.gz` & `tmp/Lshengpackage-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.4.1.tar", last modified: Thu May 18 05:50:47 2023, max compression
+gzip compressed data, was "Lshengpackage-0.4.3.tar", last modified: Thu May 18 15:12:47 2023, max compression
```

## Comparing `Lshengpackage-0.4.1.tar` & `Lshengpackage-0.4.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.849434 Lshengpackage-0.4.1/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.1/License.md
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.812837 Lshengpackage-0.4.1/Lshengpackage/
--rw-rw-rw-   0        0        0      287 2023-05-18 05:38:59.000000 Lshengpackage-0.4.1/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.820916 Lshengpackage-0.4.1/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.824917 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     3318 2023-05-17 13:41:00.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.825918 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.828918 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/__init__.py
--rw-rw-rw-   0        0        0     7389 2023-05-18 05:50:00.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
--rw-rw-rw-   0        0        0  3646951 2023-05-17 12:12:22.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/image_data.py
--rw-rw-rw-   0        0        0     1601 2023-05-18 05:50:00.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/adb/re_Pic.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.836434 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4669 2023-05-18 05:50:00.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.843434 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/mock_findFr.py
--rw-rw-rw-   0        0        0     2371 2023-05-14 10:04:42.000000 Lshengpackage-0.4.1/Lshengpackage/simulate/mock_findPic.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.849434 Lshengpackage-0.4.1/Lshengpackage/tools/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.1/Lshengpackage/tools/ChaoJiYing.py
--rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.4.1/Lshengpackage/tools/General.py
--rw-rw-rw-   0        0        0     1659 2023-05-18 05:50:00.000000 Lshengpackage-0.4.1/Lshengpackage/tools/Loading.py
--rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.4.1/Lshengpackage/tools/OperateFile.py
--rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.1/Lshengpackage/tools/SearchFile.py
--rw-rw-rw-   0        0        0       49 2023-05-14 09:58:14.000000 Lshengpackage-0.4.1/Lshengpackage/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:50:47.817916 Lshengpackage-0.4.1/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      858 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-18 05:50:47.000000 Lshengpackage-0.4.1/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      299 2023-05-17 15:14:59.000000 Lshengpackage-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2023-05-18 05:50:47.850497 Lshengpackage-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.1/README.md
--rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.4.1/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-18 05:50:47.851503 Lshengpackage-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1987 2023-05-18 05:50:24.000000 Lshengpackage-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.068992 Lshengpackage-0.4.3/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.3/License.md
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.025359 Lshengpackage-0.4.3/Lshengpackage/
+-rw-rw-rw-   0        0        0       51 2023-05-18 15:10:46.000000 Lshengpackage-0.4.3/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.035380 Lshengpackage-0.4.3/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2023-05-18 15:10:46.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.038872 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     3318 2023-05-17 13:41:00.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       49 2023-05-18 15:10:46.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.039878 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.042877 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/dingtalk/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/dingtalk/__init__.py
+-rw-rw-rw-   0        0        0     7591 2023-05-18 15:10:46.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
+-rw-rw-rw-   0        0        0  3646951 2023-05-17 12:12:22.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/dingtalk/image_data.py
+-rw-rw-rw-   0        0        0     1603 2023-05-18 15:10:46.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/adb/re_Pic.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.055986 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4669 2023-05-18 05:50:00.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.060990 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2381 2023-05-18 14:57:22.000000 Lshengpackage-0.4.3/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.068009 Lshengpackage-0.4.3/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.3/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      757 2023-05-18 15:10:46.000000 Lshengpackage-0.4.3/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0     1659 2023-05-18 15:10:46.000000 Lshengpackage-0.4.3/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3311 2023-05-18 14:57:22.000000 Lshengpackage-0.4.3/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.3/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       47 2023-05-18 14:57:22.000000 Lshengpackage-0.4.3/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:12:47.031359 Lshengpackage-0.4.3/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-05-18 15:12:46.000000 Lshengpackage-0.4.3/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-18 15:12:46.000000 Lshengpackage-0.4.3/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:12:46.000000 Lshengpackage-0.4.3/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-18 15:12:46.000000 Lshengpackage-0.4.3/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-18 15:12:46.000000 Lshengpackage-0.4.3/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      299 2023-05-17 15:14:59.000000 Lshengpackage-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2023-05-18 15:12:47.068992 Lshengpackage-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.3/README.md
+-rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.4.3/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-18 15:12:47.069991 Lshengpackage-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1987 2023-05-18 15:11:16.000000 Lshengpackage-0.4.3/setup.py
```

### Comparing `Lshengpackage-0.4.1/LICENSE` & `Lshengpackage-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/License.md` & `Lshengpackage-0.4.3/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/adb/Command_adb.py` & `Lshengpackage-0.4.3/Lshengpackage/simulate/adb/Command_adb.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py` & `Lshengpackage-0.4.3/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: UTF-8 -*-
 import os
-import pickle
 from time import sleep
 
 from simulate.adb.Command_adb import command
 from simulate.adb.re_Pic import refind_image, refiinsclick_image, refiloadclick_image, refiload_image
 
 
 # 检测当前连接状态
@@ -21,14 +20,15 @@
 
 
 # 连接adb
 def connect_api(ip):
     connect = os.system('adb connect {}'.format(ip))
     if connect == 0:
         txt = '连接设备{},成功'.format(ip)
+        # print(txt)
         return txt
 
 
 # 检测dingding当前界面
 def ding_current_api(fol_path, path, _system):
     # Lshengpackage.simulate.adb.Command_adb.command().tap_work(419,953)
     sleep(0.1)
@@ -65,30 +65,30 @@
 # 打开应用接口 #答题 op_answer.png 自查 op_exaself.png
 def open_app_api(fol_path, path, _system, op_name):  # op_name op的名
     xy = refiinsclick_image(fol_path, path, 'is_work', _system)
     if xy is False:
         refiinsclick_image(fol_path, path, 'work', _system)
     else:
         pass
+    refiload_image(fol_path, path, 'op_answer', _system)
     op_answer = refiinsclick_image(fol_path, path, op_name, _system)
+
     if op_answer is False:
         is_work = refind_image(fol_path, path, 'is_work', _system)
         if is_work is not None:
             command().swip_work(int(is_work[0]), int(is_work[1] - 400), int(is_work[0]), int(is_work[1]))
     else:
-        sleep(1)
-        op_answer = refiinsclick_image(fol_path, path, op_name, _system)
         print('{}页已打开,持续更近中'.format(op_name))
         return True
     for i in range(2):
         op_answer = refind_image(fol_path, path, op_name, _system)
-        if op_answer is False:
+        if op_answer is None:
             sleep(0.1)
             is_work = refind_image(fol_path, path, 'is_work', _system)
-            command().swip_work(int(is_work[0]), int(is_work[1] - 100), int(is_work[0]), int(is_work[1] - 500))
+            command().swip_work(int(is_work[0]), int(is_work[1] - 200), int(is_work[0]), int(is_work[1] - 500))
         else:
             op_answer = refiinsclick_image(fol_path, path, op_name, _system)
             print('{}页已打开,持续更近中'.format(op_name))
             return True
 
 
 # 安全答题程序执行程序接口
@@ -120,17 +120,19 @@
     refiloadclick_image(fol_path, path, 'ose', _system)
 
 
 def _upup(fol_path, path, _system, a):
     while True:
 
         sh = refiload_image(fol_path, path, 'shouqi', _system)  # 加载
-
+        print(sh)
         command().swip_work(int(sh[0]), int(sh[1]), int(sh[0]), int(sh[1] - 100))
+
         pu = refind_image(fol_path, path, 'push', _system)  # 加载
+        print(pu)
         if pu is not None:
             return True
         else:
             if a == 5:
                 command().swip_work(int(sh[0]), int(sh[1]), int(sh[0]), int(sh[1] - 500))
                 return True
 
@@ -148,29 +150,39 @@
                              int_y2=1080)
         if yesok is not None:
             return True
 
 
 # 每日安全自查程序接口
 def do_checkself_api(fol_path, path, _system):
+    sleep(0.3)
     refiloadclick_image(fol_path, path, 'city', _system)
+    sleep(0.1)
     refiloadclick_image(fol_path, path, 'jiujiang', _system)
+    sleep(0.1)
     refiloadclick_image(fol_path, path, 'district', _system)
+    sleep(0.1)
     refiloadclick_image(fol_path, path, 'lianxiqu', _system)
+    sleep(0.1)
     att = refiload_image(fol_path, path, 'attribute', _system)
+    sleep(0.1)
     command().tap_work(int(att[0]), int(att[1]))
+    sleep(0.1)
     refiloadclick_image(fol_path, path, 'safeguard', _system)
+    sleep(0.1)
     refiloadclick_image(fol_path, path, 'specialized', _system)
+    sleep(0.1)
     refiloadclick_image(fol_path, path, 'guest', _system)
-
+    sleep(0.1)
     command().swip_work(int(att[0]), int(att[1]), int(att[0]), int(att[1] - 60))
-
+    sleep(0.1)
     te = refiload_image(fol_path, path, 'temp', _system)
+    sleep(0.1)
     command().tap_work(int(te[0]), int(te[1] + 20))
-    sleep(1)
+    sleep(0.5)
     os.popen('adb shell input text 36')  # 输入文本
     while True:
         command().swip_work(int(te[0]), int(te[1]), int(te[0]), int(te[1] - 150))
         for i in range(5):
             ye = refiinsclick_image(fol_path, path, 'yes', _system)
             if ye is False:
                 break
```

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/adb/dingtalk/image_data.py` & `Lshengpackage-0.4.3/Lshengpackage/simulate/adb/dingtalk/image_data.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/adb/re_Pic.py` & `Lshengpackage-0.4.3/Lshengpackage/simulate/adb/re_Pic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*coding:utf-8 -*-
 # !/usr/bin/env python
 import pickle
 from PIL import Image
+
 from simulate.mock_findPic import find_image
-from tools.Loading import load_click, insclick, load
+from tools.Loading import load_click, load, insclick
 
 
 def start_picdata(pypath):
     global image_data
     with open(pypath, 'rb') as f:
         image_data = pickle.load(f)
```

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.4.3/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.4.3/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc` & `Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.4.3/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/simulate/mock_findPic.py` & `Lshengpackage-0.4.3/Lshengpackage/simulate/mock_findPic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from time import sleep
 import os
 import sys
 import cv2
 import pyautogui
-from .adb.Command_adb import command
 from PIL import Image
 
+from simulate.adb.Command_adb import command
+
 
 # 截图
 def screen_shot(fol_path):
     sleep(0.1)
     pyautogui.screenshot(fol_path)
```

### Comparing `Lshengpackage-0.4.1/Lshengpackage/tools/ChaoJiYing.py` & `Lshengpackage-0.4.3/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/tools/General.py` & `Lshengpackage-0.4.3/Lshengpackage/tools/General.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # !/usr/bin/env python
 # -*-coding:utf-8 -*-
 
 
 import time
 import random
-
 import pyautogui
 import pyperclip
 
 
 # 随机数等待时间
 class Delay:
     @classmethod
```

### Comparing `Lshengpackage-0.4.1/Lshengpackage/tools/Loading.py` & `Lshengpackage-0.4.3/Lshengpackage/tools/Loading.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage/tools/OperateFile.py` & `Lshengpackage-0.4.3/Lshengpackage/tools/OperateFile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: UTF-8 -*-
 import os
 from collections import defaultdict
 from openpyxl import Workbook, load_workbook
 import pandas as pd
 
+
 # 删除文件夹下所有文件
 def del_Files(dir_path):
     """
     :param dir_path: 文件夹路径
     :type dir_path:  str
     :return:
     :rtype:
@@ -70,14 +71,15 @@
         # print(path + '/' + f)
         data = pd.DataFrame(pd.read_excel(path + '/' + f_name, sheet_name=sheet_name))  # 读取xls文件
         data.to_excel(os.getcwd() + '/exc/' + file_name_be + '.xlsx', sheet_name=sheet_name, index=False)  # 格式转换
         return file_name_be + '.xlsx'
     else:
         pass
 
+
 def copy_sheet(src_xlsx, ssheetname, dst_xlsx, nsheetname=None):
     if nsheetname == None:
         nsheetname = ssheetname
     try:
         sw = load_workbook(f'{src_xlsx}')
     except KeyError:
         raise KeyError('旧工作簿不存在 The old xlsx is not exists')
@@ -104,8 +106,8 @@
 
     for row in src_sheet.iter_rows():
         # print(row)
         row_list = []
         for cell in row:
             row_list.append(cell.value)
         sheet.append(row_list)
-    dw.save(f'{dst_xlsx}')
+    dw.save(f'{dst_xlsx}')
```

### Comparing `Lshengpackage-0.4.1/Lshengpackage/tools/SearchFile.py` & `Lshengpackage-0.4.3/Lshengpackage/tools/SearchFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.4.3/Lshengpackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.1
+Version: 0.4.3
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.4.1/Lshengpackage.egg-info/SOURCES.txt` & `Lshengpackage-0.4.3/Lshengpackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/PKG-INFO` & `Lshengpackage-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.1
+Version: 0.4.3
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.4.1/README.md` & `Lshengpackage-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.1/setup.py` & `Lshengpackage-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.4.1',  # Start with a small number and increase it with every change you make
+    version='0.4.3',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
     url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
```

