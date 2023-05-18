# Comparing `tmp/h5parm-1.0.2.tar.gz` & `tmp/h5parm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5parm-1.0.2.tar", last modified: Thu May 18 09:05:27 2023, max compression
+gzip compressed data, was "h5parm-1.0.3.tar", last modified: Thu May 18 12:01:34 2023, max compression
```

## Comparing `h5parm-1.0.2.tar` & `h5parm-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 09:05:27.057930 h5parm-1.0.2/
--rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.2/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 09:05:27.057930 h5parm-1.0.2/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.2/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 09:05:27.057930 h5parm-1.0.2/h5parm/
--rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 09:05:27.057930 h5parm-1.0.2/h5parm/arrays/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/arrays/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.2/h5parm/arrays/dsa2000.W.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/arrays/gmrtPos.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/arrays/lofar.antenna.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/arrays/lofar.hba.antenna.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)    33202 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/datapack.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/maintenance.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15652 2023-05-18 09:03:26.000000 h5parm-1.0.2/h5parm/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 09:05:27.057930 h5parm-1.0.2/h5parm.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 09:05:27.000000 h5parm-1.0.2/h5parm.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      396 2023-05-18 09:05:27.000000 h5parm-1.0.2/h5parm.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-05-18 09:05:27.000000 h5parm-1.0.2/h5parm.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-05-18 09:05:27.000000 h5parm-1.0.2/h5parm.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-05-18 09:05:27.057930 h5parm-1.0.2/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-05-18 09:04:18.000000 h5parm-1.0.2/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:01:34.339587 h5parm-1.0.3/
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.3/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 12:01:34.339587 h5parm-1.0.3/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.3/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:01:34.335586 h5parm-1.0.3/h5parm/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:01:34.339587 h5parm-1.0.3/h5parm/arrays/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/arrays/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.3/h5parm/arrays/dsa2000.W.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/arrays/gmrtPos.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/arrays/lofar.antenna.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/arrays/lofar.hba.antenna.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)    33542 2023-05-18 11:59:57.000000 h5parm-1.0.3/h5parm/datapack.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.3/h5parm/maintenance.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15652 2023-05-18 09:03:26.000000 h5parm-1.0.3/h5parm/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 12:01:34.335586 h5parm-1.0.3/h5parm.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 12:01:34.000000 h5parm-1.0.3/h5parm.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      396 2023-05-18 12:01:34.000000 h5parm-1.0.3/h5parm.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-05-18 12:01:34.000000 h5parm-1.0.3/h5parm.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-05-18 12:01:34.000000 h5parm-1.0.3/h5parm.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-05-18 12:01:34.339587 h5parm-1.0.3/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-05-18 12:01:23.000000 h5parm-1.0.3/setup.py
```

### Comparing `h5parm-1.0.2/LICENSE` & `h5parm-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.2/PKG-INFO` & `h5parm-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 1.0.2
+Version: 1.0.3
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `h5parm-1.0.2/README.md` & `h5parm-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.2/h5parm/arrays/dsa2000.W.cfg` & `h5parm-1.0.3/h5parm/arrays/dsa2000.W.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.2/h5parm/arrays/gmrtPos.cfg` & `h5parm-1.0.3/h5parm/arrays/gmrtPos.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.2/h5parm/arrays/lofar.antenna.cfg` & `h5parm-1.0.3/h5parm/arrays/lofar.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.2/h5parm/arrays/lofar.hba.antenna.cfg` & `h5parm-1.0.3/h5parm/arrays/lofar.hba.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.2/h5parm/datapack.py` & `h5parm-1.0.3/h5parm/datapack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,54 @@
-import tables as tb
+import itertools
+import logging
 import os
-import numpy as np
-import astropy.units as au
-import astropy.time as at
-import astropy.coordinates as ac
+import re
 import sys
 import time
-import itertools
-import re
-import logging
+from typing import List
+
+import astropy.coordinates as ac
+import astropy.time as at
+import astropy.units as au
+import numpy as np
+import tables as tb
 
 logger = logging.getLogger(__name__)
 
 from h5parm.maintenance import deprecated
 
 
-def _load_array_file(array_file):
+def load_array_file(array_file):
     '''Loads a csv where each row is x,y,z in geocentric ITRS coords of the antennas'''
 
     types = np.dtype({'names': ['station', 'X_ITRS', 'Y_ITRS', 'Z_ITRS'],
                       'formats': ['S16', np.double, np.double, np.double, np.double]})
     d = np.genfromtxt(array_file, comments='#', delimiter=',', dtype=types)
-    labels = np.array(d['station'].astype(str))
+    labels = d['station'].astype(np.str_)
     locs = ac.SkyCoord(x=d['X_ITRS'] * au.m, y=d['Y_ITRS'] * au.m, z=d['Z_ITRS'] * au.m, frame='itrs')
     Nantenna = int(np.size(d['X_ITRS']))
     diameters = None
-    return np.array(labels).astype(np.str_), locs.cartesian.xyz.to(au.m).value.transpose()
+    return labels, locs.cartesian.xyz.to(au.m).value.transpose()
+
+
+def save_array_file(array_file, antennas: ac.ITRS, labels: List[bytes] | None = None):
+    antennas = antennas.cartesian.xyz.to(au.m).value.T
+    Na = len(labels)
+    with open(array_file, 'w') as f:
+        f.write('# Created on {0} by Joshua G. Albert\n'.format(time.strftime("%a %c", time.localtime())))
+        f.write('#ITRS(m)\n')
+        f.write('#station\tX\tY\tZ\n')
+        i = 0
+        while i < Na:
+            f.write(
+                '{3},{0:1.9e},{1:1.9e},{2:1.9e}'.format(antennas[i, 0], antennas[i, 1], antennas[i, 2],
+                                                        labels[i].decode()))
+            if i < Na - 1:
+                f.write('\n')
+            i += 1
 
 
 def update_h5parm(old_h5parm, new_h5parm):
     """
     Clones an old H5parm typically created with LoSoTO, that only has readonly access.
 
     :param old_h5parm:
@@ -212,15 +231,15 @@
             self.current_solset = solset
             return
         with self:
             self._H.create_group(self._H.root, solset, title='Solset: {}'.format(solset))
             self.current_solset = solset
             self.add_antenna_table()
             if antennas is None:
-                antenna_labels, antennas = _load_array_file(self.lofar_array_hba if array_file is None else array_file)
+                antenna_labels, antennas = load_array_file(self.lofar_array_hba if array_file is None else array_file)
             self.set_antennas(antenna_labels, antennas)
             self.add_directions_table()
             if directions is not None:
                 self.set_directions(patch_names, directions)
             logger.info("Created solset {}.".format(solset))
 
     def add_soltab(self, soltab, values=None, weights=None, weightDtype='f16', **axes):
@@ -342,32 +361,23 @@
             direction_table = solset_group._v_leaves['source']
             direction_table.remove_rows(0)
             direction_table.append(list(zip(patch_names, directions)))
             logger.info("Set the direction table.")
 
     def save_array_file(self, array_file):
         with self:
-            ants = self._solset.getAnt()
+            ants = self.antennas
             labels = []
             locs = []
-            for label, pos in ants.items():
+            for label, pos in zip(*ants):
                 labels.append(label)
                 locs.append(pos)
-            Na = len(labels)
-        with open(array_file, 'w') as f:
-            f.write('# Created on {0} by Joshua G. Albert\n'.format(time.strftime("%a %c", time.localtime())))
-            f.write('# ITRS(m)\n')
-            f.write('# X\tY\tZ\tlabels\n')
-            i = 0
-            while i < Na:
-                f.write(
-                    '{0:1.9e}\t{1:1.9e}\t{2:1.9e}\t{4}'.format(locs[i][0], locs[i][1], locs[i][2], labels[i]))
-                if i < Na - 1:
-                    f.write('\n')
-                i += 1
+        locs = np.asarray(locs)
+        antennas = ac.ITRS(x=locs[:, 0] * au.m, y=locs[:, 1] * au.m, z=locs[:, 2] * au.m)
+        save_array_file(array_file, antennas=antennas, labels=labels)
 
     @property
     def antennas(self):
         with self:
             if self.current_solset is None:
                 raise ValueError("Current solset is None.")
             solset_group = self._H.root._v_groups[self.current_solset]
@@ -762,12 +772,12 @@
         times are stored as mjs
         """
         times = at.Time(times / 86400., format='mjd')
         return times.isot, times
 
     def get_freqs(self, freqs):
         labs = ['{:.1f}MHz'.format(f / 1e6) for f in freqs]
-        return np.array(labs), freqs*au.Hz
+        return np.array(labs), freqs * au.Hz
 
     def get_pols(self, pols):
         with self:
             return pols, np.arange(len(pols), dtype=np.int32)
```

### Comparing `h5parm-1.0.2/h5parm/maintenance.py` & `h5parm-1.0.3/h5parm/maintenance.py`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.2/h5parm/utils.py` & `h5parm-1.0.3/h5parm/utils.py`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.2/h5parm.egg-info/PKG-INFO` & `h5parm-1.0.3/h5parm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 1.0.2
+Version: 1.0.3
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `h5parm-1.0.2/setup.py` & `h5parm-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                   'tables>=' + __minimum_tables_version__,
                   'astropy>=' + __minimum_astropy_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='h5parm',
-      version='1.0.2',
+      version='1.0.3',
       description='H5Parm data pack interface',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/h5parm",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

