# Comparing `tmp/ezsession-0.0.1.tar.gz` & `tmp/ezsession-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsession-0.0.1.tar", last modified: Thu May 18 20:18:44 2023, max compression
+gzip compressed data, was "ezsession-0.0.2.tar", last modified: Thu May 18 21:43:43 2023, max compression
```

## Comparing `ezsession-0.0.1.tar` & `ezsession-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:18:44.013545 ezsession-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-18 20:18:44.013545 ezsession-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-18 20:18:32.000000 ezsession-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 20:18:32.000000 ezsession-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-18 20:18:44.013545 ezsession-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-18 20:18:32.000000 ezsession-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:18:44.013545 ezsession-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:18:44.013545 ezsession-0.0.1/src/ezsession/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-18 20:18:32.000000 ezsession-0.0.1/src/ezsession/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:18:44.013545 ezsession-0.0.1/src/ezsession.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-18 20:18:44.000000 ezsession-0.0.1/src/ezsession.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 20:18:44.000000 ezsession-0.0.1/src/ezsession.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:18:44.000000 ezsession-0.0.1/src/ezsession.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 20:18:44.000000 ezsession-0.0.1/src/ezsession.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:43:43.463143 ezsession-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-18 21:43:43.463143 ezsession-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-18 21:43:29.000000 ezsession-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 21:43:29.000000 ezsession-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-18 21:43:43.463143 ezsession-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-18 21:43:29.000000 ezsession-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:43:43.463143 ezsession-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:43:43.463143 ezsession-0.0.2/src/ezsession/
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-18 21:43:29.000000 ezsession-0.0.2/src/ezsession/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:43:43.463143 ezsession-0.0.2/src/ezsession.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-18 21:43:43.000000 ezsession-0.0.2/src/ezsession.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 21:43:43.000000 ezsession-0.0.2/src/ezsession.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:43:43.000000 ezsession-0.0.2/src/ezsession.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 21:43:43.000000 ezsession-0.0.2/src/ezsession.egg-info/top_level.txt
```

### Comparing `ezsession-0.0.1/PKG-INFO` & `ezsession-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
 
+```
+pip install ezsession
+```
+
 ## Auth Types and Required Inputs
 
-1. **oauth** - `client_id`, `client_secret`, `audience`
-2. **oauth_basic** - `username`, `password`
-3. **oauth_password** - `username`, `password`
-4. **basic** - `username`, `password`
+1. **oauth** - `auth_uri`, `client_id`, `client_secret`, `audience`
+2. **oauth_basic** - `auth_uri`, `username`, `password`
+3. **oauth_password** - `auth_uri`, `username`, `password`
+4. **basic** - `username`, `password`, `auth_uri` (optional)
 5. **bearer** - `api_key`
 6. **ApiToken** - `api_key`
-7. **dell** - `client_id`, `client_secret`
+7. **dell** - `auth_uri`, `client_id`, `client_secret`
 
 ## Examples
 Example usage for getting a Datto RMM or Huntress session:
 
 ```python
 from ezsession import get_session
 def datto_rmm_auth(api_key, api_secret):
```

### Comparing `ezsession-0.0.1/README.md` & `ezsession-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
 
+```
+pip install ezsession
+```
+
 ## Auth Types and Required Inputs
 
-1. **oauth** - `client_id`, `client_secret`, `audience`
-2. **oauth_basic** - `username`, `password`
-3. **oauth_password** - `username`, `password`
-4. **basic** - `username`, `password`
+1. **oauth** - `auth_uri`, `client_id`, `client_secret`, `audience`
+2. **oauth_basic** - `auth_uri`, `username`, `password`
+3. **oauth_password** - `auth_uri`, `username`, `password`
+4. **basic** - `username`, `password`, `auth_uri` (optional)
 5. **bearer** - `api_key`
 6. **ApiToken** - `api_key`
-7. **dell** - `client_id`, `client_secret`
+7. **dell** - `auth_uri`, `client_id`, `client_secret`
 
 ## Examples
 Example usage for getting a Datto RMM or Huntress session:
 
 ```python
 from ezsession import get_session
 def datto_rmm_auth(api_key, api_secret):
```

### Comparing `ezsession-0.0.1/setup.py` & `ezsession-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ezsession",
-    version="0.0.1",
+    version="0.0.2",
     description="A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `ezsession-0.0.1/src/ezsession/__init__.py` & `ezsession-0.0.2/src/ezsession/__init__.py`

 * *Files identical despite different names*

### Comparing `ezsession-0.0.1/src/ezsession.egg-info/PKG-INFO` & `ezsession-0.0.2/src/ezsession.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
 
+```
+pip install ezsession
+```
+
 ## Auth Types and Required Inputs
 
-1. **oauth** - `client_id`, `client_secret`, `audience`
-2. **oauth_basic** - `username`, `password`
-3. **oauth_password** - `username`, `password`
-4. **basic** - `username`, `password`
+1. **oauth** - `auth_uri`, `client_id`, `client_secret`, `audience`
+2. **oauth_basic** - `auth_uri`, `username`, `password`
+3. **oauth_password** - `auth_uri`, `username`, `password`
+4. **basic** - `username`, `password`, `auth_uri` (optional)
 5. **bearer** - `api_key`
 6. **ApiToken** - `api_key`
-7. **dell** - `client_id`, `client_secret`
+7. **dell** - `auth_uri`, `client_id`, `client_secret`
 
 ## Examples
 Example usage for getting a Datto RMM or Huntress session:
 
 ```python
 from ezsession import get_session
 def datto_rmm_auth(api_key, api_secret):
```

