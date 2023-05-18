# Comparing `tmp/pypck-0.7.8.tar.gz` & `tmp/pypck-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypck-0.7.8.tar", last modified: Tue Jan  5 06:33:00 2021, max compression
+gzip compressed data, was "dist/pypck-0.7.9.tar", last modified: Sun Jan 17 14:08:49 2021, max compression
```

## Comparing `pypck-0.7.8.tar` & `pypck-0.7.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-05 06:33:00.470626 pypck-0.7.8/
--rw-r--r--   0 root         (0) root         (0)     6082 2021-01-05 06:33:00.470626 pypck-0.7.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4614 2020-12-02 19:38:54.000000 pypck-0.7.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-05 06:33:00.470626 pypck-0.7.8/pypck/
--rw-r--r--   0 root         (0) root         (0)      750 2021-01-04 21:45:04.000000 pypck-0.7.8/pypck/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26490 2021-01-05 06:11:47.000000 pypck-0.7.8/pypck/connection.py
--rw-r--r--   0 root         (0) root         (0)    35855 2021-01-05 06:11:47.000000 pypck-0.7.8/pypck/inputs.py
--rw-r--r--   0 root         (0) root         (0)     2383 2021-01-04 21:45:04.000000 pypck-0.7.8/pypck/lcn_addr.py
--rw-r--r--   0 root         (0) root         (0)    39849 2021-01-04 21:45:04.000000 pypck-0.7.8/pypck/lcn_defs.py
--rw-r--r--   0 root         (0) root         (0)    38420 2021-01-05 06:11:47.000000 pypck-0.7.8/pypck/module.py
--rw-r--r--   0 root         (0) root         (0)    45357 2021-01-04 21:45:04.000000 pypck-0.7.8/pypck/pck_commands.py
--rw-r--r--   0 root         (0) root         (0)    24218 2021-01-04 21:45:04.000000 pypck-0.7.8/pypck/request_handlers.py
--rw-r--r--   0 root         (0) root         (0)     4660 2021-01-04 21:45:04.000000 pypck-0.7.8/pypck/timeout_retry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-05 06:33:00.470626 pypck-0.7.8/pypck.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6082 2021-01-05 06:33:00.000000 pypck-0.7.8/pypck.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2021-01-05 06:33:00.000000 pypck-0.7.8/pypck.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-05 06:33:00.000000 pypck-0.7.8/pypck.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-01-05 06:33:00.000000 pypck-0.7.8/pypck.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-01-05 06:33:00.470626 pypck-0.7.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      762 2021-01-05 06:11:47.000000 pypck-0.7.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-05 06:33:00.470626 pypck-0.7.8/tests/
--rw-r--r--   0 root         (0) root         (0)       30 2020-06-19 09:46:02.000000 pypck-0.7.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2664 2021-01-05 06:11:47.000000 pypck-0.7.8/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-05 06:33:00.470626 pypck-0.7.8/tests/messages/
--rw-r--r--   0 root         (0) root         (0)       56 2020-11-25 16:14:08.000000 pypck-0.7.8/tests/messages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1365 2021-01-05 06:11:47.000000 pypck-0.7.8/tests/messages/test_input_flow.py
--rw-r--r--   0 root         (0) root         (0)     1943 2021-01-05 06:11:47.000000 pypck-0.7.8/tests/messages/test_output_status.py
--rw-r--r--   0 root         (0) root         (0)     1786 2021-01-05 06:11:47.000000 pypck-0.7.8/tests/messages/test_send_command_host.py
--rw-r--r--   0 root         (0) root         (0)    12519 2021-01-05 06:11:47.000000 pypck-0.7.8/tests/test_connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 14:08:49.015674 pypck-0.7.9/
+-rw-r--r--   0 root         (0) root         (0)     6082 2021-01-17 14:08:49.015674 pypck-0.7.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4614 2021-01-17 13:10:56.000000 pypck-0.7.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 14:08:49.015674 pypck-0.7.9/pypck/
+-rw-r--r--   0 root         (0) root         (0)      777 2021-01-17 13:38:44.000000 pypck-0.7.9/pypck/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25333 2021-01-17 14:03:33.000000 pypck-0.7.9/pypck/connection.py
+-rw-r--r--   0 root         (0) root         (0)      861 2021-01-17 13:38:44.000000 pypck-0.7.9/pypck/helpers.py
+-rw-r--r--   0 root         (0) root         (0)    35855 2021-01-17 13:10:56.000000 pypck-0.7.9/pypck/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2021-01-04 21:45:04.000000 pypck-0.7.9/pypck/lcn_addr.py
+-rw-r--r--   0 root         (0) root         (0)    39849 2021-01-17 13:41:59.000000 pypck-0.7.9/pypck/lcn_defs.py
+-rw-r--r--   0 root         (0) root         (0)    38304 2021-01-17 13:38:44.000000 pypck-0.7.9/pypck/module.py
+-rw-r--r--   0 root         (0) root         (0)    45357 2021-01-04 21:45:04.000000 pypck-0.7.9/pypck/pck_commands.py
+-rw-r--r--   0 root         (0) root         (0)    24248 2021-01-17 13:38:44.000000 pypck-0.7.9/pypck/request_handlers.py
+-rw-r--r--   0 root         (0) root         (0)     4580 2021-01-17 13:38:44.000000 pypck-0.7.9/pypck/timeout_retry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 14:08:49.015674 pypck-0.7.9/pypck.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6082 2021-01-17 14:08:48.000000 pypck-0.7.9/pypck.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2021-01-17 14:08:48.000000 pypck-0.7.9/pypck.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-17 14:08:48.000000 pypck-0.7.9/pypck.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2021-01-17 14:08:48.000000 pypck-0.7.9/pypck.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-01-17 14:08:49.015674 pypck-0.7.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      762 2021-01-17 14:06:43.000000 pypck-0.7.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 14:08:49.015674 pypck-0.7.9/tests/
+-rw-r--r--   0 root         (0) root         (0)       30 2020-06-19 09:46:02.000000 pypck-0.7.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2021-01-17 13:38:44.000000 pypck-0.7.9/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 14:08:49.015674 pypck-0.7.9/tests/messages/
+-rw-r--r--   0 root         (0) root         (0)       56 2020-11-25 16:14:08.000000 pypck-0.7.9/tests/messages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2021-01-17 13:10:56.000000 pypck-0.7.9/tests/messages/test_input_flow.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2021-01-17 13:10:56.000000 pypck-0.7.9/tests/messages/test_output_status.py
+-rw-r--r--   0 root         (0) root         (0)     1786 2021-01-17 13:10:56.000000 pypck-0.7.9/tests/messages/test_send_command_host.py
+-rw-r--r--   0 root         (0) root         (0)    12519 2021-01-17 13:10:56.000000 pypck-0.7.9/tests/test_connection.py
```

### Comparing `pypck-0.7.8/PKG-INFO` & `pypck-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypck
-Version: 0.7.8
+Version: 0.7.9
 Summary: LCN-PCK library
 Home-page: https://github.com/alengwenus/pypck
 Author: Andre Lengwenus
 Author-email: alengwenus@gmail.com
 License: EPL-2.0
 Description: # pypck - Asynchronous LCN-PCK library written in Python
