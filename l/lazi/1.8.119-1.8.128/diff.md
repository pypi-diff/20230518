# Comparing `tmp/lazi-1.8.119.tar.gz` & `tmp/lazi-1.8.128.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.8.119.tar", max compression
+gzip compressed data, was "lazi-1.8.128.tar", max compression
```

## Comparing `lazi-1.8.119.tar` & `lazi-1.8.128.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.8.119/LICENSE
--rw-r--r--   0        0        0     1932 2023-05-18 00:07:27.608818 lazi-1.8.119/README.md
--rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.8.119/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.8.119/lazi/conf/auto.py
--rw-r--r--   0        0        0     2079 2023-05-18 00:36:16.419385 lazi-1.8.119/lazi/conf/base.py
--rw-r--r--   0        0        0     5271 2023-05-18 00:34:04.425666 lazi-1.8.119/lazi/conf/conf.py
--rw-r--r--   0        0        0     1327 2023-05-17 06:09:50.989623 lazi-1.8.119/lazi/conf/envs.py
--rw-r--r--   0        0        0      287 2023-05-17 23:57:14.444788 lazi-1.8.119/lazi/core/__init__.py
--rw-r--r--   0        0        0     5297 2023-05-18 00:53:46.881029 lazi-1.8.119/lazi/core/finder.py
--rw-r--r--   0        0        0     5285 2023-05-18 00:54:51.789873 lazi-1.8.119/lazi/core/loader.py
--rw-r--r--   0        0        0     3837 2023-05-18 00:10:10.834956 lazi-1.8.119/lazi/core/module.py
--rw-r--r--   0        0        0     1855 2023-05-18 00:45:50.554840 lazi-1.8.119/lazi/core/spec.py
--rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.8.119/lazi/core/stat.py
--rw-r--r--   0        0        0       21 2023-05-17 06:09:37.997455 lazi-1.8.119/lazi/lazo/__init__.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.8.119/lazi/util/__init__.py
--rw-r--r--   0        0        0      801 2023-05-18 00:45:50.550840 lazi-1.8.119/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.8.119/lazi/util/functional.py
--rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.8.119/lazi/util/util.py
--rw-r--r--   0        0        0     1655 2023-05-18 00:56:28.803134 lazi-1.8.119/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.8.119/tests/__init__.py
--rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.8.119/tests/standalone/sa_array.py
--rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.8.119/tests/standalone/sa_nested.py
--rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.8.119/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.8.119/tests/test_array.py
--rw-r--r--   0        0        0      378 2023-05-17 06:09:23.165264 lazi-1.8.119/tests/test_asyncio.py
--rw-r--r--   0        0        0     1187 2023-05-18 00:16:22.071819 lazi-1.8.119/tests/test_django.py
--rw-r--r--   0        0        0     1249 2023-05-18 00:14:16.170170 lazi-1.8.119/tests/test_importlib.py
--rw-r--r--   0        0        0      199 2023-05-17 23:05:39.388245 lazi-1.8.119/tests/test_lazy.py
--rw-r--r--   0        0        0      304 2023-05-17 06:13:14.860256 lazi-1.8.119/tests/test_pygments.py
--rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.8.119/tests/test_requests.py
--rw-r--r--   0        0        0     1004 2023-05-17 07:14:47.163887 lazi-1.8.119/tests/test_rich.py
--rw-r--r--   0        0        0     1186 2023-05-18 00:24:02.109826 lazi-1.8.119/tests/test_stat.py
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 lazi-1.8.119/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.8.128/LICENSE
+-rw-r--r--   0        0        0     9889 2023-05-18 03:31:46.016263 lazi-1.8.128/README.md
+-rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.8.128/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.8.128/lazi/conf/auto.py
+-rw-r--r--   0        0        0     1935 2023-05-18 02:19:06.579567 lazi-1.8.128/lazi/conf/base.py
+-rw-r--r--   0        0        0     4708 2023-05-18 02:24:12.623535 lazi-1.8.128/lazi/conf/conf.py
+-rw-r--r--   0        0        0     1330 2023-05-18 02:20:03.676308 lazi-1.8.128/lazi/conf/envs.py
+-rw-r--r--   0        0        0      287 2023-05-17 23:57:14.444788 lazi-1.8.128/lazi/core/__init__.py
+-rw-r--r--   0        0        0     5160 2023-05-18 02:53:08.158015 lazi-1.8.128/lazi/core/finder.py
+-rw-r--r--   0        0        0     5087 2023-05-18 03:23:08.925510 lazi-1.8.128/lazi/core/loader.py
+-rw-r--r--   0        0        0     3817 2023-05-18 03:03:19.185969 lazi-1.8.128/lazi/core/module.py
+-rw-r--r--   0        0        0     1884 2023-05-18 03:03:19.185969 lazi-1.8.128/lazi/core/spec.py
+-rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.8.128/lazi/core/stat.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.8.128/lazi/util/__init__.py
+-rw-r--r--   0        0        0      822 2023-05-18 03:21:34.884282 lazi-1.8.128/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.8.128/lazi/util/functional.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.8.128/lazi/util/util.py
+-rw-r--r--   0        0        0     1655 2023-05-18 03:38:10.145256 lazi-1.8.128/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.8.128/tests/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.8.128/tests/standalone/sa_array.py
+-rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.8.128/tests/standalone/sa_nested.py
+-rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.8.128/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.8.128/tests/test_array.py
+-rw-r--r--   0        0        0      378 2023-05-17 06:09:23.165264 lazi-1.8.128/tests/test_asyncio.py
+-rw-r--r--   0        0        0     1187 2023-05-18 00:16:22.071819 lazi-1.8.128/tests/test_django.py
+-rw-r--r--   0        0        0     1251 2023-05-18 01:33:30.900017 lazi-1.8.128/tests/test_importlib.py
+-rw-r--r--   0        0        0      230 2023-05-18 01:11:43.475022 lazi-1.8.128/tests/test_lazy.py
+-rw-r--r--   0        0        0      307 2023-05-18 01:33:30.888016 lazi-1.8.128/tests/test_pygments.py
+-rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.8.128/tests/test_requests.py
+-rw-r--r--   0        0        0     1004 2023-05-17 07:14:47.163887 lazi-1.8.128/tests/test_rich.py
+-rw-r--r--   0        0        0     1200 2023-05-18 01:33:30.900017 lazi-1.8.128/tests/test_stat.py
+-rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 lazi-1.8.128/PKG-INFO
```

### Comparing `lazi-1.8.119/LICENSE` & `lazi-1.8.128/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.8.119/lazi/conf/base.py` & `lazi-1.8.128/lazi/conf/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 #
 TRACE: int = 0                          # Enable debug traces. Currently using levels 0-4.
 #                                       # - Tracing relies on __debug__ and asserts, so -O will disable completely.
 AUTO_AUTO: bool = True                  # Automatically install when importing lazi.auto.
 CORE_AUTO: bool = False                 # Automatically install when importing lazi.core.
 #
 NO_HOOK: bool = False                   # Disable all spec loader hooks.
