# Comparing `tmp/titiler.extensions-0.11.6.tar.gz` & `tmp/titiler.extensions-0.11.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.extensions-0.11.6.tar", last modified: Mon Apr 17 11:02:26 2023, max compression
+gzip compressed data, was "titiler.extensions-0.11.7.tar", last modified: Thu May 18 16:08:14 2023, max compression
```

## Comparing `titiler.extensions-0.11.6.tar` & `titiler.extensions-0.11.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4700 2023-04-17 11:01:43.800545 titiler.extensions-0.11.6/README.md
--rw-r--r--   0        0        0     1656 2023-04-17 11:01:43.800545 titiler.extensions-0.11.6/pyproject.toml
--rw-r--r--   0        0        0      244 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/__init__.py
--rw-r--r--   0        0        0     1011 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/cogeo.py
--rw-r--r--   0        0        0     5274 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/stac.py
--rw-r--r--   0        0        0    29081 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/cog_index.html
--rw-r--r--   0        0        0    33552 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/stac_index.html
--rw-r--r--   0        0        0     2231 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.0.0.xml
--rw-r--r--   0        0        0     2715 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.1.1.xml
--rw-r--r--   0        0        0     3452 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.3.0.xml
--rw-r--r--   0        0        0     2320 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/viewer.py
--rw-r--r--   0        0        0    20973 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/wms.py
--rw-r--r--   0        0        0     5828 1970-01-01 00:00:00.000000 titiler.extensions-0.11.6/PKG-INFO
+-rw-r--r--   0        0        0     4700 2023-05-18 16:07:25.370668 titiler.extensions-0.11.7/README.md
+-rw-r--r--   0        0        0     1656 2023-05-18 16:07:25.370668 titiler.extensions-0.11.7/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/__init__.py
+-rw-r--r--   0        0        0     1011 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/cogeo.py
+-rw-r--r--   0        0        0     5274 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/stac.py
+-rw-r--r--   0        0        0    30665 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/cog_viewer.html
+-rw-r--r--   0        0        0    35135 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/stac_viewer.html
+-rw-r--r--   0        0        0     2231 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.0.0.xml
+-rw-r--r--   0        0        0     2715 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.1.1.xml
+-rw-r--r--   0        0        0     3452 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.3.0.xml
+-rw-r--r--   0        0        0     2194 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/viewer.py
+-rw-r--r--   0        0        0    20787 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/wms.py
+-rw-r--r--   0        0        0     5828 1970-01-01 00:00:00.000000 titiler.extensions-0.11.7/PKG-INFO
```

### Comparing `titiler.extensions-0.11.6/README.md` & `titiler.extensions-0.11.7/README.md`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.6/pyproject.toml` & `titiler.extensions-0.11.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = []
 dependencies = [
-    "titiler.core==0.11.6",
+    "titiler.core==0.11.7",
 ]
-version = "0.11.6"
+version = "0.11.7"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 test = [
     "pytest",
```

### Comparing `titiler.extensions-0.11.6/titiler/extensions/cogeo.py` & `titiler.extensions-0.11.7/titiler/extensions/cogeo.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.6/titiler/extensions/stac.py` & `titiler.extensions-0.11.7/titiler/extensions/stac.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.6/titiler/extensions/templates/cog_index.html` & `titiler.extensions-0.11.7/titiler/extensions/templates/cog_viewer.html`

 * *Files 0% similar despite different names*

