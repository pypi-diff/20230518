# Comparing `tmp/lazi-1.7.87.tar.gz` & `tmp/lazi-1.8.119.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.7.87.tar", max compression
+gzip compressed data, was "lazi-1.8.119.tar", max compression
```

## Comparing `lazi-1.7.87.tar` & `lazi-1.8.119.tar`

### file list

```diff
@@ -1,28 +1,33 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.7.87/LICENSE
--rw-r--r--   0        0        0     1913 2023-05-16 03:20:51.902303 lazi-1.7.87/README.md
--rw-r--r--   0        0        0      166 2023-05-16 09:03:05.840594 lazi-1.7.87/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.7.87/lazi/conf/auto.py
--rw-r--r--   0        0        0     1464 2023-05-16 09:36:44.515049 lazi-1.7.87/lazi/conf/base.py
--rw-r--r--   0        0        0     4738 2023-05-15 22:42:51.727662 lazi-1.7.87/lazi/conf/conf.py
--rw-r--r--   0        0        0       99 2023-05-15 22:42:51.727662 lazi-1.7.87/lazi/conf/test.py
--rw-r--r--   0        0        0      295 2023-05-16 07:44:18.361362 lazi-1.7.87/lazi/core/__init__.py
--rw-r--r--   0        0        0     4049 2023-05-16 09:57:14.887124 lazi-1.7.87/lazi/core/finder.py
--rw-r--r--   0        0        0     3977 2023-05-16 10:05:55.785938 lazi-1.7.87/lazi/core/loader.py
--rw-r--r--   0        0        0     2625 2023-05-16 09:54:40.373106 lazi-1.7.87/lazi/core/module.py
--rw-r--r--   0        0        0     1434 2023-05-16 05:37:58.378560 lazi-1.7.87/lazi/core/spec.py
--rw-r--r--   0        0        0     2429 2023-05-16 09:05:13.038270 lazi-1.7.87/lazi/core/stat.py
--rw-r--r--   0        0        0       21 2023-05-16 07:53:56.744459 lazi-1.7.87/lazi/lazo/__init__.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.7.87/lazi/util/__init__.py
--rw-r--r--   0        0        0      448 2023-05-15 22:42:51.727662 lazi-1.7.87/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.7.87/lazi/util/functional.py
--rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.7.87/lazi/util/util.py
--rw-r--r--   0        0        0     1555 2023-05-16 10:08:39.284111 lazi-1.7.87/pyproject.toml
--rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.7.87/tests/standalone/sa_array.py
--rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.7.87/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.7.87/tests/test_array.py
--rw-r--r--   0        0        0      378 2023-05-16 06:33:09.290071 lazi-1.7.87/tests/test_asyncio.py
--rw-r--r--   0        0        0     1206 2023-05-16 09:44:09.484866 lazi-1.7.87/tests/test_django.py
--rw-r--r--   0        0        0      361 2023-05-16 09:40:27.189960 lazi-1.7.87/tests/test_pygments.py
--rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.7.87/tests/test_requests.py
--rw-r--r--   0        0        0     1956 2023-05-16 09:40:27.205960 lazi-1.7.87/tests/test_rich.py
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 lazi-1.7.87/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.8.119/LICENSE
+-rw-r--r--   0        0        0     1932 2023-05-18 00:07:27.608818 lazi-1.8.119/README.md
+-rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.8.119/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.8.119/lazi/conf/auto.py
+-rw-r--r--   0        0        0     2079 2023-05-18 00:36:16.419385 lazi-1.8.119/lazi/conf/base.py
+-rw-r--r--   0        0        0     5271 2023-05-18 00:34:04.425666 lazi-1.8.119/lazi/conf/conf.py
+-rw-r--r--   0        0        0     1327 2023-05-17 06:09:50.989623 lazi-1.8.119/lazi/conf/envs.py
+-rw-r--r--   0        0        0      287 2023-05-17 23:57:14.444788 lazi-1.8.119/lazi/core/__init__.py
+-rw-r--r--   0        0        0     5297 2023-05-18 00:53:46.881029 lazi-1.8.119/lazi/core/finder.py
+-rw-r--r--   0        0        0     5285 2023-05-18 00:54:51.789873 lazi-1.8.119/lazi/core/loader.py
+-rw-r--r--   0        0        0     3837 2023-05-18 00:10:10.834956 lazi-1.8.119/lazi/core/module.py
+-rw-r--r--   0        0        0     1855 2023-05-18 00:45:50.554840 lazi-1.8.119/lazi/core/spec.py
+-rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.8.119/lazi/core/stat.py
+-rw-r--r--   0        0        0       21 2023-05-17 06:09:37.997455 lazi-1.8.119/lazi/lazo/__init__.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.8.119/lazi/util/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-18 00:45:50.550840 lazi-1.8.119/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.8.119/lazi/util/functional.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.8.119/lazi/util/util.py
+-rw-r--r--   0        0        0     1655 2023-05-18 00:56:28.803134 lazi-1.8.119/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.8.119/tests/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.8.119/tests/standalone/sa_array.py
+-rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.8.119/tests/standalone/sa_nested.py
+-rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.8.119/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.8.119/tests/test_array.py
+-rw-r--r--   0        0        0      378 2023-05-17 06:09:23.165264 lazi-1.8.119/tests/test_asyncio.py
+-rw-r--r--   0        0        0     1187 2023-05-18 00:16:22.071819 lazi-1.8.119/tests/test_django.py
+-rw-r--r--   0        0        0     1249 2023-05-18 00:14:16.170170 lazi-1.8.119/tests/test_importlib.py
+-rw-r--r--   0        0        0      199 2023-05-17 23:05:39.388245 lazi-1.8.119/tests/test_lazy.py
+-rw-r--r--   0        0        0      304 2023-05-17 06:13:14.860256 lazi-1.8.119/tests/test_pygments.py
+-rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.8.119/tests/test_requests.py
+-rw-r--r--   0        0        0     1004 2023-05-17 07:14:47.163887 lazi-1.8.119/tests/test_rich.py
+-rw-r--r--   0        0        0     1186 2023-05-18 00:24:02.109826 lazi-1.8.119/tests/test_stat.py
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 lazi-1.8.119/PKG-INFO
```

### Comparing `lazi-1.7.87/LICENSE` & `lazi-1.8.119/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.7.87/lazi/conf/base.py` & `lazi-1.8.119/lazi/conf/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 """Base project configuration.
 """
 __meta__ = dict(                        # Internal configuration for <root>.conf.conf (cannot override elsewhere).
     root="lazi",                        # - Root namespace package name.
 )                                       # See conf.py for more options.
 #