+NO_LAZY: bool = False                   # Hook loaders, but skip lazy loading.
 NO_HOOK_STD: bool = False               # Disable spec loader hooking for stdlib modules.
 NO_HOOK_BI: bool = False                # Disable spec loader hooking for built-in modules.
-NO_LAZY_LOAD: bool = False              # Next call to exec_module() skips lazy loading.
 #
 INVAL_SOFT: bool = False                # Keep modules in sys.modules after cache invalidation.
 INVAL_GC: bool = (not INVAL_SOFT)       # Enable garbage collection on cache invalidation.
 #                                       # - Only makes sense if INVAL_SOFT is False.
 #
 #
 CONF_NO_CACHING: bool | None = None     # Disable caching of conf vars.
 #                                         - None: Use the default caching behavior, which will disable
 #                                                 caching if `lazi.core` is already present in sys.modules
 #                                                 when lazi.conf.conf is imported.
 #
-CONF_KEYS: set = {                      # Configuration keys that are allowed to be set.
-    key for key in globals()            # - Can be inherited / changed, but support is untested.
-    if not key.startswith("_")          # - envs.py does not support anything other than this base value,
-    and key.isupper()                   # along with __meta__["keys"] and __meta__["root"] as a prefix (TBD).
-}
+__all__: list = [                       # Configuration keys that are allowed to be set.
+    key for key in globals()            # - Not inherited or mutable.
+    if not key.startswith("_")          # - Can be supplemented from __meta__['keys'].
+    and key.isupper()
+]
```

### Comparing `lazi-1.8.119/lazi/conf/conf.py` & `lazi-1.8.128/lazi/conf/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,29 +57,28 @@
 
     __root__: ModuleType = _import_module(base.__meta__["root"])
     __conf__: ModuleType = _import_module(f"{__root__.__name__}.{__name__.rpartition('.')[-1]}")
 
     __core__: str = f"{__root__.__name__}.{base.__meta__.get('core', 'core')}"
     __auto__: str = f"{__conf__.__name__}.{base.__meta__.get('auto', 'auto')}"
 
