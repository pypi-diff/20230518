# Comparing `tmp/api-client-lnx-edge-0.3.2.tar.gz` & `tmp/api-client-lnx-edge-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ntulli/Leadnomics/edge-api-client/dist/.tmp-ps05jeni/api-client-lnx-edge-0.3.2.tar", last modified: Wed May 17 23:57:49 2023, max compression
+gzip compressed data, was "/Users/ntulli/Leadnomics/edge-api-client/dist/.tmp-87rdjv0n/api-client-lnx-edge-0.3.3.tar", last modified: Thu May 18 15:08:29 2023, max compression
```

## Comparing `api-client-lnx-edge-0.3.2.tar` & `api-client-lnx-edge-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/
--rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/PKG-INFO
--rw-r--r--   0 ntulli     (502) staff       (20)      738 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.2/README.md
--rw-r--r--   0 ntulli     (502) staff       (20)      100 2021-08-23 17:29:30.000000 api-client-lnx-edge-0.3.2/pyproject.toml
--rw-r--r--   0 ntulli     (502) staff       (20)       38 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/setup.cfg
--rw-r--r--   0 ntulli     (502) staff       (20)      767 2023-05-17 23:53:59.000000 api-client-lnx-edge-0.3.2/setup.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/
--rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/PKG-INFO
--rw-r--r--   0 ntulli     (502) staff       (20)      542 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/SOURCES.txt
--rw-r--r--   0 ntulli     (502) staff       (20)        1 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/dependency_links.txt
--rw-r--r--   0 ntulli     (502) staff       (20)       50 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/requires.txt
--rw-r--r--   0 ntulli     (502) staff       (20)       16 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/top_level.txt
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/
--rw-r--r--   0 ntulli     (502) staff       (20)       26 2022-10-11 15:31:34.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/__init__.py
--rw-r--r--   0 ntulli     (502) staff       (20)     1279 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/base.py
--rw-r--r--   0 ntulli     (502) staff       (20)    20333 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/edge.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/
--rw-r--r--   0 ntulli     (502) staff       (20)       90 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/__init__.py
--rw-r--r--   0 ntulli     (502) staff       (20)     2532 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/funcs.py
--rw-r--r--   0 ntulli     (502) staff       (20)     5044 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/schemas.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/tests/
--rw-r--r--   0 ntulli     (502) staff       (20)      322 2021-08-23 19:03:52.000000 api-client-lnx-edge-0.3.2/tests/test_auth.py
--rw-r--r--   0 ntulli     (502) staff       (20)     1074 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/tests/test_endpoints.py
--rw-r--r--   0 ntulli     (502) staff       (20)      810 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/tests/test_schemas.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/
+-rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/PKG-INFO
+-rw-r--r--   0 ntulli     (502) staff       (20)      738 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.3/README.md
+-rw-r--r--   0 ntulli     (502) staff       (20)      100 2021-08-23 17:29:30.000000 api-client-lnx-edge-0.3.3/pyproject.toml
+-rw-r--r--   0 ntulli     (502) staff       (20)       38 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/setup.cfg
+-rw-r--r--   0 ntulli     (502) staff       (20)      767 2023-05-18 15:08:15.000000 api-client-lnx-edge-0.3.3/setup.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/api_client_lnx_edge.egg-info/
+-rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/api_client_lnx_edge.egg-info/PKG-INFO
+-rw-r--r--   0 ntulli     (502) staff       (20)      542 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/api_client_lnx_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)        1 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/api_client_lnx_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)       50 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/api_client_lnx_edge.egg-info/requires.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)       16 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/api_client_lnx_edge.egg-info/top_level.txt
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/edge_api_client/
+-rw-r--r--   0 ntulli     (502) staff       (20)       26 2022-10-11 15:31:34.000000 api-client-lnx-edge-0.3.3/src/edge_api_client/__init__.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     1279 2023-05-17 23:59:37.000000 api-client-lnx-edge-0.3.3/src/edge_api_client/base.py
+-rw-r--r--   0 ntulli     (502) staff       (20)    20350 2023-05-18 15:07:57.000000 api-client-lnx-edge-0.3.3/src/edge_api_client/edge.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/src/edge_api_client/utilities/
+-rw-r--r--   0 ntulli     (502) staff       (20)       90 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.3/src/edge_api_client/utilities/__init__.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     2532 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.3/src/edge_api_client/utilities/funcs.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     5044 2023-05-18 13:50:37.000000 api-client-lnx-edge-0.3.3/src/edge_api_client/utilities/schemas.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-18 15:08:29.000000 api-client-lnx-edge-0.3.3/tests/
+-rw-r--r--   0 ntulli     (502) staff       (20)      322 2021-08-23 19:03:52.000000 api-client-lnx-edge-0.3.3/tests/test_auth.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     1042 2023-05-18 13:48:13.000000 api-client-lnx-edge-0.3.3/tests/test_endpoints.py
+-rw-r--r--   0 ntulli     (502) staff       (20)      810 2023-05-17 23:59:37.000000 api-client-lnx-edge-0.3.3/tests/test_schemas.py
```

### Comparing `api-client-lnx-edge-0.3.2/PKG-INFO` & `api-client-lnx-edge-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-client-lnx-edge
-Version: 0.3.2
+Version: 0.3.3
 Summary: Client for the LNX Edge API
 Home-page: https://github.com/Lnmix/edge_api_client
 Author: Nick Tulli
 Author-email: ntulli@leadnomics.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `api-client-lnx-edge-0.3.2/README.md` & `api-client-lnx-edge-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.2/setup.py` & `api-client-lnx-edge-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='api-client-lnx-edge',
-    version='0.3.2',
+    version='0.3.3',
     description='Client for the LNX Edge API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lnmix/edge_api_client',
     author='Nick Tulli',
     author_email='ntulli@leadnomics.com',
     package_dir={'': 'src'},
```

