# Comparing `tmp/dagger_io-0.5.3.tar.gz` & `tmp/dagger_io-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagger_io-0.5.3.tar", max compression
+gzip compressed data, was "dagger_io-0.5.4.tar", max compression
```

## Comparing `dagger_io-0.5.3.tar` & `dagger_io-0.5.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0    10758 2023-05-11 19:41:57.916076 dagger_io-0.5.3/LICENSE
--rw-r--r--   0        0        0     4727 2023-05-11 19:41:57.916076 dagger_io-0.5.3/README.md
--rw-r--r--   0        0        0     6344 2023-05-11 19:43:04.841204 dagger_io-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      313 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/__init__.py
--rw-r--r--   0        0        0       49 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/__main__.py
--rw-r--r--   0        0        0       69 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/.gitattributes
--rw-r--r--   0        0        0        0 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/__init__.py
--rw-r--r--   0        0        0    11434 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/base.py
--rw-r--r--   0        0        0    83180 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/gen.py
--rw-r--r--   0        0        0    82872 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/api/gen_sync.py
--rw-r--r--   0        0        0     1683 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/cli.py
--rw-r--r--   0        0        0    18459 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/codegen.py
--rw-r--r--   0        0        0     1302 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/config.py
--rw-r--r--   0        0        0     1585 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/connection.py
--rw-r--r--   0        0        0      964 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/context.py
--rw-r--r--   0        0        0       37 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/.gitattributes
--rw-r--r--   0        0        0       35 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/__init__.py
--rw-r--r--   0        0        0       64 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/_version.py
--rw-r--r--   0        0        0     4202 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/cli.py
--rw-r--r--   0        0        0     2068 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/conn.py
--rw-r--r--   0        0        0     8163 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/engine/download.py
--rw-r--r--   0        0        0     3042 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/exceptions.py
--rw-r--r--   0        0        0      677 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/log.py
--rw-r--r--   0        0        0        0 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/py.typed
--rw-r--r--   0        0        0     2320 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/server/__init__.py
--rw-r--r--   0        0        0      911 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/server/cli.py
--rw-r--r--   0        0        0      865 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/server/converter.py
--rw-r--r--   0        0        0     3892 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/session.py
--rw-r--r--   0        0        0        0 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/transport/__init__.py
--rw-r--r--   0        0        0     5820 2023-05-11 19:41:57.916076 dagger_io-0.5.3/src/dagger/transport/httpx.py
--rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.5.3/setup.py
--rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-18 17:53:16.702461 dagger_io-0.5.4/LICENSE
+-rw-r--r--   0        0        0     4727 2023-05-18 17:53:16.702461 dagger_io-0.5.4/README.md
+-rw-r--r--   0        0        0     6344 2023-05-18 17:54:33.893909 dagger_io-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/__main__.py
+-rw-r--r--   0        0        0       69 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/.gitattributes
+-rw-r--r--   0        0        0        0 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/__init__.py
+-rw-r--r--   0        0        0    11866 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/base.py
+-rw-r--r--   0        0        0    88720 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/gen.py
+-rw-r--r--   0        0        0    88384 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/gen_sync.py
+-rw-r--r--   0        0        0     1683 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/cli.py
+-rw-r--r--   0        0        0    19680 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/codegen.py
+-rw-r--r--   0        0        0     1302 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/config.py
+-rw-r--r--   0        0        0     1585 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/connection.py
+-rw-r--r--   0        0        0      964 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/context.py
+-rw-r--r--   0        0        0       37 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/.gitattributes
+-rw-r--r--   0        0        0       35 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/_version.py
+-rw-r--r--   0        0        0     4202 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/cli.py
+-rw-r--r--   0        0        0     2068 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/conn.py
+-rw-r--r--   0        0        0     8163 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/download.py
+-rw-r--r--   0        0        0     3042 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/exceptions.py
+-rw-r--r--   0        0        0      677 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/py.typed
+-rw-r--r--   0        0        0     2320 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/server/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/server/__main__.py
+-rw-r--r--   0        0        0      911 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/server/cli.py
+-rw-r--r--   0        0        0      865 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/server/converter.py
+-rw-r--r--   0        0        0     3892 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/session.py
+-rw-r--r--   0        0        0        0 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/transport/__init__.py
+-rw-r--r--   0        0        0     5820 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/transport/httpx.py
+-rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.5.4/setup.py
+-rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.5.4/PKG-INFO
```

### Comparing `dagger_io-0.5.3/LICENSE` & `dagger_io-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/README.md` & `dagger_io-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/pyproject.toml` & `dagger_io-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dagger-io"
-version = "0.5.3"
+version = "0.5.4"
 description = "A client package for running Dagger pipelines in Python."
 license = "Apache-2.0"
 authors = ["Dagger <hello@dagger.io>"]
 readme = "README.md"
 homepage = "https://dagger.io"
 documentation = "https://docs.dagger.io/sdk/python"
 repository = "https://github.com/dagger/dagger/tree/main/sdk/python"
