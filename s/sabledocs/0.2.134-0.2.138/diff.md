# Comparing `tmp/sabledocs-0.2.134.tar.gz` & `tmp/sabledocs-0.2.138.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.2.134.tar", last modified: Thu May 18 15:46:06 2023, max compression
+gzip compressed data, was "sabledocs-0.2.138.tar", last modified: Thu May 18 16:00:31 2023, max compression
```

## Comparing `sabledocs-0.2.134.tar` & `sabledocs-0.2.138.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 15:46:06.032629 sabledocs-0.2.134/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-05-18 15:45:53.000000 sabledocs-0.2.134/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-18 15:45:53.000000 sabledocs-0.2.134/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4117 2023-05-18 15:46:06.032629 sabledocs-0.2.134/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3577 2023-05-18 15:45:53.000000 sabledocs-0.2.134/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-18 15:45:53.000000 sabledocs-0.2.134/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-05-18 15:46:06.032629 sabledocs-0.2.134/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 15:46:06.028629 sabledocs-0.2.134/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 15:46:06.032629 sabledocs-0.2.134/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2853 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2023 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13641 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 15:46:06.028629 sabledocs-0.2.134/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 15:46:06.032629 sabledocs-0.2.134/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 15:46:06.032629 sabledocs-0.2.134/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-05-18 15:45:53.000000 sabledocs-0.2.134/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 15:46:06.032629 sabledocs-0.2.134/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4117 2023-05-18 15:46:06.000000 sabledocs-0.2.134/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-18 15:46:06.000000 sabledocs-0.2.134/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-18 15:46:06.000000 sabledocs-0.2.134/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-18 15:46:06.000000 sabledocs-0.2.134/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-18 15:46:06.000000 sabledocs-0.2.134/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-05-18 15:46:06.000000 sabledocs-0.2.134/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-05-18 16:00:18.000000 sabledocs-0.2.138/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-18 16:00:18.000000 sabledocs-0.2.138/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4117 2023-05-18 16:00:31.808618 sabledocs-0.2.138/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3577 2023-05-18 16:00:18.000000 sabledocs-0.2.138/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-18 16:00:18.000000 sabledocs-0.2.138/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-05-18 16:00:31.808618 sabledocs-0.2.138/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.804618 sabledocs-0.2.138/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2853 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2023 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.804618 sabledocs-0.2.138/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4117 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.2.134/LICENSE` & `sabledocs-0.2.138/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/PKG-INFO` & `sabledocs-0.2.138/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.2.134
+Version: 0.2.138
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.2.134/README.md` & `sabledocs-0.2.138/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/pyproject.toml` & `sabledocs-0.2.138/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/__main__.py` & `sabledocs-0.2.138/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/lunr_search.py` & `sabledocs-0.2.138/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.2.138/src/sabledocs/proto_descriptor_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def build_source_code_url(repository_url, repository_type, repository_branch, file_path, line_number):
     match repository_type:
         case RepositoryType.NONE:
             return None
         case RepositoryType.GITHUB:
             return f"{repository_url.strip('/')}/blob/{repository_branch}/{file_path}#L{line_number}"
         case RepositoryType.BITBUCKET:
-            return f"{repository_url.strip('/')}/src/{repository_branch}/{file_path}#lines-{line_number}"
+            return f"{repository_url.strip('/')}/src/{repository_branch}/{file_path}#lines-{line_number + 1}"
     return ""
 
 
 class ParseContext:
     def __init__(self, config, package, source_file_path, path, locations):
         self.config = config
         self.package = package
```

### Comparing `sabledocs-0.2.134/src/sabledocs/proto_model.py` & `sabledocs-0.2.138/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/sable_config.py` & `sabledocs-0.2.138/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/base.html` & `sabledocs-0.2.138/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.2.138/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/index.html` & `sabledocs-0.2.138/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/message.html` & `sabledocs-0.2.138/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/package.html` & `sabledocs-0.2.138/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/search.html` & `sabledocs-0.2.138/src/sabledocs/templates/_default/search.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/service.html` & `sabledocs-0.2.138/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.2.138/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.2.138/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.134/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.2.138/src/sabledocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.2.134
+Version: 0.2.138
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.2.134/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.2.138/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

