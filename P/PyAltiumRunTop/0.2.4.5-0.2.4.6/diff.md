# Comparing `tmp/PyAltiumRunTop-0.2.4.5.tar.gz` & `tmp/PyAltiumRunTop-0.2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAltiumRunTop-0.2.4.5.tar", last modified: Thu May 11 09:28:37 2023, max compression
+gzip compressed data, was "PyAltiumRunTop-0.2.4.6.tar", last modified: Thu May 18 03:30:27 2023, max compression
```

## Comparing `PyAltiumRunTop-0.2.4.5.tar` & `PyAltiumRunTop-0.2.4.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.789040 PyAltiumRunTop-0.2.4.5/
--rw-rw-rw-   0        0        0     1051 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/LICENSE
--rw-rw-rw-   0        0        0       33 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2801 2023-05-11 09:28:37.789040 PyAltiumRunTop-0.2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     1943 2023-03-08 01:12:55.000000 PyAltiumRunTop-0.2.4.5/README.md
--rw-rw-rw-   0        0        0      819 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/pyproject.toml
--rw-rw-rw-   0        0        0     1228 2023-05-11 09:28:37.790036 PyAltiumRunTop-0.2.4.5/setup.cfg
--rw-rw-rw-   0        0        0       69 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.756127 PyAltiumRunTop-0.2.4.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.760117 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/
--rw-rw-rw-   0        0        0     2672 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      575 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 09:14:50.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       73 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.768095 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/
--rw-rw-rw-   0        0        0    20034 2023-04-16 12:00:32.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRun.py
--rw-rw-rw-   0        0        0    20094 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRun15.py
--rw-rw-rw-   0        0        0    20041 2023-04-16 11:56:03.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunAd.py
--rw-rw-rw-   0        0        0    20149 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunAd15.py
--rw-rw-rw-   0        0        0    23181 2023-05-11 09:28:11.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunEnv.py
--rw-rw-rw-   0        0        0    23191 2023-05-11 09:28:11.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunEnv15.py
--rw-rw-rw-   0        0        0    20045 2023-04-16 12:05:11.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunexe.py
--rw-rw-rw-   0        0        0    20105 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunexe15.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.774079 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/helpers/
--rw-rw-rw-   0        0        0     2415 2023-04-26 07:29:08.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/helpers/AltiumHelper.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/helpers/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.788147 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/
--rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/__init__.py
--rw-rw-rw-   0        0        0      525 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/logger.pas
--rw-rw-rw-   0        0        0      478 2023-02-27 09:06:28.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/main.pas
--rw-rw-rw-   0        0        0     7285 2023-03-06 02:14:13.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas
-drwxrwxrwx   0        0        0        0 2023-05-11 09:28:37.773082 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/
--rw-rw-rw-   0        0        0     2801 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 09:40:41.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       73 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 09:28:37.000000 PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-16 11:51:19.000000 PyAltiumRunTop-0.2.4.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 03:30:27.704899 PyAltiumRunTop-0.2.4.6/
+-rw-rw-rw-   0        0        0     1051 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2801 2023-05-18 03:30:27.704899 PyAltiumRunTop-0.2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1943 2023-03-08 01:12:55.000000 PyAltiumRunTop-0.2.4.6/README.md
+-rw-rw-rw-   0        0        0      819 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1228 2023-05-18 03:30:27.705897 PyAltiumRunTop-0.2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0       69 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 03:30:27.586871 PyAltiumRunTop-0.2.4.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-18 03:30:27.614223 PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/
+-rw-rw-rw-   0        0        0     2672 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      575 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 09:14:50.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       73 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-02-27 09:22:56.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 03:30:27.672882 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/
+-rw-rw-rw-   0        0        0    20034 2023-04-16 12:00:32.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRun.py
+-rw-rw-rw-   0        0        0    20094 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRun15.py
+-rw-rw-rw-   0        0        0    20041 2023-04-16 11:56:03.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunAd.py
+-rw-rw-rw-   0        0        0    20149 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunAd15.py
+-rw-rw-rw-   0        0        0    23197 2023-05-17 09:44:41.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunEnv.py
+-rw-rw-rw-   0        0        0    23207 2023-05-18 03:30:26.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunEnv15.py
+-rw-rw-rw-   0        0        0    20045 2023-04-16 12:05:11.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunexe.py
+-rw-rw-rw-   0        0        0    20105 2023-04-26 07:44:50.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunexe15.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 03:30:27.690187 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/helpers/
+-rw-rw-rw-   0        0        0     2415 2023-04-26 07:29:08.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/helpers/AltiumHelper.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/helpers/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-18 03:30:27.692744 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/scriptingbase/
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/scriptingbase/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-02-27 09:05:47.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/scriptingbase/logger.pas
+-rw-rw-rw-   0        0        0      478 2023-02-27 09:06:28.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/scriptingbase/main.pas
+-rw-rw-rw-   0        0        0     7285 2023-03-06 02:14:13.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas
+drwxrwxrwx   0        0        0        0 2023-05-18 03:30:27.677629 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/
+-rw-rw-rw-   0        0        0     2801 2023-05-18 03:30:27.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-05-18 03:30:27.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 03:30:27.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 09:40:41.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       73 2023-05-18 03:30:27.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-18 03:30:27.000000 PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-16 11:51:19.000000 PyAltiumRunTop-0.2.4.6/src/__init__.py
```

### Comparing `PyAltiumRunTop-0.2.4.5/LICENSE` & `PyAltiumRunTop-0.2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/PKG-INFO` & `PyAltiumRunTop-0.2.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAltiumRunTop
-Version: 0.2.4.5
+Version: 0.2.4.6
 Summary: A library that can run scripts in altium designer
 Home-page: https://github.com/wqh0109663/PyAltiumRun
 Author: Dylan Gybels,wqh0109663
 Author-email: dylangybels@gmail.com,wqh0109663@gmail.com
 License: MIT
 Keywords: Altium,Scripting,Runner
 Platform: win32