```

### Comparing `dagger_io-0.5.3/src/dagger/api/base.py` & `dagger_io-0.5.4/src/dagger/api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 import enum
 import functools
 import logging
 import typing
 from collections import deque
 from collections.abc import Callable, Sequence
-from typing import Annotated, Any, ParamSpec, TypeGuard, TypeVar
+from typing import Annotated, Any, ParamSpec, TypeGuard, TypeVar, overload
 
 import anyio
 import attrs
 import cattrs
 import graphql
 import httpx
 from beartype import beartype
@@ -87,29 +87,45 @@
             selectable = parent.select(selectable)
 
         return selectable
 
     def query(self) -> graphql.DocumentNode:
         return dsl_gql(DSLQuery(self.build()))
 
+    @overload
+    async def execute(self, return_type: None) -> None:
+        ...
+
+    @overload
     async def execute(self, return_type: type[T]) -> T:
+        ...
+
+    async def execute(self, return_type: type[T] | None = None) -> T | None:
         assert isinstance(self.session, AsyncClientSession)
         await self.resolve_ids()
         query = self.query()
         with self._handle_execute(query):
             result = await self.session.execute(query)
-        return self.get_value(result, return_type)
+        return self.get_value(result, return_type) if return_type else None
 
+    @overload
+    def execute_sync(self, return_type: None) -> None:
+        ...
+
+    @overload
     def execute_sync(self, return_type: type[T]) -> T:
+        ...
+
+    def execute_sync(self, return_type: type[T] | None = None) -> T | None:
         assert isinstance(self.session, SyncClientSession)
         self.resolve_ids_sync()
         query = self.query()
         with self._handle_execute(query):
             result = self.session.execute(query)
-        return self.get_value(result, return_type)
+        return self.get_value(result, return_type) if return_type else None
 
     async def resolve_ids(self) -> None:
         """Replace Type object instances with their ID implicitly."""
 
         # mutating to avoid re-fetching on forked pipeline
         async def _resolve_id(pos: int, k: str, v: IDType):
             sel = self.selections[pos]
```

### Comparing `dagger_io-0.5.3/src/dagger/api/gen.py` & `dagger_io-0.5.4/src/dagger/api/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 
 class Platform(Scalar):
     """The platform config OS and architecture in a Container.  The format
     is [os]/[platform]/[version] (e.g., "darwin/arm64/v7",
     "windows/amd64", "linux/arm64")."""
 
 
+class ProjectCommandID(Scalar):
+    """A unique project command identifier."""
+
+
+class ProjectID(Scalar):
+    """A unique project identifier."""
+
+
 class SecretID(Scalar):
     """A unique identifier for a secret."""
 
 
 class SocketID(Scalar):
     """A content-addressed socket identifier."""
 
@@ -50,14 +58,26 @@
     PRIVATE = "PRIVATE"
     """Keeps a cache volume for a single build pipeline"""
 
     SHARED = "SHARED"
     """Shares the cache volume amongst many build pipelines"""
 
 
+class ImageLayerCompression(Enum):
+    """Compression algorithm to use for image layers"""
+
+    EStarGZ = "EStarGZ"
+
+    Gzip = "Gzip"
+
+    Uncompressed = "Uncompressed"
+
+    Zstd = "Zstd"
+
+
 class NetworkProtocol(Enum):
     """Transport layer network protocol associated to a port."""
 
     TCP = "TCP"
     """TCP (Transmission Control Protocol)"""
 
     UDP = "UDP"
@@ -365,14 +385,15 @@
         return await _ctx.execute(int)
 
     @typecheck
     async def export(
         self,
         path: str,
         platform_variants: Optional[Sequence["Container"]] = None,
+        forced_compression: Optional[ImageLayerCompression] = None,
     ) -> bool:
         """Writes the container as an OCI tarball to the destination file path on
         the host for the specified platform variants.
 
         Return true on success.
         It can also publishes platform variants.
 
@@ -380,14 +401,24 @@
         ----------
         path:
             Host's destination path (e.g., "./tarball").
             Path can be relative to the engine's workdir or absolute.
         platform_variants:
             Identifiers for other platform specific containers.
             Used for multi-platform image.
+        forced_compression:
+            Force each layer of the exported image to use the specified
+            compression algorithm.
+            If this is unset, then if a layer already has a compressed blob in
+            the engine's
+            cache, that will be used (this can result in a mix of compression
+            algorithms for
+            different layers). If this is unset and a layer has no compressed
+            blob in the
+            engine's cache, then it will be compressed using Gzip.
 
         Returns
         -------
         bool
             The `Boolean` scalar type represents `true` or `false`.
 
         Raises
@@ -396,14 +427,15 @@
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
             Arg("platformVariants", platform_variants, None),
+            Arg("forcedCompression", forced_compression, None),
         ]
         _ctx = self._select("export", _args)
         return await _ctx.execute(bool)
 
     @typecheck
     def exposed_ports(self) -> "Port":
         """Retrieves the list of exposed ports.
