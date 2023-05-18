# Comparing `tmp/aioconnectors-1.6.2.tar.gz` & `tmp/aioconnectors-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioconnectors-1.6.2.tar", last modified: Sat May 13 06:05:42 2023, max compression
+gzip compressed data, was "aioconnectors-1.6.3.tar", last modified: Thu May 18 17:29:40 2023, max compression
```

## Comparing `aioconnectors-1.6.2.tar` & `aioconnectors-1.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-05-13 06:05:42.596231 aioconnectors-1.6.2/
--rw-r--r--   0 mm        (1000) mm        (1000)    11357 2020-06-11 21:16:01.000000 aioconnectors-1.6.2/LICENSE
--rw-rw-r--   0 mm        (1000) mm        (1000)    67137 2023-05-13 06:05:42.596231 aioconnectors-1.6.2/PKG-INFO
--rw-rw-r--   0 mm        (1000) mm        (1000)    66485 2023-05-13 06:03:20.000000 aioconnectors-1.6.2/README.md
-drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-05-13 06:05:42.592231 aioconnectors-1.6.2/aioconnectors/
--rw-rw-r--   0 mm        (1000) mm        (1000)     1950 2023-05-13 06:03:20.000000 aioconnectors-1.6.2/aioconnectors/__init__.py
--rw-rw-r--   0 mm        (1000) mm        (1000)    13030 2023-05-13 06:03:20.000000 aioconnectors-1.6.2/aioconnectors/__main__.py
--rw-rw-r--   0 mm        (1000) mm        (1000)    65878 2023-05-13 06:03:20.000000 aioconnectors-1.6.2/aioconnectors/api.py
--rw-rw-r--   0 mm        (1000) mm        (1000)    53057 2023-03-05 21:23:45.000000 aioconnectors-1.6.2/aioconnectors/applications.py
--rw-rw-r--   0 mm        (1000) mm        (1000)   100549 2022-09-09 15:58:05.000000 aioconnectors-1.6.2/aioconnectors/connection.py
--rw-rw-r--   0 mm        (1000) mm        (1000)   135021 2022-11-02 04:23:50.000000 aioconnectors-1.6.2/aioconnectors/core.py
--rw-rw-r--   0 mm        (1000) mm        (1000)     5078 2023-05-13 06:03:20.000000 aioconnectors-1.6.2/aioconnectors/helpers.py
--rw-rw-r--   0 mm        (1000) mm        (1000)    33740 2023-03-05 21:29:30.000000 aioconnectors-1.6.2/aioconnectors/ssl_helper.py
-drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-05-13 06:05:42.592231 aioconnectors-1.6.2/aioconnectors.egg-info/
--rw-rw-r--   0 mm        (1000) mm        (1000)    67137 2023-05-13 06:05:42.000000 aioconnectors-1.6.2/aioconnectors.egg-info/PKG-INFO
--rw-rw-r--   0 mm        (1000) mm        (1000)      380 2023-05-13 06:05:42.000000 aioconnectors-1.6.2/aioconnectors.egg-info/SOURCES.txt
--rw-rw-r--   0 mm        (1000) mm        (1000)        1 2023-05-13 06:05:42.000000 aioconnectors-1.6.2/aioconnectors.egg-info/dependency_links.txt
--rw-rw-r--   0 mm        (1000) mm        (1000)       14 2023-05-13 06:05:42.000000 aioconnectors-1.6.2/aioconnectors.egg-info/top_level.txt
--rw-rw-r--   0 mm        (1000) mm        (1000)       38 2023-05-13 06:05:42.596231 aioconnectors-1.6.2/setup.cfg
--rw-rw-r--   0 mm        (1000) mm        (1000)     6788 2023-05-13 06:03:20.000000 aioconnectors-1.6.2/setup.py
+drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-05-18 17:29:40.806884 aioconnectors-1.6.3/
+-rw-r--r--   0 mm        (1000) mm        (1000)    11357 2020-06-11 21:16:01.000000 aioconnectors-1.6.3/LICENSE
+-rw-rw-r--   0 mm        (1000) mm        (1000)    67343 2023-05-18 17:29:40.806884 aioconnectors-1.6.3/PKG-INFO
+-rw-rw-r--   0 mm        (1000) mm        (1000)    66691 2023-05-18 17:29:18.000000 aioconnectors-1.6.3/README.md
+drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-05-18 17:29:40.802884 aioconnectors-1.6.3/aioconnectors/
+-rw-rw-r--   0 mm        (1000) mm        (1000)     1950 2023-05-18 16:47:20.000000 aioconnectors-1.6.3/aioconnectors/__init__.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)    13030 2023-05-13 06:03:20.000000 aioconnectors-1.6.3/aioconnectors/__main__.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)    66101 2023-05-18 17:18:31.000000 aioconnectors-1.6.3/aioconnectors/api.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)    53097 2023-05-18 17:20:14.000000 aioconnectors-1.6.3/aioconnectors/applications.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)   100565 2023-05-18 16:48:21.000000 aioconnectors-1.6.3/aioconnectors/connection.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)   135107 2023-05-18 16:51:03.000000 aioconnectors-1.6.3/aioconnectors/core.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)     5399 2023-05-18 17:08:12.000000 aioconnectors-1.6.3/aioconnectors/helpers.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)    33740 2023-03-05 21:29:30.000000 aioconnectors-1.6.3/aioconnectors/ssl_helper.py
+drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-05-18 17:29:40.802884 aioconnectors-1.6.3/aioconnectors.egg-info/
+-rw-rw-r--   0 mm        (1000) mm        (1000)    67343 2023-05-18 17:29:40.000000 aioconnectors-1.6.3/aioconnectors.egg-info/PKG-INFO
+-rw-rw-r--   0 mm        (1000) mm        (1000)      380 2023-05-18 17:29:40.000000 aioconnectors-1.6.3/aioconnectors.egg-info/SOURCES.txt
+-rw-rw-r--   0 mm        (1000) mm        (1000)        1 2023-05-18 17:29:40.000000 aioconnectors-1.6.3/aioconnectors.egg-info/dependency_links.txt
+-rw-rw-r--   0 mm        (1000) mm        (1000)       14 2023-05-18 17:29:40.000000 aioconnectors-1.6.3/aioconnectors.egg-info/top_level.txt
+-rw-rw-r--   0 mm        (1000) mm        (1000)       38 2023-05-18 17:29:40.806884 aioconnectors-1.6.3/setup.cfg
+-rw-rw-r--   0 mm        (1000) mm        (1000)     6788 2023-05-18 16:43:09.000000 aioconnectors-1.6.3/setup.py
```

### Comparing `aioconnectors-1.6.2/LICENSE` & `aioconnectors-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioconnectors-1.6.2/PKG-INFO` & `aioconnectors-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioconnectors
-Version: 1.6.2
+Version: 1.6.3
 Summary: Simple secure asynchronous message queue
 Home-page: https://github.com/mori-b/aioconnectors
 Author: Mori Benech
 Author-email: moribirom@gmail.com
 License: UNKNOWN
 Keywords: message queue,broker,asyncio,simple,easy
 Platform: UNKNOWN
