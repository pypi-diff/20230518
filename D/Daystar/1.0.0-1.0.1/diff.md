# Comparing `tmp/Daystar-1.0.0-py3-none-any.whl.zip` & `tmp/Daystar-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2978 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1657 b- defN 80-Jan-01 00:00 Daystar/__init__.py
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 Daystar-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1503 b- defN 80-Jan-01 00:00 Daystar-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 Daystar-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 80-Jan-01 00:00 Daystar-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      461 b- defN 80-Jan-01 00:00 Daystar-1.0.0.dist-info/RECORD
-6 files, 4790 bytes uncompressed, 2144 bytes compressed:  55.2%
+Zip file size: 3238 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2351 b- defN 80-Jan-01 00:00 Daystar/__init__.py
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 Daystar-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1503 b- defN 80-Jan-01 00:00 Daystar-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 Daystar-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 80-Jan-01 00:00 Daystar-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      461 b- defN 80-Jan-01 00:00 Daystar-1.0.1.dist-info/RECORD
+6 files, 5484 bytes uncompressed, 2404 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: Daystar/__init__.py
 Comment: 
 
-Filename: Daystar-1.0.0.dist-info/LICENSE
+Filename: Daystar-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: Daystar-1.0.0.dist-info/METADATA
+Filename: Daystar-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: Daystar-1.0.0.dist-info/WHEEL
+Filename: Daystar-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: Daystar-1.0.0.dist-info/top_level.txt
+Filename: Daystar-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Daystar-1.0.0.dist-info/RECORD
+Filename: Daystar-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Daystar/__init__.py

```diff
@@ -1,11 +1,32 @@
 from Solarflare.solarflare import *
 import datetime
 
 
+def to_islamic(year):
+  return (year - 622) * 1.03
+
+
+def to_islamic_solar(year):
+  return (to_islamic(year) / 34) - 1429
+
+
+def gregorian_to_hindu_true_solar(lat, long, date=datetime.datetime.now()):
+  # Get the current Gregorian date
+  sun_longitude = ecliptical_longitude(sunrise(lat, long, date))
+  gregorian_date = datetime.date.today()
+  # Get the Sun's longitude at sunrise on January 1st
+  sun_longitude_jan_1 = 280.4588  # This is an approximate value
+  # Calculate the Hindu true solar date
+  hindu_true_solar_date = gregorian_date + datetime.timedelta(
+    days=(sun_longitude / 360) - (sun_longitude_jan_1 / 360))
+  # Return the Hindu true solar date
+  return hindu_true_solar_date
+
+
 class Daystar:
 
   def __init__(self, lat, long):
     self.lat = lat
     self.long = long
 
   def risetime(self, date=datetime.datetime.now()):
```

## Comparing `Daystar-1.0.0.dist-info/LICENSE` & `Daystar-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Daystar-1.0.0.dist-info/METADATA` & `Daystar-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Daystar
-Version: 1.0.0
+Version: 1.0.1
 Summary: Solar calculation class for Python
 Author: Siddhu Pendyala
 Author-email: siddhu.pendyala@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

