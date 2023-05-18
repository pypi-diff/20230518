# Comparing `tmp/imap_structure-0.1.3.tar.gz` & `tmp/imap_structure-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap_structure-0.1.3.tar", max compression
+gzip compressed data, was "imap_structure-0.1.4.tar", max compression
```

## Comparing `imap_structure-0.1.3.tar` & `imap_structure-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       44 2023-05-18 03:04:19.021602 imap_structure-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-18 03:04:19.021602 imap_structure-0.1.3/imap_structure/__init__.py
--rw-r--r--   0        0        0    10793 2023-05-18 04:21:04.349483 imap_structure-0.1.3/imap_structure/body_structure.py
--rw-r--r--   0        0        0     4816 2023-05-18 03:04:19.021602 imap_structure-0.1.3/imap_structure/metadata.py
--rw-r--r--   0        0        0     1467 2023-05-18 03:04:19.021602 imap_structure-0.1.3/imap_structure/parser.py
--rw-r--r--   0        0        0      540 2023-05-18 04:21:04.349483 imap_structure-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.3/setup.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-05-18 03:04:19.021602 imap_structure-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 03:04:19.021602 imap_structure-0.1.4/imap_structure/__init__.py
+-rw-r--r--   0        0        0    10793 2023-05-18 04:21:04.349483 imap_structure-0.1.4/imap_structure/body_structure.py
+-rw-r--r--   0        0        0     5032 2023-05-18 05:31:45.507524 imap_structure-0.1.4/imap_structure/metadata.py
+-rw-r--r--   0        0        0     1467 2023-05-18 03:04:19.021602 imap_structure-0.1.4/imap_structure/parser.py
+-rw-r--r--   0        0        0      540 2023-05-18 05:32:14.067512 imap_structure-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.4/setup.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.4/PKG-INFO
```

### Comparing `imap_structure-0.1.3/imap_structure/body_structure.py` & `imap_structure-0.1.4/imap_structure/body_structure.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.3/imap_structure/metadata.py` & `imap_structure-0.1.4/imap_structure/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import collections.abc
 import imaplib
+import logging
 import re
 from dataclasses import dataclass
 from email.message import Message
 from typing import Optional, Sequence
 
 from imap_structure.body_structure import BodyStructure, parse_body_structure
 from imap_structure.parser import guess_encoding, parse_bytes
 
+logger = logging.getLogger(__name__)
+
+
 METADATA_MESSAGE_PARTS = (
     "(" + " ".join(["UID", "FLAGS", "BODYSTRUCTURE", "BODY[HEADER]"]) + ")"
 )
 
 
 @dataclass
 class Metadata:
@@ -31,15 +35,17 @@
         assert not isinstance(
             message_set, str
         )  # We don't want to get a string like "(1,2,3)"
         message_set_inner = ",".join(str(x) for x in message_set)
         message_set = f"({message_set_inner})"
 
     result, response = mail.fetch(message_set, METADATA_MESSAGE_PARTS)
-    assert result == "OK"
+    if result != "OK":
+        logger.error(response)
+        raise mail.error("Failed to fetch metadata")
     assert isinstance(response, list)
     return response
 
 
 def fetch_raw_metadatas_uid(
     mail: imaplib.IMAP4, uid_set: str | int | Sequence[int] | Sequence[str]
 ) -> list:
@@ -51,15 +57,17 @@
         assert not isinstance(
             uid_set, str
         )  # We don't want to get a string like "(1,2,3)"
         message_set_inner = ",".join(str(x) for x in uid_set)
         uid_set = f"({message_set_inner})"
 
     result, response = mail.uid("fetch", uid_set, METADATA_MESSAGE_PARTS)
-    assert result == "OK"
+    if result != "OK":
+        logger.error(response)
+        raise mail.error("Failed to fetch metadata")
     assert isinstance(response, list)
     return response
 
 
 def split_raw_metadatas(metadatas: list[tuple]) -> dict[int, list[bytes]]:
     result: dict[int, list[bytes]] = {}
     sequence: Optional[int] = None
```

### Comparing `imap_structure-0.1.3/imap_structure/parser.py` & `imap_structure-0.1.4/imap_structure/parser.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.3/pyproject.toml` & `imap_structure-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imap-structure"
-version = "0.1.3"
+version = "0.1.4"
 description = "IMAP BODYSTRUCTURE parser"
 authors = ["Kiruya Momochi <65301509+kiruyamomochi@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "imap_structure" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `imap_structure-0.1.3/setup.py` & `imap_structure-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyparsing>=3.0.9,<4.0.0']
 
 setup_kwargs = {
     'name': 'imap-structure',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'IMAP BODYSTRUCTURE parser',
     'long_description': '# imap-structure\n\nIMAP BODYSTRUCTURE parser\n',
     'author': 'Kiruya Momochi',
     'author_email': '65301509+kiruyamomochi@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

