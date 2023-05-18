# Comparing `tmp/chatcmd-1.0.15.tar.gz` & `tmp/chatcmd-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.15.tar", last modified: Mon May 15 22:45:35 2023, max compression
+gzip compressed data, was "chatcmd-1.0.16.tar", last modified: Thu May 18 21:30:17 2023, max compression
```

## Comparing `chatcmd-1.0.15.tar` & `chatcmd-1.0.16.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 22:45:35.259228 chatcmd-1.0.15/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.15/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5347 2023-05-15 22:45:35.258985 chatcmd-1.0.15/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3831 2023-05-15 22:45:03.000000 chatcmd-1.0.15/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 22:45:35.256468 chatcmd-1.0.15/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.15/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.15/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3525 2023-05-15 22:45:03.000000 chatcmd-1.0.15/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3770 2023-05-15 21:19:30.000000 chatcmd-1.0.15/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2783 2023-05-15 19:10:56.000000 chatcmd-1.0.15/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2602 2023-05-15 19:07:09.000000 chatcmd-1.0.15/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-15 22:45:35.258625 chatcmd-1.0.15/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5347 2023-05-15 22:45:35.000000 chatcmd-1.0.15/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-15 22:45:35.000000 chatcmd-1.0.15/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-15 22:45:35.000000 chatcmd-1.0.15/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-15 22:45:35.000000 chatcmd-1.0.15/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       28 2023-05-15 22:45:35.000000 chatcmd-1.0.15/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-15 22:45:35.000000 chatcmd-1.0.15/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1653 2023-05-15 22:45:03.000000 chatcmd-1.0.15/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-15 22:45:35.259305 chatcmd-1.0.15/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      537 2023-05-15 22:45:03.000000 chatcmd-1.0.15/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-18 21:30:17.453202 chatcmd-1.0.16/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.16/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5488 2023-05-18 21:30:17.452904 chatcmd-1.0.16/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-18 21:29:40.000000 chatcmd-1.0.16/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-18 21:30:17.450266 chatcmd-1.0.16/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.16/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-14 22:57:58.000000 chatcmd-1.0.16/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3525 2023-05-18 21:29:40.000000 chatcmd-1.0.16/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3770 2023-05-15 21:19:30.000000 chatcmd-1.0.16/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     2783 2023-05-15 19:10:56.000000 chatcmd-1.0.16/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2602 2023-05-15 19:07:09.000000 chatcmd-1.0.16/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-18 21:30:17.452490 chatcmd-1.0.16/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5488 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       28 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-18 21:30:17.000000 chatcmd-1.0.16/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1653 2023-05-18 21:29:40.000000 chatcmd-1.0.16/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-18 21:30:17.453286 chatcmd-1.0.16/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      537 2023-05-18 21:29:40.000000 chatcmd-1.0.16/setup.py
```

### Comparing `chatcmd-1.0.15/LICENSE` & `chatcmd-1.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.15/PKG-INFO` & `chatcmd-1.0.16/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.15
+Version: 1.0.16
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -54,22 +54,32 @@
 - Display library information.
 
 ## Requirements
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
+    pip3 install chatcmd
+    
+If pip not installed:
+
     python3 -m pip install chatcmd
 
+Installation output should display:
+
     Collecting chatcmd
-    Using cached chatcmd-1.0.15-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.16-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.15
+    Successfully installed chatcmd-1.0.16
 
 ### Uninstall ###
+    pip3 uninstall chatcmd
+
+If pip not installed:
+
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
 
 chatcmd [options]
```

### Comparing `chatcmd-1.0.15/README.md` & `chatcmd-1.0.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,32 @@
 - Display library information.
 
 ## Requirements
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
+    pip3 install chatcmd
+    
+If pip not installed:
+
     python3 -m pip install chatcmd
 
+Installation output should display:
+
     Collecting chatcmd
-    Using cached chatcmd-1.0.15-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.16-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.15
+    Successfully installed chatcmd-1.0.16
 
 ### Uninstall ###
+    pip3 uninstall chatcmd
+
+If pip not installed:
+
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
 
 chatcmd [options]
```

### Comparing `chatcmd-1.0.15/chatcmd/api.py` & `chatcmd-1.0.16/chatcmd/api.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.15/chatcmd/chatcmd.py` & `chatcmd-1.0.16/chatcmd/chatcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print('ChatCMD \033[32m1.0.15\033[0m')
+            print('ChatCMD \033[32m1.0.16\033[0m')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
```

### Comparing `chatcmd-1.0.15/chatcmd/commands.py` & `chatcmd-1.0.16/chatcmd/commands.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.15/chatcmd/helpers.py` & `chatcmd-1.0.16/chatcmd/helpers.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.15/chatcmd/lookup.py` & `chatcmd-1.0.16/chatcmd/lookup.py`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.15/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.16/chatcmd.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.15
+Version: 1.0.16
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -54,22 +54,32 @@
 - Display library information.
 
 ## Requirements
     Python >= 3.8.9
     OpenAI account and valid API key
     https://platform.openai.com/signup
 ## Installation
+    pip3 install chatcmd
+    
+If pip not installed:
+
     python3 -m pip install chatcmd
 
+Installation output should display:
+
     Collecting chatcmd
-    Using cached chatcmd-1.0.15-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.16-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.15
+    Successfully installed chatcmd-1.0.16
 
 ### Uninstall ###
+    pip3 uninstall chatcmd
+
+If pip not installed:
+
     python3 -m pip uninstall chatcmd
 ## Usage
 
 ```
 Usage:
 
 chatcmd [options]
```

### Comparing `chatcmd-1.0.15/pyproject.toml` & `chatcmd-1.0.16/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 65",
     "wheel >= 0.38",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.15"
+version = "1.0.16"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.15/setup.py` & `chatcmd-1.0.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.15",
+    version="1.0.16",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