-    __keys__: set = {"CONF_KEYS"} | CONF_KEYS | base.__meta__.get("keys", set())
+    __keys__: set = set(base.__all__) | set(base.__meta__.get("keys", set()))
 
     conf: dict[str, object | EllipsisType] = {key: ... for key in __keys__}
 
     __mods: dict[str, ModuleType] = base.__meta__.get("mods", {})
     __CONF_NO_CACHING: bool = base.__meta__.get("CONF_NO_CACHING", __core__ in _sys.modules)
     __CONF_NO_CACHING_DFL: bool = __CONF_NO_CACHING
 
     def __init__(self):
         super().__init__(__name__)
         self.__conf__.__getattr__ = lambda attr: getattr(self, attr)
         if (conf_no_caching := self.CONF_NO_CACHING) is not None:
             self.__CONF_NO_CACHING = conf_no_caching
         self.CONF_NO_CACHING = self.__CONF_NO_CACHING
-        self.CONF_KEYS = self.__keys__
 
     def __iter__(self) -> Iterator[tuple[str, object]]:
         return ((key, getattr(self, key)) for key in self.conf)
 
     def get(self) -> dict:
         return dict(self)
 
@@ -96,55 +95,44 @@
 
     def __mods__(self) -> Iterator[ModuleInfo]:
         return (
             mi for mi in _iter_modules(self.__conf__.__path__, self.__conf__.__name__ + ".")
             if mi.name not in {self.__root__.__name__, self.base.__name__, self.__auto__, self.__name__}
         )
 
-    def __getattr__(self, attr) -> object:
+    def __getattr__(self, attr: str) -> object:
 
-        if (value := self.conf.get(attr, miss := AttributeError())) is miss:
+        if (value := self.conf.get(attr, miss := object())) is miss:
             raise AttributeError(f"Module {__name__!r} has no attribute {attr!r}")
 
         elif value is ...:
             value = getattr(self.base, attr)
 
             for mi in self.__mods__():
                 if (mod := self.__mods.get(mi.name, miss)) is miss:
                     mod = _import_module(mi.name)
                     if not self.__CONF_NO_CACHING:
                         self.__mods[mi.name] = mod
 
                 value = getattr(mod, attr, value)
 
-            value = self.__setattr__(attr, value)
+            self.__setattr__(attr, value)
 
         return value
 
-    def __setattr__(self, key, value) -> object:
-        if key.startswith("_"):
-            super().__setattr__(key, value)
-            return value
+    def __setattr__(self, attr: str, value: object) -> None:
+        if attr.startswith("_") or not attr.isupper():
+            super().__setattr__(attr, value)
+            return
 
-        if key not in self.conf and key != "CONF_KEYS" and key not in self.CONF_KEYS:
-            raise AttributeError(f"Conf key {key!r} is not defined.")
+        if attr not in self.conf:
+            raise AttributeError(f"Conf key {attr!r} is not defined.")
         if not self.__CONF_NO_CACHING:
