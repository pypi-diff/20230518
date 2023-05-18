# Comparing `tmp/references_parser-0.2.4.tar.gz` & `tmp/references_parser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "references_parser-0.2.4.tar", last modified: Sun May 14 16:28:00 2023, max compression
+gzip compressed data, was "references_parser-1.0.0.tar", last modified: Thu May 18 06:25:01 2023, max compression
```

## Comparing `references_parser-0.2.4.tar` & `references_parser-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:28:00.279685 references_parser-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-14 16:28:00.279685 references_parser-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-14 16:27:47.000000 references_parser-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-14 16:27:47.000000 references_parser-0.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:28:00.279685 references_parser-0.2.4/references_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:28:00.279685 references_parser-0.2.4/references_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/parsers/IeeeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/parsers/SsauParser.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:28:00.279685 references_parser-0.2.4/references_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:28:00.279685 references_parser-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-14 16:27:47.000000 references_parser-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:25:01.091219 references_parser-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-18 06:25:01.091219 references_parser-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-18 06:24:45.000000 references_parser-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 06:24:45.000000 references_parser-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:25:01.091219 references_parser-1.0.0/references_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:25:01.091219 references_parser-1.0.0/references_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/parsers/IeeeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/parsers/SsauParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 06:24:45.000000 references_parser-1.0.0/references_parser/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:25:01.091219 references_parser-1.0.0/references_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 06:25:01.000000 references_parser-1.0.0/references_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:25:01.095219 references_parser-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 06:24:45.000000 references_parser-1.0.0/setup.py
```

### Comparing `references_parser-0.2.4/references_parser/parse.py` & `references_parser-1.0.0/references_parser/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,57 @@
-import argparse
+import click
+from .converters.url_converter import convert_urls_to_bibtex
 from .parsers import SsauParser
 from .parsers import IEEEParser
 
+
 PARSER_MAPPING = {
     'ssau': SsauParser(),
     'ieee': IEEEParser(),
 
 }
 
-if __name__ == '__main__':
-    argparser = argparse.ArgumentParser()
-    argparser.add_argument('path', type=str,
-                           help='Path to the file containing bibtext citations.')
-    argparser.add_argument('-s', '--save', type=str,
-                           help='Path to file where to save the result of parsing.', default='')
-    argparser.add_argument('-p', '--parser', type=str,
-                           help='Parser to use. Available parsers: ieee, ssau. Default: ssau.', default='ssau')
 
-    args = argparser.parse_args()
-    with open(args.path, 'r', encoding='utf-8') as f:
+@click.group()
+def cli():
+    pass
+
+
+@cli.command()
+@click.argument('path', type=str)
+@click.option('-s', '--save', type=str, help='Path to file where to save the result of parsing.', default='')
+@click.option('-p', '--parser', type=str, help='Parser to use. Available parsers: ieee, ssau. Default: ssau.', default='ssau')
+def parse(path: str, save: str, parser: str, *args, **kwargs):
+    with open(path, 'r', encoding='utf-8') as f:
         citations = f.read()
 
-    parser_type = args.parser.lower()
+    parser_type = parser.lower()
     parser = PARSER_MAPPING.get(parser_type)
     if parser is None:
         raise ValueError(f"Unknown parser type. Expect one of {list(PARSER_MAPPING.keys())}, but received"
                          f"{parser_type}")
 
     result = parser(citations)
     for entry in result:
         print(entry, end="\n\n")
 
-    if args.save != '':
-        with open(args.save, 'w', encoding='utf-8') as f:
+    if save:
+        with open(save, 'w', encoding='utf-8') as f:
             for entry in result:
                 f.write(entry + '\n\n')
-        print(f'Saved result to {args.save}.')
+        print(f'Saved result to {save}.')
+
+
+@cli.command()
+@click.argument('path', type=str)
+def prepare_urls(path: str):
+    with open(path, 'r', encoding='utf-8') as f:
+        citations = f.read()
+        
+    citations = convert_urls_to_bibtex(citations)
+    
+    with open(path, 'w', encoding='utf-8') as f:
+        f.write(citations)
+        
+        
+if __name__ == '__main__':
+    cli()
```

### Comparing `references_parser-0.2.4/references_parser/parsers/IeeeParser.py` & `references_parser-1.0.0/references_parser/parsers/IeeeParser.py`

 * *Files identical despite different names*

### Comparing `references_parser-0.2.4/setup.py` & `references_parser-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,22 +3,32 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='references_parser',
     packages=setuptools.find_packages(),
-    version='0.2.4',
+    version='1.0.0',
     description="Tool for parsing bibtex in ssau's format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mukhin Artem',
     author_email='artemmukhinssau@gmail.com',
     url='https://github.com/Banayaki/ReferencesParser',
     include_package_data=True,
     classifiers=[
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
-    ], install_requires=[
-        'bibtexparser~=1.2.0'
-    ]
+    ], 
+    install_requires=[
+        "beautifulsoup4==4.12.2",
+        "bibtexparser==1.4.0",
+        "click==8.1.3",
+        "duckpy==3.2.0",
+        "Requests==2.30.0",
+    ],
+    entry_points={
+        'console_scripts': [
+            'references_parser=references_parser.cli:main'
+        ]
+    }
 )
```

