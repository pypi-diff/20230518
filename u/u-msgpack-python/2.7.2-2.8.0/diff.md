# Comparing `tmp/u-msgpack-python-2.7.2.tar.gz` & `tmp/u-msgpack-python-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "u-msgpack-python-2.7.2.tar", last modified: Tue Nov  8 06:14:14 2022, max compression
+gzip compressed data, was "u-msgpack-python-2.8.0.tar", last modified: Thu May 18 09:28:05 2023, max compression
```

## Comparing `u-msgpack-python-2.7.2.tar` & `u-msgpack-python-2.8.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2022-11-08 06:14:14.205145 u-msgpack-python-2.7.2/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1099 2022-11-08 06:02:37.000000 u-msgpack-python-2.7.2/LICENSE
--rw-r--r--   0 anteater  (1000) anteater  (1000)       41 2017-08-05 01:25:46.000000 u-msgpack-python-2.7.2/MANIFEST.in
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1306 2022-11-08 06:14:14.205145 u-msgpack-python-2.7.2/PKG-INFO
--rw-r--r--   0 anteater  (1000) anteater  (1000)    18483 2022-11-08 06:07:34.000000 u-msgpack-python-2.7.2/README.md
--rw-r--r--   0 anteater  (1000) anteater  (1000)      111 2022-11-08 06:14:14.205145 u-msgpack-python-2.7.2/setup.cfg
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1486 2022-11-08 06:07:34.000000 u-msgpack-python-2.7.2/setup.py
--rw-r--r--   0 anteater  (1000) anteater  (1000)    32752 2020-10-25 03:50:17.000000 u-msgpack-python-2.7.2/test_umsgpack.py
-drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2022-11-08 06:14:14.205145 u-msgpack-python-2.7.2/u_msgpack_python.egg-info/
--rw-r--r--   0 anteater  (1000) anteater  (1000)     1306 2022-11-08 06:14:14.000000 u-msgpack-python-2.7.2/u_msgpack_python.egg-info/PKG-INFO
--rw-r--r--   0 anteater  (1000) anteater  (1000)      237 2022-11-08 06:14:14.000000 u-msgpack-python-2.7.2/u_msgpack_python.egg-info/SOURCES.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)        1 2022-11-08 06:14:14.000000 u-msgpack-python-2.7.2/u_msgpack_python.egg-info/dependency_links.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)        9 2022-11-08 06:14:14.000000 u-msgpack-python-2.7.2/u_msgpack_python.egg-info/top_level.txt
--rw-r--r--   0 anteater  (1000) anteater  (1000)    43450 2022-11-08 06:07:34.000000 u-msgpack-python-2.7.2/umsgpack.py
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-05-18 09:28:05.021552 u-msgpack-python-2.8.0/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1099 2023-05-03 05:48:38.000000 u-msgpack-python-2.8.0/LICENSE
+-rw-r--r--   0 anteater  (1000) anteater  (1000)       41 2017-08-05 01:25:46.000000 u-msgpack-python-2.8.0/MANIFEST.in
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1306 2023-05-18 09:28:05.021552 u-msgpack-python-2.8.0/PKG-INFO
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     5331 2023-05-18 09:23:20.000000 u-msgpack-python-2.8.0/README.md
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      111 2023-05-18 09:28:05.021552 u-msgpack-python-2.8.0/setup.cfg
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1538 2023-05-18 09:23:20.000000 u-msgpack-python-2.8.0/setup.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    32752 2020-10-25 03:50:17.000000 u-msgpack-python-2.8.0/test_umsgpack.py
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-05-18 09:28:05.021552 u-msgpack-python-2.8.0/u_msgpack_python.egg-info/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1306 2023-05-18 09:28:04.000000 u-msgpack-python-2.8.0/u_msgpack_python.egg-info/PKG-INFO
+-rw-r--r--   0 anteater  (1000) anteater  (1000)      268 2023-05-18 09:28:04.000000 u-msgpack-python-2.8.0/u_msgpack_python.egg-info/SOURCES.txt
+-rw-r--r--   0 anteater  (1000) anteater  (1000)        1 2023-05-18 09:28:04.000000 u-msgpack-python-2.8.0/u_msgpack_python.egg-info/dependency_links.txt
+-rw-r--r--   0 anteater  (1000) anteater  (1000)        9 2023-05-18 09:28:04.000000 u-msgpack-python-2.8.0/u_msgpack_python.egg-info/top_level.txt
+drwxr-xr-x   0 anteater  (1000) anteater  (1000)        0 2023-05-18 09:28:05.021552 u-msgpack-python-2.8.0/umsgpack/
+-rw-r--r--   0 anteater  (1000) anteater  (1000)    43617 2023-05-18 09:23:20.000000 u-msgpack-python-2.8.0/umsgpack/__init__.py
+-rw-r--r--   0 anteater  (1000) anteater  (1000)     1275 2023-05-18 09:18:04.000000 u-msgpack-python-2.8.0/umsgpack/__init__.pyi
```

### Comparing `u-msgpack-python-2.7.2/LICENSE` & `u-msgpack-python-2.8.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
- Copyright (c) 2013-2022 vsergeev / Ivan (Vanya) A. Sergeev
+ Copyright (c) 2013-2023 vsergeev / Ivan (Vanya) A. Sergeev
 
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `u-msgpack-python-2.7.2/PKG-INFO` & `u-msgpack-python-2.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: u-msgpack-python
-Version: 2.7.2
+Version: 2.8.0
 Summary: A portable, lightweight MessagePack serializer and deserializer written in pure Python.
 Home-page: https://github.com/vsergeev/u-msgpack-python
 Author: vsergeev
 Author-email: v@sergeev.io
 License: MIT
 Keywords: msgpack serialization deserialization
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `u-msgpack-python-2.7.2/setup.py` & `u-msgpack-python-2.8.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='u-msgpack-python',
-    version='2.7.2',
+    version='2.8.0',
     description='A portable, lightweight MessagePack serializer and deserializer written in pure Python.',
     author='vsergeev',
     author_email='v@sergeev.io',
     url='https://github.com/vsergeev/u-msgpack-python',
