# Comparing `tmp/osais-1.0.44.tar.gz` & `tmp/osais-1.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-wztvg7u7\osais-1.0.44.tar", last modified: Wed May 17 10:39:07 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-03tn37f_\osais-1.0.45.tar", last modified: Thu May 18 17:02:33 2023, max compression
```

## Comparing `osais-1.0.44.tar` & `osais-1.0.45.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 10:39:07.357032 osais-1.0.44/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.44/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-05-17 10:39:07.356032 osais-1.0.44/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.44/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 10:39:07.351032 osais-1.0.44/osais/
--rw-rw-rw-   0        0        0     1006 2023-05-17 10:38:31.000000 osais-1.0.44/osais/__init__.py
--rw-rw-rw-   0        0        0    54100 2023-05-17 10:37:38.000000 osais-1.0.44/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-05-17 10:39:07.355031 osais-1.0.44/osais.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-17 10:39:07.000000 osais-1.0.44/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.44/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 10:39:07.357032 osais-1.0.44/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-05-17 10:38:49.000000 osais-1.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:02:33.442157 osais-1.0.45/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.45/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-05-18 17:02:33.441158 osais-1.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.45/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:02:33.436149 osais-1.0.45/osais/
+-rw-rw-rw-   0        0        0     1006 2023-05-18 17:00:02.000000 osais-1.0.45/osais/__init__.py
+-rw-rw-rw-   0        0        0    54406 2023-05-18 16:59:27.000000 osais-1.0.45/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:02:33.440157 osais-1.0.45/osais.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 17:02:33.000000 osais-1.0.45/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.45/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:02:33.442157 osais-1.0.45/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-05-18 17:00:20.000000 osais-1.0.45/setup.py
```

### Comparing `osais-1.0.44/LICENSE` & `osais-1.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.44/PKG-INFO` & `osais-1.0.45/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.44
+Version: 1.0.45
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.44/osais/__init__.py` & `osais-1.0.45/osais/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.44"
+__version__="1.0.45"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isDebug
 from .osais import osais_isDocker
 from .osais import osais_isLocal
 from .osais import osais_isVirtualAI
```

### Comparing `osais-1.0.44/osais/osais.py` & `osais-1.0.45/osais/osais.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.44"
+__version__="1.0.45"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -362,14 +362,15 @@
     if gS3!=None:
         try:
             # Filename - File to upload
             # Bucket - Bucket to upload to (the top level directory under AWS S3)
             # Key - S3 object name (can contain subdirectories). If not specified then file_name is used
             _baseName=os.path.basename(_filename)
             gS3.meta.client.upload_file(Filename=_filename, Bucket=gS3Bucket, Key=_dirS3+_baseName)
+            print("=> Uploaded "+_filename+" to S3")
             return root+_dirS3+_baseName
             
         except Exception as err:
             consoleLog({"msg":"Could not upload file to S3"})
             raise err
         
     return False
@@ -383,17 +384,18 @@
             # Filename - File to upload
             # Bucket - Bucket to upload to (the top level directory under AWS S3)
             # Key - S3 object name (can contain subdirectories). If not specified then file_name is used
             _baseName=os.path.basename(_filePath)
             local_file_path = _dir+_baseName
 
             gS3.Bucket(gS3Bucket).download_file(_filePath, local_file_path)
+            print("=> Downloaded "+_filePath+" from S3")
             return local_file_path
         except Exception as err:
-            consoleLog({"msg":"Could not download file from S3"})
+            consoleLog({"msg":"Could not download file "+_filePath+" from S3"})
             raise err
         
     return False
 
 
 ## ========================================================================
 ## 
@@ -507,20 +509,22 @@
         _dirFile=f'{current_working_directory}/{_name}.json'
         fJSON = open(_dirFile)
         _json = json.load(fJSON)
     except Exception as err:
         print(f'CRITICAL: No config file {_dirFile}')
         sys.exit()
 
-    gVersion=_json["version"]
-    gDescription=_json["description"]
-    gOrigin=_json["origin"]
-    _cost=_json["default_cost"]
-    if _cost!=None:
-        gDefaultCost=_cost
+    # do not set global vars for osais config
+    if _name!= "osais":
+        gVersion=_json["version"]
+        gDescription=_json["description"]
+        gOrigin=_json["origin"]
+        _cost=_json["default_cost"]
+        if _cost!=None:
+            gDefaultCost=_cost
 
     return _json
 
 # get the full AI config, including JSON params and hardware info
 def _getFullConfig(_name) :
     global gUsername
     global gPortAI
@@ -533,16 +537,16 @@
     global gExtIP
     global gIsLocal
  
     _ip=gExtIP
     if gIsDebug:
         _ip=gIPLocal                ## we register with local ip if we are in local gateway mode
 
-    _jsonAI=_loadConfig(_name)
     _jsonBase=_loadConfig("osais")
+    _jsonAI=_loadConfig(_name)
 
     objCudaInfo=getCudaInfo()
     gpuName="no GPU"
     if objCudaInfo != 0 and "name" in objCudaInfo and objCudaInfo["name"]:
         gpuName=objCudaInfo["name"]
 
     return {
@@ -663,14 +667,15 @@
     if os.environ.get('AWS_ACCESS_KEY_ID') and AWSID==None:
         AWSID=os.environ.get('AWS_ACCESS_KEY_ID')
     if os.environ.get('AWS_ACCESS_KEY_SECRET') and AWSSecret==None:
         AWSSecret=os.environ.get('AWS_ACCESS_KEY_SECRET')
 
     if AWSID!=None and AWSSecret!=None:
         gAWSSession = boto3.Session(
+            region_name="eu-west-2",            ## todo : externalise this
             aws_access_key_id=AWSID,
             aws_secret_access_key=AWSSecret
         )
         gS3 = gAWSSession.resource('s3')
         print(f'=> Logged into AWS S3')
         
     if gIsDebug: 
@@ -1077,16 +1082,17 @@
     fn_run=args[0]
     _args=args[1]
 
     ## do not process twice same uid
     _uid=_args.get('-uid')
     if _uid in gAProcessed:
         consoleLog({"msg": "Not processing "+str(_uid)+", already tried!"})
-        return  None
-    
+        return  None    
+    print ("\r\n=> Processing request with UID "+str(_uid))
+
     ## process the filename and download it locally
     try:
         ## the filename of the locally downloaded "url_upload" url (or the S3 url)
         _filename=_args.get('-filename')
 
         # if file was in S3, download it
         _isFileInS3= getS3BucketRoot() in _filename
@@ -1096,22 +1102,21 @@
                 _basename=_filename[11:]
                 _filename=osais_downloadFileFromS3(_basename, gInputDir)
                 _args["-filename"]=os.path.basename(_filename)
                 _args["-idir"]=gInputDir
                 _args["-odir"]=gOutputDir
 
             except Exception as err:
-                consoleLog({"msg":"Could not download image from S3"})
                 raise err
         else:
             if not _args["-warmup"]:
                 raise ValueError("CRITICAL: require a upload url in S3 ")
                 
     except Exception as err:
-        consoleLog({"msg":"did not get an upload url"})
+        consoleLog({"msg":"did not get a -filename or could not process"})
         raise err
 
     ## start time
     gIsBusy=True
     beg_date = datetime.utcnow()
     
     ## reprocess AI args
```

### Comparing `osais-1.0.44/osais.egg-info/PKG-INFO` & `osais-1.0.45/osais.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.44
+Version: 1.0.45
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.44/setup.py` & `osais-1.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.44',
+    version='1.0.45',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

