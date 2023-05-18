# Comparing `tmp/mailtrap-2.0.0.tar.gz` & `tmp/mailtrap-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailtrap-2.0.0.tar", last modified: Sat Mar 11 10:02:00 2023, max compression
+gzip compressed data, was "mailtrap-2.0.1.tar", last modified: Thu May 18 15:49:17 2023, max compression
```

## Comparing `mailtrap-2.0.0.tar` & `mailtrap-2.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 leonid     (501) staff       (20)        0 2023-03-11 10:02:00.115364 mailtrap-2.0.0/
--rw-r--r--   0 leonid     (501) staff       (20)     1096 2023-03-10 21:28:24.000000 mailtrap-2.0.0/LICENSE.txt
-drwxr-xr-x   0 leonid     (501) staff       (20)        0 2023-03-11 10:02:00.112283 mailtrap-2.0.0/Mailtrap.egg-info/
--rw-r--r--   0 leonid     (501) staff       (20)     7655 2023-03-11 10:02:00.000000 mailtrap-2.0.0/Mailtrap.egg-info/PKG-INFO
--rw-r--r--   0 leonid     (501) staff       (20)      600 2023-03-11 10:02:00.000000 mailtrap-2.0.0/Mailtrap.egg-info/SOURCES.txt
--rw-r--r--   0 leonid     (501) staff       (20)        1 2023-03-11 10:02:00.000000 mailtrap-2.0.0/Mailtrap.egg-info/dependency_links.txt
--rw-r--r--   0 leonid     (501) staff       (20)       17 2023-03-11 10:02:00.000000 mailtrap-2.0.0/Mailtrap.egg-info/requires.txt
--rw-r--r--   0 leonid     (501) staff       (20)        9 2023-03-11 10:02:00.000000 mailtrap-2.0.0/Mailtrap.egg-info/top_level.txt
--rw-r--r--   0 leonid     (501) staff       (20)     7655 2023-03-11 10:02:00.115141 mailtrap-2.0.0/PKG-INFO
--rw-r--r--   0 leonid     (501) staff       (20)     5350 2023-03-11 10:00:28.000000 mailtrap-2.0.0/README.md
-drwxr-xr-x   0 leonid     (501) staff       (20)        0 2023-03-11 10:02:00.112850 mailtrap-2.0.0/mailtrap/
--rw-r--r--   0 leonid     (501) staff       (20)      348 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/__init__.py
--rw-r--r--   0 leonid     (501) staff       (20)     1553 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/client.py
--rw-r--r--   0 leonid     (501) staff       (20)      408 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/exceptions.py
-drwxr-xr-x   0 leonid     (501) staff       (20)        0 2023-03-11 10:02:00.114798 mailtrap-2.0.0/mailtrap/mail/
--rw-r--r--   0 leonid     (501) staff       (20)      230 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/mail/__init__.py
--rw-r--r--   0 leonid     (501) staff       (20)      414 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/mail/address.py
--rw-r--r--   0 leonid     (501) staff       (20)     1055 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/mail/attachment.py
--rw-r--r--   0 leonid     (501) staff       (20)     1726 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/mail/base.py
--rw-r--r--   0 leonid     (501) staff       (20)      416 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/mail/base_entity.py
--rw-r--r--   0 leonid     (501) staff       (20)     1420 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/mail/from_template.py
--rw-r--r--   0 leonid     (501) staff       (20)     1828 2023-03-10 21:28:24.000000 mailtrap-2.0.0/mailtrap/mail/mail.py
--rw-r--r--   0 leonid     (501) staff       (20)     1324 2023-03-11 09:57:36.000000 mailtrap-2.0.0/pyproject.toml
--rw-r--r--   0 leonid     (501) staff       (20)       38 2023-03-11 10:02:00.115419 mailtrap-2.0.0/setup.cfg
+drwxr-xr-x   0 vovapihol   (501) staff       (20)        0 2023-05-18 15:49:17.543429 mailtrap-2.0.1/
+-rw-r--r--   0 vovapihol   (501) staff       (20)     1096 2023-05-18 07:59:31.000000 mailtrap-2.0.1/LICENSE.txt
+-rw-r--r--   0 vovapihol   (501) staff       (20)     7659 2023-05-18 15:49:17.543119 mailtrap-2.0.1/PKG-INFO
+-rw-r--r--   0 vovapihol   (501) staff       (20)     5354 2023-05-18 07:59:31.000000 mailtrap-2.0.1/README.md
+drwxr-xr-x   0 vovapihol   (501) staff       (20)        0 2023-05-18 15:49:17.537932 mailtrap-2.0.1/mailtrap/
+-rw-r--r--   0 vovapihol   (501) staff       (20)      348 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/__init__.py
+-rw-r--r--   0 vovapihol   (501) staff       (20)     1677 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/client.py
+-rw-r--r--   0 vovapihol   (501) staff       (20)      408 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/exceptions.py
+drwxr-xr-x   0 vovapihol   (501) staff       (20)        0 2023-05-18 15:49:17.542612 mailtrap-2.0.1/mailtrap/mail/
+-rw-r--r--   0 vovapihol   (501) staff       (20)      230 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/mail/__init__.py
+-rw-r--r--   0 vovapihol   (501) staff       (20)      414 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/mail/address.py
+-rw-r--r--   0 vovapihol   (501) staff       (20)     1055 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/mail/attachment.py
+-rw-r--r--   0 vovapihol   (501) staff       (20)     1726 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/mail/base.py
+-rw-r--r--   0 vovapihol   (501) staff       (20)      416 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/mail/base_entity.py
+-rw-r--r--   0 vovapihol   (501) staff       (20)     1420 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/mail/from_template.py
+-rw-r--r--   0 vovapihol   (501) staff       (20)     1828 2023-05-18 07:59:31.000000 mailtrap-2.0.1/mailtrap/mail/mail.py
+drwxr-xr-x   0 vovapihol   (501) staff       (20)        0 2023-05-18 15:49:17.539876 mailtrap-2.0.1/mailtrap.egg-info/
+-rw-r--r--   0 vovapihol   (501) staff       (20)     7659 2023-05-18 15:49:17.000000 mailtrap-2.0.1/mailtrap.egg-info/PKG-INFO
+-rw-r--r--   0 vovapihol   (501) staff       (20)      441 2023-05-18 15:49:17.000000 mailtrap-2.0.1/mailtrap.egg-info/SOURCES.txt
+-rw-r--r--   0 vovapihol   (501) staff       (20)        1 2023-05-18 15:49:17.000000 mailtrap-2.0.1/mailtrap.egg-info/dependency_links.txt
+-rw-r--r--   0 vovapihol   (501) staff       (20)       17 2023-05-18 15:49:17.000000 mailtrap-2.0.1/mailtrap.egg-info/requires.txt
+-rw-r--r--   0 vovapihol   (501) staff       (20)        9 2023-05-18 15:49:17.000000 mailtrap-2.0.1/mailtrap.egg-info/top_level.txt
+-rw-r--r--   0 vovapihol   (501) staff       (20)     1324 2023-05-18 15:32:44.000000 mailtrap-2.0.1/pyproject.toml
+-rw-r--r--   0 vovapihol   (501) staff       (20)       38 2023-05-18 15:49:17.543516 mailtrap-2.0.1/setup.cfg
```

### Comparing `mailtrap-2.0.0/LICENSE.txt` & `mailtrap-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mailtrap-2.0.0/Mailtrap.egg-info/PKG-INFO` & `mailtrap-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailtrap
-Version: 2.0.0
+Version: 2.0.1
 Summary: Official mailtrap.io API client
 Author-email: Railsware Products Studio LLC <support@mailtrap.io>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Railsware Products Studio LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -204,12 +204,12 @@
 ```sh
 # To use the FORMER version of the mailtrap package, now known as Sendria:
 pip install --force-reinstall -v "mailtrap==1.0.1"
 ```
 
 ## License
 
