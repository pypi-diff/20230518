# Comparing `tmp/prose-3.0.1.tar.gz` & `tmp/prose-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prose-3.0.1.tar", max compression
+gzip compressed data, was "prose-3.0.2.tar", max compression
```

## Comparing `prose-3.0.1.tar` & `prose-3.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1097 2023-05-17 14:21:18.875805 prose-3.0.1/LICENSE
--rw-r--r--   0        0        0     2574 2023-05-17 14:21:18.875805 prose-3.0.1/README.md
--rw-r--r--   0        0        0      651 2023-05-17 14:21:18.967806 prose-3.0.1/prose/__init__.py
--rw-r--r--   0        0        0       84 2023-05-17 14:21:18.967806 prose-3.0.1/prose/archive/__init__.py
--rw-r--r--   0        0        0     2397 2023-05-17 14:21:18.967806 prose-3.0.1/prose/archive/pos1.py
--rw-r--r--   0        0        0     2071 2023-05-17 14:21:18.967806 prose-3.0.1/prose/archive/sdss.py
--rw-r--r--   0        0        0      254 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/__init__.py
--rw-r--r--   0        0        0     3848 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/alignment.py
--rw-r--r--   0        0        0     3598 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/background.py
--rw-r--r--   0        0        0     8569 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/catalogs.py
--rw-r--r--   0        0        0     8767 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/centroids.py
--rw-r--r--   0        0        0    13242 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/detection.py
--rw-r--r--   0        0        0     6597 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/geometry.py
--rw-r--r--   0        0        0     3937 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/photometry.py
--rw-r--r--   0        0        0    14105 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/psf.py
--rw-r--r--   0        0        0     3703 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/shepard.py
--rw-r--r--   0        0        0    20531 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/utils.py
--rw-r--r--   0        0        0     4012 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/visualization.py
--rw-r--r--   0        0        0     4069 2023-05-17 14:21:18.967806 prose-3.0.1/prose/builtins.py
--rw-r--r--   0        0        0     5933 2023-05-17 14:21:18.967806 prose-3.0.1/prose/config.py
--rw-r--r--   0        0        0     3733 2023-05-17 14:21:18.967806 prose-3.0.1/prose/console_utils.py
--rw-r--r--   0        0        0      120 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/__init__.py
--rw-r--r--   0        0        0     3651 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/block.py
--rw-r--r--   0        0        0    22985 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/image.py
--rw-r--r--   0        0        0    10521 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/sequence.py
--rw-r--r--   0        0        0    16375 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/source.py
--rw-r--r--   0        0        0    17092 2023-05-17 14:21:18.967806 prose-3.0.1/prose/fluxes.py
--rw-r--r--   0        0        0      137 2023-05-17 14:21:18.967806 prose-3.0.1/prose/io/__init__.py
--rw-r--r--   0        0        0      686 2023-05-17 14:21:18.967806 prose-3.0.1/prose/io/create_fm_db.sql
--rw-r--r--   0        0        0    20101 2023-05-17 14:21:18.971806 prose-3.0.1/prose/io/fitsmanager.py
--rw-r--r--   0        0        0     6374 2023-05-17 14:21:18.971806 prose-3.0.1/prose/io/io.py
--rw-r--r--   0        0        0    15085 2023-05-17 14:21:18.971806 prose-3.0.1/prose/simulations.py
--rw-r--r--   0        0        0     7901 2023-05-17 14:21:18.971806 prose-3.0.1/prose/telescope.py
--rw-r--r--   0        0        0    14447 2023-05-17 14:21:18.971806 prose-3.0.1/prose/utils.py
--rw-r--r--   0        0        0    29851 2023-05-17 14:21:18.971806 prose-3.0.1/prose/visualization.py
--rw-r--r--   0        0        0     1007 2023-05-17 14:21:18.971806 prose-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 prose-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-18 09:42:09.964263 prose-3.0.2/LICENSE
+-rw-r--r--   0        0        0     2574 2023-05-18 09:42:09.964263 prose-3.0.2/README.md
+-rw-r--r--   0        0        0      651 2023-05-18 09:42:10.076267 prose-3.0.2/prose/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-18 09:42:10.076267 prose-3.0.2/prose/archive/__init__.py
+-rw-r--r--   0        0        0     2397 2023-05-18 09:42:10.076267 prose-3.0.2/prose/archive/pos1.py
+-rw-r--r--   0        0        0     2071 2023-05-18 09:42:10.076267 prose-3.0.2/prose/archive/sdss.py
+-rw-r--r--   0        0        0      254 2023-05-18 09:42:10.076267 prose-3.0.2/prose/blocks/__init__.py
+-rw-r--r--   0        0        0     3932 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/alignment.py
+-rw-r--r--   0        0        0     3680 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/background.py
+-rw-r--r--   0        0        0     8717 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/catalogs.py
+-rw-r--r--   0        0        0     8768 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/centroids.py
+-rw-r--r--   0        0        0    13402 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/detection.py
+-rw-r--r--   0        0        0     6605 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/geometry.py
+-rw-r--r--   0        0        0     4135 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/photometry.py
+-rw-r--r--   0        0        0    13998 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/psf.py
+-rw-r--r--   0        0        0     3703 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/shepard.py
+-rw-r--r--   0        0        0    20531 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/utils.py
+-rw-r--r--   0        0        0     4012 2023-05-18 09:42:10.080267 prose-3.0.2/prose/blocks/visualization.py
+-rw-r--r--   0        0        0     4069 2023-05-18 09:42:10.080267 prose-3.0.2/prose/builtins.py
+-rw-r--r--   0        0        0     5933 2023-05-18 09:42:10.080267 prose-3.0.2/prose/config.py
+-rw-r--r--   0        0        0     3733 2023-05-18 09:42:10.080267 prose-3.0.2/prose/console_utils.py
+-rw-r--r--   0        0        0      120 2023-05-18 09:42:10.080267 prose-3.0.2/prose/core/__init__.py
+-rw-r--r--   0        0        0     3651 2023-05-18 09:42:10.080267 prose-3.0.2/prose/core/block.py
+-rw-r--r--   0        0        0    24631 2023-05-18 09:42:10.080267 prose-3.0.2/prose/core/image.py
+-rw-r--r--   0        0        0    11016 2023-05-18 09:42:10.080267 prose-3.0.2/prose/core/sequence.py
+-rw-r--r--   0        0        0    16435 2023-05-18 09:42:10.080267 prose-3.0.2/prose/core/source.py
+-rw-r--r--   0        0        0    17092 2023-05-18 09:42:10.080267 prose-3.0.2/prose/fluxes.py
+-rw-r--r--   0        0        0      137 2023-05-18 09:42:10.080267 prose-3.0.2/prose/io/__init__.py
+-rw-r--r--   0        0        0      686 2023-05-18 09:42:10.080267 prose-3.0.2/prose/io/create_fm_db.sql
+-rw-r--r--   0        0        0    24173 2023-05-18 09:42:10.080267 prose-3.0.2/prose/io/fitsmanager.py
+-rw-r--r--   0        0        0     6374 2023-05-18 09:42:10.080267 prose-3.0.2/prose/io/io.py
+-rw-r--r--   0        0        0    15085 2023-05-18 09:42:10.080267 prose-3.0.2/prose/simulations.py
+-rw-r--r--   0        0        0     7901 2023-05-18 09:42:10.080267 prose-3.0.2/prose/telescope.py
+-rw-r--r--   0        0        0    14447 2023-05-18 09:42:10.080267 prose-3.0.2/prose/utils.py
+-rw-r--r--   0        0        0    29851 2023-05-18 09:42:10.080267 prose-3.0.2/prose/visualization.py
+-rw-r--r--   0        0        0     1007 2023-05-18 09:42:10.080267 prose-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 prose-3.0.2/PKG-INFO
```

### Comparing `prose-3.0.1/LICENSE` & `prose-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/README.md` & `prose-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/__init__.py` & `prose-3.0.2/prose/__init__.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/archive/pos1.py` & `prose-3.0.2/prose/archive/pos1.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/archive/sdss.py` & `prose-3.0.2/prose/archive/sdss.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/blocks/alignment.py` & `prose-3.0.2/prose/blocks/alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 
 # TODO test inverse
 class Align(Block):
     def __init__(self, reference, name=None):
         """Align image data to a reference
 
+        |read| :code:`Image.data`
+
+        |modify|
+
         Parameters
         ----------
         reference: :py:class:`~prose.Image`
             reference image to align images on
         name : str, optional
             name of the block, by default None
         """
