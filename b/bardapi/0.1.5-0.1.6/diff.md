# Comparing `tmp/bardapi-0.1.5.tar.gz` & `tmp/bardapi-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardapi-0.1.5.tar", last modified: Thu May 18 02:59:24 2023, max compression
+gzip compressed data, was "bardapi-0.1.6.tar", last modified: Thu May 18 06:26:37 2023, max compression
```

## Comparing `bardapi-0.1.5.tar` & `bardapi-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 02:59:24.365530 bardapi-0.1.5/
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     7841 2023-05-18 02:59:24.362525 bardapi-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6748 2023-05-17 18:58:35.000000 bardapi-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 02:59:24.337369 bardapi-0.1.5/bardapi/
--rw-rw-rw-   0        0        0      198 2023-05-18 02:59:01.000000 bardapi-0.1.5/bardapi/__init__.py
--rw-rw-rw-   0        0        0     3714 2023-05-17 16:54:40.000000 bardapi-0.1.5/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:59:24.357525 bardapi-0.1.5/bardapi.egg-info/
--rw-rw-rw-   0        0        0     7841 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 02:59:24.000000 bardapi-0.1.5/bardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 02:59:24.366529 bardapi-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1853 2023-05-18 02:58:49.000000 bardapi-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.426518 bardapi-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     8139 2023-05-18 06:26:37.425507 bardapi-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7046 2023-05-18 06:23:46.000000 bardapi-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.410647 bardapi-0.1.6/bardapi/
+-rw-rw-rw-   0        0        0      208 2023-05-18 06:26:01.000000 bardapi-0.1.6/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     4506 2023-05-18 06:23:59.000000 bardapi-0.1.6/bardapi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-18 06:26:37.422865 bardapi-0.1.6/bardapi.egg-info/
+-rw-rw-rw-   0        0        0     8139 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 06:26:37.000000 bardapi-0.1.6/bardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 06:26:37.426518 bardapi-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1853 2023-05-18 06:25:27.000000 bardapi-0.1.6/setup.py
```

### Comparing `bardapi-0.1.5/LICENSE` & `bardapi-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bardapi-0.1.5/PKG-INFO` & `bardapi-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.5
+Version: 0.1.6
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -77,83 +77,95 @@
 <br>
 
 ## Usage 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) 
 
 
 Simple Usage
+
 ```python
 from bardapi import Bard
-import os
 
+token = 'xxxxxxxxxx'
+bard = Bard(token=token)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+```
+Or you can use this
+```python
+from bardapi import Bard
+import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
+
 Bard().get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
-
-Or you can use this
+To get reponse dictionary
 ```python
 import bardapi
 import os
 
 # set your __Secure-1PSID value to key
-os.environ['_BARD_API_KEY']="xxxxxxxx"
+token = 'xxxxxxxxxx'
 
 # set your input text
 input_text = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 
 # Send an API request and get a response.
-response = bardapi.core.Bard().get_answer(input_text)
+response = bardapi.core.Bard(token).get_answer(input_text)
 ```
 
+
+
 Addressing errors caused by delayed responses in environments like Google Colab and containers. If an error occurs despite following the proper procedure, utilize the timeout argument.
 ```python
 from bardapi import Bard
 import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 
-bard = Bard(timeout=10) # Set timeout in seconds
+bard = Bard(timeout=30) # Set timeout in seconds
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 <br>
 
 ## Futher
 ### Behind a proxy
 If you are working behind a proxy, use the following.
 ```python
 from bardapi import Bard
 import os
-
 os.environ['_BARD_API_KEY']="xxxxxxxx"
+
 # Change 'http://127.0.0.1:1080' to your http proxy
 # timeout in seconds
 bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 ### Reusable session object
 ```python
 from bardapi import Bard
 import os
 import requests
-
 os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx'
+# token='xxxxxxxxxxx'
+
 session = requests.Session()
 session.headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
         }
-session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) 
+# session.cookies.set("__Secure-1PSID", token) 
 
-bard = Bard(session=session)
+bard = Bard(session=session, timeout=30)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 Simple Example
 <br>
 
 <a href="https://bard.google.com/"><img src="./assets/bardimg.png" height="600px">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.5 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.6 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Natural Language :: Korean Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
