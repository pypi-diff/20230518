# Comparing `tmp/arthub_api-1.6.7.tar.gz` & `tmp/arthub_api-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.6.7.tar", last modified: Wed May 17 11:52:05 2023, max compression
+gzip compressed data, was "arthub_api-1.6.8.tar", last modified: Thu May 18 12:09:46 2023, max compression
```

## Comparing `arthub_api-1.6.7.tar` & `arthub_api-1.6.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 11:52:05.013626 arthub_api-1.6.7/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.7/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-05-17 11:52:05.012629 arthub_api-1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 11:52:04.989691 arthub_api-1.6.7/arthub_api/
--rw-rw-rw-   0        0        0      666 2023-05-15 09:23:22.000000 arthub_api-1.6.7/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3483 2023-05-16 10:40:32.000000 arthub_api-1.6.7/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.7/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.7/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.7/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    38742 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2070 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    23614 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.7/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.7/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.7/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.7/arthub_api/models.py
--rw-rw-rw-   0        0        0    42130 2023-05-17 11:50:58.000000 arthub_api-1.6.7/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.7/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.7/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:52:05.000660 arthub_api-1.6.7/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.7/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-17 11:52:04.000000 arthub_api-1.6.7/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.7/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 11:52:05.013626 arthub_api-1.6.7/setup.cfg
--rw-rw-rw-   0        0        0     2973 2023-05-16 11:29:25.000000 arthub_api-1.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:52:05.011632 arthub_api-1.6.7/tests/
--rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.7/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.7/tests/_utils.py
--rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.7/tests/conftest.py
--rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.7/tests/test_open_api.py
--rw-rw-rw-   0        0        0    17832 2023-05-16 10:40:32.000000 arthub_api-1.6.7/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.7/tests/test_storage.py
--rw-rw-rw-   0        0        0     4290 2023-05-17 11:50:58.000000 arthub_api-1.6.7/tests/test_storage_blade.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:09:46.204836 arthub_api-1.6.8/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.8/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-05-18 12:09:46.204836 arthub_api-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 12:09:46.181896 arthub_api-1.6.8/arthub_api/
+-rw-rw-rw-   0        0        0      645 2023-05-18 12:05:48.000000 arthub_api-1.6.8/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3483 2023-05-16 10:40:32.000000 arthub_api-1.6.8/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-05-18 12:05:48.000000 arthub_api-1.6.8/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.8/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.8/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.8/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    42964 2023-05-18 12:05:48.000000 arthub_api-1.6.8/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2070 2023-05-17 11:50:58.000000 arthub_api-1.6.8/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    26249 2023-05-18 12:05:48.000000 arthub_api-1.6.8/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.8/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.8/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.8/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.8/arthub_api/models.py
+-rw-rw-rw-   0        0        0    42130 2023-05-17 11:50:58.000000 arthub_api-1.6.8/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.8/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.8/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:09:46.192868 arthub_api-1.6.8/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.8/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      108 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 12:09:45.000000 arthub_api-1.6.8/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.8/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 12:09:46.204836 arthub_api-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     2973 2023-05-16 11:29:25.000000 arthub_api-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 12:09:46.202907 arthub_api-1.6.8/tests/
+-rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.8/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.8/tests/_utils.py
+-rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.8/tests/conftest.py
+-rw-rw-rw-   0        0        0     6110 2023-05-18 07:59:55.000000 arthub_api-1.6.8/tests/test_open_api.py
+-rw-rw-rw-   0        0        0    17906 2023-05-18 12:05:48.000000 arthub_api-1.6.8/tests/test_open_api_blade.py
+-rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.8/tests/test_storage.py
+-rw-rw-rw-   0        0        0     6853 2023-05-18 12:05:48.000000 arthub_api-1.6.8/tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.7/LICENSE` & `arthub_api-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/PKG-INFO` & `arthub_api-1.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.6.7
+Version: 1.6.8
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.7/README.md` & `arthub_api-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/__init__.py` & `arthub_api-1.6.8/arthub_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     __copyright__,
     __description__,
     __license__,
     __title__,
     __url__,
     __version__,
 )