@@ -665,14 +697,15 @@
         return await _ctx.execute(Platform)
 
     @typecheck
     async def publish(
         self,
         address: str,
         platform_variants: Optional[Sequence["Container"]] = None,
+        forced_compression: Optional[ImageLayerCompression] = None,
     ) -> str:
         """Publishes this container as a new image to the specified address.
 
         Publish returns a fully qualified ref.
         It can also publish platform variants.
 
         Parameters
@@ -680,14 +713,24 @@
         address:
             Registry's address to publish the image to.
             Formatted as [host]/[user]/[repo]:[tag] (e.g.
             "docker.io/dagger/dagger:main").
         platform_variants:
             Identifiers for other platform specific containers.
             Used for multi-platform image.
+        forced_compression:
+            Force each layer of the published image to use the specified
+            compression algorithm.
+            If this is unset, then if a layer already has a compressed blob in
+            the engine's
+            cache, that will be used (this can result in a mix of compression
+            algorithms for
+            different layers). If this is unset and a layer has no compressed
+            blob in the
+            engine's cache, then it will be compressed using Gzip.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -698,14 +741,15 @@
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("address", address),
             Arg("platformVariants", platform_variants, None),
+            Arg("forcedCompression", forced_compression, None),
         ]
         _ctx = self._select("publish", _args)
         return await _ctx.execute(str)
 
     @typecheck
     def rootfs(self) -> "Directory":
         """Retrieves this container's root filesystem. Mounts are not included."""
@@ -760,14 +804,32 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("stdout", _args)
         return await _ctx.execute(str)
 
     @typecheck
+    async def sync(self) -> "Container":
+        """Forces evaluation of the pipeline in the engine.
+
+        It doesn't run the default command if no exec has been set.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("sync", _args)
+        await _ctx.execute()
+        return self
+
+    @typecheck
     async def user(self) -> Optional[str]:
         """Retrieves the user to be set for all commands.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
@@ -1653,23 +1715,14 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(DirectoryID)
 
     @typecheck
-    def load_project(self, config_path: str) -> "Project":
-        """load a project's metadata"""
-        _args = [
-            Arg("configPath", config_path),
-        ]
-        _ctx = self._select("loadProject", _args)
-        return Project(_ctx)
-
-    @typecheck
     def pipeline(
         self,
         name: str,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
     ) -> "Directory":
         """Creates a named sub-pipeline
@@ -2400,53 +2453,148 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("protocol", _args)
         return await _ctx.execute(NetworkProtocol)
 
 
 class Project(Type):
-    """A set of scripts and/or extensions"""
+    """A collection of Dagger resources that can be queried and
+    invoked."""
 
     @typecheck
-    def extensions(self) -> "Project":
-        """extensions in this project"""
+    def commands(self) -> "ProjectCommand":
+        """Commands provided by this project"""
         _args: list[Arg] = []
-        _ctx = self._select("extensions", _args)
+        _ctx = self._select("commands", _args)
+        return ProjectCommand(_ctx)
+
+    @typecheck
+    async def id(self) -> str:
+        """A unique identifier for this project.
+
+        Note
+        ----
+        This is lazyly evaluated, no operation is actually run.
+
+        Returns
+        -------
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("id", _args)
+        return await _ctx.execute(str)
+
+    @typecheck
+    def load(
+        self,
+        source: Directory,
+        config_path: str,
+    ) -> "Project":
+        """Initialize this project from the given directory and config path"""
+        _args = [
+            Arg("source", source),
+            Arg("configPath", config_path),
+        ]
+        _ctx = self._select("load", _args)
         return Project(_ctx)
 
     @typecheck
-    def generated_code(self) -> Directory:
-        """Code files generated by the SDKs in the project"""
+    async def name(self) -> str:
+        """Name of the project
+
+        Returns
+        -------
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("name", _args)
+        return await _ctx.execute(str)
+
+
+class ProjectCommand(Type):
+    """A command defined in a project that can be invoked from the CLI."""
+
+    @typecheck
+    async def description(self) -> Optional[str]:
+        """Documentation for what this command does.
+
+        Returns
+        -------
+        Optional[str]
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
         _args: list[Arg] = []
-        _ctx = self._select("generatedCode", _args)
-        return Directory(_ctx)
+        _ctx = self._select("description", _args)
+        return await _ctx.execute(Optional[str])
+
+    @typecheck
+    def flags(self) -> "ProjectCommandFlag":
+        """Flags accepted by this command."""
+        _args: list[Arg] = []
+        _ctx = self._select("flags", _args)
+        return ProjectCommandFlag(_ctx)
 
     @typecheck
