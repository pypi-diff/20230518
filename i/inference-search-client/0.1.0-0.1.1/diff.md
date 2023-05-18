# Comparing `tmp/inference_search_client-0.1.0.tar.gz` & `tmp/inference_search_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference_search_client-0.1.0.tar", max compression
+gzip compressed data, was "inference_search_client-0.1.1.tar", max compression
```

## Comparing `inference_search_client-0.1.0.tar` & `inference_search_client-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     9723 2023-05-16 16:54:17.158630 inference_search_client-0.1.0/README.md
--rw-r--r--   0        0        0      819 2023-05-16 16:54:17.160242 inference_search_client-0.1.0/inference_search_client/__init__.py
--rw-r--r--   0        0        0    58532 2023-05-16 16:54:17.160638 inference_search_client-0.1.0/inference_search_client/api_client.py
--rw-r--r--   0        0        0      214 2023-05-16 16:54:17.160873 inference_search_client-0.1.0/inference_search_client/apis/__init__.py
--rw-r--r--   0        0        0      344 2023-05-16 16:54:17.160999 inference_search_client-0.1.0/inference_search_client/apis/path_to_api.py
--rw-r--r--   0        0        0      250 2023-05-16 16:54:17.161181 inference_search_client-0.1.0/inference_search_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      113 2023-05-16 16:54:17.161325 inference_search_client-0.1.0/inference_search_client/apis/paths/search_poi.py
--rw-r--r--   0        0        0      338 2023-05-16 16:54:17.161452 inference_search_client-0.1.0/inference_search_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      320 2023-05-16 16:54:17.161650 inference_search_client-0.1.0/inference_search_client/apis/tags/__init__.py
--rw-r--r--   0        0        0      488 2023-05-16 16:54:17.161789 inference_search_client-0.1.0/inference_search_client/apis/tags/default_api.py
--rw-r--r--   0        0        0    15181 2023-05-16 16:54:17.161925 inference_search_client-0.1.0/inference_search_client/configuration.py
--rw-r--r--   0        0        0     4510 2023-05-16 16:54:17.162080 inference_search_client-0.1.0/inference_search_client/exceptions.py
--rw-r--r--   0        0        0      357 2023-05-16 16:54:17.162322 inference_search_client-0.1.0/inference_search_client/model/__init__.py
--rw-r--r--   0        0        0     2414 2023-05-16 16:54:17.162463 inference_search_client-0.1.0/inference_search_client/model/generic_error_response.py
--rw-r--r--   0        0        0     2414 2023-05-16 16:54:17.162573 inference_search_client-0.1.0/inference_search_client/model/generic_error_response.pyi
--rw-r--r--   0        0        0     4005 2023-05-16 16:54:17.162674 inference_search_client-0.1.0/inference_search_client/model/poi.py
--rw-r--r--   0        0        0     4005 2023-05-16 16:54:17.162790 inference_search_client-0.1.0/inference_search_client/model/poi.pyi
--rw-r--r--   0        0        0     7045 2023-05-16 16:54:17.162942 inference_search_client-0.1.0/inference_search_client/model/poi_search_request.py
--rw-r--r--   0        0        0     7045 2023-05-16 16:54:17.163080 inference_search_client-0.1.0/inference_search_client/model/poi_search_request.pyi
--rw-r--r--   0        0        0     3321 2023-05-16 16:54:17.163193 inference_search_client-0.1.0/inference_search_client/model/poi_search_response.py
--rw-r--r--   0        0        0     3321 2023-05-16 16:54:17.163305 inference_search_client-0.1.0/inference_search_client/model/poi_search_response.pyi
--rw-r--r--   0        0        0      691 2023-05-16 16:54:17.163496 inference_search_client-0.1.0/inference_search_client/models/__init__.py
--rw-r--r--   0        0        0      330 2023-05-16 16:54:17.163670 inference_search_client-0.1.0/inference_search_client/paths/__init__.py
--rw-r--r--   0        0        0      325 2023-05-16 16:54:17.163891 inference_search_client-0.1.0/inference_search_client/paths/search_poi/__init__.py
--rw-r--r--   0        0        0    13529 2023-05-16 16:54:17.164058 inference_search_client-0.1.0/inference_search_client/paths/search_poi/get.py
--rw-r--r--   0        0        0    13358 2023-05-16 16:54:17.164230 inference_search_client-0.1.0/inference_search_client/paths/search_poi/get.pyi
--rw-r--r--   0        0        0    10547 2023-05-16 16:54:17.164380 inference_search_client-0.1.0/inference_search_client/rest.py
--rw-r--r--   0        0        0    97664 2023-05-16 16:54:17.164861 inference_search_client-0.1.0/inference_search_client/schemas.py
--rw-r--r--   0        0        0      384 2023-05-17 21:20:42.474158 inference_search_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10276 1970-01-01 00:00:00.000000 inference_search_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9674 2023-05-18 15:54:57.172417 inference_search_client-0.1.1/README.md
+-rw-r--r--   0        0        0      819 2023-05-18 15:47:24.630166 inference_search_client-0.1.1/inference_search_client/__init__.py
+-rw-r--r--   0        0        0    58532 2023-05-18 15:47:24.655096 inference_search_client-0.1.1/inference_search_client/api_client.py
+-rw-r--r--   0        0        0      214 2023-05-18 15:47:24.663813 inference_search_client-0.1.1/inference_search_client/apis/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-18 15:47:24.593407 inference_search_client-0.1.1/inference_search_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      250 2023-05-18 15:47:24.594216 inference_search_client-0.1.1/inference_search_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-18 15:47:24.595618 inference_search_client-0.1.1/inference_search_client/apis/paths/search_poi.py
+-rw-r--r--   0        0        0      338 2023-05-18 15:47:24.592881 inference_search_client-0.1.1/inference_search_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      320 2023-05-18 15:47:24.593830 inference_search_client-0.1.1/inference_search_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0      489 2023-05-18 15:47:24.601300 inference_search_client-0.1.1/inference_search_client/apis/tags/default_api.py
+-rw-r--r--   0        0        0    15181 2023-05-18 15:47:24.629042 inference_search_client-0.1.1/inference_search_client/configuration.py
+-rw-r--r--   0        0        0     4510 2023-05-18 15:47:24.630925 inference_search_client-0.1.1/inference_search_client/exceptions.py
+-rw-r--r--   0        0        0      357 2023-05-18 15:47:24.663498 inference_search_client-0.1.1/inference_search_client/model/__init__.py
+-rw-r--r--   0        0        0     2414 2023-05-18 15:47:23.782322 inference_search_client-0.1.1/inference_search_client/model/generic_error_response.py
+-rw-r--r--   0        0        0     2414 2023-05-18 15:47:23.808467 inference_search_client-0.1.1/inference_search_client/model/generic_error_response.pyi
+-rw-r--r--   0        0        0     4005 2023-05-18 15:47:23.933368 inference_search_client-0.1.1/inference_search_client/model/poi.py
+-rw-r--r--   0        0        0     4005 2023-05-18 15:47:24.016802 inference_search_client-0.1.1/inference_search_client/model/poi.pyi
+-rw-r--r--   0        0        0     7045 2023-05-18 15:47:24.230978 inference_search_client-0.1.1/inference_search_client/model/poi_search_request.py
+-rw-r--r--   0        0        0     7045 2023-05-18 15:47:24.311899 inference_search_client-0.1.1/inference_search_client/model/poi_search_request.pyi
+-rw-r--r--   0        0        0     3321 2023-05-18 15:47:24.384109 inference_search_client-0.1.1/inference_search_client/model/poi_search_response.py
+-rw-r--r--   0        0        0     3321 2023-05-18 15:47:24.401754 inference_search_client-0.1.1/inference_search_client/model/poi_search_response.pyi
+-rw-r--r--   0        0        0      691 2023-05-18 15:47:24.663114 inference_search_client-0.1.1/inference_search_client/models/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-18 15:47:24.591789 inference_search_client-0.1.1/inference_search_client/paths/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-18 15:47:24.592246 inference_search_client-0.1.1/inference_search_client/paths/search_poi/__init__.py
+-rw-r--r--   0        0        0    13536 2023-05-18 15:47:24.517311 inference_search_client-0.1.1/inference_search_client/paths/search_poi/post.py
+-rw-r--r--   0        0        0    13365 2023-05-18 15:47:24.591066 inference_search_client-0.1.1/inference_search_client/paths/search_poi/post.pyi
+-rw-r--r--   0        0        0    10547 2023-05-18 15:47:24.657133 inference_search_client-0.1.1/inference_search_client/rest.py
+-rw-r--r--   0        0        0    97664 2023-05-18 15:47:24.662274 inference_search_client-0.1.1/inference_search_client/schemas.py
+-rw-r--r--   0        0        0      384 2023-05-18 15:58:31.880436 inference_search_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10227 1970-01-01 00:00:00.000000 inference_search_client-0.1.1/PKG-INFO
```

### Comparing `inference_search_client-0.1.0/README.md` & `inference_search_client-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install inference_search_client
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
+(you may need to run `pip` with root permission: `sudo pip install inference_search_client`)
 
 Then import the package:
 ```python
 import inference_search_client
 ```
 
 ### Setuptools