@@ -40,43 +40,47 @@
 dsdanielpark/Bard-API.git ```
 ## Authentication 1. Visit https://bard.google.com/ 2. F12 for console 3.
 Session: Application â Cookies â Copy the value of `__Secure-1PSID` cookie.
 
 ## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) Simple Usage ```python from
-bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard
-().get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
-ìë ¤ì¤")['content'] ``` Or you can use this ```python import bardapi import
-os # set your __Secure-1PSID value to key os.environ
-['_BARD_API_KEY']="xxxxxxxx" # set your input text input_text = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤" # Send an API
-request and get a response. response = bardapi.core.Bard().get_answer
-(input_text) ``` Addressing errors caused by delayed responses in environments
-like Google Colab and containers. If an error occurs despite following the
-proper procedure, utilize the timeout argument. ```python from bardapi import
-Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) #
-Set timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
-ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+bardapi import Bard token = 'xxxxxxxxxx' bard = Bard(token=token)
+bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤")['content'] ``` Or you can use this ```python from bardapi import
+Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard().get_answer("ëì
+ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content']
+``` To get reponse dictionary ```python import bardapi import os # set your
+__Secure-1PSID value to key token = 'xxxxxxxxxx' # set your input text
+input_text = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤" # Send an API request and get a response. response =
+bardapi.core.Bard(token).get_answer(input_text) ``` Addressing errors caused by
+delayed responses in environments like Google Colab and containers. If an error
+occurs despite following the proper procedure, utilize the timeout argument.
+```python from bardapi import Bard import os os.environ
+['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=30) # Set timeout in seconds
+bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤")['content'] ```
 ## Futher ### Behind a proxy If you are working behind a proxy, use the
 following. ```python from bardapi import Bard import os os.environ
 ['_BARD_API_KEY']="xxxxxxxx" # Change 'http://127.0.0.1:1080' to your http
 proxy # timeout in seconds bard = Bard(proxies={'http':'http://127.0.0.1:1080',
 'https':'http://127.0.0.1:1080'}, timeout=10) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
 ### Reusable session object ```python from bardapi import Bard import os import
-requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' session = requests.Session
-() session.headers = { "Host": "bard.google.com", "X-Same-Domain": "1", "User-
-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like
-Gecko) Chrome/91.0.4472.114 Safari/537.36", "Content-Type": "application/x-www-
-form-urlencoded;charset=UTF-8", "Origin": "https://bard.google.com", "Referer":
-"https://bard.google.com/", } session.cookies.set("__Secure-1PSID", os.environ
-["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
-Simple Example
+requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' # token='xxxxxxxxxxx'
+session = requests.Session() session.headers = { "Host": "bard.google.com", "X-
+Same-Domain": "1", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64)
+AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
+"Content-Type": "application/x-www-form-urlencoded;charset=UTF-8", "Origin":
+"https://bard.google.com", "Referer": "https://bard.google.com/", }
+session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) #
+session.cookies.set("__Secure-1PSID", token) bard = Bard(session=session,
+timeout=30) bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ``` Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
 [MIT](https://opensource.org/license/mit/)_
 I_hold_no_legal_responsibility;_for_more_information,_please_refer_to_the
 bottom_of_the_readme_file._I_just_want_you_to_give_me_and_[them](https://
```

### Comparing `bardapi-0.1.5/README.md` & `bardapi-0.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -52,83 +52,95 @@
 <br>
 
 ## Usage 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) 
 
 
 Simple Usage
+
 ```python
 from bardapi import Bard
-import os
 
+token = 'xxxxxxxxxx'
+bard = Bard(token=token)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+```
+Or you can use this
+```python
+from bardapi import Bard
+import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
+
 Bard().get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
-
-Or you can use this
+To get reponse dictionary
 ```python
 import bardapi
 import os
 
 # set your __Secure-1PSID value to key
-os.environ['_BARD_API_KEY']="xxxxxxxx"
+token = 'xxxxxxxxxx'
 
 # set your input text
 input_text = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 
 # Send an API request and get a response.
-response = bardapi.core.Bard().get_answer(input_text)
+response = bardapi.core.Bard(token).get_answer(input_text)
 ```
 
+
+
 Addressing errors caused by delayed responses in environments like Google Colab and containers. If an error occurs despite following the proper procedure, utilize the timeout argument.
 ```python
 from bardapi import Bard
 import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 
-bard = Bard(timeout=10) # Set timeout in seconds
+bard = Bard(timeout=30) # Set timeout in seconds
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 <br>
 
 ## Futher
 ### Behind a proxy
 If you are working behind a proxy, use the following.
 ```python
 from bardapi import Bard
 import os
-
 os.environ['_BARD_API_KEY']="xxxxxxxx"
+
 # Change 'http://127.0.0.1:1080' to your http proxy
 # timeout in seconds
 bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 ### Reusable session object
 ```python
 from bardapi import Bard
 import os
 import requests
-
 os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx'
+# token='xxxxxxxxxxx'
+
 session = requests.Session()
 session.headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
         }
-session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) 
+# session.cookies.set("__Secure-1PSID", token) 
 
