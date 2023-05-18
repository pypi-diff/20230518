# Comparing `tmp/catprompt-0.1.1.tar.gz` & `tmp/catprompt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catprompt-0.1.1.tar", last modified: Wed May  3 15:23:38 2023, max compression
+gzip compressed data, was "catprompt-0.2.0.tar", last modified: Thu May 18 08:42:25 2023, max compression
```

## Comparing `catprompt-0.1.1.tar` & `catprompt-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-03 15:23:38.623459 catprompt-0.1.1/
--rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.1.1/LICENSE
--rw-r--r--   0 juanre     (501) staff       (20)     8875 2023-05-03 15:23:38.623254 catprompt-0.1.1/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)     7248 2023-05-03 15:18:22.000000 catprompt-0.1.1/README.md
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-03 15:23:38.622101 catprompt-0.1.1/catprompt/
--rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.1.1/catprompt/__init__.py
--rw-r--r--   0 juanre     (501) staff       (20)     7216 2023-05-03 14:28:16.000000 catprompt-0.1.1/catprompt/prompter.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-03 15:23:38.622711 catprompt-0.1.1/catprompt.egg-info/
--rw-r--r--   0 juanre     (501) staff       (20)     8875 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)      328 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/SOURCES.txt
--rw-r--r--   0 juanre     (501) staff       (20)        1 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/dependency_links.txt
--rw-r--r--   0 juanre     (501) staff       (20)       54 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/entry_points.txt
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/requires.txt
--rw-r--r--   0 juanre     (501) staff       (20)       10 2023-05-03 15:23:38.000000 catprompt-0.1.1/catprompt.egg-info/top_level.txt
--rw-r--r--   0 juanre     (501) staff       (20)      832 2023-05-03 15:21:54.000000 catprompt-0.1.1/pyproject.toml
--rw-r--r--   0 juanre     (501) staff       (20)       38 2023-05-03 15:23:38.623491 catprompt-0.1.1/setup.cfg
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.1.1/setup.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-03 15:23:38.623090 catprompt-0.1.1/test/
--rw-r--r--   0 juanre     (501) staff       (20)      796 2023-04-28 10:52:58.000000 catprompt-0.1.1/test/test_example.py
--rw-r--r--   0 juanre     (501) staff       (20)     3900 2023-05-03 14:03:45.000000 catprompt-0.1.1/test/test_prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-18 08:42:25.147489 catprompt-0.2.0/
+-rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.2.0/LICENSE
+-rw-r--r--   0 juanre     (501) staff       (20)     8919 2023-05-18 08:42:25.147344 catprompt-0.2.0/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)     7292 2023-05-18 08:39:14.000000 catprompt-0.2.0/README.md
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-18 08:42:25.145918 catprompt-0.2.0/catprompt/
+-rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.2.0/catprompt/__init__.py
+-rw-r--r--   0 juanre     (501) staff       (20)     7422 2023-05-18 08:39:35.000000 catprompt-0.2.0/catprompt/prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-18 08:42:25.146556 catprompt-0.2.0/catprompt.egg-info/
+-rw-r--r--   0 juanre     (501) staff       (20)     8919 2023-05-18 08:42:25.000000 catprompt-0.2.0/catprompt.egg-info/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)      328 2023-05-18 08:42:25.000000 catprompt-0.2.0/catprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 juanre     (501) staff       (20)        1 2023-05-18 08:42:25.000000 catprompt-0.2.0/catprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       54 2023-05-18 08:42:25.000000 catprompt-0.2.0/catprompt.egg-info/entry_points.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-05-18 08:42:25.000000 catprompt-0.2.0/catprompt.egg-info/requires.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       10 2023-05-18 08:42:25.000000 catprompt-0.2.0/catprompt.egg-info/top_level.txt
+-rw-r--r--   0 juanre     (501) staff       (20)      832 2023-05-18 08:39:45.000000 catprompt-0.2.0/pyproject.toml
+-rw-r--r--   0 juanre     (501) staff       (20)       38 2023-05-18 08:42:25.147523 catprompt-0.2.0/setup.cfg
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.2.0/setup.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-05-18 08:42:25.146967 catprompt-0.2.0/test/
+-rw-r--r--   0 juanre     (501) staff       (20)      796 2023-04-28 10:52:58.000000 catprompt-0.2.0/test/test_example.py
+-rw-r--r--   0 juanre     (501) staff       (20)     3900 2023-05-03 14:03:45.000000 catprompt-0.2.0/test/test_prompter.py
```

### Comparing `catprompt-0.1.1/LICENSE` & `catprompt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `catprompt-0.1.1/PKG-INFO` & `catprompt-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.1.1
+Version: 0.2.0
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -56,24 +56,25 @@
 `catprompt [-r reverse_file] [-f flavor] path/to/prompt.txt [path/to/other-prompts.txt] [-c config_file]`
 
 4. Use the processed content from the clipboard in ChatGPT.
 
 ### Options
 
 - `-c`, `--config`: Specify one or more configuration files containing private words and flavors (default: ~/.catprompt.ini and ./catprompt.ini).
-- `-r`, `--reverse`: Reverse the privatization from a given file and output the original content to stdout.
+- `-u`, `--unscramble`: Reverse the scrambling of private words from a given file, output to stdout.
 - `-f`, `--flavor`: Use a flavor to prefix the output, extracted from the config file.
+- `-v`, `--stay-verbose`: Do not append "Be concise" to the prompt.
 
 ## Configuration Files (ini files)
 
 Configuration files (`.ini` format) can be used to store private words and flavors. By default, catprompt looks for configuration files at `~/.catprompt.ini` and `./catprompt.ini`. You can specify other locations using the `-c` or `--config` option.
 
 ### Private Words
 
-Private words are words that should be replaced with placeholders in the output. To define private words, create a section called `PrivateWords` and list them as a comma-separated string under the `list` key:
+Private words are words that should be scrambled in the output. To define private words, create a section called `PrivateWords` and list them as a comma-separated string under the `list` key:
 
 ```
 [PrivateWords]
 list = private_word_1, private_word_2, private_word_3
 ```
```