```diff
@@ -252,14 +252,32 @@
         <div id="minmax-data" class='px6 py6 none'>
           <div class='txt-h5 mb6 color-black'><svg class='icon icon--l inline-block'><use xlink:href='#icon-smooth-ramp'/></svg> Rescale</div>
           <input id="data-min" class='input input--s w120-ml w60 inline-block align-center color-black' value='0' />
           <input id="data-max" class='input input--s w120-ml w60 inline-block align-center color-black' value='0' />
           <button id="btn-rescale" class='btn bts--xs btn--stroke bg-darken25-on-hover inline-block txt-s color-black mt6'>Apply</button>
         </div>
 
+        <!-- Zoom to point -->
+        <div class="px6 py6 w-full">
+          <div class='txt-h5 color-black'><svg class='icon icon--l inline-block'><use xlink:href='#icon-marker'/></svg> Zoom to point</div>
+          <form class='grid grid--gut12 mx12 mt12' id="zoom-to-point-form">
+            <div class="col">
+              <label for="zoomLng" class='row'>Longitude:</label>
+              <input name="zoomLng" id="zoomLng" type="number" class="input input--s row" min="-180" max="180" required/>
+            </div>
+            <div class="col">
+              <label for="zoomLat" class='row'>Latitude:</label>
+              <input name="zoomLat" id="zoomLat" type="number" class="input input--s row" min="-90" max="90" required/>
+            </div>
+            <div id='zoom-to-point-div' class='w-full align-center'>
+              <button type="submit" class='btn bts--xs btn--stroke bg-darken25-on-hover inline-block txt-s color-black mx12 my12'>Zoom to point</button>
+            </div>
+          </form>
+        </div>
+
         <!-- Histogram -->
         <div class='px6 py6 w-full'>
           <div class='txt-h5 color-black'><svg class='icon icon--l inline-block'><use xlink:href='#icon-graph'/></svg> Histogram</div>
           <div id='fetch-stats-div' class='w-full align-center'>
             <button id="btn-stats" class='btn bts--xs btn--stroke bg-darken25-on-hover inline-block txt-s color-black mx12 my12'>Get Dataset Statistics</button>
           </div>
           <div id="histogram" class="w-full h120 h240-ml relative loading none"></div>
@@ -450,14 +468,18 @@
       set3bViz()
       break
     default:
       throw new Error(`Invalid ${rasterType}`)
   }
 }
 
+const addZoomToPoint = () => {
+
+}
+
 const addHisto3Bands = () => {
   const r = document.getElementById('r-selector').selectedOptions[0].getAttribute("bname")
   const g = document.getElementById('g-selector').selectedOptions[0].getAttribute("bname")
   const b = document.getElementById('b-selector').selectedOptions[0].getAttribute("bname")
 
   const rStats = scope.dataset_statistics[r]
   const gStats = scope.dataset_statistics[g]
@@ -648,14 +670,37 @@
         let text = document.createTextNode(element[key]);
         cell.appendChild(text);
       }
     }
     table.classList.remove('none')
 }
 
+let centerMarker;
+
+document.getElementById('zoom-to-point-form').addEventListener('submit', (e) => {
+  e.preventDefault()
+  if (map) {
+    let lng = document.getElementById('zoomLng').value
+    let lat = document.getElementById('zoomLat').value
+    map.flyTo({
+      center: [lng, lat],
+      zoom: 10,
+      essential: false
+    });
+
+    if (!centerMarker) {
+      centerMarker = new mapboxgl.Marker()
+      .setLngLat([lng, lat])
+      .addTo(map);
+    } else {
+      centerMarker.setLngLat([lng, lat])
+    }
+  }
+})
+
 document.getElementById('btn-stats').addEventListener('click', () => {
   document.getElementById('fetch-stats-div').classList.add('none')
   document.getElementById('histogram').classList.remove('none')
   document.getElementById('histogram-table').classList.remove('none')
 
   fetch(`${stats_endpoint}?url=${scope.url}&max_size=256`)
     .then(res => {
```

#### html2text {}

```diff
@@ -8,10 +8,14 @@
  Layers
 Color Map
 [One of: Internal/CFastie/RPlumbo/Schwarzwald (elevation)/Viridis/Blue-Red/
 Blue-Green/Yellow-Green/Magma/Earth/Ocean/Terrain]
 
 Rescale
 [0                   ] [0                   ] Apply
+Zoom to point
+Longitude: [Unknown INPUT type]
+Latitude: [Unknown INPUT type]
+Zoom to point
 Histogram
 Get Dataset Statistics
```

### Comparing `titiler.extensions-0.11.6/titiler/extensions/templates/stac_index.html` & `titiler.extensions-0.11.7/titiler/extensions/templates/stac_viewer.html`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,32 @@
 
         <div id='cformula-section' class='px6 py6'>
           <div class='txt-h5 mb6 color-black'>Color Formula</div>
           <input id="ColorFormulaValue" class='input input--s w-full color-black' value='' />
           <button id="updateColor" class='btn bts--xs btn--stroke bg-darken25-on-hover txt-s color-black mt6'>Apply</button>
         </div>
 
