# Comparing `tmp/prose-3.0.0.tar.gz` & `tmp/prose-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prose-3.0.0.tar", max compression
+gzip compressed data, was "prose-3.0.1.tar", max compression
```

## Comparing `prose-3.0.0.tar` & `prose-3.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1097 2023-05-17 11:58:22.053360 prose-3.0.0/LICENSE
--rw-r--r--   0        0        0     2574 2023-05-17 11:58:22.053360 prose-3.0.0/README.md
--rw-r--r--   0        0        0      651 2023-05-17 11:58:22.177361 prose-3.0.0/prose/__init__.py
--rw-r--r--   0        0        0       84 2023-05-17 11:58:22.177361 prose-3.0.0/prose/archive/__init__.py
--rw-r--r--   0        0        0     2397 2023-05-17 11:58:22.177361 prose-3.0.0/prose/archive/pos1.py
--rw-r--r--   0        0        0     2071 2023-05-17 11:58:22.177361 prose-3.0.0/prose/archive/sdss.py
--rw-r--r--   0        0        0      254 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/__init__.py
--rw-r--r--   0        0        0     3553 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/alignment.py
--rw-r--r--   0        0        0     3028 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/background.py
--rw-r--r--   0        0        0     8569 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/catalogs.py
--rw-r--r--   0        0        0     8706 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/centroids.py
--rw-r--r--   0        0        0    13532 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/detection.py
--rw-r--r--   0        0        0     6597 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/geometry.py
--rw-r--r--   0        0        0     3743 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/photometry.py
--rw-r--r--   0        0        0    13913 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/psf.py
--rw-r--r--   0        0        0     3703 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/shepard.py
--rw-r--r--   0        0        0    20531 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/utils.py
--rw-r--r--   0        0        0     4012 2023-05-17 11:58:22.181361 prose-3.0.0/prose/blocks/visualization.py
--rw-r--r--   0        0        0     4069 2023-05-17 11:58:22.181361 prose-3.0.0/prose/builtins.py
--rw-r--r--   0        0        0     5113 2023-05-17 11:58:22.181361 prose-3.0.0/prose/config.py
--rw-r--r--   0        0        0     3733 2023-05-17 11:58:22.181361 prose-3.0.0/prose/console_utils.py
--rw-r--r--   0        0        0      120 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/__init__.py
--rw-r--r--   0        0        0     3356 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/block.py
--rw-r--r--   0        0        0    22974 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/image.py
--rw-r--r--   0        0        0    10521 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/sequence.py
--rw-r--r--   0        0        0    16375 2023-05-17 11:58:22.181361 prose-3.0.0/prose/core/source.py
--rw-r--r--   0        0        0    17092 2023-05-17 11:58:22.181361 prose-3.0.0/prose/fluxes.py
--rw-r--r--   0        0        0      137 2023-05-17 11:58:22.181361 prose-3.0.0/prose/io/__init__.py
--rw-r--r--   0        0        0      686 2023-05-17 11:58:22.181361 prose-3.0.0/prose/io/create_fm_db.sql
--rw-r--r--   0        0        0    20099 2023-05-17 11:58:22.181361 prose-3.0.0/prose/io/fitsmanager.py
--rw-r--r--   0        0        0     6386 2023-05-17 11:58:22.181361 prose-3.0.0/prose/io/io.py
--rw-r--r--   0        0        0    15085 2023-05-17 11:58:22.181361 prose-3.0.0/prose/simulations.py
--rw-r--r--   0        0        0     7901 2023-05-17 11:58:22.181361 prose-3.0.0/prose/telescope.py
--rw-r--r--   0        0        0    14620 2023-05-17 11:58:22.181361 prose-3.0.0/prose/utils.py
--rw-r--r--   0        0        0    29851 2023-05-17 11:58:22.181361 prose-3.0.0/prose/visualization.py
--rw-r--r--   0        0        0      996 2023-05-17 11:58:22.181361 prose-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 prose-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-17 14:21:18.875805 prose-3.0.1/LICENSE
+-rw-r--r--   0        0        0     2574 2023-05-17 14:21:18.875805 prose-3.0.1/README.md
+-rw-r--r--   0        0        0      651 2023-05-17 14:21:18.967806 prose-3.0.1/prose/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-17 14:21:18.967806 prose-3.0.1/prose/archive/__init__.py
+-rw-r--r--   0        0        0     2397 2023-05-17 14:21:18.967806 prose-3.0.1/prose/archive/pos1.py
+-rw-r--r--   0        0        0     2071 2023-05-17 14:21:18.967806 prose-3.0.1/prose/archive/sdss.py
+-rw-r--r--   0        0        0      254 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/__init__.py
+-rw-r--r--   0        0        0     3848 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/alignment.py
+-rw-r--r--   0        0        0     3598 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/background.py
+-rw-r--r--   0        0        0     8569 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/catalogs.py
+-rw-r--r--   0        0        0     8767 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/centroids.py
+-rw-r--r--   0        0        0    13242 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/detection.py
+-rw-r--r--   0        0        0     6597 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/geometry.py
+-rw-r--r--   0        0        0     3937 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/photometry.py
+-rw-r--r--   0        0        0    14105 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/psf.py
+-rw-r--r--   0        0        0     3703 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/shepard.py
+-rw-r--r--   0        0        0    20531 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/utils.py
+-rw-r--r--   0        0        0     4012 2023-05-17 14:21:18.967806 prose-3.0.1/prose/blocks/visualization.py
+-rw-r--r--   0        0        0     4069 2023-05-17 14:21:18.967806 prose-3.0.1/prose/builtins.py
+-rw-r--r--   0        0        0     5933 2023-05-17 14:21:18.967806 prose-3.0.1/prose/config.py
+-rw-r--r--   0        0        0     3733 2023-05-17 14:21:18.967806 prose-3.0.1/prose/console_utils.py
+-rw-r--r--   0        0        0      120 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/__init__.py
+-rw-r--r--   0        0        0     3651 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/block.py
+-rw-r--r--   0        0        0    22985 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/image.py
+-rw-r--r--   0        0        0    10521 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/sequence.py
+-rw-r--r--   0        0        0    16375 2023-05-17 14:21:18.967806 prose-3.0.1/prose/core/source.py
+-rw-r--r--   0        0        0    17092 2023-05-17 14:21:18.967806 prose-3.0.1/prose/fluxes.py
+-rw-r--r--   0        0        0      137 2023-05-17 14:21:18.967806 prose-3.0.1/prose/io/__init__.py
+-rw-r--r--   0        0        0      686 2023-05-17 14:21:18.967806 prose-3.0.1/prose/io/create_fm_db.sql
+-rw-r--r--   0        0        0    20101 2023-05-17 14:21:18.971806 prose-3.0.1/prose/io/fitsmanager.py
+-rw-r--r--   0        0        0     6374 2023-05-17 14:21:18.971806 prose-3.0.1/prose/io/io.py
+-rw-r--r--   0        0        0    15085 2023-05-17 14:21:18.971806 prose-3.0.1/prose/simulations.py
+-rw-r--r--   0        0        0     7901 2023-05-17 14:21:18.971806 prose-3.0.1/prose/telescope.py
+-rw-r--r--   0        0        0    14447 2023-05-17 14:21:18.971806 prose-3.0.1/prose/utils.py
+-rw-r--r--   0        0        0    29851 2023-05-17 14:21:18.971806 prose-3.0.1/prose/visualization.py
+-rw-r--r--   0        0        0     1007 2023-05-17 14:21:18.971806 prose-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 prose-3.0.1/PKG-INFO
```

### Comparing `prose-3.0.0/LICENSE` & `prose-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/README.md` & `prose-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/__init__.py` & `prose-3.0.1/prose/__init__.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/archive/pos1.py` & `prose-3.0.1/prose/archive/pos1.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/archive/sdss.py` & `prose-3.0.1/prose/archive/sdss.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/blocks/alignment.py` & `prose-3.0.1/prose/blocks/alignment.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,14 +36,18 @@
                 image.transform.inverse,
                 cval=np.nanmedian(image.data),
                 output_shape=image.shape,
             )
         except np.linalg.LinAlgError:
             image.discard = True
 
