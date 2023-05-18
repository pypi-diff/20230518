# Comparing `tmp/databar-0.5.0.tar.gz` & `tmp/databar-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databar-0.5.0.tar", last modified: Wed Feb  8 21:28:41 2023, max compression
+gzip compressed data, was "databar-0.6.0.tar", last modified: Thu May 18 14:58:25 2023, max compression
```

## Comparing `databar-0.5.0.tar` & `databar-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 adilet    (1000) adilet    (1000)        0 2023-02-08 21:28:41.947508 databar-0.5.0/
--rw-rw-r--   0 adilet    (1000) adilet    (1000)     1069 2022-06-16 18:09:25.000000 databar-0.5.0/LICENSE
--rw-rw-r--   0 adilet    (1000) adilet    (1000)       81 2022-06-16 18:09:25.000000 databar-0.5.0/MANIFEST.in
--rw-rw-r--   0 adilet    (1000) adilet    (1000)     1421 2023-02-08 21:28:41.947508 databar-0.5.0/PKG-INFO
--rw-rw-r--   0 adilet    (1000) adilet    (1000)     1089 2023-02-08 21:21:28.000000 databar-0.5.0/README.md
--rw-rw-r--   0 adilet    (1000) adilet    (1000)     1670 2023-02-08 21:28:41.948508 databar-0.5.0/setup.cfg
--rw-rw-r--   0 adilet    (1000) adilet    (1000)       86 2022-06-16 18:09:25.000000 databar-0.5.0/setup.py
-drwxrwxr-x   0 adilet    (1000) adilet    (1000)        0 2023-02-08 21:28:41.945508 databar-0.5.0/src/
-drwxrwxr-x   0 adilet    (1000) adilet    (1000)        0 2023-02-08 21:28:41.946508 databar-0.5.0/src/databar/
--rw-rw-r--   0 adilet    (1000) adilet    (1000)       96 2022-06-16 18:09:25.000000 databar-0.5.0/src/databar/__init__.py
--rw-rw-r--   0 adilet    (1000) adilet    (1000)    19173 2023-02-08 21:21:28.000000 databar-0.5.0/src/databar/connection.py
--rw-rw-r--   0 adilet    (1000) adilet    (1000)     2800 2022-12-07 17:06:57.000000 databar-0.5.0/src/databar/helpers.py
--rw-rw-r--   0 adilet    (1000) adilet    (1000)     9635 2022-12-07 17:06:57.000000 databar-0.5.0/src/databar/table.py
-drwxrwxr-x   0 adilet    (1000) adilet    (1000)        0 2023-02-08 21:28:41.947508 databar-0.5.0/src/databar.egg-info/
--rw-rw-r--   0 adilet    (1000) adilet    (1000)     1421 2023-02-08 21:28:41.000000 databar-0.5.0/src/databar.egg-info/PKG-INFO
--rw-rw-r--   0 adilet    (1000) adilet    (1000)      377 2023-02-08 21:28:41.000000 databar-0.5.0/src/databar.egg-info/SOURCES.txt
--rw-rw-r--   0 adilet    (1000) adilet    (1000)        1 2023-02-08 21:28:41.000000 databar-0.5.0/src/databar.egg-info/dependency_links.txt
--rw-rw-r--   0 adilet    (1000) adilet    (1000)      144 2023-02-08 21:28:41.000000 databar-0.5.0/src/databar.egg-info/requires.txt
--rw-rw-r--   0 adilet    (1000) adilet    (1000)        8 2023-02-08 21:28:41.000000 databar-0.5.0/src/databar.egg-info/top_level.txt
-drwxrwxr-x   0 adilet    (1000) adilet    (1000)        0 2023-02-08 21:28:41.947508 databar-0.5.0/tests/
--rw-rw-r--   0 adilet    (1000) adilet    (1000)        0 2022-06-16 18:09:25.000000 databar-0.5.0/tests/__init__.py
--rw-rw-r--   0 adilet    (1000) adilet    (1000)      274 2022-06-16 18:09:25.000000 databar-0.5.0/tests/test_metadata.py
--rw-rw-r--   0 adilet    (1000) adilet    (1000)     4770 2022-06-16 18:09:25.000000 databar-0.5.0/tests/test_table.py
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.771646 databar-0.6.0/
+-rw-r--r--   0 sadilet    (502) staff       (20)     1069 2023-05-18 14:36:56.000000 databar-0.6.0/LICENSE
+-rw-r--r--   0 sadilet    (502) staff       (20)       81 2023-05-18 14:36:56.000000 databar-0.6.0/MANIFEST.in
+-rw-r--r--   0 sadilet    (502) staff       (20)     1421 2023-05-18 14:58:25.771705 databar-0.6.0/PKG-INFO
+-rw-r--r--   0 sadilet    (502) staff       (20)     1089 2023-05-18 14:36:56.000000 databar-0.6.0/README.md
+-rw-r--r--   0 sadilet    (502) staff       (20)     1670 2023-05-18 14:58:25.772181 databar-0.6.0/setup.cfg
+-rw-r--r--   0 sadilet    (502) staff       (20)       86 2023-05-18 14:36:56.000000 databar-0.6.0/setup.py
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.769056 databar-0.6.0/src/
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.770582 databar-0.6.0/src/databar/
+-rw-r--r--   0 sadilet    (502) staff       (20)       96 2023-05-18 14:36:56.000000 databar-0.6.0/src/databar/__init__.py
+-rw-r--r--   0 sadilet    (502) staff       (20)    14089 2023-05-18 14:47:29.000000 databar-0.6.0/src/databar/connection.py
+-rw-r--r--   0 sadilet    (502) staff       (20)     2800 2023-05-18 14:36:56.000000 databar-0.6.0/src/databar/helpers.py
+-rw-r--r--   0 sadilet    (502) staff       (20)     9645 2023-05-18 14:36:56.000000 databar-0.6.0/src/databar/table.py
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.771165 databar-0.6.0/src/databar.egg-info/
+-rw-r--r--   0 sadilet    (502) staff       (20)     1421 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/PKG-INFO
+-rw-r--r--   0 sadilet    (502) staff       (20)      377 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/SOURCES.txt
+-rw-r--r--   0 sadilet    (502) staff       (20)        1 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/dependency_links.txt
+-rw-r--r--   0 sadilet    (502) staff       (20)      144 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/requires.txt
+-rw-r--r--   0 sadilet    (502) staff       (20)        8 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/top_level.txt
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.771523 databar-0.6.0/tests/
+-rw-r--r--   0 sadilet    (502) staff       (20)        0 2023-05-18 14:36:56.000000 databar-0.6.0/tests/__init__.py
+-rw-r--r--   0 sadilet    (502) staff       (20)      274 2023-05-18 14:36:56.000000 databar-0.6.0/tests/test_metadata.py
+-rw-r--r--   0 sadilet    (502) staff       (20)     4770 2023-05-18 14:36:56.000000 databar-0.6.0/tests/test_table.py
```

### Comparing `databar-0.5.0/LICENSE` & `databar-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databar-0.5.0/PKG-INFO` & `databar-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databar
-Version: 0.5.0
+Version: 0.6.0
 Summary: Official Databar.ai python package
 Home-page: https://github.com/databar-ai/databar-python
 Author: Databar.ai Team
 Author-email: founders@databar.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `databar-0.5.0/README.md` & `databar-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `databar-0.5.0/setup.cfg` & `databar-0.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 description = Official Databar.ai python package
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = databar
 url = https://github.com/databar-ai/databar-python
