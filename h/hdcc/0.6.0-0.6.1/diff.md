# Comparing `tmp/hdcc-0.6.0.tar.gz` & `tmp/hdcc-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcc-0.6.0.tar", max compression
+gzip compressed data, was "hdcc-0.6.1.tar", max compression
```

## Comparing `hdcc-0.6.0.tar` & `hdcc-0.6.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       90 2023-05-18 07:58:44.444416 hdcc-0.6.0/README.md
--rw-r--r--   0        0        0    19811 2023-05-18 10:55:34.543769 hdcc-0.6.0/hdcc/HDProg.py
--rw-r--r--   0        0        0    16280 2023-05-18 09:07:27.261645 hdcc-0.6.0/hdcc/HDTypes.py
--rw-r--r--   0        0        0        0 2023-05-18 07:58:44.444416 hdcc-0.6.0/hdcc/__init__.py
--rw-r--r--   0        0        0      330 2023-05-18 10:56:38.371800 hdcc-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-04-27 19:50:34.511536 hdcc-0.6.1/README.md
+-rw-r--r--   0        0        0    19811 2023-05-18 20:05:24.076365 hdcc-0.6.1/hdcc/HDProg.py
+-rw-r--r--   0        0        0    16880 2023-05-18 20:48:03.039852 hdcc-0.6.1/hdcc/HDTypes.py
+-rw-r--r--   0        0        0        0 2023-04-27 19:50:34.512471 hdcc-0.6.1/hdcc/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-18 20:48:43.754063 hdcc-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 hdcc-0.6.1/PKG-INFO
```

### Comparing `hdcc-0.6.0/hdcc/HDProg.py` & `hdcc-0.6.1/hdcc/HDProg.py`

 * *Files identical despite different names*

### Comparing `hdcc-0.6.0/hdcc/HDTypes.py` & `hdcc-0.6.1/hdcc/HDTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,36 +41,51 @@
         assert self.dim == other.dim
         return np.mean(np.cos(self.data - other.data))
 
     def bind(self, other: HV_FHRR) -> HV_FHRR:
         # bind two vectors
         assert self.dim == other.dim
         data = self.data + other.data
-        return HV_FHRR(self.dim, data)
+        # wrap data to [-pi, pi)
+        data = np.where(data > np.pi, data - 2 * np.pi, data)
+        data = np.where(data < -np.pi, data + 2 * np.pi, data)
+        res = HV_FHRR(self.dim, data)
+        HV_FHRR.check_range([res])
+        return res
     
     def unbind(self, other: HV_FHRR) -> HV_FHRR:
         # unbind two vectors
         # TODO: check if this is correct
         assert self.dim == other.dim
         data = other.data - self.data
         return HV_FHRR(self.dim, data)
     
     @staticmethod
+    def check_range(vectors: list[HV_FHRR]):
+        # assert all data in v is between -pi and pi
+        if not all([np.all(v.data >= -np.pi) and np.all(v.data <= np.pi) for v in vectors]):
+            for v in vectors:
+                print(v)
+            raise Exception("Data in vectors must be between -pi and pi")
+    
+    @staticmethod
     def bundle(vectors: list[HV_FHRR]) -> HV_FHRR:
         # bundle multiple vectors
         # angles of element addition
         # convert the angles to unit complex exponential then add then convert back to angles
         dim = vectors[0].dim
         assert all([v.dim == dim for v in vectors])
+        HV_FHRR.check_range(vectors)
         data = np.angle(np.sum(np.exp(1j * np.array([v.data for v in vectors])), axis=0))
         return HV_FHRR(dim, data)
     
     def frac_bind(self, frac: float) -> HV_FHRR:
         # bind vector with real number
         data = frac * self.data
+        
         return HV_FHRR(self.dim, data)
 
 
 class HV_HRR(HyperVector):
     def __init__(self, dim: int):
         self.dim = dim
         self.repr = Representation.HRR
```

### Comparing `hdcc-0.6.0/PKG-INFO` & `hdcc-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcc
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Author: Yifan Yang
 Author-email: yyang29@stanford.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

