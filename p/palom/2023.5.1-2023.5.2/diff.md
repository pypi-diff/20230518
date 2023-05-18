# Comparing `tmp/palom-2023.5.1.tar.gz` & `tmp/palom-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palom-2023.5.1.tar", max compression
+gzip compressed data, was "palom-2023.5.2.tar", max compression
```

## Comparing `palom-2023.5.1.tar` & `palom-2023.5.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     9486 2023-05-18 04:20:32.792050 palom-2023.5.1/README.md
--rw-r--r--   0        0        0      331 2023-05-18 04:20:22.703787 palom-2023.5.1/palom/__init__.py
--rw-r--r--   0        0        0     9679 2023-05-18 04:20:32.791173 palom-2023.5.1/palom/align.py
--rw-r--r--   0        0        0     3449 2023-05-17 03:40:00.979667 palom-2023.5.1/palom/block_affine.py
--rw-r--r--   0        0        0        0 2022-11-16 17:08:01.770570 palom-2023.5.1/palom/cli/__init__.py
--rw-r--r--   0        0        0     5352 2023-05-18 04:20:32.791222 palom-2023.5.1/palom/cli/align_he.py
--rw-r--r--   0        0        0    11965 2023-05-18 04:20:32.791300 palom-2023.5.1/palom/cli/flow.py
--rw-r--r--   0        0        0     2694 2022-11-16 17:08:01.770704 palom-2023.5.1/palom/cli/helper.py
--rw-r--r--   0        0        0      284 2022-11-16 17:08:01.770861 palom-2023.5.1/palom/cli/schema/__init__.py
--rw-r--r--   0        0        0      471 2022-11-16 17:08:01.770975 palom-2023.5.1/palom/cli/schema/svs-config-example.yml
--rw-r--r--   0        0        0     1842 2022-11-16 17:08:01.771106 palom-2023.5.1/palom/cli/schema/svs-config-schema.yml
--rw-r--r--   0        0        0     9132 2023-05-17 04:20:02.909374 palom-2023.5.1/palom/cli/svs.py
--rw-r--r--   0        0        0     3855 2023-05-18 04:20:32.792018 palom-2023.5.1/palom/color.py
--rw-r--r--   0        0        0     1803 2022-11-16 17:08:01.771500 palom-2023.5.1/palom/extract.py
--rw-r--r--   0        0        0     2610 2023-05-17 04:20:02.909766 palom-2023.5.1/palom/img_util.py
--rw-r--r--   0        0        0     7642 2023-05-18 01:07:11.995667 palom-2023.5.1/palom/pyramid.py
--rw-r--r--   0        0        0     6114 2023-05-17 04:20:02.909455 palom-2023.5.1/palom/reader.py
--rw-r--r--   0        0        0     8339 2023-05-17 03:40:00.981700 palom-2023.5.1/palom/register.py
--rw-r--r--   0        0        0     2665 2023-05-17 03:40:00.981734 palom-2023.5.1/palom/register_util.py
--rw-r--r--   0        0        0      979 2023-05-18 04:28:01.340556 palom-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0    10422 1970-01-01 00:00:00.000000 palom-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0     9417 2023-05-18 04:54:34.668047 palom-2023.5.2/README.md
+-rw-r--r--   0        0        0      330 2023-05-18 04:54:34.665691 palom-2023.5.2/palom/__init__.py
+-rw-r--r--   0        0        0     9662 2023-05-18 04:54:34.665840 palom-2023.5.2/palom/align.py
+-rw-r--r--   0        0        0     3446 2023-05-18 04:54:34.666753 palom-2023.5.2/palom/block_affine.py
+-rw-r--r--   0        0        0        0 2022-11-16 17:08:01.770570 palom-2023.5.2/palom/cli/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-18 04:54:34.666702 palom-2023.5.2/palom/cli/align_he.py
+-rw-r--r--   0        0        0    11953 2023-05-18 04:54:34.666352 palom-2023.5.2/palom/cli/flow.py
+-rw-r--r--   0        0        0     2690 2023-05-18 04:54:34.666887 palom-2023.5.2/palom/cli/helper.py
+-rw-r--r--   0        0        0     3081 2023-05-18 04:42:47.392902 palom-2023.5.2/palom/cli/pyramid_tools.py
+-rw-r--r--   0        0        0      284 2022-11-16 17:08:01.770861 palom-2023.5.2/palom/cli/schema/__init__.py
+-rw-r--r--   0        0        0      471 2022-11-16 17:08:01.770975 palom-2023.5.2/palom/cli/schema/svs-config-example.yml
+-rw-r--r--   0        0        0     1840 2023-05-18 04:54:34.667328 palom-2023.5.2/palom/cli/schema/svs-config-schema.yml
+-rw-r--r--   0        0        0     9096 2023-05-18 04:54:34.667007 palom-2023.5.2/palom/cli/svs.py
+-rw-r--r--   0        0        0     3850 2023-05-18 04:54:34.667057 palom-2023.5.2/palom/color.py
+-rw-r--r--   0        0        0     1802 2023-05-18 04:54:34.667089 palom-2023.5.2/palom/extract.py
+-rw-r--r--   0        0        0     3189 2023-05-18 04:54:34.667513 palom-2023.5.2/palom/img_util.py
+-rw-r--r--   0        0        0     9037 2023-05-18 04:54:34.667434 palom-2023.5.2/palom/pyramid.py
+-rw-r--r--   0        0        0     6109 2023-05-18 04:54:34.667748 palom-2023.5.2/palom/reader.py
+-rw-r--r--   0        0        0     8328 2023-05-18 04:54:34.667786 palom-2023.5.2/palom/register.py
+-rw-r--r--   0        0        0     2663 2023-05-18 04:54:34.667871 palom-2023.5.2/palom/register_util.py
+-rw-r--r--   0        0        0      979 2023-05-18 04:54:36.596686 palom-2023.5.2/pyproject.toml
+-rw-r--r--   0        0        0    10353 1970-01-01 00:00:00.000000 palom-2023.5.2/PKG-INFO
```

### Comparing `palom-2023.5.1/README.md` & `palom-2023.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 Running the following command to generate the configuration file
 
 ```bash
 palom-svs-helper -i "Y:\DATA\SARDANA\MIHC\768473\RAW" -n "*Hem*" -o "Y:\DATA\SARDANA\MIHC\768473\RAW\palom\768473.ome.tif" -c "Y:\DATA\SARDANA\MIHC\768473\768473.yml"
 ```
 
-And the resulting `Y:\DATA\SARDANA\MIHC\768473\768473.yml` file 
+And the resulting `Y:\DATA\SARDANA\MIHC\768473\768473.yml` file
 
 ```yaml
 input dir: Y:\DATA\SARDANA\MIHC\768473\RAW
 output full path: Y:\DATA\SARDANA\MIHC\768473\RAW\palom\768473.ome.tif
 reference image:
   filename: .\KB_SARDANA_768473_C01R3_Hem.svs
   output mode: hematoxylin
@@ -149,15 +149,15 @@
 After reviewing the configuration file, process those SVS files by running
 
 ```bash
 palom-svs run -c "Y:\DATA\SARDANA\MIHC\768473\768473.yml"
 ```
 
 When the process is finished, a pyramidal OME-TIFF file will be generated along
-with PNG files showing the feature-based registration results and a log file. 
+with PNG files showing the feature-based registration results and a log file.
 
 ```
 Y:\DATA\SARDANA\MIHC\768473\RAW
 │   CBB_SARDANA_768473_C04R1_CD8.svs
 │   KB_SARDANA_768473_C01R1_PD1.svs
 │   KB_SARDANA_768473_C01R2_PDL1.svs
 │   KB_SARDANA_768473_C01R3_Hem.svs
