# Comparing `tmp/checkpoint_tool-0.7.6.tar.gz` & `tmp/checkpoint_tool-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.7.6.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.7.7.tar", max compression
```

## Comparing `checkpoint_tool-0.7.6.tar` & `checkpoint_tool-0.7.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7199 2023-05-18 00:40:34.124837 checkpoint_tool-0.7.6/README.md
--rw-r--r--   0        0        0      608 2023-05-09 01:50:05.066517 checkpoint_tool-0.7.6/checkpoint/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-09 01:19:11.117797 checkpoint_tool-0.7.6/checkpoint/app.py
--rw-r--r--   0        0        0     4004 2023-05-03 13:31:12.624944 checkpoint_tool-0.7.6/checkpoint/database.py
--rw-r--r--   0        0        0     7243 2023-05-18 04:16:07.403508 checkpoint_tool-0.7.6/checkpoint/graph.py
--rw-r--r--   0        0        0    10986 2023-05-18 04:15:50.488265 checkpoint_tool-0.7.6/checkpoint/task.py
--rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 checkpoint_tool-0.7.6/checkpoint/types.py
--rw-r--r--   0        0        0      677 2023-05-18 04:18:59.185017 checkpoint_tool-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     8004 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     7248 2023-05-18 16:17:30.843008 checkpoint_tool-0.7.7/README.md
+-rw-r--r--   0        0        0      608 2023-05-09 01:50:05.066517 checkpoint_tool-0.7.7/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2514 2023-05-18 16:34:53.180387 checkpoint_tool-0.7.7/checkpoint/app.py
+-rw-r--r--   0        0        0     4517 2023-05-18 16:13:03.919978 checkpoint_tool-0.7.7/checkpoint/database.py
+-rw-r--r--   0        0        0     7245 2023-05-18 16:35:39.947857 checkpoint_tool-0.7.7/checkpoint/graph.py
+-rw-r--r--   0        0        0    11335 2023-05-18 17:02:34.386785 checkpoint_tool-0.7.7/checkpoint/task.py
+-rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 checkpoint_tool-0.7.7/checkpoint/types.py
+-rw-r--r--   0        0        0      677 2023-05-18 16:21:55.175049 checkpoint_tool-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     8053 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.7/PKG-INFO
```

### Comparing `checkpoint_tool-0.7.6/README.md` & `checkpoint_tool-0.7.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -159,18 +159,19 @@
     def build_task(self, task_dict: dict[str, Task[float]]):
         self.scores = task_dict
 
     def run_task(self) -> float:
         return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
 
-The output of the `main` method should be serializable with `cloudpickle`.
-Large outputs can be stored with compression via `zlib`:
+The output of the `run_task` method should be serializable with `cloudpickle`,
+which is then compressed with `gzip`.
+The compression level can be changed as follows (defaults to 9).
 ```python
-class LargeOutputTask(Task, compress_level=-1):
+class LargeOutputTask(Task, compress_level=0):
     ...
 ```
 
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
@@ -217,15 +218,15 @@
 
 # Task-level concurrency control
 SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_name: 1})
 
 ```
 
 ### Commandline tool
-We can use checkpoint-tool from commandline like `python -m checkpoint.app path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
+We can use checkpoint-tool from commandline like `python -m checkpoint.app path/to/taskfile.py`, where `taskfile.py` defines the `Main` task as follows:
 ```python
 # taskfile.py
 
 class Main(Task):
     ...
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
```

### Comparing `checkpoint_tool-0.7.6/checkpoint/__init__.py` & `checkpoint_tool-0.7.7/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.6/checkpoint/app.py` & `checkpoint_tool-0.7.7/checkpoint/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 from __future__ import annotations
 from typing import Any
 from pathlib import Path
 import sys
 import json
 import pprint
+import logging
+import io
 
 import click
 
 from .types import Context
 from .task import TaskType
 
 
