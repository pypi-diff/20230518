# Comparing `tmp/paykassa-api-sdk-1.0.1.tar.gz` & `tmp/paykassa-api-sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paykassa-api-sdk-1.0.1.tar", last modified: Tue May  3 09:33:49 2022, max compression
+gzip compressed data, was "paykassa-api-sdk-1.1.0.tar", last modified: Thu May 18 17:55:04 2023, max compression
```

## Comparing `paykassa-api-sdk-1.0.1.tar` & `paykassa-api-sdk-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 selyakovadim   (501) staff       (20)        0 2022-05-03 09:33:49.277267 paykassa-api-sdk-1.0.1/
--rw-r--r--   0 selyakovadim   (501) staff       (20)     1064 2022-05-02 06:41:45.000000 paykassa-api-sdk-1.0.1/LICENSE
--rw-r--r--   0 selyakovadim   (501) staff       (20)     3905 2022-05-03 09:33:49.277334 paykassa-api-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 selyakovadim   (501) staff       (20)     3034 2022-05-03 09:01:04.000000 paykassa-api-sdk-1.0.1/README.md
--rw-r--r--   0 selyakovadim   (501) staff       (20)       84 2022-05-02 06:54:50.000000 paykassa-api-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 selyakovadim   (501) staff       (20)      920 2022-05-03 09:33:49.277603 paykassa-api-sdk-1.0.1/setup.cfg
-drwxr-xr-x   0 selyakovadim   (501) staff       (20)        0 2022-05-03 09:33:49.275026 paykassa-api-sdk-1.0.1/src/
-drwxr-xr-x   0 selyakovadim   (501) staff       (20)        0 2022-05-03 09:33:49.276597 paykassa-api-sdk-1.0.1/src/paykassa/
--rw-r--r--   0 selyakovadim   (501) staff       (20)        0 2022-05-02 06:52:37.000000 paykassa-api-sdk-1.0.1/src/paykassa/__init__.py
--rw-r--r--   0 selyakovadim   (501) staff       (20)    11976 2022-05-02 06:41:50.000000 paykassa-api-sdk-1.0.1/src/paykassa/dto.py
--rw-r--r--   0 selyakovadim   (501) staff       (20)     3065 2022-05-02 06:41:50.000000 paykassa-api-sdk-1.0.1/src/paykassa/merchant.py
--rw-r--r--   0 selyakovadim   (501) staff       (20)     2181 2022-05-02 06:41:50.000000 paykassa-api-sdk-1.0.1/src/paykassa/payment.py
--rw-r--r--   0 selyakovadim   (501) staff       (20)      861 2022-05-02 06:41:50.000000 paykassa-api-sdk-1.0.1/src/paykassa/struct.py
-drwxr-xr-x   0 selyakovadim   (501) staff       (20)        0 2022-05-03 09:33:49.277174 paykassa-api-sdk-1.0.1/src/paykassa_api_sdk.egg-info/
--rw-r--r--   0 selyakovadim   (501) staff       (20)     3905 2022-05-03 09:33:49.000000 paykassa-api-sdk-1.0.1/src/paykassa_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 selyakovadim   (501) staff       (20)      378 2022-05-03 09:33:49.000000 paykassa-api-sdk-1.0.1/src/paykassa_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 selyakovadim   (501) staff       (20)        1 2022-05-03 09:33:49.000000 paykassa-api-sdk-1.0.1/src/paykassa_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 selyakovadim   (501) staff       (20)       17 2022-05-03 09:33:49.000000 paykassa-api-sdk-1.0.1/src/paykassa_api_sdk.egg-info/requires.txt
--rw-r--r--   0 selyakovadim   (501) staff       (20)        9 2022-05-03 09:33:49.000000 paykassa-api-sdk-1.0.1/src/paykassa_api_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-05-18 17:55:04.782478 paykassa-api-sdk-1.1.0/
+-rw-r--r--   0 macbookair   (501) staff       (20)     1064 2023-05-12 16:24:48.000000 paykassa-api-sdk-1.1.0/LICENSE
+-rw-r--r--   0 macbookair   (501) staff       (20)     3879 2023-05-18 17:55:04.782553 paykassa-api-sdk-1.1.0/PKG-INFO
+-rw-r--r--   0 macbookair   (501) staff       (20)     3045 2023-05-18 17:28:28.000000 paykassa-api-sdk-1.1.0/README.md
+-rw-r--r--   0 macbookair   (501) staff       (20)       84 2023-05-12 16:24:48.000000 paykassa-api-sdk-1.1.0/pyproject.toml
+-rw-r--r--   0 macbookair   (501) staff       (20)      920 2023-05-18 17:55:04.782838 paykassa-api-sdk-1.1.0/setup.cfg
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-05-18 17:55:04.778588 paykassa-api-sdk-1.1.0/src/
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-05-18 17:55:04.780405 paykassa-api-sdk-1.1.0/src/paykassa/
+-rw-r--r--   0 macbookair   (501) staff       (20)        0 2023-05-12 16:24:48.000000 paykassa-api-sdk-1.1.0/src/paykassa/__init__.py
+-rw-r--r--   0 macbookair   (501) staff       (20)    11994 2023-05-18 17:34:51.000000 paykassa-api-sdk-1.1.0/src/paykassa/dto.py
+-rw-r--r--   0 macbookair   (501) staff       (20)     3065 2023-05-18 17:24:54.000000 paykassa-api-sdk-1.1.0/src/paykassa/merchant.py
+-rw-r--r--   0 macbookair   (501) staff       (20)     2181 2023-05-18 16:12:16.000000 paykassa-api-sdk-1.1.0/src/paykassa/payment.py
+-rw-r--r--   0 macbookair   (501) staff       (20)      899 2023-05-18 17:12:53.000000 paykassa-api-sdk-1.1.0/src/paykassa/struct.py
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-05-18 17:55:04.781395 paykassa-api-sdk-1.1.0/src/paykassa_api_sdk.egg-info/
+-rw-r--r--   0 macbookair   (501) staff       (20)     3879 2023-05-18 17:55:04.000000 paykassa-api-sdk-1.1.0/src/paykassa_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 macbookair   (501) staff       (20)      441 2023-05-18 17:55:04.000000 paykassa-api-sdk-1.1.0/src/paykassa_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)        1 2023-05-18 17:55:04.000000 paykassa-api-sdk-1.1.0/src/paykassa_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)       17 2023-05-18 17:55:04.000000 paykassa-api-sdk-1.1.0/src/paykassa_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 macbookair   (501) staff       (20)        9 2023-05-18 17:55:04.000000 paykassa-api-sdk-1.1.0/src/paykassa_api_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 macbookair   (501) staff       (20)        0 2023-05-18 17:55:04.782214 paykassa-api-sdk-1.1.0/tests/
+-rw-r--r--   0 macbookair   (501) staff       (20)     3705 2023-05-18 17:21:45.000000 paykassa-api-sdk-1.1.0/tests/test_dto.py
+-rw-r--r--   0 macbookair   (501) staff       (20)     7702 2023-05-18 17:31:15.000000 paykassa-api-sdk-1.1.0/tests/test_merchant.py
+-rw-r--r--   0 macbookair   (501) staff       (20)     3102 2023-05-18 17:23:01.000000 paykassa-api-sdk-1.1.0/tests/test_payment.py
```

### Comparing `paykassa-api-sdk-1.0.1/LICENSE` & `paykassa-api-sdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paykassa-api-sdk-1.0.1/PKG-INFO` & `paykassa-api-sdk-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: paykassa-api-sdk
-Version: 1.0.1
+Version: 1.1.0
 Summary: Paykassa API & SCI
 Home-page: https://paykassa.pro
 Author: Vadim Selyakov
 Author-email: selyakovadim@gmail.com
