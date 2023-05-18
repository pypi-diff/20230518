# Comparing `tmp/lazi-1.8.128.tar.gz` & `tmp/lazi-1.9.137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.8.128.tar", max compression
+gzip compressed data, was "lazi-1.9.137.tar", max compression
```

## Comparing `lazi-1.8.128.tar` & `lazi-1.9.137.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.8.128/LICENSE
--rw-r--r--   0        0        0     9889 2023-05-18 03:31:46.016263 lazi-1.8.128/README.md
--rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.8.128/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.8.128/lazi/conf/auto.py
--rw-r--r--   0        0        0     1935 2023-05-18 02:19:06.579567 lazi-1.8.128/lazi/conf/base.py
--rw-r--r--   0        0        0     4708 2023-05-18 02:24:12.623535 lazi-1.8.128/lazi/conf/conf.py
--rw-r--r--   0        0        0     1330 2023-05-18 02:20:03.676308 lazi-1.8.128/lazi/conf/envs.py
--rw-r--r--   0        0        0      287 2023-05-17 23:57:14.444788 lazi-1.8.128/lazi/core/__init__.py
--rw-r--r--   0        0        0     5160 2023-05-18 02:53:08.158015 lazi-1.8.128/lazi/core/finder.py
--rw-r--r--   0        0        0     5087 2023-05-18 03:23:08.925510 lazi-1.8.128/lazi/core/loader.py
--rw-r--r--   0        0        0     3817 2023-05-18 03:03:19.185969 lazi-1.8.128/lazi/core/module.py
--rw-r--r--   0        0        0     1884 2023-05-18 03:03:19.185969 lazi-1.8.128/lazi/core/spec.py
--rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.8.128/lazi/core/stat.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.8.128/lazi/util/__init__.py
--rw-r--r--   0        0        0      822 2023-05-18 03:21:34.884282 lazi-1.8.128/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.8.128/lazi/util/functional.py
--rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.8.128/lazi/util/util.py
--rw-r--r--   0        0        0     1655 2023-05-18 03:38:10.145256 lazi-1.8.128/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.8.128/tests/__init__.py
--rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.8.128/tests/standalone/sa_array.py
--rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.8.128/tests/standalone/sa_nested.py
--rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.8.128/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.8.128/tests/test_array.py
--rw-r--r--   0        0        0      378 2023-05-17 06:09:23.165264 lazi-1.8.128/tests/test_asyncio.py
--rw-r--r--   0        0        0     1187 2023-05-18 00:16:22.071819 lazi-1.8.128/tests/test_django.py
--rw-r--r--   0        0        0     1251 2023-05-18 01:33:30.900017 lazi-1.8.128/tests/test_importlib.py
--rw-r--r--   0        0        0      230 2023-05-18 01:11:43.475022 lazi-1.8.128/tests/test_lazy.py
--rw-r--r--   0        0        0      307 2023-05-18 01:33:30.888016 lazi-1.8.128/tests/test_pygments.py
--rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.8.128/tests/test_requests.py
--rw-r--r--   0        0        0     1004 2023-05-17 07:14:47.163887 lazi-1.8.128/tests/test_rich.py
--rw-r--r--   0        0        0     1200 2023-05-18 01:33:30.900017 lazi-1.8.128/tests/test_stat.py
--rw-r--r--   0        0        0    10985 1970-01-01 00:00:00.000000 lazi-1.8.128/PKG-INFO
+-rw-r--r--   0        0        0      150 2023-05-17 23:57:14.424788 lazi-1.9.137/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.9.137/lazi/conf/auto.py
+-rw-r--r--   0        0        0     2037 2023-05-18 07:52:43.688996 lazi-1.9.137/lazi/conf/base.py
+-rw-r--r--   0        0        0     4708 2023-05-18 02:24:12.623535 lazi-1.9.137/lazi/conf/conf.py
+-rw-r--r--   0        0        0     1330 2023-05-18 02:20:03.676308 lazi-1.9.137/lazi/conf/envs.py
+-rw-r--r--   0        0        0      287 2023-05-18 04:13:09.132500 lazi-1.9.137/lazi/core/__init__.py
+-rw-r--r--   0        0        0     5195 2023-05-18 05:29:27.848235 lazi-1.9.137/lazi/core/finder.py
+-rw-r--r--   0        0        0     5620 2023-05-18 07:41:29.408157 lazi-1.9.137/lazi/core/loader.py
+-rw-r--r--   0        0        0     3817 2023-05-18 03:03:19.185969 lazi-1.9.137/lazi/core/module.py
+-rw-r--r--   0        0        0     1998 2023-05-18 07:52:43.688996 lazi-1.9.137/lazi/core/spec.py
+-rw-r--r--   0        0        0     3571 2023-05-17 06:13:14.860256 lazi-1.9.137/lazi/core/stat.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.9.137/lazi/util/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-18 05:48:25.043176 lazi-1.9.137/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.9.137/lazi/util/functional.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.9.137/lazi/util/util.py
+-rw-r--r--   0        0        0     1655 2023-05-18 07:53:34.741665 lazi-1.9.137/pyproject.toml
+-rw-r--r--   0        0        0     9607 2023-05-18 06:08:26.930976 lazi-1.9.137/readme.md
+-rw-r--r--   0        0        0        0 2023-05-17 06:10:55.650459 lazi-1.9.137/tests/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.9.137/tests/standalone/sa_array.py
+-rw-r--r--   0        0        0      922 2023-05-18 00:51:41.543400 lazi-1.9.137/tests/standalone/sa_nested.py
+-rw-r--r--   0        0        0       43 2023-05-18 04:25:44.850316 lazi-1.9.137/tests/standalone/sa_pandas.py
+-rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.9.137/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.9.137/tests/test_array.py
+-rw-r--r--   0        0        0      378 2023-05-17 06:09:23.165264 lazi-1.9.137/tests/test_asyncio.py
+-rw-r--r--   0        0        0     1187 2023-05-18 00:16:22.071819 lazi-1.9.137/tests/test_django.py
+-rw-r--r--   0        0        0     1251 2023-05-18 01:33:30.900017 lazi-1.9.137/tests/test_importlib.py
+-rw-r--r--   0        0        0      230 2023-05-18 01:11:43.475022 lazi-1.9.137/tests/test_lazy.py
+-rw-r--r--   0        0        0      307 2023-05-18 01:33:30.888016 lazi-1.9.137/tests/test_pygments.py
+-rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.9.137/tests/test_requests.py
+-rw-r--r--   0        0        0     1004 2023-05-17 07:14:47.163887 lazi-1.9.137/tests/test_rich.py
+-rw-r--r--   0        0        0     1200 2023-05-18 01:33:30.900017 lazi-1.9.137/tests/test_stat.py
+-rw-r--r--   0        0        0    10703 1970-01-01 00:00:00.000000 lazi-1.9.137/PKG-INFO
```

### Comparing `lazi-1.8.128/README.md` & `lazi-1.9.137/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: lazi
+Version: 1.9.137
+Summary: A lightweight and extensible way to implement lazy imports globally.
+Home-page: https://github.com/sitbon/lazi
+License: AGPLv3
+Author: Phillip Sitbon
+Author-email: phillip.sitbon@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Project-URL: Repository, https://github.com/sitbon/lazi
+Description-Content-Type: text/markdown
+
 # Lazi: Lazy Imports Everywhere
 
 An easy way to implement and track lazy imports globally.
 
 No external dependencies.
 
 **Requres Python 3.11.**