+    @property
+    def citations(self) -> list:
+        return super().citations + ["scikit-image"]
+
 
 class AlignReferenceSources(Block):
     def __init__(self, reference: Image, name=None, verbose=False):
         """Set Image sources to reference Image sources, properly aligned
 
         |read| Image.sources
 
@@ -77,14 +81,18 @@
                 > 100
             ):
                 image.discard = True
             else:
                 sources.coords = new_sources_coords
                 image.sources = sources
 
+    @property
+    def citations(self) -> list:
+        return super().citations + ["scikit-image"]
+
 
 class AlignReferenceWCS(Block):
     def __init__(self, reference: Image, name=None, verbose=False, n=6):
         """Create WCS based on reference WCS. To use this block, Image sources must match the sources from the reference (e.g. using AlignReferenceSources), i.e. same sources should be found at a given index in both images.
 
         |read| Image.sources
 
@@ -106,7 +114,11 @@
     def run(self, image: Image):
         ref_skycoords = self.reference.wcs.pixel_to_world(
             *self.reference.sources.coords[0 : self.n].T
         )
         image.wcs = fit_wcs_from_points(
             image.sources.coords[0 : self.n].T, ref_skycoords
         )
+
+    @property
+    def citations(self) -> list:
+        return super().citations + ["astropy"]
```

### Comparing `prose-3.0.0/prose/blocks/catalogs.py` & `prose-3.0.1/prose/blocks/catalogs.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/blocks/centroids.py` & `prose-3.0.1/prose/blocks/centroids.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
             np.linalg.norm(image.sources.coords - sources_coords, axis=1) < self.limit
         )
         final_sources_coords = image.sources.coords.copy()
         final_sources_coords[in_limit] = sources_coords[in_limit]
         image.sources.coords = final_sources_coords
 
     @property
