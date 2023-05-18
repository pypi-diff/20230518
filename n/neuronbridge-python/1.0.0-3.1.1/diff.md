# Comparing `tmp/neuronbridge-python-1.0.0.tar.gz` & `tmp/neuronbridge-python-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuronbridge-python-1.0.0.tar", last modified: Mon Apr 25 21:04:12 2022, max compression
+gzip compressed data, was "neuronbridge-python-3.1.1.tar", last modified: Thu May 18 20:18:34 2023, max compression
```

## Comparing `neuronbridge-python-1.0.0.tar` & `neuronbridge-python-3.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 rokickik (196774796) staff       (20)        0 2022-04-25 21:04:12.419515 neuronbridge-python-1.0.0/
--rw-r--r--   0 rokickik (196774796) staff       (20)     1539 2022-04-25 18:51:43.000000 neuronbridge-python-1.0.0/LICENSE
--rw-r--r--   0 rokickik (196774796) staff       (20)     1653 2022-04-25 21:04:12.419100 neuronbridge-python-1.0.0/PKG-INFO
--rw-r--r--   0 rokickik (196774796) staff       (20)     1150 2022-04-25 20:30:23.000000 neuronbridge-python-1.0.0/README.md
-drwxr-xr-x   0 rokickik (196774796) staff       (20)        0 2022-04-25 21:04:12.415574 neuronbridge-python-1.0.0/neuronbridge/
--rw-r--r--   0 rokickik (196774796) staff       (20)        1 2022-04-25 18:51:43.000000 neuronbridge-python-1.0.0/neuronbridge/__init__.py
--rw-r--r--   0 rokickik (196774796) staff       (20)     5670 2022-04-25 18:51:43.000000 neuronbridge-python-1.0.0/neuronbridge/client.py
--rw-r--r--   0 rokickik (196774796) staff       (20)      554 2022-04-25 18:51:43.000000 neuronbridge-python-1.0.0/neuronbridge/generate_schemas.py
--rw-r--r--   0 rokickik (196774796) staff       (20)     8532 2022-04-25 18:51:43.000000 neuronbridge-python-1.0.0/neuronbridge/model.py
--rw-r--r--   0 rokickik (196774796) staff       (20)      836 2022-04-25 18:51:43.000000 neuronbridge-python-1.0.0/neuronbridge/utils.py
-drwxr-xr-x   0 rokickik (196774796) staff       (20)        0 2022-04-25 21:04:12.418378 neuronbridge-python-1.0.0/neuronbridge_python.egg-info/
--rw-r--r--   0 rokickik (196774796) staff       (20)     1653 2022-04-25 21:04:11.000000 neuronbridge-python-1.0.0/neuronbridge_python.egg-info/PKG-INFO
--rw-r--r--   0 rokickik (196774796) staff       (20)      365 2022-04-25 21:04:12.000000 neuronbridge-python-1.0.0/neuronbridge_python.egg-info/SOURCES.txt
--rw-r--r--   0 rokickik (196774796) staff       (20)        1 2022-04-25 21:04:11.000000 neuronbridge-python-1.0.0/neuronbridge_python.egg-info/dependency_links.txt
--rw-r--r--   0 rokickik (196774796) staff       (20)       66 2022-04-25 21:04:11.000000 neuronbridge-python-1.0.0/neuronbridge_python.egg-info/requires.txt
--rw-r--r--   0 rokickik (196774796) staff       (20)       13 2022-04-25 21:04:11.000000 neuronbridge-python-1.0.0/neuronbridge_python.egg-info/top_level.txt
--rw-r--r--   0 rokickik (196774796) staff       (20)       38 2022-04-25 21:04:12.419675 neuronbridge-python-1.0.0/setup.cfg
--rw-r--r--   0 rokickik (196774796) staff       (20)     1000 2022-04-25 20:20:14.000000 neuronbridge-python-1.0.0/setup.py
+drwxr-xr-x   0 rokickik   (502) staff       (20)        0 2023-05-18 20:18:34.680687 neuronbridge-python-3.1.1/
+-rw-r--r--   0 rokickik   (502) staff       (20)     1539 2023-05-18 15:22:37.000000 neuronbridge-python-3.1.1/LICENSE.md
+-rw-r--r--   0 rokickik   (502) staff       (20)     2338 2023-05-18 20:18:34.680423 neuronbridge-python-3.1.1/PKG-INFO
+-rw-r--r--   0 rokickik   (502) staff       (20)     1832 2023-05-18 20:13:18.000000 neuronbridge-python-3.1.1/README.md
+drwxr-xr-x   0 rokickik   (502) staff       (20)        0 2023-05-18 20:18:34.678741 neuronbridge-python-3.1.1/neuronbridge/
+-rw-r--r--   0 rokickik   (502) staff       (20)        1 2022-04-11 17:38:47.000000 neuronbridge-python-3.1.1/neuronbridge/__init__.py
+-rw-r--r--   0 rokickik   (502) staff       (20)     6208 2023-05-18 19:25:32.000000 neuronbridge-python-3.1.1/neuronbridge/client.py
+-rwxr-xr-x   0 rokickik   (502) staff       (20)      723 2023-05-18 15:22:37.000000 neuronbridge-python-3.1.1/neuronbridge/generate_schemas.py
+-rw-r--r--   0 rokickik   (502) staff       (20)    11628 2023-05-18 17:32:41.000000 neuronbridge-python-3.1.1/neuronbridge/model.py
+-rw-r--r--   0 rokickik   (502) staff       (20)      854 2023-05-18 18:38:43.000000 neuronbridge-python-3.1.1/neuronbridge/utils.py
+-rwxr-xr-x   0 rokickik   (502) staff       (20)    12325 2023-05-18 15:22:49.000000 neuronbridge-python-3.1.1/neuronbridge/validate_ray.py
+drwxr-xr-x   0 rokickik   (502) staff       (20)        0 2023-05-18 20:18:34.680024 neuronbridge-python-3.1.1/neuronbridge_python.egg-info/
+-rw-r--r--   0 rokickik   (502) staff       (20)     2338 2023-05-18 20:18:34.000000 neuronbridge-python-3.1.1/neuronbridge_python.egg-info/PKG-INFO
+-rw-r--r--   0 rokickik   (502) staff       (20)      397 2023-05-18 20:18:34.000000 neuronbridge-python-3.1.1/neuronbridge_python.egg-info/SOURCES.txt
+-rw-r--r--   0 rokickik   (502) staff       (20)        1 2023-05-18 20:18:34.000000 neuronbridge-python-3.1.1/neuronbridge_python.egg-info/dependency_links.txt
+-rw-r--r--   0 rokickik   (502) staff       (20)      150 2023-05-18 20:18:34.000000 neuronbridge-python-3.1.1/neuronbridge_python.egg-info/requires.txt
+-rw-r--r--   0 rokickik   (502) staff       (20)       13 2023-05-18 20:18:34.000000 neuronbridge-python-3.1.1/neuronbridge_python.egg-info/top_level.txt
+-rw-r--r--   0 rokickik   (502) staff       (20)       38 2023-05-18 20:18:34.680783 neuronbridge-python-3.1.1/setup.cfg
+-rw-r--r--   0 rokickik   (502) staff       (20)     1000 2023-05-18 20:16:31.000000 neuronbridge-python-3.1.1/setup.py
```

### Comparing `neuronbridge-python-1.0.0/LICENSE` & `neuronbridge-python-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neuronbridge-python-1.0.0/PKG-INFO` & `neuronbridge-python-3.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,37 @@
-Metadata-Version: 2.1
-Name: neuronbridge-python
-Version: 1.0.0
-Summary: Python API for NeuronBridge
-Home-page: https://github.com/JaneliaSciComp/neuronbridge-python/
-Author: Konrad Rokicki
-Author-email: rokickik@janelia.hhmi.org
-License: BSD 3-Clause
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# NeuronBridge Python API
 