@@ -45,17 +49,17 @@
         return super().citations + ["scikit-image"]
 
 
 class AlignReferenceSources(Block):
     def __init__(self, reference: Image, name=None, verbose=False):
         """Set Image sources to reference Image sources, properly aligned
 
-        |read| Image.sources
+        |read| :code:`Image.sources`
 
-        |write| Image.sources
+        |write| :code:`Image.sources`
 
         Parameters
         ----------
         reference : Image
             reference image containing sources
         name : _type_, optional
             _description_, by default None
@@ -90,18 +94,17 @@
         return super().citations + ["scikit-image"]
 
 
 class AlignReferenceWCS(Block):
     def __init__(self, reference: Image, name=None, verbose=False, n=6):
         """Create WCS based on reference WCS. To use this block, Image sources must match the sources from the reference (e.g. using AlignReferenceSources), i.e. same sources should be found at a given index in both images.
 
-        |read| Image.sources
-
-        |write| Image.wcs
+        |read| :code:`Image.sources`
 
+        |write| :code:`Image.wcs`
 
         Parameters
         ----------
         reference : Image
             reference image containing a valid WCS
         n : int, optional
             number of stars used to match WCS, by default 6
```

### Comparing `prose-3.0.1/prose/blocks/background.py` & `prose-3.0.2/prose/blocks/background.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from astropy.stats import SigmaClip
 from photutils.background import Background2D, MedianBackground
 
 from prose import Block
 from prose.blocks.psf import *
 from prose.utils import binn2D
 
