# Comparing `tmp/casbin_async_sqlalchemy_adapter-1.0.0.tar.gz` & `tmp/casbin_async_sqlalchemy_adapter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.0.0.tar", last modified: Thu May 18 13:50:17 2023, max compression
+gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.0.1.tar", last modified: Thu May 18 14:04:37 2023, max compression
```

## Comparing `casbin_async_sqlalchemy_adapter-1.0.0.tar` & `casbin_async_sqlalchemy_adapter-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:50:17.504403 casbin_async_sqlalchemy_adapter-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 13:49:41.000000 casbin_async_sqlalchemy_adapter-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-18 13:50:17.504403 casbin_async_sqlalchemy_adapter-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-18 13:49:41.000000 casbin_async_sqlalchemy_adapter-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:50:17.500403 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 13:49:41.000000 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-05-18 13:49:41.000000 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:50:17.504403 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-18 13:50:17.000000 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-18 13:50:17.000000 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:50:17.000000 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 13:50:17.000000 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 13:50:17.000000 casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 13:50:17.504403 casbin_async_sqlalchemy_adapter-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-18 13:49:41.000000 casbin_async_sqlalchemy_adapter-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:50:17.504403 casbin_async_sqlalchemy_adapter-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-05-18 13:49:41.000000 casbin_async_sqlalchemy_adapter-1.0.0/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 14:04:37.000000 casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:04:37.958326 casbin_async_sqlalchemy_adapter-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-05-18 14:04:12.000000 casbin_async_sqlalchemy_adapter-1.0.1/tests/test_adapter.py
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.0/LICENSE` & `casbin_async_sqlalchemy_adapter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.0.0/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_async_sqlalchemy_adapter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.0/README.md` & `casbin_async_sqlalchemy_adapter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter/adapter.py` & `casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter/adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,34 @@
+# Copyright 2023 The casbin Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from contextlib import asynccontextmanager
 
 from casbin import persist
 from sqlalchemy import Column, Integer, String
 from sqlalchemy import create_engine, or_
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.future import select
 from sqlalchemy.orm import sessionmaker
 
 Base = declarative_base()
 
+
 class CasbinRule(Base):
     __tablename__ = "casbin_rule"
 
     id = Column(Integer, primary_key=True)
     ptype = Column(String(255))
     v0 = Column(String(255))
     v1 = Column(String(255))
@@ -39,35 +54,36 @@
     v0 = []
     v1 = []
     v2 = []
     v3 = []
     v4 = []
     v5 = []
 