@@ -768,14 +768,15 @@
 -**request\_id** and **response\_id** are optional (integer or string) : they are helpful to keep track of asynchronous messages on the application layer. At the application level, the remote peer should answer with response\_id equal to the request\_id of the request. The request sender can then associate the received response with the request sent.  
 -The **publish\_message** and **publish\_message\_sync** methods are the same as the send_message ones, but used by a client in the publish/subscribe approach.  
 -The **send\_message\_await\_response** method is the same as send_message, but automatically sets await_response to True.  
 -The **send\_message\_sync** method is almost the same as send_message, but called synchronously (not an async coroutine). It can also receive a "loop" as a kwarg. If a loop is running in the background, it schedules and returns a task. Otherwise it returns the peer response if called with await\_response.  
 -**wait\_for\_ack** is not recommended for high throughputs, since it slows down dramatically. Basic testing showed a rate of ten messages per second, instead of a few thousands messages per second in the point to point approach.  
 Not a benchmark, but some point-to-point and pubsub trials (VM with 8GB RAM and 4 cores) showed that up until 4000 messages (with data of 100 bytes) per second could be received by a server without delay, and from that point the receive queue started to be non empty. This test gave the same result with 100 clients sending each 40 events per second, and with 1 client sending 4000 events per second.  
 -**with\_file** lets you embed a file, with {'src\_path':'','dst\_type':'', 'dst\_name':'', 'delete':False, 'owner':''}. **src\_path** is the source path of the file to be sent, **dst\_type** is the type of the file, which enables the remote peer to evaluate the destination path thanks to its ConnectorManager attribute "file\_recv\_config" dictionary. **dst\_name** is the name the file will be stored under. **delete** is a boolean telling if to delete the source file after it has been sent. **owner** is the optional user:group of your uploaded file : if used, it overrides the "owner" value optionally set on server side in file\_recv\_config. If an error occurs while opening the file to send, the file will not be sent but with\_file will still be present in transport\_json received by peer, and will contain an additional key **file\_error** telling the error to the peer application.  
+-**tag** lets you add a tag string to your message in transport\_json : it has the advantage of being accessible at reception directly in transport\_json without the need to look into the data structure.  
 
 
 <a name="management"></a>
 ### 6.Management programmatic tools
 
 The class ConnectorManager has several methods to manage your connector. These methods are explained in <a href="#cli">7-</a>.  
 -**delete\_client\_certificate**, **delete\_client\_token**, **disconnect\_client**, **reload\_tokens**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioconnectors Version: 1.6.2 Summary: Simple secure
+Metadata-Version: 2.1 Name: aioconnectors Version: 1.6.3 Summary: Simple secure
 asynchronous message queue Home-page: https://github.com/mori-b/aioconnectors
 Author: Mori Benech Author-email: moribirom@gmail.com License: UNKNOWN
 Keywords: message queue,broker,asyncio,simple,easy Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-
@@ -711,28 +711,31 @@
 "file\_recv\_config" dictionary. **dst\_name** is the name the file will be
 stored under. **delete** is a boolean telling if to delete the source file
 after it has been sent. **owner** is the optional user:group of your uploaded
 file : if used, it overrides the "owner" value optionally set on server side in
 file\_recv\_config. If an error occurs while opening the file to send, the file
 will not be sent but with\_file will still be present in transport\_json
 received by peer, and will contain an additional key **file\_error** telling