-# TODO
-
 
 class PhotutilsBackground2D(Block):
     def __init__(self, subtract=True, box_size=(50, 50), filter_size=(3, 3), name=None):
         """
         Initializes the PhotutilsBackground2D block.
 
+        |read| :code:`Image.data`
+
+        |write| :code:`Image.data`, :code:`Image.bkg`
+
         Parameters
         ----------
         subtract : bool, optional
             Whether to subtract the estimated background from the image. Default is True.
         box_size : tuple of int, optional
             The size of the box used to compute the background. Default is (50, 50).
         filter_size : tuple of int, optional
```

### Comparing `prose-3.0.1/prose/blocks/catalogs.py` & `prose-3.0.2/prose/blocks/catalogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,21 +115,24 @@
                     new_df_dict.append(nans)
 
             catalog = pd.DataFrame(new_df_dict)
 
         image.catalogs[self.catalog_name] = catalog.iloc[0 : self.limit]
 
 
-# TODO
 class PlateSolve(Block):
     def __init__(
         self, reference=None, n=30, tolerance=10, radius=1.2, debug=False, **kwargs
     ):
         """Plate solve an image using twirl
 
+        |read| :code:`Image.sources`
+
+        |write| :code:`Image.wcs`, :code:`Image.plate_solved_success`
+
         Parameters
         ----------
         reference : Image, optional
             _description_, by default None
         n : int, optional
             _description_, by default 30
         tolerance : int, optional
@@ -182,15 +185,15 @@
     def __init__(self, correct_pm=True, limit=10000, mode=None):
         """Query gaia catalog
 
         Catalog is written in Image.catalogs as a pandas DataFrame. If mode is ""crossmatch" the index of catalog sources in the DataFrame matches with the index of sources in Image.sources
 
         |read| :code:`Image.sources` if mode is "crossmatch"
 
-        |write|
+        |write| :code:`Image.catalogs`
 
         - :code:`Image.sources` if mode is "crossmatch"
         - :code:`Image.catalogs`
 
         Parameters
         ----------
         correct_pm : bool, optional
@@ -219,15 +222,15 @@
     def __init__(self, limit=10000, mode=None):
         """Query TESS (TIC) catalog
 
         Catalog is written in Image.catalogs as a pandas DataFrame. If mode is ""crossmatch" the index of catalog sources in the DataFrame matches with the index of sources in Image.sources
 
         |read| :code:`Image.sources` if mode is "crossmatch"
 
-        |write|
+        |write| :code:`Image.catalogs`
 
         - :code:`Image.sources` if mode is "crossmatch"
         - :code:`Image.catalogs`
 
 
         Parameters
         ----------
```

### Comparing `prose-3.0.1/prose/blocks/centroids.py` & `prose-3.0.2/prose/blocks/centroids.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         return super().citations + ["tensorflow", "keras"]
 
 
 class CentroidBallet(_CNNCentroid):
     """Centroiding with  `ballet <https://github.com/lgrcia/ballet>`_.
 
     |write| ``Image.stars_coords``
+
     """
 
     def __init__(self, **kwargs):
         super().__init__(cutout=15, filename="centroid.h5", **kwargs)
         self.import_and_check_model()
 
     def build_model(self):
```

### Comparing `prose-3.0.1/prose/blocks/detection.py` & `prose-3.0.2/prose/blocks/detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,15 +125,19 @@
         n=None,
         sort=True,
         min_separation=None,
         name=None,
         min_area=0,
         minor_length=0,
     ):
