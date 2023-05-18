# Comparing `tmp/hollihop_api_client-0.0.1.tar.gz` & `tmp/hollihop_api_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hollihop_api_client-0.0.1.tar", last modified: Sat Jan 28 16:02:32 2023, max compression
+gzip compressed data, was "hollihop_api_client-0.0.2.tar", last modified: Thu May 18 11:10:30 2023, max compression
```

## Comparing `hollihop_api_client-0.0.1.tar` & `hollihop_api_client-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/
--rw-rw-r--   0 oem      (29999) oem      (29999)     1070 2023-01-28 12:01:18.000000 hollihop_api_client-0.0.1/LICENSE
--rw-rw-r--   0 oem      (29999) oem      (29999)     2391 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/PKG-INFO
--rw-r--r--   0 oem      (29999) oem      (29999)     1741 2023-01-28 15:30:55.000000 hollihop_api_client-0.0.1/README.md
--rw-rw-r--   0 oem      (29999) oem      (29999)      742 2023-01-28 14:19:23.000000 hollihop_api_client-0.0.1/pyproject.toml
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/setup.cfg
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/src/
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/src/hollihop_api_client/
--rwxr-xr-x   0 oem      (29999) oem      (29999)       71 2023-01-28 13:49:14.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/__init__.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/src/hollihop_api_client/api/
--rw-r--r--   0 oem      (29999) oem      (29999)      114 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/api/__init__.py
--rwxr-xr-x   0 oem      (29999) oem      (29999)      596 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/api/abc.py
--rwxr-xr-x   0 oem      (29999) oem      (29999)     2637 2023-01-28 14:17:33.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/api/api.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/src/hollihop_api_client/base/
--rw-r--r--   0 oem      (29999) oem      (29999)       63 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/base/__init__.py
--rw-r--r--   0 oem      (29999) oem      (29999)      540 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/base/category.py
--rw-r--r--   0 oem      (29999) oem      (29999)      935 2023-01-28 15:28:20.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/categories.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/src/hollihop_api_client/methods/
--rw-r--r--   0 oem      (29999) oem      (29999)        0 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/methods/__init__.py
--rw-r--r--   0 oem      (29999) oem      (29999)     6426 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/methods/ed_unit_student.py
--rw-r--r--   0 oem      (29999) oem      (29999)     2699 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/methods/ed_units.py
--rw-r--r--   0 oem      (29999) oem      (29999)     2154 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/methods/leads.py
--rw-r--r--   0 oem      (29999) oem      (29999)     1232 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/methods/locations.py
--rw-r--r--   0 oem      (29999) oem      (29999)     1506 2023-01-28 11:52:49.000000 hollihop_api_client-0.0.1/src/hollihop_api_client/methods/offices.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-01-28 16:02:32.540438 hollihop_api_client-0.0.1/src/hollihop_api_client.egg-info/
--rw-rw-r--   0 oem      (29999) oem      (29999)     2391 2023-01-28 16:02:32.000000 hollihop_api_client-0.0.1/src/hollihop_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)      754 2023-01-28 16:02:32.000000 hollihop_api_client-0.0.1/src/hollihop_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-01-28 16:02:32.000000 hollihop_api_client-0.0.1/src/hollihop_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       20 2023-01-28 16:02:32.000000 hollihop_api_client-0.0.1/src/hollihop_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.638727 hollihop_api_client-0.0.2/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1073 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/LICENSE
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-18 11:10:30.638605 hollihop_api_client-0.0.2/PKG-INFO
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1753 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/README.md
+-rw-r--r--   0 malts.tech   (501) staff       (20)      716 2023-05-18 11:10:16.000000 hollihop_api_client-0.0.2/pyproject.toml
+-rw-r--r--   0 malts.tech   (501) staff       (20)       38 2023-05-18 11:10:30.638760 hollihop_api_client-0.0.2/setup.cfg
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.633410 hollihop_api_client-0.0.2/src/
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.634604 hollihop_api_client-0.0.2/src/hollihop_api_client/
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.635656 hollihop_api_client-0.0.2/src/hollihop_api_client/api/
+-rw-r--r--   0 malts.tech   (501) staff       (20)      138 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/api/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      594 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/api/abc.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2687 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/api/api.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.635971 hollihop_api_client-0.0.2/src/hollihop_api_client/base/
+-rw-r--r--   0 malts.tech   (501) staff       (20)       63 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/base/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      520 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/base/category.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      933 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/categories.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.636742 hollihop_api_client-0.0.2/src/hollihop_api_client/methods/
+-rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/methods/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     6766 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/methods/ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     6434 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/methods/ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2765 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/methods/leads.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1303 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/methods/locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1611 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/methods/offices.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1436 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/test.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.638221 hollihop_api_client-0.0.2/src/hollihop_api_client/tests/
+-rw-r--r--   0 malts.tech   (501) staff       (20)        0 2023-03-11 10:01:33.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/tests/__init__.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1528 2023-03-12 11:14:09.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/tests/conftest.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      474 2023-03-12 18:14:57.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/tests/test_ed_unit_students.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      995 2023-03-12 11:19:09.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/tests/test_ed_units.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      165 2023-03-12 11:17:10.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/tests/test_lead.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      374 2023-03-12 11:16:33.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/tests/test_locations.py
+-rw-r--r--   0 malts.tech   (501) staff       (20)      636 2023-03-12 11:15:54.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/tests/test_offices.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.638430 hollihop_api_client-0.0.2/src/hollihop_api_client/tools/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     3143 2023-05-18 10:42:19.000000 hollihop_api_client-0.0.2/src/hollihop_api_client/tools/__init__.py
+drwxr-xr-x   0 malts.tech   (501) staff       (20)        0 2023-05-18 11:10:30.635167 hollihop_api_client-0.0.2/src/hollihop_api_client.egg-info/
+-rw-r--r--   0 malts.tech   (501) staff       (20)     2401 2023-05-18 11:10:30.000000 hollihop_api_client-0.0.2/src/hollihop_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 malts.tech   (501) staff       (20)     1116 2023-05-18 11:10:30.000000 hollihop_api_client-0.0.2/src/hollihop_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)        1 2023-05-18 11:10:30.000000 hollihop_api_client-0.0.2/src/hollihop_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 malts.tech   (501) staff       (20)       20 2023-05-18 11:10:30.000000 hollihop_api_client-0.0.2/src/hollihop_api_client.egg-info/top_level.txt
```

### Comparing `hollihop_api_client-0.0.1/PKG-INFO` & `hollihop_api_client-0.0.2/src/hollihop_api_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: hollihop_api_client
-Version: 0.0.1
-Summary: This library helps you easily create a python application with Hollihop API 
-Author-email: Nicholas Maltsev <nmmaltsev@outlook.com>
-Project-URL: Homepage, https://github.com/nicholasChieftain/hollyhope-api-client
-Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollyhope-api-client/issues
+Name: hollihop-api-client
+Version: 0.0.2
+Summary: This library helps you easily create a python application with Hollihop API
+Author-email: Nicholas Maltseb <nmmaltsev@outlook.com>
+Project-URL: Homepage, https://github.com/nicholasChieftain/hollihop_api_client/
+Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollihop_api_client/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,17 +24,17 @@
 ```
 
 ## Использование
 
 ### Инициализация
 
 ```python
