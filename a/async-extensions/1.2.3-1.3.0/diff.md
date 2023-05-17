# Comparing `tmp/async_extensions-1.2.3.tar.gz` & `tmp/async_extensions-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_extensions-1.2.3.tar", max compression
+gzip compressed data, was "async_extensions-1.3.0.tar", max compression
```

## Comparing `async_extensions-1.2.3.tar` & `async_extensions-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1092 2023-05-07 12:20:20.359473 async_extensions-1.2.3/LICENSE
--rw-r--r--   0        0        0     2578 2023-05-07 12:20:20.359473 async_extensions-1.2.3/README.md
--rw-r--r--   0        0        0     2888 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/__init__.py
--rw-r--r--   0        0        0      732 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/blocking.py
--rw-r--r--   0        0        0      431 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/cancel.py
--rw-r--r--   0        0        0     1174 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/channel.py
--rw-r--r--   0        0        0     1781 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/close.py
--rw-r--r--   0        0        0     7840 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/collect.py
--rw-r--r--   0        0        0      118 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/constants.py
--rw-r--r--   0        0        0       80 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/current.py
--rw-r--r--   0        0        0       88 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/errors.py
--rw-r--r--   0        0        0      101 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/file.py
--rw-r--r--   0        0        0      174 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/low_level.py
--rw-r--r--   0        0        0       44 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/path.py
--rw-r--r--   0        0        0       87 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/process.py
--rw-r--r--   0        0        0        0 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/py.typed
--rw-r--r--   0        0        0      385 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/run.py
--rw-r--r--   0        0        0       76 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/signal.py
--rw-r--r--   0        0        0       77 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/sleep.py
--rw-r--r--   0        0        0     1333 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/standard.py
--rw-r--r--   0        0        0      143 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/synchronization.py
--rw-r--r--   0        0        0       70 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/task_group.py
--rw-r--r--   0        0        0      176 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/types.py
--rw-r--r--   0        0        0      859 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/typing.py
--rw-r--r--   0        0        0      732 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/wait.py
--rw-r--r--   0        0        0     2230 2023-05-07 12:20:20.363473 async_extensions-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 async_extensions-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-17 22:52:57.634115 async_extensions-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2578 2023-05-17 22:52:57.634115 async_extensions-1.3.0/README.md
+-rw-r--r--   0        0        0     2968 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/__init__.py
+-rw-r--r--   0        0        0      732 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/blocking.py
+-rw-r--r--   0        0        0      431 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/cancel.py
+-rw-r--r--   0        0        0     1174 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/channel.py
+-rw-r--r--   0        0        0     1581 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/close.py
+-rw-r--r--   0        0        0     7825 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/collect.py
+-rw-r--r--   0        0        0      118 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/constants.py
+-rw-r--r--   0        0        0       80 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/current.py
+-rw-r--r--   0        0        0       88 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/errors.py
+-rw-r--r--   0        0        0      101 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/file.py
+-rw-r--r--   0        0        0      174 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/low_level.py
+-rw-r--r--   0        0        0       44 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/path.py
+-rw-r--r--   0        0        0       87 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/process.py
+-rw-r--r--   0        0        0        0 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/py.typed
+-rw-r--r--   0        0        0      396 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/run.py
+-rw-r--r--   0        0        0       76 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/signal.py
+-rw-r--r--   0        0        0       77 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/sleep.py
+-rw-r--r--   0        0        0     1327 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/standard.py
+-rw-r--r--   0        0        0      143 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/synchronization.py
+-rw-r--r--   0        0        0      253 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/task_group.py
+-rw-r--r--   0        0        0      176 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/types.py
+-rw-r--r--   0        0        0      617 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/typing.py
+-rw-r--r--   0        0        0      732 2023-05-17 22:52:57.634115 async_extensions-1.3.0/async_extensions/wait.py
+-rw-r--r--   0        0        0     2438 2023-05-17 22:52:57.634115 async_extensions-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 async_extensions-1.3.0/PKG-INFO
```

### Comparing `async_extensions-1.2.3/LICENSE` & `async_extensions-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.3/README.md` & `async_extensions-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.2.3"
+async-extensions = "^1.3.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

