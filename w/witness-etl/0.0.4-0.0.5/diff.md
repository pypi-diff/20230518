# Comparing `tmp/witness-etl-0.0.4.tar.gz` & `tmp/witness-etl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "witness-etl-0.0.4.tar", last modified: Mon Oct  3 06:13:07 2022, max compression
+gzip compressed data, was "witness-etl-0.0.5.tar", last modified: Thu May 18 16:04:14 2023, max compression
```

## Comparing `witness-etl-0.0.4.tar` & `witness-etl-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-10-03 06:13:07.428914 witness-etl-0.0.4/
--rw-rw-rw-   0        0        0    11558 2022-04-10 07:08:20.000000 witness-etl-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      877 2022-10-03 06:13:07.428914 witness-etl-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      339 2022-08-03 10:10:00.000000 witness-etl-0.0.4/README.md
--rw-rw-rw-   0        0        0      217 2022-06-24 13:23:37.000000 witness-etl-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      985 2022-10-03 06:13:07.429914 witness-etl-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-03 06:13:07.411914 witness-etl-0.0.4/witness/
--rw-rw-rw-   0        0        0      926 2022-06-17 14:48:03.000000 witness-etl-0.0.4/witness/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:13:07.414914 witness-etl-0.0.4/witness/core/
--rw-rw-rw-   0        0        0      672 2022-06-17 14:48:03.000000 witness-etl-0.0.4/witness/core/__init__.py
--rw-rw-rw-   0        0        0     2620 2022-10-03 05:37:04.000000 witness-etl-0.0.4/witness/core/abstract.py
--rw-rw-rw-   0        0        0     3097 2022-10-03 05:37:04.000000 witness-etl-0.0.4/witness/core/batch.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:13:07.418415 witness-etl-0.0.4/witness/extractors/
--rw-rw-rw-   0        0        0      632 2022-06-17 14:48:03.000000 witness-etl-0.0.4/witness/extractors/__init__.py
--rw-rw-rw-   0        0        0     2612 2022-08-03 10:10:01.000000 witness-etl-0.0.4/witness/extractors/database.py
--rw-rw-rw-   0        0        0      999 2022-06-17 14:48:03.000000 witness-etl-0.0.4/witness/extractors/file.py
--rw-rw-rw-   0        0        0     1108 2022-08-03 10:10:01.000000 witness-etl-0.0.4/witness/extractors/http.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:13:07.418915 witness-etl-0.0.4/witness/loaders/
--rw-rw-rw-   0        0        0      632 2022-06-17 14:48:03.000000 witness-etl-0.0.4/witness/loaders/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:13:07.420414 witness-etl-0.0.4/witness/providers/
--rw-rw-rw-   0        0        0        0 2022-10-03 05:37:04.000000 witness-etl-0.0.4/witness/providers/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:13:07.424414 witness-etl-0.0.4/witness/providers/pandas/
--rw-rw-rw-   0        0        0      672 2022-10-03 05:37:04.000000 witness-etl-0.0.4/witness/providers/pandas/__init__.py
--rw-rw-rw-   0        0        0     3362 2022-10-03 05:37:04.000000 witness-etl-0.0.4/witness/providers/pandas/core.py
--rw-rw-rw-   0        0        0     2306 2022-10-03 05:37:04.000000 witness-etl-0.0.4/witness/providers/pandas/extractors.py
--rw-rw-rw-   0        0        0     2145 2022-10-03 05:37:04.000000 witness-etl-0.0.4/witness/providers/pandas/loaders.py
--rw-rw-rw-   0        0        0     1105 2022-06-17 14:48:03.000000 witness-etl-0.0.4/witness/version.py
-drwxrwxrwx   0        0        0        0 2022-10-03 06:13:07.428413 witness-etl-0.0.4/witness_etl.egg-info/
--rw-rw-rw-   0        0        0      877 2022-10-03 06:13:07.000000 witness-etl-0.0.4/witness_etl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2022-10-03 06:13:07.000000 witness-etl-0.0.4/witness_etl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-03 06:13:07.000000 witness-etl-0.0.4/witness_etl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2022-10-03 06:13:07.000000 witness-etl-0.0.4/witness_etl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-03 06:13:07.000000 witness-etl-0.0.4/witness_etl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.616954 witness-etl-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2022-10-24 01:46:22.000000 witness-etl-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1179 2023-05-18 16:04:14.618392 witness-etl-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-05-11 16:29:07.000000 witness-etl-0.0.5/README.md
+-rw-rw-rw-   0        0        0      217 2022-10-24 01:46:22.000000 witness-etl-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1013 2023-05-18 16:04:14.622405 witness-etl-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.426718 witness-etl-0.0.5/tests/
+-rw-rw-rw-   0        0        0     1204 2023-05-11 15:36:54.000000 witness-etl-0.0.5/tests/test_batch.py
+-rw-rw-rw-   0        0        0     1916 2023-05-11 16:04:37.000000 witness-etl-0.0.5/tests/test_dump.py
+-rw-rw-rw-   0        0        0     2415 2023-05-11 11:47:54.000000 witness-etl-0.0.5/tests/test_http_extractors.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.447478 witness-etl-0.0.5/witness/
+-rw-rw-rw-   0        0        0      959 2023-05-11 09:39:22.000000 witness-etl-0.0.5/witness/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.491371 witness-etl-0.0.5/witness/core/
+-rw-rw-rw-   0        0        0      712 2023-05-11 09:39:22.000000 witness-etl-0.0.5/witness/core/__init__.py
+-rw-rw-rw-   0        0        0     4046 2023-05-11 11:19:15.000000 witness-etl-0.0.5/witness/core/abstract.py
+-rw-rw-rw-   0        0        0     4304 2023-05-11 16:00:54.000000 witness-etl-0.0.5/witness/core/batch.py
+-rw-rw-rw-   0        0        0     1810 2023-05-11 16:27:43.000000 witness-etl-0.0.5/witness/core/meta.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.529668 witness-etl-0.0.5/witness/extractors/
+-rw-rw-rw-   0        0        0      632 2022-10-24 01:46:22.000000 witness-etl-0.0.5/witness/extractors/__init__.py
+-rw-rw-rw-   0        0        0     2359 2022-11-24 13:54:30.000000 witness-etl-0.0.5/witness/extractors/database.py
+-rw-rw-rw-   0        0        0      861 2023-05-15 09:26:02.000000 witness-etl-0.0.5/witness/extractors/file.py
+-rw-rw-rw-   0        0        0     1251 2023-05-11 11:19:15.000000 witness-etl-0.0.5/witness/extractors/http.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.532330 witness-etl-0.0.5/witness/loaders/
+-rw-rw-rw-   0        0        0      632 2022-10-24 01:46:22.000000 witness-etl-0.0.5/witness/loaders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.533743 witness-etl-0.0.5/witness/providers/
+-rw-rw-rw-   0        0        0        0 2022-11-01 04:30:23.000000 witness-etl-0.0.5/witness/providers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.555180 witness-etl-0.0.5/witness/providers/pandas/
+-rw-rw-rw-   0        0        0      630 2023-01-09 04:38:56.000000 witness-etl-0.0.5/witness/providers/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3300 2023-05-18 15:51:50.000000 witness-etl-0.0.5/witness/providers/pandas/core.py
+-rw-rw-rw-   0        0        0     1500 2023-05-18 15:31:12.000000 witness-etl-0.0.5/witness/providers/pandas/extractors.py
+-rw-rw-rw-   0        0        0     2922 2023-05-18 15:51:50.000000 witness-etl-0.0.5/witness/providers/pandas/loaders.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.569709 witness-etl-0.0.5/witness/serializers/
+-rw-rw-rw-   0        0        0        0 2023-01-09 04:29:12.000000 witness-etl-0.0.5/witness/serializers/__init__.py
+-rw-rw-rw-   0        0        0      953 2023-01-12 11:39:38.000000 witness-etl-0.0.5/witness/serializers/http.py
+-rw-rw-rw-   0        0        0      997 2022-11-22 11:45:30.000000 witness-etl-0.0.5/witness/version.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:04:14.615955 witness-etl-0.0.5/witness_etl.egg-info/
+-rw-rw-rw-   0        0        0     1179 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      796 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-18 16:04:14.000000 witness-etl-0.0.5/witness_etl.egg-info/top_level.txt
```

### Comparing `witness-etl-0.0.4/LICENSE` & `witness-etl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.4/PKG-INFO` & `witness-etl-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: witness-etl
-Version: 0.0.4
+Version: 0.0.5
 Summary: A minimal ETL library.
 Author: Eugene Popov
 Author-email: evgeniypalych@gmail.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eppv/witness
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
@@ -12,21 +12,39 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # witness
 
