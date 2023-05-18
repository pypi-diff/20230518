# Comparing `tmp/pytmv1-0.5.0.tar.gz` & `tmp/pytmv1-0.5.1.tar.gz`

## Comparing `pytmv1-0.5.0.tar` & `pytmv1-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.0/.coveragerc
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.0/tox.ini
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/__about__.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/__init__.py
--rwxr-xr-x   0        0        0    26298 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/caller.py
--rwxr-xr-x   0        0        0    10916 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/core.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/exceptions.py
--rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/mapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/py.typed
--rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/results.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/__init__.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/commons.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/enums.py
--rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/requests.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/responses.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.0/.gitignore
--rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.0/LICENSE.txt
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.0/README.md
--rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.1/.coveragerc
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.1/tox.ini
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/__about__.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/__init__.py
+-rwxr-xr-x   0        0        0    26633 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/caller.py
+-rwxr-xr-x   0        0        0    10964 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/core.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/exceptions.py
+-rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/mapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/py.typed
+-rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/results.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/__init__.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/commons.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/enums.py
+-rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/requests.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.1/src/pytmv1/model/responses.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.1/.gitignore
+-rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.1/LICENSE.txt
+-rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.1/README.md
+-rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.1/PKG-INFO
```

### Comparing `pytmv1-0.5.0/src/pytmv1/__init__.py` & `pytmv1-0.5.1/src/pytmv1/__init__.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/src/pytmv1/caller.py` & `pytmv1-0.5.1/src/pytmv1/caller.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from functools import lru_cache
 from logging import Logger
 from typing import Callable, Optional, Type, Union
 
 from . import utils
-from .core import DEFAULT_POLL_TIME, Core
+from .core import Core
 from .model.commons import (
     Endpoint,
     ExceptionObject,
     SaeAlert,
     SuspiciousObject,
     TiAlert,
 )
@@ -52,35 +52,51 @@
 
 def client(
     name: str,
     token: str,
     url: str,
     pool_connections: int = 1,
     pool_maxsize: int = 1,
+    connect_timeout: int = 30,
+    read_timeout: int = 30,
 ) -> Client:
     """Helper function to initialize a :class:`Client`.
 
     :param name: Identify the application using this library.
     :type name: str
     :param token: Authentication token created for your account.
     :type token: str
     :param url: Vision One API url this client connects to.
     :type url: str
-    :param pool_connections: Number of connection pools to cache.
+    :param pool_connections: (optional) Number of connection to cache.
     :type pool_connections: int
-    :param pool_maxsize: Maximum size of the pool.
+    :param pool_maxsize: (optional) Maximum size of the pool.
     :type pool_maxsize: int
+    :param connect_timeout: (optional) Seconds before connection timeout.
+    :type connect_timeout: int
+    :param read_timeout: (optional) Seconds before read timeout.
+    :type connect_timeout: int
     :rtype: Client
     """
     log.debug(
         "Initializing new client with [Appname=%s, Token=*****, URL=%s]",
         name,
         url,
     )
-    return Client(Core(name, token, url, pool_connections, pool_maxsize))
+    return Client(
+        Core(
+            name,
+            token,
+            url,
+            pool_connections,
+            pool_maxsize,
+            connect_timeout,
+            read_timeout,
+        )
+    )
 
 
 @lru_cache(maxsize=None)
 class Client:
     def __init__(self, core: Core):
         self._core = core
 
@@ -274,15 +290,15 @@
             ],
         )
 
     def download_sandbox_analysis_result(
         self,
         submit_id: str,
         poll: bool = True,
-        poll_time_sec: float = DEFAULT_POLL_TIME,
+        poll_time_sec: float = 1800,
     ) -> Result[BytesResp]:
         """Downloads the analysis results of the specified object as PDF.
 
         :param submit_id: Sandbox submission id.
         :type submit_id: str
         :param poll: If we should wait until the task is finished before
         to return the result.
@@ -300,15 +316,15 @@
             poll_time_sec,
         )
 
     def download_sandbox_investigation_package(
         self,
         submit_id: str,
         poll: bool = True,
-        poll_time_sec: float = DEFAULT_POLL_TIME,
+        poll_time_sec: float = 1800,
     ) -> Result[BytesResp]:
         """Downloads the Investigation Package of the specified object.
 
         :param submit_id: Sandbox submission id.
         :type submit_id: str
         :param poll: If we should wait until the task is finished before
         to return the result.