-bard = Bard(session=session)
+bard = Bard(session=session, timeout=30)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 Simple Example
 <br>
 
 <a href="https://bard.google.com/"><img src="./assets/bardimg.png" height="600px">
```

#### html2text {}

```diff
@@ -26,43 +26,47 @@
 dsdanielpark/Bard-API.git ```
 ## Authentication 1. Visit https://bard.google.com/ 2. F12 for console 3.
 Session: Application â Cookies â Copy the value of `__Secure-1PSID` cookie.
 
 ## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) Simple Usage ```python from
-bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard
-().get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
-ìë ¤ì¤")['content'] ``` Or you can use this ```python import bardapi import
-os # set your __Secure-1PSID value to key os.environ
-['_BARD_API_KEY']="xxxxxxxx" # set your input text input_text = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤" # Send an API
-request and get a response. response = bardapi.core.Bard().get_answer
-(input_text) ``` Addressing errors caused by delayed responses in environments
-like Google Colab and containers. If an error occurs despite following the
-proper procedure, utilize the timeout argument. ```python from bardapi import
-Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) #
-Set timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
-ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+bardapi import Bard token = 'xxxxxxxxxx' bard = Bard(token=token)
+bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤")['content'] ``` Or you can use this ```python from bardapi import
+Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard().get_answer("ëì
+ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content']
+``` To get reponse dictionary ```python import bardapi import os # set your
+__Secure-1PSID value to key token = 'xxxxxxxxxx' # set your input text
+input_text = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤" # Send an API request and get a response. response =
+bardapi.core.Bard(token).get_answer(input_text) ``` Addressing errors caused by
+delayed responses in environments like Google Colab and containers. If an error
+occurs despite following the proper procedure, utilize the timeout argument.
+```python from bardapi import Bard import os os.environ
+['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=30) # Set timeout in seconds
+bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤")['content'] ```
 ## Futher ### Behind a proxy If you are working behind a proxy, use the
 following. ```python from bardapi import Bard import os os.environ
 ['_BARD_API_KEY']="xxxxxxxx" # Change 'http://127.0.0.1:1080' to your http
 proxy # timeout in seconds bard = Bard(proxies={'http':'http://127.0.0.1:1080',
 'https':'http://127.0.0.1:1080'}, timeout=10) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
 ### Reusable session object ```python from bardapi import Bard import os import
-requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' session = requests.Session
-() session.headers = { "Host": "bard.google.com", "X-Same-Domain": "1", "User-
-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like
-Gecko) Chrome/91.0.4472.114 Safari/537.36", "Content-Type": "application/x-www-
-form-urlencoded;charset=UTF-8", "Origin": "https://bard.google.com", "Referer":
-"https://bard.google.com/", } session.cookies.set("__Secure-1PSID", os.environ
-["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
-Simple Example
+requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' # token='xxxxxxxxxxx'
+session = requests.Session() session.headers = { "Host": "bard.google.com", "X-
+Same-Domain": "1", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64)
+AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
+"Content-Type": "application/x-www-form-urlencoded;charset=UTF-8", "Origin":
+"https://bard.google.com", "Referer": "https://bard.google.com/", }
+session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) #
+session.cookies.set("__Secure-1PSID", token) bard = Bard(session=session,
+timeout=30) bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ``` Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
 [MIT](https://opensource.org/license/mit/)_
 I_hold_no_legal_responsibility;_for_more_information,_please_refer_to_the
 bottom_of_the_readme_file._I_just_want_you_to_give_me_and_[them](https://
```

### Comparing `bardapi-0.1.5/bardapi/core.py` & `bardapi-0.1.6/bardapi/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,71 @@
-import json
+import os
 import random
-import re
 import string
-import os
 import requests
+import json
+import re
 
 
 class Bard:
-    def __init__(self, timeout=6, proxies=None, session=None):
+    def __init__(
+        self, token=os.getenv("_BARD_API_KEY"), timeout=10, proxies=None, session=None
+    ):
         """
         Initialize Bard
 
+        :param token: (`str`, *optional*)
+            Enter the __Secure-1PSID value. defaults to os.getenv("_BARD_API_KEY")
         :param timeout: (`int`, *optional*)
             Timeout in seconds when connecting bard server. The timeout is used on each request.
         :param proxies: (`Dict[str, str]`, *optional*)
             A dictionary of proxy servers to use by protocol or endpoint, e.g., `{'http': 'foo.bar:3128',
             'http://hostname': 'foo.bar:4012'}`. The proxies are used on each request.
         :param session: (`requests.Session`, *optional*)
             An existing requests.Session object to be used for making HTTP requests.
         """
-        self.proxies = proxies
-        self.timeout = timeout
         headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) "
             "Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
         }