+LOGGER = logging.getLogger(__name__)
+
+
 @click.command
 @click.argument('taskfile', type=Path)
 @click.option('-e', '--entrypoint', default='Main', help='Task name for entrypoint.')
 @click.option('-t', '--exec-type', type=click.Choice(['process', 'thread']), default='process')
 @click.option('-w', '--max-workers', type=int, default=-1)
 @click.option('--cache-dir', type=Path, default=None)
 @click.option('--rate-limits', type=json.loads, default=None, help='JSON dictionary for rate_limits.')
 @click.option('-D', '--detect-source-change', is_flag=True, help='Automatically discard the cache per task once the source code (AST) is changed.')
 @click.option('--dont-force-entrypoint', is_flag=True, help='Do nothing if the cache of the entripoint task is up-to-date.')
+@click.option('-l', '--loglevel', type=click.Choice(['debug', 'info', 'warning', 'error']), default='warning')
 def main(taskfile: Path,
          entrypoint: str,
          exec_type: str,
          max_workers: int,
          cache_dir: Path | None,
          rate_limits: dict[str, Any] | None,
          detect_source_change: bool,
-         dont_force_entrypoint: bool
+         dont_force_entrypoint: bool,
+         loglevel: str,
          ) -> int:
-    # Set arguments as environment variables
-    # os.environ['CP_EXECUTOR'] = exec_type
-    # os.environ['CP_MAX_WORKERS'] = str(max_workers)
-    # os.environ['CP_CACHE_DIR'] = str(taskfile.parent / '.cache') if cache_dir is None else str(cache_dir)
-    # os.environ['CP_DETECT_SOURCE_CHANGE'] = str(int(detect_source_change))
+    logging.basicConfig(level=getattr(logging, loglevel.upper()))
+
     Context.executor_name = exec_type
     Context.max_workers = max_workers
     Context.cache_dir = taskfile.parent / '.cache' if cache_dir is None else cache_dir
     Context.detect_source_change = detect_source_change
 
     # Run script as module
     module_name = taskfile.with_suffix('').name
     sys.path.append(str(taskfile.parent))
     module = __import__(module_name)
-    # import importlib.util
-    # spec = importlib.util.spec_from_file_location(module_name, taskfile)
-    # assert spec is not None
-    # assert spec.loader is not None
-    # module = importlib.util.module_from_spec(spec)
-    # sys.modules[module_name] = module
-    # spec.loader.exec_module(module)
 
     # Run the main task
     entrypoint_fn = getattr(module, entrypoint)
     assert issubclass(entrypoint_fn, TaskType), \
             f'Taskfile `{taskfile}` should contain a task(factory) `{entrypoint}`, but found `{entrypoint_fn}`.'
     entrypoint_task = entrypoint_fn()
     if not dont_force_entrypoint:
         entrypoint_task.clear_task()
     _, stats = entrypoint_task.run_graph_with_stats(rate_limits=rate_limits)
 
