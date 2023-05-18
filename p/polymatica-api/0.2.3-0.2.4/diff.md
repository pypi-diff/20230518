# Comparing `tmp/polymatica_api-0.2.3.tar.gz` & `tmp/polymatica_api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.2.3.tar", last modified: Tue May 16 16:53:52 2023, max compression
+gzip compressed data, was "polymatica_api-0.2.4.tar", last modified: Thu May 18 08:28:07 2023, max compression
```

## Comparing `polymatica_api-0.2.3.tar` & `polymatica_api-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-16 16:53:52.508423 polymatica_api-0.2.3/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.2.3/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-16 16:53:52.508286 polymatica_api-0.2.3/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      948 2023-05-06 17:31:41.000000 polymatica_api-0.2.3/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-16 16:53:52.507270 polymatica_api-0.2.3/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     3022 2023-05-16 16:53:01.000000 polymatica_api-0.2.3/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.2.3/polymatica_api/data.py
--rw-r--r--   0 leggnom    (501) staff       (20)     5825 2023-05-06 15:46:48.000000 polymatica_api-0.2.3/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)     2674 2023-05-10 18:55:53.000000 polymatica_api-0.2.3/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-16 16:53:52.508081 polymatica_api-0.2.3/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-16 16:53:52.000000 polymatica_api-0.2.3/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-16 16:53:52.000000 polymatica_api-0.2.3/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-16 16:53:52.000000 polymatica_api-0.2.3/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-16 16:53:52.000000 polymatica_api-0.2.3/polymatica_api.egg-info/requires.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-16 16:53:52.000000 polymatica_api-0.2.3/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-16 16:53:52.508461 polymatica_api-0.2.3/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-16 16:51:07.000000 polymatica_api-0.2.3/setup.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-18 08:28:07.728046 polymatica_api-0.2.4/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.2.4/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-18 08:28:07.727870 polymatica_api-0.2.4/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      948 2023-05-06 17:31:41.000000 polymatica_api-0.2.4/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-18 08:28:07.727014 polymatica_api-0.2.4/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     3015 2023-05-18 08:27:17.000000 polymatica_api-0.2.4/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.2.4/polymatica_api/data.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     5825 2023-05-06 15:46:48.000000 polymatica_api-0.2.4/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     2674 2023-05-16 22:27:23.000000 polymatica_api-0.2.4/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-18 08:28:07.727675 polymatica_api-0.2.4/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-18 08:28:07.000000 polymatica_api-0.2.4/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-18 08:28:07.000000 polymatica_api-0.2.4/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-18 08:28:07.000000 polymatica_api-0.2.4/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-18 08:28:07.000000 polymatica_api-0.2.4/polymatica_api.egg-info/requires.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-18 08:28:07.000000 polymatica_api-0.2.4/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-18 08:28:07.728098 polymatica_api-0.2.4/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-18 08:28:02.000000 polymatica_api-0.2.4/setup.py
```

### Comparing `polymatica_api-0.2.3/LICENSE` & `polymatica_api-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.2.3/PKG-INFO` & `polymatica_api-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica_api
-Version: 0.2.3
+Version: 0.2.4
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
```

### Comparing `polymatica_api-0.2.3/README.md` & `polymatica_api-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.2.3/polymatica_api/__init__.py` & `polymatica_api-0.2.4/polymatica_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             "Authorization": token
         }
 
     def from_dataset(self, name) -> DataOption:
         return DataOption(name, self)
 
     def delete_line(self, dataset_id: int, line_id: str):
-        return self._session.delete(self.route('delete_line').format(id=dataset_id, uid=line_id)).json()
+        return self._session.delete(self.route('delete_line').format(id=dataset_id, uid=line_id))
 
     def update_line(self, dataset_id: int, line_id: str, row: typing.Dict):
         return self._session.put(self.route('update_line').format(id=dataset_id, uid=line_id), json=row).json()
 
     def write_line(self, dataset_id: int, row: typing.Dict):
         return self._session.post(self.route('write_line').format(id=dataset_id), json=row).json()
```

### Comparing `polymatica_api-0.2.3/polymatica_api/data_option.py` & `polymatica_api-0.2.4/polymatica_api/data_option.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.2.3/polymatica_api/types.py` & `polymatica_api-0.2.4/polymatica_api/types.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.2.3/polymatica_api.egg-info/PKG-INFO` & `polymatica_api-0.2.4/polymatica_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica-api
-Version: 0.2.3
+Version: 0.2.4
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
```

### Comparing `polymatica_api-0.2.3/setup.py` & `polymatica_api-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     "pydantic==1.10.7",
     "requests==2.29.0"
 ]
 
 setuptools.setup(
     name="polymatica_api",
-    version="0.2.3",
+    version="0.2.4",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.7',
```