-    async def install(self) -> bool:
-        """install the project's schema
+    async def id(self) -> str:
+        """A unique identifier for this command.
+
+        Note
+        ----
+        This is lazyly evaluated, no operation is actually run.
 
         Returns
         -------
-        bool
-            The `Boolean` scalar type represents `true` or `false`.
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("install", _args)
-        return await _ctx.execute(bool)
+        _ctx = self._select("id", _args)
+        return await _ctx.execute(str)
 
     @typecheck
     async def name(self) -> str:
-        """name of the project
+        """The name of the command.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -2459,16 +2607,27 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
-    async def schema(self) -> Optional[str]:
-        """schema provided by the project
+    def subcommands(self) -> "ProjectCommand":
+        """Subcommands, if any, that this command provides."""
+        _args: list[Arg] = []
+        _ctx = self._select("subcommands", _args)
+        return ProjectCommand(_ctx)
+
+
+class ProjectCommandFlag(Type):
+    """A flag accepted by a project command."""
+
+    @typecheck
+    async def description(self) -> Optional[str]:
+        """Documentation for what this flag sets.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -2477,38 +2636,38 @@
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("schema", _args)
+        _ctx = self._select("description", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
-    async def sdk(self) -> Optional[str]:
-        """sdk used to generate code for and/or execute this project
+    async def name(self) -> str:
+        """The name of the flag.
 
         Returns
         -------
-        Optional[str]
+        str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("sdk", _args)
-        return await _ctx.execute(Optional[str])
+        _ctx = self._select("name", _args)
+        return await _ctx.execute(str)
 
 
 class Client(Root):
     @typecheck
     def cache_volume(self, key: str) -> CacheVolume:
         """Constructs a cache volume for a given cache key.
 
@@ -2665,23 +2824,35 @@
             Arg("description", description, None),
             Arg("labels", labels, None),
         ]
         _ctx = self._select("pipeline", _args)
         return Client(_ctx)
 
     @typecheck
-    def project(self, name: str) -> Project:
-        """Look up a project by name"""
+    def project(self, id: Optional[ProjectID] = None) -> Project:
+        """Load a project from ID."""
         _args = [
-            Arg("name", name),
+            Arg("id", id, None),
         ]
         _ctx = self._select("project", _args)
         return Project(_ctx)
 
     @typecheck
+    def project_command(
+        self,
+        id: Optional[ProjectCommandID] = None,
+    ) -> ProjectCommand:
+        """Load a project command from ID."""
+        _args = [
+            Arg("id", id, None),
+        ]
+        _ctx = self._select("projectCommand", _args)
+        return ProjectCommand(_ctx)
+
+    @typecheck
     def secret(self, id: SecretID) -> "Secret":
         """Loads a secret from its ID."""
         _args = [
             Arg("id", id),
         ]
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
@@ -2794,17 +2965,20 @@
 
 __all__ = [
     "CacheID",
     "ContainerID",
     "DirectoryID",
     "FileID",
     "Platform",
+    "ProjectCommandID",
+    "ProjectID",
     "SecretID",
     "SocketID",
     "CacheSharingMode",
+    "ImageLayerCompression",
     "NetworkProtocol",
     "BuildArg",
     "PipelineLabel",
     "CacheVolume",
     "Container",
     "Directory",
     "EnvVariable",
@@ -2812,11 +2986,13 @@
     "GitRef",
     "GitRepository",
     "Host",
     "HostVariable",
     "Label",
     "Port",
     "Project",
+    "ProjectCommand",
+    "ProjectCommandFlag",
     "Client",
     "Secret",
     "Socket",
 ]
```

### Comparing `dagger_io-0.5.3/src/dagger/api/gen_sync.py` & `dagger_io-0.5.4/src/dagger/api/gen_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 
 class Platform(Scalar):
     """The platform config OS and architecture in a Container.  The format
     is [os]/[platform]/[version] (e.g., "darwin/arm64/v7",
     "windows/amd64", "linux/arm64")."""
 
 
+class ProjectCommandID(Scalar):
+    """A unique project command identifier."""
+
+
+class ProjectID(Scalar):
+    """A unique project identifier."""
+
+
 class SecretID(Scalar):
     """A unique identifier for a secret."""
 
 
 class SocketID(Scalar):
     """A content-addressed socket identifier."""
 
@@ -50,14 +58,26 @@
     PRIVATE = "PRIVATE"
     """Keeps a cache volume for a single build pipeline"""
 
     SHARED = "SHARED"
     """Shares the cache volume amongst many build pipelines"""
 
 
+class ImageLayerCompression(Enum):
+    """Compression algorithm to use for image layers"""
+
+    EStarGZ = "EStarGZ"
+
+    Gzip = "Gzip"
+
+    Uncompressed = "Uncompressed"
+
+    Zstd = "Zstd"
+
+
 class NetworkProtocol(Enum):
     """Transport layer network protocol associated to a port."""
 
     TCP = "TCP"
     """TCP (Transmission Control Protocol)"""
 
     UDP = "UDP"
@@ -365,14 +385,15 @@
         return _ctx.execute_sync(int)
 
     @typecheck
     def export(
         self,
         path: str,
         platform_variants: Optional[Sequence["Container"]] = None,
+        forced_compression: Optional[ImageLayerCompression] = None,
     ) -> bool:
         """Writes the container as an OCI tarball to the destination file path on
         the host for the specified platform variants.
 
         Return true on success.
         It can also publishes platform variants.
 
@@ -380,14 +401,24 @@
         ----------
         path:
             Host's destination path (e.g., "./tarball").
             Path can be relative to the engine's workdir or absolute.
         platform_variants:
             Identifiers for other platform specific containers.
             Used for multi-platform image.
+        forced_compression:
+            Force each layer of the exported image to use the specified
+            compression algorithm.
+            If this is unset, then if a layer already has a compressed blob in
+            the engine's
+            cache, that will be used (this can result in a mix of compression
+            algorithms for
+            different layers). If this is unset and a layer has no compressed
+            blob in the
+            engine's cache, then it will be compressed using Gzip.
 
         Returns
         -------
         bool
             The `Boolean` scalar type represents `true` or `false`.
 
         Raises
@@ -396,14 +427,15 @@
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
             Arg("platformVariants", platform_variants, None),
+            Arg("forcedCompression", forced_compression, None),
         ]
         _ctx = self._select("export", _args)
         return _ctx.execute_sync(bool)
 
     @typecheck
     def exposed_ports(self) -> "Port":
         """Retrieves the list of exposed ports.
@@ -665,14 +697,15 @@
         return _ctx.execute_sync(Platform)
 
     @typecheck
     def publish(
         self,
         address: str,
         platform_variants: Optional[Sequence["Container"]] = None,
+        forced_compression: Optional[ImageLayerCompression] = None,
     ) -> str:
         """Publishes this container as a new image to the specified address.
 
         Publish returns a fully qualified ref.
         It can also publish platform variants.
 
         Parameters
