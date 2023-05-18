# Comparing `tmp/dea-tools-0.2.8.dev94.tar.gz` & `tmp/dea-tools-0.2.8.dev95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dea-tools-0.2.8.dev94.tar", last modified: Wed May 17 01:17:15 2023, max compression
+gzip compressed data, was "dea-tools-0.2.8.dev95.tar", last modified: Thu May 18 10:10:20 2023, max compression
```

## Comparing `dea-tools-0.2.8.dev94.tar` & `dea-tools-0.2.8.dev95.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:17:15.453630 dea-tools-0.2.8.dev94/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-17 01:17:15.453630 dea-tools-0.2.8.dev94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:17:15.449630 dea-tools-0.2.8.dev94/dea_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:17:15.453630 dea-tools-0.2.8.dev94/dea_tools/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32250 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/app/miningrehab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/bom.py
--rw-r--r--   0 runner    (1001) docker     (123)    62213 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)    60087 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    51764 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (123)    39758 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/landcover.py
--rw-r--r--   0 runner    (1001) docker     (123)    37726 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/pyfes_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/dea_tools/waterbodies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:17:15.449630 dea-tools-0.2.8.dev94/dea_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-17 01:17:13.000000 dea-tools-0.2.8.dev94/dea_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-17 01:17:15.000000 dea-tools-0.2.8.dev94/dea_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:17:13.000000 dea-tools-0.2.8.dev94/dea_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 01:17:13.000000 dea-tools-0.2.8.dev94/dea_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 01:17:13.000000 dea-tools-0.2.8.dev94/dea_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 01:17:15.453630 dea-tools-0.2.8.dev94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-17 01:14:59.000000 dea-tools-0.2.8.dev94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.353197 dea-tools-0.2.8.dev95/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-18 10:10:20.353197 dea-tools-0.2.8.dev95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.349197 dea-tools-0.2.8.dev95/dea_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.353197 dea-tools-0.2.8.dev95/dea_tools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32250 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/changefilmstrips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/crophealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/deacoastlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/imageexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/miningrehab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/app/widgetconstructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/bandindices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/bom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62213 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60087 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/coastal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51764 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/datahandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39758 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/landcover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37726 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/pyfes_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/dea_tools/waterbodies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:10:20.349197 dea-tools-0.2.8.dev95/dea_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-18 10:10:18.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-18 10:10:20.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:10:18.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-18 10:10:18.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 10:10:18.000000 dea-tools-0.2.8.dev95/dea_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 10:10:20.353197 dea-tools-0.2.8.dev95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-18 10:08:13.000000 dea-tools-0.2.8.dev95/setup.py
```

### Comparing `dea-tools-0.2.8.dev94/LICENSE` & `dea-tools-0.2.8.dev95/LICENSE`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/PKG-INFO` & `dea-tools-0.2.8.dev95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev94
+Version: 0.2.8.dev95
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: earth.observation@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.2.8.dev94/README.rst` & `dea-tools-0.2.8.dev95/README.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/app/animations.py` & `dea-tools-0.2.8.dev95/dea_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/app/changefilmstrips.py` & `dea-tools-0.2.8.dev95/dea_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/app/crophealth.py` & `dea-tools-0.2.8.dev95/dea_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/app/deacoastlines.py` & `dea-tools-0.2.8.dev95/dea_tools/app/deacoastlines.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,33 +280,38 @@
     ######################################
 
     # Set the output csv
     def update_fileupload_transects(self, change):
 
         # Clear any drawn data if present
         self.gdf_drawn = None
+        
+        # Temporary compatibility fix for ipywidget > 8.0
+        # TODO: Update code to use new fileupload API documented here:
+        # https://ipywidgets.readthedocs.io/en/latest/user_migration_guides.html#fileupload
+        uploaded_data = {f["name"]: {"content": f.content.tobytes()} for f in change.new}            
 
         # Save to file
-        for uploaded_filename in change.new.keys():
+        for uploaded_filename in uploaded_data.keys():
             with open(uploaded_filename, "wb") as output_file:
-                content = change.new[uploaded_filename]['content']
+                content = uploaded_data[uploaded_filename]["content"]
                 output_file.write(content)
 
         with self.status_info:
 
             try:            
 
                 print('Loading vector data...', end='\r')
                 valid_files = [
-                    file for file in change.new.keys()
+                    file for file in uploaded_data.keys()
                     if file.lower().endswith(('.shp', '.geojson'))
                 ]
                 valid_file = valid_files[0]
                 transect_gdf = (gpd.read_file(valid_file).to_crs(
-                    "EPSG:4326").explode().reset_index(drop=True))
+                    "EPSG:4326").explode(index_parts=True).reset_index(drop=True))
 
                 # Use ID column if it exists
                 if 'id' in transect_gdf:
                     transect_gdf = transect_gdf.set_index('id')
                     print(f"Uploaded '{valid_file}'; automatically labelling "
                           "transects using column 'id'.")
                 else:
@@ -369,15 +374,15 @@
         deacl_url = WMS_ADDRESS
         deacl_layer = "dea:DEACoastlines"
         deacoastlines = WMSLayer(
             url=deacl_url,
             layers=deacl_layer,
             format="image/png",
             transparent=True,
-            attribution="DEA Coastlines © 2020 Geoscience Australia")
+            attribution="DEA Coastlines © 2023 Geoscience Australia")
 
         if self.product == "none":
             self.map_layers.clear_layers()
             self.map_layers.add_layer(deacoastlines)
 
         elif self.product == "open_street_map":
             self.map_layers.clear_layers()
@@ -496,8 +501,8 @@
                         print(
                             "No valid shoreline data intersects with the "
                             "supplied transect. This can occur if:\n\n"
                             " - the transect does not intersect with any shorelines\n"
                             " - the transect intersects with shorelines more than once in 'distance' mode\n"
                             " - the transect intersects with shorelines only once in 'width' mode\n\n"
                             "Please draw or upload a new transect.",
-                            end='\r')
+                            end='\r')
```

