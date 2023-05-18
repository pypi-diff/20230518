# Comparing `tmp/cometspy-0.4.8.tar.gz` & `tmp/cometspy-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cometspy-0.4.8.tar", last modified: Wed May 26 18:00:52 2021, max compression
+gzip compressed data, was "dist/cometspy-0.4.9.tar", last modified: Thu May 27 16:12:13 2021, max compression
```

## Comparing `cometspy-0.4.8.tar` & `cometspy-0.4.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 djordje   (1000) djordje   (1000)        0 2021-05-26 18:00:52.001556 cometspy-0.4.8/
--rw-rw-r--   0 djordje   (1000) djordje   (1000)      696 2021-05-26 18:00:52.001556 cometspy-0.4.8/PKG-INFO
-drwxrwxr-x   0 djordje   (1000) djordje   (1000)        0 2021-05-26 18:00:52.001556 cometspy-0.4.8/cometspy/
--rw-r--r--   0 djordje   (1000) djordje   (1000)     1622 2020-12-09 15:02:01.000000 cometspy-0.4.8/cometspy/__init__.py
--rw-rw-r--   0 djordje   (1000) djordje   (1000)    32268 2021-05-14 17:16:46.608964 cometspy-0.4.8/cometspy/comets.py
--rw-r--r--   0 djordje   (1000) djordje   (1000)    60468 2021-05-14 02:24:11.312630 cometspy-0.4.8/cometspy/layout.py
--rw-r--r--   0 djordje   (1000) djordje   (1000)    42138 2021-05-26 17:57:48.680947 cometspy-0.4.8/cometspy/model.py
--rw-r--r--   0 djordje   (1000) djordje   (1000)    17512 2021-05-14 02:09:32.378270 cometspy-0.4.8/cometspy/params.py
--rwxr--r--   0 djordje   (1000) djordje   (1000)     6031 2020-12-09 19:56:28.000000 cometspy-0.4.8/cometspy/utils.py
--rw-r--r--   0 djordje   (1000) djordje   (1000)       62 2020-07-15 15:16:42.000000 cometspy-0.4.8/setup.cfg
--rw-r--r--   0 djordje   (1000) djordje   (1000)     1059 2021-05-26 17:58:19.813805 cometspy-0.4.8/setup.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2021-05-27 16:12:13.000000 cometspy-0.4.9/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      696 2021-05-27 16:12:13.000000 cometspy-0.4.9/PKG-INFO
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2021-05-27 16:12:13.000000 cometspy-0.4.9/cometspy/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1622 2021-05-27 15:31:40.000000 cometspy-0.4.9/cometspy/__init__.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)    32447 2021-05-27 15:49:46.000000 cometspy-0.4.9/cometspy/comets.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)    60466 2021-05-27 15:33:30.000000 cometspy-0.4.9/cometspy/layout.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)    42138 2021-05-27 15:31:40.000000 cometspy-0.4.9/cometspy/model.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)    17512 2021-05-27 15:31:40.000000 cometspy-0.4.9/cometspy/params.py
+-rwxr-xr-x   0 jeremy    (1000) jeremy    (1000)     6031 2021-05-27 15:31:40.000000 cometspy-0.4.9/cometspy/utils.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       62 2021-05-27 15:31:40.000000 cometspy-0.4.9/setup.cfg
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1059 2021-05-27 16:05:59.000000 cometspy-0.4.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cometspy-0.4.8/PKG-INFO` & `cometspy-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: cometspy
-Version: 0.4.8
+Version: 0.4.9
 Summary: The Python interface to COMETS
 Home-page: https://github.com/segrelab/cometspy
 Author: The COMETSPy Core Team
 Author-email: djordje.bajic@yale.edu
 License: GPL
