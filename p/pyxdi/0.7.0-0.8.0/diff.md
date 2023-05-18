# Comparing `tmp/pyxdi-0.7.0.tar.gz` & `tmp/pyxdi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxdi-0.7.0.tar", max compression
+gzip compressed data, was "pyxdi-0.8.0.tar", max compression
```

## Comparing `pyxdi-0.7.0.tar` & `pyxdi-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 pyxdi-0.7.0/LICENSE
--rw-r--r--   0        0        0     1635 2023-05-16 11:55:56.046789 pyxdi-0.7.0/README.md
--rw-r--r--   0        0        0     1667 2023-05-16 12:55:03.253417 pyxdi-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      239 2023-05-16 11:55:56.049371 pyxdi-0.7.0/pyxdi/__init__.py
--rw-r--r--   0        0        0    30760 2023-05-16 11:55:56.049921 pyxdi-0.7.0/pyxdi/core.py
--rw-r--r--   0        0        0     2464 2023-05-16 11:55:56.050184 pyxdi-0.7.0/pyxdi/decorators.py
--rw-r--r--   0        0        0      263 2023-05-16 11:55:56.050387 pyxdi-0.7.0/pyxdi/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633484 pyxdi-0.7.0/pyxdi/ext/__init__.py
--rw-r--r--   0        0        0     2768 2023-05-16 11:55:56.050777 pyxdi-0.7.0/pyxdi/ext/fastapi.py
--rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633846 pyxdi-0.7.0/pyxdi/ext/starlette/__init__.py
--rw-r--r--   0        0        0      635 2023-03-24 15:06:03.633960 pyxdi-0.7.0/pyxdi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2023-02-14 18:16:50.285713 pyxdi-0.7.0/pyxdi/py.typed
--rw-r--r--   0        0        0     1846 2023-05-16 12:54:50.100696 pyxdi-0.7.0/pyxdi/utils.py
--rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 pyxdi-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 pyxdi-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1547 2023-05-18 06:53:42.467888 pyxdi-0.8.0/README.md
+-rw-r--r--   0        0        0     1593 2023-05-18 06:54:49.408916 pyxdi-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      261 2023-05-18 06:53:42.470025 pyxdi-0.8.0/pyxdi/__init__.py
+-rw-r--r--   0        0        0    30693 2023-05-18 06:53:42.470484 pyxdi-0.8.0/pyxdi/core.py
+-rw-r--r--   0        0        0     2324 2023-05-18 06:53:42.470811 pyxdi-0.8.0/pyxdi/decorators.py
+-rw-r--r--   0        0        0      263 2023-05-16 11:55:56.050387 pyxdi-0.8.0/pyxdi/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633484 pyxdi-0.8.0/pyxdi/ext/__init__.py
+-rw-r--r--   0        0        0     2768 2023-05-16 11:55:56.050777 pyxdi-0.8.0/pyxdi/ext/fastapi.py
+-rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633846 pyxdi-0.8.0/pyxdi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0      629 2023-05-18 06:53:42.471309 pyxdi-0.8.0/pyxdi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2023-02-14 18:16:50.285713 pyxdi-0.8.0/pyxdi/py.typed
+-rw-r--r--   0        0        0     1487 2023-05-18 06:53:42.471733 pyxdi-0.8.0/pyxdi/utils.py
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 pyxdi-0.8.0/PKG-INFO
```

### Comparing `pyxdi-0.7.0/LICENSE` & `pyxdi-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxdi-0.7.0/README.md` & `pyxdi-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,35 +13,31 @@
 
 http://pyxdi.readthedocs.io/
 
 ---
 
 ## Requirements
 
