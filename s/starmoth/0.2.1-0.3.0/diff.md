# Comparing `tmp/starmoth-0.2.1.tar.gz` & `tmp/starmoth-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starmoth-0.2.1.tar", last modified: Wed Mar  1 20:49:02 2023, max compression
+gzip compressed data, was "starmoth-0.3.0.tar", last modified: Thu May 18 01:47:02 2023, max compression
```

## Comparing `starmoth-0.2.1.tar` & `starmoth-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 20:49:02.006607 starmoth-0.2.1/
--rw-r--r--   0 root         (0) root         (0)      762 2023-03-01 20:49:02.006607 starmoth-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      478 2023-03-01 19:53:50.000000 starmoth-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 20:49:02.002607 starmoth-0.2.1/moth/
--rw-rw-rw-   0 root         (0) root         (0)     2302 2023-03-01 19:53:50.000000 starmoth-0.2.1/moth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 20:49:02.002607 starmoth-0.2.1/moth/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1901 2023-03-01 19:53:50.000000 starmoth-0.2.1/moth/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 20:49:02.002607 starmoth-0.2.1/moth/driver/
--rw-rw-rw-   0 root         (0) root         (0)     2006 2023-03-01 19:53:50.000000 starmoth-0.2.1/moth/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 20:49:02.002607 starmoth-0.2.1/moth/message/
--rw-rw-rw-   0 root         (0) root         (0)     4158 2023-03-01 19:53:50.000000 starmoth-0.2.1/moth/message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.2.1/moth/message/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 20:49:02.002607 starmoth-0.2.1/moth/server/
--rw-rw-rw-   0 root         (0) root         (0)     2703 2023-03-01 19:53:50.000000 starmoth-0.2.1/moth/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-01 20:49:02.006607 starmoth-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 20:49:02.006607 starmoth-0.2.1/starmoth.egg-info/
--rw-r--r--   0 root         (0) root         (0)      762 2023-03-01 20:49:01.000000 starmoth-0.2.1/starmoth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-03-01 20:49:01.000000 starmoth-0.2.1/starmoth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 20:49:01.000000 starmoth-0.2.1/starmoth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-01 20:49:01.000000 starmoth-0.2.1/starmoth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-03-01 20:49:01.000000 starmoth-0.2.1/starmoth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-01 20:49:01.000000 starmoth-0.2.1/starmoth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.166228 starmoth-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-05-18 01:47:02.166228 starmoth-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2023-05-17 18:11:33.000000 starmoth-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.158228 starmoth-0.3.0/moth/
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-05-17 16:52:15.000000 starmoth-0.3.0/moth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.162228 starmoth-0.3.0/moth/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-05-11 20:09:31.000000 starmoth-0.3.0/moth/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.162228 starmoth-0.3.0/moth/driver/
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-05-17 16:52:15.000000 starmoth-0.3.0/moth/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.162228 starmoth-0.3.0/moth/message/
+-rw-rw-rw-   0 root         (0) root         (0)     6535 2023-05-17 16:52:15.000000 starmoth-0.3.0/moth/message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-01 19:53:50.000000 starmoth-0.3.0/moth/message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.162228 starmoth-0.3.0/moth/server/
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2023-05-11 20:09:31.000000 starmoth-0.3.0/moth/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 01:47:02.166228 starmoth-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-03-01 19:53:50.000000 starmoth-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:47:02.166228 starmoth-0.3.0/starmoth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-18 01:47:02.000000 starmoth-0.3.0/starmoth.egg-info/top_level.txt
```

### Comparing `starmoth-0.2.1/moth/__init__.py` & `starmoth-0.3.0/moth/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import zmq
 
-from moth.message import HandshakeMsg, ImagePromptMsg, parse_message
+from moth.message import HandshakeMsg, ImagePromptMsg, parse_message, HandshakeTaskTypes
 from moth.message.exceptions import MothMessageError
 
 
 class Moth:
     _PROMPT_FUNCTIONS = []
     _MATH_FUNCTIONS = []
 
-    def __init__(self, name: str, token: str = ""):
+    def __init__(self, name: str, token: str = "", task_type: HandshakeTaskTypes = HandshakeTaskTypes.CLASSIFICATION):
         self.name = name
         self._token = token
         self.stop = False
