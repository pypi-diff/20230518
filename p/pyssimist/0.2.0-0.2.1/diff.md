# Comparing `tmp/pyssimist-0.2.0.tar.gz` & `tmp/pyssimist-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\A477372\PycharmProjects\pysimist\dist\.tmp-sws62pay\pyssimist-0.2.0.tar", last modified: Thu Mar  2 08:12:11 2023, max compression
+gzip compressed data, was "C:\Users\A477372\PycharmProjects\pysimist\dist\.tmp-ktjku4ez\pyssimist-0.2.1.tar", last modified: Thu May 18 08:23:33 2023, max compression
```

## Comparing `pyssimist-0.2.0.tar` & `pyssimist-0.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 08:12:11.000000 pyssimist-0.2.0/
--rw-rw-rw-   0        0        0    35823 2018-11-01 13:39:45.000000 pyssimist-0.2.0/LICENSE
--rw-rw-rw-   0        0        0        0 2021-05-02 15:47:58.000000 pyssimist-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      285 2023-03-02 08:12:11.000000 pyssimist-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       85 2021-03-24 21:22:02.000000 pyssimist-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 08:12:11.000000 pyssimist-0.2.0/common/
--rw-rw-rw-   0        0        0        0 2018-11-13 17:26:53.000000 pyssimist-0.2.0/common/__init__.py
--rw-rw-rw-   0        0        0     8735 2023-02-17 14:24:14.000000 pyssimist-0.2.0/common/client.py
--rw-rw-rw-   0        0        0    10133 2020-02-06 15:37:36.000000 pyssimist-0.2.0/common/client_server.py
--rw-rw-rw-   0        0        0    20433 2021-03-24 21:21:36.000000 pyssimist-0.2.0/common/server.py
--rw-rw-rw-   0        0        0     1128 2019-07-01 07:11:00.000000 pyssimist-0.2.0/common/tc_logging.py
--rw-rw-rw-   0        0        0    15352 2023-02-23 16:15:13.000000 pyssimist-0.2.0/common/util.py
--rw-rw-rw-   0        0        0     3527 2023-02-18 14:41:45.000000 pyssimist-0.2.0/common/view.py
-drwxrwxrwx   0        0        0        0 2023-03-02 08:12:11.000000 pyssimist-0.2.0/csta/
--rw-rw-rw-   0        0        0    18959 2023-02-20 10:48:26.000000 pyssimist-0.2.0/csta/CstaApplication.py
--rw-rw-rw-   0        0        0    10493 2020-07-31 13:54:58.000000 pyssimist-0.2.0/csta/CstaEndpoint.py
--rw-rw-rw-   0        0        0     1154 2021-05-25 14:36:47.000000 pyssimist-0.2.0/csta/CstaFlows.py
--rw-rw-rw-   0        0        0     3557 2021-05-10 08:38:46.000000 pyssimist-0.2.0/csta/CstaMessage.py
--rw-rw-rw-   0        0        0     8525 2023-02-15 10:21:35.000000 pyssimist-0.2.0/csta/CstaParser.py
-drwxrwxrwx   0        0        0        0 2023-03-02 08:12:11.000000 pyssimist-0.2.0/csta/CstaPool/
--rw-rw-rw-   0        0        0      493 2020-08-01 10:13:35.000000 pyssimist-0.2.0/csta/CstaPool/ClearConnection.xml
--rw-rw-rw-   0        0        0      361 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/ClearConnectionResponse.xml
--rw-rw-rw-   0        0        0      749 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/ConnectionClearedEvent.xml
--rw-rw-rw-   0        0        0     1239 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/DeliveredEvent.xml
--rw-rw-rw-   0        0        0     1266 2020-08-01 10:13:35.000000 pyssimist-0.2.0/csta/CstaPool/EstablishedEvent.xml
--rw-rw-rw-   0        0        0      516 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/MakeCall.xml
--rw-rw-rw-   0        0        0      443 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/MakeCallResponse.xml
--rw-rw-rw-   0        0        0      443 2020-08-01 10:13:35.000000 pyssimist-0.2.0/csta/CstaPool/MonitorStart.xml
--rw-rw-rw-   0        0        0      456 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/MonitorStartResponse.xml
--rw-rw-rw-   0        0        0     1054 2020-08-01 10:13:35.000000 pyssimist-0.2.0/csta/CstaPool/OriginatedEvent.xml
--rw-rw-rw-   0        0        0      986 2020-08-01 10:13:35.000000 pyssimist-0.2.0/csta/CstaPool/ServiceInitiatedEvent.xml
--rw-rw-rw-   0        0        0      280 2020-08-01 09:18:45.000000 pyssimist-0.2.0/csta/CstaPool/SnapshotDevice.xml
--rw-rw-rw-   0        0        0      225 2020-08-16 09:55:52.000000 pyssimist-0.2.0/csta/CstaPool/SnapshotDeviceResponse.xml
--rw-rw-rw-   0        0        0      499 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/SystemRegister.xml
--rw-rw-rw-   0        0        0      155 2018-11-13 17:26:53.000000 pyssimist-0.2.0/csta/CstaPool/SystemRegisterResponse.xml
--rw-rw-rw-   0        0        0      410 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/SystemStatus.xml
--rw-rw-rw-   0        0        0      131 2020-08-10 10:52:00.000000 pyssimist-0.2.0/csta/CstaPool/SystemStatusResponse.xml
--rw-rw-rw-   0        0        0      466 2020-08-01 10:13:34.000000 pyssimist-0.2.0/csta/CstaPool/SystemStatus_RegisterID.xml
--rw-rw-rw-   0        0        0     7454 2023-02-20 15:19:29.000000 pyssimist-0.2.0/csta/CstaUser.py
--rw-rw-rw-   0        0        0        0 2018-11-13 17:26:53.000000 pyssimist-0.2.0/csta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-02 08:12:11.000000 pyssimist-0.2.0/pyssimist.egg-info/
--rw-rw-rw-   0        0        0      285 2023-03-02 08:12:11.000000 pyssimist-0.2.0/pyssimist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1334 2023-03-02 08:12:11.000000 pyssimist-0.2.0/pyssimist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 08:12:11.000000 pyssimist-0.2.0/pyssimist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-03-02 08:12:11.000000 pyssimist-0.2.0/pyssimist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-02 08:12:11.000000 pyssimist-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      427 2023-03-02 07:40:15.000000 pyssimist-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-02 08:12:11.000000 pyssimist-0.2.0/sip/
--rw-rw-rw-   0        0        0    27636 2023-02-18 14:12:26.000000 pyssimist-0.2.0/sip/SipEndpoint.py
--rw-rw-rw-   0        0        0     1229 2019-05-03 06:51:09.000000 pyssimist-0.2.0/sip/SipFlows.py
--rw-rw-rw-   0        0        0    10589 2022-05-27 07:57:05.000000 pyssimist-0.2.0/sip/SipMessage.py
--rw-rw-rw-   0        0        0     8055 2021-05-02 15:48:04.000000 pyssimist-0.2.0/sip/SipParser.py
--rw-rw-rw-   0        0        0        0 2018-11-13 17:26:53.000000 pyssimist-0.2.0/sip/__init__.py
--rw-rw-rw-   0        0        0     8109 2020-10-14 19:36:32.000000 pyssimist-0.2.0/sip/messages.py
-drwxrwxrwx   0        0        0        0 2023-03-02 08:12:11.000000 pyssimist-0.2.0/tshark_tools/
--rw-rw-rw-   0        0        0        0 2020-02-23 12:42:57.000000 pyssimist-0.2.0/tshark_tools/__init__.py
--rw-rw-rw-   0        0        0    13557 2020-04-22 16:56:12.000000 pyssimist-0.2.0/tshark_tools/analyze_gui.py
--rw-rw-rw-   0        0        0      531 2020-02-23 13:56:23.000000 pyssimist-0.2.0/tshark_tools/check_trace.py
--rw-rw-rw-   0        0        0     4364 2020-04-16 21:43:47.000000 pyssimist-0.2.0/tshark_tools/describe.py
--rw-rw-rw-   0        0        0     4471 2020-05-08 12:49:12.000000 pyssimist-0.2.0/tshark_tools/diff.py
--rw-rw-rw-   0        0        0    22596 2020-05-08 12:40:43.000000 pyssimist-0.2.0/tshark_tools/lib.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:23:33.000000 pyssimist-0.2.1/
+-rw-rw-rw-   0        0        0    35823 2018-11-01 13:39:45.000000 pyssimist-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2021-05-02 15:47:58.000000 pyssimist-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      285 2023-05-18 08:23:33.000000 pyssimist-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2021-03-24 21:22:02.000000 pyssimist-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 08:23:33.000000 pyssimist-0.2.1/common/
+-rw-rw-rw-   0        0        0        0 2018-11-13 17:26:53.000000 pyssimist-0.2.1/common/__init__.py
+-rw-rw-rw-   0        0        0     9760 2023-04-28 13:37:49.000000 pyssimist-0.2.1/common/client.py
+-rw-rw-rw-   0        0        0    10133 2020-02-06 15:37:36.000000 pyssimist-0.2.1/common/client_server.py
+-rw-rw-rw-   0        0        0    20433 2021-03-24 21:21:36.000000 pyssimist-0.2.1/common/server.py
+-rw-rw-rw-   0        0        0     1128 2023-03-20 17:07:12.000000 pyssimist-0.2.1/common/tc_logging.py
+-rw-rw-rw-   0        0        0    16142 2023-04-28 10:07:57.000000 pyssimist-0.2.1/common/util.py
+-rw-rw-rw-   0        0        0     7279 2023-05-01 08:57:08.000000 pyssimist-0.2.1/common/view.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:23:33.000000 pyssimist-0.2.1/csta/
+-rw-rw-rw-   0        0        0    22043 2023-04-28 08:13:38.000000 pyssimist-0.2.1/csta/CstaApplication.py
+-rw-rw-rw-   0        0        0    10493 2020-07-31 13:54:58.000000 pyssimist-0.2.1/csta/CstaEndpoint.py
+-rw-rw-rw-   0        0        0     1154 2021-05-25 14:36:47.000000 pyssimist-0.2.1/csta/CstaFlows.py
+-rw-rw-rw-   0        0        0     3557 2023-03-17 16:38:53.000000 pyssimist-0.2.1/csta/CstaMessage.py
+-rw-rw-rw-   0        0        0    12374 2023-03-17 16:28:36.000000 pyssimist-0.2.1/csta/CstaParser.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:23:33.000000 pyssimist-0.2.1/csta/CstaPool/
+-rw-rw-rw-   0        0        0      493 2020-08-01 10:13:35.000000 pyssimist-0.2.1/csta/CstaPool/ClearConnection.xml
+-rw-rw-rw-   0        0        0      361 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/ClearConnectionResponse.xml
+-rw-rw-rw-   0        0        0      749 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/ConnectionClearedEvent.xml
+-rw-rw-rw-   0        0        0     1239 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/DeliveredEvent.xml
+-rw-rw-rw-   0        0        0     1266 2020-08-01 10:13:35.000000 pyssimist-0.2.1/csta/CstaPool/EstablishedEvent.xml
+-rw-rw-rw-   0        0        0      516 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/MakeCall.xml
+-rw-rw-rw-   0        0        0      443 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/MakeCallResponse.xml
+-rw-rw-rw-   0        0        0      443 2020-08-01 10:13:35.000000 pyssimist-0.2.1/csta/CstaPool/MonitorStart.xml
+-rw-rw-rw-   0        0        0      456 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/MonitorStartResponse.xml
+-rw-rw-rw-   0        0        0     1054 2020-08-01 10:13:35.000000 pyssimist-0.2.1/csta/CstaPool/OriginatedEvent.xml
+-rw-rw-rw-   0        0        0      986 2020-08-01 10:13:35.000000 pyssimist-0.2.1/csta/CstaPool/ServiceInitiatedEvent.xml
+-rw-rw-rw-   0        0        0      280 2020-08-01 09:18:45.000000 pyssimist-0.2.1/csta/CstaPool/SnapshotDevice.xml
+-rw-rw-rw-   0        0        0      225 2020-08-16 09:55:52.000000 pyssimist-0.2.1/csta/CstaPool/SnapshotDeviceResponse.xml
+-rw-rw-rw-   0        0        0      499 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/SystemRegister.xml
+-rw-rw-rw-   0        0        0      155 2018-11-13 17:26:53.000000 pyssimist-0.2.1/csta/CstaPool/SystemRegisterResponse.xml
+-rw-rw-rw-   0        0        0      410 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/SystemStatus.xml
+-rw-rw-rw-   0        0        0      131 2020-08-10 10:52:00.000000 pyssimist-0.2.1/csta/CstaPool/SystemStatusResponse.xml
+-rw-rw-rw-   0        0        0      466 2020-08-01 10:13:34.000000 pyssimist-0.2.1/csta/CstaPool/SystemStatus_RegisterID.xml
+-rw-rw-rw-   0        0        0     7762 2023-03-17 16:53:34.000000 pyssimist-0.2.1/csta/CstaUser.py
+-rw-rw-rw-   0        0        0        0 2018-11-13 17:26:53.000000 pyssimist-0.2.1/csta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:23:33.000000 pyssimist-0.2.1/pyssimist.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-05-18 08:23:33.000000 pyssimist-0.2.1/pyssimist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1334 2023-05-18 08:23:33.000000 pyssimist-0.2.1/pyssimist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 08:23:33.000000 pyssimist-0.2.1/pyssimist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-18 08:23:33.000000 pyssimist-0.2.1/pyssimist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 08:23:33.000000 pyssimist-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      427 2023-05-17 06:56:58.000000 pyssimist-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:23:33.000000 pyssimist-0.2.1/sip/
+-rw-rw-rw-   0        0        0    34183 2023-04-28 09:23:29.000000 pyssimist-0.2.1/sip/SipEndpoint.py
+-rw-rw-rw-   0        0        0     1229 2019-05-03 06:51:09.000000 pyssimist-0.2.1/sip/SipFlows.py
+-rw-rw-rw-   0        0        0    10417 2023-04-28 09:20:27.000000 pyssimist-0.2.1/sip/SipMessage.py
+-rw-rw-rw-   0        0        0     8078 2023-04-28 09:09:09.000000 pyssimist-0.2.1/sip/SipParser.py
+-rw-rw-rw-   0        0        0        0 2018-11-13 17:26:53.000000 pyssimist-0.2.1/sip/__init__.py
+-rw-rw-rw-   0        0        0     8109 2020-10-14 19:36:32.000000 pyssimist-0.2.1/sip/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:23:33.000000 pyssimist-0.2.1/tshark_tools/
+-rw-rw-rw-   0        0        0        0 2020-02-23 12:42:57.000000 pyssimist-0.2.1/tshark_tools/__init__.py
+-rw-rw-rw-   0        0        0    13557 2020-04-22 16:56:12.000000 pyssimist-0.2.1/tshark_tools/analyze_gui.py
+-rw-rw-rw-   0        0        0      531 2020-02-23 13:56:23.000000 pyssimist-0.2.1/tshark_tools/check_trace.py
+-rw-rw-rw-   0        0        0     4364 2020-04-16 21:43:47.000000 pyssimist-0.2.1/tshark_tools/describe.py
+-rw-rw-rw-   0        0        0     4471 2020-05-08 12:49:12.000000 pyssimist-0.2.1/tshark_tools/diff.py
+-rw-rw-rw-   0        0        0    22596 2020-05-08 12:40:43.000000 pyssimist-0.2.1/tshark_tools/lib.py
```

### Comparing `pyssimist-0.2.0/LICENSE` & `pyssimist-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/common/client.py` & `pyssimist-0.2.1/common/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Initial Version: Costas Skarakis 11/11/2018
 """
 import selectors
 import socket
 import ssl
 import io
 from threading import Lock
-
+from time import sleep
 from common.tc_logging import debug
 from common.util import wait_for_sip_data, NoData, IncompleteData
 
 
 class TCPClient(object):
     def __init__(self, ip, port):
         self.sip_buffer = []
@@ -83,14 +83,21 @@
                     all_data = io.BytesIO(client.socket.recv(bufsize))
                     while True:
                         try:
                             # There may be more than one sip messages in the socket
                             # I think select will not trigger if we only read one of them
                             # and then come back for the second one
                             client.sip_buffer.append(wait_for_sip_data(all_data))
+                            # We will replace all_data with everything following the current
+                            # read location to discard the message that was already added to the
+                            # buffer.
+                            # In case all_data contained more than one message and the second one
+                            # was incomplete, we have to reread only the second message
+                            # not the first one again which is already in the sip_buffer
+                            all_data = io.BytesIO(all_data.read())
                         except EOFError:
                             if client.sip_buffer:
                                 data = client.sip_buffer.pop(0)
                                 break
                             else:
                                 client.wait_select(timeout)
                                 all_data = io.BytesIO(client.socket.recv(bufsize))
@@ -100,20 +107,23 @@
                             all_data = io.BytesIO(all_data.getvalue() + client.socket.recv(bufsize))
                             continue
                         except NoData:
                             if client.sip_buffer:
                                 data = client.sip_buffer.pop(0)
                             else:
                                 data = all_data.getvalue()
-                                raise ValueError
+                                debug('Invalid SIP Data in socket: ' + data.decode())
+                                all_data = io.BytesIO(all_data.read())
+                                continue
+                                # raise ValueError
                             break
             except ValueError:
                 debug('Value Error: '+data.decode())
                 # debug(line.decode())
-                raise
+                # raise
             except socket.timeout:
                 debug('Data received before timeout: "{}"'.format(data.decode()))
                 raise
             finally:
                 client.socket.settimeout(bkp)
             debug("Received on port {}:\n\n".format(client.port) + data.decode("utf8").replace("\r\n", "\n"))
             return data
@@ -126,24 +136,28 @@
             elif timeout is None:
                 self.socket.setblocking(True)
             try:
                 # header = ""
                 # while not header:
                 header = self.socket.recv(4)
                 if not header:
-                    # disconnected socket
+                    debug("Csta socket was probably disconnected from the other side")
                     return None
                 datalength = int(''.join(["%02X" % x for x in header]), base=16) - 4
                 data = b''
                 while len(data) < datalength:
                     data += self.socket.recv(datalength - len(data))
+                    sleep(0.001)
                 debug(
                     "Received on port {} message of length {}:\n\n".format(self.port, datalength) + (header + data).decode(
                         "utf8",
                         "backslashreplace").replace("\r\n", "\n"))
+            except socket.timeout:
+                debug('Data received before timeout: "{}"'.format(data.decode()))
+                raise
             finally:
                 self.socket.settimeout(bkp)
             return header + data
 
     def shutdown(self):
         self.socket.shutdown(socket.SHUT_RDWR)
```

### Comparing `pyssimist-0.2.0/common/client_server.py` & `pyssimist-0.2.1/common/client_server.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/common/server.py` & `pyssimist-0.2.1/common/server.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/common/tc_logging.py` & `pyssimist-0.2.1/common/tc_logging.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/common/util.py` & `pyssimist-0.2.1/common/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     Cyclically yields the next member of a sequence unless the specified condition is False
 
     :param sequence: input sequence, eg a list
     :param condition: a function to be run on the next member eg:
             lambda x: x.registered
     :return: yields the next eligible member
     """
