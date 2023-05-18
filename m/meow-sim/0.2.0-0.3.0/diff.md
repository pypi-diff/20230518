# Comparing `tmp/meow-sim-0.2.0.tar.gz` & `tmp/meow-sim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.2.0.tar", last modified: Mon Apr 24 18:58:49 2023, max compression
+gzip compressed data, was "meow-sim-0.3.0.tar", last modified: Thu May 18 03:59:08 2023, max compression
```

## Comparing `meow-sim-0.2.0.tar` & `meow-sim-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.508033 meow-sim-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-04-24 18:58:44.000000 meow-sim-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3105 2023-04-24 18:58:49.508033 meow-sim-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2007 2023-04-24 18:58:44.000000 meow-sim-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.496033 meow-sim-0.2.0/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.496033 meow-sim-0.2.0/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8007 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.500033 meow-sim-0.2.0/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4608 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.500033 meow-sim-0.2.0/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3440 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)     9206 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10776 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3564 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)     9797 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     2677 2023-04-24 18:58:44.000000 meow-sim-0.2.0/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.504033 meow-sim-0.2.0/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3105 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      657 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      349 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-24 18:58:49.000000 meow-sim-0.2.0/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1832 2023-04-24 18:58:44.000000 meow-sim-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 18:58:49.508033 meow-sim-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:58:49.508033 meow-sim-0.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4008 2023-04-24 18:58:44.000000 meow-sim-0.2.0/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-04-24 18:58:44.000000 meow-sim-0.2.0/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:59:08.835261 meow-sim-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-05-18 03:59:04.000000 meow-sim-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-05-18 03:59:08.835261 meow-sim-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-18 03:59:04.000000 meow-sim-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:59:08.827261 meow-sim-0.3.0/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:59:08.827261 meow-sim-0.3.0/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8007 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:59:08.827261 meow-sim-0.3.0/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4608 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:59:08.831261 meow-sim-0.3.0/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3440 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10785 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     9814 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-05-18 03:59:04.000000 meow-sim-0.3.0/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:59:08.831261 meow-sim-0.3.0/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-05-18 03:59:08.000000 meow-sim-0.3.0/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-18 03:59:08.000000 meow-sim-0.3.0/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 03:59:08.000000 meow-sim-0.3.0/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-18 03:59:08.000000 meow-sim-0.3.0/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-18 03:59:08.000000 meow-sim-0.3.0/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-18 03:59:04.000000 meow-sim-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 03:59:08.835261 meow-sim-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 03:59:08.831261 meow-sim-0.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4009 2023-05-18 03:59:04.000000 meow-sim-0.3.0/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-05-18 03:59:04.000000 meow-sim-0.3.0/tests/test_nbs.py
```

### Comparing `meow-sim-0.2.0/LICENSE` & `meow-sim-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/PKG-INFO` & `meow-sim-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: min
+Provides-Extra: vis
 Provides-Extra: jax
 Provides-Extra: klu
 Provides-Extra: ipy
 Provides-Extra: gds
 Provides-Extra: dev
 Provides-Extra: full
 License-File: LICENSE
@@ -52,14 +53,15 @@
 You can select which features to enable during installation as follows:
 ```sh
 pip install meow-sim[feature1,feature2,...]
 ```
 
 #### Available features
 * `min`: minimal installation (equivalent to not specifying any features)
+* `vis`: explicitly installs matplotlib and trimesh.
 * `jax`: use JAX in stead of numpy to calculate the S-matrices
 * `klu`: use `klujax` to speed up S-matric calculations (implies `jax`). Note: you need
 the SuiteSparse headers on your computer for this to work.
 * `gds`: enable GDS creation with GDSFactory (see GDS Taper example).
 * `ipy`: install useful jupyter/ipython packages.
 * `dev`: install dev dependencies
 * `full`: enable all the above features.
```

### Comparing `meow-sim-0.2.0/README.md` & `meow-sim-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 You can select which features to enable during installation as follows:
 ```sh
 pip install meow-sim[feature1,feature2,...]
 ```
 
 #### Available features
 * `min`: minimal installation (equivalent to not specifying any features)
+* `vis`: explicitly installs matplotlib and trimesh.
 * `jax`: use JAX in stead of numpy to calculate the S-matrices
 * `klu`: use `klujax` to speed up S-matric calculations (implies `jax`). Note: you need
 the SuiteSparse headers on your computer for this to work.
 * `gds`: enable GDS creation with GDSFactory (see GDS Taper example).
 * `ipy`: install useful jupyter/ipython packages.
 * `dev`: install dev dependencies
 * `full`: enable all the above features.