-# neuronbridge-python
+[![DOI](https://zenodo.org/badge/479832149.svg)](https://zenodo.org/badge/latestdoi/479832149)
 
 A Python API for the [NeuronBridge](https://github.com/JaneliaSciComp/neuronbridge) neuron similarity search service.
 
 See [this notebook](notebooks/python_api_examples.ipynb) for usage examples.
 
+![Data Model Diagram](model_diagram.png)
+
+
 ## Development Notes
 
 Create a conda env with all the dependencies including Jupyter:
 
     conda env create -f environment.yml
     conda activate neuronbridge-python
 
+Then install it as a Jupyter kernel:
+    
+    python -m ipykernel install --user --name=neuronbridge-python
+
 
 ### Install for development
 
 You can install the module for development like this:
 
     conda create --name neuronbridge-python python=3.8
     conda activate neuronbridge-python
-    python setup.py develop
+    pip install -e .
 
 
 ### Useful shell commands
 
 To update conda_requirements.txt:
 
     conda env export --from-history --file conda_requirements.txt
@@ -65,8 +58,16 @@
     python setup.py sdist bdist_wheel
 
 4) Upload to PyPI:
 
     twine upload dist/*
 
 
+### Running validation using Ray
+
+You can run validation multithreaded on a single machine like this:
+
+    ./neuronbridge/validate_ray.py
+
+To run the validation script in a distributed manner on the Janelia cluster, you must first install [ray-janelia](https://github.com/JaneliaSciComp/ray-janelia) in a sister directory to where this code base is cloned. Then run a script to bsub the Ray cluster:
 
+    ./scripts/launch_validation.sh
```

### Comparing `neuronbridge-python-1.0.0/neuronbridge/client.py` & `neuronbridge-python-3.1.1/neuronbridge/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         When the client is created, it retrieves the configuration for the specified version. 
         If ``version='current'`` then the latest version is first retrieved from NeuronBridge.
         
         Args:
             data_bucket:
                 name of the S3 bucket containing the NeuronBridge metadata
             version:
-                version number (e.g. "v2.4.0") or "current" to use the latest version
+                version number (e.g. "v3.0.0") or "current" to use the latest version
                 
         """
 
         data_url_prefix = f"https://{data_bucket}.s3.us-east-1.amazonaws.com"
 
         if version == "current":
             url = data_url_prefix + "/current.txt"
@@ -31,29 +31,66 @@
             
         self.data_url = f"{data_url_prefix}/{self.version}"
         url = self.data_url + "/config.json"
         res = requests.get(url)
         if res.status_code != 200:
             raise Exception("Could not retrieve "+url)
 
-        self.config = res.json()
+        self.config = DataConfig(**res.json())
 
 
+    def _get_image(self, url):
+        """
+        Fetches and opens the image at the given URL.
+        """
+        res = requests.get(url, stream=True)
+
+        if res.status_code != 200:
+            raise Exception("Could not retrieve "+url)
+
+        return Image.open(res.raw)
+
+
+    def _get_files_url(self, files : Files, file_key : str) -> str:
+        """
+        Returns the full URL to the given file.
+        """
+        store = files.store
+        prefixes = self.config.stores[store].prefixes
+        prefix = prefixes[file_key]
+        if not prefix: raise Exception("Config has no prefix for file type '"+file_key+"'")
+        path = getattr(files, file_key)
+        if not path: return None
+        return prefix + path
+
+
+    def _get_match_url(self, match : Union[NeuronImage, CDSMatch], file_key : str) -> str:
+        """
+        Returns the full URL to the given file, checking both the match files and image files.
+        In case of the file type being in both places, the match file is returned.
+        """
+        url = self._get_files_url(match.files, file_key)
+        if url: return url
+        url = self._get_files_url(match.image.files, file_key)
+        if url: return url
+        raise Exception("Match contains no file with type '"+file_key+"'")
+    
+
     def get_em_image(self, body_id) -> EMImage:
         """
         Returns the EMImage for the specified body ID.
         """
         
         url = f"{self.data_url}/metadata/by_body/{body_id}.json"
         res = requests.get(url)
 
         if res.status_code != 200:
             raise Exception("Could not retrieve "+url)
 
-        images = EMImageLookup(**res.json()).results
+        images = ImageLookup(**res.json()).results
         if not images: return None
         return images[0]
 
     
     def get_lm_images(self, line_id) -> List[LMImage]:
         """
         Returns the LMImages for the specified line ID.
@@ -61,109 +98,96 @@
         
         url = f"{self.data_url}/metadata/by_line/{line_id}.json"
         res = requests.get(url)
 
         if res.status_code != 200:
             raise Exception("Could not retrieve "+url)
 
-        return LMImageLookup(**res.json()).results
+        return ImageLookup(**res.json()).results
 
     
     def get_cds_matches(self, neuron_image : NeuronImage) -> List[CDSMatch]:
         """
         Returns the CDS matches for the specified neuron image (i.e. LMImage or EMImage).
         """
 
-        url = f"{self.data_url}/metadata/cdsresults/{neuron_image.id}.json"
+        url = self._get_files_url(neuron_image.files, 'CDSResults')
         res = requests.get(url)
 
         if res.status_code != 200:
             raise Exception("Could not retrieve "+url)
 
-        cds_matches = CDSMatches(**res.json())
+        cds_matches = PrecomputedMatches(**res.json())
         results = cds_matches.results
 
-        # TODO: this is a hack to get around the fact that PPP imagery is stored under the mask library name
-        for result in results:
-            result.maskLibraryName = cds_matches.maskLibraryName
         return results
     
     
     def get_ppp_matches(self, em_image : EMImage) -> List[PPPMatch]:
         """
         Returns the PPPM matches for the specified EMImage.
         """
-
-        url = f"{self.data_url}/metadata/pppresults/{em_image.publishedName}.json"
+        url = self._get_files_url(em_image.files, 'PPPMResults')
         res = requests.get(url)
 
         if res.status_code != 200:
             raise Exception("Could not retrieve "+url)
 
-        ppp_matches = PPPMatches(**res.json())
+        ppp_matches = PrecomputedMatches(**res.json())
         results = ppp_matches.results
 
-        # TODO: this is a hack to get around the fact that PPP imagery is stored under the mask library name
-        for result in results:
-            result.maskLibraryName = ppp_matches.maskLibraryName
         return results
 
-    def _get_image(self, url):
-
-        res = requests.get(url, stream=True)
-
-        if res.status_code != 200:
-            raise Exception("Could not retrieve "+url)
-
-        return Image.open(res.raw)
-
 
     def get_cds_image(self, match : Union[NeuronImage, CDSMatch], thumbnail=False) -> Image:
         """
         Returns the representative PNG image for the specified CDSMatch or NeuronImage.
         """
-
         if thumbnail:
-            url = self.config['thumbnailsBaseURLs'] + "/" + match.thumbnailURL
+            url = self._get_match_url(match, 'CDMThumbnail')
         else:
-            url = self.config['imageryBaseURL'] + "/" + match.imageURL
+            url = self._get_match_url(match, 'CDM')
         return self._get_image(url)
 
 
     def get_target_searchable_image(self, match : CDSMatch) -> Image:
         """
         Returns the target image for the specified CDSMatch.
         """
-        url = f"{self.config['imageryBaseURL']}/{match.alignmentSpace}/{match.maskLibraryName.replace(' ','_')}/searchable_neurons/pngs/{match.sourceSearchablePNG}"
+        store = match.files.store
+        url = self._get_match_url(match, 'CDMInput')
         return self._get_image(url)
 
 
     def get_match_searchable_image(self, match : CDSMatch) -> Image:
         """
         Returns the matched image for the specified CDSMatch.
         """
-
-        url = f"{self.config['imageryBaseURL']}/{match.alignmentSpace}/{match.libraryName.replace(' ','_')}/searchable_neurons/pngs/{match.searchablePNG}"
+        url = self._get_match_url(match, 'CDMMatch')
         return self._get_image(url)
 
 
-    def get_ppp_image(self, match : PPPMatch) -> Image:
+    def get_ppp_image(self, match : PPPMatch, thumbnail=False) -> Image:
         """
         Returns the representative PNG image for the specified PPPMatch.
         """
-        url = f"{self.config['pppImageryBaseURL']}/{match.alignmentSpace}/{match.maskLibraryName}/{match.files.ColorDepthMip}"
+        if thumbnail:
+            url = self._get_match_url(match, 'CDMBestThumbnail')
+        else:
+            url = self._get_match_url(match, 'CDMBest')
         return self._get_image(url)
 
 
     def get_swc_skeleton(self, match : PPPMatch) -> Image:
         """
         Returns the SWC skeleton for the specified PPPMatch.
         """
-        url = f"{self.config['swcBaseURL']}/{match.publishedName}.swc"
+        url = self._get_match_url(match, 'AlignedBodySWC')
         return self._get_image(url)
 
 
     def get_image_stack(self, match : Match) -> Image:
         """
         Returns the LM image stack for the specified Match.
         """
-        return self._get_image(match.imageStack)
+        url = self._get_match_url(match, 'VisuallyLosslessStack')
+        return self._get_image(url)
```

### Comparing `neuronbridge-python-1.0.0/neuronbridge_python.egg-info/PKG-INFO` & `neuronbridge-python-3.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 Metadata-Version: 2.1
 Name: neuronbridge-python
-Version: 1.0.0
+Version: 3.1.1
 Summary: Python API for NeuronBridge
 Home-page: https://github.com/JaneliaSciComp/neuronbridge-python/
 Author: Konrad Rokicki
 Author-email: rokickik@janelia.hhmi.org
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 
-# neuronbridge-python
+# NeuronBridge Python API
+
+[![DOI](https://zenodo.org/badge/479832149.svg)](https://zenodo.org/badge/latestdoi/479832149)
 
 A Python API for the [NeuronBridge](https://github.com/JaneliaSciComp/neuronbridge) neuron similarity search service.
 
 See [this notebook](notebooks/python_api_examples.ipynb) for usage examples.
 
+![Data Model Diagram](model_diagram.png)
+
+
 ## Development Notes
 
 Create a conda env with all the dependencies including Jupyter:
 
     conda env create -f environment.yml
     conda activate neuronbridge-python
 
+Then install it as a Jupyter kernel:
+    
+    python -m ipykernel install --user --name=neuronbridge-python
+
 
 ### Install for development
 
 You can install the module for development like this:
 
     conda create --name neuronbridge-python python=3.8
     conda activate neuronbridge-python
-    python setup.py develop
+    pip install -e .
 
 
 ### Useful shell commands
 
 To update conda_requirements.txt:
 
     conda env export --from-history --file conda_requirements.txt
@@ -65,8 +74,18 @@
     python setup.py sdist bdist_wheel
 
 4) Upload to PyPI:
 
     twine upload dist/*
 
 
+### Running validation using Ray
+
+You can run validation multithreaded on a single machine like this:
+
+    ./neuronbridge/validate_ray.py
+
+To run the validation script in a distributed manner on the Janelia cluster, you must first install [ray-janelia](https://github.com/JaneliaSciComp/ray-janelia) in a sister directory to where this code base is cloned. Then run a script to bsub the Ray cluster:
+
+    ./scripts/launch_validation.sh
+
```

### Comparing `neuronbridge-python-1.0.0/setup.py` & `neuronbridge-python-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     requirements = [l for l in requirements if not l.strip().startswith('#')]
 
 setup(
     name='neuronbridge-python',
     packages=find_packages(),
-    version='1.0.0',
+    version='3.1.1',
     description='Python API for NeuronBridge',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Konrad Rokicki',
     author_email='rokickik@janelia.hhmi.org',
     url='https://github.com/JaneliaSciComp/neuronbridge-python/',
     license='BSD 3-Clause',
```

