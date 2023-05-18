# Comparing `tmp/obrpy-0.0.7.tar.gz` & `tmp/obrpy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obrpy-0.0.7.tar", last modified: Mon May  8 16:22:43 2023, max compression
+gzip compressed data, was "obrpy-0.0.8.tar", last modified: Thu May 18 15:09:10 2023, max compression
```

## Comparing `obrpy-0.0.7.tar` & `obrpy-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 16:22:43.881211 obrpy-0.0.7/
--rw-rw-rw-   0        0        0      283 2023-05-08 16:22:43.881211 obrpy-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 16:22:43.854033 obrpy-0.0.7/obrpy/
--rw-rw-rw-   0        0        0     1341 2023-02-23 12:03:19.000000 obrpy-0.0.7/obrpy/PathSelector.py
--rw-rw-rw-   0        0        0     5304 2023-05-04 14:08:11.000000 obrpy-0.0.7/obrpy/__init__.py
--rw-rw-rw-   0        0        0     2022 2023-05-03 10:35:47.000000 obrpy-0.0.7/obrpy/load.py
--rw-rw-rw-   0        0        0     8391 2023-04-26 14:25:18.000000 obrpy-0.0.7/obrpy/obr.py
--rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.0.7/obrpy/obrsdk.py
--rw-rw-rw-   0        0        0     2663 2023-04-26 14:11:20.000000 obrpy-0.0.7/obrpy/save.py
--rw-rw-rw-   0        0        0     3729 2023-04-26 15:09:07.000000 obrpy-0.0.7/obrpy/settings.py
--rw-rw-rw-   0        0        0     3425 2023-05-03 08:58:35.000000 obrpy-0.0.7/obrpy/take_a_look.py
--rw-rw-rw-   0        0        0     1930 2023-04-26 12:15:31.000000 obrpy-0.0.7/obrpy/update.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:22:43.874187 obrpy-0.0.7/obrpy.egg-info/
--rw-rw-rw-   0        0        0      283 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-08 16:22:43.000000 obrpy-0.0.7/obrpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 16:22:43.881211 obrpy-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-05-08 16:19:00.000000 obrpy-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:22:43.880217 obrpy-0.0.7/test/
--rw-rw-rw-   0        0        0      697 2023-05-04 15:23:53.000000 obrpy-0.0.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:09:10.910730 obrpy-0.0.8/
+-rw-rw-rw-   0        0        0      283 2023-05-18 15:09:10.910730 obrpy-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 15:09:10.870723 obrpy-0.0.8/obrpy/
+-rw-rw-rw-   0        0        0     1341 2023-02-23 12:03:19.000000 obrpy-0.0.8/obrpy/PathSelector.py
+-rw-rw-rw-   0        0        0     8506 2023-05-10 14:51:12.000000 obrpy-0.0.8/obrpy/__init__.py
+-rw-rw-rw-   0        0        0     1328 2023-05-10 14:52:06.000000 obrpy-0.0.8/obrpy/checkouts.py
+-rw-rw-rw-   0        0        0     1063 2023-05-10 14:43:49.000000 obrpy-0.0.8/obrpy/clear.py
+-rw-rw-rw-   0        0        0     2246 2023-05-10 14:46:47.000000 obrpy-0.0.8/obrpy/load.py
+-rw-rw-rw-   0        0        0     8323 2023-05-10 11:38:23.000000 obrpy-0.0.8/obrpy/obr.py
+-rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.0.8/obrpy/obrsdk.py
+-rw-rw-rw-   0        0        0     3212 2023-05-10 14:09:36.000000 obrpy-0.0.8/obrpy/save.py
+-rw-rw-rw-   0        0        0     3741 2023-05-10 12:02:20.000000 obrpy-0.0.8/obrpy/settings.py
+-rw-rw-rw-   0        0        0     3425 2023-05-03 08:58:35.000000 obrpy-0.0.8/obrpy/take_a_look.py
+-rw-rw-rw-   0        0        0     3350 2023-05-10 15:00:23.000000 obrpy-0.0.8/obrpy/update.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:09:10.902723 obrpy-0.0.8/obrpy.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 15:09:10.910730 obrpy-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-05-18 15:08:49.000000 obrpy-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:09:10.910730 obrpy-0.0.8/test/
+-rw-rw-rw-   0        0        0      812 2023-05-10 14:57:34.000000 obrpy-0.0.8/test/test.py
```

### Comparing `obrpy-0.0.7/obrpy/PathSelector.py` & `obrpy-0.0.8/obrpy/PathSelector.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.7/obrpy/__init__.py` & `obrpy-0.0.8/obrpy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -126,37 +126,110 @@
     class Settings(object):
         """ Class to manage settings information """
 
         def __init__(self,situation):
 
             self.situation = situation         
             self.info = {'Calibration':None,'Test':None}
