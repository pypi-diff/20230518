# Comparing `tmp/pytreeclass-0.3.4.tar.gz` & `tmp/pytreeclass-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.3.4.tar", last modified: Fri May 12 18:36:35 2023, max compression
+gzip compressed data, was "pytreeclass-0.3.6.tar", last modified: Thu May 18 18:30:40 2023, max compression
```

## Comparing `pytreeclass-0.3.4.tar` & `pytreeclass-0.3.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/code_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28159 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    28279 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/pytreeclass/_src/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 18:36:35.000000 pytreeclass-0.3.4/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:35.767387 pytreeclass-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-12 18:36:26.000000 pytreeclass-0.3.4/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.929109 pytreeclass-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-18 18:30:40.929109 pytreeclass-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.925109 pytreeclass-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.925109 pytreeclass-0.3.6/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.925109 pytreeclass-0.3.6/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28722 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.925109 pytreeclass-0.3.6/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 18:30:40.000000 pytreeclass-0.3.6/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 18:30:40.929109 pytreeclass-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:40.929109 pytreeclass-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-18 18:30:17.000000 pytreeclass-0.3.6/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.3.4/LICENSE` & `pytreeclass-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/PKG-INFO` & `pytreeclass-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.4
+Version: 0.3.6
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytreeclass-0.3.4/README.md` & `pytreeclass-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/docs/conf.py` & `pytreeclass-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/pytreeclass/__init__.py` & `pytreeclass-0.3.6/pytreeclass/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,8 +46,8 @@
     "tree_map_with_trace",
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
     "Partial",
 )
 
