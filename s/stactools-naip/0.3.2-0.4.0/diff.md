# Comparing `tmp/stactools-naip-0.3.2.tar.gz` & `tmp/stactools-naip-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-naip-0.3.2.tar", last modified: Wed May  3 18:24:13 2023, max compression
+gzip compressed data, was "stactools-naip-0.4.0.tar", last modified: Thu May 18 19:54:37 2023, max compression
```

## Comparing `stactools-naip-0.3.2.tar` & `stactools-naip-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.544901 stactools-naip-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.544901 stactools-naip-0.3.2/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.548901 stactools-naip-0.3.2/src/stactools/naip/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/src/stactools/naip/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/src/stactools_naip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 18:24:13.000000 stactools-naip-0.3.2/src/stactools_naip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:13.552901 stactools-naip-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/tests/test_stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-03 18:23:50.000000 stactools-naip-0.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:37.606020 stactools-naip-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-18 19:54:37.606020 stactools-naip-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-18 19:54:37.606020 stactools-naip-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:37.602020 stactools-naip-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:37.602020 stactools-naip-0.4.0/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:37.606020 stactools-naip-0.4.0/src/stactools/naip/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/src/stactools/naip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/src/stactools/naip/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/src/stactools/naip/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/src/stactools/naip/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/src/stactools/naip/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:37.606020 stactools-naip-0.4.0/src/stactools_naip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-18 19:54:37.000000 stactools-naip-0.4.0/src/stactools_naip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-18 19:54:37.000000 stactools-naip-0.4.0/src/stactools_naip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:54:37.000000 stactools-naip-0.4.0/src/stactools_naip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 19:54:37.000000 stactools-naip-0.4.0/src/stactools_naip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 19:54:37.000000 stactools-naip-0.4.0/src/stactools_naip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:37.606020 stactools-naip-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/tests/test_stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-18 19:54:21.000000 stactools-naip-0.4.0/tests/test_utils.py
```

### Comparing `stactools-naip-0.3.2/LICENSE` & `stactools-naip-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.2/PKG-INFO` & `stactools-naip-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-naip
-Version: 0.3.2
+Version: 0.4.0
 Summary: PROVIDE DESCRIPTION HERE
 Home-page: https://github.com/stactools-naips/stactools-naip
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://stactools-naip.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stactools-naips/stactools-naip/issues
 Keywords: stactools,pystac,catalog,STAC
```

### Comparing `stactools-naip-0.3.2/README.md` & `stactools-naip-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.2/setup.cfg` & `stactools-naip-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.2/src/stactools/naip/commands.py` & `stactools-naip-0.4.0/src/stactools/naip/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.2/src/stactools/naip/constants.py` & `stactools-naip-0.4.0/src/stactools/naip/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.2/src/stactools/naip/stac.py` & `stactools-naip-0.4.0/src/stactools/naip/stac.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Final, List, Optional, Pattern
 
 import fsspec
 import pystac
 import rasterio as rio
 import shapely
 from lxml import etree
+from pystac import Item
 from pystac.extensions.eo import EOExtension
 from pystac.extensions.grid import GridExtension
 from pystac.extensions.item_assets import ItemAssetsExtension
 from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.raster import DataType, RasterBand, RasterExtension
 from pystac.extensions.scientific import CollectionScientificExtension, Publication
 from pystac.utils import str_to_datetime