### Comparing `dea-tools-0.2.8.dev94/dea_tools/app/imageexport.py` & `dea-tools-0.2.8.dev95/dea_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/app/miningrehab.py` & `dea-tools-0.2.8.dev95/dea_tools/app/miningrehab.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/app/widgetconstructors.py` & `dea-tools-0.2.8.dev95/dea_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/bandindices.py` & `dea-tools-0.2.8.dev95/dea_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/bom.py` & `dea-tools-0.2.8.dev95/dea_tools/bom.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/classification.py` & `dea-tools-0.2.8.dev95/dea_tools/classification.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/climate.py` & `dea-tools-0.2.8.dev95/dea_tools/climate.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/coastal.py` & `dea-tools-0.2.8.dev95/dea_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/dask.py` & `dea-tools-0.2.8.dev95/dea_tools/dask.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/datahandling.py` & `dea-tools-0.2.8.dev95/dea_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/landcover.py` & `dea-tools-0.2.8.dev95/dea_tools/landcover.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/plotting.py` & `dea-tools-0.2.8.dev95/dea_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/pyfes_model.py` & `dea-tools-0.2.8.dev95/dea_tools/pyfes_model.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/spatial.py` & `dea-tools-0.2.8.dev95/dea_tools/spatial.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/temporal.py` & `dea-tools-0.2.8.dev95/dea_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/validation.py` & `dea-tools-0.2.8.dev95/dea_tools/validation.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools/waterbodies.py` & `dea-tools-0.2.8.dev95/dea_tools/waterbodies.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/dea_tools.egg-info/PKG-INFO` & `dea-tools-0.2.8.dev95/dea_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev94
+Version: 0.2.8.dev95
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
 Author-email: earth.observation@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dea-tools-0.2.8.dev94/dea_tools.egg-info/SOURCES.txt` & `dea-tools-0.2.8.dev95/dea_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/index.rst` & `dea-tools-0.2.8.dev95/index.rst`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev94/setup.py` & `dea-tools-0.2.8.dev95/setup.py`

 * *Files identical despite different names*