```

### Comparing `pypck-0.7.8/README.md` & `pypck-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pypck-0.7.8/pypck/__init__.py` & `pypck-0.7.9/pypck/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 
 SPDX-License-Identifier: EPL-2.0
 
 Contributors:
   Andre Lengwenus - port to Python and further improvements
   Tobias Juettner - initial LCN binding for openHAB (Java)
 """
-
 from pypck import (
     connection,
+    helpers,
     inputs,
     lcn_addr,
     lcn_defs,
     module,
     pck_commands,
     timeout_retry,
 )
 
 __all__ = [
     "connection",
     "inputs",
+    "helpers",
     "lcn_addr",
     "lcn_defs",
     "module",
     "pck_commands",
     "timeout_retry",
 ]
```

### Comparing `pypck-0.7.8/pypck/connection.py` & `pypck-0.7.9/pypck/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,50 +13,28 @@
   Andre Lengwenus - port to Python and further improvements
   Tobias Juettner - initial LCN binding for openHAB (Java)
 """
 
 import asyncio
 import logging
 from types import TracebackType
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Set,
-    Type,
-    Union,
-)
+from typing import Any, Awaitable, Callable, Dict, Iterable, List, Optional, Type, Union
 
 from pypck import inputs, lcn_defs
+from pypck.helpers import cancel_all_tasks, create_task
 from pypck.lcn_addr import LcnAddr
 from pypck.module import AbstractConnection, GroupConnection, ModuleConnection
 from pypck.pck_commands import PckGenerator
 
 _LOGGER = logging.getLogger(__name__)
 
 READ_TIMEOUT = -1
 SOCKET_CLOSED = -2
 
 
