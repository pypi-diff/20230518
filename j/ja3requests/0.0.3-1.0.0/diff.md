# Comparing `tmp/ja3requests-0.0.3.tar.gz` & `tmp/ja3requests-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja3requests-0.0.3.tar", last modified: Fri May 12 09:34:27 2023, max compression
+gzip compressed data, was "ja3requests-1.0.0.tar", last modified: Thu May 18 09:59:47 2023, max compression
```

## Comparing `ja3requests-0.0.3.tar` & `ja3requests-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-12 09:34:27.260316 ja3requests-0.0.3/
--rw-r--r--   0 pledgebox   (501) staff       (20)    11357 2023-04-25 06:02:38.000000 ja3requests-0.0.3/LICENSE
--rw-r--r--   0 pledgebox   (501) staff       (20)      444 2023-05-12 09:34:27.259991 ja3requests-0.0.3/PKG-INFO
--rw-r--r--   0 pledgebox   (501) staff       (20)       75 2023-04-25 06:02:38.000000 ja3requests-0.0.3/README.md
-drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-12 09:34:27.256071 ja3requests-0.0.3/ja3requests/
--rw-r--r--   0 pledgebox   (501) staff       (20)        0 2023-04-26 10:28:27.000000 ja3requests-0.0.3/ja3requests/__init__.py
--rw-r--r--   0 pledgebox   (501) staff       (20)      395 2023-05-12 09:33:43.000000 ja3requests-0.0.3/ja3requests/__version__.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     4320 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/connections.py
--rw-r--r--   0 pledgebox   (501) staff       (20)      665 2023-04-26 10:28:27.000000 ja3requests-0.0.3/ja3requests/const.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     1223 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/context.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     1537 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/exceptions.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     6651 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/request.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     3176 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/response.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     4596 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/sessions.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     2118 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/utils.py
-drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-12 09:34:27.257839 ja3requests-0.0.3/ja3requests.egg-info/
--rw-r--r--   0 pledgebox   (501) staff       (20)      444 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/PKG-INFO
--rw-r--r--   0 pledgebox   (501) staff       (20)      522 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/SOURCES.txt
--rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/dependency_links.txt
--rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/not-zip-safe
--rw-r--r--   0 pledgebox   (501) staff       (20)       12 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/top_level.txt
--rw-r--r--   0 pledgebox   (501) staff       (20)      640 2023-04-26 10:28:27.000000 ja3requests-0.0.3/pyproject.toml
--rw-r--r--   0 pledgebox   (501) staff       (20)       38 2023-05-12 09:34:27.260406 ja3requests-0.0.3/setup.cfg
--rw-r--r--   0 pledgebox   (501) staff       (20)     1890 2023-04-26 10:28:27.000000 ja3requests-0.0.3/setup.py
-drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-12 09:34:27.259137 ja3requests-0.0.3/test/
--rw-r--r--   0 pledgebox   (501) staff       (20)      431 2023-05-11 09:18:14.000000 ja3requests-0.0.3/test/test_ready_request.py
--rw-r--r--   0 pledgebox   (501) staff       (20)      310 2023-05-12 09:33:31.000000 ja3requests-0.0.3/test/test_session.py
--rw-r--r--   0 pledgebox   (501) staff       (20)      244 2023-04-26 10:28:27.000000 ja3requests-0.0.3/test/test_utils.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-18 09:59:47.021001 ja3requests-1.0.0/
+-rw-r--r--   0 pledgebox   (501) staff       (20)    11357 2023-04-25 06:02:38.000000 ja3requests-1.0.0/LICENSE
+-rw-r--r--   0 pledgebox   (501) staff       (20)      446 2023-05-18 09:59:47.020654 ja3requests-1.0.0/PKG-INFO
+-rw-r--r--   0 pledgebox   (501) staff       (20)       77 2023-05-18 09:57:19.000000 ja3requests-1.0.0/README.md
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-18 09:59:47.015693 ja3requests-1.0.0/ja3requests/
+-rw-r--r--   0 pledgebox   (501) staff       (20)        0 2023-04-26 10:28:27.000000 ja3requests-1.0.0/ja3requests/__init__.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      395 2023-05-18 09:58:19.000000 ja3requests-1.0.0/ja3requests/__version__.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     4199 2023-05-18 09:57:19.000000 ja3requests-1.0.0/ja3requests/connections.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      878 2023-05-18 09:57:19.000000 ja3requests-1.0.0/ja3requests/const.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     1417 2023-05-18 09:57:19.000000 ja3requests-1.0.0/ja3requests/context.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     1648 2023-05-18 09:57:19.000000 ja3requests-1.0.0/ja3requests/exceptions.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     7055 2023-05-18 09:57:19.000000 ja3requests-1.0.0/ja3requests/request.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     6718 2023-05-18 09:57:19.000000 ja3requests-1.0.0/ja3requests/response.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     4483 2023-05-18 09:57:19.000000 ja3requests-1.0.0/ja3requests/sessions.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     2118 2023-05-12 09:33:31.000000 ja3requests-1.0.0/ja3requests/utils.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-18 09:59:47.017792 ja3requests-1.0.0/ja3requests.egg-info/
+-rw-r--r--   0 pledgebox   (501) staff       (20)      446 2023-05-18 09:59:46.000000 ja3requests-1.0.0/ja3requests.egg-info/PKG-INFO
+-rw-r--r--   0 pledgebox   (501) staff       (20)      522 2023-05-18 09:59:46.000000 ja3requests-1.0.0/ja3requests.egg-info/SOURCES.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-18 09:59:46.000000 ja3requests-1.0.0/ja3requests.egg-info/dependency_links.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-18 09:59:46.000000 ja3requests-1.0.0/ja3requests.egg-info/not-zip-safe
+-rw-r--r--   0 pledgebox   (501) staff       (20)       12 2023-05-18 09:59:46.000000 ja3requests-1.0.0/ja3requests.egg-info/top_level.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)      640 2023-04-26 10:28:27.000000 ja3requests-1.0.0/pyproject.toml
+-rw-r--r--   0 pledgebox   (501) staff       (20)       38 2023-05-18 09:59:47.021084 ja3requests-1.0.0/setup.cfg
+-rw-r--r--   0 pledgebox   (501) staff       (20)     1890 2023-04-26 10:28:27.000000 ja3requests-1.0.0/setup.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-18 09:59:47.019910 ja3requests-1.0.0/test/
+-rw-r--r--   0 pledgebox   (501) staff       (20)      431 2023-05-11 09:18:14.000000 ja3requests-1.0.0/test/test_ready_request.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      310 2023-05-12 09:33:31.000000 ja3requests-1.0.0/test/test_session.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      244 2023-04-26 10:28:27.000000 ja3requests-1.0.0/test/test_utils.py
```

### Comparing `ja3requests-0.0.3/LICENSE` & `ja3requests-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.3/ja3requests/const.py` & `ja3requests-1.0.0/ja3requests/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,10 +27,17 @@
             raise self.ConstCaseError(f"{key}-constants need to be capitalized.")
 
         self.__dict__[key] = value
 
 
 const = _Const()
 