@@ -195,15 +195,15 @@
 LEVEL = 1
 THUMBNAIL_LEVEL = 2
 
 c1rp = palom.color.PyramidHaxProcessor(c1r.pyramid, thumbnail_level=THUMBNAIL_LEVEL)
 c2rp = palom.color.PyramidHaxProcessor(c2r.pyramid, thumbnail_level=THUMBNAIL_LEVEL)
 
 c21l = palom.align.Aligner(
-    c1rp.get_processed_color(LEVEL), 
+    c1rp.get_processed_color(LEVEL),
     c2rp.get_processed_color(LEVEL),
     ref_thumbnail=c1rp.get_processed_color(THUMBNAIL_LEVEL).compute(),
     moving_thumbnail=c2rp.get_processed_color(THUMBNAIL_LEVEL).compute(),
     ref_thumbnail_down_factor=c1r.level_downsamples[THUMBNAIL_LEVEL] / c1r.level_downsamples[LEVEL],
     moving_thumbnail_down_factor=c2r.level_downsamples[THUMBNAIL_LEVEL] / c2r.level_downsamples[LEVEL]
 )
 
@@ -216,15 +216,15 @@
 c2m = palom.align.block_affine_transformed_moving_img(
     c1rp.get_processed_color(LEVEL),
     c2rp.get_processed_color(LEVEL, 'aec'),
     mxs=c21l.block_affine_matrices_da
 )
 
 palom.pyramid.write_pyramid(
-    palom.pyramid.normalize_mosaics([c2m]),
+    [c2m],
     r"Y:\DATA\SARDANA\MIHC\75684\mosaic.ome.tif",
     pixel_size=c1r.pixel_size*c1r.level_downsamples[LEVEL],
 )
 ```
 
 ### For TIFF and OME-TIFF files
 
@@ -278,18 +278,18 @@
     # select all the three channels (RGB) in moving image to transform
     moving_img=c2r.pyramid[LEVEL],
     mxs=c21l.block_affine_matrices_da
 )
 
 # write the registered images to a pyramidal ome-tiff
 palom.pyramid.write_pyramid(
-    mosaics=palom.pyramid.normalize_mosaics([
+    mosaics=[
         # select only the first three channels in referece image to be written
         # to the output ome-tiff; for writing all channels, use
         # `c1r.pyramid[LEVEL]` instead
         c1r.read_level_channels(LEVEL, [0, 1, 2]),
         c2m
-    ]),
+    ],
     output_path=r"Z:\P37_Pilot2\mosaic.ome.tif",
     pixel_size=c1r.pixel_size*c1r.level_downsamples[LEVEL]
 )
 ```
```

### Comparing `palom-2023.5.1/palom/align.py` & `palom-2023.5.2/palom/align.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,20 +89,20 @@
             plt.cm.gray(np.linspace(0.5, 1, 256))
         ])
     )
     im = ax.imshow(distances.reshape(grid_shape), norm=divnorm, cmap=custom_cmap)
     cax = ax.inset_axes([1.04, 0.0, 0.02, 1])
     colorbar = plt.colorbar(im, cax=cax)
     colorbar.set_ticks(colorbar_ticks)
-    
+   
     return ax
 
 
 def block_affine_matrices(mx, shifts):