-version = 0.5.0
+version = 0.6.0
 
 [mypy]
 check_untyped_defs = True
 
 [mypy-aiohttp.*]
 ignore_missing_imports = True
 
@@ -70,15 +70,15 @@
 [options]
 include_package_data = True
 setup_requires = 
 	numpy==1.22.4
 install_requires = 
 	pandas==1.4.2
 	requests==2.28.2
-	aiohttp==3.8.1
+	aiohttp==3.8.4
 	tabulate==0.9.0
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 
 [options.extras_require]
```

### Comparing `databar-0.5.0/src/databar/connection.py` & `databar-0.6.0/src/databar/connection.py`

 * *Files 17% similar despite different names*

```diff
@@ -98,133 +98,14 @@
             if response_json["next"]:
                 print(f"There are more endpoints. Request next {page + 1} page.")
             else:
                 print("\nNo more endpoints there.")
         else:
             print("No endpoints found.")
 
-    def get_endpoint_docs(self, endpoint: str):
-        api, endpoint = endpoint.split("--", maxsplit=1)
-        response = self._session.post(
-            urljoin(self._base_url, "v1/dataset/retrieve/"),
-            json={"api": api, "dataset": endpoint},
-        )
-        raise_for_status(response)
-        endpoint_id = response.json()["id"]
-
-        params_response = self._session.get(
-            urljoin(self._base_url, f"v2/datasets/{endpoint_id}/params/")
-        )
-        raise_for_status(params_response)
-        headers_response = self._session.get(
-            urljoin(self._base_url, f"v1/dataset/{endpoint_id}/headers/")
-        )
-        raise_for_status(headers_response)
-
-        params_response_json = params_response.json()
-        headers_response_json = headers_response.json()
-
-        if params_response_json["authorization_is_required"]:
-            if params_response_json["oauth_based"]:
-                print(
-                    f"Authorization: This api uses OAuth2 for authorization. "
-                    f"Generate link to authorize via following code: "
-                    f"connection.authorize(api='{api}'). "
-                    f"To check existing keys call connection.api_keys(api='{api}')\n"
-                )
-            else:
-                print(
-                    f"Authorization: This api requires your own api key. "
-                    f"To add new one, please use next method: "
-                    f"connection.authorize(api='{api}', value='<your_api_key_here>'). "
-                    f"To check existing keys call connection.api_keys(api='{api}')\n"
-                )
-        else:
-            print("Authorization: No authorization required.\n")
-
-        if pagination := params_response_json["pagination"]:
-            if pagination["is_based_on_rows"]:
-                rows_count = pagination["rows_count_per_request"]
-                print(
-                    "Pagination: this endpoint pagination is based on rows. Default ",
-                    f"{rows_count} rows. Rows count must be multiple of {rows_count}, "
-                    f"e.g. {rows_count}, {rows_count * 2}, {rows_count * 3}, etc.\n",
-                )
-            else:
-                print(
-                    "Pagination: this endpoint pagination is page-based,"
-                    " e.g. 1, 2, 3, etc. Default 1.\n"
-                )
-        else:
-            print("Pagination: No pagination required.\n")
-
-        if params := params_response_json["params"]:
-            print("Input parameters:")
-            for param in params:
-                id_of_param = param.pop("id", None)
-                if param["type"] in ("choice", "multiplechoice"):
-                    param["description"] = (param["description"] or "").rstrip(".") + (
-                        f". To see all available choices call: "
-                        f"connection.get_choices(param_id={id_of_param})"
-                    )
-            print(tabulate(params, headers="keys", tablefmt="pretty"))
-        else:
-            print("Input parameters: No parameters required.\n")
-
-        if headers_response_json:
-            headers = [
-                {
-                    "name": header["inner_name_field"],
-                    "type": header["type_field"],
-                }
-                for header in headers_response_json
-            ]
-            print("\nResult columns:")
-            print(tabulate(headers, headers="keys", tablefmt="pretty"))
-        else:
-            print(
-                "Result columns: Houston, we have a problem, "
-                "there are no columns to return. Please, "
-                "contact our administrator at info@databar.ai"
-            )
-
-    def get_choices(
-        self, param_id: int, search_query: Optional[str] = None, page: int = 1
-    ):
-        q = ""
-        qr = ""
-        if search_query:
-            q = f"&search={search_query}"
-            qr = f", search query '{search_query}'"
-
-        response = self._session.get(
-            urljoin(
-                self._base_url, f"v1/request-param/{param_id}/options/?page={page}{q}"
-            ),
-        )
-        raise_for_status(response)
-        response_json = response.json()
-        options = response_json["result"]
-        if options:
-            print(f"Parameters: page {page}{qr}. {len(options)} results found.")
-            print(
-                tabulate(
-                    [
-                        {"id": option["id"], "name": option["name"]}
-                        for option in options
-                    ],
-                    headers="keys",
-                    tablefmt="pretty",
-                )
-            )
-            if response_json["next"]:
-                print(f"There are more endpoints. Request next {page + 1} page.")
-        else:
-            print("No choices found")
-
     def authorize(
         self,
         api: str,
         api_key_value: Optional[str] = None,
         name: Optional[str] = None,
     ):
         response = self._session.post(
@@ -336,34 +217,27 @@
             )
             raise_for_status(response)
             data = list(itertools.chain(*response.json().values()))
             if fmt == "json":
                 return data
             else:
                 return pd.DataFrame(data=data)