### Comparing `async_extensions-1.2.3/async_extensions/__init__.py` & `async_extensions-1.3.0/async_extensions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,41 +2,53 @@
 
 __description__ = "Asynchronous extensions."
 __url__ = "https://github.com/nekitdev/async-extensions"
 
 __title__ = "async_extensions"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.2.3"
+__version__ = "1.3.0"
 
 from async_extensions.blocking import run_blocking_in_process, run_blocking_in_thread
 from async_extensions.cancel import CancelScope, create_cancel_scope, shield
 from async_extensions.channel import (
-    MemoryChannel, MemoryChannelFactory, MemoryReceiveChannel, MemorySendChannel
+    MemoryChannel,
+    MemoryChannelFactory,
+    MemoryReceiveChannel,
+    MemorySendChannel,
 )
 from async_extensions.close import (
-    AsyncCloseable, AsyncClosing, async_close, async_close_forcefully, async_closing
+    AsyncCloseable,
+    AsyncClosing,
+    async_close,
+    async_close_forcefully,
+    async_closing,
 )
 from async_extensions.collect import (
-    collect, collect_iterable, collect_iterable_results, collect_results
+    collect,
+    collect_iterable,
+    collect_iterable_results,
+    collect_results,
 )
 from async_extensions.current import current_async_library
 from async_extensions.errors import AsyncLibraryNotFoundError
 from async_extensions.file import AsyncFile, open_file, wrap_file
 from async_extensions.low_level import (
-    cancel_shielded_checkpoint, checkpoint, checkpoint_if_cancelled
+    cancel_shielded_checkpoint,
+    checkpoint,
+    checkpoint_if_cancelled,
 )
 from async_extensions.path import Path
 from async_extensions.process import open_process, run_process
 from async_extensions.run import run
 from async_extensions.signal import open_signal_receiver
 from async_extensions.sleep import sleep, sleep_forever
 from async_extensions.standard import async_iter, async_next, iter_to_async_iter
 from async_extensions.synchronization import CapacityLimiter, Condition, Event, Lock, Semaphore
-from async_extensions.task_group import create_task_group
+from async_extensions.task_group import TaskGroup, create_task_group
 from async_extensions.wait import fail_after, move_on_after, wait_for, wait_for_or_else
 
 __all__ = (
     # blocking
     "run_blocking_in_process",
     "run_blocking_in_thread",
     # cancel
@@ -90,14 +102,15 @@
     # synchronization
     "CapacityLimiter",
     "Condition",
     "Event",
     "Lock",
     "Semaphore",
     # task group
+    "TaskGroup",
     "create_task_group",
     # wait
     "fail_after",
     "move_on_after",
     "wait_for",
     "wait_for_or_else",
 )
```

### Comparing `async_extensions-1.2.3/async_extensions/blocking.py` & `async_extensions-1.3.0/async_extensions/blocking.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.3/async_extensions/channel.py` & `async_extensions-1.3.0/async_extensions/channel.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.3/async_extensions/collect.py` & `async_extensions-1.3.0/async_extensions/collect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-from typing import (
-    Any, AsyncIterable, AsyncIterator, Awaitable, List, Tuple, TypeVar, Union, overload
-)
+from typing import Any, AsyncIterable, AsyncIterator, Awaitable, List, Tuple, TypeVar, overload
+
+from funcs.typing import AnyError, DynamicTuple, EmptyTuple
+from wraps.result import Error, Ok, Result
 
 from async_extensions.standard import iter_to_async_iter
 from async_extensions.task_group import create_task_group
