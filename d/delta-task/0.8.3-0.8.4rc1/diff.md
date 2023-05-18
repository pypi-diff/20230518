# Comparing `tmp/delta-task-0.8.3.tar.gz` & `tmp/delta-task-0.8.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delta-task-0.8.3.tar", last modified: Fri Mar 17 09:45:08 2023, max compression
+gzip compressed data, was "delta-task-0.8.4rc1.tar", last modified: Thu May 18 02:48:43 2023, max compression
```

## Comparing `delta-task-0.8.3.tar` & `delta-task-0.8.4rc1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.303748 delta-task-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-03-17 09:45:08.303748 delta-task-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-03-17 09:44:53.000000 delta-task-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.295748 delta-task-0.8.3/delta/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.295748 delta-task-0.8.3/delta/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.295748 delta-task-0.8.3/delta/core/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/strategy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/strategy/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/strategy/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/strategy/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/strategy/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/strategy/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/core/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.299748 delta-task-0.8.3/delta/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/dataset/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/dataset/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/delta_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.299748 delta-task-0.8.3/delta/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/pandas/op_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    26412 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/pandas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.303748 delta-task-0.8.3/delta/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/serialize/arr.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/serialize/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.303748 delta-task-0.8.3/delta/statsmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/statsmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/statsmodel/logit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/statsmodel/mnlogit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/statsmodel/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.303748 delta-task-0.8.3/delta/task/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/task/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19314 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/task/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-17 09:44:53.000000 delta-task-0.8.3/delta/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:45:08.303748 delta-task-0.8.3/delta_task.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-03-17 09:45:08.000000 delta-task-0.8.3/delta_task.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-17 09:45:08.000000 delta-task-0.8.3/delta_task.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 09:45:08.000000 delta-task-0.8.3/delta_task.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 09:45:08.000000 delta-task-0.8.3/delta_task.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-17 09:45:08.000000 delta-task-0.8.3/delta_task.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 09:45:08.000000 delta-task-0.8.3/delta_task.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-17 09:45:08.303748 delta-task-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-17 09:44:53.000000 delta-task-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.991991 delta-task-0.8.4rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-18 02:48:43.991991 delta-task-0.8.4rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.983991 delta-task-0.8.4rc1/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.983991 delta-task-0.8.4rc1/delta/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.987991 delta-task-0.8.4rc1/delta/core/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/strategy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/strategy/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/strategy/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/strategy/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/strategy/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/strategy/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/core/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.987991 delta-task-0.8.4rc1/delta/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/dataset/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/dataset/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/delta_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.987991 delta-task-0.8.4rc1/delta/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29404 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/pandas/op_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26412 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/pandas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.987991 delta-task-0.8.4rc1/delta/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/serialize/arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/serialize/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.987991 delta-task-0.8.4rc1/delta/statsmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/statsmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/statsmodel/logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/statsmodel/mnlogit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/statsmodel/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.987991 delta-task-0.8.4rc1/delta/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/task/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20945 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/task/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/delta/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:48:43.991991 delta-task-0.8.4rc1/delta_task.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-18 02:48:43.000000 delta-task-0.8.4rc1/delta_task.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-18 02:48:43.000000 delta-task-0.8.4rc1/delta_task.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:48:43.000000 delta-task-0.8.4rc1/delta_task.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:48:43.000000 delta-task-0.8.4rc1/delta_task.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-18 02:48:43.000000 delta-task-0.8.4rc1/delta_task.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 02:48:43.000000 delta-task-0.8.4rc1/delta_task.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 02:48:43.991991 delta-task-0.8.4rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-18 02:48:27.000000 delta-task-0.8.4rc1/setup.py
```

### Comparing `delta-task-0.8.3/PKG-INFO` & `delta-task-0.8.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-task
-Version: 0.8.3
+Version: 0.8.4rc1
 Summary: delta framework
 Home-page: https://github.com/delta-mpc/delta
 Author: miaohong
 Author-email: 73902525@qq.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `delta-task-0.8.3/README.md` & `delta-task-0.8.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/core/strategy/__init__.py` & `delta-task-0.8.4rc1/delta/core/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/core/strategy/analytics.py` & `delta-task-0.8.4rc1/delta/core/strategy/analytics.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/core/strategy/learning.py` & `delta-task-0.8.4rc1/delta/core/strategy/learning.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/core/strategy/merge.py` & `delta-task-0.8.4rc1/delta/core/strategy/merge.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/core/strategy/result.py` & `delta-task-0.8.4rc1/delta/core/strategy/result.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/core/strategy/select.py` & `delta-task-0.8.4rc1/delta/core/strategy/select.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/core/strategy/strategy.py` & `delta-task-0.8.4rc1/delta/core/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/core/task.py` & `delta-task-0.8.4rc1/delta/core/task.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/dataset/dataframe.py` & `delta-task-0.8.4rc1/delta/dataset/dataframe.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/dataset/dataset.py` & `delta-task-0.8.4rc1/delta/dataset/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,16 +27,16 @@
             filename=dataset,
             default=None,
             **kwargs,
         )
 
 
 class FileDataset(TorchDataset):
-    def __init__(self, filename: str) -> None:
-        result = load_file(filename)
+    def __init__(self, filename: str, **kwargs) -> None:
+        result = load_file(filename, **kwargs)
         if isinstance(result, Image.Image):
             raise ValueError("file dataset does not support image file")
         self._result = result
 
     def __getitem__(self, index):
         if isinstance(self._result, pd.DataFrame):
             item = self._result.iloc[index]
@@ -46,17 +46,18 @@
         return item
 
     def __len__(self) -> int:
         return len(self._result)
 
 
 class DirectoryDataset(TorchDataset):
-    def __init__(self, directory: str) -> None:
+    def __init__(self, directory: str, **kwargs) -> None:
         self._xs = []
         self._ys = []
+        self._kwargs = kwargs
         root, dirnames, filenames = next(os.walk(directory))
         if len(filenames) > 0 and len(dirnames) == 0:
             self._xs.extend([os.path.join(root, filename) for filename in filenames])
         elif len(filenames) == 0 and len(dirnames) > 0:
             for dirname in dirnames:
                 sub_root, sub_dirs, sub_files = next(
                     os.walk(os.path.join(root, dirname))
@@ -73,15 +74,15 @@
         else:
             raise ValueError(
                 "directory can only contain files or sub directory that contains file"
             )
 
     def __getitem__(self, index):
         filename = self._xs[index]
-        x = load_file(filename)
+        x = load_file(filename, **self._kwargs)
         y = None
         if len(self._ys) > 0:
             y = self._ys[index]
         if y is not None:
             return x, y
         return x
 
@@ -117,35 +118,35 @@
     left_indices, right_indices = indices[:frac_count], indices[frac_count:]
     return IndexLookUpDataset(left_indices, dataset), IndexLookUpDataset(
         right_indices, dataset
     )
 
 
 def load_dataset(
-    dataset_name: str,
+    dataset_name: str, **kwargs
 ) -> TorchDataset | Tuple[TorchDataset, TorchDataset]:
     if not os.path.exists(dataset_name):
         raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), dataset_name)
     if os.path.isfile(dataset_name):
-        dataset = FileDataset(dataset_name)
+        dataset = FileDataset(dataset_name, **kwargs)
         return dataset
     else:
         train_path = os.path.join(dataset_name, "train")
         val_path = os.path.join(dataset_name, "val")
         if (
             os.path.exists(train_path)
             and os.path.isdir(train_path)
             and os.path.exists(val_path)
             and os.path.isdir(val_path)
         ):
             train_root, _, train_files = next(os.walk(train_path))
             val_root, _, val_files = next(os.walk(val_path))
             if len(train_files) == 1 and len(val_files) == 1:
-                train_dataset = FileDataset(os.path.join(train_root, train_files[0]))
-                val_dataset = FileDataset(os.path.join(val_root, val_files[0]))
+                train_dataset = FileDataset(os.path.join(train_root, train_files[0]), **kwargs)
+                val_dataset = FileDataset(os.path.join(val_root, val_files[0]), **kwargs)
             else:
-                train_dataset = DirectoryDataset(train_path)
-                val_dataset = DirectoryDataset(val_path)
+                train_dataset = DirectoryDataset(train_path, **kwargs)
+                val_dataset = DirectoryDataset(val_path, **kwargs)
             return train_dataset, val_dataset
         else:
-            dataset = DirectoryDataset(dataset_name)
+            dataset = DirectoryDataset(dataset_name, **kwargs)
             return dataset
```