-        
+       
     def shift_affine_mx(mx, shift):
         y, x = shift
         mx_shift = np.eye(3)
         mx_shift[:2, 2] = x, y
         return mx_shift @ mx
 
     mxs = [
@@ -151,45 +151,45 @@
         affine_matrix = register.feature_based_registration(
             ref_img, moving_img,
             **default_kwargs
         )
         self.coarse_affine_matrix = np.vstack(
             [affine_matrix, [0, 0, 1]]
         )
-    
+   
     @property
     def affine_matrix(self):
         if not hasattr(self, 'coarse_affine_matrix'):
             self.coarse_register_affine()
         affine = skimage.transform.AffineTransform
         mx_ref = affine(scale=1/self.ref_thumbnail_down_factor).params
         mx_moving = affine(scale=1/self.moving_thumbnail_down_factor).params
         affine_matrix = (
             np.linalg.inv(mx_ref) @
             self.coarse_affine_matrix.copy() @
             mx_moving
         )
         return affine_matrix
-    
+   
     @property
     def tform(self):
         return skimage.transform.AffineTransform(
             matrix=self.affine_matrix
         )
-    
+   
     def affine_transformed_moving_img(self, mxs=None):
         if mxs is None:
             mxs = self.affine_matrix
         ref_img = self.ref_img
         moving_img = self.moving_img
 
         return block_affine_transformed_moving_img(
             ref_img, moving_img, mxs
         )
-    
+   
     def compute_shifts(self, pcc_kwargs=None):
         logger.info(f"Computing block-wise shifts")
         ref_img = self.ref_img
         moving_img = self.affine_transformed_moving_img(self.affine_matrix)
         shifts_da = block_shifts(ref_img, moving_img, pcc_kwargs=pcc_kwargs)
         with tqdm.dask.TqdmCallback(
             ascii=True, desc='Computing shifts',
@@ -208,29 +208,29 @@
     def constrain_shifts(self):
         if not hasattr(self, 'original_shifts'):
             self.original_shifts = self.shifts.copy()
         self.shifts = constrain_block_shifts(
             self.original_shifts,
             self.grid_shape
         )
-    
+   
     @property
     def block_affine_matrices(self):
         mx = self.affine_matrix
         shifts = self.shifts
         return block_affine_matrices(mx, shifts)
 
     @property
     def block_affine_matrices_da(self):
         return block_affine_matrices_da(
             self.block_affine_matrices,
             self.grid_shape
         )
 
-    def overlay_grid(self, ax=None): 
+    def overlay_grid(self, ax=None):
         import matplotlib.pyplot as plt
         img = self.ref_thumbnail
         img = skimage.exposure.rescale_intensity(img, out_range=np.uint16)
         shape = self.grid_shape
         grid = np.arange(np.multiply(*shape)).reshape(shape)
         h, w = np.divide(
             img.shape,
@@ -245,15 +245,15 @@
             func(img),
             cmap=cmap,
             extent=(-0.5, w-0.5, h-0.5, -0.5)
         )
         # checkerboard pattern
         ax.imshow(np.indices(shape).sum(axis=0) % 2, cmap='cool', alpha=0.2)
         return grid
-    
+   
     def plot_shifts(self):
         import matplotlib.pyplot as plt
         fig, axs = plt.subplots(1, 2, sharex=True, sharey=True)
         self.overlay_grid(axs[0])
         shifts = getattr(self, 'original_shifts', self.shifts)
         viz_shifts(shifts, self.grid_shape, ax=axs[1])
         return fig
@@ -267,22 +267,22 @@
 ):
     if None in [thumbnail_level1, thumbnail_level2]:
         thumbnail_level1, thumbnail_level2 = match_thumbnail_level(
             [reader1, reader2]
         )
     if thumbnail_level1 <= -1: thumbnail_level1 += len(reader1.pyramid)
     if thumbnail_level2 <= -1: thumbnail_level2 += len(reader2.pyramid)
-    return Aligner( 
-        reader1.read_level_channels(level1, channel1),  
-        reader2.read_level_channels(level2, channel2), 
-        reader1.read_level_channels(thumbnail_level1, channel1), 
-        reader2.read_level_channels(thumbnail_level2, channel2), 
-        reader1.level_downsamples[thumbnail_level1] / reader1.level_downsamples[level1], 
-        reader2.level_downsamples[thumbnail_level2] / reader2.level_downsamples[level2] 
-    ) 
+    return Aligner(
+        reader1.read_level_channels(level1, channel1), 
+        reader2.read_level_channels(level2, channel2),
+        reader1.read_level_channels(thumbnail_level1, channel1),
+        reader2.read_level_channels(thumbnail_level2, channel2),
+        reader1.level_downsamples[thumbnail_level1] / reader1.level_downsamples[level1],
+        reader2.level_downsamples[thumbnail_level2] / reader2.level_downsamples[level2]
+    )
 
 
 def match_thumbnail_level(readers):
     assert len(readers) > 1
     level_px_sizes = [
         {
             rr.pixel_size*vv: kk
```

### Comparing `palom-2023.5.1/palom/block_affine.py` & `palom-2023.5.2/palom/block_affine.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,21 @@
         transformation, src_array,
         fill_empty=fill_empty, multichannel=multichannel,
         is_mask=is_mask
     )
 
 
 def block_affine(
-    position, block_shape, 
+    position, block_shape,
     transformation, src_img,
     fill_empty=0, multichannel=False,
     is_mask=False
 ):
     assert np.min(block_shape) >= 0, (
-        f'block_shape {block_shape} is invalid' 
+        f'block_shape {block_shape} is invalid'
     )
     if multichannel:
         assert np.min(block_shape) == block_shape[0], (
             'multichannel block must has shape of (C, Y, X)'
         )
         assert np.min(src_img.shape) == src_img.shape[0], (
             'multichannel image must be shaped as (C, Y, X)'
@@ -64,15 +64,15 @@
 
     x1_src, y1_src = np.ceil(
         np.clip(inversed_corners.max(axis=0), 0, None)
     ).astype(int)
     x0_src, y0_src = np.floor(
         np.clip(inversed_corners.min(axis=0), 0, None)
     ).astype(int)
-    
+   
     if multichannel:
         src_img_block = src_img[:, y0_src:y1_src, x0_src:x1_src]
         src_img_block = np.moveaxis(src_img_block, 0, 2)
     else:
         src_img_block = src_img[y0_src:y1_src, x0_src:x1_src]
     src_dtype = src_img.dtype
     if 0 in src_img_block.shape:
```

### Comparing `palom-2023.5.1/palom/cli/align_he.py` & `palom-2023.5.2/palom/cli/align_he.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,35 +38,35 @@
         channel1=thumbnail_channel1, channel2=thumbnail_channel2,
         level1=LEVEL, level2=LEVEL
     )
 
     aligner.coarse_register_affine(n_keypoints=5000, detect_flip_rotate=True)
     plt.gcf().suptitle(f"{p2.name} (coarse alignment)", fontsize=8)
     plt.gca().set_title(f"{p1.name} - {p2.name}", fontsize=6)
-    
+   
     if viz_coarse_napari:
         _ = viz_coarse(r1, r2, LEVEL, LEVEL, channel1, channel2, aligner.affine_matrix)
 
     if not only_coarse:
         aligner.ref_img = r1.read_level_channels(LEVEL, channel1)
         aligner.moving_img = r2.read_level_channels(LEVEL, channel2)
-        
+       
         aligner.compute_shifts()
-        
+       
         fig = aligner.plot_shifts()
         fig.suptitle(f"{p2.name} (block shift distance)", fontsize=8)
         fig.axes[0].set_title(p1.name, fontsize=6)
 
         aligner.constrain_shifts()
 
     set_matplotlib_font(font_size=8)
     save_all_figs(out_dir=out_dir / 'qc', format='png')
-    
+   
     if not only_qc:
-        mx = aligner.affine_matrix 
+        mx = aligner.affine_matrix
         if not only_coarse:
             mx = aligner.block_affine_matrices_da
         mosaic = palom.align.block_affine_transformed_moving_img(
             ref_img=aligner.ref_img,
             moving_img=r2.pyramid[LEVEL],
             mxs=mx
         )
@@ -80,15 +80,15 @@
     return 0
 
 
 def viz_coarse(r1, r2, level1, level2, channel1, channel2, mx):
     try:
         import napari
     except ImportError:
-        return 
+        return
     import dask.array as da
     v = napari.Viewer()
     is_bf1 = palom.img_util.is_brightfield_img(r1.pyramid[-1][channel1])
     is_bf2 = palom.img_util.is_brightfield_img(r2.pyramid[-1][channel2])
     inv = {True: da.invert, False: da.array}
     v.add_image(
         [inv[is_bf1](p[channel1]) for p in r1.pyramid[level1:]],
@@ -135,25 +135,25 @@
 
     fire.Fire(align_he)
 
     if '--viz_coarse_napari' in sys.argv:
         try: import napari
         except ImportError: print("napari is not installed")
         else: napari.run()
-    
+   
     '''
     Example 1: inspect coarse alignment using napari
     python align_he.py \
         Z:\RareCyte-S3\P54_CRCstudy_Bridge\P54_S33_Full_Or6_A31_C90c_HMS@20221025_001610_632297.ome.tiff \
         "X:\crc-scans\histowiz scans\20230105-orion_2_cycles\22199$P54_33_HE$US$SCAN$OR$001 _104050.svs" \
         "X:\crc-scans\histowiz scans\20230105-orion_2_cycles\test" \
         --px_size1 0.325 --only_qc --only_coarse --viz_coarse_napari
 
     Example 2: process pair and output registered image
     python align_he.py \
         Z:\RareCyte-S3\P54_CRCstudy_Bridge\P54_S33_Full_Or6_A31_C90c_HMS@20221025_001610_632297.ome.tiff \
         "X:\crc-scans\histowiz scans\20230105-orion_2_cycles\22199$P54_33_HE$US$SCAN$OR$001 _104050.svs" \
         "X:\crc-scans\histowiz scans\20230105-orion_2_cycles\test" \
         --px_size1 0.325
-    
+   
     '''
```

### Comparing `palom-2023.5.1/palom/cli/flow.py` & `palom-2023.5.2/palom/cli/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,28 +57,28 @@
     shape = Reader(p1).pyramid[0].shape[1:]
     ref = da.ones((1, *shape), chunks=chunk_size)
 
     mask_shape = da.ones(shape, chunks=block_size).numblocks
     if mask is None:
         mask = np.ones(mask_shape, dtype=bool)
     assert mask.shape == mask_shape
-    
+   
     def func(
         p1, p2, ch1, ch2, mask,
         block_info=None
     ):
         _, rloc, cloc = block_info[None]['array-location']
         chunk1 = Reader(p1).pyramid[0][ch1, slice(*rloc), slice(*cloc)]
         chunk2 = Reader(p2).pyramid[0][ch2, slice(*rloc), slice(*cloc)]
         chunk_mask = mask[
             slice(*np.ceil(np.divide(rloc, block_size)).astype(int)),
             slice(*np.ceil(np.divide(cloc, block_size)).astype(int))
         ]
         return block_optical_flow(chunk1, chunk2, block_size, mask=chunk_mask)
-    
+   
     shifts = da.map_blocks(
         func,
         p1=p1, p2=p2, ch1=ch1, ch2=ch2, mask=mask,
         dtype=float,
         chunks=ref.chunks,
     )
 
@@ -100,20 +100,20 @@
     img1 = np.asarray(img1)
     img2 = np.asarray(img2)
     block_shape = (block_size, block_size)
     block_shape = np.min(np.vstack([img1.shape, block_shape]), axis=0)
     wv_img1 = skimage.util.view_as_windows(img1, block_shape, block_shape)
     wv_img2 = skimage.util.view_as_windows(img2, block_shape, block_shape)
     h, w = wv_img1.shape[:2]
-    
+   
     wv_mask = np.ones((h, w, 1, 1), dtype=bool)
     if mask is not None:
         wv_mask = mask[..., np.newaxis, np.newaxis]
         wv_mask = wv_mask[..., :h, :w]
-    
+   
     out = np.zeros((3, h, w), dtype=np.float32)
     product_func = itertools.product
     if show_progress:
         product_func = tqdm.contrib.itertools.product
     idxs = product_func(range(h), range(w))
     for rr, cc in idxs:
         out[:, rr, cc] = pc(
@@ -154,15 +154,15 @@
         img2,
         in_range=(np.mean(img2[~mask]), np.percentile(img2[mask], 99.9)),
         out_range=np.float32
     )
     rimg2 = skimage.exposure.match_histograms(rimg2, rimg1)
     out = np.array([rimg1, rimg2, rimg1])
     return out
- 
+
 
 def plot_legend(
     shifts, max_radius, plot_scatter, plot_kde,
     pad_plot=False, plot_flow=False, ax=None
 ):
 
     import matplotlib.pylab as plt
@@ -248,15 +248,15 @@
 ):
     img_path = pathlib.Path(img_path)
     reader = palom.reader.OmePyramidReader(img_path)
 
     mask = None
     if compute_mask:
         mask = reader_block_mask(reader, block_size)
-    
+   
     num_cpus = dask.system.cpu_count()
     if num_workers > num_cpus:
         num_workers =num_cpus
 
     print()
     print(f"Processing {img_path.name} using {num_workers} cores")
     print(f"Block size: {block_size}; image shape {reader.pyramid[0].shape[1:]}")
@@ -305,24 +305,24 @@
 
         _ = plot_legend(
             shifts, max_radius, True, True, plot_flow=False, ax=fig.add_subplot(gs[3])
         )
 
         for ax in fig.get_axes():
             ax.set_anchor('N')
-        
+       
         plt.tight_layout()
         out_dir = img_path.parent / 'qc'
         out_dir.mkdir(exist_ok=True)
         fig.savefig(
             out_dir / f"flow-field-{img_path.stem}-channel-{ref_channel}-{channel}.png",
             bbox_inches='tight', dpi=144
         )
         figures.append(fig)
-    
+   
     if as_script: return
     return all_shifts, figures
 
 
 if __name__ == '__main__':
     import fire
     fire.Fire(process_img_channel_pair)
@@ -350,23 +350,23 @@
         -c, --compute_mask=COMPUTE_MASK
             Type: bool Default: True
         -n, --num_workers=NUM_WORKERS
             Type: int Default: 4
         -a, --as_script=AS_SCRIPT
             Default: True
 
-    --- 
-    
+    ---
+   
     NOTE: OTHER_CHANNELS is a list of integers, use [1] to indicate the
     second channel and [1,2,3] (do not include space) for second, third and
     fourth channels.
 
     Ref https://google.github.io/python-fire/guide/#argument-parsing
-    
-    Examples 
+   
+    Examples
 
     python flow.py \
         "Z:\RareCyte-S3\P54_CRCstudy_Bridge\S32-Tonsil-P54_Strip_P76.ome.tif" \
         0 [1,2,3] \
         128
 
     python flow.py \
```

### Comparing `palom-2023.5.1/palom/cli/helper.py` & `palom-2023.5.2/palom/cli/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def main(argv=sys.argv):
 
     parser = argparse.ArgumentParser(
         description=(
             'Generate configuration yaml file for palom-svs run'
         )
     )
-    
+   
     parser.add_argument(
         '-i',
         metavar='input-dir',
         help='directory that contains all the SVS files to be processed',
         required=True
     )
     parser.add_argument(
@@ -32,17 +32,17 @@
     )
     parser.add_argument(
         '-c',
         metavar='yaml-path',
         help='full path to the resulting configuration yaml file',
         required=True
     )
-    
+   
     args = parser.parse_args(argv[1:])
-    
+   
     if len(argv) == 1:
         parser.print_help()
         return 0
 
     svs_dir = pathlib.Path(args.i)
     name_pattern = args.n
     output_path = pathlib.Path(args.o)
@@ -64,15 +64,15 @@
             break
 
     assert ref_slide is not None, (
         f"Cannot find reference SVS file with name pattern: {name_pattern}"
     )
 
     channel_names = [
-        '-'.join(p.name.split('_')[-2:][::-1]).replace('.svs', '') 
+        '-'.join(p.name.split('_')[-2:][::-1]).replace('.svs', '')
         for p in ([ref_slide] + svs_paths)
     ]
 
     config = {
         'input dir': str(svs_dir),
         'output full path': str(output_path),
         'reference image': {
```

### Comparing `palom-2023.5.1/palom/cli/schema/svs-config-schema.yml` & `palom-2023.5.2/palom/cli/schema/svs-config-schema.yml`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
 ---
 # Image object schema
 image collection: any(include('bright-field image'), include('fluorescent image'))
 
 _image_base: &_image_base
     # Filename or the remaining path to the imaging data relative to the input
-    # dir field 
+    # dir field
     filename: str()
     # [optional but recommended]
     # Channel name in the output ome-tiff
     channel name: str(required=False)
     channel names: list(str(), min=1, required=False)
 
 bright-field image:
     <<: *_image_base
     channel names: list(str(), min=1, max=3, required=False)
     # Output color mode, currently the following 4 modes are available
     output mode: enum('aec', 'hematoxylin', 'color', 'grayscale', 'dab')
-  
+ 
 fluorescent image:
     <<: *_image_base
     output mode: str(equals='multichannel')
     output channels: list(int(min=1), required=False)
 
 output format: any(str(ends_with='.ome.tif'), str(ends_with='.ome.tiff'))
```

### Comparing `palom-2023.5.1/palom/cli/svs.py` & `palom-2023.5.2/palom/cli/svs.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,19 +63,19 @@
             ' `palom-svs show example`'
         ),
         required=True
     )
     parser_run.set_defaults(func=run)
 
     args = parser.parse_args(argv[1:])
-    
+   
     if len(argv) == 1:
         parser.print_help()
         return 0
-    
+   
     if args.version:
         print(f"palom v{_version}")
         return 0
 
     return args.func(args)
 
 
@@ -106,15 +106,15 @@
     logger.info(f"Running palom v{_version}")
     logger.info(f"Reading {config_file.name}\n\n{config_file.read().strip()}\n")
     config_file.close()
 
     config_data = yamale.make_data(config_file.name)
     if validate_config(config_data) == 1:
         return 1
-    
+   
     config = config_data[0][0]
 
     LEVEL = 0
     if 'pyramid level' in config:
         LEVEL = config['pyramid level']
 
     if 'pixel size' in config:
@@ -123,15 +123,15 @@
     else: pixel_size = None
 
     DOWNSCALE_FACTOR = 4
     if 'pyramid downscale factor' in config:
         DOWNSCALE_FACTOR = config['pyramid downscale factor']
 
     images = get_image_list(config)
-    
+   
     image_paths = [
         pathlib.Path(config['input dir']) / pathlib.Path(i['filename'])
         for i in images
     ]
 
     image_output_modes = [
         i['output mode']
@@ -162,15 +162,15 @@
         channel_names=channel_names,
         output_path=output_path,
         qc_path=qc_path,
         level=LEVEL,
         downscale_factor=DOWNSCALE_FACTOR
     )
 
-    logger.info(f"Finishing {config_file.name}")    
+    logger.info(f"Finishing {config_file.name}")   
     logger.remove(logger_id)
     # Can't `pathlib.Path.replace` across different disk drive
     shutil.copy(log_path, qc_path / f"{output_path.name}.log")
     log_path.unlink()
 
     return run_result
 
@@ -205,30 +205,30 @@
             ref_color_proc.get_processed_color(ref_thumbnail_level, 'grayscale').compute(),
             moving_color_proc.get_processed_color(moving_thumbnail_level, 'grayscale').compute(),
             ref_reader.level_downsamples[ref_thumbnail_level] / ref_reader.level_downsamples[level],
             moving_reader.level_downsamples[moving_thumbnail_level] / moving_reader.level_downsamples[level]
         )
 
         aligner.coarse_register_affine()
-        
-        # FIXME move the saving figure logic 
+       
+        # FIXME move the saving figure logic
         plt.suptitle(f"L: {ref_reader.path.name}\nR: {p.name}")
         fig_w = max(plt.gca().get_xlim())
         fig_h = max(plt.gca().get_ylim()) + 100
         factor = 1600 / max(fig_w, fig_h)
         plt.gcf().set_size_inches(fig_w*factor/72, fig_h*factor/72)
         plt.tight_layout()
         plt.savefig(qc_path / f"{idx+1:02d}-{p.name}.png", dpi=72)
         plt.close()
-        
+       
         aligner.compute_shifts()
         aligner.constrain_shifts()
 
         block_affines.append(aligner.block_affine_matrices_da)
-    
+   
     mosaics = []
     m_ref = ref_color_proc.get_processed_color(level=level, mode=img_modes[0])
     mosaics.append(m_ref)
     for p, m, mx in zip(img_paths[1:], img_modes[1:], block_affines):
         moving_color_proc = color.PyramidHaxProcessor(
             reader.SvsReader(p).pyramid
         )
@@ -239,15 +239,15 @@
         )
         mosaics.append(m_moving)
 
     if pixel_size is None:
         pixel_size = ref_reader.pixel_size
 
     pyramid.write_pyramid(
-        pyramid.normalize_mosaics(mosaics),
+        mosaics,
         output_path,
         pixel_size=pixel_size,
         channel_names=channel_names,
         downscale_factor=downscale_factor
     )
     return 0
