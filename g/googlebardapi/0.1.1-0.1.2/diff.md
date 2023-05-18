# Comparing `tmp/googlebardapi-0.1.1.tar.gz` & `tmp/googlebardapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googlebardapi-0.1.1.tar", last modified: Thu May 18 08:01:45 2023, max compression
+gzip compressed data, was "googlebardapi-0.1.2.tar", last modified: Thu May 18 14:07:16 2023, max compression
```

## Comparing `googlebardapi-0.1.1.tar` & `googlebardapi-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 08:01:45.882751 googlebardapi-0.1.1/
--rw-rw-rw-   0        0        0     1067 2023-05-18 07:20:15.000000 googlebardapi-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     8145 2023-05-18 08:01:45.881734 googlebardapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6861 2023-05-18 07:20:15.000000 googlebardapi-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 08:01:45.863782 googlebardapi-0.1.1/bardapi/
--rw-rw-rw-   0        0        0      200 2023-05-18 08:01:32.000000 googlebardapi-0.1.1/bardapi/__init__.py
--rw-rw-rw-   0        0        0     4106 2023-05-18 08:01:12.000000 googlebardapi-0.1.1/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:01:45.879328 googlebardapi-0.1.1/googlebardapi.egg-info/
--rw-rw-rw-   0        0        0     8145 2023-05-18 08:01:45.000000 googlebardapi-0.1.1/googlebardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-18 08:01:45.000000 googlebardapi-0.1.1/googlebardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 08:01:45.000000 googlebardapi-0.1.1/googlebardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 08:01:45.000000 googlebardapi-0.1.1/googlebardapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 08:01:45.000000 googlebardapi-0.1.1/googlebardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 08:01:45.882751 googlebardapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1805 2023-05-18 08:01:26.000000 googlebardapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:07:16.849413 googlebardapi-0.1.2/
+-rw-rw-rw-   0        0        0     1067 2023-05-18 07:20:15.000000 googlebardapi-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     8145 2023-05-18 14:07:16.848410 googlebardapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6861 2023-05-18 07:20:15.000000 googlebardapi-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 14:07:16.824940 googlebardapi-0.1.2/bardapi/
+-rw-rw-rw-   0        0        0      200 2023-05-18 14:06:55.000000 googlebardapi-0.1.2/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     3990 2023-05-18 14:06:21.000000 googlebardapi-0.1.2/bardapi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-18 14:07:16.846408 googlebardapi-0.1.2/googlebardapi.egg-info/
+-rw-rw-rw-   0        0        0     8145 2023-05-18 14:07:16.000000 googlebardapi-0.1.2/googlebardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-18 14:07:16.000000 googlebardapi-0.1.2/googlebardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 14:07:16.000000 googlebardapi-0.1.2/googlebardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 14:07:16.000000 googlebardapi-0.1.2/googlebardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 14:07:16.000000 googlebardapi-0.1.2/googlebardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 14:07:16.849413 googlebardapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1805 2023-05-18 14:06:52.000000 googlebardapi-0.1.2/setup.py
```

### Comparing `googlebardapi-0.1.1/LICENSE` & `googlebardapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `googlebardapi-0.1.1/PKG-INFO` & `googlebardapi-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googlebardapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: googlebardapi Version: 0.1.1 Summary: The python
+Metadata-Version: 2.1 Name: googlebardapi Version: 0.1.2 Summary: The python
 package that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Natural Language :: Korean Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
```

### Comparing `googlebardapi-0.1.1/README.md` & `googlebardapi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `googlebardapi-0.1.1/bardapi/core.py` & `googlebardapi-0.1.2/bardapi/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,110 @@
 import os
 import random
-import string
-import requests
+import aiohttp
+import asyncio
 import json
-import re
 
 
 class Bard:
     HEADERS = {
         "Host": "bard.google.com",
         "X-Same-Domain": "1",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
         "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
         "Origin": "https://bard.google.com",
         "Referer": "https://bard.google.com/",
     }
 
-    def __init__(self, token=None, timeout=20, proxies=None, session=None):
-        """
-        Initialize Bard
-
-        :param token: (`str`, *optional*)
-            __Secure-1PSID value. default to os.getenv("_BARD_API_KEY")
-        :param timeout: (`int`, *optional*)
-            Timeout in seconds when connecting bard server. The timeout is used on each request.
-        :param proxies: (`Dict[str, str]`, *optional*)
-            A dictionary of proxy servers to use by protocol or endpoint, e.g., `{'http': 'foo.bar:3128',
-            'http://hostname': 'foo.bar:4012'}`. The proxies are used on each requpest.
-        :param session: (`requests.Session`, *optional*)
-            An existing requests.Session object to be used for making HTTP requests.
-        """
+    session = None
+
+    def __init__(self, token=None, timeout=20, proxies=None):
         self.token = token or os.getenv("_BARD_API_KEY")
-        self.proxies = proxies
         self.timeout = timeout
-        self._reqid = int("".join(random.choices(string.digits, k=4)))
+        self.proxies = proxies
+        self._reqid = random.randint(10000, 99999)
         self.conversation_id = ""
         self.response_id = ""
         self.choice_id = ""
