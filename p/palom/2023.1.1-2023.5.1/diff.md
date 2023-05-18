# Comparing `tmp/palom-2023.1.1.tar.gz` & `tmp/palom-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palom-2023.1.1.tar", max compression
+gzip compressed data, was "palom-2023.5.1.tar", max compression
```

## Comparing `palom-2023.1.1.tar` & `palom-2023.5.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      331 2021-11-30 23:03:29.885474 palom-2023.1.1/palom/__init__.py
--rw-r--r--   0        0        0     9607 2023-01-11 23:16:52.689629 palom-2023.1.1/palom/align.py
--rw-r--r--   0        0        0     3449 2022-11-16 20:08:23.273397 palom-2023.1.1/palom/block_affine.py
--rw-r--r--   0        0        0        0 2021-11-04 17:46:44.649265 palom-2023.1.1/palom/cli/__init__.py
--rw-r--r--   0        0        0     2694 2021-11-30 23:03:29.889461 palom-2023.1.1/palom/cli/helper.py
--rw-r--r--   0        0        0      284 2021-11-04 21:58:01.051871 palom-2023.1.1/palom/cli/schema/__init__.py
--rw-r--r--   0        0        0      471 2021-11-30 23:03:29.889461 palom-2023.1.1/palom/cli/schema/svs-config-example.yml
--rw-r--r--   0        0        0     1842 2022-11-16 18:05:06.130208 palom-2023.1.1/palom/cli/schema/svs-config-schema.yml
--rw-r--r--   0        0        0     9132 2022-11-16 18:05:06.132204 palom-2023.1.1/palom/cli/svs.py
--rw-r--r--   0        0        0     3809 2022-02-23 23:37:51.043051 palom-2023.1.1/palom/color.py
--rw-r--r--   0        0        0     1803 2022-11-16 18:05:06.133204 palom-2023.1.1/palom/extract.py
--rw-r--r--   0        0        0     2610 2023-01-11 23:16:52.689629 palom-2023.1.1/palom/img_util.py
--rw-r--r--   0        0        0     7642 2023-01-11 23:16:52.691625 palom-2023.1.1/palom/pyramid.py
--rw-r--r--   0        0        0     6114 2023-01-05 02:14:26.822974 palom-2023.1.1/palom/reader.py
--rw-r--r--   0        0        0     8339 2023-01-11 23:16:52.690627 palom-2023.1.1/palom/register.py
--rw-r--r--   0        0        0     2665 2023-01-11 23:16:52.690627 palom-2023.1.1/palom/register_util.py
--rw-r--r--   0        0        0      972 2023-01-11 23:17:20.505648 palom-2023.1.1/pyproject.toml
--rw-r--r--   0        0        0     9485 2022-11-16 18:05:06.138186 palom-2023.1.1/README.md
--rw-r--r--   0        0        0    10783 1970-01-01 00:00:00.000000 palom-2023.1.1/setup.py
--rw-r--r--   0        0        0    10364 1970-01-01 00:00:00.000000 palom-2023.1.1/PKG-INFO
+-rw-r--r--   0        0        0     9486 2023-05-18 04:20:32.792050 palom-2023.5.1/README.md
+-rw-r--r--   0        0        0      331 2023-05-18 04:20:22.703787 palom-2023.5.1/palom/__init__.py
+-rw-r--r--   0        0        0     9679 2023-05-18 04:20:32.791173 palom-2023.5.1/palom/align.py
+-rw-r--r--   0        0        0     3449 2023-05-17 03:40:00.979667 palom-2023.5.1/palom/block_affine.py
+-rw-r--r--   0        0        0        0 2022-11-16 17:08:01.770570 palom-2023.5.1/palom/cli/__init__.py
+-rw-r--r--   0        0        0     5352 2023-05-18 04:20:32.791222 palom-2023.5.1/palom/cli/align_he.py
+-rw-r--r--   0        0        0    11965 2023-05-18 04:20:32.791300 palom-2023.5.1/palom/cli/flow.py
+-rw-r--r--   0        0        0     2694 2022-11-16 17:08:01.770704 palom-2023.5.1/palom/cli/helper.py
+-rw-r--r--   0        0        0      284 2022-11-16 17:08:01.770861 palom-2023.5.1/palom/cli/schema/__init__.py
+-rw-r--r--   0        0        0      471 2022-11-16 17:08:01.770975 palom-2023.5.1/palom/cli/schema/svs-config-example.yml
+-rw-r--r--   0        0        0     1842 2022-11-16 17:08:01.771106 palom-2023.5.1/palom/cli/schema/svs-config-schema.yml
+-rw-r--r--   0        0        0     9132 2023-05-17 04:20:02.909374 palom-2023.5.1/palom/cli/svs.py
+-rw-r--r--   0        0        0     3855 2023-05-18 04:20:32.792018 palom-2023.5.1/palom/color.py
+-rw-r--r--   0        0        0     1803 2022-11-16 17:08:01.771500 palom-2023.5.1/palom/extract.py
+-rw-r--r--   0        0        0     2610 2023-05-17 04:20:02.909766 palom-2023.5.1/palom/img_util.py
+-rw-r--r--   0        0        0     7642 2023-05-18 01:07:11.995667 palom-2023.5.1/palom/pyramid.py
+-rw-r--r--   0        0        0     6114 2023-05-17 04:20:02.909455 palom-2023.5.1/palom/reader.py
+-rw-r--r--   0        0        0     8339 2023-05-17 03:40:00.981700 palom-2023.5.1/palom/register.py
+-rw-r--r--   0        0        0     2665 2023-05-17 03:40:00.981734 palom-2023.5.1/palom/register_util.py
+-rw-r--r--   0        0        0      979 2023-05-18 04:28:01.340556 palom-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10422 1970-01-01 00:00:00.000000 palom-2023.5.1/PKG-INFO
```

### Comparing `palom-2023.1.1/palom/align.py` & `palom-2023.5.1/palom/align.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,19 +232,21 @@
         img = skimage.exposure.rescale_intensity(img, out_range=np.uint16)
         shape = self.grid_shape
         grid = np.arange(np.multiply(*shape)).reshape(shape)
         h, w = np.divide(
             img.shape,
             np.divide(self.ref_img.chunksize, self.ref_thumbnail_down_factor)
         )