-
-            if key == "CONF_KEYS" and value is not self.__keys__:
-                self.__all__ = list(set(self.__all__) | set(value))
-                for conf_key in (_ for _ in dict(self.conf) if _ != "CONF_KEYS" and _ not in value):
-                    del self.conf[conf_key]
-                for conf_key in (_ for _ in value if _ != "CONF_KEYS" and _ not in self.conf):
-                    self.conf[conf_key] = ...
-                self.conf["CONF_KEYS"] = value
-
-            self.conf[key] = value
-            super().__setattr__(key, value)
-
-        return value
+            self.conf[attr] = value
+            super().__setattr__(attr, value)
 
 
 _sys.modules[__name__] = Conf()  # Replace module with instance.
 
 __all__.extend(_sys.modules[__name__].__keys__)
 
 del ModuleType, EllipsisType, Iterator, ModuleInfo
```

### Comparing `lazi-1.8.119/lazi/conf/envs.py` & `lazi-1.8.128/lazi/conf/envs.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 continue
     return _type_map[typp](valu)
 
 
 def load():
     from lazi.conf import base
     typd: dict[str, type] = _typing.get_type_hints(base)
-    keys: set[str] = base.CONF_KEYS | base.__meta__.get("keys", set())
+    keys: set[str] = set(base.__all__) | base.__meta__.get("keys", set())
 
     for key in (_ for _ in keys if _ in _os.environ and _ in typd):
         if (value := _os.getenv(key, no := object())) is not no:
             globals()[key] = parse_item(typd[key], value)
 
 
 load()
```

### Comparing `lazi-1.8.119/lazi/core/finder.py` & `lazi-1.8.128/lazi/core/finder.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def __del__(self):
         try:
             if self in self.__finders__:
                 self.__finders__.remove(self)
                 self.invalidate_caches()
         except Exception as e:
-            assert None is debug.log(
+            assert None is debug.info(
                 f"[{id(self)}] DEL! {self.__class__.__name__} !!!! {type(e).__name__}: {e}"
             )
 
     def __enter__(self) -> Finder:
         if self not in sys.meta_path:
             assert self.__refs == 0, self.__refs
             assert None is debug.traced(
@@ -118,32 +118,33 @@
             else:
                 if path is not None:
                     spec.path = path
                 if target is not None:
                     spec.target = target
 
             assert None is debug.traced(
-                1 if (target := spec.target) is None else 0,  # NB: Alters state in assert, do not use variable later.
-                f"[{id(self)}] FIND {spec.loader_state} {spec.f_name} "
-                f"[{Path(c).suffix[1:] if (c:=spec.cached) else Path(o).suffix[1:] if (o:=spec.origin) else '-'}] "
-                f"[{id(target) if target is not None else '-'}] {'S' if spec.stdlib else ''}{'B' if spec.builtin else ''} "
+                1,
+                f"[{id(self)}] FIND " +
+                ((Path(c).suffix[1:] if (c := spec.cached) else Path(o).suffix[1:] if (o := spec.origin) else '?') +
+                    f"{'S' if spec.stdlib else ''}{'B' if spec.builtin else ''}").ljust(5) +
+                spec.f_name
             )
 
             return spec
 
     def _find_spec(self, name: str, path: list[str] | None, target: ModuleType | None) -> ModuleSpec | None:
         for finder in (_ for _ in sys.meta_path if _ is not self):
             if (spec := finder.find_spec(name, path, target)) is not None:
                 return spec
 
     def invalidate_caches(self) -> None:
         if not INVAL_SOFT:
             while self.specs and (spec := self.specs.popitem()[1]):
                 if hasattr(spec.loader, "invalidate_caches"):
-                    spec.loader.invalidate_caches(spec)
+                    spec.loader.invalidate_caches()
         else:
             self.specs.clear()
 
         if INVAL_GC:
             gc.collect()
```

### Comparing `lazi-1.8.119/lazi/core/loader.py` & `lazi-1.8.128/lazi/core/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from lazi.util import debug
 
 __all__ = "Loader",
 
 Spec = ForwardRef("Spec")
 Module = ForwardRef("Module")
 
-NO_LAZY_LOAD = conf.NO_LAZY_LOAD
+NO_LAZY = conf.NO_LAZY
 
 
 class Loader(_Loader):
     spec: Spec
     loader: _Loader
     __busy: bool = False
     __forc: bool = False
@@ -55,30 +55,27 @@
         try:
             target = spec.target if spec.target is not None else self.loader.create_module(spec)
             target = ModuleType(spec.name) if target is None else target
             target = spec.finder.Module(spec, target) if not isinstance(target, spec.finder.Module) else target
 
             spec.loader_state = Loader.State.CREA
 
-            if NO_LAZY_LOAD:  # or spec.s_path is None:  # Consider whether spec is a package?
+            if NO_LAZY:  # or spec.s_path is None:  # Consider whether spec is a package?
                 self.__forc = True
 
             modules[spec.name] = target
 
             return target
 
         finally:
             self.__busy = False
 
-    def exec_module(self, module: Module, spec: Spec | None = None, force: bool | None = None, /):
-        spec = spec if spec is not None else self.spec
-        lazy = not (force if force is not None else self.__forc)
-
-        assert spec is module.__spec__, (spec, module.__spec__)
-        assert spec.loader is self, (spec.loader, self)
+    def exec_module(self, module: Module, force: bool | None = None, /):
+        spec = self.spec
+        lazy = not ((force or self.__forc) if force is not None else self.__forc)
 
         name = spec.name
         name_ = spec.f_name
         state = spec.loader_state
         nexts = Loader.State.LAZY if lazy else Loader.State.EXEC
         target = spec.target
 
@@ -117,15 +114,15 @@
                 1,  # if nexts is Loader.State.LOAD else 2,
                 f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_} "
                 f"++++ "
             )
 
         except Exception as e:
             spec.loader_state = nexts = Loader.State.DEAD