+
 class Adapter(persist.Adapter):
     """the interface for Casbin adapters."""
 
     def __init__(self, engine, db_class=None, filtered=False):
         if isinstance(engine, str):
             self._engine = create_async_engine(engine, future=True)
         else:
             self._engine = engine
 
         if db_class is None:
             db_class = CasbinRule
         else:
             for attr in (
-                "id",
-                "ptype",
-                "v0",
-                "v1",
-                "v2",
-                "v3",
-                "v4",
-                "v5",
+                    "id",
+                    "ptype",
+                    "v0",
+                    "v1",
+                    "v2",
+                    "v3",
+                    "v4",
+                    "v5",
             ):  # id attr was used by filter
                 if not hasattr(db_class, attr):
                     raise Exception(f"{attr} not found in custom DatabaseClass.")
             Base.metadata = db_class.metadata
 
         self._db_class = db_class
         self.session_local = sessionmaker(
@@ -220,38 +236,37 @@
             for index in range(len(longest_rule)):
                 if index < len(new_rule):
                     setattr(old_rule_line, "v{}".format(index), new_rule[index])
                 else:
                     setattr(old_rule_line, "v{}".format(index), None)
 
     async def update_policies(
-        self,
-        sec: str,
-        ptype: str,
-        old_rules: [
-            [str],
-        ],
-        new_rules: [
-            [str],
-        ],
+            self,
+            sec: str,
+            ptype: str,
+            old_rules: [
+                [str],
+            ],
+            new_rules: [
+                [str],
+            ],
     ) -> None:
         """
         Update the old_rules with the new_rules in the database (storage).
 
         :param sec: section type
         :param ptype: policy type
         :param old_rules: the old rules that need to be modified
         :param new_rules: the new rules to replace the old rules
 
         :return: None
         """
         for i in range(len(old_rules)):
             await self.update_policy(sec, ptype, old_rules[i], new_rules[i])
 
-
     async def update_filtered_policies(
             self, sec, ptype, new_rules: [[str]], field_index, *field_values
     ) -> [[str]]:
         """update_filtered_policies updates all the policies on the basis of the filter."""
 
         filter = Filter()
         filter.ptype = ptype
@@ -265,15 +280,14 @@
 
         return await self._update_filtered_policies(new_rules, filter)
 
     async def _update_filtered_policies(self, new_rules, filter) -> [[str]]:
         """_update_filtered_policies updates all the policies on the basis of the filter."""
 
         async with self._session_scope() as session:
-
             # Load old policies
 
             query = session.query(self._db_class).filter(
                 self._db_class.ptype == filter.ptype
             )
             filtered_query = self.filter_query(query, filter)
             old_rules = await filtered_query.all()
@@ -284,8 +298,8 @@
 
             # Insert new policies
 
             await self.add_policies("p", filter.ptype, new_rules)
 
             # return deleted rules
 
-            return old_rules
+            return old_rules
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.0.1/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-async-sqlalchemy-adapter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.0/setup.py` & `casbin_async_sqlalchemy_adapter-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 The casbin Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from setuptools import setup, find_packages, __version__
 from os import path
 
 desc_file = "README.md"
 
 with open(desc_file, "r") as fh:
     long_description = fh.read()
```

### Comparing `casbin_async_sqlalchemy_adapter-1.0.0/tests/test_adapter.py` & `casbin_async_sqlalchemy_adapter-1.0.1/tests/test_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 The casbin Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import asyncio
 import os
 from casbin_async_sqlalchemy_adapter import Adapter
 from casbin_async_sqlalchemy_adapter import Base
 from casbin_async_sqlalchemy_adapter import CasbinRule
 from casbin_async_sqlalchemy_adapter.adapter import Filter
 from unittest import IsolatedAsyncioTestCase
@@ -9,14 +23,15 @@
 from unittest import async_case
 import casbin
 from sqlalchemy import create_engine, Column, Integer, String
 from sqlalchemy.orm import sessionmaker
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 
+
 def get_fixture(path):
     dir_path = os.path.split(os.path.realpath(__file__))[0] + "/"
     return os.path.abspath(dir_path + path)
 
 
 def get_enforcer():
     engine = create_engine("sqlite://")
@@ -68,16 +83,14 @@
         self.assertFalse(e.enforce("alice", "data4", "read"))
         model = e.get_model()
         model.clear_policy()
         model.add_policy("p", "p", ["alice", "data4", "read"])
 
         self.assertTrue(e.enforce("alice", "data4", "read"))
 
-
-
     async def test_add_policy(self):
         e = get_enforcer()
 
         self.assertFalse(e.enforce("eve", "data3", "read"))
         self.assertFalse(e.enforce("eve", "data4", "read"))
 
         model = e.get_model()
@@ -96,15 +109,14 @@
         model = e.get_model()
         model.clear_policy()
         model.add_policies("p", "p", [("eve", "data3", "read"), ("eve", "data4", "read")])
 
         self.assertTrue(e.enforce("eve", "data3", "read"))
         self.assertTrue(e.enforce("eve", "data4", "read"))
 
-
     async def test_save_policy(self):
         e = get_enforcer()
         self.assertFalse(e.enforce("alice", "data4", "read"))
 
         model = e.get_model()
         model.clear_policy()
```

