# Comparing `tmp/Log_Api-0.0.5.tar.gz` & `tmp/Log_Api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Log_Api-0.0.5.tar", last modified: Wed May 17 21:01:45 2023, max compression
+gzip compressed data, was "Log_Api-0.0.6.tar", last modified: Thu May 18 17:26:48 2023, max compression
```

## Comparing `Log_Api-0.0.5.tar` & `Log_Api-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:45.023326 Log_Api-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:44.955503 Log_Api-0.0.5/Log_Api/
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:44.994403 Log_Api-0.0.5/Log_Api/Class/
--rw-rw-rw-   0        0        0     2050 2023-05-16 21:33:41.000000 Log_Api-0.0.5/Log_Api/Class/Database.py
--rw-rw-rw-   0        0        0     3212 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Class/LogAPI.py
--rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Class/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Class/response..py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:44.997394 Log_Api-0.0.5/Log_Api/Models/
--rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Models/LogAPI.py
--rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.5/Log_Api/Models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:45.020333 Log_Api-0.0.5/Log_Api/Utils/
--rw-rw-rw-   0        0        0     7752 2023-05-17 21:00:18.000000 Log_Api-0.0.5/Log_Api/Utils/Aws.py
--rw-rw-rw-   0        0        0     3494 2023-05-15 20:49:03.000000 Log_Api-0.0.5/Log_Api/Utils/ModelsType.py
--rw-rw-rw-   0        0        0     4008 2023-05-15 19:54:00.000000 Log_Api-0.0.5/Log_Api/Utils/Response.py
--rw-rw-rw-   0        0        0     1181 2023-05-15 20:49:32.000000 Log_Api-0.0.5/Log_Api/Utils/Template.py
--rw-rw-rw-   0        0        0      117 2023-05-15 20:43:57.000000 Log_Api-0.0.5/Log_Api/Utils/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-15 20:44:12.000000 Log_Api-0.0.5/Log_Api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 21:01:44.986454 Log_Api-0.0.5/Log_Api.egg-info/
--rw-rw-rw-   0        0        0      284 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.5/Log_Api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-05-17 21:01:44.000000 Log_Api-0.0.5/Log_Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2023-05-17 21:01:45.022328 Log_Api-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.5/README.md
--rw-rw-rw-   0        0        0    14763 2023-05-17 21:01:41.000000 Log_Api-0.0.5/aws_handler_decorators.py
--rw-rw-rw-   0        0        0       42 2023-05-17 21:01:45.023326 Log_Api-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-05-17 17:23:19.000000 Log_Api-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:26:48.431662 Log_Api-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-18 17:26:48.372807 Log_Api-0.0.6/Log_Api/
+drwxrwxrwx   0        0        0        0 2023-05-18 17:26:48.405719 Log_Api-0.0.6/Log_Api/Class/
+-rw-rw-rw-   0        0        0     2050 2023-05-16 21:33:41.000000 Log_Api-0.0.6/Log_Api/Class/Database.py
+-rw-rw-rw-   0        0        0     3212 2023-05-15 16:56:09.000000 Log_Api-0.0.6/Log_Api/Class/LogAPI.py
+-rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.6/Log_Api/Class/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.6/Log_Api/Class/response..py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:26:48.408709 Log_Api-0.0.6/Log_Api/Models/
+-rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.6/Log_Api/Models/LogAPI.py
+-rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.6/Log_Api/Models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:26:48.428668 Log_Api-0.0.6/Log_Api/Utils/
+-rw-rw-rw-   0        0        0     8335 2023-05-18 17:25:34.000000 Log_Api-0.0.6/Log_Api/Utils/Aws.py
+-rw-rw-rw-   0        0        0     3494 2023-05-15 20:49:03.000000 Log_Api-0.0.6/Log_Api/Utils/ModelsType.py
+-rw-rw-rw-   0        0        0     4008 2023-05-15 19:54:00.000000 Log_Api-0.0.6/Log_Api/Utils/Response.py
+-rw-rw-rw-   0        0        0     1181 2023-05-15 20:49:32.000000 Log_Api-0.0.6/Log_Api/Utils/Template.py
+-rw-rw-rw-   0        0        0      117 2023-05-15 20:43:57.000000 Log_Api-0.0.6/Log_Api/Utils/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-15 20:44:12.000000 Log_Api-0.0.6/Log_Api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:26:48.398737 Log_Api-0.0.6/Log_Api.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-05-18 17:26:48.000000 Log_Api-0.0.6/Log_Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-05-18 17:26:48.000000 Log_Api-0.0.6/Log_Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:26:48.000000 Log_Api-0.0.6/Log_Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.6/Log_Api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2023-05-18 17:26:48.000000 Log_Api-0.0.6/Log_Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-05-18 17:26:48.000000 Log_Api-0.0.6/Log_Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2023-05-18 17:26:48.430651 Log_Api-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.6/README.md
+-rw-rw-rw-   0        0        0    14763 2023-05-18 17:26:20.000000 Log_Api-0.0.6/aws_handler_decorators.py
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:26:48.431662 Log_Api-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      665 2023-05-17 17:23:19.000000 Log_Api-0.0.6/setup.py
```

### Comparing `Log_Api-0.0.5/Log_Api/Class/Database.py` & `Log_Api-0.0.6/Log_Api/Class/Database.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/Log_Api/Class/LogAPI.py` & `Log_Api-0.0.6/Log_Api/Class/LogAPI.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/Log_Api/Class/response..py` & `Log_Api-0.0.6/Log_Api/Class/response..py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/Log_Api/Models/LogAPI.py` & `Log_Api-0.0.6/Log_Api/Models/LogAPI.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/Log_Api/Utils/Aws.py` & `Log_Api-0.0.6/Log_Api/Utils/Aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,17 +93,33 @@
         response = client.invoke(
             FunctionName=function_name,
             Payload=data,
             LogType='Tail',
             InvocationType=inv_type
         )
 
+        if inv_type == 'RequestResponse':
+            response = cls.get_data_from_response(response)
         return response
 
     @classmethod
+    def get_data_from_response(cls, response):
+        """
+        Obtener datos de la respuesta de la función lambda
+        :param: response
+            respuesta de la función lambda
+        :return: data
+        """
+        response_document = response['Payload'].read().decode('utf-8')
+        response_document = json.loads(response_document)
+        response_body = json.loads(response_document['body'])
+
+        return response_body
+    
+    @classmethod
     def function_name(cls, function: str, service: str='', stage=os.getenv('STAGE'), ext_app=False):
         """
         Crea nombre de función lambda
         :param: function
             nombre de la función
         :param: stage
             nombre del stage
```

### Comparing `Log_Api-0.0.5/Log_Api/Utils/ModelsType.py` & `Log_Api-0.0.6/Log_Api/Utils/ModelsType.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/Log_Api/Utils/Response.py` & `Log_Api-0.0.6/Log_Api/Utils/Response.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/Log_Api/Utils/Template.py` & `Log_Api-0.0.6/Log_Api/Utils/Template.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/Log_Api.egg-info/SOURCES.txt` & `Log_Api-0.0.6/Log_Api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/README.md` & `Log_Api-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.5/aws_handler_decorators.py` & `Log_Api-0.0.6/aws_handler_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     basestring
 except NameError:
     basestring = str
 
 logger = logging.getLogger(__name__)
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 class AwsHandlerDecorator(object):
     def __init__(self, func):
         update_wrapper(self, func)
         self.func = func
 
     def __call__(self, event, context):
```

### Comparing `Log_Api-0.0.5/setup.py` & `Log_Api-0.0.6/setup.py`

 * *Files identical despite different names*