+            
+            self.T0 = ''    # [ºC]
+            self.T1 = ''    # [ºC/m]      T(x) = T0 + T1 * x  -> Name of temperature coeficients in OBRbook 
+            self.E0 = ''    # []          E(x) = E0 + E1 * x  -> Name of strain coeficients in OBRbook
+            self.E1 = ''    # [1/m]
+            self.z_ini = 0  # Initial point of the segment of interest x=0
+            self.z_fin = 0  # Final point of the segment of interest x=0
+        
+        def update(self):
+
+            self.T0     = str(self.info['Calibration'].loc[0, 1])
+            self.T1     = str(self.info['Calibration'].loc[0, 3])
+            self.E0     = str(self.info['Calibration'].loc[1, 1])
+            self.E1     = str(self.info['Calibration'].loc[1, 3])
+            self.z_ini  = float(self.info['Calibration'].loc[2, 1])
+            self.z_fin  = float(self.info['Calibration'].loc[3, 1])
+
 
     class Signal(object):
 
         """ Class to contain all singal analysis functions available """
 
         def __init__(self) -> None:
             pass
 
+
         from .SIGNAL.cross_spectrum import PSSS
         from .SIGNAL.spectral_shift import spectral_shift, spectral_shift_GPU
 
+    class Slice(object):
+        """
+        Container class for one slice
+        """
+
+        def __init__(self):
+            self.ID           = 0       # ID of the slice, within the slices objet
+            self.T            = 0       # Temperature of the slice
+            self.E            = 0       # Strain of the slice
+            self.z            = 0       # [m]   spatial axis
+            self.x            = 0       # [mm]  Relative position of this slide into the segment of interest (to compute T and E as uniform variables)
+            self.f_0          = 0       # [GHz] Initial scan frequency
+            self.f_end        = 0       # [GHz] Final scan frequency
+            self.delta        = 0       # [Number of points] Sensor spacing 
+            self.window       = 0       # [Number of points] Sensor length
+            self.date         = ''      # Date of the measurement formatted as %Y,%M,%D,%h:%m:%s
+            self.parent_file  = ''      # File where the data has been extracted
+            self.P            = list()  # p-polarization signal, later it will be a complex numpy array
+            self.S            = list()  # s-polarization signal, later it will be a complex numpy array
+
+    class Slices(object):
+
+        """
+        Class to contain a dataset of slices
+        """
+
+        def __init__(self):
+
+                self.last_ID = -1
+                self.slices  = dict()
+
+        def update_from_file(self,path):
+
+            self.path   = path
+            self.name   = '' # TO BE DONE (just taking from path, you know ...)
+
+            try:
+                self.load()
+                print('\nSLICES found!')
+
+            except Exception as e:
+
+                if 'No such file or directory' in str(e):
+                    print('\nNO SLICES FOUND IN PATH')
+                else:
+                    print(e)
+                    exit()
+
+        from .load import load
     
 
     ######### Methods definitions #########
 
     # from .take_a_look import take_a_look # TO BE DONE
 
     from .load import load, new
 
-    from .save import save, save_something , save_OBRbook, save_OBRfiles, save_settings
+    from .save import save, save_something , save_OBRbook, save_OBRfiles, save_settings, save_slicesbook, save_slices
 
-    from .update import update_OBRbook, update_OBRfiles, update_settings
+    from .update import update_OBRbook, update_OBRfiles, update_settings, update_slicesbook, update_slicesbook_from_slices, update_slices, update_slices_from_slicesbook
 
