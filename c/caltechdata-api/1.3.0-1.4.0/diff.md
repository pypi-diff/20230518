# Comparing `tmp/caltechdata_api-1.3.0.tar.gz` & `tmp/caltechdata_api-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caltechdata_api-1.3.0.tar", last modified: Thu Apr  6 20:22:20 2023, max compression
+gzip compressed data, was "caltechdata_api-1.4.0.tar", last modified: Wed May 17 22:51:50 2023, max compression
```

## Comparing `caltechdata_api-1.3.0.tar` & `caltechdata_api-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-04-06 20:22:20.368445 caltechdata_api-1.3.0/
--rw-r--r--   0 tmorrell   (502) staff       (20)     1523 2017-11-22 17:15:19.000000 caltechdata_api-1.3.0/LICENSE
--rw-r--r--   0 tmorrell   (502) staff       (20)     2514 2023-04-06 20:22:20.367644 caltechdata_api-1.3.0/PKG-INFO
--rw-r--r--   0 tmorrell   (502) staff       (20)     1825 2022-12-06 00:24:56.000000 caltechdata_api-1.3.0/README.md
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-04-06 20:22:20.308954 caltechdata_api-1.3.0/caltechdata_api/
--rw-r--r--   0 tmorrell   (502) staff       (20)      400 2022-12-01 21:58:52.000000 caltechdata_api-1.3.0/caltechdata_api/__init__.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     7836 2023-04-06 20:14:53.000000 caltechdata_api-1.3.0/caltechdata_api/caltechdata_edit.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     8067 2023-04-06 20:14:53.000000 caltechdata_api-1.3.0/caltechdata_api/caltechdata_write.py
--rw-r--r--   0 tmorrell   (502) staff       (20)    15796 2023-04-06 20:14:53.000000 caltechdata_api-1.3.0/caltechdata_api/customize_schema.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     1983 2022-10-28 23:31:55.000000 caltechdata_api-1.3.0/caltechdata_api/download_file.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     1981 2021-09-03 16:50:58.000000 caltechdata_api-1.3.0/caltechdata_api/get_files.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     2489 2022-10-28 18:19:39.000000 caltechdata_api-1.3.0/caltechdata_api/get_metadata.py
--rw-r--r--   0 tmorrell   (502) staff       (20)     2742 2022-12-06 16:41:11.000000 caltechdata_api-1.3.0/caltechdata_api/utils.py
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-04-06 20:22:20.366581 caltechdata_api-1.3.0/caltechdata_api/vocabularies/
--rw-r--r--   0 tmorrell   (502) staff       (20)      794 2021-09-15 17:27:24.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies/date_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)      497 2021-09-15 17:27:24.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies/description_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)     1396 2022-12-06 16:41:11.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies/identifier_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)    51301 2021-09-15 17:27:24.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies/licenses.csv
--rw-r--r--   0 tmorrell   (502) staff       (20)     2682 2021-09-15 17:27:24.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies/relation_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)    16372 2022-11-18 19:12:39.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies/resource_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)     1815 2021-09-15 17:27:24.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies/roles.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)      332 2021-09-15 17:27:24.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies/title_types.yaml
--rw-r--r--   0 tmorrell   (502) staff       (20)      601 2021-09-21 20:43:40.000000 caltechdata_api-1.3.0/caltechdata_api/vocabularies.yaml
-drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-04-06 20:22:20.349155 caltechdata_api-1.3.0/caltechdata_api.egg-info/
--rw-r--r--   0 tmorrell   (502) staff       (20)     2514 2023-04-06 20:22:19.000000 caltechdata_api-1.3.0/caltechdata_api.egg-info/PKG-INFO
--rw-r--r--   0 tmorrell   (502) staff       (20)      884 2023-04-06 20:22:19.000000 caltechdata_api-1.3.0/caltechdata_api.egg-info/SOURCES.txt
--rw-r--r--   0 tmorrell   (502) staff       (20)        1 2023-04-06 20:22:19.000000 caltechdata_api-1.3.0/caltechdata_api.egg-info/dependency_links.txt
--rw-r--r--   0 tmorrell   (502) staff       (20)       49 2023-04-06 20:22:19.000000 caltechdata_api-1.3.0/caltechdata_api.egg-info/requires.txt
--rw-r--r--   0 tmorrell   (502) staff       (20)       16 2023-04-06 20:22:19.000000 caltechdata_api-1.3.0/caltechdata_api.egg-info/top_level.txt
--rw-r--r--   0 tmorrell   (502) staff       (20)       38 2023-04-06 20:22:20.368563 caltechdata_api-1.3.0/setup.cfg
--rwxr-xr-x   0 tmorrell   (502) staff       (20)     4595 2023-04-06 20:14:24.000000 caltechdata_api-1.3.0/setup.py
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-05-17 22:51:50.946769 caltechdata_api-1.4.0/
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1523 2017-11-22 17:15:19.000000 caltechdata_api-1.4.0/LICENSE
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2514 2023-05-17 22:51:50.945053 caltechdata_api-1.4.0/PKG-INFO
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1825 2022-12-06 00:24:56.000000 caltechdata_api-1.4.0/README.md
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-05-17 22:51:50.863161 caltechdata_api-1.4.0/caltechdata_api/
+-rw-r--r--   0 tmorrell   (502) staff       (20)      400 2022-12-01 21:58:52.000000 caltechdata_api-1.4.0/caltechdata_api/__init__.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     8007 2023-05-12 23:45:34.000000 caltechdata_api-1.4.0/caltechdata_api/caltechdata_edit.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     9094 2023-05-15 19:12:43.000000 caltechdata_api-1.4.0/caltechdata_api/caltechdata_write.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)    15913 2023-05-02 22:03:31.000000 caltechdata_api-1.4.0/caltechdata_api/customize_schema.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1983 2022-10-28 23:31:55.000000 caltechdata_api-1.4.0/caltechdata_api/download_file.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1304 2023-05-08 16:21:06.000000 caltechdata_api-1.4.0/caltechdata_api/get_files.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2489 2022-10-28 18:19:39.000000 caltechdata_api-1.4.0/caltechdata_api/get_metadata.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2742 2022-12-06 16:41:11.000000 caltechdata_api-1.4.0/caltechdata_api/utils.py
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-05-17 22:51:50.919555 caltechdata_api-1.4.0/caltechdata_api/vocabularies/
+-rw-r--r--   0 tmorrell   (502) staff       (20)      794 2021-09-15 17:27:24.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies/date_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)      614 2023-05-11 18:15:35.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies/description_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1396 2022-12-06 16:41:11.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies/identifier_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)    51301 2021-09-15 17:27:24.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies/licenses.csv
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2682 2021-09-15 17:27:24.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies/relation_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)    16372 2022-11-18 19:12:39.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies/resource_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1815 2021-09-15 17:27:24.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies/roles.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)      332 2021-09-15 17:27:24.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies/title_types.yaml
+-rw-r--r--   0 tmorrell   (502) staff       (20)      601 2021-09-21 20:43:40.000000 caltechdata_api-1.4.0/caltechdata_api/vocabularies.yaml
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-05-17 22:51:50.899416 caltechdata_api-1.4.0/caltechdata_api.egg-info/
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2514 2023-05-17 22:51:50.000000 caltechdata_api-1.4.0/caltechdata_api.egg-info/PKG-INFO
+-rw-r--r--   0 tmorrell   (502) staff       (20)      950 2023-05-17 22:51:50.000000 caltechdata_api-1.4.0/caltechdata_api.egg-info/SOURCES.txt
+-rw-r--r--   0 tmorrell   (502) staff       (20)        1 2023-05-17 22:51:50.000000 caltechdata_api-1.4.0/caltechdata_api.egg-info/dependency_links.txt
+-rw-r--r--   0 tmorrell   (502) staff       (20)       49 2023-05-17 22:51:50.000000 caltechdata_api-1.4.0/caltechdata_api.egg-info/requires.txt
+-rw-r--r--   0 tmorrell   (502) staff       (20)       16 2023-05-17 22:51:50.000000 caltechdata_api-1.4.0/caltechdata_api.egg-info/top_level.txt
+-rw-r--r--   0 tmorrell   (502) staff       (20)       38 2023-05-17 22:51:50.946905 caltechdata_api-1.4.0/setup.cfg
+-rwxr-xr-x   0 tmorrell   (502) staff       (20)     4595 2023-04-06 20:14:24.000000 caltechdata_api-1.4.0/setup.py
+drwxr-xr-x   0 tmorrell   (502) staff       (20)        0 2023-05-17 22:51:50.941631 caltechdata_api-1.4.0/tests/
+-rw-r--r--   0 tmorrell   (502) staff       (20)     2046 2021-05-26 23:04:00.000000 caltechdata_api-1.4.0/tests/test_conversion.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)      818 2021-09-28 21:03:28.000000 caltechdata_api-1.4.0/tests/test_download.py
+-rw-r--r--   0 tmorrell   (502) staff       (20)     1668 2021-10-07 20:58:02.000000 caltechdata_api-1.4.0/tests/test_rdm.py
```

### Comparing `caltechdata_api-1.3.0/LICENSE` & `caltechdata_api-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/PKG-INFO` & `caltechdata_api-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltechdata_api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python wrapper for CaltechDATA API.
 Home-page: https://github.com/caltechlibrary/caltechdata_api
 Author: Thomas E Morrell
 Author-email: tmorrell@caltech.edu
 License: https://data.caltech.edu/license
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `caltechdata_api-1.3.0/README.md` & `caltechdata_api-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/caltechdata_edit.py` & `caltechdata_api-1.4.0/caltechdata_api/caltechdata_edit.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,17 @@
     production=False,
     schema="43",
     publish=False,
     file_links=[],
     s3=None,
     community=None,
     new_version=False,
+    file_descriptions=[],
+    s3_link=None,
+    default_preview=None,
 ):
 
     # If no token is provided, get from RDMTOK environment variable
     if not token:
         token = os.environ["RDMTOK"]
 
     # If files is a string - change to single value array
@@ -85,18 +88,22 @@
         else:
             descriptions.append(d)
     # We remove file link descriptions, and re-add below
     metadata["descriptions"] = descriptions
 
     # If user has provided file links as a cli option, we add those
     if file_links:
-        metadata = add_file_links(metadata, file_links)
+        metadata = add_file_links(
+            metadata, file_links, file_descriptions, s3_link=s3_link
+        )
     # Otherwise we add file links found in the mtadata file
     elif ex_file_links:
-        metadata = add_file_links(metadata, ex_file_links)
+        metadata = add_file_links(
+            metadata, ex_file_links, file_descriptions, s3_link=s3_link
+        )
 
     if production == True:
         url = "https://data.caltech.edu"
     else:
         url = "https://data.caltechlibrary.dev"
 
     headers = {
@@ -190,15 +197,18 @@
             "client": "datacite",
         }
     metadata["pids"] = pids
 
     data = customize_schema.customize_schema(copy.deepcopy(metadata), schema=schema)
 
     if files:
-        data["files"] = {"enabled": True}
+        if default_preview:
+            data["files"] = {"enabled": True, "default_preview": default_preview}
+        else:
+            data["files"] = {"enabled": True}
         # Update metadata
         result = requests.put(
             url + "/api/records/" + idv + "/draft",
             headers=headers,
             json=data,
         )
         if result.status_code != 200:
@@ -225,29 +235,26 @@
                 url + "/api/records/" + idv,
                 headers=headers,
             )
             if result.status_code != 200:
                 raise Exception(result.text)
         # We want files to stay the same as the existing record
         data["files"] = existing.json()["files"]
+        if default_preview:
+            data["files"]["default_preview"] = default_preview
         # Update metadata
         result = requests.put(
             url + "/api/records/" + idv + "/draft",
             headers=headers,
             json=data,
         )
         if result.status_code != 200:
             raise Exception(result.text)
 
-    if community:
-        review_link = result.json()["links"]["review"]
-        result = send_to_community(review_link, data, headers, publish, community)
-        doi = result.json()["pids"]["doi"]["identifier"]
-        return doi
-    elif publish:
+    if publish:
         publish_link = f"{url}/api/records/{idv}/draft/actions/publish"
         result = requests.post(publish_link, headers=headers)
         if result.status_code != 202:
             raise Exception(result.text)
         doi = result.json()["pids"]["doi"]["identifier"]
         return doi
     else:
```