-    def citations(self):
-        return "photutils"
+    def citations(self) -> list:
+        return super().citations + ["photutils"]
 
 
 class CentroidCOM(_PhotutilsCentroid):
     """Centroiding using ``photutils.centroids.centroid_com``
 
     |read| ``Image.sources``
 
@@ -187,15 +187,15 @@
         )
         final_sources_coords = image.sources.coords.copy()
         final_sources_coords[in_limit] = sources_coords[in_limit]
         image.sources.coords = final_sources_coords
 
     @property
     def citations(self):
-        return "tensorflow"
+        return super().citations + ["tensorflow", "keras"]
 
 
 class CentroidBallet(_CNNCentroid):
     """Centroiding with  `ballet <https://github.com/lgrcia/ballet>`_.
 
     |write| ``Image.stars_coords``
     """
```

### Comparing `prose-3.0.0/prose/blocks/detection.py` & `prose-3.0.1/prose/blocks/detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,18 +200,14 @@
             regions = [regions[i] for i in idxs]
 
         sources = Sources(
             np.array([PointSource.from_region(region) for region in regions])
         )
         image.sources = Sources(self.clean(sources), source_type="PointSource")
 
-    @property
-    def citations(self):
-        return "scikit-image", "scipy"
-
 
 class TraceDetection(_SourceDetection):
     def __init__(self, minor_length=5, **kwargs):
         """Detect trace sources  (as :py:class:`~prose.core.source.TraceSource`)
 
         Parameters
         ----------
@@ -233,18 +229,14 @@
         super().__init__(minor_length=minor_length, **kwargs)
 
     def run(self, image):
         regions = self.regions(image)
         sources = np.array([TraceSource.from_region(region) for region in regions])
         image.sources = Sources(sources)
 