-DEBUG_TRACING: int = 0                  # Enable debug traces. Currently using levels 0-4.
+TRACE: int = 0                          # Enable debug traces. Currently using levels 0-4.
+#                                       # - Tracing relies on __debug__ and asserts, so -O will disable completely.
+AUTO_AUTO: bool = True                  # Automatically install when importing lazi.auto.
+CORE_AUTO: bool = False                 # Automatically install when importing lazi.core.
+#
+NO_HOOK: bool = False                   # Disable all spec loader hooks.
+NO_HOOK_STD: bool = False               # Disable spec loader hooking for stdlib modules.
+NO_HOOK_BI: bool = False                # Disable spec loader hooking for built-in modules.
+NO_LAZY_LOAD: bool = False              # Next call to exec_module() skips lazy loading.
+#
+INVAL_SOFT: bool = False                # Keep modules in sys.modules after cache invalidation.
+INVAL_GC: bool = (not INVAL_SOFT)       # Enable garbage collection on cache invalidation.
+#                                       # - Only makes sense if INVAL_SOFT is False.
 #
-LAZI_AUTO_INSTALL: bool = True          # Automatically install when importing lazi.auto.
-CORE_AUTO_INSTALL: bool = False         # Automatically install when importing lazi.core.
-FORCE_LOAD_MODULE: bool = False         # Immediately call exec_module() on imported modules.
-NO_STDLIB_MODULES: bool = False          # Disable loader hooking for stdlib modules.
-DISABLE_LOAD_HOOK: bool = False         # Disable all loader hooks.
-SOFT_INVALIDATION: bool = False         # Keep modules in sys.modules after cache invalidation.
-GARBAG_COLLECTION: bool = (             # Enable garbage collection on cache invalidation.
-    not SOFT_INVALIDATION)              # - Only makes sense if SOFT_INVALIDATION is False.
 #
 CONF_NO_CACHING: bool | None = None     # Disable caching of conf vars.
 #                                         - None: Use the default caching behavior, which will disable
 #                                                 caching if `lazi.core` is already present in sys.modules
 #                                                 when lazi.conf.conf is imported.
+#
+CONF_KEYS: set = {                      # Configuration keys that are allowed to be set.
+    key for key in globals()            # - Can be inherited / changed, but support is untested.
+    if not key.startswith("_")          # - envs.py does not support anything other than this base value,
+    and key.isupper()                   # along with __meta__["keys"] and __meta__["root"] as a prefix (TBD).
+}
```

### Comparing `lazi-1.7.87/lazi/conf/conf.py` & `lazi-1.8.119/lazi/conf/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 - Any value that is also defined in base.py will be overwritten by the value in the module.
 - Configuration values will be accessible from the conf namespace package.
 - The import order of the modules determines the resulting configuration.
 
 Use like this (recommended for package mdules):
 
 >>> from lazi.conf import conf