+const.MAX_LINE = 65536
+const.MAX_HEADERS = 100
+const.DEFAULT_CHUNKED_SIZE = 2048
+const.DEFAULT_HTTP_SCHEME = "http"
+const.DEFAULT_HTTPS_SCHEME = "https"
+const.DEFAULT_HTTP_PORT = 80
+const.DEFAULT_HTTPS_PORT = 443
 const.DEFAULT_REDIRECT_LIMIT = 8  # max redirect
 
 sys.modules[__name__] = const
```

### Comparing `ja3requests-0.0.3/ja3requests/context.py` & `ja3requests-1.0.0/ja3requests/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,45 +10,51 @@
 
 
 DEFAULT_HTTP_CONTEXT_PROTOCOL = 11
 DEFAULT_HTTP_VERSION = "HTTP/1.1"
 
 
 class HTTPContext(BaseContext):
+    """
+    HTTPContext
+    """
 
     def __init__(self, connection):
-
         super().__init__()
         self.protocol = DEFAULT_HTTP_CONTEXT_PROTOCOL
         self.version = DEFAULT_HTTP_VERSION
         self.connection = connection
 
     @property
     def message(self):
-        self.start_line = " ".join(
-            [self.method, self.connection.path, self.version]
-        )
-        self._message = "\r\n".join(
-            [self.start_line, self.put_headers()]
-        )
+        """
+        HTTP Context message to send
+        :return:
+        """
+        self.start_line = " ".join([self.method, self.connection.path, self.version])
+        self._message = "\r\n".join([self.start_line, self.put_headers()])
         self._message += "\r\n\r\n"
 
         return self._message.encode()
 