-__version__ = "0.3.4"
+__version__ = "0.3.6"
```

### Comparing `pytreeclass-0.3.4/pytreeclass/_src/code_build.py` & `pytreeclass-0.3.6/pytreeclass/_src/code_build.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,149 +1,127 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""Constructor code generation from type annotations."""
+
 from __future__ import annotations
 
 import functools as ft
 import sys
 from collections.abc import Callable, MutableMapping, MutableSequence
 from types import FunctionType, MappingProxyType
-from typing import Any, NamedTuple, Sequence
-
-"""Constructor code generation from type annotations."""
+from typing import Any, Literal, NamedTuple, Sequence, TypeVar, get_args
 
+T = TypeVar("T")
 PyTree = Any
 EllipsisType = type(Ellipsis)
-_NOT_SET = type("NOT_SET", (), {"__repr__": lambda _: "NOT_SET"})()
-_MUTABLE_TYPES = (MutableSequence, MutableMapping, set)
+ArgKindType = Literal["POS_ONLY", "POS_OR_KW", "KW_ONLY"]
+ArgKind = get_args(ArgKindType)
+NULL = type("NULL", (), {"__repr__": lambda _: "NULL"})()
+MUTABLE_TYPES = (MutableSequence, MutableMapping, set)
 # https://github.com/google/jax/issues/14295
 
 
 class Field(NamedTuple):
     name: str | None = None
     type: type | None = None
-    default: Any = _NOT_SET
-    factory: Any = None
+    default: Any = NULL
     init: bool = True
     repr: bool = True
-    kw_only: bool = False
-    pos_only: bool = False
-    metadata: MappingProxyType[str, Any] | None = None
+    kind: ArgKindType = "POS_OR_KW"
+    metadata: dict[str, Any] | None = None
     callbacks: Sequence[Any] = ()
     alias: str | None = None
 
+    def __call__(self, value: Any):
+        """Call the field's callbacks on `value`."""
+        for callback in self.callbacks:
+            try:
+                value = callback(value)
+            except Exception as e:
+                cname = getattr(callback, "__name__", callback)
+                raise type(e)(f"On applying {cname} for field=`{self.name}`:\n{e}")
+        return value
+
 
 def field(
+    default: Any = NULL,
     *,
-    default: Any = _NOT_SET,
-    factory: Callable | None = None,
     init: bool = True,
     repr: bool = True,
-    kw_only: bool = False,
-    pos_only: bool = False,
+    kind: ArgKindType = "POS_OR_KW",
     metadata: dict[str, Any] | None = None,  # type: ignore
     callbacks: Sequence[Any] = (),
     alias: str | None = None,
 ) -> Field:
     """
     Args:
-        default: The default value of the field. Mutually exclusive with `factory`.
-        factory: A 0-argument function called to initialize field value.
-            Mutually exclusive with `default`.
+        default: The default value of the field.
         init: Whether the field is included in the object's __init__ function.
         repr: Whether the field is included in the object's __repr__ function.
-        kw_only: Whether the field is keyword-only. Mutually exclusive
-            with `pos_only`, effectively placing `/` in the constructor.
-        pos_only: Whether the field is positional-only. Mutually exclusive
-            with `kw_only`, effectively placing `*` in the constructor.
+        kind: Argument kind, one of 'POS_ONLY', 'KW_ONLY', or 'POS_OR_KW'.
         metadata: A mapping of user-defined data for the field.
         callbacks: A sequence of functions to called on `setattr` during
             initialization to modify the field value.
         alias: An a alias for the field name in the constructor.
 
     Example:
         >>> import pytreeclass as pytc
-        >>> def instance_cb_factory(klass):
-        ...    def wrapper(x):
-        ...        assert isinstance(x, klass)
+        >>> class IsInstance(pytc.TreeClass):
+        ...    klass: type
+        ...    def __call__(self, x):
+        ...        assert isinstance(x, self.klass)
+        ...        return x
+        >>> class Range(pytc.TreeClass):
+        ...    start: int|float = float("-inf")
+        ...    stop: int|float = float("inf")
+        ...    def __call__(self, x):
+        ...        assert self.start <= x <= self.stop
         ...        return x
-        ...    return wrapper
-
-        >>> def positive_check_callback(x):
-        ...    assert x > 0
-        ...    return x
-
         >>> class Employee(pytc.TreeClass):
         ...    # assert employee `name` is str
-        ...    name: str = pytc.field(callbacks=[instance_cb_factory(str)])
+        ...    name: str = pytc.field(callbacks=[IsInstance(str)])
         ...    # use callback compostion to assert employee `age` is int and positive
-        ...    age: int = pytc.field(callbacks=[instance_cb_factory(int), positive_check_callback])
+        ...    age: int = pytc.field(callbacks=[IsInstance(int), Range(1)])
         ...    # use `id` in the constructor for `_id` attribute
         ...    # this is useful for private attributes that are not supposed
         ...    # to be accessed directly and hide it from the repr
         ...    _id: int = pytc.field(alias="id", repr=False)
-
-        >>> tree = Employee(name="Asem", age=10, id=1)
-        >>> print(tree)  # _id is not shown
+        >>> employee = Employee(name="Asem", age=10, id=1)
+        >>> print(employee)  # _id is not shown
         Employee(name=Asem, age=10)
-        >>> assert tree._id == 1  # this is the private attribute
+        >>> assert employee._id == 1  # this is the private attribute
     """
     if not isinstance(alias, (str, type(None))):
-        raise TypeError(
-            "`alias` must be a string describing the alias name of the field"
-            "in the constructor or `None` if no alias is provided, "
-            f"got type=`{type(alias).__name__}` instead."
-        )
-
-    if default is not _NOT_SET and factory is not None:
-        raise ValueError(
-            "`default` and `factory` are mutually exclusive arguments."
-            "Use `default` if the value is immutable or a zero-argument "
-            "function returning a mutable value in `factory` otherwise.\n"
-            f"got {default=} and {factory=}"
-        )
-
-    if kw_only is True and pos_only is True:
-        raise ValueError(
-            "`kw_only` and `pos_only` are mutually exclusive arguments."
-            "Use `kw_only` if the field is a keyword-only argument in "
-            "the constructor and `pos_only` if the field is positional only, "
-            f"got {kw_only=} and {pos_only=}"
-        )
-
-    if isinstance(metadata, dict):
-        metadata = MappingProxyType(metadata)  # type: ignore
-    elif metadata is not None:
-        raise TypeError(
-            "`metadata` must be a dictionary describing the metadata of "
-            "the field or `None` if no metadata is provided, "
-            f"got type=`{type(metadata).__name__}` instead."
-        )
-
+        raise TypeError(f"Non-string {alias=} argument provided to `field`")
+    if not isinstance(metadata, (dict, type(None))):
+        raise TypeError(f"Non-dict {metadata=} argument provided to `field`")
+    if kind not in ArgKind:
+        raise ValueError(f"{kind=} not in {ArgKind}")
     if not isinstance(callbacks, Sequence):
