# Comparing `tmp/fling_client-0.1.1.tar.gz` & `tmp/fling_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_client-0.1.1.tar", max compression
+gzip compressed data, was "fling_client-0.1.4.tar", max compression
```

## Comparing `fling_client-0.1.1.tar` & `fling_client-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,35 @@
--rw-r--r--   0        0        0        0 2023-04-06 03:37:25.245135 fling_client-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     3730 2023-04-05 23:18:00.740582 fling_client-0.1.1/README.md
--rw-r--r--   0        0        0      149 2023-04-07 22:05:07.570365 fling_client-0.1.1/fling_client/__init__.py
--rw-r--r--   0        0        0       47 2023-04-07 22:05:06.953346 fling_client-0.1.1/fling_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 22:05:06.980578 fling_client-0.1.1/fling_client/api/data/__init__.py
--rw-r--r--   0        0        0     5452 2023-04-07 22:05:07.608034 fling_client-0.1.1/fling_client/api/data/add_data_fling_id_add_post.py
--rw-r--r--   0        0        0     5464 2023-04-07 22:05:07.611362 fling_client-0.1.1/fling_client/api/data/add_to_index_index_put.py
--rw-r--r--   0        0        0     4398 2023-04-07 22:05:07.618597 fling_client-0.1.1/fling_client/api/data/get_repo_list_repolist_get.py
--rw-r--r--   0        0        0     5299 2023-04-07 22:05:07.616227 fling_client-0.1.1/fling_client/api/data/read_data_fling_id_get.py
--rw-r--r--   0        0        0     4939 2023-04-07 22:05:07.618604 fling_client-0.1.1/fling_client/api/data/read_index_index_get.py
--rw-r--r--   0        0        0        0 2023-04-07 22:05:06.961606 fling_client-0.1.1/fling_client/api/default/__init__.py
--rw-r--r--   0        0        0     4519 2023-04-07 22:05:07.628278 fling_client-0.1.1/fling_client/api/default/github_code_callback_get.py
--rw-r--r--   0        0        0     4265 2023-04-07 22:05:07.644925 fling_client-0.1.1/fling_client/api/default/github_login_github_login_get.py
--rw-r--r--   0        0        0     2345 2023-04-07 22:05:07.638700 fling_client-0.1.1/fling_client/api/default/index_get.py
--rw-r--r--   0        0        0        0 2023-04-07 22:05:06.979871 fling_client-0.1.1/fling_client/api/names/__init__.py
--rw-r--r--   0        0        0     5510 2023-04-07 22:05:07.652793 fling_client-0.1.1/fling_client/api/names/generate_names_namer_get.py
--rw-r--r--   0        0        0     2817 2023-04-07 22:05:07.642295 fling_client-0.1.1/fling_client/client.py
--rw-r--r--   0        0        0      470 2023-04-07 22:05:07.621478 fling_client-0.1.1/fling_client/errors.py
--rw-r--r--   0        0        0     1098 2023-04-07 22:05:07.317069 fling_client-0.1.1/fling_client/models/__init__.py
--rw-r--r--   0        0        0     1375 2023-04-07 22:05:07.655933 fling_client-0.1.1/fling_client/models/add_data_fling_id_add_post_response_add_data_fling_id_add_post.py
--rw-r--r--   0        0        0     1339 2023-04-07 22:05:07.634127 fling_client-0.1.1/fling_client/models/add_to_index_index_put_response_add_to_index_index_put.py
--rw-r--r--   0        0        0     1363 2023-04-07 22:05:07.632978 fling_client-0.1.1/fling_client/models/generate_names_namer_get_response_generate_names_namer_get.py
--rw-r--r--   0        0        0     2131 2023-04-07 22:05:07.655547 fling_client-0.1.1/fling_client/models/http_validation_error.py
--rw-r--r--   0        0        0     1339 2023-04-07 22:05:07.660376 fling_client-0.1.1/fling_client/models/read_data_fling_id_get_response_read_data_fling_id_get.py
--rw-r--r--   0        0        0     1323 2023-04-07 22:05:07.647403 fling_client-0.1.1/fling_client/models/read_index_index_get_response_read_index_index_get.py
--rw-r--r--   0        0        0     2091 2023-04-07 22:05:07.666992 fling_client-0.1.1/fling_client/models/validation_error.py
--rw-r--r--   0        0        0       25 2023-04-07 22:05:06.907242 fling_client-0.1.1/fling_client/py.typed
--rw-r--r--   0        0        0      974 2023-04-07 22:05:07.652872 fling_client-0.1.1/fling_client/types.py
--rw-r--r--   0        0        0      726 2023-04-07 22:11:13.977220 fling_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 fling_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-06 03:37:25.245135 fling_client-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0     3730 2023-04-05 23:18:00.740582 fling_client-0.1.4/README.md
+-rw-r--r--   0        0        0      149 2023-05-17 20:06:54.137357 fling_client-0.1.4/fling_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-17 20:06:53.456248 fling_client-0.1.4/fling_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:06:53.486509 fling_client-0.1.4/fling_client/api/data/__init__.py
+-rw-r--r--   0        0        0     6008 2023-05-17 20:06:54.194327 fling_client-0.1.4/fling_client/api/data/add_data_fling_id_add_post.py
+-rw-r--r--   0        0        0     5464 2023-05-17 20:06:54.194196 fling_client-0.1.4/fling_client/api/data/add_to_index_index_put.py
+-rw-r--r--   0        0        0     4398 2023-05-17 20:06:54.190193 fling_client-0.1.4/fling_client/api/data/get_repo_list_repolist_get.py
+-rw-r--r--   0        0        0     5299 2023-05-17 20:06:54.196157 fling_client-0.1.4/fling_client/api/data/read_data_fling_id_get.py
+-rw-r--r--   0        0        0     4939 2023-05-17 20:06:54.198829 fling_client-0.1.4/fling_client/api/data/read_index_index_get.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:06:53.464841 fling_client-0.1.4/fling_client/api/default/__init__.py
+-rw-r--r--   0        0        0     4519 2023-05-17 20:06:54.210836 fling_client-0.1.4/fling_client/api/default/github_code_callback_get.py
+-rw-r--r--   0        0        0     4265 2023-05-17 20:06:54.202376 fling_client-0.1.4/fling_client/api/default/github_login_github_login_get.py
+-rw-r--r--   0        0        0     2345 2023-05-17 20:06:54.192458 fling_client-0.1.4/fling_client/api/default/index_get.py
+-rw-r--r--   0        0        0     4532 2023-05-17 20:06:54.234993 fling_client-0.1.4/fling_client/api/default/token_to_web_callback_web_prod_get.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:06:53.483087 fling_client-0.1.4/fling_client/api/loophost/__init__.py
+-rw-r--r--   0        0        0     5769 2023-05-17 20:06:54.241754 fling_client-0.1.4/fling_client/api/loophost/add_txt_record_txt_record_put.py
+-rw-r--r--   0        0        0     5772 2023-05-17 20:06:54.239222 fling_client-0.1.4/fling_client/api/loophost/del_txt_record_txt_record_delete.py
+-rw-r--r--   0        0        0     5540 2023-05-17 20:06:54.245499 fling_client-0.1.4/fling_client/api/loophost/expose_app_expose_app_put.py
+-rw-r--r--   0        0        0        0 2023-05-17 20:06:53.485382 fling_client-0.1.4/fling_client/api/names/__init__.py
+-rw-r--r--   0        0        0     5510 2023-05-17 20:06:54.247772 fling_client-0.1.4/fling_client/api/names/generate_names_namer_get.py
+-rw-r--r--   0        0        0     2817 2023-05-17 20:06:54.220901 fling_client-0.1.4/fling_client/client.py
+-rw-r--r--   0        0        0      470 2023-05-17 20:06:54.205098 fling_client-0.1.4/fling_client/errors.py
+-rw-r--r--   0        0        0     1098 2023-05-17 20:06:53.839624 fling_client-0.1.4/fling_client/models/__init__.py
+-rw-r--r--   0        0        0     1375 2023-05-17 20:06:54.226763 fling_client-0.1.4/fling_client/models/add_data_fling_id_add_post_response_add_data_fling_id_add_post.py
+-rw-r--r--   0        0        0     1339 2023-05-17 20:06:54.221901 fling_client-0.1.4/fling_client/models/add_to_index_index_put_response_add_to_index_index_put.py
+-rw-r--r--   0        0        0     1363 2023-05-17 20:06:54.230958 fling_client-0.1.4/fling_client/models/generate_names_namer_get_response_generate_names_namer_get.py
+-rw-r--r--   0        0        0     2131 2023-05-17 20:06:54.248072 fling_client-0.1.4/fling_client/models/http_validation_error.py
+-rw-r--r--   0        0        0     1339 2023-05-17 20:06:54.239922 fling_client-0.1.4/fling_client/models/read_data_fling_id_get_response_read_data_fling_id_get.py
+-rw-r--r--   0        0        0     1323 2023-05-17 20:06:54.246141 fling_client-0.1.4/fling_client/models/read_index_index_get_response_read_index_index_get.py
+-rw-r--r--   0        0        0     2091 2023-05-17 20:06:54.252806 fling_client-0.1.4/fling_client/models/validation_error.py
+-rw-r--r--   0        0        0       25 2023-05-17 20:06:53.403201 fling_client-0.1.4/fling_client/py.typed
+-rw-r--r--   0        0        0      974 2023-05-17 20:06:54.250956 fling_client-0.1.4/fling_client/types.py
+-rw-r--r--   0        0        0      726 2023-05-17 22:09:41.668375 fling_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 fling_client-0.1.4/PKG-INFO
```

### Comparing `fling_client-0.1.1/README.md` & `fling_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/api/data/add_data_fling_id_add_post.py` & `fling_client-0.1.4/fling_client/api/loophost/expose_app_expose_app_put.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,204 +1,199 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.add_data_fling_id_add_post_response_add_data_fling_id_add_post import (
-    AddDataFlingIdAddPostResponseAddDataFlingIdAddPost,
-)
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Response
+from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    fling_id: str,
     *,
     client: Client,
