# Comparing `tmp/upstash_py-0.3.0.tar.gz` & `tmp/upstash_py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_py-0.3.0.tar", max compression
+gzip compressed data, was "upstash_py-0.4.0.tar", max compression
```

## Comparing `upstash_py-0.3.0.tar` & `upstash_py-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       37 2023-03-04 10:43:41.243570 upstash_py-0.3.0/README.md
--rw-r--r--   0        0        0      379 2023-05-13 16:15:09.549732 upstash_py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_py-0.3.0/upstash_py/__init__.py
--rw-r--r--   0        0        0    83443 2023-05-13 15:26:15.134417 upstash_py-0.3.0/upstash_py/client.py
--rw-r--r--   0        0        0      308 2023-05-13 15:46:08.357723 upstash_py-0.3.0/upstash_py/config.py
--rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_py-0.3.0/upstash_py/exception.py
--rw-r--r--   0        0        0      755 2023-05-04 15:53:00.952164 upstash_py-0.3.0/upstash_py/http/decode.py
--rw-r--r--   0        0        0     1887 2023-05-13 15:33:46.517564 upstash_py-0.3.0/upstash_py/http/execute.py
--rw-r--r--   0        0        0     1030 2023-05-04 15:39:39.039487 upstash_py-0.3.0/upstash_py/play.py
--rw-r--r--   0        0        0       75 2023-05-13 15:44:19.293211 upstash_py-0.3.0/upstash_py/play2.py
--rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_py-0.3.0/upstash_py/schema/commands/parameters.py
--rw-r--r--   0        0        0     1119 2023-05-13 16:00:21.639249 upstash_py-0.3.0/upstash_py/schema/commands/returns.py
--rw-r--r--   0        0        0      761 2023-04-13 15:35:06.241703 upstash_py-0.3.0/upstash_py/schema/http.py
--rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_py-0.3.0/upstash_py/utils/base.py
--rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_py-0.3.0/upstash_py/utils/comparison.py
--rw-r--r--   0        0        0     3333 2023-05-04 07:39:00.163434 upstash_py-0.3.0/upstash_py/utils/exception.py
--rw-r--r--   0        0        0     4088 2023-05-04 15:26:27.420397 upstash_py-0.3.0/upstash_py/utils/format.py
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 upstash_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-03-04 10:43:41.243570 upstash_py-0.4.0/README.md
+-rw-r--r--   0        0        0      379 2023-05-18 16:55:54.788352 upstash_py-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_py-0.4.0/upstash_py/__init__.py
+-rw-r--r--   0        0        0    87469 2023-05-16 16:11:10.452567 upstash_py-0.4.0/upstash_py/client.py
+-rw-r--r--   0        0        0      308 2023-05-16 14:24:46.481207 upstash_py-0.4.0/upstash_py/config.py
+-rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_py-0.4.0/upstash_py/exception.py
+-rw-r--r--   0        0        0      755 2023-05-04 15:53:00.952164 upstash_py-0.4.0/upstash_py/http/decode.py
+-rw-r--r--   0        0        0     2445 2023-05-16 14:52:47.823004 upstash_py-0.4.0/upstash_py/http/execute.py
+-rw-r--r--   0        0        0     1030 2023-05-04 15:39:39.039487 upstash_py-0.4.0/upstash_py/play.py
+-rw-r--r--   0        0        0       65 2023-05-16 14:51:29.801586 upstash_py-0.4.0/upstash_py/play2.py
+-rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_py-0.4.0/upstash_py/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1119 2023-05-13 16:00:21.639249 upstash_py-0.4.0/upstash_py/schema/commands/returns.py
+-rw-r--r--   0        0        0      761 2023-04-13 15:35:06.241703 upstash_py-0.4.0/upstash_py/schema/http.py
+-rw-r--r--   0        0        0      188 2023-05-15 17:17:17.515782 upstash_py-0.4.0/upstash_py/schema/telemetry.py
+-rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_py-0.4.0/upstash_py/utils/base.py
+-rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_py-0.4.0/upstash_py/utils/comparison.py
+-rw-r--r--   0        0        0     3333 2023-05-04 07:39:00.163434 upstash_py-0.4.0/upstash_py/utils/exception.py
+-rw-r--r--   0        0        0     4088 2023-05-04 15:26:27.420397 upstash_py-0.4.0/upstash_py/utils/format.py
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 upstash_py-0.4.0/PKG-INFO
```

### Comparing `upstash_py-0.3.0/upstash_py/client.py` & `upstash_py-0.4.0/upstash_py/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from upstash_py.http.execute import execute
 from upstash_py.schema.http import RESTResult, RESTEncoding
