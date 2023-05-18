# Comparing `tmp/longPolling-0.0.2.tar.gz` & `tmp/longPolling-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longPolling-0.0.2.tar", last modified: Thu May 18 14:40:22 2023, max compression
+gzip compressed data, was "longPolling-0.0.3.tar", last modified: Thu May 18 15:36:35 2023, max compression
```

## Comparing `longPolling-0.0.2.tar` & `longPolling-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 14:40:22.063311 longPolling-0.0.2/
--rw-rw-rw-   0        0        0     1854 2023-05-18 14:40:22.063311 longPolling-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-05-18 14:34:19.000000 longPolling-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-18 14:40:22.057797 longPolling-0.0.2/longPolling/
--rw-rw-rw-   0        0        0       67 2023-04-26 15:30:57.000000 longPolling-0.0.2/longPolling/__init__.py
--rw-rw-rw-   0        0        0     5477 2023-05-18 14:17:12.000000 longPolling-0.0.2/longPolling/client.py
--rw-rw-rw-   0        0        0     6453 2023-05-18 14:18:27.000000 longPolling-0.0.2/longPolling/server.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:40:22.062310 longPolling-0.0.2/longPolling.egg-info/
--rw-rw-rw-   0        0        0     1854 2023-05-18 14:40:21.000000 longPolling-0.0.2/longPolling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-18 14:40:21.000000 longPolling-0.0.2/longPolling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 14:40:21.000000 longPolling-0.0.2/longPolling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-18 14:40:21.000000 longPolling-0.0.2/longPolling.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 14:40:21.000000 longPolling-0.0.2/longPolling.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 14:40:22.064313 longPolling-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-05-18 14:29:38.000000 longPolling-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:36:35.663687 longPolling-0.0.3/
+-rw-rw-rw-   0        0        0     1854 2023-05-18 15:36:35.662687 longPolling-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-05-18 14:34:19.000000 longPolling-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-18 15:36:35.636687 longPolling-0.0.3/longPolling/
+-rw-rw-rw-   0        0        0       67 2023-04-26 15:30:57.000000 longPolling-0.0.3/longPolling/__init__.py
+-rw-rw-rw-   0        0        0     5478 2023-05-18 15:30:27.000000 longPolling-0.0.3/longPolling/client.py
+-rw-rw-rw-   0        0        0     6998 2023-05-18 15:30:47.000000 longPolling-0.0.3/longPolling/server.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:36:35.662687 longPolling-0.0.3/longPolling.egg-info/
+-rw-rw-rw-   0        0        0     1854 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-18 15:36:35.000000 longPolling-0.0.3/longPolling.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 15:36:35.663687 longPolling-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2023-05-18 15:36:19.000000 longPolling-0.0.3/setup.py
```

### Comparing `longPolling-0.0.2/PKG-INFO` & `longPolling-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longPolling
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple long polling implementation
 Home-page: https://kuankuan2007.gitee.io/docs/long-polling/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: long polling,flask,http,thread
 Platform: windows
```

### Comparing `longPolling-0.0.2/README.rst` & `longPolling-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `longPolling-0.0.2/longPolling/client.py` & `longPolling-0.0.3/longPolling/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             raise LookupError("No login has been performed")
         data=rsa.encrypt(data,self.pubKey)
         retsult=requests.post(self.host+f"/{self.id}/send",data=data)
     def login(self,name)->bool:
         if self.key!=None:
             return False
         try:
-            (public_key, private_key) = rsa.newkeys(512)
+            (public_key, private_key) = rsa.newkeys(1024)
             retsult=requests.post(self.host+"/login",json={
                 "username":name,
                 "key": public_key.save_pkcs1().decode("utf-8")
             })
             if retsult.status_code==200:
                 self.id=name
                 self.key=private_key
```

### Comparing `longPolling-0.0.2/longPolling/server.py` & `longPolling-0.0.3/longPolling/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,61 +7,62 @@
 import rsa
 import random
 def _randString():
     return "".join(random.choices(["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v","w", "x", "y", "z",
                     "A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V","W", "X", "Y", "Z",
                     "1","2","3","4","5","6","7","8","9","0"],k=random.randint(10,100)))
 class Server:
-    def __init__(self,host:Union[str,None]=None,port:Union[int,None]=None,timeout:int=60,name:str='Server',login:Union[None,Callable[[str],Any]]=None,logout:Union[None,Callable[[str],Any]]=None):
+    def __init__(self,host:Union[str,None]=None,port:Union[int,None]=None,timeout:int=60,name:str='Server',login:Union[None,Callable[[Any,str],Any]]=None,logout:Union[None,Callable[[Any,str],Any]]=None,threaded:bool=True,started:bool=True):
         """
         :param host:the host to listen on
         :param port:the port to listen on
         :param timeout: the number of seconds, it should be same as the timeout in client
         :param name: the name of the server. it can be changed at any time.
         :param login: it will be caller after a new user is login successfully
         :param logout: it will be caller after a user is logout successfully
+        :threaded: Whether to run in a new thread
+        :started: Whether to start the server
         """
         self.app = flask.Flask(name)
         self.logger = logging.getLogger(name)
         self.host = host
         self.port = port
         self.keys:Dict[str,rsa.PublicKey]={}
         self.loginCallBack=login
         self.logoutCallBack=logout
         self.timeout = timeout
         self.messages:Dict[str,List[bytes]] = {}