-from async_extensions.typing import (
-    AnyException, AnyIterable, DynamicTuple, EmptyTuple, is_async_iterable, is_error, is_iterable
-)
+from async_extensions.typing import AnyIterable, is_async_iterable, is_iterable
 
 __all__ = ("collect", "collect_results", "collect_iterable", "collect_iterable_results")
 
 T = TypeVar("T")
-ET = TypeVar("ET", bound=AnyException)
+ErrorT = TypeVar("ErrorT", bound=AnyError)
 
 
-Result = Union[T, ET]
-TaggedResult = Tuple[int, Result[T, ET]]
+TaggedResult = Tuple[int, Result[T, ErrorT]]
 
-AnyTaggedResult = TaggedResult[T, AnyException]
-AnyResult = Result[T, AnyException]
+AnyTaggedResult = TaggedResult[T, AnyError]
+AnyResult = Result[T, AnyError]
 
 
 async def append_tagged_result(
     awaitable: Awaitable[T],
     tag: int,
     results: List[AnyTaggedResult[T]],
 ) -> None:
     result: AnyResult[T]
 
     try:
-        result = await awaitable
+        result = Ok(await awaitable)
 
-    except AnyException as error:
-        result = error
+    except AnyError as error:
+        result = Error(error)
 
     results.append((tag, result))
 
 
 def by_tag(tagged_result: AnyTaggedResult[Any]) -> int:
     tag, _ = tagged_result
 
     return tag
 
 
-def result(tagged_result: TaggedResult[T, ET]) -> Result[T, ET]:
+def result(tagged_result: TaggedResult[T, ErrorT]) -> Result[T, ErrorT]:
     _, result = tagged_result
 
     return result
 
 
 A = TypeVar("A")
 B = TypeVar("B")
@@ -108,17 +106,15 @@
 async def collect_results(
     __awaitable_a: Awaitable[A],
     __awaitable_b: Awaitable[B],
     __awaitable_c: Awaitable[C],
     __awaitable_d: Awaitable[D],
     __awaitable_e: Awaitable[E],
     __awaitable_f: Awaitable[F],
-) -> Tuple[
-    AnyResult[A], AnyResult[B], AnyResult[C], AnyResult[D], AnyResult[E], AnyResult[F]
-]:
+) -> Tuple[AnyResult[A], AnyResult[B], AnyResult[C], AnyResult[D], AnyResult[E], AnyResult[F]]:
     ...
 
 
 @overload
 async def collect_results(
     __awaitable_a: Awaitable[A],
     __awaitable_b: Awaitable[B],
@@ -168,28 +164,29 @@
     __awaitable_b: Awaitable[Any],
     __awaitable_c: Awaitable[Any],
     __awaitable_d: Awaitable[Any],
     __awaitable_e: Awaitable[Any],
     __awaitable_f: Awaitable[Any],
     __awaitable_g: Awaitable[Any],
     __awaitable_h: Awaitable[Any],
+    __awaitable_n: Awaitable[Any],
     *awaitables: Awaitable[Any],
 ) -> DynamicTuple[AnyResult[Any]]:
     ...
 
 
 async def collect_results(*awaitables: Awaitable[Any]) -> DynamicTuple[AnyResult[Any]]:
     return tuple(await collect_iterable_results(awaitables))
 
 
 NOT_ANY_ITERABLE = "{} is neither an async iterable, nor an iterable"
 
 
 async def tag_awaitables(
-    awaitables: AsyncIterable[Awaitable[T]]
+    awaitables: AsyncIterable[Awaitable[T]],
 ) -> AsyncIterator[Tuple[int, Awaitable[T]]]:
     tag = 0
 
     async for awaitable in awaitables:
         yield (tag, awaitable)
 
         tag += 1
@@ -216,35 +213,26 @@
             task_group.start_soon(append_tagged_result, awaitable, tag, results)
 
     results.sort(key=by_tag)
 
     return list(map(result, results))  # type: ignore
 
 
