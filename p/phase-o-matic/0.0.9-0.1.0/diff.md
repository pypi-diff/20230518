# Comparing `tmp/phase-o-matic-0.0.9.tar.gz` & `tmp/phase-o-matic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phase-o-matic-0.0.9.tar", last modified: Fri May 12 19:44:01 2023, max compression
+gzip compressed data, was "phase-o-matic-0.1.0.tar", last modified: Thu May 18 16:33:49 2023, max compression
```

## Comparing `phase-o-matic-0.0.9.tar` & `phase-o-matic-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/phase_o_matic/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/phase_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/phase_o_matic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-12 19:43:43.000000 phase-o-matic-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/tests/test_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:33:49.604728 phase-o-matic-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-18 16:33:49.604728 phase-o-matic-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:33:49.604728 phase-o-matic-0.1.0/phase_o_matic/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/phase_o_matic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/phase_o_matic/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/phase_o_matic/phase_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/phase_o_matic/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/phase_o_matic/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/phase_o_matic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:33:49.604728 phase-o-matic-0.1.0/phase_o_matic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-18 16:33:49.000000 phase-o-matic-0.1.0/phase_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-18 16:33:49.000000 phase-o-matic-0.1.0/phase_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:33:49.000000 phase-o-matic-0.1.0/phase_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-18 16:33:49.000000 phase-o-matic-0.1.0/phase_o_matic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 16:33:49.000000 phase-o-matic-0.1.0/phase_o_matic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:33:49.604728 phase-o-matic-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:33:49.604728 phase-o-matic-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/tests/test_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/tests/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-18 16:33:34.000000 phase-o-matic-0.1.0/tests/test_presto.py
```

### Comparing `phase-o-matic-0.0.9/LICENSE` & `phase-o-matic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.9/PKG-INFO` & `phase-o-matic-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.9
+Version: 0.1.0
 Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,17 +14,19 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # phase-o-matic