-    print('Execution summary:')
-    pprint.pprint(stats['stats'], sort_dicts=False)
+    LOGGER.info('Execution summary:')
+    buf = io.StringIO()
+    pprint.pprint(stats['stats'], sort_dicts=False, stream=buf)
+    for line in buf.getvalue().splitlines():
+        LOGGER.info(line)
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `checkpoint_tool-0.7.6/checkpoint/database.py` & `checkpoint_tool-0.7.7/checkpoint/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,132 +1,157 @@
 from __future__ import annotations
 from typing import Callable, Generic, TypeVar, Any
-from typing_extensions import ParamSpec, Self
+from typing_extensions import Self
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 import shutil
+import gzip
 
 import cloudpickle
-import zlib
 import diskcache as dc
 
 from .types import Context
 from .types import Json
 
 
-K = TypeVar('K')
 T = TypeVar('T')
-S = TypeVar('S')
-U = TypeVar('U')
-P = ParamSpec('P')
-Q = ParamSpec('Q')
-R = TypeVar('R', covariant=True)
 
 
 Serializer = tuple[Callable[[Any], bytes], Callable[[bytes], Any]]
 DEFAULT_SERIALIZER: Serializer = (cloudpickle.dumps, cloudpickle.loads)
-
-
 @dataclass(frozen=True)
 class Database(Generic[T]):
     """ Manage the cache of tasks.
     Layout:
-    Context.cache_dir / 'checkpoint' / name / result     # return values
-    Context.cache_dir / 'checkpoint' / name / timestamp  # timestamps
-    Context.cache_dir / 'checkpoint' / name / data       # other data created by tasks
+    Context.cache_dir / 'checkpoint' / name /
+        * source.txt
+        * id_table
+        * results /
+            * 0.pkl.gz
+            * 1.pkl.gz
+            ...
+        * data /
+            * 0 /
+            * 1 /
+            ...
     """
     name: str
     base_path: Path
     compress_level: int
-    result_cache: dc.Cache
-    timestamp_cache: dc.Cache
+    id_table: IdTable
     serializer: Serializer = DEFAULT_SERIALIZER
 
     @classmethod
     def make(cls, name: str, compress_level: int) -> Self:
         base_path = Context.cache_dir / 'checkpoint' / name
         return Database(
                 name=name,
                 base_path=base_path,
                 compress_level=compress_level,
-                result_cache=dc.Cache(base_path / 'result'),
-                timestamp_cache=dc.Cache(base_path / 'timestamp'),
+                id_table=IdTable(base_path / 'id_table')
                 )
 
     def __post_init__(self) -> None:
         self.data_directory.mkdir(exist_ok=True)
-        self.source_path.parent.mkdir(exist_ok=True)
+        self.result_directory.mkdir(exist_ok=True)
+
+    @property
+    def result_directory(self) -> Path:
+        return Path(self.base_path) / 'results'
+
+    def get_result_path(self, key: Json) -> Path:
+        taskid = self.id_table.get(key)
+        return self.result_directory / f'{taskid}.pkl.gz'
 
     @property
     def data_directory(self) -> Path:
         return Path(self.base_path) / 'data'
 
+    def get_data_directory(self, key: Json) -> Path:
+        taskid = self.id_table.get(key)
+        return self.data_directory / f'{taskid}'
+
     @property
     def source_path(self) -> Path:
-        return Path(self.base_path) / 'code' / 'source.txt'
+        return Path(self.base_path) / 'source.txt'
 
     def update_source_if_necessary(self, source: str) -> datetime:
         # Update source cache
         if self.source_path.exists():
             cached_source = open(self.source_path, 'r').read()
         else:
             cached_source = None
         if cached_source != source:
             open(self.source_path, 'w').write(source)
         return self.load_source_timestamp()
 
     def load_source_timestamp(self) -> datetime:
-        timestamp = self.source_path.stat().st_mtime_ns / 10 ** 9
-        return datetime.fromtimestamp(timestamp)
-
-    def _dumps(self, obj: Any) -> bytes:
-        dumps, _ = self.serializer
-        return zlib.compress(dumps(obj), level=self.compress_level)
-
-    def _loads(self, data: bytes) -> Any:
-        _, loads = self.serializer
-        return loads(zlib.decompress(data))
+        return _get_timestamp(self.source_path)
 
     def save(self, key: Json, obj: T) -> datetime:
-        data = self._dumps(obj)
-        with self.result_cache as ref:
-            ref[key] = data
-
-        timestamp = datetime.now()
-        with self.timestamp_cache as ref:
-            ref[key] = timestamp.timestamp()
-        return timestamp
+        path = self.get_result_path(key)
+        with gzip.open(path, 'wb', compresslevel=self.compress_level) as ref:
+            cloudpickle.dump(obj, ref)
+        return _get_timestamp(path)
 
     def load(self, key: Json) -> T:
-        with self.result_cache as ref:
-            data = ref[key]
-        return self._loads(data)
+        path = self.get_result_path(key)
+        with gzip.open(path, 'rb') as ref:
+            return cloudpickle.load(ref)
 
     def load_timestamp(self, key: Json) -> datetime:
-        with self.timestamp_cache as ref:
-            ts = ref[key]
-        return datetime.fromtimestamp(ts)
-
-    def __contains__(self, key: T) -> bool:
-        with self.result_cache as ref:
-            return key in ref
-
-    def list_keys(self) -> list[str]:
-        with self.result_cache as ref:
-            return list(map(str, ref))
-
-    def _get_caches(self) -> list[dc.Cache]:
-        return [self.result_cache, self.timestamp_cache]
+        path = self.get_result_path(key)
+        if path.exists():
+            return _get_timestamp(path)
+        else:
+            raise KeyError(key)
 
     def clear(self) -> None:
-        for cache in self._get_caches():
-            cache.clear()
+        self.id_table.clear()
         if self.data_directory.exists():
             shutil.rmtree(self.data_directory)
+        if self.result_directory.exists():
+            shutil.rmtree(self.result_directory)
         self.data_directory.mkdir()
+        self.result_directory.mkdir()
 
     def delete(self, key: Json) -> None:
-        for cache in self._get_caches():
-            with cache as ref:
-                del ref[key]
+        resdir = self.get_result_path(key)
+        if resdir.exists():
+            resdir.unlink()
+        else:
+            raise KeyError(key)
+        datadir = self.get_data_directory(key)
+        if datadir.exists():
+            shutil.rmtree(datadir)
+
+
+def _get_timestamp(path: Path) -> datetime:
+    timestamp = path.stat().st_mtime_ns / 10 ** 9
+    return datetime.fromtimestamp(timestamp)
+
+
+@dataclass
+class IdTable:
+    def __init__(self, path: Path | str) -> None:
+        self.table = dc.Cache(directory=path)
+    
+    def get(self, x: Any) -> int:
+        with self.table as ref:
+            try:
+                return ref[x]
+            except KeyError:
+                n = len(ref)
+                ref[x] = n
+                return n
+
+    def __contains__(self, key: Any) -> bool:
+        with self.table as ref:
+            return key in ref
 
+    def list_keys(self) -> list[str]:
+        with self.table as ref:
+            return list(map(str, ref))
+
+    def clear(self) -> None:
+        self.table.clear()
```

