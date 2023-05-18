# Comparing `tmp/moat-modbus-0.5.3.tar.gz` & `tmp/moat-modbus-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moat-modbus-0.5.3.tar", last modified: Tue Jan  3 13:20:48 2023, max compression
+gzip compressed data, was "moat-modbus-0.6.2.tar", last modified: Thu May 18 12:46:00 2023, max compression
```

## Comparing `moat-modbus-0.5.3.tar` & `moat-modbus-0.6.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/
--rw-r--r--   0 smurf      (501) smurf      (501)      436 2023-01-03 13:20:44.000000 moat-modbus-0.5.3/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)      114 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/.gitmodules
--rw-r--r--   0 smurf      (501) smurf      (501)      242 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)     1923 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)     1319 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/README.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/moat/
--rw-r--r--   0 smurf      (501) smurf      (501)       65 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/moat/modbus/
--rw-r--r--   0 smurf      (501) smurf      (501)      690 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     8373 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/__main__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      351 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/_main.py
--rw-r--r--   0 smurf      (501) smurf      (501)    29419 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/client.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/moat/modbus/dev/
--rw-r--r--   0 smurf      (501) smurf      (501)      109 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/dev/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2496 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/dev/_main.py
--rw-r--r--   0 smurf      (501) smurf      (501)    12121 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/dev/device.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2541 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/dev/distkv.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3996 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/dev/poll.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3817 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/dev/server.py
--rw-r--r--   0 smurf      (501) smurf      (501)    12561 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/server.py
--rw-r--r--   0 smurf      (501) smurf      (501)     3084 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/typemap.py
--rw-r--r--   0 smurf      (501) smurf      (501)    16290 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/moat/modbus/types.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/moat_modbus.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)     1923 2023-01-03 13:20:48.000000 moat-modbus-0.5.3/moat_modbus.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)      715 2023-01-03 13:20:48.000000 moat-modbus-0.5.3/moat_modbus.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-01-03 13:20:48.000000 moat-modbus-0.5.3/moat_modbus.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       69 2023-01-03 13:20:48.000000 moat-modbus-0.5.3/moat_modbus.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        5 2023-01-03 13:20:48.000000 moat-modbus-0.5.3/moat_modbus.egg-info/top_level.txt
--rw-r--r--   0 smurf      (501) smurf      (501)     2032 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/pyproject.toml
--rw-r--r--   0 smurf      (501) smurf      (501)       38 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/setup.cfg
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/systemd/
--rw-r--r--   0 smurf      (501) smurf      (501)      339 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/systemd/moat-modbus-poll@.service
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:20:48.290473 moat-modbus-0.5.3/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)      261 2022-09-16 15:26:41.000000 moat-modbus-0.5.3/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)      141 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/tests/conftest.py
--rw-r--r--   0 smurf      (501) smurf      (501)     4218 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/tests/full.yaml
--rw-r--r--   0 smurf      (501) smurf      (501)     2518 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/tests/kwb.yaml
--rw-r--r--   0 smurf      (501) smurf      (501)     1015 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/tests/sdm.yaml
--rw-r--r--   0 smurf      (501) smurf      (501)      139 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/tests/test_basic.py
--rw-r--r--   0 smurf      (501) smurf      (501)     1526 2023-01-03 13:08:05.000000 moat-modbus-0.5.3/tests/test_misc.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:00.141813 moat-modbus-0.6.2/
+-rw-r--r--   0 smurf      (501) smurf      (501)      436 2023-05-18 12:45:55.000000 moat-modbus-0.6.2/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      114 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/.gitmodules
+-rw-r--r--   0 smurf      (501) smurf      (501)      272 2023-05-18 12:45:30.000000 moat-modbus-0.6.2/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)     1940 2023-05-18 12:46:00.141813 moat-modbus-0.6.2/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)     1336 2023-05-18 12:45:30.000000 moat-modbus-0.6.2/README.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:00.137813 moat-modbus-0.6.2/moat/
+-rw-r--r--   0 smurf      (501) smurf      (501)      105 2023-05-18 12:45:30.000000 moat-modbus-0.6.2/moat/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:00.137813 moat-modbus-0.6.2/moat/modbus/
+-rw-r--r--   0 smurf      (501) smurf      (501)      690 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     8517 2023-05-18 12:45:30.000000 moat-modbus-0.6.2/moat/modbus/__main__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2475 2023-05-18 12:45:30.000000 moat-modbus-0.6.2/moat/modbus/_main.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    29849 2023-05-18 12:45:30.000000 moat-modbus-0.6.2/moat/modbus/client.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:00.141813 moat-modbus-0.6.2/moat/modbus/dev/
+-rw-r--r--   0 smurf      (501) smurf      (501)      109 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/dev/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2496 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/dev/_main.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    12121 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/dev/device.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2625 2023-05-18 12:45:30.000000 moat-modbus-0.6.2/moat/modbus/dev/distkv.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3996 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/dev/poll.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3817 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/dev/server.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    12561 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/server.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     3084 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/typemap.py
+-rw-r--r--   0 smurf      (501) smurf      (501)    16290 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/moat/modbus/types.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:00.141813 moat-modbus-0.6.2/moat_modbus.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1940 2023-05-18 12:45:59.000000 moat-modbus-0.6.2/moat_modbus.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)      715 2023-05-18 12:46:00.000000 moat-modbus-0.6.2/moat_modbus.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-05-18 12:45:59.000000 moat-modbus-0.6.2/moat_modbus.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       69 2023-05-18 12:45:59.000000 moat-modbus-0.6.2/moat_modbus.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        5 2023-05-18 12:45:59.000000 moat-modbus-0.6.2/moat_modbus.egg-info/top_level.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)     2050 2023-05-18 12:45:30.000000 moat-modbus-0.6.2/pyproject.toml
+-rw-r--r--   0 smurf      (501) smurf      (501)       38 2023-05-18 12:46:00.141813 moat-modbus-0.6.2/setup.cfg
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:00.141813 moat-modbus-0.6.2/systemd/
+-rw-r--r--   0 smurf      (501) smurf      (501)      339 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/systemd/moat-modbus-poll@.service
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:00.141813 moat-modbus-0.6.2/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)      261 2022-09-16 15:26:41.000000 moat-modbus-0.6.2/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      141 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/tests/conftest.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     4218 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/tests/full.yaml
+-rw-r--r--   0 smurf      (501) smurf      (501)     2518 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/tests/kwb.yaml
+-rw-r--r--   0 smurf      (501) smurf      (501)     1015 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/tests/sdm.yaml
+-rw-r--r--   0 smurf      (501) smurf      (501)      139 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/tests/test_basic.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     1526 2023-01-03 13:08:05.000000 moat-modbus-0.6.2/tests/test_misc.py
```

### Comparing `moat-modbus-0.5.3/PKG-INFO` & `moat-modbus-0.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-modbus
-Version: 0.5.3
+Version: 0.6.2
 Summary: Modular async modbus client and server
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 Project-URL: homepage, https://m-o-a-t.org
 Project-URL: repository, https://github.com/M-o-a-T/moat-modbus
 Keywords: MoaT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -65,11 +65,11 @@
 
 The values can be modified (factor+offset); the gateway works in both
 directions (command/state).
 
 TODO
 ++++
 