-        """Detect all sources
+        """Detect all sources.
+
+        |read| :code:`Image.data`
+
+        |write| :code:`Image.sources`
 
         Parameters
         ----------
         threshold : float, optional
             detection threshold for sources, by default 4
         n : int, optional
             number of sources to detect, by default None
@@ -162,15 +166,19 @@
         regions = self.regions(image)
         sources = np.array([auto_source(region) for region in regions])
         image.sources = Sources(self.clean(sources))
 
 
 class PointSourceDetection(_SourceDetection):
     def __init__(self, unit_euler=False, min_area=3, minor_length=2, **kwargs):
-        """Detect point sources (as :py:class:`~prose.core.source.PointSource`)
+        """Detect point sources (as :py:class:`~prose.core.source.PointSource`).
+
+        |read| :code:`Image.data`
+
+        |write| :code:`Image.sources`
 
         Parameters
         ----------
         unit_euler : bool, optional
             whether to consider sources with euler number == 1, by default False
         min_area : str, optional
             minimum area in pixels of the sources to detect, by default 0
@@ -248,15 +256,15 @@
             n=n_stars, min_area=min_area, minor_length=minor_length, **kwargs
         )
         self.unit_euler = unit_euler
         self.min_area = min_area
         self.minor_length = minor_length
 
 
-# TODO
+# TODO: document
 class Peaks(Block):
     def __init__(self, cutout=11, **kwargs):
         super().__init__(**kwargs)
         self.cutout = cutout
 
     def run(self, image, **kwargs):
         idxs, cuts = cutouts(image.data, image.sources.coords, size=self.cutout)
```

### Comparing `prose-3.0.1/prose/blocks/geometry.py` & `prose-3.0.2/prose/blocks/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,17 @@
         )
 
 
 class ComputeTransform(Block):
     """
     Compute transformation fromm a reference image
 
-    |read| ``Image.sources`` on both reference and input image
+    |read| :code:`Image.sources` on both reference and input image
 
-    |write| ``Image.transform``
+    |write| :code:`Image.transform`
 
     Parameters
     ----------
     ref : Image
         image containing detected sources
     n : int, optional
         number of stars to consider to compute transformation, by default 10
```

### Comparing `prose-3.0.1/prose/blocks/photometry.py` & `prose-3.0.2/prose/blocks/photometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 from prose import Block, Image
 
 __all__ = ["AperturePhotometry", "AnnulusBackground"]
 
 
 class AperturePhotometry(Block):
     def __init__(self, radii: np.ndarray = None, scale: bool = True, name=None):
-        """Perform aperture photometry of each sources
+        """Perform aperture photometry of each sources.
+
+        |read| :code:`Image.data`, :code:`Image.sources`
+
+        |write| :code:`Image.aperture`
 
         Parameters
         ----------
         radii : np.ndarray, optional
-            apertures radii (definition vary depending of sources), by default None
+            apertures radii (definition varies depending on sources), by default None
         scale : bool, optional
             whether to scale radii with :code:`Image.fwhm` usually present in :code:`Image.epsf`, by default True
         name : str, optional
             name of the block, by default None
         """
         super().__init__(name=name)
         if radii is None:
@@ -63,19 +67,22 @@
         self,
         rin: float = 5,
         rout: float = 8,
         sigma: float = 3,
         scale=True,
         name: str = None,
     ):
-        """Estimate background around each source using an annulus aperture
+        """Estimate background around each source using an annulus aperture.
+
+        |read| :code:`Image.data`, :code:`Image.sources`
+
+        |write| :code:`Image.annulus`
 
         Parameters
         ----------
-
         rin : float, optional
             inner radius of the annulus, by default 5
         rout : float, optional
             outer radius of the annulus, by default 8
         sigma : float, optional
             sigma clipping applied to pixel within annulus before taking the median value, by default 3.
         scale : bool, optional
```

### Comparing `prose-3.0.1/prose/blocks/psf.py` & `prose-3.0.2/prose/blocks/psf.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,27 +44,25 @@
         "background": background,
         "theta": 0.0,
         "beta": 3.0,
     }
 
 
 class MedianEPSF(Block):
