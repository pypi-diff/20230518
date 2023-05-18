# Comparing `tmp/ampapi-1.1.3.tar.gz` & `tmp/ampapi-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampapi-1.1.3.tar", last modified: Thu May  4 03:29:29 2023, max compression
+gzip compressed data, was "ampapi-1.1.4.tar", last modified: Thu May 18 02:20:21 2023, max compression
```

## Comparing `ampapi-1.1.3.tar` & `ampapi-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-04 03:29:29.137461 ampapi-1.1.3/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-05-04 03:26:52.000000 ampapi-1.1.3/LICENCE
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-05-04 03:29:29.137461 ampapi-1.1.3/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     3610 2023-05-04 03:26:52.000000 ampapi-1.1.3/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-04 03:29:29.137461 ampapi-1.1.3/ampapi/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-05-04 03:26:52.000000 ampapi-1.1.3/ampapi/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)   160317 2023-05-04 03:27:51.000000 ampapi-1.1.3/ampapi/ampapi.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-04 03:29:29.137461 ampapi-1.1.3/ampapi.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-05-04 03:29:29.000000 ampapi-1.1.3/ampapi.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-05-04 03:29:29.000000 ampapi-1.1.3/ampapi.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-05-04 03:29:29.000000 ampapi-1.1.3/ampapi.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-05-04 03:29:29.000000 ampapi-1.1.3/ampapi.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-05-04 03:26:52.000000 ampapi-1.1.3/pyproject.toml
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-05-04 03:29:29.137461 ampapi-1.1.3/setup.cfg
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-18 02:20:21.950864 ampapi-1.1.4/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-05-18 02:15:32.000000 ampapi-1.1.4/LICENCE
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-05-18 02:20:21.950864 ampapi-1.1.4/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     3610 2023-05-18 02:15:32.000000 ampapi-1.1.4/README.md
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-18 02:20:21.946864 ampapi-1.1.4/ampapi/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-05-18 02:15:32.000000 ampapi-1.1.4/ampapi/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)   160593 2023-05-18 02:20:09.000000 ampapi-1.1.4/ampapi/ampapi.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-18 02:20:21.950864 ampapi-1.1.4/ampapi.egg-info/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-05-18 02:20:21.000000 ampapi-1.1.4/ampapi.egg-info/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-05-18 02:20:21.000000 ampapi-1.1.4/ampapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-05-18 02:20:21.000000 ampapi-1.1.4/ampapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-05-18 02:20:21.000000 ampapi-1.1.4/ampapi.egg-info/top_level.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-05-18 02:15:32.000000 ampapi-1.1.4/pyproject.toml
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-05-18 02:20:21.950864 ampapi-1.1.4/setup.cfg
```

### Comparing `ampapi-1.1.3/LICENCE` & `ampapi-1.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `ampapi-1.1.3/PKG-INFO` & `ampapi-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.1.3/README.md` & `ampapi-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ampapi-1.1.3/ampapi/ampapi.py` & `ampapi-1.1.4/ampapi/ampapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,15 @@
             AMP Type: String
         :param FriendlyName: A friendly name for this instance. If left blank, AMP will generate one for you.
         :type FriendlyName: strTrue
             AMP Type: String
         :param Secret: Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.
         :type Secret: strTrue
             AMP Type: String
-        :param PostCreate: 0: Do nothing, 10: Start instance only, 20: Start instance and update application, 30: Full application startup.
+        :param PostCreate: 0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.
             AMP Type: PostCreateActions
         :param ExtraProvisionSettings: A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.
         :type ExtraProvisionSettings: dict[str, str]True
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: RunningTask
         """
         return self.APICall(endpoint="ADSModule/DeployTemplate", data={
@@ -500,15 +500,15 @@
             AMP Type: String
         :param FriendlyName: A friendly name for this instance. If left blank, AMP will generate one for you.
         :type FriendlyName: strTrue
             AMP Type: String
         :param Secret: Must be a non-empty strong in order to get a callback on deployment state change. This secret will be passed back to you in the callback so you can verify the request.
         :type Secret: strTrue
             AMP Type: String
-        :param PostCreate: 0: Do nothing, 10: Start instance only, 20: Start instance and update application, 30: Full application startup.
+        :param PostCreate: 0: Do nothing, 1: Start instance only, 2: Start instance and update application, 3: Full application startup.
             AMP Type: PostCreateActions
         :param ExtraProvisionSettings: A dictionary of setting nodes and values to create the new instance with. Identical in function to the provisioning arguments in the template itself.
         :type ExtraProvisionSettings: dict[str, str]True
             AMP Type: Dictionary<String, String>
         :returns: AMP Type: RunningTask
         """
         return await self.APICallAsync(endpoint="ADSModule/DeployTemplate", data={
@@ -2046,42 +2046,50 @@
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/AppendFileChunk", data={
             "Filename": Filename, 
             "Data": Data, 
             "Delete": Delete, 
         })
 
-    def FileManagerPlugin_ReadFileChunk(self, Filename: str, Offset: int):
+    def FileManagerPlugin_ReadFileChunk(self, Filename: str, Offset: int, ChunkSize: int):
         """
         :param Filename: 
         :type Filename: strFalse
             AMP Type: String
         :param Offset: 
         :type Offset: intFalse
             AMP Type: Int64
+        :param ChunkSize: 
+        :type ChunkSize: intTrue
+            AMP Type: Int64
         :returns: AMP Type: ActionResult<String>
         """
         return self.APICall(endpoint="FileManagerPlugin/ReadFileChunk", data={
             "Filename": Filename, 
             "Offset": Offset, 
+            "ChunkSize": ChunkSize, 
         })
 
-    async def FileManagerPlugin_ReadFileChunkAsync(self, Filename: str, Offset: int):
+    async def FileManagerPlugin_ReadFileChunkAsync(self, Filename: str, Offset: int, ChunkSize: int):
         """
         :param Filename: 
         :type Filename: strFalse
             AMP Type: String
         :param Offset: 
         :type Offset: intFalse
             AMP Type: Int64
+        :param ChunkSize: 
+        :type ChunkSize: intTrue
+            AMP Type: Int64
         :returns: AMP Type: ActionResult<String>
         """
         return await self.APICallAsync(endpoint="FileManagerPlugin/ReadFileChunk", data={
             "Filename": Filename, 
             "Offset": Offset, 
+            "ChunkSize": ChunkSize, 
         })
 
     def FileManagerPlugin_WriteFileChunk(self, Filename: str, Data: str, Offset: int, FinalChunk: bool):
         """
         :param Filename: 
         :type Filename: strFalse
             AMP Type: String
```

### Comparing `ampapi-1.1.3/ampapi.egg-info/PKG-INFO` & `ampapi-1.1.4/ampapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ampapi-1.1.3/setup.cfg` & `ampapi-1.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ampapi
-version = 1.1.3
+version = 1.1.4
 author = Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 author_email = p0t4t0sandwich@gmail.com
 description = A Python implemenation of the Cubecoders AMP API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/p0t4t0sandwich/ampapi-python
 classifiers =
```

