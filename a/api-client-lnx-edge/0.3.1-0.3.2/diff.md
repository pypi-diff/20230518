# Comparing `tmp/api-client-lnx-edge-0.3.1.tar.gz` & `tmp/api-client-lnx-edge-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ntulli/Leadnomics/edge-api-client/dist/.tmp-2s374mv6/api-client-lnx-edge-0.3.1.tar", last modified: Mon May 15 18:13:19 2023, max compression
+gzip compressed data, was "/Users/ntulli/Leadnomics/edge-api-client/dist/.tmp-ps05jeni/api-client-lnx-edge-0.3.2.tar", last modified: Wed May 17 23:57:49 2023, max compression
```

## Comparing `api-client-lnx-edge-0.3.1.tar` & `api-client-lnx-edge-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/
--rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/PKG-INFO
--rw-r--r--   0 ntulli     (502) staff       (20)      738 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.1/README.md
--rw-r--r--   0 ntulli     (502) staff       (20)      100 2021-08-23 17:29:30.000000 api-client-lnx-edge-0.3.1/pyproject.toml
--rw-r--r--   0 ntulli     (502) staff       (20)       38 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/setup.cfg
--rw-r--r--   0 ntulli     (502) staff       (20)      767 2023-05-15 18:04:36.000000 api-client-lnx-edge-0.3.1/setup.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/
--rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/PKG-INFO
--rw-r--r--   0 ntulli     (502) staff       (20)      496 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/SOURCES.txt
--rw-r--r--   0 ntulli     (502) staff       (20)        1 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/dependency_links.txt
--rw-r--r--   0 ntulli     (502) staff       (20)       50 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/requires.txt
--rw-r--r--   0 ntulli     (502) staff       (20)       16 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/top_level.txt
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/
--rw-r--r--   0 ntulli     (502) staff       (20)       26 2022-10-11 15:31:34.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/__init__.py
--rw-r--r--   0 ntulli     (502) staff       (20)     1135 2022-10-22 18:30:37.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/base.py
--rw-r--r--   0 ntulli     (502) staff       (20)    18902 2023-05-15 18:01:45.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/edge.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/
--rw-r--r--   0 ntulli     (502) staff       (20)       90 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/__init__.py
--rw-r--r--   0 ntulli     (502) staff       (20)     2532 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/funcs.py
--rw-r--r--   0 ntulli     (502) staff       (20)     2446 2022-11-09 18:30:15.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/schemas.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/tests/
--rw-r--r--   0 ntulli     (502) staff       (20)      322 2021-08-23 19:03:52.000000 api-client-lnx-edge-0.3.1/tests/test_auth.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/
+-rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/PKG-INFO
+-rw-r--r--   0 ntulli     (502) staff       (20)      738 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.2/README.md
+-rw-r--r--   0 ntulli     (502) staff       (20)      100 2021-08-23 17:29:30.000000 api-client-lnx-edge-0.3.2/pyproject.toml
+-rw-r--r--   0 ntulli     (502) staff       (20)       38 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/setup.cfg
+-rw-r--r--   0 ntulli     (502) staff       (20)      767 2023-05-17 23:53:59.000000 api-client-lnx-edge-0.3.2/setup.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/
+-rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/PKG-INFO
+-rw-r--r--   0 ntulli     (502) staff       (20)      542 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)        1 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)       50 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/requires.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)       16 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/top_level.txt
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/
+-rw-r--r--   0 ntulli     (502) staff       (20)       26 2022-10-11 15:31:34.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/__init__.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     1279 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/base.py
+-rw-r--r--   0 ntulli     (502) staff       (20)    20333 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/edge.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/
+-rw-r--r--   0 ntulli     (502) staff       (20)       90 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/__init__.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     2532 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/funcs.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     5044 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/schemas.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-17 23:57:49.000000 api-client-lnx-edge-0.3.2/tests/
+-rw-r--r--   0 ntulli     (502) staff       (20)      322 2021-08-23 19:03:52.000000 api-client-lnx-edge-0.3.2/tests/test_auth.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     1074 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/tests/test_endpoints.py
+-rw-r--r--   0 ntulli     (502) staff       (20)      810 2023-05-17 23:52:30.000000 api-client-lnx-edge-0.3.2/tests/test_schemas.py
```

### Comparing `api-client-lnx-edge-0.3.1/PKG-INFO` & `api-client-lnx-edge-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-client-lnx-edge
-Version: 0.3.1
+Version: 0.3.2
 Summary: Client for the LNX Edge API
 Home-page: https://github.com/Lnmix/edge_api_client
 Author: Nick Tulli
 Author-email: ntulli@leadnomics.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `api-client-lnx-edge-0.3.1/README.md` & `api-client-lnx-edge-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.1/setup.py` & `api-client-lnx-edge-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='api-client-lnx-edge',
-    version='0.3.1',
+    version='0.3.2',
     description='Client for the LNX Edge API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lnmix/edge_api_client',
     author='Nick Tulli',
     author_email='ntulli@leadnomics.com',
     package_dir={'': 'src'},
```