->>> conf.DEBUG_TRACING
+>>> conf.TRACE
 
 Or like this (recommended for client modules):
 
 >>> import lazi.conf.auto
->>> lazi.conf.DEBUG_TRACING
+>>> lazi.conf.TRACE
 >>> from lazi.conf import auto
->>> auto.DEBUG_TRACING
+>>> auto.TRACE
 
 But not like this:
 
 >>> import lazi.conf        # This is not the same as the above.
 >>> from lazi import conf   # Still no worky. Only imports the namespace module without loading.
 """
 import sys as _sys
@@ -41,16 +41,15 @@
 
 base: ModuleType
 
 __root__: ModuleType        # <meta: root>
 __conf__: ModuleType        # <root>.conf
 __core__: str               # <root>.<meta: core>
 __auto__: str               # <conf>.<meta: auto>
-
-__keys__: set = {key for key in globals() if not key.startswith("_") and key.isupper()}
+__keys__: set               # <meta: keys>
 
 conf: dict
 
 
 class Conf(ModuleType):
     __all__ = __all__
 
@@ -58,28 +57,29 @@
 
     __root__: ModuleType = _import_module(base.__meta__["root"])
     __conf__: ModuleType = _import_module(f"{__root__.__name__}.{__name__.rpartition('.')[-1]}")
 
     __core__: str = f"{__root__.__name__}.{base.__meta__.get('core', 'core')}"
     __auto__: str = f"{__conf__.__name__}.{base.__meta__.get('auto', 'auto')}"
 
-    __keys__: set = {key for key in globals() if not key.startswith("_") and key.isupper()}
+    __keys__: set = {"CONF_KEYS"} | CONF_KEYS | base.__meta__.get("keys", set())
 
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
+        self.CONF_KEYS = self.__keys__
 
     def __iter__(self) -> Iterator[tuple[str, object]]:
         return ((key, getattr(self, key)) for key in self.conf)
 
     def get(self) -> dict:
         return dict(self)
 
@@ -93,15 +93,15 @@
                 delattr(_sys.modules[self.__auto__], key)
 
         self.__CONF_NO_CACHING = self.__CONF_NO_CACHING_DFL
 
     def __mods__(self) -> Iterator[ModuleInfo]:
         return (
             mi for mi in _iter_modules(self.__conf__.__path__, self.__conf__.__name__ + ".")
-            if mi.name not in (self.__auto__, self.base.__name__, __name__)
+            if mi.name not in {self.__root__.__name__, self.base.__name__, self.__auto__, self.__name__}
         )
 
     def __getattr__(self, attr) -> object:
 
         if (value := self.conf.get(attr, miss := AttributeError())) is miss:
             raise AttributeError(f"Module {__name__!r} has no attribute {attr!r}")
 
@@ -121,20 +121,30 @@
         return value
 
     def __setattr__(self, key, value) -> object:
         if key.startswith("_"):
             super().__setattr__(key, value)
             return value
 
-        if key not in self.conf:
+        if key not in self.conf and key != "CONF_KEYS" and key not in self.CONF_KEYS:
             raise AttributeError(f"Conf key {key!r} is not defined.")
         if not self.__CONF_NO_CACHING:
+
+            if key == "CONF_KEYS" and value is not self.__keys__:
+                self.__all__ = list(set(self.__all__) | set(value))
+                for conf_key in (_ for _ in dict(self.conf) if _ != "CONF_KEYS" and _ not in value):
+                    del self.conf[conf_key]
+                for conf_key in (_ for _ in value if _ != "CONF_KEYS" and _ not in self.conf):
+                    self.conf[conf_key] = ...
+                self.conf["CONF_KEYS"] = value
+
             self.conf[key] = value
             super().__setattr__(key, value)
+
         return value
 
 
 _sys.modules[__name__] = Conf()  # Replace module with instance.
 
-__all__.extend(__keys__)
+__all__.extend(_sys.modules[__name__].__keys__)
 
 del ModuleType, EllipsisType, Iterator, ModuleInfo
```

### Comparing `lazi-1.7.87/lazi/core/module.py` & `lazi-1.8.119/lazi/core/module.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     __package__: str
     __spec__: Spec
 
     def __init__(self, spec: Spec, module: ModuleType):
         super().__init__(spec.name)
         self.__spec__ = module.__spec__ = spec
         spec.target = module
+        self.__spec__ = spec
 
         for module_attr, attr in MODULE_SPEC_ATTR_MAP.items():
             match attr:
                 case "__file__":
                     if spec.has_location:
                         module.__file__ = spec.origin
                 case "__cached__":
@@ -46,32 +47,58 @@
                         module.__path__ = spec.submodule_search_locations
                 case _:
                     setattr(module, module_attr, getattr(spec, attr))
 
     def __getattribute__(self, attr):
         spec = super().__getattribute__("__spec__")
 
-        assert None is debug.traced(3, f"[{id(self)}] <GET>  {spec.loader_state} {spec.name}[.{attr}]")
+        if (target := getattr(spec, "target", None)) is None:
+            if attr == "__spec__":
+                return spec
+            return super().__getattribute__(attr)
+
+        assert None is debug.traced(
+            3, f"[{id(self)}] {spec.loader_state} **** [{id(target) if target is not None else '*' * 15}] "
+               f"{spec.f_name}[.{attr}]"
+        )
 
         if attr in GETATTR_PASS and (index := GETATTR_PASS.index(attr)) >= 0:
-            return spec if not index else getattr(spec.target, attr)
+            return spec if not index else target.__getattribute__(attr)
 
         if attr in MODULE_SPEC_ATTR_MAP:
-            return getattr(spec.target, attr)
+            return target.__getattribute__(attr)
 
         if spec.loader_state.value <= spec.loader.State.LAZY.value:
-            assert None is debug.trace(f"[{id(self)}] <get>  {spec.loader_state} {spec.name}[.{attr}]")
+            assert None is debug.trace(
+                f"[{id(self)}] {spec.loader_state} >>>> [{id(target) if target is not None else '*' * 15}] "
+                f"{spec.f_name}[.{attr}]"
+            )
             spec.loader.exec_module(self, spec, True)
 
-        return getattr(spec.target, attr)
+        return spec.target.__getattribute__(attr)  # NB: Don't use `target` here, as it may have changed.
 
     def __setattr__(self, attr, valu):
         if attr == "__spec__":
+            if (target := getattr(valu, "target", None)) is not None:
+                target.__setattr__(attr, valu)
             return super().__setattr__(attr, valu)
 
         spec = super().__getattribute__("__spec__")
 
-        setattr(spec.target, attr, valu)
+        assert None is debug.traced(
+            3, f"[{id(self)}] {spec.loader_state} %%%% [{id(spec.target) if spec.target is not None else '*' * 15}] "
+               f"{spec.f_name}[.{attr}] = [{id(valu)}]"
+        )
+
+        if (target := getattr(spec, "target", None)) is None:
+            return super().__setattr__(attr, valu)
 
         if attr not in SETATTR_PASS and spec.loader_state.value <= spec.loader.State.LAZY.value:
-            assert None is debug.trace(f"[{id(self)}] <set>  {spec.loader_state} {spec.name}[.{attr}] [{id(valu)}]")
+            assert None is debug.trace(
+                f"[{id(self)}] {spec.loader_state} <<<< [{id(target) if target is not None else '*' * 15}] "
+                f"{spec.f_name}[.{attr}] = [{id(valu)}]"
+            )
+
+            target.__setattr__(attr, valu)  # Preload the variable? Yes: Fixes stdlib (asyncio.coroutines) errors in README.md.
             spec.loader.exec_module(self, spec, True)
+
+        spec.target.__setattr__(attr, valu)  # NB: Don't use `target` here, as it may have changed.
```

### Comparing `lazi-1.7.87/pyproject.toml` & `lazi-1.8.119/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.7.87"
+version = "1.8.119"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
@@ -50,14 +50,18 @@
 [tool.poetry.group.direct.dependencies]
 presto-requests = {git = "https://github.com/sitbon/presto"}
 
 
 [tool.pytest.ini_options]
 addopts = "-v --no-header -rA"
 cache_dir = ".cache/pytest"
+# log_cli = true
+log_cli_level = "DEBUG"
+log_cli_format = "%(message)s"
+log_format = "%(message)s"
 testpaths = [
     "tests",
 ]
 markers = [
     "test_test",
 ]
```

### Comparing `lazi-1.7.87/tests/test_django.py` & `lazi-1.8.119/tests/test_django.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
     from lazi.core.finder import Finder
 
     with Finder() as finder:
         debug.trace("test_django_version_lazy: finder.lazy ->")
         django = finder.lazy("django")
         debug.trace("test_django_version_lazy: ^- finder.lazy")
         version = django.VERSION
-        debug.trace("test_django_version_lazy: ^- VERSION: ", version)
+        debug.trace(f"test_django_version_lazy: ^- VERSION: {version}")
         assert isinstance(version, tuple), version
 
 
-# def test_django_version_import():
-#     from lazi.util import debug
-#     from lazi.core.finder import Finder
-#
-#     with Finder():
-#         debug.trace("test_django_version_import: import django ->")
-#         import django
-#         debug.trace("test_django_version_import: ^- import django")
-#         version = django.VERSION
-#         debug.trace("test_django_version_import: ^- VERSION: ", version)
-#         assert isinstance(version, tuple), version
+def test_django_version_import():
+    from lazi.util import debug
+    from lazi.core.finder import Finder
+
+    with Finder():
+        debug.trace("test_django_version_import: import django ->")
+        import django
+        debug.trace("test_django_version_import: ^- import django")
+        version = django.VERSION
+        debug.trace(f"test_django_version_import: ^- VERSION: {version}")
+        assert isinstance(version, tuple), version
 
 
 def test_asgiref():
     from lazi.util import debug
     from lazi.core import lazi
 
     with lazi:
```

### Comparing `lazi-1.7.87/tests/test_requests.py` & `lazi-1.8.119/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `lazi-1.7.87/tests/test_rich.py` & `lazi-1.8.119/tests/test_rich.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,27 +18,7 @@
             debug.trace("^- pretty.install(console=console) -^")
             debug.trace("-> traceback.install(console=console) ->")
             traceback.install(console=console)
             debug.trace("^- traceback.install(console=console) -^")
 
         setup()
         debug.trace("^- setup() -^")
-
-
-def test_rich_import_ctx():
-    from lazi.util import debug
-    # from lazi.core.finder import Finder
-    from lazi.core import lazi
-
-    with lazi:
-        debug.trace("-> from rich import console as rc, pretty, traceback ->")
-        from rich import console as rc, pretty, traceback
-        debug.trace("^- from rich import console as rc, pretty, traceback -^")
-        debug.trace("-> console = rc.Console(color_system='256', force_terminal=True) ->")
-        console = rc.Console(color_system="256", force_terminal=True)
-        debug.trace("^- console = rc.Console(color_system='256', force_terminal=True) -^")
-        debug.trace("-> pretty.install(console=console) ->")
-        pretty.install(console=console)
-        debug.trace("^- pretty.install(console=console) -^")
-        debug.trace("-> traceback.install(console=console) ->")
-        traceback.install(console=console)
-        debug.trace("^- traceback.install(console=console) -^")
```

### Comparing `lazi-1.7.87/PKG-INFO` & `lazi-1.8.119/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.7.87
+Version: 1.8.119
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Web Environment
@@ -34,28 +34,26 @@
 
 ## Usage:
 
 ```shell
 poetry add lazi
 ```
 ```shell
-DEBUG_TRACING=1 python3
+TRACE=1 python3
 ```
 ```pycon
 Python 3.11.2
 >>> import lazi.auto
-[140402520740240] +Finder refs:0 inst:0 sys:5
 >>> from django import test
-[140402520858096] <get> LAZY django[.test]
-[140402518572896] <set> LAZY django.utils[.version] [140402518571056]
-[140402518571056] <get> LAZY django.utils.version[.get_version]
-[140402518606128] <get> LAZY django.utils.regex_helper[._lazy_re_compile]
-[140402518607408] <get> LAZY django.utils.functional[.SimpleLazyObject]
+[139840712693360] LAZY >>>> [139840715383056] django[.test]
+[139840712694640] LAZY <<<< [139840712694240] django.utils[.version] = [139840712695040]
+[139840712695040] LAZY >>>> [139840712694880] [django.utils.]django.utils.version[.get_version]
+[139840712696720] LAZY >>>> [139840712696000] [django.utils.]django.utils.regex_helper[._lazy_re_compile]
+[139840712697680] LAZY >>>> [139840712697280] [django.utils.]django.utils.functional[.SimpleLazyObject]
 >>> test.TestCase
-[140402519121472] <get> LAZY django.test[.TestCase]
 # ... A lot of output ...
 <class 'django.test.testcases.TestCase'>
 >>> _
 ```
 
 ### Use for specific modules:
 
@@ -94,12 +92,13 @@
 
 It's also possible to manually change the configuration at runtime,
 with the caveat that some variables may have already been used by
 `lazi.core`. To avoid this, configure Lazi before importing it:
 
 ```python
 from lazi.conf import conf
-conf.DEBUG_TRACING = 1
+
+conf.TRACE = 1
 import lazi.auto
 # ...
 ```
```

