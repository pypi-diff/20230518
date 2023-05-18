# Comparing `tmp/checkpoint_tool-0.7.7.tar.gz` & `tmp/checkpoint_tool-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkpoint_tool-0.7.7.tar", max compression
+gzip compressed data, was "checkpoint_tool-0.7.8.tar", max compression
```

## Comparing `checkpoint_tool-0.7.7.tar` & `checkpoint_tool-0.7.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7248 2023-05-18 16:17:30.843008 checkpoint_tool-0.7.7/README.md
--rw-r--r--   0        0        0      608 2023-05-09 01:50:05.066517 checkpoint_tool-0.7.7/checkpoint/__init__.py
--rw-r--r--   0        0        0     2514 2023-05-18 16:34:53.180387 checkpoint_tool-0.7.7/checkpoint/app.py
--rw-r--r--   0        0        0     4517 2023-05-18 16:13:03.919978 checkpoint_tool-0.7.7/checkpoint/database.py
--rw-r--r--   0        0        0     7245 2023-05-18 16:35:39.947857 checkpoint_tool-0.7.7/checkpoint/graph.py
--rw-r--r--   0        0        0    11335 2023-05-18 17:02:34.386785 checkpoint_tool-0.7.7/checkpoint/task.py
--rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 checkpoint_tool-0.7.7/checkpoint/types.py
--rw-r--r--   0        0        0      677 2023-05-18 16:21:55.175049 checkpoint_tool-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     8053 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     7585 2023-05-18 17:58:28.559869 checkpoint_tool-0.7.8/README.md
+-rw-r--r--   0        0        0      608 2023-05-09 01:50:05.066517 checkpoint_tool-0.7.8/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2514 2023-05-18 16:34:53.180387 checkpoint_tool-0.7.8/checkpoint/app.py
+-rw-r--r--   0        0        0     4517 2023-05-18 16:13:03.919978 checkpoint_tool-0.7.8/checkpoint/database.py
+-rw-r--r--   0        0        0     7245 2023-05-18 16:35:39.947857 checkpoint_tool-0.7.8/checkpoint/graph.py
+-rw-r--r--   0        0        0    11598 2023-05-18 17:58:37.784526 checkpoint_tool-0.7.8/checkpoint/task.py
+-rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 checkpoint_tool-0.7.8/checkpoint/types.py
+-rw-r--r--   0        0        0      677 2023-05-18 17:59:01.461549 checkpoint_tool-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     8390 1970-01-01 00:00:00.000000 checkpoint_tool-0.7.8/PKG-INFO
```

### Comparing `checkpoint_tool-0.7.7/README.md` & `checkpoint_tool-0.7.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 ans = Choose(6, 3).run_graph()
 
 # Delete all the cache associated with `Choose`,
 # equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.Choose`.
 Choose.clear_all_tasks()            
 ```
 
-### Limitations of Task I/O
+### Task IO
 
 The arguments of the `init` method can be anything JSON serializable:
 ```python
 class T1(Task):
     def build_task(self, **param1):
         ...
     ...
@@ -159,27 +159,42 @@
     def build_task(self, task_dict: dict[str, Task[float]]):
         self.scores = task_dict
 
     def run_task(self) -> float:
         return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
 
+One can also directly access the items of dictionary-valued upstream tasks with `get_taskitem`.
+```python
+class MultiOutputTask(Task):
+    ...
+
+    def run_task(self) -> dict[str, int]:
+        return {'foo': 42, ...}
+
+class DownstreamTask(Task):
+    dep: Requires[int]
+
+    def build_task(self):
+        self.dep = MultiOutputTask().get_taskitem('foo')
+```
+
 The output of the `run_task` method should be serializable with `cloudpickle`,
 which is then compressed with `gzip`.
 The compression level can be changed as follows (defaults to 9).
 ```python
-class LargeOutputTask(Task, compress_level=0):
+class NoCompressionTask(Task, compress_level=0):
     ...
 ```
 
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
-`{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{cryptic_task_id}`
+`{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
 class TrainModel(Task):
     ...
 
     def run_task(self) -> str:
         ...
```