-The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
+The project is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
 
 ## Code of Conduct
 
 Everyone interacting in the Mailtrap project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](CODE_OF_CONDUCT.md)
```

### Comparing `mailtrap-2.0.0/PKG-INFO` & `mailtrap-2.0.1/mailtrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailtrap
-Version: 2.0.0
+Version: 2.0.1
 Summary: Official mailtrap.io API client
 Author-email: Railsware Products Studio LLC <support@mailtrap.io>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Railsware Products Studio LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -204,12 +204,12 @@
 ```sh
 # To use the FORMER version of the mailtrap package, now known as Sendria:
 pip install --force-reinstall -v "mailtrap==1.0.1"
 ```
 
 ## License
 
-The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
+The project is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
 
 ## Code of Conduct
 
 Everyone interacting in the Mailtrap project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](CODE_OF_CONDUCT.md)
```

### Comparing `mailtrap-2.0.0/README.md` & `mailtrap-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -159,12 +159,12 @@
 ```sh
 # To use the FORMER version of the mailtrap package, now known as Sendria:
 pip install --force-reinstall -v "mailtrap==1.0.1"
 ```
 
 ## License
 
-The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
+The project is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
 
 ## Code of Conduct
 
 Everyone interacting in the Mailtrap project's codebases, issue trackers, chat rooms and mailing lists is expected to follow the [code of conduct](CODE_OF_CONDUCT.md)
```

### Comparing `mailtrap-2.0.0/mailtrap/client.py` & `mailtrap-2.0.1/mailtrap/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         return f"https://{self.api_host.rstrip('/')}:{self.api_port}"
 
     @property
     def headers(self) -> Dict[str, str]:
         return {
             "Authorization": f"Bearer {self.token}",
             "Content-Type": "application/json",
+            "User-Agent": (
+                "mailtrap-python (https://github.com/railsware/mailtrap-python)"
+            ),
         }
 
     @staticmethod
     def _handle_failed_response(response: requests.Response) -> NoReturn:
         status_code = response.status_code
         data = response.json()
```

### Comparing `mailtrap-2.0.0/mailtrap/mail/attachment.py` & `mailtrap-2.0.1/mailtrap/mail/attachment.py`

 * *Files identical despite different names*

### Comparing `mailtrap-2.0.0/mailtrap/mail/base.py` & `mailtrap-2.0.1/mailtrap/mail/base.py`

 * *Files identical despite different names*

### Comparing `mailtrap-2.0.0/mailtrap/mail/from_template.py` & `mailtrap-2.0.1/mailtrap/mail/from_template.py`

 * *Files identical despite different names*

### Comparing `mailtrap-2.0.0/mailtrap/mail/mail.py` & `mailtrap-2.0.1/mailtrap/mail/mail.py`

 * *Files identical despite different names*

### Comparing `mailtrap-2.0.0/pyproject.toml` & `mailtrap-2.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailtrap"
-version = "2.0.0"
+version = "2.0.1"
 description = "Official mailtrap.io API client"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Railsware Products Studio LLC", email = "support@mailtrap.io"}]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