+        self.token, self.proxies, self.timeout = token, proxies, timeout
         self._reqid = int("".join(random.choices(string.digits, k=4)))
-        self.conversation_id = ""
-        self.response_id = ""
-        self.choice_id = ""
-
-        if session is None:
-            self.session = requests.Session()
-            self.session.headers = headers
-            self.session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
-        else:
-            self.session = session
-
+        self.conversation_id = self.response_id = self.choice_id = ""
+        self.session = requests.Session() if session is None else session
+        self.session.headers = headers
+        self.session.cookies.set("__Secure-1PSID", self.token)
         self.SNlM0e = self._get_snim0e()
 
     def _get_snim0e(self):
+        if self.token and self.token[-1] != ".":
+            raise Exception(
+                "__Secure-1PSID value must end with a single dot. Enter correct __Secure-1PSID value."
+            )
+        elif not self.token:
+            raise Exception("No token value entered.")
         resp = self.session.get(
-            url="https://bard.google.com/", timeout=self.timeout, proxies=self.proxies
+            "https://bard.google.com/", timeout=self.timeout, proxies=self.proxies
         )
         if resp.status_code != 200:
-            raise Exception(f"Response Status: {resp.status_code}")
-        return re.search(r"SNlM0e\":\"(.*?)\"", resp.text).group(1)
+            raise Exception(
+                f"Response code not 200. \n - Try Bard on https://bard.google.com/ \n "
+                f"- Check service area on https://support.google.com/bard/answer/13575153?hl=en. \n "
+                f"- Response Status is {resp.status_code}"
+            )
+        snim0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text)
+        if not snim0e:
+            raise Exception(
+                "SNlM0e value not found in response. Check __Secure-1PSID value."
+            )
+        return snim0e.group(1)
 
     def get_answer(self, input_text: str) -> dict:
         params = {
             "bl": "boq_assistant-bard-web-server_20230419.00_p1",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
@@ -71,24 +82,28 @@
             "https://bard.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate",
             params=params,
             data=data,
             timeout=self.timeout,
             proxies=self.proxies,
         )
         resp_dict = json.loads(resp.content.splitlines()[3])[0][2]
-        if resp_dict is None:
+
+        if not resp_dict:
             return {"content": f"Response Error: {resp.content}."}
+
         parsed_answer = json.loads(resp_dict)
         bard_answer = {
             "content": parsed_answer[0][0],
             "conversation_id": parsed_answer[1][0],
             "response_id": parsed_answer[1][1],
             "factualityQueries": parsed_answer[3],
-            "textQuery": parsed_answer[2][0] if parsed_answer[2] is not None else "",
+            "textQuery": parsed_answer[2][0] if parsed_answer[2] else "",
             "choices": [{"id": i[0], "content": i[1]} for i in parsed_answer[4]],
         }