```

### Comparing `meow-sim-0.2.0/meow/__init__.py` & `meow-sim-0.3.0/meow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.2.0/meow/assets/silicon.csv` & `meow-sim-0.3.0/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/assets/silicon_oxide.csv` & `meow-sim-0.3.0/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/base_model.py` & `meow-sim-0.3.0/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/cache.py` & `meow-sim-0.3.0/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/cell.py` & `meow-sim-0.3.0/meow/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """ an EME Cell """
 
 from typing import Any, Dict, List, Tuple, Union
 
-import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib.colors import ListedColormap, to_rgba
 from pydantic import Field
 
 from .base_model import BaseModel
 from .mesh import Mesh2d
 from .structures import Structure, sort_structures
 
 
@@ -75,14 +73,17 @@
         return 0.5 * (self.z_min + self.z_max)
 
     @property
     def length(self):
         return np.abs(self.z_max - self.z_min)
 
     def _visualize(self, c="z", axs=None):
+        import matplotlib.pyplot as plt
+        from matplotlib.colors import ListedColormap, to_rgba
+
         colors = [(0, 0, 0, 0)] + [
             to_rgba(m.meta.get("color", (0, 0, 0, 0))) for m in self.materials
         ]
         cmap = ListedColormap(colors=colors)  # type: ignore
         if axs is None:
             _, axs = plt.subplots(1, len(c), figsize=(3 * len(c), 3))
         c_list = list(c)
```

### Comparing `meow-sim-0.2.0/meow/cross_section.py` & `meow-sim-0.3.0/meow/cross_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """ A CrossSection """
 from typing import Any, Dict
 
-import matplotlib.pyplot as plt
 import numpy as np
 from pydantic import Field
 
 from .base_model import BaseModel
 from .cell import Cell
 from .environment import Environment
 
@@ -60,14 +59,16 @@
         return self.cell.mesh
 
     @property
     def structures(self):
         return self.cell.structures
 
     def _visualize(self, c="z", axs=None):
+        import matplotlib.pyplot as plt
+
         if axs is None:
             _, axs = plt.subplots(1, len(c), figsize=(3 * len(c), 3))
         c_list = list(c)
         if any(c not in "xyz" for c in c_list):
             raise ValueError(f"Invalid component. Got: {c}. Should be 'x', 'y' or 'z'.")
         axs = np.array(axs, dtype=object).ravel()
         for ax, c in zip(axs, c_list):
