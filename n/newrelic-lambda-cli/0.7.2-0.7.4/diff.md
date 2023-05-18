# Comparing `tmp/newrelic-lambda-cli-0.7.2.tar.gz` & `tmp/newrelic-lambda-cli-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newrelic-lambda-cli-0.7.2.tar", last modified: Wed Jul 20 23:11:21 2022, max compression
+gzip compressed data, was "dist/newrelic-lambda-cli-0.7.4.tar", last modified: Thu May 18 21:46:41 2023, max compression
```

## Comparing `newrelic-lambda-cli-0.7.2.tar` & `newrelic-lambda-cli-0.7.4.tar`

### file list

```diff
@@ -1,41 +1,50 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3220 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2403 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11345 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20433 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20090 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4486 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/THIRD_PARTY_NOTICES.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      149 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14848 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/api.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      520 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2601 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9497 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/integrations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5678 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/layers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/subscriptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      902 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cliutils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2773 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26627 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/integrations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14262 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/layers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9093 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5632 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/subscriptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3591 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/templates/import-template.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1849 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/templates/license-key-secret.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2874 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2219 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4514 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20433 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1136 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      234 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2022-07-20 23:11:21.000000 newrelic-lambda-cli-0.7.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1002 2022-07-20 23:11:15.000000 newrelic-lambda-cli-0.7.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3220 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2403 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11345 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       71 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20440 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20097 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4486 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/THIRD_PARTY_NOTICES.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      149 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14848 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/api.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      520 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2601 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9497 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/integrations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5678 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/layers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/subscriptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      902 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cliutils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2773 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26627 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/integrations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14262 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/layers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9093 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5632 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/subscriptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3591 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/templates/import-template.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1849 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/templates/license-key-secret.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2874 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2219 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4628 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20440 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1328 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       65 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      234 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       94 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1002 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-18 21:46:41.000000 newrelic-lambda-cli-0.7.4/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6327 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/tests/test_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2332 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/tests/test_functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16052 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/tests/test_integrations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16549 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/tests/test_layers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      548 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/tests/test_new_relic_gql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7112 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/tests/test_permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3580 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/tests/test_subscriptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2023-05-18 21:46:34.000000 newrelic-lambda-cli-0.7.4/tests/test_utils.py
```

### Comparing `newrelic-lambda-cli-0.7.2/CODE_OF_CONDUCT.md` & `newrelic-lambda-cli-0.7.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/CONTRIBUTING.md` & `newrelic-lambda-cli-0.7.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/LICENSE` & `newrelic-lambda-cli-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/PKG-INFO` & `newrelic-lambda-cli-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-lambda-cli
-Version: 0.7.2
+Version: 0.7.4
 Summary: A CLI to install the New Relic AWS Lambda integration and layers.
 Home-page: https://github.com/newrelic/newrelic-lambda-cli
 Author: New Relic
 Author-email: serverless-dev@newrelic.com
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -58,15 +58,15 @@
 * python3.9
 
 **Note:** Automatic handler wrapping is only supported for Node.js and Python. For other runtimes,
 manual function wrapping is required using the runtime specific New Relic agent.
 
 ## Requirements
 