@@ -14,19 +40,19 @@
 ```shell
 TRACE=1 python3
 ```
 ```pycon
 >>> import lazi.auto
 >>> import django
 >>> django.VERSION
-[140071460506656] LAZY >>>> [140071460989312] django[.VERSION]  # Lazy loaded django due to VERSION attr access.
-[140071459492368] LAZY <<<< [140071459492448] django.utils[.version] = [140071459492928] # Ditto for django.utils setattr.
-[140071459492928] LAZY >>>> [140071459492848] [django.utils.]django.utils.version[.get_version]
-[140071459495168] LAZY >>>> [140071459495008] [django.utils.]django.utils.regex_helper[._lazy_re_compile]
-[140071459496048] LAZY >>>> [140071459495888] [django.utils.]django.utils.functional[.SimpleLazyObject]
+[140016542011360] LAZY >>>> [140016544686432] django VERSION  # Lazy loaded django due to VERSION attr access.
+[140016542012960] LAZY <<<< [140016542013120] django.utils version = [140016542013520]  # Ditto for django.utils setattr.
+[140016542013520] LAZY >>>> [140016542013920] django.utils|version get_version
+[140016542015600] LAZY >>>> [140016542015840] django.utils|regex_helper _lazy_re_compile
+[140016542016640] LAZY >>>> [140016542016880] django.utils|functional SimpleLazyObject
 (4, 2, 1, 'final', 0)
 >>> _
 ```
 
 And with `TRACE=2`:
 
 ```pycon
@@ -94,89 +120,93 @@
 >>> from lazi.core import lazy
 >>> django = lazy("django")
 >>> django.VERSION
 (4, 2, 1, 'final', 0)
 >>> _
 ```
 
