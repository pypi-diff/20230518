# Comparing `tmp/python-oauth-token-manager-0.2.0.tar.gz` & `tmp/python-oauth-token-manager-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-oauth-token-manager-0.2.0.tar", last modified: Fri Oct 14 16:30:05 2022, max compression
+gzip compressed data, was "python-oauth-token-manager-0.2.2.tar", last modified: Thu May 18 18:02:58 2023, max compression
```

## Comparing `python-oauth-token-manager-0.2.0.tar` & `python-oauth-token-manager-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-10-14 16:30:05.194130 python-oauth-token-manager-0.2.0/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)    11357 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/LICENSE
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      670 2022-10-14 16:30:05.194130 python-oauth-token-manager-0.2.0/PKG-INFO
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2344 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/README.md
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-10-14 16:30:05.190130 python-oauth-token-manager-0.2.0/auth/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      610 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/__init__.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4035 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/abstract_datastore.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5760 2022-10-14 16:24:52.000000 python-oauth-token-manager-0.2.0/auth/credentials.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1322 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/credentials_helpers.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1057 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/credentials_helpers_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/decorators.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/decorators_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      739 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/exceptions.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4695 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/firestore.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5977 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/gcs_datastore.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     8319 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/gcs_datastore_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5061 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/local_datastore.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     6314 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/local_datastore_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     5226 2022-08-25 19:59:09.000000 python-oauth-token-manager-0.2.0/auth/secret_manager.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       98 2022-08-24 18:15:10.000000 python-oauth-token-manager-0.2.0/pyproject.toml
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2022-10-14 16:30:05.194130 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      670 2022-10-14 16:30:05.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      620 2022-10-14 16:30:05.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-10-14 16:30:05.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-08-24 18:09:16.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/not-zip-safe
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2022-10-14 16:30:05.000000 python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/top_level.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)       38 2022-10-14 16:30:05.194130 python-oauth-token-manager-0.2.0/setup.cfg
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1498 2022-10-14 16:29:59.000000 python-oauth-token-manager-0.2.0/setup.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/
+-rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.2/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2936 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2344 2022-08-23 16:30:58.000000 python-oauth-token-manager-0.2.2/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-18 18:02:58.645086 python-oauth-token-manager-0.2.2/auth/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      749 2023-05-18 18:01:29.000000 python-oauth-token-manager-0.2.2/auth/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2022-07-08 21:15:10.000000 python-oauth-token-manager-0.2.2/auth/abstract_datastore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5774 2023-05-16 15:53:57.000000 python-oauth-token-manager-0.2.2/auth/credentials.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.2/auth/credentials_helpers.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.2/auth/credentials_helpers_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/auth/datastore/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.2/auth/datastore/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5969 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.2/auth/datastore/cloud_storage.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.2/auth/datastore/cloud_storage_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4687 2023-05-18 14:47:50.000000 python-oauth-token-manager-0.2.2/auth/datastore/firestore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5048 2023-05-18 14:51:31.000000 python-oauth-token-manager-0.2.2/auth/datastore/local_file.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.2/auth/datastore/local_file_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5986 2023-05-18 14:49:59.000000 python-oauth-token-manager-0.2.2/auth/datastore/secret_manager.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.2/auth/decorators.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.2/auth/decorators_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.2.2/auth/exceptions.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       98 2022-08-24 18:15:10.000000 python-oauth-token-manager-0.2.2/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2936 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      746 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-08-24 18:09:16.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/not-zip-safe
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/setup.cfg
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2516 2023-05-18 18:02:25.000000 python-oauth-token-manager-0.2.2/setup.py
```

### Comparing `python-oauth-token-manager-0.2.0/LICENSE` & `python-oauth-token-manager-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/README.md` & `python-oauth-token-manager-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/auth/__init__.py` & `python-oauth-token-manager-0.2.2/auth/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/auth/abstract_datastore.py` & `python-oauth-token-manager-0.2.2/auth/abstract_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/auth/credentials.py` & `python-oauth-token-manager-0.2.2/auth/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,16 @@
 
       if creds.expired:
         creds.expiry = expiry
         self._refresh_credentials(creds=creds)
 
     else:
       creds = None