-from . import utils
 from .__main__ import init_config
 
 from .open_api import (
     OpenAPI,
     APIResponse
 )
```

### Comparing `arthub_api-1.6.7/arthub_api/__main__.py` & `arthub_api-1.6.8/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/_internal_utils.py` & `arthub_api-1.6.8/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/asset_matrix.py` & `arthub_api-1.6.8/arthub_api/asset_matrix.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/blade_api.py` & `arthub_api-1.6.8/arthub_api/blade_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,18 @@
         return "%s//%s/blade/blade/openapi/%s/thm/%s" % (
             self.http_scheme, self.api_host, self._api_version_blade, api_method)
 
     def _blade_resolving_url(self, api_method):
         return "%s//%s/resolving/resolving/openapi/%s/core/%s" % (
             self.http_scheme, self.api_host, self._api_version_blade, api_method)
 
+    def _blade_resolving_sign_url(self, api_method):
+        return "%s//%s/resolving/resolving/openapi/%s/sign/%s" % (
+            self.http_scheme, self.api_host, self._api_version_blade, api_method)
+
     def add_headers(self, headers):
         if self.blade_public_token != "":
             headers["blade-public-token"] = self.blade_public_token
 
     def has_credential(self):
         r"""Checks if credential is already set or not for Blade"""
         # public_token from pan is not valid credential for blade
