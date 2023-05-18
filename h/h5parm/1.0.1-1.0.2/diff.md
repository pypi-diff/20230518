# Comparing `tmp/h5parm-1.0.1.tar.gz` & `tmp/h5parm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5parm-1.0.1.tar", last modified: Fri May 12 10:29:49 2023, max compression
+gzip compressed data, was "h5parm-1.0.2.tar", last modified: Thu May 18 09:05:27 2023, max compression
```

## Comparing `h5parm-1.0.1.tar` & `h5parm-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-12 10:29:49.916323 h5parm-1.0.1/
--rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.1/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-12 10:29:49.916323 h5parm-1.0.1/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.1/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-12 10:29:49.912323 h5parm-1.0.1/h5parm/
--rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.1/h5parm/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-12 10:29:49.916323 h5parm-1.0.1/h5parm/arrays/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.1/h5parm/arrays/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.1/h5parm/arrays/dsa2000.W.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.1/h5parm/arrays/gmrtPos.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.1/h5parm/arrays/lofar.antenna.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.1/h5parm/arrays/lofar.hba.antenna.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)    33202 2021-06-02 01:08:45.000000 h5parm-1.0.1/h5parm/datapack.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.1/h5parm/maintenance.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    13395 2023-05-12 10:28:26.000000 h5parm-1.0.1/h5parm/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-12 10:29:49.912323 h5parm-1.0.1/h5parm.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-12 10:29:49.000000 h5parm-1.0.1/h5parm.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      396 2023-05-12 10:29:49.000000 h5parm-1.0.1/h5parm.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-05-12 10:29:49.000000 h5parm-1.0.1/h5parm.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-05-12 10:29:49.000000 h5parm-1.0.1/h5parm.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-05-12 10:29:49.916323 h5parm-1.0.1/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-05-12 10:29:40.000000 h5parm-1.0.1/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 09:05:27.057930 h5parm-1.0.2/
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.2/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 09:05:27.057930 h5parm-1.0.2/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.2/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 09:05:27.057930 h5parm-1.0.2/h5parm/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 09:05:27.057930 h5parm-1.0.2/h5parm/arrays/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/arrays/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.2/h5parm/arrays/dsa2000.W.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/arrays/gmrtPos.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/arrays/lofar.antenna.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/arrays/lofar.hba.antenna.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)    33202 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/datapack.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.2/h5parm/maintenance.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15652 2023-05-18 09:03:26.000000 h5parm-1.0.2/h5parm/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-18 09:05:27.057930 h5parm-1.0.2/h5parm.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-18 09:05:27.000000 h5parm-1.0.2/h5parm.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      396 2023-05-18 09:05:27.000000 h5parm-1.0.2/h5parm.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-05-18 09:05:27.000000 h5parm-1.0.2/h5parm.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-05-18 09:05:27.000000 h5parm-1.0.2/h5parm.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-05-18 09:05:27.057930 h5parm-1.0.2/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-05-18 09:04:18.000000 h5parm-1.0.2/setup.py
```

### Comparing `h5parm-1.0.1/LICENSE` & `h5parm-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.1/PKG-INFO` & `h5parm-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 1.0.1
+Version: 1.0.2
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `h5parm-1.0.1/README.md` & `h5parm-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.1/h5parm/arrays/dsa2000.W.cfg` & `h5parm-1.0.2/h5parm/arrays/dsa2000.W.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.1/h5parm/arrays/gmrtPos.cfg` & `h5parm-1.0.2/h5parm/arrays/gmrtPos.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.1/h5parm/arrays/lofar.antenna.cfg` & `h5parm-1.0.2/h5parm/arrays/lofar.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.1/h5parm/arrays/lofar.hba.antenna.cfg` & `h5parm-1.0.2/h5parm/arrays/lofar.hba.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.1/h5parm/datapack.py` & `h5parm-1.0.2/h5parm/datapack.py`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.1/h5parm/maintenance.py` & `h5parm-1.0.2/h5parm/maintenance.py`

 * *Files identical despite different names*

### Comparing `h5parm-1.0.1/h5parm/utils.py` & `h5parm-1.0.2/h5parm/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import re
+from typing import List
 
 import numpy as np
 
 logger = logging.getLogger(__name__)
 import os
 from h5parm.datapack import DataPack
 import astropy.time as at