-License: UNKNOWN
 Project-URL: Source, https://github.com/paykassa-dev/python-api-sdk
 Project-URL: Documentation, https://paykassa.pro/en/developers/
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -43,15 +41,15 @@
 ### Check Balance
 
 ```python
 from paykassa.dto import CheckBalanceRequest
 from paykassa.struct import System, Currency
 
 request = CheckBalanceRequest() \
-    .set_shop("123")
+    .set_shop_id("123")
 
 response = client.check_balance(request)
 
 if not response.has_error():
     print(response.get_balance(System.BITCOIN, Currency.BTC))
     print(response.get_balance(System.ETHEREUM, Currency.ETH))
 ```
@@ -59,16 +57,16 @@
 ### Make Payment
 
 ```python
 from paykassa.dto import MakePaymentRequest
 from paykassa.struct import System, Currency, CommissionPayer, TransactionPriority 
 
 request = MakePaymentRequest() \
-    .set_shop("123") \
-    .set_amount(1.02) \
+    .set_shop_id("123") \
+    .set_amount("1.02") \
     .set_priority(TransactionPriority.MEDIUM) \
     .set_system(System.BITCOIN) \
     .set_currency(Currency.BTC) \
     .set_paid_commission(CommissionPayer.SHOP) \
     .set_number("3J98t1WpEZ73CNmQviecrnyiWrnqRhWNLy")
  
 response = client.make_payment(request)
@@ -120,15 +118,15 @@
 ### Generate Address
 
 ```python
 from paykassa.dto import GenerateAddressRequest
 from paykassa.struct import System, Currency, CommissionPayer
 
 request = GenerateAddressRequest() \