-        self.session = session or requests.Session()
-        self.session.headers = self.HEADERS
-        self.session.cookies.set("__Secure-1PSID", self.token)
-        self.SNlM0e = self._get_snim0e()
+        self.SNlM0e = None
+
+    async def create_session(self):
+        return aiohttp.ClientSession()
 
-    def _get_snim0e(self):
+    async def initialize(self):
         if not self.token or self.token[-1] != ".":
-            raise Exception(
-                "__Secure-1PSID value must end with a single dot. Enter correct __Secure-1PSID value."
-            )
-        resp = self.session.get(
-            "https://bard.google.com/", timeout=self.timeout, proxies=self.proxies
+            raise ValueError("__Secure-1PSID value must end with a single dot. Enter the correct __Secure-1PSID value.")
+        if Bard.session is None:
+            Bard.session = await self.create_session()
+
+        resp = await Bard.session.get(
+            "https://bard.google.com/",
+            timeout=self.timeout,
+            proxy=self.proxies,
+            headers=self.HEADERS,
+            cookies={"__Secure-1PSID": self.token},
         )
-        if resp.status_code != 200:
-            raise Exception(
-                f"Response code not 200. Response Status is {resp.status_code}"
-            )
-        snim0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text)
-        if not snim0e:
-            raise Exception(
-                "SNlM0e value not found in response. Check __Secure-1PSID value."
-            )
-        return snim0e.group(1)
+        resp.raise_for_status()
+        resp_text = await resp.text()
+        snim0e_start = resp_text.find('SNlM0e":"')
+        if snim0e_start == -1:
+            raise ValueError("SNlM0e value not found in the response. Check the __Secure-1PSID value.")
+        snim0e_start += 9
+        snim0e_end = resp_text.find('"', snim0e_start)
+        if snim0e_end == -1:
+            raise ValueError("SNlM0e value not found in the response. Check the __Secure-1PSID value.")
+        self.SNlM0e = resp_text[snim0e_start:snim0e_end]
+
+    def get_session(self):
+        if Bard.session is None:
+            loop = asyncio.get_event_loop()
+            Bard.session = loop.run_until_complete(self.create_session())
+        return Bard.session
 
-    def get_answer(self, input_text: str) -> dict:
+    async def get_answer(self, input_text):
+        session = self.get_session()
         params = {
             "bl": "boq_assistant-bard-web-server_20230419.00_p1",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
         input_text_struct = [
             [input_text],
             None,
             [self.conversation_id, self.response_id, self.choice_id],
         ]
         data = {
-            "f.req": json.dumps([None, json.dumps(input_text_struct)]),
+            "f.req": [None, json.dumps(input_text_struct)],
             "at": self.SNlM0e,
         }
-        resp = self.session.post(
+
+        async with session.post(
             "https://bard.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate",
             params=params,
-            data=data,
+            json=data,
             timeout=self.timeout,
-            proxies=self.proxies,
-        )
-        resp_dict = json.loads(resp.content.splitlines()[3])[0][2]
-
-        if not resp_dict:
-            return {"content": f"Response Error: {resp.content}."}
-        parsed_answer = json.loads(resp_dict)
-        bard_answer = {
-            "content": parsed_answer[0][0],
-            "conversation_id": parsed_answer[1][0],
-            "response_id": parsed_answer[1][1],
-            "factualityQueries": parsed_answer[3],
-            "textQuery": parsed_answer[2][0] if parsed_answer[2] else "",
-            "choices": [{"id": i[0], "content": i[1]} for i in parsed_answer[4]],
-        }
-        self.conversation_id, self.response_id, self.choice_id = (
-            bard_answer["conversation_id"],
-            bard_answer["response_id"],
-            bard_answer["choices"][0]["id"],
-        )
-        self._reqid += 100000
+            proxy=self.proxies,
+            headers=self.HEADERS,
+        ) as resp:
+            resp.raise_for_status()
+            resp_json = await resp.json()
+            resp_dict = resp_json[0][2]
+
+            if not resp_dict:
+                return {"content": f"Response Error: {resp.content}."}
+            parsed_answer = json.loads(resp_dict)
+            bard_answer = {
+                "content": parsed_answer[0][0],
+                "conversation_id": parsed_answer[1][0],
+                "response_id": parsed_answer[1][1],
+                "factualityQueries": parsed_answer[3],
+                "textQuery": parsed_answer[2][0] if parsed_answer[2] else "",
+                "choices": [{"id": i[0], "content": i[1]} for i in parsed_answer[4]],
+            }
+            self.conversation_id, self.response_id, self.choice_id = (
+                bard_answer["conversation_id"],
+                bard_answer["response_id"],
+                bard_answer["choices"][0]["id"],
+            )
+            self._reqid += 100000
 
-        return bard_answer
+            return bard_answer
```

### Comparing `googlebardapi-0.1.1/googlebardapi.egg-info/PKG-INFO` & `googlebardapi-0.1.2/googlebardapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googlebardapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: googlebardapi Version: 0.1.1 Summary: The python
+Metadata-Version: 2.1 Name: googlebardapi Version: 0.1.2 Summary: The python
 package that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Natural Language :: Korean Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
```

### Comparing `googlebardapi-0.1.1/setup.py` & `googlebardapi-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="googlebardapi",
-    version="0.1.1",
+    version="0.1.2",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="The python package that returns Response of Google Bard through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/Bard-API",
     packages=find_packages(exclude=[]),
```

