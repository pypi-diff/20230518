# Comparing `tmp/motionrender-0.1.0.tar.gz` & `tmp/motionrender-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motionrender-0.1.0.tar", last modified: Thu May 18 00:59:55 2023, max compression
+gzip compressed data, was "motionrender-0.1.1.tar", last modified: Thu May 18 02:33:36 2023, max compression
```

## Comparing `motionrender-0.1.0.tar` & `motionrender-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 00:59:55.617221 motionrender-0.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34523 2023-05-18 00:59:55.000000 motionrender-0.1.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-05-18 00:59:55.617221 motionrender-0.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-05-18 00:59:55.000000 motionrender-0.1.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 00:59:55.617221 motionrender-0.1.0/motionrender/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-05-18 00:59:55.000000 motionrender-0.1.0/motionrender/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3252 2023-05-18 00:59:55.000000 motionrender-0.1.0/motionrender/plot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1760 2023-05-18 00:59:55.000000 motionrender-0.1.0/motionrender/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5978 2023-05-18 00:59:55.000000 motionrender-0.1.0/motionrender/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 00:59:55.617221 motionrender-0.1.0/motionrender.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-05-18 00:59:55.000000 motionrender-0.1.0/motionrender.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-05-18 00:59:55.000000 motionrender-0.1.0/motionrender.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-18 00:59:55.000000 motionrender-0.1.0/motionrender.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-18 00:59:55.000000 motionrender-0.1.0/motionrender.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-18 00:59:55.617221 motionrender-0.1.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-05-18 00:59:55.000000 motionrender-0.1.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 02:33:36.316563 motionrender-0.1.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34523 2023-05-18 02:33:35.000000 motionrender-0.1.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-05-18 02:33:36.316563 motionrender-0.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-05-18 02:33:35.000000 motionrender-0.1.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 02:33:36.316563 motionrender-0.1.1/motionrender/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-05-18 02:33:35.000000 motionrender-0.1.1/motionrender/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3278 2023-05-18 02:33:35.000000 motionrender-0.1.1/motionrender/plot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1759 2023-05-18 02:33:35.000000 motionrender-0.1.1/motionrender/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5978 2023-05-18 02:33:35.000000 motionrender-0.1.1/motionrender/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 02:33:36.316563 motionrender-0.1.1/motionrender.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-05-18 02:33:36.000000 motionrender-0.1.1/motionrender.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      260 2023-05-18 02:33:36.000000 motionrender-0.1.1/motionrender.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-18 02:33:36.000000 motionrender-0.1.1/motionrender.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-18 02:33:36.000000 motionrender-0.1.1/motionrender.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-18 02:33:36.316563 motionrender-0.1.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-05-18 02:33:35.000000 motionrender-0.1.1/setup.py
```

### Comparing `motionrender-0.1.0/LICENSE` & `motionrender-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `motionrender-0.1.0/PKG-INFO` & `motionrender-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionrender
-Version: 0.1.0
+Version: 0.1.1
 Summary: A motion tracking 3D movier render
 Author: Derek Harter
 Author-email: Derek.Harter@tamuc.edu
 License: GPL-3
 Keywords: motion tracking,3D rendering
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `motionrender-0.1.0/README.md` & `motionrender-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `motionrender-0.1.0/motionrender/plot.py` & `motionrender-0.1.1/motionrender/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,9 +82,10 @@
     -------
     fig - This function creates and returns a matplotlib figure object
        that can be displayed or saved as a single frame image.
     """
     fig = plt.figure(figsize=figsize)
     ax = fig.add_subplot(projection="3d")
     _ = create_joint_frame(ax, joints, joint_graph, joint_names)
+    ax.view_init(-90, 90)
     return fig
```

### Comparing `motionrender-0.1.0/motionrender/render.py` & `motionrender-0.1.1/motionrender/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     ax.set_zlim3d([100, 200])
     ax.view_init(-90, 90)
 
     # create animation object
     # TODO: probably need to set/calculate interval as well not hardcode
     ani = animation.FuncAnimation(
         fig, update_elements, num_frames,
-        fargs=(time_df, ax, joint_graph, joint_names), interval=100)
+        fargs=(time_df, ax, joint_graph, joint_names), interval=50)
 
     return ani
```

### Comparing `motionrender-0.1.0/motionrender/util.py` & `motionrender-0.1.1/motionrender/util.py`

 * *Files identical despite different names*

### Comparing `motionrender-0.1.0/motionrender.egg-info/PKG-INFO` & `motionrender-0.1.1/motionrender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionrender
-Version: 0.1.0
+Version: 0.1.1
 Summary: A motion tracking 3D movier render
 Author: Derek Harter
 Author-email: Derek.Harter@tamuc.edu
 License: GPL-3
 Keywords: motion tracking,3D rendering
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `motionrender-0.1.0/setup.py` & `motionrender-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'A motion tracking 3D movier render'
 LONG_DESCRIPTION = 'A package that renders movies from 3D motion tracked data, for example from 3D skeleton joint tracking data'
 
 setup(
     name="motionrender",
     version=VERSION,
     description=DESCRIPTION,
```