-Python 3.7+
+Python 3.8+
+
+* [lazy-object-proxy](https://github.com/ionelmc/python-lazy-object-proxy) (for supporting lazy injections)
 
 and optional dependencies:
 
 * [anyio](https://github.com/agronholm/anyio) (for supporting synchronous resources with an asynchronous runtime)
-* [lazy-object-proxy](https://github.com/ionelmc/python-lazy-object-proxy) (for supporting lazy injections)
+
 
 ## Installation
 
 Install using `pip`:
 
 ```shell
 pip install pyxdi
 ```
 
-or with all dependencies (anyio, lazy-object-proxy)
-
-```shell
-pip install pyxdi[all]
-```
-
 or using `poetry`:
 
 ```shell
 poetry add pyxdi
 ```
 
 ## Quick Example
```

### Comparing `pyxdi-0.7.0/pyproject.toml` & `pyxdi-0.8.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 [tool.poetry]
 name = "pyxdi"
-version = "0.7.0"
+version = "0.8.0"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/pyxdi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 packages = [
     { include = "pyxdi", from = "." },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
+lazy-object-proxy = "^1.9.0"
 anyio = { version = "^3.6.2", optional = true }
-lazy-object-proxy = { version = "^1.9.0", optional = true }
 mkdocs = { version = "^1.4.2", optional = true }
-mkdocs-material = { version = "^9.0.12", optional = true }
+mkdocs-material = { version = "^9.1.13", optional = true }
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-material"]
-all = ["anyio", "lazy-object-proxy"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.3.0"
 ruff = "^0.0.267"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 anyio = "^3.6.2"
-lazy-object-proxy = "^1.9.0"
 fastapi = "^0.95.1"
 httpx = "^0.24.0"
+sqlalchemy = "^2.0.13"
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
 include = '\.pyi?$'
 
 [tool.ruff]
```

### Comparing `pyxdi-0.7.0/pyxdi/core.py` & `pyxdi-0.8.0/pyxdi/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import contextlib
 import importlib
 import inspect
 import logging
 import pkgutil
+import types
 import typing as t
 import uuid
 from collections import defaultdict
 from contextvars import ContextVar
 from dataclasses import dataclass
 from functools import cached_property, wraps
-from types import ModuleType, TracebackType
 
 from typing_extensions import Annotated, ParamSpec
 
 try:
     from types import NoneType
 except ImportError:
     NoneType = type(None)  # type: ignore[assignment,misc]
@@ -63,15 +63,15 @@
 
     @cached_property
     def is_class(self) -> bool:
         return inspect.isclass(self.obj)
 
     @cached_property
     def is_function(self) -> bool:
-        return inspect.isfunction(self.obj) and not (
+        return (inspect.isfunction(self.obj) or inspect.ismethod(self.obj)) and not (
             self.is_resource or self.is_async_resource
         )
 
     @cached_property
     def is_resource(self) -> bool:
         return inspect.isgeneratorfunction(self.obj)
 
@@ -84,31 +84,26 @@
 class UnresolvedProvider:
     interface: t.Type[t.Any]
     parameter_name: str
     provider: Provider
 
 
 @dataclass(frozen=True)
-class ScannedProvider:
-    member: t.Any
-    scope: Scope
-
-
-@dataclass(frozen=True)
 class ScannedDependency:
     member: t.Any
-    module: ModuleType
+    module: types.ModuleType
     lazy: t.Optional[bool] = None
 
 
-class _DependencyMark:
+class DependencyMark:
     __slots__ = ()
 
 
-dep = t.cast(t.Any, _DependencyMark())
+# Dependency mark with Any type
+dep = t.cast(t.Any, DependencyMark())
 
 
 def named(tp: t.Type[T], name: str) -> Annotated[t.Type[T], str]:
     """
     Cast annotated type helper.
     """
     return t.cast(Annotated[t.Type[T], str], Annotated[tp, name])
@@ -123,28 +118,36 @@
 class PyxDI:
     def __init__(
         self,
         *,
         default_scope: Scope = "singleton",
         auto_register: bool = False,
         lazy_inject: bool = False,
+        modules: t.Optional[
+            t.Sequence[t.Union[Module, t.Type[Module], t.Callable[["PyxDI"], None]]],
+        ] = None,
     ) -> None:
         self._default_scope = default_scope
         self._auto_register = auto_register
         self._lazy_inject = lazy_inject
         self._providers: t.Dict[t.Type[t.Any], Provider] = {}
         self._singleton_context = ScopedContext("singleton", self)
         self._request_context_var: ContextVar[t.Optional[ScopedContext]] = ContextVar(
             "request_context", default=None
         )
         self._unresolved_providers: t.Dict[
             t.Type[t.Any], t.List[UnresolvedProvider]
         ] = defaultdict(list)
         self._unresolved_dependencies: t.Dict[t.Type[t.Any], UnresolvedDependency] = {}
 
+        # Register modules
+        modules = modules or []
+        for module in modules:
+            self.register_module(module)
+
     @property
     def default_scope(self) -> Scope:
         return self._default_scope
 
     @property
     def auto_register(self) -> bool:
         return self._auto_register
@@ -165,52 +168,47 @@
     def register_provider(
         self,
         interface: t.Type[t.Any],
         obj: t.Callable[..., t.Any],
         *,
         scope: t.Optional[Scope] = None,
         override: bool = False,
-        ignore: bool = False,
     ) -> Provider:
         provider = Provider(obj=obj, scope=scope or self.default_scope)
 
         if (provider.is_resource or provider.is_async_resource) and (
             interface is NoneType or interface is None
         ):
             interface = type(f"EventResource_{uuid.uuid4()}", (), {})
 
         try:
-            registered_provider = self.get_provider(interface)
+            self.get_provider(interface)
         except ProviderError:
             pass
         else:
             if override:
                 self._providers[interface] = provider
                 return provider
 
-            if ignore:
-                logger.info(
-                    f"Ignoring the `{provider}` provider as it "
-                    "has already been registered."
-                )
-                return registered_provider
-
             raise ProviderError(
                 f"The provider interface `{get_full_qualname(interface)}` "
                 "already registered."
             )
 
         self._validate_provider_scope(provider)
         self._validate_provider_type(provider)
         self._validate_provider_match_scopes(interface, provider)
 
         self._providers[interface] = provider
         return provider
 
     def unregister_provider(self, interface: t.Type[t.Any]) -> None:
+        """
+        Unregister provider by interface.
+        """
         if not self.has_provider(interface):
             raise ProviderError(
                 "The provider interface "
                 f"`{get_full_qualname(interface)}` not registered."
             )
 
         provider = self.get_provider(interface)
@@ -226,26 +224,32 @@
 
         # Cleanup provider references
         self._providers.pop(interface, None)
         self._unresolved_providers.pop(interface, None)
         self._unresolved_dependencies.pop(interface, None)
 
     def get_provider(self, interface: t.Type[t.Any]) -> Provider:
+        """
+        Get provider by interface.
+        """
         try:
             return self._providers[interface]
         except KeyError as exc:
             raise ProviderError(
                 f"The provider interface for `{get_full_qualname(interface)}` has "
                 "not been registered. Please ensure that the provider interface is "
                 "properly registered before attempting to use it."
             ) from exc
 
     def singleton(
         self, interface: t.Type[T], instance: t.Any, *, override: bool = False
     ) -> Provider:
+        """
+        Register singleton instance provider.
+        """
         return self.register_provider(
             interface, lambda: instance, scope="singleton", override=override
         )
 
     # Validators
     def _validate_provider_scope(self, provider: Provider) -> None:
         if provider.scope not in t.get_args(Scope):
@@ -355,14 +359,38 @@
                 return
             message = "\n".join(errors)
             raise UnknownDependency(
                 "The following unknown injected dependencies were detected:"
                 f"\n{message}."
             )
 
+    # Modules
+    def register_module(
+        self, module: t.Union[Module, t.Type[Module], t.Callable[["PyxDI"], None]]
+    ) -> None:
+        """
+        Register module as callable, Module type or Module instance.
+        """
+        # Callable Module
+        if inspect.isfunction(module):
+            module(self)
+            return
+
+        # Class based Module or Module type
+        if inspect.isclass(module) and issubclass(module, Module):
+            module = module()
+        if isinstance(module, Module):
+            module.configure(self)
+            for _, method in inspect.getmembers(module):
+                provided = getattr(method, "__pyxdi_provider__", None)
+                if not provided:
+                    continue
+                scope = provided.get("scope")
+                self.provider(scope=scope, override=True)(method)
+
     # Lifespan
 
     def start(self) -> None:
         self.validate()
         self._singleton_context.start()
 
     def close(self) -> None:
@@ -370,40 +398,40 @@
 
     def request_context(
         self,
     ) -> t.ContextManager["ScopedContext"]:
         return contextlib.contextmanager(self._request_context)()
 
     def _request_context(self) -> t.Iterator["ScopedContext"]:
-        with self.create_request_context() as context:
+        with self._create_request_context() as context:
             token = self._request_context_var.set(context)
             yield context
             self._request_context_var.reset(token)
 
     # Asynchronous lifespan
 
     async def astart(self) -> None:
         self.validate()
         await self._singleton_context.astart()
 
     async def aclose(self) -> None:
         await self._singleton_context.aclose()
 
-    async def arequest_context(
+    def arequest_context(
         self,
     ) -> t.AsyncContextManager["ScopedContext"]:
         return contextlib.asynccontextmanager(self._arequest_context)()
 
     async def _arequest_context(self) -> t.AsyncIterator["ScopedContext"]:
-        async with self.create_request_context() as context:
+        async with self._create_request_context() as context:
             token = self._request_context_var.set(context)
             yield context
             self._request_context_var.reset(token)
 
-    def create_request_context(self) -> "ScopedContext":
+    def _create_request_context(self) -> "ScopedContext":
         return ScopedContext("request", self)
 
     def _get_request_context(self) -> "ScopedContext":
         request_context = self._request_context_var.get()
         if request_context is None:
             raise LookupError(
                 "The request context has not been started. Please ensure that "
@@ -411,14 +439,17 @@
                 "to use it."
             )
         return request_context
 
     # Instance
 
     def get(self, interface: t.Type[T]) -> T:
+        """
+        Get instance by interface.
+        """
         try:
             provider = self.get_provider(interface)
         except ProviderError:
             if (
                 self.auto_register
                 and inspect.isclass(interface)
                 and not is_builtin_type(interface)
@@ -431,14 +462,17 @@
         scoped_context = self._get_scoped_context(provider.scope)
         if scoped_context:
             return scoped_context.get(interface)
 
         return t.cast(T, self.create_instance(provider))
 
     def has(self, interface: t.Type[T]) -> bool:
+        """
+        Check that container contains instance by interface.
+        """
         try:
             provider = self.get_provider(interface)
         except ProviderError:
             return False
         scoped_context = self._get_scoped_context(provider.scope)
         if scoped_context:
             return scoped_context.has(interface)
@@ -523,35 +557,27 @@
 
     @t.overload
     def provider(
         self,
         *,
         scope: t.Optional[Scope] = None,
         override: bool = False,
-        ignore: bool = False,
     ) -> t.Callable[[t.Callable[P, T]], t.Callable[P, T]]:
         ...
 
     def provider(
         self,
         func: t.Optional[t.Callable[P, T]] = None,
         *,
         scope: t.Optional[Scope] = None,
         override: bool = False,
-        ignore: bool = False,
     ) -> t.Union[t.Callable[P, T], t.Callable[[t.Callable[P, T]], t.Callable[P, T]]]:
         def decorator(func: t.Callable[P, T]) -> t.Callable[P, T]:
             interface = self._get_provider_annotation(func)
-            self.register_provider(
-                interface,
-                func,
-                scope=scope,
-                override=override,
-                ignore=ignore,
-            )
+            self.register_provider(interface, func, scope=scope, override=override)
             return func
 
         if func is None:
             return decorator
         return decorator(func)
 
     @t.overload
@@ -619,90 +645,68 @@
 
     # Scanner
 
     def scan(
         self,
         /,
         packages: t.Union[
-            t.Union[ModuleType, str],
-            t.Iterable[t.Union[ModuleType, str]],
+            t.Union[types.ModuleType, str],
+            t.Iterable[t.Union[types.ModuleType, str]],
         ],
         *,
         tags: t.Optional[t.Iterable[str]] = None,
     ) -> None:
-        scanned_providers: t.List[ScannedProvider] = []
-        scanned_dependencies: t.List[ScannedDependency] = []
+        dependencies: t.List[ScannedDependency] = []
 
         if isinstance(packages, t.Iterable) and not isinstance(packages, str):
-            scan_packages: t.Iterable[t.Union[ModuleType, str]] = packages
+            scan_packages: t.Iterable[t.Union[types.ModuleType, str]] = packages
         else:
-            scan_packages = t.cast(t.Iterable[t.Union[ModuleType, str]], [packages])
+            scan_packages = t.cast(
+                t.Iterable[t.Union[types.ModuleType, str]], [packages]
+            )
 
         for package in scan_packages:
-            _scanned_providers, _scanned_dependencies = self._scan_package(
-                package, tags=tags
-            )
-            scanned_providers.extend(_scanned_providers)
-            scanned_dependencies.extend(_scanned_dependencies)
+            dependencies.extend(self._scan_package(package, tags=tags))
 
-        for scanned_provider in scanned_providers:
-            self.provider(
-                scope=scanned_provider.scope,
-                override=False,
-                ignore=True,
-            )(scanned_provider.member)
-
-        for scanned_dependency in scanned_dependencies:
-            decorator = self.inject(lazy=scanned_dependency.lazy)(
-                scanned_dependency.member
-            )
-            setattr(
-                scanned_dependency.module,
-                scanned_dependency.member.__name__,
-                decorator,
-            )
+        for dependency in dependencies:
+            decorator = self.inject(lazy=dependency.lazy)(dependency.member)
+            setattr(dependency.module, dependency.member.__name__, decorator)
 
     def _scan_package(
         self,
-        package: t.Union[ModuleType, str],
+        package: t.Union[types.ModuleType, str],
         *,
         tags: t.Optional[t.Iterable[str]] = None,
-    ) -> t.Tuple[t.List[ScannedProvider], t.List[ScannedDependency]]:
+    ) -> t.List[ScannedDependency]:
         tags = tags or []
         if isinstance(package, str):
             package = importlib.import_module(package)
 
         package_path = getattr(package, "__path__", None)
 
         if not package_path:
             return self._scan_module(package, tags=tags)
 
-        scanned_providers: t.List[ScannedProvider] = []
-        scanned_dependencies: t.List[ScannedDependency] = []
+        dependencies: t.List[ScannedDependency] = []
 
         for module_info in pkgutil.walk_packages(
             path=package_path, prefix=package.__name__ + "."
         ):
             module = importlib.import_module(module_info.name)
-            _scanned_providers, _scanned_dependencies = self._scan_module(
-                module, tags=tags
-            )
-            scanned_providers.extend(_scanned_providers)
-            scanned_dependencies.extend(_scanned_dependencies)
+            dependencies.extend(self._scan_module(module, tags=tags))
 
-        return scanned_providers, scanned_dependencies
+        return dependencies
 
     def _scan_module(
         self,
-        module: ModuleType,
+        module: types.ModuleType,
         *,
         tags: t.Iterable[str],
-    ) -> t.Tuple[t.List[ScannedProvider], t.List[ScannedDependency]]:
-        scanned_providers: t.List[ScannedProvider] = []
-        scanned_dependencies: t.List[ScannedDependency] = []
+    ) -> t.List[ScannedDependency]:
+        dependencies: t.List[ScannedDependency] = []
 
         for _, member in inspect.getmembers(module):
             if getattr(member, "__module__", None) != module.__name__ or not callable(
                 member
             ):
                 continue
 
@@ -710,44 +714,40 @@
             if tags and (
                 member_tags
                 and not set(member_tags).intersection(tags)
                 or not member_tags
             ):
                 continue
 
-            provided = getattr(member, "__pyxdi_provider__", None)
-            if provided:
-                scope = provided["scope"]
-                scanned_providers.append(ScannedProvider(member=member, scope=scope))
-                continue
-
             injected = getattr(member, "__pyxdi_inject__", None)
             if injected:
                 lazy = injected["lazy"]
-                scanned_dependencies.append(
-                    self._scanned_dependency(member=member, module=module, lazy=lazy)
+                dependencies.append(
+                    self._create_scanned_dependency(
+                        member=member, module=module, lazy=lazy
+                    )
                 )
                 continue
 
             # Get by pyxdi.dep mark
             if inspect.isclass(member):
                 signature = get_signature(member.__init__)
             else:
                 signature = get_signature(member)
             for parameter in signature.parameters.values():
-                if isinstance(parameter.default, _DependencyMark):
-                    scanned_dependencies.append(
-                        self._scanned_dependency(member=member, module=module)
+                if isinstance(parameter.default, DependencyMark):
+                    dependencies.append(
+                        self._create_scanned_dependency(member=member, module=module)
                     )
                     continue
 
-        return scanned_providers, scanned_dependencies
+        return dependencies
 
-    def _scanned_dependency(
-        self, member: t.Any, module: ModuleType, lazy: t.Optional[bool] = None
+    def _create_scanned_dependency(
+        self, member: t.Any, module: types.ModuleType, lazy: t.Optional[bool] = None
     ) -> ScannedDependency:
         if hasattr(member, "__wrapped__"):
             member = member.__wrapped__
         return ScannedDependency(member=member, module=module, lazy=lazy)
 
     # Inspection
 
@@ -790,15 +790,15 @@
             else:
                 kwargs[parameter.name] = instance
         return args, kwargs
 
     def _get_injectable_params(self, obj: t.Callable[..., t.Any]) -> t.Dict[str, t.Any]:
         injectable_params = {}
         for parameter in get_signature(obj).parameters.values():
-            if not isinstance(parameter.default, _DependencyMark):
+            if not isinstance(parameter.default, DependencyMark):
                 continue
 
             annotation = parameter.annotation
             if annotation is inspect._empty:  # noqa
                 raise AnnotationError(
                     f"Missing `{get_full_qualname(obj)}` parameter annotation."
                 )
@@ -883,29 +883,38 @@
         self.start()
         return self
 
     def __exit__(
         self,
         exc_type: t.Type[BaseException] | None,
         exc_val: BaseException | None,
-        exc_tb: TracebackType | None,
+        exc_tb: types.TracebackType | None,
     ) -> None:
         self.close()
         return
 
     async def __aenter__(self) -> ScopedContext:
         await self.astart()
         return self
 
     async def __aexit__(
         self,
         exc_type: t.Type[BaseException] | None,
         exc_val: BaseException | None,
-        exc_tb: TracebackType | None,
+        exc_tb: types.TracebackType | None,
     ) -> None:
         await self.aclose()
         return
 
     def _iter_providers(self) -> t.Iterator[t.Tuple[t.Type[t.Any], Provider]]:
         for interface, provider in self._root.providers.items():
             if provider.scope == self._scope:
                 yield interface, provider
+
+
+class Module:
+    """
+    Module base class.
+    """
+
+    def configure(self, di: PyxDI) -> None:
+        ...
```

### Comparing `pyxdi-0.7.0/pyxdi/decorators.py` & `pyxdi-0.8.0/pyxdi/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,34 +28,31 @@
     ...
 
 
 @t.overload
 def provider(
     *,
     scope: t.Optional[Scope] = None,
-    tags: t.Optional[t.Iterable[str]] = None,
 ) -> t.Callable[[t.Callable[P, T]], t.Callable[P, T]]:
     ...
 
 
 def provider(
     target: t.Optional[t.Callable[P, T]] = None,
     *,
     scope: t.Optional[Scope] = None,
-    tags: t.Optional[t.Iterable[str]] = None,
 ) -> t.Union[t.Callable[P, T], t.Callable[[t.Callable[P, T]], t.Callable[P, T]]]:
     def decorator(target: t.Callable[P, T]) -> t.Callable[P, T]:
         setattr(
             target,
             "__pyxdi_provider__",
             {
                 "scope": scope,
             },
         )
-        setattr(target, "__pyxdi_tags__", tags)
         return target
 
     if target is None:
         return decorator
     return decorator(target)
```

### Comparing `pyxdi-0.7.0/pyxdi/ext/fastapi.py` & `pyxdi-0.8.0/pyxdi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `pyxdi-0.7.0/pyxdi/ext/starlette/middleware.py` & `pyxdi-0.8.0/pyxdi/ext/starlette/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
     def __init__(self, app: ASGIApp, di: pyxdi.PyxDI):
         super().__init__(app)
         self._di = di
 
     async def dispatch(
         self, request: Request, call_next: RequestResponseEndpoint
     ) -> Response:
-        async with await self._di.arequest_context() as ctx:
+        async with self._di.arequest_context() as ctx:
             ctx.set(Request, instance=request)
             return await call_next(request)
```

### Comparing `pyxdi-0.7.0/pyxdi/utils.py` & `pyxdi-0.8.0/pyxdi/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 import functools
 import inspect
 import sys
 import typing as t
 
+import lazy_object_proxy
+
 try:
     import anyio  # noqa
 
     anyio_installed = True
 except ImportError:
     anyio_installed = False
 
 
-try:
-    import lazy_object_proxy  # noqa
-
-    lazy_object_proxy_installed = True
-except ImportError:
-    lazy_object_proxy_installed = False
-
-
 HAS_SIGNATURE_EVAL_STR_ARG = sys.version_info >= (3, 10)
 
 T = t.TypeVar("T")
 
 
 def get_full_qualname(obj: t.Any) -> str:
     qualname = getattr(obj, "__qualname__", f"unknown[{type(obj).__qualname__}]")
@@ -41,19 +35,14 @@
 
 
 def is_builtin_type(tp: t.Type[t.Any]) -> bool:
     return tp.__module__ == "builtins"
 
 
 def make_lazy(func: t.Callable[..., T], /, *args: t.Any, **kwargs: t.Any) -> T:
-    if not lazy_object_proxy_installed:
-        raise ImportError(
-            "`lazy-object-proxy` library is not currently installed. Please make sure "
-            "to install it first, or consider using `pyxdi[full]` instead."
-        )
     return t.cast(T, lazy_object_proxy.Proxy(functools.partial(func, *args, **kwargs)))
 
 
 async def run_async(func: t.Callable[..., T], /, *args: t.Any, **kwargs: t.Any) -> T:
     if not anyio_installed:
         raise ImportError(
             "`anyio` library is not currently installed. Please make sure to install "
```

### Comparing `pyxdi-0.7.0/PKG-INFO` & `pyxdi-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: pyxdi
-Version: 0.7.0
+Version: 0.8.0
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/pyxdi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: all
 Provides-Extra: docs
-Requires-Dist: anyio (>=3.6.2,<4.0.0) ; extra == "all"
-Requires-Dist: lazy-object-proxy (>=1.9.0,<2.0.0) ; extra == "all"
+Requires-Dist: anyio (>=3.6.2,<4.0.0)
+Requires-Dist: lazy-object-proxy (>=1.9.0,<2.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0) ; extra == "docs"
-Requires-Dist: mkdocs-material (>=9.0.12,<10.0.0) ; extra == "docs"
+Requires-Dist: mkdocs-material (>=9.1.13,<10.0.0) ; extra == "docs"
 Project-URL: Repository, https://github.com/antonrh/pyxdi
 Description-Content-Type: text/markdown
 
 # PyxDI
 
 `PyxDI` is a modern, lightweight and async-friendly Python Dependency Injection library that leverages type annotations ([PEP 484](https://peps.python.org/pep-0484/))
 to effortlessly manage dependencies in your applications.
@@ -38,35 +37,31 @@
 
 http://pyxdi.readthedocs.io/
 
 ---
 
 ## Requirements
 
-Python 3.7+
+Python 3.8+
+
+* [lazy-object-proxy](https://github.com/ionelmc/python-lazy-object-proxy) (for supporting lazy injections)
 
 and optional dependencies:
 
 * [anyio](https://github.com/agronholm/anyio) (for supporting synchronous resources with an asynchronous runtime)
-* [lazy-object-proxy](https://github.com/ionelmc/python-lazy-object-proxy) (for supporting lazy injections)
+
 
 ## Installation
 
 Install using `pip`:
 
 ```shell
 pip install pyxdi
 ```
 
-or with all dependencies (anyio, lazy-object-proxy)
-
-```shell
-pip install pyxdi[all]
-```
-
 or using `poetry`:
 
 ```shell
 poetry add pyxdi
 ```
 
 ## Quick Example
```