### Comparing `checkpoint_tool-0.7.6/checkpoint/graph.py` & `checkpoint_tool-0.7.7/checkpoint/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,29 +127,29 @@
         executor: Executor,
         rate_limits: dict[str, int] | None = None,
         dump_graphs: bool = False,
         ) -> dict[str, Any]:
     """ Consume task graph concurrently.
     """
     stats = {k: len(args) for k, args in graph.get_nodes_by_task().items()}
-    LOGGER.info(f'Following tasks will be called: {stats}')
+    LOGGER.debug(f'Following tasks will be called: {stats}')
     info = {'stats': stats, 'generations': []}
 
     # Read concurrency budgets
     if rate_limits is None:
         rate_limits = {}
     occupied = {k: 0 for k in rate_limits}
 
     # Execute tasks
     standby = graph.get_initial_tasks()
     in_process: set[Future[tuple[ChannelLabels, TaskKey]]] = set()
     with executor as executor:
         while standby or in_process:
             # Log some stats
-            LOGGER.info(
+            LOGGER.debug(
                     f'nodes: {graph.size}, '
                     f'standby: {len(standby)}, '
                     f'in_process: {len(in_process)}'
                     )
             if dump_graphs:
                 info['generations'].append(graph.get_nodes_by_task())
```

### Comparing `checkpoint_tool-0.7.6/checkpoint/task.py` & `checkpoint_tool-0.7.7/checkpoint/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,19 @@
 from typing import Callable, Generic, Mapping, Protocol, Sequence, Type, TypeVar, Any, cast
 from typing_extensions import ParamSpec, Self, get_origin, overload
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from concurrent.futures import Executor
 import ast
-import os
 import logging
 import inspect
 import json
-import base64
 import shutil
 
-import zlib
-
 from .types import Json, TaskKey, Context
 from .database import Database
 from .graph import TaskGraph, run_task_graph
 
 
 LOGGER = logging.getLogger(__name__)
 
@@ -47,18 +43,14 @@
         self.channels = (self.name,) + channels
         self.worker_registry: dict[Json, TaskWorker[R]] = {}
 
         source = inspect.getsource(task_class)
         formatted_source = ast.unparse(ast.parse(source))
         self.source_timestamp = self.db.update_source_if_necessary(formatted_source)
 
-    @property
-    def data_directory(self) -> Path:
-        return self.db.data_directory
-
     def clear_all(self) -> None:
         self.db.clear()
 
 
 class TaskWorker(Generic[R]):
     @classmethod
     def make(cls, config: TaskConfig[P, R], instance: TaskType[P, R], *args: P.args, **kwargs: P.kwargs) -> Self:
@@ -108,22 +100,17 @@
         db = self.config.db
         if self.directory.exists():
             shutil.rmtree(self.directory)
         out = self.instance.run_task()
         db.save(self.arg_key, out)
 
     @property
-    def _relative_path(self) -> str:
-        _, arg_str = self.to_tuple()
-        id_ = base64.urlsafe_b64encode(zlib.compress(arg_str.encode(), level=9)).decode().replace('=', '')
-        return os.path.join(*[id_[i:i+255] for i in range(0, len(id_), 255)])
-
-    @property
     def _directory_uninit(self) -> Path:
-        return Path(self.config.data_directory) / self._relative_path
+        _, arg_str = self.to_tuple()
+        return self.config.db.get_data_directory(arg_str)
 
     @property
     def directory(self) -> Path:
         out = self._directory_uninit
         out.mkdir(exist_ok=True)
         return out
 
@@ -161,15 +148,15 @@
             channels = tuple(_channel)
             assert all(isinstance(q, str) for q in channels)
         elif _channel is None:
             channels = tuple()
         else:
             raise ValueError('Invalid channel value:', _channel)
 
-        compress_level = kwargs.pop('compress_level', 0)
+        compress_level = kwargs.pop('compress_level', 9)
 
         # Fill missing requirement
         ann = inspect.get_annotations(cls, eval_str=True)
         for k, v in ann.items():
             if get_origin(v) is Req and getattr(cls, k, None) is None:
                 req = Req()
                 req.__set_name__(None, k)
@@ -228,14 +215,17 @@
         if executor is None:
             executor = Context.get_executor(max_workers=max_workers)
         else:
             assert max_workers is None
         stats = run_task_graph(graph=graph, executor=executor, rate_limits=rate_limits, dump_graphs=dump_generations)
         return self._task_worker.get_result(), stats
 
+    def map_task(self, func: Callable[[R], T]) -> MappedTask[T]:
+        return MappedTask(self, func)
+
 
 class TaskClassProtocol(Protocol[P, R]):
     def build_task(self, *args: P.args, **kwargs: P.kwargs) -> None: ...
     def run_task(self) -> R: ...
 
 
 def infer_task_type(cls: Type[TaskClassProtocol[P, R]]) -> Type[TaskType[P, R]]:
@@ -263,14 +253,31 @@
         if isinstance(o, TaskType):
             return {'__task__': o._task_worker.to_tuple()}
         else:
             # Let the base class default method raise the TypeError
             return super().default(o)
 
 
+@dataclass
+class MappedTask(Generic[R]):
+    task: TaskLike[Any]
+    mapping: Callable[..., R]
+
+    @classmethod
+    def make(cls, task: TaskLike[T], mapping: Callable[[T], R]) -> Self:
+        return MappedTask(task, mapping)
+
+    def get_origin(self) -> TaskType[..., Any] | Const[Any]:
+        x = self.task
+        if isinstance(x, MappedTask):
+            return x.get_origin()
+        else:
+            return x
+
+
 class Req(Generic[T, R]):
     def __set_name__(self, _: Any, name: str) -> None:
         self.public_name = name
         self.private_name = '_requires__' + name
 
     def __set__(self, obj: TaskType[..., Any], value: T) -> None:
         setattr(obj, self.private_name, value)
@@ -278,34 +285,40 @@
     @overload
     def __get__(self: Req[TaskLike[U], U], obj: TaskType[..., Any], _=None) -> U: ...
     @overload
     def __get__(self: Req[list[TaskLike[U]], list[U]], obj: TaskType[..., Any], _=None) -> list[U]: ...
     @overload
     def __get__(self: Req[dict[K, TaskLike[U]], dict[K, U]], obj: TaskType[..., Any], _=None) -> dict[K, U]: ...
     def __get__(self, obj: TaskType[..., Any], _=None) -> Any:
-        x = getattr(obj, self.private_name)
 
-        def get_worker(task: Task[Any]) -> TaskWorker[Any]:
-            assert isinstance(task, TaskType)
-            return task._task_worker
+        def get_result(task_like: TaskLike[R]) -> R:
+            if isinstance(task_like, TaskType):
+                return task_like._task_worker.get_result()
+            elif isinstance(task_like, MappedTask):
+                return task_like.mapping(get_result(task_like.task))
+            elif isinstance(task_like, Const):
+                return task_like.value
+            else:
+                raise TypeError(f'Unsupported requirement type: {type(task_like)}')
 
-        if isinstance(x, TaskType):
-            return get_worker(x).get_result()
-        elif isinstance(x, list):
-            return [get_worker(t).get_result() for t in x]
+        x = getattr(obj, self.private_name)
+        if isinstance(x, list):
+            return [get_result(t) for t in x]
         elif isinstance(x, dict):
-            return {k: get_worker(v).get_result() for k, v in x.items()}
-        elif isinstance(x, Const):
-            return x.value
+            return {k: get_result(v) for k, v in x.items()}
         else:
-            raise TypeError(f'Unsupported requirement type: {type(x)}')
+            return get_result(x)
 
     def get_task_list(self, obj: TaskType[..., Any]) -> list[TaskType[..., Any]]:
         x = getattr(obj, self.private_name, None)
         assert x is not None, f'Requirement `{self.public_name}` is not set in {obj}.'
+
+        if isinstance(x, MappedTask):
+            x = x.get_origin()
+
         if isinstance(x, TaskType):
             return [x]
         elif isinstance(x, list):
             return x
         elif isinstance(x, dict):
             return list(x.values())
         elif isinstance(x, Const):
@@ -319,13 +332,13 @@
     value: R
 
     def get_result(self) -> R:
         return self.value
 
 
 Task = TaskType[..., R]
-TaskLike = Task[R] | Const[R]
+TaskLike = Task[R] | Const[R] | MappedTask[R]
 
 
 Requires = Req[TaskLike[R], R]
 RequiresList = Req[Sequence[TaskLike[R]], list[R]]
 RequiresDict = Req[Mapping[K, TaskLike[R]], dict[K, R]]
```

### Comparing `checkpoint_tool-0.7.6/checkpoint/types.py` & `checkpoint_tool-0.7.7/checkpoint/types.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.6/pyproject.toml` & `checkpoint_tool-0.7.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.7.6"
+version = "0.7.7"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint"}]
```

### Comparing `checkpoint_tool-0.7.6/PKG-INFO` & `checkpoint_tool-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.7.6
+Version: 0.7.7
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -180,18 +180,19 @@
     def build_task(self, task_dict: dict[str, Task[float]]):
         self.scores = task_dict
 
     def run_task(self) -> float:
         return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
 
-The output of the `main` method should be serializable with `cloudpickle`.
-Large outputs can be stored with compression via `zlib`:
+The output of the `run_task` method should be serializable with `cloudpickle`,
+which is then compressed with `gzip`.
+The compression level can be changed as follows (defaults to 9).
 ```python
-class LargeOutputTask(Task, compress_level=-1):
+class LargeOutputTask(Task, compress_level=0):
     ...
 ```
 
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
@@ -238,15 +239,15 @@
 
 # Task-level concurrency control
 SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_name: 1})
 
 ```
 
 ### Commandline tool
-We can use checkpoint-tool from commandline like `python -m checkpoint.app path/to/taskfile.py`, where `taskfile.py` defines the `main` task as follows:
+We can use checkpoint-tool from commandline like `python -m checkpoint.app path/to/taskfile.py`, where `taskfile.py` defines the `Main` task as follows:
 ```python
 # taskfile.py
 
 class Main(Task):
     ...
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/checkpoint/...`.
```