```

### Comparing `palom-2023.5.1/palom/color.py` & `palom-2023.5.2/palom/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,21 +18,21 @@
         assert self.contrast_ref_img.ndim == 3, (
             f"`contrast_ref_img` must be 3D, preferably in (C, Y, X) order"
         )
 
     def find_processed_color_contrast_range(self, mode: str):
         supported_modes = ['grayscale', 'hematoxylin', 'aec', 'dab']
         assert mode in supported_modes
-        
+       
         mode_range = f'_{mode}_range'
         if hasattr(self, mode_range):
             return getattr(self, mode_range)
-        
+       
         contrast_ref_img = self.contrast_img
-        
+       
         process_func = self.__getattribute__(f"rgb2{mode}")
         img = process_func(contrast_ref_img)
 
         setattr(self, mode_range, (
             img.min(), img.max()
         ))
         return getattr(self, mode_range)
@@ -64,15 +64,15 @@
         return hax[..., 0].astype(np.float32)
 
     def get_processed_color(self, rgb_img, mode='grayscale'):
         assert mode in ['grayscale', 'hematoxylin', 'aec', 'dab']
 
         process_func = self.__getattribute__(f"rgb2{mode}")
         intensity_range = self.find_processed_color_contrast_range(mode)
-        
+       
         processed = da.map_blocks(
             process_func,
             rgb_img,
             dtype=np.float32,
             drop_axis=2
         )
 