-            assert None is debug.log(
+            assert None is getattr(debug, "info" if isinstance(e, ImportError) else "exception")(
                 f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_}\n" +
                 " " * 18 + f"!!!! {type(e).__name__}: {e}"
             )
             raise
 
         if (mod := modules.get(name)) is not module and mod is not None:
             assert None is debug.trace(
@@ -133,24 +130,23 @@
                 f"::[{id(mod) if mod is not target else 'same' if mod is not None else '-'}] "
                 "(after)"
             )
 
             spec.target = target = mod
             modules[name] = module
 
-        # if nexts is Loader.State.LOAD and target is not None:
-        #     modules[name] = target
+    def invalidate_caches(self) -> None:
+        spec = self.spec
 
-    def invalidate_caches(self, spec: Spec | None = None) -> None:
-        spec = spec if spec is not None else self.spec
-        module = modules.pop(spec.name, None)
+        if (mod := modules.get(spec.name)) is spec.target and mod is not None:
+            del modules[spec.name]
 
         assert None is debug.traced(
             1,
-            f"[{id(module) if module else '*'*15}] "
+            f"[{id(mod) if mod is not None else '*'*15}] "
             f"{spec.loader_state} DEAD [{id(spec.target) if spec.target else '*'*15}] {spec.f_name}"
         )
 
         spec.loader = self.loader
         spec.loader_state = None  # type: ignore
         spec.target = None
         self.__forc = False
