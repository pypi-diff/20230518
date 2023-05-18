# Comparing `tmp/algokit_utils-1.1.2b2-py3-none-any.whl.zip` & `tmp/algokit_utils-1.2.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 33779 bytes, number of entries: 15
+Zip file size: 33938 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     3697 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    32559 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
--rw-r--r--  2.0 unx     4309 b- defN 80-Jan-01 00:00 algokit_utils/models.py
+-rw-r--r--  2.0 unx     4883 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.1.2b2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.1.2b2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.1.2b2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.1.2b2.dist-info/RECORD
-15 files, 128566 bytes uncompressed, 31687 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b1.dist-info/RECORD
+15 files, 129140 bytes uncompressed, 31846 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.1.2b2.dist-info/LICENSE
+Filename: algokit_utils-1.2.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.1.2b2.dist-info/METADATA
+Filename: algokit_utils-1.2.0b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.1.2b2.dist-info/WHEEL
+Filename: algokit_utils-1.2.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.1.2b2.dist-info/RECORD
+Filename: algokit_utils-1.2.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/models.py

```diff
@@ -1,22 +1,37 @@
 import dataclasses
 from collections.abc import Sequence
 from typing import Any, Protocol, TypeAlias, TypedDict
 
 from algosdk import transaction
 from algosdk.abi import Method
-from algosdk.atomic_transaction_composer import AtomicTransactionResponse, TransactionSigner
+from algosdk.atomic_transaction_composer import AccountTransactionSigner, AtomicTransactionResponse, TransactionSigner
+from algosdk.encoding import decode_address
 
 
 @dataclasses.dataclass(kw_only=True)
 class Account:
     """Holds the private_key and address for an account"""
 
     private_key: str
+    """Base64 encoded private key"""
     address: str
+    """Address for this account"""
+
+    @property
+    def public_key(self) -> bytes:
+        """The public key for this account"""
+        public_key = decode_address(self.address)  # type: ignore[no-untyped-call]
+        assert isinstance(public_key, bytes)
+        return public_key
+
+    @property
+    def signer(self) -> AccountTransactionSigner:
+        """An AccountTransactionSigner for this account"""
+        return AccountTransactionSigner(self.private_key)
 
 
 @dataclasses.dataclass(kw_only=True)
 class TransactionResponse:
     """Response for a non ABI call"""
 
     tx_id: str
```

## Comparing `algokit_utils-1.1.2b2.dist-info/LICENSE` & `algokit_utils-1.2.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.1.2b2.dist-info/METADATA` & `algokit_utils-1.2.0b1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.1.2b2
+Version: 1.2.0b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.1.2b2.dist-info/RECORD` & `algokit_utils-1.2.0b1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=3oON9YJ-fU3rFhxacSPNxrpmnHUgG349oMH_Id9NdIA,53906
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=qJDgrHpoZMZA0upQ8QnriO62b5OnRkJHBULpRdQ4khc,32559
 algokit_utils/logic_error.py,sha256=ypu2DSyus-Kjy51_1oE8T3LHVhRSOrc21Gpbau_WjAc,1981
-algokit_utils/models.py,sha256=_0vVN1qW1VxyqjkhuxLpxcrOfVtw2LtCcOeQXJSv-4A,4309
+algokit_utils/models.py,sha256=qd2hy1ZIijD2yVs_1Zj_c8NZCk42FbEF5D6-m-eIB0g,4883
 algokit_utils/network_clients.py,sha256=0cbUHCEWycFnduEu5cJ4dY6pfDOOzvHO1cXmcxAe83M,4841
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.1.2b2.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.1.2b2.dist-info/METADATA,sha256=Nz1nyai_X7pX0zWOASr873PRk9fblmMg6_4qjfaMyPM,2037
-algokit_utils-1.1.2b2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.1.2b2.dist-info/RECORD,,
+algokit_utils-1.2.0b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.2.0b1.dist-info/METADATA,sha256=EvMKL1LdA028HF_bbC8EtAJXqNxW8N8eIoNqQegFSCs,2037
+algokit_utils-1.2.0b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.2.0b1.dist-info/RECORD,,
```

