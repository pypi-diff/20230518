# Comparing `tmp/edx-enterprise-subsidy-client-0.3.2.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.3.2.tar", last modified: Tue May 16 20:19:17 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.3.3.tar", last modified: Thu May 18 20:04:32 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.3.2.tar` & `edx-enterprise-subsidy-client-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8723 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10408 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8723 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8909 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10533 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8909 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-18 20:04:32.000000 edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 20:04:32.123772 edx-enterprise-subsidy-client-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3178 2023-05-18 20:04:27.000000 edx-enterprise-subsidy-client-0.3.3/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.3.2/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.3.3/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.3]
+*******
+* admin-list transactions will also be filtered by ``created`` state by default.
+* Adds an ADR explaining the default states for which this client filters transactions.
+
 [0.3.2]
 *******
 * admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
   Caller may specify other valid states (e.g. `failed` or `created`).
 
 [0.3.1]
 *******
```

### Comparing `edx-enterprise-subsidy-client-0.3.2/LICENSE` & `edx-enterprise-subsidy-client-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.2/LICENSE.txt` & `edx-enterprise-subsidy-client-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.2/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.2
+Version: 0.3.3
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.3]
+*******
+* admin-list transactions will also be filtered by ``created`` state by default.
+* Adds an ADR explaining the default states for which this client filters transactions.
+
 [0.3.2]
 *******
 * admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
   Caller may specify other valid states (e.g. `failed` or `created`).
 
 [0.3.1]
 *******
```

### Comparing `edx-enterprise-subsidy-client-0.3.2/README.rst` & `edx-enterprise-subsidy-client-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
         self.client = OAuthAPIClient(
             settings.OAUTH2_PROVIDER_URL,
             settings.BACKEND_SERVICE_EDX_OAUTH2_KEY,
             settings.BACKEND_SERVICE_EDX_OAUTH2_SECRET,
         )
 
     def get_content_metadata_url(self, content_identifier):
-        """Helper method to generate the subsidy service metadata API url."""
-        return self.CONTENT_METADATA_ENDPOINT + content_identifier
+        """Helper method to generate the subsidy service metadata API url, with a trailing slash."""
+        return self.CONTENT_METADATA_ENDPOINT + content_identifier + '/'
 
     def get_subsidy_content_data(self, enterprise_customer_uuid, content_identifier):
         """
         Client method to fetch enterprise specific content data.
 
         Args:
             enterprise_customer_uuid (str): Enterprise customer UUID
@@ -248,15 +248,19 @@
         lms_user_id=None, content_key=None,
         subsidy_access_policy_uuid=None, transaction_states=None,
     ):
         """
         List transactions in a subsidy with admin- or operator-level permissions.
         """
         query_params = {
-            'state': [TransactionStateChoices.COMMITTED, TransactionStateChoices.PENDING],
+            'state': [
+                TransactionStateChoices.COMMITTED,
+                TransactionStateChoices.PENDING,
+                TransactionStateChoices.CREATED,
+            ],
         }
         if include_aggregates:
             query_params['include_aggregates'] = include_aggregates
         if lms_user_id:
             query_params['lms_user_id'] = lms_user_id
         if content_key:
             query_params['content_key'] = content_key
```

### Comparing `edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.2
+Version: 0.3.3
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.3]
+*******
+* admin-list transactions will also be filtered by ``created`` state by default.
+* Adds an ADR explaining the default states for which this client filters transactions.
+
 [0.3.2]
 *******
 * admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
   Caller may specify other valid states (e.g. `failed` or `created`).
 
 [0.3.1]
 *******
```

### Comparing `edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.3.3/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.2/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.3.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.2/setup.py` & `edx-enterprise-subsidy-client-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.2/tests/test_client.py` & `edx-enterprise-subsidy-client-0.3.3/tests/test_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,26 +58,37 @@
     subsidy_uuid = uuid.uuid4()
     lms_user_id = 123
     content_key = 'the-best-content'
     subsidy_access_policy_uuid = uuid.uuid4()
 
     subsidy_service_client = EnterpriseSubsidyAPIClientV2()
 
-    response = subsidy_service_client.list_subsidy_transactions(
-        subsidy_uuid=subsidy_uuid,
-        lms_user_id=lms_user_id,
-        content_key=content_key,
-        subsidy_access_policy_uuid=subsidy_access_policy_uuid,
-        transaction_states=['committed', 'pending', 'district-of-columbia'],
-    )
+    data_driven_test = [
+        (
+            {'transaction_states': ['committed', 'pending', 'district-of-columbia']},
+            ['committed', 'pending'],
+        ),
+        (
+            {},
+            ['committed', 'pending', 'created'],
+        ),
+    ]
+    for state_kwargs, expected_state_call_param in data_driven_test:
+        response = subsidy_service_client.list_subsidy_transactions(
+            subsidy_uuid=subsidy_uuid,
+            lms_user_id=lms_user_id,
+            content_key=content_key,
+            subsidy_access_policy_uuid=subsidy_access_policy_uuid,
+            **state_kwargs,
+        )
 
-    assert response == mocked_response_data
-    mock_oauth_client.return_value.get.assert_called_once_with(
-        f'enterprise-subsidy-service-base-url/api/v2/subsidies/{subsidy_uuid}/admin/transactions/',
-        params={
-            'state': ['committed', 'pending'],
-            'include_aggregates': True,
-            'lms_user_id': 123,
-            'content_key': 'the-best-content',
-            'subsidy_access_policy_uuid': str(subsidy_access_policy_uuid),
-        },
-    )
+        assert response == mocked_response_data
+        mock_oauth_client.return_value.get.assert_called_with(
+            f'enterprise-subsidy-service-base-url/api/v2/subsidies/{subsidy_uuid}/admin/transactions/',
+            params={
+                'state': expected_state_call_param,
+                'include_aggregates': True,
+                'lms_user_id': 123,
+                'content_key': 'the-best-content',
+                'subsidy_access_policy_uuid': str(subsidy_access_policy_uuid),
+            },
+        )
```

