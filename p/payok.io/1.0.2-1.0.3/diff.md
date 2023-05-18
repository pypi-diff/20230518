# Comparing `tmp/payok.io-1.0.2.tar.gz` & `tmp/payok.io-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payok.io-1.0.2.tar", last modified: Wed May 17 15:10:43 2023, max compression
+gzip compressed data, was "payok.io-1.0.3.tar", last modified: Thu May 18 16:53:54 2023, max compression
```

## Comparing `payok.io-1.0.2.tar` & `payok.io-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.908498 payok.io-1.0.2/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1063 2023-05-17 13:59:37.000000 payok.io-1.0.2/LICENSE
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-05-17 15:10:43.908498 payok.io-1.0.2/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1518 2023-05-17 15:09:15.000000 payok.io-1.0.2/README.md
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.904498 payok.io-1.0.2/payok/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      494 2023-05-17 14:50:33.000000 payok.io-1.0.2/payok/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     7300 2023-05-17 15:01:27.000000 payok.io-1.0.2/payok/api.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.904498 payok.io-1.0.2/payok/enums/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      362 2023-05-17 13:37:52.000000 payok.io-1.0.2/payok/enums/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      162 2023-05-17 14:34:42.000000 payok.io-1.0.2/payok/enums/base.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      114 2023-05-17 14:34:58.000000 payok.io-1.0.2/payok/enums/comission_type.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      138 2023-05-17 14:35:37.000000 payok.io-1.0.2/payok/enums/currency.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       99 2023-05-17 14:38:46.000000 payok.io-1.0.2/payok/enums/pay_status.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      293 2023-05-17 14:35:18.000000 payok.io-1.0.2/payok/enums/payment_method.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      455 2023-05-17 14:35:26.000000 payok.io-1.0.2/payok/enums/payout_method.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      103 2023-05-17 14:20:25.000000 payok.io-1.0.2/payok/enums/webhook_status.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      272 2023-05-17 14:06:53.000000 payok.io-1.0.2/payok/exceptions.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.908498 payok.io-1.0.2/payok/models/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      208 2023-05-17 14:49:34.000000 payok.io-1.0.2/payok/models/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      139 2023-05-16 21:14:21.000000 payok.io-1.0.2/payok/models/balance.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      196 2023-05-17 14:49:19.000000 payok.io-1.0.2/payok/models/new_payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      898 2023-05-17 14:55:52.000000 payok.io-1.0.2/payok/models/payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      967 2023-05-17 14:25:29.000000 payok.io-1.0.2/payok/models/transaction.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-17 15:10:43.904498 payok.io-1.0.2/payok.io.egg-info/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      576 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/SOURCES.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/dependency_links.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       17 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/requires.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        6 2023-05-17 15:10:43.000000 payok.io-1.0.2/payok.io.egg-info/top_level.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-05-17 15:10:43.908498 payok.io-1.0.2/setup.cfg
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1269 2023-05-17 15:10:05.000000 payok.io-1.0.2/setup.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-18 16:53:54.317048 payok.io-1.0.3/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1063 2023-05-17 13:59:37.000000 payok.io-1.0.3/LICENSE
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-05-18 16:53:54.317048 payok.io-1.0.3/PKG-INFO
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1518 2023-05-17 15:09:15.000000 payok.io-1.0.3/README.md
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-18 16:53:54.317048 payok.io-1.0.3/payok/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      494 2023-05-17 14:50:33.000000 payok.io-1.0.3/payok/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     7300 2023-05-17 15:01:27.000000 payok.io-1.0.3/payok/api.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-18 16:53:54.317048 payok.io-1.0.3/payok/enums/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      362 2023-05-17 13:37:52.000000 payok.io-1.0.3/payok/enums/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      162 2023-05-17 14:34:42.000000 payok.io-1.0.3/payok/enums/base.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      114 2023-05-17 14:34:58.000000 payok.io-1.0.3/payok/enums/comission_type.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      138 2023-05-17 14:35:37.000000 payok.io-1.0.3/payok/enums/currency.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       99 2023-05-17 14:38:46.000000 payok.io-1.0.3/payok/enums/pay_status.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      293 2023-05-17 14:35:18.000000 payok.io-1.0.3/payok/enums/payment_method.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      455 2023-05-17 14:35:26.000000 payok.io-1.0.3/payok/enums/payout_method.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      103 2023-05-17 14:20:25.000000 payok.io-1.0.3/payok/enums/webhook_status.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      272 2023-05-17 14:06:53.000000 payok.io-1.0.3/payok/exceptions.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-18 16:53:54.317048 payok.io-1.0.3/payok/models/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      208 2023-05-17 14:49:34.000000 payok.io-1.0.3/payok/models/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      139 2023-05-16 21:14:21.000000 payok.io-1.0.3/payok/models/balance.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      196 2023-05-17 14:49:19.000000 payok.io-1.0.3/payok/models/new_payout.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      898 2023-05-17 14:55:52.000000 payok.io-1.0.3/payok/models/payout.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1000 2023-05-18 16:53:23.000000 payok.io-1.0.3/payok/models/transaction.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-18 16:53:54.317048 payok.io-1.0.3/payok.io.egg-info/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-05-18 16:53:54.000000 payok.io-1.0.3/payok.io.egg-info/PKG-INFO
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      576 2023-05-18 16:53:54.000000 payok.io-1.0.3/payok.io.egg-info/SOURCES.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-05-18 16:53:54.000000 payok.io-1.0.3/payok.io.egg-info/dependency_links.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       17 2023-05-18 16:53:54.000000 payok.io-1.0.3/payok.io.egg-info/requires.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)        6 2023-05-18 16:53:54.000000 payok.io-1.0.3/payok.io.egg-info/top_level.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-05-18 16:53:54.317048 payok.io-1.0.3/setup.cfg
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1269 2023-05-18 16:53:32.000000 payok.io-1.0.3/setup.py
```

### Comparing `payok.io-1.0.2/LICENSE` & `payok.io-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.2/PKG-INFO` & `payok.io-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok.io
-Version: 1.0.2
+Version: 1.0.3
 Summary: Asynchronous PayOK API wrapper
 Home-page: https://github.com/nikitalm8/payok
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/payok
 Project-URL: Bug Tracker, https://github.com/nikitalm8/payok/issues
 Project-URL: API Docs, https://payok.io/cabinet/documentation/doc_api_main