-the error to the peer application.  ### 6.Management programmatic tools The
-class ConnectorManager has several methods to manage your connector. These
-methods are explained in 7-. -**delete\_client\_certificate**,
-**delete\_client\_token**, **disconnect\_client**, **reload\_tokens** -
-**add\_blacklist_client, remove\_blacklist_client**, **add\_whitelist_client,
-remove\_whitelist_client** -**delete\_previous\_persistence\_remains** -
-**ignore\_peer\_traffic\_show**, **ignore\_peer\_traffic\_enable**,
-**ignore\_peer\_traffic\_enable\_unique**, **ignore\_peer\_traffic\_disable** -
-**show\_connected\_peers** -**show\_log\_level**, **set\_log\_level** -
-**show\_subscribe\_message\_types**, **set\_subscribe\_message\_types** -
-**start\_connector**, **stop\_connector**, **restart\_connector** The same
-methods can be executed remotely, with the ConnectorRemoteTool class. This
-class is instantiated exactly like ConnectorAPI, with the same arguments
-(except for receive_from_any_connector_owner) connector_remote_tool =
+the error to the peer application. -**tag** lets you add a tag string to your
+message in transport\_json : it has the advantage of being accessible at
+reception directly in transport\_json without the need to look into the data
+structure.  ### 6.Management programmatic tools The class ConnectorManager has
+several methods to manage your connector. These methods are explained in 7-. -
+**delete\_client\_certificate**, **delete\_client\_token**,
+**disconnect\_client**, **reload\_tokens** -**add\_blacklist_client,
+remove\_blacklist_client**, **add\_whitelist_client, remove\_whitelist_client**
+-**delete\_previous\_persistence\_remains** -**ignore\_peer\_traffic\_show**,
+**ignore\_peer\_traffic\_enable**, **ignore\_peer\_traffic\_enable\_unique**,
+**ignore\_peer\_traffic\_disable** -**show\_connected\_peers** -
+**show\_log\_level**, **set\_log\_level** -**show\_subscribe\_message\_types**,
+**set\_subscribe\_message\_types** -**start\_connector**, **stop\_connector**,
+**restart\_connector** The same methods can be executed remotely, with the
+ConnectorRemoteTool class. This class is instantiated exactly like
+ConnectorAPI, with the same arguments (except for
+receive_from_any_connector_owner) connector_remote_tool =
 aioconnectors.ConnectorRemoteTool(config_file_path=config_file_path) An example
 of ConnectorRemoteTool is available in applications.py in the cli
 implementation.  ### 7.Other management command line tools python3 -
 m aioconnectors cli to run several interesting commands like : -**start/stop/
 restart** your connectors. -**show\_connected\_peers** : show currently
 connected peers. -**delete\_client\_certificate** enables your server to delete
 a specific client certificate. delete\_client\_certificate enables your client
```

### Comparing `aioconnectors-1.6.2/README.md` & `aioconnectors-1.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -749,14 +749,15 @@
 -**request\_id** and **response\_id** are optional (integer or string) : they are helpful to keep track of asynchronous messages on the application layer. At the application level, the remote peer should answer with response\_id equal to the request\_id of the request. The request sender can then associate the received response with the request sent.  
 -The **publish\_message** and **publish\_message\_sync** methods are the same as the send_message ones, but used by a client in the publish/subscribe approach.  
 -The **send\_message\_await\_response** method is the same as send_message, but automatically sets await_response to True.  
 -The **send\_message\_sync** method is almost the same as send_message, but called synchronously (not an async coroutine). It can also receive a "loop" as a kwarg. If a loop is running in the background, it schedules and returns a task. Otherwise it returns the peer response if called with await\_response.  
 -**wait\_for\_ack** is not recommended for high throughputs, since it slows down dramatically. Basic testing showed a rate of ten messages per second, instead of a few thousands messages per second in the point to point approach.  
 Not a benchmark, but some point-to-point and pubsub trials (VM with 8GB RAM and 4 cores) showed that up until 4000 messages (with data of 100 bytes) per second could be received by a server without delay, and from that point the receive queue started to be non empty. This test gave the same result with 100 clients sending each 40 events per second, and with 1 client sending 4000 events per second.  
 -**with\_file** lets you embed a file, with {'src\_path':'','dst\_type':'', 'dst\_name':'', 'delete':False, 'owner':''}. **src\_path** is the source path of the file to be sent, **dst\_type** is the type of the file, which enables the remote peer to evaluate the destination path thanks to its ConnectorManager attribute "file\_recv\_config" dictionary. **dst\_name** is the name the file will be stored under. **delete** is a boolean telling if to delete the source file after it has been sent. **owner** is the optional user:group of your uploaded file : if used, it overrides the "owner" value optionally set on server side in file\_recv\_config. If an error occurs while opening the file to send, the file will not be sent but with\_file will still be present in transport\_json received by peer, and will contain an additional key **file\_error** telling the error to the peer application.  
+-**tag** lets you add a tag string to your message in transport\_json : it has the advantage of being accessible at reception directly in transport\_json without the need to look into the data structure.  
 
 
 <a name="management"></a>
 ### 6.Management programmatic tools
 
 The class ConnectorManager has several methods to manage your connector. These methods are explained in <a href="#cli">7-</a>.  
 -**delete\_client\_certificate**, **delete\_client\_token**, **disconnect\_client**, **reload\_tokens**