```

### Comparing `meow-sim-0.2.0/meow/eme/__init__.py` & `meow-sim-0.3.0/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/eme/common.py` & `meow-sim-0.3.0/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/eme/sax.py` & `meow-sim-0.3.0/meow/eme/sax.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ SAX backend for EME (default backend) """
 from functools import partial
 from typing import List
 
-import sax
 import numpy as np
+import sax
 from sax.backends import circuit_backends
-from sax.netlist import Netlist
 from sax.circuit import _make_singlemode_or_multimode
+from sax.netlist import Netlist
 
 from ..base_model import _array
 from ..mode import Mode
 from .common import compute_interface_s_matrices, compute_propagation_s_matrices
 from .common import select_ports as select_ports
 
 try:
```

### Comparing `meow-sim-0.2.0/meow/environment.py` & `meow-sim-0.3.0/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/fde/lumerical.py` & `meow-sim-0.3.0/meow/fde/lumerical.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     """compute ``Modes` for a given ``FdeSpec` (Lumerical backend)
 
     Args:
         sim: the lumerical simulation object
         spec: The FDE simulation specification
         unit: Conversion factor between MEOW unit (probably um) and Lumerical unit (probably m).
     """
-    _assert_default_mesh_setting(cs.cell.mesh.angle_phi == 0, "angle_phi")
-    _assert_default_mesh_setting(cs.cell.mesh.angle_theta == 0, "angle_theta")
-    _assert_default_mesh_setting(cs.cell.mesh.bend_radius > 1e10, "bend_radius")
+    _assert_default_mesh_setting(cs.cell.mesh.angle_phi != 0, "angle_phi")
+    _assert_default_mesh_setting(cs.cell.mesh.angle_theta != 0, "angle_theta")
+    _assert_default_mesh_setting(cs.cell.mesh.bend_radius < 1e10, "bend_radius")
 
     if sim is None:
         sim = get_sim()
 
     assert sim is not None
 
     sim.switchtolayout()
```

### Comparing `meow-sim-0.2.0/meow/fde/tidy3d.py` & `meow-sim-0.3.0/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/gds_structures.py` & `meow-sim-0.3.0/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/geometries.py` & `meow-sim-0.3.0/meow/geometries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 """ Geometries """
 
 from secrets import token_hex
 from typing import Dict, List, Literal, Tuple, Union, cast
 
 import numpy as np
 import shapely.geometry as sg
-from matplotlib.colors import to_rgba as _to_rgba_mpl
 from pydantic import Field, validator
-from trimesh import Trimesh
-from trimesh.creation import extrude_polygon
-from trimesh.scene import Scene
-from trimesh.transformations import rotation_matrix
 
 from .base_model import BaseModel
 from .mesh import Mesh2d
 
 GEOMETRIES: Dict[str, type] = {}
 
 
@@ -22,29 +17,30 @@
     type: str = ""
 
     def __init_subclass__(cls):
         GEOMETRIES[cls.__name__] = cls
 
     def __new__(cls, **kwargs):
         cls = GEOMETRIES.get(kwargs.get("type", cls.__name__), cls)
-        return BaseModel.__new__(
-            cls
-        )  # , **kwargs) # weird pydantic black magic: kwargs are not explicitly propagated
+        return BaseModel.__new__(cls)  # type: ignore
 
     @validator("type", pre=True, always=True)
     def validate_type(cls, value):
         if not value:
             value = getattr(cls, "__name__", "Geometry")
         if value not in GEOMETRIES:
             raise ValueError(
                 f"Invalid Geometry type. Got: {value!r}. Valid types: {GEOMETRIES}."
             )
         return value
 
     def _visualize(self, scale=None):
+        from trimesh.scene import Scene
+        from trimesh.transformations import rotation_matrix
+
         scene = Scene()
         scene.add_geometry(self._trimesh(scale=scale))
         scene.apply_transform(rotation_matrix(-np.pi / 6, (0, 1, 0)))
         return scene.show()
 
     def _mask2d_single(self, X, Y, z):
         raise NotImplementedError(f"{self.__class__.__name__!r} cannot be masked.")
@@ -103,14 +99,17 @@
             material=material_name,
             override_mesh_order_from_material_database=True,
             mesh_order=mesh_order,
             **kwargs,
         )
 
     def _trimesh(self, color=None, scale=None):
+        from trimesh import Trimesh
+        from trimesh.creation import extrude_polygon
+
         sx, sy, sz = scale or (1, 1, 1)
         poly = sg.Polygon(
             [
                 (self.x_min * sx, self.y_min * sy),
                 (self.x_min * sx, self.y_max * sy),
                 (self.x_max * sx, self.y_max * sy),
                 (self.x_max * sx, self.y_min * sy),
@@ -212,14 +211,16 @@
 
         if xyz in ["yzx", "zxy"]:
             raise NotImplementedError(
                 "Only prisms extruded perpendicular to the 'chip surface' are currently supported in Lumerical."
             )
 
     def _trimesh(self, color=None, scale=None):
+        from trimesh.creation import extrude_polygon
+
         poly = sg.Polygon(self.poly)
         prism = extrude_polygon(poly, self.h_max - self.h_min)
         prism = prism.apply_translation((0, 0, self.h_min))
         if self.axis == "x":
             prism.vertices = np.roll(prism.vertices, shift=1, axis=1)  # type: ignore
         if self.axis == "y":
             prism.vertices = np.roll(prism.vertices, shift=-1, axis=1)  # type: ignore
@@ -247,10 +248,12 @@
             "x": (1, 0, 0),
             "y": (0, 1, 0),
             "z": (0, 0, 1),
         }[self.axis]
 
 
 def _to_rgba(c):
+    from matplotlib.colors import to_rgba as _to_rgba_mpl
+
     r, g, b, a = _to_rgba_mpl(c)
     a = min(max(a, 0.1), 0.9)
     return float(r), float(g), float(b), float(a)
```

### Comparing `meow-sim-0.2.0/meow/integrate.py` & `meow-sim-0.3.0/meow/integrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from scipy.interpolate import RegularGridInterpolator
 from scipy.integrate import dblquad, simpson
+from scipy.interpolate import RegularGridInterpolator
 
 
 def integrate_interpolate_2d(x, y, data, extent=None):
     """
     First the data on the given grid is interpolated and then integrated using `scipy.dblquad`.