@@ -680,14 +713,24 @@
         address:
             Registry's address to publish the image to.
             Formatted as [host]/[user]/[repo]:[tag] (e.g.
             "docker.io/dagger/dagger:main").
         platform_variants:
             Identifiers for other platform specific containers.
             Used for multi-platform image.
+        forced_compression:
+            Force each layer of the published image to use the specified
+            compression algorithm.
+            If this is unset, then if a layer already has a compressed blob in
+            the engine's
+            cache, that will be used (this can result in a mix of compression
+            algorithms for
+            different layers). If this is unset and a layer has no compressed
+            blob in the
+            engine's cache, then it will be compressed using Gzip.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -698,14 +741,15 @@
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("address", address),
             Arg("platformVariants", platform_variants, None),
+            Arg("forcedCompression", forced_compression, None),
         ]
         _ctx = self._select("publish", _args)
         return _ctx.execute_sync(str)
 
     @typecheck
     def rootfs(self) -> "Directory":
         """Retrieves this container's root filesystem. Mounts are not included."""
@@ -760,14 +804,32 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("stdout", _args)
         return _ctx.execute_sync(str)
 
     @typecheck
+    def sync(self) -> "Container":
+        """Forces evaluation of the pipeline in the engine.
+
+        It doesn't run the default command if no exec has been set.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("sync", _args)
+        _ctx.execute_sync()
+        return self
+
+    @typecheck
     def user(self) -> Optional[str]:
         """Retrieves the user to be set for all commands.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
@@ -1653,23 +1715,14 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(DirectoryID)
 
     @typecheck
-    def load_project(self, config_path: str) -> "Project":
-        """load a project's metadata"""
-        _args = [
-            Arg("configPath", config_path),
-        ]
-        _ctx = self._select("loadProject", _args)
-        return Project(_ctx)
-
-    @typecheck
     def pipeline(
         self,
         name: str,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
     ) -> "Directory":
         """Creates a named sub-pipeline
@@ -2400,53 +2453,148 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("protocol", _args)
         return _ctx.execute_sync(NetworkProtocol)
 
 
 class Project(Type):
-    """A set of scripts and/or extensions"""
+    """A collection of Dagger resources that can be queried and
+    invoked."""
 
     @typecheck
-    def extensions(self) -> "Project":
-        """extensions in this project"""
+    def commands(self) -> "ProjectCommand":
+        """Commands provided by this project"""
         _args: list[Arg] = []
-        _ctx = self._select("extensions", _args)
+        _ctx = self._select("commands", _args)
+        return ProjectCommand(_ctx)
+
+    @typecheck
+    def id(self) -> str:
+        """A unique identifier for this project.
+
+        Note
+        ----
+        This is lazyly evaluated, no operation is actually run.
+
+        Returns
+        -------
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("id", _args)
+        return _ctx.execute_sync(str)
+
+    @typecheck
+    def load(
+        self,
+        source: Directory,
+        config_path: str,
+    ) -> "Project":
+        """Initialize this project from the given directory and config path"""
+        _args = [
+            Arg("source", source),
+            Arg("configPath", config_path),
+        ]
+        _ctx = self._select("load", _args)
         return Project(_ctx)
 
     @typecheck