### Comparing `catprompt-0.1.1/README.md` & `catprompt-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,25 @@
 `catprompt [-r reverse_file] [-f flavor] path/to/prompt.txt [path/to/other-prompts.txt] [-c config_file]`
 
 4. Use the processed content from the clipboard in ChatGPT.
 
 ### Options
 
 - `-c`, `--config`: Specify one or more configuration files containing private words and flavors (default: ~/.catprompt.ini and ./catprompt.ini).
-- `-r`, `--reverse`: Reverse the privatization from a given file and output the original content to stdout.
+- `-u`, `--unscramble`: Reverse the scrambling of private words from a given file, output to stdout.
 - `-f`, `--flavor`: Use a flavor to prefix the output, extracted from the config file.
+- `-v`, `--stay-verbose`: Do not append "Be concise" to the prompt.
 
 ## Configuration Files (ini files)
 
 Configuration files (`.ini` format) can be used to store private words and flavors. By default, catprompt looks for configuration files at `~/.catprompt.ini` and `./catprompt.ini`. You can specify other locations using the `-c` or `--config` option.
 
 ### Private Words
 
-Private words are words that should be replaced with placeholders in the output. To define private words, create a section called `PrivateWords` and list them as a comma-separated string under the `list` key:
+Private words are words that should be scrambled in the output. To define private words, create a section called `PrivateWords` and list them as a comma-separated string under the `list` key:
 
 ```
 [PrivateWords]
 list = private_word_1, private_word_2, private_word_3
 ```
```

### Comparing `catprompt-0.1.1/catprompt/prompter.py` & `catprompt-0.2.0/catprompt/prompter.py`

 * *Files 9% similar despite different names*

```diff
@@ -126,66 +126,68 @@
             replacement_map[word] = f"private{len(replacement_map)}"
 
         content = content.replace(word, replacement_map[word])
 
     return content
 
 
-def reverse_private_words(content, private_words):
+def unscramble_private_words(content, private_words):
     replacement_map = {}
     for word in private_words:
         if word not in replacement_map:
             replacement_map[word] = f"private{len(replacement_map)}"
 
-    reversed_map = {v: k for k, v in replacement_map.items()}
+    unscrambled_map = {v: k for k, v in replacement_map.items()}
 
-    for key, value in reversed_map.items():
+    for key, value in unscrambled_map.items():
         content = content.replace(key, value)
 
     return content
 
 
 def main():
     parser = argparse.ArgumentParser(
-        description="Process text files and copy processed content to the clipboard")
-    parser.add_argument("input_files", metavar="input_file", type=str, nargs="*",
-                        help="Input file(s) to process")
-    parser.add_argument("-c", "--config", metavar="config_file", type=str, nargs="*",
-                        default=[os.path.expanduser("~/.catprompt.ini"), "catprompt.ini"],
-                        help=("Configuration file(s) containing private words and "
-                              "flavors: (default: ~/.catprompt.ini and ./catprompt.ini)"))
-    parser.add_argument("-r", "--reverse", metavar="reverse_file", type=str,
-                        help=("Reverse the privatization from a given file and output "
-                              "the original content to stdout"))
-    parser.add_argument("-f", "--flavor", metavar="flavor", type=str,
-                        help=("The flavor to use to prefix the output, extracted"
-                              "from the config file file"))
+        description='Process text files and copy processed content to the clipboard')
+    parser.add_argument('input_files', metavar='input_file', type=str, nargs='*',
+                        help='Input file(s) to process')
+    parser.add_argument('-c', '--config', metavar='config_file', type=str, nargs='*',
+                        default=[os.path.expanduser('~/.catprompt.ini'), 'catprompt.ini'],
+                        help=('Configuration file(s) containing private words and '
+                              'flavors: (default: ~/.catprompt.ini and ./catprompt.ini)'))
+    parser.add_argument('-u', '--unscramble', type=str,
+                        help=('Reverse the scrambling of private words from a given file, '
+                              'output to stdout'))
+    parser.add_argument('-f', '--flavor', type=str,
+                        help=('The flavor to use to prefix the output, extracted'
+                              'from the config file file'))
+    parser.add_argument('-v', '--stay-verbose', action='store_true',
+                        help='Do not append "Be concise" to the prompt.')
 
     args = parser.parse_args()
 