-    This procedure is best suited if one wants to integrate over a (small) region of interest that can be placed at off-grid positions"""
+    This procedure is best suited if one wants to integrate over a (small) region of interest that can be placed at off-grid positions
+    """
     interp = RegularGridInterpolator((x, y), data)
     if extent is None:
         extent = [[min(x), max(x)], [min(y), max(y)]]
 
     def integrable(x, y):
         return interp((x, y))
```

### Comparing `meow-sim-0.2.0/meow/materials.py` & `meow-sim-0.3.0/meow/materials.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import re
 from hashlib import md5
 from typing import Any, Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
-from matplotlib.cm import get_cmap
 from numpy.typing import NDArray
 from pydantic import Field, root_validator
 from scipy.constants import c
 from scipy.ndimage import map_coordinates
 
 from .base_model import BaseModel, _array
 from .environment import Environment
@@ -116,14 +115,16 @@
         ni = result.take(pos["targets"]["ni"], axs["targets"])
         n = nr + 1j * ni
         # FIXME: ideally we should just be able to return `n` here...
         # return n
         return np.squeeze(np.real(n))  # TODO: allow complex multi-dimensional n
 
     def _lumadd(self, sim, env, unit):
+        from matplotlib.cm import get_cmap
+
         n = self(env)
         wl = np.asarray(env.wl * unit, dtype=complex).ravel()
         eps = np.asarray(n, dtype=complex).ravel() ** 2
         data = np.stack([c / wl, eps], 1)  # permittivity, not index
 
         if not sim.materialexists(self.name):
             sim.setmaterial(sim.addmaterial("Sampled data"), "name", self.name)
```

### Comparing `meow-sim-0.2.0/meow/mesh.py` & `meow-sim-0.3.0/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/meow/mode.py` & `meow-sim-0.3.0/meow/mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """ An EigenMode """
 
 import pickle
 from itertools import product
-from typing import List, Tuple, Any
+from typing import Any, List, Tuple
 
-import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib import colors
 from pydantic import Field, PrivateAttr
 from scipy.constants import epsilon_0 as eps0
 from scipy.constants import mu_0 as mu0
 from scipy.linalg import norm
-from .integrate import integrate_2d
 
 from .base_model import BaseModel
 from .cross_section import CrossSection
+from .integrate import integrate_2d
 
 
 class Mode(BaseModel):
     """A `Mode` contains the field information for a given `CrossSection`."""
 
     neff: complex = Field(description="the effective index of the mode")
     cs: CrossSection = Field(
@@ -118,14 +116,17 @@
         fields=None,
         ax=None,
         n_cmap=None,
         mode_cmap=None,
         num_levels=8,
         operation=lambda x: np.abs(x) ** 2,
     ):
+        import matplotlib.pyplot as plt
+        from matplotlib import colors
+
         if fields is None or len(fields) == 0:
             fields = ["Ex"]
 
         if len(fields) > 1:
             if ax is None:
                 _, ax = plt.subplots(len(fields), 1, figsize=(5, len(fields) * 3))
             if len(ax) < len(fields):
```

### Comparing `meow-sim-0.2.0/meow/structures.py` & `meow-sim-0.3.0/meow/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """ a Structure is a combination of a geometry with a material (and an optional mesh order) """
 
 import numpy as np
 from pydantic import Field, validator
-from trimesh.scene import Scene
-from trimesh.transformations import rotation_matrix
 
 from .base_model import BaseModel
 from .geometries import Geometry
 from .materials import Material
 
 
 class Structure(BaseModel):
@@ -33,14 +31,17 @@
 
     def _visualize(self, scale=None):
         return self._trimesh(scale=scale).show()
 
 
 def visualize_structures(structures, scale=None):
     """easily visualize a collection (list) of `Structure` objects"""
+    from trimesh.scene import Scene
+    from trimesh.transformations import rotation_matrix
+
     scene = Scene(
         geometry=[s._trimesh(scale=scale) for s in sort_structures(structures)]
     )
     scene.apply_transform(rotation_matrix(np.pi - np.pi / 6, (0, 1, 0)))
     return scene.show()
```

### Comparing `meow-sim-0.2.0/meow/visualize.py` & `meow-sim-0.3.0/meow/visualize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """ Visualizations for common meow-datatypes """
 
 from typing import Any
 
