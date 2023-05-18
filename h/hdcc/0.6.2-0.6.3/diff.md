# Comparing `tmp/hdcc-0.6.2.tar.gz` & `tmp/hdcc-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcc-0.6.2.tar", max compression
+gzip compressed data, was "hdcc-0.6.3.tar", max compression
```

## Comparing `hdcc-0.6.2.tar` & `hdcc-0.6.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       90 2023-04-27 19:50:34.511536 hdcc-0.6.2/README.md
--rw-r--r--   0        0        0    19811 2023-05-18 20:05:24.076365 hdcc-0.6.2/hdcc/HDProg.py
--rw-r--r--   0        0        0    17275 2023-05-18 20:55:49.255047 hdcc-0.6.2/hdcc/HDTypes.py
--rw-r--r--   0        0        0        0 2023-04-27 19:50:34.512471 hdcc-0.6.2/hdcc/__init__.py
--rw-r--r--   0        0        0      330 2023-05-18 20:56:16.097024 hdcc-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-04-27 19:50:34.511536 hdcc-0.6.3/README.md
+-rw-r--r--   0        0        0    19811 2023-05-18 20:05:24.076365 hdcc-0.6.3/hdcc/HDProg.py
+-rw-r--r--   0        0        0    17423 2023-05-18 21:43:21.092307 hdcc-0.6.3/hdcc/HDTypes.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:50:34.512471 hdcc-0.6.3/hdcc/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-18 21:43:37.710350 hdcc-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.6.3/PKG-INFO
```

### Comparing `hdcc-0.6.2/hdcc/HDProg.py` & `hdcc-0.6.3/hdcc/HDProg.py`

 * *Files identical despite different names*

### Comparing `hdcc-0.6.2/hdcc/HDTypes.py` & `hdcc-0.6.3/hdcc/HDTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,21 @@
     
     @staticmethod
     def bundle(vectors: list[HV_FHRR]) -> HV_FHRR:
         # bundle multiple vectors
         # angles of element addition
         # convert the angles to unit complex exponential then add then convert back to angles
         dim = vectors[0].dim
+        HV_FHRR.check_range(vectors)
         assert all([v.dim == dim for v in vectors])
-        data = np.angle(np.sum(np.exp(1j * np.array([v.data for v in vectors])), axis=0))
+        # data = np.angle(np.sum(np.exp(1j * np.array([v.data for v in vectors])), axis=0))
+        vectors = np.array([v.data for v in vectors])
+        data = np.arctan2(np.sum(np.sin(vectors), axis=0), np.sum(np.cos(vectors), axis=0))
         res =  HV_FHRR(dim, data)
         HV_FHRR.wrap_vector(res)
-        HV_FHRR.check_range(vectors)
         return res
     
     @staticmethod
     def wrap_vector(v: HV_FHRR):
         # wrap vector to [-pi, pi)
         while np.any(v.data > np.pi) or np.any(v.data < -np.pi):
             v.data = np.where(v.data > np.pi, v.data - 2 * np.pi, v.data)
```

### Comparing `hdcc-0.6.2/PKG-INFO` & `hdcc-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcc
-Version: 0.6.2
+Version: 0.6.3
 Summary: 
 Author: Yifan Yang
 Author-email: yyang29@stanford.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

