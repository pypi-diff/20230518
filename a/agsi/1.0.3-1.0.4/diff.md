# Comparing `tmp/agsi-1.0.3.tar.gz` & `tmp/agsi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.0.3.tar", last modified: Wed May 17 09:28:46 2023, max compression
+gzip compressed data, was "agsi-1.0.4.tar", last modified: Thu May 18 10:06:10 2023, max compression
```

## Comparing `agsi-1.0.3.tar` & `agsi-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:28:46.762694 agsi-1.0.3/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       46 2023-05-17 09:19:08.000000 agsi-1.0.3/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-17 09:28:46.762694 agsi-1.0.3/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.3/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:28:46.762694 agsi-1.0.3/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.3/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:28:46.762694 agsi-1.0.3/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    12758 2023-05-17 09:27:46.000000 agsi-1.0.3/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.3/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.3/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.3/agsi/main.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:28:46.762694 agsi-1.0.3/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      261 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-17 09:28:46.000000 agsi-1.0.3/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-17 09:28:46.762694 agsi-1.0.3/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-17 09:28:43.000000 agsi-1.0.3/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-17 09:39:46.000000 agsi-1.0.4/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-18 10:06:10.523172 agsi-1.0.4/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.0.4/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.0.4/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    13918 2023-05-18 10:00:01.000000 agsi-1.0.4/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.0.4/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.0.4/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)   970300 2023-05-18 10:02:54.000000 agsi-1.0.4/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.0.4/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.0.4/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      214 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      325 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-18 10:06:10.000000 agsi-1.0.4/agsi.egg-info/top_level.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-18 10:06:10.523172 agsi-1.0.4/dist/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     7045 2023-05-17 09:28:46.000000 agsi-1.0.4/dist/agsi-1.0.3.tar.gz
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-18 10:06:10.523172 agsi-1.0.4/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      369 2023-05-18 10:05:58.000000 agsi-1.0.4/setup.py
```

### Comparing `agsi-1.0.3/README.md` & `agsi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `agsi-1.0.3/agsi/data/FarmData.py` & `agsi-1.0.4/agsi/data/FarmData.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,29 @@
     for farm_id,farm_properties in self.farms_info.items():
       all_blocks={}
       for block_id,block_properties in self.blocks_info.items():
          if block_properties['farm_id']==farm_id:
             all_blocks[block_id]=self.blocks[block_id]
       all_farms[farm_id]=Farm(farm_properties,all_blocks)
     return all_farms 
-
+  
+  def get_farm_by_name(self,farm_name):
+     
+     for farm_key,farm_obj in self.farms_info.items():
+        
+        if farm_obj['owner']==farm_name:
+           return farm_obj
+        
+  def get_block_by_name(self,block_name):
+    
+    for block_key,block_obj in self.farms_info.items():
+      
+      if block_obj['block_name']==block_name:
+          return block_obj 
+        
   def __get_block_objects__(self):
 
     all_blocks={}
     for block_id,properties in self.blocks_info.items():
       farm_id=properties['farm_id']
       all_blocks[block_id]=Block(properties,self.farms_info[farm_id])
     return all_blocks        
@@ -77,30 +91,34 @@
           # Iterate through rows and populate modalities and data fields
           for row in reader:
               info = {'owner': None, 'area': None,'data_path': {}}
               info['owner'] = row['farm_name']
               info['farm_id'] =row['farm_id']
               info['area'] = None
               timestamp=row['time']
+              
               info['data_path'][timestamp]={}
               for column in row:
                   # Check if the column name contains 'drone_' and get the resolution from the column name
                   if 'drone_' in column:
-                      resolution = column
-                      if resolution not in info['data_path'][row['time']]:
-                          info['data_path'][timestamp][resolution] = row[resolution]
+                      modality = column
+                      if modality not in info['data_path'][timestamp]:
+                          info['data_path'][timestamp][modality] = row[modality]
                   # Check if the column name contains 'sat_' and add the timestamp and image_path to satellite data
                   elif 'sat_' in column:
                       if row[column]:
                           image_path = row[column]
                           image_path = convert_path(image_path)
                           if column not in info['data_path'][timestamp]:
                               info['data_path'][timestamp][column]=image_path
-                              
-              all_info[info['farm_id']]=info        
+
+              if info['farm_id'] in all_info:      
+                all_info[info['farm_id']]['data_path'][timestamp]=info['data_path'][timestamp]
+              else:
+                all_info[info['farm_id']]=info
 
       return all_info
   
   def __get_blocks_info__(self,block_csv_path):
         # Open CSV file
         with open(block_csv_path, newline='') as csvfile:
             reader = csv.DictReader(csvfile)
@@ -176,15 +194,15 @@
           crs (str): The Coordinate Reference System (CRS) for the geospatial data.
     """  
 
     self.info=farm_info
     self.farm_id=self.info['farm_id']
     self.blocks=blocks          
 
-  def get_modality(self,modality_type="drone_75",timestamp=None,shp_clip=False):
+  def get_modality(self,modality_type="drone_75",timestamp=None,shp_clip=False,only_rgb=False):
 
     """
       Retrieves a specific modality (e.g., drone or satellite) for the farm.
 
       Args:
           modality_type (str, optional): The type of modality (e.g., "drone" or "satellite"). Defaults to "drone".
           resolution (int, optional): The resolution of the modality. Defaults to 75.
@@ -197,22 +215,24 @@
      """
 
     if not shp_clip:
 
       farm_image_path=self.info['data_path'][timestamp][modality_type]
       farm_image_path=convert_path(farm_image_path)
       raster=open_tiff(farm_image_path)
-      return raster
-    
+      if only_rgb:
+        return raster.read([1,2,3])
+      else:
+         return raster
     else: #to be implemented when accessing satellite images not in use right now.
 
       shp_file=self.farm_df[self.farm_df["farm_id"]==self.farm_id]["shp_file"].values[0]
       polygon=open_tiff(shp_file)['geometry'].values[0]
       clipped_chip=get_clipped_chip(self.full_image_path,[polygon])
-      return clipped_chip,self.block 
+      return clipped_chip,self.block
 
   def visualize_blocks(self,modality_type="drone",resolution=75,timestamp=None):
 
     """
   Displays the farm image with the block polygons overlaid.
 
   Args:
@@ -234,14 +254,37 @@
     farm_image_path=self.info['data_path'][timestamp][modality_type]
     src=rasterio.open(farm_image_path)
     ax = rasterio.plot.show(src,ax=ax, cmap="pink")
     all_polygon_df.plot(ax=ax)
     patches = [PolygonPatch(feature) for feature in all_polygons]
     ax.add_collection(mpl.collections.PatchCollection(patches))  
 
+  def get_times(self):
+     times = self.info['data_path'].keys()
+     return list(times)
+  
+  def get_modalities_for_times(self,time):
+      
+      valid_mods=[]
+      modalities=list(self.info['data_path'][time].keys())
+      for mods in modalities:
+         if self.info['data_path'][time][mods]!="":
+            valid_mods.append(mods)
+
+      return valid_mods
+
+  def get_block_by_name(self,block_name):
+  
+    for block_key,block_obj in self.blocks.items():
+      if block_obj.info['block_name']==block_name:
+          return block_obj      
+            
+
+
+
     
 class Block():
 
   def __init__(self,block_info,farm_info):
       
       """
         A subclass of FarmData that represents a block and provides methods to access and manipulate block information.
```

### Comparing `agsi-1.0.3/agsi/data/utils.py` & `agsi-1.0.4/agsi/data/utils.py`

 * *Files identical despite different names*