### Comparing `delta-task-0.8.3/delta/dataset/file.py` & `delta-task-0.8.4rc1/delta/dataset/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         result = pd.read_csv(filename, sep=",", **kwargs)
     elif filename.endswith(".tsv") or filename.endswith(".txt"):
         if "sep" in kwargs:
             kwargs.pop("sep")
         result = pd.read_csv(filename, sep=r"\s+", **kwargs)
     elif filename.endswith(".xls") or filename.endswith(".xlsx"):
         result = pd.read_excel(filename, **kwargs)
+    elif filename.endswith(".json"):
+        result = pd.read_json(filename, **kwargs)
     else:
         try:
             result = Image.open(filename, **kwargs)
         except UnidentifiedImageError:
             raise UnsupportedFileError(filename)
     return result
```

### Comparing `delta-task-0.8.3/delta/debug.py` & `delta-task-0.8.4rc1/delta/debug.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/delta_node.py` & `delta-task-0.8.4rc1/delta/delta_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,33 @@
 
 class DeltaNode(object):
     def __init__(self, url: str) -> None:
         self._url = url
 
     def create_task(self, task: Task) -> int:
         url = f"{self._url}/v1/task"
-        with TemporaryFile(mode="w+b") as file:
-            serialize.dump_task(file, task)
-            file.seek(0)
-            resp = httpx.post(url, files={"file": file}, timeout=None)
+        with TemporaryFile(mode="w+b") as task_file, TemporaryFile(mode="w+b") as config_file:
+            task_config = {
+                "name": task.name,
+                "dataset": task.dataset,
+                "type": task.type,
+                "enable_verify": task.enable_verify,
+                "options": task.options
+            }
+            pickle.dump(task_config, config_file)
+            config_file.seek(0)
+
+            serialize.dump_task(task_file, task)
+            task_file.seek(0)
+            files = {
+                "file": ("task_file.pkl", task_file, "application/octet-stream"),
+                "config": ("task_config_file.pkl", config_file, "application/pickle")
+            }
+
+            resp = httpx.post(url, files=files, timeout=None)
             resp.raise_for_status()
             data = resp.json()
             task_id = data["task_id"]
             return task_id
 
     def wait(self, task_id: int) -> bool:
         url = f"{self._url}/v1/task/metadata"
