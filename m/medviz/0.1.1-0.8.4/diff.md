# Comparing `tmp/medviz-0.1.1.tar.gz` & `tmp/medviz-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medviz-0.1.1.tar", last modified: Fri Apr 28 23:21:09 2023, max compression
+gzip compressed data, was "medviz-0.8.4.tar", last modified: Thu May 18 15:01:56 2023, max compression
```

## Comparing `medviz-0.1.1.tar` & `medviz-0.8.4.tar`

### file list

```diff
@@ -1,19 +1,44 @@
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-28 23:21:09.994586 medviz-0.1.1/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-02-17 19:26:43.000000 medviz-0.1.1/LICENSE
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       26 2023-02-17 19:26:43.000000 medviz-0.1.1/MANIFEST.in
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-04-28 23:21:09.994586 medviz-0.1.1/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-0.1.1/README.rst
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-28 23:21:09.994586 medviz-0.1.1/medviz/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       47 2023-04-28 23:06:17.000000 medviz-0.1.1/medviz/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1160 2023-04-28 23:00:59.000000 medviz-0.1.1/medviz/example.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2049 2023-04-27 15:48:58.000000 medviz-0.1.1/medviz/gif.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2022 2023-04-28 22:56:59.000000 medviz-0.1.1/medviz/layered_plot.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-04-28 23:21:09.994586 medviz-0.1.1/medviz.egg-info/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      277 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/SOURCES.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/dependency_links.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      108 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/requires.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-04-28 23:21:09.000000 medviz-0.1.1/medviz.egg-info/top_level.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1015 2023-04-28 23:20:56.000000 medviz-0.1.1/pyproject.toml
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-04-28 23:21:09.994586 medviz-0.1.1/setup.cfg
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.1.1/setup.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 15:01:56.184193 medviz-0.8.4/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-02-17 19:26:43.000000 medviz-0.8.4/LICENSE
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      149 2023-05-18 14:59:54.000000 medviz-0.8.4/MANIFEST.in
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-05-18 15:01:56.184193 medviz-0.8.4/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-0.8.4/README.rst
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        5 2023-05-18 15:01:50.000000 medviz-0.8.4/VERSION
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 15:01:56.180193 medviz-0.8.4/medviz/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      926 2023-05-18 14:56:52.000000 medviz-0.8.4/medviz/__init__.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 15:01:56.180193 medviz-0.8.4/medviz/plots/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       55 2023-05-18 02:10:54.000000 medviz-0.8.4/medviz/plots/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1552 2023-05-18 02:42:18.000000 medviz-0.8.4/medviz/plots/_plot_image.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    10511 2023-05-14 06:38:00.000000 medviz-0.8.4/medviz/plots/gif.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2273 2023-05-18 02:31:56.000000 medviz-0.8.4/medviz/plots/helper_plot.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     3702 2023-05-17 17:02:52.000000 medviz-0.8.4/medviz/plots/layered_plot2D.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 15:01:56.180193 medviz-0.8.4/medviz/plots/plot2d/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       46 2023-05-17 21:56:40.000000 medviz-0.8.4/medviz/plots/plot2d/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       86 2023-05-18 02:47:21.000000 medviz-0.8.4/medviz/plots/plot2d/image_masks.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1336 2023-05-18 02:10:51.000000 medviz-0.8.4/medviz/plots/plot2d/images.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 15:01:56.180193 medviz-0.8.4/medviz/plots/plot3d/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       46 2023-05-18 02:18:22.000000 medviz-0.8.4/medviz/plots/plot3d/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2461 2023-05-18 02:47:13.000000 medviz-0.8.4/medviz/plots/plot3d/images.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2364 2023-05-12 19:13:22.000000 medviz-0.8.4/medviz/plots/plot3d/layered_plot.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 15:01:56.184193 medviz-0.8.4/medviz/preprocess/
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       86 2023-05-14 03:50:56.000000 medviz-0.8.4/medviz/preprocess/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1656 2023-05-14 03:51:57.000000 medviz-0.8.4/medviz/preprocess/mask.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1658 2023-05-14 04:20:25.000000 medviz-0.8.4/medviz/preprocess/match_image_mask.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 15:01:56.184193 medviz-0.8.4/medviz/utils/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      476 2023-05-18 03:12:21.000000 medviz-0.8.4/medviz/utils/__init__.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2175 2023-05-13 17:59:38.000000 medviz-0.8.4/medviz/utils/array_profile.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      662 2023-05-13 18:05:32.000000 medviz-0.8.4/medviz/utils/array_threshold.py
+-rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)      120 2023-01-02 16:26:25.000000 medviz-0.8.4/medviz/utils/custom_type.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4587 2023-05-14 03:54:29.000000 medviz-0.8.4/medviz/utils/helper_mask.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      689 2023-01-02 16:26:25.000000 medviz-0.8.4/medviz/utils/log.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      940 2023-04-02 15:43:58.000000 medviz-0.8.4/medviz/utils/reader.py
+-rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)       80 2023-05-17 19:24:17.000000 medviz-0.8.4/medviz/utils/utility.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 15:01:56.180193 medviz-0.8.4/medviz.egg-info/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-05-18 15:01:56.000000 medviz-0.8.4/medviz.egg-info/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      861 2023-05-18 15:01:56.000000 medviz-0.8.4/medviz.egg-info/SOURCES.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-05-18 15:01:56.000000 medviz-0.8.4/medviz.egg-info/dependency_links.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      145 2023-05-18 15:01:56.000000 medviz-0.8.4/medviz.egg-info/requires.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-05-18 15:01:56.000000 medviz-0.8.4/medviz.egg-info/top_level.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1247 2023-05-18 14:57:24.000000 medviz-0.8.4/pyproject.toml
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-05-18 15:01:56.184193 medviz-0.8.4/setup.cfg
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.8.4/setup.py
```

### Comparing `medviz-0.1.1/LICENSE` & `medviz-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medviz-0.1.1/PKG-INFO` & `medviz-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.1.1
+Version: 0.8.4
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-0.1.1/README.rst` & `medviz-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `medviz-0.1.1/medviz/gif.py` & `medviz-0.8.4/medviz/plots/plot3d/layered_plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,97 @@
-# DocString: Create a gif from a 3D image and multiple 3D masks
-"""
-Create a gif from a 3D image and multiple 3D masks
-
-Parameters
-----------
-image_path : str
-    Path to the 3D image
-mask_paths : list
-    List of paths to the 3D masks
-mask_colors : list  
-    List of colors for each mask
-interval : int, optional    
-    Interval between frames in milliseconds (default is 100)
-start_slice : int, optional
-    Starting slice (default is 0)
-end_slice : int, optional
-    Ending slice (default is None)
-title : str, optional
-    Title of the gif (default is "Layered Plot")
-save_path : str, optional
-    Path to save the gif (default is "animation.gif")
-
-Returns
--------
-None
-
-"""
+from pathlib import Path
 
 import matplotlib.pyplot as plt
-import matplotlib.animation as animation
-import nibabel as nib
+from matplotlib.widgets import Slider
 
+import medviz as viz
 
-def gif(
-    image_path,
-    mask_paths,
-    mask_colors,
-    interval=100,
-    start_slice=0,
-    end_slice=None,
-    title="Layered Plot",
-    save_path="animation.gif",
-):
-    img = nib.load(image_path)
-    data = img.get_fdata()
+assert_shape = viz.assert_shape
 
-    mask_imgs = []
-    for mask_path in mask_paths:
-        mask_imgs.append(nib.load(mask_path))
+image_path_to_data = viz.image_path_to_data_ax
+mask_path_to_data = viz.mask_path_to_data_ax
+
+generate_mask_colors = viz.generate_mask_colors
+plot_image = viz.plot_image
+plot_contour = viz.plot_contour
+
+
+def layered_plot_path3D(
+    image_path, mask_paths, mask_colors=None, title="Layered Plot", save_path=None
+):
+    image_data = image_path_to_data(image_path)
 
     masks_data = []
-    for mask_img in mask_imgs:
-        masks_data.append(mask_img.get_fdata())
+    for mask_path in mask_paths:
+        mask_data = mask_path_to_data(mask_path)
+        masks_data.append(mask_data)
 
-    fig = plt.figure()
+    layered_plot_data3D(
+        image_data,
+        masks_data,
+        mask_colors=mask_colors,
+        title=title,
+        save_path=save_path,
+    )
 
-    end_slice = data.shape[2] if end_slice is None else end_slice
 
-    slice_range = range(start_slice, data.shape[2])
+def layered_plot_data3D(
+    image_data, masks_data, mask_colors=None, title="Layered Plot", save_path=None
+):
+    print("Loading images...")
 
-    # Define the update function for the animation
+    num_masks = len(masks_data)
 
-    def update_slice(frame):
-        global current_slice
+    init_slice, last_slice = assert_shape(image_data + masks_data)
 
-        current_slice = frame
+    mask_colors = generate_mask_colors(num_masks, mask_colors)
 
-        plt.clf()
+    _, ax = plt.subplots()
+    plt.subplots_adjust(bottom=0.25)
 
-        plt.imshow(data[:, :, current_slice].T, cmap="gray")
+    plot_image(ax, image_data[:, :, init_slice], cmap="gray")
 
-        for i in range(len(masks_data)):
-            plt.contour(
-                masks_data[i][:, :, current_slice].T,
-                colors=mask_colors[i],
-                levels=[0.5],
-            )
+    for i in range(num_masks):
+        plot_contour(
+            ax, masks_data[i][:, :, init_slice], color=mask_colors[i], levels=[0.5]
+        )
 
-        plt.title(f"{title} Slice {current_slice}")
-        plt.xlabel("X")
+    ax.set_xlabel(f"Slice Number: {init_slice}")
+    ax.set_title(title)
 
-        plt.axis("off")
+    slider_ax = plt.axes([0.2, 0.1, 0.6, 0.03])
 
-    ani = animation.FuncAnimation(
-        fig, update_slice, frames=slice_range, interval=interval
+    slider = Slider(
+        slider_ax,
+        "Slice",
+        0,
+        last_slice,
+        valinit=init_slice,
+        valstep=1,
     )
 
-    ani.save(save_path, writer="pillow")
+    def update(val):
+        slice_num = int(slider.val)
+        ax.clear()
+
+        plot_image(ax, image_data[:, :, slice_num], cmap="gray")
+        for i in range(num_masks):
+            plot_contour(ax, masks_data[i][:, :, slice_num], color=mask_colors[i])
+
+        ax.set_xlabel(f"Slice Number: {slice_num}")
+        ax.set_title(title)
+
+    slider.on_changed(update)
 
     plt.show()
+
+    if save_path:
+        if isinstance(save_path, str):
+            save_path = Path(save_path)
+
+        if save_path.suffix != ".png":
+            save_path = save_path.with_suffix(".png")
+
+        if not save_path.parent.exists():
+            save_path.parent.mkdir(parents=True)
+
+        plt.savefig(save_path)
```