@@ -92,15 +92,15 @@
         pyramid: list[da.Array],
         thumbnail_level: int = None
     ) -> None:
         if thumbnail_level is None:
             thumbnail_level = len(pyramid) - 1
         super().__init__(pyramid[thumbnail_level], channel_axis=0)
         self.pyramid = pyramid
-    
+   
     def get_processed_color(self, level, mode='grayscale', out_dtype=None):
         if mode == 'color':
             return self.pyramid[level]
         rgb_img = np.moveaxis(self.pyramid[level], 0, 2)
         processed = super().get_processed_color(rgb_img, mode=mode)
         if out_dtype is None:
             out_dtype = rgb_img.dtype
```

### Comparing `palom-2023.5.1/palom/extract.py` & `palom-2023.5.2/palom/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     )
     channel_idx = shape.index(3)
     rgb_img = skimage.util.img_as_float(rgb_img)
     rgb = np.moveaxis(rgb_img, channel_idx, 0)
 
     cmy = 1-rgb
     k = cmy.min(axis=0)
-    
+   
     s = 1-k
 
     with warnings.catch_warnings():
         warnings.filterwarnings(
             'ignore', 'invalid value encountered in true_divide', RuntimeWarning,
         )
         f_cmy = (cmy-k) / s
```

### Comparing `palom-2023.5.1/palom/img_util.py` & `palom-2023.5.2/palom/img_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         size_max //= 2
     return pyramid
 
 
 def whiten(img, sigma=1):
     border_mode = cv2.BORDER_REFLECT
     g_img = img if sigma == 0 else cv2.GaussianBlur(
-        img, (0, 0), sigma, 
+        img, (0, 0), sigma,
         borderType=border_mode
     ).astype(np.float32)
     log_img = cv2.Laplacian(
         g_img, cv2.CV_32F, ksize=1,
         borderType=border_mode
     )
     # log_img = cv2.convertScaleAbs(log_img)
@@ -51,18 +51,19 @@
     entropy = skimage.filters.rank.entropy(img, np.ones((kernel_size, kernel_size)))
     return entropy > skimage.filters.threshold_otsu(entropy)
 
 
 def is_brightfield_img(img, max_size=100):
     img = np.array(img)
     downscale_factor = int(max(img.shape) / max_size)
-    thumbnail = skimage.transform.downscale_local_mean(img, (downscale_factor, downscale_factor))
-    mask = entropy_mask(thumbnail)
+    if downscale_factor > 1:
+        img = cv2_downscale_local_mean(img, downscale_factor)
+    mask = entropy_mask(img)
     # is using mean better?
