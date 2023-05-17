# Comparing `tmp/opengsq-1.5.0.tar.gz` & `tmp/opengsq-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengsq-1.5.0.tar", last modified: Wed Mar 15 23:44:45 2023, max compression
+gzip compressed data, was "opengsq-1.5.1.tar", last modified: Sat Mar 18 22:29:27 2023, max compression
```

## Comparing `opengsq-1.5.0.tar` & `opengsq-1.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:44:45.891113 opengsq-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-15 23:44:35.000000 opengsq-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-03-15 23:44:45.891113 opengsq-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-03-15 23:44:35.000000 opengsq-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:44:45.887113 opengsq-1.5.0/opengsq/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/binary_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocol_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:44:45.891113 opengsq-1.5.0/opengsq/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/battlefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/doom3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/gamespy1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/gamespy2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/gamespy3.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/gamespy4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/quake1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/quake2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/quake3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/raknet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/samp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/satisfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/teamspeak3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/vcmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/protocols/won.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/socket_async.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-15 23:44:35.000000 opengsq-1.5.0/opengsq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:44:45.887113 opengsq-1.5.0/opengsq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-03-15 23:44:45.000000 opengsq-1.5.0/opengsq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-15 23:44:45.000000 opengsq-1.5.0/opengsq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 23:44:45.000000 opengsq-1.5.0/opengsq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-15 23:44:45.000000 opengsq-1.5.0/opengsq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 23:44:45.000000 opengsq-1.5.0/opengsq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-15 23:44:45.891113 opengsq-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-15 23:44:35.000000 opengsq-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:29:27.448399 opengsq-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-18 22:29:15.000000 opengsq-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-03-18 22:29:27.448399 opengsq-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-03-18 22:29:15.000000 opengsq-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:29:27.444398 opengsq-1.5.1/opengsq/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/binary_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocol_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:29:27.448399 opengsq-1.5.1/opengsq/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/battlefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/doom3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/gamespy1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/gamespy2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/gamespy3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/gamespy4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/quake1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/quake2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/raknet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/samp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/satisfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/teamspeak3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/vcmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/protocols/won.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/socket_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-18 22:29:15.000000 opengsq-1.5.1/opengsq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 22:29:27.444398 opengsq-1.5.1/opengsq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-03-18 22:29:27.000000 opengsq-1.5.1/opengsq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-18 22:29:27.000000 opengsq-1.5.1/opengsq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 22:29:27.000000 opengsq-1.5.1/opengsq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-18 22:29:27.000000 opengsq-1.5.1/opengsq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-18 22:29:27.000000 opengsq-1.5.1/opengsq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-18 22:29:27.448399 opengsq-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-18 22:29:15.000000 opengsq-1.5.1/setup.py
```

### Comparing `opengsq-1.5.0/LICENSE` & `opengsq-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/PKG-INFO` & `opengsq-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengsq
-Version: 1.5.0
+Version: 1.5.1
 Summary: 🐍 OpenGSQ - Python library for querying game servers
 Home-page: https://github.com/opengsq/opengsq-python
 Author: OpenGSQ
 License: MIT
 Project-URL: Bug Tracker, https://github.com/opengsq/opengsq-python/issues
 Project-URL: Source Code, https://github.com/opengsq/opengsq-python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opengsq-1.5.0/README.md` & `opengsq-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/binary_reader.py` & `opengsq-1.5.1/opengsq/binary_reader.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/cli.py` & `opengsq-1.5.1/opengsq/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                     sub.add_argument('--function', default=method_names[0], type=str, help='(default: %(default)s)')
                     sub.add_argument('--indent', default=None, type=int, nargs='?')
 
     # Get the query response in json format
     async def run(self, args: Sequence[str]) -> str:
         # Return version if -V or --version
         if args.version:
-            return __version__
+            return 'v' + __version__
         else:
             del args.version
 
         # Load the obj from path
         obj = locate(self.__paths[args.subparser_name])
         del args.subparser_name