### Comparing `caltechdata_api-1.3.0/caltechdata_api/caltechdata_write.py` & `caltechdata_api-1.4.0/caltechdata_api/caltechdata_write.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,23 @@
 from caltechdata_api import customize_schema
 from caltechdata_api.utils import humanbytes
 
 
 def write_files_rdm(files, file_link, headers, f_headers, s3=None):
     f_json = []
     f_list = {}
+    fnames = []
     for f in files:
-        filename = f.split("/")[-1]
+        split = f.split("/")
+        filename = split[-1]
+        if filename in fnames:
+            # We can't have a duplicate filename
+            # Assume that the previous path value makes a unique name
+            filename = f"{split[-2]}-{split[-1]}" 
+        fnames.append(filename)
         f_json.append({"key": filename})
         f_list[filename] = f
     # Now we see if any existing draft files need to be replaced
     result = requests.get(file_link, headers=f_headers)
     if result.status_code == 200:
         ex_files = result.json()["entries"]
         for ex in ex_files:
@@ -33,15 +40,17 @@
     for entry in result.json()["entries"]:
         self = entry["links"]["self"]
         link = entry["links"]["content"]
         commit = entry["links"]["commit"]
         name = entry["key"]
         if name in f_list:
             if s3:
-                infile = s3.open(f_list[name], "rb")
+                print("Downloading", f_list[name])
+                s3.download(f_list[name], name)
+                infile = open(name, "rb")
             else:
                 infile = open(f_list[name], "rb")
             # size = infile.seek(0, 2)
             # infile.seek(0, 0)  # reset at beginning
             result = requests.put(link, headers=f_headers, data=infile)
             if result.status_code != 200:
                 raise Exception(result.text)