-    return np.median(thumbnail[mask]) < np.median(thumbnail[~mask])
+    return np.median(img[mask]) < np.median(img[~mask])
 
 
 def block_labeled_mask(img_shape, block_shape, out_chunks=None):
     assert len(img_shape) == 2
     if len(block_shape) == 1:
         block_shape = (block_shape[0], block_shape[0])
     da_template = da.zeros(img_shape, chunks=block_shape)
@@ -76,11 +77,29 @@
         axis=1
     )[:img_shape[0], :img_shape[1]]
     if out_chunks is None:
         out_chunks = block_shape
     return da.from_array(full_mask, chunks=out_chunks)
 
 
-def to_napari_affine(mx): 
+def to_napari_affine(mx):
     ul = np.flip(mx[:2, :2], (0, 1))
     rows = np.hstack([ul, np.flipud(mx[:2, 2:3])])
-    return np.vstack((rows, [0, 0, 1]))
+    return np.vstack((rows, [0, 0, 1]))
+
+
+# orders of magnitute faster than skimage.transform.downscale_local_mean
+# also the gives sensible values of pixels on the edge
+def cv2_downscale_local_mean(img, factor):
+    assert img.ndim in [2, 3]
+    img = np.asarray(img)
+    axis_moved = False
+    channel_ax = np.argmin(img.shape)
+    if (img.ndim == 3) & (channel_ax != 2):
+        img = np.moveaxis(img, channel_ax, 2)
+        axis_moved = True
+    simg = cv2.blur(
+        img, ksize=(factor, factor), anchor=(0, 0)
+    )[::factor, ::factor]
+    if axis_moved:
+        simg = np.moveaxis(simg, 2, channel_ax)
+    return simg
```

### Comparing `palom-2023.5.1/palom/pyramid.py` & `palom-2023.5.2/palom/pyramid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import math
+
+import cv2
+import dask.array as da
+import numpy as np
 import tifffile
 import tqdm
-import numpy as np
-import skimage.transform
+import zarr
 from loguru import logger
 
 from . import __version__ as _version
 
 
 class PyramidSetting:
 
@@ -108,30 +111,40 @@
     mosaics,
     output_path,
     pixel_size=1,
     channel_names=None,
     verbose=True,
     downscale_factor=4,
     compression=None,
-    is_mask=False
+    is_mask=False,
+    tile_size=None,
+    save_RAM=False,
+    kwargs_tifffile=None
 ):
+    mosaics = normalize_mosaics(mosaics)
     ref_m = mosaics[0]
     path = output_path
     num_channels = count_num_channels(mosaics)
     base_shape = ref_m.shape[1:3]
     assert int(downscale_factor) == downscale_factor
     assert downscale_factor < min(base_shape)
     pyramid_setting = PyramidSetting(
         downscale_factor=int(downscale_factor),
         tile_size=max(ref_m.chunksize)
     )
     num_levels = pyramid_setting.num_levels(base_shape)
     tile_shapes = pyramid_setting.tile_shapes(base_shape)
     shapes = pyramid_setting.pyramid_shapes(base_shape)
 