-        self.conversation_id = bard_answer["conversation_id"]
-        self.response_id = bard_answer["response_id"]
-        self.choice_id = bard_answer["choices"][0]["id"]
+        self.conversation_id, self.response_id, self.choice_id = (
+            bard_answer["conversation_id"],
+            bard_answer["response_id"],
+            bard_answer["choices"][0]["id"],
+        )
         self._reqid += 100000
 
         return bard_answer
```

### Comparing `bardapi-0.1.5/bardapi.egg-info/PKG-INFO` & `bardapi-0.1.6/bardapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bardapi
-Version: 0.1.5
+Version: 0.1.6
 Summary: The python package that returns Response of Google Bard through API.
 Home-page: https://github.com/dsdanielpark/Bard-API
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -77,83 +77,95 @@
 <br>
 
 ## Usage 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) 
 
 
 Simple Usage
+
 ```python
 from bardapi import Bard
-import os
 
+token = 'xxxxxxxxxx'
+bard = Bard(token=token)
+bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
+```
+Or you can use this
+```python
+from bardapi import Bard
+import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
+
 Bard().get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
-
-Or you can use this
+To get reponse dictionary
 ```python
 import bardapi
 import os
 
 # set your __Secure-1PSID value to key
-os.environ['_BARD_API_KEY']="xxxxxxxx"
+token = 'xxxxxxxxxx'
 
 # set your input text
 input_text = "나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘"
 
 # Send an API request and get a response.
-response = bardapi.core.Bard().get_answer(input_text)
+response = bardapi.core.Bard(token).get_answer(input_text)
 ```
 
+
+
 Addressing errors caused by delayed responses in environments like Google Colab and containers. If an error occurs despite following the proper procedure, utilize the timeout argument.
 ```python
 from bardapi import Bard
 import os
 os.environ['_BARD_API_KEY']="xxxxxxxx"
 
-bard = Bard(timeout=10) # Set timeout in seconds
+bard = Bard(timeout=30) # Set timeout in seconds
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 <br>
 
 ## Futher
 ### Behind a proxy
 If you are working behind a proxy, use the following.
 ```python
 from bardapi import Bard
 import os
-
 os.environ['_BARD_API_KEY']="xxxxxxxx"
+
 # Change 'http://127.0.0.1:1080' to your http proxy
 # timeout in seconds
 bard = Bard(proxies={'http':'http://127.0.0.1:1080', 'https':'http://127.0.0.1:1080'}, timeout=10)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 ### Reusable session object
 ```python
 from bardapi import Bard
 import os
 import requests
-
 os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx'
+# token='xxxxxxxxxxx'
+
 session = requests.Session()
 session.headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
         }
-session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
+session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) 
+# session.cookies.set("__Secure-1PSID", token) 
 