+from upstash_py.schema.telemetry import TelemetryData
 from upstash_py.config import (
     REST_ENCODING,
     REST_RETRIES,
     REST_RETRY_INTERVAL,
     ALLOW_TELEMETRY,
     ALLOW_DEPRECATED,
     FORMAT_RETURN
@@ -45,51 +46,56 @@
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,
         allow_deprecated: bool = ALLOW_DEPRECATED,
         format_return: bool = FORMAT_RETURN,
-        allow_telemetry: bool = ALLOW_TELEMETRY
+        allow_telemetry: bool = ALLOW_TELEMETRY,
+        telemetry_data: TelemetryData | None = None
     ):
         self.url = url
         self.token = token
 
         self.allow_telemetry = allow_telemetry
 
         self.allow_deprecated = allow_deprecated
         self.format_return = format_return
 
         self.rest_encoding = rest_encoding
         self.rest_retries = rest_retries
         self.rest_retry_interval = rest_retry_interval
 
+        self.telemetry_data = telemetry_data
+
     @classmethod
     def from_env(
         cls,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,
         allow_deprecated: bool = ALLOW_DEPRECATED,
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
+        telemetry_data: TelemetryData | None = None
     ):
         """
         Load the credentials from environment.
         """
 
         return cls(
             environ["UPSTASH_REDIS_REST_URL"],
             environ["UPSTASH_REDIS_REST_TOKEN"],
             rest_encoding,
             rest_retries,
             rest_retry_interval,
             allow_deprecated,
             format_return,
-            allow_telemetry
+            allow_telemetry,
+            telemetry_data
         )
 
     async def __aenter__(self) -> ClientSession:
         """
         Enter the async context.
         """
 
@@ -113,15 +119,16 @@
             session=self._session,
             url=self.url,
             token=self.token,
             encoding=self.rest_encoding,
             retries=self.rest_retries,
             retry_interval=self.rest_retry_interval,
             command=command,
-            allow_telemetry=self.allow_telemetry
+            allow_telemetry=self.allow_telemetry,
+            telemetry_data=self.telemetry_data
         )
 
     async def bitcount(self, key: str, start: int | None = None, end: int | None = None) -> int:
         """
         See https://redis.io/commands/bitcount
         """
 
@@ -225,14 +232,16 @@
         command: list = ["ECHO", message]
 
         return await self.run(command)
 
     async def copy(self, source: str, destination: str, replace: bool = False) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/copy
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["COPY", source, destination]
 
         if replace:
             command.append("REPLACE")
 