-    @property
-    def citations(self):
-        return "scikit-image", "scipy"
-
 
 # backward compatibility
 class SegmentedPeaks(PointSourceDetection):
     def __init__(
         self, unit_euler=False, min_area=3, minor_length=2, n_stars=None, **kwargs
     ):
         """Detect point sources (backward compatibility)
@@ -271,18 +263,14 @@
         peaks = np.ones(len(image.stars_coords)) * -1
         for j, i in enumerate(idxs):
             cut = cuts[j]
             if cut is not None:
                 peaks[i] = np.max(cut.data)
         image.peaks = peaks
 
-    @property
-    def citations(self):
-        return "photutils"
-
 
 class _SimplePointSourceDetection(_SourceDetection):
     def __init__(self, n_stars=None, min_separation=None, sort=True, name=None):
         super().__init__(n=n_stars, sort=sort, min_separation=min_separation, name=name)
 
     def run(self, image):
         coordinates, peaks = self.detect(image)
@@ -339,18 +327,14 @@
         coordinates = np.transpose(
             np.array([sources["xcentroid"].data, sources["ycentroid"].data])
         )
         peaks = sources["peak"]
 
         return coordinates, peaks
 
-    @property
-    def citations(self):
-        return "photutils"
-
 
 try:
     from sep import extract
 except:
     raise AssertionError("sep not installed")
 
 
@@ -386,12 +370,12 @@
         coordinates = np.array([sep_data["x"], sep_data["y"]]).T
         fluxes = np.array(sep_data["flux"])
 
         return coordinates, fluxes
 
     @property
     def citations(self):
-        return "source extractor", "sep"
+        return super().citations + ["sep"]
 
 
 class AlignSources(Block):
     pass  # TODO
```

### Comparing `prose-3.0.0/prose/blocks/geometry.py` & `prose-3.0.1/prose/blocks/geometry.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/blocks/photometry.py` & `prose-3.0.1/prose/blocks/photometry.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,22 +37,30 @@
         apertures = [image.sources.apertures(r) for r in radii]
         aperture_fluxes = np.array(
             [aperture_photometry(image.data, a)["aperture_sum"].data for a in apertures]
         ).T
 
         image.aperture = {"fluxes": aperture_fluxes, "radii": radii}
 
+    @property
+    def citations(self) -> list:
+        return super().citations + ["photutils"]
+
 
 class _AnnulusPhotometry(Block):
     def __init__(self, name=None, rin=5, rout=8, scale=True):
         super().__init__(name=name)
         self.rin = rin
         self.rout = rout
         self.scale = scale
 
+    @property
+    def citations(self) -> list:
+        return super().citations + ["photutils"]
+
 
 class AnnulusBackground(_AnnulusPhotometry):
     def __init__(
         self,
         rin: float = 5,
         rout: float = 8,
         sigma: float = 3,
```

### Comparing `prose-3.0.0/prose/blocks/psf.py` & `prose-3.0.1/prose/blocks/psf.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,18 @@
         image.fwhm = image.epsf.fwhm
         self._last_init = params
 
     @property
     def model(self):
         return self.model_function()
 
+    @property
+    def citations(self) -> list:
+        return super().citations + ["astropy", "scipy"]
+
 
 class _JAXPSFModel(_PSFModelBase):
     def __init__(self, reference_image=None, name=None, verbose=False):
         super().__init__(reference_image, name, verbose)
 
     def optimize(self, data):
         @jax.jit
@@ -141,14 +145,18 @@
             ll = jnp.sum(jnp.power((self._opt_model(params) - data), 2))
             return ll
 
         opt = ScipyMinimize(fun=nll)
         params = opt.run(self._last_init).params
         return params
 
+    @property
+    def citations(self) -> list:
+        return self.citations + ["jax"]
+
 
 class JAXGaussian2D(_JAXPSFModel):
     def __init__(self, reference_image: Image = None, name=None, verbose=False):
         """Model :code:`Image.epsf` as a 2D Gaussian profile (powered by `JAX`_)
 
         |read| :code:`Image.epsf`
```

### Comparing `prose-3.0.0/prose/blocks/shepard.py` & `prose-3.0.1/prose/blocks/shepard.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/blocks/utils.py` & `prose-3.0.1/prose/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/blocks/visualization.py` & `prose-3.0.1/prose/blocks/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/builtins.py` & `prose-3.0.1/prose/builtins.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/config.py` & `prose-3.0.1/prose/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,40 @@
 from prose.builtins import built_in_telescopes
 
 info = print
 package_name = "prose"
 
 
 class ConfigManager:
+    """
+    A class for managing configuration settings for the package.
+
+    Attributes
+    ----------
+    config : dict
+        A dictionary containing the current configuration settings.
+    folder_path : Path
+        A Path object representing the folder where the configuration files are stored.
+    config_file : Path
+        A Path object representing the configuration file.
+    telescopes_dict : dict
+        A dictionary containing the available telescopes.
+    logs : list
+        A list of log files.
+
+    Methods
+    -------
+    check_config_file(load=False)
+        Checks if the configuration file exists and loads it if it does.
+    save()
+        Saves the current configuration settings to the configuration file.
+    get(key)
+        Returns the value of the specified configuration setting.
+    """
+
     def __init__(self):
         self.config = None
 
         self.folder_path = Path.home() / f".{package_name}"
         self.folder_path.mkdir(exist_ok=True)
 
         self.config_file = self.folder_path / "config"
```

### Comparing `prose-3.0.0/prose/console_utils.py` & `prose-3.0.1/prose/console_utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/core/block.py` & `prose-3.0.1/prose/core/block.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import inspect
 from time import time
 from typing import Union
 
-import pytest
-
 from prose.console_utils import warning
-from prose.core.image import Image, Buffer
+from prose.core.image import Buffer, Image
 
 
 class Block(object):
     """Single unit of processing acting on the :py:class:`~prose.Image` object
 
     Reading, processing and writing :py:class:`~prose.Image` attributes. When placed in a sequence, it goes through two steps:
 
@@ -70,30 +68,39 @@
         raise NotImplementedError()
 
     def terminate(self):
         """Method called after block's :py:class:`~prose.Sequence` is finished (if any)"""
         pass
 
     @property
-    def citations(self):
-        return None
+    def citations(self) -> list:
+        """
+        Returns a string listing the packages used by the block.
+
+        Returns
+        -------
+        str
+            A string listing the packages used by the block.
+        """
+        return ["astropy", "prose", "numpy", "scipy"]
 
     @staticmethod
     def _doc():
         return ""
 
     def __call__(self, image):
         image_copy = image.copy()
         self.run(image_copy)
         if image_copy.discard:
             warning(f"{self.__class__.__name__} discarded Image")
         return image_copy
 
 
 # rewrite the tested function to accept Block instances as well as strings
+# requires pytest and is not used in the docs for now
 def is_tested(block_class: Union[Block, str]) -> bool:
     """Check if a block is tested
 
     Parameters
     ----------
     block_class : Block or str
         block to be tested
@@ -104,14 +111,16 @@
         True if the block is tested, False otherwise
 
     Raises
     ------
     TypeError
         if block is not a Block subclass or a string
     """
+    import pytest
+
     if isinstance(block_class, str):
         block_name = block_class
     elif issubclass(block_class, Block):
         block_name = block_class.__name__
     else:
         raise TypeError(f"block must be a Block subclass or a string")
     result = pytest.main(["-q", "-k", block_name])
```

### Comparing `prose-3.0.0/prose/core/image.py` & `prose-3.0.1/prose/core/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         """
         self.computed[name] = value
 
     def get(self, name):
         return self.computed[name]
 
     @property
-    def sources(self):
+    def sources(self) -> Sources:
         """Image sources.
 
         Returns
         -------
         prose.core.source.Sources
         """
         return self._sources
```

### Comparing `prose-3.0.0/prose/core/sequence.py` & `prose-3.0.1/prose/core/sequence.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/core/source.py` & `prose-3.0.1/prose/core/source.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/fluxes.py` & `prose-3.0.1/prose/fluxes.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/io/create_fm_db.sql` & `prose-3.0.1/prose/io/create_fm_db.sql`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/io/fitsmanager.py` & `prose-3.0.1/prose/io/fitsmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,29 +344,29 @@
         else:
             query = f"select * from observations where {where}"
             df = self.to_pandas(query)
 
         return df.set_index(["id"])
 
     def calibrations(self, **kwargs):
-        """return a pandas DataFrame of calibrations observations given some metadata constraints in the form of wildcards
+        """return a pandas DataFrame of calibrations observations given some metadata constraints in the form of wildcards.
 
         Parameters
         ----------
         **kwargs:
             wildcards value for telescope, target, filter or id, default is '*'
         """
         darks = self.observations(type="dark", **kwargs)
         flats = self.observations(type="flat", **kwargs)
         bias = self.observations(type="bias", **kwargs)
 
         return pd.concat([darks, flats, bias], axis=0)
 
     def files(self, id=None, path=False, exposure=0, tolerance=1000, **kwargs):