```

### Comparing `delta-task-0.8.3/delta/pandas/dataframe.py` & `delta-task-0.8.4rc1/delta/pandas/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 map_op.outputs.append(output)
             output.src = map_op
 
         return output
 
     def _dispatch_binary_op(
         self,
-        other: "DataFrame" | "Series" | List[float] | float,
+        other: "DataFrame | Series | List[float] | float",
         op_name: str,
         op: Callable[..., Any],
         **kwargs: Any,
     ) -> "DataFrame":
         if not isinstance(other, GraphNode):
             other_node = InputGraphNode(default=other, location=DataLocation.SERVER)
         else:
```

### Comparing `delta-task-0.8.3/delta/pandas/op_mixin.py` & `delta-task-0.8.4rc1/delta/pandas/op_mixin.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/pandas/series.py` & `delta-task-0.8.4rc1/delta/pandas/series.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/serialize/arr.py` & `delta-task-0.8.4rc1/delta/serialize/arr.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/serialize/task.py` & `delta-task-0.8.4rc1/delta/serialize/task.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/statsmodel/logit.py` & `delta-task-0.8.4rc1/delta/statsmodel/logit.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/statsmodel/mnlogit.py` & `delta-task-0.8.4rc1/delta/statsmodel/mnlogit.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/statsmodel/optimizer.py` & `delta-task-0.8.4rc1/delta/statsmodel/optimizer.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/task/analytics.py` & `delta-task-0.8.4rc1/delta/task/analytics.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta/task/learning.py` & `delta-task-0.8.4rc1/delta/task/learning.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,35 +117,63 @@
         iteration: int,
         strategy: LearningStrategy,
     ) -> None:
         self.dataloader = dataloader
         self.epoch = epoch
         self.iteration = iteration
         self.strategy = strategy
+        self.batch_sampler = None
 
     def __iter__(self):
         return self._get_iter()
 
+    def _make_dataloader(self) -> DataLoader:
+        if self.batch_sampler is None:
+            return self.dataloader
+        else:
+            return DataLoader(
+                dataset=self.dataloader.dataset,
+                batch_sampler=self.batch_sampler,
+                num_workers=self.dataloader.num_workers,
+                collate_fn=self.dataloader.collate_fn,
+                pin_memory=self.dataloader.pin_memory,
+                timeout=self.dataloader.timeout,
+                worker_init_fn=self.dataloader.worker_init_fn,
+                multiprocessing_context=self.dataloader.multiprocessing_context,
+                generator=self.dataloader.generator,
+                prefetch_factor=self.dataloader.prefetch_factor,
+                persistent_workers=self.dataloader.persistent_workers,
+                pin_memory_device=self.dataloader.pin_memory_device,
+            )
+
     def _get_iter(self):
         finished = False
 
         while not finished:
-            for batch in self.dataloader:
+            count = 0
+            dataloader = self._make_dataloader()
+            for batch in dataloader:
                 if finished:
                     break
 
                 _logger.info(f"Training epoch {self.epoch} iteration {self.iteration}")
 
                 yield batch
-
+                
+                count += 1
                 if self.strategy.should_merge(self.epoch, self.iteration, False):
                     _logger.info(f"iteration {self.iteration}, start to merge")