+        <!-- Zoom to point -->
+        <div class="px6 py6 w-full">
+          <div class='txt-h5 color-black'><svg class='icon icon--l inline-block'><use xlink:href='#icon-marker'/></svg> Zoom to point</div>
+          <form class='grid grid--gut12 mx12 mt12' id="zoom-to-point-form">
+            <div class="col">
+              <label for="zoomLng" class='row'>Longitude:</label>
+              <input name="zoomLng" id="zoomLng" type="number" class="input input--s row" min="-180" max="180" required/>
+            </div>
+            <div class="col">
+              <label for="zoomLat" class='row'>Latitude:</label>
+              <input name="zoomLat" id="zoomLat" type="number" class="input input--s row" min="-90" max="90" required/>
+            </div>
+            <div id='zoom-to-point-div' class='w-full align-center'>
+              <button type="submit" class='btn bts--xs btn--stroke bg-darken25-on-hover inline-block txt-s color-black mx12 my12'>Zoom to point</button>
+            </div>
+          </form>
+        </div>
+
         <!-- Histogram -->
         <div class='px6 py6 w-full'>
           <div class='txt-h5 color-black'><svg class='icon icon--l inline-block'><use xlink:href='#icon-graph'/></svg> Histogram</div>
           <div id='fetch-stats-div' class='w-full align-center'>
           <button id="btn-stats" class='btn bts--xs btn--stroke bg-darken25-on-hover inline-block txt-s color-black mx12 my12'>Get Dataset Statistics</button>
           </div>
           <div id="histogram" class="w-full h120 h240-ml relative loading none"></div>
@@ -655,14 +673,38 @@
     .attr('x', 1)
     .attr('transform', d => { return 'translate(' + x(d.value) + ',' + y(d.count) + ')' })
     .attr('width', 10)
     .attr('height', d => { return height - y(d.count) })
     .style('fill', '#69b3a2')
 }
 