-    def generated_code(self) -> Directory:
-        """Code files generated by the SDKs in the project"""
+    def name(self) -> str:
+        """Name of the project
+
+        Returns
+        -------
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("name", _args)
+        return _ctx.execute_sync(str)
+
+
+class ProjectCommand(Type):
+    """A command defined in a project that can be invoked from the CLI."""
+
+    @typecheck
+    def description(self) -> Optional[str]:
+        """Documentation for what this command does.
+
+        Returns
+        -------
+        Optional[str]
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
         _args: list[Arg] = []
-        _ctx = self._select("generatedCode", _args)
-        return Directory(_ctx)
+        _ctx = self._select("description", _args)
+        return _ctx.execute_sync(Optional[str])
+
+    @typecheck
+    def flags(self) -> "ProjectCommandFlag":
+        """Flags accepted by this command."""
+        _args: list[Arg] = []
+        _ctx = self._select("flags", _args)
+        return ProjectCommandFlag(_ctx)
 
     @typecheck
-    def install(self) -> bool:
-        """install the project's schema
+    def id(self) -> str:
+        """A unique identifier for this command.
+
+        Note
+        ----
+        This is lazyly evaluated, no operation is actually run.
 
         Returns
         -------
-        bool
-            The `Boolean` scalar type represents `true` or `false`.
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("install", _args)
-        return _ctx.execute_sync(bool)
+        _ctx = self._select("id", _args)
+        return _ctx.execute_sync(str)
 
     @typecheck
     def name(self) -> str:
-        """name of the project
+        """The name of the command.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -2459,16 +2607,27 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return _ctx.execute_sync(str)
 
     @typecheck
-    def schema(self) -> Optional[str]:
-        """schema provided by the project
+    def subcommands(self) -> "ProjectCommand":
+        """Subcommands, if any, that this command provides."""
+        _args: list[Arg] = []
+        _ctx = self._select("subcommands", _args)
+        return ProjectCommand(_ctx)
+
+
+class ProjectCommandFlag(Type):
+    """A flag accepted by a project command."""
+
+    @typecheck
+    def description(self) -> Optional[str]:
+        """Documentation for what this flag sets.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -2477,38 +2636,38 @@
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("schema", _args)
+        _ctx = self._select("description", _args)
         return _ctx.execute_sync(Optional[str])
 
     @typecheck
-    def sdk(self) -> Optional[str]:
-        """sdk used to generate code for and/or execute this project
+    def name(self) -> str:
+        """The name of the flag.
 
         Returns
         -------
