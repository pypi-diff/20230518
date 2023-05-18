# Comparing `tmp/northgravity-0.1.5.tar.gz` & `tmp/northgravity-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "northgravity-0.1.5.tar", last modified: Tue Apr 18 12:32:31 2023, max compression
+gzip compressed data, was "northgravity-0.1.6.tar", last modified: Thu May 18 09:41:56 2023, max compression
```

## Comparing `northgravity-0.1.5.tar` & `northgravity-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:32:31.781472 northgravity-0.1.5/
--rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    27037 2023-04-18 12:32:31.781472 northgravity-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    26604 2023-04-18 12:32:31.000000 northgravity-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:32:31.781472 northgravity-0.1.5/northgravity/
--rw-rw-r--   0 root         (0) root         (0)     1112 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/Authenticator.py
--rw-rw-r--   0 root         (0) root         (0)     9175 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/DatalakeHandler.py
--rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/ExceptionHandler.py
--rw-rw-r--   0 root         (0) root         (0)     6567 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/HTTPCalller.py
--rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/StatusHandler.py
--rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/TaskHandler.py
--rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/Timeseries.py
--rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.5/northgravity/__init__.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:32:31.781472 northgravity-0.1.5/northgravity.egg-info/
--rw-r--r--   0 root         (0) root         (0)    27037 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 12:32:31.000000 northgravity-0.1.5/northgravity.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 12:32:31.781472 northgravity-0.1.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:41:56.023805 northgravity-0.1.6/
+-rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    29830 2023-05-18 09:41:56.023805 northgravity-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29397 2023-05-18 09:41:55.000000 northgravity-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:41:56.019805 northgravity-0.1.6/northgravity/
+-rw-rw-r--   0 root         (0) root         (0)     1327 2023-05-18 09:33:33.000000 northgravity-0.1.6/northgravity/Authenticator.py
+-rw-rw-r--   0 root         (0) root         (0)     9175 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/DatalakeHandler.py
+-rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/ExceptionHandler.py
+-rw-rw-r--   0 root         (0) root         (0)     6567 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/HTTPCalller.py
+-rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/StatusHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/TaskHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/Timeseries.py
+-rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.6/northgravity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:41:56.023805 northgravity-0.1.6/northgravity.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    29830 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 09:41:55.000000 northgravity-0.1.6/northgravity.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 09:41:56.023805 northgravity-0.1.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.6/setup.py
```

### Comparing `northgravity-0.1.5/LICENSE` & `northgravity-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.5/PKG-INFO` & `northgravity-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,15 @@
 
 - a single python script that is ran thanks to the Python Runner task within a pipeline in the NG application
 
 - a single Jupyter Notebook that is ran thanks to the Jupyter Runner task within a pipeline in the NG application
 
 - an ensemble of python scripts that are part of a container, for a Task created by the user, used in a pipeline in the NG application
 
+Examples of usage can be found at the bottom of the documentation.
  
 
 Note that the SDK does not cover everything from API documentation but rather commonly used features.
 
 The scope of the SDK:
 
 - **Datalake Handler** - downloading / uploading / reading files from the data lake  
