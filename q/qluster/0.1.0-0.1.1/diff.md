# Comparing `tmp/qluster-0.1.0.tar.gz` & `tmp/qluster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qluster-0.1.0.tar", last modified: Tue May  2 17:09:40 2023, max compression
+gzip compressed data, was "qluster-0.1.1.tar", last modified: Thu May 18 02:08:38 2023, max compression
```

## Comparing `qluster-0.1.0.tar` & `qluster-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-02 17:09:40.525324 qluster-0.1.0/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2023-02-23 15:50:36.000000 qluster-0.1.0/LICENSE
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      528 2023-05-02 17:09:40.525324 qluster-0.1.0/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      258 2023-04-07 00:27:06.000000 qluster-0.1.0/README.md
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-02 17:09:40.525324 qluster-0.1.0/qluster/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       23 2023-04-30 14:02:45.000000 qluster-0.1.0/qluster/__init__.py
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     5428 2023-04-30 14:31:14.000000 qluster-0.1.0/qluster/qluster.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-02 17:09:40.525324 qluster-0.1.0/qluster.egg-info/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      528 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      219 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/SOURCES.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/dependency_links.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       40 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/requires.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        8 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/top_level.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-05-02 17:09:40.525324 qluster-0.1.0/setup.cfg
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      640 2023-05-02 17:08:48.000000 qluster-0.1.0/setup.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-18 02:08:38.674212 qluster-0.1.1/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2023-05-18 02:03:06.000000 qluster-0.1.1/LICENSE
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      634 2023-05-18 02:08:38.674212 qluster-0.1.1/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      364 2023-05-18 02:03:06.000000 qluster-0.1.1/README.md
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-18 02:08:38.670212 qluster-0.1.1/qluster/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       23 2023-05-18 02:03:06.000000 qluster-0.1.1/qluster/__init__.py
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     5430 2023-05-18 02:03:06.000000 qluster-0.1.1/qluster/qluster.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-18 02:08:38.670212 qluster-0.1.1/qluster.egg-info/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      634 2023-05-18 02:08:38.000000 qluster-0.1.1/qluster.egg-info/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      219 2023-05-18 02:08:38.000000 qluster-0.1.1/qluster.egg-info/SOURCES.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-05-18 02:08:38.000000 qluster-0.1.1/qluster.egg-info/dependency_links.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       40 2023-05-18 02:08:38.000000 qluster-0.1.1/qluster.egg-info/requires.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        8 2023-05-18 02:08:38.000000 qluster-0.1.1/qluster.egg-info/top_level.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-05-18 02:08:38.674212 qluster-0.1.1/setup.cfg
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      640 2023-05-18 02:03:17.000000 qluster-0.1.1/setup.py
```

### Comparing `qluster-0.1.0/LICENSE` & `qluster-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qluster-0.1.0/PKG-INFO` & `qluster-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qluster
-Version: 0.1.0
+Version: 0.1.1
 Summary: qluster
 Home-page: https://github.com/mdmould/qluster
 Author: Matthew Mould
 Author-email: mattdmould@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # qluster
 
 Quick clusters of merging binary black holes: `pip install qluster`.
 
-Based on [Gerosa and Berti (2019) arXiv:1906.05295](https://arxiv.org/abs/1906.05295) and [Mould, Gerosa, and Taylor (2022) arXiv:2203.03651](https://arxiv.org/abs/2203.03651).
+The code is described in [Gerosa and Mould (2023)](https://arxiv.org/abs/2305.04987). Key results were reported in [Gerosa and Berti (2019) arXiv:1906.05295](https://arxiv.org/abs/1906.05295) and [Mould, Gerosa, and Taylor (2022) arXiv:2203.03651](https://arxiv.org/abs/2203.03651).
```

### Comparing `qluster-0.1.0/qluster/qluster.py` & `qluster-0.1.1/qluster/qluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     return file
 
 
 def cluster(
     vesc,
     n_1g, gamma, mmin, mmax, chimin, chimax,
     alpha, beta,
-    file='./cluster.h5'
+    file='./cluster.h5',
     seed=None,
     ):
 
     file = check_file(file)
 
     np.random.seed(seed)
 
@@ -141,15 +141,15 @@
     n_clusters, delta, vescmin, vescmax,
     n_1g, gamma, mmin, mmax, chimin, chimax,
     alpha, beta,
     file='./cluster.h5',
     seed=None,
     n_cpus=1,
     group_clusters=True,
-    keep_clusters=False
+    keep_clusters=False,
     ):
 
     file = check_file(file)
     
     np.random.seed(seed)
 
     print('Clusters')
```

### Comparing `qluster-0.1.0/qluster.egg-info/PKG-INFO` & `qluster-0.1.1/qluster.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qluster
-Version: 0.1.0
+Version: 0.1.1
 Summary: qluster
 Home-page: https://github.com/mdmould/qluster
 Author: Matthew Mould
 Author-email: mattdmould@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # qluster
 
 Quick clusters of merging binary black holes: `pip install qluster`.
 
-Based on [Gerosa and Berti (2019) arXiv:1906.05295](https://arxiv.org/abs/1906.05295) and [Mould, Gerosa, and Taylor (2022) arXiv:2203.03651](https://arxiv.org/abs/2203.03651).
+The code is described in [Gerosa and Mould (2023)](https://arxiv.org/abs/2305.04987). Key results were reported in [Gerosa and Berti (2019) arXiv:1906.05295](https://arxiv.org/abs/1906.05295) and [Mould, Gerosa, and Taylor (2022) arXiv:2203.03651](https://arxiv.org/abs/2203.03651).
```

### Comparing `qluster-0.1.0/setup.py` & `qluster-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 name = 'qluster'
-version = '0.1.0'
+version = '0.1.1'
 
 with open('README.md' ,'r') as f:
     long_description = f.read().strip()
 
 setup(
     name=name,
     version=version,
```

