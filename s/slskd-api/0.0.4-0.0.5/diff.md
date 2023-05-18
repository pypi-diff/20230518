# Comparing `tmp/slskd-api-0.0.4.tar.gz` & `tmp/slskd-api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slskd-api-0.0.4.tar", last modified: Tue May 16 22:02:06 2023, max compression
+gzip compressed data, was "slskd-api-0.0.5.tar", last modified: Thu May 18 21:22:59 2023, max compression
```

## Comparing `slskd-api-0.0.4.tar` & `slskd-api-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:02:06.856621 slskd-api-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-16 22:02:06.856621 slskd-api-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-16 22:01:51.000000 slskd-api-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 22:02:06.856621 slskd-api-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-16 22:01:51.000000 slskd-api-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:02:06.856621 slskd-api-0.0.4/slskd_api/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:02:06.856621 slskd-api-0.0.4/slskd_api/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/conversations.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/rooms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/searches.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/shares.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/apis/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-16 22:01:51.000000 slskd-api-0.0.4/slskd_api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:02:06.856621 slskd-api-0.0.4/slskd_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-16 22:02:06.000000 slskd-api-0.0.4/slskd_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-16 22:02:06.000000 slskd-api-0.0.4/slskd_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:02:06.000000 slskd-api-0.0.4/slskd_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 22:02:06.000000 slskd-api-0.0.4/slskd_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 22:02:06.000000 slskd-api-0.0.4/slskd_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:22:59.288311 slskd-api-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-05-18 21:22:47.000000 slskd-api-0.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-18 21:22:59.288311 slskd-api-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-18 21:22:47.000000 slskd-api-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:22:59.288311 slskd-api-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-18 21:22:47.000000 slskd-api-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:22:59.284311 slskd-api-0.0.5/slskd_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:22:59.288311 slskd-api-0.0.5/slskd_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/conversations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/public_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/shares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/apis/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-18 21:22:47.000000 slskd-api-0.0.5/slskd_api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:22:59.288311 slskd-api-0.0.5/slskd_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-18 21:22:59.000000 slskd-api-0.0.5/slskd_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 21:22:59.000000 slskd-api-0.0.5/slskd_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:22:59.000000 slskd-api-0.0.5/slskd_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 21:22:59.000000 slskd-api-0.0.5/slskd_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 21:22:59.000000 slskd-api-0.0.5/slskd_api.egg-info/top_level.txt
```

### Comparing `slskd-api-0.0.4/PKG-INFO` & `slskd-api-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,13 @@
-Metadata-Version: 2.1
-Name: slskd-api
-Version: 0.0.4
-Summary: API Wrapper to interact with slskd
-Author: bigoulours
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # slskd-api
 
 ## Goal
 This project aims at providing a python API for [slskd](https://github.com/slskd/slskd).
 
-A comprehensive python API could help improve integration and increase slskd adoption by enabling rapid development of various software, like:
+A comprehensive python API could help improve integration and increase slskd adoption by enabling rapid development of various software, such as:
  * Desktop/Mobile Clients
  * [beets](https://github.com/beetbox/beets) plugin(s)
  * [headphones](https://github.com/rembo10/headphones) integration
 
 ## Installation
 The package is availaible on [pypi](https://pypi.org/project/slskd-api/):
 ```
@@ -24,13 +16,13 @@
 
 ## Usage
 Create a `slskd` instance with the following:
 ```
 import slskd_api
 slskd = slskd_api.SlskdClient(host, api_key, url_base)
 ```
-Then you'll be able to access all API methods, like:
+Then you'll be able to access all API methods:
 ```
 app_status = slskd.application.state()
 available_rooms = slskd.rooms.get_all()
 ```
 See the [doc](https://slskd-api.readthedocs.io/) for further details.
```

### Comparing `slskd-api-0.0.4/slskd_api/apis/__init__.py` & `slskd-api-0.0.5/slskd_api/apis/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from .application import ApplicationApi
 from .conversations import ConversationsApi
 from .logs import LogsApi
 from .options import OptionsApi
+from .public_chat import PublicChatApi
+from .relay import RelayApi
 from .rooms import RoomsApi
 from .searches import SearchesApi
 from .server import ServerApi
 from .session import SessionApi
 from .shares import SharesApi
 from .transfers import TransfersApi
 from .users import UsersApi
 
 __all__ = (
     'ApplicationApi',
     'ConversationsApi',
     'LogsApi',
     'OptionsApi',
+    'PublicChatApi',
+    'RelayApi',
     'RoomsApi',
     'SearchesApi',
     'ServerApi',
     'SessionApi',
     'SharesApi',
     'TransfersApi',
     'UsersApi'
```

### Comparing `slskd-api-0.0.4/slskd_api/apis/application.py` & `slskd-api-0.0.5/slskd_api/apis/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,75 @@
 from .base import *
 
 class ApplicationApi(BaseApi):
     """
     This class contains the methods to interact with the Application API.
     """
 
-    def state(self):
+    def state(self) -> dict:
         """
         Gets the current state of the application.
         """
         url = self.api_url + '/application'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def stop(self):
-        """
-        Stops the application.
-        """
-        url = self.api_url + '/application'
-        response = requests.delete(url, headers=self.header)
-        return response.json()
+# Getting Error 'Unauthorized' even with admin API-Key:
+    # def stop(self):
+    #     """
+    #     Stops the application.
+    #     """
+    #     url = self.api_url + '/application'
+    #     response = requests.delete(url, headers=self.header)
+    #     return response.ok
     
 
-    def restart(self):
-        """
-        Restarts the application.
-        """
-        url = self.api_url + '/application'
-        response = requests.put(url, headers=self.header)
-        return response.json()
+# Getting Error 'Unauthorized' even with admin API-Key:
+    # def restart(self):
+    #     """
+    #     Restarts the application.
+    #     """
+    #     url = self.api_url + '/application'
+    #     response = requests.put(url, headers=self.header)
+    #     return response.json()
     
 
-    def version(self):
+    def version(self) -> str:
         """
         Gets the current application version.
         """
         url = self.api_url + '/application/version'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def check_updates(self, forceCheck=False):
+    def check_updates(self, forceCheck: bool = False) -> dict:
         """
         Checks for updates.
         """
         url = self.api_url + '/application/version/latest'
         params = dict(
             forceCheck=forceCheck
         )
         response = requests.get(url, headers=self.header, params=params)
         return response.json()
     
 
-    def gc(self):
+    def gc(self) -> bool:
         """
         Forces garbage collection.
+
+        :return: True if successful.
         """
         url = self.api_url + '/application/gc'
         response = requests.post(url, headers=self.header)
-        return response.json()
+        return response.ok
     
     
-    # def application_dump(self):
+# Getting error 'Could not find file...':
+    # def dump(self):
     #     """
-    #     Returns error 'Could not find file...'
     #     """
     #     url = self.api_url + '/application/dump'
     #     response = requests.get(url, headers=self.header)
     #     return response.json()
```

### Comparing `slskd-api-0.0.4/slskd_api/apis/conversations.py` & `slskd-api-0.0.5/slskd_api/apis/conversations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,84 @@
 from .base import *
 
 class ConversationsApi(BaseApi):
     """
     This class contains the methods to interact with the Conversations API.
     """
 
-    def acknowledge(self, username, id):
+    def acknowledge(self, username: str, id: int) -> bool:
         """
         Acknowledges the given message id for the given username.
+
+        :return: True if successful.
         """
         url = self.api_url + f'/conversations/{username}/{id}'
         response = requests.put(url, headers=self.header)
-        return response.json()
+        return response.ok
     
 
-    def acknowledge_all(self, username):
+    def acknowledge_all(self, username: str) -> bool:
         """
         Acknowledges all messages from the given username.
+
+        :return: True if successful.
         """
         url = self.api_url + f'/conversations/{username}'
         response = requests.put(url, headers=self.header)
-        return response.json()
+        return response.ok
     
 
-    def delete(self, username):
+    def delete(self, username: str) -> bool:
         """
         Closes the conversation associated with the given username.
+
+        :return: True if successful.
         """
         url = self.api_url + f'/conversations/{username}'
         response = requests.delete(url, headers=self.header)
-        return response.json()
+        return response.ok
     
 
-    def get(self, username, includeMessages=True):
+    def get(self, username: str, includeMessages: bool = True) -> dict:
         """
         Gets the conversation associated with the specified username.
         """
         url = self.api_url + f'/conversations/{username}'
         params = dict(
             includeMessages=includeMessages
         )
         response = requests.get(url, headers=self.header, params=params)
         return response.json()
     
 
-    def send(self, username, message):
+    def send(self, username: str, message: str) -> bool:
         """
         Sends a private message to the specified username.
+
+        :return: True if successful.
         """
         url = self.api_url + f'/conversations/{username}'
         response = requests.post(url, headers=self.header, json=message)
-        return response
+        return response.ok
     
 
-    def get_all(self, includeInactive=False, unAcknowledgedOnly=False):
+    def get_all(self, includeInactive: bool = False, unAcknowledgedOnly : bool = False) -> list:
         """
         Gets all active conversations.
         """
         url = self.api_url + '/conversations'
         params = dict(
             includeInactive=includeInactive,
             unAcknowledgedOnly=unAcknowledgedOnly
         )
         response = requests.get(url, headers=self.header, params=params)
         return response.json()
     
 
-    def get_messages(self, username, unAcknowledgedOnly=False):
+    def get_messages(self, username: str, unAcknowledgedOnly : bool = False) -> list:
         """
         Gets all messages associated with the specified username.
         """
         url = self.api_url + f'/conversations/{username}/messages'
         params = dict(
             username=username,
             unAcknowledgedOnly=unAcknowledgedOnly
```

### Comparing `slskd-api-0.0.4/slskd_api/apis/rooms.py` & `slskd-api-0.0.5/slskd_api/apis/users.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,63 @@
 from .base import *
 
-class RoomsApi(BaseApi):
+class UsersApi(BaseApi):
     """
-    This class contains the methods to interact with the Rooms API.
+    This class contains the methods to interact with the Users API.
     """
 
-    def get_all_joined(self):
+    def address(self, username: str) -> dict:
         """
-        Gets all joined rooms.
+        Retrieves the address of the specified username.
         """
-        url = self.api_url + '/rooms/joined'
+        url = self.api_url + f'/users/{username}/endpoint'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def join(self, room):
+    def browse(self, username: str) -> dict:
         """
-        Joins a room.
+        Retrieves the files shared by the specified username.
         """
-        url = self.api_url + '/rooms/joined'
-        response = requests.post(url, headers=self.header, json=room)
-        return response.json()
-
-
-    def get_joined(self, roomName):
-        """
-        Gets the specified room.
-        """
-        url = self.api_url + f'/rooms/joined/{roomName}'
+        url = self.api_url + f'/users/{username}/browse'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def leave(self, roomName):
-        """
-        Leaves a room.
-        """
-        url = self.api_url + f'/rooms/joined/{roomName}'
-        response = requests.delete(url, headers=self.header)
-        return response.ok
-    
-
-    def send(self, roomName, message):
-        """
-        Sends a message to the specified room.
-        """
-        url = self.api_url + f'/rooms/joined/{roomName}/messages'
-        response = requests.post(url, headers=self.header, json=message)
-        return response.ok
-
-
-    def get_messages(self, roomName):
-        """
-        Gets the current list of messages for the specified room.
-        """
-        url = self.api_url + f'/rooms/joined/{roomName}/messages'
-        response = requests.get(url, headers=self.header)
+# Getting Error 404 'Not Found' 
+    # def browsing_status(self, username: str):
+    #     """
+    #     Retrieves the status of the current browse operation for the specified username, if any.
+    #     """
+    #     url = self.api_url + f'/users/{username}/browse/status'
+    #     response = requests.get(url, headers=self.header)
+    #     return response.json()
+    
+
+    def directory(self, username: str, directory: str) -> dict:
+        """
+        Retrieves the files from the specified directory from the specified username.
+        """
+        url = self.api_url + f'/users/{username}/directory'
+        data = {
+            "directory": directory
+        }
+        response = requests.post(url, headers=self.header, json=data)
         return response.json()
-
-
-    def set_tocker(self, roomName, ticker):
-        """
-        Sets a ticker for the specified room.
-        """
-        url = self.api_url + f'/rooms/joined/{roomName}/ticker'
-        response = requests.post(url, headers=self.header, json=ticker)
-        return response.ok
-    
-
-    def add_member(self, roomName, username):
-        """
-        Adds a member to a private room.
-        """
-        url = self.api_url + f'/rooms/joined/{roomName}/members'
-        response = requests.post(url, headers=self.header, json=username)
-        return response.ok
     
 
-    def get_users(self, roomName):
+    def info(self, username: str) -> dict:
         """
-        Gets the current list of users for the specified room.
+        Retrieves information about the specified username.
         """
-        url = self.api_url + f'/rooms/joined/{roomName}/users'
+        url = self.api_url + f'/users/{username}/info'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def get_all(self):
+    def status(self, username: str) -> dict:
         """
-        Gets a list of rooms from the server.
+        Retrieves status for the specified username.
         """
-        url = self.api_url + '/rooms/available'
+        url = self.api_url + f'/users/{username}/status'
         response = requests.get(url, headers=self.header)
         return response.json()
```

### Comparing `slskd-api-0.0.4/slskd_api/apis/server.py` & `slskd-api-0.0.5/slskd_api/apis/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from .base import *
 
 class ServerApi(BaseApi):
     """
     This class contains the methods to interact with the Search API.
     """
 
-    def connect(self):
+    def connect(self) -> bool:
         """
         Connects the client.
+
+        :return: True if successful.
         """
         url = self.api_url + '/server'
         response = requests.put(url, headers=self.header)
         return response.ok
     
 
-    def disconnect(self):
+    def disconnect(self) -> bool:
         """
         Disconnects the client.
+
+        :return: True if successful.
         """
         url = self.api_url + '/server'
         response = requests.delete(url, headers=self.header, json='')
         return response.ok
     
 
-    def state(self):
+    def state(self) -> dict:
         """
         Retrieves the current state of the server.
         """
         url = self.api_url + '/server'
         response = requests.get(url, headers=self.header)
         return response.json()
```

### Comparing `slskd-api-0.0.4/slskd_api/apis/session.py` & `slskd-api-0.0.5/slskd_api/apis/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from .base import *
 
 class SessionApi(BaseApi):
     """
     This class contains the methods to interact with the Server API.
     """
 
-    def auth_valid(self):
+    def auth_valid(self) -> bool:
         """
         Checks whether the provided authentication is valid.
         """
         url = self.api_url + '/session'
         response = requests.get(url, headers=self.header)
         return response.ok
     
 
-    def login(self, username, password):
+    def login(self, username: str, password: str) -> dict:
         """
         Logs in.
+
+        :return: Session info for the given user incl. token.
         """
         url = self.api_url + '/session'
         data = {
             'username': username,
             'password': password
         }
         response = requests.post(url, headers=self.header, json=data)
         return response.json()
     
 
-    def security_enabled(self):
+    def security_enabled(self) -> bool:
         """
         Checks whether security is enabled.
         """
         url = self.api_url + '/session/enabled'
         response = requests.get(url, headers=self.header)
         return response.json()
```

### Comparing `slskd-api-0.0.4/slskd_api/apis/shares.py` & `slskd-api-0.0.5/slskd_api/apis/shares.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 from .base import *
 
 class SharesApi(BaseApi):
     """
     This class contains the methods to interact with the Shares API.
     """
 
-    def get_all(self):
+    def get_all(self) -> dict:
         """
         Gets the current list of shares.
         """
         url = self.api_url + '/shares'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def start_scan(self):
+    def start_scan(self) -> bool:
         """
         Initiates a scan of the configured shares.
+
+        :return: True if successful.
         """
         url = self.api_url + '/shares'
         response = requests.put(url, headers=self.header)
-        return response
+        return response.ok
     
 
-    def cancel_scan(self):
+    def cancel_scan(self) -> bool:
         """
         Cancels a share scan, if one is running.
+
+        :return: True if successful.
         """
         url = self.api_url + '/shares'
         response = requests.delete(url, headers=self.header)
-        return response
+        return response.ok
     
 
-    def get(self, id):
+    def get(self, id: str) -> dict:
         """
         Gets the share associated with the specified id.
         """
         url = self.api_url + f'/shares/{id}'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def get_all_contents(self):
+    def all_contents(self) -> list:
         """
         Returns a list of all shared directories and files.
         """
         url = self.api_url + '/shares/contents'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def get_contents(self, id):
+    def contents(self, id: str) -> list:
         """
         Gets the contents of the share associated with the specified id.
         """
         url = self.api_url + f'/shares/{id}/contents'
         response = requests.get(url, headers=self.header)
         return response.json()
```

### Comparing `slskd-api-0.0.4/slskd_api/apis/transfers.py` & `slskd-api-0.0.5/slskd_api/apis/transfers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,125 +1,142 @@
 from .base import *
+from typing import Union
 
 class TransfersApi(BaseApi):
     """
     This class contains the methods to interact with the Transfers API.
     """
 
-    def cancel_download(self, username, id, remove=False):
+    def cancel_download(self, username: str, id:str, remove: bool = False) -> bool:
         """
         Cancels the specified download.
+
+        :return: True if successful.
         """
         url = self.api_url + f'/transfers/downloads/{username}/{id}'
         params = dict(
             remove=remove
         )
         response = requests.delete(url, headers=self.header, params=params)
         return response.ok
     
 
-    def get_download(self, username, id):
+    def get_download(self, username: str, id: str) -> dict:
         """
         Gets the specified download.
         """
         url = self.api_url + f'/transfers/downloads/{username}/{id}'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def remove_completed_downloads(self):
+    def remove_completed_downloads(self) -> bool:
         """
         Removes all completed downloads, regardless of whether they failed or succeeded.
+
+        :return: True if successful.
         """
         url = self.api_url + '/transfers/downloads/all/completed'
         response = requests.delete(url, headers=self.header)
         return response.ok
     
 
-    def cancel_upload(self, username, id, remove=False):
+    def cancel_upload(self, username: str, id: str, remove: bool = False) -> bool:
         """
         Cancels the specified upload.
+
+        :return: True if successful.
         """
         url = self.api_url + f'/transfers/uploads/{username}/{id}'
         params = dict(
             remove=remove
         )
         response = requests.delete(url, headers=self.header, params=params)
         return response.ok
     
 
-    def get_upload(self, username, id):
+    def get_upload(self, username: str, id: str) -> dict:
         """
         Gets the specified upload.
         """
         url = self.api_url + f'/transfers/uploads/{username}/{id}'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def remove_completed_uploads(self):
+    def remove_completed_uploads(self) -> bool:
         """
         Removes all completed uploads, regardless of whether they failed or succeeded.
+
+        :return: True if successful.
         """
         url = self.api_url + '/transfers/uploads/all/completed'
         response = requests.delete(url, headers=self.header)
         return response.ok
     
 
-    def enqueue(self, username, files):
+    def enqueue(self, username: str, files: list) -> bool:
         """
         Enqueues the specified download.
+
+        :param username: User to download from.
+        :param files: A list of dictionaries in the same form as what's returned 
+            by :py:func:`~slskd_api.apis.SearchesApi.search_responses`:
+            [{'filename': <filename>, 'size': <filesize>}...]
+        :return: True if successful.
         """
         url = self.api_url + f'/transfers/downloads/{username}'
         response = requests.post(url, headers=self.header, json=files)
-        return response.json()
+        return response.ok
     
 
-    def get_downloads(self, username):
+    def get_downloads(self, username: str) -> dict:
         """
         Gets all downloads for the specified username.
         """
         url = self.api_url + f'/transfers/downloads/{username}'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def get_all_downloads(self, includeRemoved=False):
+    def get_all_downloads(self, includeRemoved: bool = False) -> list:
         """
         Gets all downloads.
         """
         url = self.api_url + '/transfers/downloads/'
         params = dict(
             includeRemoved=includeRemoved
         )
         response = requests.get(url, headers=self.header, params=params)
         return response.json()
     
 
-    def get_queue_position(self, username, id):
+    def get_queue_position(self, username: str, id: str) -> Union[int,str]:
         """
         Gets the download for the specified username matching the specified filename, and requests the current place in the remote queue of the specified download.
+        
+        :return: Queue position or error message
         """
         url = self.api_url + f'/transfers/downloads/{username}/{id}/position'
         response = requests.get(url, headers=self.header)
         return response.json()
     
 
-    def get_all_uploads(self, includeRemoved=False):
+    def get_all_uploads(self, includeRemoved: bool = False) -> list:
         """
         Gets all uploads.
         """
         url = self.api_url + '/transfers/uploads/'
         params = dict(
             includeRemoved=includeRemoved
         )
         response = requests.get(url, headers=self.header, params=params)
         return response.json()
     
 
-    def get_uploads(self, username):
+    def get_uploads(self, username: str) -> dict:
         """
         Gets all uploads for the specified username.
         """
         url = self.api_url + f'/transfers/uploads/{username}'
         response = requests.get(url, headers=self.header)
         return response.json()
```

### Comparing `slskd-api-0.0.4/slskd_api/client.py` & `slskd-api-0.0.5/slskd_api/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,52 +11,63 @@
     The main class that allows access to the different APIs of a slskd instance.
     An API-Key with appropriate permissions (`readwrite` for most use cases) must be set in slskd config file.
     Usage::
         slskd = slskd_api.SlskdClient(host, api_key, url_base)
         app_status = slskd.application.state()
     """
 
-    def __init__(self, host, api_key, url_base='/'):
+    def __init__(self,
+                 host: str,
+                 api_key: str,
+                 url_base: str = '/'
+    ):
         api_url = reduce(urljoin, [host, f'{url_base}/', f'api/{API_VERSION}'])
         header = {
             'accept': '*/*',
             'X-API-Key': api_key
         }
         base_args = (api_url, header)
         
         self.application = ApplicationApi(*base_args)
         self.conversations = ConversationsApi(*base_args)
         self.logs = LogsApi(*base_args)
         self.options = OptionsApi(*base_args)
+        self.public_chat = PublicChatApi(*base_args)
+        self.relay = RelayApi(*base_args)
         self.rooms = RoomsApi(*base_args)
         self.searches = SearchesApi(*base_args)
         self.server = ServerApi(*base_args)
         self.session = SessionApi(*base_args)
         self.shares = SharesApi(*base_args)
         self.transfers = TransfersApi(*base_args)
         self.users = UsersApi(*base_args)
     
 
 class MetricsApi:
     """
-    Getting the metrics works with a different end point. Default: <slskd_url>:5030/metrics.
+    Getting the metrics works with a different endpoint. Default: <slskd_url>:5030/metrics.
     Metrics should be first activated in slskd config file.
     User/pass is independent from the main application and default value (slskd:slskd) should be changed.
     Usage::
-        metrics_conn = slskd_api.MetricsApi(host, metrics_usr='slskd', metrics_pwd='slskd')
-        metrics = metrics_conn.get()
+        metrics_api = slskd_api.MetricsApi(host, metrics_usr='slskd', metrics_pwd='slskd')
+        metrics = metrics_api.get()
     """
 
-    def __init__(self, host, metrics_usr=None, metrics_pwd=None, metrics_url_base='/metrics'):
+    def __init__(self,
+                 host: str,
+                 metrics_usr: str = 'slskd',
+                 metrics_pwd: str = 'slskd',
+                 metrics_url_base: str = '/metrics'
+    ):
         self.metrics_url = urljoin(host, metrics_url_base)
         basic_auth = b64encode(bytes(f'{metrics_usr}:{metrics_pwd}', 'utf-8'))
         self.header = {
             'accept': '*/*',
             'Authorization': f'Basic {basic_auth.decode()}' 
         }
 
-    def get(self):
+    def get(self) -> str:
         """
         Gets the Prometheus metrics as text.
         """
         response = requests.get(self.metrics_url, headers=self.header)
         return response.text
```

### Comparing `slskd-api-0.0.4/slskd_api.egg-info/PKG-INFO` & `slskd-api-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: slskd-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: API Wrapper to interact with slskd
 Author: bigoulours
+Project-URL: Documentation, https://slskd-api.readthedocs.io
+Project-URL: Source, https://github.com/bigoulours/slskd-python-api
+Project-URL: Funding, https://liberapay.com/bigoulours/donate
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # slskd-api
 
 ## Goal
 This project aims at providing a python API for [slskd](https://github.com/slskd/slskd).
 
-A comprehensive python API could help improve integration and increase slskd adoption by enabling rapid development of various software, like:
+A comprehensive python API could help improve integration and increase slskd adoption by enabling rapid development of various software, such as:
  * Desktop/Mobile Clients
  * [beets](https://github.com/beetbox/beets) plugin(s)
  * [headphones](https://github.com/rembo10/headphones) integration
 
 ## Installation
 The package is availaible on [pypi](https://pypi.org/project/slskd-api/):
 ```
@@ -24,13 +28,13 @@
 
 ## Usage
 Create a `slskd` instance with the following:
 ```
 import slskd_api
 slskd = slskd_api.SlskdClient(host, api_key, url_base)
 ```
-Then you'll be able to access all API methods, like:
+Then you'll be able to access all API methods:
 ```
 app_status = slskd.application.state()
 available_rooms = slskd.rooms.get_all()
 ```
 See the [doc](https://slskd-api.readthedocs.io/) for further details.
```

### Comparing `slskd-api-0.0.4/slskd_api.egg-info/SOURCES.txt` & `slskd-api-0.0.5/slskd_api.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.py
 slskd_api/__init__.py
 slskd_api/client.py
 slskd_api.egg-info/PKG-INFO
 slskd_api.egg-info/SOURCES.txt
 slskd_api.egg-info/dependency_links.txt
@@ -9,14 +10,16 @@
 slskd_api.egg-info/top_level.txt
 slskd_api/apis/__init__.py
 slskd_api/apis/application.py
 slskd_api/apis/base.py
 slskd_api/apis/conversations.py
 slskd_api/apis/logs.py
 slskd_api/apis/options.py
+slskd_api/apis/public_chat.py
+slskd_api/apis/relay.py
 slskd_api/apis/rooms.py
 slskd_api/apis/searches.py
 slskd_api/apis/server.py
 slskd_api/apis/session.py
 slskd_api/apis/shares.py
 slskd_api/apis/transfers.py
 slskd_api/apis/users.py
```