+let centerMarker;
+
+document.getElementById('zoom-to-point-form').addEventListener('submit', (e) => {
+  e.preventDefault()
+  if (map) {
+    let lng = document.getElementById('zoomLng').value
+    let lat = document.getElementById('zoomLat').value
+    console.log(`${lng}, ${lat}`)
+    map.flyTo({
+      center: [lng, lat],
+      zoom: 10,
+      essential: false
+    });
+
+    if (!centerMarker) {
+      centerMarker = new mapboxgl.Marker()
+      .setLngLat([lng, lat])
+      .addTo(map);
+    } else {
+      centerMarker.setLngLat([lng, lat])
+    }
+  }
+})
+
 document.getElementById('btn-stats').addEventListener('click', () => {
   document.getElementById('fetch-stats-div').classList.add('none')
   document.getElementById('histogram').classList.remove('none')
   document.getElementById('histogram-table').classList.remove('none')
 
   fetch(`${stats_endpoint}?url=${scope.url}&max_size=256`)
     .then(res => {
```

#### html2text {}

```diff
@@ -13,9 +13,13 @@
 [One of: Internal/CFastie/RPlumbo/Schwarzwald (elevation)/Viridis/Blue-Red/
 Blue-Green/Yellow-Green/Magma/Earth/Ocean/Terrain]
 
 Rescale
 [0                   ] [0                   ] Apply
 Color Formula
 [                    ] Apply
+Zoom to point
+Longitude: [Unknown INPUT type]
+Latitude: [Unknown INPUT type]
+Zoom to point
 Histogram
 Get Dataset Statistics
```

### Comparing `titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.0.0.xml` & `titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.0.0.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.1.1.xml` & `titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.1.1.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.3.0.xml` & `titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.3.0.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.6/titiler/extensions/viewer.py` & `titiler.extensions-0.11.7/titiler/extensions/viewer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 """titiler Viewer Extensions."""
 
 from dataclasses import dataclass
 
+import jinja2
 from starlette.requests import Request
 from starlette.responses import HTMLResponse
 from starlette.templating import Jinja2Templates
 
 from titiler.core.factory import BaseTilerFactory, FactoryExtension
 
-try:
-    from importlib.resources import files as resources_files  # type: ignore
-except ImportError:
-    # Try backported to PY<39 `importlib_resources`.
-    from importlib_resources import files as resources_files  # type: ignore
-
-# TODO: mypy fails in python 3.9, we need to find a proper way to do this
-templates = Jinja2Templates(directory=str(resources_files(__package__) / "templates"))  # type: ignore
+DEFAULT_TEMPLATES = Jinja2Templates(
+    directory="",
+    loader=jinja2.ChoiceLoader([jinja2.PackageLoader(__package__, "templates")]),
+)  # type:ignore
 
 
 @dataclass
 class cogViewerExtension(FactoryExtension):
     """Add /viewer endpoint to the TilerFactory."""
 
+    templates: Jinja2Templates = DEFAULT_TEMPLATES
+
     def register(self, factory: BaseTilerFactory):
         """Register endpoint to the tiler factory."""
 
         @factory.router.get("/viewer", response_class=HTMLResponse)
         def cog_viewer(request: Request):
             """COG Viewer."""
-            return templates.TemplateResponse(
-                name="cog_index.html",
+            return self.templates.TemplateResponse(
+                name="cog_viewer.html",
                 context={
                     "request": request,
                     "tilejson_endpoint": factory.url_for(request, "tilejson"),
                     "info_endpoint": factory.url_for(request, "info"),
                     "statistics_endpoint": factory.url_for(request, "statistics"),
                 },
                 media_type="text/html",
             )
 
 
 @dataclass
 class stacViewerExtension(FactoryExtension):
     """Add /viewer endpoint to the TilerFactory."""
 
+    templates: Jinja2Templates = DEFAULT_TEMPLATES
+
     def register(self, factory: BaseTilerFactory):
         """Register endpoint to the tiler factory."""
 
         @factory.router.get("/viewer", response_class=HTMLResponse)
         def stac_viewer(request: Request):
             """STAC Viewer."""
-            return templates.TemplateResponse(
-                name="stac_index.html",
+            return self.templates.TemplateResponse(
+                name="stac_viewer.html",
                 context={
                     "request": request,
                     "tilejson_endpoint": factory.url_for(request, "tilejson"),
                     "info_endpoint": factory.url_for(request, "info"),
                     "statistics_endpoint": factory.url_for(request, "asset_statistics"),
                 },
                 media_type="text/html",
```

### Comparing `titiler.extensions-0.11.6/titiler/extensions/wms.py` & `titiler.extensions-0.11.7/titiler/extensions/wms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 """wms Extension."""
 
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple
 from urllib.parse import urlencode
 
+import jinja2
 import numpy
 import rasterio
 from fastapi import Depends, HTTPException, Query
 from rasterio.crs import CRS
 from rio_tiler.mosaic import mosaic_reader
 from rio_tiler.mosaic.methods.base import MosaicMethodBase
 from starlette.requests import Request
 from starlette.responses import Response
 from starlette.templating import Jinja2Templates
 
 from titiler.core.dependencies import RescalingParams
 from titiler.core.factory import BaseTilerFactory, FactoryExtension
 from titiler.core.resources.enums import ImageType, MediaType
 
-try:
-    from importlib.resources import files as resources_files  # type: ignore
-except ImportError:
-    # Try backported to PY<39 `importlib_resources`.
-    from importlib_resources import files as resources_files  # type: ignore
-
-# TODO: mypy fails in python 3.9, we need to find a proper way to do this
-templates = Jinja2Templates(directory=str(resources_files(__package__) / "templates"))  # type: ignore
+DEFAULT_TEMPLATES = Jinja2Templates(
+    directory="",
+    loader=jinja2.ChoiceLoader([jinja2.PackageLoader(__package__, "templates")]),
+)  # type:ignore
 
 
 class WMSMediaType(str, Enum):
     """Responses Media types for WMS"""
 
     tif = "image/tiff; application=geotiff"
     jp2 = "image/jp2"
@@ -69,14 +66,15 @@
             "image/jp2",
             "image/tiff; application=geotiff",
         ]
     )
     supported_version: List[str] = field(
         default_factory=lambda: ["1.0.0", "1.1.1", "1.3.0"]
     )
+    templates: Jinja2Templates = DEFAULT_TEMPLATES
 
     def register(self, factory: BaseTilerFactory):  # noqa: C901
         """Register endpoint to the tiler factory."""
 
         @factory.router.get(
             "/wms",
             response_class=Response,
@@ -370,15 +368,15 @@
                             layers_dict[layer]["abstract"] = src_dst.info().json()
 
                 # Build information for the whole service
                 minx, miny, maxx, maxy = zip(
                     *[layers_dict[layer]["bounds_wgs84"] for layer in layers_dict]
                 )
 
-                return templates.TemplateResponse(
+                return self.templates.TemplateResponse(
                     f"wms_{version}.xml",
                     {
                         "request": request,
                         "request_url": wms_url,
                         "formats": self.supported_format,
                         "available_epsgs": self.supported_crs,
                         "layers_dict": layers_dict,
```

### Comparing `titiler.extensions-0.11.6/PKG-INFO` & `titiler.extensions-0.11.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.extensions
-Version: 0.11.6
+Version: 0.11.7
 Summary: Extensions for TiTiler Factories.
 License: MIT
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,GDAL,Rasterio,OGC
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