### Comparing `checkpoint_tool-0.7.7/checkpoint/__init__.py` & `checkpoint_tool-0.7.8/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.7/checkpoint/app.py` & `checkpoint_tool-0.7.8/checkpoint/app.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.7/checkpoint/database.py` & `checkpoint_tool-0.7.8/checkpoint/database.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.7/checkpoint/graph.py` & `checkpoint_tool-0.7.8/checkpoint/graph.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.7/checkpoint/task.py` & `checkpoint_tool-0.7.8/checkpoint/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 K = TypeVar('K')
 T = TypeVar('T')
+S = TypeVar('S')
 U = TypeVar('U')
 P = ParamSpec('P')
 R = TypeVar('R', covariant=True)
 
 
 class TaskConfig(Generic[P, R]):
     """ Information specific to a task class (not instance) """
@@ -215,16 +216,16 @@
         if executor is None:
             executor = Context.get_executor(max_workers=max_workers)
         else:
             assert max_workers is None
         stats = run_task_graph(graph=graph, executor=executor, rate_limits=rate_limits, dump_graphs=dump_generations)
         return self._task_worker.get_result(), stats
 
-    def map_task(self, func: Callable[[R], T]) -> MappedTask[T]:
-        return MappedTask(self, func)
+    def get_taskitem(self: TaskType[..., Mapping[K, T]], key: K) -> _MappedTask[K, T]:
+        return _MappedTask(self, key)
 
 
 class TaskClassProtocol(Protocol[P, R]):
     def build_task(self, *args: P.args, **kwargs: P.kwargs) -> None: ...
     def run_task(self) -> R: ...
 
 
@@ -248,35 +249,41 @@
     return cast(Json, json.dumps(arguments, separators=(',', ':'), sort_keys=True, cls=CustomJSONEncoder))
 
 
 class CustomJSONEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, TaskType):
             return {'__task__': o._task_worker.to_tuple()}
+        elif isinstance(o, _MappedTask):
+            return {'__task__': o.get_origin()._task_worker.to_tuple(), '__key__': o.get_args()}
         else:
             # Let the base class default method raise the TypeError
             return super().default(o)
 
 
 @dataclass
-class MappedTask(Generic[R]):
-    task: TaskLike[Any]
-    mapping: Callable[..., R]
+class _MappedTask(Generic[K, T]):
+    task: TaskType[..., Mapping[K, T]] | _MappedTask[Any, Mapping[K, T]]
+    key: K
 
-    @classmethod
-    def make(cls, task: TaskLike[T], mapping: Callable[[T], R]) -> Self:
-        return MappedTask(task, mapping)
-
-    def get_origin(self) -> TaskType[..., Any] | Const[Any]:
+    def get_origin(self) -> TaskType[..., Any]:
         x = self.task
-        if isinstance(x, MappedTask):
+        if isinstance(x, _MappedTask):
             return x.get_origin()
         else:
             return x
 
+    def get_args(self) -> list[Any]:
+        out = []
+        x = self
+        while isinstance(x, _MappedTask):
+            out.append(x.key)
+            x = x.task
+        return out[::-1]
+
 
 class Req(Generic[T, R]):
     def __set_name__(self, _: Any, name: str) -> None:
         self.public_name = name
         self.private_name = '_requires__' + name
 
     def __set__(self, obj: TaskType[..., Any], value: T) -> None:
@@ -286,19 +293,19 @@
     def __get__(self: Req[TaskLike[U], U], obj: TaskType[..., Any], _=None) -> U: ...
     @overload
     def __get__(self: Req[list[TaskLike[U]], list[U]], obj: TaskType[..., Any], _=None) -> list[U]: ...
     @overload
     def __get__(self: Req[dict[K, TaskLike[U]], dict[K, U]], obj: TaskType[..., Any], _=None) -> dict[K, U]: ...
     def __get__(self, obj: TaskType[..., Any], _=None) -> Any:
 
-        def get_result(task_like: TaskLike[R]) -> R:
+        def get_result(task_like: TaskLike[S]) -> S:
             if isinstance(task_like, TaskType):
                 return task_like._task_worker.get_result()