-      raise CredentialsError(f'credentials not found for user {self._email}')
+      raise CredentialsError(
+          message='credentials not found', email=self._email)
 
     return creds
 
   @property
   def auth_headers(self) -> Dict[str, Any]:
     """Returns authorized http headers.
```

### Comparing `python-oauth-token-manager-0.2.0/auth/credentials_helpers.py` & `python-oauth-token-manager-0.2.2/auth/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/auth/credentials_helpers_test.py` & `python-oauth-token-manager-0.2.2/auth/credentials_helpers_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/auth/decorators.py` & `python-oauth-token-manager-0.2.2/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/auth/decorators_test.py` & `python-oauth-token-manager-0.2.2/auth/decorators_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/auth/exceptions.py` & `python-oauth-token-manager-0.2.2/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.0/auth/firestore.py` & `python-oauth-token-manager-0.2.2/auth/datastore/firestore.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
-from . import decorators
-from .abstract_datastore import AbstractDatastore
+import decorators
+from abstract_datastore import AbstractDatastore
 
 from google.cloud import firestore
 
 
 class Firestore(AbstractDatastore):
   @decorators.lazy_property
   def client(self) -> Any:
```

### Comparing `python-oauth-token-manager-0.2.0/auth/gcs_datastore.py` & `python-oauth-token-manager-0.2.2/auth/datastore/cloud_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import json
 from typing import Any, Callable, Dict, List, Mapping, Optional
 
 import gcsfs
 
 from auth.local_datastore import LocalDatastore
 
-from . import decorators
-from .abstract_datastore import AbstractDatastore
+import decorators
+from abstract_datastore import AbstractDatastore
 
 
 def persist(f: Callable) -> Any:
   """Persists the datastore after internal manipulations.
 
   This is used to decorate functions that modify the internal json object
   containing the authentication credentials and ensures that any changes
@@ -45,15 +45,15 @@
       fs = gcsfs.GCSFileSystem(project=datastore.project)
       file_name = f'{datastore.bucket}/{datastore.datastore_file}'
       with fs.open(file_name, 'w') as storage:
         storage.write(json.dumps(datastore.datastore, indent=2))
   return f_persist
 
 
-class GCSDatastore(LocalDatastore):
+class CloudStorage(LocalDatastore):
   """A datastore for storing auth credentials in GCS.
   """
   @decorators.lazy_property
   def datastore(self) -> Dict[str, Any]:
     try:
       fs = gcsfs.GCSFileSystem(project=self.project)
       file_name = f'{self.bucket}/{self.datastore_file}'
```

### Comparing `python-oauth-token-manager-0.2.0/auth/gcs_datastore_test.py` & `python-oauth-token-manager-0.2.2/auth/datastore/cloud_storage_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import unittest
 from unittest import mock
 
-from . import gcs_datastore
+from . import cloud_storage
 
 from copy import deepcopy
 from typing import Any, Dict
 
 MASTER_CONFIG = {
     "auth": {
         "api_key": "api_key",
@@ -31,144 +31,144 @@
         },
     },
 }
 
 CLASS_UNDER_TEST = 'auth.gcs_datastore'
 
 