```

### Comparing `lazi-1.8.119/lazi/core/module.py` & `lazi-1.8.128/lazi/core/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,51 +54,51 @@
         if (target := getattr(spec, "target", None)) is None:
             if attr == "__spec__":
                 return spec
             return super().__getattribute__(attr)
 
         assert None is debug.traced(
             3, f"[{id(self)}] {spec.loader_state} **** [{id(target) if target is not None else '*' * 15}] "
-               f"{spec.f_name}[.{attr}]"
+               f"{spec.f_name} {attr}"
         )
 
         if attr in GETATTR_PASS and (index := GETATTR_PASS.index(attr)) >= 0:
             return spec if not index else target.__getattribute__(attr)
 
         if attr in MODULE_SPEC_ATTR_MAP:
             return target.__getattribute__(attr)
 
         if spec.loader_state.value <= spec.loader.State.LAZY.value:
             assert None is debug.trace(
                 f"[{id(self)}] {spec.loader_state} >>>> [{id(target) if target is not None else '*' * 15}] "
-                f"{spec.f_name}[.{attr}]"
+                f"{spec.f_name} {attr}"
             )
-            spec.loader.exec_module(self, spec, True)
+            spec.loader.exec_module(self, True)
 
         return spec.target.__getattribute__(attr)  # NB: Don't use `target` here, as it may have changed.
 
     def __setattr__(self, attr, valu):
         if attr == "__spec__":
             if (target := getattr(valu, "target", None)) is not None:
                 target.__setattr__(attr, valu)
             return super().__setattr__(attr, valu)
 
         spec = super().__getattribute__("__spec__")
 
         assert None is debug.traced(
             3, f"[{id(self)}] {spec.loader_state} %%%% [{id(spec.target) if spec.target is not None else '*' * 15}] "
-               f"{spec.f_name}[.{attr}] = [{id(valu)}]"
+               f"{spec.f_name} {attr} = [{id(valu)}]"
         )
 
         if (target := getattr(spec, "target", None)) is None:
             return super().__setattr__(attr, valu)
 
         if attr not in SETATTR_PASS and spec.loader_state.value <= spec.loader.State.LAZY.value:
             assert None is debug.trace(
                 f"[{id(self)}] {spec.loader_state} <<<< [{id(target) if target is not None else '*' * 15}] "
-                f"{spec.f_name}[.{attr}] = [{id(valu)}]"
+                f"{spec.f_name} {attr} = [{id(valu)}]"
             )
 
             target.__setattr__(attr, valu)  # Preload the variable? Yes: Fixes stdlib (asyncio.coroutines) errors in README.md.
-            spec.loader.exec_module(self, spec, True)
+            spec.loader.exec_module(self, True)
 
         spec.target.__setattr__(attr, valu)  # NB: Don't use `target` here, as it may have changed.
```

### Comparing `lazi-1.8.119/lazi/core/spec.py` & `lazi-1.8.128/lazi/core/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     loader: Loader
     s_path: list[str] | None
     target: ModuleType | None
 
     stdlib: bool = cached_property(lambda self: self.origin and STDLIB_PATH in Path(self.origin).parents)
     builtin: bool = cached_property(lambda self: self.origin == "built-in")
 
