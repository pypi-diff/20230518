# Comparing `tmp/VSautomatic-2.1.tar.gz` & `tmp/VSautomatic-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VSautomatic-2.1.tar", last modified: Tue May 16 06:12:00 2023, max compression
+gzip compressed data, was "VSautomatic-2.2.tar", last modified: Thu May 18 01:37:53 2023, max compression
```

## Comparing `VSautomatic-2.1.tar` & `VSautomatic-2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 06:12:00.573331 VSautomatic-2.1/
--rw-rw-rw-   0        0        0      259 2023-05-16 06:12:00.573331 VSautomatic-2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 06:12:00.563331 VSautomatic-2.1/VSautomatic/
--rw-rw-rw-   0        0        0       10 2023-05-15 06:47:27.000000 VSautomatic-2.1/VSautomatic/Auth_Token.txt
--rw-rw-rw-   0        0        0   432646 2016-06-02 01:39:06.000000 VSautomatic-2.1/VSautomatic/DeviceDB.xml
--rw-rw-rw-   0        0        0    24737 2022-10-28 06:26:28.000000 VSautomatic-2.1/VSautomatic/Dictionary.txt
--rw-rw-rw-   0        0        0     3326 2018-08-08 06:11:30.000000 VSautomatic-2.1/VSautomatic/IR_Remote.xml
--rw-rw-rw-   0        0        0   302689 2018-11-23 08:40:34.000000 VSautomatic-2.1/VSautomatic/MacroList.xml
--rw-rw-rw-   0        0        0     2708 2023-05-16 06:09:22.000000 VSautomatic-2.1/VSautomatic/MyCamera.py
--rw-rw-rw-   0        0        0     1460 2023-05-15 09:48:39.000000 VSautomatic-2.1/VSautomatic/MyRedRat.py
--rw-rw-rw-   0        0        0     5228 2023-05-15 09:48:39.000000 VSautomatic-2.1/VSautomatic/MyTools.py
--rw-rw-rw-   0        0        0     1481 2018-03-09 10:13:06.000000 VSautomatic-2.1/VSautomatic/NLog.config
--rw-rw-rw-   0        0        0   612864 2018-02-27 16:35:06.000000 VSautomatic-2.1/VSautomatic/NLog.dll
--rw-rw-rw-   0        0        0    18705 2023-05-15 09:48:39.000000 VSautomatic-2.1/VSautomatic/ReSTTerminal.py
--rw-rw-rw-   0        0        0   842240 2018-07-25 04:16:14.000000 VSautomatic-2.1/VSautomatic/RedRat.dll
--rw-rw-rw-   0        0        0    10752 2018-07-25 04:16:10.000000 VSautomatic-2.1/VSautomatic/RedRatHub.Connection.dll
--rw-rw-rw-   0        0        0     1768 2023-05-15 09:48:39.000000 VSautomatic-2.1/VSautomatic/RedRatHub.py
--rwxrwxrwx   0        0        0    14336 2018-07-25 04:16:16.000000 VSautomatic-2.1/VSautomatic/RedRatHubCmd.exe
--rw-rw-rw-   0        0        0      146 2018-03-09 10:13:06.000000 VSautomatic-2.1/VSautomatic/RedRatHubCmd.exe.config
--rw-rw-rw-   0        0        0    48640 2018-07-25 04:16:14.000000 VSautomatic-2.1/VSautomatic/RedRatHubCore.dll
--rw-rw-rw-   0        0        0     1052 2023-05-16 05:16:48.000000 VSautomatic-2.1/VSautomatic/RedRatHubS.py
--rw-rw-rw-   0        0        0     2522 2023-05-15 09:48:39.000000 VSautomatic-2.1/VSautomatic/TestCfgParse.py
--rw-rw-rw-   0        0        0    48335 2018-11-01 05:37:28.000000 VSautomatic-2.1/VSautomatic/Vizio.xml
--rw-rw-rw-   0        0        0    14450 2022-03-17 01:56:03.000000 VSautomatic-2.1/VSautomatic/Vizio_IR.xml
--rw-rw-rw-   0        0        0      154 2023-05-15 09:48:39.000000 VSautomatic-2.1/VSautomatic/__init__.py
--rw-rw-rw-   0        0        0     1121 2023-05-15 09:48:39.000000 VSautomatic-2.1/VSautomatic/deco.py
--rw-rw-rw-   0        0        0     3230 2023-05-15 09:48:39.000000 VSautomatic-2.1/VSautomatic/my_serial.py
--rw-rw-rw-   0        0        0       81 2023-05-15 06:49:02.000000 VSautomatic-2.1/VSautomatic/restlog.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 06:12:00.573331 VSautomatic-2.1/VSautomatic.egg-info/
--rw-rw-rw-   0        0        0      259 2023-05-16 06:12:00.000000 VSautomatic-2.1/VSautomatic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2023-05-16 06:12:00.000000 VSautomatic-2.1/VSautomatic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 06:12:00.000000 VSautomatic-2.1/VSautomatic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 06:12:00.000000 VSautomatic-2.1/VSautomatic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 06:12:00.573331 VSautomatic-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1026 2023-05-16 06:10:46.000000 VSautomatic-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 01:37:53.321280 VSautomatic-2.2/
+-rw-rw-rw-   0        0        0      259 2023-05-18 01:37:53.321280 VSautomatic-2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 01:37:53.311298 VSautomatic-2.2/VSautomatic/
+-rw-rw-rw-   0        0        0       10 2023-05-15 06:47:27.000000 VSautomatic-2.2/VSautomatic/Auth_Token.txt
+-rw-rw-rw-   0        0        0   432646 2016-06-02 01:39:06.000000 VSautomatic-2.2/VSautomatic/DeviceDB.xml
+-rw-rw-rw-   0        0        0    24737 2022-10-28 06:26:28.000000 VSautomatic-2.2/VSautomatic/Dictionary.txt
+-rw-rw-rw-   0        0        0     3326 2018-08-08 06:11:30.000000 VSautomatic-2.2/VSautomatic/IR_Remote.xml
+-rw-rw-rw-   0        0        0   302689 2018-11-23 08:40:34.000000 VSautomatic-2.2/VSautomatic/MacroList.xml
+-rw-rw-rw-   0        0        0     2708 2023-05-16 06:09:22.000000 VSautomatic-2.2/VSautomatic/MyCamera.py
+-rw-rw-rw-   0        0        0     1460 2023-05-15 09:48:39.000000 VSautomatic-2.2/VSautomatic/MyRedRat.py
+-rw-rw-rw-   0        0        0     5370 2023-05-18 01:36:44.000000 VSautomatic-2.2/VSautomatic/MyTools.py
+-rw-rw-rw-   0        0        0     1481 2018-03-09 10:13:06.000000 VSautomatic-2.2/VSautomatic/NLog.config
+-rw-rw-rw-   0        0        0   612864 2018-02-27 16:35:06.000000 VSautomatic-2.2/VSautomatic/NLog.dll
+-rw-rw-rw-   0        0        0    18705 2023-05-15 09:48:39.000000 VSautomatic-2.2/VSautomatic/ReSTTerminal.py
+-rw-rw-rw-   0        0        0   842240 2018-07-25 04:16:14.000000 VSautomatic-2.2/VSautomatic/RedRat.dll
+-rw-rw-rw-   0        0        0    10752 2018-07-25 04:16:10.000000 VSautomatic-2.2/VSautomatic/RedRatHub.Connection.dll
+-rw-rw-rw-   0        0        0     1768 2023-05-15 09:48:39.000000 VSautomatic-2.2/VSautomatic/RedRatHub.py
+-rwxrwxrwx   0        0        0    14336 2018-07-25 04:16:16.000000 VSautomatic-2.2/VSautomatic/RedRatHubCmd.exe
+-rw-rw-rw-   0        0        0      146 2018-03-09 10:13:06.000000 VSautomatic-2.2/VSautomatic/RedRatHubCmd.exe.config
+-rw-rw-rw-   0        0        0    48640 2018-07-25 04:16:14.000000 VSautomatic-2.2/VSautomatic/RedRatHubCore.dll
+-rw-rw-rw-   0        0        0     1052 2023-05-16 05:16:48.000000 VSautomatic-2.2/VSautomatic/RedRatHubS.py
+-rw-rw-rw-   0        0        0     2522 2023-05-15 09:48:39.000000 VSautomatic-2.2/VSautomatic/TestCfgParse.py
+-rw-rw-rw-   0        0        0    48335 2018-11-01 05:37:28.000000 VSautomatic-2.2/VSautomatic/Vizio.xml
+-rw-rw-rw-   0        0        0    14450 2022-03-17 01:56:03.000000 VSautomatic-2.2/VSautomatic/Vizio_IR.xml
+-rw-rw-rw-   0        0        0      154 2023-05-15 09:48:39.000000 VSautomatic-2.2/VSautomatic/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-05-15 09:48:39.000000 VSautomatic-2.2/VSautomatic/deco.py
+-rw-rw-rw-   0        0        0     3230 2023-05-15 09:48:39.000000 VSautomatic-2.2/VSautomatic/my_serial.py
+-rw-rw-rw-   0        0        0       81 2023-05-15 06:49:02.000000 VSautomatic-2.2/VSautomatic/restlog.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 01:37:53.321280 VSautomatic-2.2/VSautomatic.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-05-18 01:37:53.000000 VSautomatic-2.2/VSautomatic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2023-05-18 01:37:53.000000 VSautomatic-2.2/VSautomatic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 01:37:53.000000 VSautomatic-2.2/VSautomatic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-18 01:37:53.000000 VSautomatic-2.2/VSautomatic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 01:37:53.321280 VSautomatic-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-05-18 01:37:32.000000 VSautomatic-2.2/setup.py
```

### Comparing `VSautomatic-2.1/VSautomatic/DeviceDB.xml` & `VSautomatic-2.2/VSautomatic/DeviceDB.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/Dictionary.txt` & `VSautomatic-2.2/VSautomatic/Dictionary.txt`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/IR_Remote.xml` & `VSautomatic-2.2/VSautomatic/IR_Remote.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/MacroList.xml` & `VSautomatic-2.2/VSautomatic/MacroList.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/MyCamera.py` & `VSautomatic-2.2/VSautomatic/MyCamera.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/MyRedRat.py` & `VSautomatic-2.2/VSautomatic/MyRedRat.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/MyTools.py` & `VSautomatic-2.2/VSautomatic/MyTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,16 @@
     def __init__(self):
         self.my_serial = None
         self.my_camera = None
         self.my_rest = None
         self.RedRatS = None
         self.RedRatC = None
 
-    
     # COM-Serial-Start
-    def serial_start(self, portname):
+    def serial_connect(self, portname):
         '''
         portname:COMx
         | `Serial Start`    | COM3 |
         '''
         if self.my_serial is None:
             self.my_serial = SigmaSerial()
         try:
@@ -68,24 +67,23 @@
                 # logfile.close()
         except Exception as e:
             print(e)
 
     def serial_writer(self, command):
         self.my_serial.writes(command)
         
-
-
-    def serial_stop(self):
+    def serial_disconnect(self):
         if not self.my_serial is None:
             self.alive = False
             if self.my_serial.isOpen():
                 self.my_serial.close()
     
     # COM-Serial-End
     # ====================================================================================================================================
+
     # Rest-Start
     def rest_pair(self,ip):
         self.my_rest = restterminal(ip)
         self.auth_token = self.my_rest.sshpair()
         fw = open(Auth_Token, "w")
         fw.write(self.auth_token)
         fw.close()
@@ -101,14 +99,15 @@
         restValue = self.my_rest.parse_command(command, self.read_auth_token)
         print('restValue:{}'.format(restValue))
         time.sleep(3)
         self.my_rest.parse_command("restlog", self.read_auth_token)
 
     # Rest-End
     # ====================================================================================================================================
+
     # Camera-Start
     def camera_open(self):
         if self.my_camera is None:
             self.my_camera = CameraCapture()
         try:
             self.my_camera.open()
             if self.my_camera.isOpen():
@@ -118,37 +117,38 @@
                 # self.thread_read.start()
                 return True
             else:
                 return False
         except Exception as e:
             return False
             
-
     def camera_imageCapture(self,picName,frameNum):
         self.my_camera.imageCapture(picName,frameNum)
 
     def camera_videoCapture(self,vidName,duration):
         self.my_camera.videoCapture(vidName,duration)
 
-
-    def camera_stop(self):
+    def camera_closed(self):
         if not self.my_camera is None:
             self.alive = False
             if self.my_camera.isOpen():
                 self.my_camera.close()
 
     # Camera-End
     # ====================================================================================================================================
+
     # RedRat_Start
     def RedRat_Run_Server(self,RedRatdate):
         self.RedRatS = RedRatHubCmdSetUp(RedRatdate)
         self.RedRatS.run()
         
     def RedRat_Kill_Server(self):
         self.RedRatS.kill()
 
     def RedRat_Client(self,test_pc_ip,redRat_Name,redRatDataset):
         self.RedRatC = DEV_REDRAT(test_pc_ip,redRat_Name,redRatDataset)
 
     def RedRat_Client_Send(self,IRMessage,PauseTimer):
         self.RedRatC.IR_GEN(IRMessage,int(PauseTimer))
+
     # RedRat_End
+    # ====================================================================================================================================
```