+    assert sequence, "Refused to make empty pool"
     p = cycle(sequence)
     while True:
         c = next(p)
         if condition(c):
             yield c
         else:
             # If all are busy it may get intense...
@@ -112,36 +113,44 @@
     data += sockfile.readline()
 
     while True:
         line = sockfile.readline()
         data += line
         if not line.strip():
             break
+        if not line.endswith(b"\r\n"):
+            raise IncompleteData
         try:
             header, value = [x.strip() for x in line.split(b":", 1)]
         except ValueError:
-            print("Incorrect header line:", repr(line))
-            print("Message up to that:", data)
+            logger.warning("Incorrect header line (no ':') in SIP message: " + repr(line) +
+                           "\n" + "Data received up to that:" + repr(data) +
+                           "\n" + "Will attempt to get the rest of the message from the network")
             continue
         if header == b"Content-Length" or header == b"content-length":
             content_length = int(value)
 
     if not data.strip():
         raise EOFError
 
     body = ""
     if content_length > 0:
         body = sockfile.read(content_length)
         if len(body) < content_length:
-            raise IncompleteData
+            raise IncompleteData("Message body not yet complete: " + repr(data))
         else:
             data += body
 
     if content_length == -1:
-        raise IncompleteData("No content length in message: " + repr(data))
+        if line == b"\r\n":
+            # This is the case were the message ended with no Content length.
+            # This is probably an invalid message/data
+            raise NoData
+        else:
+            raise IncompleteData("No content length in message yet: " + repr(data))
     return data
 
 
 class NoData(Exception):
     pass
 
 
