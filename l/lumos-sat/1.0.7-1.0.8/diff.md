# Comparing `tmp/lumos-sat-1.0.7.tar.gz` & `tmp/lumos-sat-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumos-sat-1.0.7.tar", last modified: Fri May  5 00:09:14 2023, max compression
+gzip compressed data, was "lumos-sat-1.0.8.tar", last modified: Thu May 18 18:37:42 2023, max compression
```

## Comparing `lumos-sat-1.0.7.tar` & `lumos-sat-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 00:09:14.761242 lumos-sat-1.0.7/
--rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      834 2023-05-05 00:09:14.749334 lumos-sat-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 00:09:14.677888 lumos-sat-1.0.7/lumos/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.7/lumos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:09:14.687417 lumos-sat-1.0.7/lumos/brdf/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.7/lumos/brdf/__init__.py
--rw-rw-rw-   0        0        0     6648 2023-05-02 20:42:09.000000 lumos-sat-1.0.7/lumos/brdf/library.py
--rw-rw-rw-   0        0        0     3255 2023-05-03 21:42:13.000000 lumos-sat-1.0.7/lumos/brdf/tools.py
--rw-rw-rw-   0        0        0    14276 2023-05-03 22:10:42.000000 lumos-sat-1.0.7/lumos/calculator.py
--rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.7/lumos/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:09:14.695948 lumos-sat-1.0.7/lumos/constellation/
--rw-rw-rw-   0        0        0        0 2023-05-02 20:49:52.000000 lumos-sat-1.0.7/lumos/constellation/__init__.py
--rw-rw-rw-   0        0        0     5105 2023-05-03 19:16:32.000000 lumos-sat-1.0.7/lumos/constellation/library.py
--rw-rw-rw-   0        0        0     1088 2023-05-03 19:16:14.000000 lumos-sat-1.0.7/lumos/constellation/tools.py
--rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.7/lumos/conversions.py
--rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.7/lumos/functions.py
--rw-rw-rw-   0        0        0     3971 2023-05-01 19:53:20.000000 lumos-sat-1.0.7/lumos/geometry.py
--rw-rw-rw-   0        0        0     9728 2023-05-03 22:36:00.000000 lumos-sat-1.0.7/lumos/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:09:14.748338 lumos-sat-1.0.7/lumos_sat.egg-info/
--rw-rw-rw-   0        0        0      834 2023-05-05 00:09:14.000000 lumos-sat-1.0.7/lumos_sat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-05-05 00:09:14.000000 lumos-sat-1.0.7/lumos_sat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 00:09:14.000000 lumos-sat-1.0.7/lumos_sat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      246 2023-05-05 00:09:14.000000 lumos-sat-1.0.7/lumos_sat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-05 00:09:14.000000 lumos-sat-1.0.7/lumos_sat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      630 2023-05-05 00:08:23.000000 lumos-sat-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 00:09:14.762248 lumos-sat-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.724074 lumos-sat-1.0.8/
+-rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-05-18 18:37:42.722095 lumos-sat-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.680190 lumos-sat-1.0.8/lumos/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.8/lumos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.689167 lumos-sat-1.0.8/lumos/brdf/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.8/lumos/brdf/__init__.py
+-rw-rw-rw-   0        0        0     6648 2023-05-02 20:42:09.000000 lumos-sat-1.0.8/lumos/brdf/library.py
+-rw-rw-rw-   0        0        0     3255 2023-05-17 23:11:16.000000 lumos-sat-1.0.8/lumos/brdf/tools.py
+-rw-rw-rw-   0        0        0    14276 2023-05-03 22:10:42.000000 lumos-sat-1.0.8/lumos/calculator.py
+-rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.8/lumos/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.697145 lumos-sat-1.0.8/lumos/constellation/
+-rw-rw-rw-   0        0        0        0 2023-05-02 20:49:52.000000 lumos-sat-1.0.8/lumos/constellation/__init__.py
+-rw-rw-rw-   0        0        0     5105 2023-05-03 19:16:32.000000 lumos-sat-1.0.8/lumos/constellation/library.py
+-rw-rw-rw-   0        0        0     1088 2023-05-03 19:16:14.000000 lumos-sat-1.0.8/lumos/constellation/tools.py
+-rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.8/lumos/conversions.py
+-rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.8/lumos/functions.py
+-rw-rw-rw-   0        0        0     3875 2023-05-12 20:46:28.000000 lumos-sat-1.0.8/lumos/geometry.py
+-rw-rw-rw-   0        0        0     9728 2023-05-18 18:18:47.000000 lumos-sat-1.0.8/lumos/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-18 18:37:42.720089 lumos-sat-1.0.8/lumos_sat.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-18 18:37:42.000000 lumos-sat-1.0.8/lumos_sat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-18 18:37:42.000000 lumos-sat-1.0.8/lumos_sat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 18:37:42.000000 lumos-sat-1.0.8/lumos_sat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      246 2023-05-18 18:37:42.000000 lumos-sat-1.0.8/lumos_sat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 18:37:42.000000 lumos-sat-1.0.8/lumos_sat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      630 2023-05-18 18:16:41.000000 lumos-sat-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 18:37:42.724074 lumos-sat-1.0.8/setup.cfg
```

### Comparing `lumos-sat-1.0.7/LICENSE` & `lumos-sat-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/PKG-INFO` & `lumos-sat-1.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.7
+Version: 1.0.8
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.7/README.md` & `lumos-sat-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/lumos/brdf/library.py` & `lumos-sat-1.0.8/lumos/brdf/library.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/lumos/brdf/tools.py` & `lumos-sat-1.0.8/lumos/brdf/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     """
     Fits a model to experimental data.
 
     :param data_file: A path to a .csv file containing BRDF data. DESCRIBE FORMAT.
     :type data_file: str
     :param model_func: A BRDF model to fit
     :type model_func: function
-    :param bounds: Bounds passed to :function:`scipy.optimize.curve_fit`
+    :param bounds: Bounds passed to :py:func:`scipy.optimize.curve_fit`
     :type bounds: tuple
-    :param p0: Initial guess for parameters passed to :function:`scipy.optimize.curve_fit`
+    :param p0: Initial guess for parameters passed to :py:func:`scipy.optimize.curve_fit`
     :type p0: tuple
     :param log_space: Whether or not to fit BRDF in log_space
     :type log_space: bool
     :param clip: Removes BRDF data below this cutoff from fitting
     :type clip: float
     """
 