@@ -105,15 +106,15 @@
 def create_item(
     state,
     year,
     cog_href,
     fgdc_metadata_href: Optional[str],
     thumbnail_href=None,
     additional_providers=None,
-):
+) -> Item:
     """Creates a STAC Item from NAIP data.
 
     Args:
         state (str): The 2-letter state code for the state this item belongs to.
         year (str): The NAIP year.
         fgdc_metadata_href (str): The href to the FGDC metadata
             for this NAIP scene. Optional, a some NAIP scenes to not have this
@@ -140,16 +141,16 @@
         geom = reproject_geom(
             ds.crs,
             "epsg:4326",
             shapely.geometry.mapping(shapely.geometry.box(*ds.bounds)),
             precision=6,
         )
 
-    if fgdc_metadata_href is not None:
-        if year == "2020":
+    if fgdc_metadata_href:
+        if year in ["2020", "2021"]:
             first_xpath = "gmd:fileIdentifier/gco:CharacterString"
 
             second_xpath = "idinfo/citation/citeinfo/title"
 
             with fsspec.open(fgdc_metadata_href) as file:
                 root = XmlElement(
                     etree.parse(file, base_url=fgdc_metadata_href).getroot()
```

### Comparing `stactools-naip-0.3.2/src/stactools/naip/utils.py` & `stactools-naip-0.4.0/src/stactools/naip/utils.py`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.2/src/stactools_naip.egg-info/PKG-INFO` & `stactools-naip-0.4.0/src/stactools_naip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-naip
-Version: 0.3.2
+Version: 0.4.0
 Summary: PROVIDE DESCRIPTION HERE
 Home-page: https://github.com/stactools-naips/stactools-naip
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://stactools-naip.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stactools-naips/stactools-naip/issues
 Keywords: stactools,pystac,catalog,STAC
```

### Comparing `stactools-naip-0.3.2/tests/test_commands.py` & `stactools-naip-0.4.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `stactools-naip-0.3.2/tests/test_stac.py` & `stactools-naip-0.4.0/tests/test_stac.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
 from datetime import datetime
 
 import pytest
 from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.raster import DataType, RasterExtension
 from pystac.extensions.scientific import CollectionScientificExtension
+from pystac.utils import datetime_to_str
 
 from stactools.naip.stac import create_collection, create_item
 from tests import test_data
 
 
 class StacTest(unittest.TestCase):
     def test_create_collection(self):
@@ -40,16 +41,15 @@
             self.assertEqual(raster_band.data_type, DataType.UINT8)
             self.assertEqual(raster_band.unit, "none")
 
         projection = ProjectionExtension.ext(item)
         projection.centroid["lat"] == pytest.approx(30.96876)
         projection.centroid["lon"] == pytest.approx(-85.90624)
 
-    # test stac on year = 2020
-    def test_create_item_xml(self):
+    def test_create_item_xml_2020(self):
         item = create_item(
             "tx",
             "2020",
             test_data.get_path(
                 "data-files/m_3610332_se_13_060_20200903-downsampled.tif"
             ),
             test_data.get_path("data-files/m_3610332_se_13_060_20200903_20201204.xml"),
@@ -63,14 +63,39 @@
             self.assertEqual(raster_band.spatial_resolution, item.properties["gsd"])
             self.assertEqual(raster_band.data_type, DataType.UINT8)
             self.assertEqual(raster_band.unit, "none")
 
         self.assertEqual(type(item.datetime), datetime)
         self.assertEqual(type(item.id), str)
 
+    def test_create_item_xml_2021(self):
+        item = create_item(
+            "va",
+            "2021",
+            test_data.get_path(
+                "data-files/m_3907864_sw_17_060_20210912_downsampled.tif"
+            ),
+            test_data.get_path("data-files/m_3907864_sw_17_060_20210912_20211220.xml"),
+        )
+
+        image_asset = item.assets["image"]
+        raster_ext = RasterExtension.ext(image_asset)
+        self.assertEqual(len(raster_ext.bands), 4)
+        for raster_band in RasterExtension.ext(image_asset).bands:
+            self.assertEqual(raster_band.nodata, 0)
+            self.assertEqual(raster_band.spatial_resolution, item.properties["gsd"])
+            self.assertEqual(raster_band.data_type, DataType.UINT8)
+            self.assertEqual(raster_band.unit, "none")
+
+        self.assertEqual(datetime_to_str(item.datetime), "2021-09-12T16:00:00Z")
+        self.assertEqual(item.id, "va_m_3907864_sw_17_060_20210912")
+        self.assertEqual(
+            item.properties["proj:centroid"], {"lat": 39.0315, "lon": -78.09348}
+        )
+
     # test stac on year 2011
     # resource description key is missing from the metadata
     def test_incorrect_metadata_txt(self):
         item = create_item(
             "al",
             "2011",
             test_data.get_path("data-files/m_3008501_ne_16_1_20110815.tif"),
```

### Comparing `stactools-naip-0.3.2/tests/test_utils.py` & `stactools-naip-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