-    def __init__(self, max_sources=1, name=None, normalize=True):
+    def __init__(self, max_sources=1, normalize=True, name=None):
         """Stack cutouts into :code:`Image.epsf`: a median effective PSF
 
-        |read| Image.source
+        |read| Image.cutouts
 
-        [write] Image.epsf
+        |write| Image.epsf
 
         Parameters
         ----------
         max_sources : int, optional
-            max number of sources cutout to be stacked should have, by default 1, meaning only cutouts with a single source are used
-        name : _type_, optional
-            _description_, by default None
+            maximum number of sources in a cutout for the cutout to be used, by default 1
         normalize : bool, optional
             whether to normalize cutouts to form a normalized EPSF, by default True
         """
         super().__init__(name=name)
         self.max_sources = max_sources
         self.normalize = normalize
         self._parallel_friendly = True
@@ -318,15 +316,14 @@
             theta = params["theta"]
             m = params["background"]
             return self.model_function()(height, xo, yo, sx, sy, theta, m)
 
         return _model
 
 
-# TODO
 class Moffat2D(_PSFModelBase):
     def __init__(self, reference_image: Image = None, name=None, verbose=False):
         """Model :code:`Image.epsf` as a 2D Moffat profile
 
         |read| :code:`Image.epsf`
 
         |write|
@@ -402,14 +399,15 @@
             m = params["background"]
             beta = params["beta"]
             return self.model_function()(height, xo, yo, sx, sy, theta, m, beta)
 
         return _model
 
 
+# TODO: document
 class HFD(Block):
     # https://www.focusmax.org/Documents_V4/ITS%20Paper.pdf
 
     def __init__(self, order=4, **kwargs):
         super().__init__(**kwargs)
         self.sorted_idxs = None
         self.order = order
```

### Comparing `prose-3.0.1/prose/blocks/shepard.py` & `prose-3.0.2/prose/blocks/shepard.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/blocks/utils.py` & `prose-3.0.2/prose/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/blocks/visualization.py` & `prose-3.0.2/prose/blocks/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/builtins.py` & `prose-3.0.2/prose/builtins.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/config.py` & `prose-3.0.2/prose/config.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/console_utils.py` & `prose-3.0.2/prose/console_utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/core/block.py` & `prose-3.0.2/prose/core/block.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/core/image.py` & `prose-3.0.2/prose/core/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 from astropy.nddata import Cutout2D as astopy_Cutout2D
 from astropy.nddata import overlap_slices
 from astropy.time import Time
 from astropy.wcs import WCS
 from astropy.wcs.wcs import WCS
 from dateutil import parser as dparser
 from matplotlib import gridspec
-from PIL import Image
 
 from prose import utils, viz
 from prose.core.source import Sources
 from prose.telescope import Telescope
 
 
 @dataclass
 class Image:
     """
-    Image object containing image data and metadata
+    Image object containing image data and metadata.
 
     This is a Python Data Class, so that most attributes described below can be used as
-    keyword-arguments when instantiated
+    keyword-arguments when instantiated.
     """
 
     data: np.ndarray = None
     """Image data"""
 
     metadata: dict = None
     """Image metadata"""
@@ -206,14 +205,15 @@
         if value is not None:
             return value * unit
         else:
             return None
 
     @property
     def shape(self):
+        """Image.data shape"""
         return np.array(self.data.shape)
 
     @property
     def ra(self):
         """Right-Ascension as an astropy Quantity"""
         return self._from_metadata_with_unit("ra")
 
@@ -228,14 +228,15 @@
         if "exposure" in self.metadata:
             return self._from_metadata_with_unit("exposure")
         else:
             return None
 
     @property
     def jd(self):
+        """Julian Date of the observation"""
         return self.metadata["jd"]
 
     @property
     def pixel_scale(self):
         """Pixel scale (or plate scale) as an astropy Quantity"""
         return self._from_metadata_with_unit("pixel_scale")
 
@@ -284,14 +285,26 @@
             name of the computed value
         value : any
             value to set
         """
         self.computed[name] = value
 
     def get(self, name):
+        """Get computed value
+
+        Parameters
+        ----------
+        name : str
+            name of the computed value
+
+        Returns
+        -------
+        any
+            computed value
+        """
         return self.computed[name]
 
     @property
     def sources(self) -> Sources:
         """Image sources.
 
         Returns
@@ -310,15 +323,15 @@
     def cutout(
         self,
         coords: Union[list, tuple, np.ndarray],
         shape: Union[int, tuple],
         wcs: bool = True,
         sources: bool = True,
         reset_index: bool = True,
-    ) -> Image:
+    ):
         """Return a cutout Image instance.
 
         Parameters
         ----------
         coords : list, tuple, np.ndarray
             cutout center coordinates
         shape : tuple or int
