# Comparing `tmp/serialization_tool-0.3.tar.gz` & `tmp/serialization_tool-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialization_tool-0.3.tar", last modified: Wed May  3 21:20:36 2023, max compression
+gzip compressed data, was "serialization_tool-0.5.tar", last modified: Thu May 18 08:34:29 2023, max compression
```

## Comparing `serialization_tool-0.3.tar` & `serialization_tool-0.5.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 21:20:36.243926 serialization_tool-0.3/
--rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      313 2023-05-03 21:20:36.244909 serialization_tool-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-0.3/README.md
--rw-rw-rw-   0        0        0      115 2023-05-03 21:20:36.252577 serialization_tool-0.3/setup.cfg
--rw-rw-rw-   0        0        0      423 2023-05-03 21:20:30.000000 serialization_tool-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:20:36.183683 serialization_tool-0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 21:20:36.201691 serialization_tool-0.3/src/serialization_tool/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.3/src/serialization_tool/__init__.py
--rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-0.3/src/serialization_tool/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:20:36.231464 serialization_tool-0.3/src/serialization_tool/serialization/
--rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-0.3/src/serialization_tool/serialization/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-05-03 17:44:51.000000 serialization_tool-0.3/src/serialization_tool/serialization/constants.py
--rw-rw-rw-   0        0        0    10603 2023-05-03 17:27:36.000000 serialization_tool-0.3/src/serialization_tool/serialization/serializer.py
--rw-rw-rw-   0        0        0      465 2023-05-03 20:36:54.000000 serialization_tool-0.3/src/serialization_tool/serialization_factory.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:20:36.234455 serialization_tool-0.3/src/serialization_tool/types/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.3/src/serialization_tool/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:20:36.239460 serialization_tool-0.3/src/serialization_tool/types/json/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.3/src/serialization_tool/types/json/__init__.py
--rw-rw-rw-   0        0        0      138 2023-04-28 13:23:00.000000 serialization_tool-0.3/src/serialization_tool/types/json/constants.py
--rw-rw-rw-   0        0        0      582 2023-05-03 17:32:34.000000 serialization_tool-0.3/src/serialization_tool/types/json/json.py
--rw-rw-rw-   0        0        0     6692 2023-05-03 19:58:39.000000 serialization_tool-0.3/src/serialization_tool/types/json/utilities.py
--rw-rw-rw-   0        0        0      468 2023-05-01 04:12:05.000000 serialization_tool-0.3/src/serialization_tool/types/serialization.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:20:36.242908 serialization_tool-0.3/src/serialization_tool/types/xml/
--rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.3/src/serialization_tool/types/xml/__init__.py
--rw-rw-rw-   0        0        0      254 2023-05-03 20:41:52.000000 serialization_tool-0.3/src/serialization_tool/types/xml/utilities.py
--rw-rw-rw-   0        0        0      467 2023-05-03 20:39:50.000000 serialization_tool-0.3/src/serialization_tool/types/xml/xml.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:20:36.225386 serialization_tool-0.3/src/serialization_tool.egg-info/
--rw-rw-rw-   0        0        0      313 2023-05-03 21:20:36.000000 serialization_tool-0.3/src/serialization_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      893 2023-05-03 21:20:36.000000 serialization_tool-0.3/src/serialization_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 21:20:36.000000 serialization_tool-0.3/src/serialization_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-03 21:20:36.000000 serialization_tool-0.3/src/serialization_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.145834 serialization_tool-0.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-03 21:01:07.000000 serialization_tool-0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      313 2023-05-18 08:34:29.145834 serialization_tool-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-03 20:59:54.000000 serialization_tool-0.5/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-18 08:34:29.161846 serialization_tool-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-05-18 08:33:47.000000 serialization_tool-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:34:28.993830 serialization_tool-0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.037846 serialization_tool-0.5/src/serialization_tool/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.5/src/serialization_tool/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-03 16:35:22.000000 serialization_tool-0.5/src/serialization_tool/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.109830 serialization_tool-0.5/src/serialization_tool/serialization/
+-rw-rw-rw-   0        0        0        0 2023-05-01 04:12:05.000000 serialization_tool-0.5/src/serialization_tool/serialization/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-05-03 17:44:51.000000 serialization_tool-0.5/src/serialization_tool/serialization/constants.py
+-rw-rw-rw-   0        0        0     9770 2023-05-18 08:09:13.000000 serialization_tool-0.5/src/serialization_tool/serialization/serializer.py
+-rw-rw-rw-   0        0        0      465 2023-05-03 20:36:54.000000 serialization_tool-0.5/src/serialization_tool/serialization_factory.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.117870 serialization_tool-0.5/src/serialization_tool/types/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.5/src/serialization_tool/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.129829 serialization_tool-0.5/src/serialization_tool/types/json/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.5/src/serialization_tool/types/json/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-28 13:23:00.000000 serialization_tool-0.5/src/serialization_tool/types/json/constants.py
+-rw-rw-rw-   0        0        0      578 2023-05-17 19:50:20.000000 serialization_tool-0.5/src/serialization_tool/types/json/json.py
+-rw-rw-rw-   0        0        0     6666 2023-05-11 06:39:24.000000 serialization_tool-0.5/src/serialization_tool/types/json/utilities.py
+-rw-rw-rw-   0        0        0      468 2023-05-01 04:12:05.000000 serialization_tool-0.5/src/serialization_tool/types/serialization.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.141834 serialization_tool-0.5/src/serialization_tool/types/xml/
+-rw-rw-rw-   0        0        0        0 2023-04-28 13:21:41.000000 serialization_tool-0.5/src/serialization_tool/types/xml/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-05-11 08:00:16.000000 serialization_tool-0.5/src/serialization_tool/types/xml/constants.py
+-rw-rw-rw-   0        0        0     5111 2023-05-18 08:07:49.000000 serialization_tool-0.5/src/serialization_tool/types/xml/utilities.py
+-rw-rw-rw-   0        0        0      857 2023-05-17 19:38:24.000000 serialization_tool-0.5/src/serialization_tool/types/xml/xml.py
+drwxrwxrwx   0        0        0        0 2023-05-18 08:34:29.097847 serialization_tool-0.5/src/serialization_tool.egg-info/
+-rw-rw-rw-   0        0        0      313 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-18 08:34:28.000000 serialization_tool-0.5/src/serialization_tool.egg-info/top_level.txt
```

### Comparing `serialization_tool-0.3/LICENSE.txt` & `serialization_tool-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `serialization_tool-0.3/src/serialization_tool/serialization/constants.py` & `serialization_tool-0.5/src/serialization_tool/serialization/constants.py`

 * *Files identical despite different names*