-    .set_amount(1.123456) \
+    .set_amount("1.123456") \
     .set_currency(Currency.DOGE) \
     .set_system(System.DOGECOIN) \
     .set_comment("test") \
     .set_paid_commission(CommissionPayer.CLIENT)
 
 response = client.generate_address(request)
 
@@ -140,25 +138,23 @@
 ### Get Payment Url
 
 ```python
 from paykassa.dto import GetPaymentUrlRequest
 from paykassa.struct import System, Currency, CommissionPayer
 
 request = GetPaymentUrlRequest() \
-    .set_amount(110) \
-    .set_currency(Currency.USD) \
-    .set_system(System.PERFECTMONEY) \
+    .set_amount("110") \
+    .set_currency(Currency.USDT) \
+    .set_system(System.TRON_TRC20) \
     .set_comment("test") \
     .set_paid_commission(CommissionPayer.CLIENT)
 
 response = client.get_payment_url(request)
 
 if not response.has_error():
     print(response.get_method())
     print(response.get_url())
 ```
 
 ## References
 - [Devs Documentation](https://paykassa.pro/en/developers)
 - [API Documentation](https://paykassa.pro/docs/)
-
-
```

### Comparing `paykassa-api-sdk-1.0.1/README.md` & `paykassa-api-sdk-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ### Check Balance
 
 ```python
 from paykassa.dto import CheckBalanceRequest
 from paykassa.struct import System, Currency
 
 request = CheckBalanceRequest() \
-    .set_shop("123")
+    .set_shop_id("123")
 
 response = client.check_balance(request)
 
 if not response.has_error():
     print(response.get_balance(System.BITCOIN, Currency.BTC))
     print(response.get_balance(System.ETHEREUM, Currency.ETH))
 ```
@@ -35,16 +35,16 @@
 ### Make Payment
 
 ```python
 from paykassa.dto import MakePaymentRequest
 from paykassa.struct import System, Currency, CommissionPayer, TransactionPriority 
 
 request = MakePaymentRequest() \
-    .set_shop("123") \
-    .set_amount(1.02) \
+    .set_shop_id("123") \
+    .set_amount("1.02") \
     .set_priority(TransactionPriority.MEDIUM) \
     .set_system(System.BITCOIN) \
     .set_currency(Currency.BTC) \
     .set_paid_commission(CommissionPayer.SHOP) \
     .set_number("3J98t1WpEZ73CNmQviecrnyiWrnqRhWNLy")
  
 response = client.make_payment(request)
@@ -96,15 +96,15 @@
 ### Generate Address
 
 ```python
 from paykassa.dto import GenerateAddressRequest
 from paykassa.struct import System, Currency, CommissionPayer
 
 request = GenerateAddressRequest() \
-    .set_amount(1.123456) \
+    .set_amount("1.123456") \
     .set_currency(Currency.DOGE) \
     .set_system(System.DOGECOIN) \
     .set_comment("test") \
     .set_paid_commission(CommissionPayer.CLIENT)
 
 response = client.generate_address(request)
 
@@ -116,17 +116,17 @@
 ### Get Payment Url
 
 ```python
 from paykassa.dto import GetPaymentUrlRequest
 from paykassa.struct import System, Currency, CommissionPayer
 
 request = GetPaymentUrlRequest() \
-    .set_amount(110) \
-    .set_currency(Currency.USD) \
-    .set_system(System.PERFECTMONEY) \
+    .set_amount("110") \
+    .set_currency(Currency.USDT) \
+    .set_system(System.TRON_TRC20) \
     .set_comment("test") \
     .set_paid_commission(CommissionPayer.CLIENT)
 
 response = client.get_payment_url(request)
 
 if not response.has_error():
     print(response.get_method())
```

### Comparing `paykassa-api-sdk-1.0.1/setup.cfg` & `paykassa-api-sdk-1.1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = paykassa-api-sdk
-version = 1.0.1
+version = 1.1.0
 author = Vadim Selyakov
 author_email = selyakovadim@gmail.com
 description = Paykassa API & SCI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://paykassa.pro
 project_urls =
```

### Comparing `paykassa-api-sdk-1.0.1/src/paykassa/dto.py` & `paykassa-api-sdk-1.1.0/src/paykassa/dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 class Request(object):
     def normalize(self) -> dict:
         pass
 
 
 class Response:
     _response_systems = {
-        "PerfectMoney": System.PERFECTMONEY,
         "Berty": System.BERTY,
         "BitCoin": System.BITCOIN,
         "Ethereum": System.ETHEREUM,
         "Litecoin": System.BITCOIN,
         "Dogecoin": System.DOGECOIN,
         "Dash": System.DASH,
         "BitcoinCash": System.BITCOINCASH,
         "Zcash": System.ZCASH,
         "Ripple": System.RIPPLE,
         "TRON": System.TRON,
         "Stellar": System.STELLAR,
         "BinanceCoin": System.BINANCECOIN,
         "TRON_TRC20": System.TRON_TRC20,
         "BinanceSmartChain_BEP20": System.BINANCESMARTCHAIN_BEP20,
-        "Ethereum_ERC20": System.ETHEREUM_ERC20
+        "Ethereum_ERC20": System.ETHEREUM_ERC20,
+        "EthereumClassic": System.ETHEREUMCLASSIC,
     }
 
     def __init__(self, data: dict):
         self._error = data["error"]
         self._message = data["message"]
         self._data = data["data"]
 
@@ -42,55 +42,55 @@
             raise KeyError("Unknown system: " + name)
 
         return self._response_systems[name]
 
 
 class CheckBalanceRequest(Request):
     def __init__(self):
-        self.__shop = ""
+        self.__shop_id = ""
 
-    def set_shop(self, shop: str):
-        self.__shop = shop
+    def set_shop_id(self, shop_id: str):
+        self.__shop_id = shop_id
         return self
 
     def normalize(self) -> dict:
         return {
-            "shop": self.__shop
+            "shop_id": self.__shop_id
         }
 
 
 class CheckBalanceResponse(Response):
-    def get_balance(self, system: System, currency: Currency) -> float:
+    def get_balance(self, system: System, currency: Currency) -> str:
         if self.__get_system_currency_pair(currency, system) not in self._data:
             raise KeyError("Can't get a balance by system %s and currency %s" % (system.name, currency.name))
 
-        return float(self._data[self.__get_system_currency_pair(currency, system)])
+        return str(self._data[self.__get_system_currency_pair(currency, system)])
 
     @staticmethod
     def __get_system_currency_pair(currency, system):
         return system.name.lower() + '_' + currency.name.lower()
 
 
 class MakePaymentRequest(Request):
     def __init__(self):
         self.__test = False
         self.__priority = TransactionPriority.MEDIUM
-        self.__tag = 0
+        self.__tag = "0"
         self.__number = ""
         self.__paid_commission = CommissionPayer.SHOP
         self.__system = System.BITCOIN
         self.__currency = Currency.BTC
-        self.__shop = ""
-        self.__amount = 0.0
+        self.__shop_id = ""
+        self.__amount = "0.0"
 
-    def set_shop(self, shop: str):
-        self.__shop = shop
+    def set_shop_id(self, shop_id: str):
+        self.__shop_id = shop_id
         return self
 
-    def set_amount(self, amount: float):
+    def set_amount(self, amount: str):
         self.__amount = amount
         return self
 
     def set_currency(self, currency: Currency):
         self.__currency = currency
         return self
 
@@ -102,15 +102,15 @@
         self.__paid_commission = paid_commission
         return self
 
     def set_number(self, number: str):
         self.__number = number
         return self
 
-    def set_tag(self, tag: int):
+    def set_tag(self, tag: str):
         self.__tag = tag
         return self
 
     def set_priority(self, priority: TransactionPriority):
         self.__priority = priority
         return self
 
@@ -122,15 +122,15 @@
         return {
             "priority": self.__priority.value,
             "tag": self.__tag,
             "number": self.__number,
             "paid_commission": self.__paid_commission.value,
             "system": self.__system.value,
             "currency": self.__currency.value,
-            "shop": self.__shop,
+            "shop_id": self.__shop_id,
             "amount": self.__amount,
             "test": self.__test,
         }
 
 
 class MakePaymentResponse(Response):
     def get_shop_id(self) -> str:
@@ -138,34 +138,34 @@
 
     def get_transaction(self) -> str:
         return str(self._data["transaction"])
 
     def get_txid(self) -> str:
         return str(self._data["txid"])
 
-    def get_amount(self) -> float:
-        return float(self._data["amount"])
+    def get_amount(self) -> str:
+        return str(self._data["amount"])
 
-    def get_amount_pay(self) -> float:
-        return float(self._data["amount_pay"])
+    def get_amount_pay(self) -> str:
+        return str(self._data["amount_pay"])
 
     def get_system(self) -> System:
         return self._get_system(self._data["system"])
 
     def get_currency(self) -> Currency:
         return Currency(str(self._data["currency"]))
 
     def get_number(self) -> str:
         return str(self._data["number"])
 
-    def get_shop_commission_percent(self) -> float:
-        return float(self._data["shop_comission_percent"])
+    def get_shop_commission_percent(self) -> str:
+        return str(self._data["shop_commission_percent"])
 
-    def get_shop_commission_amount(self) -> float:
-        return float(self._data["shop_comission_amount"])
+    def get_shop_commission_amount(self) -> str:
+        return str(self._data["shop_commission_amount"])
 
     def get_paid_commission(self) -> str:
         return str(self._data["paid_commission"])
 
 
 class CheckPaymentRequest(Request):
     def __init__(self):
@@ -185,24 +185,24 @@
             "private_hash": self.__private_hash,
             "test": self.__test,
         }
 
 
 class CheckPaymentResponse(Response):
     def get_transaction(self) -> int:
-        return int(self._data["transaction"])
+        return str(self._data["transaction"])
 
-    def get_shop_id(self) -> int:
-        return int(self._data["shop_id"])
+    def get_shop_id(self) -> str:
+        return str(self._data["shop_id"])
 
     def get_order_id(self) -> str:
         return str(self._data["order_id"])
 
-    def get_amount(self) -> float:
-        return float(self._data["amount"])
+    def get_amount(self) -> str:
+        return str(self._data["amount"])
 
     def get_currency(self) -> Currency:
         return Currency(self._data["currency"])
 
     def get_system(self) -> System:
         return self._get_system(self._data["system"])
 
@@ -236,31 +236,31 @@
         return {
             "private_hash": self.__private_hash,
             "test": self.__test,
         }
 
 
 class CheckTransactionResponse(Response):
-    def get_transaction(self) -> int:
-        return int(self._data["transaction"])
+    def get_transaction(self) -> str:
+        return str(self._data["transaction"])
 
     def get_txid(self) -> str:
         return str(self._data["txid"])
 
-    def get_shop_id(self) -> int:
-        return int(self._data["shop_id"])
+    def get_shop_id(self) -> str:
+        return str(self._data["shop_id"])
 
     def get_order_id(self) -> str:
         return str(self._data["order_id"])
 
-    def get_amount(self) -> float:
-        return float(self._data["amount"])
+    def get_amount(self) -> str:
+        return str(self._data["amount"])
 
-    def get_fee(self) -> float:
-        return float(self._data["fee"])
+    def get_fee(self) -> str:
+        return str(self._data["fee"])
 
     def get_currency(self) -> Currency:
         return Currency(self._data["currency"])
 
     def get_system(self) -> System:
         return self._get_system(self._data["system"])
 
@@ -302,15 +302,15 @@
         self.__comment = ""
         self.__paid_commission = CommissionPayer.SHOP
 
     def set_order_id(self, order_id: str):
         self.__order_id = order_id
         return self
 
-    def set_amount(self, amount: float):
+    def set_amount(self, amount: str):
         self.__amount = amount
         return self
 
     def set_currency(self, currency: Currency):
         self.__currency = currency
         return self
 
@@ -340,28 +340,28 @@
             "paid_commission": self.__paid_commission.value,
             "phone": False,
             "test": self.__test,
         }
 
 
 class GenerateAddressResponse(Response):
