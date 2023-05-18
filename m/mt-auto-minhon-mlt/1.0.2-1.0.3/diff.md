# Comparing `tmp/mt-auto-minhon-mlt-1.0.2.tar.gz` & `tmp/mt-auto-minhon-mlt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mt-auto-minhon-mlt-1.0.2.tar", last modified: Sat May  6 03:30:19 2023, max compression
+gzip compressed data, was "mt-auto-minhon-mlt-1.0.3.tar", last modified: Thu May 18 15:52:05 2023, max compression
```

## Comparing `mt-auto-minhon-mlt-1.0.2.tar` & `mt-auto-minhon-mlt-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    53482 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/assets/support_translate.json
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/tranlator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 03:30:19.000000 mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:19.385880 mt-auto-minhon-mlt-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-06 03:30:07.000000 mt-auto-minhon-mlt-1.0.2/tests/test_tranlator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:52:05.719142 mt-auto-minhon-mlt-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-18 15:52:05.719142 mt-auto-minhon-mlt-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-18 15:51:53.000000 mt-auto-minhon-mlt-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-18 15:51:53.000000 mt-auto-minhon-mlt-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:52:05.719142 mt-auto-minhon-mlt-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:52:05.715141 mt-auto-minhon-mlt-1.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:51:53.000000 mt-auto-minhon-mlt-1.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:52:05.719142 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 15:51:53.000000 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:52:05.719142 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    53482 2023-05-18 15:51:53.000000 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt/assets/support_translate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-18 15:51:53.000000 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt/tranlator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:52:05.719142 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-18 15:52:05.000000 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-18 15:52:05.000000 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:52:05.000000 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 15:52:05.000000 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:52:05.000000 mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:52:05.719142 mt-auto-minhon-mlt-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-18 15:51:53.000000 mt-auto-minhon-mlt-1.0.3/tests/test_tranlator.py
```

### Comparing `mt-auto-minhon-mlt-1.0.2/PKG-INFO` & `mt-auto-minhon-mlt-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mt-auto-minhon-mlt
-Version: 1.0.2
+Version: 1.0.3
 Summary: みんなの自動翻訳 Python Library
 Project-URL: Homepage, https://github.com/MIDORIBIN/mt-auto-minhon-mlt
 Project-URL: Bug Tracker, https://github.com/MIDORIBIN/mt-auto-minhon-mlt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-![](docs/assets/header.png)