### Comparing `medviz-0.1.1/medviz/layered_plot.py` & `medviz-0.8.4/medviz/plots/helper_plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-## Docstring: Layered plot of CT image and mask
-"""
+import secrets
+from pathlib import Path
 
-    Args:
-        image_path (str): Path to CT image
-        mask_paths (list): List of paths to masks
-        mask_colors (list): List of colors for masks
-        title (str): Title of plot
-
-    Returns:
-        None
-
-    Examples:
-        >>> import medviz
-        >>> medviz.layered_plot("data/ct.nii.gz", ["data/lung_mask.nii.gz", "data/heart_mask.nii.gz"], ["red", "yellow"], "Layered Plot")
-
-"""
-import numpy as np
-import nibabel as nib
-import matplotlib.pyplot as plt
-from matplotlib.widgets import Slider
-
-
-def layered_plot(image_path, mask_paths, mask_colors, title="Layered Plot"):
-    print("Loading images...")
-
-    ct_img = nib.load(image_path)
-    ct_data = ct_img.get_fdata()
-    ct_data = np.flip(np.rot90(ct_data, axes=(1, 0)), axis=1)
-
-    mask_datas = []
-    for mask_path in mask_paths:
-        mask_data = nib.load(mask_path)
-        mask_data = np.flip(np.rot90(mask_data.get_fdata(), axes=(1, 0)), axis=1)
-        mask_datas.append(mask_data)
-
-    _, ax = plt.subplots()
-    plt.subplots_adjust(bottom=0.25)
-    ax.imshow(ct_data[:, :, ct_data.shape[2] // 2], cmap="gray")
-
-    for i in range(len(mask_datas)):
-        ax.contour(
-            mask_datas[i][:, :, mask_datas[i].shape[2] // 2],
-            colors=mask_colors[i],
-            levels=[0.5],
-        )
 
-    ax.set_xlabel("Slice Number")
+def assert_shape(arr: list) -> tuple:
+    """
+    Asserts that all segments have the same shape as the image
+    :param arr: list of np arrays
+    :return: tuple of the middle slice and the last slice
+    usage:
+        init_slice, last_slice = assert_shape(ct_data + masks_data)
+    """
+    # arr[0] is the image
+    # arr[1:] are the segments
+    # m,n,d are the dimensions of the image
+    n, m, d = arr[0].shape
+    try:
+        for np_array in arr:
+            assert np_array.shape == (m, n, d)
+    except AssertionError:
+        raise ValueError("All segments must have the same shape as the image")
+
+    return d // 2, d - 1
+
+
+def generate_mask_colors(num_masks, mask_colors=None):
+    if mask_colors is None:
+        mask_colors = ["#" + secrets.token_hex(3) for _ in range(num_masks)]
+
+        return mask_colors
+    else:
+        try:
+            assert num_masks == len(mask_colors)
+            return mask_colors
+        except AssertionError:
+            raise ValueError(
+                f"Number of masks ({num_masks}) does not match number of colors ({len(mask_colors)})"
+            )
+
+
+def plot_image(ax, image_data, cmap="gray"):
+    ax.imshow(image_data, cmap=cmap)
+
+
+def plot_image_imshow(ax, arr, cmap="gray", origin="lower", title="", RGB=False):
+    # ax.imshow(arr, cmap=cmap, origin=origin)
+    ax.imshow(arr, cmap=cmap)
+
     ax.set_title(title)
 
-    slider_ax = plt.axes([0.2, 0.1, 0.6, 0.03])
 
-    slider = Slider(
-        slider_ax,
-        "Slice",
-        0,
-        ct_data.shape[2] - 1,
-        valinit=ct_data.shape[2] // 2,
-        valstep=1,
-    )
-
-    def update(val):
-        slice_num = int(slider.val)
-        ax.clear()
-        ax.imshow(ct_data[:, :, slice_num], cmap="gray")
-        for i in range(len(mask_datas)):
-            ax.contour(
-                mask_datas[i][:, :, slice_num], colors=mask_colors[i], levels=[0.5]
-            )
+def plot_mask_neighbor(ax, mask_data, cmap="jet", alpha=0.3):
+    # ax.imshow(mask_data, cmap=cmap, alpha=alpha, interpolation="bilinear", vmin=0, vmax=1)
+    ax.imshow(mask_data, cmap=cmap, alpha=alpha)
+
+
+# def plot_contour(ax, mask_data, color, line_width=0.5,levels=[0.5]):
+#     ax.contour(mask_data, colors=color, linewidths=line_width,levels=levels)
+# ax.contour(mask_data, colors=color, linewidths=line_width, levels=[0.5], alpha=0.5)
+
+
+def plot_contour(ax, mask_data, color, levels=[0.5]):
+    ax.contour(mask_data, colors=color, levels=levels)
+
+
+def save_image(plt, save_path):
+    if isinstance(save_path, str):
+        save_path = Path(save_path)
 
-        ax.set_xlabel("Slice Number")
-        ax.set_title(title)
+    if save_path.suffix != ".png":
+        save_path = save_path.with_suffix(".png")
 
-    slider.on_changed(update)
+    if not save_path.parent.exists():
+        save_path.parent.mkdir(parents=True)
 
-    plt.show()
+    plt.savefig(save_path)
```

### Comparing `medviz-0.1.1/medviz.egg-info/PKG-INFO` & `medviz-0.8.4/medviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.1.1
+Version: 0.8.4
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