@@ -359,15 +368,15 @@
         self.flow = flow
         self.args = flow_args
         self.interval = interval
         self.quantity = quantity
         self.duration = duration
         self.stopCondition = stopCondition
         self.startTime = time()
-        self.active = []
+        self.active = set()
         st_logger = logging.getLogger('Statistics')
         handler = logging.handlers.RotatingFileHandler("Statistics.txt", mode="w", maxBytes=20000000, backupCount=5)
         st_logger.addHandler(handler)
         self.log = st_logger
         self.calls = {"Started": 0, "Finished": 0, "Passed": 0, "Failed": 0}
         self.loop = LoadThread(target=self._start)
         self.statistics()
@@ -399,50 +408,50 @@
         The running executions will not be interrupted
         """
         self.stopCondition = True
 
     def run_next_flow(self):
         c = LoadThread(target=self.flow, args=self.args)
         c.start()
-        self.active.append(c)
+        self.active.add(c)
         self.calls["Started"] += 1
 
     def monitor(self):
         t_prev = time()
         calls_prev = self.calls["Started"]
         while self.active or not self.stopCondition:
             sleep(0.1)
             t_now = time()
             t = t_now - t_prev
-            if t > self.interval:
+            if t > self.interval and not self.stopCondition:
                 calls_now = self.calls["Started"]
                 calls_since = calls_now - calls_prev
                 cps = calls_since / t
                 average_cps = calls_now / (t_now - self.startTime)
                 self.calls["Instant Calls Per second"] = cps
                 self.calls["Total Average Calls Per second"] = average_cps
                 calls_prev = calls_now
                 t_prev = t_now
-            for inst in (ins for ins in self.active if not ins.is_alive()):
+            for inst in (ins for ins in self.active.copy() if not ins.is_alive()):
                 try:
                     inst.join()
                     if inst.exc:
                         # Test results implied that if the exception was caught the test was counted as passed
                         self.calls["Failed"] += 1  # welp... this is not counted.
                     elif inst.exc is None:
                         self.calls["Started"] -= 1
                         continue
                     else:
                         self.calls["Passed"] += 1
-                    self.calls["Finished"] += 1
                 # except NoMoreAvailableExecutors:
                 #     continue
-                # except Exception as e:
-                #     self.calls["Failed"] += 1  # could I stop all threads in this scenario?
+                except:
+                    self.calls["Failed"] += 1  # could I stop all threads in this scenario?
                 finally:
+                    self.calls["Finished"] += 1
                     self.active.remove(inst)
         self.loop.join()
 
     def statistics(self):
         self.calls["Active"] = len(self.active)
         self.log.info("{}:{}".format(time(), self.calls))
         if not self.stopCondition and (self.duration < 0 or time() - self.startTime < self.duration) or self.active:
@@ -463,13 +472,21 @@
             # Maybe execution should be rescheduled?
             self.exc = None
             return
         except Exception as e:
             self.exc = e
             logger.exception("Exception in Thread: " + self.name)
             logger.exception(traceback.format_exc())
-            raise
+            # raise
+        finally:
+            self.cleanup()
 
     def join(self, timeout=None):
         super().join(timeout)
         if self.exc:
             raise self.exc
+
+    def cleanup(self, *args, **kwargs):
+        """
+        Custom cleanup method that will be executed when Thread exits. Should be overridden
+        """
+        pass
```

### Comparing `pyssimist-0.2.0/csta/CstaApplication.py` & `pyssimist-0.2.1/csta/CstaApplication.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,73 @@
 """\
 Purpose: Simulate a CSTA Application
-Initial Version: Costas Skarakis 7/20/2020  
+Initial Version: Costas Skarakis 7/20/2020
 """
 import os
 import traceback
 from _socket import timeout as sock_timeout
 from threading import Lock, Thread, Event
 from time import time, sleep
 
 from common.client import TCPClient
 from common.tc_logging import debug, warning, exception
 from csta.CstaEndpoint import get_xml
 from csta.CstaUser import CstaUser
 from csta.CstaParser import parseBytes, buildMessageFromFile, buildMessage
 
 
-def get_buffered_message(buffer, message):
+def get_buffered_message(buffer, message, call_id=None, monitor_x_ref_id=None, calling_device=None):
     """
     Get a message from the specified buffer.
     Best used within a threading.Lock context
 
     :param buffer: the buffer to search