+    if tile_size is not None:
+        assert tile_size % 16 == 0, (
+            f"tile_size must be None or multiples of 16, not {tile_size}"
+        )
+        tile_shapes = [(tile_size, tile_size)] * num_levels
+
     dtype = ref_m.dtype
 
     software = f'palom {_version}'
     pixel_size = pixel_size
     metadata = {
         'Creator': software,
         'Pixels': {
@@ -149,40 +162,46 @@
         if len(names) == num_channels:
             metadata.update({
                 'Channel': {'Name': names},
             })
 
     logger.info(f"Writing to {path}")
     with tifffile.TiffWriter(path, bigtiff=True) as tif:
+        kwargs = dict(
+            metadata=metadata,
+            software=software,
+            compression=compression
+        )
+        if kwargs_tifffile is None:
+            kwargs_tifffile = {}
         tif.write(
             data=tile_from_combined_mosaics(
-                mosaics, tile_shape=tile_shapes[0]
+                mosaics, tile_shape=tile_shapes[0], save_RAM=save_RAM
             ),
-            metadata=metadata,
-            software=software,
             shape=(num_channels, *shapes[0]),
             subifds=int(num_levels - 1),
             dtype=dtype,
-            compression=compression,
-            tile=tile_shapes[0]
+            tile=tile_shapes[0],
+            **{**kwargs, **kwargs_tifffile}
         )
         logger.info('Generating pyramid')
         for level, (shape, tile_shape) in enumerate(
             zip(shapes[1:], tile_shapes[1:])
         ):
             if verbose:
                 logger.info(f"    Level {level+1} ({shape[0]} x {shape[1]})")
             tif.write(
                 data=tile_from_pyramid(
                     path,
                     num_channels,
                     tile_shape=tile_shape,
                     downscale_factor=downscale_factor,
                     level=level,
-                    is_mask=is_mask
+                    is_mask=is_mask,
+                    save_RAM=save_RAM
                 ),
                 shape=(num_channels, *shape),
                 subfiletype=1,
                 dtype=dtype,
                 compression=compression,
                 tile=tile_shape
             )
@@ -191,57 +210,72 @@
 def count_num_channels(imgs):
     for img in imgs:
         assert img.ndim == 2 or img.ndim == 3
     return sum([
         1 if img.ndim == 2 else img.shape[0]
         for img in imgs
     ])
-    
+   
 
-def tile_from_combined_mosaics(mosaics, tile_shape):
+def tile_from_combined_mosaics(mosaics, tile_shape, save_RAM=False):
     num_rows, num_cols = mosaics[0].shape[1:3]
     h, w = tile_shape
     n = len(mosaics)
     for idx, m in enumerate(mosaics):
         for cidx, c in enumerate(m):
             # the performance is heavily degraded without pre-computing the
             # mosaic channel
             with tqdm.dask.TqdmCallback(
                 ascii=True,
                 desc=(
                     f"Assembling mosaic {idx+1:2}/{n:2} (channel"
                     f" {cidx+1:2}/{m.shape[0]:2})"
                 ),
             ):
-                c = c.compute()
+                c = c.persist() if save_RAM else c.compute()
             for y in range(0, num_rows, h):
                 for x in range(0, num_cols, w):
                     yield np.array(c[y:y+h, x:x+w])
-                # yield m[y:y+h, x:x+w].copy().compute()
+                    # yield m[y:y+h, x:x+w].copy().compute()
+            c = None
 
 
 def tile_from_pyramid(
     path,
     num_channels,
     tile_shape,
     downscale_factor=2,
     level=0,
-    is_mask=False
+    is_mask=False,
+    save_RAM=False
 ):
-    h, w = tile_shape
-    for c in tqdm.trange(
-            num_channels,
-            ascii=True, desc=f'Processing channel'
-        ):
-        img = tifffile.imread(
-            path, is_ome=False, series=0, key=c, level=level
-        )
-        if is_mask:
-            img = img[::downscale_factor, ::downscale_factor]
-        else:
-            img = skimage.transform.downscale_local_mean(
-                img, (downscale_factor, downscale_factor)
-            ).astype(img.dtype)
+    # workaround progress bar
+    # https://forum.image.sc/t/tifffile-ome-tiff-generation-is-taking-too-much-ram/41865/26
+    pbar = tqdm.tqdm(total=num_channels, ascii=True, desc=f'Processing channel')
+    for c in range(num_channels):
+        img = da.from_zarr(zarr.open(tifffile.imread(
+            path, series=0, level=level, aszarr=True
+        )))[c]
+        # read using key seems to generate a RAM spike
+        # img = tifffile.imread(path, series=0, level=level, key=c)
+        if not is_mask:
+            img = img.map_blocks(
+                cv2.blur,
+                ksize=(downscale_factor, downscale_factor), anchor=(0, 0)
+            )
+        img = img.persist() if save_RAM else img.compute()
         num_rows, num_columns = img.shape
+        h, w = tile_shape
+        h *= downscale_factor
+        w *= downscale_factor
+        last_c = range(num_channels)[-1]
+        last_y = range(0, num_rows, h)[-1]
+        last_x = range(0, num_columns, w)[-1]
         for y in range(0, num_rows, h):
             for x in range(0, num_columns, w):
-                yield np.array(img[y:y+h, x:x+w])
+                if (y == last_y) & (x == last_x):
+                    pbar.update(1)
+                    if c == last_c:
+                        pbar.close()
+                yield np.array(img[y:y+h:downscale_factor, x:x+w:downscale_factor])
+        # setting img to None seems necessary to prevent RAM spike
+        img = None
```

### Comparing `palom-2023.5.1/palom/reader.py` & `palom-2023.5.2/palom/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 
     @staticmethod
     def validate_pyramid(pyramid: list[da.Array], channel_axis:int) -> bool:
         for i, level in enumerate(pyramid):
             assert level.ndim == 3, ''
             if np.argmin(level.shape) != channel_axis:
                 logger.warning(
-                    f"level {i} has shape of {level.shape} while given" 
+                    f"level {i} has shape of {level.shape} while given"
                     f" `channel_axis` is {channel_axis}"
                 )
         return True
-    
+   
     def normalize_axis_order(self):
         if self.channel_axis == 0:
             return self.pyramid
         return [
             da.moveaxis(level, self.channel_axis, 0)
             for level in self.pyramid
         ]
@@ -79,15 +79,15 @@
 
     @property
     def level_downsamples(self) -> dict[int, int]:
         return {
             i: round(self.pyramid[0].shape[1] / level.shape[1])
             for i, level in enumerate(self.pyramid)
         }
-    
+   
     @property
     def pixel_dtype(self) -> np.dtype:
         return self.pyramid[0].dtype
 
     def get_thumbnail_level_of_size(self, size: float) -> int:
         shapes = [
             np.abs(np.mean(level.shape[1:3]) - size)
@@ -147,29 +147,29 @@
         path: str | pathlib.Path,
         pixel_size: float | None = None
     ) -> None:
         # FIXME maybe move napari_lazy_openslide to optional dependency?
         # https://python-poetry.org/docs/pyproject/#extras
         # https://github.com/AllenCellModeling/aicsimageio/blob/main/aicsimageio/readers/bioformats_reader.py#L33-L40
         from napari_lazy_openslide import OpenSlideStore
-        
+       
         self.path = pathlib.Path(path)
         self.store = OpenSlideStore(str(self.path))
         self.zarr = zarr.open(self.store, mode='r')
         self._pixel_size = pixel_size
         pyramid = self.pyramid_from_svs()
         channel_axis = 2
         super().__init__(pyramid, channel_axis)
 
     def pyramid_from_svs(self) -> list[da.Array]:
         return [
             da.from_zarr(self.store, component=d['path'])[..., :3]
             for d in self.zarr.attrs['multiscales'][0]['datasets']
         ]
-    
+   
     @property
     def pixel_size(self):
         if self._pixel_size is not None:
             return self._pixel_size
         try:
             return float(self.store._slide.properties['openslide.mpp-x'])
         except Exception:
```

### Comparing `palom-2023.5.1/palom/register.py` & `palom-2023.5.2/palom/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 if hasattr(skimage.registration, 'phase_cross_correlation'):
     register_translation = skimage.registration.phase_cross_correlation
 else:
     register_translation = skimage.feature.register_translation
 
 
-# 
+#
 # Image-based registration
-# 
+#
 def phase_cross_correlation(img1, img2, sigma, upsample=10, module='skimage'):
     assert module in ['cv2', 'skimage']
-    
+   
     img1w = img_util.whiten(img1, sigma)
     img2w = img_util.whiten(img2, sigma)
-    
+   
     if module == 'skimage':
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 # two patterns observed
                 # 1. invalid value encountered in true_divide
                 # 2. invalid value encountered in divide
                 'ignore', 'invalid value encountered in',
@@ -40,15 +40,15 @@
             kwargs = dict(upsample_factor=upsample)
             # `normalization` kwarg was introduced in skimage v0.19
             if 'normalization' in inspect.signature(register_translation).parameters:
                 kwargs.update(normalization=None)
             shift, _error, _phasediff = register_translation(
                 img1w, img2w, **kwargs
             )
-    
+   
     elif module == 'cv2':
         shift_xy, _response = cv2.phaseCorrelate(img1w, img2w)
         shift = shift_xy[::-1]
 
     # At this point we may have a shift in the wrong quadrant since the FFT
     # assumes the signal is periodic. We test all four possibilities and return
     # the shift that gives the highest direct correlation (sum of products).
@@ -71,15 +71,15 @@
     return shift, error
 
 
 def cv2_translate(img, shift):
     assert img.ndim == len(shift) == 2
     sy, sx = shift
     return cv2.warpAffine(
-        img,    
+        img,   
         np.array([[1, 0, sx], [0, 1, sy]], dtype=float),
         img.shape[::-1]
     )
 
 
 def normalized_phase_correlation(img1, img2, sigma):
     w1 = img_util.whiten(img1, sigma)
@@ -87,27 +87,27 @@
     corr = scipy.fft.fftshift(np.abs(scipy.fft.ifft2(
         scipy.fft.fft2(w1) * scipy.fft.fft2(w2).conj()
     )))
     corr /= (np.linalg.norm(w1) * np.linalg.norm(w2))
     return corr
 
 
-# 
+#
 # Feature-based registration
-# 
+#
 def feature_based_registration(
     img_left, img_right,
     detect_flip_rotate=False,
     n_keypoints=1000, plot_match_result=False,
     plot_individual_result=False, ransacReprojThreshold=5
 ):
     flip_rotate_func, mx_fr = np.array, np.eye(3)
     if detect_flip_rotate:
         flip_rotate_func, mx_fr = match_test_flip_rotate(img_left, img_right)
-    
+   
     img_right = flip_rotate_func(img_right)
     mx_affine = ensambled_match(
         img_left, img_right,
         n_keypoints, plot_match_result,
         plot_individual_result, ransacReprojThreshold,
     )
     mx_affine = (np.vstack([mx_affine, [0, 0, 1]]) @ mx_fr)[:2, :]
@@ -176,15 +176,15 @@
         )
         for img_pair in img_pairs
     ]
     all_src = np.vstack([i[0] for i in all_found])
     all_dst = np.vstack([i[1] for i in all_found])
 
     t_matrix, mask = cv2.estimateAffine2D(
-        all_dst, all_src, 
+        all_dst, all_src,
         method=cv2.RANSAC,
         ransacReprojThreshold=ransacReprojThreshold,
         maxIters=5000
     )
     if plot_match_result == True:
         plt.figure()
         plt.gray()
