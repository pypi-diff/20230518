# Comparing `tmp/flask_pydantic_api-0.9.3-py3-none-any.whl.zip` & `tmp/flask_pydantic_api-0.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12719 bytes, number of entries: 12
+Zip file size: 12866 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       98 b- defN 23-Apr-06 01:39 flask_pydantic_api/__init__.py
--rw-r--r--  2.0 unx     6964 b- defN 23-Apr-06 02:20 flask_pydantic_api/api_wrapper.py
+-rw-r--r--  2.0 unx     7129 b- defN 23-May-17 21:33 flask_pydantic_api/api_wrapper.py
 -rw-r--r--  2.0 unx      819 b- defN 23-Mar-18 20:39 flask_pydantic_api/apidocs_views.py
--rw-r--r--  2.0 unx     7386 b- defN 23-Apr-13 22:12 flask_pydantic_api/openapi.py
+-rw-r--r--  2.0 unx     7733 b- defN 23-May-17 21:59 flask_pydantic_api/openapi.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-19 03:04 flask_pydantic_api/py.typed
 -rw-r--r--  2.0 unx     2342 b- defN 23-Apr-06 02:14 flask_pydantic_api/utils.py
 -rw-r--r--  2.0 unx      447 b- defN 23-Mar-18 20:21 flask_pydantic_api/templates/rapidoc.html
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    11905 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1056 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/RECORD
-12 files, 32201 bytes uncompressed, 10913 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-17 22:01 flask_pydantic_api-0.9.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12093 b- defN 23-May-17 22:01 flask_pydantic_api-0.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 22:01 flask_pydantic_api-0.9.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-17 22:01 flask_pydantic_api-0.9.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1056 b- defN 23-May-17 22:01 flask_pydantic_api-0.9.4.dist-info/RECORD
+12 files, 32901 bytes uncompressed, 11060 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: flask_pydantic_api/utils.py
 Comment: 
 
 Filename: flask_pydantic_api/templates/rapidoc.html
 Comment: 
 
-Filename: flask_pydantic_api-0.9.3.dist-info/LICENSE
+Filename: flask_pydantic_api-0.9.4.dist-info/LICENSE
 Comment: 
 
-Filename: flask_pydantic_api-0.9.3.dist-info/METADATA
+Filename: flask_pydantic_api-0.9.4.dist-info/METADATA
 Comment: 
 
-Filename: flask_pydantic_api-0.9.3.dist-info/WHEEL
+Filename: flask_pydantic_api-0.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: flask_pydantic_api-0.9.3.dist-info/top_level.txt
+Filename: flask_pydantic_api-0.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_pydantic_api-0.9.3.dist-info/RECORD
+Filename: flask_pydantic_api-0.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_pydantic_api/api_wrapper.py

```diff
@@ -21,14 +21,15 @@
 except ImportError:
     pass
 
 
 class EndpointConfig(BaseModel):
     name: Optional[str]
     tags: Optional[List[str]]
+    openapi_schema_extra: Optional[Dict[str, Any]]
     success_status_code: int
     request_fields_name: str
 
 
 def get_request_args(
     view_kwargs: Dict[str, Any],
     for_model: Optional[Type[BaseModel]] = None,
@@ -91,14 +92,15 @@
 def pydantic_api(
     name: Optional[str] = None,
     tags: Optional[List[str]] = None,
     success_status_code: int = 200,
     maximum_expansion_depth=5,
     request_fields_name: str = "fields",
     merge_path_parameters: bool = False,
+    openapi_schema_extra: Optional[Dict[str, Any]] = None,
 ) -> Callable:
     def wrap(view_func: Callable) -> Callable:
         request_model_param_name, request_model, response_models = get_annotated_models(
             view_func
         )
 
         @wraps(view_func)
@@ -187,12 +189,13 @@
         # This adds some markers that are useful for introspection of
         # endpoints (such as generating schema).
         wrapped_endpoint.__pydantic_api__ = EndpointConfig(  # type: ignore
             name=name,
             tags=tags,
             success_status_code=success_status_code,
             request_fields_name=request_fields_name,
+            openapi_schema_extra=openapi_schema_extra,
         )
 
         return wrapped_endpoint
 
     return wrap
```

## flask_pydantic_api/openapi.py

```diff
@@ -144,14 +144,17 @@
                 "summary": view_func_config.name,
                 "requestBody": request_body,
                 "tags": view_func_config.tags or [],
                 "parameters": parameters,
                 "responses": responses,
             }
 
+            if view_func_config.openapi_schema_extra:
+                _deep_update(paths[path][method], view_func_config.openapi_schema_extra)
+
     return paths
 
 
 def add_response_schema(
     openapi: OpenAPI, status_code: str, schema: Type[BaseModel]
 ) -> OpenAPI:
     if not openapi.paths:
@@ -226,9 +229,15 @@
     for key in from_dict.keys():
         if (
             key in into_dict
             and isinstance(from_dict[key], dict)
             and isinstance(into_dict[key], dict)
         ):
             _deep_update(into_dict[key], from_dict[key])
+        elif (
+            key in into_dict
+            and isinstance(from_dict[key], list)
+            and isinstance(into_dict[key], list)
+        ):
+            into_dict[key].extend(from_dict[key])
         else:
             into_dict[key] = from_dict[key]
```

## Comparing `flask_pydantic_api-0.9.3.dist-info/LICENSE` & `flask_pydantic_api-0.9.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flask_pydantic_api-0.9.3.dist-info/METADATA` & `flask_pydantic_api-0.9.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-pydantic-api
-Version: 0.9.3
+Version: 0.9.4
 Summary: Pydantic based API support for Flask
 Home-page: https://github.com/adamsussman/flask-pydantic-api
 Author: Adam Sussman
 Author-email: adam.sussman@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
@@ -147,14 +147,15 @@
 
 * `name`: str - Name for this operation that will be used in the OpenAPI schema
 * `Tags`: List[str] - Tags that will be used for this operation in the OpenAPI schema
 * `success_status_code`: int = 200 - HTTP Status code that will be used on successful response
 * `merge_path_parameters`: bool = False - See [Path Parameter Folding](#patharguments)
 * `request_fields_name`: str = "fields" - If using `pydantic-enhanced-serialzer` this is the name of the request parameter that controls the fieldsets returned. See [Using the Enhanced Serializer](#serializer).
 * `maximum_expansion_depth`: int = 5 - If using `pydantic-enhanced-serialzer` this controls how deep expansions can go. See [Using the Enhanced Serializer](#serializer).
+* `openapi_schema_extra`: Optional[Dict[str, Any]] - Optional extra data to add to the openapi schema.  Will be merged with automatically generated schema data at `paths.<path>.<method>`.
 
 Flask configuration:
 
 * `FLASK_PYDANTIC_API_RENDER_ERRORS`: bool = True.  If true, pydantic validation errors will be rendered to json and returned as a normal response.  If false, pydantic errors will yield a standard ValidationError exception.
 * `FLASK_PYDANTIC_API_ERROR_STATUS_CODE`: int = 400.  If `FLASK_PYDANTIC_API_RENDER_ERRORS` is true, this is the HTTP status code that will be returned.
 
 <a name="patharguments"></a>
```