@@ -437,14 +450,35 @@
             name in self.catalogs
         ), f"Catalog '{name}' not present, consider using ..."
         x, y = self.catalogs[name][["x", "y"]].values.T
         labels = self.catalogs[name]["id"].values if label else None
         viz.plot_marks(x, y, labels, color=color)
 
     def plot_model(self, data, figsize=(5, 5), cmap=None, c="C0", contour=False):
+        """
+        Plot the data and a model side by side.
+
+        Parameters
+        ----------
+        data : numpy.ndarray
+            The model data to plot.
+        figsize : tuple, optional
+            The size of the figure, by default (5, 5).
+        cmap : str or matplotlib.colors.Colormap, optional
+            The colormap to use for the data, by default None.
+        c : str, optional
+            The color to use for the data, by default "C0".
+        contour : bool, optional
+            Whether to plot the contours of the model, by default False.
+
+        Returns
+        -------
+        None
+        """
+
         plt.figure(figsize=figsize)
         axes = gridspec.GridSpec(2, 2, width_ratios=[9, 2], height_ratios=[2, 9])
         axes.update(wspace=0, hspace=0)
 
         # axtt = plt.subplot(gs[1, 1])
         ax = plt.subplot(axes[1, 0])
         axr = plt.subplot(axes[1, 1], sharey=ax)
@@ -469,32 +503,65 @@
         im_dict = asdict(self.copy())
         if low_data:
             im_dict["data"] = utils.z_scale(im_dict["data"]) * (2**7 - 1)
             image_dtype = "int8"
         im_dict["data"] = im_dict["data"].astype(image_dtype)
         return im_dict
 
-    def save(self, filepath, image_dtype="int16", low_data=True):
+    def save(self, filepath, image_dtype="float64", low_data=True):
+        """
+        Save the image to a file using pickle.
+
+        Note that the pickle will hold the Image dataclass dict attributes.
+
+        Parameters
+        ----------
+        filepath : str
+            The path to the file to save.
+        image_dtype : str, optional
+            The data type to use for the image data, by default "int16".
+        low_data : bool, optional
+            Whether to scale the data to a lower range, by default True.
+
+        Returns
+        -------
+        None
+        """
+
         with open(filepath, "wb") as f:
             pickle.dump(self.asdict(image_dtype=image_dtype, low_data=low_data), f)
 
     @classmethod
     def load(cls, filepath):
+        """
+        Load an image from a file.
+
+        Parameters
+        ----------
+        filepath : str
+            The path to the file to load.
+
+        Returns
+        -------
+        Image
+            The loaded image.
+        """
+
         return cls(**pickle.load(open(filepath, "rb")))
 
-    def symetric_profile(self, source, binn=1.0):
+    def _symetric_profile(self, source, binn=1.0):
         x, y = source.coords
         Y, X = np.indices(self.shape)
         radii = (np.sqrt((X - x) ** 2 + (Y - y) ** 2)).flatten()
-        d, values = self.profile(radii)
+        d, values = self._profile(radii)
         idxs = utils.index_binning(d, binn)
         mean = lambda x: np.array([np.mean(x[i]) for i in idxs])
         return mean(d), mean(values)
 
-    def profile(self, d):
+    def _profile(self, d):
         idxs = np.argsort(d)
         _d = d[idxs]
         pixels = self.data.flatten()
         pixels = pixels[idxs]
 
         return _d, pixels
 
@@ -526,15 +593,15 @@
             c = np.zeros(shape)
             large, small = overlap_slices(self.shape, shape, (y, x))
             c[small] = self.data[large]
             cutouts.append(c)
 
         return np.array(cutouts)
 
-    def major_profile(self, source, binn=1.0, debug=False):
+    def _major_profile(self, source, binn=1.0, debug=False):
         p1 = source.coords[:, None, None]
         p2 = (source.vertexes[0])[:, None, None]
         Y, X = np.indices(self.data.shape)
         p3 = np.array([X, Y])
 
         # projection
         # https://stackoverflow.com/questions/61341712/calculate-projected-point-location-x-y-on-given-line-startx-y-endx-y
```

### Comparing `prose-3.0.1/prose/core/sequence.py` & `prose-3.0.2/prose/core/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,30 @@
             ""
         )
 
         return tex, "\n\n".join(cites.values())
 
 
 class SequenceParallel(Sequence):