@@ -227,15 +227,15 @@
     src_pts = np.float32(
         [keypoints_left[m.queryIdx].pt for m in matches]
     )
     dst_pts = np.float32(
         [keypoints_right[m.trainIdx].pt for m in matches]
     )
     t_matrix, mask = cv2.estimateAffine2D(
-        dst_pts, src_pts, 
+        dst_pts, src_pts,
         method=cv2.RANSAC, ransacReprojThreshold=30, maxIters=5000
     )
     if plot_match_result == True:
         plt.figure()
         imgmatch_ransac = cv2.drawMatches(
             img_left, keypoints_left,
             img_right, keypoints_right,
```

### Comparing `palom-2023.5.1/palom/register_util.py` & `palom-2023.5.2/palom/register_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 def match_bf_fl_histogram(img1, img2):
     img1 = img1.astype(np.float32)
     img2 = img2.astype(np.float32)
     # TODO does it make a difference to min/max rescale before histogram
     # matching?
     is_bf_img1, is_bf_img2 = [
-        img_util.is_brightfield_img(i) 
+        img_util.is_brightfield_img(i)
         for i in (img1, img2)
     ]
     if is_bf_img1 == is_bf_img2:
         return img1, skimage.exposure.match_histograms(img2, img1)
     elif is_bf_img1:
         return img1, skimage.exposure.match_histograms(-img2, img1)
     elif is_bf_img2:
@@ -57,15 +57,15 @@
     fig, axs = plt.subplots(1, len(imgs))
     for i, k, a in zip(imgs, keypoints, axs):
         a.imshow(cv2.drawKeypoints(
             i, k, None,
             flags=cv2.DRAW_MATCHES_FLAGS_DEFAULT
         ))
         a.set_title(len(k))
-    return 
+    return
 
 
 def get_flip_mx(img_shape, flip_axis):
     assert flip_axis in [0, 1, (0, 1), (1, 0)]
     mx = np.eye(3)
     offset_xy = np.array(img_shape)[::-1] - 1
     if type(flip_axis) == int:
```

### Comparing `palom-2023.5.1/pyproject.toml` & `palom-2023.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "palom"
-version = "2023.5.1"
+version = "2023.5.2"
 description = "Piecewise alignment for layers of mosaics"
 authors = ["Yu-An Chen <atwood12@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/palom/"
 repository = "https://github.com/Yu-AnChen/palom"
 keywords = [
     "microscopy",
```

### Comparing `palom-2023.5.1/PKG-INFO` & `palom-2023.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palom
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Piecewise alignment for layers of mosaics
 Home-page: https://pypi.org/project/palom/
 Keywords: microscopy,multiplex imaging,image registration,digital pathology,atlas
 Author: Yu-An Chen
 Author-email: atwood12@gmail.com
 Requires-Python: >=3.7.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
@@ -143,15 +143,15 @@
 
 Running the following command to generate the configuration file
 
 ```bash
 palom-svs-helper -i "Y:\DATA\SARDANA\MIHC\768473\RAW" -n "*Hem*" -o "Y:\DATA\SARDANA\MIHC\768473\RAW\palom\768473.ome.tif" -c "Y:\DATA\SARDANA\MIHC\768473\768473.yml"
 ```
 
-And the resulting `Y:\DATA\SARDANA\MIHC\768473\768473.yml` file 
+And the resulting `Y:\DATA\SARDANA\MIHC\768473\768473.yml` file
 
 ```yaml
 input dir: Y:\DATA\SARDANA\MIHC\768473\RAW
 output full path: Y:\DATA\SARDANA\MIHC\768473\RAW\palom\768473.ome.tif
 reference image:
   filename: .\KB_SARDANA_768473_C01R3_Hem.svs
   output mode: hematoxylin
@@ -180,15 +180,15 @@
 After reviewing the configuration file, process those SVS files by running
 
 ```bash
 palom-svs run -c "Y:\DATA\SARDANA\MIHC\768473\768473.yml"
 ```
 
 When the process is finished, a pyramidal OME-TIFF file will be generated along
-with PNG files showing the feature-based registration results and a log file. 
+with PNG files showing the feature-based registration results and a log file.
 
 ```
 Y:\DATA\SARDANA\MIHC\768473\RAW
 │   CBB_SARDANA_768473_C04R1_CD8.svs
 │   KB_SARDANA_768473_C01R1_PD1.svs
 │   KB_SARDANA_768473_C01R2_PDL1.svs
 │   KB_SARDANA_768473_C01R3_Hem.svs
@@ -226,15 +226,15 @@
 LEVEL = 1
 THUMBNAIL_LEVEL = 2
 
 c1rp = palom.color.PyramidHaxProcessor(c1r.pyramid, thumbnail_level=THUMBNAIL_LEVEL)
 c2rp = palom.color.PyramidHaxProcessor(c2r.pyramid, thumbnail_level=THUMBNAIL_LEVEL)
 
 c21l = palom.align.Aligner(
-    c1rp.get_processed_color(LEVEL), 
+    c1rp.get_processed_color(LEVEL),
     c2rp.get_processed_color(LEVEL),
     ref_thumbnail=c1rp.get_processed_color(THUMBNAIL_LEVEL).compute(),
     moving_thumbnail=c2rp.get_processed_color(THUMBNAIL_LEVEL).compute(),
     ref_thumbnail_down_factor=c1r.level_downsamples[THUMBNAIL_LEVEL] / c1r.level_downsamples[LEVEL],
     moving_thumbnail_down_factor=c2r.level_downsamples[THUMBNAIL_LEVEL] / c2r.level_downsamples[LEVEL]
 )
 
@@ -247,15 +247,15 @@
 c2m = palom.align.block_affine_transformed_moving_img(
     c1rp.get_processed_color(LEVEL),
     c2rp.get_processed_color(LEVEL, 'aec'),
     mxs=c21l.block_affine_matrices_da
 )
 
 palom.pyramid.write_pyramid(
-    palom.pyramid.normalize_mosaics([c2m]),
+    [c2m],
     r"Y:\DATA\SARDANA\MIHC\75684\mosaic.ome.tif",
     pixel_size=c1r.pixel_size*c1r.level_downsamples[LEVEL],
 )
 ```
 
 ### For TIFF and OME-TIFF files
 
@@ -309,19 +309,19 @@
     # select all the three channels (RGB) in moving image to transform
     moving_img=c2r.pyramid[LEVEL],
     mxs=c21l.block_affine_matrices_da
 )
 
 # write the registered images to a pyramidal ome-tiff
 palom.pyramid.write_pyramid(
-    mosaics=palom.pyramid.normalize_mosaics([
+    mosaics=[
         # select only the first three channels in referece image to be written
         # to the output ome-tiff; for writing all channels, use
         # `c1r.pyramid[LEVEL]` instead
         c1r.read_level_channels(LEVEL, [0, 1, 2]),
         c2m
-    ]),
+    ],
     output_path=r"Z:\P37_Pilot2\mosaic.ome.tif",
     pixel_size=c1r.pixel_size*c1r.level_downsamples[LEVEL]
 )
 ```
```