-    :param message: the message to get
+    :param message: the message_type to get
+    :param call_id: the callID (if any) to request
+    :param calling_device: used to separate csta events when needed
+    :param monitor_x_ref_id: the monitorCrossRefID (if any) to request
     :return: the corresponding CstaMessage object
     """
-    for i in range(len(buffer)):
-        buffered_message = buffer.pop(0)
-        if buffered_message.event == message:
+    if message.endswith("Event"):
+        # This will fail for first csta event
+        key = str(call_id) + str(monitor_x_ref_id) + str(message)
+        if key in buffer:
+            buffered_message = buffer[key].pop(0)
+            if not buffer[key]:
+                buffer.pop(key)
             return buffered_message
-        else:
-            buffer.append(buffered_message)
+
+    # Here we look for first csta event, or csta responses
+    for k in buffer:
+        if ((message.endswith("Event") and call_id is None) or message.endswith("Response")) and \
+                k.endswith(str(message)):
+            buffered_message = buffer[k][0]
+
+            if (calling_device is not None and
+                    calling_device not in str(buffered_message).split("callingDevice")[1].split("callingDevice")[0]):
+                continue
+            else:
+                buffer[k].pop(0)
+                if not buffer[k]:
+                    buffer.pop(k)
+                return buffered_message
 
 
 class CstaApplication:
     def __init__(self, server=False):
         self.ip = None
         self.port = None
         self.link = None
         self.min_event_id = 0
         self.users = {}
         self.parameters = {}
         self.server = server
-        self.message_buffer = []
+        self.message_buffer = {}
         self.buffer_mod_time = None
+        self.buffer_trigger_count = 0
         self.lock = Lock()
         self.buffer_event = Event()
         self.shutdown_flag = False
         self.waitForCstaMessage = self.wait_for_csta_message  # compatibility alias
         self.wait_thread = None
 
     def shutdown(self):
@@ -77,16 +98,23 @@
                 break
             if inbytes is None:
                 warning("Disconnected. Will retry in 1 second")
                 sleep(1)
             else:
                 inmessage = parseBytes(inbytes)
                 try:
-                    with self.lock:
-                        self.buffer_message(inmessage)
+                    net_object = self
+                    for dn in self.users:
+                        user = self.users[dn]
+                        if (inmessage.is_event() and user.monitorCrossRefID == inmessage["monitorCrossRefID"]) or \
+                                (inmessage.is_response() and inmessage.eventid in user.out_transactions):
+                            net_object = user
+                            break
+                    with net_object.lock:
+                        self.buffer_message(net_object, inmessage)
                 except:
                     exception(traceback.format_exc())
 
     def connect(self, local_address, destination_address, protocol="tcp"):
         """ Connect to CSTA Server """
         local_ip, local_port = local_address
         self.ip = local_ip
@@ -139,49 +167,55 @@
         :param directory_number: The DN of the device to monitor
         :param force: Force sending another monitor request and create another Monitor Record for the same device
         :return: None
         """
 
         directory_number = str(directory_number)
         user = self.get_user(directory_number)
-        if force or directory_number not in self.get_monitored_users():
+        if force or user.monitorCrossRefID is None:
+            user.monitorCrossRefID = ""  # set this temporarily to avoid race condition sending monitor twice for a user
             user.parameters["user"] = directory_number
-            user.send("MonitorStart")
-            inmessage = user.wait_for_message("MonitorStartResponse")
-            user.parameters["monitorCrossRefID"] = inmessage["monitorCrossRefID"]
+            try:
+                user.send("MonitorStart")
+                inmessage = user.wait_for_message("MonitorStartResponse")
+                user.parameters["monitorCrossRefID"] = inmessage["monitorCrossRefID"]
+                user.monitorCrossRefID = user.parameters["monitorCrossRefID"]
+            except sock_timeout:
+                user.monitorCrossRefID = None
         else:
             debug("Skip MonitorStart for already Monitored user: " + directory_number + ". Use force=True to override.")
 
     # def monitor_stop(self, directory_number):
     #     """ Send MonitorStop and delete directory number from monitored users"""
     #     csta_link = self.link
     #     m = buildMessageFromFile(get_xml("MonitorStop.xml"), {"user": directory_number}, eventid=1)
     #     csta_link.send(m.contents())
     #     in_bytes = csta_link.waitForData()
     #     inmessage = parseBytes(in_bytes)
     #     assert inmessage.event == "MonitorStopResponse", "Sent:{}  Received:{}".format(m.event, str(inmessage))
     #     self.parameters.pop(directory_number)
 
     def get_monitored_users(self):
-        return list(user for user in self.users if self.get_user(user).parameters["monitorCrossRefID"] is not None)
+        return list(user for user in self.users if self.users[str(user)].monitorCrossRefID is not None)
 
     def prepare_message(self, from_user, message):
         """
         Convert a SIP message string to SipMessage object
 
         :param message: The message string
         :param from_user: The originating CSTA subscriber object
         :return: A CstaMessage object
         """
         user = self.users[from_user]
         return buildMessage(message, user.parameters)
 
-    def send(self, message, from_user=None, to_user=None):
+    def send(self, message, from_user=None, to_user=None, callID=None):
         """ Send a CSTA message
 
+        :param callID: if provided, will use this callID in the outgoing message
         :param from_user: calling number
         :param to_user: called number
         :param message: This could be a predefined csta message or just the type of the message.
                        There are already several builtin xml files that are named after the corresponding messages
                        In order to access them just provide the type of the CSTA message.
                        There should be a matching filename in csta/xml
 
@@ -193,77 +227,91 @@
         user.set_parameter("callingDevice", from_user)
         user.set_parameter("calledDirectoryNumber", to_user)
         if message.strip().startswith("<?xml"):
             m = buildMessage(message, user.parameters, eventid=0)
         else:
             m = buildMessageFromFile(get_xml(message), user.parameters, eventid=0)
         if from_user and m.event != "MonitorStart":
-            assert from_user in self.get_monitored_users(), "User {} must be monitored before sending messages".format(
+            assert user.monitorCrossRefID, "User {} must be monitored before sending messages".format(
                 from_user)
         with self.lock:
             # must do this serially to avoid sending multiple requests with the same invoke id
             eventid = user.get_transaction_id(m.event)
             m.set_eventid(eventid)
             if m["deviceID"] and m["callID"]:
                 m["deviceID"] = user.deviceID
-                m["callID"] = user.callID
+                if callID:
+                    m["callID"] = callID
+                    user.callID = callID
+                else:
+                    m["callID"] = user.callID
             user.update_outgoing_transactions(m)
+            user.update_call_id(m)
         # old_link = self.link
         # try:
         self.link.send(m.contents())
         # except IOError:
         #     while old_link is self.link:
         #         sleep(0.1)
         #     debug("Retransmitting {} after disconnection and reconnection".format(m.event))
         #     self.link.send(m.contents())
 
         return m
 
-    def wait_for_csta_message(self, for_user, message, ignore_messages=(), timeout=5.0):
+    def wait_for_csta_message(self, for_user, message, calling_device=None, ignore_messages=(), timeout=5.0):
         """
         Wait for CSTA message
         :param for_user: The message intended recipient
         :param message: The message to wait for