@@ -408,15 +424,15 @@
             ),
         )
 
     def get_base_task_result(
         self,
         task_id: str,
         poll: bool = True,
-        poll_time_sec: float = DEFAULT_POLL_TIME,
+        poll_time_sec: float = 1800,
     ) -> Result[BaseTaskResp]:
         """Retrieves the result of a response task.
 
         :param task_id: Task id.
         :type task_id: str
         :param poll: If we should wait until the task is finished before
          to return the result.
@@ -455,15 +471,15 @@
         """
         return self._core.send(GetExceptionListResp, Api.GET_EXCEPTION_LIST)
 
     def get_sandbox_analysis_result(
         self,
         submit_id: str,
         poll: bool = True,
-        poll_time_sec: float = DEFAULT_POLL_TIME,
+        poll_time_sec: float = 1800,
     ) -> Result[SandboxAnalysisResultResp]:
         """Retrieves the analysis results of the specified object.
 
         :param submit_id: Sandbox submission id.
         :type submit_id: str
         :param poll: If we should wait until the task is finished before
          to return the result.
@@ -495,15 +511,15 @@
             Api.GET_SANDBOX_SUBMISSION_STATUS.value.format(submit_id),
         )
 
     def get_sandbox_suspicious_list(
         self,
         submit_id: str,
         poll: bool = True,
-        poll_time_sec: float = DEFAULT_POLL_TIME,
+        poll_time_sec: float = 1800,
     ) -> Result[SandboxSuspiciousListResp]:
         """Retrieves the suspicious object list associated to the
         specified object.
 
         :param submit_id: Sandbox submission id.
         :type submit_id: str
         :param poll: If we should wait until the task is finished before
@@ -532,15 +548,15 @@
         return self._core.send(GetSuspiciousListResp, Api.GET_SUSPICIOUS_LIST)
 
     def get_task_result(
         self,
         task_id: str,
         class_: Type[S],
         poll: bool = True,
-        poll_time_sec: float = DEFAULT_POLL_TIME,
+        poll_time_sec: float = 1800,
     ) -> Result[S]:
         """Retrieves the result of a response task.
 
         :param task_id: Task id.
         :type task_id: str
         :param class_: Expected task result class.
         :type class_: Type[S]
```

### Comparing `pytmv1-0.5.0/src/pytmv1/core.py` & `pytmv1-0.5.1/src/pytmv1/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,31 +45,32 @@
     S,
     SandboxSubmissionStatusResp,
 )
 from .results import multi_result, result
 
 USERAGENT_SUFFIX: str = "PyTMV1"
 API_VERSION: str = "v3.0"
-DEFAULT_POLL_TIME: float = 1800
-CONNECT_TIMEOUT: int = 5
-READ_TIMEOUT: int = 30
 
 log: Logger = logging.getLogger(__name__)
 
 
 class Core:
     def __init__(
         self,
         appname: str,
         token: str,
         url: str,
         pool_connections: int,
         pool_maxsize: int,
+        connect_timeout: int,
+        read_timeout: int,
     ):
         self._adapter = HTTPAdapter(pool_connections, pool_maxsize, 0, True)
+        self._c_timeout = connect_timeout
+        self._r_timeout = read_timeout
         self._appname = appname
         self._token = token
         self._url = parse_obj_as(AnyHttpUrl, _format(url))
         self._headers: Dict[str, str] = {
             "Authorization": f"Bearer {self._token}",
             "User-Agent": f"{self._appname}-{USERAGENT_SUFFIX}/{__version__}",
         }
@@ -242,15 +243,15 @@
             (
                 request.body.decode("utf-8")
                 if type(request.body) == bytes
                 else request.body
             ),
         )
         response: Response = self._adapter.send(
-            request, stream=False, timeout=(CONNECT_TIMEOUT, READ_TIMEOUT)
+            request, timeout=(self._c_timeout, self._r_timeout)
         )
         log.info(
             "Received response [Status=%s, Headers=%s, Body=%s]",
             response.status_code,
             response.headers,
             _hide_binary(response),
         )
```

### Comparing `pytmv1-0.5.0/src/pytmv1/exceptions.py` & `pytmv1-0.5.1/src/pytmv1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/src/pytmv1/mapper.py` & `pytmv1-0.5.1/src/pytmv1/mapper.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/src/pytmv1/results.py` & `pytmv1-0.5.1/src/pytmv1/results.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/src/pytmv1/utils.py` & `pytmv1-0.5.1/src/pytmv1/utils.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/src/pytmv1/model/commons.py` & `pytmv1-0.5.1/src/pytmv1/model/commons.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/src/pytmv1/model/enums.py` & `pytmv1-0.5.1/src/pytmv1/model/enums.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/src/pytmv1/model/requests.py` & `pytmv1-0.5.1/src/pytmv1/model/requests.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/src/pytmv1/model/responses.py` & `pytmv1-0.5.1/src/pytmv1/model/responses.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/LICENSE.txt` & `pytmv1-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/README.md` & `pytmv1-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/pyproject.toml` & `pytmv1-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytmv1-0.5.0/PKG-INFO` & `pytmv1-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmv1
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python library for Trend Micro Vision One
 Project-URL: Source, https://github.com/TrendATI/pytmv1
 Project-URL: Issues, https://github.com/TrendATI/pytmv1/issues
 Author-email: Thomas Legros <thomas_legros@trendmicro.com>
 Maintainer-email: TrendATI <ati-integration@trendmicro.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