-def unwrap_error(result: AnyResult[T]) -> T:
-    if is_error(result):
-        raise result
-
-    return result  # type: ignore
-
-
 @overload
 async def collect() -> EmptyTuple:
     ...  # pragma: overload
 
 
 @overload
 async def collect(__awaitable_a: Awaitable[A]) -> Tuple[A]:
     ...  # pragma: overload
 
 
 @overload
-async def collect(
-    __awaitable_a: Awaitable[A], __awaitable_b: Awaitable[B]
-) -> Tuple[A, B]:
+async def collect(__awaitable_a: Awaitable[A], __awaitable_b: Awaitable[B]) -> Tuple[A, B]:
     ...  # pragma: overload
 
 
 @overload
 async def collect(
     __awaitable_a: Awaitable[A], __awaitable_b: Awaitable[B], __awaitable_c: Awaitable[C]
 ) -> Tuple[A, B, C]:
@@ -327,8 +315,12 @@
 
 
 async def collect(*awaitables: Awaitable[Any]) -> DynamicTuple[Any]:
     return tuple(await collect_iterable(awaitables))
 
 
 async def collect_iterable(iterable: AnyIterable[Awaitable[T]]) -> List[T]:
-    return list(map(unwrap_error, await collect_iterable_results(iterable)))
+    return list(map(raising, await collect_iterable_results(iterable)))
+
+
+def raising(result: AnyResult[T]) -> T:
+    return result.raising()
```

### Comparing `async_extensions-1.2.3/async_extensions/standard.py` & `async_extensions-1.3.0/async_extensions/standard.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 
 
 @overload
 async def async_next(async_iterator: AsyncIterator[T], default: U) -> Union[T, U]:
     ...
 
 
-async def async_next(
-    async_iterator: AsyncIterator[Any], default: Any = no_default
-) -> Any:
+async def async_next(async_iterator: AsyncIterator[Any], default: Any = no_default) -> Any:
     if is_instance(async_iterator, AsyncIterator):
         try:
             return await async_iterator.__anext__()
 
         except StopAsyncIteration:
             if default is no_default:
                 raise
```

### Comparing `async_extensions-1.2.3/async_extensions/wait.py` & `async_extensions-1.3.0/async_extensions/wait.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.3/pyproject.toml` & `async_extensions-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-extensions"
-version = "1.2.3"
+version = "1.3.0"
 description = "Asynchronous extensions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/async-extensions"
@@ -27,38 +27,50 @@
 
 [[tool.poetry.packages]]
 include = "async_extensions"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
+attrs = ">= 23.1.0"
+
 anyio = ">= 3.6.2"
 solus = ">= 1.1.0"
+funcs = ">= 0.5.1"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
 black = "23.3.0"
+flake8-pyproject = "1.2.3"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.11.5"
+version = "5.12.0"
+python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "1.1.1"
+mypy = "1.3.0"
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.1.0"
+changelogging = "1.2.0"
 
 [tool.black]
 line_length = 100
 
+[tool.flake8]
+max_line_length = 100
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.mypy]
 show_column_numbers = true
 
@@ -82,15 +94,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "async-extensions"
-version = "1.2.3"
+version = "1.3.0"
 url = "https://github.com/nekitdev/async-extensions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `async_extensions-1.2.3/PKG-INFO` & `async_extensions-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-extensions
-Version: 1.2.3
+Version: 1.3.0
 Summary: Asynchronous extensions.
 Home-page: https://github.com/nekitdev/async-extensions
 License: MIT
 Keywords: python,async,extensions
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: anyio (>=3.6.2)
+Requires-Dist: attrs (>=23.1.0)
+Requires-Dist: funcs (>=0.5.1)
 Requires-Dist: solus (>=1.1.0)
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/solus/issues
 Project-URL: Repository, https://github.com/nekitdev/async-extensions
 Description-Content-Type: text/markdown
 
@@ -65,15 +67,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.2.3"
+async-extensions = "^1.3.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