-* Python >= 3.3
+* Python >= 3.3 < 3.10
 * Retrieve your [New relic Account ID](https://docs.newrelic.com/docs/accounts/install-new-relic/account-setup/account-id) and [User API Key](https://docs.newrelic.com/docs/apis/get-started/intro-apis/types-new-relic-api-keys#user-api-key)
 
 ## Recommendations
 
 * Install the [AWS CLI](https://github.com/aws/aws-cli) and configure your environment with `aws configure`
 
 ## Installation
```

### Comparing `newrelic-lambda-cli-0.7.2/README.md` & `newrelic-lambda-cli-0.7.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 * python3.9
 
 **Note:** Automatic handler wrapping is only supported for Node.js and Python. For other runtimes,
 manual function wrapping is required using the runtime specific New Relic agent.
 
 ## Requirements
 
-* Python >= 3.3
+* Python >= 3.3 < 3.10
 * Retrieve your [New relic Account ID](https://docs.newrelic.com/docs/accounts/install-new-relic/account-setup/account-id) and [User API Key](https://docs.newrelic.com/docs/apis/get-started/intro-apis/types-new-relic-api-keys#user-api-key)
 
 ## Recommendations
 
 * Install the [AWS CLI](https://github.com/aws/aws-cli) and configure your environment with `aws configure`
 
 ## Installation
```

### Comparing `newrelic-lambda-cli-0.7.2/THIRD_PARTY_NOTICES.md` & `newrelic-lambda-cli-0.7.4/THIRD_PARTY_NOTICES.md`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/api.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/api.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/__init__.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/decorators.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/functions.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/functions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/integrations.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/integrations.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/layers.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/layers.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cli/subscriptions.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cli/subscriptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/cliutils.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/cliutils.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/functions.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/functions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/integrations.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/integrations.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/layers.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/layers.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/permissions.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/permissions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/subscriptions.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/subscriptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/templates/import-template.yaml` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/templates/import-template.yaml`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/templates/license-key-secret.yaml` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/templates/license-key-secret.yaml`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/types.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/types.py`

 * *Files identical despite different names*

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli/utils.py` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
         "Handler": "newrelic-lambda-wrapper.handler",
         "LambdaExtension": True,
     },
     "nodejs16.x": {
         "Handler": "newrelic-lambda-wrapper.handler",
         "LambdaExtension": True,
     },
+    "nodejs18.x": {
+        "Handler": "newrelic-lambda-wrapper.handler",
+        "LambdaExtension": True,
+    },
     "provided": {"LambdaExtension": True},
     "provided.al2": {"LambdaExtension": True},
     "python3.6": {
         "Handler": "newrelic_lambda_wrapper.handler",
         "LambdaExtension": False,
     },
     "python3.7": {
```

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/PKG-INFO` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-lambda-cli
-Version: 0.7.2
+Version: 0.7.4
 Summary: A CLI to install the New Relic AWS Lambda integration and layers.
 Home-page: https://github.com/newrelic/newrelic-lambda-cli
 Author: New Relic
 Author-email: serverless-dev@newrelic.com
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -58,15 +58,15 @@
 * python3.9
 
 **Note:** Automatic handler wrapping is only supported for Node.js and Python. For other runtimes,
 manual function wrapping is required using the runtime specific New Relic agent.
 
 ## Requirements
 
-* Python >= 3.3
+* Python >= 3.3 < 3.10
 * Retrieve your [New relic Account ID](https://docs.newrelic.com/docs/accounts/install-new-relic/account-setup/account-id) and [User API Key](https://docs.newrelic.com/docs/apis/get-started/intro-apis/types-new-relic-api-keys#user-api-key)
 
 ## Recommendations
 
 * Install the [AWS CLI](https://github.com/aws/aws-cli) and configure your environment with `aws configure`
 
 ## Installation
```

### Comparing `newrelic-lambda-cli-0.7.2/newrelic_lambda_cli.egg-info/SOURCES.txt` & `newrelic-lambda-cli-0.7.4/newrelic_lambda_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -28,8 +28,16 @@
 newrelic_lambda_cli/cli/decorators.py
 newrelic_lambda_cli/cli/functions.py
 newrelic_lambda_cli/cli/integrations.py
 newrelic_lambda_cli/cli/layers.py
 newrelic_lambda_cli/cli/subscriptions.py
 newrelic_lambda_cli/templates/import-template.yaml
 newrelic_lambda_cli/templates/license-key-secret.yaml
-newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml
+newrelic_lambda_cli/templates/nr-lambda-integration-role.yaml
+tests/test_api.py
+tests/test_functions.py
+tests/test_integrations.py
+tests/test_layers.py
+tests/test_new_relic_gql.py
+tests/test_permissions.py
+tests/test_subscriptions.py
+tests/test_utils.py
```

### Comparing `newrelic-lambda-cli-0.7.2/setup.py` & `newrelic-lambda-cli-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 
 README = open(os.path.join(os.path.dirname(__file__), "README.md"), "r").read()
 
 setup(
     name="newrelic-lambda-cli",
-    version="0.7.2",
+    version="0.7.4",
     python_requires=">=3.3",
     description="A CLI to install the New Relic AWS Lambda integration and layers.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="New Relic",
     author_email="serverless-dev@newrelic.com",
     url="https://github.com/newrelic/newrelic-lambda-cli",
```