-    key: str,
-    val: str,
+    app_name: str,
+    ssh_public_key: Union[Unset, None, str] = UNSET,
+    gh_token: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/{fling_id}/add".format(client.base_url, fling_id=fling_id)
+    url = "{}/expose_app".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    if not isinstance(gh_token, Unset):
+        headers["gh-token"] = gh_token
+
     params: Dict[str, Any] = {}
-    params["key"] = key
+    params["app_name"] = app_name
 
-    params["val"] = val
+    params["ssh_public_key"] = ssh_public_key
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
-        "method": "post",
+        "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, HTTPValidationError]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = AddDataFlingIdAddPostResponseAddDataFlingIdAddPost.from_dict(response.json())
-
+        response_200 = cast(Any, response.json())
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = HTTPValidationError.from_dict(response.json())
 
         return response_422
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, HTTPValidationError]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    fling_id: str,
     *,
     client: Client,
-    key: str,
-    val: str,
-) -> Response[Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]]:
-    """Add Data
+    app_name: str,
+    ssh_public_key: Union[Unset, None, str] = UNSET,
+    gh_token: Union[Unset, str] = UNSET,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Expose App
 
     Args:
-        fling_id (str):
-        key (str):
-        val (str):
+        app_name (str):
+        ssh_public_key (Union[Unset, None, str]):
+        gh_token (Union[Unset, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]]
+        Response[Union[Any, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
-        fling_id=fling_id,
         client=client,
-        key=key,
-        val=val,
+        app_name=app_name,
+        ssh_public_key=ssh_public_key,
+        gh_token=gh_token,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    fling_id: str,
     *,
     client: Client,
-    key: str,
-    val: str,
-) -> Optional[Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]]:
-    """Add Data
+    app_name: str,
+    ssh_public_key: Union[Unset, None, str] = UNSET,
+    gh_token: Union[Unset, str] = UNSET,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Expose App
 
     Args:
-        fling_id (str):
-        key (str):
-        val (str):
+        app_name (str):
+        ssh_public_key (Union[Unset, None, str]):
+        gh_token (Union[Unset, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]
+        Union[Any, HTTPValidationError]
     """
 
     return sync_detailed(
-        fling_id=fling_id,
         client=client,
-        key=key,
-        val=val,
+        app_name=app_name,
+        ssh_public_key=ssh_public_key,
+        gh_token=gh_token,
     ).parsed
 
 
 async def asyncio_detailed(
-    fling_id: str,
     *,
     client: Client,
-    key: str,
-    val: str,
-) -> Response[Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]]:
-    """Add Data
+    app_name: str,
+    ssh_public_key: Union[Unset, None, str] = UNSET,
+    gh_token: Union[Unset, str] = UNSET,
+) -> Response[Union[Any, HTTPValidationError]]:
+    """Expose App
 
     Args:
-        fling_id (str):
-        key (str):
-        val (str):
+        app_name (str):
+        ssh_public_key (Union[Unset, None, str]):
+        gh_token (Union[Unset, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]]
+        Response[Union[Any, HTTPValidationError]]
     """
 
     kwargs = _get_kwargs(
-        fling_id=fling_id,
         client=client,
-        key=key,
-        val=val,
+        app_name=app_name,
+        ssh_public_key=ssh_public_key,
+        gh_token=gh_token,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    fling_id: str,
     *,
     client: Client,
-    key: str,
-    val: str,
-) -> Optional[Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]]:
-    """Add Data
+    app_name: str,
+    ssh_public_key: Union[Unset, None, str] = UNSET,
+    gh_token: Union[Unset, str] = UNSET,
+) -> Optional[Union[Any, HTTPValidationError]]:
+    """Expose App
 
     Args:
-        fling_id (str):
-        key (str):
-        val (str):
+        app_name (str):
+        ssh_public_key (Union[Unset, None, str]):
+        gh_token (Union[Unset, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[AddDataFlingIdAddPostResponseAddDataFlingIdAddPost, HTTPValidationError]
+        Union[Any, HTTPValidationError]
     """
 
     return (
         await asyncio_detailed(
-            fling_id=fling_id,
             client=client,
-            key=key,
-            val=val,
+            app_name=app_name,
+            ssh_public_key=ssh_public_key,
+            gh_token=gh_token,
         )
     ).parsed
```

### Comparing `fling_client-0.1.1/fling_client/api/data/add_to_index_index_put.py` & `fling_client-0.1.4/fling_client/api/data/add_to_index_index_put.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/api/data/get_repo_list_repolist_get.py` & `fling_client-0.1.4/fling_client/api/data/get_repo_list_repolist_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/api/data/read_data_fling_id_get.py` & `fling_client-0.1.4/fling_client/api/data/read_data_fling_id_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/api/data/read_index_index_get.py` & `fling_client-0.1.4/fling_client/api/data/read_index_index_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/api/default/github_code_callback_get.py` & `fling_client-0.1.4/fling_client/api/default/github_code_callback_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/api/default/github_login_github_login_get.py` & `fling_client-0.1.4/fling_client/api/default/github_login_github_login_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/api/default/index_get.py` & `fling_client-0.1.4/fling_client/api/default/index_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/api/names/generate_names_namer_get.py` & `fling_client-0.1.4/fling_client/api/names/generate_names_namer_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/client.py` & `fling_client-0.1.4/fling_client/client.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/models/__init__.py` & `fling_client-0.1.4/fling_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/models/add_data_fling_id_add_post_response_add_data_fling_id_add_post.py` & `fling_client-0.1.4/fling_client/models/add_data_fling_id_add_post_response_add_data_fling_id_add_post.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/models/add_to_index_index_put_response_add_to_index_index_put.py` & `fling_client-0.1.4/fling_client/models/add_to_index_index_put_response_add_to_index_index_put.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/models/generate_names_namer_get_response_generate_names_namer_get.py` & `fling_client-0.1.4/fling_client/models/generate_names_namer_get_response_generate_names_namer_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/models/http_validation_error.py` & `fling_client-0.1.4/fling_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/models/read_data_fling_id_get_response_read_data_fling_id_get.py` & `fling_client-0.1.4/fling_client/models/read_data_fling_id_get_response_read_data_fling_id_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/models/read_index_index_get_response_read_index_index_get.py` & `fling_client-0.1.4/fling_client/models/read_index_index_get_response_read_index_index_get.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/models/validation_error.py` & `fling_client-0.1.4/fling_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/fling_client/types.py` & `fling_client-0.1.4/fling_client/types.py`

 * *Files identical despite different names*

### Comparing `fling_client-0.1.1/pyproject.toml` & `fling_client-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fling-client"
-version = "0.1.1"
+version = "0.1.4"
 description = "A client library for accessing fling"
 authors = ["Joshua McKenty <jmckenty@gmail.com>", "Anouk Ruhaak <anoukruhaak@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "fling_client"},
 ]
 include = ["CHANGELOG.md", "fling_client/py.typed"]
```

### Comparing `fling_client-0.1.1/PKG-INFO` & `fling_client-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-client
-Version: 0.1.1
+Version: 0.1.4
 Summary: A client library for accessing fling
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

