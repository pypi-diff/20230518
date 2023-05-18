# Comparing `tmp/muffin_grpc-0.5.5.tar.gz` & `tmp/muffin_grpc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_grpc-0.5.5.tar", max compression
+gzip compressed data, was "muffin_grpc-0.6.0.tar", max compression
```

## Comparing `muffin_grpc-0.5.5.tar` & `muffin_grpc-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6014 2023-04-11 06:24:08.703393 muffin_grpc-0.5.5/README.rst
--rw-r--r--   0        0        0     6947 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/muffin_grpc/__init__.py
--rw-r--r--   0        0        0    11986 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/muffin_grpc/proto3.py
--rw-r--r--   0        0        0        0 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/muffin_grpc/py.typed
--rw-r--r--   0        0        0     1420 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/muffin_grpc/utils.py
--rw-r--r--   0        0        0     1969 2023-04-11 06:24:08.707393 muffin_grpc-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     7262 1970-01-01 00:00:00.000000 muffin_grpc-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     6018 2023-05-18 05:44:23.175222 muffin_grpc-0.6.0/README.rst
+-rw-r--r--   0        0        0     7251 2023-05-18 05:44:23.175222 muffin_grpc-0.6.0/muffin_grpc/__init__.py
+-rw-r--r--   0        0        0    11986 2023-05-18 05:44:23.175222 muffin_grpc-0.6.0/muffin_grpc/proto3.py
+-rw-r--r--   0        0        0        0 2023-05-18 05:44:23.175222 muffin_grpc-0.6.0/muffin_grpc/py.typed
+-rw-r--r--   0        0        0     1420 2023-05-18 05:44:23.175222 muffin_grpc-0.6.0/muffin_grpc/utils.py
+-rw-r--r--   0        0        0     2020 2023-05-18 05:44:23.175222 muffin_grpc-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7266 1970-01-01 00:00:00.000000 muffin_grpc-0.6.0/PKG-INFO
```

### Comparing `muffin_grpc-0.5.5/README.rst` & `muffin_grpc-0.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     from .proto.helloworld import GreeterStub, HelloRequest
 
     @app.route('/')
     async def index(request):
         name = request.url.query.get('name') or 'anonymous'
         try:
-            async with grpc.channel() as channel:
+            async with grpc.get_channel() as channel:
                 stub = GreeterStub(channel)
                 response = await stub.SayHello(
                     HelloRequest(name=request.url.query['name']), timeout=10)
                 message = response.message
 
         except AioRpcError as exc:
             message = exc.details()