-    def get_invoice(self) -> int:
-        return int(self._data["invoice"])
+    def get_invoice_id(self) -> int:
+        return str(self._data["invoice_id"])
 
     def get_status(self) -> str:
         return str(self._data["status"])
 
     def get_order_id(self) -> str:
         return str(self._data["order_id"])
 
     def get_wallet(self) -> str:
         return str(self._data["wallet"])
 
-    def get_amount(self) -> float:
-        return float(self._data["amount"])
+    def get_amount(self) -> str:
+        return str(self._data["amount"])
 
     def get_system(self) -> System:
         return self._get_system(self._data["system"])
 
     def get_currency(self) -> Currency:
         return Currency(self._data["currency"])
 
@@ -373,24 +373,24 @@
 
 
 class GetPaymentUrlRequest(Request):
     def __init__(self):
         self.__test = False
         self.__order_id = ""
         self.__amount = 0.0
-        self.__currency = Currency.USD
-        self.__system = System.PERFECTMONEY
+        self.__currency = Currency.USDT
+        self.__system = System.TRON_TRC20
         self.__comment = ""
         self.__paid_commission = CommissionPayer.SHOP
 
     def set_order_id(self, order_id: str):
         self.__order_id = order_id
         return self
 
-    def set_amount(self, amount: float):
+    def set_amount(self, amount: str):
         self.__amount = amount
         return self
 
     def set_currency(self, currency: Currency):
         self.__currency = currency
         return self
