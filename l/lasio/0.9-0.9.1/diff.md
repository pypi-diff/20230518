# Comparing `tmp/lasio-0.9-py2.py3-none-any.whl.zip` & `tmp/lasio-0.9.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13933 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat    35200 b- defN 15-Nov-11 12:54 lasio/las.py
+Zip file size: 13994 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat    35283 b- defN 15-Nov-11 13:12 lasio/las.py
 -rw-rw-rw-  2.0 fat     1998 b- defN 15-Nov-04 13:07 lasio/las2excel.py
 -rw-rw-rw-  2.0 fat       62 b- defN 15-Nov-04 13:07 lasio/__init__.py
--rw-rw-rw-  2.0 fat     2426 b- defN 15-Nov-11 13:09 lasio-0.9.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat       52 b- defN 15-Nov-11 13:09 lasio-0.9.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat     1517 b- defN 15-Nov-11 13:09 lasio-0.9.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        6 b- defN 15-Nov-11 13:09 lasio-0.9.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat      116 b- defN 15-Nov-11 13:09 lasio-0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     3817 b- defN 15-Nov-11 13:09 lasio-0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat      782 b- defN 15-Nov-11 13:09 lasio-0.9.dist-info/RECORD
-10 files, 45976 bytes uncompressed, 12625 bytes compressed:  72.5%
+-rw-rw-rw-  2.0 fat     2426 b- defN 15-Nov-11 13:12 lasio-0.9.1.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat       52 b- defN 15-Nov-11 13:12 lasio-0.9.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat     1519 b- defN 15-Nov-11 13:12 lasio-0.9.1.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        6 b- defN 15-Nov-11 13:12 lasio-0.9.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat      116 b- defN 15-Nov-11 13:12 lasio-0.9.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     3819 b- defN 15-Nov-11 13:12 lasio-0.9.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      796 b- defN 15-Nov-11 13:12 lasio-0.9.1.dist-info/RECORD
+10 files, 46077 bytes uncompressed, 12658 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: lasio/las2excel.py
 Comment: 
 
 Filename: lasio/__init__.py
 Comment: 
 
-Filename: lasio-0.9.dist-info/DESCRIPTION.rst
+Filename: lasio-0.9.1.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: lasio-0.9.dist-info/entry_points.txt
+Filename: lasio-0.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: lasio-0.9.dist-info/metadata.json
+Filename: lasio-0.9.1.dist-info/metadata.json
 Comment: 
 
-Filename: lasio-0.9.dist-info/top_level.txt
+Filename: lasio-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: lasio-0.9.dist-info/WHEEL
+Filename: lasio-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: lasio-0.9.dist-info/METADATA
+Filename: lasio-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: lasio-0.9.dist-info/RECORD
+Filename: lasio-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lasio/las.py

```diff
@@ -45,15 +45,15 @@
 import numpy
 
 # Optional third-party packages available on PyPI are mostly
 # imported inline below.
 
 
 logger = logging.getLogger(__name__)
-__version__ = "0.9"
+__version__ = "0.9.1"
 
 
 HeaderItem = namedlist("HeaderItem", ["mnemonic", "unit", "value", "descr"])
 Curve = namedlist("Curve", ["mnemonic", "unit", "value", "descr", "data"])
 
 
 class LASDataError(Exception):
@@ -178,30 +178,30 @@
         self.curves = list(DEFAULT_ITEMS["curves"])
         self.params = OrderedDictionary(DEFAULT_ITEMS["params"].items())
         self.other = str(DEFAULT_ITEMS["other"])
 
         if not (file_ref is None):
             self.read(file_ref, **kwargs)
 
-    def read(self, file_ref, use_pandas="auto", **kwargs):
+    def read(self, file_ref, use_pandas="auto", null_subs=True, **kwargs):
         '''Read a LAS file.
 
         Arguments:
             file_ref: either a filename, an open file object, or a string of
                 a LAS file contents.
 
         Keyword Arguments:
             use_pandas (str): bool or "auto" -- use pandas if available -- provide
                 False option for faster loading where pandas functionality is not
                 needed. "auto" becomes True if pandas is installed, and False if not.
             encoding (str): character encoding to open file_ref with
             encoding_errors (str): "strict", "replace" (default), "ignore" - how to
                 handle errors with encodings (see standard library codecs module or
                 Python Unicode HOWTO for more information)
-            autodetect_encoding (bool): use chardet/ccharet to detect encoding
+            autodetect_encoding (bool): use chardet/cchardet to detect encoding
             autodetect_encoding_chars (int/None): number of chars to read from LAS
                 file for auto-detection of encoding.
 
         '''
         if not use_pandas is None:
             self._use_pandas = use_pandas
 
@@ -238,15 +238,15 @@
         except LASHeaderError:
             logger.warning(traceback.format_exc().splitlines()[-1])
         self.other = reader.read_raw_text('~O')
 
         # Set null value
         reader.null = self.well['NULL'].value
 
-        data = reader.read_data(len(self.curves))
+        data = reader.read_data(len(self.curves), null_subs=null_subs)
 
         for i, c in enumerate(self.curves):
             d = data[:, i]
             c.data = d
 
         if (self.well["STRT"].unit.upper() == "M" and
                 self.well["STOP"].unit.upper() == "M" and
@@ -611,15 +611,15 @@
                 raise LASHeaderError("Failed in %s section on line:\n%s%s" % (
                     section_name, line,
                     traceback.format_exc().splitlines()[-1]))
             else:
                 l.append(parser(**values))
         return l
 
-    def read_data(self, number_of_curves=None):
+    def read_data(self, number_of_curves=None, null_subs=True):
         s = self.read_data_string()
         if not self.wrap:
             try:
                 arr = numpy.loadtxt(StringIO(s))
             except:
                 raise LASDataError("Failed to read data:\n%s" % (
                                    traceback.format_exc().splitlines()[-1]))
@@ -636,15 +636,16 @@
             arr = numpy.reshape(arr, (-1, number_of_curves))
         if not arr.shape or (arr.ndim == 1 and arr.shape[0] == 0):
             logger.warning('No data present.')
             return None, None
         else:
             logger.info('LAS file shape = %s' % str(arr.shape))
         logger.debug('checking for nulls (NULL = %s)' % self.null)
-        arr[arr == self.null] = numpy.nan
+        if null_subs:
+            arr[arr == self.null] = numpy.nan
         return arr
 
     def read_data_string(self):
         start_data = None
         for i, line in enumerate(self.lines):
             line = line.strip().strip('\t').strip()
             if line.startswith('~A'):
```

## Comparing `lasio-0.9.dist-info/DESCRIPTION.rst` & `lasio-0.9.1.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `lasio-0.9.dist-info/metadata.json` & `lasio-0.9.1.dist-info/metadata.json`

 * *Files 0% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.9.1'"}*

```diff
@@ -64,9 +64,9 @@
                 "namedlist",
                 "numpy",
                 "ordereddict"
             ]
         }
     ],
     "summary": "Read/write well data from Log ASCII Standard (LAS) files",
-    "version": "0.9"
+    "version": "0.9.1"
 }
```

## Comparing `lasio-0.9.dist-info/METADATA` & `lasio-0.9.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: lasio
-Version: 0.9
+Version: 0.9.1
 Summary: Read/write well data from Log ASCII Standard (LAS) files
 Home-page: https://github.com/kinverarity1/lasio
 Author: Kent Inverarity
 Author-email: kinverarity1@gmail.com
 License: MIT
 Keywords: science geophysics io
 Platform: UNKNOWN
```