+        :param calling_device: The calling device number. Used to separated csta events when necessary
         :param ignore_messages: Messages to ignore
         :param timeout: Defined timeout in seconds.
         :return: the CstaMessage received
         """
-        inmessage = None
+        callID = None
         # other_users_xrefid = [usr.parameters["monitorCrossRefID"]
         #                       if "monitorCrossRefID" in usr.parameters else None
         #                       for usr in self.users.values() if usr != for_user]
         # other_users_transactions = [usr.out_transactions for usr in self.users.values() if usr != for_user]
         user_xrefid = None
         this_user = None
         net_object = self
         if for_user is not None:
             this_user = self.users[for_user]
-            user_xrefid = this_user.parameters.get("monitorCrossRefID", None)
+            # We are not using the below line, because if the same user is used, the xref id will be global
+            # not thread specific
+            # user_xrefid = this_user.parameters.get("monitorCrossRefID", None)
+            user_xrefid = this_user.monitorCrossRefID
             net_object = this_user
-
+            callID = this_user.parameters["callID"]
         # checked_buffer = None
         t0_tout = time()
-        inmessage = get_buffered_message(net_object.message_buffer, message)
+        with net_object.lock:
+            inmessage = get_buffered_message(net_object.message_buffer, message, callID, user_xrefid, calling_device)
         while not inmessage:
             # if not checked_buffer == net_object.buffer_mod_time:
             #     checked_buffer = net_object.buffer_mod_time
             if self.server:
                 continue
 
-#            if not inmessage:
+            #            if not inmessage:
             rem_timeout = timeout - (time() - t0_tout)
             if rem_timeout > 0:
                 net_object.buffer_event.wait(rem_timeout)
                 net_object.buffer_event.clear()
                 with net_object.lock:
-                    inmessage = get_buffered_message(net_object.message_buffer, message)
+                    inmessage = get_buffered_message(net_object.message_buffer, message, callID, user_xrefid,
+                                                     calling_device)
                     if inmessage is None:
                         continue
             else:
-                exception(str(for_user) + " No " + str(message) + " " + str(net_object.message_buffer))
+                exception("%s (CSTA) No %s. Buffer lengths: %s. " % (for_user,
+                                                                     message,
+                                                                     str([(k, len(net_object.message_buffer[k]))
+                                                                          for k in net_object.message_buffer])))
                 raise sock_timeout
 
                 # try:
                 #     inbytes = self.link.waitForCstaData(timeout=timeout)
                 #     inmessage = parseBytes(inbytes)
 
                 # except UnicodeDecodeError:
@@ -280,32 +328,39 @@
                 continue
 
             if message and (
                     # received message is not of expected type or
                     (isinstance(message, str) and message != inmessage_type) or
 
                     # received message type is not in list of expected types or
-                    (type(message) in (list, tuple) and not any([m == inmessage_type for m in message]))  # or
+                    (type(message) in (list, tuple) and not any([m == inmessage_type for m in message])) or
+
+                    # received message is event and has an unexpected callID
+                    (inmessage.is_event() and
+                     this_user is not None and
+                     inmessage["callID"] and
+                     callID and
+                     callID != inmessage["callID"])  # or
 
                     # received message is a csta response that has an unknown/incorrect invokeID (eventid)
                     # (this_user is not None and
                     #  inmessage.is_response() and
                     #  inmessage.eventid not in this_user.out_transactions) or
 
                     # received message type is for another user (different xref_id and not MonitorStartResponse)
                     # # ie we are expecting message for a specific user
                     # (this_user is not None and
-                     # # the message has a xrefid tag and our user has an xrefid parameter (although it may be empty)
-                     # inmessage["monitorCrossRefID"] and user_xrefid is not None and
-                     # # # the message xrefid is different than our user's xrefid
-                     # inmessage["monitorCrossRefID"] != user_xrefid and
-                     # # the message is not a MonitorStartResponse. This is the normal case where we send MonitorStart
-                     # # at which time the user will not have xrefid assigned yet and we expect a response that we will
-                     # # use to assign xrefid to the user
-                     # inmessage_type != "MonitorStartResponse")
+                    # # the message has a xrefid tag and our user has an xrefid parameter (although it may be empty)
+                    # inmessage["monitorCrossRefID"] and user_xrefid is not None and
+                    # # # the message xrefid is different than our user's xrefid
+                    # inmessage["monitorCrossRefID"] != user_xrefid and
+                    # # the message is not a MonitorStartResponse. This is the normal case where we send MonitorStart
+                    # # at which time the user will not have xrefid assigned yet and we expect a response that we will
+                    # # use to assign xrefid to the user
+                    # inmessage_type != "MonitorStartResponse")
             ):
 
                 # buffer received message if it is intended for another user or if it is an event that came sooner
                 # than expected or if it is a response to a request from another user
                 if (
                         # (this_user is not None and
                         #  inmessage["monitorCrossRefID"] and user_xrefid and
@@ -314,82 +369,87 @@
 
                         (inmessage.is_event() and
                          inmessage["monitorCrossRefID"] and user_xrefid and
                          inmessage["monitorCrossRefID"] == user_xrefid) or
 
                         (inmessage.is_event() and
                          inmessage["monitorCrossRefID"] and
-                         user_xrefid is None)  # or
+                         user_xrefid is None) or
+
+                        (inmessage.is_event() and
+                         inmessage["callID"] in this_user.calls)
 
                         # (this_user is not None and
                         #  inmessage.is_response() and
                         #  {inmessage.eventid: inmessage_type.replace("Response", "")} in other_users_transactions)
                 ):
-                    # with net_object.lock:
-                    with self.lock:
+                    with net_object.lock:
+                    # with self.lock:
                         # trying global lock to buffer messages
-                        self.buffer_message(inmessage, ntfy_subs=False)
-                    # debug(
-                    #     "BUFFERED MESSAGE '{}' with xrefid '{}' for '{}' because I am '{}' waiting for '{}' in '{}'".format(
+                        self.buffer_message(net_object, inmessage, ntfy_subs=False)
+                    # warning(
+                    #     "BUFFERED MESSAGE '{}' with callID '{}' for '{}' because I am '{}' waiting for '{}' in '{}' '{}'".format(
                     #         inmessage_type,
-                    #         inmessage["monitorCrossRefID"],
+                    #         inmessage["callID"],
                     #         inmessage["deviceID"], for_user, message,
-                    #         this_user.parameters["monitorCrossRefID"]))
+                    #         this_user.monitorCrossRefID, this_user.callID))
                     inmessage = None
                 else:
                     if this_user is None:
                         raise AssertionError('Got "{}" with callID {} and xrefid {} '
                                              'while expecting "{}"'.format(inmessage_type,
                                                                            inmessage["callID"],
                                                                            inmessage["monitorCrossRefID"],
                                                                            message))
                     else:
-                        raise AssertionError('Got "{}" with callID {}, eventid {} and xrefid {} while expecting "{}" with '
-                                             'callID {} and xrefid {}. '
-                                             'Known transactions are:\n"{}"\n{} '.format(inmessage_type,
-                                                                                         inmessage["callID"],
-                                                                                         inmessage.eventid,
-                                                                                         inmessage["monitorCrossRefID"],
-                                                                                         message,
-                                                                                         this_user.parameters.get(
-                                                                                             "callID",
-                                                                                             None),
-                                                                                         this_user.parameters.get(
-                                                                                             "monitorCrossRefID",
-                                                                                             None),
-                                                                                         this_user.out_transactions,
-                                                                                         inmessage))
+                        raise AssertionError(
+                            'Got "{}" with callID {}, eventid {} and xrefid {} while expecting "{}" with '
+                            'callID {} and xrefid {}. '
+                            'Known transactions are:\n"{}"\n{} '.format(inmessage_type,
+                                                                        inmessage["callID"],
+                                                                        inmessage.eventid,
+                                                                        inmessage["monitorCrossRefID"],
+                                                                        message,
+                                                                        this_user.parameters.get(
+                                                                            "callID",
+                                                                            None),
+                                                                        this_user.parameters.get(
+                                                                            "monitorCrossRefID",
+                                                                            None),
+                                                                        this_user.out_transactions,
+                                                                        inmessage))
         if this_user is not None:
             # Evaluate the invoke id
             this_user.update_incoming_transactions(inmessage)
-            this_user.update_connection_id(inmessage)
+            this_user.update_call_id(inmessage)
 
         return inmessage
 
-    def buffer_message(self, message, ntfy_subs=True):
+    def buffer_message(self, user, message, ntfy_subs=True):
         """
         Add csta message to csta user's or csta application's buffer.
         :param message: the message to buffer
         :param ntfy_subs: notify the user whose buffer was changed
+        :param user: the user who's buffer to use
         :return: None
         """
-        net_object = self
-        for dn in self.users:
-            user = self.users[dn]
-            if (message.is_event() and user.parameters["monitorCrossRefID"] == message["monitorCrossRefID"]) or \
-               (message.is_response() and message.eventid in user.out_transactions):
-                net_object = user
-                break
-        if net_object is self:
+        if user is self:
             warning("Unexpected message. Adding to global buffer: " + str(message))
 
-        net_object.message_buffer.append(message)
-        net_object.buffer_mod_time = time()
+        key = str(message["callID"]) + str(message["monitorCrossRefID"]) + str(message.event)
+        if key in user.message_buffer:
+            user.message_buffer[key].append(message)
+        else:
+            user.message_buffer[key] = [message]
+        user.buffer_mod_time = time()
         if ntfy_subs:
-            net_object.buffer_event.set()
+            self.buffer_trigger_count += 1
+        if self.buffer_trigger_count:
+            user.buffer_event.set()
+            self.buffer_trigger_count -= 1
 
     def update_call_parameters(self, directory_number, inresponse):
         """ Update our parameters based on the given incoming CSTA message """
         try:
             if not inresponse.event.endswith("Event") and not inresponse.event.endswith("Response"):
                 self.parameters[directory_number]["last_request_eventid"] = inresponse.eventid
             for key in "deviceID", "monitorCrossRefID", "callID":
```

### Comparing `pyssimist-0.2.0/csta/CstaEndpoint.py` & `pyssimist-0.2.1/csta/CstaEndpoint.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaFlows.py` & `pyssimist-0.2.1/csta/CstaFlows.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaMessage.py` & `pyssimist-0.2.1/csta/CstaMessage.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaPool/ConnectionClearedEvent.xml` & `pyssimist-0.2.1/csta/CstaPool/ConnectionClearedEvent.xml`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaPool/DeliveredEvent.xml` & `pyssimist-0.2.1/csta/CstaPool/DeliveredEvent.xml`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaPool/EstablishedEvent.xml` & `pyssimist-0.2.1/csta/CstaPool/EstablishedEvent.xml`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaPool/MakeCall.xml` & `pyssimist-0.2.1/csta/CstaPool/MakeCall.xml`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaPool/OriginatedEvent.xml` & `pyssimist-0.2.1/csta/CstaPool/OriginatedEvent.xml`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaPool/ServiceInitiatedEvent.xml` & `pyssimist-0.2.1/csta/CstaPool/ServiceInitiatedEvent.xml`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/csta/CstaUser.py` & `pyssimist-0.2.1/csta/CstaUser.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 class CstaUser:
     def __init__(self, number, csta_application):
         self.number = number
         self.busy = False
         self.csta_application = csta_application
         self.monitorCrossRefID = None
         self.callID = None
+        self.calls = []  # store multiple callIDs
         # Transactions are a dictionary of eventid to request eg {353: "MakeCall"}
         self.inc_transactions = {}
         self.out_transactions = {}
         self.deviceID = number
-        self.message_buffer = []
+        self.message_buffer = {}
         self.buffer_event = Event()
         self.buffer_mod_time = None
         self.lock = Lock()
         self.parameters = {"monitorCrossRefID": self.monitorCrossRefID,
                            "CSTA_CREATE_MONITOR_CROSS_REF_ID": self.monitorCrossRefID,
                            "CSTA_USE_MONITOR_CROSS_REF_ID": self.monitorCrossRefID,
                            "callID": self.callID,
@@ -91,18 +92,21 @@
                                                                                   message.eventid,
                                                                                   self.inc_transactions[message.eventid]))
             self.inc_transactions[message.eventid] = message.event
             self.csta_application.min_event_id = max(self.csta_application.min_event_id, message.eventid + 1)
         else:
             assert message.is_event(), "Message {} is not a response, request or event".format(message.event)
 
-    def update_connection_id(self, message):
-        if message["deviceID"] and message["callID"]:
-            self.callID = message["callID"]
-            self.set_parameter("callID", self.callID)
+    def update_call_id(self, message):
+        callID = message["callID"]
+        if message["deviceID"] and callID:
+            self.callID = callID
+            if callID not in self.calls:
+                self.calls.append(callID)
+            self.set_parameter("callID", callID)
 
     def monitor_start(self):
         return self.csta_application.monitor_start(self.number)
 
     def set_parameter(self, key, value):
         self.parameters[key] = value
 
@@ -111,26 +115,28 @@
         Convert a SIP message string to SipMessage object
 
         :param message: The message string
         :return: A CstaMessage object
         """
         return self.csta_application.prepare_message(self.number, message)
 