-### Tricky Situations.
-
-#### 1. Circular imports.
-
-Usually shows up as `AttributeError: 'module' object has no attribute 'attr'`.
+## Tricky Situations
 
-#### 2. Expected global state is not there.
+### Expected global state is not there.
 
 This is the most common issue when using `lazi.auto`, and can be difficult to debug.
 
 Fortunately, Lazi will show some useful tracebacks including the original exception before
-it was transformed into an `ImportError` or `AttributeError` (by CPython, thowing away the original traceback).
+it was transformed into an `ImportError` (by CPython, thowing away the original traceback).
 
 Example:
 ```pycon
 >>> import lazi.auto
 >>> import pandas.core.nanops
-ERROR:root:[140549280569824] EXEC DEAD [140549280573824] pandas.core|nanops
+[140343991111888] EXEC DEAD [140343991111968] dateutil.tz|win !!!! six.moves  # This is unrelated.
+[140343977781872] EXEC DEAD [140343977777872] pandas.core|nanops !!!! 
                   !!!! OptionError: No such keys(s): 'compute.use_bottleneck'
 Traceback (most recent call last):
   File "/home/jq/pr/lazi/lazi/core/loader.py", line 107, in exec_module
     self.loader.exec_module(target if target is not None else module)
   File "<frozen importlib._bootstrap_external>", line 940, in exec_module
   File "<frozen importlib._bootstrap>", line 241, in _call_with_frames_removed
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/core/nanops.py", line 74, in <module>
+  File "/.../pandas/core/nanops.py", line 74, in <module>
     set_use_bottleneck(get_option("compute.use_bottleneck"))
                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/_config/config.py", line 261, in __call__
+  File "/.../pandas/_config/config.py", line 261, in __call__
     return self.__func__(*args, **kwds)
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/_config/config.py", line 135, in _get_option
+  File "/.../pandas/_config/config.py", line 135, in _get_option
     key = _get_single_key(pat, silent)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/_config/config.py", line 121, in _get_single_key
+  File "/.../pandas/_config/config.py", line 121, in _get_single_key
     raise OptionError(f"No such keys(s): {repr(pat)}")
 pandas._config.config.OptionError: No such keys(s): 'compute.use_bottleneck'
+[140343976684704] EXEC DEAD [140343976684864] pandas.core.arrays.sparse|array !!!! pandas.core.nanops
+[140343976682224] EXEC DEAD [140343976682464] pandas.core.arrays.sparse|accessor !!!! pandas.core.nanops
+[140343976681984] EXEC DEAD [140343976681744] pandas.core.arrays.sparse !!!! pandas.core.nanops
+[140343980659536] EXEC DEAD [140343980659456] pandas.core.arrays !!!! pandas.core.nanops # No traceback means
+[140343980335376] EXEC DEAD [140343980335456] pandas.core|api !!!! pandas.core.nanops    # that this is a chain
+[140345351918096] EXEC DEAD [140345351918496] pandas !!!! pandas.core.nanops             # of ImportError's.
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   File "/home/jq/pr/lazi/lazi/core/module.py", line 102, in __setattr__
     spec.loader.exec_module(self, True)
   File "/home/jq/pr/lazi/lazi/core/loader.py", line 107, in exec_module
     self.loader.exec_module(target if target is not None else module)
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/__init__.py", line 48, in <module>
+  File "/<site-packages>/pandas/__init__.py", line 48, in <module>
     from pandas.core.api import (
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
   File "/home/jq/pr/lazi/lazi/core/loader.py", line 107, in exec_module
     self.loader.exec_module(target if target is not None else module)
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/core/api.py", line 27, in <module>
+  File "/<site-packages>/pandas/core/api.py", line 27, in <module>
     from pandas.core.arrays import Categorical
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
   File "/home/jq/pr/lazi/lazi/core/loader.py", line 107, in exec_module
     self.loader.exec_module(target if target is not None else module)
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/core/arrays/__init__.py", line 19, in <module>
+  File "/<site-packages>/pandas/core/arrays/__init__.py", line 19, in <module>
     from pandas.core.arrays.sparse import SparseArray
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
   File "/home/jq/pr/lazi/lazi/core/loader.py", line 107, in exec_module
     self.loader.exec_module(target if target is not None else module)
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/core/arrays/sparse/__init__.py", line 1, in <module>
+  File "/<site-packages>/pandas/core/arrays/sparse/__init__.py", line 1, in <module>
     from pandas.core.arrays.sparse.accessor import (
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
   File "/home/jq/pr/lazi/lazi/core/loader.py", line 107, in exec_module
     self.loader.exec_module(target if target is not None else module)
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/core/arrays/sparse/accessor.py", line 16, in <module>
+  File "/<site-packages>/pandas/core/arrays/sparse/accessor.py", line 16, in <module>
     from pandas.core.arrays.sparse.array import SparseArray
   File "/home/jq/pr/lazi/lazi/core/module.py", line 75, in __getattribute__
     spec.loader.exec_module(self, True)
   File "/home/jq/pr/lazi/lazi/core/loader.py", line 107, in exec_module
     self.loader.exec_module(target if target is not None else module)
-  File "/home/jq/.cache/pypoetry/virtualenvs/lazi-5AqQzycq-py3.11/lib/python3.11/site-packages/pandas/core/arrays/sparse/array.py", line 101, in <module>
+  File "/<site-packages>/pandas/core/arrays/sparse/array.py", line 101, in <module>
     from pandas.core.nanops import check_below_min_count
 ImportError: cannot import name 'check_below_min_count' from 'pandas.core.nanops' (unknown location)
+
 >>> _
 ```
 
 _Unforunately_... This isn't something that can be worked around without outer dependency tracking, which
 generally results in entire packages getting loaded anyway.
 
 If you're more interested in just tracking imports with Lazi, use the `NO_HOOK` config variable (see below).