-    if not args.input_files and not args.reverse:
-        print("Error: No input files or reverse file specified.")
+    if not args.input_files and not args.unscramble:
+        print('Error: No input files or file to unscramble specified.')
         sys.exit(1)
 
     config_files = args.config
 
     private_words, flavors = read_config_files(config_files)
 
     flavor_text = ""
     if args.flavor:
         flavor = args.flavor.lower()
         if flavor not in flavors:
             print(f"Error: Flavor '{args.flavor}' not found in the configuration files.")
             sys.exit(1)
         flavor_text = flavors[flavor]
 
-    if args.reverse:
-        with open(args.reverse, "r", encoding='utf-8') as reverse_file:
-            content = reverse_file.read()
-            original_content = reverse_private_words(content, private_words)
+    if args.unscramble:
+        with open(args.unscramble, "r", encoding='utf-8') as unscramble_file:
+            content = unscramble_file.read()
+            original_content = unscramble_private_words(content, private_words)
             print(original_content)
             return
 
     input_files = args.input_files
     processed_lines = []
 
     for input_file in input_files:
@@ -195,14 +197,18 @@
             sys.exit(1)
         print(f'Reading {input_file}')
         process_file(file_path, processed_lines)
 
     processed_content = "\n".join(filter(None, processed_lines))
     processed_content = flavor_text + '\n\n' + \
         replace_private_words(processed_content, private_words)
+
+    if not args.stay_verbose:
+        processed_content += '\n\nBe concise.'
+
     clipboard.copy(processed_content)
 
     encoding = 'cl100k_base'
     tokenizer = tiktoken.get_encoding(encoding)
     tokens = tokenizer.encode(processed_content)
     print(f"Processed content copied to clipboard, {len(tokens)} {encoding} tokens")
```

### Comparing `catprompt-0.1.1/catprompt.egg-info/PKG-INFO` & `catprompt-0.2.0/catprompt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.1.1
+Version: 0.2.0
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -56,24 +56,25 @@
 `catprompt [-r reverse_file] [-f flavor] path/to/prompt.txt [path/to/other-prompts.txt] [-c config_file]`
 
 4. Use the processed content from the clipboard in ChatGPT.
 
 ### Options
 
 - `-c`, `--config`: Specify one or more configuration files containing private words and flavors (default: ~/.catprompt.ini and ./catprompt.ini).
-- `-r`, `--reverse`: Reverse the privatization from a given file and output the original content to stdout.
+- `-u`, `--unscramble`: Reverse the scrambling of private words from a given file, output to stdout.
 - `-f`, `--flavor`: Use a flavor to prefix the output, extracted from the config file.
+- `-v`, `--stay-verbose`: Do not append "Be concise" to the prompt.
 
 ## Configuration Files (ini files)
 
 Configuration files (`.ini` format) can be used to store private words and flavors. By default, catprompt looks for configuration files at `~/.catprompt.ini` and `./catprompt.ini`. You can specify other locations using the `-c` or `--config` option.
 
 ### Private Words
 
-Private words are words that should be replaced with placeholders in the output. To define private words, create a section called `PrivateWords` and list them as a comma-separated string under the `list` key:
+Private words are words that should be scrambled in the output. To define private words, create a section called `PrivateWords` and list them as a comma-separated string under the `list` key:
 
 ```
 [PrivateWords]
 list = private_word_1, private_word_2, private_word_3
 ```
```

### Comparing `catprompt-0.1.1/pyproject.toml` & `catprompt-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "catprompt"
-version = "0.1.1"
+version = "0.2.0"
 description = "Combine prompts for chatgpt."
 readme = "README.md"
 authors = [
     { name = "Juan Reyero", email="juan@juanreyero.com" }
 ]
 requires-python = ">=3.8"
 license = { file="LICENSE" }
```

### Comparing `catprompt-0.1.1/test/test_example.py` & `catprompt-0.2.0/test/test_example.py`

 * *Files identical despite different names*

### Comparing `catprompt-0.1.1/test/test_prompter.py` & `catprompt-0.2.0/test/test_prompter.py`

 * *Files identical despite different names*