-class GCSDatastoreTest(unittest.TestCase):
+class CloudStorageTest(unittest.TestCase):
   def setUp(self):
     self.open = mock.mock_open(read_data=json.dumps(MASTER_CONFIG))
     # mock.patch('gcsfs.GCSFileSystem', autospec=True).start()
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_get_document_with_key(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
 
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
       self.assertEqual({'api_key': 'api_key'},
                        datastore.get_document('auth', 'api_key'))
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_get_document_without_key(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
       self.assertEqual(MASTER_CONFIG,
                        datastore.get_document('auth'))
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_get_document_missing_type(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
       self.assertEqual(None, datastore.get_document('10011'))
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_get_document_missing_id(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
       self.assertEqual(None, datastore.get_document('10011'))
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_get_document_missing_key(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
       self.assertEqual(None, datastore.get_document('auth', 'foo'))
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_store_new_document(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
       datastore.store_document(id='0000', document={'id': '0000'})
 
       expected = deepcopy(MASTER_CONFIG)
       expected.update({'0000': {'id': '0000'}})
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_store_new_document_new_name(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(
+      datastore = cloud_storage.CloudStorage(
           project='westley',
           bucket='buttercup',
           datastore_file='new_datastore.json')
       datastore.store_document(id='0000', document={'id': '0000'})
 
       expected = deepcopy(MASTER_CONFIG)
       expected.update({'0000': {'id': '0000'}})
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_list_documents_all(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
 
       _docs = datastore.list_documents()
       expected = MASTER_CONFIG
       self.assertDictEqual(expected, _docs)
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_list_documents_auth(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
 
       _docs = datastore.list_documents('auth')
       expected = MASTER_CONFIG.get('auth')
       self.assertEqual(expected.keys(), _docs)
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_list_documents_none(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
 
       _docs = datastore.list_documents('foo')
       self.assertIsNone(_docs)
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_get_all_documents(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
 
       _docs = datastore.get_all_documents()
       expected = MASTER_CONFIG
       self.assertEqual(expected, _docs)
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_delete_document_collection(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
 
       datastore.delete_document(id='auth')
       self.assertEqual({}, datastore.datastore)
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_delete_document_key(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
 
       datastore.delete_document(
           id='auth', key='api_key')
       self.assertEqual({
           'auth': {'bHVrZUBza3l3YWxrZXIuY29t': {
               '_key': 'luke@skywalker.com',
@@ -176,27 +176,27 @@
                               'refresh_token': 'refresh_token'}}},
           datastore.datastore)
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_delete_document_key_missing(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
 
       datastore.delete_document(
           id='auth', key='foo')
       self.assertEqual(MASTER_CONFIG,
                        datastore.datastore)
 
   @mock.patch('gcsfs.GCSFileSystem')
   def test_update_document_existing(self, mock_filesystem):
     mock_filesystem.return_value.get.return_value = []
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = gcs_datastore.GCSDatastore(project='westley',
+      datastore = cloud_storage.CloudStorage(project='westley',
                                              bucket='buttercup')
 
       expected = {'api_key': 'new api key'}
       datastore.update_document(id='auth',
                                 new_data=expected)
       self.assertEqual(expected.get('api_key'),
                        datastore.datastore.get('auth').get('api_key'))
```

### Comparing `python-oauth-token-manager-0.2.0/auth/local_datastore.py` & `python-oauth-token-manager-0.2.2/auth/datastore/local_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import json
 from typing import Any, Callable, Dict, List, Mapping, Optional
 
-from . import decorators
-from .abstract_datastore import AbstractDatastore
+import decorators
+from abstract_datastore import AbstractDatastore
 
 
 def persist(f: Callable) -> Any:
   def f_persist(*args: Mapping[str, Any], **kw: Mapping[str, Any]) -> Any:
     datastore = args[0]
     try:
       return f(*args, **kw)
     finally:
       with open(datastore.datastore_file, 'w') as storage:
         storage.write(json.dumps(datastore.datastore, indent=2))
   return f_persist
 
 
-class LocalDatastore(AbstractDatastore):
+class LocalFile(AbstractDatastore):
   @decorators.lazy_property
   def datastore(self) -> Dict[str, Any]:
     try:
       with open(self.datastore_file, 'r') as store:
         if data := store.read():
           return json.loads(data)
         else:
```

### Comparing `python-oauth-token-manager-0.2.0/auth/local_datastore_test.py` & `python-oauth-token-manager-0.2.2/auth/datastore/local_file_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import unittest
 from unittest import mock
 
-from . import local_datastore
+from . import local_file
 
 from copy import deepcopy
 from typing import Any, Dict
 
 MASTER_CONFIG = {
     "auth": {
         "api_key": "api_key",
@@ -31,129 +31,129 @@
         },
     },
 }
 
 CLASS_UNDER_TEST = 'auth.local_datastore'
 
 
-class LocalDatastoreTest(unittest.TestCase):
+class LocalFileTest(unittest.TestCase):
   def setUp(self):
     self.open = mock.mock_open(read_data=json.dumps(MASTER_CONFIG))
 
   def test_get_document_with_key(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
       self.assertEqual({'api_key': 'api_key'},
                        datastore.get_document('auth', 'api_key'))
 
   def test_get_document_without_key(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
       self.assertEqual(MASTER_CONFIG,
                        datastore.get_document('auth'))
 
   def test_get_document_missing_type(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
       self.assertEqual(None, datastore.get_document('10011'))
 
   def test_get_document_missing_id(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
       self.assertEqual(None, datastore.get_document('10011'))
 
   def test_get_document_missing_key(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
       self.assertEqual(None, datastore.get_document('auth', 'foo'))
 
   def test_store_new_document(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
       datastore.store_document(id='0000', document={'id': '0000'})
 
       expected = deepcopy(MASTER_CONFIG)
       expected.update({'0000': {'id': '0000'}})
       self.open.assert_called_with('datastore.json', 'w')
       self.open().write.assert_called_with(json.dumps(expected, indent=2))
 
   def test_store_new_document_new_name(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore(
+      datastore = local_file.LocalFile(
           datastore_file='new_datastore.json')
       datastore.store_document(id='0000', document={'id': '0000'})
 
       expected = deepcopy(MASTER_CONFIG)
       expected.update({'0000': {'id': '0000'}})
       self.open.assert_called_with('new_datastore.json', 'w')
       self.open().write.assert_called_with(json.dumps(expected, indent=2))
 
   def test_list_documents_all(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
 
       _docs = datastore.list_documents()
       expected = MASTER_CONFIG
       self.assertDictEqual(expected, _docs)
 
   def test_list_documents_auth(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
 
       _docs = datastore.list_documents('auth')
       expected = MASTER_CONFIG.get('auth')
       self.assertEqual(expected.keys(), _docs)
 
   def test_list_documents_none(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
 
       _docs = datastore.list_documents('foo')
       self.assertIsNone(_docs)
 
   def test_get_all_documents(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
 
       _docs = datastore.get_all_documents()
       expected = MASTER_CONFIG
       self.assertEqual(expected, _docs)
 
   def test_delete_document_collection(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
 
       datastore.delete_document(id='auth')
       self.assertEqual({}, datastore.datastore)
 
   def test_delete_document_key(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
 
       datastore.delete_document(
           id='auth', key='api_key')
       self.assertEqual({
           'auth': {'bHVrZUBza3l3YWxrZXIuY29t': {
               '_key': 'luke@skywalker.com',
               'access_token': 'access_token',
                               'refresh_token': 'refresh_token'}}},
           datastore.datastore)
 
   def test_delete_document_key_missing(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
 
       datastore.delete_document(
           id='auth', key='foo')
       self.assertEqual(MASTER_CONFIG,
                        datastore.datastore)
 
   def test_update_document_existing(self):
     with mock.patch(f'{CLASS_UNDER_TEST}.open', self.open):
-      datastore = local_datastore.LocalDatastore()
+      datastore = local_file.LocalFile()
 
       expected = {'api_key': 'new api key'}
       datastore.update_document(id='auth',
                                 new_data=expected)
       self.open().write.assert_called_once()
       self.assertEqual(expected.get('api_key'),
                        datastore.datastore.get('auth').get('api_key'))
```

### Comparing `python-oauth-token-manager-0.2.0/auth/secret_manager.py` & `python-oauth-token-manager-0.2.2/auth/datastore/secret_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 from __future__ import annotations
 
 import json
 from typing import Any, List, Mapping, Optional, Type
 
 from google.cloud import secretmanager, secretmanager_v1
 from google.cloud.secretmanager_v1.types import resources
+from google.cloud.secretmanager_v1.services.secret_manager_service import pagers
 
-from . import decorators
-from .abstract_datastore import AbstractDatastore
+import decorators
+from abstract_datastore import AbstractDatastore
 
 
 class SecretManager(AbstractDatastore):
 
   def __init__(self, email: str = None,
                project: str = None) -> AbstractDatastore:
     self._project = project
@@ -56,15 +57,15 @@
                                                    secret_id=id)
     response = self.client.create_secret(request=request)
 
     return response
 
   @decorators.implicit_create(creator=create_secret)
   def store_document(self,  id: str, document: Mapping[str, Any],
-                     type: Optional[Type] = None) -> None:
+                     type: Optional[Type] = None) -> resources.SecretVersion:
     """Stores a document.
 
     Store a document in Secret Manager. This will, for credentials, always be
     the OAuth token.
 
     Arguments:
         id (str): The document id.
@@ -72,29 +73,47 @@
         type (Optional[Type]): Unused.
     """
     payload = secretmanager_v1.SecretPayload(
         data=json.dumps(document).encode('utf-8'))
     request = secretmanager_v1.AddSecretVersionRequest(
         parent=self.client.secret_path(self._project, id),
         payload=payload)
-    self.client.add_secret_version(request=request)
+    return self.client.add_secret_version(request=request)
 
   def update_document(self, id: str, new_data: Mapping[str, Any],
                       type: Optional[Type] = None) -> None:
     """Updates a document.
 
     Update a document in Secret Manager. If the document is not already there,
     it will be created as a net-new document. If it is, it will be updated.
 
+    As this is a specific 'update' request, remove any other enabled versions.
+
     Args:
         id (str): the id of the document.
         new_data (Dict[str, Any]): the document content.
         type (Optional[Type]): Unused.
     """
-    self.store_document(id=id, type=type, document=new_data)
+    new_version = self.store_document(id=id, type=type, document=new_data)
+
+    # Destroy other versions
+    request = secretmanager_v1.ListSecretVersionsRequest(
+        parent=self.client.secret_path(project=self._project, secret=id),
+        filter='state:enabled'
+    )
+    version_list = self.client.list_secret_versions(request=request)
+    for page in version_list.pages:
+      for version in page.versions:
+        if version == new_version:
+          continue
+        else:
+          self.client.destroy_secret_version(
+              secretmanager_v1.DestroySecretVersionRequest(
+                  name=version.name
+              ))
 
   def get_document(self, id: str, type: Optional[Type] = None,
                    key: Optional[str] = None) -> Mapping[str, Any]:
     """Fetches a document (could be anything).
 
     Fetch a document
```

### Comparing `python-oauth-token-manager-0.2.0/python_oauth_token_manager.egg-info/SOURCES.txt` & `python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 auth/abstract_datastore.py
 auth/credentials.py
 auth/credentials_helpers.py
 auth/credentials_helpers_test.py
 auth/decorators.py
 auth/decorators_test.py
 auth/exceptions.py
-auth/firestore.py
-auth/gcs_datastore.py
-auth/gcs_datastore_test.py
-auth/local_datastore.py
-auth/local_datastore_test.py
-auth/secret_manager.py
+auth/datastore/__init__.py
+auth/datastore/cloud_storage.py
+auth/datastore/cloud_storage_test.py
+auth/datastore/firestore.py
+auth/datastore/local_file.py
+auth/datastore/local_file_test.py
+auth/datastore/secret_manager.py
 python_oauth_token_manager.egg-info/PKG-INFO
 python_oauth_token_manager.egg-info/SOURCES.txt
 python_oauth_token_manager.egg-info/dependency_links.txt
 python_oauth_token_manager.egg-info/not-zip-safe
+python_oauth_token_manager.egg-info/requires.txt
 python_oauth_token_manager.egg-info/top_level.txt
```

