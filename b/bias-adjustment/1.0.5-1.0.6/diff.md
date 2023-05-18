# Comparing `tmp/bias_adjustment-1.0.5.tar.gz` & `tmp/bias_adjustment-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bias_adjustment-1.0.5.tar", max compression
+gzip compressed data, was "bias_adjustment-1.0.6.tar", max compression
```

## Comparing `bias_adjustment-1.0.5.tar` & `bias_adjustment-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-05-10 14:11:11.340594 bias_adjustment-1.0.5/LICENSE
--rw-r--r--   0        0        0      274 2022-11-15 06:42:37.967412 bias_adjustment-1.0.5/README.md
--rw-r--r--   0        0        0      705 2023-05-17 05:35:50.089939 bias_adjustment-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      205 2023-05-10 14:11:11.361595 bias_adjustment-1.0.5/src/bias_adjustment/__init__.py
--rw-r--r--   0        0        0     2662 2023-05-17 05:38:22.798586 bias_adjustment-1.0.5/src/bias_adjustment/bias_adjustment.py
--rw-r--r--   0        0        0       37 2023-05-17 03:12:37.290749 bias_adjustment-1.0.5/src/bias_adjustment/const.py
--rw-r--r--   0        0        0       97 2023-05-10 14:11:11.361595 bias_adjustment-1.0.5/src/bias_adjustment/distributions/__init__.py
--rw-r--r--   0        0        0     5089 2023-05-10 14:11:11.361595 bias_adjustment-1.0.5/src/bias_adjustment/distributions/distributions.py
--rw-r--r--   0        0        0      300 2023-05-10 14:11:11.361595 bias_adjustment-1.0.5/src/bias_adjustment/quantile_mapping/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-17 05:20:35.485008 bias_adjustment-1.0.5/src/bias_adjustment/quantile_mapping/dqm.py
--rw-r--r--   0        0        0     1206 2023-05-17 05:23:57.053434 bias_adjustment-1.0.5/src/bias_adjustment/quantile_mapping/qdm.py
--rw-r--r--   0        0        0     2779 2023-05-17 05:18:00.598322 bias_adjustment-1.0.5/src/bias_adjustment/quantile_mapping/qm.py
--rw-r--r--   0        0        0      647 2023-05-17 03:56:00.857244 bias_adjustment-1.0.5/src/bias_adjustment/utils.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 bias_adjustment-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-10 14:11:11.340594 bias_adjustment-1.0.6/LICENSE
+-rw-r--r--   0        0        0      274 2022-11-15 06:42:37.967412 bias_adjustment-1.0.6/README.md
+-rw-r--r--   0        0        0      705 2023-05-18 08:20:15.543487 bias_adjustment-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      205 2023-05-10 14:11:11.361595 bias_adjustment-1.0.6/src/bias_adjustment/__init__.py
+-rw-r--r--   0        0        0     2662 2023-05-17 05:38:22.798586 bias_adjustment-1.0.6/src/bias_adjustment/bias_adjustment.py
+-rw-r--r--   0        0        0       37 2023-05-17 03:12:37.290749 bias_adjustment-1.0.6/src/bias_adjustment/const.py
+-rw-r--r--   0        0        0       97 2023-05-10 14:11:11.361595 bias_adjustment-1.0.6/src/bias_adjustment/distributions/__init__.py
+-rw-r--r--   0        0        0     5103 2023-05-18 08:19:35.854057 bias_adjustment-1.0.6/src/bias_adjustment/distributions/distributions.py
+-rw-r--r--   0        0        0      300 2023-05-10 14:11:11.361595 bias_adjustment-1.0.6/src/bias_adjustment/quantile_mapping/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-17 05:20:35.485008 bias_adjustment-1.0.6/src/bias_adjustment/quantile_mapping/dqm.py
+-rw-r--r--   0        0        0     1206 2023-05-17 05:23:57.053434 bias_adjustment-1.0.6/src/bias_adjustment/quantile_mapping/qdm.py
+-rw-r--r--   0        0        0     2779 2023-05-17 05:18:00.598322 bias_adjustment-1.0.6/src/bias_adjustment/quantile_mapping/qm.py
+-rw-r--r--   0        0        0      647 2023-05-17 03:56:00.857244 bias_adjustment-1.0.6/src/bias_adjustment/utils.py
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 bias_adjustment-1.0.6/setup.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 bias_adjustment-1.0.6/PKG-INFO
```

### Comparing `bias_adjustment-1.0.5/LICENSE` & `bias_adjustment-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.5/pyproject.toml` & `bias_adjustment-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bias-adjustment"
-version = "1.0.5"
+version = "1.0.6"
 description = "Bias Adjusment by Quantile Mapping"
 authors = ["Emilio Gozo <emiliogozo@proton.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/emiliogozo/bias_adjustment"
 keywords = ["climatology", "data analysis", "quantile mapping", "bias correction"]
 packages = [{include = "bias_adjustment", from = "src"}]
```

### Comparing `bias_adjustment-1.0.5/src/bias_adjustment/bias_adjustment.py` & `bias_adjustment-1.0.6/src/bias_adjustment/bias_adjustment.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.5/src/bias_adjustment/distributions/distributions.py` & `bias_adjustment-1.0.6/src/bias_adjustment/distributions/distributions.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         if len(v) < min_len:
             raise ValueError(f"Length of `{v}` must be greater than {min_len}.")
 
     for v in [bins]:
         if not isinstance(v, int):
             raise TypeError(f"`{v}` is not an integer.")
 
-    h = np.histogram(data[~np.isnan(data)], bins=bins)
+    h = np.histogram(data[~np.isnan(data)], bins=bins, density=True)
     return st.rv_histogram(h)
 
 
 def _fit_dist(data: FloatNDArray, dist_type="gamma"):
     """Generate a distribution given a distribution type
 
     Args:
```

### Comparing `bias_adjustment-1.0.5/src/bias_adjustment/quantile_mapping/dqm.py` & `bias_adjustment-1.0.6/src/bias_adjustment/quantile_mapping/dqm.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.5/src/bias_adjustment/quantile_mapping/qdm.py` & `bias_adjustment-1.0.6/src/bias_adjustment/quantile_mapping/qdm.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.5/src/bias_adjustment/quantile_mapping/qm.py` & `bias_adjustment-1.0.6/src/bias_adjustment/quantile_mapping/qm.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.5/src/bias_adjustment/utils.py` & `bias_adjustment-1.0.6/src/bias_adjustment/utils.py`

 * *Files identical despite different names*

### Comparing `bias_adjustment-1.0.5/PKG-INFO` & `bias_adjustment-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bias-adjustment
-Version: 1.0.5
+Version: 1.0.6
 Summary: Bias Adjusment by Quantile Mapping
 Home-page: https://github.com/emiliogozo/bias_adjustment
 License: MIT
 Keywords: climatology,data analysis,quantile mapping,bias correction
 Author: Emilio Gozo
 Author-email: emiliogozo@proton.me
 Requires-Python: >=3.8.1,<3.9
```