-    def send(self, message, to_user=None):
-        return self.csta_application.send(message, from_user=self.number, to_user=to_user)
+    def send(self, message, to_user=None, callID=None):
+        return self.csta_application.send(message, from_user=self.number, to_user=to_user, callID=callID)
 
-    def wait_for_message(self, message, ignore_messages=(), timeout=5.0):
+    def wait_for_message(self, message, calling_device=None, ignore_messages=(), timeout=5.0):
         return self.csta_application.wait_for_csta_message(self.number,
                                                            message,
+                                                           calling_device=calling_device,
                                                            ignore_messages=ignore_messages,
                                                            timeout=timeout)
 
     def reset(self):
         with self.lock:
             buffer = self.message_buffer
-            self.message_buffer = []
+            self.message_buffer = {}
             self.busy = False
             self.callID = None
+            self.calls = []
             self.inc_transactions = {}
             self.out_transactions = {}
             self.buffer_mod_time = None
         return buffer
```

### Comparing `pyssimist-0.2.0/pyssimist.egg-info/SOURCES.txt` & `pyssimist-0.2.1/pyssimist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/sip/SipEndpoint.py` & `pyssimist-0.2.1/sip/SipEndpoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """\
 Purpose: Simulate a SIP phone/line appearance/user
 Initial Version: Costas Skarakis
 """
-from threading import Timer
+from threading import Timer, Event
 
-from common.tc_logging import exception
+from _socket import timeout as sock_timeout
+import traceback
+from common.tc_logging import exception, warning
 from sip.SipParser import parseBytes, buildMessage
 import common.util as util
 import common.client as client
 import sip.SipFlows as flow
-from threading import Lock
+from threading import Lock, Thread
 from sip.SipMessage import SipMessage
+from time import time, sleep
 
 
 def dialog_hash(dialog):
     return "|".join([dialog["Call-ID"], dialog["from_tag"], dialog["to_tag"]])
 
 
 class SipEndpoint(object):
@@ -32,15 +35,16 @@
         self.number = directory_number
         self.parameters = {"user": directory_number,
                            "callId": None,
                            "fromTag": None,
                            "viaBranch": None,
                            "epid": None,
                            "expires": 360,
-                           "cseq": None
+                           "cseq": "0",
+                           "method": None
                            }
         self.last_messages_per_dialog = []
         self.dialogs = []
         self.requests = []
         self.current_dialog = {
             "Call-ID": None,
             "from_tag": None,
@@ -52,19 +56,31 @@
                                     "cseq": "0",
                                     "method": None
                                     }
 
         self.waitForMessage = self.wait_for_message  # compatibility alias
         self.reply_to = self.send_in_ctx_of  # method alias
         self.secondary_lines = []
-        self.message_buffer = []
+        self.message_buffer = set()
+        self.buffer_event = Event()
+        # self.buffer_mod_count = [0]  # using a int in a list to be able to share and muate between objects in use_link()
         self.registered = False
         self.re_register_timer = None
         self.busy = False
         self.lock = Lock()
+        self.wait_thread = None
+        self.shutdown_flag = False
+
+    def shutdown(self):
+        """
+        Try to stop threads and cleanup connections
+        """
+        self.shutdown_flag = True
+        self.link.shutdown()
+        self.wait_thread.join()
 
     def make_busy(self, busy=True):
         self.busy = busy
 
     def update_parameters(self, params, force=False):
         """
         Update endpoint parameters. This is useful for adding more flexibility in the creation of SIP messages
@@ -93,14 +109,46 @@
             # for MTLS this might be needed
             # context.load_cert_chain('/path/to/certchain.pem', '/path/to/private.key')
             self.link = client.TLSClient(local_ip, local_port, certificate)
         else:
             raise NotImplementedError("{} client not implemented".format(protocol))
         self.link.connect(dest_ip, dest_port)
         self.set_address((local_ip, self.link.port))
+        self.start_wait_thread()
+
+    def start_wait_thread(self):
+        """
+        Starts a separate thread that will consume incoming csta traffic and place it into buffers
+        """
+        if self.wait_thread is None:
+            self.wait_thread = Thread(target=self.wait_loop)
+            self.wait_thread.start()
+
+    def wait_loop(self):
+        """
+        Continuously wait for incoming sip messages. Add all messages to buffers
+        """
+        while not self.shutdown_flag:
+            try:
+                inbytes = self.link.waitForSipData(timeout=None)
+                # inbytes = self.link.waitForSipData(timeout=timeout, client=link)
+            except ConnectionError:
+                # might need to add what kind of disconnection that was
+                warning("Disconnected. Exiting")
+                break
+            if inbytes is None:
+                warning("Disconnected. Will retry in 1 second")
+                sleep(1)
+            else:
+                inmessage = parseBytes(inbytes)
+                try:
+                    self.message_buffer.add(inmessage)
+                    self.buffer_event.set()
+                except:
+                    exception(traceback.format_exc())
 
     def update_to_tag(self, in_dialog):
         """
         Update the to_tag on an existing dialog that has no to_tag
         :param in_dialog: the complete dialog
         :return: None
         """
@@ -140,16 +188,28 @@
         """
         local_ip, local_port = address
         self.ip = local_ip
         self.port = local_port
         self.parameters["source_ip"] = local_ip
         self.parameters["source_port"] = local_port
 
-    def use_link(self, link):
-        """ Convenience function to use an existing network connection"""
+    def use_link(self, other):
+        """ Convenience function to use an existing network connection
+        If parameter is SipEndpoint, we will use also share a common message buffer and dialog tracking
+        """
+        if isinstance(other, SipEndpoint):
+            link = other.link
+            self.message_buffer = other.message_buffer
+            self.dialogs = other.dialogs
+            self.requests = other.requests
+            self.last_messages_per_dialog = other.last_messages_per_dialog
+            self.buffer_event = other.buffer_event
+            self.wait_thread = other.wait_thread
+        else:
+            link = other
         protocol = ["TCP", "UDP"][link.socket.proto]
         local_ip = link.ip
         local_port = link.port
         dest_ip = link.rip
         dest_port = link.rport
         self.link = link
         self.ip = local_ip
@@ -157,73 +217,119 @@
         self.parameters["source_ip"] = local_ip
         self.parameters["source_port"] = local_port
         self.parameters["dest_ip"] = dest_ip
         self.parameters["dest_port"] = dest_port
         self.parameters["transport"] = protocol
         # self.link.endpoints_connected += 1
 
+    def get_dialog(self):
+        """ Will use this method to get thread-local dialogs """
+        return {"Call-ID": self.parameters["callId"],
+                "from_tag": self.parameters["fromTag"],
+                "to_tag": self.parameters["toTag"]}
+
+    def get_transaction(self):
+        """ Will use this method to get thread-local transactions """
+        return {"via_branch": self.parameters["viaBranch"],
+                "cseq": self.parameters["cseq"],
+                "method": self.parameters["method"]}
+
     def set_dialog(self, dialog):
         """ Change current dialog to the one provided """
         if not isinstance(dialog, dict):
             exception("Must provide a dialog in the form of Python dictionary")
