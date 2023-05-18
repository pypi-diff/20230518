# Comparing `tmp/references_parser-1.0.0.tar.gz` & `tmp/references_parser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "references_parser-1.0.0.tar", last modified: Thu May 18 06:25:01 2023, max compression
+gzip compressed data, was "references_parser-1.1.0.tar", last modified: Thu May 18 06:34:43 2023, max compression
```

## Comparing `references_parser-1.0.0.tar` & `references_parser-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:25:01.091219 references_parser-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-18 06:25:01.091219 references_parser-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-18 06:24:45.000000 references_parser-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 06:24:45.000000 references_parser-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:25:01.091219 references_parser-1.0.0/references_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:25:01.091219 references_parser-1.0.0/references_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/parsers/IeeeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/parsers/SsauParser.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:25:01.091219 references_parser-1.0.0/references_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:25:01.095219 references_parser-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 06:24:45.000000 references_parser-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:34:43.651840 references_parser-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-18 06:34:43.651840 references_parser-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-18 06:34:27.000000 references_parser-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 06:34:27.000000 references_parser-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:34:43.647840 references_parser-1.1.0/references_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:34:27.000000 references_parser-1.1.0/references_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 06:34:27.000000 references_parser-1.1.0/references_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-18 06:34:27.000000 references_parser-1.1.0/references_parser/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:34:43.651840 references_parser-1.1.0/references_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-18 06:34:27.000000 references_parser-1.1.0/references_parser/parsers/IeeeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-18 06:34:27.000000 references_parser-1.1.0/references_parser/parsers/SsauParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 06:34:27.000000 references_parser-1.1.0/references_parser/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:34:43.651840 references_parser-1.1.0/references_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-18 06:34:43.000000 references_parser-1.1.0/references_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 06:34:43.000000 references_parser-1.1.0/references_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:34:43.000000 references_parser-1.1.0/references_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 06:34:43.000000 references_parser-1.1.0/references_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 06:34:43.000000 references_parser-1.1.0/references_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 06:34:43.000000 references_parser-1.1.0/references_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:34:43.651840 references_parser-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 06:34:27.000000 references_parser-1.1.0/setup.py
```

### Comparing `references_parser-1.0.0/PKG-INFO` & `references_parser-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: references_parser
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tool for parsing bibtex in ssau's format
 Home-page: https://github.com/Banayaki/ReferencesParser
 Author: Mukhin Artem
 Author-email: artemmukhinssau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
@@ -14,22 +14,24 @@
 ```bash
 pip install references-parser
 ```
 # Usage
 
 ### Use help to see CLI parameters
 ```bash
-➜ python -m references_parser parse --help
+➜ python -m references_parser parse --help        
 Usage: python -m references_parser parse [OPTIONS] PATH
 
 Options:
-  -s, --save TEXT    Path to file where to save the result of parsing.
-  -p, --parser TEXT  Parser to use. Available parsers: ieee, ssau. Default:
-                     ssau.
-  --help             Show this message and exit.
+  -s, --save TEXT         Path to file where to save the result of parsing.
+  -p, --parser TEXT       Parser to use. Available parsers: ieee, ssau.
+                          Default: ssau.
+  -v, --verbose           Whether to print output to stdout or not
+  -b, --beautify INTEGER  Number of line wraps between references. Default: 1
+  --help                  Show this message and exit.
 ```
 
 ### Usual way of using the script
 ```bash
 python -m references_parser parse in.txt
 ```
```

### Comparing `references_parser-1.0.0/README.md` & `references_parser-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 ```bash
 pip install references-parser
 ```
 # Usage
 
 ### Use help to see CLI parameters
 ```bash
-➜ python -m references_parser parse --help
+➜ python -m references_parser parse --help        
 Usage: python -m references_parser parse [OPTIONS] PATH
 
 Options:
-  -s, --save TEXT    Path to file where to save the result of parsing.
-  -p, --parser TEXT  Parser to use. Available parsers: ieee, ssau. Default:
-                     ssau.
-  --help             Show this message and exit.
+  -s, --save TEXT         Path to file where to save the result of parsing.
+  -p, --parser TEXT       Parser to use. Available parsers: ieee, ssau.
+                          Default: ssau.
+  -v, --verbose           Whether to print output to stdout or not
+  -b, --beautify INTEGER  Number of line wraps between references. Default: 1
+  --help                  Show this message and exit.
 ```
 
 ### Usual way of using the script
 ```bash
 python -m references_parser parse in.txt
 ```