-from hollihop_api_client import hhAPI
+from hollihop_api_client import HolliHopAPI
 
-hh_api = hhAPI(HH_DOMAIN, HH_COMMON_API_KEY)
+hh_api = HolliHopAPI(HH_DOMAIN, HH_COMMON_API_KEY)
 ```
 
 Обратите внимание, что ключи нужно получать из переменных среды:
 
 ```python
 from os import environ
```

### Comparing `hollihop_api_client-0.0.1/README.md` & `hollihop_api_client-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 ```
 
 ## Использование
 
 ### Инициализация
 
 ```python
-from hollihop_api_client import hhAPI
+from hollihop_api_client import HolliHopAPI
 
-hh_api = hhAPI(HH_DOMAIN, HH_COMMON_API_KEY)
+hh_api = HolliHopAPI(HH_DOMAIN, HH_COMMON_API_KEY)
 ```
 
 Обратите внимание, что ключи нужно получать из переменных среды:
 
 ```python
 from os import environ
```

### Comparing `hollihop_api_client-0.0.1/pyproject.toml` & `hollihop_api_client-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
-requires = ["setuptools", "requests", "phonenumbers"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hollihop_api_client"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Nicholas Maltsev", email="nmmaltsev@outlook.com" },
+  { name="Nicholas Maltseb", email="nmmaltsev@outlook.com" },
 ]
-description = "This library helps you easily create a python application with Hollihop API "
+description = "This library helps you easily create a python application with Hollihop API"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
-    "Operating System :: POSIX :: Linux",
+    "Operating System :: POSIX :: Linux"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/nicholasChieftain/hollyhope-api-client"
-"Bug Tracker" = "https://github.com/nicholasChieftain/hollyhope-api-client/issues"
-
+"Homepage" = "https://github.com/nicholasChieftain/hollihop_api_client/"
+"Bug Tracker" = "https://github.com/nicholasChieftain/hollihop_api_client/issues"
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client/api/abc.py` & `hollihop_api_client-0.0.2/src/hollihop_api_client/api/abc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import NoReturn, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from requests import Response
 