```

### Comparing `opengsq-1.5.0/opengsq/protocols/__init__.py` & `opengsq-1.5.1/opengsq/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/ase.py` & `opengsq-1.5.1/opengsq/protocols/ase.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/battlefield.py` & `opengsq-1.5.1/opengsq/protocols/battlefield.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/doom3.py` & `opengsq-1.5.1/opengsq/protocols/doom3.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/gamespy1.py` & `opengsq-1.5.1/opengsq/protocols/gamespy1.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
             value = br.read_string(b'\\')
             kv[key] = value.strip()
 
         return kv
 
     def __parse_as_object(self, br: BinaryReader, is_player=False):
-        items, keyhashes, filters = [], [], []
+        items, keyhashes, filters = {}, [], []
 
         while br.length() > 0:
             # Get the key, for example player_1, frags_1, ping_1, etc...
             key = br.read_string(b'\\').lower()
 
             if is_player and key.startswith('teamname_'):
                 # Read already, so add it back
@@ -159,30 +159,31 @@
             # Some servers (bf1942) report the same player multiple times, so filter it by keyhash
             if name == 'keyhash':
                 if value in keyhashes:
                     filters.append(index)
                 else:
                     keyhashes.append(value)
 
-            # Append a dict to items if next index appears
-            if len(items) <= index:
-                items.append({})
+            # Create a dict on items if next index appears
+            if index not in items:
+                items[index] = {}
 
             # Save
             items[index][name] = value
 
         # Filter items by filters
-        return [item for i, item in enumerate(items) if i not in filters]
+        return [v for k, v in items.items() if k not in filters]
 
 
 if __name__ == '__main__':
     import asyncio
     import json
 
     async def main_async():
         gs1 = GameSpy1(address='51.81.48.224', query_port=23000, timeout=5.0)  # bfield1942
         #gs1 = GameSpy1(address='139.162.235.20', query_port=7778, timeout=5.0)  # ut
         #gs1 = GameSpy1(address='192.223.24.6', query_port=7778, timeout=5.0)  # ut
+        gs1 = GameSpy1(address='141.94.205.35', query_port=12300, timeout=5.0)  # mohaa
         status = await gs1.get_status()
         print(json.dumps(status, indent=None) + '\n')
 
     asyncio.run(main_async())
```

### Comparing `opengsq-1.5.0/opengsq/protocols/gamespy2.py` & `opengsq-1.5.1/opengsq/protocols/gamespy2.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/gamespy3.py` & `opengsq-1.5.1/opengsq/protocols/gamespy3.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/minecraft.py` & `opengsq-1.5.1/opengsq/protocols/minecraft.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/quake1.py` & `opengsq-1.5.1/opengsq/protocols/quake1.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/quake2.py` & `opengsq-1.5.1/opengsq/protocols/quake2.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/quake3.py` & `opengsq-1.5.1/opengsq/protocols/quake3.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/raknet.py` & `opengsq-1.5.1/opengsq/protocols/raknet.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/samp.py` & `opengsq-1.5.1/opengsq/protocols/samp.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/satisfactory.py` & `opengsq-1.5.1/opengsq/protocols/satisfactory.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/source.py` & `opengsq-1.5.1/opengsq/protocols/source.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/teamspeak3.py` & `opengsq-1.5.1/opengsq/protocols/teamspeak3.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/unreal2.py` & `opengsq-1.5.1/opengsq/protocols/unreal2.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/vcmp.py` & `opengsq-1.5.1/opengsq/protocols/vcmp.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/protocols/won.py` & `opengsq-1.5.1/opengsq/protocols/won.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq/socket_async.py` & `opengsq-1.5.1/opengsq/socket_async.py`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/opengsq.egg-info/PKG-INFO` & `opengsq-1.5.1/opengsq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengsq
-Version: 1.5.0
+Version: 1.5.1
 Summary: 🐍 OpenGSQ - Python library for querying game servers
 Home-page: https://github.com/opengsq/opengsq-python
 Author: OpenGSQ
 License: MIT
 Project-URL: Bug Tracker, https://github.com/opengsq/opengsq-python/issues
 Project-URL: Source Code, https://github.com/opengsq/opengsq-python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opengsq-1.5.0/opengsq.egg-info/SOURCES.txt` & `opengsq-1.5.1/opengsq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengsq-1.5.0/setup.py` & `opengsq-1.5.1/setup.py`

 * *Files identical despite different names*