@@ -187,21 +217,21 @@
 that get autoloaded (in import order) by `lazi.conf.conf`.
 It is fully decoupled from the rest of the codebase.
 
 As a result, it's possible configure Lazi by creating `lazi.conf`
 modules in your project (within the `lazi.conf` namespace package),
 and use conf modules provided by other packages.
 
-Configuration is not yet controllable via environment variables,
-but this is planned for the future. Update: Supported for DEBUG_TRACING.
+Configuration variables can also be set from the environment.
 
 It's also possible to manually change the configuration at runtime,
 with the caveat that some variables may have already been used by
 `lazi.core`. To avoid this, configure Lazi before importing it:
 
 ```python
 from lazi.conf import conf
 
 conf.TRACE = 1
 import lazi.auto
 # ...
 ```
+
```

### Comparing `lazi-1.8.128/lazi/conf/base.py` & `lazi-1.9.137/lazi/conf/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Base project configuration.
 """
 __meta__ = dict(                        # Internal configuration for <root>.conf.conf (cannot override elsewhere).
     root="lazi",                        # - Root namespace package name.
 )                                       # See conf.py for more options.
 #
 TRACE: int = 0                          # Enable debug traces. Currently using levels 0-4.
+TRACEE: bool = False                     # Enable debug traces for loader exceptions when TRACE is 0.
 #                                       # - Tracing relies on __debug__ and asserts, so -O will disable completely.
 AUTO_AUTO: bool = True                  # Automatically install when importing lazi.auto.
 CORE_AUTO: bool = False                 # Automatically install when importing lazi.core.
 #
 NO_HOOK: bool = False                   # Disable all spec loader hooks.
 NO_LAZY: bool = False                   # Hook loaders, but skip lazy loading.
 NO_HOOK_STD: bool = False               # Disable spec loader hooking for stdlib modules.
```

### Comparing `lazi-1.8.128/lazi/conf/conf.py` & `lazi-1.9.137/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/lazi/conf/envs.py` & `lazi-1.9.137/lazi/conf/envs.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/lazi/core/finder.py` & `lazi-1.9.137/lazi/core/finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                     spec.target = target
 
             assert None is debug.traced(
                 1,
                 f"[{id(self)}] FIND " +
                 ((Path(c).suffix[1:] if (c := spec.cached) else Path(o).suffix[1:] if (o := spec.origin) else '?') +
                     f"{'S' if spec.stdlib else ''}{'B' if spec.builtin else ''}").ljust(5) +
-                spec.f_name
+                f"{spec.f_name} {'*' if path is None else ''}"
             )
 
             return spec
 
     def _find_spec(self, name: str, path: list[str] | None, target: ModuleType | None) -> ModuleSpec | None:
         for finder in (_ for _ in sys.meta_path if _ is not self):
             if (spec := finder.find_spec(name, path, target)) is not None:
```

### Comparing `lazi-1.8.128/lazi/core/loader.py` & `lazi-1.9.137/lazi/core/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 __all__ = "Loader",
 
 Spec = ForwardRef("Spec")
 Module = ForwardRef("Module")
 
 NO_LAZY = conf.NO_LAZY
-
+TRACE = conf.TRACE
+TRACEE = conf.TRACEE
 
 class Loader(_Loader):
     spec: Spec
     loader: _Loader
     __busy: bool = False
     __forc: bool = False
 
@@ -74,26 +75,30 @@
         lazy = not ((force or self.__forc) if force is not None else self.__forc)
 
         name = spec.name
         name_ = spec.f_name
         state = spec.loader_state
         nexts = Loader.State.LAZY if lazy else Loader.State.EXEC
         target = spec.target
+        in_sys = name in modules
 
         assert state in (Loader.State.CREA, Loader.State.LAZY), state
 
-        if (mod := modules.get(name)) is not module and mod is not None:
-            assert None is debug.trace(
-                f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_} "
-                f"::[{id(mod) if mod is not target else 'same' if mod is not None else '-'}] "
-                "(before)"
-            )
+        if (mod := modules.get(name)) is not module:
+            if in_sys:
+                assert None is debug.trace(
+                    f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_} "
+                    f"::[{id(mod) if mod is not target else 'same' if mod is not None else '-'}] "
+                    "(before)"
+                ), "module was replaced in sys.modules before exec_module"
+
+                modules[name] = module
 
-            spec.target = target = mod
-            modules[name] = module
+            if mod is not None and mod is not target:
+                spec.target = target = mod
 
         assert None is debug.traced(
             1,  # if nexts is Loader.State.EXEC else 2,
             f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_} "
             f"{'>>>> ' if nexts is Loader.State.EXEC else '.... '}"
         )
 
@@ -114,38 +119,45 @@
                 1,  # if nexts is Loader.State.LOAD else 2,
                 f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_} "
                 f"++++ "
             )
 
         except Exception as e:
             spec.loader_state = nexts = Loader.State.DEAD
-            assert None is getattr(debug, "info" if isinstance(e, ImportError) else "exception")(
-                f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_}\n" +
-                " " * 18 + f"!!!! {type(e).__name__}: {e}"
+            assert None is getattr(
+                debug,
+                "exception" if not isinstance(e, ImportError) and (TRACEE or TRACE > 0) else
+                "trace" if not TRACEE else "info"
+            )(
+                f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_} !!!! " +
+                (('\n' + " " * 18 + f"!!!! {type(e).__name__}: {e}") if not isinstance(e, ImportError) else e.name)
             )
             raise
 
-        if (mod := modules.get(name)) is not module and mod is not None:
-            assert None is debug.trace(
-                f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_} "
-                f"::[{id(mod) if mod is not target else 'same' if mod is not None else '-'}] "
-                "(after)"
-            )
+        if (mod := modules.get(name)) is not module:
+            if in_sys:
+                assert None is debug.trace(
+                    f"[{id(module)}] {state} {nexts} [{id(target) if target is not None else '*'*15}] {name_} "
+                    f"::[{id(mod) if mod is not target else 'same' if mod is not None else '-'}] "
+                    "(after)"
+                ), "module was replaced in sys.modules after exec_module"
+
+                modules[name] = module
 
-            spec.target = target = mod
-            modules[name] = module
+            if mod is not None and mod is not spec.target:
+                spec.target = mod
 
     def invalidate_caches(self) -> None:
         spec = self.spec
 
         if (mod := modules.get(spec.name)) is spec.target and mod is not None:
             del modules[spec.name]
 
         assert None is debug.traced(
-            1,
+            2,
             f"[{id(mod) if mod is not None else '*'*15}] "
             f"{spec.loader_state} DEAD [{id(spec.target) if spec.target else '*'*15}] {spec.f_name}"
         )
 
         spec.loader = self.loader
         spec.loader_state = None  # type: ignore
         spec.target = None
```

### Comparing `lazi-1.8.128/lazi/core/module.py` & `lazi-1.9.137/lazi/core/module.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/lazi/core/spec.py` & `lazi-1.9.137/lazi/core/spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,25 +36,27 @@
 
     _f_name = lambda self, wrap=lambda _, __: f"{_}|{__.replace(f'{_}.', '', 1)}": (
         wrap(parent, name) if (name := self.name) != (parent := self.parent) and parent else name
     )
 
     f_name: str | None = cached_property(lambda self: self._f_name())
 
+    is_package: bool = cached_property(lambda self: self.submodule_search_locations is not None)
+
     def __init__(self, finder: Finder, spec: ModuleSpec, path: list[str] | None = None, target: ModuleType | None = None):
         self.finder = finder
         self.s_path = path
         self.target = target
 
         super().__init__(
             name=spec.name,
             loader=spec.loader,
             origin=spec.origin,
             loader_state=spec.loader_state,
-            is_package=spec.submodule_search_locations is not None,
+            is_package=spec.submodule_search_locations is not None or path is None,
         )
 
         self.__dict__.update(spec.__dict__)
         self.loader = finder.Loader(self) if self.hook else self.loader
 
     @cached_property
     def hook(self) -> bool:
```

### Comparing `lazi-1.8.128/lazi/core/stat.py` & `lazi-1.9.137/lazi/core/stat.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/lazi/util/debug.py` & `lazi-1.9.137/lazi/util/debug.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from contextlib import contextmanager
 import logging
 
 from lazi.conf import conf
 
 __all__ = "trace", "traced", "info", "track"
 
-
-info = logging.info
 exception = logging.exception
 
 TRACE = conf.TRACE
 
-if __debug__ and TRACE:
+if __debug__:
 
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(message)s",
     )
 
     traced = lambda at, /, *args, **kwds: logging.debug(*args, **kwds) if TRACE > at else None  # noqa
     trace = lambda *args, **kwds: traced(0, *args, **kwds)
+    info = lambda *_, **__: traced(-1, *_, **__)
 
 else:
     traced = lambda at, /, *args, **kwds: None
     trace = lambda *args, **kwds: None
+    info = lambda *_, **__: None
 
 
 @contextmanager
 def track(msg: str, log=info, exc=info):
     log(f"... {msg} ...")
     try:
         yield
```

### Comparing `lazi-1.8.128/pyproject.toml` & `lazi-1.9.137/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "lazi"
-version = "1.8.128"
+version = "1.9.137"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
-readme = "README.md"
+readme = "readme.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Natural Language :: English",
```

### Comparing `lazi-1.8.128/tests/standalone/sa_nested.py` & `lazi-1.9.137/tests/standalone/sa_nested.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/tests/test_django.py` & `lazi-1.9.137/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/tests/test_importlib.py` & `lazi-1.9.137/tests/test_importlib.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/tests/test_requests.py` & `lazi-1.9.137/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/tests/test_rich.py` & `lazi-1.9.137/tests/test_rich.py`

 * *Files identical despite different names*

### Comparing `lazi-1.8.128/tests/test_stat.py` & `lazi-1.9.137/tests/test_stat.py`

 * *Files identical despite different names*