-async def cancel(task: "asyncio.Task[Any]") -> None:
-    """Cancel a task.
-
-    Wait for cancellation completed but do not propagate a possible CancelledError.
-    """
-    task.cancel()
-    try:
-        await task
-    except asyncio.CancelledError:
-        pass
-
-
 class PchkLicenseError(Exception):
     """Exception which is raised if a license error occurred."""
 
     def __init__(self, message: Optional[str] = None):
         """Initialize instance."""
         if message is None:
             message = (
@@ -108,42 +86,41 @@
     def __init__(self, host: str, port: int, connection_id: str = "PCHK"):
         """Construct PchkConnection."""
         self.host = host
         self.port = port
         self.connection_id = connection_id
         self.reader: Optional[asyncio.StreamReader] = None
         self.writer: Optional[asyncio.StreamWriter] = None
-        self.read_data_loop_task: Optional["asyncio.Task[None]"] = None
         self.event_handler: Callable[
             [str], Awaitable[None]
         ] = self.default_event_handler
 
     async def async_connect(self) -> None:
         """Connect to a PCHK server (no authentication or license error check)."""
         self.reader, self.writer = await asyncio.open_connection(self.host, self.port)
         address = self.writer.get_extra_info("peername")
         _LOGGER.debug("%s server connected at %s:%d", self.connection_id, *address)
 
         # main read loop
-        self.read_data_loop_task = asyncio.create_task(self.read_data_loop())
+        create_task(self.read_data_loop())
 
     def connect(self) -> None:
         """Create a task to connect to a PCHK server concurrently."""
-        asyncio.create_task(self.async_connect())
+        create_task(self.async_connect())
 
     async def read_data_loop(self) -> None:
         """Is called when some data is received."""
         assert self.reader is not None
         assert self.writer is not None
         while not self.writer.is_closing():
             try:
                 data = await self.reader.readuntil(PckGenerator.TERMINATION.encode())
             except asyncio.IncompleteReadError:
                 _LOGGER.debug("Connection to %s lost", self.connection_id)
-                asyncio.create_task(self.event_handler("connection-lost"))
+                create_task(self.event_handler("connection-lost"))
                 await self.async_close()
                 break
             except asyncio.CancelledError:
                 break
 
             message = data.decode().split(PckGenerator.TERMINATION)[0]
             await self.process_message(message)
@@ -173,17 +150,15 @@
 
         :param    str    input:    Input text message
         """
         _LOGGER.debug("from %s: %s", self.connection_id, message)
 
     async def async_close(self) -> None:
         """Close the active connection."""
-        if self.read_data_loop_task is not None:
-            # or asyncio.current_task() == self.read_data_loop_task
-            await cancel(self.read_data_loop_task)
+        await cancel_all_tasks()
         if self.writer:
             self.writer.close()
             await self.writer.wait_closed()
 
     def set_event_handler(self, coro: Callable[[str], Awaitable[None]]) -> None:
         """Set the event handler for specific LCN events."""
         if coro is None:
@@ -246,30 +221,23 @@
         self.password = password
 
         if settings is None:
             settings = {}
         self.settings = lcn_defs.default_connection_settings
         self.settings.update(settings)
 
-        self.ping_interval = 60 * 10  # seconds
+        self.ping_timeout = self.settings["PING_TIMEOUT"] / 1000  # seconds
         self.ping_counter = 0
 
         self.dim_mode = self.settings["DIM_MODE"]
         self.status_mode = lcn_defs.OutputPortStatusMode.PERCENT
 
         self.is_lcn_connected = True
         self.local_seg_id = 0
 
-        # Tasks
-        self.ping_task: Optional["asyncio.Task[None]"] = None
-        self.read_data_loop_task: Optional["asyncio.Task[None]"] = None
-        self.request_serials_tasks: Set[
-            "asyncio.Task[Dict[str, Union[int, lcn_defs.HardwareType]]]"
-        ] = set()
-
         # Events, Futures, Locks for synchronization
         self.segment_scan_completed_event = asyncio.Event()
         self.authentication_completed_future: "asyncio.Future[bool]" = asyncio.Future()
         self.license_error_future: "asyncio.Future[bool]" = asyncio.Future()
         self.module_serial_number_received = asyncio.Lock()
         self.segment_coupler_response_received = asyncio.Lock()
 
@@ -326,29 +294,29 @@
     async def on_successful_login(self) -> None:
         """Is called after connection to LCN bus system is established."""
         _LOGGER.debug("%s login successful.", self.connection_id)
         await self.send_command(
             PckGenerator.set_operation_mode(self.dim_mode, self.status_mode),
             to_host=True,
         )
-        self.ping_task = asyncio.create_task(self.ping())
+        create_task(self.ping())
 
     async def lcn_connection_status_changed(self, is_lcn_connected: bool) -> None:
         """Set the current connection state to the LCN bus.
 
         :param    bool    is_lcn_connected: Current connection status
         """
         self.is_lcn_connected = is_lcn_connected
-        asyncio.create_task(self.event_handler("lcn-connection-status-changed"))
+        create_task(self.event_handler("lcn-connection-status-changed"))
         if is_lcn_connected:
             _LOGGER.debug("%s: LCN is connected.", self.connection_id)
-            asyncio.create_task(self.event_handler("lcn-connected"))
+            create_task(self.event_handler("lcn-connected"))
         else:
             _LOGGER.debug("%s: LCN is not connected.", self.connection_id)
-            asyncio.create_task(self.event_handler("lcn-disconnected"))
+            create_task(self.event_handler("lcn-disconnected"))
 
     async def async_connect(self, timeout: int = 30) -> None:
         """Establish a connection to PCHK at the given socket.
 
         Ensures that the LCN bus is present and authorizes at PCHK.
         Raise a :class:`TimeoutError`, if connection could not be established
         within the given timeout.
@@ -383,19 +351,16 @@
         # start segment scan
         await self.scan_segment_couplers(
             self.settings["SK_NUM_TRIES"], self.settings["DEFAULT_TIMEOUT_MSEC"]
         )
 
     async def async_close(self) -> None:
         """Close the active connection."""
-        await super().async_close()
-        if self.ping_task is not None:
-            await cancel(self.ping_task)
-        await asyncio.gather(*(cancel(t) for t in self.request_serials_tasks))
         await self.cancel_requests()
+        await super().async_close()
         _LOGGER.debug("Connection to %s closed.", self.connection_id)
 
     def set_local_seg_id(self, local_seg_id: int) -> None:
         """Set the local segment id.
 
         :param    int    local_seg_id:    The local segment_id.
         """
@@ -460,17 +425,15 @@
         assert not addr.is_group
         if addr.seg_id == 0 and self.local_seg_id != -1:
             addr = LcnAddr(self.local_seg_id, addr.addr_id, addr.is_group)
         address_conn = self.address_conns.get(addr, None)
         if address_conn is None:
             address_conn = ModuleConnection(self, addr)
             if request_serials:
-                request_task = asyncio.create_task(address_conn.request_serials())
-                self.request_serials_tasks.add(request_task)
-                request_task.add_done_callback(self.request_serials_tasks.remove)
+                create_task(address_conn.request_serials())
             self.address_conns[addr] = address_conn
 
         return address_conn
 
     def get_group_conn(self, addr: LcnAddr) -> GroupConnection:
         """Create and return the GroupConnection for the given group.
 
@@ -610,15 +573,15 @@
 
     async def ping(self) -> None:
         """Send pings."""
         assert self.writer is not None
         while not self.writer.is_closing():
             await self.send_command(f"^ping{self.ping_counter:d}", to_host=True)
             self.ping_counter += 1
-            await asyncio.sleep(self.settings["PING_TIMEOUT"])
+            await asyncio.sleep(self.ping_timeout)
 
     async def process_message(self, message: str) -> None:
         """Is called when a new text message is received from the PCHK server.
 
         This class should be reimplemented in any subclass which evaluates
         received messages.
```

### Comparing `pypck-0.7.8/pypck/inputs.py` & `pypck-0.7.9/pypck/inputs.py`

 * *Files identical despite different names*

### Comparing `pypck-0.7.8/pypck/lcn_addr.py` & `pypck-0.7.9/pypck/lcn_addr.py`

 * *Files identical despite different names*

### Comparing `pypck-0.7.8/pypck/lcn_defs.py` & `pypck-0.7.9/pypck/lcn_defs.py`

 * *Files identical despite different names*

### Comparing `pypck-0.7.8/pypck/module.py` & `pypck-0.7.9/pypck/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     Sequence,
     Set,
     Union,
     cast,
 )
 
 from pypck import inputs, lcn_defs