-    _f_name = lambda self, wrap=lambda _, __: f"[{_}.]{__}": (
+    _f_name = lambda self, wrap=lambda _, __: f"{_}|{__.replace(f'{_}.', '', 1)}": (
         wrap(parent, name) if (name := self.name) != (parent := self.parent) and parent else name
     )
 
-    f_name: str | None = property(lambda self: self._f_name())
+    f_name: str | None = cached_property(lambda self: self._f_name())
 
     def __init__(self, finder: Finder, spec: ModuleSpec, path: list[str] | None = None, target: ModuleType | None = None):
         self.finder = finder
         self.s_path = path
         self.target = target
 
         super().__init__(
```

### Comparing `lazi-1.8.119/lazi/core/stat.py` & `lazi-1.8.128/lazi/core/stat.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.119/lazi/util/debug.py` & `lazi-1.8.128/lazi/util/debug.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from contextlib import contextmanager
 import logging
 
 from lazi.conf import conf
 
-__all__ = "trace", "traced", "log", "track"
+__all__ = "trace", "traced", "info", "track"
 
-TRACE = conf.TRACE
 
+info = logging.info
+exception = logging.exception
+
+TRACE = conf.TRACE
 
 if __debug__ and TRACE:
 
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(message)s",
     )
 
     traced = lambda at, /, *args, **kwds: logging.debug(*args, **kwds) if TRACE > at else None  # noqa
     trace = lambda *args, **kwds: traced(0, *args, **kwds)
 
 else:
     traced = lambda at, /, *args, **kwds: None
     trace = lambda *args, **kwds: None
-    init_pretty = lambda: None
-
-log = logging.info
 
 
 @contextmanager
-def track(msg: str):
+def track(msg: str, log=info, exc=info):
     log(f"... {msg} ...")
     try:
         yield
     except Exception as e:
-        log(_log := f"!!! {msg} !!! {type(e).__name__}: {e}")
+        exc(_log := f"!!! {msg} !!! {type(e).__name__}: {e}")
         raise
     else:
         log(f"^^^ {msg} ^^^")
```

### Comparing `lazi-1.8.119/pyproject.toml` & `lazi-1.8.128/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.8.119"
+version = "1.8.128"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
```

### Comparing `lazi-1.8.119/tests/standalone/sa_nested.py` & `lazi-1.8.128/tests/standalone/sa_nested.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.119/tests/test_django.py` & `lazi-1.8.128/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.119/tests/test_importlib.py` & `lazi-1.8.128/tests/test_importlib.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,21 +11,21 @@
     (None, "idna", "requests.packages", ModuleType),
     ("TestCase", "django.test", None, ModuleType),
     (None, "test", "django", ModuleType),
     (None, "pandas.core.nanops", None, ModuleType),
     (None, "django.db.models.aggregates", "django.db.", ModuleType),
 ])
 def test_import_module(attr, name, package, expected_type):
-    from lazi.util.debug import track, log
+    from lazi.util.debug import track, info
     from lazi.core import lazi
 
     with lazi, track(f"import {name}{f'[.{attr}]' if attr else ''}"):
         if issubclass(expected_type, Exception):
             with pytest.raises(expected_type):
                 importlib.import_module(name, package)
         else:
             module = importlib.import_module(name, package)
             if attr is not None:
                 with track(f"getattr({name}, {attr})"):
                     value = getattr(module, attr)
-                    log(f"value: {repr(value)}")
+                    info(f"value: {repr(value)}")
             assert issubclass(type(module), expected_type)
```

### Comparing `lazi-1.8.119/tests/test_requests.py` & `lazi-1.8.128/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.119/tests/test_rich.py` & `lazi-1.8.128/tests/test_rich.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.119/tests/test_stat.py` & `lazi-1.8.128/tests/test_stat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import pytest
 
 
 def test_stat_django_test():
-    from lazi.util.debug import track, log
+    from lazi.util.debug import track, info
 
     from lazi.core.stat import Stat
     from lazi.core import lazi
 
     with lazi:
         with track("import django.test"):
-            log(Stat())
+            info(Stat())
             import django.test as dt
-            log(Stat())
+            info(Stat())
 
         with track("TestCase = dt.TestCase"):
             TestCase = dt.TestCase
-            log(Stat())
+            info(Stat())
 
 
-@pytest.mark.skip(reason="not working")
+# @pytest.mark.skip(reason="not working")
 def test_stat_presto():
-    from lazi.util.debug import track, log
+    from lazi.util.debug import track, info
 
     from lazi.core.stat import Stat
     from lazi.core import lazi
 
     with lazi:
         with track("import presto"):
-            log(Stat())
+            info(Stat())
             from presto import Presto
-            log(Stat())
+            info(Stat())
 
         with track("p = Presto('https://httpbin.org')"):
             p = Presto("https://httpbin.org")
-            log(Stat())
+            info(Stat())
 
 
 def test_stat_nolazi_presto():
-    from lazi.util.debug import track, log
+    from lazi.util.debug import track, info
 
     from lazi.core.stat import Stat
 
     with track("import presto"):
-        log(Stat())
+        info(Stat())
         from presto import Presto
-        log(Stat())
+        info(Stat())
 
     with track("p = Presto('https://httpbin.org')"):
         p = Presto("https://httpbin.org")
-        log(Stat())
+        info(Stat())
```