-        
+        self.threaded=threaded
         
         @self.app.route("/<user>/listen",methods=["GET"])
         def main(user):
             return self.main(user)
         
         @self.app.route("/login",methods=["POST"])
         def doLogin():
             return self.doLogin()
         
         @self.app.route("/logout",methods=["POST"])
         def doLogout():
             return self.doLogout()
+        if started:
+            self.start()
         
-        self.logger.info("start server")
-        self.thread = threading.Thread(target=self._start,daemon=True)
-        self.thread.start()
     def doLogin(self):
         try:
             now=flask.request.json
             assert type(now)==dict
         except:
             return "decode error",400
         if (all([i in now for i in ["username","key"]])):
             if (now["username"] in self.keys):
                 return "duplicate user name",403
             self.keys[now["username"]]=rsa.PublicKey.load_pkcs1(now["key"].encode("utf-8"))
             if (self.loginCallBack):
-                self.loginCallBack(now["username"])
+                self.loginCallBack(self,now["username"])
             return "succeed",200
         else:
             return "insufficient",400
     def doLogout(self):
         try:
             now=flask.request.json
             assert type(now)==dict
@@ -71,15 +72,15 @@
             if (now["username"] not in self.keys):
                 return "unregistered",400
             test=_randString()
             try:
                 assert rsa.decrypt(rsa.encrypt(test.encode("utf-8"),self.keys[now["username"]]),rsa.PrivateKey.load_pkcs1(now["key"].encode("utf-8")))==test.encode("utf-8")
                 del self.keys[now["username"]]
                 if (self.logoutCallBack):
-                    self.logoutCallBack(now["username"])
+                    self.logoutCallBack(self,now["username"])
                 return "succeed",200
             except:
                 return "key error",403
         else:
             return "insufficient",400
     def main(self,user):
         start=time.time()
@@ -89,59 +90,70 @@
             if (user not in self.keys):
                 return "unregistered",403
             if (time.time()-start)>=self.timeout:
                 return "timeout",500
             if (self.messages.get(user,[])):
                 return rsa.encrypt(self.messages[user][0],self.keys[user]),200
             time.sleep(1)
+    def start(self):
+        self.logger.info("start server")
+        if self.threaded:
+            self.thread = threading.Thread(target=self._start,daemon=True)
+            self.thread.start()
+        else:
+            self._start()
     def _start(self):
         self.app.run(self.host,self.port,threaded=True)
     def send(self,user:str,message:Union[dict,list,bytes])->None:
         """
         :param user: username
         :param message: message to send to user,must be bytes-like object or dict or list
         """
         if type(message)!=bytes:
             message = json.dumps(message).encode("utf-8")
         if (user not in self.messages):
             self.messages[user]=[]
         self.messages[user].append(message)
         self.logger.info("new message sent to user "+user)
 class BothwayServer(Server):
-    def __init__(self,host:Union[str,None]=None,port:Union[int,None]=None,timeout:int=60,name:str='Server',login:Union[None,Callable[[str],Any]]=None,logout:Union[None,Callable[[str],Any]]=None,receive:Union[None,Callable[[str,bytes],Any]]=None):
+    def __init__(self,host:Union[str,None]=None,port:Union[int,None]=None,timeout:int=60,name:str='Server',login:Union[None,Callable[[Server,str],Any]]=None,logout:Union[None,Callable[[Server,str],Any]]=None,receive:Union[None,Callable[[Server,str,bytes],Any]]=None,threaded:bool=True,started:bool=True):
         """
         :param host:the host to listen on
         :param port:the port to listen on
         :param timeout: the number of seconds, it should be same as the timeout in client
         :param name: the name of the server. it can be changed at any time.
         :param login: it will be caller after a new user is login successfully
         :param logout: it will be caller after a user is logout successfully
         :param receive: it will be caller after receive a message
+        :threaded: Whether to run in a new thread
+        :started: Whether to start the server
         """
-        super().__init__(host,port,timeout,name,login,logout)
+        super().__init__(host,port,timeout,name,login,logout,threaded,False)
         self.receive=receive
         @self.app.route("/<user>/send",methods=["POST"])
         def doListen(user):
             return self.doListen(user,flask.request.stream.read())
         self.priKey:Dict[str,rsa.PrivateKey]={}
+        if started:
+            self.start()
     def doListen(self,user:str,data:bytes):
         try:
             data=rsa.decrypt(data,self.priKey[user])
         except:
             return "keyError",403
         if (self.receive):
-            self.receive(user,data)
+            self.receive(self,user,data)
         return "success"
     def doLogin(self):
         retsult=super().doLogin()
         if(retsult[1]==200):
             try:
                 now=flask.request.json
                 assert type(now)==dict
             except:
                 return "decode error",400
-            (public_key, private_key) = rsa.newkeys(512)
+            (public_key, private_key) = rsa.newkeys(1024)
             self.priKey[now["username"]]=private_key
             return json.dumps({
                 "key":public_key.save_pkcs1().decode("utf-8")
             }),200
         return retsult
```

### Comparing `longPolling-0.0.2/longPolling.egg-info/PKG-INFO` & `longPolling-0.0.3/longPolling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longPolling
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple long polling implementation
 Home-page: https://kuankuan2007.gitee.io/docs/long-polling/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: long polling,flask,http,thread
 Platform: windows
```

### Comparing `longPolling-0.0.2/setup.py` & `longPolling-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 setup(
     name = 'longPolling',
-    version = '0.0.2',
+    version = '0.0.3',
     keywords = ['long polling',"flask","http","thread"],
     description = 'Simple long polling implementation',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/long-polling/",
     install_requires = [
```