@@ -1023,7 +1027,97 @@
         :rtype: arthub_api.APIResponse
             result: (number) count of packages
         """
         url = self._blade_resolving_url("get-package-count")
         res = self._make_api_request(url, {})
         res.set_result_by_key("count")
         return res
+
+    def blade_upload_sign(self, items, force=False):
+        r"""
+        :param items: List[dict]. [{"cos_key": str, "expired": 1200}, ...]
+        :param force: bool. example: false. default: false
+        :rtype: arthub_api.APIResponse
+            [{"signed_url": str, "origin_url": str}, ...]
+            result length should match input items length.
+            signed_url is used for PUT request, see more at s3 PutObject
+        """
+        url = self._blade_resolving_sign_url("upload")
+        return self._make_api_request(url, {"items": items, "force": force})
+
+    def blade_begin_multipart_upload_sign(self, items, force=False):
+        r"""
+        :param items: List[dict]. [{"cos_key": str, "expired": 1200}, ...]
+        :param force: bool. example: false. default: false
+        :rtype: arthub_api.APIResponse
+            [{"signed_url": str, "origin_url": str}, ...]
+            result length should match input items length.
+            signed_url is used for POST request, see more at s3 CreateMultipartUpload
+            after POST request, you should obtain a `upload_id` str
+        """
+        url = self._blade_resolving_sign_url("begin-multipart-upload")
+        return self._make_api_request(url, {"items": items, "force": force})
+
+    def blade_part_upload_sign(self, items, force=False):
+        r"""
+        :param items: List[dict]. 
+            [{
+                "cos_key": str,
+                "expired": 1200,
+                "upload_id": "16835262901cf8ebac376ade701dd7ce4ce881a32799ab71ad2297f4ef8660a9f68d9e6d2c",
+                "part_number":1
+            }, ...]
+        :param force: bool. example: false. default: false
+        :rtype: arthub_api.APIResponse
+            [{
+                "signed_url": str, 
+                "origin_url": str,
+                "upload_id": "16835262901cf8ebac376ade701dd7ce4ce881a32799ab71ad2297f4ef8660a9f68d9e6d2c",
+                "part_number":1
+            }, ...]
+            result length should match input items length.
+            part_number starts from 1.
+            signed_url is used for PUT request, see more at s3 UploadPart
+            after PUT request, you should obtain a `ETag` header for this part
+        """
+        url = self._blade_resolving_sign_url("part-upload")
+        return self._make_api_request(url, {"items": items, "force": force})
+
+    def blade_complete_multipart_upload_sign(self, items, force=False):
+        r"""
+        :param items: List[dict].
+            [{
+                "cos_key": str,
+                "expired": 1200,
+                "upload_id": "16835262901cf8ebac376ade701dd7ce4ce881a32799ab71ad2297f4ef8660a9f68d9e6d2c",
+            }, ...]
+        :param force: bool. example: false. default: false
+        :rtype: arthub_api.APIResponse
+            [{
+                "signed_url": str, 
+                "origin_url": str,
+                "upload_id": "16835262901cf8ebac376ade701dd7ce4ce881a32799ab71ad2297f4ef8660a9f68d9e6d2c"
+            }, ...]
+            result length should match input items length.
+            signed_url is used for POST request, see more at s3 CompleteMultipartUpload
+            ETag and PartNumber should be set in POST body
+        """
+        url = self._blade_resolving_sign_url("complete-multipart-upload")
+        return self._make_api_request(url, {"items": items, "force": force})
+
+    def blade_download_sign(self, items):
+        r"""
+        :param items: List[dict].
+            [{
+                "cos_key": str,
+                "expired": 1200
+            }, ...]
+        :rtype: arthub_api.APIResponse
+            [{
+                "signed_url": str, 
+                "origin_url": str,
+                "size": 1601
+            }, ...]
+            size is bytes size of existed file, useful for multipart download
+        """
+        url = self._blade_resolving_sign_url("download")
+        return self._make_api_request(url, {"items": items})
```

### Comparing `arthub_api-1.6.7/arthub_api/blade_api_instance.py` & `arthub_api-1.6.8/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/blade_storage.py` & `arthub_api-1.6.8/arthub_api/blade_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     class FileNotFoundError(IOError):
         pass
 
 class SignerError(RuntimeError):
     pass
 
 # signer for blade api
-class RemoteSigner(object):    
+class RemoteSignerForPackage(object):    
     def __init__(self, blade_backend, force=False):
         self.cli = blade_backend
         self.force = force
         
     @classmethod
     def _remove_suffix(cls, s, sf):
         if s.endswith(sf):
@@ -67,66 +67,118 @@
             return {}
         result[4] = cls._remove_suffix(result[4], ".7z")
         if result[2] != result[4]:
             return {}
         return {"name": result[2], "version": result[3]}
     
     def _take_signed_url(self, arthub_response, type_of_sign=""):
-        if not arthub_response.is_succeeded():
-            raise SignerError("arthub api: {0}".format(str(arthub_response.errors)))
+        arthub_response.raise_for_err()
         logger.debug('{0} sign-url rsp is {1}'.format(type_of_sign, arthub_response.result))
         if len(arthub_response.result) == 0:
             raise SignerError("arthub api: result is empty")
         return "https:" + arthub_response.result[0].get('signed_url')
         
     # we use bucket + key to identify a file. 
     # however bucket might be fixed for ArtHub condition, so bucket input is ignored
-    def _get_package_download_sign(self, bucket, key):
+    # pkg do not supports for expired argument
+    def _get_package_download_sign(self, bucket, key, expired=1200):
         pkg = self._key_to_pkg(key)
         # this will return a url expires in 10 minutes
         signed = self.cli.blade_download_package([pkg])
-        if not signed.is_succeeded():
-            raise SignerError("arthub api: {0}".format(str(signed.errors)))
+        signed.raise_for_err()
+        if len(signed.result) == 0:
+            raise SignerError("arthub api: result is empty")
         logger.debug("download sign-url rsp is {0}".format(signed.result))
         return signed.result
     
-    def get_download_url(self, bucket, key):
-        signed = self._get_package_download_sign(bucket, key)
-        if len(signed) == 0:
-            raise SignerError("arthub api: result is empty")
+    # pkg do not supports for expired argument
+    def get_download_url(self, bucket, key, expired=1200):
+        signed = self._get_package_download_sign(bucket, key, expired)
         return "https:" + signed[0].get('signed_url')
         
     def get_file_size(self, bucket, key):
         signed = self._get_package_download_sign(bucket, key)
-        if len(signed) == 0:
-            raise SignerError("arthub api: result is empty")
         return signed[0].get('size')
     
-    def get_upload_url(self, bucket, key):
+    def get_upload_url(self, bucket, key, expired=1200):
         pkg = self._key_to_pkg(key)
         signed = self.cli.blade_upload_package([pkg], self.force)
         return self._take_signed_url(signed, "upload")
     
-    def get_begin_multipart_upload_url(self, bucket, key):
+    def get_begin_multipart_upload_url(self, bucket, key, expired=1200):
         pkg = self._key_to_pkg(key)
         signed = self.cli.blade_begin_multipart_package_upload([pkg], self.force)
         return self._take_signed_url(signed, "begin multipart upload")
     
-    def get_upload_part_url(self, bucket, key, upload_id, part_number):
+    def get_upload_part_url(self, bucket, key, upload_id, part_number, expired=1200):
         pkg = self._key_to_pkg(key)
         pkg.update({"upload_id": upload_id, "part_number": part_number})
         signed = self.cli.blade_part_package_upload([pkg], self.force)
         return self._take_signed_url(signed, "upload part")
     
-    def get_complete_multipart_upload_url(self, bucket, key, upload_id):
+    def get_complete_multipart_upload_url(self, bucket, key, upload_id, expired=1200):
         pkg = self._key_to_pkg(key)
         pkg.update({"upload_id": upload_id})
         signed = self.cli.blade_complete_multipart_package_upload([pkg], self.force)
         return self._take_signed_url(signed, "end multipart upload")
 
+class RemoteSigner(object):    
+    def __init__(self, blade_backend, force=False):
+        self.cli = blade_backend
+        self.force = force
+
+    def _take_signed_url(self, arthub_response, type_of_sign=""):
+        arthub_response.raise_for_err()
+        logger.debug('{0} sign-url rsp is {1}'.format(type_of_sign, arthub_response.result))
+        if len(arthub_response.result) == 0:
+            raise SignerError("arthub api: result is empty")
+        return "https:" + arthub_response.result[0].get('signed_url')
+        
+    # we use bucket + key to identify a file. 
+    # however bucket might be fixed for ArtHub condition, so bucket input is ignored
+    def _get_download_sign(self, bucket, key, expired=1200):
+        # this will return a url expires in 10 minutes
+        signed = self.cli.blade_download_sign([{"cos_key": key, "expired": expired}])
+        signed.raise_for_err()
+        if len(signed.result) == 0:
+            raise SignerError("arthub api: result is empty")
+        logger.debug("download sign-url rsp is {0}".format(signed.result))
+        return signed.result
+    
+    def get_download_url(self, bucket, key, expired=1200):
+        signed = self._get_download_sign(bucket, key, expired)
+        return "https:" + signed[0].get('signed_url')
+        
+    def get_file_size(self, bucket, key):
+        signed = self._get_download_sign(bucket, key)
+        size = signed[0].get('size')
+        if not size:
+            return 0
+        return size
+    
+    def get_upload_url(self, bucket, key, expired=1200):
+        item = {"cos_key": key, "expired": expired}
+        signed = self.cli.blade_upload_sign([item], self.force)
+        return self._take_signed_url(signed, "upload")
+    
+    def get_begin_multipart_upload_url(self, bucket, key, expired=1200):
+        item = {"cos_key": key, "expired": expired}
+        signed = self.cli.blade_begin_multipart_upload_sign([item], self.force)
+        return self._take_signed_url(signed, "begin multipart upload")
+    
+    def get_upload_part_url(self, bucket, key, upload_id, part_number, expired=1200):
+        item = {"cos_key": key, "expired": expired, "upload_id": upload_id, "part_number": part_number}
+        signed = self.cli.blade_part_upload_sign([item], self.force)
+        return self._take_signed_url(signed, "upload part")
+    
+    def get_complete_multipart_upload_url(self, bucket, key, upload_id, expired=1200):
+        item = {"cos_key": key, "expired": expired, "upload_id": upload_id}
+        signed = self.cli.blade_complete_multipart_upload_sign([item], self.force)
+        return self._take_signed_url(signed, "end multipart upload")
+
 
 class ProgressCallback():
     def __init__(self, file_size, progress_callback):
         self.__lock = threading.Lock()
         self.__finished_size = 0
         self.__file_size = file_size
         self.__progress_callback = progress_callback
@@ -486,24 +538,25 @@
             part_number.text = str(item[0])
         return ElementTree.tostring(root)
 
 class BladeCOSApi(object):
     """API to access THM pipeline installers on Blade storage."""
     # user input:
     def __init__(self, api, force=False, retry=3, cli=None, signer=None):
-        self.api = api
         self.force = force
         self.retry = retry
         self.signer = signer
         self.cli = cli
         self.logger = logging.getLogger(__name__)
-        if self.signer is None:
-            self.signer = RemoteSigner(self.api, self.force)
-        if self.cli is None:
-            self.cli = Client(self.signer)
+        if signer is None:
+            signer = RemoteSignerForPackage(api, force)
+        self.signer = signer
+        if cli is None:
+            cli = Client(signer)
+        self.cli = cli
 
     def check_file_exist(self, server_path):
         try:
             return self.cli.check_exists("", server_path)
         except ValueError:
             return False
```

### Comparing `arthub_api-1.6.7/arthub_api/config.py` & `arthub_api-1.6.8/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/exception.py` & `arthub_api-1.6.8/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/models.py` & `arthub_api-1.6.8/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/open_api.py` & `arthub_api-1.6.8/arthub_api/open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/storage.py` & `arthub_api-1.6.8/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api/utils.py` & `arthub_api-1.6.8/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.6.8/arthub_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.6.7
+Version: 1.6.8
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.7/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.6.8/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/setup.py` & `arthub_api-1.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/tests/test_open_api.py` & `arthub_api-1.6.8/tests/test_open_api.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-import arthub_api
-import pytest
-import logging
-from arthub_api import arthub_api_config
-from . import _utils
-from arthub_api import (
-    OpenAPI,
-    utils
-)
-
-TEST_DEPOT_NAME = "apg"
-
-open_api = None
-
-
-def on_api_failed(res):
-    logging.error("[TEST][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
-
-
-@pytest.mark.run(order=1)
-def test_init(env):
-    global open_api
-    _c = _utils.get_config(env)
-    open_api = OpenAPI(_c, False)
-    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        pytest.exit("login failed, exit test", returncode=1)
-
-    logging.info("[TEST][API] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
-
-
-def test_depot_get_root_id():
-    res = open_api.depot_get_root_id(TEST_DEPOT_NAME)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, depot id: %d" % (res.url, res.results.get(0)))
-
-
-def test_depot_get_node_brief_by_ids():
-    res = open_api.depot_get_node_brief_by_ids(TEST_DEPOT_NAME, [120347220059298, 120347220059299])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node_1 = res.results.get(0)
-    node_2 = res.results.get(1)
-    logging.info("[TEST][API] \"%s\" success, name_1: %s, name_2: %s" % (res.url, node_1["name"], node_2["name"]))
-
-
-def test_depot_get_child_node_count():
-    res = open_api.depot_get_child_node_count(TEST_DEPOT_NAME, [120347220059339])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, count: %d" % (res.url, res.results.get(0)["count"]))
-
-
-def test_depot_get_download_signature():
-    res = open_api.depot_get_download_signature(TEST_DEPOT_NAME,
-                                                nodes=[{"object_id": 120347220059338, "object_meta": "origin_url"}])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res.url, res.results.get(0)["signed_url"]))
-
-
-def test_depot_get_upload_signature():
-    file_name = "new_asset_to_upload"
-    res_0 = open_api.depot_create_asset(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": file_name,
-        "add_new_version": False
-    }])
-    if not res_0.is_succeeded():
-        on_api_failed(res_0)
-        assert 0
-
-    asset_id = res_0.results.get(0)["id"]
-
-    res_1 = open_api.depot_get_upload_signature(TEST_DEPOT_NAME, nodes=[
-        {"object_id": asset_id, "object_meta": "origin_url", "file_name": file_name}])
-    if not res_1.is_succeeded():
-        on_api_failed(res_1)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res_1.url, res_1.results.get(0)["signed_url"]))
-
-
-def test_depot_get_child_node_id_in_range():
-    res = open_api.depot_get_child_node_id_in_range(TEST_DEPOT_NAME, parent_id=120347220059339, offset=0, count=2,
-                                                    query_filters=[{"meta": "type", "condition": "x != directory"}],
-                                                    is_recursive=True)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    nodes = res.results.get(0)["nodes"]
-    logging.info("[TEST][API] \"%s\" success" % res.url)
-
-
-def test_depot_get_node_brief_by_path():
-    res = open_api.depot_get_node_brief_by_path(TEST_DEPOT_NAME, root_id=120347220059296,
-                                                path="open_api_test/asset.jpg")
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node = res.results.get(0)
-    logging.info("[TEST][API] \"%s\" success, name: %s" % (res.url, node["name"]))
-
-
-def test_depot_add_asset_tag():
-    res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=[utils.get_random_string(5)])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    node = res.results.get(0)
-    logging.info("[TEST][API] \"%s\" success, tag id: %d" % (res.url, node))
-
-
-def test_get_account_detail():
-    res = open_api.get_account_detail()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, email: %s" % (res.url, res.results.get(0)["email"]))
-
-
-def test_get_ticket():
-    res = open_api.get_ticket()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, ticket: %s" % (res.url, res.results.get(0)))
-
-
-def test_get_last_access_location_by_account():
-    res = open_api.get_last_access_location_by_account()
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, last access location: %s" % (res.url, res.results.get(0)))
-
-
-def test_depot_create_directory():
-    res = open_api.depot_create_directory(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": "new_dir",
-        "allowed_rename": True,
-        "return_existing_id": False
-    }])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, new dir id: %s" % (res.url, res.results.get(0)["id"]))
-
-
-def test_depot_create_multi_asset():
-    res = open_api.depot_create_multi_asset(TEST_DEPOT_NAME, [{
-        "parent_id": 120347220059339,
-        "name": "new_multi_asset"
-    }])
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success, new multi asset id: %s" % (res.url, res.results.get(0)["id"]))
-
-
-def test_depot_move_node():
-    res = open_api.depot_move_node(TEST_DEPOT_NAME, ids=[120347220064827], other_parent_id=120347220064825)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        assert 0
-
-    logging.info("[TEST][API] \"%s\" success" % res.url)
+import arthub_api
+import pytest
+import logging
+from arthub_api import arthub_api_config
+from . import _utils
+from arthub_api import (
+    OpenAPI,
+    utils
+)
+
+TEST_DEPOT_NAME = "apg"
+
+open_api = None
+
+
+def on_api_failed(res):
+    logging.error("[TEST][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
+
+
+@pytest.mark.run(order=1)
+def test_init(env):
+    global open_api
+    _c = _utils.get_config(env)
+    open_api = OpenAPI(_c, False)
+    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        pytest.exit("login failed, exit test", returncode=1)
+
+    logging.info("[TEST][API] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
+
+
+def test_depot_get_root_id():
+    res = open_api.depot_get_root_id(TEST_DEPOT_NAME)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, depot id: %d" % (res.url, res.results.get(0)))
+
+
+def test_depot_get_node_brief_by_ids():
+    res = open_api.depot_get_node_brief_by_ids(TEST_DEPOT_NAME, [120347220059298, 120347220059299])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node_1 = res.results.get(0)
+    node_2 = res.results.get(1)
+    logging.info("[TEST][API] \"%s\" success, name_1: %s, name_2: %s" % (res.url, node_1["name"], node_2["name"]))
+
+
+def test_depot_get_child_node_count():
+    res = open_api.depot_get_child_node_count(TEST_DEPOT_NAME, [120347220059339])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, count: %d" % (res.url, res.results.get(0)["count"]))
+
+
+def test_depot_get_download_signature():
+    res = open_api.depot_get_download_signature(TEST_DEPOT_NAME,
+                                                nodes=[{"object_id": 120347220059338, "object_meta": "origin_url"}])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res.url, res.results.get(0)["signed_url"]))
+
+
+def test_depot_get_upload_signature():
+    file_name = "new_asset_to_upload"
+    res_0 = open_api.depot_create_asset(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": file_name,
+        "add_new_version": False
+    }])
+    if not res_0.is_succeeded():
+        on_api_failed(res_0)
+        assert 0
+
+    asset_id = res_0.results.get(0)["id"]
+
+    res_1 = open_api.depot_get_upload_signature(TEST_DEPOT_NAME, nodes=[
+        {"object_id": asset_id, "object_meta": "origin_url", "file_name": file_name}])
+    if not res_1.is_succeeded():
+        on_api_failed(res_1)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res_1.url, res_1.results.get(0)["signed_url"]))
+
+
+def test_depot_get_child_node_id_in_range():
+    res = open_api.depot_get_child_node_id_in_range(TEST_DEPOT_NAME, parent_id=120347220059339, offset=0, count=2,
+                                                    query_filters=[{"meta": "type", "condition": "x != directory"}],
+                                                    is_recursive=True)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    nodes = res.results.get(0)["nodes"]
+    logging.info("[TEST][API] \"%s\" success" % res.url)
+
+
+def test_depot_get_node_brief_by_path():
+    res = open_api.depot_get_node_brief_by_path(TEST_DEPOT_NAME, root_id=120347220059296,
+                                                path="open_api_test/asset.jpg")
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node = res.results.get(0)
+    logging.info("[TEST][API] \"%s\" success, name: %s" % (res.url, node["name"]))
+
+
+def test_depot_add_asset_tag():
+    res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=[utils.get_random_string(5)])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    node = res.results.get(0)
+    logging.info("[TEST][API] \"%s\" success, tag id: %d" % (res.url, node))
+
+
+def test_get_account_detail():
+    res = open_api.get_account_detail()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, email: %s" % (res.url, res.results.get(0)["email"]))
+
+
+def test_get_ticket():
+    res = open_api.get_ticket()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, ticket: %s" % (res.url, res.results.get(0)))
+
+
+def test_get_last_access_location_by_account():
+    res = open_api.get_last_access_location_by_account()
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, last access location: %s" % (res.url, res.results.get(0)))
+
+
+def test_depot_create_directory():
+    res = open_api.depot_create_directory(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": "new_dir",
+        "allowed_rename": True,
+        "return_existing_id": False
+    }])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, new dir id: %s" % (res.url, res.results.get(0)["id"]))
+
+
+def test_depot_create_multi_asset():
+    res = open_api.depot_create_multi_asset(TEST_DEPOT_NAME, [{
+        "parent_id": 120347220059339,
+        "name": "new_multi_asset"
+    }])
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success, new multi asset id: %s" % (res.url, res.results.get(0)["id"]))
+
+
+def test_depot_move_node():
+    res = open_api.depot_move_node(TEST_DEPOT_NAME, ids=[120347220064827], other_parent_id=120347220064825)
+    if not res.is_succeeded():
+        on_api_failed(res)
+        assert 0
+
+    logging.info("[TEST][API] \"%s\" success" % res.url)
```

### Comparing `arthub_api-1.6.7/tests/test_open_api_blade.py` & `arthub_api-1.6.8/tests/test_open_api_blade.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,14 +529,16 @@
     # get 2
     res = blade_api.blade_get_package(name="arthub_test_pkg", version="0.0.1")
     assert res.is_succeeded()
     pkg_info_2 = res.result
     del pkg_info_2["api_modified"]
     
     # cmp
+    del pkg_info_1["downloads_url"]
+    del pkg_info_2["downloads_url"]
     assert pkg_info_1 == pkg_info_2
     assert pkg_info_2.get("tools") == ["no-tools"]
     logging.info("[TEST][API] edit package success: %s" % pkg_info)
 
     # download
     res = blade_api.blade_download_package([{"name":pkg_info.get("name"), "version":pkg_info.get("version")}])
     assert res.is_succeeded()
```

### Comparing `arthub_api-1.6.7/tests/test_storage.py` & `arthub_api-1.6.8/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.7/tests/test_storage_blade.py` & `arthub_api-1.6.8/tests/test_storage_blade.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from __future__ import print_function
 
 import arthub_api
 import pytest
 import sys
 import logging
 from arthub_api import arthub_api_config
+from arthub_api.blade_storage import RemoteSigner
+from arthub_api.open_api import APIError
 from . import _utils
 import requests
 import os
 from arthub_api import (
     BladeAPI,
     Client,
     BladeCOSApi,
@@ -76,15 +78,15 @@
     target = "pkg_distribution/7z/arthub_test_pkg/0.0.1/arthub_test_pkg.7z"
     source = os.path.join(str(tmp_path), "tmp.7z")
         
     cli = BladeCOSApi(api=blade_api)
     cli.download_file(target,source)
     try:
         cli.upload_file(target, source)
-    except RuntimeError:
+    except APIError:
         # expected condition:
         return
     # package should already uploaded, an error should be raised
     assert False 
 
 def test_blade_check_exists(env, tmp_path):
     blade_api = init_api(env)
@@ -118,8 +120,71 @@
     target = "pkg_distribution/7z/arthub_test_pkg/0.0.1/arthub_test_pkg.7z"
     def print_percent1(a, b):
         print_percent(a, b)
         if a > b/2:
             import os
             os.exit(1)
     cli.upload_file(target, source, print_percent)
+    
+# tests for general signer
+
+def test_blade_downloader_general_signer(env, tmp_path):
+    blade_api = init_api(env)
+    target = "test_space/7z/arthub_test_pkg-0.0.1.7z"
+    local = os.path.join(str(tmp_path), "tmp.7z")
+        
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api))
+    cli.download_file(target, local)
+    
+def test_blade_uploader_fail_general_signer(env, tmp_path):
+    blade_api = init_api(env)
+    target = "pkg_distribution/7z/arthub_test_pkg/0.0.1/arthub_test_pkg.7z"
+    source = os.path.join(str(tmp_path), "tmp.7z")
+        
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api))
+    cli.download_file(target,source)
+    try:
+        target = "test_space/7z/arthub_test_pkg-0.0.1.7z"
+        cli.upload_file(target, source)
+    except APIError:
+        # expected condition:
+        return
+    # package should already uploaded, an error should be raised
+    assert False 
+
+def test_blade_check_exists_general_signer(env, tmp_path):
+    blade_api = init_api(env)
+    target = "test_space/7z/arthub_test_pkg-0.0.2.7z"
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api, force=True))
+    assert cli.check_file_exist(target)
+
+def test_blade_get_download_url_general_signer(env, tmp_path):
+    blade_api = init_api(env)
+    target = "test_space/7z/arthub_test_pkg-0.0.2.7z"
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api, force=True))
+    assert cli.get_download_url(target)
+    
+def test_blade_uploader_general_signer(env, tmp_path):
+    blade_api = init_api(env)
+    target = "test_space/7z/arthub_test_pkg-0.0.2.7z"
+    source = os.path.join(str(tmp_path), "tmp.7z")
+        
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api, force=True))
+    cli.download_file(target,source)
+    cli.upload_file(target, source, print_percent)
+        
+def test_blade_uploader_bigfile_general_signer(env, tmp_path):
+    blade_api = init_api(env)
+    
+    cli = BladeCOSApi(api=blade_api, signer=RemoteSigner(blade_api, force=True))
+    target = "pkg_distribution/7z/pyqt/5.15.2-ng.1/pyqt.7z"
+    source = os.path.join(str(tmp_path), "tmpbig.7z")
+    cli.download_file(target,source)
+    
+    target = "test_space/7z/arthub_test_pkg-0.0.2.7z"
+    def print_percent1(a, b):
+        print_percent(a, b)
+        if a > b/2:
+            import os
+            os.exit(1)
+    cli.upload_file(target, source, print_percent)
```