### Comparing `serialization_tool-0.3/src/serialization_tool/serialization/serializer.py` & `serialization_tool-0.5/src/serialization_tool/serialization/serializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
         return result
     
     def serialize_dict(self, obj: dict):
         result = dict()
         result[TYPE] = DICTIONARY
         result[VALUE] = {}
-        
+
         for key, value in obj.items():
             key_result = self.serialize(key)
             value_result = self.serialize(value)
             result[VALUE][key_result] = value_result
         
         result[VALUE] = tuple((k, result[VALUE][k])
                             for k in result[VALUE])
@@ -108,15 +108,15 @@
 
         result[VALUE] = tuple((k, result[VALUE][k]) for k in result[VALUE])
         return result
     
     
     def serialize_class(self, obj):
         ans = dict()
-        ans[TYPE] =CLASS
+        ans[TYPE] = CLASS
         ans[VALUE] = {}
         ans[VALUE][self.serialize(NAME)] = self.serialize(obj.__name__)
         members = []
         for i in inspect.getmembers(obj):
             if not (i[0] in NOT_CLASS_ATTRIBUTES):
                 members.append(i)
 
@@ -212,31 +212,15 @@
     def deserialize_type(self, object_type, obj):
         if object_type == TYPES[5]:
             return None
 
         if object_type == TYPES[2] and isinstance(obj, str):
             return obj == "True"
 
-        return locate(object_type)(obj)
-            # result = object
-
-        # if object_type == TYPES[0]:
-        #     result = int(obj)
-        # elif object_type == TYPES[1]:
-        #     result = float(obj)
-        # elif object_type == TYPES[2]:
-        #     result = (obj == "True")
-        # elif object_type == TYPES[4]:
-        #     result = complex(obj)
-        # elif object_type == TYPES[5]:
-        #     result = None
-        # else:
-        #     result = obj
-
-        # return result      
+        return locate(object_type)(obj)    
 
 
     def deserialize_iterable(self, object_type, obj):
         result = []
 
         for value in obj:
             result.append(self.deserialize(value))