+from pypck.helpers import create_task
 from pypck.lcn_addr import LcnAddr
 from pypck.pck_commands import PckGenerator
 from pypck.request_handlers import (
     CommentRequestHandler,
     GroupMembershipDynamicRequestHandler,
     GroupMembershipStaticRequestHandler,
     NameRequestHandler,
@@ -829,17 +830,15 @@
         )
         self.dynamic_groups_request_handler = GroupMembershipDynamicRequestHandler(
             self, num_tries, timeout_msec
         )
 
         self.status_requests_handler = StatusRequestsHandler(self)
         if self.activate_status_requests:
-            self.activate_srh_task = asyncio.create_task(
-                self.activate_status_request_handlers()
-            )
+            create_task(self.activate_status_request_handlers())
 
     async def send_command(self, wants_ack: bool, pck: Union[str, bytes]) -> bool:
         """Send a command to the module represented by this class.
 
         :param    bool    wants_ack:    Also send a request for acknowledge.
         :param    str     pck:          PCK command (without header).
         """
@@ -884,26 +883,25 @@
         :param     int    code:           The LCN internal code. -1 means
                                           "positive" acknowledge
         """
         await self.acknowledges.put(code)
 
     async def activate_status_request_handler(self, item: Any) -> None:
         """Activate a specific TimeoutRetryHandler for status requests."""
-        await self.status_requests_handler.activate(item)
+        create_task(self.status_requests_handler.activate(item))
 
     async def activate_status_request_handlers(self) -> None:
         """Activate all TimeoutRetryHandlers for status requests."""
-        await self.status_requests_handler.activate_all(activate_s0=self.has_s0_enabled)
+        create_task(
+            self.status_requests_handler.activate_all(activate_s0=self.has_s0_enabled)
+        )
 
     async def cancel_status_request_handler(self, item: Any) -> None:
         """Cancel a specific TimeoutRetryHandler for status requests."""
         await self.status_requests_handler.cancel(item)
-        if self.activate_status_requests:
-            self.activate_srh_task.cancel()
-            await self.activate_srh_task
 
     async def cancel_status_request_handlers(self) -> None:
         """Canecl all TimeoutRetryHandlers for status requests."""
         await self.status_requests_handler.cancel_all()
 
     async def cancel_requests(self) -> None:
         """Cancel all TimeoutRetryHandlers."""
```

### Comparing `pypck-0.7.8/pypck/pck_commands.py` & `pypck-0.7.9/pypck/pck_commands.py`

 * *Files identical despite different names*

### Comparing `pypck-0.7.8/pypck/request_handlers.py` & `pypck-0.7.9/pypck/request_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   Andre Lengwenus - Request handler logic
 """
 
 import asyncio
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Union
 
 from pypck import inputs, lcn_defs