-        for key in self.current_dialog:
+        for key in self.get_dialog():
             if key not in dialog:
                 exception("Not a valid dialog. Missing key: " + key)
         dialog = self.get_complete_dialog(dialog)
         if dialog not in self.dialogs:
             self.dialogs.append(dialog)
             self.requests.append([])
             # If we don't know this dialog it means we didn't started so it must be an incoming Request
-            self.tags[dialog_hash(dialog)] = "to_tag"
+            with self.lock:
+                self.tags[dialog_hash(dialog)] = "to_tag"
         self.current_dialog = dialog
-        self.parameters["callId"] = self.current_dialog["Call-ID"]
-        self.parameters["fromTag"] = self.current_dialog["from_tag"]
-        self.parameters["toTag"] = self.current_dialog["to_tag"]
+        self.parameters["callId"] = dialog["Call-ID"]
+        self.parameters["fromTag"] = dialog["from_tag"]
+        self.parameters["toTag"] = dialog["to_tag"]
         return dialog
 
+    def reset_dialog_and_transaction(self):
+        """
+        Reset current dialog and transaction to initial state
+        :return: None
+        """
+        self.parameters["viaBranch"] = None
+        self.parameters["epid"] = None
+        self.parameters["cseq"] = "0"
+        self.parameters["method"] = None
+        self.parameters["callId"] = None
+        self.parameters["fromTag"] = None
+        self.parameters["toTag"] = None
+        self.current_dialog = {
+            "Call-ID": None,
+            "from_tag": None,
+            "to_tag": None
+        }
+        self.current_transaction = {"via_branch": None,
+                                    "cseq": "0",
+                                    "method": None
+                                    }
+
     def switch_tags(self, dialog=None):
         if not dialog:
-            dialog = self.current_dialog
+            dialog = self.get_dialog()
         dhash = dialog_hash(dialog)
         dialog["from_tag"], dialog["to_tag"] = dialog["to_tag"], dialog["from_tag"]
         dhash_switched = dialog_hash(dialog)
         self.set_dialog(dialog)
-        if self.tags[dhash] == "to_tag":
-            self.tags[dhash_switched] = "from_tag"
-        else:
-            self.tags[dhash_switched] = "to_tag"
+        with self.lock:
+            if self.tags[dhash] == "to_tag":
+                self.tags[dhash_switched] = "from_tag"
+            else:
+                self.tags[dhash_switched] = "to_tag"
 
     def set_transaction(self, transaction):
         """ Change current transaction to the one provided """
         if not isinstance(transaction, dict):
             exception("Must provide a transaction in the form of Python dictionary")
+            return
         for key in self.current_transaction:
             if key not in transaction:
                 exception("Not a valid transaction. Missing key: " + key)
+                return
         for key in self.current_transaction:
             self.current_transaction[key] = transaction[key]
+        self.parameters["viaBranch"] = transaction["via_branch"]
+        self.parameters["cseq"] = transaction["cseq"]
+        self.parameters["method"] = transaction["method"]
 
     def start_new_dialog(self):
         """ Refresh the SIP dialog specific parameters """
         dialog = {
             "Call-ID": util.randomCallID(),
             "from_tag": util.randomTag(),
             "to_tag": ""
             # "epid": lambda x=6: "SC" + util.randStr(x),
         }
         self.current_dialog = dialog
-        self.tags[dialog_hash(dialog)] = "from_tag"
+        self.parameters["callId"] = dialog["Call-ID"]
+        self.parameters["fromTag"] = dialog["from_tag"]
+        self.parameters["toTag"] = dialog["to_tag"]
+        with self.lock:
+            self.tags[dialog_hash(dialog)] = "from_tag"
         self.dialogs.append(dialog)
         self.requests.append([])
         return dialog
 
     def get_last_message_in(self, dialog):
         """ Get the last message sent or received in the provided dialog """
         # If we have received no messages yet return None
-        if self.current_dialog == {"Call-ID": None, "from_tag": None, "to_tag": None}:
+        null_d = {"Call-ID": None, "from_tag": None, "to_tag": None}
+        if self.current_dialog == null_d or dialog == null_d:
             return None
         with self.lock:
             # First check for complete dialogs
             for message in self.last_messages_per_dialog:
                 if message.get_dialog() == dialog:
                     return message
             # Second check for incomplete dialogs
@@ -251,15 +357,15 @@
         :return: A SipMessage object
         """
         return buildMessage(message, self.parameters)
 
     def start_new_transaction(self, method, dialog=None):
         """ Refresh the via branch and CSeq header """
         if not dialog:
-            dialog = self.current_dialog
+            dialog = self.get_dialog()
         try:
             last_message_in_dialog = self.get_last_message_in(dialog)
         except:
             last_message_in_dialog = None
         branch = util.randomBranch()
         if method in ("ACK", "CANCEL"):
             # Not really a new transaction
@@ -350,15 +456,15 @@
             m = message_string
         else:
             m = buildMessage(message_string, self.parameters)
 
         if dialog:
             dialog = self.set_dialog(dialog)
         else:
-            dialog = self.current_dialog
+            dialog = self.get_dialog()
 
         try:
             previous_message = self.get_last_message_in(dialog)
             m.make_response_to(previous_message)
             self.update_to_tag(m.get_dialog())
         except:  # caused by get_last_message_in(dialog) if no message has been exchanged in this dialog yet
             # New dialog, same call-id, eg NOTIFY after Keyset SUBSCRIBE.
@@ -377,39 +483,47 @@
                     self.tags[dialog_hash(dialog)] == "to_tag":
                 self.switch_tags(dialog)
             m.set_dialog_from(dialog)
         else:
             self.free_resources(m)
         self.save_message(m)
 
-        m.set_transaction_from(self.current_transaction)
+        m.set_transaction_from(self.get_transaction())
         self.link.send(m.contents())
         return m
 
-    def get_buffered_message(self, dialog):
+    def get_buffered_message(self, message_type, dialog):
         """
         Return the first buffered message found in the given dialog
 
+        :param message_type: the requested message type
         :param dialog: The dialog in question
         :return: the buffered SipMessage
         """
         msg = None
         # for message in self.message_buffer:
-        for i in range(len(self.message_buffer)):
-            message = self.message_buffer[i]
-            d = message.get_dialog()
-            # If we have received no messages yet return the first message in the buffer
-            if self.current_dialog == {"Call-ID": None, "from_tag": None, "to_tag": None} or \
-                    (d["Call-ID"] == dialog["Call-ID"] and d["from_tag"] == dialog["from_tag"]):
-                msg = message
-                self.message_buffer.pop(i)
-                break
+        with self.lock:
+            for message in self.message_buffer:
+                m_dialog = message.get_dialog()
+                m_type = message.get_status_or_method()
+                # If we have received no messages yet return the first message in the buffer
+                if m_type == message_type \
+                        and (self.current_dialog["Call-ID"] is None
+                             or dialog["Call-ID"] is None
+                             or m_dialog["Call-ID"] == dialog["Call-ID"]):
+                    msg = message
+                    self.message_buffer.remove(message)
+                    break
+                # else:
+                #     self.message_buffer.append(message)
+        # if msg is None:
+        #     print(self.number, "Buffer returned None for", message_type, "in callid and from_tag", dialog["Call-ID"], dialog["from_tag"], "although it has", self.message_buffer)
         return msg
 
-    def wait_for_message(self, message_type, dialog=None, ignore_messages=(), link=None, timeout=5.0):
+    def wait_for_message(self, message_type, dialog=None, ignore_messages=(), timeout=5.0):
         """
         Wait for a specific type of SIP message.
         :param message_type: is a string that we will make sure is
                              contained in the received message request or response line
                              Set this to None or "" to accept any incoming message
 
                              if a list or tuple is given any of the contained message types