-* plain MQTT
 * configurable codecs
 * get/set attributes
 * pack multiple values into a message
+* read-after-write if no slot
```

### Comparing `moat-modbus-0.5.3/README.rst` & `moat-modbus-0.6.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -47,11 +47,11 @@
 
 The values can be modified (factor+offset); the gateway works in both
 directions (command/state).
 
 TODO
 ++++
 
-* plain MQTT
 * configurable codecs
 * get/set attributes
 * pack multiple values into a message
+* read-after-write if no slot
```

### Comparing `moat-modbus-0.5.3/moat/modbus/__init__.py` & `moat-modbus-0.6.2/moat/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/moat/modbus/__main__.py` & `moat-modbus-0.6.2/moat/modbus/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 async def _server(host, port, debug, args):
     """
     Basic Modbus server, for static tests.
     """
     if debug:
         log.setLevel(logging.DEBUG)
     if not args:
-        click.UsageError("You didn't add any values to serve")
+        raise click.UsageError("You didn't add any values to serve")
 
     from moat.modbus.server import ModbusServer  # pylint: disable=import-outside-toplevel
 
     s = ModbusServer(address=host, port=port)
     unit = None
     kind = InputRegisters
     typ = IntValue
@@ -147,15 +147,14 @@
         log.setLevel(logging.DEBUG)
 
     from moat.modbus.client import ModbusClient  # pylint: disable=import-outside-toplevel
 
     async with ModbusClient() as g, g.host(host, port) as h, h.unit(unit) as u, u.slot(
         "default"
     ) as s:
-
         k = map_kind[kind[0]]
         t = get_type(type_)
         if values:
             if len(values) == 1:
                 values = values * num
             elif len(values) != num:
                 raise click.UsageError("One or N values!")
@@ -213,15 +212,14 @@
         log.setLevel(logging.DEBUG)
 
     from moat.modbus.client import ModbusClient  # pylint: disable=import-outside-toplevel
 
     async with ModbusClient() as g, g.serial(
         port=port, baudrate=baudrate, stopbits=stopbits, parity=parity
     ) as h, h.unit(unit) as u, u.slot("default") as s:
-
         k = map_kind[kind[0]]
         t = get_type(type_)
         if values:
             if len(values) == 1:
                 values = values * num
             elif len(values) != num:
                 raise click.UsageError("One or N values!")
@@ -238,14 +236,25 @@
             else:
                 res = await s._getValues()  # pylint:disable=protected-access  ## TODO
                 pprint(res)
         except Exception as exc:  # pylint: disable=broad-except
             log.exception("Problem: %r", exc)
 
 
+def add_serial_cfg(c):
+    """Helper for serial port configuration"""
+    c = click.option(
+        "--port", "-p", required=True, type=str, help="destination port (/dev/ttyXXX)"
+    )(c)
+    c = click.option("--baudrate", "-b", type=int, default=9600, help="Baud rate (9600)")(c)
+    c = click.option("--parity", "-P", type=str, default="N", help="Parity (NEO), default N")(c)
+    c = click.option("--stopbits", "-S", type=int, default=1, help="Stopbits (12), default 1")(c)
+    return c
+
+
 def mk_serial_client(m):
     """helper to create a sserial client"""
     c = _serclient
     c = click.argument("values", nargs=-1)(c)
     c = click.option("--debug", "-d", is_flag=True, help="Log debug messages")(c)
     c = click.option(
         "--type",
@@ -255,19 +264,16 @@
         help="value type: s1,s2,s4,u1,u2,u4,f2,f4,raw; Sx/Fx=swapped",
     )(c)
     c = click.option("--num", "-n", type=int, default=1, help="number of values")(c)
     c = click.option("--start", "-s", default=0, help="starting register")(c)
     c = click.option("--kind", "-k", default="i", help="query type: input, discrete, hold, coil")(
         c
     )
+    c = add_serial_cfg(c)
     c = click.option("--unit", "-u", type=int, default=1, help="unit to query")(c)
-    c = click.option("--port", "-p", type=str, help="destination port (/dev/ttyXXX)")(c)
-    c = click.option("--baudrate", "-b", type=int, default=9600, help="Baud rate (9600)")(c)
-    c = click.option("--parity", "-P", type=str, default="N", help="Parity (NEO), default N")(c)
-    c = click.option("--stopbits", "-S", type=int, default=1, help="Stopbits (12), default 1")(c)
     c = m.command("serial", context_settings=dict(show_default=True))(c)
     return c
 
 
 serialclient = mk_serial_client(main)
```

### Comparing `moat-modbus-0.5.3/moat/modbus/client.py` & `moat-modbus-0.6.2/moat/modbus/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,25 @@
         """Run a unit in an `AsyncScope`"""
         return await scope.service(f"MH_{id36(self)}:{unit}", self._unit, unit)
 
     def _nextTID(self):
         self._tid = (self._tid + 1) % 0xFFFF
         return self._tid
 