+from pypck.helpers import create_task
 from pypck.lcn_addr import LcnAddr
 from pypck.pck_commands import PckGenerator
 from pypck.timeout_retry import TimeoutRetryHandler
 
 if TYPE_CHECKING:
     from pypck.module import ModuleConnection
 
@@ -45,15 +46,15 @@
 
     async def request(self) -> Any:
         """Request information from module."""
         raise NotImplementedError()
 
     def process_input(self, inp: inputs.Input) -> None:
         """Create a task to process the input object concurrently."""
-        asyncio.create_task(self.async_process_input(inp))
+        create_task(self.async_process_input(inp))
 
     async def async_process_input(self, inp: inputs.Input) -> None:
         """Process incoming input object.
 
         Method to handle incoming commands for this request handler.
         """
         raise NotImplementedError()
```

### Comparing `pypck-0.7.8/pypck/timeout_retry.py` & `pypck-0.7.9/pypck/timeout_retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
   Tobias Juettner - initial LCN binding for openHAB (Java)
 """
 
 import asyncio
 import logging
 from typing import Any, Awaitable, Callable, Dict, Optional, Tuple, Union
 
+from pypck.helpers import cancel_task, create_task
+
 _LOGGER = logging.getLogger(__name__)
 
 # The default timeout to use for requests. Worst case: Requesting threshold
 # 4-4 takes at least 1.8s
 DEFAULT_TIMEOUT_MSEC = 3500
 
 
@@ -64,35 +66,31 @@
         """
         self._timeout_callback = timeout_callback
         self._timeout_args = timeout_args
         self._timeout_kwargs = timeout_kwargs
 
     def activate(self) -> None:
         """Schedule the next activation."""