### Comparing `api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/PKG-INFO` & `api-client-lnx-edge-0.3.3/src/api_client_lnx_edge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-client-lnx-edge
-Version: 0.3.2
+Version: 0.3.3
 Summary: Client for the LNX Edge API
 Home-page: https://github.com/Lnmix/edge_api_client
 Author: Nick Tulli
 Author-email: ntulli@leadnomics.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/SOURCES.txt` & `api-client-lnx-edge-0.3.3/src/api_client_lnx_edge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.2/src/edge_api_client/base.py` & `api-client-lnx-edge-0.3.3/src/edge_api_client/base.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.2/src/edge_api_client/edge.py` & `api-client-lnx-edge-0.3.3/src/edge_api_client/edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,24 +433,24 @@
         """ Given an offer ID, return all approved affiliates.
 
         :param offer_id: an Edge offer ID
         :return: response object
         """
         return self._get('api/offers/{}/affiliates'.format(offer_id), **kwargs)
     
-    def update_affiliate_offer_settings(self, settings: dict, **kwargs) -> requests.Response:
+    def update_affiliate_offer_settings(self, settings: List[dict], **kwargs) -> requests.Response:
         """ Change an affiliate's aff+offer settings. Please see API docs for route PUT `/api/affiliate-offer-settings` 
         for a valid schema definition.
 
-        :param settings: new affiliate offer settings represented as JSON (a dictionary)
-        :type settings: dict
+        :param settings: new affiliate offer settings represented as JSON (a list of dicts)
+        :type settings: List[dict]
         :return: response object
         """
         if not settings:
-            settings = {}
+            settings = [{}]
 
         aos_schema = AffiliateOfferSettingsSchema(many=True)
         json_data = aos_schema.load(settings)
 
         return self._put('api/affiliate-offer-settings', json=aos_schema.dump(json_data), **kwargs)
     
     def change_affiliate_offer_approval(self, affiliate_id, offer_id, status: str, **kwargs):
```

### Comparing `api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/funcs.py` & `api-client-lnx-edge-0.3.3/src/edge_api_client/utilities/funcs.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/schemas.py` & `api-client-lnx-edge-0.3.3/src/edge_api_client/utilities/schemas.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.2/tests/test_endpoints.py` & `api-client-lnx-edge-0.3.3/tests/test_endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,11 +25,10 @@
     assert resp.status_code == 200
     assert resp.json()[0]['status'] == target_status
 
 
 def test_get_offer_approvals():
     resp = edge.get_offer_approvals(offer_id=310841)
     assert resp.status_code == 200
-    assert len(resp.json()) > 0
 
     bad_resp = affiliate_permissions.get_offer_approvals(offer_id=310841)
     assert bad_resp.status_code != 200
```

### Comparing `api-client-lnx-edge-0.3.2/tests/test_schemas.py` & `api-client-lnx-edge-0.3.3/tests/test_schemas.py`

 * *Files identical despite different names*