+    async def send(self, msg):
+        """
+        Send a packet.
+
+        This is a low-level function. If you are a client, you want to use
+        `execute` instead.
+        """
+        packet = self.framer.buildPacket(msg)
+        async with self._send_lock:
+            await self.stream.send(packet)
+
     async def execute(self, request):
         """
         Send a pymodbus request and wait for / return the reply.
         """
         # pylint: disable=logging-fstring-interpolation,protected-access
 
         request.transaction_id = self._nextTID()
@@ -165,17 +176,15 @@
         async with self.cap:
             request._response_value = ValueEvent()
 
             await self._connected.wait()
 
             try:
                 self._transactions[request.transaction_id] = request
-                packet = self.framer.buildPacket(request)
-                async with self._send_lock:
-                    await self.stream.send(packet)
+                await self.send(request)
                 with anyio.fail_after(self.timeout):
                     res = await request._response_value.get()
             except TimeoutError:
                 await self.stream.aclose()
                 raise
             else:
                 if res.isError():
@@ -369,21 +378,22 @@
             ...
     """
 
     _tg = None
 
     max_req_len = 50  # max number of registers to fetch w/ one request
 
-    def __init__(self, gate, /, port, timeout=10, cap=1, debug=False, **ser):
+    def __init__(self, gate, /, port, timeout=10, cap=1, debug=False, monitor=None, **ser):
         self.port = port
         self.ser = ser
         self.framer = ModbusRtuFramer(ClientDecoder(), self)
 
         log = logging.getLogger(f"modbus.{Path(port).name}")
         self._trace = log.info if debug else log.debug
+        self._monitor = monitor
 
         super().__init__(gate, timeout, cap)
 
     def __repr__(self):
         return f"<ModbusHost:{self.port}:{self.ser.get('baudrate',0)}>"
 
     @asynccontextmanager
@@ -427,14 +437,15 @@
                 _logger.exception("Re-Write")
 
         await _send_trans()
         self._connected.set()
         task_status.started()
         self._trace("recv START")
 
+        mon = self._monitor
         while True:
             try:
                 data = await self.stream.receive(4096)
                 # pylint: disable=logging-not-lazy
                 self._trace("recv: " + " ".join([hex(x) for x in data]))
 
                 # unit = self.framer.decode_data(data).get("uid", 0)
@@ -469,22 +480,26 @@
 
                 t, self._transactions = self._transactions, {}
                 for req in t.values():
                     req._response_value.set_error(exc)
                 raise
 
             else:
-                for reply in replies:
-                    tid = reply.transaction_id
-                    try:
-                        request = self._transactions.pop(tid)
-                    except KeyError:
-                        _logger.info("Unrequested message: %s", reply)
-                    else:
-                        request._response_value.set(reply)
+                if mon:
+                    for reply in replies:
+                        await mon(reply)
+                else:
+                    for reply in replies:
+                        tid = reply.transaction_id
+                        try:
+                            request = self._transactions.pop(tid)
+                        except KeyError:
+                            _logger.info("Unrequested message: %s", reply)
+                        else:
+                            request._response_value.set(reply)
 
     async def aclose(self):
         """Stop talking."""
         if self.gate is None:
             return
         self.gate._del_host(self)  # pylint: disable=protected-access
         self.gate = None
```

### Comparing `moat-modbus-0.5.3/moat/modbus/dev/_main.py` & `moat-modbus-0.6.2/moat/modbus/dev/_main.py`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/moat/modbus/dev/device.py` & `moat-modbus-0.6.2/moat/modbus/dev/device.py`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/moat/modbus/dev/distkv.py` & `moat-modbus-0.6.2/moat/modbus/dev/distkv.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,23 +50,25 @@
         """Copy a Modbus value to MQTT"""
         async for val in self:
             logger.debug("%s r %r", self.path, val)
             await dkv.msg_send(list(self.data.dest), val)
 
     async def send_dkv(self, dkv):
         """Copy a DistKV value to Modbus"""
-        async for val in dkv.monitor(self.data.src):
-            logger.debug("%s W %r", self.path, val.value)
-            await self._set(val.value)
+        async with dkv.watch(self.data.src) as mon:
+            async for val in mon:
+                logger.debug("%s W %r", self.path, val.value)
+                await self._set(val.value)
 
     async def send_dkv_raw(self, dkv):
         """Copy an MQTT value to Modbus"""
-        async for val in dkv.msg_monitor(self.data.src):
-            logger.debug("%s w %r", self.path, val.value)
-            await self._set(val.value)
+        async with dkv.msg_monitor(self.data.src) as mon:
+            async for val in mon:
+                logger.debug("%s w %r", self.path, val.value)
+                await self._set(val.value)
 
     async def _set(self, value):
         self.value = value
 
         if self.data.get("dest") and self.data.get("mirror", False):
             if self.data.dest.mark == "r":
                 await self.dkv.msg_send(list(self.data.dest), self.value)
```

### Comparing `moat-modbus-0.5.3/moat/modbus/dev/poll.py` & `moat-modbus-0.6.2/moat/modbus/dev/poll.py`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/moat/modbus/dev/server.py` & `moat-modbus-0.6.2/moat/modbus/dev/server.py`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/moat/modbus/server.py` & `moat-modbus-0.6.2/moat/modbus/server.py`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/moat/modbus/typemap.py` & `moat-modbus-0.6.2/moat/modbus/typemap.py`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/moat/modbus/types.py` & `moat-modbus-0.6.2/moat/modbus/types.py`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/moat_modbus.egg-info/PKG-INFO` & `moat-modbus-0.6.2/moat_modbus.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-modbus
-Version: 0.5.3
+Version: 0.6.2
 Summary: Modular async modbus client and server
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 Project-URL: homepage, https://m-o-a-t.org
 Project-URL: repository, https://github.com/M-o-a-T/moat-modbus
 Keywords: MoaT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -65,11 +65,11 @@
 
 The values can be modified (factor+offset); the gateway works in both
 directions (command/state).
 
 TODO
 ++++
 
-* plain MQTT
 * configurable codecs
 * get/set attributes
 * pack multiple values into a message
+* read-after-write if no slot
```

### Comparing `moat-modbus-0.5.3/moat_modbus.egg-info/SOURCES.txt` & `moat-modbus-0.6.2/moat_modbus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/pyproject.toml` & `moat-modbus-0.6.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	"License :: OSI Approved",
 	"Development Status :: 4 - Beta",
 	]
 dependencies = [
 	"anyio ~= 3.0",
 	"pymodbus",
 	"anyio-serial",
-	"moat-util ~= 0.26.5",
+	"moat-util ~= 0.35.0",
 	"asyncscope ~= 0.8.3",
 	]
 dynamic = [ "version",]
 keywords = [ "MoaT",]
 requires-python = ">=3.8"
 name = "moat-modbus"
 description = "Modular async modbus client and server"
@@ -42,15 +42,15 @@
 
 [tool.isort]
 line_length = 99
 multi_line_output = 3
 profile = "black"
 
 [tool.setuptools]
-packages = [ "moat.modbus",]
+packages = [ "moat.modbus","moat.modbus.dev" ]
 [tool.setuptools.package-data]
 "*" = ["*.yaml"]
 
 [tool.setuptools_scm]
 
 [tool.black]
 line-length = 99
```

### Comparing `moat-modbus-0.5.3/tests/full.yaml` & `moat-modbus-0.6.2/tests/full.yaml`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/tests/kwb.yaml` & `moat-modbus-0.6.2/tests/kwb.yaml`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/tests/sdm.yaml` & `moat-modbus-0.6.2/tests/sdm.yaml`

 * *Files identical despite different names*

### Comparing `moat-modbus-0.5.3/tests/test_misc.py` & `moat-modbus-0.6.2/tests/test_misc.py`

 * *Files identical despite different names*

