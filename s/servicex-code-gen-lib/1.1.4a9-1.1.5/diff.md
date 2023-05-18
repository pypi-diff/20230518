# Comparing `tmp/servicex_code_gen_lib-1.1.4a9.tar.gz` & `tmp/servicex_code_gen_lib-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_code_gen_lib-1.1.4a9.tar", max compression
+gzip compressed data, was "servicex_code_gen_lib-1.1.5.tar", max compression
```

## Comparing `servicex_code_gen_lib-1.1.4a9.tar` & `servicex_code_gen_lib-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1520 2023-02-03 23:00:42.434175 servicex_code_gen_lib-1.1.4a9/LICENSE
--rw-r--r--   0        0        0      138 2023-02-03 23:00:42.434175 servicex_code_gen_lib-1.1.4a9/README.md
--rw-r--r--   0        0        0      736 2023-02-03 23:01:02.218101 servicex_code_gen_lib-1.1.4a9/pyproject.toml
--rw-r--r--   0        0        0     2882 2023-02-03 23:00:42.434175 servicex_code_gen_lib-1.1.4a9/servicex_codegen/__init__.py
--rw-r--r--   0        0        0     2194 2023-02-03 23:00:42.434175 servicex_code_gen_lib-1.1.4a9/servicex_codegen/code_generator.py
--rw-r--r--   0        0        0     4797 2023-02-03 23:00:42.434175 servicex_code_gen_lib-1.1.4a9/servicex_codegen/post_operation.py
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.4a9/setup.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.4a9/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/README.md
+-rw-r--r--   0        0        0      749 2023-05-18 18:01:16.277930 servicex_code_gen_lib-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2882 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/servicex_codegen/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/servicex_codegen/code_generator.py
+-rw-r--r--   0        0        0     4797 2023-05-18 18:00:53.213698 servicex_code_gen_lib-1.1.5/servicex_codegen/post_operation.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5/setup.py
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 servicex_code_gen_lib-1.1.5/PKG-INFO
```

### Comparing `servicex_code_gen_lib-1.1.4a9/LICENSE` & `servicex_code_gen_lib-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.4a9/pyproject.toml` & `servicex_code_gen_lib-1.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "servicex-code-gen-lib"
-version = "1.1.4-alpha.9"
+version = "1.1.5"
 description = "Library for creating ServiceX Code Generators"
 authors = ["Ben Galewsky <bengal1@illinois.edu>"]
 readme = "README.md"
 packages = [{include = "servicex_codegen"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-Flask = "^2.2.2"
+python = "^3.10"
+Flask = "^2.3.2"
 Flask-RESTful = "^0.3.9"
 Flask-WTF = "^1.0.1"
 itsdangerous = "^2.1.2"
 Werkzeug = "^2.2.2"
 Jinja2 = "^3.1.2"
 requests-toolbelt = "^0.10.1"
+urllib3 = "1.26.15"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 codecov = "^2.1.12"
 flake8 = "^5.0.4"
```

### Comparing `servicex_code_gen_lib-1.1.4a9/servicex_codegen/__init__.py` & `servicex_code_gen_lib-1.1.5/servicex_codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.4a9/servicex_codegen/code_generator.py` & `servicex_code_gen_lib-1.1.5/servicex_codegen/code_generator.py`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.4a9/servicex_codegen/post_operation.py` & `servicex_code_gen_lib-1.1.5/servicex_codegen/post_operation.py`

 * *Files identical despite different names*

### Comparing `servicex_code_gen_lib-1.1.4a9/setup.py` & `servicex_code_gen_lib-1.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Flask-RESTful>=0.3.9,<0.4.0',
  'Flask-WTF>=1.0.1,<2.0.0',
- 'Flask>=2.2.2,<3.0.0',
+ 'Flask>=2.3.2,<3.0.0',
  'Jinja2>=3.1.2,<4.0.0',
  'Werkzeug>=2.2.2,<3.0.0',
  'itsdangerous>=2.1.2,<3.0.0',
- 'requests-toolbelt>=0.10.1,<0.11.0']
+ 'requests-toolbelt>=0.10.1,<0.11.0',
+ 'urllib3==1.26.15']
 
 setup_kwargs = {
     'name': 'servicex-code-gen-lib',
-    'version': '1.1.4a9',
+    'version': '1.1.5',
     'description': 'Library for creating ServiceX Code Generators',
     'long_description': '<!-- @format -->\n\n# ServiceX Code Generator Library\n\nThis library provides common code for creating Code Generator services for\nServiceX.\n',
     'author': 'Ben Galewsky',
     'author_email': 'bengal1@illinois.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

