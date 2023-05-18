# Comparing `tmp/bardapi-0.1.6.tar.gz` & `tmp/bardapi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardapi-0.1.6.tar", last modified: Thu May 18 06:26:37 2023, max compression
+gzip compressed data, was "bardapi-0.1.7.tar", last modified: Thu May 18 07:02:24 2023, max compression
```

## Comparing `bardapi-0.1.6.tar` & `bardapi-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.426518 bardapi-0.1.6/
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     8139 2023-05-18 06:26:37.425507 bardapi-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7046 2023-05-18 06:23:46.000000 bardapi-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.410647 bardapi-0.1.6/bardapi/
--rw-rw-rw-   0        0        0      208 2023-05-18 06:26:01.000000 bardapi-0.1.6/bardapi/__init__.py
--rw-rw-rw-   0        0        0     4506 2023-05-18 06:23:59.000000 bardapi-0.1.6/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.422865 bardapi-0.1.6/bardapi.egg-info/
--rw-rw-rw-   0        0        0     8139 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 06:26:37.426518 bardapi-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1853 2023-05-18 06:25:27.000000 bardapi-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:02:24.452448 bardapi-0.1.7/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     8139 2023-05-18 07:02:24.451443 bardapi-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7046 2023-05-18 06:23:46.000000 bardapi-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 07:02:24.438265 bardapi-0.1.7/bardapi/
+-rw-rw-rw-   0        0        0      208 2023-05-18 07:02:04.000000 bardapi-0.1.7/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     3712 2023-05-18 07:02:07.000000 bardapi-0.1.7/bardapi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-18 07:02:24.449437 bardapi-0.1.7/bardapi.egg-info/
+-rw-rw-rw-   0        0        0     8139 2023-05-18 07:02:24.000000 bardapi-0.1.7/bardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-18 07:02:24.000000 bardapi-0.1.7/bardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 07:02:24.000000 bardapi-0.1.7/bardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 07:02:24.000000 bardapi-0.1.7/bardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 07:02:24.000000 bardapi-0.1.7/bardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 07:02:24.452448 bardapi-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1853 2023-05-18 07:02:09.000000 bardapi-0.1.7/setup.py
```

### Comparing `bardapi-0.1.6/LICENSE` & `bardapi-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bardapi-0.1.6/PKG-INFO` & `bardapi-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.6 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.7 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Natural Language :: Korean Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
```

### Comparing `bardapi-0.1.6/README.md` & `bardapi-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `bardapi-0.1.6/bardapi/core.py` & `bardapi-0.1.7/bardapi/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,60 @@
-import os
+import json
 import random
+import re
 import string
+import os
 import requests
-import json
-import re
 
 
 class Bard:
-    def __init__(
-        self, token=os.getenv("_BARD_API_KEY"), timeout=10, proxies=None, session=None
-    ):
+    def __init__(self, timeout=6, proxies=None, session=None):
         """
         Initialize Bard
 
-        :param token: (`str`, *optional*)
-            Enter the __Secure-1PSID value. defaults to os.getenv("_BARD_API_KEY")
         :param timeout: (`int`, *optional*)
             Timeout in seconds when connecting bard server. The timeout is used on each request.
         :param proxies: (`Dict[str, str]`, *optional*)
             A dictionary of proxy servers to use by protocol or endpoint, e.g., `{'http': 'foo.bar:3128',
             'http://hostname': 'foo.bar:4012'}`. The proxies are used on each request.
         :param session: (`requests.Session`, *optional*)
             An existing requests.Session object to be used for making HTTP requests.
         """
+        self.proxies = proxies
+        self.timeout = timeout
         headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) "
             "Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
         }
-        self.token, self.proxies, self.timeout = token, proxies, timeout
         self._reqid = int("".join(random.choices(string.digits, k=4)))
-        self.conversation_id = self.response_id = self.choice_id = ""
-        self.session = requests.Session() if session is None else session
-        self.session.headers = headers
-        self.session.cookies.set("__Secure-1PSID", self.token)
+        self.conversation_id = ""
+        self.response_id = ""
+        self.choice_id = ""
+
+        if session is None:
+            self.session = requests.Session()
+            self.session.headers = headers
+            self.session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+        else:
+            self.session = session
+
         self.SNlM0e = self._get_snim0e()
 
     def _get_snim0e(self):
-        if self.token and self.token[-1] != ".":
-            raise Exception(
-                "__Secure-1PSID value must end with a single dot. Enter correct __Secure-1PSID value."
-            )
-        elif not self.token:
-            raise Exception("No token value entered.")
         resp = self.session.get(
-            "https://bard.google.com/", timeout=self.timeout, proxies=self.proxies
+            url="https://bard.google.com/", timeout=self.timeout, proxies=self.proxies
         )
         if resp.status_code != 200:
-            raise Exception(
-                f"Response code not 200. \n - Try Bard on https://bard.google.com/ \n "
-                f"- Check service area on https://support.google.com/bard/answer/13575153?hl=en. \n "
-                f"- Response Status is {resp.status_code}"
-            )
-        snim0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text)
-        if not snim0e:
-            raise Exception(
-                "SNlM0e value not found in response. Check __Secure-1PSID value."
-            )
-        return snim0e.group(1)
+            raise Exception(f"Response Status: {resp.status_code}")
+        return re.search(r"SNlM0e\":\"(.*?)\"", resp.text).group(1)
 
     def get_answer(self, input_text: str) -> dict:
         params = {
             "bl": "boq_assistant-bard-web-server_20230419.00_p1",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
@@ -82,28 +71,24 @@
             "https://bard.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate",
             params=params,
             data=data,
             timeout=self.timeout,
             proxies=self.proxies,
         )
         resp_dict = json.loads(resp.content.splitlines()[3])[0][2]
-
-        if not resp_dict:
+        if resp_dict is None:
             return {"content": f"Response Error: {resp.content}."}
-
         parsed_answer = json.loads(resp_dict)
         bard_answer = {
             "content": parsed_answer[0][0],
             "conversation_id": parsed_answer[1][0],
             "response_id": parsed_answer[1][1],
             "factualityQueries": parsed_answer[3],
-            "textQuery": parsed_answer[2][0] if parsed_answer[2] else "",
+            "textQuery": parsed_answer[2][0] if parsed_answer[2] is not None else "",
             "choices": [{"id": i[0], "content": i[1]} for i in parsed_answer[4]],
         }
-        self.conversation_id, self.response_id, self.choice_id = (
-            bard_answer["conversation_id"],
-            bard_answer["response_id"],
-            bard_answer["choices"][0]["id"],
-        )
+        self.conversation_id = bard_answer["conversation_id"]
+        self.response_id = bard_answer["response_id"]
+        self.choice_id = bard_answer["choices"][0]["id"]
         self._reqid += 100000
 
-        return bard_answer
+        return bard_answer
```

### Comparing `bardapi-0.1.6/bardapi.egg-info/PKG-INFO` & `bardapi-0.1.7/bardapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.6
+Version: 0.1.7
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
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.6 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.7 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Natural Language :: Korean Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
```

### Comparing `bardapi-0.1.6/setup.py` & `bardapi-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="bardapi",
-    version="0.1.6",
+    version="0.1.7",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="The python package that returns Response of Google Bard through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/Bard-API",
     packages=find_packages(exclude=[]),
```

