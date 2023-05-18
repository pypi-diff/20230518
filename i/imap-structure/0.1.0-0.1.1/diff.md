# Comparing `tmp/imap_structure-0.1.0.tar.gz` & `tmp/imap_structure-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap_structure-0.1.0.tar", max compression
+gzip compressed data, was "imap_structure-0.1.1.tar", max compression
```

## Comparing `imap_structure-0.1.0.tar` & `imap_structure-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       44 2023-05-18 02:15:45.592944 imap_structure-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-18 02:11:07.503068 imap_structure-0.1.0/imap_structure/__init__.py
--rw-r--r--   0        0        0    10088 2023-05-18 02:13:15.533013 imap_structure-0.1.0/imap_structure/body_structure.py
--rw-r--r--   0        0        0     4828 2023-05-18 02:13:15.553013 imap_structure-0.1.0/imap_structure/metadata.py
--rw-r--r--   0        0        0     1467 2023-05-18 02:13:15.573013 imap_structure-0.1.0/imap_structure/parser.py
--rw-r--r--   0        0        0      540 2023-05-18 02:33:43.092447 imap_structure-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.0/setup.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-05-18 02:15:45.592944 imap_structure-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 02:11:07.503068 imap_structure-0.1.1/imap_structure/__init__.py
+-rw-r--r--   0        0        0    10088 2023-05-18 02:13:15.533013 imap_structure-0.1.1/imap_structure/body_structure.py
+-rw-r--r--   0        0        0     4816 2023-05-18 02:50:48.401972 imap_structure-0.1.1/imap_structure/metadata.py
+-rw-r--r--   0        0        0     1467 2023-05-18 02:13:15.573013 imap_structure-0.1.1/imap_structure/parser.py
+-rw-r--r--   0        0        0      540 2023-05-18 02:51:21.481960 imap_structure-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 imap_structure-0.1.1/setup.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 imap_structure-0.1.1/PKG-INFO
```

### Comparing `imap_structure-0.1.0/imap_structure/body_structure.py` & `imap_structure-0.1.1/imap_structure/body_structure.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.0/imap_structure/metadata.py` & `imap_structure-0.1.1/imap_structure/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import collections.abc
 import imaplib
 import re
 from dataclasses import dataclass
 from email.message import Message
 from typing import Optional, Sequence
 
-from mail2mattermost.mail.body_structure import BodyStructure, parse_body_structure
-from mail2mattermost.mail.parser import guess_encoding, parse_bytes
+from imap_structure.body_structure import BodyStructure, parse_body_structure
+from imap_structure.parser import guess_encoding, parse_bytes
 
 METADATA_MESSAGE_PARTS = (
     "(" + " ".join(["UID", "FLAGS", "BODYSTRUCTURE", "BODY[HEADER]"]) + ")"
 )
 
 
 @dataclass
```

### Comparing `imap_structure-0.1.0/imap_structure/parser.py` & `imap_structure-0.1.1/imap_structure/parser.py`

 * *Files identical despite different names*

### Comparing `imap_structure-0.1.0/pyproject.toml` & `imap_structure-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imap-structure"
-version = "0.1.0"
+version = "0.1.1"
 description = "IMAP BODYSTRUCTURE parser"
 authors = ["Kiruya Momochi <65301509+kiruyamomochi@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "imap_structure" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `imap_structure-0.1.0/setup.py` & `imap_structure-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyparsing>=3.0.9,<4.0.0']
 
 setup_kwargs = {
     'name': 'imap-structure',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'IMAP BODYSTRUCTURE parser',
     'long_description': '# imap-structure\n\nIMAP BODYSTRUCTURE parser\n',
     'author': 'Kiruya Momochi',
     'author_email': '65301509+kiruyamomochi@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