-bard = Bard(session=session)
+bard = Bard(session=session, timeout=30)
 bard.get_answer("나와 내 동년배들이 좋아하는 뉴진스에 대해서 알려줘")['content']
 ```
 
 Simple Example
 <br>
 
 <a href="https://bard.google.com/"><img src="./assets/bardimg.png" height="600px">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bardapi Version: 0.1.5 Summary: The python package
+Metadata-Version: 2.1 Name: bardapi Version: 0.1.6 Summary: The python package
 that returns Response of Google Bard through API. Home-page: https://
 github.com/dsdanielpark/Bard-API Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Python,API,Bard,Google Bard,Large Language
 Model,Chatbot API,Google API,Chatbot Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Natural Language :: Korean Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
@@ -40,43 +40,47 @@
 dsdanielpark/Bard-API.git ```
 ## Authentication 1. Visit https://bard.google.com/ 2. F12 for console 3.
 Session: Application â Cookies â Copy the value of `__Secure-1PSID` cookie.
 
 ## Usage [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/drive/
 1YIMA8aBmEQSSk90bB0Q9tznaLLQcluGA?usp=share_link) Simple Usage ```python from
-bardapi import Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard
-().get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
-ìë ¤ì¤")['content'] ``` Or you can use this ```python import bardapi import
-os # set your __Secure-1PSID value to key os.environ
-['_BARD_API_KEY']="xxxxxxxx" # set your input text input_text = "ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤" # Send an API
-request and get a response. response = bardapi.core.Bard().get_answer
-(input_text) ``` Addressing errors caused by delayed responses in environments
-like Google Colab and containers. If an error occurs despite following the
-proper procedure, utilize the timeout argument. ```python from bardapi import
-Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=10) #
-Set timeout in seconds bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
-ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
+bardapi import Bard token = 'xxxxxxxxxx' bard = Bard(token=token)
+bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤")['content'] ``` Or you can use this ```python from bardapi import
+Bard import os os.environ['_BARD_API_KEY']="xxxxxxxx" Bard().get_answer("ëì
+ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content']
+``` To get reponse dictionary ```python import bardapi import os # set your
+__Secure-1PSID value to key token = 'xxxxxxxxxx' # set your input text
+input_text = "ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤" # Send an API request and get a response. response =
+bardapi.core.Bard(token).get_answer(input_text) ``` Addressing errors caused by
+delayed responses in environments like Google Colab and containers. If an error
+occurs despite following the proper procedure, utilize the timeout argument.
+```python from bardapi import Bard import os os.environ
+['_BARD_API_KEY']="xxxxxxxx" bard = Bard(timeout=30) # Set timeout in seconds
+bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì
+ìë ¤ì¤")['content'] ```
 ## Futher ### Behind a proxy If you are working behind a proxy, use the
 following. ```python from bardapi import Bard import os os.environ
 ['_BARD_API_KEY']="xxxxxxxx" # Change 'http://127.0.0.1:1080' to your http
 proxy # timeout in seconds bard = Bard(proxies={'http':'http://127.0.0.1:1080',
 'https':'http://127.0.0.1:1080'}, timeout=10) bard.get_answer("ëì ë´
 ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
 ### Reusable session object ```python from bardapi import Bard import os import
-requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' session = requests.Session
-() session.headers = { "Host": "bard.google.com", "X-Same-Domain": "1", "User-
-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like
-Gecko) Chrome/91.0.4472.114 Safari/537.36", "Content-Type": "application/x-www-
-form-urlencoded;charset=UTF-8", "Origin": "https://bard.google.com", "Referer":
-"https://bard.google.com/", } session.cookies.set("__Secure-1PSID", os.environ
-["_BARD_API_KEY"]) bard = Bard(session=session) bard.get_answer("ëì ë´
-ëëë°°ë¤ì´ ì¢ìíë ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ```
-Simple Example
+requests os.environ['_BARD_API_KEY'] = 'xxxxxxxxxxx' # token='xxxxxxxxxxx'
+session = requests.Session() session.headers = { "Host": "bard.google.com", "X-
+Same-Domain": "1", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64)
+AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
+"Content-Type": "application/x-www-form-urlencoded;charset=UTF-8", "Origin":
+"https://bard.google.com", "Referer": "https://bard.google.com/", }
+session.cookies.set("__Secure-1PSID", os.getenv("_BARD_API_KEY")) #
+session.cookies.set("__Secure-1PSID", token) bard = Bard(session=session,
+timeout=30) bard.get_answer("ëì ë´ ëëë°°ë¤ì´ ì¢ìíë
+ë´ì§ì¤ì ëí´ì ìë ¤ì¤")['content'] ``` Simple Example
 [./assets/bardimg.png]_
 ##_Scripts_In_the_scripts_[folder](./scripts/),_I_have_released_a_script_to
 help_you_compare_[OpenAI-ChatGPT](./scripts/openai_api.ipynb)_and_[Google-Bard]
 (./scripts/google_api.ipynb)._I_hope_they_will_help_more_developers._##_License
 [MIT](https://opensource.org/license/mit/)_
 I_hold_no_legal_responsibility;_for_more_information,_please_refer_to_the
 bottom_of_the_readme_file._I_just_want_you_to_give_me_and_[them](https://
```

### Comparing `bardapi-0.1.5/setup.py` & `bardapi-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="bardapi",
-    version="0.1.5",
+    version="0.1.6",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="The python package that returns Response of Google Bard through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/Bard-API",
     packages=find_packages(exclude=[]),
```