+    """
+    A class for running a sequence of blocks in parallel using multiprocessing.
+
+    The data_blocks allow blocks carying large amount of data to be run sequentially
+    so that they are not copied from one process to another.
+
+    Parameters
+    ----------
+    blocks : list
+        A list of blocks to be executed in parallel.
+    data_blocks : list, optional
+        A list of data blocks to be executed in parallel.
+    name : str, optional
+        A name for the sequence.
+    """
+
     def __init__(self, blocks, data_blocks=None, name=""):
         super().__init__(blocks, name=name)
         if data_blocks is None:
             self.data = None
             self._has_data = False
         else:
             self.data = Sequence(data_blocks)
```

### Comparing `prose-3.0.1/prose/core/source.py` & `prose-3.0.2/prose/core/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,16 @@
         return EllipticalAperture(self.coords, a, b, self.orientation)
 
     def rectangular_aperture(self, r, scale=True):
         if scale:
             a, b = 2 * r * self.a, 2 * r * self.b
         else:
             a, b = 2 * r, 2 * r * self.eccentricity
+        a = np.max([0.01, a])
+        b = np.max([0.01, b])
         return RectangularAperture(
             self.coords, float(np.abs(a)), float(np.abs(b)), self.orientation
         )
 
     def circular_annulus(self, r0, r1, scale=False):
         if scale:
             r0 = r0 * self.a
```

### Comparing `prose-3.0.1/prose/fluxes.py` & `prose-3.0.2/prose/fluxes.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/io/create_fm_db.sql` & `prose-3.0.2/prose/io/create_fm_db.sql`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/io/fitsmanager.py` & `prose-3.0.2/prose/io/fitsmanager.py`

 * *Files 24% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                 jd,
                 id,
                 exposure,
             ),
         )
 
     def get_files(self, folders, extension, scan=None, depth=0):
-        """Return path of files with specific extension in the specified folder(s)
+        """Return paths of files with specific extension in the specified folder(s)
 
         Parameters
         ----------
         folders : str or list of str
             path or list of paths of folders to look into
         extension : str
             wildcard pattern for file extension
@@ -416,14 +416,40 @@
         past=1e3,
         future=0,
         tolerance=1e15,
         same_telescope=True,
         lights="images",
         show=True,
     ):