@@ -39,19 +40,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.5
+pip3 install northgravity==0.1.6
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.5
+northgravity==0.1.6
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
 
 
@@ -65,16 +66,16 @@
 
 - LOGIN → login received from NG
 
 - PASSWORD → password to log in. Credentials are used to generate the token so that each request is authenticated.
 
 - NG_API_ENDPOINT → the URL to the NG platform API (by default, the url is set to https://api.northgravity.com)
  
-
 This allows to pass the authentication process and directs users' requests to the NG environment API.
+Alternatively, instead of the LOGIN and PASSWORD, you may set NG_API_KEY environment variable with an API key generated within the NG platform to enable the authentication process.
 
 Other variables may be useful when creating the tasks within the platform:
 
 - NG_STATUS_GROUP_NAME → the group on the data lake where the pipeline is located, and is used to display the statuses
 
 - JOBID → any value; when the pipeline is executed, this value is set by the NG platform
 
@@ -676,15 +677,15 @@
 
 i=1
 if i>1:
     raise PythonStepWarnException(message='The value of i is bigger than 1! Stopping pipeline execution.')
 
 ```
 --- -
-## Example
+## Example 1 - OOP
 To simplify the use of the SDK methods in a script, Python SDK methods can be inherited by the user’s main class. 
 
 Below is an example of a class that has 3 methods:
 
 - Download raw data (or take from the previous task)
 - Process the data  
 - Upload the data to datalake and pass it to the next task
@@ -732,10 +733,76 @@
 if __name__ == '__main__':
     status = ng.StatusHandler()
     Runner().run()
     status.info('Test Pipeline Finished')
 
  ```
 
+## Example 2 - functional programming
+
+The SDK methods may be used in functional programming simple scripts.
+Below is an example of a script that:
+- Downloads the data from Input #1
+- Processes the data
+- Uploads the data to datalake and passes it to the next task
+
+ ```python
+
+######## 
+#This part consists of local running setup for development and testing purposes.
+# It is not needed when running on the northgravity platform, since those variables are available in the platform's environment
+
+import os
+# login and password to the northgravity application for authentication 
+os.environ['LOGIN'] = ''
+os.environ['PASSWORD'] = ''
+
+# filename and name of the DataLake group to download the data from
+os.environ['Input #1'] = "{'name':'', 'groupName':''}"
+
+# the DataLake group to save the file to
+# on the platform defaults to the group where the pipeline running the script is saved
+os.environ['NG_STATUS_GROUP_NAME'] = ''
+
+# specify the api endpoint to northgravity application
+os.environ['NG_API_ENDPOINT'] = ''
+
+######## 
+
+import os, sys
+import io
+import northgravity as ng
+import pandas as pd
+
+# logging
+import logging ; logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+log = logging.getLogger()
+
+# initialize taskhandler from the Python SDK to communicate between pipeline tasks
+th = ng.TaskHandler()
+
+# download data from Input #1 of the task (Python Runner)
+df_io = th.download_from_input_parameter('Input #1')
+df = pd.read_csv(df_io)
+log.info('Data from Input #1 downloaded.')
+
+# your code here
+df_processed = your_processing_function(df)
+
+# stream the dataframe as the Bytes IO file (does not save the csv to disc)
+file_io = io.BytesIO(df_processed.to_csv(index=False).encode())
+
+# upload the file to Output #1 of the task
+th.upload_to_output_parameter(output_name='Output #1',
+                                        file=file_io,
+                                        # add your file name here
+                                        file_upload_name='',
+                                        # the group name defaults to the pipeline group
+                                        # you can also use it explicitly: group_name='Name of The Group on Datalake'
+                                        group_name=os.environ.get('NG_STATUS_GROUP_NAME'),
+                                        # the dataframe is saved as a flat file
+                                        # use file_type='NCSV' to save NCSV-type datasets into Timeseries database
+                                        file_type='SOURCE')
+```
 
 ### Who do I talk to? ###
 * Admin: NorthGravity info@northgravity.com
```

### Comparing `northgravity-0.1.5/README.md` & `northgravity-0.1.6/northgravity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,34 @@
+Metadata-Version: 2.1
+Name: northgravity
+Version: 0.1.6
+Summary: Python SDK for NorthGravity platform
+Home-page: https://www.northgravity.com/
+Author: NorthGravity
+Author-email: info@northgravity.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # NORTH GRAVITY PYTHON SDK #
 
 This document describes the North Gravity Python SDK which enables external users to use the NG platform tools within their python scripts. 
 
 The Python SDK can be used within:
 
 - a single python script that is ran thanks to the Python Runner task within a pipeline in the NG application
 
 - a single Jupyter Notebook that is ran thanks to the Jupyter Runner task within a pipeline in the NG application
 
 - an ensemble of python scripts that are part of a container, for a Task created by the user, used in a pipeline in the NG application
 
+Examples of usage can be found at the bottom of the documentation.
  
 
 Note that the SDK does not cover everything from API documentation but rather commonly used features.
 
 The scope of the SDK:
 
 - **Datalake Handler** - downloading / uploading / reading files from the data lake  
@@ -25,19 +40,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.5
+pip3 install northgravity==0.1.6
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.5
+northgravity==0.1.6
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
 
 
@@ -51,16 +66,16 @@
 
 - LOGIN → login received from NG
 
 - PASSWORD → password to log in. Credentials are used to generate the token so that each request is authenticated.
 
 - NG_API_ENDPOINT → the URL to the NG platform API (by default, the url is set to https://api.northgravity.com)
  
-
 This allows to pass the authentication process and directs users' requests to the NG environment API.
+Alternatively, instead of the LOGIN and PASSWORD, you may set NG_API_KEY environment variable with an API key generated within the NG platform to enable the authentication process.
 
 Other variables may be useful when creating the tasks within the platform:
 
 - NG_STATUS_GROUP_NAME → the group on the data lake where the pipeline is located, and is used to display the statuses
 
 - JOBID → any value; when the pipeline is executed, this value is set by the NG platform
 
@@ -662,15 +677,15 @@
 
 i=1
 if i>1:
     raise PythonStepWarnException(message='The value of i is bigger than 1! Stopping pipeline execution.')
 
 ```
 --- -
-## Example
+## Example 1 - OOP
 To simplify the use of the SDK methods in a script, Python SDK methods can be inherited by the user’s main class. 
 
 Below is an example of a class that has 3 methods:
 
 - Download raw data (or take from the previous task)
 - Process the data  
 - Upload the data to datalake and pass it to the next task
@@ -718,10 +733,76 @@
 if __name__ == '__main__':
     status = ng.StatusHandler()
     Runner().run()
     status.info('Test Pipeline Finished')
 
  ```
 
+## Example 2 - functional programming
+
+The SDK methods may be used in functional programming simple scripts.
+Below is an example of a script that:
+- Downloads the data from Input #1
+- Processes the data
+- Uploads the data to datalake and passes it to the next task
+
+ ```python
+
+######## 
+#This part consists of local running setup for development and testing purposes.
+# It is not needed when running on the northgravity platform, since those variables are available in the platform's environment
+
+import os
+# login and password to the northgravity application for authentication 
+os.environ['LOGIN'] = ''
+os.environ['PASSWORD'] = ''
+
+# filename and name of the DataLake group to download the data from
+os.environ['Input #1'] = "{'name':'', 'groupName':''}"
+
+# the DataLake group to save the file to
+# on the platform defaults to the group where the pipeline running the script is saved
+os.environ['NG_STATUS_GROUP_NAME'] = ''
+
+# specify the api endpoint to northgravity application
+os.environ['NG_API_ENDPOINT'] = ''
+
+######## 
+
+import os, sys
+import io
+import northgravity as ng
+import pandas as pd
+
+# logging
+import logging ; logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+log = logging.getLogger()
+
+# initialize taskhandler from the Python SDK to communicate between pipeline tasks
+th = ng.TaskHandler()
+
+# download data from Input #1 of the task (Python Runner)
+df_io = th.download_from_input_parameter('Input #1')
+df = pd.read_csv(df_io)
+log.info('Data from Input #1 downloaded.')
+
+# your code here
+df_processed = your_processing_function(df)
+
+# stream the dataframe as the Bytes IO file (does not save the csv to disc)
+file_io = io.BytesIO(df_processed.to_csv(index=False).encode())
+
+# upload the file to Output #1 of the task
+th.upload_to_output_parameter(output_name='Output #1',
+                                        file=file_io,
+                                        # add your file name here
+                                        file_upload_name='',
+                                        # the group name defaults to the pipeline group
+                                        # you can also use it explicitly: group_name='Name of The Group on Datalake'
+                                        group_name=os.environ.get('NG_STATUS_GROUP_NAME'),
+                                        # the dataframe is saved as a flat file
+                                        # use file_type='NCSV' to save NCSV-type datasets into Timeseries database
+                                        file_type='SOURCE')
+```
 
 ### Who do I talk to? ###
-* Admin: NorthGravity info@northgravity.com
+* Admin: NorthGravity info@northgravity.com
```

### Comparing `northgravity-0.1.5/northgravity/Authenticator.py` & `northgravity-0.1.6/northgravity/Authenticator.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 
 log = logging.getLogger(LOGGER_NAME)
 
 
 class Authenticator:
     def __init__(self):       
         self.token = os.getenv('NG_API_AUTHTOKEN')
+        self.api_key = os.getenv('NG_API_KEY')
         self.login = os.getenv('LOGIN')
         self.password = os.getenv('PASSWORD')
 
     def get_token(self):
         if self.token is not None:
             log.debug('Authentication with Web Token ...')
             return {'Authorization': f'Bearer {self.token}'}
+        
+        elif self.api_key is not None:
+            log.debug('Authentication with API Key ...')
+            return {'Authorization': f'ApiKey {self.api_key}'}
 
         else:
             if self.login is not None and self.password is not None:
                 log.debug('Authentication with Credentials ...')
                 credentials = self.login + ":" + self.password
                 message_bytes = credentials.encode('ascii')
                 base64_enc = base64.b64encode(message_bytes).decode('UTF-8')
```

### Comparing `northgravity-0.1.5/northgravity/DatalakeHandler.py` & `northgravity-0.1.6/northgravity/DatalakeHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.5/northgravity/HTTPCalller.py` & `northgravity-0.1.6/northgravity/HTTPCalller.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.5/northgravity/StatusHandler.py` & `northgravity-0.1.6/northgravity/StatusHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.5/northgravity/TaskHandler.py` & `northgravity-0.1.6/northgravity/TaskHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.5/northgravity/Timeseries.py` & `northgravity-0.1.6/northgravity/Timeseries.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.5/northgravity/__init__.py` & `northgravity-0.1.6/northgravity/__init__.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.5/northgravity.egg-info/PKG-INFO` & `northgravity-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,20 @@
-Metadata-Version: 2.1
-Name: northgravity
-Version: 0.1.5
-Summary: Python SDK for NorthGravity platform
-Home-page: https://www.northgravity.com/
-Author: NorthGravity
-Author-email: info@northgravity.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NORTH GRAVITY PYTHON SDK #
 
 This document describes the North Gravity Python SDK which enables external users to use the NG platform tools within their python scripts. 
 
 The Python SDK can be used within:
 
 - a single python script that is ran thanks to the Python Runner task within a pipeline in the NG application
 
 - a single Jupyter Notebook that is ran thanks to the Jupyter Runner task within a pipeline in the NG application
 
 - an ensemble of python scripts that are part of a container, for a Task created by the user, used in a pipeline in the NG application
 
+Examples of usage can be found at the bottom of the documentation.
  
 
 Note that the SDK does not cover everything from API documentation but rather commonly used features.
 
 The scope of the SDK:
 
 - **Datalake Handler** - downloading / uploading / reading files from the data lake  
@@ -39,19 +26,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.5
+pip3 install northgravity==0.1.6
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.5
+northgravity==0.1.6
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
 
 
@@ -65,16 +52,16 @@
 
 - LOGIN → login received from NG
 
 - PASSWORD → password to log in. Credentials are used to generate the token so that each request is authenticated.
 
 - NG_API_ENDPOINT → the URL to the NG platform API (by default, the url is set to https://api.northgravity.com)
  
-
 This allows to pass the authentication process and directs users' requests to the NG environment API.
+Alternatively, instead of the LOGIN and PASSWORD, you may set NG_API_KEY environment variable with an API key generated within the NG platform to enable the authentication process.
 
 Other variables may be useful when creating the tasks within the platform:
 
 - NG_STATUS_GROUP_NAME → the group on the data lake where the pipeline is located, and is used to display the statuses
 
 - JOBID → any value; when the pipeline is executed, this value is set by the NG platform
 
@@ -676,15 +663,15 @@
 
 i=1
 if i>1:
     raise PythonStepWarnException(message='The value of i is bigger than 1! Stopping pipeline execution.')
 
 ```
 --- -
-## Example
+## Example 1 - OOP
 To simplify the use of the SDK methods in a script, Python SDK methods can be inherited by the user’s main class. 
 
 Below is an example of a class that has 3 methods:
 
 - Download raw data (or take from the previous task)
 - Process the data  
 - Upload the data to datalake and pass it to the next task
@@ -732,10 +719,76 @@
 if __name__ == '__main__':
     status = ng.StatusHandler()
     Runner().run()
     status.info('Test Pipeline Finished')
 
  ```
 
+## Example 2 - functional programming
+
+The SDK methods may be used in functional programming simple scripts.
+Below is an example of a script that:
+- Downloads the data from Input #1
+- Processes the data
+- Uploads the data to datalake and passes it to the next task
+
+ ```python
+
+######## 
+#This part consists of local running setup for development and testing purposes.
+# It is not needed when running on the northgravity platform, since those variables are available in the platform's environment
+
+import os
+# login and password to the northgravity application for authentication 
+os.environ['LOGIN'] = ''
+os.environ['PASSWORD'] = ''
+
+# filename and name of the DataLake group to download the data from
+os.environ['Input #1'] = "{'name':'', 'groupName':''}"
+
+# the DataLake group to save the file to
+# on the platform defaults to the group where the pipeline running the script is saved
+os.environ['NG_STATUS_GROUP_NAME'] = ''
+
+# specify the api endpoint to northgravity application
+os.environ['NG_API_ENDPOINT'] = ''
+
+######## 
+
+import os, sys
+import io
+import northgravity as ng
+import pandas as pd
+
+# logging
+import logging ; logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+log = logging.getLogger()
+
+# initialize taskhandler from the Python SDK to communicate between pipeline tasks
+th = ng.TaskHandler()
+
+# download data from Input #1 of the task (Python Runner)
+df_io = th.download_from_input_parameter('Input #1')
+df = pd.read_csv(df_io)
+log.info('Data from Input #1 downloaded.')
+
+# your code here
+df_processed = your_processing_function(df)
+
+# stream the dataframe as the Bytes IO file (does not save the csv to disc)
+file_io = io.BytesIO(df_processed.to_csv(index=False).encode())
+
+# upload the file to Output #1 of the task
+th.upload_to_output_parameter(output_name='Output #1',
+                                        file=file_io,
+                                        # add your file name here
+                                        file_upload_name='',
+                                        # the group name defaults to the pipeline group
+                                        # you can also use it explicitly: group_name='Name of The Group on Datalake'
+                                        group_name=os.environ.get('NG_STATUS_GROUP_NAME'),
+                                        # the dataframe is saved as a flat file
+                                        # use file_type='NCSV' to save NCSV-type datasets into Timeseries database
+                                        file_type='SOURCE')
+```
 
 ### Who do I talk to? ###
-* Admin: NorthGravity info@northgravity.com
+* Admin: NorthGravity info@northgravity.com
```

### Comparing `northgravity-0.1.5/setup.py` & `northgravity-0.1.6/setup.py`

 * *Files identical despite different names*