```

### Comparing `references_parser-1.0.0/references_parser/cli.py` & `references_parser-1.1.0/references_parser/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,32 +16,38 @@
     pass
 
 
 @cli.command()
 @click.argument('path', type=str)
 @click.option('-s', '--save', type=str, help='Path to file where to save the result of parsing.', default='')
 @click.option('-p', '--parser', type=str, help='Parser to use. Available parsers: ieee, ssau. Default: ssau.', default='ssau')
-def parse(path: str, save: str, parser: str, *args, **kwargs):
+@click.option('-v', '--verbose', is_flag=True, help='Whether to print output to stdout or not', default=False)
+@click.option('-b', '--beautify', type=int, help='Number of line wraps between references. Default: 1', default=1)
+def parse(path: str, save: str, parser: str, verbose: bool, beautify: int):
     with open(path, 'r', encoding='utf-8') as f:
         citations = f.read()
 
     parser_type = parser.lower()
     parser = PARSER_MAPPING.get(parser_type)
     if parser is None:
         raise ValueError(f"Unknown parser type. Expect one of {list(PARSER_MAPPING.keys())}, but received"
                          f"{parser_type}")
 
     result = parser(citations)
-    for entry in result:
-        print(entry, end="\n\n")
+    
+    end = "".join(["\n" for _ in range(beautify)])
+    
+    if verbose:
+        for entry in result:
+            print(entry, end=end)
 
     if save:
         with open(save, 'w', encoding='utf-8') as f:
             for entry in result:
-                f.write(entry + '\n\n')
+                f.write(entry + end)
         print(f'Saved result to {save}.')
 
 
 @cli.command()
 @click.argument('path', type=str)
 def prepare_urls(path: str):
     with open(path, 'r', encoding='utf-8') as f:
```

### Comparing `references_parser-1.0.0/references_parser/parsers/IeeeParser.py` & `references_parser-1.1.0/references_parser/parsers/IeeeParser.py`

 * *Files identical despite different names*

### Comparing `references_parser-1.0.0/references_parser/parsers/SsauParser.py` & `references_parser-1.1.0/references_parser/parsers/SsauParser.py`

 * *Files identical despite different names*

### Comparing `references_parser-1.0.0/references_parser.egg-info/PKG-INFO` & `references_parser-1.1.0/references_parser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: references-parser
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tool for parsing bibtex in ssau's format
 Home-page: https://github.com/Banayaki/ReferencesParser
 Author: Mukhin Artem
 Author-email: artemmukhinssau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
@@ -14,22 +14,24 @@
 ```bash
 pip install references-parser
 ```
 # Usage
 
 ### Use help to see CLI parameters
 ```bash
-➜ python -m references_parser parse --help
+➜ python -m references_parser parse --help        
 Usage: python -m references_parser parse [OPTIONS] PATH
 
 Options:
-  -s, --save TEXT    Path to file where to save the result of parsing.
-  -p, --parser TEXT  Parser to use. Available parsers: ieee, ssau. Default:
-                     ssau.
-  --help             Show this message and exit.
+  -s, --save TEXT         Path to file where to save the result of parsing.
+  -p, --parser TEXT       Parser to use. Available parsers: ieee, ssau.
+                          Default: ssau.
+  -v, --verbose           Whether to print output to stdout or not
+  -b, --beautify INTEGER  Number of line wraps between references. Default: 1
+  --help                  Show this message and exit.
 ```
 
 ### Usual way of using the script
 ```bash
 python -m references_parser parse in.txt
 ```
```

### Comparing `references_parser-1.0.0/setup.py` & `references_parser-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='references_parser',
     packages=setuptools.find_packages(),
-    version='1.0.0',
+    version='1.1.0',
     description="Tool for parsing bibtex in ssau's format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mukhin Artem',
     author_email='artemmukhinssau@gmail.com',
     url='https://github.com/Banayaki/ReferencesParser',
     include_package_data=True,
```