+    from .clear import clear_slices, clear_dataset
+
+    from .checkouts import OBR_checkout, settings_file_checkout, slices_checkout
+    
     from .obr import mainOBR, genOBRbook, computeOBR
 
     from .obrsdk import OBRSDKcalibration, OBRSDKalignment, OBRSDKscan, OBRSDKextendedScan
 
     from .settings import genSettingsTemplate, genSettings, _getNewValuesFromOBRbook
 
     from .ANALYSIS.global_analysis import global_analysis, global_analysis_GPU
+
+    from .ANALYSIS.local_analysis import genSlices, _obr2slices
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `obrpy-0.0.7/obrpy/load.py` & `obrpy-0.0.8/obrpy/load.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,22 +42,34 @@
             shutil.move(os.path.join(self.path,file), os.path.join(self.path,self.folders['OBR'],file))
 
     # Information filenames
     self.INFO = {
     'OBR book filename'             :   'OBR_book.csv',
     'OBRfiles filename'             :   'OBRfiles.pkl',
     'settings filename'             :   'settings.xlsx',
-    '':'',
-    'measures filename'             :   'measures.pkl',
     'slices book filename'          :   'slices_book.csv',
     'slices filename'               :   'slices.pkl',
+    '':'',
+    'measures filename'             :   'measures.pkl',
     'dataset book filename'         :   'dataset_book.csv',
     'dataset filename'              :   'dataset.pkl',
     'fiber distribution filename'   :   'fiber_distribution.txt'}
 
     ######### Other atributes inicialization  #########
 
     # All OBR files as a dictionary
     self.OBRfiles = dict()
 
     # OBR book as a pandas df 
     self.OBRbook = None
+
+    # Settings
+    self.settings = self.Settings(None)
+
+    # Signal module
+    self.signal = self.Signal()
+
+    # Slices
+    self.slices = self.Slices()
+
+    # Slices book as pandas df
+    self.slicesbook = None
```

### Comparing `obrpy-0.0.7/obrpy/obr.py` & `obrpy-0.0.8/obrpy/obr.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,36 +125,35 @@
         return
     else:
         pass
 
     # Check for region of interest
     if limit1==None and limit2==None:
 
-        if not os.path.exists(os.path.join(self.path,self.folders['INFORMATION'],self.INFO['settings filename'])):
+        if self.settings.info['Calibration'] is None and self.settings.info['Test'] is None:
             # If there is not settings file, display warning
             print('WARNING: No settings found')
             print('Please if you want to configure the DOFS settings run:')
-            print('     your_obrpy_object.genSETTINGStemplate()')
+            print('     your_obrpy_object.genSettingsTemplate()')
             print('and edit it')
             print('WARNING: No limits were specified')
             print(' if you want to compute the full lenght of sensors leave empty the next prompts')
 
             limit1 = input(' Region of interest start point [m]: ')
             limit2 = input(' Region of interest end point [m]: ')
 
             limit1 = False if limit1 == "" else float(limit1)
             limit2 = False if limit2 == "" else float(limit2)
 
 
         else:
-            # Gets limits from conditions file
-            df = pd.read_csv(os.path.join(self.path,self.folders['INFORMATION'],self.INFO['settings filename']))
-
-            limit1 = float(df['limit1\n[m]'][0])
-            limit2 = float(df['limit2\n[m]'][0])
+            # Gets limits from settings
+            
+            limit1 = self.settings.z_ini
+            limit2 = self.settings.z_fin
 
     # Generate datasets from selected data
     for key, OBRfile in self.OBRfiles.items():
 
         import psutil
         if psutil.virtual_memory()[2] < 90:
 
@@ -175,26 +174,27 @@
             print('just run again DATASETS.computeOBR() until no more .obr files are read')
             self.save()
             return False
             exit()
 
     return True
 
-def find_OBR(path:str) -> list:
+def find_OBR(path:str, verbose=False) -> list:
     """ Function to find all .obr files from a folder
 
         param:  path      (str)          : path to folder
         return: OBR_files (list of str)  : list of OBR filenames
 
     """
     # Find all .obr files
     OBR_files = glob.glob(os.path.join(path,'*.obr'))