-        cmap = 'grays_r' if img_util.is_brightfield_img(img) else 'gray'
+        cmap = 'gray_r' if img_util.is_brightfield_img(img) else 'gray'
+        func = np.array if img_util.is_brightfield_img(img) else np.log1p
+
         if ax is None:
             _, ax = plt.subplots()
         ax.imshow(
-            np.log1p(img),
+            func(img),
             cmap=cmap,
             extent=(-0.5, w-0.5, h-0.5, -0.5)
         )
         # checkerboard pattern
         ax.imshow(np.indices(shape).sum(axis=0) % 2, cmap='cool', alpha=0.2)
         return grid
```

### Comparing `palom-2023.1.1/palom/block_affine.py` & `palom-2023.5.1/palom/block_affine.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/cli/helper.py` & `palom-2023.5.1/palom/cli/helper.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/cli/schema/svs-config-schema.yml` & `palom-2023.5.1/palom/cli/schema/svs-config-schema.yml`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/cli/svs.py` & `palom-2023.5.1/palom/cli/svs.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/color.py` & `palom-2023.5.1/palom/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         self._contrast_img = self.contrast_ref_img
         if isinstance(self._contrast_img, da.Array):
             self._contrast_img = self._contrast_img.compute()
         return self._contrast_img
 
     def rgb2grayscale(self, rgb_img):
         import cv2
-        return cv2.cvtColor(rgb_img, cv2.COLOR_BGR2GRAY)
+        # FIXME should be cv2.COLOR_RGB2GRAY
+        return cv2.cvtColor(rgb_img, cv2.COLOR_RGB2GRAY)
         # return skimage.color.rgb2gray(rgb_img).astype(np.float32)
 
     def rgb2aec(self, rgb_img):
         return extract.rgb2aec(rgb_img).astype(np.float32)
 
     def rgb2dab(self, rgb_img):
         hdx = skimage.color.separate_stains(rgb_img, skimage.color.hdx_from_rgb)
```

### Comparing `palom-2023.1.1/palom/extract.py` & `palom-2023.5.1/palom/extract.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/img_util.py` & `palom-2023.5.1/palom/img_util.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/pyramid.py` & `palom-2023.5.1/palom/pyramid.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/reader.py` & `palom-2023.5.1/palom/reader.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/register.py` & `palom-2023.5.1/palom/register.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/palom/register_util.py` & `palom-2023.5.1/palom/register_util.py`

 * *Files identical despite different names*