-A minimal ETL library.
+A minimal batch processing ETL library.
+
 Intended to be simple and concise.
 
+Made to wrap common instrumental approaches in a high-level abstraction.
+And for fun.
+
 ## Installation
 ```
 python3 -m pip install witness-etl
 ```
 
+## Concepts
+
+### Batch
+The main concept of the lib. It's a container for some useful data and metadata. 
+
+```python
+from witness import Batch
+
+batch = Batch()
+
+print(batch)
+
+```
+
 ## Versioning
 This lib supports [SemVer](https://semver.org/) approach for all packages released.
 
 ## Contributing
 Want to help or got questions? 
 [Contact me.](mailto:evgeniypalych@gmail.com)
```

### Comparing `witness-etl-0.0.4/setup.cfg` & `witness-etl-0.0.5/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6974 6e65 7373 2d65 746c 0d0a   = witness-etl..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 340d  version = 0.0.4.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 350d  version = 0.0.5.
 00000030: 0a61 7574 686f 7220 3d20 4575 6765 6e65  .author = Eugene
 00000040: 2050 6f70 6f76 0d0a 6175 7468 6f72 5f65   Popov..author_e
 00000050: 6d61 696c 203d 2065 7667 656e 6979 7061  mail = evgeniypa
 00000060: 6c79 6368 4067 6d61 696c 2e63 6f6d 0d0a  lych@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000080: 6d69 6e69 6d61 6c20 4554 4c20 6c69 6272  minimal ETL libr
 00000090: 6172 792e 0d0a 6c6f 6e67 5f64 6573 6372  ary...long_descr
@@ -41,22 +41,24 @@
 00000280: 6865 656c 0d0a 696e 7374 616c 6c5f 7265  heel..install_re
 00000290: 7175 6972 6573 203d 200d 0a09 7079 6172  quires = ...pyar
 000002a0: 726f 773e 3d38 2e30 2e30 0d0a 0970 796f  row>=8.0.0...pyo
 000002b0: 6462 633e 3d34 2e30 2e30 0d0a 096e 756d  dbc>=4.0.0...num
 000002c0: 7079 3e3d 312e 3233 2e30 3b20 7079 7468  py>=1.23.0; pyth
 000002d0: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2233  on_version >= "3
 000002e0: 2e39 220d 0a09 7061 6e64 6173 3e3d 312e  .9"...pandas>=1.
-000002f0: 342e 300d 0a09 7371 6c61 6c63 6865 6d79  4.0...sqlalchemy
-00000300: 3e3d 312e 342e 300d 0a09 7265 7175 6573  >=1.4.0...reques
-00000310: 7473 3e3d 322e 302e 300d 0a0d 0a5b 6f70  ts>=2.0.0....[op
-00000320: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000330: 696e 645d 0d0a 696e 636c 7564 6520 3d20  ind]..include = 
-00000340: 0d0a 0977 6974 6e65 7373 2a0d 0a65 7863  ...witness*..exc
-00000350: 6c75 6465 203d 200d 0a09 7465 6d70 2a0d  lude = ...temp*.
-00000360: 0a09 7363 7269 7074 732a 0d0a 0964 6f63  ..scripts*...doc
-00000370: 732a 0d0a 0974 6573 7473 2a0d 0a09 7769  s*...tests*...wi
-00000380: 746e 6573 732e 7465 7374 732a 0d0a 0d0a  tness.tests*....
-00000390: 5b66 696c 6573 5d0d 0a70 6163 6b61 6765  [files]..package
-000003a0: 7320 3d20 7769 746e 6573 730d 0a0d 0a5b  s = witness....[
-000003b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000003c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000003d0: 6520 3d20 300d 0a0d 0a                   e = 0....
+000002f0: 342e 302c 3c32 2e30 0d0a 0973 716c 616c  4.0,<2.0...sqlal
+00000300: 6368 656d 793e 3d31 2e34 2e30 2c3c 322e  chemy>=1.4.0,<2.
+00000310: 300d 0a09 7265 7175 6573 7473 3e3d 322e  0...requests>=2.
+00000320: 302e 300d 0a09 7065 6e64 756c 756d 3e3d  0.0...pendulum>=
+00000330: 322e 312e 300d 0a0d 0a5b 6f70 7469 6f6e  2.1.0....[option
+00000340: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000350: 0d0a 696e 636c 7564 6520 3d20 0d0a 0977  ..include = ...w
+00000360: 6974 6e65 7373 2a0d 0a65 7863 6c75 6465  itness*..exclude
+00000370: 203d 200d 0a09 7465 6d70 2a0d 0a09 7363   = ...temp*...sc
+00000380: 7269 7074 732a 0d0a 0964 6f63 732a 0d0a  ripts*...docs*..
+00000390: 0974 6573 7473 2a0d 0a09 7769 746e 6573  .tests*...witnes
+000003a0: 732e 7465 7374 732a 0d0a 0d0a 5b66 696c  s.tests*....[fil
+000003b0: 6573 5d0d 0a70 6163 6b61 6765 7320 3d20  es]..packages = 
+000003c0: 7769 746e 6573 730d 0a0d 0a5b 6567 675f  witness....[egg_
+000003d0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+000003e0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000003f0: 300d 0a0d 0a                             0....
```

### Comparing `witness-etl-0.0.4/witness/__init__.py` & `witness-etl-0.0.5/witness/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 from .core.batch import Batch
+from .core.meta import MetaData
 from . import version
 
 # Meta
 __version__ = version.version
 __author__ = 'Eugene Popov'
```

### Comparing `witness-etl-0.0.4/witness/core/__init__.py` & `witness-etl-0.0.5/witness/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 from witness.core.batch import Batch
+from witness.core.meta import MetaData
```

### Comparing `witness-etl-0.0.4/witness/core/abstract.py` & `witness-etl-0.0.5/witness/core/abstract.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
 import logging
 from abc import ABCMeta, abstractmethod
-from datetime import datetime
+from typing import Optional
+import pendulum
 
 log = logging.getLogger(__name__)
 
 
 class AbstractBatch(metaclass=ABCMeta):
 
     @abstractmethod
@@ -40,19 +41,23 @@
 
 class AbstractExtractor(metaclass=ABCMeta):
 
     def __init__(self, uri=None):
 
         self.uri = uri
         self.output = None
-        self.extraction_timestamp: datetime or None = None
+        self.extraction_timestamp: Optional[pendulum.DateTime] = None
+        self.serializer: Optional[AbstractSerializer] = None
+        self.is_unified = False
 
-    @abstractmethod
     def _set_extraction_timestamp(self):
-        raise NotImplementedError
+        setattr(self, 'extraction_timestamp', pendulum.now())
+
+    def _set_unified_true(self):
+        setattr(self, 'is_unified', True)
 
     @abstractmethod
     def extract(self):
         """
         An abstract method for data extraction.
         """
         raise NotImplementedError
@@ -67,33 +72,64 @@
 
 class AbstractLoader(metaclass=ABCMeta):
 
     def __init__(self, uri=None):
 
         self.uri = uri
         self.batch = None
+        self.meta_to_attach: Optional[dict] = None
         self.output = None
+        self.serializer: Optional[AbstractSerializer] = None
 
     @abstractmethod
     def prepare(self, batch):
         """
         An abstract method of preparing data from a Batch object for loading.
         """
         self._set_batch(batch)
 
     @abstractmethod
-    def attach_meta(self, meta_elements: [list[str]] or None = None):
+    def attach_meta(self, meta_elements: Optional[list] = None):
         """
         An abstract method for attaching meta from Batch-object
         to data prepared for loading.
         """
-        raise NotImplementedError
+        self._set_meta_to_attach(meta_elements)
 
     @abstractmethod
     def load(self):
         """
         An abstract method for loading data to destination store.
         """
         raise NotImplementedError
 
     def _set_batch(self, batch):
         setattr(self, 'batch', batch)
+
+    def _set_meta_to_attach(self, meta_elements):
+        try:
+            meta = self.batch.meta
+        except AttributeError:
+            log.exception('No batch object was passed to loader.'
+                          'Pass a batch object to "prepare" method first.')
+            raise AttributeError('No batch object was passed to loader')
+        if meta_elements is None:
+            elements_to_attach = {element: str(getattr(meta, element)) for element in meta}
+        else:
+            elements_to_attach = {element: str(getattr(meta, element)) for element in meta_elements}
+
+        setattr(self, 'meta_to_attach', elements_to_attach)
+
+
+class AbstractSerializer(metaclass=ABCMeta):
+
+    def to_batch(self, raw, *args, **kwargs):
+        """
+        An abstract method for serializing extracted data to unified batch format.
+        """
+        raise NotImplementedError
+
+    def from_batch(self, data, *args, **kwargs):
+        """
+        An abstract method for deserializing data from unified batch format.
+        """
+        raise NotImplementedError
```

### Comparing `witness-etl-0.0.4/witness/core/batch.py` & `witness-etl-0.0.5/witness/providers/pandas/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,88 +8,95 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
-from witness.core.abstract import AbstractBatch
-import pickle
+import pandas as pd
+import logging
+from typing import Optional, Union
+from witness.core.abstract import AbstractLoader, AbstractSerializer, AbstractExtractor
+
+log = logging.getLogger(__name__)
+
+
+class PandasSerializer(AbstractSerializer):
+  
+    @staticmethod
+    def handle_df_list(raw: list) -> pd.DataFrame:
+        return pd.concat(raw)
+
+    @staticmethod
+    def handle_df_dict(raw: dict) -> pd.DataFrame:
+        dfs = []
+        for df_name, df in raw.items():
+            df.dropna(axis=1, inplace=True, how="all")
+            df["df_name"] = df_name
+            dfs.append(df)
+        return pd.concat(dfs)
+
+    def to_batch(self, raw: Union[pd.DataFrame, list, dict], *args, **kwargs):
+        if isinstance(raw, pd.DataFrame):
+            return raw.to_dict(orient="records")
+        elif isinstance(raw, dict):
+            return self.handle_df_dict(raw)
+        elif isinstance(raw, list):
+            return self.handle_df_list(raw)
+        else:
+            raise ValueError("Unknown datastructure passed.")
+
+    def from_batch(self, data, *args, dtype="str", **kwargs):
+        df = pd.DataFrame(data, dtype=dtype)
+        return df
+
+
+class PandasLoader(AbstractLoader):
+    def __init__(
+        self, uri, serializer: Optional[AbstractSerializer] = PandasSerializer()
+    ):
+        super().__init__(uri)
+        self.serializer = serializer
+
+    def prepare(self, batch):
+        super().prepare(batch)
+        df = self.serializer.from_batch(batch.data)
+        self.output = df
+        return self
+
+    def attach_meta(self, meta_elements: Optional[list[str]] = None):
+        super().attach_meta(meta_elements)
+        for element in self.meta_to_attach:
+            self.output[element] = self.meta_to_attach[element]
+
+        return self
 
+    def load(self):
+        raise NotImplementedError
 
-class Batch(AbstractBatch):
+
+class PandasExtractor(AbstractExtractor):
     """
-    Central class of entire lib.
-    Able to store standardized data structure
-    containing data in form of records and metadata dictionary.
+    Basic pandas extractor class.
+    Provides a single 'unify' method for all child pandas extractors.
     """
 
-    __slots__ = ('data', 'meta')
-
-    def __init__(self, data=None, meta=None):
+    def __init__(self, uri, serializer: Optional[AbstractSerializer] = PandasSerializer()):
+        super().__init__(uri)
+        self.serializer = PandasSerializer()
 
-        self.data: list or None = data
-        self.meta: dict or None = meta
-        self.is_restored = False
-
-    def info(self):
-
-        if self.meta is None and self.data is None:
-            return 'Batch object is not containing any data.'
-
-        number_of_records = len(self.data) if self.data is not None else None
-
-        message = f"""
-        Number of records: {number_of_records}
-        Was {'restored from dump ' + f"{self.meta['dump_uri']}" if self.is_restored else 'originally extracted'}
-        Source: {self.meta['record_source']}
-        Extraction datetime: {self.meta['extraction_timestamp']}
-        """
-
-        try:
-            message = message + f"Tags: {self.meta['tags']}\n"
-        except KeyError:
-            pass
-
-        return message
-
-    def fill(self, extractor):
-        """
-        Fills batch internal datastructures using
-        the extractor passed in.
-        """
-        output = extractor.extract().unify().output
-        setattr(self, 'data', output['data'])
-        setattr(self, 'meta', output['meta'])
-        return self
+    output: pd.DataFrame
 
-    def push(self, loader, meta_elements: [list[str]] or None = None):
-        """
-        Pushes data, with the appropriate meta attached,
-        to the store defined by the loader passed in.
-        """
-        loader.prepare(self).attach_meta(meta_elements).load()
+    def extract(self):
+        self._set_extraction_timestamp()
         return self
 
-    def _register_dump(self, uri):
-        self.meta['dump_uri'] = uri
+    def unify(self):
+        data = self.serializer.to_batch(self.output)
+        meta = {
+            "extraction_timestamp": self.extraction_timestamp,
+            "record_source": self.uri,
+        }
 
-    def dump(self, uri):
-        """
-        Dumps batch data to pickle file with defined uri.
-        """
-        with open(uri, 'wb') as file:
-            pickle.dump(self.data, file)
-        self._register_dump(uri)
-
-    def restore(self, uri=None):
-        """
-        Fills batch with data from dump.
-        If no dump uri provided it'll try search in batch meta.
-        """
-        uri = self.meta['dump_uri'] if uri is None else uri
-        with open(uri, 'rb') as file:
-            output = pickle.load(file)
-        setattr(self, 'data', output)
-        self.is_restored = True
+        setattr(self, "output", {"meta": meta, "data": data})
+        self._set_unified_true()
         return self
-
```

### Comparing `witness-etl-0.0.4/witness/extractors/__init__.py` & `witness-etl-0.0.5/witness/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.4/witness/extractors/database.py` & `witness-etl-0.0.5/witness/extractors/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,35 +21,28 @@
 
 
 class DatabaseExtractor(AbstractExtractor):
 
     def __init__(self, uri):
         super().__init__(uri)
 
-    def _set_extraction_timestamp(self):
-        setattr(self, 'extraction_timestamp', datetime.now())
-
     def extract(self):
         self._set_extraction_timestamp()
 
     def unify(self):
         raise NotImplementedError
 
 
 class ODBCExtractor(DatabaseExtractor):
 
     def __init__(self, uri: str, query: str):
         self.uri: str = uri
         self.query: str = query if isinstance(query, str) and is_select(query) else None
         super().__init__(uri)
 
-    def _set_extraction_timestamp(self):
-        from datetime import datetime
-        setattr(self, 'extraction_timestamp', datetime.now())
-
     def extract(self):
         from pyodbc import connect
 
         connector = connect(self.uri)
         cursor = connector.cursor()
         rows = cursor.execute(self.query).fetchall()
```

### Comparing `witness-etl-0.0.4/witness/extractors/file.py` & `witness-etl-0.0.5/witness/extractors/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
-from datetime import datetime
 
 from witness.core.abstract import AbstractExtractor
 
 
 class FileExtractor(AbstractExtractor):
 
-    def _set_extraction_timestamp(self):
-        setattr(self, 'extraction_timestamp', datetime.now())
-
     def extract(self):
         self._set_extraction_timestamp()
 
     def unify(self):
         raise NotImplementedError
```

### Comparing `witness-etl-0.0.4/witness/extractors/http.py` & `witness-etl-0.0.5/witness/extractors/http.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 
-from datetime import datetime
-from witness.core.abstract import AbstractExtractor
+from witness.core.abstract import AbstractExtractor, AbstractSerializer
+from witness.serializers.http import JsonSerializer
 import requests
 from requests.auth import AuthBase
+from typing import Optional
 
 
 class HttpGetExtractor(AbstractExtractor):
 
-    def __init__(self, uri, params: dict or None = None, auth: AuthBase = None):
+    def __init__(self,
+                 uri,
+                 params: Optional[dict] = None,
+                 auth: Optional[AuthBase] = None,
+                 serializer: Optional[AbstractSerializer] = JsonSerializer()):
+        super().__init__(uri)
+        self.serializer = serializer
         self.params: dict or None = params
         self.auth = auth
-        super().__init__(uri)
-
-    def _set_extraction_timestamp(self):
-        setattr(self, 'extraction_timestamp', datetime.now())
 
     def extract(self):
 
         response = requests.get(url=self.uri, params=self.params, auth=self.auth)
         response.raise_for_status()
 
         setattr(self, 'output', response)
         self._set_extraction_timestamp()
 
         return self
 
     def unify(self):
-        raise NotImplementedError
-
-
-class JsonHttpGetExtractor(HttpGetExtractor):
-
-    def unify(self):
-
-        data = self.output.json()
         meta = {'extraction_timestamp': self.extraction_timestamp,
                 'record_source': self.uri}
-
+        data = self.serializer.to_batch(self.output)
         setattr(self, 'output', {'meta': meta, 'data': data})
-
+        self._set_unified_true()
         return self
+
+
+JsonHttpGetExtractor = HttpGetExtractor  # deprecated
```

### Comparing `witness-etl-0.0.4/witness/loaders/__init__.py` & `witness-etl-0.0.5/witness/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `witness-etl-0.0.4/witness/providers/pandas/__init__.py` & `witness-etl-0.0.5/witness/providers/pandas/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
-
-from .core import PandasBatch as Batch
```

### Comparing `witness-etl-0.0.4/witness/providers/pandas/core.py` & `witness-etl-0.0.5/witness/providers/pandas/loaders.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,97 +8,81 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
+
+from witness.providers.pandas.core import PandasLoader
 import pandas as pd
-import logging
-import pickle
-from witness.core.abstract import AbstractBatch, AbstractLoader, AbstractExtractor
-
-log = logging.getLogger(__name__)
-
-
-class PandasBatch(AbstractBatch):
-
-    __slots__ = ('data', 'meta')
-
-    def __init__(self, data=None, meta=None):
-        self.data: pd.DataFrame or None = data
-        self.meta: dict or None = meta
-        self.is_restored = False
-
-    def fill(self, extractor):
-        """
-        Fills batch internal datastructures using
-        the extractor passed in.
-        """
-        output = extractor.extract().unify().output
-        setattr(self, 'data', output['data'])
-        setattr(self, 'meta', output['meta'])
-        return self
 
-    def push(self, loader, meta_elements: [list[str]] or None = None):
-        """
-        Pushes data, with the appropriate meta attached,
-        to the store defined by the loader passed in.
-        """
-        loader.prepare(self).attach_meta(meta_elements).load()
-        return self
 
-    def _register_dump(self, uri):
-        self.meta['dump_uri'] = uri
+class PandasSQLLoader(PandasLoader):
+    """
+    Loader that uses Pandas DataFrame.to_sql method for loading data.
+
+    :param engine: sqlalchemy engine;
+    :param table: name of the destination table;
+    :param schema: name of the destination schema, None if not defined.
+    """
+
+    def __init__(
+        self, engine, table: str, schema: str or None = None, method: str or None = None
+    ):
+        self.engine = engine
+        self.schema = schema
+        self.table = table
+        self.method = method
+        uri = f"{schema}.{table}"
+        super().__init__(uri)
 
-    def dump(self, uri):
-        with open(uri, 'wb') as file:
-            pickle.dump(self.data, file)
-        self._register_dump(uri)
-
-    def restore(self, uri=None):
-        """
-        Fills batch with data from dump.
-        If no dump uri provided it'll try search in batch meta.
-        """
-        uri = self.meta['dump_uri'] if uri is None else uri
-        with open(uri, 'rb') as file:
-            output = pickle.load(file)
-        setattr(self, 'data', output)
-        self.is_restored = True
+    def load(self):
+        self.output.to_sql(
+            name=self.table,
+            con=self.engine,
+            schema=self.schema,
+            if_exists="append",
+            method=self.method,
+        )
         return self
 
-    def info(self):
-        pass
-
 
-class PandasLoader(AbstractLoader):
+class PandasExcelLoader(PandasLoader):
+    def __init__(self, uri, sheet_name="Sheet1", add_index=True):
 
-    def __init__(self, uri):
+        self.sheet_name = sheet_name
+        self.add_index = add_index
         super().__init__(uri)
 
-    def prepare(self, batch):
-        super().prepare(batch)
-        df = pd.DataFrame(batch.data, dtype='str')
-        self.output = df
+    def __load_single_sheet(self, **writer_kwargs):
+        with pd.ExcelWriter(path=self.uri, **writer_kwargs) as writer:
+            self.output.to_excel(
+                excel_writer=writer, sheet_name=self.sheet_name, index=self.add_index
+            )
         return self
 
-    def attach_meta(self, meta_elements: [list[str]] or None = None):
-        try:
-            meta = self.batch.meta
-            for element in meta:
-                meta[element] = str(meta[element])
-        except AttributeError:
-            log.exception('No batch object was passed to loader.'
-                          'Pass a batch object to "prepare" method first.')
-            raise AttributeError('No batch object was passed to loader')
-        if meta_elements is None:
-            for element in meta:
-                self.output[element] = meta[element]
-        else:
-            for element in meta_elements:
-                self.output[element] = meta[element]
+    def __load_multiple_sheets(self, **writer_kwargs):
+        with pd.ExcelWriter(path=self.uri, **writer_kwargs) as writer:
+            for sheet_name, df in self.output.items():
+                df.to_excel(
+                    excel_writer=writer,
+                    sheet_name=self.sheet_name,
+                    index=self.add_index,
+                )
+        return self
 
+    def load(self, **writer_kwargs):
+        if isinstance(self.output, pd.DataFrame):
+            return self.__load_single_sheet(**writer_kwargs)
+        elif isinstance(self.output, dict):
+            return self.__load_multiple_sheets(**writer_kwargs)
         return self
 
+
+class PandasFeatherLoader(PandasLoader):
+    def __init__(self, uri):
+        super().__init__(uri)
+
     def load(self):
-        raise NotImplementedError
+        self.output.to_feather(self.uri)
+        return self
```

### Comparing `witness-etl-0.0.4/witness/providers/pandas/extractors.py` & `witness-etl-0.0.5/witness/providers/pandas/extractors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,46 @@
-
 #  Copyright (c) 2022.  Eugene Popov.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #     you may not use this file except in compliance with the License.
 #     You may obtain a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 
-from witness.core.abstract import AbstractExtractor
-from datetime import datetime
 import pandas as pd
 import logging
 
-log = logging.getLogger(__name__)
-
-
-class PandasExtractor(AbstractExtractor):
-    """
-    Basic pandas extractor class.
-    Provides a single 'unify' method for all child pandas extractors.
-    """
-    def __init__(self, uri):
-        super().__init__(uri)
-
-    output: pd.DataFrame
-
-    def _set_extraction_timestamp(self):
-        setattr(self, 'extraction_timestamp', datetime.now())
-
-    def extract(self):
-        self._set_extraction_timestamp()
+from witness.providers.pandas.core import PandasExtractor
 
-    def unify(self):
-
-        data = self.output.to_dict(orient='records')
-        meta = {'extraction_timestamp': self.extraction_timestamp,
-                'record_source': self.uri}
-
-        setattr(self, 'output', {'meta': meta, 'data': data})
-
-        return self
+log = logging.getLogger(__name__)
 
 
 class PandasFeatherExtractor(PandasExtractor):
-
     def extract(self):
         df = pd.read_feather(self.uri)
-        setattr(self, 'output', df)
+        setattr(self, "output", df)
         super().extract()
 
         return self
 
 
 class PandasExcelExtractor(PandasExtractor):
-
     def __init__(self, uri, sheet_name=0, header=0, dtype=None):
         self.sheet_name: str or int or None = sheet_name
         self.header: int = header
         self.dtype: str or dict or None = dtype
         super().__init__(uri)
 
     def extract(self):
-        df = pd.read_excel(self.uri,
-                           sheet_name=self.sheet_name,
-                           header=self.header,
-                           dtype=self.dtype)
-        setattr(self, 'output', df)
+        df = pd.read_excel(
+            self.uri, sheet_name=self.sheet_name, header=self.header, dtype=self.dtype
+        )
+        setattr(self, "output", df)
         super().extract()
 
         return self
-
```

### Comparing `witness-etl-0.0.4/witness/version.py` & `witness-etl-0.0.5/witness/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 except ImportError:
     from importlib import metadata  # type: ignore[no-redef]
 
 try:
     version = metadata.version('witness-etl')
 except metadata.PackageNotFoundError:
     import logging
+    version = '0.0.5'
 
-    # log = logging.getLogger(__name__)
-    # log.warning("Package metadata could not be found. Overriding it hardcoded.")
-    version = '0.0.1'
-    # from setup import version
 
 del metadata
+
+if __name__ == '__main__':
+    print(version)
```

### Comparing `witness-etl-0.0.4/witness_etl.egg-info/PKG-INFO` & `witness-etl-0.0.5/witness_etl.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: witness-etl
-Version: 0.0.4
+Version: 0.0.5
 Summary: A minimal ETL library.
 Author: Eugene Popov
 Author-email: evgeniypalych@gmail.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eppv/witness
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
@@ -12,21 +12,39 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # witness
 
-A minimal ETL library.
+A minimal batch processing ETL library.
+
 Intended to be simple and concise.
 
+Made to wrap common instrumental approaches in a high-level abstraction.
+And for fun.
+
 ## Installation
 ```
 python3 -m pip install witness-etl
 ```
 
+## Concepts
+
+### Batch
+The main concept of the lib. It's a container for some useful data and metadata. 
+
+```python
+from witness import Batch
+
+batch = Batch()
+
+print(batch)
+
+```
+
 ## Versioning
 This lib supports [SemVer](https://semver.org/) approach for all packages released.
 
 ## Contributing
 Want to help or got questions? 
 [Contact me.](mailto:evgeniypalych@gmail.com)
```