-        """Return a pandas DataFrame of files given some metadata constraints in the form of wildcards
+        """Return a pandas DataFrame of files given some metadata constraints in the form of wildcards.
 
         Parameters
         ----------
         id : int, optional
             id of the observation for which files are retrieved, by default None, i.e. all files
         path : bool, optional
             whether to include files paths in the pandas.DataFrame header, by default False
```

### Comparing `prose-3.0.0/prose/io/io.py` & `prose-3.0.1/prose/io/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                 last_telescope = telescope_id
         else:
             _telescope = telescope
 
         df_list.append(
             dict(
                 path=i,
-                date=_telescope.date(header).isoformat(),
+                date=_telescope.date(header),
                 telescope=_telescope.name,
                 type=_telescope.image_type(header),
                 target=header.get(_telescope.keyword_object, ""),
                 filter=header.get(_telescope.keyword_filter, ""),
                 dimensions=(header.get("NAXIS1", 1), header.get("NAXIS2", 1)),
                 flip=header.get(_telescope.keyword_flip, ""),
                 jd=header.get(_telescope.keyword_jd, ""),
```

### Comparing `prose-3.0.0/prose/simulations.py` & `prose-3.0.1/prose/simulations.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/telescope.py` & `prose-3.0.1/prose/telescope.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/prose/utils.py` & `prose-3.0.1/prose/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,22 +435,14 @@
 
 def binn2D(arr, factor):
     new_shape = np.array(arr.shape) // factor
     shape = (new_shape[0], factor, new_shape[1], factor)
     return np.mean(arr.reshape(shape).mean(-1), 1)
 
 
-from functools import partial
-
-import numpy as np
-from scipy.spatial import KDTree
-from skimage.transform import AffineTransform as skAT
-from twirl import utils as tutils
-
-
 def distance(p1, p2):
     return np.sqrt(np.power(p1[0] - p2[0], 2) + np.power(p1[1] - p2[1], 2))
 
 
 def distances(coords, coord):
     return [
         np.sqrt(((coord[0] - x) ** 2 + (coord[1] - y) ** 2))
```

### Comparing `prose-3.0.0/prose/visualization.py` & `prose-3.0.1/prose/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.0.0/pyproject.toml` & `prose-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prose"
-version = "3.0.0"
+version = "3.0.1"
 description = "Modular image processing pipelines for Astronomy"
 authors = ["Lionel Garcia"]
 license = "MIT"
 readme = "README.md"
 include = ["prose/io/*.sql"]
 
 [tool.poetry.dependencies]
@@ -42,11 +42,12 @@
 docutils = "*"
 jupyterlab = "*"
 myst-parser = "*"
 sphinx-book-theme = "^1.0.0"
 myst-nb = "*"
 sphinx-copybutton = "*"
 sphinx-design = "*"
+toml = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `prose-3.0.0/PKG-INFO` & `prose-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prose
-Version: 3.0.0
+Version: 3.0.1
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
-Metadata-Version: 2.1 Name: prose Version: 3.0.0 Summary: Modular image
+Metadata-Version: 2.1 Name: prose Version: 3.0.1 Summary: Modular image
 processing pipelines for Astronomy License: MIT Author: Lionel Garcia Requires-
 Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: astropy (>=5.1.1,<6.0.0) Requires-
 Dist: astroquery (>=0.4.6,<0.5.0) Requires-Dist: celerite2 Requires-Dist:
```