```

#### html2text {}

```diff
@@ -703,28 +703,31 @@
 "file\_recv\_config" dictionary. **dst\_name** is the name the file will be
 stored under. **delete** is a boolean telling if to delete the source file
 after it has been sent. **owner** is the optional user:group of your uploaded
 file : if used, it overrides the "owner" value optionally set on server side in
 file\_recv\_config. If an error occurs while opening the file to send, the file
 will not be sent but with\_file will still be present in transport\_json
 received by peer, and will contain an additional key **file\_error** telling
-the error to the peer application.  ### 6.Management programmatic tools The
-class ConnectorManager has several methods to manage your connector. These
-methods are explained in 7-. -**delete\_client\_certificate**,
-**delete\_client\_token**, **disconnect\_client**, **reload\_tokens** -
-**add\_blacklist_client, remove\_blacklist_client**, **add\_whitelist_client,
-remove\_whitelist_client** -**delete\_previous\_persistence\_remains** -
-**ignore\_peer\_traffic\_show**, **ignore\_peer\_traffic\_enable**,
-**ignore\_peer\_traffic\_enable\_unique**, **ignore\_peer\_traffic\_disable** -
-**show\_connected\_peers** -**show\_log\_level**, **set\_log\_level** -
-**show\_subscribe\_message\_types**, **set\_subscribe\_message\_types** -
-**start\_connector**, **stop\_connector**, **restart\_connector** The same
-methods can be executed remotely, with the ConnectorRemoteTool class. This
-class is instantiated exactly like ConnectorAPI, with the same arguments
-(except for receive_from_any_connector_owner) connector_remote_tool =
+the error to the peer application. -**tag** lets you add a tag string to your
+message in transport\_json : it has the advantage of being accessible at
+reception directly in transport\_json without the need to look into the data
+structure.  ### 6.Management programmatic tools The class ConnectorManager has
+several methods to manage your connector. These methods are explained in 7-. -
+**delete\_client\_certificate**, **delete\_client\_token**,
+**disconnect\_client**, **reload\_tokens** -**add\_blacklist_client,
+remove\_blacklist_client**, **add\_whitelist_client, remove\_whitelist_client**
+-**delete\_previous\_persistence\_remains** -**ignore\_peer\_traffic\_show**,
+**ignore\_peer\_traffic\_enable**, **ignore\_peer\_traffic\_enable\_unique**,
+**ignore\_peer\_traffic\_disable** -**show\_connected\_peers** -
+**show\_log\_level**, **set\_log\_level** -**show\_subscribe\_message\_types**,
+**set\_subscribe\_message\_types** -**start\_connector**, **stop\_connector**,
+**restart\_connector** The same methods can be executed remotely, with the
+ConnectorRemoteTool class. This class is instantiated exactly like
+ConnectorAPI, with the same arguments (except for
+receive_from_any_connector_owner) connector_remote_tool =
 aioconnectors.ConnectorRemoteTool(config_file_path=config_file_path) An example
 of ConnectorRemoteTool is available in applications.py in the cli
 implementation.  ### 7.Other management command line tools python3 -
 m aioconnectors cli to run several interesting commands like : -**start/stop/
 restart** your connectors. -**show\_connected\_peers** : show currently
 connected peers. -**delete\_client\_certificate** enables your server to delete
 a specific client certificate. delete\_client\_certificate enables your client