@@ -417,83 +531,113 @@
 
         :param dialog: Set the dialog to expect the message in. If None will expect a message in current dialog
         :param ignore_messages: a list of message_types to ignore if they come before
                                 the expected message_type
         :param timeout: Defined timeout in seconds.
         :return: A SipMessage constructed from the incoming message
         """
-        if not link:
-            link = self.link
+
         if not dialog:
-            dialog = self.current_dialog
+            dialog = {"Call-ID": self.parameters["callId"],
+                      "from_tag": self.parameters["fromTag"]}
+            if "toTag" in self.parameters:
+                dialog["to_tag"] = self.parameters["toTag"]
+
         else:
             dialog = self.get_complete_dialog(dialog)
 
-        inmessage = None
         last_sent_message = self.get_last_message_in(dialog)
+        transaction = None
         if last_sent_message:
             transaction = last_sent_message.get_transaction()
-        len_buffer = len(self.message_buffer)
-        count = 0
 
-        while not inmessage:
+        t0_tout = time()
+        inmessage = self.get_buffered_message(message_type, dialog)
+        inmessage = self.handleDA(last_sent_message, inmessage)
 
-            if count < len_buffer:
-                # first get a message from the buffer
-                inmessage = self.get_buffered_message(dialog)
-                count += 1
-
-            if not inmessage:
-                # no (more) buffered messages. try the network
-                inbytes = self.link.waitForSipData(timeout=timeout, client=link)
-                inmessage = self.handleDA(last_sent_message, parseBytes(inbytes))
+        while not inmessage:
+            rem_timeout = timeout - (time() - t0_tout)
+            if rem_timeout > 0:
+                self.buffer_event.wait(rem_timeout)
+                self.buffer_event.clear()
+                inmessage = self.get_buffered_message(message_type, dialog)
+                inmessage = self.handleDA(last_sent_message, inmessage)
+                if inmessage is None:
+                    continue
+            else:
+                exception("%s No %s. Buffer length: %d." % (self.number,
+                                                            message_type,
+                                                            len(self.message_buffer)))
+                raise sock_timeout
+
+            # if not inmessage:
+            #     # no (more) buffered messages. try the network
+            #     inbytes = self.link.waitForSipData(timeout=timeout, client=link)
+            #     inmessage = self.handleDA(last_sent_message, parseBytes(inbytes))
 
             inmessage_type = inmessage.get_status_or_method()
             inmessage_dialog = inmessage.get_dialog()
             inmessage.cseq_method = inmessage.get_transaction()["method"]
 
+            # when sharing buffers we can get a message of other endpoints
+            # buffer message of correct type but incorrect callid
+            # keep it if we are mentioned in the "To" header
+            if inmessage_type == message_type and \
+                    inmessage_dialog["Call-ID"] != dialog["Call-ID"] and \
+                    "sip:{}@{}".format(self.number, self.ip) not in inmessage["To"]:
+                # print(self.number, "Aborting", inmessage_type, "with callid", inmessage_dialog["Call-ID"])
+                # print(self.number, "My callid is", dialog["Call-ID"])
+
+                self.message_buffer.add(inmessage)
+                self.buffer_event.set()
+                inmessage = None
+                continue
+
             if inmessage_type in ignore_messages:
                 inmessage = None
                 continue
 
             if message_type and \
                     ((isinstance(message_type, str) and message_type not in inmessage_type) or
                      (type(message_type) in (list, tuple) and not any([m in inmessage_type for m in message_type])) or
                      (inmessage.type == "Response" and inmessage.cseq_method != transaction["method"])):
                 # we have received an unexpected message. buffer it if there is an active dialog for it
-                if inmessage_dialog in self.dialogs or inmessage_type == "INVITE":
+                if self.get_complete_dialog(inmessage_dialog) or inmessage_type == "INVITE":
                     # message is part of another active dialog or a new call, so buffer it
-                    self.message_buffer.append(inmessage)
+                    # print(self.number, "Aborting", inmessage_type, "with callid", inmessage_dialog["Call-ID"])
+                    self.message_buffer.add(inmessage)
+                    self.buffer_event.set()
                     # print("Appended {} with {} to buffer. Will keep waiting for {} in {} ".format(inmessage_type,
                     #                                                                        inmessage_dialog,
                     #                                                                        message_type,
                     #                                                                            dialog))
                     inmessage = None
                 else:
                     d = ["sip:{}@".format(line.number) in inmessage["To"] for line in self.secondary_lines]
                     if any(d):
                         # message is meant for another line in this device
-                        self.secondary_lines[d.index(True)].message_buffer.append(inmessage)
+                        self.secondary_lines[d.index(True)].message_buffer.add(inmessage)
                         inmessage = None
                     else:
                         raise AssertionError('{}: Got "{}" in {} while expecting "{}" in {}. '
                                              'Other active dialogs:{}.'.format(self.number,
                                                                                inmessage_type,
                                                                                inmessage_dialog,
                                                                                message_type,
                                                                                dialog,
                                                                                self.dialogs))
 
         self.save_message(inmessage)
         if inmessage.type == "Request":
-            self.set_transaction(inmessage.get_transaction())
+            inmessage_transaction = inmessage.get_transaction()
+            self.set_transaction(inmessage_transaction)
         else:
-            assert inmessage.cseq_method == transaction["method"], \
+            assert inmessage.get_transaction()["method"] == transaction["method"], \
                 "Got {} to {} instead of {} to {}".format(inmessage.get_status_or_method(),
-                                                          inmessage.cseq_method,
+                                                          inmessage.get_transaction()["method"],
                                                           message_type,
                                                           transaction["method"])
             self.update_to_tag(inmessage.get_dialog())
             self.free_resources(inmessage)
         self.set_dialog(inmessage.get_dialog())
         return inmessage
 
@@ -541,14 +685,16 @@
             "da_user": username,
             "da_pass": password,
             "realm": realm
         })
 
     def handleDA(self, request, response):
         """" Add DA to message and send again """
+        if response is None:
+            return
         # Usual case in lab, password same as username
         if "da_pass" not in self.parameters or "da_user" not in self.parameters:
             self.set_digest_credentials(self.number, self.number, "")
         user, pwd = self.parameters["da_user"], self.parameters["da_pass"]
         if response.type == "Response" and response.status == "401 Unauthorized":
             request.addAuthorization(response["WWW-Authenticate"], user, pwd)
             self.link.send(request.contents())
@@ -561,14 +707,15 @@
         """ Convenience function to register a SipEndpoint """
         if not expiration_in_seconds:
             return self.unregister()
         if re_register_time and self.registered:
             self.re_register_timer = Timer(re_register_time, self.register, (expiration_in_seconds, re_register_time))
             self.re_register_timer.start()
         flow.register(self, expiration_in_seconds)
+        self.reset_dialog_and_transaction()
         self.registered = True
 
     def unregister(self):
         """ Convenience function to un-register a SipEndpoint"""
         if self.re_register_timer:
             self.re_register_timer.cancel()
         flow.unregister(self)
```

### Comparing `pyssimist-0.2.0/sip/SipFlows.py` & `pyssimist-0.2.1/sip/SipFlows.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/sip/SipMessage.py` & `pyssimist-0.2.1/sip/SipMessage.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,30 +51,33 @@
             if M:
                 self.from_tag = M.group(1)
         if "Via" in self.header:
             M = re.search(r"branch=([^;]+)", self.header["Via"])
             if M:
                 self.via_branch = M.group(1)
 
-    def __eq__(self, message_or_method_or_status):
+    def __hash__(self):
+        return hash(repr(self))
+
+    def __eq__(self, other):
         """
-        Override equality operator to return comparison only based on the method or status string
+        Override equality operator to return comparison based on string comparison
 
-        :param message_or_method_or_status: The method or status string in the request line of the message
+        :param other: The other string message or SipMessage to compare against
         :return: True or False
         """
-        if isinstance(message_or_method_or_status, str):
-            other_status_or_method = message_or_method_or_status
-        elif isinstance(message_or_method_or_status, SipMessage):
-            other_status_or_method = message_or_method_or_status.get_status_or_method()
+        if isinstance(other, str):
+            other_contents = other
+        elif isinstance(other, SipMessage):
+            other_contents = repr(other)
         else:
             raise Exception("Can only compare SipMessage to str or SipMessage, "
-                            "not {}".format(type(message_or_method_or_status)))
+                            "not {}".format(type(other)))
 
-        return self.get_status_or_method() == other_status_or_method
+        return repr(self) == other_contents
 
     def __getitem__(self, key):
         for k in self.header:
             # handle different letter case
             if k.upper() == key.upper():
                 return self.header[k]
         raise KeyError("%s not in message headers" % key)
```

### Comparing `pyssimist-0.2.0/sip/SipParser.py` & `pyssimist-0.2.1/sip/SipParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,9 +155,10 @@
           '\n'
     ackm = buildMessage(ack, {})
     print(ackm.contents())
     byem = buildMessage(bye, {})
     print(byem.contents())
     byem.make_response_to(ackm)
     print(byem.contents())
+    print(hash(byem))
```

### Comparing `pyssimist-0.2.0/sip/messages.py` & `pyssimist-0.2.1/sip/messages.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/tshark_tools/analyze_gui.py` & `pyssimist-0.2.1/tshark_tools/analyze_gui.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/tshark_tools/check_trace.py` & `pyssimist-0.2.1/tshark_tools/check_trace.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/tshark_tools/describe.py` & `pyssimist-0.2.1/tshark_tools/describe.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/tshark_tools/diff.py` & `pyssimist-0.2.1/tshark_tools/diff.py`

 * *Files identical despite different names*

### Comparing `pyssimist-0.2.0/tshark_tools/lib.py` & `pyssimist-0.2.1/tshark_tools/lib.py`

 * *Files identical despite different names*