### Comparing `VSautomatic-2.1/VSautomatic/NLog.config` & `VSautomatic-2.2/VSautomatic/NLog.config`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/NLog.dll` & `VSautomatic-2.2/VSautomatic/NLog.dll`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/ReSTTerminal.py` & `VSautomatic-2.2/VSautomatic/ReSTTerminal.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/RedRat.dll` & `VSautomatic-2.2/VSautomatic/RedRat.dll`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/RedRatHub.Connection.dll` & `VSautomatic-2.2/VSautomatic/RedRatHub.Connection.dll`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/RedRatHub.py` & `VSautomatic-2.2/VSautomatic/RedRatHub.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/RedRatHubCmd.exe` & `VSautomatic-2.2/VSautomatic/RedRatHubCmd.exe`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/RedRatHubCore.dll` & `VSautomatic-2.2/VSautomatic/RedRatHubCore.dll`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/RedRatHubS.py` & `VSautomatic-2.2/VSautomatic/RedRatHubS.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/TestCfgParse.py` & `VSautomatic-2.2/VSautomatic/TestCfgParse.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/Vizio.xml` & `VSautomatic-2.2/VSautomatic/Vizio.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/Vizio_IR.xml` & `VSautomatic-2.2/VSautomatic/Vizio_IR.xml`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/deco.py` & `VSautomatic-2.2/VSautomatic/deco.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic/my_serial.py` & `VSautomatic-2.2/VSautomatic/my_serial.py`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/VSautomatic.egg-info/SOURCES.txt` & `VSautomatic-2.2/VSautomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VSautomatic-2.1/setup.py` & `VSautomatic-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
  
 # requirements = ['numpy']       # 自定义工具中需要的依赖包
  
 setuptools.setup(
     name="VSautomatic",       # 自定义工具包的名字
-    version="2.1",             # 版本号
+    version="2.2",             # 版本号
     author="jasonliu",           # 作者名字
     author_email="batianhu4444@gmail.com",  # 作者邮箱
     description="VS Automatic Tools", # 自定义工具包的简介
     license='MIT-0',           # 许可协议
     url="https://pypi.org/manage/projects/",              # 项目开源地址
     packages=setuptools.find_packages(),  # 自动发现自定义工具包中的所有包和子包
     # install_requires=requirements,  # 安装自定义工具包需要依赖的包
```