+                    assert dataloader.batch_sampler is not None
+                    if self.batch_sampler is None:
+                        self.batch_sampler = list(dataloader.batch_sampler)
+                    self.batch_sampler = self.batch_sampler[count:]
                     finished = True
                 self.iteration += 1
-
+            
+            self.batch_sampler = None
             if self.strategy.should_merge(self.epoch, self.iteration, True):
                 _logger.info(f"epoch {self.epoch}, start to merge")
                 finished = True
             if (self.iteration - 1) % len(self.dataloader) == 0:
                 self.epoch += 1
 
 
@@ -368,17 +396,22 @@
             def map(
                 self,
                 dataloader: DataLoader,
                 weight: np.ndarray,
                 epoch: int,
                 iteration: int,
             ) -> Tuple[Dict[str, np.ndarray], int, int]:
-                self.learning.strategy.weight_to_params(
-                    weight, self.learning.state_dict()
-                )
+                if len(weight) > 0:
+                    self.learning.strategy.weight_to_params(
+                        weight, self.learning.state_dict()
+                    )
+                else:
+                    weight = self.learning.strategy.params_to_weight(
+                        self.learning.state_dict()
+                    )
                 _logger.info(f"Round {self.round} training")
                 train_iter = TrainIterator(
                     dataloader, epoch, iteration, self.learning.strategy
                 )
                 self.learning.train(train_iter)
                 _logger.info(f"Round {self.round} training complete")
                 params = self.learning.state_dict()
@@ -513,15 +546,18 @@
                 self,
                 weight: np.ndarray,
                 metrics: Dict[str, np.ndarray | float] | None = None,
             ) -> Any:
                 self.learning.strategy.weight_to_params(
                     weight, self.learning.state_dict()
                 )
-                return self.learning.state_dict()
+                res: Dict[str, Any] = {"weight": self.learning.state_dict()}
+                if metrics is not None:
+                    res["metrics"] = metrics
+                return res
 
         input_nodes: List[DataNode] = [weight_node]
         if metrics_node is not None:
             input_nodes.append(metrics_node)
 
         result_op = _ResultOp(
             name="result", inputs=input_nodes, outputs=[result_node], learning=self
@@ -537,17 +573,16 @@
 
         epoch_node = InputGraphNode(
             name="epoch", location=DataLocation.CLIENT, default=1
         )
         iteration_node = InputGraphNode(
             name="iteration", location=DataLocation.CLIENT, default=1
         )
-        weight_arr = self.strategy.params_to_weight(self.state_dict())
         weight_node = InputGraphNode(
-            name="weight_0", location=DataLocation.SERVER, default=weight_arr
+            name="weight_0", location=DataLocation.SERVER, default=np.empty(0)
         )
         metrics_node = None
         inputs = [dataset_node, epoch_node, iteration_node, weight_node]
         for i in range(self.max_rounds):
             train_dataloader_node = dataloader_nodes[0]
             if len(dataloader_nodes) > 1:
                 val_dataloader_node = dataloader_nodes[1]
```

### Comparing `delta-task-0.8.3/delta/task/task.py` & `delta-task-0.8.4rc1/delta/task/task.py`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/delta_task.egg-info/PKG-INFO` & `delta-task-0.8.4rc1/delta_task.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-task
-Version: 0.8.3
+Version: 0.8.4rc1
 Summary: delta framework
 Home-page: https://github.com/delta-mpc/delta
 Author: miaohong
 Author-email: 73902525@qq.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `delta-task-0.8.3/delta_task.egg-info/SOURCES.txt` & `delta-task-0.8.4rc1/delta_task.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delta-task-0.8.3/setup.py` & `delta-task-0.8.4rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,28 +26,28 @@
 
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
 
 setup(
     name="delta-task",
-    version="0.8.3",
+    version="0.8.4rc1",
     license_files=("LICENSE"),
     packages=find_packages(),
     include_package_data=True,
     exclude_package_data={"": [".gitignore"]},
     install_requires=[
-        "cloudpickle==1.6.0",
-        "httpx==0.23.0",
-        "numpy==1.22.0",
-        "Pillow==9.1.1",
-        "pandas==1.2.3",
-        "pytest==6.2.5",
-        "torch==1.8.2+cpu",
-        "networkx==2.7.1"
+        "cloudpickle>=1.6.0",
+        "httpx>=0.23.0",
+        "numpy>=1.22.0",
+        "Pillow>=9.1.1",
+        "pandas>=1.2.3",
+        "pytest>=6.2.5",
+        "torch>=1.8.2",
+        "networkx>=2.7.1"
     ],
     tests_require=["pytest"],
     cmdclass={"test": PyTest},
     test_suite="tests",
     zip_safe=False,
     author="miaohong",
     author_email="73902525@qq.com",
```

