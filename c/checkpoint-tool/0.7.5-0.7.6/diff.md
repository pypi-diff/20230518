# Comparing `tmp/checkpoint_tool-0.7.5.tar.gz` & `tmp/checkpoint_tool-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.7.5.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.7.6.tar", max compression
```

## Comparing `checkpoint_tool-0.7.5.tar` & `checkpoint_tool-0.7.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7153 2023-05-09 01:45:57.090652 checkpoint_tool-0.7.5/README.md
--rw-r--r--   0        0        0      608 2023-05-09 01:50:05.066517 checkpoint_tool-0.7.5/checkpoint/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-09 01:19:11.117797 checkpoint_tool-0.7.5/checkpoint/app.py
--rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.5/checkpoint/database.py
--rw-r--r--   0        0        0     7214 2023-05-09 01:48:29.158359 checkpoint_tool-0.7.5/checkpoint/graph.py
--rw-r--r--   0        0        0    10996 2023-05-09 01:49:51.784680 checkpoint_tool-0.7.5/checkpoint/task.py
--rw-r--r--   0        0        0     1461 2023-05-03 14:04:28.456816 checkpoint_tool-0.7.5/checkpoint/types.py
--rw-r--r--   0        0        0      676 2023-05-09 01:49:27.861375 checkpoint_tool-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     8007 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     7199 2023-05-18 00:40:34.124837 checkpoint_tool-0.7.6/README.md
+-rw-r--r--   0        0        0      608 2023-05-09 01:50:05.066517 checkpoint_tool-0.7.6/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-09 01:19:11.117797 checkpoint_tool-0.7.6/checkpoint/app.py
+-rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.6/checkpoint/database.py
+-rw-r--r--   0        0        0     7243 2023-05-18 04:16:07.403508 checkpoint_tool-0.7.6/checkpoint/graph.py
+-rw-r--r--   0        0        0    10986 2023-05-18 04:15:50.488265 checkpoint_tool-0.7.6/checkpoint/task.py
+-rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 checkpoint_tool-0.7.6/checkpoint/types.py
+-rw-r--r--   0        0        0      677 2023-05-18 04:18:59.185017 checkpoint_tool-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     8004 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.6/PKG-INFO
```

### Comparing `checkpoint_tool-0.7.5/README.md` & `checkpoint_tool-0.7.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -230,11 +230,12 @@
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
 Please refer to `python -m checkpoint.app --help` for more info.
 
 
 
 ## TODO
- - [ ] Loader-based serialization
- - [ ] Simple visualizers
+- [ ] Shrink the role of DBCache to task directory manager
+- [ ] Task as functor
+- [ ] Simple visualizers
     - [ ] Task-wise progressbar
     - [ ] Graph visualizer
```

### Comparing `checkpoint_tool-0.7.5/checkpoint/__init__.py` & `checkpoint_tool-0.7.6/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.5/checkpoint/app.py` & `checkpoint_tool-0.7.6/checkpoint/app.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.5/checkpoint/database.py` & `checkpoint_tool-0.7.6/checkpoint/database.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.5/checkpoint/graph.py` & `checkpoint_tool-0.7.6/checkpoint/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ DAG processor """
 from __future__ import annotations
 from datetime import datetime
-from typing import Any, Protocol, Self, Sequence, runtime_checkable
+from typing import Any, Sequence
+from typing_extensions import Self, runtime_checkable, Protocol
 from collections import defaultdict
 from dataclasses import dataclass
 from concurrent.futures import Future, wait, FIRST_COMPLETED, Executor
 import logging
 
 import cloudpickle
 import networkx as nx
```

### Comparing `checkpoint_tool-0.7.5/checkpoint/task.py` & `checkpoint_tool-0.7.6/checkpoint/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
-from typing import Callable, ClassVar, Generic, Mapping, Protocol, Self, Sequence, Type, TypeVar, Any, cast, overload, get_origin
-from typing_extensions import ParamSpec
+from typing import Callable, Generic, Mapping, Protocol, Sequence, Type, TypeVar, Any, cast
+from typing_extensions import ParamSpec, Self, get_origin, overload
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from concurrent.futures import Executor
 import ast
 import os
 import logging
```

### Comparing `checkpoint_tool-0.7.5/checkpoint/types.py` & `checkpoint_tool-0.7.6/checkpoint/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
-from datetime import datetime
-from typing import Any, NewType, ParamSpec, Protocol, Type, TypeVar, runtime_checkable, Callable
+from typing import NewType, ParamSpec, TypeVar, Callable
 import os
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, Executor
 from pathlib import Path
 
 
 P = ParamSpec('P')
 R = TypeVar('R', covariant=True)
```

### Comparing `checkpoint_tool-0.7.5/pyproject.toml` & `checkpoint_tool-0.7.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.7.5"
+version = "0.7.6"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 typing-extensions = "^4.5.0"
 diskcache = "^5.6.1"
 cloudpickle = "^2.2.1"
 networkx = "^3.1"
 click = "^8.1.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `checkpoint_tool-0.7.5/PKG-INFO` & `checkpoint_tool-0.7.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.7.5
+Version: 0.7.6
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
@@ -252,12 +251,13 @@
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
 Please refer to `python -m checkpoint.app --help` for more info.
 
 
 
 ## TODO
- - [ ] Loader-based serialization
- - [ ] Simple visualizers
+- [ ] Shrink the role of DBCache to task directory manager
+- [ ] Task as functor
+- [ ] Simple visualizers
     - [ ] Task-wise progressbar
     - [ ] Graph visualizer
```

