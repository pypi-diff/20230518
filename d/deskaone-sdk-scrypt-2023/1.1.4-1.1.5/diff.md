# Comparing `tmp/deskaone_sdk_scrypt_2023-1.1.4.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.4.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.5.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.1.4.tar` & `deskaone_sdk_scrypt_2023-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      754 2023-05-17 23:52:27.140868 deskaone_sdk_scrypt_2023-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.4/README.md
--rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     6046 2023-05-09 16:58:57.983045 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-09 16:39:36.272506 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      491 2023-05-17 23:52:22.165847 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    30170 2023-05-17 23:52:15.674584 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.4/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-05-17 23:56:25.812906 deskaone_sdk_scrypt_2023-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.5/README.md
+-rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     6046 2023-05-09 16:58:57.983045 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-09 16:39:36.272506 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-17 23:56:19.494552 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    30045 2023-05-17 23:56:15.831112 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.5/setup.py
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.5/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.1.4"
+version = "1.1.5"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
         
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=socks4&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
         Saves = [Proxy for Proxy in Result.replace(' ', '').replace('\r', '').split('\n')]
         for i in range(len(Saves)):
             Proxy = Saves[random.randint(0, len(Saves) - 1)]
@@ -254,15 +254,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
         
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=socks5&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
         Saves = [Proxy for Proxy in Result.replace(' ', '').replace('\r', '').split('\n')]
         for i in range(len(Saves)):
             Proxy = Saves[random.randint(0, len(Saves) - 1)]
@@ -277,15 +277,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -316,15 +316,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -355,15 +355,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -393,15 +393,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
     
     @property
     def __https__(self):
         r  = self.Session.get('https://www.proxy-list.download/HTTPS')
         Result = BeautifulSoup(r.content, 'html5lib')
         Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
@@ -421,15 +421,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
         
     @property
     def __socks4__(self):
         r  = self.Session.get('https://www.proxy-list.download/SOCKS4')
         Result = BeautifulSoup(r.content, 'html5lib')
         Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
@@ -449,15 +449,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
         
     @property
     def __socks5__(self):
         r  = self.Session.get('https://www.proxy-list.download/SOCKS5')
         Result = BeautifulSoup(r.content, 'html5lib')
         Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
@@ -477,15 +477,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
     
     @property
     def __proxy__(self):
         self.__http__
         self.__https__
         self.__socks4__
@@ -524,15 +524,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
-                if i == random.randint(20, len(Saves) - 1): break
+                if i == 20: break
             except Error:pass
             
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
@@ -565,19 +565,29 @@
     
     @property
     def ListProxy(self) -> List[Dict[str, str]]:
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
     def __get__(self, Authorization: Optional[str] = None, New = True, *args, **kwargs):
         if Authorization is not None and Authorization != '':__WebShare__(Authorization).Main(New)
-        if kwargs.get('ProxyScrape') is True or kwargs.get('ProxyScrape') is None:__ProxyScrape__().Main(New)
-        if kwargs.get('Geonode') is True or kwargs.get('Geonode') is None:__Geonode__().Main(New)
-        if kwargs.get('FreeProxyList') is True or kwargs.get('FreeProxyList') is None:__FreeProxyList__().Main(New)
-        if kwargs.get('ProxyList') is True or kwargs.get('ProxyList') is None:__ProxyList__().Main(New)
-        if kwargs.get('HideMy') is True or kwargs.get('HideMy') is None:__HideMy__().Main(New)
+        try:
+            if kwargs.get('ProxyScrape') is True or kwargs.get('ProxyScrape') is None:__ProxyScrape__().Main(New)
+        except:pass
+        try:
+            if kwargs.get('Geonode') is True or kwargs.get('Geonode') is None:__Geonode__().Main(New)
+        except:pass
+        try:
+            if kwargs.get('FreeProxyList') is True or kwargs.get('FreeProxyList') is None:__FreeProxyList__().Main(New)
+        except:pass
+        try:
+            if kwargs.get('ProxyList') is True or kwargs.get('ProxyList') is None:__ProxyList__().Main(New)
+        except:pass
+        try:
+            if kwargs.get('HideMy') is True or kwargs.get('HideMy') is None:__HideMy__().Main(New)
+        except:pass
     
     def __check__(self, *args, **kwargs):
         if kwargs.get('IpPort') is None: raise Error('IpPort Required')
         ListProxy, Count = self.ListProxy, 0
         while True:
             Count += 1
             try:
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.5/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/setup.py` & `deskaone_sdk_scrypt_2023-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.1.4',
+    'version': '1.1.5',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.4/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.1.4
+Version: 1.1.5
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