@@ -263,25 +272,29 @@
         command: list = ["EXISTS", *keys]
 
         return await self.run(command)
 
     async def expire(self, key: str, seconds: int) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/expire
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["EXPIRE", key, seconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def expireat(self, key: str, unix_time_seconds: int) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/expireat
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["EXPIREAT", key, unix_time_seconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -294,36 +307,42 @@
         command: list = ["KEYS", pattern]
 
         return await self.run(command)
 
     async def persist(self, key: str) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/persist
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["PERSIST", key]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def pexpire(self, key: str, milliseconds: int) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/pexpire
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["PEXPIRE", key, milliseconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def pexpireat(self, key: str, unix_time_milliseconds: int) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/pexpireat
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["PEXPIREAT", key, unix_time_milliseconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -354,14 +373,16 @@
         command: list = ["RENAME", key, new_name]
 
         return await self.run(command)
 
     async def renamenx(self, key: str, new_name: str) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/renamenx
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["RENAMENX", key, new_name]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -380,28 +401,31 @@
         :param pattern: replacement for "MATCH"
 
         :param count: defaults to 10 on the server side
 
         :param scan_type: replacement for "TYPE"
 
         :param return_cursor: if set to False, it won't return the cursor
+
+        :return: The cursor will be an integer if "format_return" is True.
+        Only the list of elements will be returned if "return_cursor" is False
         """
 
         command: list = ["SCAN", cursor]
 
         if pattern is not None:
             command.extend(["MATCH", pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
         if scan_type is not None:
             command.extend(["TYPE", scan_type])
 
-        # The raw result is composed of the new cursor and the array of elements.
+        # The raw result is composed of the new cursor and the list of elements.
         raw: list[str | list[str]] = await self.run(command)
 
         if return_cursor:
             return [int(raw[0]), raw[1]] if self.format_return else raw
 
         return raw[1]
 
@@ -488,14 +512,16 @@
         key: str,
         first_member: str,
         second_member: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"] = "M"
     ) -> str | float | None:
         """
         See https://redis.io/commands/geodist
+
+        :return: A float value if "format_return" is True.
         """
 
         command: list = ["GEODIST", key, first_member, second_member, unit]
 
         raw: str | None = await self.run(command)
 
         return float(raw) if self.format_return else raw
@@ -512,14 +538,16 @@
     async def geopos(
         self,
         key: str,
         *members: str
     ) -> list[list[str] | None] | list[dict[str, float] | None]:
         """
         See https://redis.io/commands/geopos
+
+        :return: A list of dicts with either None or the longitude and latitude if "format_return" is True.
         """
 
         command: list = ["GEOPOS", key, *members]
 
         raw: list[list[str] | None] = await self.run(command)
 
         return format_geo_positions_return(raw) if self.format_return else raw
@@ -543,14 +571,16 @@
         """
         See https://redis.io/commands/georadius
 
         :param count_any: replacement for "ANY"
 
         :param store_as: replacement for "STORE"
         :param store_distance_as: replacement for "STORE_DIST"
+
+        :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
         if not self.allow_deprecated:
             raise Exception("""From version 6.2.0, this command is deprecated.
 It can be replaced by "geosearch" and "geosearchstore" with the "radius" argument.
 Source: https://redis.io/commands/georadius""")
 
@@ -611,14 +641,16 @@
         count_any: bool = False,
         sort: Literal["ASC", "DESC"] | None = None
     ) -> GeoMembersReturn | FormattedGeoMembersReturn:
         """
         See https://redis.io/commands/georadius_ro
 
         :param count_any: replacement for "ANY"
+
+        :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
         if not self.allow_deprecated:
             raise Exception("""From version 6.2.0, this command is deprecated.
 It can be replaced by "geosearch" with the "radius" argument.
 Source: https://redis.io/commands/georadius_ro""")
 
@@ -670,14 +702,16 @@
         """
         See https://redis.io/commands/georadiusbymember
 
         :param count_any: replacement for "ANY"
 
         :param store_as: replacement for "STORE"
         :param store_distance_as: replacement for "STORE_DIST"
+
+        :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
         if not self.allow_deprecated:
             raise Exception("""From version 6.2.0, this command is deprecated.
 It can be replaced by "geosearch" and "geosearchstore" with the "radius" and "member" arguments.
 Source: https://redis.io/commands/georadiusbymember""")
 
@@ -737,14 +771,16 @@
         count_any: bool = False,
         sort: Literal["ASC", "DESC"] | None = None
     ) -> GeoMembersReturn | FormattedGeoMembersReturn:
         """
         See https://redis.io/commands/georadiusbymember
 
         :param count_any: replacement for "ANY"
+
+        :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
         if not self.allow_deprecated:
             raise Exception("""From version 6.2.0, this command is deprecated.
         It can be replaced by "geosearch" with the "radius" and "member" arguments.
         Source: https://redis.io/commands/georadiusbymember""")
 
@@ -805,14 +841,16 @@
 
         :param radius: replacement for "BYRADIUS"
 
         :param width: replacement for "BYBOX" together with "height"
         :param height: replacement for "BYBOX" together with "width"
 
         :param count_any: replacement for "ANY"
+
+        :return: A list of dicts with the requested properties if "format_return" is True.
         """
 
         handle_geosearch_exceptions(member, longitude, latitude, radius, width, height, count, count_any)
 
         command: list = ["GEOSEARCH", key]
 
         if member is not None:
@@ -930,14 +968,16 @@
         command: list = ["HDEL", key, *fields]
 
         return await self.run(command)
 
     async def hexists(self, key: str, field: str) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/hexists
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["HEXISTS", key, field]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -950,14 +990,16 @@
         command: list = ["HGET", key, field]
 
         return await self.run(command)
 
     async def hgetall(self, key: str) -> HashReturn | FormattedHashReturn:
         """
         See https://redis.io/commands/hgetall
+
+        :return: A dict of field-value pairs if "format_return" is True.
         """
 
         command: list = ["HGETALL", key]
 
         raw: HashReturn = await self.run(command)
 
         return format_hash_return(raw) if self.format_return else raw
@@ -970,14 +1012,16 @@
         command: list = ["HINCRBY", key, field, increment]
 
         return await self.run(command)
 
     async def hincrbyfloat(self, key: str, field: str, increment: float) -> str | float:
         """
         See https://redis.io/commands/hincrbyfloat
+
+        :return: A float if "format_return" is True.
         """
 
         command: list = ["HINCRBYFLOAT", key, field, increment]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
@@ -1035,14 +1079,16 @@
         count: int | None = None,
         with_values: bool = False
     ) -> (str | None) | (HashReturn | FormattedHashReturn):
         """
         See https://redis.io/commands/hrandfield
 
         :param count: defaults to 1 on the server side
+
+        :return: A dict of field-value pairs if "count" and "with_values" are specified and "format_return" is True.
         """
 
         if count is None and with_values:
             raise Exception("\"with_values\" can only be used together with \"count\"")
 
         command: list = ["HRANDFIELD", key]
 
@@ -1070,25 +1116,28 @@
         See https://redis.io/commands/hscan
 
         :param pattern: replacement for "MATCH"
 
         :param count: defaults to 10 on the server side
 
         :param return_cursor: if set to False, it won't return the cursor
+
+        :return: The cursor will be an integer if "format_return" is True.
+        Only a dict of field-value pairs will be returned if "return_cursor" is False and "format_return" is True.
         """
 
         command: list = ["HSCAN", key, cursor]
 
         if pattern is not None:
             command.extend(["MATCH", pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        # The raw result is composed of the new cursor and the array of elements.
+        # The raw result is composed of the new cursor and the list of elements.
         raw: list[str | HashReturn] | HashReturn = await self.run(command)
 
         if return_cursor:
             return [int(raw[0]), format_hash_return(raw[1])] if self.format_return else raw
 
         return format_hash_return(raw[1]) if self.format_return else raw[1]
 
@@ -1103,14 +1152,16 @@
             command.extend([field, value])
 
         return await self.run(command)
 
     async def hsetnx(self, key: str, field: str, value: Any) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/hsetnx
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["HSETNX", key, field, value]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -1132,14 +1183,16 @@
         command: list = ["HVALS", key]
 
         return await self.run(command)
 
     async def pfadd(self, key: str, *elements: Any) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/pfadd
+
+        :return: A bool if "format_return" is True.
         """
 
         command: list = ["PFADD", key, *elements]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -1470,14 +1523,16 @@
             command.append(mode)
 
         return await self.run(command)
 
     async def server_time(self) -> list[str] | dict[str, int]:
         """
         See https://redis.io/commands/time
+
+        :return: A dict with the keys "seconds" and "microseconds" if self.format_return is True.
         """
 
         command: list = ["TIME"]
 
         raw: list[str] = await self.run(command)
 
         return format_server_time_return(raw) if self.format_return else raw
@@ -1550,14 +1605,16 @@
         command: list = ["SINTERSTORE", destination_key, *keys]
 
         return await self.run(command)
 
     async def sismember(self, key: str, member: Any) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/sismember
+
+        :return: A bool if self.format_return is True.
         """
 
         command: list = ["SISMEMBER", key, member]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -1570,14 +1627,16 @@
         command: list = ["SMEMBERS", key]
 
         return await self.run(command)
 
     async def smove(self, source_key: str, destination_key: str, member: Any) -> Literal[1, 0] | bool:
         """
         See https://redis.io/commands/smove
+
+        :return: A bool if self.format_return is True.
         """
 
         command: list = ["SMOVE", source_key, destination_key, member]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -1634,25 +1693,28 @@
         See https://redis.io/commands/sscan
 
         :param pattern: replacement for "MATCH"
 
         :param count: defaults to 10 on the server side
 
         :param return_cursor: if set to False, it won't return the cursor
+
+        :return: The cursor will be an integer if "format_return" is True.
+        Only the list of elements will be returned if "return_cursor" is False.
         """
 
         command: list = ["SSCAN", key, cursor]
 
         if pattern is not None:
             command.extend(["MATCH", pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        # The raw result is composed of the new cursor and the array of elements.
+        # The raw result is composed of the new cursor and the list of elements.
         raw: list[str | list[str]] = await self.run(command)
 
         if return_cursor:
             return [int(raw[0]), raw[1]] if self.format_return else raw
 
         return raw[1]
 
@@ -1691,14 +1753,17 @@
         ch: bool = False,
         incr: bool = False
     ) -> int | (str | None | float):
         """
         See https://redis.io/commands/zadd
 
         :param sorted_set_members: a dict containing their names and scores.
+
+        :return: A float representing the number of elements added or None if "incr" is False
+        and "format_return" is True.
         """
 
         if nx and xx:
             raise Exception("\"nx\" and \"xx\" are mutually exclusive.")
 
         if gt and lt:
             raise Exception("\"gt\" and \"lt\" are mutually exclusive.")
@@ -1763,14 +1828,16 @@
     whether "with_scores" is True or not, its raw return type will be list[str].
     """
     async def zdiff(self, *keys: str, with_scores: bool = False) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zdiff
 
         The number of keys is calculated automatically.
+
+        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: list = ["ZDIFF", len(keys), *keys]
 
@@ -1796,14 +1863,16 @@
         command: list = ["ZDIFFSTORE", destination_key, len(keys), *keys]
 
         return await self.run(command)
 
     async def zincrby(self, key: str, increment: float, member: str) -> str | float:
         """
         See https://redis.io/commands/zincrby
+
+        :return: A float if "format_return" is True.
         """
 
         command: list = ["ZINCRBY", key, increment, member]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
@@ -1821,14 +1890,16 @@
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zinter
 
         The number of keys is calculated automatically.
 
         :param multiplication_factors: replacement for "WEIGHTS"
+
+        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: list = ["ZINTER", len(keys), *keys]
 
@@ -1888,14 +1959,16 @@
         command: list = ["ZLEXCOUNT", key, min_score, max_score]
 
         return await self.run(command)
 
     async def zmscore(self, key: str, *members: str) -> list[str | None] | list[float | None]:
         """
         See https://redis.io/commands/zmscore
+
+        :return: A list of float or None values if "format_return" is True.
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be specified.")
 
         command: list = ["ZMSCORE", key, *members]
 
@@ -1904,14 +1977,16 @@
         return format_float_list(raw) if self.format_return else raw
 
     async def zpopmax(self, key: str, count: int | None = None) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zpopmax
 
         :param count: defaults to 1 on the server side
+
+        :return: A dict of member-score pairs if "format_return" is True.
         """
 
         command: list = ["ZPOPMAX", key]
 
         if count is not None:
             command.append(count)
 
@@ -1920,14 +1995,16 @@
         return format_sorted_set_return(raw) if self.format_return else raw
 
     async def zpopmin(self, key: str, count: int | None = None) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zpopmin
 
         :param count: defaults to 1 on the server side
+
+        :return: A dict of member-score pairs if "format_return" is True.
         """
 
         command: list = ["ZPOPMIN", key]
 
         if count is not None:
             command.append(count)
 
@@ -1941,14 +2018,16 @@
         count: int | None = None,
         with_scores: bool = False
     ) -> (str | None) | (SortedSetReturn | FormattedSortedSetReturn):
         """
         See https://redis.io/commands/zrandmember
 
         :param count: defaults to 1 on the server side
+
+        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if count is None and with_scores:
             raise Exception("\"with_scores\" can only be used with \"count\".")
 
         command: list = ["ZRANDMEMBER", key]
 
@@ -1979,14 +2058,16 @@
         count: int | None = None,
         with_scores: bool = False
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zrange
 
         If you need to use "-inf" and "+inf", please write them as strings.
+
+        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         handle_non_deprecated_zrange_exceptions(range_method, start, stop, offset, count)
 
         command: list = ["ZRANGE", key, start, stop]
 
         if range_method:
@@ -2047,14 +2128,16 @@
         offset: int | None = None,
         count: int | None = None
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
+
+        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if not self.allow_deprecated:
             raise Exception(
                 """From 6.2.0, this command is deprecated.
 It can be replaced by "zrange" with "range_method" set to "BYSCORE".
 Source: https://redis.io/commands/zrangebyscore""")
@@ -2175,14 +2258,16 @@
         key: str,
         start: int,
         stop: int,
         with_scores: bool = False
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zrevrange
+
+        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if not self.allow_deprecated:
             raise Exception("""From 6.2.0, this command is deprecated.
 It can be replaced by "zrange" with "rev" set to True.
 Source: https://redis.io/commands/zrevrange""")
 
@@ -2236,14 +2321,16 @@
         offset: int | None = None,
         count: int | None = None
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zrevrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
+
+        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if not self.allow_deprecated:
             raise Exception("""From 6.2.0, this command is deprecated.
 It can be replaced by "zrange" with "rev" set to True and "range_method" set to "BYSCORE".
 Source: https://redis.io/commands/zrevrangebyscore""")
 
@@ -2289,14 +2376,17 @@
         See https://redis.io/commands/zscan
 
         :param pattern: replacement for "MATCH"
 
         :param count: defaults to 10 on the server side
 
         :param return_cursor: if set to False, it won't return the cursor
+
+        :return: The cursor will be an integer if "format_return" is True.
+        Only a dict of member-score pairs will be returned if "return_cursor" is False and "format_return" is True.
         """
 
         command: list = ["ZSCAN", key, cursor]
 
         if pattern is not None:
             command.extend(["MATCH", pattern])
 
@@ -2304,20 +2394,22 @@
             command.extend(["COUNT", count])
 
         raw: list[int | SortedSetReturn] = await self.run(command)
 
         if return_cursor:
             return [int(raw[0]), format_sorted_set_return(raw[1])] if self.format_return else raw
 
-        # The raw result is composed of the new cursor and the array of elements.
+        # The raw result is composed of the new cursor and the list of elements.
         return format_sorted_set_return(raw[1]) if self.format_return else raw[1]
 
     async def zscore(self, key: str, member: str) -> str | None | float:
         """
         See https://redis.io/commands/zscore
+
+        :return: A float or None if "format_return" is True.
         """
 
         command: list = ["ZSCORE", key, member]
 
         raw: str | None = await self.run(command)
 
         return float(raw) if self.format_return and raw is not None else raw
@@ -2335,14 +2427,16 @@
     ) -> SortedSetReturn | FormattedSortedSetReturn:
         """
         See https://redis.io/commands/zunion
 
         The number of keys is calculated automatically.
 
         :param multiplication_factors: replacement for "WEIGHTS"
+
+        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
         command: list = ["ZUNION", len(keys), *keys]
 
@@ -2509,14 +2603,16 @@
         command: list = ["INCRBY", key, increment]
 
         return await self.run(command)
 
     async def incrbyfloat(self, key: str, increment: float) -> str | float:
         """
         See https://redis.io/commands/incrbyfloat
+
+        :return: A float if "format_return" is True.
         """
 
         command: list = ["INCRBYFLOAT", key, increment]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
@@ -2802,14 +2898,16 @@
         self.command.append("NUMPAT")
 
         return await self.client.run(command=self.command)
 
     async def numsub(self, *channels: str) -> list[str | int] | dict[str, int]:
         """
         See https://redis.io/commands/pubsub-numsub
+
+        :return: A dict with channel-(number-of-subscribers) pairs if "format_return" is True.
         """
 
         self.command.extend(["NUMSUB", *channels])
 
         raw: list[str | int] = await self.client.run(command=self.command)
 
         return format_pubsub_numsub_return(raw) if self.client.format_return else raw
@@ -2819,14 +2917,16 @@
     def __init__(self, client: Redis):
         self.client = client
         self.command: list = ["SCRIPT"]
 
     async def exists(self, *sha1_digests: str) -> list[Literal[1, 0]] | list[bool]:
         """
         See https://redis.io/commands/script-exists
+
+        :return: A list of bools if "format_return" is True.
         """
 
         if len(sha1_digests) == 0:
             raise Exception("At least one sha1 digest must be provided.")
 
         self.command.extend(["EXISTS", *sha1_digests])
```

### Comparing `upstash_py-0.3.0/upstash_py/http/decode.py` & `upstash_py-0.4.0/upstash_py/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.3.0/upstash_py/http/execute.py` & `upstash_py-0.4.0/upstash_py/http/execute.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from upstash_py.exception import UpstashException
 from upstash_py.http.decode import decode
 from upstash_py.schema.http import RESTResult, RESTResponse, RESTEncoding
+from upstash_py.schema.telemetry import TelemetryData
 from asyncio import sleep
 from aiohttp import ClientSession
 from json import dumps
 from platform import python_version
 
 
 async def execute(
     session: ClientSession,
     url: str,
     token: str,
     encoding: RESTEncoding,
     retries: int,
     retry_interval: int,
     command: list,
-    allow_telemetry: bool
+    allow_telemetry: bool,
+    telemetry_data: TelemetryData | None = None
 ) -> RESTResult:
     """
     Execute the given command over the REST API.
     """
 
     # Serialize the command; more specifically, write string-incompatible types as JSON strings.
     command = [
@@ -31,22 +33,31 @@
     ]
 
     for i in range(retries + 1):
         try:
             headers: dict[str, str] = {"Authorization": f'Bearer {token}'}
 
             if allow_telemetry:
-                headers["Upstash-Telemetry-Runtime"] = f'python@v.{python_version()}'
-                headers["Upstash-Telemetry-Sdk"] = "upstash_py@development"
+                if telemetry_data:
+                    headers["Upstash-Telemetry-Runtime"] = telemetry_data["runtime"]
+                    headers["Upstash-Telemetry-Sdk"] = telemetry_data["sdk"]
+
+                    # Avoid the [] syntax to prevent KeyError from being raised.
+                    if telemetry_data.get("platform"):
+                        headers["Upstash-Telemetry-Platform"] = telemetry_data["platform"]
+                else:
+                    headers["Upstash-Telemetry-Runtime"] = f'python@v{python_version()}'
+                    headers["Upstash-Telemetry-Sdk"] = "upstash-py@development"
 
             if encoding:
                 headers["Upstash-Encoding"] = encoding
 
             async with session.post(url, headers=headers, json=command) as response:
                 body: RESTResponse[RESTResult] = await response.json()
+
                 # Avoid the [] syntax to prevent KeyError from being raised.
                 if body.get("error"):
                     raise UpstashException(body.get("error"))
 
                 return decode(raw=body["result"], encoding=encoding) if encoding else body["result"]
             break
         except Exception as exception:
```

### Comparing `upstash_py-0.3.0/upstash_py/play.py` & `upstash_py-0.4.0/upstash_py/play.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.3.0/upstash_py/schema/commands/returns.py` & `upstash_py-0.4.0/upstash_py/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.3.0/upstash_py/schema/http.py` & `upstash_py-0.4.0/upstash_py/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.3.0/upstash_py/utils/exception.py` & `upstash_py-0.4.0/upstash_py/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.3.0/upstash_py/utils/format.py` & `upstash_py-0.4.0/upstash_py/utils/format.py`

 * *Files identical despite different names*