```

### Comparing `PyAltiumRunTop-0.2.4.5/README.md` & `PyAltiumRunTop-0.2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/pyproject.toml` & `PyAltiumRunTop-0.2.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/setup.cfg` & `PyAltiumRunTop-0.2.4.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7941 6c74 6975 6d52 756e 546f   = PyAltiumRunTo
 00000020: 700d 0a76 6572 7369 6f6e 203d 2030 2e32  p..version = 0.2
-00000030: 2e34 2e35 0d0a 6465 7363 7269 7074 696f  .4.5..descriptio
+00000030: 2e34 2e36 0d0a 6465 7363 7269 7074 696f  .4.6..descriptio
 00000040: 6e20 3d20 4120 6c69 6272 6172 7920 7468  n = A library th
 00000050: 6174 2063 616e 2072 756e 2073 6372 6970  at can run scrip
 00000060: 7473 2069 6e20 616c 7469 756d 2064 6573  ts in altium des
 00000070: 6967 6e65 720d 0a6c 6f6e 675f 6465 7363  igner..long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 000000a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
```

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/PKG-INFO` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRun.egg-info/SOURCES.txt` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRun.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRun.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRun15.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRun15.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunAd.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunAd.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunAd15.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunAd15.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunEnv.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunEnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,21 +501,21 @@
             if len(text) > 1:
                 text = text[:-2]
             return text + "]"
         print(type(param))
         return None
 
     def _generate_script_from_base(self, name: str, variables: Dict[str, Any] = {}) -> None:
-        origin = 'D:\\adTempPcb\\scriptingbase\\' + name
+        origin = 'D:\\adTemp\\adTempPcb\\scriptingbase\\' + name
         destination = self._project_path + '/' + name
         self._generate_script_from_source(origin, destination, variables)
 
 
     def _generate_script_from_base_top(self, name: str) -> None:
-        origin = 'D:\\adTempPcb\\scriptingbase\\' + name
+        origin = 'D:\\adTemp\\adTempPcb\\scriptingbase\\' + name
         destination = self._project_path + '/' + name
         self._generate_script_from_source_top(origin, destination)
     def _generate_script_from_source_top(self, origin: str, destination: str) -> None:
         f_or = open(origin, 'r')
         f_de = open(destination, 'w')
         line = f_or.readline()
         while line:
```

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunEnv15.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunEnv15.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,21 +501,21 @@
             if len(text) > 1:
                 text = text[:-2]
             return text + "]"
         print(type(param))
         return None
 
     def _generate_script_from_base(self, name: str, variables: Dict[str, Any] = {}) -> None:
-        origin = 'D:\\adTempPcb15\\scriptingbase\\' + name
+        origin = 'D:\\adTemp\\adTempPcb15\\scriptingbase\\' + name
         destination = self._project_path + '/' + name
         self._generate_script_from_source(origin, destination, variables)
 
 
     def _generate_script_from_base_top(self, name: str) -> None:
-        origin = 'D:\\adTempPcb15\\scriptingbase\\' + name
+        origin = 'D:\\adTemp\\adTempPcb15\\scriptingbase\\' + name
         destination = self._project_path + '/' + name
         self._generate_script_from_source_top(origin, destination)
     def _generate_script_from_source_top(self, origin: str, destination: str) -> None:
         f_or = open(origin, 'r')
         f_de = open(destination, 'w')
         line = f_or.readline()
         while line:
```

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunexe.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunexe.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/AltiumRunexe15.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/AltiumRunexe15.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/helpers/AltiumHelper.py` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/helpers/AltiumHelper.py`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/logger.pas` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/scriptingbase/logger.pas`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop/scriptingbase/updateSitNum0302.pas`

 * *Files identical despite different names*

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/PKG-INFO` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAltiumRunTop
-Version: 0.2.4.5
+Version: 0.2.4.6
 Summary: A library that can run scripts in altium designer
 Home-page: https://github.com/wqh0109663/PyAltiumRun
 Author: Dylan Gybels,wqh0109663
 Author-email: dylangybels@gmail.com,wqh0109663@gmail.com
 License: MIT
 Keywords: Altium,Scripting,Runner
 Platform: win32
```

### Comparing `PyAltiumRunTop-0.2.4.5/src/PyAltiumRunTop.egg-info/SOURCES.txt` & `PyAltiumRunTop-0.2.4.6/src/PyAltiumRunTop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

