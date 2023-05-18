# Comparing `tmp/iphack-1.3.4.tar.gz` & `tmp/iphack-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphack-1.3.4.tar", last modified: Thu May 18 19:01:55 2023, max compression
+gzip compressed data, was "iphack-1.3.6.tar", last modified: Thu May 18 19:18:01 2023, max compression
```

## Comparing `iphack-1.3.4.tar` & `iphack-1.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:01:55.875580 iphack-1.3.4/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7315 2023-05-18 19:01:55.875580 iphack-1.3.4/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     5795 2023-05-18 18:56:47.000000 iphack-1.3.4/README.md
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:01:55.871580 iphack-1.3.4/iphack/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.4/iphack/__init__.py
--rw-------   0 u0_a314  (10314) u0_a314  (10314)    44261 2023-05-18 19:01:52.000000 iphack-1.3.4/iphack/iphack.py
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:01:55.871580 iphack-1.3.4/iphack.egg-info/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7315 2023-05-18 19:01:55.000000 iphack-1.3.4/iphack.egg-info/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-05-18 19:01:55.000000 iphack-1.3.4/iphack.egg-info/SOURCES.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-05-18 19:01:55.000000 iphack-1.3.4/iphack.egg-info/dependency_links.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       65 2023-05-18 19:01:55.000000 iphack-1.3.4/iphack.egg-info/requires.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-05-18 19:01:55.000000 iphack-1.3.4/iphack.egg-info/top_level.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-05-18 19:01:55.875580 iphack-1.3.4/setup.cfg
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     2293 2023-05-18 19:01:43.000000 iphack-1.3.4/setup.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:18:01.183580 iphack-1.3.6/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7315 2023-05-18 19:18:01.183580 iphack-1.3.6/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     5795 2023-05-18 18:56:47.000000 iphack-1.3.6/README.md
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:18:01.183580 iphack-1.3.6/iphack/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.6/iphack/__init__.py
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)    44289 2023-05-18 19:17:41.000000 iphack-1.3.6/iphack/iphack.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-18 19:18:01.183580 iphack-1.3.6/iphack.egg-info/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7315 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/SOURCES.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/dependency_links.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       65 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/requires.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-05-18 19:18:01.000000 iphack-1.3.6/iphack.egg-info/top_level.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-05-18 19:18:01.183580 iphack-1.3.6/setup.cfg
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     2293 2023-05-18 19:17:51.000000 iphack-1.3.6/setup.py
```

### Comparing `iphack-1.3.4/PKG-INFO` & `iphack-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.3.4
+Version: 1.3.6
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.3.4 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.6 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
```

### Comparing `iphack-1.3.4/README.md` & `iphack-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `iphack-1.3.4/iphack/iphack.py` & `iphack-1.3.6/iphack/iphack.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 red = '\033[31m'
 yellow = '\033[93m'
 lgreen = '\033[92m'
 clear = '\033[0m'
 bold = '\033[01m'
 cyan = '\033[96m'
-version = "1.3.4"
+version = "1.3.6"
 referer_list = ["https://www.google.com/", "https://www.youtube.com/", "https://www.twitter.com/", "https://www.discord.com/", "https://www.tiktok.com/", "https://www.instagram.com/", "https://check-host.net/", "https://github.com", "https://gitlab.com", "https://he1zen.rf.gd"]
 
 major = str(sys.version_info.major)
 minor = str(sys.version_info.minor)
 path = str(sys.exec_prefix+"/lib/python"+major+"."+minor+"/site-packages/iphack/")
 
 global log
@@ -375,14 +375,15 @@
         find = find.replace("/", "")
         find = find.replace(" ", "")
         get = requests.get("https://raw.githubusercontent.com/mishakorzik/mishakorzik.menu.io/master/%D0%A1%D0%B5%D1%80%D0%B2%D0%B5%D1%80/https.json").json()
         ip = str(get["mailip"])
         port = int(get["mailport"])
         check = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         check.connect((ip, port))
+        check.settimeout(5)
         find = str(find)
         check.sendall(bytes("get|domain,ip|info|"+find,'UTF-8'))
         code = check.recv(256)
         get = code.decode('utf-8')
         if get == "-":
             print("not found")
         else:
```

### Comparing `iphack-1.3.4/iphack.egg-info/PKG-INFO` & `iphack-1.3.6/iphack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.3.4
+Version: 1.3.6
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.3.4 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.6 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
```

### Comparing `iphack-1.3.4/setup.py` & `iphack-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='iphack',  # should match the package folder
     packages=['iphack'],  # should match the package folder
-    version='1.3.4',  # important for updates
+    version='1.3.6',  # important for updates
     python_requires=">=3.4",
     license='Apache 2.0',  # should match your chosen license
     description='the most ideal tool for finding out information about IP, etc.',
     long_description=long_description,  # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='MishaKorzhik_He1Zen',
     author_email='developer.mishakorzhik@gmail.com',
```