### Comparing `api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/PKG-INFO` & `api-client-lnx-edge-0.3.2/src/api_client_lnx_edge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-client-lnx-edge
-Version: 0.3.1
+Version: 0.3.2
 Summary: Client for the LNX Edge API
 Home-page: https://github.com/Lnmix/edge_api_client
 Author: Nick Tulli
 Author-email: ntulli@leadnomics.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `api-client-lnx-edge-0.3.1/src/edge_api_client/base.py` & `api-client-lnx-edge-0.3.2/src/edge_api_client/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,17 @@
         return self._get(endpoint, append_url=append_url, **kwargs)
 
     def _get(self, endpoint='', append_url=True, **kwargs):
         return self._request('get', endpoint, append_url=append_url, **kwargs)
 
     def _post(self, endpoint='', append_url=True, **kwargs):
         return self._request('post', endpoint, append_url=append_url, **kwargs)
+    
+    def _put(self, endpoint='', append_url=True, **kwargs):
+        return self._request('put', endpoint, append_url=append_url, **kwargs)
 
     def _request(self, method, endpoint, params=None, data=None, append_url=True, **kwargs):
         url = self._build_url(endpoint) if append_url else self.base_url
         params = params or {}
         data = data or {}
 
         response = self.session.request(method, url, params=params, data=data, **kwargs)
```

### Comparing `api-client-lnx-edge-0.3.1/src/edge_api_client/edge.py` & `api-client-lnx-edge-0.3.2/src/edge_api_client/edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import requests
 from typing import List, Tuple
 from datetime import datetime, date
 
 from .base import BaseAPIClient
 from .utilities import get_dayparting, format_adjustment_date, build_filters, build_daterange
-from .utilities.schemas import CreateOfferSchema
+from .utilities.schemas import CreateOfferSchema, AffiliateOfferSettingsSchema
 
 
 class EdgeAPI(BaseAPIClient):
 
     def __init__(self, api_key=None, staging=False):
         super(EdgeAPI, self).__init__()
 
@@ -432,10 +432,43 @@
     def get_offer_approvals(self, offer_id, **kwargs) -> requests.Response:
         """ Given an offer ID, return all approved affiliates.
 
         :param offer_id: an Edge offer ID
         :return: response object
         """
         return self._get('api/offers/{}/affiliates'.format(offer_id), **kwargs)
+    
+    def update_affiliate_offer_settings(self, settings: dict, **kwargs) -> requests.Response:
+        """ Change an affiliate's aff+offer settings. Please see API docs for route PUT `/api/affiliate-offer-settings` 
+        for a valid schema definition.
+
+        :param settings: new affiliate offer settings represented as JSON (a dictionary)
+        :type settings: dict
+        :return: response object
+        """
+        if not settings:
+            settings = {}
+
+        aos_schema = AffiliateOfferSettingsSchema(many=True)
+        json_data = aos_schema.load(settings)
+
+        return self._put('api/affiliate-offer-settings', json=aos_schema.dump(json_data), **kwargs)
+    
+    def change_affiliate_offer_approval(self, affiliate_id, offer_id, status: str, **kwargs):
+        """ Change the application status on a specific offer for an affiliate. Please see API docs for 
+        route PUT `/api/affiliate-offer-settings` for a valid schema definition.
+
+        :param affiliate_id: an Edge affiliate ID
+        :param offer_id: an Edge offer ID
+        :param status: a valid application status. One of: Applied, Denied, Approved
+        :return: response object
+        """
+        body = [{
+            'affiliateId': affiliate_id,
+            'offerId': offer_id,
+            'status': status
+        }]
+
+        return self.update_affiliate_offer_settings(settings=body, **kwargs)
 
     def __repr__(self):
         return f'EdgeAPI(staging={self.staging})'
