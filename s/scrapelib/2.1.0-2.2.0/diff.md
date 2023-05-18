# Comparing `tmp/scrapelib-2.1.0.tar.gz` & `tmp/scrapelib-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapelib-2.1.0.tar", max compression
+gzip compressed data, was "scrapelib-2.2.0.tar", max compression
```

## Comparing `scrapelib-2.1.0.tar` & `scrapelib-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1349 2020-02-05 22:39:56.366411 scrapelib-2.1.0/LICENSE
--rw-r--r--   0        0        0     1719 2021-11-09 22:16:39.970513 scrapelib-2.1.0/README.md
--rw-r--r--   0        0        0     1184 2022-11-07 01:01:29.483849 scrapelib-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    22081 2022-11-07 01:01:53.194461 scrapelib-2.1.0/scrapelib/__init__.py
--rw-r--r--   0        0        0     1586 2021-04-09 16:38:34.506709 scrapelib-2.1.0/scrapelib/__main__.py
--rw-r--r--   0        0        0      755 2021-04-09 16:38:34.507304 scrapelib-2.1.0/scrapelib/_types.py
--rw-r--r--   0        0        0     7802 2021-04-09 16:38:34.508033 scrapelib-2.1.0/scrapelib/cache.py
--rw-r--r--   0        0        0        0 2021-04-09 18:20:01.398445 scrapelib-2.1.0/scrapelib/py.typed
--rw-r--r--   0        0        0        0 2020-02-05 22:39:56.368706 scrapelib-2.1.0/scrapelib/tests/__init__.py
--rw-r--r--   0        0        0     3487 2021-04-09 16:38:34.508685 scrapelib-2.1.0/scrapelib/tests/test_cache.py
--rw-r--r--   0        0        0    14478 2022-11-07 00:56:10.455778 scrapelib-2.1.0/scrapelib/tests/test_scraper.py
--rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 scrapelib-2.1.0/setup.py
--rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 scrapelib-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1349 2023-05-18 16:50:02.270516 scrapelib-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1716 2023-05-18 16:50:02.270596 scrapelib-2.2.0/README.md
+-rw-r--r--   0        0        0     1247 2023-05-18 21:44:59.424737 scrapelib-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    22174 2023-05-18 21:44:47.192007 scrapelib-2.2.0/scrapelib/__init__.py
+-rw-r--r--   0        0        0     1586 2023-05-18 16:50:02.271542 scrapelib-2.2.0/scrapelib/__main__.py
+-rw-r--r--   0        0        0      836 2023-05-18 16:50:02.271604 scrapelib-2.2.0/scrapelib/_types.py
+-rw-r--r--   0        0        0     7803 2023-05-18 16:50:02.271690 scrapelib-2.2.0/scrapelib/cache.py
+-rw-r--r--   0        0        0        0 2023-05-18 16:50:02.271718 scrapelib-2.2.0/scrapelib/py.typed
+-rw-r--r--   0        0        0        0 2023-05-18 16:50:02.271795 scrapelib-2.2.0/scrapelib/tests/__init__.py
+-rw-r--r--   0        0        0     3487 2023-05-18 16:50:02.271900 scrapelib-2.2.0/scrapelib/tests/test_cache.py
+-rw-r--r--   0        0        0    14479 2023-05-18 16:50:02.272001 scrapelib-2.2.0/scrapelib/tests/test_scraper.py
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 scrapelib-2.2.0/PKG-INFO
```

### Comparing `scrapelib-2.1.0/LICENSE` & `scrapelib-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapelib-2.1.0/README.md` & `scrapelib-2.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Source: [https://github.com/jamesturk/scrapelib](https://github.com/jamesturk/scrapelib)
 
 Documentation: [https://jamesturk.github.io/scrapelib/](https://jamesturk.github.io/scrapelib/)
 
 Issues: [https://github.com/jamesturk/scrapelib/issues](https://github.com/jamesturk/scrapelib/issues)
 
 [![PyPI badge](https://badge.fury.io/py/scrapelib.svg)](https://badge.fury.io/py/scrapelib)
-[![Test badge](https://github.com/jamesturk/scrapelib/workflows/Test/badge.svg)](https://github.com/jamesturk/scrapelib/actions?query=workflow%3A%22Test)
+[![Test badge](https://github.com/jamesturk/scrapelib/workflows/Test/badge.svg)](https://github.com/jamesturk/scrapelib/actions?query=workflow%3ATest)
 
 ## Features
 
 **scrapelib** originated as part of the [Open States](http://openstates.org/)
 project to scrape the websites of all 50 state legislatures and as a result
 was therefore designed with features desirable when dealing with sites that
 have intermittent errors or require rate-limiting.
```

### Comparing `scrapelib-2.1.0/pyproject.toml` & `scrapelib-2.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapelib"
-version = "2.1.0"
+version = "2.2.0"
 description = ""
 readme = "README.md"
 authors = ["James Turk <dev@jamesturk.net>"]
 license = "BSD-2-Clause"
 repository = "https://github.com/jamesturk/scrapelib"
 classifiers=[
   "Development Status :: 6 - Mature",
@@ -12,33 +12,35 @@
   "License :: OSI Approved :: BSD License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.scripts]
 scrapeshell = "scrapelib.__main__:scrapeshell"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = {extras = ["security"], version = "^2.28.1"}
+urllib3 = "^1.26"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.961"
 flake8 = "^3.9.0"
 mock = "^4.0.3"
 pytest = "^7.1.2"
 pytest-cov = "^2.11.1"
 coveralls = "^3.3.1"
-mkdocs-material = "^8.3.9"
+mkdocs-material = "^8.5.9"
 mkdocstrings = "0.19.0"
-types-requests = "^2.28.0"
+types-requests = "^2.28.11"
 types-mock = "^4.0.15"
 importlib-metadata = "<5.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `scrapelib-2.1.0/scrapelib/__init__.py` & `scrapelib-2.2.0/scrapelib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     RequestsCookieJar,
     _HooksInput,
     _AuthType,
     Response,
 )
 
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 _user_agent = " ".join(("scrapelib", __version__, requests.utils.default_user_agent()))
 
 
 _log = logging.getLogger("scrapelib")
 _log.addHandler(logging.NullHandler())
 
 
@@ -296,14 +296,18 @@
             resp.headers = requests.structures.CaseInsensitiveDict()
             resp._content = real_resp.read()
             resp.raw = _dummy
             return resp
         except URLError:
             raise FTPError(cast(str, request.url))
 
+    def close(self) -> None:
+        # needed to use session as context manager
+        ...
+
 
 # compose sessions, order matters (cache then throttle then retry)
 class CachingSession(ThrottledSession):
     def __init__(self, cache_storage: Optional[CacheStorageBase] = None) -> None:
         super().__init__()
         self.cache_storage = cache_storage
         self.cache_write_only = False
```

### Comparing `scrapelib-2.1.0/scrapelib/__main__.py` & `scrapelib-2.2.0/scrapelib/__main__.py`

 * *Files identical despite different names*

### Comparing `scrapelib-2.1.0/scrapelib/_types.py` & `scrapelib-2.2.0/scrapelib/_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,25 +6,26 @@
     Mapping,
     Text,
     Callable,
     List,
     MutableMapping,
     Iterable,
     Any,
-    IO,
 )
 
-_Data = Union[
-    None,
-    Text,
-    bytes,
-    Mapping[str, Any],
-    Mapping[Text, Any],
-    Iterable[Tuple[Text, Optional[Text]]],
-    IO,
+_Data = Optional[
+    Union[
+        Iterable[bytes],
+        str,
+        bytes,
+        #        SupportsRead[Union[str, bytes]],
+        List[Tuple[Any, Any]],
+        Tuple[Tuple[Any, Any], ...],
+        Mapping[Any, Any],
+    ]
 ]
 
 
 RequestsCookieJar = requests.cookies.RequestsCookieJar
 Response = requests.models.Response
 Request = requests.models.Request
 PreparedRequest = requests.models.PreparedRequest
```

### Comparing `scrapelib-2.1.0/scrapelib/cache.py` & `scrapelib-2.2.0/scrapelib/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                         "last-modified", line, flags=re.I
                     ):
                         # line contains last modified header
                         head_resp = requests.head(orig_key)
 
                         try:
                             new_lm = head_resp.headers["last-modified"]
-                            old_lm = line[line.find(":") + 1:].strip()
+                            old_lm = line[line.find(":") + 1 :].strip()
                             if old_lm != new_lm:
                                 # last modified timestamps don't match, need to download again
                                 return None
                         except KeyError:
                             # no last modified header present, so redownload
                             return None
```

### Comparing `scrapelib-2.1.0/scrapelib/tests/test_cache.py` & `scrapelib-2.2.0/scrapelib/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `scrapelib-2.1.0/scrapelib/tests/test_scraper.py` & `scrapelib-2.2.0/scrapelib/tests/test_scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
         raise URLError("ftp failure!")
 
     mock_urlopen = mock.Mock(side_effect=side_effect)
 
     # retry on
     with mock.patch("scrapelib.urllib_urlopen", mock_urlopen):
         s = Scraper(retry_attempts=2, retry_wait_seconds=0.001)
-        r = s.get("ftp://dummy/", retry_on_404=True) # type: ignore
+        r = s.get("ftp://dummy/", retry_on_404=True)  # type: ignore
         assert r.content == b"ftp success!"
     assert mock_urlopen.call_count == 2
 
     # retry off, retry_on_404 on (shouldn't matter)
     count = []
     mock_urlopen.reset_mock()
     with mock.patch("scrapelib.urllib_urlopen", mock_urlopen):
```

### Comparing `scrapelib-2.1.0/PKG-INFO` & `scrapelib-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapelib
-Version: 2.1.0
+Version: 2.2.0
 Summary: 
 Home-page: https://github.com/jamesturk/scrapelib
 License: BSD-2-Clause
 Author: James Turk
 Author-email: dev@jamesturk.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 6 - Mature
@@ -15,32 +15,34 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: requests[security] (>=2.28.1,<3.0.0)
+Requires-Dist: urllib3 (>=1.26,<2.0)
 Project-URL: Repository, https://github.com/jamesturk/scrapelib
 Description-Content-Type: text/markdown
 
 **scrapelib** is a library for making requests to less-than-reliable websites.
 
 Source: [https://github.com/jamesturk/scrapelib](https://github.com/jamesturk/scrapelib)
 
 Documentation: [https://jamesturk.github.io/scrapelib/](https://jamesturk.github.io/scrapelib/)
 
 Issues: [https://github.com/jamesturk/scrapelib/issues](https://github.com/jamesturk/scrapelib/issues)
 
 [![PyPI badge](https://badge.fury.io/py/scrapelib.svg)](https://badge.fury.io/py/scrapelib)
-[![Test badge](https://github.com/jamesturk/scrapelib/workflows/Test/badge.svg)](https://github.com/jamesturk/scrapelib/actions?query=workflow%3A%22Test)
+[![Test badge](https://github.com/jamesturk/scrapelib/workflows/Test/badge.svg)](https://github.com/jamesturk/scrapelib/actions?query=workflow%3ATest)
 
 ## Features
 
 **scrapelib** originated as part of the [Open States](http://openstates.org/)
 project to scrape the websites of all 50 state legislatures and as a result
 was therefore designed with features desirable when dealing with sites that
 have intermittent errors or require rate-limiting.
```