### Comparing `palom-2023.1.1/pyproject.toml` & `palom-2023.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "palom"
-version = "2023.1.1"
+version = "2023.5.1"
 description = "Piecewise alignment for layers of mosaics"
 authors = ["Yu-An Chen <atwood12@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/palom/"
 repository = "https://github.com/Yu-AnChen/palom"
 keywords = [
     "microscopy",
@@ -12,15 +12,15 @@
     "image registration",
     "digital pathology",
     "atlas"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.8"
-scikit-image = ">=0.18"
+scikit-image = ">=0.18, <0.20"
 scikit-learn = ">=0.24"
 opencv-python = "^4.5.3.56"
 zarr = "^2.10.0"
 tifffile = ">=2021.10.12"
 imagecodecs = ">=2021.11.11"
 matplotlib = "^3.4.3"
 tqdm = "^4.62.3"
```

### Comparing `palom-2023.1.1/README.md` & `palom-2023.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 installing miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 ### Step 1
 
 Create a named conda environment - _palom_, in the following example, and activate the environment.
 
 ```
-conda create -n palom python=3.7 pip -c conda-forge
+conda create -n palom python=3.10 pip -c conda-forge
 conda activate palom
 ```
 
 ### Step 2
 
 Install openslide in the conda environment.
```

### Comparing `palom-2023.1.1/setup.py` & `palom-2023.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,327 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: palom
+Version: 2023.5.1
+Summary: Piecewise alignment for layers of mosaics
+Home-page: https://pypi.org/project/palom/
+Keywords: microscopy,multiplex imaging,image registration,digital pathology,atlas
+Author: Yu-An Chen
+Author-email: atwood12@gmail.com
+Requires-Python: >=3.7.8,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dask (>=2021.10.0)
+Requires-Dist: imagecodecs (>=2021.11.11)
+Requires-Dist: loguru (>=0.5.3,<0.6.0)
+Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
+Requires-Dist: napari-lazy-openslide (>=0.2.0)
+Requires-Dist: numpy (>=1.21.3,<2.0.0)
+Requires-Dist: opencv-python (>=4.5.3.56,<5.0.0.0)
+Requires-Dist: scikit-image (>=0.18,<0.20)
+Requires-Dist: scikit-learn (>=0.24)
+Requires-Dist: scipy (>=1.7.1,<2.0.0)
+Requires-Dist: tifffile (>=2021.10.12)
+Requires-Dist: tqdm (>=4.62.3,<5.0.0)
+Requires-Dist: yamale (>=4.0.2,<5.0.0)
+Requires-Dist: zarr (>=2.10.0,<3.0.0)
+Project-URL: Repository, https://github.com/Yu-AnChen/palom
+Description-Content-Type: text/markdown
 
-packages = \
-['palom', 'palom.cli', 'palom.cli.schema']
+<h2>
+    <img alt="palom" height="60" src="palom-logo.svg">
+    <br>
+    Piecewise alignment for layers of mosaics
+</h2>
 
-package_data = \
-{'': ['*']}
+Palom started as a tool for registering [whole-slide
+images](https://en.wikipedia.org/wiki/Digital_pathology) of the same [FFPE
+section](https://en.wikipedia.org/wiki/Histology#Sample_preparation) with
+different [IHC stainings](https://en.wikipedia.org/wiki/Immunohistochemistry).
 
-install_requires = \
-['dask>=2021.10.0',
- 'imagecodecs>=2021.11.11',
- 'loguru>=0.5.3,<0.6.0',
- 'matplotlib>=3.4.3,<4.0.0',
- 'napari-lazy-openslide>=0.2.0',
- 'numpy>=1.21.3,<2.0.0',
- 'opencv-python>=4.5.3.56,<5.0.0.0',
- 'scikit-image>=0.18',
- 'scikit-learn>=0.24',
- 'scipy>=1.7.1,<2.0.0',
- 'tifffile>=2021.10.12',
- 'tqdm>=4.62.3,<5.0.0',
- 'yamale>=4.0.2,<5.0.0',
- 'zarr>=2.10.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['palom-svs = palom.cli.svs:main',
-                     'palom-svs-helper = palom.cli.helper:main']}
-
-setup_kwargs = {
-    'name': 'palom',
-    'version': '2023.1.1',
-    'description': 'Piecewise alignment for layers of mosaics',
-    'long_description': '<h2>\n    <img alt="palom" height="60" src="palom-logo.svg">\n    <br>\n    Piecewise alignment for layers of mosaics\n</h2>\n\nPalom started as a tool for registering [whole-slide\nimages](https://en.wikipedia.org/wiki/Digital_pathology) of the same [FFPE\nsection](https://en.wikipedia.org/wiki/Histology#Sample_preparation) with\ndifferent [IHC stainings](https://en.wikipedia.org/wiki/Immunohistochemistry).\n\n---\n\n## Installation\n\nInstalling palom in a fresh conda environment is recommended. [Instruction for\ninstalling miniconda](https://docs.conda.io/en/latest/miniconda.html)\n\n### Step 1\n\nCreate a named conda environment - _palom_, in the following example, and activate the environment.\n\n```\nconda create -n palom python=3.7 pip -c conda-forge\nconda activate palom\n```\n\n### Step 2\n\nInstall openslide in the conda environment.\n\n- For MacOS, use conda-forge channel\n\n```\nconda install openslide -c conda-forge\n```\n\n- For Windows and Linux, use sdvillal channel\n\n```\nconda install openslide -c sdvillal\n```\n\n### Step 3\n\nInstall palom from pypi in the conda environment.\n\n```\npython -m pip install palom\n```\n\n---\n\n## CLI usage\n\n### Configuration YAML file\n\nPalom CLI tool merges multiple SVS files into a pyramidal OME-TIFF file, with\nthe option to perform preset stain separation (5 modes are available - `output\nmode`: `hematoxylin`, `aec`, `dab`, `grayscale`, `color`)\n\nA user-defined configuration YAML file is required for the run. A configuration\nexample can be printed to the console by running\n\n```bash\npalom-svs show example\n```\n\n```yaml\ninput dir: Y:\\user\\me\\projects\\data\\mihc\noutput full path: Y:\\user\\me\\projects\\analysis\\mihc\\2021\\skin-case-356.ome.tif\n\nreference image:\n    filename: 20210111/skin_case_356_HEM_C11R3_HEM.svs\n    output mode: hematoxylin\n    channel name: Hematoxylin\n\nmoving images:\n- filename: 20210101/skin_case_356_HEM_C01R1_PD1.svs\n  output mode: aec\n  channel name: PD-1\n- filename: 20210101/skin_case_356_HEM_C01R2_PDL1.svs\n  output mode: aec\n  channel name: PD-L1\n```\n\nTo show the configuration schema, run the following command\n\n```bash\npalom-svs show schema\n```\n\n### Use the helper script to generate the configuration file\n\n[A helper\nscript](https://github.com/Yu-AnChen/palom/blob/main/palom/cli/helper.py) is\nincluded showing how to automatically generate the configuration file if the SVS\nfiles are organized and have specific naming pattern.\n\nHere\'s an example directory containing many SVS files\n\n```\nY:\\DATA\\SARDANA\\MIHC\\768473\\RAW\n    CBB_SARDANA_768473_C04R1_CD8.svs\n    KB_SARDANA_768473_C01R1_PD1.svs\n    KB_SARDANA_768473_C01R2_PDL1.svs\n    KB_SARDANA_768473_C01R3_Hem.svs\n    KB_SARDANA_768473_C02R1_CD4.svs\n    KB_SARDANA_768473_C03R1_CD3.svs\n    KB_SARDANA_768473_C03R3_DCLAMP.svs\n```\n\nRunning the following command to generate the configuration file\n\n```bash\npalom-svs-helper -i "Y:\\DATA\\SARDANA\\MIHC\\768473\\RAW" -n "*Hem*" -o "Y:\\DATA\\SARDANA\\MIHC\\768473\\RAW\\palom\\768473.ome.tif" -c "Y:\\DATA\\SARDANA\\MIHC\\768473\\768473.yml"\n```\n\nAnd the resulting `Y:\\DATA\\SARDANA\\MIHC\\768473\\768473.yml` file \n\n```yaml\ninput dir: Y:\\DATA\\SARDANA\\MIHC\\768473\\RAW\noutput full path: Y:\\DATA\\SARDANA\\MIHC\\768473\\RAW\\palom\\768473.ome.tif\nreference image:\n  filename: .\\KB_SARDANA_768473_C01R3_Hem.svs\n  output mode: hematoxylin\n  channel name: Hem-C01R3\nmoving images:\n- filename: .\\KB_SARDANA_768473_C01R1_PD1.svs\n  output mode: aec\n  channel name: PD1-C01R1\n- filename: .\\KB_SARDANA_768473_C01R2_PDL1.svs\n  output mode: aec\n  channel name: PDL1-C01R2\n- filename: .\\KB_SARDANA_768473_C02R1_CD4.svs\n  output mode: aec\n  channel name: CD4-C02R1\n- filename: .\\KB_SARDANA_768473_C03R1_CD3.svs\n  output mode: aec\n  channel name: CD3-C03R1\n- filename: .\\KB_SARDANA_768473_C03R3_DCLAMP.svs\n  output mode: aec\n  channel name: DCLAMP-C03R3\n- filename: .\\CBB_SARDANA_768473_C04R1_CD8.svs\n  output mode: aec\n  channel name: CD8-C04R1\n```\n\nAfter reviewing the configuration file, process those SVS files by running\n\n```bash\npalom-svs run -c "Y:\\DATA\\SARDANA\\MIHC\\768473\\768473.yml"\n```\n\nWhen the process is finished, a pyramidal OME-TIFF file will be generated along\nwith PNG files showing the feature-based registration results and a log file. \n\n```\nY:\\DATA\\SARDANA\\MIHC\\768473\\RAW\n│   CBB_SARDANA_768473_C04R1_CD8.svs\n│   KB_SARDANA_768473_C01R1_PD1.svs\n│   KB_SARDANA_768473_C01R2_PDL1.svs\n│   KB_SARDANA_768473_C01R3_Hem.svs\n│   KB_SARDANA_768473_C02R1_CD4.svs\n│   KB_SARDANA_768473_C03R1_CD3.svs\n│   KB_SARDANA_768473_C03R3_DCLAMP.svs\n│\n└───palom\n    │   768473.ome.tif\n    │\n    └───qc\n            01-KB_SARDANA_768473_C01R1_PD1.svs.png\n            02-KB_SARDANA_768473_C01R2_PDL1.svs.png\n            03-KB_SARDANA_768473_C02R1_CD4.svs.png\n            04-KB_SARDANA_768473_C03R1_CD3.svs.png\n            05-KB_SARDANA_768473_C03R3_DCLAMP.svs.png\n            06-CBB_SARDANA_768473_C04R1_CD8.svs.png\n            768473.ome.tif.log\n```\n\n---\n\n## Scripting\n\n__WARNING__ API may change in the future\n\n### For SVS files\n\n```python\nimport palom\n\nc1r = palom.reader.SvsReader(r\'Y:\\DATA\\SARDANA\\MIHC\\75684\\GG_TNP_75684_D21_C11R3_HEM.svs\')\nc2r = palom.reader.SvsReader(r\'Y:\\DATA\\SARDANA\\MIHC\\75684\\GG_TNP_75684_D23_C01R1_PD1.svs\')\n\nLEVEL = 1\nTHUMBNAIL_LEVEL = 2\n\nc1rp = palom.color.PyramidHaxProcessor(c1r.pyramid, thumbnail_level=THUMBNAIL_LEVEL)\nc2rp = palom.color.PyramidHaxProcessor(c2r.pyramid, thumbnail_level=THUMBNAIL_LEVEL)\n\nc21l = palom.align.Aligner(\n    c1rp.get_processed_color(LEVEL), \n    c2rp.get_processed_color(LEVEL),\n    ref_thumbnail=c1rp.get_processed_color(THUMBNAIL_LEVEL).compute(),\n    moving_thumbnail=c2rp.get_processed_color(THUMBNAIL_LEVEL).compute(),\n    ref_thumbnail_down_factor=c1r.level_downsamples[THUMBNAIL_LEVEL] / c1r.level_downsamples[LEVEL],\n    moving_thumbnail_down_factor=c2r.level_downsamples[THUMBNAIL_LEVEL] / c2r.level_downsamples[LEVEL]\n)\n\nc21l.coarse_register_affine()\nc21l.compute_shifts()\nc21l.constrain_shifts()\n\nc21l.block_affine_matrices_da\n\nc2m = palom.align.block_affine_transformed_moving_img(\n    c1rp.get_processed_color(LEVEL),\n    c2rp.get_processed_color(LEVEL, \'aec\'),\n    mxs=c21l.block_affine_matrices_da\n)\n\npalom.pyramid.write_pyramid(\n    palom.pyramid.normalize_mosaics([c2m]),\n    r"Y:\\DATA\\SARDANA\\MIHC\\75684\\mosaic.ome.tif",\n    pixel_size=c1r.pixel_size*c1r.level_downsamples[LEVEL],\n)\n```\n\n### For TIFF and OME-TIFF files\n\n```python\nimport palom\n\n# reference image is a multichannel immunofluoroscence imaging\nc1r = palom.reader.OmePyramidReader(r"Z:\\P37_Pilot2\\P37_S12_Full.ome.tiff")\n# moving image is a brightfield imaging (H&E staining) of the same tissue\n# section as the reference image\nc2r = palom.reader.OmePyramidReader(r"Z:\\P37_Pilot2\\HE\\P37_S12_E033_93_HE.ome.tiff")\n\n# use second-to-the-bottom pyramid level for a quick test; set `LEVEL = 0` for\n# processing lowest level pyramid (full resolution)\nLEVEL = 1\n# choose thumbnail pyramid level for feature-based affine registration as\n# initial coarse alignment\n# `THUMBNAIL_LEVEL = c1r.get_thumbnail_level_of_size(2000)` might be a good\n# starting point\nTHUMBNAIL_LEVEL = 3\n\nc21l = palom.align.Aligner(\n    # use the first channel (Hoechst staining) in the reference image as the\n    # registration reference\n    ref_img=c1r.read_level_channels(LEVEL, 0),\n    # use the second channel (G channel) in the moving image, it usually has\n    # better contrast\n    moving_img=c2r.read_level_channels(LEVEL, 1),\n    # select the same channels for the thumbnail images\n    ref_thumbnail=c1r.read_level_channels(THUMBNAIL_LEVEL, 0).compute(),\n    moving_thumbnail=c2r.read_level_channels(THUMBNAIL_LEVEL, 1).compute(),\n    # specify the downsizing factors so that the affine matrix can be scaled to\n    # match the registration reference\n    ref_thumbnail_down_factor=c1r.level_downsamples[THUMBNAIL_LEVEL] / c1r.level_downsamples[LEVEL],\n    moving_thumbnail_down_factor=c2r.level_downsamples[THUMBNAIL_LEVEL] / c2r.level_downsamples[LEVEL]\n)\n\n# run feature-based affine registration using thumbnails\nc21l.coarse_register_affine(n_keypoints=4000)\n# after coarsly affine registered, run phase correlation on each of the\n# corresponding chunks (blocks/pieces) to refine translations\nc21l.compute_shifts()\n# discard incorrect shifts which is usually due to low contrast in the\n# background regions; this is needed for WSI but maybe not for ROI images\nc21l.constrain_shifts()\n\n# configure the transformation of aligning the moving image to the registration\n# reference\nc2m = palom.align.block_affine_transformed_moving_img(\n    ref_img=c1r.read_level_channels(LEVEL, 0),\n    # select all the three channels (RGB) in moving image to transform\n    moving_img=c2r.pyramid[LEVEL],\n    mxs=c21l.block_affine_matrices_da\n)\n\n# write the registered images to a pyramidal ome-tiff\npalom.pyramid.write_pyramid(\n    mosaics=palom.pyramid.normalize_mosaics([\n        # select only the first three channels in referece image to be written\n        # to the output ome-tiff; for writing all channels, use\n        # `c1r.pyramid[LEVEL]` instead\n        c1r.read_level_channels(LEVEL, [0, 1, 2]),\n        c2m\n    ]),\n    output_path=r"Z:\\P37_Pilot2\\mosaic.ome.tif",\n    pixel_size=c1r.pixel_size*c1r.level_downsamples[LEVEL]\n)\n```\n',
-    'author': 'Yu-An Chen',
-    'author_email': 'atwood12@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://pypi.org/project/palom/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.8,<4.0.0',
-}
+---
 
+## Installation
+
+Installing palom in a fresh conda environment is recommended. [Instruction for
+installing miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+### Step 1
+
+Create a named conda environment - _palom_, in the following example, and activate the environment.
+
+```
+conda create -n palom python=3.10 pip -c conda-forge
+conda activate palom
+```
+
+### Step 2
+
+Install openslide in the conda environment.
+
+- For MacOS, use conda-forge channel
+
+```
+conda install openslide -c conda-forge
+```
+
+- For Windows and Linux, use sdvillal channel
+
+```
+conda install openslide -c sdvillal
+```
+
+### Step 3
+
+Install palom from pypi in the conda environment.
+
+```
+python -m pip install palom
+```
+
+---
+
+## CLI usage
+
+### Configuration YAML file
+
+Palom CLI tool merges multiple SVS files into a pyramidal OME-TIFF file, with
+the option to perform preset stain separation (5 modes are available - `output
+mode`: `hematoxylin`, `aec`, `dab`, `grayscale`, `color`)
+
+A user-defined configuration YAML file is required for the run. A configuration
+example can be printed to the console by running
+
+```bash
+palom-svs show example
+```
+
+```yaml
+input dir: Y:\user\me\projects\data\mihc
+output full path: Y:\user\me\projects\analysis\mihc\2021\skin-case-356.ome.tif
+
+reference image:
+    filename: 20210111/skin_case_356_HEM_C11R3_HEM.svs
+    output mode: hematoxylin
+    channel name: Hematoxylin
+
+moving images:
+- filename: 20210101/skin_case_356_HEM_C01R1_PD1.svs
+  output mode: aec
+  channel name: PD-1
+- filename: 20210101/skin_case_356_HEM_C01R2_PDL1.svs
+  output mode: aec
+  channel name: PD-L1
+```
+
+To show the configuration schema, run the following command
+
+```bash
+palom-svs show schema
+```
+
+### Use the helper script to generate the configuration file
+
+[A helper
+script](https://github.com/Yu-AnChen/palom/blob/main/palom/cli/helper.py) is
+included showing how to automatically generate the configuration file if the SVS
+files are organized and have specific naming pattern.
+
+Here's an example directory containing many SVS files
+
+```
+Y:\DATA\SARDANA\MIHC\768473\RAW
+    CBB_SARDANA_768473_C04R1_CD8.svs
+    KB_SARDANA_768473_C01R1_PD1.svs
+    KB_SARDANA_768473_C01R2_PDL1.svs
+    KB_SARDANA_768473_C01R3_Hem.svs
+    KB_SARDANA_768473_C02R1_CD4.svs
+    KB_SARDANA_768473_C03R1_CD3.svs
+    KB_SARDANA_768473_C03R3_DCLAMP.svs
+```
+
+Running the following command to generate the configuration file
+
+```bash
+palom-svs-helper -i "Y:\DATA\SARDANA\MIHC\768473\RAW" -n "*Hem*" -o "Y:\DATA\SARDANA\MIHC\768473\RAW\palom\768473.ome.tif" -c "Y:\DATA\SARDANA\MIHC\768473\768473.yml"
+```
+
+And the resulting `Y:\DATA\SARDANA\MIHC\768473\768473.yml` file 
+
+```yaml
+input dir: Y:\DATA\SARDANA\MIHC\768473\RAW
+output full path: Y:\DATA\SARDANA\MIHC\768473\RAW\palom\768473.ome.tif
+reference image:
+  filename: .\KB_SARDANA_768473_C01R3_Hem.svs
+  output mode: hematoxylin
+  channel name: Hem-C01R3
+moving images:
+- filename: .\KB_SARDANA_768473_C01R1_PD1.svs
+  output mode: aec
+  channel name: PD1-C01R1
+- filename: .\KB_SARDANA_768473_C01R2_PDL1.svs
+  output mode: aec
+  channel name: PDL1-C01R2
+- filename: .\KB_SARDANA_768473_C02R1_CD4.svs
+  output mode: aec
+  channel name: CD4-C02R1
+- filename: .\KB_SARDANA_768473_C03R1_CD3.svs
+  output mode: aec
+  channel name: CD3-C03R1
+- filename: .\KB_SARDANA_768473_C03R3_DCLAMP.svs
+  output mode: aec
+  channel name: DCLAMP-C03R3
+- filename: .\CBB_SARDANA_768473_C04R1_CD8.svs
+  output mode: aec
+  channel name: CD8-C04R1
+```
+
+After reviewing the configuration file, process those SVS files by running
+
+```bash
+palom-svs run -c "Y:\DATA\SARDANA\MIHC\768473\768473.yml"
+```
+
+When the process is finished, a pyramidal OME-TIFF file will be generated along
+with PNG files showing the feature-based registration results and a log file. 
+
+```
+Y:\DATA\SARDANA\MIHC\768473\RAW
+│   CBB_SARDANA_768473_C04R1_CD8.svs
+│   KB_SARDANA_768473_C01R1_PD1.svs
+│   KB_SARDANA_768473_C01R2_PDL1.svs
+│   KB_SARDANA_768473_C01R3_Hem.svs
+│   KB_SARDANA_768473_C02R1_CD4.svs
+│   KB_SARDANA_768473_C03R1_CD3.svs
+│   KB_SARDANA_768473_C03R3_DCLAMP.svs
+│
+└───palom
+    │   768473.ome.tif
+    │
+    └───qc
+            01-KB_SARDANA_768473_C01R1_PD1.svs.png
+            02-KB_SARDANA_768473_C01R2_PDL1.svs.png
+            03-KB_SARDANA_768473_C02R1_CD4.svs.png
+            04-KB_SARDANA_768473_C03R1_CD3.svs.png
+            05-KB_SARDANA_768473_C03R3_DCLAMP.svs.png
+            06-CBB_SARDANA_768473_C04R1_CD8.svs.png
+            768473.ome.tif.log
+```
+
+---
+
+## Scripting
+
+__WARNING__ API may change in the future
+
+### For SVS files
+
+```python
+import palom
+
+c1r = palom.reader.SvsReader(r'Y:\DATA\SARDANA\MIHC\75684\GG_TNP_75684_D21_C11R3_HEM.svs')
+c2r = palom.reader.SvsReader(r'Y:\DATA\SARDANA\MIHC\75684\GG_TNP_75684_D23_C01R1_PD1.svs')
+
+LEVEL = 1
+THUMBNAIL_LEVEL = 2
+
+c1rp = palom.color.PyramidHaxProcessor(c1r.pyramid, thumbnail_level=THUMBNAIL_LEVEL)
+c2rp = palom.color.PyramidHaxProcessor(c2r.pyramid, thumbnail_level=THUMBNAIL_LEVEL)
+
+c21l = palom.align.Aligner(
+    c1rp.get_processed_color(LEVEL), 
+    c2rp.get_processed_color(LEVEL),
+    ref_thumbnail=c1rp.get_processed_color(THUMBNAIL_LEVEL).compute(),
+    moving_thumbnail=c2rp.get_processed_color(THUMBNAIL_LEVEL).compute(),
+    ref_thumbnail_down_factor=c1r.level_downsamples[THUMBNAIL_LEVEL] / c1r.level_downsamples[LEVEL],
+    moving_thumbnail_down_factor=c2r.level_downsamples[THUMBNAIL_LEVEL] / c2r.level_downsamples[LEVEL]
+)
+
+c21l.coarse_register_affine()
+c21l.compute_shifts()
+c21l.constrain_shifts()
+
+c21l.block_affine_matrices_da
+
+c2m = palom.align.block_affine_transformed_moving_img(
+    c1rp.get_processed_color(LEVEL),
+    c2rp.get_processed_color(LEVEL, 'aec'),
+    mxs=c21l.block_affine_matrices_da
+)
+
+palom.pyramid.write_pyramid(
+    palom.pyramid.normalize_mosaics([c2m]),
+    r"Y:\DATA\SARDANA\MIHC\75684\mosaic.ome.tif",
+    pixel_size=c1r.pixel_size*c1r.level_downsamples[LEVEL],
+)
+```
+
+### For TIFF and OME-TIFF files
+
+```python
+import palom
+
+# reference image is a multichannel immunofluoroscence imaging
+c1r = palom.reader.OmePyramidReader(r"Z:\P37_Pilot2\P37_S12_Full.ome.tiff")
+# moving image is a brightfield imaging (H&E staining) of the same tissue
+# section as the reference image
+c2r = palom.reader.OmePyramidReader(r"Z:\P37_Pilot2\HE\P37_S12_E033_93_HE.ome.tiff")
+
+# use second-to-the-bottom pyramid level for a quick test; set `LEVEL = 0` for
+# processing lowest level pyramid (full resolution)
+LEVEL = 1
+# choose thumbnail pyramid level for feature-based affine registration as
+# initial coarse alignment
+# `THUMBNAIL_LEVEL = c1r.get_thumbnail_level_of_size(2000)` might be a good
+# starting point
+THUMBNAIL_LEVEL = 3
+
+c21l = palom.align.Aligner(
+    # use the first channel (Hoechst staining) in the reference image as the
+    # registration reference
+    ref_img=c1r.read_level_channels(LEVEL, 0),
+    # use the second channel (G channel) in the moving image, it usually has
+    # better contrast
+    moving_img=c2r.read_level_channels(LEVEL, 1),
+    # select the same channels for the thumbnail images
+    ref_thumbnail=c1r.read_level_channels(THUMBNAIL_LEVEL, 0).compute(),
+    moving_thumbnail=c2r.read_level_channels(THUMBNAIL_LEVEL, 1).compute(),
+    # specify the downsizing factors so that the affine matrix can be scaled to
+    # match the registration reference
+    ref_thumbnail_down_factor=c1r.level_downsamples[THUMBNAIL_LEVEL] / c1r.level_downsamples[LEVEL],
+    moving_thumbnail_down_factor=c2r.level_downsamples[THUMBNAIL_LEVEL] / c2r.level_downsamples[LEVEL]
+)
+
+# run feature-based affine registration using thumbnails
+c21l.coarse_register_affine(n_keypoints=4000)
+# after coarsly affine registered, run phase correlation on each of the
+# corresponding chunks (blocks/pieces) to refine translations
+c21l.compute_shifts()
+# discard incorrect shifts which is usually due to low contrast in the
+# background regions; this is needed for WSI but maybe not for ROI images
+c21l.constrain_shifts()
+
+# configure the transformation of aligning the moving image to the registration
+# reference
+c2m = palom.align.block_affine_transformed_moving_img(
+    ref_img=c1r.read_level_channels(LEVEL, 0),
+    # select all the three channels (RGB) in moving image to transform
+    moving_img=c2r.pyramid[LEVEL],
+    mxs=c21l.block_affine_matrices_da
+)
+
+# write the registered images to a pyramidal ome-tiff
+palom.pyramid.write_pyramid(
+    mosaics=palom.pyramid.normalize_mosaics([
+        # select only the first three channels in referece image to be written
+        # to the output ome-tiff; for writing all channels, use
+        # `c1r.pyramid[LEVEL]` instead
+        c1r.read_level_channels(LEVEL, [0, 1, 2]),
+        c2m
+    ]),
+    output_path=r"Z:\P37_Pilot2\mosaic.ome.tif",
+    pixel_size=c1r.pixel_size*c1r.level_downsamples[LEVEL]
+)
+```
 
-setup(**setup_kwargs)
```

