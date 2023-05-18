# Comparing `tmp/ape-pokt-0.1.0.tar.gz` & `tmp/ape-pokt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-pokt-0.1.0.tar", last modified: Tue May  2 08:41:58 2023, max compression
+gzip compressed data, was "ape-pokt-0.1.2.tar", last modified: Thu May 18 14:37:07 2023, max compression
```

## Comparing `ape-pokt-0.1.0.tar` & `ape-pokt-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:41:58.551624 ape-pokt-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:41:58.551624 ape-pokt-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:41:58.551624 ape-pokt-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:41:58.551624 ape-pokt-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-02 08:41:58.551624 ape-pokt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:41:58.551624 ape-pokt-0.1.0/ape_pokt/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/ape_pokt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/ape_pokt/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/ape_pokt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 08:41:58.000000 ape-pokt-0.1.0/ape_pokt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:41:58.551624 ape-pokt-0.1.0/ape_pokt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-02 08:41:58.000000 ape-pokt-0.1.0/ape_pokt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-02 08:41:58.000000 ape-pokt-0.1.0/ape_pokt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:41:58.000000 ape-pokt-0.1.0/ape_pokt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:41:58.000000 ape-pokt-0.1.0/ape_pokt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-02 08:41:58.000000 ape-pokt-0.1.0/ape_pokt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 08:41:58.000000 ape-pokt-0.1.0/ape_pokt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-02 08:41:58.555624 ape-pokt-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:41:58.551624 ape-pokt-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-02 08:40:34.000000 ape-pokt-0.1.0/tests/test_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:37:07.678671 ape-pokt-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:37:07.674671 ape-pokt-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:37:07.674671 ape-pokt-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:37:07.674671 ape-pokt-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-18 14:37:07.678671 ape-pokt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:37:07.674671 ape-pokt-0.1.2/ape_pokt/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/ape_pokt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/ape_pokt/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/ape_pokt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 14:37:07.000000 ape-pokt-0.1.2/ape_pokt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:37:07.674671 ape-pokt-0.1.2/ape_pokt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-18 14:37:07.000000 ape-pokt-0.1.2/ape_pokt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-18 14:37:07.000000 ape-pokt-0.1.2/ape_pokt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:37:07.000000 ape-pokt-0.1.2/ape_pokt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:37:07.000000 ape-pokt-0.1.2/ape_pokt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-18 14:37:07.000000 ape-pokt-0.1.2/ape_pokt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 14:37:07.000000 ape-pokt-0.1.2/ape_pokt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 14:37:07.678671 ape-pokt-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:37:07.674671 ape-pokt-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-18 14:36:09.000000 ape-pokt-0.1.2/tests/test_providers.py
```

### Comparing `ape-pokt-0.1.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-pokt-0.1.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-pokt-0.1.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-pokt-0.1.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.github/release-drafter.yml` & `ape-pokt-0.1.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.github/workflows/commitlint.yaml` & `ape-pokt-0.1.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.github/workflows/publish.yaml` & `ape-pokt-0.1.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.github/workflows/test.yaml` & `ape-pokt-0.1.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.github/workflows/title.yaml` & `ape-pokt-0.1.2/.github/workflows/title.yaml`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.gitignore` & `ape-pokt-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/.pre-commit-config.yaml` & `ape-pokt-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/CONTRIBUTING.md` & `ape-pokt-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/LICENSE` & `ape-pokt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/PKG-INFO` & `ape-pokt-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-pokt
-Version: 0.1.0
+Version: 0.1.2
 Summary: ape-pokt: Pokt Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-pokt
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Ape Pokt Plugin
```

### Comparing `ape-pokt-0.1.0/README.md` & `ape-pokt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/ape_pokt/providers.py` & `ape-pokt-0.1.2/ape_pokt/providers.py`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/ape_pokt.egg-info/PKG-INFO` & `ape-pokt-0.1.2/ape_pokt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-pokt
-Version: 0.1.0
+Version: 0.1.2
 Summary: ape-pokt: Pokt Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-pokt
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Ape Pokt Plugin
```

### Comparing `ape-pokt-0.1.0/ape_pokt.egg-info/SOURCES.txt` & `ape-pokt-0.1.2/ape_pokt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/pyproject.toml` & `ape-pokt-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-pokt-0.1.0/setup.py` & `ape-pokt-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-pokt",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.3.0,<0.4.0",
+        "eth-ape>=0.6.7,<0.7",
         "web3",  # Get web3 version from ape
         "importlib-metadata ; python_version<'3.8'",
         "requests",
     ],
     python_requires=">=3.7.2,<4",
     extras_require=extras_require,
     py_modules=["ape_pokt"],
```

### Comparing `ape-pokt-0.1.0/tests/test_providers.py` & `ape-pokt-0.1.2/tests/test_providers.py`

 * *Files identical despite different names*