-Download-URL: https://github.com/segrelab/cometspy/archive/v0.4.8.tar.gz
+Download-URL: https://github.com/segrelab/cometspy/archive/v0.4.9.tar.gz
 Description: UNKNOWN
 Keywords: metabolism,dynamic,flux,balance,analysis,spatial,evolution
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cometspy-0.4.8/cometspy/__init__.py` & `cometspy-0.4.9/cometspy/__init__.py`

 * *Files identical despite different names*

### Comparing `cometspy-0.4.8/cometspy/comets.py` & `cometspy-0.4.9/cometspy/comets.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,19 +399,21 @@
         self.__analyze_run_output()
         
         # '''----------- READ OUTPUT ---------------------------------------'''
         # Read total biomass output
         if self.parameters.all_params['writeTotalBiomassLog']:
             tbmf = _readlines_file(
                 self.working_dir + self.parameters.all_params['TotalBiomassLogName'])
+            tbmf = [x.replace(",",".") for x in tbmf] # for systems that use commas as decimal place
             self.total_biomass = pd.DataFrame([re.split(r'\t+', x.strip())
                                                for x in tbmf],
                                               columns=['cycle'] +
                                               self.layout.get_model_ids())
             self.total_biomass = self.total_biomass.astype('float')
+            self.total_biomass.cycle = self.total_biomass.cycle.astype('int')
             if delete_files:
                 os.remove(self.working_dir + self.parameters.all_params['TotalBiomassLogName'])
 
         # Read flux
         if self.parameters.all_params['writeFluxLog']:
 
             max_rows = 4 + max([len(m.reactions) for m in self.layout.models])
```

### Comparing `cometspy-0.4.8/cometspy/layout.py` & `cometspy-0.4.9/cometspy/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         Parameters
         ----------
         input_obj : str
             the path to the existing COMETS layout file to be loaded
 
         """
         # .. load layout file
-        f_lines = [s for s in __read_file(input_obj).splitlines() if s]
+        f_lines = [s for s in _read_file(input_obj).splitlines() if s]
         filedata_string = os.linesep.join(f_lines)
         end_blocks = []
         for i in range(0, len(f_lines)):
             if '//' in f_lines[i]:
                 end_blocks.append(i)
 
         # '''----------- GRID ------------------------------------------'''
@@ -1422,12 +1422,12 @@
                     
     def __get_met_number(self, met):
         """ returns the met number (of the external mets) given a name """
         met_number = [x for x in range(len(self.all_exchanged_mets)) if
                       self.all_exchanged_mets[x] == met][0]
         return(met_number)
 
-def __read_file(filename):
+def _read_file(filename):
     f = open(filename, 'r')
     f_lines = f.read()
     f.close()
     return f_lines
```

### Comparing `cometspy-0.4.8/cometspy/model.py` & `cometspy-0.4.9/cometspy/model.py`

 * *Files identical despite different names*

### Comparing `cometspy-0.4.8/cometspy/params.py` & `cometspy-0.4.9/cometspy/params.py`

 * *Files identical despite different names*

### Comparing `cometspy-0.4.8/cometspy/utils.py` & `cometspy-0.4.9/cometspy/utils.py`

 * *Files identical despite different names*

### Comparing `cometspy-0.4.8/setup.py` & `cometspy-0.4.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from os import path
 
 setup(
     name='cometspy',
     packages=['cometspy'],
-    version='0.4.8',
+    version='0.4.9',
     license='GPL',
     description='The Python interface to COMETS',
     author='The COMETSPy Core Team',
     author_email='djordje.bajic@yale.edu',
     url='https://github.com/segrelab/cometspy',
-    download_url='https://github.com/segrelab/cometspy/archive/v0.4.8.tar.gz',  # New releases here!! 
+    download_url='https://github.com/segrelab/cometspy/archive/v0.4.9.tar.gz',  # New releases here!! 
     keywords=['metabolism', 'dynamic', 'flux', 'balance', 'analysis', 'spatial', 'evolution'],
     install_requires=[
         # I get to this in a second
         'numpy',
         'cobra',
         'pandas>=1.0.0'],
     classifiers=[
```