```

### Comparing `muffin_grpc-0.5.5/muffin_grpc/__init__.py` & `muffin_grpc-0.6.0/muffin_grpc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Support GRPC for Muffin Framework."""
 import asyncio
 import logging
+from contextlib import suppress
 from functools import cached_property
 from importlib import import_module
 from pathlib import Path
 from signal import SIGINT, SIGTERM
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import grpc
@@ -41,14 +42,15 @@
     def __init__(self, *args, **kwargs):
         """Initialize the plugin."""
         super(Plugin, self).__init__(*args, **kwargs)
         self.proto_files: List[
             Tuple[Union[str, Path], Optional[Union[str, Path]], Dict[str, Any]]
         ] = []
         self.services = []
+        self.channel = None
 
     def setup(self, app: "Application", **options):
         """Setup grpc commands."""
         super(Plugin, self).setup(app, **options)
         self.logger = app.logger
 
         @app.manage(lifespan=True)
@@ -73,14 +75,22 @@
 
         # TODO: Proto specs
         # -----------------
         #  @app.route('proto/specs')
         #  async def proto_specs(request):
         #      pass
 
+    async def startup(self):
+        with suppress(PluginError):
+            self.channel = self.get_channel()
+
+    async def shutdown(self):
+        if self.channel is not None:
+            await self.channel.close()
+
     @cached_property
     def server(self) -> grpc.aio.Server:
         """Generate a GRPC server with registered services."""
         server = grpc.aio.server()
         for service_cls, register in self.services:
             register(service_cls(), server)
         if self.cfg.ssl_server:
@@ -91,64 +101,60 @@
 
         else:
             server.add_insecure_port(self.cfg.server_listen)
 
         return server
 
     def add_proto(
-        self,
-        path: Union[str, Path],
-        build_dir: Optional[Union[str, Path]] = None,
-        build_package: Optional[str] = None,
-        targets: Optional[List[Path]] = None,
+        self, path: Union[str, Path], build_dir: Optional[Union[str, Path]] = None, **params
     ):
         """Register/build the given proto file."""
         path = Path(path).absolute()
         build_dir = Path(build_dir or self.cfg.build_dir or path.parent)
         self.proto_files.append(
-            (path, build_dir, {"build_package": build_package, "targets": targets}),
+            (path, build_dir, params),
         )
         if self.cfg.autobuild:
-            return self.build_proto(
-                path,
-                build_dir=build_dir,
-                build_package=build_package,
-                targets=targets,
-            )
+            return self.build_proto(path, build_dir=build_dir, **params)
 
         else:
             return [build_dir / f"{ path.stem }_pb2.py"]
 
     def add_to_server(self, service_cls):
         """Register the given service class to the server."""
         proto_cls = service_cls.mro()[-2]
         proto_module = import_module(proto_cls.__module__)
         register = getattr(proto_module, f"add_{ proto_cls.__name__ }_to_server")
         self.services.append((service_cls, register))
 
-    def channel(self, target: Optional[str] = None, **options):
+    def get_channel(self, address: Optional[str] = None, **options):
         """Open a channel."""
+        address = address or self.cfg.default_channel
+        if address is None:
+            raise PluginError("No default channel")
+
         if self.cfg.ssl_client:
             return grpc.aio.secure_channel(
-                target or self.cfg.default_channel,
+                address or self.cfg.default_channel,
                 grpc.ssl_channel_credentials(*self.cfg.ssl_client_params or ()),
                 **(options or self.cfg.default_channel_options),
             )
 
         return grpc.aio.insecure_channel(
-            target=target or self.cfg.default_channel,
+            target=address or self.cfg.default_channel,
             **(options or self.cfg.default_channel_options),
         )
 
-    def build_proto(
+    def build_proto(  # noqa: PLR0913
         self,
         path: Union[str, Path],
         build_dir: Optional[Union[str, Path]] = None,
         build_package: Optional[Union[str, bool]] = None,
         targets: Optional[List[Path]] = None,
+        include: Optional[List[Path]] = None,
     ) -> List[Path]:
         """Build the given proto."""
         path = Path(path)
         if not path.exists():
             return []
 
         proto_updated = path.stat().st_ctime
@@ -187,14 +193,15 @@
 
             _generate_file(build_dir / "__init__.py")
 
             args = [
                 "grpc_tools.protoc",
                 f"--proto_path={ path.parent }",
                 f"--proto_path={ INCLUDE }",
+                *([f"--proto_path={ include }" for include in include or []]),
                 *args,
                 str(path),
             ]
             res = protoc.main(args)
             if res != 0:
                 raise PluginError("{} failed".format(" ".join(args)))
```

### Comparing `muffin_grpc-0.5.5/muffin_grpc/proto3.py` & `muffin_grpc-0.6.0/muffin_grpc/proto3.py`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.5/muffin_grpc/utils.py` & `muffin_grpc-0.6.0/muffin_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_grpc-0.5.5/pyproject.toml` & `muffin_grpc-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-grpc"
-version = "0.5.5"
+version = "0.6.0"
 description = "GRPC support for Muffin framework."
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-grpc"
 repository = "https://github.com/klen/muffin-grpc"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["grpc", "muffin", "asyncio", "asgi", "web"]
@@ -16,17 +16,15 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Framework :: AsyncIO",
 ]
-packages = [
-  { include = "muffin_grpc" },
-]
+packages = [{ include = "muffin_grpc" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 muffin = "^0"
 grpcio = "^1"
 grpcio-tools = "^1"
 parsy = "*"
@@ -74,17 +72,33 @@
 
 [tool.ruff]
 fix = true
 line-length = 100
 target-version = "py38"
 exclude = [".venv", "docs", "examples"]
 select = ["ALL"]
-ignore = ["D", "UP", "ANN", "DJ", "EM", "RSE", "SLF", "RET", "S101", "PLR2004", "PLR0912", "N804", "A003", "TRY003"]
+ignore = [
+  "ANN",
+  "COM",
+  "D",
+  "DJ",
+  "EM",
+  "UP",
+  "RSE",
+  "SLF",
+  "RET",
+  "S101",
+  "PLR2004",
+  "PLR0912",
+  "N804",
+  "A003",
+  "TRY003",
+]
 
 [tool.black]
 line-length = 100
-target-version = ["py310", "py311"]
+target-version = ["py38", "py39", "py310", "py311"]
 preview = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `muffin_grpc-0.5.5/PKG-INFO` & `muffin_grpc-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-grpc
-Version: 0.5.5
+Version: 0.6.0
 Summary: GRPC support for Muffin framework.
 Home-page: https://github.com/klen/muffin-grpc
 License: MIT
 Keywords: grpc,muffin,asyncio,asgi,web
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -164,15 +164,15 @@
 
     from .proto.helloworld import GreeterStub, HelloRequest
 
     @app.route('/')
     async def index(request):
         name = request.url.query.get('name') or 'anonymous'
         try:
-            async with grpc.channel() as channel:
+            async with grpc.get_channel() as channel:
                 stub = GreeterStub(channel)
                 response = await stub.SayHello(
                     HelloRequest(name=request.url.query['name']), timeout=10)
                 message = response.message
 
         except AioRpcError as exc:
             message = exc.details()
```