-        raise TypeError(
-            f"`callbacks` must be a Sequence of one-argument function(s) "
-            "operating on the field value, and returning a modified value, "
-            f"got type `{type(callbacks).__name__}` instead."
-        )
-
-    for index, callback in enumerate(callbacks):
+        raise TypeError(f"Non-sequence {callbacks=} argument provided to `field`")
+    for callback in callbacks:
         if not isinstance(callback, Callable):  # type: ignore
-            raise TypeError(
-                f"`callback` must be a one-argument function "
-                "operating on the field value, and returning a modified value, "
-                f"got type `{type(callback).__name__}` at {index=} instead."
-            )
+            raise TypeError(f"Non-callable {callback=} provided to `field`")
 
     return Field(
-        name=None,
-        type=None,
         default=default,
-        factory=factory,
         init=init,
         repr=repr,
-        kw_only=kw_only,
-        pos_only=pos_only,
+        kind=kind,
         metadata=metadata,  # type: ignore
         callbacks=callbacks,
         alias=alias,
     )
 
 
 @ft.lru_cache(maxsize=128)
@@ -157,92 +135,85 @@
         field_map.update(_build_field_map(base))
 
     # TODO: use inspect to get annotations, once min python version >3.9
     if "__annotations__" not in vars(klass):
         return MappingProxyType(field_map)
 
     for name in (annotation_map := vars(klass)["__annotations__"]):
-        value = vars(klass).get(name, _NOT_SET)
-        type = annotation_map[name]
+        value = vars(klass).get(name, NULL)
+        hint = annotation_map[name]
 
         if name == "self":
             # while `dataclasses` allows `self` as a field name, its confusing
             # and not recommended. so raise an error
             raise ValueError("Field name cannot be `self`.")
 
         if isinstance(value, Field):
-            if isinstance(value.default, _MUTABLE_TYPES):
+            if isinstance(value.default, MUTABLE_TYPES):
                 # example case: `x: Any = field(default=[1, 2, 3])`
-                raise TypeError(
-                    f"Mutable default value= {value.default} is not allowed"
-                    f" for field `{name}` in class `{klass.__name__}`.\n"
-                    f" use `field(... ,factory=lambda:{value.default})` instead"
-                )
+                raise TypeError(f"Mutable {value.default=} is not allowed.")
             # case: `x: Any = field(default=1)`
-            field_map[name] = value._replace(name=name, type=type)
+            field_map[name] = value._replace(name=name, type=hint)
         else:
-            if isinstance(value, _MUTABLE_TYPES):
-                # https://github.com/ericvsmith/dataclasses/issues/3
+            if isinstance(value, MUTABLE_TYPES):
                 # example case: `x: Any = [1, 2, 3]`
-                raise TypeError(
-                    f"Mutable value= {(value)} is not allowed"
-                    f" for field `{name}` in class `{klass.__name__}`.\n"
-                    f" use `field(... ,factory=lambda:{value})` instead"
-                )
+                raise TypeError(f"Mutable {value=} is not allowed")
             # case: `x: int = 1` or `x: Any`