```

### Comparing `paykassa-api-sdk-1.0.1/src/paykassa/merchant.py` & `paykassa-api-sdk-1.1.0/src/paykassa/merchant.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         pass
 
 
 class MerchantApiBase(MerchantApiInterface):
     BASE_URL = "https://paykassa.app/sci/"
     API_VERSION = 0.4
 
-    def __init__(self, api_id: int, api_key: str):
+    def __init__(self, api_id: str, api_key: str):
         self._sci_id = api_id
         self._sci_key = api_key
 
     def set_sci_id(self, api_id: str):
         self._sci_id = api_id
         return self
 
@@ -55,15 +55,15 @@
             "error": True,
             "message": str(e),
             "data": {},
         }
 
 
 class MerchantApi(MerchantApiBase):
-    def __init__(self, sci_id: int, sci_key: str):
+    def __init__(self, sci_id: str, sci_key: str):
         super(MerchantApi, self).__init__(sci_id, sci_key)
 
     # see https://paykassa.pro/docs/#api-SCI-sci_confirm_order
     def check_payment(self, request: CheckPaymentRequest) -> CheckPaymentResponse:
         return CheckPaymentResponse(self._make_request("sci_confirm_order", request.normalize()))
 
     # see https://paykassa.pro/docs/#api-SCI-sci_confirm_transaction_notification