@@ -308,7 +310,78 @@
                                     ant=antenna_labels, dir=patch_names)
             if 'phase' in soltab:
                 datapack.add_soltab(soltab, weightDtype='f16', freq=freqs, time=times.mjd * 86400., pol=pol_labels,
                                     ant=antenna_labels, dir=patch_names)
             if 'amplitude' in soltab:
                 datapack.add_soltab(soltab, weightDtype='f16', freq=freqs, time=times.mjd * 86400., pol=pol_labels,
                                     ant=antenna_labels, dir=patch_names)
+
+
+def extract_bbs_format(text) -> List[str]:
+    """
+    Gets the format string from a line in BBS file.
+
+    :param text: text that should start with '#' and end with 'format'
+
+    :return: list of field names
+    """
+    pattern = r'\((.*?)\)'
+    matches = re.findall(pattern, text)
+    if matches:
+        return [field.strip() for field in matches[0].split(',')]
+    else:
+        return []
+
+
+def parse_coordinates(ra_str, dec_str) -> ac.ICRS:
+    """
+    Parses the ra/dec strings of sky model.
+    """
+    try:
+        ra = ra_str.strip()
+        dec = dec_str.strip()
+
+        ra_parts = ra.split(':')
+        ra_str = ' '.join(ra_parts)
+
+        dec_parts = dec.split('.')
+        if len(dec_parts) == 4:
+            dec_parts[-1] = '.'.join(dec_parts[-2:])
+            dec_parts = dec_parts[:-1]
+        dec_str = ' '.join(dec_parts)
+
+        coord = ac.SkyCoord(ra_str, dec_str, unit=(au.hourangle, au.deg), frame='icrs')
+        return coord.transform_to(ac.ICRS())
+    except ValueError:
+        raise ValueError(f"Invalid coordinate string {ra_str}, {dec_str}.")
+
+
+def directions_from_sky_model(sky_model: str) -> ac.ICRS:
+    """
+    Get directions from BBS sky model.
+
+    :param sky_model: filename of bbs sky model
+
+    :return: ICRS coordinates of sky model point sources
+    """
+    data = []
+    format = None
+    with open(sky_model, 'r') as f:
+        for line in f:
+            line = line.strip()
+            if (line == ''):
+                continue
+            if line.startswith("#") and line.endswith('format'):
+                format = extract_bbs_format(line)
+                continue
+            data.append(list(map(lambda s: s.strip(), line.split(','))))
+    if format is None:
+        raise ValueError(f'Could not find format in sky model {sky_model}')
+    if 'Ra' not in format:
+        raise ValueError(f"Could not find 'Ra' in format {format}.")
+    if 'Dec' not in format:
+        raise ValueError(f"Could not find 'Dec' in format {format}.")
+    ra_idx = format.index('Ra')
+    dec_idx = format.index('Dec')
+    directions = list(map(lambda d: parse_coordinates(d[ra_idx], d[dec_idx]), data))
+    directions = ac.concatenate(directions)
+    return directions.transform_to(ac.ICRS())
```

### Comparing `h5parm-1.0.1/h5parm.egg-info/PKG-INFO` & `h5parm-1.0.2/h5parm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 1.0.1
+Version: 1.0.2
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `h5parm-1.0.1/setup.py` & `h5parm-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                   'tables>=' + __minimum_tables_version__,
                   'astropy>=' + __minimum_astropy_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='h5parm',
-      version='1.0.1',
+      version='1.0.2',
       description='H5Parm data pack interface',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/h5parm",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

