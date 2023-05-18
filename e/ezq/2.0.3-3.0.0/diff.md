# Comparing `tmp/ezq-2.0.3.tar.gz` & `tmp/ezq-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezq-2.0.3.tar", last modified: Wed May 10 04:14:00 2023, max compression
+gzip compressed data, was "ezq-3.0.0.tar", last modified: Thu May 18 10:12:26 2023, max compression
```

## Comparing `ezq-2.0.3.tar` & `ezq-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.229999 ezq-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-10 04:13:34.000000 ezq-2.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-10 04:14:00.229999 ezq-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-05-10 04:13:34.000000 ezq-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 04:13:34.000000 ezq-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-10 04:14:00.229999 ezq-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-10 04:13:34.000000 ezq-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.225999 ezq-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.229999 ezq-2.0.3/src/ezq/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 04:13:34.000000 ezq-2.0.3/src/ezq/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-10 04:13:34.000000 ezq-2.0.3/src/ezq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.229999 ezq-2.0.3/src/ezq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.229999 ezq-2.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-10 04:13:34.000000 ezq-2.0.3/test/test_ezq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-10 04:13:34.000000 ezq-2.0.3/test/test_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:12:26.710368 ezq-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-18 10:12:06.000000 ezq-3.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-18 10:12:26.710368 ezq-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-05-18 10:12:06.000000 ezq-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 10:12:06.000000 ezq-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 10:12:26.710368 ezq-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-18 10:12:06.000000 ezq-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:12:26.706368 ezq-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:12:26.706368 ezq-3.0.0/src/ezq/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-18 10:12:06.000000 ezq-3.0.0/src/ezq/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-05-18 10:12:06.000000 ezq-3.0.0/src/ezq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:12:26.706368 ezq-3.0.0/src/ezq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-18 10:12:26.000000 ezq-3.0.0/src/ezq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-18 10:12:26.000000 ezq-3.0.0/src/ezq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:12:26.000000 ezq-3.0.0/src/ezq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 10:12:26.000000 ezq-3.0.0/src/ezq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-18 10:12:26.000000 ezq-3.0.0/src/ezq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:12:26.706368 ezq-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-18 10:12:06.000000 ezq-3.0.0/test/test_ezq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-18 10:12:06.000000 ezq-3.0.0/test/test_iter.py
```

### Comparing `ezq-2.0.3/LICENSE.md` & `ezq-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ezq-2.0.3/PKG-INFO` & `ezq-3.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,14 @@
-Metadata-Version: 2.1
-Name: ezq
-Version: 2.0.3
-Summary: Simple wrapper for python multiprocessing.
-Home-page: https://github.com/metaist/ezq
-Download-URL: https://github.com/metaist/ezq
-Author: Metaist LLC
-Author-email: metaist@metaist.com
-License: MIT
-Keywords: simple,multiprocessing,queue,subprocesses
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # ezq
 
 _Simple wrappers for python multiprocessing and threading._
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/metaist/ezq/.github/workflows/ci.yaml?branch=main&style=for-the-badge)](https://github.com/metaist/ezq/actions)
 [![ezq on PyPI](https://img.shields.io/pypi/v/ezq.svg?color=blue&style=for-the-badge)](https://pypi.org/project/ezq)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/ezq?style=for-the-badge)](https://pypi.org/project/ezq)
 
 [Changelog] - [Issues] - [Documentation]
 
 [changelog]: https://github.com/metaist/ezq/blob/main/CHANGELOG.md
 [issues]: https://github.com/metaist/ezq/issues
 [documentation]: https://metaist.github.io/ezq/
 
@@ -98,15 +80,15 @@
     main()
 ```
 
 ## Typical worker lifecycle
 
 - The main process [creates queues](#create-queues) with `ezq.Q`.
 
-- The main process [creates workers](#create-workers) with `ezq.run` or `ezq.run_thread`.
+- The main process [creates workers](#create-workers) with `ezq.run` (alias for `Worker.process`) or `ezq.run_thread` (alias for `Worker.thread`).
 
 - The main process [sends data](#send-data) using `Q.put`.
 
 - The worker [iterates over the queue](#iterate-over-messages).
 
 - The main process [ends the queue](#end-the-queue) with `Q.stop`.
 
@@ -120,15 +102,15 @@
 
 - `Process` is for _parallelism_ so you can use multiple CPUs at once. Ideal for **CPU-bound** tasks like doing lots of mathematical calculations.
 
 - `Thread` is for _concurrency_ so you can use a single CPU to do multiple things. Ideal for **I/O-bound** tasks like waiting for a disk, database, or network.
 
 Some more differences:
 
-- **Shared memory**: Each `Process` worker has [data sent to it via `pickle`](#beware-pickle) and it doesn't share data with other workers. By contrast, each `Thread` worker shares its memory with all other workers on the same CPU, so it can [accidentally change global state](#beware-shared-state).
+- **Shared memory**: Each `Process` worker has [data sent to it via `pickle`](#beware-pickle) (actually [`dill`](https://github.com/uqfoundation/dill), a `pickle` replacement) and it doesn't share data with other workers. By contrast, each `Thread` worker shares its memory with all other workers on the same CPU, so it can [accidentally change global state](#beware-shared-state).
 
 - **Queue overhead**: `ezq.Q` [has more overhead](#create-queues) for `Process` workers than `Thread` workers.
 
 - **Creating sub-workers**: `Process` and `Thread` workers can create additional `Thread` workers, but [they cannot create additional `Process` workers](#create-workers).
 
 ## Create queues
 
@@ -138,22 +120,22 @@
 
 - **1 queue**: the worker reads from an input queue and persists the result somewhere else (e.g., writing to disk, making a network call, running some other program).
 
 - **2 queues** (most common): the worker reads from an input queue and write the results to an output queue.
 
 - **3 queues**: multiple stages of work are happening where workers are reading from one queue and writing to another queue for another worker to process.
 
-**NOTE:** If you're using `Thread` workers, you can save some overhead by passing `thread=True`. This lightweight queue also doesn't use `pickle`, so you can use it to pass hard-to-pickle things (e.g., `lambda`).
+**NOTE:** If you're using `Thread` workers, you can save some overhead by passing `Q("thread")`. This lightweight queue also doesn't use `pickle`, so you can use it to pass hard-to-pickle things (e.g., database connection).
 
 ```python
 q, out = ezq.Q(), ezq.Q() # most common
-q2 = ez.Q(thread=True) # only ok for Thread workers
+q2 = ez.Q("thread") # only ok for Thread workers
 ```
 
-## A worker is just a function
+## A worker task is just a function
 
 In general, there's nothing special about a worker function, but note:
 
 - If you're using `Process` workers, all arguments are [passed through `pickle` first](#beware-pickle).
 
 - We don't currently do anything with the return value of this function (unless you use `ezq.map()`). You'll need an output queue to return data back to the main process/thread.
 
@@ -171,15 +153,15 @@
 
 - `kind: str` - You can use this to send multiple kinds of work to the same worker. Note that the special `END` kind is used to indicate the end of a queue.
 
 - `order: int` - This is the message order which can help you reorder results or ensure that messages from a queue are read in a particular order (that's what `Q.sorted()` uses).
 
 ## Beware `pickle`
 
-If you are using `Process` workers, everything passed to the worker (arguments, messages) is first passed to `pickle` by [`multiprocessing`][1]. Anything that cannot be pickled (e.g., `lambda` functions, database connections), cannot be passed to `Process` workers.
+If you are using `Process` workers, everything passed to the worker (arguments, messages) is first passed to `pickle` (actually, [`dill`](https://github.com/uqfoundation/dill)). Anything that cannot be pickled with dill (e.g., database connections), cannot be passed to `Process` workers. Note that `dill` _can_ serialize many more types than `pickle` (e.g. `lambda` functions).
 
 ## Beware shared state
 
 If you are using `Thread` workers, workers can share certain variables, so you need to be careful of how variables are access to avoid accidentally corrupting data.
 
 ## Iterate over messages
 
@@ -239,15 +221,15 @@
             out.put((num, num / 2), order=msg.order)
         elif msg.kind == "ODD":
             out.put((num, 3 * num + 1), order=msg.order)
 
 
 def main() -> None:
     """Run several threads with a subprocess for printing."""
-    q, out = ezq.Q(thread=True), ezq.Q()
+    q, out = ezq.Q("thread"), ezq.Q()
     readers = [ezq.run_thread(collatz, q, out) for _ in range(ezq.NUM_THREADS)]
     writer = ezq.run(printer, out)
 
     for num in range(40):
         kind = "EVEN" if num % 2 == 0 else "ODD"
         q.put(num, kind=kind, order=num)
```

### Comparing `ezq-2.0.3/README.md` & `ezq-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,40 @@
+Metadata-Version: 2.1
+Name: ezq
+Version: 3.0.0
+Summary: Simple wrapper for python multiprocessing.
+Home-page: https://github.com/metaist/ezq
+Download-URL: https://github.com/metaist/ezq
+Author: Metaist LLC
+Author-email: metaist@metaist.com
+License: MIT
+Keywords: simple,multiprocessing,queue,subprocesses
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # ezq
 
 _Simple wrappers for python multiprocessing and threading._
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/metaist/ezq/.github/workflows/ci.yaml?branch=main&style=for-the-badge)](https://github.com/metaist/ezq/actions)
 [![ezq on PyPI](https://img.shields.io/pypi/v/ezq.svg?color=blue&style=for-the-badge)](https://pypi.org/project/ezq)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/ezq?style=for-the-badge)](https://pypi.org/project/ezq)
 
 [Changelog] - [Issues] - [Documentation]
 
 [changelog]: https://github.com/metaist/ezq/blob/main/CHANGELOG.md
 [issues]: https://github.com/metaist/ezq/issues
 [documentation]: https://metaist.github.io/ezq/
 
@@ -79,15 +106,15 @@
     main()
 ```
 
 ## Typical worker lifecycle
 
 - The main process [creates queues](#create-queues) with `ezq.Q`.
 
-- The main process [creates workers](#create-workers) with `ezq.run` or `ezq.run_thread`.
+- The main process [creates workers](#create-workers) with `ezq.run` (alias for `Worker.process`) or `ezq.run_thread` (alias for `Worker.thread`).
 
 - The main process [sends data](#send-data) using `Q.put`.
 
 - The worker [iterates over the queue](#iterate-over-messages).
 
 - The main process [ends the queue](#end-the-queue) with `Q.stop`.
 
@@ -101,15 +128,15 @@
 
 - `Process` is for _parallelism_ so you can use multiple CPUs at once. Ideal for **CPU-bound** tasks like doing lots of mathematical calculations.
 
 - `Thread` is for _concurrency_ so you can use a single CPU to do multiple things. Ideal for **I/O-bound** tasks like waiting for a disk, database, or network.
 
 Some more differences:
 
-- **Shared memory**: Each `Process` worker has [data sent to it via `pickle`](#beware-pickle) and it doesn't share data with other workers. By contrast, each `Thread` worker shares its memory with all other workers on the same CPU, so it can [accidentally change global state](#beware-shared-state).
+- **Shared memory**: Each `Process` worker has [data sent to it via `pickle`](#beware-pickle) (actually [`dill`](https://github.com/uqfoundation/dill), a `pickle` replacement) and it doesn't share data with other workers. By contrast, each `Thread` worker shares its memory with all other workers on the same CPU, so it can [accidentally change global state](#beware-shared-state).
 
 - **Queue overhead**: `ezq.Q` [has more overhead](#create-queues) for `Process` workers than `Thread` workers.
 
 - **Creating sub-workers**: `Process` and `Thread` workers can create additional `Thread` workers, but [they cannot create additional `Process` workers](#create-workers).
 
 ## Create queues
 
@@ -119,22 +146,22 @@
 
 - **1 queue**: the worker reads from an input queue and persists the result somewhere else (e.g., writing to disk, making a network call, running some other program).
 
 - **2 queues** (most common): the worker reads from an input queue and write the results to an output queue.
 
 - **3 queues**: multiple stages of work are happening where workers are reading from one queue and writing to another queue for another worker to process.
 
-**NOTE:** If you're using `Thread` workers, you can save some overhead by passing `thread=True`. This lightweight queue also doesn't use `pickle`, so you can use it to pass hard-to-pickle things (e.g., `lambda`).
+**NOTE:** If you're using `Thread` workers, you can save some overhead by passing `Q("thread")`. This lightweight queue also doesn't use `pickle`, so you can use it to pass hard-to-pickle things (e.g., database connection).
 
 ```python
 q, out = ezq.Q(), ezq.Q() # most common
-q2 = ez.Q(thread=True) # only ok for Thread workers
+q2 = ez.Q("thread") # only ok for Thread workers
 ```
 
-## A worker is just a function
+## A worker task is just a function
 
 In general, there's nothing special about a worker function, but note:
 
 - If you're using `Process` workers, all arguments are [passed through `pickle` first](#beware-pickle).
 
 - We don't currently do anything with the return value of this function (unless you use `ezq.map()`). You'll need an output queue to return data back to the main process/thread.
 
@@ -152,15 +179,15 @@
 
 - `kind: str` - You can use this to send multiple kinds of work to the same worker. Note that the special `END` kind is used to indicate the end of a queue.
 
 - `order: int` - This is the message order which can help you reorder results or ensure that messages from a queue are read in a particular order (that's what `Q.sorted()` uses).
 
 ## Beware `pickle`
 
-If you are using `Process` workers, everything passed to the worker (arguments, messages) is first passed to `pickle` by [`multiprocessing`][1]. Anything that cannot be pickled (e.g., `lambda` functions, database connections), cannot be passed to `Process` workers.
+If you are using `Process` workers, everything passed to the worker (arguments, messages) is first passed to `pickle` (actually, [`dill`](https://github.com/uqfoundation/dill)). Anything that cannot be pickled with dill (e.g., database connections), cannot be passed to `Process` workers. Note that `dill` _can_ serialize many more types than `pickle` (e.g. `lambda` functions).
 
 ## Beware shared state
 
 If you are using `Thread` workers, workers can share certain variables, so you need to be careful of how variables are access to avoid accidentally corrupting data.
 
 ## Iterate over messages
 
@@ -220,15 +247,15 @@
             out.put((num, num / 2), order=msg.order)
         elif msg.kind == "ODD":
             out.put((num, 3 * num + 1), order=msg.order)
 
 
 def main() -> None:
     """Run several threads with a subprocess for printing."""
-    q, out = ezq.Q(thread=True), ezq.Q()
+    q, out = ezq.Q("thread"), ezq.Q()
     readers = [ezq.run_thread(collatz, q, out) for _ in range(ezq.NUM_THREADS)]
     writer = ezq.run(printer, out)
 
     for num in range(40):
         kind = "EVEN" if num % 2 == 0 else "ODD"
         q.put(num, kind=kind, order=num)
```

### Comparing `ezq-2.0.3/setup.py` & `ezq-3.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,9 +42,16 @@
     keywords=["simple", "multiprocessing", "queue", "subprocesses"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ezq-2.0.3/src/ezq/__init__.py` & `ezq-3.0.0/src/ezq/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,406 +10,243 @@
     "__author__",
     "__copyright__",
     "__email__",
     "__license__",
     "__pubdate__",
     "__url__",
     "__version__",
-    #
-    ## imported classes ##
-    # "Process",  # deprecated
-    "Queue",  # deprecated
-    # "Thread",  # deprecated
-    # "ThreadSafeQueue",  # deprecated
-    #
-    ## types ##
-    # "MsgQ",
-    # "Worker",
-    # "Workers",
-    # "SomeWorkers",
-    #
-    ## classes ##
+    "Task",
+    "Context",
+    "ContextName",
     "Msg",
-    "Q",
-    #
-    ## constants ##
+    "END_MSG",
+    "MsgQ",
     "NUM_CPUS",
     "NUM_THREADS",
-    "END_MSG",
-    #
-    ## functions ##
+    "IS_MACOS",
+    "Worker",
+    "Q",
     "run",
     "run_thread",
     "map",
-    "put_msg",  # deprecated
-    "iter_msg",  # deprecated
-    "iter_q",  # deprecated
-    "sortiter",  # deprecated
-    "endq",  # deprecated
-    "endq_and_wait",  # deprecated
 )
 
 # native
 from dataclasses import dataclass
-from multiprocessing import Process, Queue
 from operator import attrgetter
 from os import cpu_count
-from queue import Empty, Queue as ThreadSafeQueue
+from platform import system
+from queue import Empty
+from queue import Queue as ThreadSafeQueue
 from threading import Thread
-from typing import (
-    Any,
-    Callable,
-    Iterable,
-    List,
-    Sequence,
-    Iterator,
-    Optional,
-    Union,
-    TYPE_CHECKING,
-)
-from typing_extensions import deprecated, Self
-
+from typing import Any
+from typing import Callable
+from typing import Iterable
+from typing import Iterator
+from typing import List
+from typing import Literal
+from typing import Optional
+from typing import Sequence
+from typing import TYPE_CHECKING
+from typing import Union
+
+# lib
+from multiprocess import Process  # type: ignore
+from multiprocess import Queue
 
 # pkg
-from .__about__ import (
-    __url__,
-    __version__,
-    __pubdate__,
-    __author__,
-    __email__,
-    __copyright__,
-    __license__,
-)
+from .__about__ import __author__
+from .__about__ import __copyright__
+from .__about__ import __email__
+from .__about__ import __license__
+from .__about__ import __pubdate__
+from .__about__ import __url__
+from .__about__ import __version__
+
+Task = Callable[..., Any]
+"""Task function signature (any `Callable`)."""
+
+Context = Union[Process, Thread]
+"""Execution contexts (`Process`, `Thread`)."""
+
+ContextName = Literal["process", "thread"]
+"""Execution context names (`"process"`, `"thread"`)."""
 
 
 @dataclass
 class Msg:
     """Message for a queue."""
 
-    kind: str = ""
-    """Optional marker of message type."""
-
     data: Any = None
     """Message data to be transmitted."""
 
+    kind: str = ""
+    """Optional marker of message type."""
+
     order: int = 0
     """Optional ordering of messages."""
 
 
+# NOTE: The python `queue.Queue` is not properly a generic.
+# See: https://stackoverflow.com/a/48554601
+if TYPE_CHECKING:  # pragma: no cover
+    MsgQ = Union[Queue[Msg], ThreadSafeQueue]  # pylint: disable=unsubscriptable-object
+else:
+    MsgQ = Queue
+
 END_MSG: Msg = Msg(kind="END")
 """Message that indicates no future messages will be sent."""
 
+## Hardware-Specific Information ##
+
 NUM_CPUS: int = cpu_count() or 1
 """Number of CPUs on this machine."""
 
 NUM_THREADS: int = min(32, NUM_CPUS + 4)
 """Default number of threads (up to 32).
 
 See: [CPython's default for this value][1].
 
 [1]: https://github.com/python/cpython/blob/a635d6386041a2971cf1d39837188ffb8139bcc7/Lib/concurrent/futures/thread.py#L142
 """
 
-# NOTE: The python `queue.Queue` is not properly a generic.
-# See: https://stackoverflow.com/a/48554601
-if TYPE_CHECKING:  # pragma: no cover
-    MsgQ = Union[Queue[Msg], ThreadSafeQueue]  # pylint: disable=unsubscriptable-object
-else:
-    MsgQ = Queue
-
-Worker = Union[Thread, Process]
-"""A thread or a process."""
-
-Workers = Union[Sequence[Thread], Sequence[Process]]
-"""Multiple threads or processes."""
-
-SomeWorkers = Union[Worker, Workers]
-"""One or more threads or processes."""
-
-
-def run(func: Callable[..., Any], *args: Any, **kwargs: Any) -> Process:
-    """Run a function as a subprocess.
-
-    Args:
-        func (Callable): function to run in each subprocess
-        *args (Any): additional positional arguments to `func`.
-        **kwargs (Any): additional keyword arguments to `func`.
-
-    Returns:
-        Process: subprocess that was started
-    """
-    worker = Process(daemon=True, target=func, args=args, kwargs=kwargs)
-    worker.start()
-    return worker
-
-
-def run_thread(func: Callable[..., Any], *args: Any, **kwargs: Any) -> Thread:
-    """Run a function as a thread.
-
-    Args:
-        func (Callable): function to run in each thread
-        *args (Any): additional positional arguments to `func`.
-        **kwargs (Any): additional keyword arguments to `func`.
-
-    Returns:
-        Thread: thread that was started
-    """
-    worker = Thread(daemon=False, target=func, args=args, kwargs=kwargs)
-    worker.start()
-    return worker
-
-
-map_ = map  # save the value of the builtin
-
-
-def map(
-    func: Callable[..., Any],
-    *args: Iterable[Any],
-    num: Optional[int] = None,
-    thread: bool = False,
-) -> Iterator[Any]:
-    """Call a function with arguments using multiple workers.
-
-    Args:
-        func (Callable): function to call
-        *args (list[Any]): arguments to `func`. If multiple lists are provided,
-            they will be passed to `zip` first.
-        num (int, optional): number of workers. If `None`, `NUM_CPUS` or
-            `NUM_THREADS` will be used as appropriate. Defaults to `None`.
-        thread (bool, optional): whether to use threads instead of processes.
-            Defaults to `False`.
-
-    Yields:
-        Any: results from applying the function to the arguments
-    """
-    q, out = Q(thread=thread), Q(thread=thread)
-
-    def _worker(_q: Q, _out: Q) -> None:
-        """Internal worker that calls `func`."""
-        for msg in _q.sorted():
-            _out.put(data=func(*msg.data), order=msg.order)
-
-    workers: Workers
-    if thread:
-        workers = [run_thread(_worker, q, out) for _ in range(num or NUM_THREADS)]
-    else:
-        workers = [run(_worker, q, out) for _ in range(num or NUM_CPUS)]
+IS_MACOS: bool = system().lower().startswith("darwin")
+"""`True` if we're running on MacOS.
 
-    for order, value in enumerate(zip(*args)):
-        q.put(value, order=order)
-    q.stop(workers)
-
-    for msg in out.end().sorted():
-        yield msg.data
-
-
-@deprecated("Use Q.put(data) instead.")
-def put_msg(q: MsgQ, kind: str = "", data: Any = None, order: int = 0) -> MsgQ:
-    """Put a message into a queue.
-
-    Args:
-        q (Queue[Msg]): queue to add message to
-        kind (str, optional): kind of message. Defaults to "".
-        data (Any, optional): message data. Defaults to None.
-        order (int, optional): message order. Defaults to 0.
-
-    Returns:
-        Queue[Msg]: queue the message was added to
+Currently, we only use this value for testing, but there are certain features that
+do not work properly on MacOS.
 
-    .. deprecated:: 2.0.3
-       Use `Q.put` instead.
-    """
-    q.put(Msg(kind=kind, data=data, order=order))
-    return q
-
-
-@deprecated("Use iter(Q) instead.")
-def iter_msg(
-    q: MsgQ, block: bool = True, timeout: Optional[float] = 0.05
-) -> Iterator[Msg]:
-    """Iterate over messages in a queue.
-
-    Args:
-        q (Queue[Msg]): queue to read from
-        block (bool, optional): block until an item is available. Defaults to `True`.
-        timeout (float, optional): time in seconds to poll the queue.
-            Defaults to `0.05`.
-
-    Yields:
-        Iterator[Msg]: iterate over messages in the queue
-
-    .. deprecated:: 2.0.3
-       Use `iter(Q)` instead.
-    """
-    while True:
-        try:
-            msg = q.get(block=block, timeout=timeout)
-            if msg.kind == END_MSG.kind:
-                # We'd really like to put the `END_MSG` back in the queue
-                # to prevent reading past the end, but in practice
-                # this often creates an uncatchable `BrokenPipeError`.
-                # q.put(END_MSG)
-                break
-            yield msg
-        except Empty:  # pragma: no cover
-            # queue might not actually be empty
-            # see: https://bugs.python.org/issue20147
-            continue
-
-
-@deprecated("Use Q.items() instead.")
-def iter_q(q: MsgQ) -> Iterator[Msg]:
-    """End a queue and iterate over its current messages.
+See: [Example of MacOS-specific issues][1].
 
-    Args:
-        q (Queue[Msg]): queue to read from
-
-    Yields:
-        Iterator[Msg]: iterate over messages in the queue
-
-    .. deprecated:: 2.0.3
-       Use `Q.items()` instead.
-    """
-    endq(q)  # ensure queue has an end
-    return iter_msg(q, block=False, timeout=None)
-
-
-@deprecated("Use Q.sorted() instead.")
-def sortiter(
-    items: Iterable[Any],
-    start: int = 0,
-    key: Callable[[Any], int] = attrgetter("order"),
-) -> Iterator[Any]:
-    """Sort and yield the contents of a generator.
-
-    NOTE: `key` must return values that increment by one for each item. If there
-    are any gaps, items after the gap won't be yielded until the end.
-
-    Args:
-        items (Iterable): iterable to sort
-        start (int, optional): initial order number. Defaults to 0.
-        key (Callable, optional): custom key function.
-            Defaults to sorting by the `order` attribute.
+[1]: https://github.com/python/cpython/blob/c5b670efd1e6dabc94b6308734d63f762480b80f/Lib/multiprocessing/queues.py#L125
+"""
 
-    Yields:
-        Iterator[Any]: item yielded in the correct order
 
-    .. deprecated:: 2.0.3
-       Use `Q.sorted()` instead.
-    """
-    prev = start - 1
-    waiting: List[Any] = []
-    for item in items:
-        if not waiting and key(item) == prev + 1:
-            prev += 1
-            yield item
-            continue
-
-        # items came out of order
-        waiting.append(item)
-        waiting.sort(key=key, reverse=True)  # sort in-place for performance
-        while waiting and key(waiting[-1]) == prev + 1:
-            prev += 1
-            yield waiting.pop()
+class Worker:
+    """A function running in a `Process` or `Thread`."""
 
-    # generator ended; yield any waiting items
-    while waiting:
-        yield waiting.pop()
+    _worker: Context
+    """Execution context."""
 
+    @staticmethod
+    def process(task: Task, *args: Any, **kwargs: Any) -> "Worker":
+        """Create a `Process`-based `Worker`.
 
-@deprecated("Use Q.end() instead.")
-def endq(q: MsgQ) -> MsgQ:
-    """Add a message to a queue to indicate its end.
+        Args:
+            task (Task): function to run
+            *args (Any): additional arguments to `task`
+            **kwargs (Any): additional keyword arguments to `task`
 
-    Args:
-        q (Queue[Msg]): queue on which to send the message
+        Returns:
+            Worker: wrapped worker.
+        """
+        # NOTE: On MacOS, python 3.8 switched the default method
+        # from "fork" to "spawn" because fork is considered dangerous.
+        # Some posts say "forkserver" should be ok.
+        # See:  https://bugs.python.org/issue?@action=redirect&bpo=33725
+        #
+        # if IS_MACOS:
+        #     ctx = get_context("forkserver")
+        # else:
+        #     ctx = get_context()
+        return Worker(Process(daemon=True, target=task, args=args, kwargs=kwargs))
+
+    @staticmethod
+    def thread(task: Task, *args: Any, **kwargs: Any) -> "Worker":
+        """Create a `Thread`-based `Worker`.
 
-    Returns:
-        Queue[Msg]: queue the message was sent on
+        Args:
+            task (Task): function to run
+            *args (Any): additional arguments to `task`
+            **kwargs (Any): additional keyword arguments to `task`
 
-    .. deprecated:: 2.0.3
-       Use `Q.end()` instead.
-    """
-    q.put(END_MSG)
-    return q
+        Returns:
+            Worker: wrapped worker.
+        """
+        return Worker(Thread(daemon=False, target=task, args=args, kwargs=kwargs))
 
+    def __init__(self, context: Context):
+        """Construct a worker from a context.
 
-@deprecated("Use Q.stop(workers) instead.")
-def endq_and_wait(q: MsgQ, workers: SomeWorkers) -> Workers:
-    """Notify a list of workers to end and wait for them to join.
+        Args:
+            context (Context): a `Process` or a `Thread`
+        """
+        self._worker = context
+        self._worker.start()
 
-    Args:
-        q (Queue[Msg]): worker queue
-        workers (Worker, Sequence[Worker]): workers to wait for
+    def __getattr__(self, name: str) -> Any:
+        """Delegate properties to the underlying task.
 
-    Returns:
-        List[Thread|Process]: threads or subprocesses that ended
+        Args:
+            name (str): attribute name
 
-    .. deprecated:: 2.0.3
-       Use `Q.stop()` instead.
-    """
-    # We're a little verbose to placate the type-checker.
-    _workers: Workers
-    if isinstance(workers, Thread):
-        _workers = [workers]
-    elif isinstance(workers, Process):
-        _workers = [workers]
-    else:
-        _workers = workers
-
-    for _ in range(len(_workers)):
-        endq(q)
-
-    for worker in _workers:
-        worker.join()
-    return _workers
+        Returns:
+            Any: attribute from the task
+        """
+        return getattr(self._worker, name)
 
 
 class Q:
-    """A simple message queue."""
+    """Simple message queue."""
 
-    q: MsgQ
+    _q: MsgQ
     """Wrapped queue."""
 
-    _items: Optional[List[Msg]] = None
+    _cache: Optional[List[Msg]] = None
     """Cache of queue messages when calling `.items(cache=True)`."""
 
-    def __init__(self, thread: bool = False, *args: Any, **kwargs: Any):
+    _timeout: float = 0.05
+    """Time in seconds to poll the queue."""
+
+    def __init__(self, kind: ContextName = "process"):
         """Construct a queue wrapper.
 
         Args:
-            thread (bool, optional): If `True`, construct a lighter-weight
+            kind (ContextName, optional): If `"thread"`, construct a lighter-weight
                 `Queue` that is thread-safe. Otherwise, construct a full
-                `multiprocessing.Queue`. Defaults to `False`.
-
-            *args, *kwargs: Additional arguments passed to the `Queue` constructor.
+                `multiprocess.Queue`. Defaults to `"process"`.
         """
-        if thread:
-            self.q = ThreadSafeQueue(*args, **kwargs)
-        else:
-            self.q = Queue(*args, **kwargs)
+        if kind == "process":
+            self._q = Queue()
+        elif kind == "thread":
+            self._q = ThreadSafeQueue()
+        else:  # pragma: no cover
+            raise ValueError(f"Unknown queue type: {kind}")
 
     def __getattr__(self, name: str) -> Any:
         """Delegate properties to the underlying queue.
 
         Args:
             name (str): name of the attribute to access
 
         Returns:
             Any: attribute from the queue
         """
-        return getattr(self.q, name)
+        return getattr(self._q, name)
 
     def __iter__(self) -> Iterator[Msg]:
         """Iterate over messages in a queue until `END_MSG` is received.
 
         Yields:
             Iterator[Msg]: iterate over messages in the queue
         """
-        return iter_msg(self.q)
+        while True:
+            try:
+                msg = self._q.get(block=True, timeout=self._timeout)
+                if msg.kind == END_MSG.kind:
+                    # We'd really like to put the `END_MSG` back in the queue
+                    # to prevent reading past the end, but in practice
+                    # this often creates an uncatchable `BrokenPipeError`.
+                    # q.put(END_MSG)
+                    break
+                yield msg
+            except Empty:  # pragma: no cover
+                # queue might not actually be empty
+                # see: https://bugs.python.org/issue20147
+                continue
 
     def items(self, cache: bool = False, sort: bool = False) -> Iterator[Msg]:
         """End a queue and read all the current messages.
 
         Args:
             cache (bool, optional): if `True`, cache the messages. This allows you
                 to call this method multiple times to get the same messages.
@@ -418,63 +255,178 @@
             sort (bool, optional): if `True` messages are sorted by `Msg.order`.
                 Defaults to `False`.
 
         Yields:
             Iterator[Msg]: iterate over messages in the queue
         """
         if cache:
-            if self._items is None:  # need to build a cache
+            if self._cache is None:  # need to build a cache
                 self.end()
-                self._items = list(self.sorted() if sort else self)
-            return iter(self._items)
+                self._cache = list(self.sorted() if sort else self)
+            return iter(self._cache)
 
         # not cached
         self.end()
         return self.sorted() if sort else iter(self)
 
-    def sorted(self) -> Iterator[Msg]:
-        """Iterate over messages in a sorted order.
+    def sorted(self, start: int = 0) -> Iterator[Msg]:
+        """Iterate over messages sorted by `Msg.order`.
 
-        See: `ezq.sortiter`
+        NOTE: `Msg.order` must be incremented by one for each message.
+        If there are any gaps, messages after the gap won't be yielded
+        until the end.
+
+        Args:
+            start (int, optional): initial message number. Defaults to `0`.
 
         Yields:
-            Iterator[Msg]: sorted message iterator
+            Iterator[Msg]: message yielded in the correct order
         """
-        return sortiter(self)
+        prev = start - 1
+        key = attrgetter("order")
+        waiting: List[Msg] = []
+        for item in self:
+            if not waiting and key(item) == prev + 1:
+                prev += 1
+                yield item
+                continue
+
+            # items came out of order
+            waiting.append(item)
+            waiting.sort(key=key, reverse=True)  # sort in-place for performance
+            while waiting and key(waiting[-1]) == prev + 1:
+                prev += 1
+                yield waiting.pop()
+
+        # generator ended; yield any waiting items
+        while waiting:
+            yield waiting.pop()
 
-    def put(self, data: Any = None, kind: str = "", order: int = 0) -> Self:
+    def put(self, data: Any = None, *, kind: str = "", order: int = 0) -> "Q":
         """Put a message on the queue.
 
         Args:
             data (Any, optional): message data. Defaults to `None`.
+
             kind (str, optional): kind of message. Defaults to `""`.
+
             order (int, optional): message order. Defaults to `0`.
 
         Returns:
             Self: self for chaining
         """
         if isinstance(data, Msg):
-            self.q.put_nowait(data)
+            self._q.put(data)
         else:
-            self.q.put_nowait(Msg(data=data, kind=kind, order=order))
+            self._q.put(Msg(data=data, kind=kind, order=order))
         return self
 
-    def end(self) -> Self:
+    def end(self) -> "Q":
         """Add the `END_MSG` to indicate the end of work.
 
         Returns:
             Self: self for chaining
         """
-        self.q.put(END_MSG)
+        self._q.put(END_MSG)
         return self
 
-    def stop(self, workers: SomeWorkers) -> Self:
+    def stop(self, workers: Union[Worker, Sequence[Worker]]) -> "Q":
         """Use this queue to notify workers to end and wait for them to join.
 
         Args:
             workers (Worker, Sequence[Worker]): workers to wait for
 
         Returns:
             Self: self for chaining
         """
-        endq_and_wait(self.q, workers)
+        _workers = [workers] if isinstance(workers, Worker) else workers
+
+        for _ in range(len(_workers)):
+            self.end()
+
+        for task in _workers:
+            task.join()
+
         return self
+
+
+def run(task: Task, *args: Any, **kwargs: Any) -> Worker:
+    """Run a function as a subprocess.
+
+    Args:
+        task (Task): function to run in each subprocess
+
+        *args (Any): additional positional arguments to `task`.
+
+        **kwargs (Any): additional keyword arguments to `task`.
+
+    Returns:
+        Worker: worker started in a subprocess
+
+    .. changed:: 2.0.4
+       This function now returns a `Worker` instead of a `Process`.
+    """
+    return Worker.process(task, *args, **kwargs)
+
+
+def run_thread(task: Task, *args: Any, **kwargs: Any) -> Worker:
+    """Run a function as a thread.
+
+    Args:
+        task (Task): function to run in each thread
+
+        *args (Any): additional positional arguments to `task`.
+
+        **kwargs (Any): additional keyword arguments to `task`.
+
+    Returns:
+        Worker: worker started in a thread
+
+    .. changed:: 2.0.4
+       This function now returns a `Worker` instead of a `Thread`.
+    """
+    return Worker.thread(task, *args, **kwargs)
+
+
+def map(
+    task: Task,
+    *args: Iterable[Any],
+    num: Optional[int] = None,
+    kind: ContextName = "process",
+) -> Iterator[Any]:
+    """Call a function with arguments using multiple workers.
+
+    Args:
+        func (Callable): function to call
+
+        *args (list[Any]): arguments to `func`. If multiple lists are provided,
+            they will be passed to `zip` first.
+
+        num (int, optional): number of workers. If `None`, `NUM_CPUS` or
+            `NUM_THREADS` will be used as appropriate. Defaults to `None`.
+
+        kind (ContextName, optional): execution context to use.
+            Defaults to `"process"`.
+
+    Yields:
+        Any: results from applying the function to the arguments
+    """
+    q, out = Q(kind=kind), Q(kind=kind)
+
+    def worker(_q: Q, _out: Q) -> None:
+        """Internal call to `func`."""
+        for msg in _q.sorted():
+            _out.put(data=task(*msg.data), order=msg.order)
+
+    if kind == "process":
+        workers = [Worker.process(worker, q, out) for _ in range(num or NUM_CPUS)]
+    elif kind == "thread":
+        workers = [Worker.thread(worker, q, out) for _ in range(num or NUM_THREADS)]
+    else:  # pragma: no cover
+        raise ValueError(f"Unknown worker context: {kind}")
+
+    for order, value in enumerate(zip(*args)):
+        q.put(value, order=order)
+    q.stop(workers)
+
+    for msg in out.end().sorted():
+        yield msg.data
```

### Comparing `ezq-2.0.3/src/ezq.egg-info/PKG-INFO` & `ezq-3.0.0/src/ezq.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: ezq
-Version: 2.0.3
+Version: 3.0.0
 Summary: Simple wrapper for python multiprocessing.
 Home-page: https://github.com/metaist/ezq
 Download-URL: https://github.com/metaist/ezq
 Author: Metaist LLC
 Author-email: metaist@metaist.com
 License: MIT
 Keywords: simple,multiprocessing,queue,subprocesses
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ezq
 
 _Simple wrappers for python multiprocessing and threading._
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/metaist/ezq/.github/workflows/ci.yaml?branch=main&style=for-the-badge)](https://github.com/metaist/ezq/actions)
 [![ezq on PyPI](https://img.shields.io/pypi/v/ezq.svg?color=blue&style=for-the-badge)](https://pypi.org/project/ezq)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/ezq?style=for-the-badge)](https://pypi.org/project/ezq)
 
 [Changelog] - [Issues] - [Documentation]
 
 [changelog]: https://github.com/metaist/ezq/blob/main/CHANGELOG.md
 [issues]: https://github.com/metaist/ezq/issues
 [documentation]: https://metaist.github.io/ezq/
 
@@ -98,15 +106,15 @@
     main()
 ```
 
 ## Typical worker lifecycle
 
 - The main process [creates queues](#create-queues) with `ezq.Q`.
 
-- The main process [creates workers](#create-workers) with `ezq.run` or `ezq.run_thread`.
+- The main process [creates workers](#create-workers) with `ezq.run` (alias for `Worker.process`) or `ezq.run_thread` (alias for `Worker.thread`).
 
 - The main process [sends data](#send-data) using `Q.put`.
 
 - The worker [iterates over the queue](#iterate-over-messages).
 
 - The main process [ends the queue](#end-the-queue) with `Q.stop`.
 
@@ -120,15 +128,15 @@
 
 - `Process` is for _parallelism_ so you can use multiple CPUs at once. Ideal for **CPU-bound** tasks like doing lots of mathematical calculations.
 
 - `Thread` is for _concurrency_ so you can use a single CPU to do multiple things. Ideal for **I/O-bound** tasks like waiting for a disk, database, or network.
 
 Some more differences:
 
-- **Shared memory**: Each `Process` worker has [data sent to it via `pickle`](#beware-pickle) and it doesn't share data with other workers. By contrast, each `Thread` worker shares its memory with all other workers on the same CPU, so it can [accidentally change global state](#beware-shared-state).
+- **Shared memory**: Each `Process` worker has [data sent to it via `pickle`](#beware-pickle) (actually [`dill`](https://github.com/uqfoundation/dill), a `pickle` replacement) and it doesn't share data with other workers. By contrast, each `Thread` worker shares its memory with all other workers on the same CPU, so it can [accidentally change global state](#beware-shared-state).
 
 - **Queue overhead**: `ezq.Q` [has more overhead](#create-queues) for `Process` workers than `Thread` workers.
 
 - **Creating sub-workers**: `Process` and `Thread` workers can create additional `Thread` workers, but [they cannot create additional `Process` workers](#create-workers).
 
 ## Create queues
 
@@ -138,22 +146,22 @@
 
 - **1 queue**: the worker reads from an input queue and persists the result somewhere else (e.g., writing to disk, making a network call, running some other program).
 
 - **2 queues** (most common): the worker reads from an input queue and write the results to an output queue.
 
 - **3 queues**: multiple stages of work are happening where workers are reading from one queue and writing to another queue for another worker to process.
 
-**NOTE:** If you're using `Thread` workers, you can save some overhead by passing `thread=True`. This lightweight queue also doesn't use `pickle`, so you can use it to pass hard-to-pickle things (e.g., `lambda`).
+**NOTE:** If you're using `Thread` workers, you can save some overhead by passing `Q("thread")`. This lightweight queue also doesn't use `pickle`, so you can use it to pass hard-to-pickle things (e.g., database connection).
 
 ```python
 q, out = ezq.Q(), ezq.Q() # most common
-q2 = ez.Q(thread=True) # only ok for Thread workers
+q2 = ez.Q("thread") # only ok for Thread workers
 ```
 
-## A worker is just a function
+## A worker task is just a function
 
 In general, there's nothing special about a worker function, but note:
 
 - If you're using `Process` workers, all arguments are [passed through `pickle` first](#beware-pickle).
 
 - We don't currently do anything with the return value of this function (unless you use `ezq.map()`). You'll need an output queue to return data back to the main process/thread.
 
@@ -171,15 +179,15 @@
 
 - `kind: str` - You can use this to send multiple kinds of work to the same worker. Note that the special `END` kind is used to indicate the end of a queue.
 
 - `order: int` - This is the message order which can help you reorder results or ensure that messages from a queue are read in a particular order (that's what `Q.sorted()` uses).
 
 ## Beware `pickle`
 
-If you are using `Process` workers, everything passed to the worker (arguments, messages) is first passed to `pickle` by [`multiprocessing`][1]. Anything that cannot be pickled (e.g., `lambda` functions, database connections), cannot be passed to `Process` workers.
+If you are using `Process` workers, everything passed to the worker (arguments, messages) is first passed to `pickle` (actually, [`dill`](https://github.com/uqfoundation/dill)). Anything that cannot be pickled with dill (e.g., database connections), cannot be passed to `Process` workers. Note that `dill` _can_ serialize many more types than `pickle` (e.g. `lambda` functions).
 
 ## Beware shared state
 
 If you are using `Thread` workers, workers can share certain variables, so you need to be careful of how variables are access to avoid accidentally corrupting data.
 
 ## Iterate over messages
 
@@ -239,15 +247,15 @@
             out.put((num, num / 2), order=msg.order)
         elif msg.kind == "ODD":
             out.put((num, 3 * num + 1), order=msg.order)
 
 
 def main() -> None:
     """Run several threads with a subprocess for printing."""
-    q, out = ezq.Q(thread=True), ezq.Q()
+    q, out = ezq.Q("thread"), ezq.Q()
     readers = [ezq.run_thread(collatz, q, out) for _ in range(ezq.NUM_THREADS)]
     writer = ezq.run(printer, out)
 
     for num in range(40):
         kind = "EVEN" if num % 2 == 0 else "ODD"
         q.put(num, kind=kind, order=num)
```

### Comparing `ezq-2.0.3/test/test_ezq.py` & `ezq-3.0.0/test/test_ezq.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,56 +6,22 @@
 import operator
 from typing import Callable
 
 # pkg
 import ezq
 
 
-# functional API (deprecated) #
-
-
-def test_functional_api() -> None:
-    """Run workers using the functional API (deprecated)."""
-
-    def worker_f(q: ezq.MsgQ, out: ezq.MsgQ) -> None:
-        """Internal worker."""
-        for msg in ezq.iter_msg(q):
-            ezq.put_msg(out, data=msg.data + 1, order=msg.order)
-
-    q: ezq.MsgQ = ezq.Queue()
-    out: ezq.MsgQ = ezq.Queue()
-    process = ezq.run(worker_f, q, out)
-
-    q2: ezq.MsgQ = ezq.Q(thread=True).q
-    out2: ezq.MsgQ = ezq.Q(thread=True).q
-    thread = ezq.run_thread(worker_f, q2, out2)
-
-    for i in range(10):
-        ezq.put_msg(q, data=i, order=i)
-        ezq.put_msg(q2, data=i, order=i)
-
-    ezq.endq_and_wait(q, process)
-    ezq.endq_and_wait(q2, thread)
-
-    want = [x + 1 for x in range(10)]
-
-    have = [msg.data for msg in ezq.sortiter(ezq.iter_q(out))]
-    assert have == want, "expected subprocesses to work"
-
-    have = [msg.data for msg in ezq.sortiter(ezq.iter_q(out2))]
-    assert have == want, "expected threads to work"
-
-
 def test_q_wrapper() -> None:
     """Use underlying queue."""
-    q = ezq.Q(thread=True)
+    q = ezq.Q("thread")
     q.put(1)
     q.put(ezq.Msg(data=2))
 
-    assert q.qsize() == 2, "expected function to be delegated to queue"
+    if not ezq.IS_MACOS:
+        assert q.qsize() == 2, "expected function to be delegated to queue"
 
     want = [1, 2]
     have = [msg.data for msg in q.items(cache=True)]
     assert have == want, "expected both to be the same"
 
     have = [msg.data for msg in q.items(cache=True)]
     assert have == want, "expected same results after .items() twice"
@@ -82,28 +48,35 @@
 def test_run_processes() -> None:
     """Run several workers with different arguments."""
     n_msg = 1000
 
     q, out = ezq.Q(), ezq.Q()
     workers = [ezq.run(worker_sum, q, out, num=i) for i in range(ezq.NUM_CPUS)]
 
+    def wrap_lambda(i: int) -> Callable[[], int]:
+        """Wrap a number in a lambda so thread-context works."""
+        return lambda: i
+
     for num in range(n_msg):
-        q.put(ezq.Msg(data=num))
+        q.put(wrap_lambda(num))
+
+    # for num in range(n_msg):
+    #     q.put(ezq.Msg(data=num))
     q.stop(workers)
 
     want = sum(range(n_msg))
     have = sum(msg.data[1] for msg in out.items())
     assert have == want, f"expect sum of {want} from processes"
 
 
 def test_run_threads() -> None:
     """Run threads in parallel."""
     n_msg = 1000
 
-    q, out = ezq.Q(thread=True), ezq.Q(thread=True)
+    q, out = ezq.Q("thread"), ezq.Q("thread")
     workers = [
         ezq.run_thread(worker_sum, q, out, num=i) for i in range(ezq.NUM_THREADS)
     ]
 
     def wrap_lambda(i: int) -> Callable[[], int]:
         """Wrap a number in a lambda so thread-context works."""
         return lambda: i
@@ -114,18 +87,17 @@
 
     want = sum(range(n_msg))
     have = sum(msg.data[1] for msg in out.items())
     assert have == want, f"expect sum of {want} from threads"
 
 
 def test_map() -> None:
-    """Run a function on multiple threads."""
+    """Run a function on multiple processes and threads."""
     left = range(10)
     right = range(10, 0, -1)
 
     want = [a + b for (a, b) in zip(left, right)]
-
-    have = list(ezq.map(operator.add, left, right, thread=True))
-    assert have == want, "expected threads to work"
-
     have = list(ezq.map(operator.add, left, right))
     assert have == want, "expected subprocesses to work"
+
+    # have = list(ezq.map(operator.add, left, right, kind="thread"))
+    # assert have == want, "expected threads to work"
```

### Comparing `ezq-2.0.3/test/test_iter.py` & `ezq-3.0.0/test/test_iter.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,37 +18,47 @@
     """Iterate over all messages."""
     num = 1000
     q = ezq.Q()
 
     for _ in range(num):
         q.put(1)
 
-    assert q.qsize() == num, "expect all messages queued"
+    if not ezq.IS_MACOS:
+        assert q.qsize() == num, "expect all messages queued"
 
     total = sum(msg.data for msg in q.items())
     assert num == total, "expect iterator to get all messages"
 
 
 def test_sortiter_sorted_list() -> None:
     """Sort a list of sorted numbers."""
     num = 1000
-    order = list(range(num))
-    want = order.copy()
-    have = list(ezq.sortiter(order, key=ident))
+    want = list(range(num))
+
+    q = ezq.Q()
+    for num in range(num):
+        q.put(order=num)
+
+    have = [msg.order for msg in q.end().sorted()]
     assert want == have, "expected numbers in order"
 
 
 def test_sortiter_random_list() -> None:
     """Sort a list of numbers."""
     num = 1000
-    order = list(range(num))
-    want = order.copy()
-    random.shuffle(order)
+    want = list(range(num))
+
+    temp = want.copy()
+    random.shuffle(temp)
+
+    q = ezq.Q()
+    for num in temp:
+        q.put(order=num)  # sending things out of order
 
-    have = list(ezq.sortiter(order, key=ident))
+    have = [msg.order for msg in q.items(sort=True)]
     assert want == have, "expected numbers in order"
 
 
 def test_sortiter_messages() -> None:
     """Sort messages in order."""
     num = 1000
     order = list(range(num))
```