-    print(OBR_files)
+    print(OBR_files) if verbose else None
     # Keep just filename and extension (basename)
     OBR_files = [os.path.basename(f) for f in OBR_files]
+    print(OBR_files) if verbose else None
     return OBR_files
 
 def get_date(file:str) -> str:
     """
     Open an .obr file to get date of the measure
 
         param: file (str): file to be read
```

### Comparing `obrpy-0.0.7/obrpy/obrsdk.py` & `obrpy-0.0.8/obrpy/obrsdk.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.7/obrpy/save.py` & `obrpy-0.0.8/obrpy/save.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,8 +83,25 @@
 
     # create the "Test" sheet
     test_data =self.settings.info['Test']
     test_data.to_excel(writer, sheet_name='Test', index=False)
 
     # save the Excel file
     writer.save()
-    print('--> settings file saved in', book_path)
+    print('--> settings file saved in', book_path)
+
+def save_slicesbook(self) -> None:
+
+    """ Save slices book as .csv"""
+    
+    book_path = os.path.join(self.path,self.folders['INFORMATION'],self.INFO['slices book filename'])
+    self.slicesbook.to_csv(book_path, index=False)
+    print('--> slices book saved in', book_path)
+
+
+def save_slices(self) -> None:
+
+    """ Save slices once computed """
+
+    path_to = os.path.join(self.path,self.folders['PROCESSED_DATA'],self.INFO['slices filename'])
+    object_to_save = self.slices
+    self.save_something(object_to_save,path_to)
```

### Comparing `obrpy-0.0.7/obrpy/settings.py` & `obrpy-0.0.8/obrpy/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         In the calibration situation the microstrain (Delta eps) and temperature (Delta T) 
         are asumed to vary in a linerar way, and only one segment (from z_ini->x=0 to z_fin)
         of the fiber is subjected to these variations.
 
     """
 
     data = [
-        ['Delta T = ','','x + ',''],
-        ['Delta eps = ','','x + ',''],
+        ['Delta T = ','','+ ','','x [m]'],
+        ['Delta eps = ','','+ ','','x [m]'],
         ['z_ini [m] =',''],
         ['z_fin [m] =','']
     ]
     df = pd.DataFrame(data)
     return df
 
 def _getNewValuesFromOBRbook(self) -> list:
```

### Comparing `obrpy-0.0.7/obrpy/take_a_look.py` & `obrpy-0.0.8/obrpy/take_a_look.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.7/setup.py` & `obrpy-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.7' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.8' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'obrpy' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Andres Pedraza Rodriguez' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'a.pedraza@upm.es' #Modificar con vuestros datos
 URL = 'https://github.com/temisAP' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = "This library is aimed for using Luna's OBR-4600 with Python." #Descripción corta
```

### Comparing `obrpy-0.0.7/test/test.py` & `obrpy-0.0.8/test/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,31 +2,41 @@
 import os
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
 from obrpy import obrpy
 
 obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
 
+obrpy_obj.update_OBRbook()
+obrpy_obj.update_OBRfiles()
+obrpy_obj.save()
+
+obrpy_obj.genSlices()
+
+exit()
+
 Y0 = obrpy_obj.OBRfiles['2'].Data
 Y1 = obrpy_obj.OBRfiles['B11'].Data
 F =  obrpy_obj.OBRfiles['2'].f
 Z =  obrpy_obj.OBRfiles['2'].z
 
 import numpy as np
 Y0 = np.array(Y0)
-Y0 = Y0[:,0:10000]
+Y0 = Y0[:,0:5000]
 
 Y1 = np.array(Y1)
-Y1 = Y1[:,0:10000]
+Y1 = Y1[:,0:5000]
 
 Z = np.array(Z)
-Z = Z[0:10000]
+Z = Z[0:5000]
+
+
 
 out = obrpy_obj.global_analysis_GPU(Y0, Y1, Z, F, local_function=obrpy_obj.Signal.spectral_shift_GPU, point=1)
 
 
 import matplotlib.pyplot as plt
 
 plt.figure()
 plt.plot(Z,out)
 plt.grid()
-plt.show()
+plt.show()
```