```

### Comparing `payok.io-1.0.2/README.md` & `payok.io-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.2/payok/api.py` & `payok.io-1.0.3/payok/api.py`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.2/payok/models/payout.py` & `payok.io-1.0.3/payok/models/payout.py`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.2/payok/models/transaction.py` & `payok.io-1.0.3/payok/models/transaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ..enums import (
     Currency,
     PayStatus, 
     WebhookStatus, 
 )
 
+from typing import Optional
 from datetime import datetime
 
 from pydantic import BaseModel, validator
 from pydantic.fields import Field
 
 
 class Transaction(BaseModel):
@@ -25,15 +26,15 @@
     comission_percent: float
     comission_fixed: float
     method: str
     transaction: int
     date: datetime
     pay_date: datetime = None
     status: PayStatus = Field(PayStatus.waiting, alias='transaction_status')
-    custom_fields: dict = {}
+    custom_fields: Optional[dict]
     webhook_status: WebhookStatus
     webhook_amount: int
 
     @property
     def is_paid(self) -> bool:
 
         return bool(self.status)
```

### Comparing `payok.io-1.0.2/payok.io.egg-info/PKG-INFO` & `payok.io-1.0.3/payok.io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok.io
-Version: 1.0.2
+Version: 1.0.3
 Summary: Asynchronous PayOK API wrapper
 Home-page: https://github.com/nikitalm8/payok
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/payok
 Project-URL: Bug Tracker, https://github.com/nikitalm8/payok/issues
 Project-URL: API Docs, https://payok.io/cabinet/documentation/doc_api_main
```

### Comparing `payok.io-1.0.2/payok.io.egg-info/SOURCES.txt` & `payok.io-1.0.3/payok.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.2/setup.py` & `payok.io-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as file:
 
     long_description = "\n" + file.read()
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'Asynchronous PayOK API wrapper'
 
 setup(
     name="payok.io",
     version=VERSION,
     author="Nikita Minaev",
     author_email="<nikita@minaev.su>",
```