+![](https://raw.githubusercontent.com/MIDORIBIN/mt-auto-minhon-mlt/main/docs/assets/header.png)
 
 # みんなの自動翻訳 Python Library
 
 [![Python application](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml/badge.svg)](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/mt-auto-minhon-mlt.svg)](https://badge.fury.io/py/mt-auto-minhon-mlt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mt-auto-minhon-mlt)](https://pypi.org/project/mt-auto-minhon-mlt/)
```

### Comparing `mt-auto-minhon-mlt-1.0.2/README.md` & `mt-auto-minhon-mlt-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![](docs/assets/header.png)
+![](https://raw.githubusercontent.com/MIDORIBIN/mt-auto-minhon-mlt/main/docs/assets/header.png)
 
 # みんなの自動翻訳 Python Library
 
 [![Python application](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml/badge.svg)](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/mt-auto-minhon-mlt.svg)](https://badge.fury.io/py/mt-auto-minhon-mlt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mt-auto-minhon-mlt)](https://pypi.org/project/mt-auto-minhon-mlt/)
```

### Comparing `mt-auto-minhon-mlt-1.0.2/pyproject.toml` & `mt-auto-minhon-mlt-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mt-auto-minhon-mlt"
-version = "1.0.2"
+version = "1.0.3"
 readme = "README.md"
 description = "みんなの自動翻訳 Python Library"
 requires-python = ">=3.7, <3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/assets/support_translate.json` & `mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt/assets/support_translate.json`

 * *Files identical despite different names*

### Comparing `mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt/tranlator.py` & `mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt/tranlator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,126 @@
 from __future__ import annotations
 
 import json
-import urllib
+from enum import Enum
 from pathlib import Path
 from urllib.parse import urlencode
-from urllib.request import Request
+from urllib.request import Request, urlopen
+
+
+class TranslateType(str, Enum):
+    FSA_NT = "fsaNT"
+    SHORT_SNT = "shortSnt"
+    VOICETRA_NT = "voicetraNT"
+    PAT_ETC = "patETC"
+    LAWS_NT = "lawsNT"
+    GENERAL_PT = "generalPT"
+    PATENT_NT = "patentNT"
+    SCIENCE = "science"
+    FSA_GO_JP = "fsaGoJP"
+    MINNA_PE = "minnaPE"
+    GENERAL_NT = "generalNT"
 
 
 def load_support_translate() -> list[tuple[str, str, str]]:
     path = Path(__file__).parent / "assets/support_translate.json"
     with open(path, encoding="utf-8") as f:
         support_languages = json.load(f)
     return [tuple(support_language) for support_language in support_languages]
 
 
-def request(url: str, data: dict[str, str], timeout=10) -> dict:
+def send_request(url: str, data: dict[str, str], timeout=10) -> dict:
     request_object = Request(url, urlencode(data).encode("ascii"), method="POST")
 
-    with urllib.request.urlopen(request_object, timeout=timeout) as response:
+    with urlopen(request_object, timeout=timeout) as response:
         response_body = response.read().decode("utf-8")
-        return json.loads(response_body)
+    return json.loads(response_body)
 
 
 class Translator:
     __DOMAIN = "https://mt-auto-minhon-mlt.ucri.jgn-x.jp"
     __SUPPORT_TRANSLATE = load_support_translate()
 
-    def __init__(self, client_id: str, client_secret: str, user_name: str):
+    def __init__(self, client_id: str, client_secret: str, user_name: str) -> None:
         self.__client_id = client_id
         self.__user_name = user_name
-        self.__access_token = self.__get_access_token(
-            client_id=client_id,
-            client_secret=client_secret,
-        )
+        self.__access_token = self.__get_access_token(client_id, client_secret)
+
+    @classmethod
+    def __get_access_token(cls, client_id: str, client_secret: str) -> str:
+        url = f"{cls.__DOMAIN}/oauth2/token.php"
+        request_data = {
+            "grant_type": "client_credentials",
+            "client_id": client_id,
+            "client_secret": client_secret,
+        }
+        response_data = send_request(url, request_data)
+        return response_data["access_token"]
 
     def translate_text(
         self,
         text: str,
         source_lang: str,
         target_lang: str,
-        translate_type: str = "generalNT",
+        translate_type: TranslateType = TranslateType.GENERAL_NT,
         split: int = None,
         history: int = None,
         xml: int = None,
         term_id: str | list[str] | int = None,
         bilingual_id: str | list[str] | int = None,
         log_use: int = None,
         data: str | int = None,
     ) -> str:
         """
         Translate text.
 
-        :param text: text to translate.
-        :param source_lang: source language.
-        :param target_lang: target language.
-        :param translate_type: translate type.
-        :param split: split text.
-        :param history: history.
-        :param xml: xml.
-        :param term_id: term id.
-        :param bilingual_id: bilingual id.
-        :param log_use: log use.
-        :param data: data.
+        :param: text: text to translate.
+        :param: source_lang: source language.
+        :param: target_lang: target language.
+        :param: translate_type: translate type.
+        :param: split: split text.
+        :param: history: history.
+        :param: xml: xml.
+        :param: term_id: term id.
+        :param: bilingual_id: bilingual id.
+        :param: log_use: log use.
+        :param: data: data.
 
         :return: translated text.
         """
         self.__check(text, translate_type, source_lang, target_lang)
 
-        url = f"{self.__DOMAIN}/api/mt/{translate_type}_{source_lang}_{target_lang}/"
-        request_data = dict(
-            access_token=self.__access_token,
-            key=self.__client_id,
-            name=self.__user_name,
-            type="json",
-            text=text,
-            split=split,
-            history=history,
-            xml=xml,
-            term_id=term_id,
-            bilingual_id=bilingual_id,
-            log_use=log_use,
-            data=data,
-        )
-        request_data = {k: v for k, v in request_data.items() if v is not None}
-
-        response = request(url, data=request_data)
-        if response["resultset"]["code"] != 0:
-            raise ValueError(f"code: {response['resultset']['code']}, message: \"{response['resultset']['message']}\"")
-        return response["resultset"]["result"]["text"]
+        url = f"{self.__DOMAIN}/api/mt/{translate_type.value}_{source_lang}_{target_lang}/"
+        request_data = {
+            "access_token": self.__access_token,
+            "key": self.__client_id,
+            "name": self.__user_name,
+            "type": "json",
+            "text": text,
+            "split": split,
+            "history": history,
+            "xml": xml,
+            "term_id": term_id,
+            "bilingual_id": bilingual_id,
+            "log_use": log_use,
+            "data": data,
+        }
+        response_data = send_request(url, request_data)
+
+        if response_data["resultset"]["code"] != 0:
+            raise ValueError(
+                f"code: {response_data['resultset']['code']}, message: \"{response_data['resultset']['message']}\""
+            )
+        return response_data["resultset"]["result"]["text"]
 
-    def __check(self, text: str, translate_type: str, source_lang: str, target_lang: str):
+    def __check(self, text: str, translate_type: TranslateType, source_lang: str, target_lang: str) -> None:
         if not self.__is_support_translate(translate_type, source_lang, target_lang):
             raise ValueError(
-                f"doesn't support. translate_type: {translate_type}, source_lang: {source_lang}"
-                f", target_lang: {target_lang}"
+                f"doesn't support. translate_type: {translate_type}, source_lang: {source_lang}, "
+                "target_lang: {target_lang}"
             )
-        if text is None or text == "":
+        if not text:
             raise ValueError("doesn't exist text")
 
     @classmethod
-    def __is_support_translate(cls, translate_type: str, src_lang: str, target_lang: str):
-        return (translate_type, src_lang, target_lang) in cls.__SUPPORT_TRANSLATE
-
-    @classmethod
-    def __get_access_token(cls, client_id: str, client_secret: str) -> str:
-        url = f"{cls.__DOMAIN}/oauth2/token.php"
-        client_data = {
-            "grant_type": "client_credentials",
-            "client_id": client_id,
-            "client_secret": client_secret,
-        }
-        response = request(url, data=client_data)
-        return response["access_token"]
+    def __is_support_translate(cls, translate_type: TranslateType, src_lang: str, target_lang: str) -> bool:
+        return (translate_type.value, src_lang, target_lang) in cls.__SUPPORT_TRANSLATE
```

### Comparing `mt-auto-minhon-mlt-1.0.2/src/mt_auto_minhon_mlt.egg-info/PKG-INFO` & `mt-auto-minhon-mlt-1.0.3/src/mt_auto_minhon_mlt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mt-auto-minhon-mlt
-Version: 1.0.2
+Version: 1.0.3
 Summary: みんなの自動翻訳 Python Library
 Project-URL: Homepage, https://github.com/MIDORIBIN/mt-auto-minhon-mlt
 Project-URL: Bug Tracker, https://github.com/MIDORIBIN/mt-auto-minhon-mlt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-![](docs/assets/header.png)
+![](https://raw.githubusercontent.com/MIDORIBIN/mt-auto-minhon-mlt/main/docs/assets/header.png)
 
 # みんなの自動翻訳 Python Library
 
 [![Python application](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml/badge.svg)](https://github.com/MIDORIBIN/mt-auto-minhon-mlt/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/mt-auto-minhon-mlt.svg)](https://badge.fury.io/py/mt-auto-minhon-mlt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mt-auto-minhon-mlt)](https://pypi.org/project/mt-auto-minhon-mlt/)
```

### Comparing `mt-auto-minhon-mlt-1.0.2/tests/test_tranlator.py` & `mt-auto-minhon-mlt-1.0.3/tests/test_tranlator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from unittest import TestCase
 
 from src.mt_auto_minhon_mlt import Translator
+from src.mt_auto_minhon_mlt.tranlator import TranslateType
 
 
 class TestTranslator(TestCase):
     @classmethod
     def setUpClass(cls):
         cls.translator = Translator(
             client_id=os.environ["CLIENT_ID"],
@@ -23,15 +24,18 @@
         jp_expected = "みんなの自動翻訳"
         jp_actual = self.translator.translate_text(en_text, source_lang="en", target_lang="ja")
         self.assertEqual(jp_expected, jp_actual)
 
         jp_text = "みんなの自動翻訳"
         en_expected = "Minna no Jido Hon'"
         en_actual = self.translator.translate_text(
-            jp_text, translate_type="voicetraNT", source_lang="ja", target_lang="en"
+            jp_text,
+            translate_type=TranslateType.GENERAL_NT,
+            source_lang="ja",
+            target_lang="en",
         )
         self.assertEqual(en_expected, en_actual)
 
     def test_translate_text_error(self):
         translator = Translator(
             client_id=os.environ["CLIENT_ID"],
             client_secret=os.environ["CLIENT_SECRET"],
```