-        Optional[str]
+        str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("sdk", _args)
-        return _ctx.execute_sync(Optional[str])
+        _ctx = self._select("name", _args)
+        return _ctx.execute_sync(str)
 
 
 class Client(Root):
     @typecheck
     def cache_volume(self, key: str) -> CacheVolume:
         """Constructs a cache volume for a given cache key.
 
@@ -2665,23 +2824,35 @@
             Arg("description", description, None),
             Arg("labels", labels, None),
         ]
         _ctx = self._select("pipeline", _args)
         return Client(_ctx)
 
     @typecheck
-    def project(self, name: str) -> Project:
-        """Look up a project by name"""
+    def project(self, id: Optional[ProjectID] = None) -> Project:
+        """Load a project from ID."""
         _args = [
-            Arg("name", name),
+            Arg("id", id, None),
         ]
         _ctx = self._select("project", _args)
         return Project(_ctx)
 
     @typecheck
+    def project_command(
+        self,
+        id: Optional[ProjectCommandID] = None,
+    ) -> ProjectCommand:
+        """Load a project command from ID."""
+        _args = [
+            Arg("id", id, None),
+        ]
+        _ctx = self._select("projectCommand", _args)
+        return ProjectCommand(_ctx)
+
+    @typecheck
     def secret(self, id: SecretID) -> "Secret":
         """Loads a secret from its ID."""
         _args = [
             Arg("id", id),
         ]
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
@@ -2794,17 +2965,20 @@
 
 __all__ = [
     "CacheID",
     "ContainerID",
     "DirectoryID",
     "FileID",
     "Platform",
+    "ProjectCommandID",
+    "ProjectID",
     "SecretID",
     "SocketID",
     "CacheSharingMode",
+    "ImageLayerCompression",
     "NetworkProtocol",
     "BuildArg",
     "PipelineLabel",
     "CacheVolume",
     "Container",
     "Directory",
     "EnvVariable",
@@ -2812,11 +2986,13 @@
     "GitRef",
     "GitRepository",
     "Host",
     "HostVariable",
     "Label",
     "Port",
     "Project",
+    "ProjectCommand",
+    "ProjectCommandFlag",
     "Client",
     "Secret",
     "Socket",
 ]
```

### Comparing `dagger_io-0.5.3/src/dagger/cli.py` & `dagger_io-0.5.4/src/dagger/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/codegen.py` & `dagger_io-0.5.4/src/dagger/codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -377,29 +377,52 @@
     """Field of an object type."""
 
     def __init__(
         self,
         ctx: Context,
         name: str,
         field: GraphQLField,
+        parent: GraphQLObjectType,
     ) -> None:
         self.ctx = ctx
         self.graphql_name = name
         self.graphql = field
 
         self.name = format_name(name)
+        self.named_type = get_named_type(field.type)
         self.args = sorted(
             (_InputField(ctx, *args, parent=self) for args in field.args.items()),
             key=attrgetter("has_default"),
         )
         self.description = field.description
 
         self.is_leaf = is_output_leaf_type(field.type)
         self.is_custom_scalar = is_custom_scalar_type(field.type)
         self.type = format_output_type(field.type).replace("Query", "Client")
+        self.convert_id = False
+
+        # FIXME: We don't have a simple way to convert any ID to its
+        # corresponding object (in codegen) so for now just return the
+        # current instance. Currently, `sync` is the only field where
+        # the error is what we care about but more could be added later.
+        # To avoid wasting a result, we return the ID which is a leaf value
+        # and triggers execution, but then convert to object in the SDK to
+        # allow continued chaining. For this, we're assuming the returned
+        # ID represents the exact same object but if that changes, we'll
+        # need to adjust.
+        if (
+            name != "id"
+            and self.is_leaf
+            and self.is_custom_scalar
+            and self.named_type.name in ctx.id_map
+        ):
+            converted = ctx.id_map[self.named_type.name]
+            if get_named_type(parent).name == converted:
+                self.type = converted
+                self.convert_id = True
 
     @joiner
     def __str__(self) -> Iterator[str]:
         yield from (
             "",
             "@typecheck",
             self.func_signature(),
@@ -428,18 +451,20 @@
             yield "_args = ["
             yield from (indent(arg.as_arg()) for arg in self.args)
             yield "]"
 
         yield f'_ctx = self._select("{self.graphql_name}", _args)'
 
         if self.is_leaf:
-            if self.ctx.sync:
-                yield f"return _ctx.execute_sync({self.type})"
+            exec_ = "_ctx.execute_sync" if self.ctx.sync else "await _ctx.execute"
+            if self.convert_id:
+                yield f"{exec_}()"
+                yield "return self"
             else:
-                yield f"return await _ctx.execute({self.type})"
+                yield f"return {exec_}({self.type})"
         else:
             yield f"return {self.type}(_ctx)"
 
     def func_doc(self) -> str:
         def _out():
             if self.description:
                 yield (textwrap.fill(line) for line in self.description.splitlines())
@@ -463,15 +488,16 @@
                         "Parameters",
                         "----------",
                     ),
                     (arg.as_doc() for arg in self.args),
                 )
 
             if self.is_leaf:
-                if return_doc := output_type_description(self.graphql.type):
+                return_doc = output_type_description(self.graphql.type)
+                if not self.convert_id and return_doc:
                     yield chain(
                         (
                             "Returns",
                             "-------",
                             self.type,
                         ),
                         wrap_indent(return_doc),
@@ -622,10 +648,10 @@
     predicate: ClassVar[Predicate] = staticmethod(is_object_type)
 
     def render_head(self, t: GraphQLObjectType) -> str:
         return super().render_head(t).replace("Query(Type)", "Client(Root)")
 
     def fields(self, t: GraphQLObjectType) -> Iterator[_ObjectField]:
         return (
-            _ObjectField(self.ctx, *args)
+            _ObjectField(self.ctx, *args, t)
             for args in cast(GraphQLFieldMap, t.fields).items()
         )
```

### Comparing `dagger_io-0.5.3/src/dagger/config.py` & `dagger_io-0.5.4/src/dagger/config.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/connection.py` & `dagger_io-0.5.4/src/dagger/connection.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/context.py` & `dagger_io-0.5.4/src/dagger/context.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/engine/cli.py` & `dagger_io-0.5.4/src/dagger/engine/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/engine/conn.py` & `dagger_io-0.5.4/src/dagger/engine/conn.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/engine/download.py` & `dagger_io-0.5.4/src/dagger/engine/download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/exceptions.py` & `dagger_io-0.5.4/src/dagger/exceptions.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/log.py` & `dagger_io-0.5.4/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/server/__init__.py` & `dagger_io-0.5.4/src/dagger/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/server/cli.py` & `dagger_io-0.5.4/src/dagger/server/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/server/converter.py` & `dagger_io-0.5.4/src/dagger/server/converter.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/session.py` & `dagger_io-0.5.4/src/dagger/session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/src/dagger/transport/httpx.py` & `dagger_io-0.5.4/src/dagger/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.3/setup.py` & `dagger_io-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'typing_extensions>=4.4.0']
 
 extras_require = \
 {'server': ['strawberry-graphql>=0.133.5']}
 
 setup_kwargs = {
     'name': 'dagger-io',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'A client package for running Dagger pipelines in Python.',
     'long_description': '# Dagger Python SDK\n\n[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/) \n[![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)\n[![License](https://img.shields.io/pypi/l/dagger-io.svg)](https://pypi.python.org/pypi/dagger-io)\n[![Code style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n\nA client package for running [Dagger](https://dagger.io/) pipelines.\n\n## What is the Dagger Python SDK?\n\nThe Dagger Python SDK contains everything you need to develop CI/CD pipelines in Python, and run them on any OCI-compatible container runtime.\n\n## Requirements\n\n- Python 3.10 or later\n- [Docker](https://docs.docker.com/engine/install/), or another OCI-compatible container runtime\n\nA compatible version of the  [Dagger CLI](https://docs.dagger.io/cli) is automatically downloaded and run by the SDK for you, although it’s possible to manage it manually.\n\n## Installation\n\nFrom [PyPI](https://pypi.org/project/dagger-io/), using `pip`:\n\n```shell\npip install dagger-io\n```\n\nYou can also install via [Conda](https://anaconda.org/conda-forge/dagger-io), from the [conda-forge](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge) channel:\n\n```shell\nconda install dagger-io\n```\n\n## Example\n\nCreate a `main.py` file:\n\n```python\nimport sys\n\nimport anyio\nimport dagger\n\n\nasync def main(args: list[str]):\n    async with dagger.Connection() as client:\n        # build container with cowsay entrypoint\n        ctr = (\n            client.container()\n            .from_("python:alpine")\n            .with_exec(["pip", "install", "cowsay"])\n            .with_entrypoint(["cowsay"])\n        )\n\n        # run cowsay with requested message\n        result = await ctr.with_exec(args).stdout()\n\n    print(result)\n\n\nanyio.run(main, sys.argv[1:])\n```\n\nRun with:\n\n```console\n$ python main.py "Simple is better than complex"\n  _____________________________\n| Simple is better than complex |\n  =============================\n                             \\\n                              \\\n                                ^__^\n                                (oo)\\_______\n                                (__)\\       )\\/\\\n                                    ||----w |\n                                    ||     ||\n```\n\n> **Note**\n> It may take a while for it to finish, especially on first run with cold cache.\n\nIf you need to debug, you can stream the logs from the engine with the `log_output`  config:\n\n```python\nconfig = dagger.Config(log_output=sys.stderr)\nasync with dagger.Connection(config) as client:\n    ...\n```\n\n## Learn more\n\n- [Documentation](https://docs.dagger.io/sdk/python)\n- [API Reference](https://dagger-io.readthedocs.org)\n- [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)\n\n## Development\n\nThis library is maintained with [Poetry](https://python-poetry.org/docs/).\n\nIf you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:\n\n```shell\npoetry install\n```\n\nThe following commands are available:\n- `poe test`: Run tests.\n- `poe fmt`: Re-format code following common styling conventions.\n- `poe lint`: Check for linting violations.\n- `poe generate`: Regenerate API client after changes to the codegen.\n- `poe docs`: Build reference docs locally.\n\n### Engine changes\n\nTesting and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet. \n\nThe simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :\n\n```shell\n../../hack/make sdk:python:test\n../../hack/make sdk:python:generate\n```\n\nYou can also build the CLI and use it directly within the Python SDK:\n\n```shell\n../../hack/dev poe test\n```\n\nOr build it separately and tell the SDK to use it directly (or any other CLI binary):\n\n```shell\n../../hack/make\n_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test\n```\n\n',
     'author': 'Dagger',
     'author_email': 'hello@dagger.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dagger.io',
```

### Comparing `dagger_io-0.5.3/PKG-INFO` & `dagger_io-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.5.3
+Version: 0.5.4
 Summary: A client package for running Dagger pipelines in Python.
 Home-page: https://dagger.io
 License: Apache-2.0
 Author: Dagger
 Author-email: hello@dagger.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