-            field_map[name] = Field(name=name, type=type, default=value)
+            field_map[name] = Field(name=name, type=hint, default=value)
     return MappingProxyType(field_map)
 
 
 def fields(x: Any) -> Sequence[Field]:
     """Returns a tuple of `Field` objects for the given instance or class.
 
     `Field` objects are generated from the class type hints and contains
     the information about the field `name`, `type`, `default` value, and other
-    information (`factory`, `init`, `repr`, `kw_only`, `pos_only`, `metadata`,
+    information (`init`, `repr`, `kind`, `metadata`,
     `callbacks`, `alias`) if the user uses the `pytreeclass.field`to annotate.
 
     Note:
         - If the class is not annotated, an empty tuple is returned.
         - The `Field` generation is cached for class and its bases.
     """
     return tuple(_build_field_map(x if isinstance(x, type) else type(x)).values())
 
 
 def _build_init_method(klass: type) -> FunctionType:
     # generate a code object for the __init__ method and compile it
     # for the given class and return the function object
-    head, body = ["self"], []
+    body = []
+    hints = dict()
+    head = ["self"]
+    heads = dict(zip(ArgKind, ([], [], [])))
+    has_post = "__post_init__" in vars(klass)
 
     for field in (field_map := _build_field_map(klass)).values():
-        name = field.name  # name in body
-        alias = field.alias or name  # name in constructor
-
-        if field.kw_only and "*" not in head and field.init:
-            head += ["*"]
+        dref = "" if field.default is NULL else f"=field_map['{field.name}'].default"
 
-        if field.default is not _NOT_SET:
-            vref = f"field_map['{name}'].default"
-            head += [f"{alias}={vref}"] if field.init else []
-            body += [f"self.{name}=" + (f"{alias}" if field.init else f"{vref}")]
-        elif field.factory is not None:
-            vref = f"field_map['{name}'].factory()"
-            head += [f"{alias}={vref}"] if field.init else []
-            body += [f"self.{name}=" + (f"{alias}" if field.init else f"{vref}")]
+        if field.init:
+            alias = field.alias or field.name
+            hints[field.name] = field.type
+            body += [f"self.{field.name}={alias}"]
+            heads[field.kind] += [f"{alias}{dref}"]
         else:
-            head += [f"{alias}"] if field.init else []
-            body += [f"self.{name}={alias}"] if field.init else []
+            body += [f"self.{field.name}{dref}"]
 
-        if field.pos_only and field.init:
-            if "/" in head:
-                head.remove("/")
-            head += ["/"]
+    hints["return"] = None
+    # add the post init call if the class has it, otherwise add a pass
+    # in case all fields are not initialized in the __init__ method
+    body += ["self.__post_init__()"] if has_post else ["pass"]
+
+    # organize the arguments order (POS_ONLY, POS_OR_KW, KW_ONLY)
+    head += (heads["POS_ONLY"] + ["/"]) if heads["POS_ONLY"] else []
+    head += heads["POS_OR_KW"]
+    head += (["*"] + heads["KW_ONLY"]) if heads["KW_ONLY"] else []
 
-    body += ["getattr(type(self), '__post_init__', lambda _: None)(self)"]
+    # generate the code for the __init__ method
     code = "def closure(field_map):\n"
     code += f"\tdef __init__({','.join(head)}):"
     code += f"\n\t\t{';'.join(body)}"
     code += f"\n\t__init__.__qualname__ = '{klass.__qualname__}.__init__'"
     code += "\n\treturn __init__"
 
     exec(code, vars(sys.modules[klass.__module__]), namespace := dict())
-    return namespace["closure"](field_map)
+    setattr(init := namespace["closure"](field_map), "__annotations__", hints)
+    return init
```

### Comparing `pytreeclass-0.3.4/pytreeclass/_src/tree_base.py` & `pytreeclass-0.3.6/pytreeclass/_src/tree_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+"""Define a class that convert a class to a JAX compatible tree structure"""
+
 from __future__ import annotations
 
 import abc
 from collections.abc import Callable
 from contextlib import contextmanager
 from typing import Any, NamedTuple, TypeVar
 
@@ -24,17 +39,14 @@
     _leafwise_transform,
     _resolve_where,
     is_tree_equal,
     tree_copy,
     tree_hash,
 )
 
