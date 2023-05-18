# Comparing `tmp/pyntelope-0.8.3.tar.gz` & `tmp/pyntelope-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntelope-0.8.3.tar", max compression
+gzip compressed data, was "pyntelope-0.8.4.tar", max compression
```

## Comparing `pyntelope-0.8.3.tar` & `pyntelope-0.8.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-01-09 20:18:32.312701 pyntelope-0.8.3/LICENSE
--rw-r--r--   0        0        0     4618 2023-01-09 20:18:32.328702 pyntelope-0.8.3/README.md
--rw-r--r--   0        0        0      133 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/__init__.py
--rw-r--r--   0        0        0      115 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/_version.py
--rw-r--r--   0        0        0      484 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/exc.py
--rw-r--r--   0        0        0     9922 2023-03-10 00:37:34.108012 pyntelope-0.8.3/pyntelope/net.py
--rw-r--r--   0        0        0    10203 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/transaction.py
--rw-r--r--   0        0        0      933 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/types/__init__.py
--rw-r--r--   0        0        0      875 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/types/base.py
--rw-r--r--   0        0        0    11680 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/types/compostes.py
--rw-r--r--   0        0        0    17252 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/types/primitives.py
--rw-r--r--   0        0        0     8413 2023-01-09 20:18:32.316702 pyntelope-0.8.3/pyntelope/utils.py
--rw-r--r--   0        0        0      934 2023-03-10 00:41:47.659089 pyntelope-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     5287 1970-01-01 00:00:00.000000 pyntelope-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-09 20:18:32.312701 pyntelope-0.8.4/LICENSE
+-rw-r--r--   0        0        0     4618 2023-01-09 20:18:32.328702 pyntelope-0.8.4/README.md
+-rw-r--r--   0        0        0      133 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/__init__.py
+-rw-r--r--   0        0        0      115 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/_version.py
+-rw-r--r--   0        0        0      484 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/exc.py
+-rw-r--r--   0        0        0    10454 2023-05-18 16:33:44.672961 pyntelope-0.8.4/pyntelope/net.py
+-rw-r--r--   0        0        0    10203 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/transaction.py
+-rw-r--r--   0        0        0      933 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/types/__init__.py
+-rw-r--r--   0        0        0      875 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/types/base.py
+-rw-r--r--   0        0        0    11680 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/types/compostes.py
+-rw-r--r--   0        0        0    17252 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/types/primitives.py
+-rw-r--r--   0        0        0     8414 2023-03-27 18:18:22.970029 pyntelope-0.8.4/pyntelope/utils.py
+-rw-r--r--   0        0        0      934 2023-05-18 16:57:38.810179 pyntelope-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     5287 1970-01-01 00:00:00.000000 pyntelope-0.8.4/PKG-INFO
```

### Comparing `pyntelope-0.8.3/LICENSE` & `pyntelope-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.3/README.md` & `pyntelope-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.3/pyntelope/net.py` & `pyntelope-0.8.4/pyntelope/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,52 +200,69 @@
         scope: str,
         json: bool = True,
         index_position: str = None,
         key_type: str = None,
         encode_type: str = None,
         lower_bound: str = None,
         upper_bound: str = None,
-        limit: int = None,
+        limit: int = 1000,
         reverse: int = None,
         show_payer: int = None,
+        full: bool = False,
     ):
         """
         Return a list with the rows in the table.
 
         Similar to get_table_rows
         https://developers.eos.io/manuals/eos/latest/nodeos/plugins/chain_api_plugin/api-reference/index#operation/get_table_rows
 
         Parameters:
         -----------
         json: bool = True
             Get the response as json
+        full: bool = True
+            Get the full table.
+            Requires multiple requests to be made.
+            The maximum number of requests made is 1000.
         """
         endpoint = "/v1/chain/get_table_rows"
+
         payload = dict(
             code=code,
             table=table,
             scope=scope,
             json=json,
             index_position=index_position,
             key_type=key_type,
             encode_type=encode_type,
             lower_bound=lower_bound,
             upper_bound=upper_bound,
             limit=limit,
             reverse=reverse,
             show_payer=show_payer,
         )
-        for k in list(payload.keys()):
-            if payload[k] is None:
-                del payload[k]
-        data = self._request(endpoint=endpoint, payload=payload)
-        if "rows" in data:
-            return data["rows"]
+        payload = {k: v for k, v in payload.items() if v is not None}
+
+        rows = []
+        for _ in range(1000):
+            logger.debug(f"Get data with {lower_bound=}")
+            data = self._request(endpoint=endpoint, payload=payload)
+            if "rows" not in data:
+                return data
+            rows += data["rows"]
+
+            if not full or not data.get("more"):
+                break
+
+            next_key = data["next_key"]
+            payload["lower_bound"] = next_key
         else:
-            return data
+            raise ValueError("Too many requests (>1000) for table")
+
+        return rows
 
     def push_transaction(
         self,
         *,
         transaction: object,
         compression: bool = False,
         packed_context_free_data: str = "",
```

### Comparing `pyntelope-0.8.3/pyntelope/transaction.py` & `pyntelope-0.8.4/pyntelope/transaction.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.3/pyntelope/types/__init__.py` & `pyntelope-0.8.4/pyntelope/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.3/pyntelope/types/base.py` & `pyntelope-0.8.4/pyntelope/types/base.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.3/pyntelope/types/compostes.py` & `pyntelope-0.8.4/pyntelope/types/compostes.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.3/pyntelope/types/primitives.py` & `pyntelope-0.8.4/pyntelope/types/primitives.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.3/pyntelope/utils.py` & `pyntelope-0.8.4/pyntelope/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 def _deterministic_generate_k_nonce(message_hash, key, nonce):
     v = b"\x01" * 32
     k = b"\x00" * 32
     try:
         key_encoded = _encode_privkey(key, "bin")
     except AssertionError:
-        raise ValueError("Error in private key provided: {key=}")
+        raise ValueError(f"Error in private key provided: {key=}")
 
     msg_int = _decode(message_hash, 256)
     message_hash = _encode(msg_int + nonce, 256, 32)
 
     k = _sha256_hmac_digest(k, v + b"\x00" + key_encoded + message_hash)
     v = _sha256_hmac_digest(k, v)
     k = _sha256_hmac_digest(k, v + b"\x01" + key_encoded + message_hash)
```

### Comparing `pyntelope-0.8.3/pyproject.toml` & `pyntelope-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyntelope"
-version = "0.8.3"
+version = "0.8.4"
 description = "Interact with Antelope blockchains"
 authors = ["Team <pyntelope@facings.io>"]
 homepage = "https://github.com/FACINGS/pyntelope"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pyntelope-0.8.3/PKG-INFO` & `pyntelope-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntelope
-Version: 0.8.3
+Version: 0.8.4
 Summary: Interact with Antelope blockchains
 Home-page: https://github.com/FACINGS/pyntelope
 Author: Team
 Author-email: pyntelope@facings.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