```

### Comparing `paykassa-api-sdk-1.0.1/src/paykassa/payment.py` & `paykassa-api-sdk-1.1.0/src/paykassa/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     def make_payment(self, request: MakePaymentRequest) -> MakePaymentResponse:
         pass
 
 
 class PaymentApiBase(PaymentApiInterface):
     BASE_URL = "https://paykassa.app/api/"
-    API_VERSION = 0.5
+    API_VERSION = 0.9
 
     def __init__(self, api_id: int, api_key: str):
         self._api_id = api_id
         self._api_key = api_key
 
     def set_api_id(self, api_id: str) -> 'PaymentApiBase':
         self._api_id = api_id
```

### Comparing `paykassa-api-sdk-1.0.1/src/paykassa_api_sdk.egg-info/PKG-INFO` & `paykassa-api-sdk-1.1.0/src/paykassa_api_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: paykassa-api-sdk
-Version: 1.0.1
+Version: 1.1.0
 Summary: Paykassa API & SCI
 Home-page: https://paykassa.pro
 Author: Vadim Selyakov
 Author-email: selyakovadim@gmail.com
-License: UNKNOWN
 Project-URL: Source, https://github.com/paykassa-dev/python-api-sdk
 Project-URL: Documentation, https://paykassa.pro/en/developers/
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -43,15 +41,15 @@
 ### Check Balance
 
 ```python
 from paykassa.dto import CheckBalanceRequest
 from paykassa.struct import System, Currency
 
 request = CheckBalanceRequest() \
-    .set_shop("123")
+    .set_shop_id("123")
 
 response = client.check_balance(request)
 
 if not response.has_error():
     print(response.get_balance(System.BITCOIN, Currency.BTC))
     print(response.get_balance(System.ETHEREUM, Currency.ETH))
 ```