-[![PIP](https://img.shields.io/badge/pip-0.0.8-purple)](https://img.shields.io/badge/pip-0.0.8-purple)
+[![PIP](https://img.shields.io/badge/pip-0.0.9-purple)](https://img.shields.io/badge/pip-0.0.9-purple)
 [![LICENSE](https://img.shields.io/badge/license-MIT-orange)](https://img.shields.io/badge/license-MIT-orange)
 [![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382) 
+[![COVERAGE](https://img.shields.io/badge/coverage-89%25-green)](https://img.shields.io/badge/coverage-89%25-green) 
+
 
 Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase.
 
 Useful publications for this repo:
  - Doin, M.-P., Lasserre, C., Peltzer, G., Cavalié, O., and Doubre, C.: Corrections of stratified tropospheric delays in SAR interferometry: Validation with global atmospheric models, J Appl Geophys, 69, 35–50, https://doi.org/10.1016/j.jappgeo.2009.03.010, 2009.
 
  - Jolivet, R., Agram, P. S., Lin, N. Y., Simons, M., Doin, M., Peltzer, G., and Li, Z.: Improving InSAR geodesy using Global Atmospheric Models, J Geophys Res Solid Earth, 119, 2324–2341, https://doi.org/10.1002/2013jb010588, 2014.
@@ -87,16 +89,27 @@
 
 fig, axes = plt.subplots(1, 2, figsize = (12, 9))
 delay_change.plot(ax = axes[0], vmax = 0, vmin = -4)
 dem.plot(ax = axes[1], vmin = 0, vmax = 2000)
 plt.savefig('../images/usage.png')
 ```
 
+## Coverage instructions
+
+Run the following from the root directory of this project to get a coverage report.
+
+You will need to have the dependencies and `coverage` packages available.
+
+```bash
+python -m coverage run -m unittest discover -s ./tests
+python -m coverage report
+```
+
 ## Citations
 
-If you end up using the ERA5 data please cite this repo:
+If you end up finding this repo useful consider citing this repo as:
 
 Keskinen, Z. (2023) Phase-o-matic: InSAR atmospheric delay calculations, https://github.com/ZachKeskinen/phase-o-matic/. DOI: 10.5281/zenodo.7926686
 
-and the ERA5 data citation:
+and any use of the ERA5 data should include the ERA5 data citation:
 
 Hersbach, H., Bell, B., Berrisford, P., Biavati, G., Horányi, A., Muñoz Sabater, J., Nicolas, J., Peubey, C., Radu, R., Rozum, I., Schepers, D., Simmons, A., Soci, C., Dee, D., Thépaut, J-N. (2023): ERA5 hourly data on single levels from 1940 to present. Copernicus Climate Change Service (C3S) Climate Data Store (CDS), DOI: 10.24381/cds.adbb2d47
```

### Comparing `phase-o-matic-0.0.9/README.md` & `phase-o-matic-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # phase-o-matic
-[![PIP](https://img.shields.io/badge/pip-0.0.8-purple)](https://img.shields.io/badge/pip-0.0.8-purple)
+[![PIP](https://img.shields.io/badge/pip-0.0.9-purple)](https://img.shields.io/badge/pip-0.0.9-purple)
 [![LICENSE](https://img.shields.io/badge/license-MIT-orange)](https://img.shields.io/badge/license-MIT-orange)
 [![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382) 
+[![COVERAGE](https://img.shields.io/badge/coverage-89%25-green)](https://img.shields.io/badge/coverage-89%25-green) 
+
 
 Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase.
 
 Useful publications for this repo:
  - Doin, M.-P., Lasserre, C., Peltzer, G., Cavalié, O., and Doubre, C.: Corrections of stratified tropospheric delays in SAR interferometry: Validation with global atmospheric models, J Appl Geophys, 69, 35–50, https://doi.org/10.1016/j.jappgeo.2009.03.010, 2009.
 
  - Jolivet, R., Agram, P. S., Lin, N. Y., Simons, M., Doin, M., Peltzer, G., and Li, Z.: Improving InSAR geodesy using Global Atmospheric Models, J Geophys Res Solid Earth, 119, 2324–2341, https://doi.org/10.1002/2013jb010588, 2014.
@@ -68,16 +70,27 @@
 
 fig, axes = plt.subplots(1, 2, figsize = (12, 9))
 delay_change.plot(ax = axes[0], vmax = 0, vmin = -4)
 dem.plot(ax = axes[1], vmin = 0, vmax = 2000)
 plt.savefig('../images/usage.png')
 ```
 
+## Coverage instructions
+
+Run the following from the root directory of this project to get a coverage report.
+
+You will need to have the dependencies and `coverage` packages available.
+
+```bash
+python -m coverage run -m unittest discover -s ./tests
+python -m coverage report
+```
+
 ## Citations
 
-If you end up using the ERA5 data please cite this repo:
+If you end up finding this repo useful consider citing this repo as:
 
 Keskinen, Z. (2023) Phase-o-matic: InSAR atmospheric delay calculations, https://github.com/ZachKeskinen/phase-o-matic/. DOI: 10.5281/zenodo.7926686
 
-and the ERA5 data citation:
+and any use of the ERA5 data should include the ERA5 data citation:
 
 Hersbach, H., Bell, B., Berrisford, P., Biavati, G., Horányi, A., Muñoz Sabater, J., Nicolas, J., Peubey, C., Radu, R., Rozum, I., Schepers, D., Simmons, A., Soci, C., Dee, D., Thépaut, J-N. (2023): ERA5 hourly data on single levels from 1940 to present. Copernicus Climate Change Service (C3S) Climate Data Store (CDS), DOI: 10.24381/cds.adbb2d47
```

### Comparing `phase-o-matic-0.0.9/phase_o_matic/download.py` & `phase-o-matic-0.1.0/phase_o_matic/download.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,64 +2,89 @@
 import numpy as np
 import pandas as pd
 from shapely import geometry
 from pathlib import Path
 from datetime import datetime
 from typing import Union
 
-def download_era(date: pd.Timestamp, out_dir: Union[str, Path], subset: Union[geometry.Polygon, None], humid_param = 'specific_humidity', LOS: bool = False) -> Path:
+def download_era(date: pd.Timestamp, out_dir: Union[str, Path], subset: Union[geometry.Polygon, None], humid_param = 'specific_humidity', LOS: bool = False, overwrite = False) -> Path:
     """
     Download era5 weather model for specific hourly timestep as netcdf. Can be subset to a specific geographic subset.
 
     Args:
     date: timestamp of the desired date and time. Will be rounded to nearest hour
     out_dir: directory to save file into
     subset: subset geometry to clip data to
     humid_param: relative or specific humidity ('relative_humidity' vs 'specific_humidity')
     LOS: download twice the area to do LOS integrations?
+    overwrite: should existing ERA5 files be overwritten?
 
     returns:
     out_fp: filepath of saved netcdf
     """
     # check to see if era5 token has been saved to .cdsapric file and create client for download
     assert Path('~/.cdsapirc').expanduser().exists(), "Must sign up for ERA5 account and save key to .cdsapric file"
     c = cdsapi.Client()
 
+    # convert out_dir to Path if its a string
     if isinstance(out_dir, str): out_dir = Path(out_dir)
-    out_dir = out_dir.expanduser()
+
+    # expand user and relative paths
+    out_dir = out_dir.expanduser().resolve()
+
+    # error check directory to save to
     assert out_dir.exists(), f"Provided directory: {out_dir} does not exist."
 
-    # pressure levels to download (this is all 37 possible)
+    # pressure levels to download (this is all 37 possible) in millibars
     era_pressure_lvls = ['1','2','3','5','7','10','20','30','50', '70','100','125',\
     '150','175','200','225', '250','300','350','400','450','500','550','600','650',\
     '700','750','775','800','825', '850','875','900','925','950','975','1000']
 
+    # try to convert date to pd datetime
     if isinstance(date, str): date = pd.to_datetime(date)
+
+    # error check bounds of date provided
     assert date < datetime.now(date.tzinfo), "provided date is in the future"
     assert date.year > 1939, "provided date is before january 1940"
 
+    # sets options for download
     indict = {'product_type'   :'reanalysis',\
                 'format'         :'netcdf',\
                 'variable'       :['geopotential','temperature', humid_param],\
                 'pressure_level' : era_pressure_lvls, \
                 'date'           : date.strftime('%Y-%m-%d'),
                 'time'           : date.strftime('%H:00')}
 
+    # name out filepath
     out_fp = out_dir.joinpath(f"ERA5_{date.strftime('%Y-%m-%dT%H:00')}.nc")
 
+    # if a subset was provided. otherwise we are dwonloading everything
     if subset:
+        # get bounds
         w, s, e, n = subset.bounds
+
+        # error check bounds
         assert w > -180 and w < 180, f"West bound: {w} is outside of globe"
         assert e > -180 and e < 180, f"East bound: {e} is outside of globe"
         assert n > -90 and n < 90, f"North bound: {n} is outside of globe"
         assert s > -90 and s < 90, f"South bound: {s} is outside of globe"
+        
+        # expand area by distance across subset if we are gonna try and do line of sight
         if LOS:
             w = np.maximum(w - abs(e - w), -180)
             e = np.minimum(e + abs(e - w), 180)
             s = np.maximum(s - abs(n - s), -90)
             n = np.minimum(n + abs(n - s), 90)
+        
+        # save to download options
         indict['area'] = f'/'.join([str(b) for b in [n, w, s, e]])
-        out_fp = out_fp.with_stem(f"{out_fp.stem}_{'_'.join([f'{b:.2f}' for b in [w, s, e, n]])}")
 
-    c.retrieve('reanalysis-era5-pressure-levels', indict, target = out_fp)
+        # change filename to include subset area
+        out_fp = out_fp.with_stem(f"{out_fp.stem}_{'_'.join([f'{b:.2f}' for b in [w, s, e, n]])}")
 
-    return out_fp
+    # if we aren't overwriting then either download or skip and return existing path
+    if not out_fp.exists() or overwrite == True:
+        c.retrieve('reanalysis-era5-pressure-levels', indict, target = out_fp)
+        return out_fp
+    else:
+        # add logging in here to warn user about not overwriting existing ERA5 file
+        return out_fp
```

### Comparing `phase-o-matic-0.0.9/phase_o_matic/phase_delay.py` & `phase-o-matic-0.1.0/phase_o_matic/phase_delay.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         dataset = dataset.reindex(height=list(reversed(dataset.height)))
 
     # calculate dry refractivity. Reference: https://www.itu.int/dms_pubrec/itu-r/rec/p/R-REC-P.453-11-201507-S!!PDF-E.pdf
     # adapted from eq 3 of Jolivet et al (2014) and https://github.com/insarlab/PyAPS/blob/main/src/pyaps3/processor.py#L216
     # https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1002/2013JB010588?src=getftr
     dataset['N_dry'] = 1.0e-6 * k1 * Rd / g * (dataset['air_pressure'] - dataset['air_pressure'].isel(height = -1))
 
+    dataset['N_dry'] = dataset['N_dry'].assign_attrs(units = '', long_name = 'Hydrostatic Refractivity')
+
     return dataset
 
 def calculate_wet_refractivity(dataset: xr.Dataset) -> xr.Dataset:
     """
     Calculate wet refractivity from vapor pressure, and temperature
     
     Args:
@@ -86,14 +88,16 @@
     s2['height'] = dataset['height']
 
     # calculate for each point along height axis
     dataset['N_wet'] = -1.0e-6 * (((k2 - (k1 * Rd / Rv)) * s1) + ( k3 * s2))
 
     # get change from highest elevation
     dataset['N_wet'] = dataset['N_wet'] - dataset['N_wet'].isel(height = -1)
+
+    dataset['N_wet'] = dataset['N_wet'].assign_attrs(units = '', long_name = 'Water Vapor Refractivity')
     
     return dataset
 
 def calculate_refractive_indexes(dataset: xr.Dataset, wavelength: float = 0.23) -> xr.Dataset:
     """
     Calculate dry and wet refractivity from air pressure, vapor pressure, and temperature.
     Integrate refractivity through atmosphere from high to low.
@@ -108,35 +112,40 @@
     # calculate the refractive index from air pressure
     dataset = calculate_dry_refractivity(dataset)
     # calculate refractivity index from water vapor
     dataset = calculate_wet_refractivity(dataset)
     # combine wet and dry refractivity
     dataset['N'] = dataset['N_dry'] + dataset['N_wet']
 
+    dataset['N'] = dataset['N'].assign_attrs(units = '', long_name = 'Total Refractivity')
+
     return dataset
 
 def get_delay(dataset: xr.Dataset, dem: xr.DataArray, inc: Union[xr.DataArray, float], wavelength: float = 4*np.pi) -> xr.Dataset:
     """
     Get delay in m (default) or radians (if wavelength provided) for each height
     https://github.com/insarlab/PyAPS/blob/244552cdfcf4e1a55de5f1439be4f08eb45872ec/src/pyaps3/objects.py#L213
 
     Args:
     ds: xarray dataset of atmosphere with refractive indexes calculated
-    geometry: xarray dataset of elevations (var_name = 'dem'), incidence angles in radians (var_name = 'inc')
-        and coords for "y" and "x".
+    dem: xarray dataArray of elevations with coords for "latitude" and "longitude".
+    inc: xarray dataArray of incidence angles in radians or a single float to use over the image
     wavelength: either default 4 * pi (returns meters of delay) or radar wavelength in meters (returns radians)
 
     Returns:
     delay: cos calculated phase delay for each weather station data point interpolated to each meter of DEM
     """
 
     assert wavelength > 0, "Can not have negative wavelength"
 
     assert 'N' in dataset.data_vars, "Must have refractivity index calculated to interpolate to DEM"
 
+    assert "latitude" in dem.coords, "Must have latitude as coordinate"
+    assert "longitude" in dem.coords, "Must have longitude as coordinate"
+
     if isinstance(inc, xr.DataArray):
 
         assert inc.mean() < 2*np.pi, f'Incidence mean over 2 pi. Check if you are inc in radians'
 
         # check to see if incidence angle and DEM are aligned and align them if not
         try:
             xr.align(dem, inc, join='exact')
@@ -158,12 +167,19 @@
 
     # interpolate across the dem's lats, longs, and elevations to find the surface delay
     dataset = dataset.interp(latitude = dem.latitude, longitude = dem.longitude, height = dem)
 
     # add phase delay data_variable
     dataset['delay'] = dataset['N']*np.pi*4.0/(wavelength*np.cos(inc))
 
+    if wavelength == 4 * np.pi:
+        dataset['delay'].attrs['units'] = 'meters'
+    else:
+        dataset['delay'].attrs['units'] = 'radians'
+
+    dataset['delay'].attrs['long_name'] = 'Atmospheric Delay'
+
     # make sure we have coordinates in the right order for plotting
     dataset = dataset.transpose('time','latitude','longitude')
 
     return dataset
```

### Comparing `phase-o-matic-0.0.9/phase_o_matic/preprocess.py` & `phase-o-matic-0.1.0/phase_o_matic/preprocess.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,20 +11,26 @@
     Args:
     dataset: xarray dataset with coordinate level in millibars
 
     Returns:
     dataset: xarray dataset with coordinate level in pascals
     """
 
-    if dataset['level'].attrs['units'] != 'pascals':
-        dataset['level'] = dataset['level'] * 100
-        dataset['level'] = dataset['level'].assign_attrs(units = 'pascals', long_name = 'pressure_level')
+    assert 'units' in dataset['level'].attrs, "No assigned units for pressure levels ['level']"
 
+    if dataset['level'].attrs['units'] == 'millibars':
+        dataset['level'] = dataset['level'] * 100
+        dataset['level'] = dataset['level'].assign_attrs(units = 'pascals', long_name = 'Pressure Level')
+    elif dataset['level'].attrs['units'] == 'pascals':
+        pass
+        # print("Pressure levels already converted to pascals")
     else:
-        print("Pressure levels already converted to pascals")
+        raise ValueError(f"Unknown units on 'level' coordinate: {dataset['level'].attrs['units']}\
+            must be one of 'pascals' or 'millibars'")
+    
 
     return dataset
 
 def cc_era(temperature: xr.DataArray):
     '''Clausius Clayperon law used by ERA Interim.
     https://github.com/insarlab/PyAPS/blob/main/src/pyaps3/era.py#L14
 
@@ -39,27 +45,27 @@
     a4w = 32.19
     a1i = 611.21
     a3i = 22.587
     a4i = -0.7
     T3  = 273.16
     Ti  = 250.16
 
-    esta = xr.zeros_like(temperature)
+    sat_vapor_pressure = xr.zeros_like(temperature)
 
     esatw = a1w*np.exp(a3w*(temperature-T3)/(temperature-a4w))
     esati = a1i*np.exp(a3i*(temperature-T3)/(temperature-a4i))
     wgt = (temperature-Ti)/(T3-Ti)
 
-    esta = esta.where(esta < T3, esatw)
-    esta = esta.where(esta > Ti, esati)
-    esta = esta.where((esta >= T3) | (esta <= Ti), esati + (esatw - esati)*wgt*wgt)
+    sat_vapor_pressure = sat_vapor_pressure.where(temperature < T3, esatw)
+    sat_vapor_pressure = sat_vapor_pressure.where(temperature > Ti, esati)
+    sat_vapor_pressure = sat_vapor_pressure.where((temperature >= T3) | (temperature <= Ti), esati + (esatw - esati)*wgt*wgt)
 
-    esta = esta.rename('vapor_saturation_pressure')
+    sat_vapor_pressure = sat_vapor_pressure.rename('vapor_saturation_pressure')
 
-    return esta
+    return sat_vapor_pressure
 
 def get_vapor_partial_pressure(dataset: xr.Dataset) -> xr.Dataset:
     """
     Get vapor partial pressure from humidity for each pressure level
 
     Args:
     dataset: dataset without vpr pressure as a variable
@@ -74,83 +80,46 @@
         # molar gas constant of dry air
         Rd = 287.05  #(J/Kg/K)
         # ratio of the two in air
         alpha = Rv/Rd
         # specific humidity calculation of partial pressure of water vapour
         # https://cran.r-project.org/web/packages/humidity/vignettes/humidity-measures.html equation 4
         # http://www.atmo.arizona.edu/students/courselinks/spring08/atmo336s1/courses/fall13/atmo551a/Site/ATMO_451a_551a_files/WaterVapor.pdf
-        # dataset['vpr'] = dataset['q'] * dataset['level'] / (alpha + (1 - alpha) * dataset['q'])
         dataset['vpr'] = dataset['q'] * dataset['level'] * alpha/ (1+ (alpha - 1)* dataset['q'])
-        # dataset['vpr'] = dataset['q'] * dataset['level']  - 0.622 * dataset['level'] / 100
 
     elif 'r' in dataset.data_vars:
         h2o_sat_partial_p = cc_era(dataset['t'])
         dataset['vpr'] = h2o_sat_partial_p * dataset['r']/100
     
     else:
         raise ValueError("Must have specific or relative humidity as a data variable")
 
     dataset['vpr'].attrs['units'] = 'pascals'
+    dataset['vpr'].attrs['long_name'] = 'Vapor Partial Pressure'
 
     return dataset
 
 def geopotential_to_geopotential_heights(ds: xr.Dataset) -> xr.Dataset:
     """
-    Convert height array from geopotential to WGS84 Ellipsoidal heights
+    Convert height array from geopotential to geopotential heights
 
     Args:
     ds: xarray dataset with geopotentials
 
     Returns:
     ds: xarray dataarray with 'gph' added
     """
     # acceleration due to gravity for geopotential
     g = 9.81 # m s-2
     # convert from geopotential to geopotenial height
     ds['gph'] = ds['z'] / g
 
-    return ds
-
-def check_start_end(hx, min_alt, max_alt):
-    """
-    Check if we need to extend hx to cover min alt to max alt
-    Included to test relative to pyaps but probably not neccessary
-    """
-    start_flag = False
-    end_flag = False
-    #Add point at start
-    if (hx.min() > min_alt):
-        start_flag = True
-        #changed from 1 to 0 (-1 should also work), CL
-        hx = np.concatenate(([min_alt-1], hx),axis = 0)
-
-    #Add point at end
-    if (hx.max() < max_alt):
-        end_flag = True
-        #changed from 1 to 0 (-1 should also work), CL
-        hx = np.concatenate((hx,[max_alt+1]),axis=0)
-    
-    return hx, start_flag, end_flag
+    ds['gph'] = ds['gph'].assign_attrs(units = 'meters', long_name = 'Geopotential Height')
 
-def hy_extend(hx, hy, start_flag, end_flag):
-    """
-    Extend hy to cover full range of min to max altitude.
-    Included to test relative to pyaps but probably not neccessary
-    """
-    if (start_flag == True):
-        val = hy[-1] +(hx[-1] - hx[-2])* (hy[-1] - hy[-2])/(hx[-2]-hx[-3])
-        #changed from 1 to 0 (-1 should also work), CL
-        hy = np.concatenate((hy,[val]),axis=0)
-
-    if (end_flag == True):
-        val = hy[0] - (hx[0] - hx[1]) * (hy[0] - hy[1])/(hx[1]-hx[2])
-        #changed from 1 to 0 (-1 should also work), CL
-        hy = np.concatenate(([val],hy),axis=0)
-    
-    return hy
+    return ds
 
 def interpolate_to_heights(dataset: xr.Dataset, min_alt = -200, n_heights = 300, max_alt: Union[None, float, xr.DataArray] = None) -> xr.Dataset:
     """
     Interpolate vapor pressure, air pressure, and temperatures from pressure level coordinates
     to geopotential height coordinates. Cubic spline is used for each lat and lon.
 
     Args:
@@ -178,15 +147,15 @@
                 'air_pressure': (['time','longitude', 'latitude','height'], np.zeros(new_size), dataset['level'].attrs),
                 'temperature': (['time', 'longitude', 'latitude','height'], np.zeros(new_size), dataset['t'].attrs),
                 'vapor_pressure': (['time', 'longitude', 'latitude','height'], np.zeros(new_size), dataset['vpr'].attrs),
             },  
             coords = {
                 "longitude" : (["longitude"], dataset['longitude'].data, dataset['longitude'].attrs),
                 "latitude" : (["latitude"], dataset['latitude'].data, dataset['latitude'].attrs),
-                "height" : (["height"], heights, {'units' :'meters', 'long_name' :'geopotential_heights'}),
+                "height" : (["height"], heights, dataset['gph'].attrs),
                 "time" : (["time"], dataset['time'].data, {'long_name' :'time'}),
             },
             attrs=dataset.attrs
         )
 
     # scipy 1d interpolate won't accept 2d array as y values so have to iterate
     for time in dataset.time:
@@ -216,9 +185,11 @@
                 interpolated_ds['temperature'].loc[{'time': time,  'latitude': lat, 'longitude': lon}] =  xr.DataArray(interpolated_temperatures, coords = [heights], dims = 'height')
                 
                 # interpolate vapor pressures to vapor pressures at each height level
                 hy = dataset['vpr'].sel(time = time).sel(latitude = lat, longitude = lon).data
                 tck = interpolate.interp1d(hx, hy, axis = -1, kind = 'cubic', fill_value = "extrapolate")
                 interpolated_vapor= tck(heights)
                 interpolated_ds['vapor_pressure'].loc[{'time': time,  'latitude': lat, 'longitude': lon}] =  xr.DataArray(interpolated_vapor, coords = [heights], dims = 'height')
-        
+    
+    interpolated_ds['air_pressure']= interpolated_ds.air_pressure.assign_attrs(long_name = 'Air Pressure')
+
     return interpolated_ds
```

### Comparing `phase-o-matic-0.0.9/phase_o_matic/utils.py` & `phase-o-matic-0.1.0/phase_o_matic/utils.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.9/phase_o_matic.egg-info/PKG-INFO` & `phase-o-matic-0.1.0/phase_o_matic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.9
+Version: 0.1.0
 Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,17 +14,19 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # phase-o-matic
-[![PIP](https://img.shields.io/badge/pip-0.0.8-purple)](https://img.shields.io/badge/pip-0.0.8-purple)
+[![PIP](https://img.shields.io/badge/pip-0.0.9-purple)](https://img.shields.io/badge/pip-0.0.9-purple)
 [![LICENSE](https://img.shields.io/badge/license-MIT-orange)](https://img.shields.io/badge/license-MIT-orange)
 [![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382) 
+[![COVERAGE](https://img.shields.io/badge/coverage-89%25-green)](https://img.shields.io/badge/coverage-89%25-green) 
+
 
 Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase.
 
 Useful publications for this repo:
  - Doin, M.-P., Lasserre, C., Peltzer, G., Cavalié, O., and Doubre, C.: Corrections of stratified tropospheric delays in SAR interferometry: Validation with global atmospheric models, J Appl Geophys, 69, 35–50, https://doi.org/10.1016/j.jappgeo.2009.03.010, 2009.
 
  - Jolivet, R., Agram, P. S., Lin, N. Y., Simons, M., Doin, M., Peltzer, G., and Li, Z.: Improving InSAR geodesy using Global Atmospheric Models, J Geophys Res Solid Earth, 119, 2324–2341, https://doi.org/10.1002/2013jb010588, 2014.
@@ -87,16 +89,27 @@
 
 fig, axes = plt.subplots(1, 2, figsize = (12, 9))
 delay_change.plot(ax = axes[0], vmax = 0, vmin = -4)
 dem.plot(ax = axes[1], vmin = 0, vmax = 2000)
 plt.savefig('../images/usage.png')
 ```
 
+## Coverage instructions
+
+Run the following from the root directory of this project to get a coverage report.
+
+You will need to have the dependencies and `coverage` packages available.
+
+```bash
+python -m coverage run -m unittest discover -s ./tests
+python -m coverage report
+```
+
 ## Citations
 
-If you end up using the ERA5 data please cite this repo:
+If you end up finding this repo useful consider citing this repo as:
 
 Keskinen, Z. (2023) Phase-o-matic: InSAR atmospheric delay calculations, https://github.com/ZachKeskinen/phase-o-matic/. DOI: 10.5281/zenodo.7926686
 
-and the ERA5 data citation:
+and any use of the ERA5 data should include the ERA5 data citation:
 
 Hersbach, H., Bell, B., Berrisford, P., Biavati, G., Horányi, A., Muñoz Sabater, J., Nicolas, J., Peubey, C., Radu, R., Rozum, I., Schepers, D., Simmons, A., Soci, C., Dee, D., Thépaut, J-N. (2023): ERA5 hourly data on single levels from 1940 to present. Copernicus Climate Change Service (C3S) Climate Data Store (CDS), DOI: 10.24381/cds.adbb2d47
```

### Comparing `phase-o-matic-0.0.9/setup.py` & `phase-o-matic-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version='0.0.9',
+    version='0.1.0',
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `phase-o-matic-0.0.9/tests/test_delay.py` & `phase-o-matic-0.1.0/tests/test_delay.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         test_ds = test_ds.interp(height = np.linspace(20000, -100, 200))
         original = test_ds.copy()
         test_ds = calculate_dry_refractivity(test_ds)
 
         original = original.reindex(height=list(reversed(original.height)))
         assert_allclose(test_ds['N_dry'], 1.0e-6 * 0.776 * 287.05 / 9.81 * (original['air_pressure']  - original['air_pressure'].isel(height = -1)))
 
+        self.assertEqual(test_ds['N_dry'].units, '')
+        self.assertEqual(test_ds['N_dry'].long_name, 'Hydrostatic Refractivity')
+
     def test_dry_refractivity_errors(self, test_ds = test_ds):
         """
         Test for correct errors in dry refractivity
         """
 
         test_ds['air_pressure'] = test_ds['air_pressure'].assign_attrs({'units':'bars'})
 
@@ -99,14 +102,17 @@
 
         if Path('./tests/test_data/wet_N_seed_1.npy').exists():
             N_wet_correct = np.load('./tests/test_data/wet_N_seed_11.npy')
             assert_allclose(test_ds['N_wet'].data, N_wet_correct)
         elif Path('./test_data/wet_N_seed_1.npy').exists():
             N_wet_correct = np.load('./test_data/wet_N_seed_11.npy')
             assert_allclose(test_ds['N_wet'].data, N_wet_correct)
+
+        self.assertEqual(test_ds['N_wet'].units, '')
+        self.assertEqual(test_ds['N_wet'].long_name, 'Water Vapor Refractivity')
     
     def test_wet_refractivity_errors(self, test_ds = test_ds):
         """
         Test for correct errors in wet refractivity
         """
 
         test_ds['vapor_pressure'] = test_ds['vapor_pressure'].assign_attrs({'units':'bars'})
@@ -145,14 +151,17 @@
 
         if directory.joinpath('test_data/wet_N_seed_1.npy').exists():
             N_wet_correct = np.load('./tests/test_data/wet_N_seed_11.npy')
             assert_allclose(test_ds['N_wet'].data, N_wet_correct)
         
         if "N_wet_correct" in locals():
             assert_allclose(test_ds['N'].data, N_wet_correct + N_dry_correct)
+        
+        self.assertEqual(test_ds['N'].units, '')
+        self.assertEqual(test_ds['N'].long_name, 'Total Refractivity')
     
     dem = xr.DataArray(np.linspace(1000, 3000, 200*300).reshape(200, 300),
                     coords = [np.linspace(43, 45, 200), np.linspace(-116, -115, 300)],
                     dims = ['latitude','longitude']
     )
 
     inc = xr.DataArray(np.linspace(0, np.deg2rad(90), 200*300).reshape(200, 300),
@@ -167,14 +176,16 @@
         test_ds = calculate_refractive_indexes(test_ds)
         original = test_ds.copy()
 
         test_ds = get_delay(test_ds, dem, inc)
 
         self.assertTrue('delay' in test_ds.data_vars)
 
+        self.assertEqual(test_ds['delay'].attrs['units'], 'meters')
+
         directory = Path(__file__).parent.resolve()
         if directory.joinpath('test_data/delay_seed_1.npy').exists():
             delay_correct = np.load('./tests/test_data/delay_seed_1.npy')
             assert_allclose(test_ds['delay'].data, delay_correct)
         
         # failure here suggests we didn't align to the DEM correctly
         try:
@@ -191,23 +202,28 @@
         
 
         test_ds = original.copy()
         try:
             test_ds = get_delay(test_ds, dem, inc = inc, wavelength = 10)
         except:
             self.fail('Failed using non default wavelength')
+        
+        self.assertEqual(test_ds['delay'].attrs['units'], 'radians')
 
         assert_allclose(test_ds['delay'].data, 4 * np.pi * delay_correct / 10)
+
+        self.assertEqual(test_ds['delay'].long_name, 'Atmospheric Delay')
         
         
     def test_get_delay_errors(self, test_ds = test_ds, dem = dem, inc = inc):
         """
         Test for corret errors through from delay function
         """
 
+        test_ds = test_ds.drop_vars('N')
         self.assertRaises(AssertionError, get_delay, test_ds, dem, inc)
         
         test_ds = calculate_refractive_indexes(test_ds)
 
         inc_to_high = inc * 100
         
         self.assertRaises(AssertionError, get_delay, test_ds, dem, inc_to_high)
```

### Comparing `phase-o-matic-0.0.9/tests/test_download.py` & `phase-o-matic-0.1.0/tests/test_download.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,45 @@
     Test functionality of downloading ERA5 model data
     """
 
     params = [geometry.box(-116, 45, -115, 46), pd.to_datetime('2020-01-03T20:01:0000'), Path('/tmp')]
 
     def test_download(self, params = params):
         """
-        Test downloading era5 data
+        Test downloading era5 data. We only try once to avoid slowing things down.
         """
         area, ts, out_dir = params
 
         out_fp = download_era(date = ts, out_dir = out_dir, subset = area, humid_param ='specific_humidity')
 
         ds = xr.open_dataset(out_fp)
 
         self.assertEqual(ds.level.size, 37, "levels are not right size")
         self.assertEqual(ds.time[0], pd.to_datetime('2020-01-03T20:00:00.000000000'), "incorrect time data")
         self.assertEqual(ds['level'][10], 100, "spot checking pressure levels")
-        self.assertEqual(ds.isel(level = 3)['q'].data.shape, (1, 5, 5), "checking data shape")
         self.assertTrue('z' in ds.data_vars, "geopotential heights present")
         self.assertTrue('t' in ds.data_vars, "Temperature present")
         self.assertTrue('q' in ds.data_vars, "Specific humidity present")
+        self.assertEqual(ds['z'].data.shape, (1, 37, 5, 5), "checking data shape")
+
+        try:
+            out_fp = download_era(date = ts, out_dir = out_dir, subset = area, humid_param ='specific_humidity')
+        except:
+            self.fail('download failed with exisiting file.')
+        
+        out_fp = download_era(date = ts, out_dir = out_dir, subset = area, humid_param ='relative_humidity', LOS = True)
+        ds = xr.open_dataset(out_fp)
+
+        self.assertEqual(ds.level.size, 37, "levels are not right size")
+        self.assertEqual(ds.time[0], pd.to_datetime('2020-01-03T20:00:00.000000000'), "incorrect time data")
+        self.assertEqual(ds['level'][10], 100, "spot checking pressure levels")
+        self.assertTrue('z' in ds.data_vars, "geopotential heights present")
+        self.assertTrue('t' in ds.data_vars, "Temperature present")
+        self.assertTrue('r' in ds.data_vars, "relative humidity present")
+        self.assertEqual(ds['z'].data.shape, (1, 37, 17, 17), "checking data shape for LOS correction")
     
     def test_invalid_inputs(self, params = params):
         """
         Test for invalid user inputs
         """
         area, ts, out_dir = params
```