-            elif isinstance(task_like, MappedTask):
-                return task_like.mapping(get_result(task_like.task))
+            elif isinstance(task_like, _MappedTask):
+                return get_result(task_like.task)[task_like.key]
             elif isinstance(task_like, Const):
                 return task_like.value
             else:
                 raise TypeError(f'Unsupported requirement type: {type(task_like)}')
 
         x = getattr(obj, self.private_name)
         if isinstance(x, list):
@@ -308,15 +315,15 @@
         else:
             return get_result(x)
 
     def get_task_list(self, obj: TaskType[..., Any]) -> list[TaskType[..., Any]]:
         x = getattr(obj, self.private_name, None)
         assert x is not None, f'Requirement `{self.public_name}` is not set in {obj}.'
 
-        if isinstance(x, MappedTask):
+        if isinstance(x, _MappedTask):
             x = x.get_origin()
 
         if isinstance(x, TaskType):
             return [x]
         elif isinstance(x, list):
             return x
         elif isinstance(x, dict):
@@ -332,13 +339,13 @@
     value: R
 
     def get_result(self) -> R:
         return self.value
 
 
 Task = TaskType[..., R]
-TaskLike = Task[R] | Const[R] | MappedTask[R]
+TaskLike = Task[R] | Const[R] | _MappedTask[Any, R]
 
 
 Requires = Req[TaskLike[R], R]
 RequiresList = Req[Sequence[TaskLike[R]], list[R]]
 RequiresDict = Req[Mapping[K, TaskLike[R]], dict[K, R]]
```

### Comparing `checkpoint_tool-0.7.7/checkpoint/types.py` & `checkpoint_tool-0.7.8/checkpoint/types.py`

 * *Files identical despite different names*

### Comparing `checkpoint_tool-0.7.7/pyproject.toml` & `checkpoint_tool-0.7.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkpoint-tool"
-version = "0.7.7"
+version = "0.7.8"
 description = "A lightweight workflow management tool written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/checkpoint"
 repository = "https://github.com/koheimiya/checkpoint"
 readme = "README.md"
 packages = [{include = "checkpoint"}]
```

### Comparing `checkpoint_tool-0.7.7/PKG-INFO` & `checkpoint_tool-0.7.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkpoint-tool
-Version: 0.7.7
+Version: 0.7.8
 Summary: A lightweight workflow management tool written in pure Python
 Home-page: https://github.com/koheimiya/checkpoint
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -98,15 +98,15 @@
 ans = Choose(6, 3).run_graph()
 
 # Delete all the cache associated with `Choose`,
 # equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.Choose`.
 Choose.clear_all_tasks()            
 ```
 
-### Limitations of Task I/O
+### Task IO
 
 The arguments of the `init` method can be anything JSON serializable:
 ```python
 class T1(Task):
     def build_task(self, **param1):
         ...
     ...
@@ -180,27 +180,42 @@
     def build_task(self, task_dict: dict[str, Task[float]]):
         self.scores = task_dict
 
     def run_task(self) -> float:
         return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
 ```
 
+One can also directly access the items of dictionary-valued upstream tasks with `get_taskitem`.
+```python
+class MultiOutputTask(Task):
+    ...
+
+    def run_task(self) -> dict[str, int]:
+        return {'foo': 42, ...}
+
+class DownstreamTask(Task):
+    dep: Requires[int]
+
+    def build_task(self):
+        self.dep = MultiOutputTask().get_taskitem('foo')
+```
+
 The output of the `run_task` method should be serializable with `cloudpickle`,
 which is then compressed with `gzip`.
 The compression level can be changed as follows (defaults to 9).
 ```python
-class LargeOutputTask(Task, compress_level=0):
+class NoCompressionTask(Task, compress_level=0):
     ...
 ```
 
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
-`{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{cryptic_task_id}`
+`{$CP_CACHE_DIR:-./.cache}/checkpoint/{module_name}.{task_name}/data/{task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
 class TrainModel(Task):
     ...
 
     def run_task(self) -> str:
         ...
```