```

### Comparing `api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/funcs.py` & `api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/funcs.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/schemas.py` & `api-client-lnx-edge-0.3.2/src/edge_api_client/utilities/schemas.py`

 * *Files 27% similar despite different names*

```diff
@@ -59,7 +59,52 @@
     unsubscribe_link = marshmallow.fields.Str()
     suppression_list = marshmallow.fields.Str()
     from_lines = marshmallow.fields.Str()
     subject_lines = marshmallow.fields.Str()
     redirectOffer = marshmallow.fields.Int(allow_none=True)
     redirectPercent = marshmallow.fields.Float(allow_none=True)
     capRedirectOffer = marshmallow.fields.Int(allow_none=True)
+
+
+class AffiliateOfferSettingsSchema(marshmallow.Schema):
+    affiliateId = marshmallow.fields.Integer(required=True)
+    offerId = marshmallow.fields.Integer(required=True)
+    status = marshmallow.fields.String(validate=lambda s: s in ['Applied', 'Denied', 'Approved'], required=True)
+    trackingDomainOverride = marshmallow.fields.Integer(allow_none=True)
+    conversionCapOverride = marshmallow.fields.Integer(allow_none=True)
+    lifetimeClickCapOverride = marshmallow.fields.Integer(allow_none=True)
+    queryPassthroughOverride = marshmallow.fields.Boolean(allow_none=True)
+    offset = marshmallow.fields.Number(allow_none=True)
+    pixel = marshmallow.fields.String(allow_none=True)
+    pageview_pixel = marshmallow.fields.String(allow_none=True)
+    pageview_postbacks = marshmallow.fields.Dict(
+        keys=marshmallow.fields.Str(),
+        values=marshmallow.fields.List(marshmallow.fields.String(), allow_none=True),
+        allow_none=True
+    )
+    click_postbacks = marshmallow.fields.Dict(
+        keys=marshmallow.fields.Str(),
+        values=marshmallow.fields.List(marshmallow.fields.String(), allow_none=True),
+        allow_none=True
+    )
+    simplePixels = marshmallow.fields.List(marshmallow.fields.Dict(
+        pixelType=marshmallow.fields.String(validate=lambda s: s in ['FACEBOOK', 'TIKTOK']),
+        eventName=marshmallow.fields.String(),
+        eventSourceUrl=marshmallow.fields.String(),
+        pixelId=marshmallow.fields.String(),
+        accessToken=marshmallow.fields.String()
+    ), allow_none=True)
+    conversionEvents = marshmallow.fields.List(marshmallow.fields.Dict(
+        id=marshmallow.fields.Integer(required=True),
+        customerId=marshmallow.fields.String(required=True),
+        conversionActionId=marshmallow.fields.String(required=True)
+    ))
+    postback = marshmallow.fields.List(marshmallow.fields.String())
+    postbackMethods = marshmallow.fields.List(marshmallow.fields.String(validate=lambda s: s in ['GET', 'POST']))
+    postbackBodies = marshmallow.fields.List(marshmallow.fields.String(allow_none=True))
+    postbackHeaders = marshmallow.fields.List(marshmallow.fields.String(allow_none=True))
+    redirectOffer = marshmallow.fields.Integer(allow_none=True)
+    redirectPercent = marshmallow.fields.Float(validate=lambda f: 0 <= f <= 100, allow_none=True)
+    capRedirectOffer = marshmallow.fields.Integer(allow_none=True)
+    viewThrough = marshmallow.fields.List(marshmallow.fields.String())
+    skipPostbackWhenRevLessThan = marshmallow.fields.Number(allow_none=True)
+    mask_id = marshmallow.fields.String(allow_none=True)
```