-"""Define a class that convert a class to a JAX compatible tree structure"""
-
-
 T = TypeVar("T", bound="TreeClass")
 PyTree = Any
 EllipsisType = type(Ellipsis)
 _no_initializer = object()
 
 # allow methods in mutable context to be called without raising `AttributeError`
 # the instances are registered  during initialization and using `at`  property
@@ -320,15 +332,15 @@
 
         with _mutable_context(self):
             # initialize the instance under the mutable context
             # to allow setting instance attributes without
             # throwing an `AttributeError`
             getattr(klass, "__init__")(self, *a, **k)
 
-        if len(keys := set(_build_field_map(klass)) - set(vars(self))):
+        if keys := set(_build_field_map(klass)) - set(vars(self)):
             raise AttributeError(f"Found uninitialized fields {keys}.")
         return self
 
 
 @dataclass_transform(field_specifiers=(field, Field))
 class TreeClass(metaclass=TreeClassMeta):
     """Convert a class to a JAX compatible tree structure.
@@ -424,36 +436,38 @@
             # useful to use with `bcmap` and creating masks by comparisons.
             klass = _leafwise_transform(klass)
 
         klass = _register_treeclass(klass)
 
     def __setattr__(self, key: str, value: Any) -> None:
         if id(self) not in _mutable_instance_registry:
+            # instance is not under a mutable context
+            # mutable context is used for setting instance attributes
+            # during initialization and when using the `at` property
+            # with call method.
             raise AttributeError(
                 f"Cannot set attribute {value=} to `{key=}`  "
                 f"on an immutable instance of `{type(self).__name__}`.\n"
                 f"Use `.at['{key}'].set({value})` "
                 "to set the value immutably.\nExample:\n"
                 f">>> tree1 = {type(self).__name__}(...)\n"
                 f">>> tree2 = tree1.at['{key}'].set({value!r})\n"
                 ">>> assert not tree1 is tree2\n"
                 f">>> tree2.{key}\n{value}"
             )
 
         if key in (field_map := _build_field_map(type(self))):
-            for callback in field_map[key].callbacks:
-                try:
-                    value = callback(value)
-                except Exception as e:
-                    raise type(e)(f"Error for field=`{key}`:\n{e}")
+            # apply field callbacks on the value before setting
+            value = field_map[key](value)
 
         getattr(object, "__setattr__")(self, key, value)
 
     def __delattr__(self, key: str) -> None:
         if id(self) not in _mutable_instance_registry:
+            # instance is not under a mutable context
             raise AttributeError(
                 f"Cannot delete attribute `{key}` "
                 f"on immutable instance of `{type(self).__name__}`.\n"
                 f"Use `.at['{key}'].set(None)` instead."
             )
 
         getattr(object, "__delattr__")(self, key)
```

### Comparing `pytreeclass-0.3.4/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.3.6/pytreeclass/_src/tree_pprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import inspect
 import math
 from itertools import chain
@@ -143,15 +157,14 @@
 
     # handle mean and std
     mean, std = f"{np.mean(node):.2f}", f"{np.std(node):.2f}"
 
     return f"{base}(μ={mean}, σ={std}, ∈{interval})"
 
 
-@ft.lru_cache
 def _func_pprint(
     func: Callable,
     *,
     indent: int,
     kind: PrintKind,
     width: int,
     depth: int,
@@ -295,15 +308,15 @@
     width: int,
     depth: int,
 ) -> str:
     name = type(node).__name__
     if depth == 0:
         return f"{name}(...)"
 
-    # avoid circular import by importing Partial here
+    # avoid circular import by importing here
     from pytreeclass import fields
 
     skip = [f.name for f in fields(node) if not f.repr]
     kvs = ((k, v) for k, v in vars(node).items() if k not in skip)
     spec = dict(indent=indent + 1, kind=kind, width=width, depth=depth - 1)
     text = (f"{k}={_node_pprint(v,**spec)}" for k, v in kvs)
     text = (", \n" + "\t" * (indent + 1)).join(text)
```

### Comparing `pytreeclass-0.3.4/pytreeclass/_src/tree_util.py` & `pytreeclass-0.3.6/pytreeclass/_src/tree_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,28 @@
+# Copyright 2023 PyTreeClass authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import hashlib
 import operator as op
+from collections import defaultdict
 from math import ceil, floor, trunc
 from typing import Any, Callable, Hashable, Iterator, Sequence, Tuple, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
@@ -529,51 +544,49 @@
     idx: int
     key: Hashable
 
     def __str__(self):
         return f".{self.key}"
 
 
+# indexing matching registry
+# define rule for indexing matching through `at` property
+# for example, `jax` internals uses `jtu.GetAttrKey` to index an attribute,
+# however its not ergonomic to use `tree.at[jtu.GetAttrKey("attr")]`
+# to index an attribute instead `tree.at['attr']` is more ergonomic
+match_registry: dict[type, Callable] = defaultdict(lambda entry: (entry,))
+match_registry[jtu.GetAttrKey] = lambda entry: (entry.name,)
+match_registry[jtu.SequenceKey] = lambda entry: (entry.idx,)
+match_registry[NamedSequenceKey] = lambda entry: (entry.idx, entry.key)
+match_registry[jtu.DictKey] = lambda entry: (entry.key,)
+match_registry[jtu.FlattenedIndexKey] = lambda entry: (entry.key,)
+
+
 def _generate_path_mask(
     tree: PyTree,
     where: tuple[int | str, ...],
     is_leaf: IsLeafType = None,
 ) -> PyTree:
     # generate a mask for `where` path in `tree`
     # where path is a tuple of indices or keys, for example
     # where=("a",) wil set all leaves of `tree` with key "a" to True and
     # all other leaves to False
     match = False
 
-    def _unpack_entry(entry) -> tuple[Any, ...]:
-        # define rule for indexing matching through `at` property
-        # in `jax` internals uses `jtu.GetAttrKey` to index an attribute,
-        # however its not ergonomic to use `tree.at[jtu.GetAttrKey("attr")]`
-        # to index an attribute instead `tree.at['attr']` is more ergonomic
-        if isinstance(entry, jtu.GetAttrKey):
-            return (entry.name,)
-        if isinstance(entry, jtu.SequenceKey):
-            return (entry.idx,)
-        if isinstance(entry, (jtu.DictKey, jtu.FlattenedIndexKey)):
-            return (entry.key,)
-        if isinstance(entry, NamedSequenceKey):
-            return (entry.idx, entry.key)
-        return (entry,)
-
     def map_func(path: TraceType, _: Any):
         keys, _ = path
 
         if len(where) > len(keys):
             # path is shorter than `where` path. for example
             # where=("a", "b") and the current path is ("a",) then
             # the current path is not a match
             return False
 
         for wi, key in zip(where, keys):
-            if wi not in (..., *_unpack_entry(key)):
+            if wi not in (..., *match_registry[type(key)](key)):
                 return False
 
         nonlocal match
 
         return (match := True)
 
     mask = tree_map_with_trace(map_func, tree, is_leaf=is_leaf)
```

### Comparing `pytreeclass-0.3.4/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.3.6/pytreeclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.3.4
+Version: 0.3.6
 Summary: JAX compatible dataclass.
 Home-page: https://github.com/ASEM000/pytreeclass
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: Apache-2.0
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytreeclass-0.3.4/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.3.6/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/setup.py` & `pytreeclass-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_indexing.py` & `pytreeclass-0.3.6/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_nn.py` & `pytreeclass-0.3.6/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_tree_freeze.py` & `pytreeclass-0.3.6/tests/test_tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_tree_operator.py` & `pytreeclass-0.3.6/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_tree_pprint.py` & `pytreeclass-0.3.6/tests/test_tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_tree_viz_util.py` & `pytreeclass-0.3.6/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.3.4/tests/test_treeclass.py` & `pytreeclass-0.3.6/tests/test_treeclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,93 +7,87 @@
 import numpy.testing as npt
 import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
 
 
-def test_field_mutually_exclusive():
-    with pytest.raises(ValueError):
-        pytc.field(default=1, factory=lambda: 1)
-
-    with pytest.raises(ValueError):
-        pytc.field(default=1, pos_only=True, kw_only=True)
-
-
 def test_fields():
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1, metadata={"meta": 1})
         b: int = 2
 
     assert len(pytc.fields(Test)) == 2
     assert pytc.fields(Test)[0].metadata == {"meta": 1}
 
+    with pytest.raises(ValueError):
+        pytc.field(kind="WRONG")
+
 
 def test_field():
     assert pytc.field(default=1).default == 1
 
     with pytest.raises(TypeError):
         pytc.field(metadata=1)
 
     class Test(pytc.TreeClass):
-        a: int = pytc.field(default=1, pos_only=True)
+        a: int = pytc.field(default=1, kind="POS_ONLY")
         b: int = 2
 
     with pytest.raises(TypeError):
         # positonal only for a
         Test(a=1, b=2)
 
     assert Test(1, b=2).a == 1
     assert Test(1, 2).b == 2
 
     class Test(pytc.TreeClass):
-        a: int = pytc.field(default=1, pos_only=True)
-        b: int = pytc.field(default=2, pos_only=True)
+        a: int = pytc.field(default=1, kind="POS_ONLY")
+        b: int = pytc.field(default=2, kind="POS_ONLY")
 
     assert Test(1, 2).a == 1
     assert Test(1, 2).b == 2
 
     # keyword only
     class Test(pytc.TreeClass):
-        a: int = pytc.field(default=1, kw_only=True)
+        a: int = pytc.field(default=1, kind="KW_ONLY")
         b: int = 2
 
     with pytest.raises(TypeError):
         Test(1, 2)
 
     with pytest.raises(TypeError):
         Test(1, b=2)
 
     assert Test(a=1, b=2).a == 1
 
     class Test(pytc.TreeClass):
-        a: int = pytc.field(default=1, pos_only=True)
-        b: int = pytc.field(default=2, kw_only=True)
+        a: int = pytc.field(default=1, kind="POS_ONLY")
+        b: int = pytc.field(default=2, kind="KW_ONLY")
 
     with pytest.raises(TypeError):
         Test(1, 2)
 
     assert Test(1, b=2).b == 2
 
     with pytest.raises(TypeError):
         Test(a=1, b=2)
 
     # test when init is False
     class Test(pytc.TreeClass):
-        a: int = pytc.field(default=1, init=False, kw_only=True)
+        a: int = pytc.field(default=1, init=False, kind="KW_ONLY")
         b: int = 2
 
     with pytest.raises(TypeError):
         Test(1, 2)
 
     assert Test(b=2).a == 1
 
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1)
-        b: int = pytc.field(factory=lambda: 1)
 
         def __init__(self) -> None:
             pass
 
     with pytest.raises(AttributeError):
         Test()
 
@@ -535,12 +529,19 @@
 
     _, tree_with_weight = tree.at["add_param"]("weight", Parameter(3))
 
     assert tree_with_weight.weight == Parameter(3)
     assert "weight" not in vars(tree)
 
 
-def test_field_factory():
-    class Tree(pytc.TreeClass):
-        a: int = pytc.field(factory=lambda: 1)
+def test_partial():
+    def f(a, b, c):
+        return a + b + c
+
+    f_a = pytc.Partial(f, ..., 2, 3)
+    assert f_a(1) == 6
+
+    f_b = pytc.Partial(f, 1, ..., 3)
+    assert f_b(2) == 6
 
-    assert Tree().a == 1
+    assert f_b == f_b
+    assert hash(f_b) == hash(f_b)
```

### Comparing `pytreeclass-0.3.4/tests/test_under_jit.py` & `pytreeclass-0.3.6/tests/test_under_jit.py`

 * *Files identical despite different names*