+        """
+        Return a dictionary of files for a given observation ID, along with calibration files.
+
+        Parameters
+        ----------
+        i : int
+            id of the observation for which files are retrieved.
+        past : float, optional
+            Number of days in the past to consider when retrieving calibrartion files, by default 1e3.
+        future : float, optional
+            Number of days in the future to consider when retrieving calibrartion files, by default 0.
+        tolerance : float, optional
+            Tolerance on the exposure constraint, by default 1e15. For example: if exposure is set to 10 and tolerance to 2, all
+            files with exposure = 10 +- 2 will be retrieved.
+        same_telescope : bool, optional
+            Whether to retrieve files from the same telescope as the observation, by default True.
+        lights : str, optional
+            key of images files in the return dict, by default "images".
+        show : bool, optional
+            Whether to print the pandas dataframe of returned files, by default True.
+
+        Returns
+        -------
+        dict
+            A dictionary containing the files for the given observation id, along with the associated calibration files.
+        """
         files = {}
 
         obs_dict = self.observations(id=i, hide_exposure=False).to_dict("records")[0]
         sql_days = SQL_DAYS_BETWEEN.format(
             date=obs_dict["date"], future=future, past=past
         )
         sql_exposure = exposure_constraint(
@@ -502,53 +528,123 @@
         Returns
         -------
         list of str
         """
         return self.files(type="light", path=True).path.values
 
     def images(self, i, show=False, **kwargs):
+        """
+        Return the paths of the observation science images for a given observation id.
+
+        Parameters
+        ----------
+        i : int
+            The observation id.
+        show : bool, optional
+            Whether to show the pandas dataframe of the returned files, by default False.
+        **kwargs : dict, optional
+            Additional arguments to pass to the `observation_files` method.
+
+        Returns
+        -------
+        list of str
+            The fits paths of the observation science images.
+        """
+
         return self.observation_files(i, show=show, **kwargs)["images"]
 
     @property
     def all_darks(self):
         """fits paths of the observation dark images
 
         Returns
         -------
         list of str
         """
         return self.files(type="dark", path=True).path.values
 
     def bias(self, i, show=False, **kwargs):
+        """
+        Return the paths of the bias images associated to a given observation.
+
+        Parameters
+        ----------
+        i : int
+            The index of the observation.
+        show : bool, optional
+            Whether to display the pandas dataframe of the files being returned, by default False.
+        **kwargs : dict
+            Additional keyword arguments to pass to the `observation_files` method.
+
+        Returns
+        -------
+        list of str
+            The fits paths of the bias images.
+        """
         return self.observation_files(i, show=show, **kwargs)["bias"]
 
     @property
     def all_bias(self):
         """fits paths of the observation bias images
 
         Returns
         -------
         list of str
         """
         return self.files(type="bias", path=True).path.values
 
     def darks(self, i, show=False, **kwargs):
+        """
+        Return the paths of the dark images associated to a given observation.
+
+        Parameters
+        ----------
+        i : int
+            The index of the observation.
+        show : bool, optional
+            Whether to display the pandas dataframe of the files being returned, by default False.
+        **kwargs : dict
+            Additional keyword arguments to pass to the `observation_files` method.
+
+        Returns
+        -------
+        list of str
+            The fits paths of the observation dark images.
+        """
         return self.observation_files(i, show=show, **kwargs)["darks"]
 
     @property
     def all_flats(self):
         """fits paths of the observation flats images
 
         Returns
         -------
         list of str
         """
         return self.files(type="flat", path=True).path.values
 
     def flats(self, i, show=False, **kwargs):
+        """
+        Return the paths of the flat images associated to a given observation.
+
+        Parameters
+        ----------
+        i : int
+            The index of the observation.
+        show : bool, optional
+            Whether to display the pandas dataframe of the files being returned, by default False.
+        **kwargs : dict
+            Additional keyword arguments to pass to the `observation_files` method.
+
+        Returns
+        -------
+        list of str
+            The fits paths of the observation flat images.
+        """
+
         return self.observation_files(i, show=show, **kwargs)["flats"]
 
     @property
     def stack(self):
         """fits paths of the observation stack image if present
 
         Returns
@@ -564,14 +660,27 @@
         Returns
         -------
         list of str
         """
         return self.files(imtype="reduced")
 
     def label(self, i):
+        """
+        Return a string label for the observation with the given index.
+
+        Parameters
+        ----------
+        i : int
+            The index of the observation.
+
+        Returns
+        -------
+        str
+            A string label in the format "{telescope}_{date}_{target}_{filter}".
+        """
         date, telescope, filter, _, target, *_ = self.observations(id=i).values[0]
         return f"{telescope}_{date.replace('-', '')}_{target}_{filter}"
 
     @property
     def obs_name(self):
         """Observation name ({telescope}_{date}_{target}_{filter}) if a single observation is present"""
         if self.unique_obs:
@@ -584,14 +693,27 @@
     def __repr__(self):
         return str(self.observations())
 
     def _repr_html_(self):
         return self.observations()._repr_html_()
 
     def to_pandas(self, query):
+        """
+        Execute a SQL query and return the result as a pandas DataFrame.
+
+        Parameters
+        ----------
+        query : str
+            The SQL query to execute.
+
+        Returns
+        -------
+        pandas.DataFrame
+            The result of the query as a pandas DataFrame.
+        """
         return pd.read_sql_query(query, self.con)
 
     def _update_observations(self, verbose=False):
         """
         Slow! This should never be used (use update_obs=True in _insert)
         """
         observations = self.to_pandas(
```

### Comparing `prose-3.0.1/prose/io/io.py` & `prose-3.0.2/prose/io/io.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/simulations.py` & `prose-3.0.2/prose/simulations.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/telescope.py` & `prose-3.0.2/prose/telescope.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/utils.py` & `prose-3.0.2/prose/utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/prose/visualization.py` & `prose-3.0.2/prose/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.1/pyproject.toml` & `prose-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prose"
-version = "3.0.1"
+version = "3.0.2"
 description = "Modular image processing pipelines for Astronomy"
 authors = ["Lionel Garcia"]
 license = "MIT"
 readme = "README.md"
 include = ["prose/io/*.sql"]
 
 [tool.poetry.dependencies]
```

### Comparing `prose-3.0.1/PKG-INFO` & `prose-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prose
-Version: 3.0.1
+Version: 3.0.2
 Summary: Modular image processing pipelines for Astronomy
 License: MIT
 Author: Lionel Garcia
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prose Version: 3.0.1 Summary: Modular image
+Metadata-Version: 2.1 Name: prose Version: 3.0.2 Summary: Modular image
 processing pipelines for Astronomy License: MIT Author: Lionel Garcia Requires-
 Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: astropy (>=5.1.1,<6.0.0) Requires-
 Dist: astroquery (>=0.4.6,<0.5.0) Requires-Dist: celerite2 Requires-Dist:
```