-import matplotlib.pyplot as plt
 import numpy as np
 
 try:
+    import matplotlib.pyplot as plt
+except ImportError:
+    plt = None
+
+try:
     import gdsfactory as gf
 except ImportError:
     gf = None
 
 try:
     from jaxlib.xla_extension import DeviceArray
 except ImportError:
     DeviceArray = None
 
 
 def _visualize_s_matrix(S, fmt=".3f", title=None):
+    import matplotlib.pyplot as plt
+
     Z = np.abs(S)
     y, x = np.arange(Z.shape[0])[::-1], np.arange(Z.shape[1])
     Y, X = np.meshgrid(y, x)
 
     plt.figure(figsize=(2 * x.shape[0] / 3, 2 * y.shape[0] / 3))
     plt.pcolormesh(X, Y, Z[::-1].T, cmap="Greys", vmin=0.0, vmax=2.0 * Z.max())
 
@@ -77,14 +83,15 @@
         (
             isinstance(obj, np.ndarray)
             or (DeviceArray is not None and isinstance(obj, DeviceArray))
         )
         and obj.ndim == 2
         and obj.shape[0] > 1
         and obj.shape[1] > 1
+        and plt is not None
     ):
         _visualize_s_matrix(obj, **kwargs)
     elif gf is not None and isinstance(obj, gf.Component):
         _visualize_gdsfactory(obj, **kwargs)
     else:
         try:
             (*objs,) = obj  # type: ignore
```

### Comparing `meow-sim-0.2.0/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.3.0/meow_sim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.2.0
+Version: 0.3.0
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: min
+Provides-Extra: vis
 Provides-Extra: jax
 Provides-Extra: klu
 Provides-Extra: ipy
 Provides-Extra: gds
 Provides-Extra: dev
 Provides-Extra: full
 License-File: LICENSE
@@ -52,14 +53,15 @@
 You can select which features to enable during installation as follows:
 ```sh
 pip install meow-sim[feature1,feature2,...]
 ```
 
 #### Available features
 * `min`: minimal installation (equivalent to not specifying any features)
+* `vis`: explicitly installs matplotlib and trimesh.
 * `jax`: use JAX in stead of numpy to calculate the S-matrices
 * `klu`: use `klujax` to speed up S-matric calculations (implies `jax`). Note: you need
 the SuiteSparse headers on your computer for this to work.
 * `gds`: enable GDS creation with GDSFactory (see GDS Taper example).
 * `ipy`: install useful jupyter/ipython packages.
 * `dev`: install dev dependencies
 * `full`: enable all the above features.
```

### Comparing `meow-sim-0.2.0/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.3.0/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.2.0/pyproject.toml` & `meow-sim-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
@@ -44,20 +44,21 @@
   "shapely",
   "tidy3d>=2.1",
   "trimesh[easy]",
 ]
 
 [project.optional-dependencies]
 min = ["meow-sim"]
+vis = ["matplotlib", "trimesh[easy]"]
 jax = ["jax", "jaxlib"]
 klu = ["klujax>0.1.2"]
 ipy = ["ipykernel", "ipywidgets", "ipympl", "nbstripout", "tqdm"]
 gds = ["gdsfactory>6.27.0", "klayout>0.28.2"]
 dev = ["bump2version", "nbstripout", "pre-commit", "black", "sphinx", "autodoc-pydantic", "myst-nb>0.17.1"]
-full = ["meow-sim[klu,jax,ipy,gds]"]
+full = ["meow-sim[vis,klu,jax,ipy,gds]"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["meow*"]
 exclude = []
 namespaces = true
```

### Comparing `meow-sim-0.2.0/tests/test_deserialization.py` & `meow-sim-0.3.0/tests/test_deserialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import lru_cache, wraps
 from typing import List
 
-import meow as mw
 import numpy as np
 from pydantic import Field, parse_raw_as
 
+import meow as mw
+
 
 class SimpleMode(mw.BaseModel):
     neff: complex = Field(description="the effective index of the mode")
     cs: mw.CrossSection = Field(
         description="the index cross section for which the mode was calculated"
     )
     te_fraction: float = Field(description="the TE polarization fraction of the mode.")
```

### Comparing `meow-sim-0.2.0/tests/test_nbs.py` & `meow-sim-0.3.0/tests/test_nbs.py`

 * *Files identical despite different names*