-        asyncio.create_task(self.async_activate())
+        create_task(self.async_activate())
 
     async def async_activate(self) -> None:
         """Clean start of next timeout_loop."""
         if self.is_active():
             await self.cancel()
-        self.timeout_loop_task = asyncio.create_task(self.timeout_loop())
+        self.timeout_loop_task = create_task(self.timeout_loop())
 
     async def done(self) -> None:
         """Signal the completion of the TimeoutRetryHandler."""
         if self.timeout_loop_task is not None:
             await self.timeout_loop_task
 
     async def cancel(self) -> None:
         """Must be called when a response (requested or not) is received."""
         if self.timeout_loop_task is not None:
-            self.timeout_loop_task.cancel()
-            try:
-                await self.timeout_loop_task
-            except asyncio.CancelledError:
-                pass
+            await cancel_task(self.timeout_loop_task)
 
     def is_active(self) -> bool:
         """Check whether the request logic is active."""
         if self.timeout_loop_task is None:
             return False
         return not self.timeout_loop_task.done()
```

### Comparing `pypck-0.7.8/pypck.egg-info/PKG-INFO` & `pypck-0.7.9/pypck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypck
-Version: 0.7.8
+Version: 0.7.9
 Summary: LCN-PCK library
 Home-page: https://github.com/alengwenus/pypck
 Author: Andre Lengwenus
 Author-email: alengwenus@gmail.com
 License: EPL-2.0
 Description: # pypck - Asynchronous LCN-PCK library written in Python
```

### Comparing `pypck-0.7.8/setup.py` & `pypck-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypck",
-    version="0.7.8",
+    version="0.7.9",
     author="Andre Lengwenus",
     author_email="alengwenus@gmail.com",
     description="LCN-PCK library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alengwenus/pypck",
     packages=setuptools.find_packages(exclude=(["tests", "tests.*"])),
```

### Comparing `pypck-0.7.8/tests/conftest.py` & `pypck-0.7.9/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Core testing functionality."""
 
 import asyncio
 from typing import Any, AsyncGenerator, List
+
 import pytest
 from pypck.connection import PchkConnectionManager
-from pypck.module import ModuleConnection
+from pypck.helpers import PYPCK_TASKS
 from pypck.lcn_addr import LcnAddr
+from pypck.module import ModuleConnection
 from pypck.pck_commands import PckGenerator
 
 from .fake_pchk import PchkServer
 
 HOST = "127.0.0.1"
 PORT = 4114
 USERNAME = "lcn_username"
@@ -69,14 +71,15 @@
     which returns if the specified message was received (and processed).
     """
     pcm = MockPchkConnectionManager(
         HOST, PORT, USERNAME, PASSWORD, settings={"SK_NUM_TRIES": 0}
     )
     yield pcm
     await pcm.async_close()
+    assert len(PYPCK_TASKS) == 0
 
 
 @pytest.fixture
 async def module10(
     pypck_client: PchkConnectionManager,
 ) -> AsyncGenerator[ModuleConnection, None]:
     """Create test module with addr_id 10."""
```

### Comparing `pypck-0.7.8/tests/messages/test_input_flow.py` & `pypck-0.7.9/tests/messages/test_input_flow.py`

 * *Files identical despite different names*

### Comparing `pypck-0.7.8/tests/messages/test_output_status.py` & `pypck-0.7.9/tests/messages/test_output_status.py`

 * *Files identical despite different names*

### Comparing `pypck-0.7.8/tests/messages/test_send_command_host.py` & `pypck-0.7.9/tests/messages/test_send_command_host.py`

 * *Files identical despite different names*

### Comparing `pypck-0.7.8/tests/test_connection.py` & `pypck-0.7.9/tests/test_connection.py`

 * *Files identical despite different names*