-from ..categories import APICategories
+from categories import APICategories
 
 
 class AbstractAPI(ABC, APICategories):
     @abstractmethod
     def request(
             self,
             method: str,
@@ -16,13 +16,13 @@
             data: None | dict = None,
             ) -> None | dict:
         pass
 
     @abstractmethod
     def _validate_response(
             self,
-            response: 'Response'
+            response: "Response"
             ) -> (None | dict) | NoReturn:
         pass
 
 
 __all__ = ['AbstractAPI']
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client/api/api.py` & `hollihop_api_client-0.0.2/src/hollihop_api_client/api/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from typing import NoReturn
+from typing import NoReturn, TYPE_CHECKING
 
 from requests import Response, Session, get
 
 from .abc import AbstractAPI
 
 
-class hhAPIError(Exception):
-    _respone_not_ok = '''Запрос к {url} не выполнен.
+class HolliHopAPIError(Exception):
+    _response_not_ok = '''Запрос к {url} не выполнен.
     Статус код {status_code}.
     {error_message}'''
     _other_errors = '''{error_message}'''
 
     def __init__(
             self,
             error_message: str,
-            status_code: None | str = None,
+            status_code: None | int = None,
             url: None | str = None
             ):
         self._status_code = status_code
         self._error_message = error_message
         self._url = url
 
     def __str__(self) -> str:
         if self._status_code is None:
-            return self._others_errors.format(
+            return self._other_errors.format(
                     error_message=self._error_message
                     )
         else:
-            return self._respone_not_ok.format(
+            return self._response_not_ok.format(
                     url=self._url,
                     status_code=self._status_code,
                     error_message=self._error_message
                 )
 
 
-class hhAPI(AbstractAPI):
+class HolliHopAPI(AbstractAPI):
     __api_version__ = 'Api/V2/'
 
     def __init__(
             self,
             domain: str = None,
             api_key: str = None
             ):
         if api_key is None:
-            raise hhAPIError(
+            raise HolliHopAPIError(
                     error_message='Не указан ключ доступа к API'
                     )
         if domain is None:
-            raise hhAPIError(
+            raise HolliHopAPIError(
                     error_message='Не указан домен для доступа к API'
                     )
         self._domain = domain
         self._api_key = api_key
 
         super().__init__(self)
 
@@ -65,27 +65,28 @@
         data.update({'authkey': self._api_key})
         with Session() as session:
             response = session.request(
                     method=http_method,
                     url=url,
                     data=data,
                     )
-        #response = get(url=url, data=data)
+
         response = self._validate_response(response)
 
         return response
 
     def _validate_response(
             self,
             response: Response,
             ) -> (None | dict) | NoReturn:
         if response.status_code == 200:
             return response.json()
         else:
-            raise hhAPIError(
+            print(response.json())
+            raise HolliHopAPIError(
                     response.url,
                     response.status_code,
                     'Ошибка выполнения запроса'
                     )
 
 
-__all__ = ['hhAPI', 'hhAPIError']
+__all__ = ['HolliHopAPI', 'HolliHopAPIError']
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client/base/category.py` & `hollihop_api_client-0.0.2/src/hollihop_api_client/base/category.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import pdb
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from ..api import AbstractAPI
+    from api import AbstractAPI
+
 
 class BaseCategory:
     def __init__(self, api: 'AbstractAPI'):
         self.api = api
 
     @classmethod
     def handle_parameters(cls, parameters: dict) -> dict:
         handled_parameters = parameters.copy()
 
         handled_parameters.pop('self')
-        
+
         for key, value in parameters.items():
             if value is None:
                 handled_parameters.pop(key)
         return handled_parameters
 
 
 __all__ = ['BaseCategory']
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client/categories.py` & `hollihop_api_client-0.0.2/src/hollihop_api_client/categories.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .methods import (
+from methods import (
         locations,
         offices,
         ed_units,
         ed_unit_students,
         leads,
         )
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from .api import AbstractAPI
+    from api import AbstractAPI
 
 
 class APICategories:
     def __init__(self, api: 'AbstractAPI'):
         self.api = api
 
     @property
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client/methods/ed_unit_student.py` & `hollihop_api_client-0.0.2/src/hollihop_api_client/methods/ed_units.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,195 +1,208 @@
-from ..base import BaseCategory
-from typing import TYPE_CHECKING, Any
-import phonenumbers
+from pprint import pprint
+
+from base import BaseCategory
+from typing import TYPE_CHECKING, Any, List
 
 from dataclasses import dataclass, field
-from datetime import datetime, time, date, timedelta
+from datetime import datetime, time
+
+from tools import dict_to_camel, dict_to_snake
 
 if TYPE_CHECKING:
-    from ..api import AbstractAPI
+    from api import AbstractAPI
+
+
+@dataclass
+class ScheduleItem:
+    begin_date: None | datetime = None
+    begin_time: None | str = None
+    classroom_id: None | int = None
+    classroom_name: None | str = None
+    classroom_link: None | str = None
+    end_date: None | datetime = None
+    end_time: None | str = None
+    id: None | int = None
+    teacher: None | str = None
+    teacher_genders: None | list[str] = None
+    teacher_id: None | int = None
+    teacher_ids: None | list[int] = None
+    teacher_photo_urls: None | list[str] = None
+    teachers: None | list[str] = None
+    weekdays: None | int = None
+
+    def __post_init__(self):
+        if not self.begin_time is None:
+            self.begin_date = datetime.fromisoformat(self.begin_date)
+        if not self.end_date is None:
+            self.end_date = datetime.fromisoformat(self.end_date)
+
+
+@dataclass
+class Day:
+    date: None | datetime = None
+    minutes: None | float = None
+    pass_: None | bool = field(init=False)
+    Pass: None | bool = None
+    description: None | str = None
+    student_payable_minutes: None | float = None
+    teacher_payable_minutes: None | float = None
+
+    def __post_init__(self):
+        if not self.date is None:
+            self.date = datetime.fromisoformat(self.date)
+        self.pass_ = self.Pass
+        del self.Pass
+        # delattr(self, 'Pass')
+
+
+@dataclass
+class FiscalInfo:
+    price_id: None | int = None
+    price_name: None | str = None
+    price_value: None | str = None
+    units: None | str = None
+    units28: None | str = None
+    units7: None | str = None
+    value: None | str = None
+    value28: None | str = None
+    value7: None | str = None
+
+    def __post_init__(self):
+        if not self.price_name is None:
+            self.price_name = self.price_name.replace('\xa0', ' ')
+        if not self.price_value is None:
+            self.price_value = self.price_value.replace('\xa0', ' ')
+        if not self.value is None:
+            self.value = self.value.replace('\xa0', ' ')
+        if not self.value28 is None:
+            self.value28 = self.value28.replace('\xa0', ' ')
+        if not self.value7 is None:
+            self.value7 = self.value7.replace('\xa0', ' ')
+
 
 @dataclass
-class StudentAgent:
-    FirstName: None | str = None
-    LastName: None | str = None
-    MiddleName: None | str = None
-    WhoIs: None | str = None
-    Mobile: None | str = None
-    UseMobileBySystem: None | str = None
-    Phone: None | str = None
-    EMail: None | str = None
-    UseEMailBySystem: None | bool = None
-    Skype: None | str = None
-    JobOrStudyPlace: None | str = None
-    Position: None | str = None
-    IsCustomer: None | bool = None
-    Birthday: None | datetime = None
+class PriceValue:
+    students: None | int = None
+    value: None | str = None
+    value_currency: None | str = None
+    value_quantity: None | float = None
+
+    def __post_init__(self):
+        if not self.value is None:
+            self.value = self.value.replace('\xa0', ' ')
+
 
+@dataclass
+class TeacherPrice:
+    price_id: None | int = None
+    price_name: None | str = None
+    price_units: None | str = None
+    price_units_quantity: None | int = None
+    price_units_type: None | str = None
+    price_values: None | list[PriceValue] = None
+    teacher_id: None | int = None
 
+    def __post_init__(self):
+        if not self.price_values is None:
+            self.price_values = [PriceValue(**_) for _ in self.price_values]
 
 
 @dataclass
-class Payer:
-    ClientId: int | None = None
-    IsCompany: bool | None = None
-    Name: str | None = None
-    Actual: bool | None = None
-    TerminatedContracts: list = None
-    PriceId: int | None = None
-    PriceName: str | None = None
-    Discounts: list | None = None
-    Surcharges: list | None = None
-    PayableMinutes: int | None = None
-    PayableUnits: str | None = None
-    PayableMinutesRanged: int | None = None
-    PayableUnitsRanged: str | None = None
-    Value: str | None = None
-    ValueRanged: str | None = None
-    ValuePaidRanged: str | None = None
-    ContractValue: str | None = None
-    ContractValueRestored: str | None = None
-    ContractValueRanged: str | None = None
-    ContractValueRangedRestored: str | None = None
-    DebtDate: datetime | None = None
-    EdUnitPayments: list | None = None
-
-
-@dataclass 
-class Student:
-    EdUnitId: int | None = None
-    EdUnitType: str | None = None
-    EdUnitName: str | None = None
-    EdUnitCorporative: bool | None = None
-    EdUnitOfficeOrCompanyId: int | None = None
-    EdUnitOfficeOrCompanyName: str | None = None
-    EdUnitDiscipline: str | None = None
-    EdUnitLevel: str | None = None
-    EdUnitMaturity: str | None = None
-    EdUnitLearningType: str | None = None
-    StudentClientId: int | None = None
-    StudentName: str | None = None
-    StudentMobile: str | None = None
-    StudentPhone: str | None = None
-    StudentEMail: str | None = None
-    StudentAgents: list[StudentAgent] | None = None
-    StudentExtraFields: list | None = None
-    BeginDate: datetime | None = None
-    EndDate: datetime | None = None
-    BeginTime: time | None = None
-    EndTime: time | None = None
-    Weekdays: int | None = None
-    Status: str | None = None
-    StudyMinutes: int | None = None
-    StudyUnits: str | None = None
-    Days: list | None = None
-    Payers: list[Payer] | None = None
-    Phones: list[str] = field(init=False) 
-
-    def __post_init__(self):
-        self.Phones = []
-        if not self.Payers is None:
-            self.Payers = [Payer(**_) for _ in self.Payers]
-        if not self.StudentAgents is None:
-            self.StudentAgents = [StudentAgent(**_) for _ in self.StudentAgents]
-            for agent in self.StudentAgents:
-                if not agent.Mobile is None:
-                    self.Phones.append(self.format_phone(agent.Mobile).replace('+', ''))
-        if not self.StudentMobile is None:
-            self.Phones.append(self.format_phone(self.StudentMobile).replace('+', ''))
-        if not self.StudentPhone is None:
-            self.Phones.append(self.format_phone(self.StudentPhone).replace('+', ''))
-
-    def format_phone(self, number) -> str:
-        return phonenumbers.format_number(
-                phonenumbers.parse(number, 'RU'),
-                phonenumbers.PhoneNumberFormat.E164
-                )
-
-    def __repr__(self) -> str:
-        return self.StudentName
-
-
-
-@dataclass 
-class Students:
-    EdUnitStudents: list[Student] = field(default_factory=list)
+class EdUnit:
+    id: int | None = None
+    type: str | None = None
+    name: str | None = None
+    corporative: bool = False
+    office_or_company_id: int | None = None
+    office_or_company_name: str | None = None
+    office_or_company_address: str | None = None
+    office_time_zone: time | None = None
+    discipline: str | None = None
+    level: str | None = None
+    maturity: str | None = None
+    learning_type: str | None = None
+    extra_fields: list | None = None
+    students_count: int | None = None
+    vacancies: int | None = None
+    study_units_in_range: str | None = None
+    description: str | None = None
+    company_contract_number: str | None = None
+    company_contract_date: datetime | None = None
+    schedule_items: list | None = None
+    days: list[Day] | None = None
+    fiscal_info: FiscalInfo | list = None
+    teacher_prices: None | list[TeacherPrice] = None
+    price_values: None | list = None
+    assignee: None | dict = None
 
+    def __post_init__(self):
+        if not self.schedule_items is None:
+            self.schedule_items = [ScheduleItem(**_) for _ in self.schedule_items]
+        if not self.days is None:
+            self.days = [Day(**_) for _ in self.days]
+        if not self.fiscal_info is None:
+            self.fiscal_info = FiscalInfo(**self.fiscal_info)
+        if not self.teacher_prices is None:
+            self.teacher_prices = [TeacherPrice(**_) for _ in self.teacher_prices]
+
+
+@dataclass(frozen=True)
+class Statuses:
+    Reserve = 'Reserve'
+    Forming = 'Forming'
+    Working = 'Working'
+    Stopped = 'Stopped'
+    Finished = 'Finished'
+
+
+@dataclass
+class EdUnits:
+    ed_units: list[EdUnit] = field(default_factory=list)
 
-class StudentsCategory(BaseCategory):
+
+class EdUnitsCategory(BaseCategory):
 
     def __init__(self, api: 'AbstractAPI'):
         self.api = api
 
-    def get_students(
+    def get_ed_units(
             self,
-            edUnitId: None | int = None,
-            edUnitTypes: None | str = None,
-            edUnitOfficeOrCompanyId: None | int = None,
-            edUnitOfficeOrCompany: None | str = None,
-            studentClientId: None | int = None,
-            dateFrom: None | datetime = None,
-            dateTo: None | datetime = None,
+            id: None | int = None,
+            types: None | str = None,
+            date_from: None | datetime = None,
+            date_to: None | datetime = None,
             statuses: None | str = None,
-            queryPayers: None | bool = None
-            ) -> list[Student]:
-        data = self.handle_parameters(locals())
+            office_or_company_id: None | int = None,
+            location_id: None | int = None,
+            disciplines: None | str = None,
+            levels: None | str = None,
+            maturities: None | str = None,
+            corporative: None | bool = None,
+            learning_types: None | str = None,
+            teacher_id: None | int = None,
+            query_days: None | bool = None,
+            query_fiscal_info: None | bool = None,
+            query_teacher_prices: None | bool = None,
+    ) -> list[EdUnit]:
+        data = dict_to_camel(self.handle_parameters(locals()))
 
         response = self.api.request(
-                method='GetEdUnitStudents',
-                http_method='GET',
-                data=data
-                )
-
-        return [Student(**_) for _ in Students(**response).EdUnitStudents]
-    
-    def get_all_students_name(self, **kwargs) -> list[str]:
-        students = self.get_students(**kwargs)
-        return [student.StudentName for student in students]
-
-    def get_all_students_id(self, **kwargs) -> list[int]:
-        students = self.get_students(**kwargs)
-        return [student.StudentClientId for student in students]
+            method='GetEdUnits',
+            http_method='GET',
+            data=data
+        )
 
-    def get_students_with_debt(
-            self,
-            in_a_week: bool = False,
-            not_newbies: bool = True,
-            **kwargs):
-        students = self.get_students(**kwargs)
-        if not_newbies:
-            students = [student 
-                    for student in students
-                    if not student.Payers[0].EdUnitPayments is None
-                    and
-                    len(student.Payers[0].EdUnitPayments) > 1
-                    ]
-        students = [student 
-                for student in students
-                if not student.Payers[0].DebtDate is None 
-                and 
-                datetime.strptime(
-                    student.Payers[0].DebtDate, 
-                    '%Y-%m-%d'
-                    ) <= datetime.now()
-                ]
-        if in_a_week:
-            today_debtors_ids = [
-                    student.StudentClientId for student in students
-                    ] 
-            students = [student
-                    for student in students 
-                    if not student.Payers[0].DebtDate is None 
-                    and
-                    datetime.strptime(
-                        student.Payers[0].DebtDate,
-                        '%Y-%m-%d'
-                        ) <= datetime.now() + timedelta(days=7) and 
-                    student.StudentClientId not in today_debtors_ids
-                    ]
+        response = dict_to_snake(response)
+
+        return [EdUnit(**_) for _ in EdUnits(**response).ed_units]
 
-        return students
+    def get_all_ed_units_name(self, **kwargs) -> list[str]:
+        ed_units = self.get_ed_units(**kwargs)
+        return [ed_unit.name for ed_unit in ed_units]
 
+    def get_all_ed_units_id(self, **kwargs) -> list[int]:
+        ed_units = self.get_ed_units(**kwargs)
+        return [ed_unit.id for ed_unit in ed_units]
 
 
-__all__ = ['StudentsCategory']
-        
+__all__ = ['EdUnitsCategory']
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client/methods/ed_units.py` & `hollihop_api_client-0.0.2/src/hollihop_api_client/methods/leads.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,102 @@
-from ..base import BaseCategory
+from base import BaseCategory
 from typing import TYPE_CHECKING, Any
 
 from dataclasses import dataclass, field
-from datetime import datetime, time
+from datetime import datetime
+
+from tools import dict_to_camel, dict_to_snake
 
 if TYPE_CHECKING:
-    from ..api import AbstractAPI
+    from api import AbstractAPI
+
+
+@dataclass
+class Agent:
+    first_name: str | None = None
+    last_name: str | None = None
+    is_customer: bool | None = None
+    use_email_by_system: bool | None = None
+    use_mobile_by_system: bool | None = None
+
+
+@dataclass
+class ExtraField:
+    name: str | None = None
+    value: str | None = None
 
 
 @dataclass
-class EdUnit:
-    Id: int | None = None
-    Type: str | None = None
-    Name: str | None = None
-    Corporative: bool = False
-    OfficeOrCompanyId: int | None = None
-    OfficeOrCompanyName: str | None = None
-    OfficeOrCompanyAddress: str | None = None
-    OfficeTimeZone: time | None = None
-    Discipline: str | None = None
-    Level: str | None = None
-    Maturity: str | None = None
-    LearningType: str | None = None
-    ExtraFields: list | None = None
-    StudentsCount: int | None = None
-    Vacancies: int | None = None
-    StudyUnitsInRange: str | None = None
-    Description: str | None = None
-    CompanyContractNumber: str | None = None
-    CompanyContractDate: datetime | None = None
-    ScheduleItems: list | None = None
-    Days: list | None = None
-    FiscalInfo: None | list = None
-    TeacherPrices: None |list = None
-    PriceValues: None | list = None
-    Assignee: None | dict = None
-
-
-@dataclass(frozen=True)
-class Statuses:
-    Reserve = 'Reserve'
-    Forming = 'Forming'
-    Working = 'Working'
-    Stopped = 'Stopped'
-    Finished = 'Finished' 
-
-
-@dataclass 
-class EdUnits:
-    EdUnits: list[EdUnit] = field(default_factory=list)
+class Lead:
+    id: int | None
+    created: datetime | None = None
+    updated: datetime | None = None
+    first_name: str | None = None
+    last_name: str | None = None
+    middle_name: str | None = None
+    address_date: datetime | None = None
+    ad_source: str | None = None
+    status_id: str | None = None
+    status: str | None = None
+    birthday: datetime | None = None
+    phone: str | None = None
+    mobile: str | None = None
+    use_mobile_by_system: bool | None = None
+    email: str | None = None
+    use_email_by_system: bool | None = None
+    maturity: str | None = None
+    learning_type: str | None = None
+    discipline: str | None = None
+    level: str | None = None
+    agents: list[Agent] | None = None
+    offices_and_companies: list | None = None
+    assignees: list | None = None
+    extra_fields: list | None = None
+    student_client_id: int | None = None
+    name: str = field(init=False)
+
+    def __post_init__(self):
+        self.name = ' '.join(filter(lambda str_obj: str_obj, [
+                             self.last_name, self.first_name, self.middle_name]))
+        if self.agents:
+            self.agents = [Agent(**_) for _ in self.agents]
+        if self.extra_fields:
+            self.extra_fields = [ExtraField(**_) for _ in self.extra_fields]
 
 
-class EdUnitsCategory(BaseCategory):
+@dataclass
+class Leads:
+    leads: None | list[Lead] = field(default_factory=list)
+    now: None | datetime = None
+
+
+class LeadsCategory(BaseCategory):
 
     def __init__(self, api: 'AbstractAPI'):
         self.api = api
 
-    def get_ed_units(
+    def get_leads(
             self,
             id: None | int = None,
-            types: None | str = None,
-            dateFrom: None | datetime = None,
-            dateTo: None | datetime = None,
-            statuses: None | str = None,
-            officeOrCompanyId: None | int = None,
-            locationId: None | int = None,
-            disciplines: None | str = None,
-            levels: None | str = None,
-            maturities: None | str = None,
-            corporative: None | bool = None,
-            learningTypes: None | str = None
-            ) -> list[EdUnit]:
-        data = self.handle_parameters(locals())
+            attached: None | bool = None,
+            student_client_id: None | int = None
+    ) -> list[Lead]:
+        data = dict_to_camel(self.handle_parameters(locals()))
 
         response = self.api.request(
-                method='GetEdUnits',
-                http_method='GET',
-                data=data
-                )
-
-        return [EdUnit(**_) for _ in EdUnits(**response).EdUnits]
-    
-    def get_all_ed_units_name(self, **kwargs) -> list[str]:
-        ed_units = self.get_ed_units(**kwargs)
-        return [ed_unit.Name for ed_unit in ed_units]
-
-    def get_all_ed_units_id(self, **kwargs) -> list[int]:
-        ed_units = self.get_ed_units(**kwargs)
-        return [ed_unit.Id for ed_unit in ed_units]
+            method='GetLeads',
+            http_method='GET',
+            data=data
+        )
+
+        response = dict_to_snake(response)
+
+        raw_leads = [Lead(**_) for _ in Leads(**response).leads]
+
+        return raw_leads
+
+    def get_all_leads_id(self, **kwargs) -> list[int]:
+        leads = self.get_leads(**kwargs)
+        return [lead.student_client_id for lead in leads]
 
 
-__all__ = ['EdUnitsCategory']
-        
+__all__ = ['LeadsCategory']
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client/methods/leads.py` & `hollihop_api_client-0.0.2/src/hollihop_api_client/methods/offices.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,65 @@
-from ..base import BaseCategory
+from base import BaseCategory
 from typing import TYPE_CHECKING, Any
 
 from dataclasses import dataclass, field
-from datetime import datetime, time, date, timedelta
+from datetime import timezone
+
+from tools import dict_to_camel, dict_to_snake
 
 if TYPE_CHECKING:
-    from ..api import AbstractAPI
+    from api import AbstractAPI
+
 
-    
 @dataclass
-class Lead:
-    Id: int | None
-    Created: datetime | None = None
-    Updated: datetime | None = None
-    FirstName: str | None = None
-    LastName: str | None = None
-    MiddleName: str | None = None
-    AddressDate: datetime | None = None
-    AdSource: str | None = None
-    StatusId: str | None = None
-    Status: str | None = None
-    Birthday: datetime | None = None
-    Phone: str | None = None
-    Mobile: str | None = None
-    UseMobileBySystem: bool | None = None
-    EMail: str | None = None
-    UseEMailBySystem: bool | None = None
-    Maturity: str | None = None
-    LearningType: str | None = None
-    Discipline: str | None = None
-    Level: str | None = None
-    Agents: list | None = None
-    OfficesAndCompanies: list | None = None
-    Assignees: list | None = None
-    ExtraFields: list | None = None
-    StudentClientId: int | None = None
-    Name: str = field(init=False)
-    
-    def __post_init__(self):
-        self.Name = self.LastName + ' ' + self.FirstName + ' ' + self.MiddleName 
+class Office:
+    id: None | int = None
+    name: None | str = None
+    location: None | str = None
+    address: None | str = None
+    email: None | str = None
+    phone: None | str = None
+    no_classrooms: None | bool = None
+    time_zone: None | timezone = None
+    license: None | str = None
 
 
 @dataclass 
-class Leads:
-    Leads: None | list[Lead] = field(default_factory=list)
-    Now: None | datetime = None
+class Offices:
+    offices: list[Office] = field(default_factory=list)
 
 
-class LeadsCategory(BaseCategory):
+class OfficesCategory(BaseCategory):
 
     def __init__(self, api: 'AbstractAPI'):
         self.api = api
 
-    def get_leads(
+    def get_offices(
             self,
             id: None | int = None,
-            attached: None | bool = None,
-            studentClientId: None | int = None
-            ) -> list[Lead]:
-        data = self.handle_parameters(locals())
+            location_id: None | int = None,
+            name: None | str = None,
+            license: None | str = None
+            ) -> list[Office]:
+        data = dict_to_camel(self.handle_parameters(locals()))
 
         response = self.api.request(
-                method='GetLeads',
+                method='GetOffices',
                 http_method='GET',
                 data=data
                 )
 
-        raw_leads = [Lead(**_) for _ in Leads(**response).Leads]
-        
-        return raw_leads
+        response = dict_to_snake(response)
+
+        return [Office(**_) for _ in Offices(**response).offices]
     
-    def get_all_leads_id(self, **kwargs) -> list[int]:
-        leads = self.get_leads(**kwargs)
-        return [lead.StudentClientId for lead in leads]
+    def get_all_offices_name(self) -> list[str]:
+        offices = self.get_offices()
+        return [office.name for office in offices]
+
+    def get_all_offices_id(self) -> list[int]:
+        offices = self.get_offices()
+        return [office.id for office in offices]
 
 
-__all__ = ['LeadsCategory']
+__all__ = ['OfficesCategory']
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client.egg-info/PKG-INFO` & `hollihop_api_client-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: hollihop-api-client
-Version: 0.0.1
-Summary: This library helps you easily create a python application with Hollihop API 
-Author-email: Nicholas Maltsev <nmmaltsev@outlook.com>
-Project-URL: Homepage, https://github.com/nicholasChieftain/hollyhope-api-client
-Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollyhope-api-client/issues
+Name: hollihop_api_client
+Version: 0.0.2
+Summary: This library helps you easily create a python application with Hollihop API
+Author-email: Nicholas Maltseb <nmmaltsev@outlook.com>
+Project-URL: Homepage, https://github.com/nicholasChieftain/hollihop_api_client/
+Project-URL: Bug Tracker, https://github.com/nicholasChieftain/hollihop_api_client/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,17 +24,17 @@
 ```
 
 ## Использование
 
 ### Инициализация
 
 ```python
-from hollihop_api_client import hhAPI
+from hollihop_api_client import HolliHopAPI
 
-hh_api = hhAPI(HH_DOMAIN, HH_COMMON_API_KEY)
+hh_api = HolliHopAPI(HH_DOMAIN, HH_COMMON_API_KEY)
 ```
 
 Обратите внимание, что ключи нужно получать из переменных среды:
 
 ```python
 from os import environ
```

### Comparing `hollihop_api_client-0.0.1/src/hollihop_api_client.egg-info/SOURCES.txt` & `hollihop_api_client-0.0.2/src/hollihop_api_client.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
-src/hollihop_api_client/__init__.py
 src/hollihop_api_client/categories.py
+src/hollihop_api_client/test.py
 src/hollihop_api_client.egg-info/PKG-INFO
 src/hollihop_api_client.egg-info/SOURCES.txt
 src/hollihop_api_client.egg-info/dependency_links.txt
 src/hollihop_api_client.egg-info/top_level.txt
 src/hollihop_api_client/api/__init__.py
 src/hollihop_api_client/api/abc.py
 src/hollihop_api_client/api/api.py
 src/hollihop_api_client/base/__init__.py
 src/hollihop_api_client/base/category.py
 src/hollihop_api_client/methods/__init__.py
-src/hollihop_api_client/methods/ed_unit_student.py
+src/hollihop_api_client/methods/ed_unit_students.py
 src/hollihop_api_client/methods/ed_units.py
 src/hollihop_api_client/methods/leads.py
 src/hollihop_api_client/methods/locations.py
-src/hollihop_api_client/methods/offices.py
+src/hollihop_api_client/methods/offices.py
+src/hollihop_api_client/tests/__init__.py
+src/hollihop_api_client/tests/conftest.py
+src/hollihop_api_client/tests/test_ed_unit_students.py
+src/hollihop_api_client/tests/test_ed_units.py
+src/hollihop_api_client/tests/test_lead.py
+src/hollihop_api_client/tests/test_locations.py
+src/hollihop_api_client/tests/test_offices.py
+src/hollihop_api_client/tools/__init__.py
```