@@ -51,33 +60,47 @@
         else:
             # Delete any files not included in this write command
             result = requests.delete(self, headers=f_headers)
             if result.status_code != 204:
                 raise Exception(result.text)
 
 
-def add_file_links(metadata, file_links):
+def add_file_links(
+    metadata, file_links, file_descriptions=[], additional_descriptions="", s3_link=None
+):
     # Currently configured for OSN S3 links
     link_string = ""
     endpoint = "https://renc.osn.xsede.org/"
     s3 = s3fs.S3FileSystem(anon=True, client_kwargs={"endpoint_url": endpoint})
+    index = 0
     for link in file_links:
         file = link.split("/")[-1]
         path = link.split(endpoint)[1]
         size = s3.info(path)["size"]
         size = humanbytes(size)
+        try:
+            desc = file_descriptions[index] + ","
+        except IndexError:
+            desc = ""
         if link_string == "":
-            cleaned = link.strip(file)
-            link_string = f"Files available via S3 at {cleaned}&lt;/p&gt;</p>"
-        link_string += f"""{file} {size} 
+            if s3_link:
+                link_string = f"Files available via S3 at {s3_link}&lt;/p&gt;</p>"
+            else:
+                cleaned = link.strip(file)
+                link_string = f"Files available via S3 at {cleaned}&lt;/p&gt;</p>"
+        link_string += f"""{file}, {desc} {size}  
         <p>&lt;a role="button" class="ui compact mini button" href="{link}"
         &gt; &lt;i class="download icon"&gt;&lt;/i&gt; Download &lt;/a&gt;</p>&lt;/p&gt;</p>
         """
+        index += 1
+    # Tack on any additional descriptions
+    if additional_descriptions != "":
+        link_string += additional_descriptions
 
-    description = {"description": link_string, "descriptionType": "Other"}
+    description = {"description": link_string, "descriptionType": "files"}
     metadata["descriptions"].append(description)
     return metadata
 
 
 def send_to_community(review_link, data, headers, publish, community):
 
     data = {
@@ -118,14 +141,17 @@
     production=False,
     schema="43",
     publish=False,
     file_links=[],
     s3=None,
     community=None,
     authors=False,
+    file_descriptions=[],
+    s3_link=None,
+    default_preview=None,
 ):
     """
     File links are links to files existing in external systems that will
     be added directly in a CaltechDATA record, instead of uploading the file.
 
     S3 is a s3sf object for directly opening files
     """
@@ -134,15 +160,17 @@
         token = os.environ["RDMTOK"]
 
     # If files is a string - change to single value array
     if isinstance(files, str) == True:
         files = [files]
 
     if file_links:
-        metadata = add_file_links(metadata, file_links)
+        metadata = add_file_links(
+            metadata, file_links, file_descriptions, s3_link=s3_link
+        )
 
     # Pull out pid information
     if production == True:
         repo_prefix = "10.22002"
     else:
         repo_prefix = "10.33569"
     pids = {}
@@ -159,14 +187,16 @@
                 doi = identifier["identifier"]
                 prefix = doi.split("/")[0]
             elif identifier["identifierType"] == "oai":
                 pids["oai"] = {
                     "identifier": identifier["identifier"],
                     "provider": "oai",
                 }
+            else:
+                doi = False
         elif "scheme" in identifier:
             # We have RDM internal metadata
             if identifier["scheme"] == "doi":
                 doi = identifier["identifier"]
                 prefix = doi.split("/")[0]
             else:
                 doi = False
@@ -207,20 +237,20 @@
     f_headers = {
         "Authorization": "Bearer %s" % token,
         "Content-type": "application/octet-stream",
     }
 
     if not files:
         data["files"] = {"enabled": False}
-    else:
-        if "README.txt" in files:
-            data["files"] = {"default_preview": "README.txt"}
+    elif default_preview:
+        data["files"] = {"enabled": True, "default_preview": default_preview}
 
-    # Make draft and publish
     print(data)
+
+    # Make draft and publish
     result = requests.post(url + "/api/records", headers=headers, json=data)
     if result.status_code != 201:
         raise Exception(result.text)
     idv = result.json()["id"]
     publish_link = result.json()["links"]["publish"]
 
     if files:
@@ -229,11 +259,11 @@
 
     if community:
         review_link = result.json()["links"]["review"]
         send_to_community(review_link, data, headers, publish, community)
 
     else:
         if publish:
-            result = requests.post(publish_link, headers=headers)
+            result = requests.post(publish_link, json=data, headers=headers)
             if result.status_code != 202:
                 raise Exception(result.text)
     return idv
```

### Comparing `caltechdata_api-1.3.0/caltechdata_api/customize_schema.py` & `caltechdata_api-1.4.0/caltechdata_api/customize_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,17 +208,14 @@
             # If metadata has Submitted date, this gets priority
             if d["dateType"] == "Submitted":
                 json_record["publication_date"] = datev
             # If we have an Issued but not a Submitted date, this is
             # publication date
             elif d["dateType"] == "Issued":
                 json_record["publication_date"] = datev
-            elif d["dateType"] == "Updated":
-                # We now let InvenioRDM handle updated dates
-                print("Skipping updated date")
             else:
                 dtype = d.pop("dateType")
                 d["type"] = {"id": datetypes[dtype]}
                 d["date"] = datev
                 change_label(d, "dateInformation", "description")
                 new.append(d)
         json_record["dates"] = new
@@ -356,27 +353,35 @@
         json_record["funding"] = new
 
     if "publicationYear" in json_record:
         json_record.pop("publicationYear")
     if "schemaVersion" in json_record:
         json_record.pop("schemaVersion")
 
+    # Now prep the final structure
+    final = {}
     # Not technically DataCite, but owner info neded for record transfer
     parent = {}
     if "owners" in json_record:
         parent = {"access": {"owned_by": [{"user": json_record["owners"][0]}]}}
     # Not technically dataset, but transfer community information
     if "community" in json_record:
         com = json_record.pop("community")
         parent["communities"] = {"ids": [com], "default": com}
+    final["parent"] = parent
     # Not technically datacite, but transfer pids information
     if "pids" in json_record:
-        pids = json_record.pop("pids")
+        final["pids"] = json_record.pop("pids")
+    # Not technically datacite, but transfer access information
+    if "access" in json_record:
+        final["access"] = json_record.pop("access")
+    # Now we should just have clear metadata left
+    final["metadata"] = json_record
 
-    return {"metadata": json_record, "pids": pids, "parent": parent}
+    return final
 
 
 if __name__ == "__main__":
     # Read in from file for demo purposes
 
     parser = argparse.ArgumentParser(
         description="customize_schema converts a DataCite 4.3 standard json record\
```

### Comparing `caltechdata_api-1.3.0/caltechdata_api/download_file.py` & `caltechdata_api-1.4.0/caltechdata_api/download_file.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/get_files.py` & `caltechdata_api-1.4.0/caltechdata_api/get_files.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,49 @@
 import argparse
-import csv
-import json
-import os
-
 import requests
-from datacite import schema40, schema43
-
-from caltechdata_api import decustomize_schema
 
 
-def get_files(idv, production=True, output=None):
-    # Returns file block or writes csv file
+def get_files(idv, production=True):
+    # Returns file block
 
     if production == True:
-        api_url = "https://data.caltech.edu/api/record/"
+        api_url = "https://data.caltech.edu/api/records/"
     else:
-        api_url = "https://cd-sandbox.tind.io/api/record/"
+        api_url = "https://data.caltechlibrary.dev/api/records/"
 
-    r = requests.get(api_url + str(idv))
+    r = requests.get(api_url + str(idv) + "/files")
     r_data = r.json()
     if "message" in r_data:
         raise AssertionError(
             "id "
             + str(idv)
             + " expected http status 200, got "
             + str(r.status_code)
             + " "
             + r_data["message"]
         )
-    if not "metadata" in r_data:
-        raise AssertionError("expected as metadata property in response, got " + r_data)
-    metadata = r_data["metadata"]
-
-    files = metadata["electronic_location_and_access"]
-
-    if output:
-        outfile = open(output, "w")
-        writer = csv.writer(outfile)
-        writer.writerow(["file_name", "file_size", "url", "embargo_status"])
-        for filem in files:
-            url = filem["uniform_resource_identifier"]
-            name = filem["electronic_name"][0]
-            writer.writerow([name, filem["file_size"], url, filem["embargo_status"]])
-
-    return files
+    if not "entries" in r_data:
+        raise AssertionError("expected as entries property in response, got " + r_data)
+    return r_data["entries"]
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="get_files queries the caltechDATA (Invenio 3) API\
-    and returns file information in a csv file"
+    and returns file information"
     )
     parser.add_argument(
         "ids",
         metavar="ID",
-        type=int,
+        type=str,
         nargs="+",
         help="The CaltechDATA ID for each record of interest",
     )
     parser.add_argument("-test", dest="production", action="store_false")
-    parser.add_argument("-csv", dest="csv_file")
 
     args = parser.parse_args()
 
     production = args.production
-    csv_file = args.csv_file
 
     for idv in args.ids:
-        metadata = get_files(idv, production, csv_file)
+        metadata = get_files(idv, production)
+        print(metadata)
```

### Comparing `caltechdata_api-1.3.0/caltechdata_api/get_metadata.py` & `caltechdata_api-1.4.0/caltechdata_api/get_metadata.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/utils.py` & `caltechdata_api-1.4.0/caltechdata_api/utils.py`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/vocabularies/date_types.yaml` & `caltechdata_api-1.4.0/caltechdata_api/vocabularies/date_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/vocabularies/identifier_types.yaml` & `caltechdata_api-1.4.0/caltechdata_api/vocabularies/identifier_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/vocabularies/licenses.csv` & `caltechdata_api-1.4.0/caltechdata_api/vocabularies/licenses.csv`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/vocabularies/relation_types.yaml` & `caltechdata_api-1.4.0/caltechdata_api/vocabularies/relation_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/vocabularies/resource_types.yaml` & `caltechdata_api-1.4.0/caltechdata_api/vocabularies/resource_types.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/vocabularies/roles.yaml` & `caltechdata_api-1.4.0/caltechdata_api/vocabularies/roles.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api/vocabularies.yaml` & `caltechdata_api-1.4.0/caltechdata_api/vocabularies.yaml`

 * *Files identical despite different names*

### Comparing `caltechdata_api-1.3.0/caltechdata_api.egg-info/PKG-INFO` & `caltechdata_api-1.4.0/caltechdata_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caltechdata-api
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python wrapper for CaltechDATA API.
 Home-page: https://github.com/caltechlibrary/caltechdata_api
 Author: Thomas E Morrell
 Author-email: tmorrell@caltech.edu
 License: https://data.caltech.edu/license
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `caltechdata_api-1.3.0/caltechdata_api.egg-info/SOURCES.txt` & `caltechdata_api-1.4.0/caltechdata_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,8 +18,11 @@
 caltechdata_api/vocabularies/date_types.yaml
 caltechdata_api/vocabularies/description_types.yaml
 caltechdata_api/vocabularies/identifier_types.yaml
 caltechdata_api/vocabularies/licenses.csv
 caltechdata_api/vocabularies/relation_types.yaml
 caltechdata_api/vocabularies/resource_types.yaml
 caltechdata_api/vocabularies/roles.yaml
-caltechdata_api/vocabularies/title_types.yaml
+caltechdata_api/vocabularies/title_types.yaml
+tests/test_conversion.py
+tests/test_download.py
+tests/test_rdm.py
```

### Comparing `caltechdata_api-1.3.0/setup.py` & `caltechdata_api-1.4.0/setup.py`

 * *Files identical despite different names*