-    py_modules=['umsgpack'],
+    packages=['umsgpack'],
+    package_data={'umsgpack': ['*.pyi', 'py.typed']},
     long_description="""u-msgpack-python is a lightweight `MessagePack <http://msgpack.org/>`_ serializer and deserializer module written in pure Python, compatible with both Python 2 and Python 3, as well as CPython and PyPy implementations of Python. u-msgpack-python is fully compliant with the latest `MessagePack specification <https://github.com/msgpack/msgpack/blob/master/spec.md>`_. In particular, it supports the new binary, UTF-8 string, and application-defined ext types. See https://github.com/vsergeev/u-msgpack-python for more information.""",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
```

### Comparing `u-msgpack-python-2.7.2/test_umsgpack.py` & `u-msgpack-python-2.8.0/test_umsgpack.py`

 * *Files identical despite different names*

### Comparing `u-msgpack-python-2.7.2/u_msgpack_python.egg-info/PKG-INFO` & `u-msgpack-python-2.8.0/u_msgpack_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: u-msgpack-python
-Version: 2.7.2
+Version: 2.8.0
 Summary: A portable, lightweight MessagePack serializer and deserializer written in pure Python.
 Home-page: https://github.com/vsergeev/u-msgpack-python
 Author: vsergeev
 Author-email: v@sergeev.io
 License: MIT
 Keywords: msgpack serialization deserialization
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `u-msgpack-python-2.7.2/umsgpack.py` & `u-msgpack-python-2.8.0/umsgpack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# u-msgpack-python v2.7.2 - v at sergeev.io
+# u-msgpack-python v2.8.0 - v at sergeev.io
 # https://github.com/vsergeev/u-msgpack-python
 #
 # u-msgpack-python is a lightweight MessagePack serializer and deserializer
 # module, compatible with both Python 2 and 3, as well CPython and PyPy
 # implementations of Python. u-msgpack-python is fully compliant with the
 # latest MessagePack specification.com/msgpack/msgpack/blob/master/spec.md). In
 # particular, it supports the new binary, UTF-8 string, and application ext
 # types.
 #
 # MIT License
 #
-# Copyright (c) 2013-2022 vsergeev / Ivan (Vanya) A. Sergeev
+# Copyright (c) 2013-2023 vsergeev / Ivan (Vanya) A. Sergeev
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -27,15 +27,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
 """
-u-msgpack-python v2.7.2 - v at sergeev.io
+u-msgpack-python v2.8.0 - v at sergeev.io
 https://github.com/vsergeev/u-msgpack-python
 
 u-msgpack-python is a lightweight MessagePack serializer and deserializer
 module, compatible with both Python 2 and 3, as well CPython and PyPy
 implementations of Python. u-msgpack-python is fully compliant with the
 latest MessagePack specification.com/msgpack/msgpack/blob/master/spec.md). In
 particular, it supports the new binary, UTF-8 string, and application ext
@@ -50,18 +50,18 @@
 import io
 
 if sys.version_info[0:2] >= (3, 3):
     from collections.abc import Hashable
 else:
     from collections import Hashable
 
-__version__ = "2.7.2"
+__version__ = "2.8.0"
 "Module version string"
 
-version = (2, 7, 2)
+version = (2, 8, 0)
 "Module version tuple"
 
 
 ##############################################################################
 # Ext Class
 ##############################################################################
 
@@ -73,32 +73,32 @@
     """
 
     def __init__(self, type, data):
         """
         Construct a new Ext object.
 
         Args:
-            type: application-defined type integer
-            data: application-defined data byte array
+            type (int): application-defined type integer
+            data (bytes): application-defined data byte array
 
-        TypeError:
-            Type is not an integer.
-        ValueError:
-            Type is out of range of -128 to 127.
-        TypeError::
-            Data is not type 'bytes' (Python 3) or not type 'str' (Python 2).
+        Raises:
+            TypeError:
+                Type is not an integer.
+            ValueError:
+                Type is out of range of -128 to 127.
+            TypeError:
+                Data is not type 'bytes' (Python 3) or not type 'str' (Python 2).
 
         Example:
-        >>> foo = umsgpack.Ext(5, b"\x01\x02\x03")
-        >>> umsgpack.packb({u"special stuff": foo, u"awesome": True})
-        '\x82\xa7awesome\xc3\xadspecial stuff\xc7\x03\x05\x01\x02\x03'
-        >>> bar = umsgpack.unpackb(_)
-        >>> print(bar["special stuff"])
-        Ext Object (Type: 5, Data: 01 02 03)
-        >>>
+            >>> foo = umsgpack.Ext(5, b"\\x01\\x02\\x03")
+            >>> umsgpack.packb({u"special stuff": foo, u"awesome": True})
+            '\\x82\\xa7awesome\\xc3\\xadspecial stuff\\xc7\\x03\\x05\\x01\\x02\\x03'
+            >>> bar = umsgpack.unpackb(_)
+            >>> print(bar["special stuff"])
+            Ext Object (Type: 5, Data: 01 02 03)
         """
         # Check type is type int and in range
         if not isinstance(type, int):
             raise TypeError("ext type is not type integer")
         elif not (-2**7 <= type <= 2**7 - 1):
             raise ValueError("ext type value {:d} is out of range (-128 to 127)".format(type))
         # Check data is type bytes or str
@@ -159,15 +159,15 @@
     Return a decorator to register a class for automatic packing and unpacking
     with the specified Ext type code. The application class should implement a
     `packb()` method that returns serialized bytes, and an `unpackb()` class
     method or static method that accepts serialized bytes and returns an
     instance of the application class.
 
     Args:
-        ext_type: application-defined Ext type code
+        ext_type (int): application-defined Ext type code
 
     Raises:
         TypeError:
             Ext type is not an integer.
         ValueError:
             Ext type is out of range of -128 to 127.
         ValueError:
@@ -262,21 +262,19 @@
 
 When compatibility mode is enabled, u-msgpack-python will serialize both
 unicode strings and bytes into the old "raw" msgpack type, and deserialize the
 "raw" msgpack type into bytes. This provides backwards compatibility with the
 old MessagePack specification.
 
 Example:
->>> umsgpack.compatibility = True
->>>
->>> umsgpack.packb([u"some string", b"some bytes"])
-b'\x92\xabsome string\xaasome bytes'
->>> umsgpack.unpackb(_)
-[b'some string', b'some bytes']
->>>
+    >>> umsgpack.compatibility = True
+    >>> umsgpack.packb([u"some string", b"some bytes"])
+    b'\\x92\\xabsome string\\xaasome bytes'
+    >>> umsgpack.unpackb(_)
+    [b'some string', b'some bytes']
 """
 
 ##############################################################################
 # Packing
 ##############################################################################
 
 # You may notice struct.pack("B", obj) instead of the simpler chr(obj) in the
@@ -458,34 +456,33 @@
     """
     Serialize a Python object into MessagePack bytes.
 
     Args:
         obj: a Python object
         fp: a .write()-supporting file-like object
 
-    Kwargs:
+    Keyword Args:
         ext_handlers (dict): dictionary of Ext handlers, mapping a custom type
                              to a callable that packs an instance of the type
                              into an Ext object
         force_float_precision (str): "single" to force packing floats as
                                      IEEE-754 single-precision floats,
                                      "double" to force packing floats as
-                                     IEEE-754 double-precision floats.
+                                     IEEE-754 double-precision floats
 
     Returns:
-        None.
+        None
 
     Raises:
-        UnsupportedType(PackException):
+        UnsupportedTypeException(PackException):
             Object type not supported for packing.
 
     Example:
-    >>> f = open('test.bin', 'wb')
-    >>> umsgpack.pack({u"compact": True, u"schema": 0}, f)
-    >>>
+        >>> f = open('test.bin', 'wb')
+        >>> umsgpack.pack({u"compact": True, u"schema": 0}, f)
     """
     global compatibility
 
     ext_handlers = options.get("ext_handlers")
 
     if obj is None:
         _pack_nil(obj, fp, options)
@@ -494,23 +491,23 @@
     elif obj.__class__ in _ext_class_to_type:
         try:
             _pack_ext(Ext(_ext_class_to_type[obj.__class__], obj.packb()), fp, options)
         except AttributeError:
             raise NotImplementedError("Ext serializable class {:s} is missing implementation of packb()".format(repr(obj.__class__)))
     elif isinstance(obj, bool):
         _pack_boolean(obj, fp, options)
-    elif isinstance(obj, (int, long)):
+    elif isinstance(obj, (int, long)):  # noqa: F821
         _pack_integer(obj, fp, options)
     elif isinstance(obj, float):
         _pack_float(obj, fp, options)
-    elif compatibility and isinstance(obj, unicode):
+    elif compatibility and isinstance(obj, unicode):  # noqa: F821
         _pack_oldspec_raw(bytes(obj), fp, options)
     elif compatibility and isinstance(obj, bytes):
         _pack_oldspec_raw(obj, fp, options)
-    elif isinstance(obj, unicode):
+    elif isinstance(obj, unicode):  # noqa: F821
         _pack_string(obj, fp, options)
     elif isinstance(obj, str):
         _pack_binary(obj, fp, options)
     elif isinstance(obj, (list, tuple)):
         _pack_array(obj, fp, options)
     elif isinstance(obj, dict):
         _pack_map(obj, fp, options)
@@ -545,34 +542,33 @@
     """
     Serialize a Python object into MessagePack bytes.
 
     Args:
         obj: a Python object
         fp: a .write()-supporting file-like object
 
-    Kwargs:
+    Keyword Args:
         ext_handlers (dict): dictionary of Ext handlers, mapping a custom type
                              to a callable that packs an instance of the type
                              into an Ext object
         force_float_precision (str): "single" to force packing floats as
                                      IEEE-754 single-precision floats,
                                      "double" to force packing floats as
-                                     IEEE-754 double-precision floats.
+                                     IEEE-754 double-precision floats
 
     Returns:
-        None.
+        None
 
     Raises:
-        UnsupportedType(PackException):
+        UnsupportedTypeException(PackException):
             Object type not supported for packing.
 
     Example:
-    >>> f = open('test.bin', 'wb')
-    >>> umsgpack.pack({u"compact": True, u"schema": 0}, f)
-    >>>
+        >>> f = open('test.bin', 'wb')
+        >>> umsgpack.pack({u"compact": True, u"schema": 0}, f)
     """
     global compatibility
 
     ext_handlers = options.get("ext_handlers")
 
     if obj is None:
         _pack_nil(obj, fp, options)
@@ -631,67 +627,65 @@
 def _packb2(obj, **options):
     """
     Serialize a Python object into MessagePack bytes.
 
     Args:
         obj: a Python object
 
-    Kwargs:
+    Keyword Args:
         ext_handlers (dict): dictionary of Ext handlers, mapping a custom type
                              to a callable that packs an instance of the type
                              into an Ext object
         force_float_precision (str): "single" to force packing floats as
                                      IEEE-754 single-precision floats,
                                      "double" to force packing floats as
-                                     IEEE-754 double-precision floats.
+                                     IEEE-754 double-precision floats
 
     Returns:
-        A 'str' containing serialized MessagePack bytes.
+        str: Serialized MessagePack bytes
 
     Raises:
-        UnsupportedType(PackException):
+        UnsupportedTypeException(PackException):
             Object type not supported for packing.
 
     Example:
-    >>> umsgpack.packb({u"compact": True, u"schema": 0})
-    '\x82\xa7compact\xc3\xa6schema\x00'
-    >>>
+        >>> umsgpack.packb({u"compact": True, u"schema": 0})
+        '\\x82\\xa7compact\\xc3\\xa6schema\\x00'
     """
     fp = io.BytesIO()
     _pack2(obj, fp, **options)
     return fp.getvalue()
 
 
 def _packb3(obj, **options):
     """
     Serialize a Python object into MessagePack bytes.
 
     Args:
         obj: a Python object
 
-    Kwargs:
+    Keyword Args:
         ext_handlers (dict): dictionary of Ext handlers, mapping a custom type
                              to a callable that packs an instance of the type
                              into an Ext object
         force_float_precision (str): "single" to force packing floats as
                                      IEEE-754 single-precision floats,
                                      "double" to force packing floats as
-                                     IEEE-754 double-precision floats.
+                                     IEEE-754 double-precision floats
 
     Returns:
-        A 'bytes' containing serialized MessagePack bytes.
+        bytes: Serialized MessagePack bytes
 
     Raises:
-        UnsupportedType(PackException):
+        UnsupportedTypeException(PackException):
             Object type not supported for packing.
 
     Example:
-    >>> umsgpack.packb({u"compact": True, u"schema": 0})
-    b'\x82\xa7compact\xc3\xa6schema\x00'
-    >>>
+        >>> umsgpack.packb({u"compact": True, u"schema": 0})
+        b'\\x82\\xa7compact\\xc3\\xa6schema\\x00'
     """
     fp = io.BytesIO()
     _pack3(obj, fp, **options)
     return fp.getvalue()
 
 #############################################################################
 # Unpacking
@@ -942,28 +936,28 @@
 def _unpack2(fp, **options):
     """
     Deserialize MessagePack bytes into a Python object.
 
     Args:
         fp: a .read()-supporting file-like object
 
-    Kwargs:
+    Keyword Args:
         ext_handlers (dict): dictionary of Ext handlers, mapping integer Ext
                              type to a callable that unpacks an instance of
                              Ext into an object
-        use_ordered_dict (bool): unpack maps into OrderedDict, instead of
-                                 unordered dict (default False)
+        use_ordered_dict (bool): unpack maps into OrderedDict, instead of dict
+                                 (default False)
         use_tuple (bool): unpacks arrays into tuples, instead of lists (default
                           False)
         allow_invalid_utf8 (bool): unpack invalid strings into instances of
-                                   InvalidString, for access to the bytes
-                                   (default False)
+                                   :class:`InvalidString`, for access to the
+                                   bytes (default False)
 
     Returns:
-        A Python object.
+        Python object
 
     Raises:
         InsufficientDataException(UnpackException):
             Insufficient data to unpack the serialized object.
         InvalidStringException(UnpackException):
             Invalid UTF-8 string encountered during unpacking.
         UnsupportedTimestampException(UnpackException):
@@ -973,43 +967,42 @@
         UnhashableKeyException(UnpackException):
             Unhashable key encountered during map unpacking.
             The serialized map cannot be deserialized into a Python dictionary.
         DuplicateKeyException(UnpackException):
             Duplicate key encountered during map unpacking.
 
     Example:
-    >>> f = open('test.bin', 'rb')
-    >>> umsgpack.unpackb(f)
-    {u'compact': True, u'schema': 0}
-    >>>
+        >>> f = open('test.bin', 'rb')
+        >>> umsgpack.unpackb(f)
+        {u'compact': True, u'schema': 0}
     """
     return _unpack(fp, options)
 
 
 def _unpack3(fp, **options):
     """
     Deserialize MessagePack bytes into a Python object.
 
     Args:
         fp: a .read()-supporting file-like object
 
-    Kwargs:
+    Keyword Args:
         ext_handlers (dict): dictionary of Ext handlers, mapping integer Ext
                              type to a callable that unpacks an instance of
                              Ext into an object
-        use_ordered_dict (bool): unpack maps into OrderedDict, instead of
-                                 unordered dict (default False)
+        use_ordered_dict (bool): unpack maps into OrderedDict, instead of dict
+                                 (default False)
         use_tuple (bool): unpacks arrays into tuples, instead of lists (default
                           False)
         allow_invalid_utf8 (bool): unpack invalid strings into instances of
-                                   InvalidString, for access to the bytes
-                                   (default False)
+                                   :class:`InvalidString`, for access to the
+                                   bytes (default False)
 
     Returns:
-        A Python object.
+        Python object
 
     Raises:
         InsufficientDataException(UnpackException):
             Insufficient data to unpack the serialized object.
         InvalidStringException(UnpackException):
             Invalid UTF-8 string encountered during unpacking.
         UnsupportedTimestampException(UnpackException):
@@ -1019,44 +1012,43 @@
         UnhashableKeyException(UnpackException):
             Unhashable key encountered during map unpacking.
             The serialized map cannot be deserialized into a Python dictionary.
         DuplicateKeyException(UnpackException):
             Duplicate key encountered during map unpacking.
 
     Example:
-    >>> f = open('test.bin', 'rb')
-    >>> umsgpack.unpackb(f)
-    {'compact': True, 'schema': 0}
-    >>>
+        >>> f = open('test.bin', 'rb')
+        >>> umsgpack.unpackb(f)
+        {'compact': True, 'schema': 0}
     """
     return _unpack(fp, options)
 
 
 # For Python 2, expects a str object
 def _unpackb2(s, **options):
     """
     Deserialize MessagePack bytes into a Python object.
 
     Args:
-        s: a 'str' or 'bytearray' containing serialized MessagePack bytes
+        s (str, bytearray): serialized MessagePack bytes
 
-    Kwargs:
+    Keyword Args:
         ext_handlers (dict): dictionary of Ext handlers, mapping integer Ext
                              type to a callable that unpacks an instance of
                              Ext into an object
-        use_ordered_dict (bool): unpack maps into OrderedDict, instead of
-                                 unordered dict (default False)
+        use_ordered_dict (bool): unpack maps into OrderedDict, instead of dict
+                                 (default False)
         use_tuple (bool): unpacks arrays into tuples, instead of lists (default
                           False)
         allow_invalid_utf8 (bool): unpack invalid strings into instances of
-                                   InvalidString, for access to the bytes
-                                   (default False)
+                                   :class:`InvalidString`, for access to the
+                                   bytes (default False)
 
     Returns:
-        A Python object.
+        Python object
 
     Raises:
         TypeError:
             Packed data type is neither 'str' nor 'bytearray'.
         InsufficientDataException(UnpackException):
             Insufficient data to unpack the serialized object.
         InvalidStringException(UnpackException):
@@ -1068,45 +1060,44 @@
         UnhashableKeyException(UnpackException):
             Unhashable key encountered during map unpacking.
             The serialized map cannot be deserialized into a Python dictionary.
         DuplicateKeyException(UnpackException):
             Duplicate key encountered during map unpacking.
 
     Example:
-    >>> umsgpack.unpackb(b'\x82\xa7compact\xc3\xa6schema\x00')
-    {u'compact': True, u'schema': 0}
-    >>>
+        >>> umsgpack.unpackb(b'\\x82\\xa7compact\\xc3\\xa6schema\\x00')
+        {u'compact': True, u'schema': 0}
     """
     if not isinstance(s, (str, bytearray)):
         raise TypeError("packed data must be type 'str' or 'bytearray'")
     return _unpack(io.BytesIO(s), options)
 
 
 # For Python 3, expects a bytes object
 def _unpackb3(s, **options):
     """
     Deserialize MessagePack bytes into a Python object.
 
     Args:
-        s: a 'bytes' or 'bytearray' containing serialized MessagePack bytes
+        s (bytes, bytearray): serialized MessagePack bytes
 
-    Kwargs:
+    Keyword Args:
         ext_handlers (dict): dictionary of Ext handlers, mapping integer Ext
                              type to a callable that unpacks an instance of
                              Ext into an object
-        use_ordered_dict (bool): unpack maps into OrderedDict, instead of
-                                 unordered dict (default False)
+        use_ordered_dict (bool): unpack maps into OrderedDict, instead of dict
+                                 (default False)
         use_tuple (bool): unpacks arrays into tuples, instead of lists (default
                           False)
         allow_invalid_utf8 (bool): unpack invalid strings into instances of
-                                   InvalidString, for access to the bytes
-                                   (default False)
+                                   :class:`InvalidString`, for access to the
+                                   bytes (default False)
 
     Returns:
-        A Python object.
+        Python object
 
     Raises:
         TypeError:
             Packed data type is neither 'bytes' nor 'bytearray'.
         InsufficientDataException(UnpackException):
             Insufficient data to unpack the serialized object.
         InvalidStringException(UnpackException):
@@ -1118,17 +1109,16 @@
         UnhashableKeyException(UnpackException):
             Unhashable key encountered during map unpacking.
             The serialized map cannot be deserialized into a Python dictionary.
         DuplicateKeyException(UnpackException):
             Duplicate key encountered during map unpacking.
 
     Example:
-    >>> umsgpack.unpackb(b'\x82\xa7compact\xc3\xa6schema\x00')
-    {'compact': True, 'schema': 0}
-    >>>
+        >>> umsgpack.unpackb(b'\\x82\\xa7compact\\xc3\\xa6schema\\x00')
+        {'compact': True, 'schema': 0}
     """
     if not isinstance(s, (bytes, bytearray)):
         raise TypeError("packed data must be type 'bytes' or 'bytearray'")
     return _unpack(io.BytesIO(s), options)
 
 #############################################################################
 # Module Initialization
```