@@ -106,8 +106,8 @@
     :type params: list[float]
     :return: B, C, d
     :rtype: :class:`np.ndarray`, :class:`np.ndarray`, float
     """
     params = np.array(params)
     B = np.reshape( params[:n * m], (n, m) )
     C = np.reshape( params[n * m:], (n, l2 - l1))
-    return B, C
+    return B, C
```

### Comparing `lumos-sat-1.0.7/lumos/calculator.py` & `lumos-sat-1.0.8/lumos/calculator.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/lumos/constellation/library.py` & `lumos-sat-1.0.8/lumos/constellation/library.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/lumos/constellation/tools.py` & `lumos-sat-1.0.8/lumos/constellation/tools.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/lumos/conversions.py` & `lumos-sat-1.0.8/lumos/conversions.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/lumos/functions.py` & `lumos-sat-1.0.8/lumos/functions.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/lumos/geometry.py` & `lumos-sat-1.0.8/lumos/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,13 +93,10 @@
         
         angles_off_plane = np.linspace(-self.max_angle, self.max_angle, density)
         angles_on_plane = np.linspace(-self.max_angle, self.min_angle, density)
         
         super().__init__(angles_off_plane, angles_on_plane)
     
     def __iter__(self):
-        """
-        Iteration Method
-        """
         for i in range(self.shape[0]):
             for j in range(self.shape[1]):
-                yield i, j, (self.x[i, j], self.y[i, j], self.z[i, j])
+                yield i, j
```

### Comparing `lumos-sat-1.0.7/lumos/plot.py` & `lumos-sat-1.0.8/lumos/plot.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.7/lumos_sat.egg-info/PKG-INFO` & `lumos-sat-1.0.8/lumos_sat.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.7
+Version: 1.0.8
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.7/pyproject.toml` & `lumos-sat-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lumos-sat"
-version = "1.0.7"
+version = "1.0.8"
 description = "Satellite Brightness Calculation Tools"
 authors = [
     {name = "Forrest Fankhauser", email = "fafankhauser@ucdavis.edu"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
```