@@ -133,60 +133,59 @@
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import time
 import inference_search_client
 from pprint import pprint
 from inference_search_client.apis.tags import default_api
 from inference_search_client.model.generic_error_response import GenericErrorResponse
 from inference_search_client.model.poi_search_request import POISearchRequest
 from inference_search_client.model.poi_search_response import POISearchResponse
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = inference_search_client.Configuration(
-    host = "http://localhost"
+    host = "https://service.mlplat-service-sbx.tamg.cloud/iss"
 )
 
 
 # Enter a context with an instance of the API client
 with inference_search_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = default_api.DefaultApi(api_client)
     poi_search_request = POISearchRequest(
         latitude=3.14,
         longitude=3.14,
-        place_types=[
+        placeTypes=[
             "place_types_example"
         ],
-        radius_in_miles=1,
+        radiusInMiles=1,
         limit=1,
         embedding=[
             3.14
         ],
     ) # POISearchRequest |  (optional)
 
     try:
         # Search neary by POIs by applying geo filter followed by embedding vector similarity
-        api_response = api_instance.search_poi(poi_search_request=poi_search_request)
+        api_response = api_instance.search_poi(body=poi_search_request)
         pprint(api_response)
     except inference_search_client.ApiException as e:
         print("Exception when calling DefaultApi->search_poi: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*DefaultApi* | [**search_poi**](docs/apis/tags/DefaultApi.md#search_poi) | **get** /search/poi | Search neary by POIs by applying geo filter followed by embedding vector similarity
+*DefaultApi* | [**search_poi**](docs/apis/tags/DefaultApi.md#search_poi) | **post** /search/poi | Search neary by POIs by applying geo filter followed by embedding vector similarity
 
 ## Documentation For Models
 
  - [GenericErrorResponse](docs/models/GenericErrorResponse.md)
  - [POI](docs/models/POI.md)
  - [POISearchRequest](docs/models/POISearchRequest.md)
  - [POISearchResponse](docs/models/POISearchResponse.md)
```

### Comparing `inference_search_client-0.1.0/inference_search_client/__init__.py` & `inference_search_client-0.1.1/inference_search_client/__init__.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/api_client.py` & `inference_search_client-0.1.1/inference_search_client/api_client.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/configuration.py` & `inference_search_client-0.1.1/inference_search_client/configuration.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/exceptions.py` & `inference_search_client-0.1.1/inference_search_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/model/generic_error_response.py` & `inference_search_client-0.1.1/inference_search_client/model/generic_error_response.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/model/generic_error_response.pyi` & `inference_search_client-0.1.1/inference_search_client/model/generic_error_response.pyi`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/model/poi.py` & `inference_search_client-0.1.1/inference_search_client/model/poi.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/model/poi.pyi` & `inference_search_client-0.1.1/inference_search_client/model/poi.pyi`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/model/poi_search_request.py` & `inference_search_client-0.1.1/inference_search_client/model/poi_search_request.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/model/poi_search_request.pyi` & `inference_search_client-0.1.1/inference_search_client/model/poi_search_request.pyi`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/model/poi_search_response.py` & `inference_search_client-0.1.1/inference_search_client/model/poi_search_response.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/model/poi_search_response.pyi` & `inference_search_client-0.1.1/inference_search_client/model/poi_search_response.pyi`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/models/__init__.py` & `inference_search_client-0.1.1/inference_search_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/paths/search_poi/get.py` & `inference_search_client-0.1.1/inference_search_client/paths/search_poi/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
             _headers.add('Content-Type', content_type)
             if 'fields' in serialized_data:
                 _fields = serialized_data['fields']
             elif 'body' in serialized_data:
                 _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             fields=_fields,
             body=_body,
             stream=stream,
             timeout=timeout,
         )
 
@@ -312,70 +312,70 @@
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def get(
+    def post(
         self,
         content_type: typing_extensions.Literal["application/json"] = ...,
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
 
     @typing.overload
-    def get(
+    def post(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def post(
         self,
         content_type: str = 'application/json',
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
```

### Comparing `inference_search_client-0.1.0/inference_search_client/paths/search_poi/get.pyi` & `inference_search_client-0.1.1/inference_search_client/paths/search_poi/post.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
             _headers.add('Content-Type', content_type)
             if 'fields' in serialized_data:
                 _fields = serialized_data['fields']
             elif 'body' in serialized_data:
                 _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             fields=_fields,
             body=_body,
             stream=stream,
             timeout=timeout,
         )
 
@@ -304,70 +304,70 @@
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def get(
+    def post(
         self,
         content_type: typing_extensions.Literal["application/json"] = ...,
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
 
     @typing.overload
-    def get(
+    def post(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
         content_type: str = ...,
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def post(
         self,
         content_type: str = 'application/json',
         body: typing.Union[SchemaForRequestBodyApplicationJson, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
```

### Comparing `inference_search_client-0.1.0/inference_search_client/rest.py` & `inference_search_client-0.1.1/inference_search_client/rest.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/inference_search_client/schemas.py` & `inference_search_client-0.1.1/inference_search_client/schemas.py`

 * *Files identical despite different names*

### Comparing `inference_search_client-0.1.0/PKG-INFO` & `inference_search_client-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-search-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: python client for talking to inference search service
 Author: Long Yao
 Author-email: l2yao@tripadvisor.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -119,17 +119,17 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install inference_search_client
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
+(you may need to run `pip` with root permission: `sudo pip install inference_search_client`)
 
 Then import the package:
 ```python
 import inference_search_client
 ```
 
 ### Setuptools
@@ -148,60 +148,59 @@
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import time
 import inference_search_client
 from pprint import pprint
 from inference_search_client.apis.tags import default_api
 from inference_search_client.model.generic_error_response import GenericErrorResponse
 from inference_search_client.model.poi_search_request import POISearchRequest
 from inference_search_client.model.poi_search_response import POISearchResponse
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = inference_search_client.Configuration(
-    host = "http://localhost"
+    host = "https://service.mlplat-service-sbx.tamg.cloud/iss"
 )
 
 
 # Enter a context with an instance of the API client
 with inference_search_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = default_api.DefaultApi(api_client)
     poi_search_request = POISearchRequest(
         latitude=3.14,
         longitude=3.14,
-        place_types=[
+        placeTypes=[
             "place_types_example"
         ],
-        radius_in_miles=1,
+        radiusInMiles=1,
         limit=1,
         embedding=[
             3.14
         ],
     ) # POISearchRequest |  (optional)
 
     try:
         # Search neary by POIs by applying geo filter followed by embedding vector similarity
-        api_response = api_instance.search_poi(poi_search_request=poi_search_request)
+        api_response = api_instance.search_poi(body=poi_search_request)
         pprint(api_response)
     except inference_search_client.ApiException as e:
         print("Exception when calling DefaultApi->search_poi: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*DefaultApi* | [**search_poi**](docs/apis/tags/DefaultApi.md#search_poi) | **get** /search/poi | Search neary by POIs by applying geo filter followed by embedding vector similarity
+*DefaultApi* | [**search_poi**](docs/apis/tags/DefaultApi.md#search_poi) | **post** /search/poi | Search neary by POIs by applying geo filter followed by embedding vector similarity
 
 ## Documentation For Models
 
  - [GenericErrorResponse](docs/models/GenericErrorResponse.md)
  - [POI](docs/models/POI.md)
  - [POISearchRequest](docs/models/POISearchRequest.md)
  - [POISearchResponse](docs/models/POISearchResponse.md)
```