@@ -59,16 +57,16 @@
 ### Make Payment
 
 ```python
 from paykassa.dto import MakePaymentRequest
 from paykassa.struct import System, Currency, CommissionPayer, TransactionPriority 
 
 request = MakePaymentRequest() \
-    .set_shop("123") \
-    .set_amount(1.02) \
+    .set_shop_id("123") \
+    .set_amount("1.02") \
     .set_priority(TransactionPriority.MEDIUM) \
     .set_system(System.BITCOIN) \
     .set_currency(Currency.BTC) \
     .set_paid_commission(CommissionPayer.SHOP) \
     .set_number("3J98t1WpEZ73CNmQviecrnyiWrnqRhWNLy")
  
 response = client.make_payment(request)
@@ -120,15 +118,15 @@
 ### Generate Address
 
 ```python
 from paykassa.dto import GenerateAddressRequest
 from paykassa.struct import System, Currency, CommissionPayer
 
 request = GenerateAddressRequest() \
-    .set_amount(1.123456) \
+    .set_amount("1.123456") \
     .set_currency(Currency.DOGE) \
     .set_system(System.DOGECOIN) \
     .set_comment("test") \
     .set_paid_commission(CommissionPayer.CLIENT)
 
 response = client.generate_address(request)
 
@@ -140,25 +138,23 @@
 ### Get Payment Url
 
 ```python
 from paykassa.dto import GetPaymentUrlRequest
 from paykassa.struct import System, Currency, CommissionPayer
 
 request = GetPaymentUrlRequest() \
-    .set_amount(110) \
-    .set_currency(Currency.USD) \
-    .set_system(System.PERFECTMONEY) \
+    .set_amount("110") \
+    .set_currency(Currency.USDT) \
+    .set_system(System.TRON_TRC20) \
     .set_comment("test") \
     .set_paid_commission(CommissionPayer.CLIENT)
 
 response = client.get_payment_url(request)
 
 if not response.has_error():
     print(response.get_method())
     print(response.get_url())
 ```
 
 ## References
 - [Devs Documentation](https://paykassa.pro/en/developers)
 - [API Documentation](https://paykassa.pro/docs/)
-
-
```