-    def set_payload(
-            self,
-            **kwargs
-    ):
-
+    def set_payload(self, **kwargs):
+        """
+        Set context payload
+        :param kwargs:
+        :return:
+        """
         for k, v in kwargs.items():
             if hasattr(self, k):
                 setattr(self, k, v)
 
     def put_headers(self):
-
+        """
+        Set context headers
+        :return:
+        """
         headers = ""
         if self.headers is not None:
             if not self.headers.get("host", None):
                 self.headers["host"] = self.connection.host
 
             headers = "\r\n".join([f"{k}: {v}" for k, v in self.headers.items()])
```

### Comparing `ja3requests-0.0.3/ja3requests/exceptions.py` & `ja3requests-1.0.0/ja3requests/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -58,8 +58,14 @@
     Raised it when can't receive streamline.
     """
 
 
 class InvalidResponseHeaders(RequestException, ValueError):
     """
     Raised it when cant receive response headers.
-    """
+    """
+
+
+class IssueError(ValueError):
+    """
+    This situation may not be considered yet, please issue it
+    """
```

### Comparing `ja3requests-0.0.3/ja3requests/request.py` & `ja3requests-1.0.0/ja3requests/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 """
 ja3requests.request
 ~~~~~~~~~~~~~~~~~~~
 
 This module create a request struct and ready request object.
 """
-from .base import BaseRequest
-from .utils import default_headers
-from .context import HTTPContext
-from .connections import HTTPConnection
-from .exceptions import NotAllowedRequestMethod, MissingScheme, NotAllowedScheme, InvalidParams
+
+
 import warnings
 from http.cookiejar import CookieJar
 from urllib.parse import urlparse, urlencode
 from typing import Any, AnyStr, Dict, List, Union, ByteString, Tuple
+from .base import BaseRequest
+from .utils import default_headers
+from .context import HTTPContext
+from .connections import HTTPConnection
+from .exceptions import (
+    NotAllowedRequestMethod,
+    MissingScheme,
+    NotAllowedScheme,
+    InvalidParams,
+)
 
 
 class ReadyRequest(BaseRequest):
+    """
+    Ready a request, e.g.(check url, check params)
+    """
 
     def __init__(
-            self,
-            method: AnyStr,
-            url: AnyStr,
-            params: Union[Dict[Any, Any], List[Tuple[Any, Any]], Tuple[Tuple[Any, Any]], ByteString, AnyStr] = None,
-            data: Union[Dict[AnyStr, Any], List, Tuple, ByteString] = None,
-            headers: Dict[AnyStr, AnyStr] = None,
-            cookies: Union[Dict[AnyStr, AnyStr], CookieJar] = None,
-            auth: Tuple = None,
-            json: Dict[AnyStr, AnyStr] = None,
+        self,
+        method: AnyStr,
+        url: AnyStr,
+        params: Union[
+            Dict[Any, Any],
+            List[Tuple[Any, Any]],
+            Tuple[Tuple[Any, Any]],
+            ByteString,
+            AnyStr,
+        ] = None,
+        data: Union[Dict[AnyStr, Any], List, Tuple, ByteString] = None,
+        headers: Dict[AnyStr, AnyStr] = None,
+        cookies: Union[Dict[AnyStr, AnyStr], CookieJar] = None,
+        auth: Tuple = None,
+        json: Dict[AnyStr, AnyStr] = None,
     ):
         super().__init__()
         self.method = method
         self.url = url
         self.params = params
         self.data = data
         self.headers = headers
@@ -79,17 +95,15 @@
             raise MissingScheme(
                 f"Invalid URL {self.url!r}: No scheme supplied. "
                 f"Perhaps you meant http://{self.url} or https://{self.url}"
             )
 
         # Just allow http or https
         if parse.scheme not in ["http", "https"]:
-            raise NotAllowedScheme(
-                f"Schema: {parse.scheme} not allowed."
-            )
+            raise NotAllowedScheme(f"Schema: {parse.scheme} not allowed.")
 
         self.scheme = parse.scheme
         if self.scheme == "https":
             self.port = 443
 
         if parse.netloc != "" and ":" in parse.netloc:
             port = parse.netloc.split(":")[-1]
@@ -140,15 +154,18 @@
 
         # Check duplicate default item
         new_headers = {}
         header_list = []
         for k, v in self.headers.items():
             header = k.lower()
             if header in header_list:
-                warnings.warn(f"Duplicate header: {k}, you should check the request headers.", RuntimeWarning)
+                warnings.warn(
+                    f"Duplicate header: {k}, you should check the request headers.",
+                    RuntimeWarning,
+                )
 
             header_list.append(header)
             new_headers[header] = v
 
         self.headers = new_headers
         del new_headers
         del header_list
@@ -182,28 +199,38 @@
         self.ready_data()
         self.ready_headers()
         self.ready_cookies()
         self.ready_auth()
         self.ready_json()
 
     def request(self):
-
+        """
+        Create a Request object.
+        :return:
+        """
         req = Request()
         req.clone(self)
 
         return req
 
 
 class Request(BaseRequest):
+    """
+    Request object to send.
+    """
 
     def __repr__(self):
         return f"<Request [{self.method}]>"
 
     def clone(self, ready_request: ReadyRequest):
-
+        """
+        Clone arguments from ReadyRequest
+        :param ready_request:
+        :return:
+        """
         for k, v in ready_request.__dict__.items():
             setattr(self, k, v)
 
     def send(self):
         """
         Connection sending.
         :return:
@@ -215,15 +242,15 @@
             self.scheme,
             self.port,
             self.source,
             self.url,
             self.timeout,
             proxy,
             proxy_username,
-            proxy_password
+            proxy_password,
         )
         context = HTTPContext(conn)
         context.set_payload(
             method=self.method,
             headers=self.headers,
         )
         response = conn.send(context)
@@ -237,17 +264,19 @@
         """
 
         if self.is_http():
             conn = HTTPConnection()
         elif self.is_https():
             # TODO: HTTPS
             # conn = HTTPSConnection()
-            raise NotImplementedError("HTTPSConnection not implemented yet.")
+            raise NotImplementedError("HTTPS not implemented yet.")
         else:
-            raise MissingScheme(f"Scheme: {self.scheme}, parse scheme failed, can't create connection.")
+            raise MissingScheme(
+                f"Scheme: {self.scheme}, parse scheme failed, can't create connection."
+            )
 
         return conn
 
     def parse_proxies(self):
         """
         TODO
         Parse proxy, proxy's username and password. if proxies is set.
```

### Comparing `ja3requests-0.0.3/ja3requests/sessions.py` & `ja3requests-1.0.0/ja3requests/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,15 @@
 
     def __init__(self):
         super().__init__()
 
         self.headers = default_headers()
         self.max_redirects = DEFAULT_REDIRECT_LIMIT
 
-    def ready(
-            self,
-            method,
-            url,
-            params,
-            data,
-            headers,
-            cookies,
-            auth,
-            json
-    ):
+    def ready(self, method, url, params, data, headers, cookies, auth, json):
         """
         Ready to send request.
         :return:
         """
 
         req = ReadyRequest(
             method=method,
@@ -98,15 +88,15 @@
             method=method,
             url=url,
             params=params,
             data=data,
             headers=headers,
             cookies=cookies,
             auth=auth,
-            json=json
+            json=json,
         )
 
         req = ready_request.request()
         response = self.send(req)
 
         return response
```

### Comparing `ja3requests-0.0.3/ja3requests/utils.py` & `ja3requests-1.0.0/ja3requests/utils.py`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.3/ja3requests.egg-info/SOURCES.txt` & `ja3requests-1.0.0/ja3requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.3/pyproject.toml` & `ja3requests-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.3/setup.py` & `ja3requests-1.0.0/setup.py`

 * *Files identical despite different names*