+        elif status == "no_data":
+            if fmt == "json":
+                return []
+            else:
+                return pd.DataFrame(data=[])
         elif status == "failed":
-            print("\nRequest failed. Check info below for details:")
             response = self._session.get(
                 urljoin(self._base_url, f"v3/request/{request_identifier}/meta/")
             )
             raise_for_status(response)
-            print(
-                tabulate(
-                    list(itertools.chain(*response.json().values())),
-                    headers="keys",
-                    tablefmt="pretty",
-                )
-            )
-            return None
+            return {"error": response.json()}
         else:
-            print(
-                "\nSomething went wrong. Unknown status of request. "
-                "Please, contact our administrator at info@databar.ai"
-            )
-            return None
+            raise ValueError(f"Unknown status: {status}")
 
     def enrich(
         self,
         df: pd.DataFrame,
         endpoint: str,
         mapping: Dict[str, str],
         api_key: Optional[int] = None,
```

### Comparing `databar-0.5.0/src/databar/helpers.py` & `databar-0.6.0/src/databar/helpers.py`

 * *Files identical despite different names*

### Comparing `databar-0.5.0/src/databar/table.py` & `databar-0.6.0/src/databar/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             f"https://databar.ai/api/v2/datasets/{self.dataset_id}/params/",
         )
         raise_for_status(response)
         return response.json()
 
     def calculate_price_of_request(
         self,
-        parameters: Dict[str, Any] = None,
+        parameters: Optional[Dict[str, Any]] = None,
         pagination: Optional[int] = None,
     ) -> float:
         """
         Calculates price of request in credits.
 
         :param parameters: Parameters which must be formed in according to dataset.
             Can be retrieved from :func:`~Table.get_params_of_dataset`.
```

### Comparing `databar-0.5.0/src/databar.egg-info/PKG-INFO` & `databar-0.6.0/src/databar.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databar
-Version: 0.5.0
+Version: 0.6.0
 Summary: Official Databar.ai python package
 Home-page: https://github.com/databar-ai/databar-python
 Author: Databar.ai Team
 Author-email: founders@databar.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `databar-0.5.0/tests/test_table.py` & `databar-0.6.0/tests/test_table.py`

 * *Files identical despite different names*