```

### Comparing `aioconnectors-1.6.2/aioconnectors/__init__.py` & `aioconnectors-1.6.3/aioconnectors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,14 @@
 - Embeds a command line interface, which can manage the broker through the command line
 - Embeds an encrypted chat/file transfer tool easily callable through the command line
 
 The command line tool can be called by "python3 -m aioconnectors --help"
 Usage examples can be found in applications.py
 '''
 
-__version__ = '1.6.2'
+__version__ = '1.6.3'
 __author__ = 'Mori Benech'
 
 from .api import ConnectorManager, ConnectorAPI, ConnectorRemoteTool
 from .connection import MessageFields
 from .helpers import get_logger, iface_to_ip, get_tmp_dir
 from . import applications
```

### Comparing `aioconnectors-1.6.2/aioconnectors/__main__.py` & `aioconnectors-1.6.3/aioconnectors/__main__.py`

 * *Files identical despite different names*

### Comparing `aioconnectors-1.6.2/aioconnectors/api.py` & `aioconnectors-1.6.3/aioconnectors/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import asyncio
 import json
 from functools import partial
 import uuid
 import ipaddress
 
-from .helpers import get_logger, chown_nobody_permissions, PYTHON_GREATER_37
+from .helpers import get_logger, chown_nobody_permissions, PYTHON_GREATER_37,\
+                                    DEFAULT_LOGGER_NAME, LOGFILE_DEFAULT_NAME, LOG_LEVEL,\
+                                    LOG_ROTATE, LOG_BK_COUNT, validate_tag
 from .core import Connector
 from .connection import Structures, MessageFields, Misc
 
-from .helpers import DEFAULT_LOGGER_NAME, LOGFILE_DEFAULT_NAME, LOG_LEVEL, LOG_ROTATE, LOG_BK_COUNT
 
 class ConnectorManager:
     def __init__(self, config_file_path=None, config_file_overrides_kwargs=True, logger=None, use_default_logger=True, 
                  default_logger_log_level=LOG_LEVEL, default_logger_rotate=LOG_ROTATE,
                  default_logger_bk_count=LOG_BK_COUNT,
                  default_logger_dirpath=Connector.CONNECTOR_FILES_DIRPATH, use_token=Connector.USE_TOKEN,
                  is_server=True, server_sockaddr=None, use_ssl=Connector.USE_SSL, ssl_allow_all=Connector.SSL_ALLOW_ALL, 
@@ -481,41 +482,41 @@
         super().__init__(*args, **kwargs)
         self.max_size_chunk_upload = max_size_chunk_upload
         self.send_message_lock = asyncio.Lock()
         self.receive_from_any_connector_owner = receive_from_any_connector_owner
         
     async def send_message_await_response(self, message_type=None, destination_id=None, request_id=None, response_id=None,
                            data=None, data_is_json=True, binary=None, await_response=False, with_file=None,
-                           wait_for_ack=False, message_type_publish=None, await_response_timeout=None):
+                           wait_for_ack=False, message_type_publish=None, await_response_timeout=None, tag=None):
         res = await self.send_message(await_response=True, message_type=message_type, destination_id=destination_id, 
                                       request_id=request_id, response_id=response_id, data=data, 
                                       data_is_json=data_is_json, binary=binary, with_file=with_file, 
                                       wait_for_ack=wait_for_ack, message_type_publish=message_type_publish,
-                                      await_response_timeout=await_response_timeout)
+                                      await_response_timeout=await_response_timeout, tag=tag)
         return res
 
     def send_message_sync(self, message_type=None, destination_id=None, request_id=None, response_id=None,
-                           data=None, data_is_json=True, binary=None, await_response=False, with_file=None, 
+                           data=None, data_is_json=True, binary=None, await_response=False, with_file=None, tag=None,
                            wait_for_ack=False, message_type_publish=None, await_response_timeout=None, loop=None):
         self.logger.debug(f'send_message_sync of type {message_type}, destination_id {destination_id}, '
                           f'request_id {request_id}, response_id {response_id}')
         
         loop = loop or asyncio.get_event_loop()
         send_task = self.send_message(message_type=message_type, destination_id=destination_id, 
                                       request_id=request_id, response_id=response_id, data=data, 
                                       data_is_json=data_is_json, binary=binary, await_response=await_response, 
-                                      with_file=with_file, wait_for_ack=wait_for_ack,
+                                      with_file=with_file, wait_for_ack=wait_for_ack, tag=tag,
                                       message_type_publish=message_type_publish, await_response_timeout=await_response_timeout)
         if loop.is_running():
             return loop.create_task(send_task)
         else:
             return loop.run_until_complete(send_task)
     
     async def send_message(self, message_type=None, destination_id=None, request_id=None, response_id=None,
-                           data=None, data_is_json=True, binary=None, await_response=False, with_file=None, 
+                           data=None, data_is_json=True, binary=None, await_response=False, with_file=None,  tag=None,
                            wait_for_ack=False, message_type_publish=None, await_response_timeout=None, check_chunk_file=True):
 
         if with_file:
             src_path = with_file.get('src_path')
             if src_path and check_chunk_file:
                 file_size = os.path.getsize(src_path)
                 number_of_chunks, last_bytes_size = divmod(file_size, self.max_size_chunk_upload)
@@ -554,15 +555,15 @@
                         chunk_name_path = os.path.join(chunk_basepath, chunk_name)                        
                         with_file['src_path'] = chunk_name_path
                         with_file['dst_name'] = chunk_name
                         with_file['chunked'] = [chunk_basename, index+1, len_override_src_file_sizes]
                         res = await self.send_message(message_type=message_type, destination_id=destination_id,
                                                       request_id=request_id, response_id=response_id,
                                                       data=data, data_is_json=data_is_json, binary=binary,
-                                                      await_response=await_response, with_file=with_file, 
+                                                      await_response=await_response, with_file=with_file, tag=tag,
                                                       wait_for_ack=wait_for_ack, message_type_publish=message_type_publish,
                                                       await_response_timeout=await_response_timeout, check_chunk_file=False)
                         if os.path.exists(chunk_name_path):
                             if await_response or wait_for_ack:
                                 try:
                                     self.logger.info(f'send_message of type {message_type}, destination_id {destination_id}, '
                                   f'request_id {request_id}, response_id {response_id} deleting chunk {chunk_name_path}')
@@ -584,17 +585,19 @@
             if data_is_json:
                 data = json.dumps(data) #, ensure_ascii=False)
             if not self.is_server and not destination_id:
                 destination_id = str(self.server_sockaddr)
             self.logger.debug(f'send_message of type {message_type}, destination_id {destination_id}, '
                               f'request_id {request_id}, response_id {response_id}')
                 
+            if tag:
+                validate_tag(tag)
             message_bytes = self.connector.pack_message(data=data, message_type=message_type, source_id=self.source_id,
                                    destination_id=destination_id, request_id=request_id, response_id=response_id, 
-                                   binary=binary, await_response=await_response, with_file=with_file, 
+                                   binary=binary, await_response=await_response, with_file=with_file, tag=tag,
                                    wait_for_ack=wait_for_ack, message_type_publish=message_type_publish)
 
             send_message_lock_internally_acquired = False
             if self.uds_path_send_preserve_socket and not await_response:
                 #try to reuse connection to uds
                 if not self.reader_writer_uds_path_send:     
                     #either there is really no reader_writer_uds_path_send, or the send_message_lock is currently 
@@ -721,27 +724,27 @@
             self.logger.warning('ConnectionResetError : '+str(exc))
         except Exception:
             self.logger.exception('send_data')
             return False
 
     async def publish_message(self, message_type=None, destination_id=None, request_id=None, response_id=None,
                            data=None, data_is_json=True, binary=None, await_response=False, with_file=None, 
-                           wait_for_ack=False):
+                           wait_for_ack=False, tag=None):
         res = await self.send_message(message_type='_pubsub', message_type_publish=message_type, destination_id=destination_id, 
                                       request_id=request_id, response_id=response_id, data=data, 
                                       data_is_json=data_is_json, binary=binary, await_response=await_response,
-                                      with_file=with_file, wait_for_ack=wait_for_ack)
+                                      with_file=with_file, wait_for_ack=wait_for_ack, tag=tag)
         return res
     
     def publish_message_sync(self, message_type=None, destination_id=None, request_id=None, response_id=None,
-                           data=None, data_is_json=True, binary=None, await_response=False, with_file=None, wait_for_ack=False):
+                           data=None, data_is_json=True, binary=None, await_response=False, with_file=None, wait_for_ack=False, tag=None):
         res = self.send_message_sync(message_type='_pubsub', message_type_publish=message_type,
                                      destination_id=destination_id, request_id=request_id, response_id=response_id,
                                      data=data, data_is_json=data_is_json, binary=binary, await_response=await_response,
-                                     with_file=with_file, wait_for_ack=wait_for_ack)
+                                     with_file=with_file, wait_for_ack=wait_for_ack, tag=tag)
         return res
             
     async def recv_message(self, reader, writer):
         try:
             self.logger.debug('recv_message')
             next_length_bytes = await reader.readexactly(Structures.MSG_4_STRUCT.size)
             next_length = Structures.MSG_4_STRUCT.unpack(next_length_bytes)[0]
```

### Comparing `aioconnectors-1.6.2/aioconnectors/applications.py` & `aioconnectors-1.6.3/aioconnectors/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,30 +496,31 @@
 
 
 def test_send_messages(config_file_path, logger=None):
     if not logger:
         logger = aioconnectors.get_logger(logger_name='test_send_messages', first_run=True)    
     logger.info('Creating connector api with config file '+config_file_path)
     connector_api = aioconnectors.ConnectorAPI(config_file_path=config_file_path)
+    tag = 'tag1'
     destination_id = None
     if connector_api.is_server:
         destination_id = input('\nPlease type the name of your remote client\n')
         
     loop = asyncio.get_event_loop()
     
     async def send_messages(destination_id):
         index = 0
         while True:
             index += 1
             for message_type in connector_api.send_message_types:
                 print(f'SENDING MESSAGE to peer {destination_id or connector_api.server_sockaddr} of type '
-                      f'{message_type} and index {index}')
+                      f'{message_type} and index {index} and tag {tag}')
                 response = await connector_api.send_message(data=f'"TEST_MESSAGE {str(index)*5}"', data_is_json=False,
                                                                                   destination_id=destination_id,
-                                                        message_type=message_type, await_response=False, request_id=index)
+                                                        message_type=message_type, await_response=False, request_id=index, tag=tag)
                                                         #response_id=None, binary=b'\x01\x02\x03\x04\x05', with_file=None, wait_for_ack=False)        
             await asyncio.sleep(2)
                     
     task_send = loop.create_task(send_messages(destination_id))
     try:
         loop.run_forever()
     except:
```

### Comparing `aioconnectors-1.6.2/aioconnectors/connection.py` & `aioconnectors-1.6.3/aioconnectors/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     AWAIT_RESPONSE = 'await_response'    #boolean
 #dict {'src_path':<str>, 'dst_name':<str>, 'dst_type':<str>, 'binary_offset':<int>, 'delete':<boolean>, 'owner':<user>:<group>}    
     WITH_FILE = 'with_file'    
     TRANSPORT_ID = 'transport_id'    #int
     WAIT_FOR_ACK = 'wait_for_ack'    #boolean
     MESSAGE_TYPE_PUBLISH = 'message_type_publish'
     ERROR = 'error'
+    TAG = 'tag'
     
 class Structures:
     MSG_4_STRUCT = Struct('I')    #4
     MSG_2_STRUCT = Struct('H')    #2
 #MSG_LENGTH_STRUCT = Struct('Q')    #8
     
 class Misc:
```

### Comparing `aioconnectors-1.6.2/aioconnectors/core.py` & `aioconnectors-1.6.3/aioconnectors/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1407,15 +1407,15 @@
         except Exception:
             self.logger.exception(f'{self.source_id} load_messages_from_persistence')        
         
         
     #4|2|json|4|data|4|binary
     def pack_message(self, transport_json=None, message_type=None, source_id=None, destination_id=None,
                      request_id=None, response_id=None, binary=None, await_response=False,
-                     with_file=None, data=None, wait_for_ack=False, message_type_publish=None):
+                     with_file=None, data=None, wait_for_ack=False, message_type_publish=None, tag=None):
         if DEBUG_SHOW_DATA:
             self.logger.debug('pack_message with params : '+str(message_type)+', '+str(data)+', '+str(transport_json))
         if transport_json is None:
             transport_json = {MessageFields.MESSAGE_TYPE : message_type or self.send_message_types[0]}
             if source_id is not None:
                 transport_json[MessageFields.SOURCE_ID] = source_id
             if destination_id is not None:
@@ -1430,14 +1430,16 @@
                 transport_json[MessageFields.AWAIT_RESPONSE] = True    
             if with_file:
                 transport_json[MessageFields.WITH_FILE] = with_file
             if wait_for_ack:
                 transport_json[MessageFields.WAIT_FOR_ACK] = wait_for_ack
             if message_type_publish:
                 transport_json[MessageFields.MESSAGE_TYPE_PUBLISH] = message_type_publish
+            if tag:
+                transport_json[MessageFields.TAG] = tag
                 
         #pack message
         json_field = json.dumps(transport_json).encode()
         if isinstance(data, str):
             data = data.encode()
         if data is None:
             data = b''
```

### Comparing `aioconnectors-1.6.2/aioconnectors/helpers.py` & `aioconnectors-1.6.3/aioconnectors/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 LOG_FORMAT_SHORT = '%(asctime)s - %(levelname)s - %(message)s'
 LOG_BK_COUNT = 5
 LOG_MAX_SIZE = 67108864 # 2**26 = 64 MB
 
 SOURCE_ID_REGEX = re.compile('^[0-9a-zA-Z-_:]+$')
 SOURCE_ID_DEFAULT_REGEX = re.compile('^default[0-9]*$')
 SOURCE_ID_MAX_LENGTH = 128
+TAG_REGEX = re.compile('^[0-9a-zA-Z-_:]+$')
+TAG_MAX_LENGTH = 128
 
 def full_path(the_path):
     if the_path is not None:
         return os.path.abspath(os.path.normpath(os.path.expandvars(os.path.expanduser(the_path))))
 
 def get_tmp_dir():
     if os.path.exists('/var/tmp'):
@@ -131,10 +133,16 @@
     #if '.' in source_id or '/' in source_id:
         #protect against path traversal
         raise Exception(f'Invalid source_id : {source_id} - please use only {SOURCE_ID_REGEX.pattern}')
     if len(source_id) > SOURCE_ID_MAX_LENGTH:
         raise Exception(f'Invalid source_id : {source_id} - of length {len(source_id)}')        
     if SOURCE_ID_DEFAULT_REGEX.match(source_id):
         raise Exception(f'Invalid source_id : {source_id} - cannot match {SOURCE_ID_DEFAULT_REGEX.pattern}')
+
+def validate_tag(tag):
+    if not TAG_REGEX.match(tag):
+        raise Exception(f'Invalid tag : {tag} - please use only {TAG_REGEX.pattern}')
+    if len(tag) > TAG_MAX_LENGTH:
+        raise Exception(f'Invalid tag : {tag} - of length {len(tag)}')        
         
 class CustomException(Exception):
     pass
```

### Comparing `aioconnectors-1.6.2/aioconnectors/ssl_helper.py` & `aioconnectors-1.6.3/aioconnectors/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `aioconnectors-1.6.2/aioconnectors.egg-info/PKG-INFO` & `aioconnectors-1.6.3/aioconnectors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioconnectors
-Version: 1.6.2
+Version: 1.6.3
 Summary: Simple secure asynchronous message queue
 Home-page: https://github.com/mori-b/aioconnectors
 Author: Mori Benech
 Author-email: moribirom@gmail.com
 License: UNKNOWN
 Keywords: message queue,broker,asyncio,simple,easy
 Platform: UNKNOWN
@@ -768,14 +768,15 @@
 -**request\_id** and **response\_id** are optional (integer or string) : they are helpful to keep track of asynchronous messages on the application layer. At the application level, the remote peer should answer with response\_id equal to the request\_id of the request. The request sender can then associate the received response with the request sent.  
 -The **publish\_message** and **publish\_message\_sync** methods are the same as the send_message ones, but used by a client in the publish/subscribe approach.  
 -The **send\_message\_await\_response** method is the same as send_message, but automatically sets await_response to True.  
 -The **send\_message\_sync** method is almost the same as send_message, but called synchronously (not an async coroutine). It can also receive a "loop" as a kwarg. If a loop is running in the background, it schedules and returns a task. Otherwise it returns the peer response if called with await\_response.  
 -**wait\_for\_ack** is not recommended for high throughputs, since it slows down dramatically. Basic testing showed a rate of ten messages per second, instead of a few thousands messages per second in the point to point approach.  
 Not a benchmark, but some point-to-point and pubsub trials (VM with 8GB RAM and 4 cores) showed that up until 4000 messages (with data of 100 bytes) per second could be received by a server without delay, and from that point the receive queue started to be non empty. This test gave the same result with 100 clients sending each 40 events per second, and with 1 client sending 4000 events per second.  
 -**with\_file** lets you embed a file, with {'src\_path':'','dst\_type':'', 'dst\_name':'', 'delete':False, 'owner':''}. **src\_path** is the source path of the file to be sent, **dst\_type** is the type of the file, which enables the remote peer to evaluate the destination path thanks to its ConnectorManager attribute "file\_recv\_config" dictionary. **dst\_name** is the name the file will be stored under. **delete** is a boolean telling if to delete the source file after it has been sent. **owner** is the optional user:group of your uploaded file : if used, it overrides the "owner" value optionally set on server side in file\_recv\_config. If an error occurs while opening the file to send, the file will not be sent but with\_file will still be present in transport\_json received by peer, and will contain an additional key **file\_error** telling the error to the peer application.  
+-**tag** lets you add a tag string to your message in transport\_json : it has the advantage of being accessible at reception directly in transport\_json without the need to look into the data structure.  
 
 
 <a name="management"></a>
 ### 6.Management programmatic tools
 
 The class ConnectorManager has several methods to manage your connector. These methods are explained in <a href="#cli">7-</a>.  
 -**delete\_client\_certificate**, **delete\_client\_token**, **disconnect\_client**, **reload\_tokens**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioconnectors Version: 1.6.2 Summary: Simple secure
+Metadata-Version: 2.1 Name: aioconnectors Version: 1.6.3 Summary: Simple secure
 asynchronous message queue Home-page: https://github.com/mori-b/aioconnectors
 Author: Mori Benech Author-email: moribirom@gmail.com License: UNKNOWN
 Keywords: message queue,broker,asyncio,simple,easy Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-
@@ -711,28 +711,31 @@
 "file\_recv\_config" dictionary. **dst\_name** is the name the file will be
 stored under. **delete** is a boolean telling if to delete the source file
 after it has been sent. **owner** is the optional user:group of your uploaded
 file : if used, it overrides the "owner" value optionally set on server side in
 file\_recv\_config. If an error occurs while opening the file to send, the file
 will not be sent but with\_file will still be present in transport\_json
 received by peer, and will contain an additional key **file\_error** telling
-the error to the peer application.  ### 6.Management programmatic tools The
-class ConnectorManager has several methods to manage your connector. These
-methods are explained in 7-. -**delete\_client\_certificate**,
-**delete\_client\_token**, **disconnect\_client**, **reload\_tokens** -
-**add\_blacklist_client, remove\_blacklist_client**, **add\_whitelist_client,
-remove\_whitelist_client** -**delete\_previous\_persistence\_remains** -
-**ignore\_peer\_traffic\_show**, **ignore\_peer\_traffic\_enable**,
-**ignore\_peer\_traffic\_enable\_unique**, **ignore\_peer\_traffic\_disable** -
-**show\_connected\_peers** -**show\_log\_level**, **set\_log\_level** -
-**show\_subscribe\_message\_types**, **set\_subscribe\_message\_types** -
-**start\_connector**, **stop\_connector**, **restart\_connector** The same
-methods can be executed remotely, with the ConnectorRemoteTool class. This
-class is instantiated exactly like ConnectorAPI, with the same arguments
-(except for receive_from_any_connector_owner) connector_remote_tool =
+the error to the peer application. -**tag** lets you add a tag string to your
+message in transport\_json : it has the advantage of being accessible at
+reception directly in transport\_json without the need to look into the data
+structure.  ### 6.Management programmatic tools The class ConnectorManager has
+several methods to manage your connector. These methods are explained in 7-. -
+**delete\_client\_certificate**, **delete\_client\_token**,
+**disconnect\_client**, **reload\_tokens** -**add\_blacklist_client,
+remove\_blacklist_client**, **add\_whitelist_client, remove\_whitelist_client**
+-**delete\_previous\_persistence\_remains** -**ignore\_peer\_traffic\_show**,
+**ignore\_peer\_traffic\_enable**, **ignore\_peer\_traffic\_enable\_unique**,
+**ignore\_peer\_traffic\_disable** -**show\_connected\_peers** -
+**show\_log\_level**, **set\_log\_level** -**show\_subscribe\_message\_types**,
+**set\_subscribe\_message\_types** -**start\_connector**, **stop\_connector**,
+**restart\_connector** The same methods can be executed remotely, with the
+ConnectorRemoteTool class. This class is instantiated exactly like
+ConnectorAPI, with the same arguments (except for
+receive_from_any_connector_owner) connector_remote_tool =
 aioconnectors.ConnectorRemoteTool(config_file_path=config_file_path) An example
 of ConnectorRemoteTool is available in applications.py in the cli
 implementation.  ### 7.Other management command line tools python3 -
 m aioconnectors cli to run several interesting commands like : -**start/stop/
 restart** your connectors. -**show\_connected\_peers** : show currently
 connected peers. -**delete\_client\_certificate** enables your server to delete
 a specific client certificate. delete\_client\_certificate enables your client
```

### Comparing `aioconnectors-1.6.2/setup.py` & `aioconnectors-1.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 # To use a consistent encoding
 from codecs import open
 from os import path
 
-VERSION = '1.6.2'
+VERSION = '1.6.3'
 
 here = path.abspath(path.dirname(__file__))
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as fd:
     long_description = fd.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
```