+        self.task_type = task_type
 
     def run(self, url="tcp://localhost:7171"):
         self.stop = False
         context = zmq.Context()
         socket = context.socket(zmq.DEALER)
         socket.setsockopt_string(zmq.IDENTITY, self.name)
 
         try:
             socket.connect(url)
             # This is a handshake call to prove our identity
-            handshake = HandshakeMsg(self.name, self._token, "v0.0.0")
+            handshake = HandshakeMsg(self.name, self._token, "v0.0.0", self.task_type)
             socket.send(handshake.serialize_envelope())
             self._req_loop(socket)
         except KeyboardInterrupt:
             print("\nExit...")
             self.stop = True
 
     def prompt(self, func):
```

### Comparing `starmoth-0.2.1/moth/cli/__init__.py` & `starmoth-0.3.0/moth/cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import numpy as np
 
 from moth import Moth
 from moth.server import Server
-from moth.message import HandshakeMsg, ImagePromptMsg, PromptResultMsg
+from moth.message import HandshakeMsg, ImagePromptMsg, ClassificationResultMsg
 from moth.driver import TestImagesInFolder
 
 
 def print_askii_image(img):
     size = img.size
     for y in range(size[1]):
         line = ""
@@ -51,22 +51,22 @@
 @click.option("--host", default="localhost", help="Where is the server running")
 @click.option("--name", default="cli-client", help="The name of this client")
 def client(port, host, name):
     click.echo("Start a moth client")
     moth = Moth(name, "t123")
 
     @moth.prompt
-    def on_prompt(prompt: ImagePromptMsg) -> PromptResultMsg:
+    def on_prompt(prompt: ImagePromptMsg) -> ClassificationResultMsg:
         if max(prompt.image.size) < 30:
             print_askii_image(prompt.image)
         else:
             prompt.image.show()
         answer = input("What class? > ")
 
-        return PromptResultMsg(prompt_id=prompt.id, class_name=answer)
+        return ClassificationResultMsg(prompt_id=prompt.id, class_name=answer)
 
     server_url = f"tcp://{host}:{port}"
     moth.run(url=server_url)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `starmoth-0.2.1/moth/driver/__init__.py` & `starmoth-0.3.0/moth/driver/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 from PIL import Image, ImageOps
 from pathlib import Path
 from typing import Optional
 
-from moth.message import ImagePromptMsg, PromptResultMsg
+from moth.message import ImagePromptMsg, ClassificationResultMsg
 
 
 class ModelDriver(abc.ABC):
     @abc.abstractmethod
     def on_model_result(self):
         raise NotImplementedError()
 
@@ -20,15 +20,15 @@
     def __init__(self, folder, ext="png"):
         self.folder = folder
         self.files = Path(folder).glob(f"*.{ext}")
         self._rubric = {}
         self._correct_count = 0
         self._error_count = 0
 
-    def on_model_result(self, result: PromptResultMsg):
+    def on_model_result(self, result: ClassificationResultMsg):
         if result.prompt_id not in self._rubric:
             print("What question are you answering?")
             return
 
         expected_answer = self._rubric[result.prompt_id]
         if expected_answer == result.class_name:
             self._correct_count += 1
```

### Comparing `starmoth-0.2.1/moth/server/__init__.py` & `starmoth-0.3.0/moth/server/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable, Dict
 import zmq
 from moth.driver import ModelDriver
-from moth.message import HandshakeMsg, PromptResultMsg, Msg, parse_message
+from moth.message import HandshakeMsg, ClassificationResultMsg, Msg, ObjectDetectionResultMsg, parse_message
 from moth.message.exceptions import MothMessageError
 
 
 class IdentityPool:
     def __init__(self):
         self._ids = []
 
@@ -65,15 +65,19 @@
                 msg_bytes = socket.recv()
 
                 try:
                     message = parse_message(msg_bytes)
                     if isinstance(message, HandshakeMsg) and self._driver_factory:
                         self._drivers[identity] = self._driver_factory(message)
 
-                    if isinstance(message, PromptResultMsg):
+                    if isinstance(message, ClassificationResultMsg):
+                        if identity in self._drivers:
+                            self._drivers[identity].on_model_result(message)
+                    
+                    if isinstance(message, ObjectDetectionResultMsg):
                         if identity in self._drivers:
                             self._drivers[identity].on_model_result(message)
 
                 except MothMessageError as err:
                     print(err)
                 except Exception as err:
                     print(err)
```

### Comparing `starmoth-0.2.1/setup.py` & `starmoth-0.3.0/setup.py`

 * *Files identical despite different names*