@@ -255,24 +239,14 @@
     def deserialize_dict(self, object_type, obj: dict):
         result = {}
         for i in obj:
             val = self.deserialize(i[1])
             result[self.deserialize(i[0])] = val
 
         return result
-        # result = {}
-        # if (type(obj[VALUE]) == tuple):
-        #     return result
-        
-        # for key, value in obj[VALUE].items():
-        #     key_result = self.deserialize(key)
-        #     value_result = self.deserialize(value)
-        #     result[key_result] = value_result
-        
-        # return result
     
 
     def deserialize_function(self, object_type, foo):
         func = [0] * 4
         code = [0] * 16
         glob = {BUILTINS: __builtins__}
```

### Comparing `serialization_tool-0.3/src/serialization_tool/types/json/json.py` & `serialization_tool-0.5/src/serialization_tool/types/json/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from ..serialization import Serialization
 from .utilities import to_json, from_json
 
+
 class JsonSerialization(Serialization):
     def dump(self, obj, file):
-        with open(file, 'w') as f:
+        with open(file, "w") as f:
             f.write(self.dumps(obj))
 
     def dumps(self, obj):
         return to_json(self.serializer.serialize(obj)).replace("\n", "\\n")
 
     def load(self, file):
-        with open(file, 'r') as f:
+        with open(file, "r") as f:
             return self.loads(f.read())
-        
+
     def loads(self, str):
         obj = from_json(str.replace("\\n", "\n"))
-        return self.serializer.deserialize(obj)
+        return self.serializer.deserialize(obj)
```

### Comparing `serialization_tool-0.3/src/serialization_tool/types/json/utilities.py` & `serialization_tool-0.5/src/serialization_tool/types/json/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from frozendict import frozendict
 from .constants import VALUE, TYPE, ARRAY_IN_ARRAY_REGEX, ARRAY_REGEX, VALUE_REGEX
 import re
 
 
 
 def to_json(obj) -> str:
     if type(obj) == tuple:
@@ -10,24 +9,24 @@
         for i in obj:
             serialized.append(f"{to_json(i)}")
         ans = ", ".join(serialized)
         return f"[{ans}]"
     else:
         return f"\"{str(obj)}\""
 
-def from_json(obj: str):
-    if obj == '[]':
+def from_json(data: str):
+    if data == '[]':
         return tuple()
-    elif obj[0] == '[':
-        obj = obj[1:len(obj) - 1]
+    elif data[0] == '[':
+        data = data[1:len(data) - 1]
         parsed = []
         depth = 0
         quote = False
         substr = ""
-        for i in obj:
+        for i in data:
             if i == '[':
                 depth += 1
             elif i == ']':
                 depth -= 1
             elif i == '\"':
                 quote = not quote
             elif i == ',' and not quote and depth == 0:
@@ -38,15 +37,15 @@
                 continue
 
             substr += i
 
         parsed.append(from_json(substr))
         return tuple(parsed)
     else:
-        return obj[1:len(obj) - 1]
+        return data[1:len(data) - 1]
 
 
 # def from_json(string):
 #     if string == '{}':
 #         return frozendict()
 #     elif string[0] == '{':
 #         ans = dict()
```

### Comparing `serialization_tool-0.3/src/serialization_tool.egg-info/SOURCES.txt` & `serialization_tool-0.5/src/serialization_tool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 setup.py
 src/serialization_tool/__init__.py
 src/serialization_tool/constants.py
 src/serialization_tool/serialization_factory.py
 src/serialization_tool.egg-info/PKG-INFO
 src/serialization_tool.egg-info/SOURCES.txt
 src/serialization_tool.egg-info/dependency_links.txt
+src/serialization_tool.egg-info/requires.txt
 src/serialization_tool.egg-info/top_level.txt
 src/serialization_tool/serialization/__init__.py
 src/serialization_tool/serialization/constants.py
 src/serialization_tool/serialization/serializer.py
 src/serialization_tool/types/__init__.py
 src/serialization_tool/types/serialization.py
 src/serialization_tool/types/json/__init__.py
 src/serialization_tool/types/json/constants.py
 src/serialization_tool/types/json/json.py
 src/serialization_tool/types/json/utilities.py
 src/serialization_tool/types/xml/__init__.py
+src/serialization_tool/types/xml/constants.py
 src/serialization_tool/types/xml/utilities.py
 src/serialization_tool/types/xml/xml.py
```

