# Comparing `tmp/rapids_singlecell-0.6.2.tar.gz` & `tmp/rapids_singlecell-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids_singlecell-0.6.2.tar", last modified: Wed May 10 13:46:47 2023, max compression
+gzip compressed data, was "rapids_singlecell-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rapids_singlecell-0.6.2.tar` & `rapids_singlecell-0.6.3.tar`

### file list

```diff
@@ -1,40 +1,54 @@
--rw-r--r--   0        0        0     1070 2023-05-04 12:56:41.030096 rapids_singlecell-0.6.2/LICENSE
--rw-r--r--   0        0        0     5989 2023-05-10 12:07:48.871399 rapids_singlecell-0.6.2/README.md
--rw-r--r--   0        0        0      998 2023-05-10 12:34:48.415020 rapids_singlecell-0.6.2/pyproject.toml
--rwxr-xr-x   0        0        0      132 2023-05-04 09:38:07.620767 rapids_singlecell-0.6.2/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0    13251 2023-05-10 12:07:48.871399 rapids_singlecell-0.6.2/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0      334 2023-05-09 15:12:57.948246 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/__init__.py
--rw-r--r--   0        0        0    36337 2023-05-10 12:07:48.871399 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_hvg.py
--rw-r--r--   0        0        0    14370 2023-05-04 11:39:21.895902 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_normalize.py
--rw-r--r--   0        0        0     3983 2023-05-04 09:38:07.656769 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_pca.py
--rw-r--r--   0        0        0     2783 2023-05-04 09:38:07.648769 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_plotting.py
--rw-r--r--   0        0        0     4823 2023-05-04 09:38:07.656769 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_regress_out.py
--rw-r--r--   0        0        0     1420 2023-05-04 09:38:07.636768 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_scale.py
--rw-r--r--   0        0        0    20357 2023-05-10 12:07:48.871399 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_simple.py
--rw-r--r--   0        0        0      683 2023-05-04 10:15:08.196605 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_utils.py
--rw-r--r--   0        0        0       29 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       68 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4609 2023-05-04 09:38:07.676770 rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6349 2023-05-04 09:38:07.700771 rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0       27 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/gr.py
--rw-r--r--   0        0        0       91 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/pl.py
--rw-r--r--   0        0        0       30 2023-05-04 09:38:07.620767 rapids_singlecell-0.6.2/rapids_singlecell/pp.py
--rw-r--r--   0        0        0      341 2023-05-04 09:38:07.624767 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/__init__.py
--rw-r--r--   0        0        0     5576 2023-05-04 09:38:07.656769 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_clustering.py
--rw-r--r--   0        0        0     3422 2023-05-04 09:38:07.648769 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_diffmap.py
--rw-r--r--   0        0        0     4040 2023-05-04 09:38:07.672770 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_draw_graph.py
--rw-r--r--   0        0        0     5159 2023-05-04 09:38:07.652769 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_embedding_density.py
--rw-r--r--   0        0        0    12177 2023-05-04 09:38:07.736773 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
--rw-r--r--   0        0        0     1745 2023-05-04 09:38:07.624767 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
--rw-r--r--   0        0        0     4136 2023-05-04 09:38:07.648769 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_pca.py
--rw-r--r--   0        0        0     2425 2023-05-04 09:38:07.644768 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_pymde.py
--rw-r--r--   0        0        0     7928 2023-05-04 09:38:07.696771 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
--rw-r--r--   0        0        0     3241 2023-05-04 09:38:07.640768 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_tsne.py
--rw-r--r--   0        0        0       68 2023-05-04 15:27:48.771998 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/__init__.py
--rw-r--r--   0        0        0     5885 2023-05-04 09:38:07.656769 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_autocorr.py
--rw-r--r--   0        0        0     6442 2023-05-04 12:11:53.259130 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_gearysc.py
--rw-r--r--   0        0        0    28951 2023-05-10 13:36:21.450416 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_ligrec.py
--rw-r--r--   0        0        0     6299 2023-05-04 12:11:49.495103 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_moransi.py
--rw-r--r--   0        0        0     5829 2023-05-04 15:55:42.727381 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_utils.py
--rw-r--r--   0        0        0       26 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rapids_singlecell-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-11 09:24:25.229932 rapids_singlecell-0.6.3/LICENSE
+-rw-r--r--   0        0        0     5987 2023-05-16 11:43:52.239538 rapids_singlecell-0.6.3/README.md
+-rw-r--r--   0        0        0      998 2023-05-11 09:24:26.571232 rapids_singlecell-0.6.3/pyproject.toml
+-rwxr-xr-x   0        0        0      132 2023-05-17 23:04:05.157900 rapids_singlecell-0.6.3/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0    13187 2023-05-17 22:08:47.953836 rapids_singlecell-0.6.3/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-11 09:24:26.629783 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/__init__.py
+-rw-r--r--   0        0        0    36773 2023-05-17 22:13:28.447148 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_hvg.py
+-rw-r--r--   0        0        0    14574 2023-05-17 22:14:35.602418 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_normalize.py
+-rw-r--r--   0        0        0     4544 2023-05-17 22:11:30.429802 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_pca.py
+-rw-r--r--   0        0        0     2783 2023-05-11 09:24:26.706782 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_plotting.py
+-rw-r--r--   0        0        0     4788 2023-05-16 11:43:52.638546 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_regress_out.py
+-rw-r--r--   0        0        0     1441 2023-05-17 22:14:46.246296 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_scale.py
+-rw-r--r--   0        0        0    20285 2023-05-17 22:10:17.988666 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_simple.py
+-rw-r--r--   0        0        0     3296 2023-05-17 22:15:20.059310 rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_utils.py
+-rw-r--r--   0        0        0       29 2023-04-19 09:06:38.422832 rapids_singlecell-0.6.3/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       68 2023-04-19 09:06:38.440176 rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4609 2023-05-11 09:24:27.214977 rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6349 2023-05-11 09:24:27.233961 rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0       27 2023-04-19 09:06:38.463999 rapids_singlecell-0.6.3/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       91 2023-04-19 09:06:38.473434 rapids_singlecell-0.6.3/rapids_singlecell/pl.py
+-rw-r--r--   0        0        0       30 2023-05-11 09:24:27.250502 rapids_singlecell-0.6.3/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0      340 2023-05-17 22:09:28.847385 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5576 2023-05-11 09:24:27.293507 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_clustering.py
+-rw-r--r--   0        0        0     3422 2023-05-11 09:24:27.312411 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_diffmap.py
+-rw-r--r--   0        0        0     4040 2023-05-11 09:24:27.331819 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_draw_graph.py
+-rw-r--r--   0        0        0     5154 2023-05-16 11:43:52.775602 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_embedding_density.py
+-rw-r--r--   0        0        0    12177 2023-05-11 09:24:27.365884 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
+-rw-r--r--   0        0        0     1729 2023-05-16 11:43:52.798464 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
+-rw-r--r--   0        0        0     2425 2023-05-11 09:24:27.423103 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_pymde.py
+-rw-r--r--   0        0        0     7928 2023-05-11 09:24:27.442438 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3241 2023-05-11 09:24:27.459468 rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_tsne.py
+-rw-r--r--   0        0        0       68 2023-05-11 09:24:27.476729 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5949 2023-05-17 22:18:00.040946 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     6440 2023-05-16 11:43:52.844153 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0    29505 2023-05-17 22:16:30.013809 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_ligrec.py
+-rw-r--r--   0        0        0     6298 2023-05-16 11:43:52.894061 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     6227 2023-05-17 22:16:29.609203 rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0   253384 2023-05-17 15:05:58.944713 rapids_singlecell-0.6.3/rapids_singlecell/tests/_data/dummy.h5ad
+-rw-r--r--   0        0        0   602117 2023-05-17 15:57:26.464925 rapids_singlecell-0.6.3/rapids_singlecell/tests/_data/test_data.h5ad
+-rw-r--r--   0        0        0    50913 2023-05-17 12:04:20.314112 rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg.csv
+-rw-r--r--   0        0        0   397058 2023-05-17 12:04:30.159721 rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg_v3.csv.gz
+-rw-r--r--   0        0        0    62865 2023-05-17 12:04:33.776581 rapids_singlecell-0.6.3/rapids_singlecell/tests/_scripts/seurat_hvg_v3_batch.csv
+-rw-r--r--   0        0        0     1362 2023-05-17 22:18:37.189568 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_autocorr.py
+-rw-r--r--   0        0        0      461 2023-05-17 22:18:37.163485 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_clustering.py
+-rw-r--r--   0        0        0      687 2023-05-17 22:18:37.187898 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_emdedding_density.py
+-rw-r--r--   0        0        0    10702 2023-05-17 22:18:37.453113 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_hvg.py
+-rw-r--r--   0        0        0     6033 2023-05-17 22:18:37.301399 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_ligrec.py
+-rw-r--r--   0        0        0     2727 2023-05-17 22:18:37.242297 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_normalization.py
+-rw-r--r--   0        0        0     3165 2023-05-17 22:18:37.291646 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_pca.py
+-rw-r--r--   0        0        0      532 2023-05-17 22:18:37.177454 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     3654 2023-05-17 22:18:37.286524 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_qc_metrics.py
+-rw-r--r--   0        0        0     1717 2023-05-17 22:18:37.213145 rapids_singlecell-0.6.3/rapids_singlecell/tests/test_rank_genes_groups_logreg.py
+-rw-r--r--   0        0        0       26 2023-04-19 09:06:38.654835 rapids_singlecell-0.6.3/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rapids_singlecell-0.6.3/PKG-INFO
```

### Comparing `rapids_singlecell-0.6.2/LICENSE` & `rapids_singlecell-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/README.md` & `rapids_singlecell-0.6.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![PyPI](https://img.shields.io/pypi/v/rapids-singlecell?logo=PyPI)](https://pypi.org/project/rapids-singlecell)
 [![PyPIDownloads](https://pepy.tech/badge/rapids-singlecell)](https://pepy.tech/project/rapids-singlecell)
 [![Documentation Status](https://readthedocs.org/projects/rapids-singlecell/badge/?version=latest)](https://rapids-singlecell.readthedocs.io/en/latest/?badge=latest)
 
 # rapids-singlecell
 
 ## Background
-This repository offers some tools to make analyses of single cell datasets faster by running them on the GPU. 
+This repository offers some tools to make analyses of single cell datasets faster by running them on the GPU.
 The functions are analogous versions of functions that can be found within [scanpy](https://github.com/scverse/scanpy) from the Theis lab or functions from [rapids-single-cell-examples](https://github.com/clara-parabricks/rapids-single-cell-examples) created by the Nvidia RAPIDS team. Most functions are kept close to the original code to ensure compatibility. My aim with this repository was to use the speedup that GPU computing offers and combine it with the ease of use from scanpy.
 
 ## Installation
 ### Conda
 The easiest way to install *rapids-singlecell* is to use one of the *yaml* file provided in the [conda](https://github.com/Intron7/rapids_singlecell/tree/main/conda) folder. These *yaml* files install everything needed to run the example notbooks and get you started.
 ```
 conda env create -f conda/rsc_rapids_23.04.yml
@@ -48,15 +48,15 @@
 If you use the accelerated decoupler functions please cite [decoupler](https://doi.org/10.1093/bioadv/vbac016)
 
 ## Notebooks
 To show the capability of these functions, I created two example notebooks evaluating the same workflow running on the CPU and GPU. These notebooks should run in the environment, that is described in Requirements. First, run the `data_downloader` notebook to create the AnnData object for the analysis. If you run both `demo_cpu` and `demo_gpu` you should see a big speedup when running the analyses on the GPU.
 
 ## Benchmarks
 
-Here are some benchmarks. I ran the notebook on the CPU with as many cores as were available where possible. 
+Here are some benchmarks. I ran the notebook on the CPU with as many cores as were available where possible.
 
 |Step                          |CPU (Ryzen 5950x, 32 Cores, 64GB RAM)|GPU (RTX 3090)|CPU (AMD Eypc Rome, 30 Cores, 500GB RAM)| GPU (Quadro RTX 6000)|GPU (A100 80GB)|
 |------------------------------|---------------------------|--------------|----------|--------------|----------------|
 |whole Notebook                | 728 s                     | 43 s         | 917 s    | 67 s         | 57 s           |
 |Preprocessing                 | 75 s                      | 21 s         | 40 s     | 34 s         | 30 s           |
 |Clustering and Visulatization | 423 s                     | 18 s         | 524 s    | 27 s         | 21 s           |
 |Normalize_total               | 252 ms                    | > 1ms        | 425 ms   | 1 ms         | 1 ms           |
```

### Comparing `rapids_singlecell-0.6.2/pyproject.toml` & `rapids_singlecell-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/cunnData/__init__.py` & `rapids_singlecell-0.6.3/rapids_singlecell/cunnData/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,23 @@
 
     def update_shape(self, shape):
         self.shape = shape
 
     def __setitem__(self, key, item):
         if self.shape == item.shape:
             if issparse_gpu(item):
+                item = item
+            elif isinstance(item, cp.ndarray):
+                item = item
+            elif not issparse_cpu(item):
+                inter = sparse.csr_matrix(item)
+                item = cp.sparse.csr_matrix(inter, dtype=cp.float32)
+            else:
+                item = cp.sparse.csr_matrix(item, dtype=cp.float32)
+            if issparse_gpu(item):
                 if item.nnz > 2**31 - 1:
                     raise ValueError(
                         "Cupy only supports Sparse Matrices with `.nnz`"
                         "with less than 2**31-1 for the int32 indptr"
                     )
             super().__setitem__(key, item)
         else:
@@ -99,14 +108,15 @@
         obs: Optional[pd.DataFrame] = None,
         var: Optional[pd.DataFrame] = None,
         uns: Optional[Mapping[str, Any]] = None,
         layers: Optional[Mapping[str, Any]] = None,
         obsm: Optional[Mapping[str, Any]] = None,
         varm: Optional[Mapping[str, Any]] = None,
     ):
+        # Initialize from adata
         if adata:
             if not issparse_cpu(adata.X):
                 inter = sparse.csr_matrix(adata.X)
                 self._X = cp.sparse.csr_matrix(inter, dtype=cp.float32)
                 del inter
             else:
                 self._X = cp.sparse.csr_matrix(adata.X, dtype=cp.float32)
@@ -115,62 +125,54 @@
             self._uns = adata.uns.copy()
             self._layers = Layer_Mapping(self.shape)
             self._obsm = obsm_Mapping(self.shape[0])
             self._varm = varm_Mapping(self.shape[1])
             self.raw = None
             if adata.layers:
                 for key, matrix in adata.layers.items():
-                    if not issparse_cpu(matrix):
-                        inter = sparse.csr_matrix(matrix)
-                        inter = cp.sparse.csr_matrix(inter, dtype=cp.float32)
-                    else:
-                        inter = cp.sparse.csr_matrix(matrix, dtype=cp.float32)
-                    self._layers[key] = inter
+                    self._layers[key] = matrix
             if adata.obsm:
                 for key, matrix in adata.obsm.items():
                     self._obsm[key] = matrix.copy()
             if adata.varm:
                 for key, matrix in adata.varm.items():
                     self._varm[key] = matrix.copy()
 
+        # Initialize from items
         else:
             if issparse_gpu(X):
                 self._X = X
             elif isinstance(X, cp.ndarray):
                 self._X = X
             elif not issparse_cpu(X):
                 inter = sparse.csr_matrix(X)
                 self._X = cp.sparse.csr_matrix(inter, dtype=cp.float32)
                 del inter
             else:
                 self._X = cp.sparse.csr_matrix(X, dtype=cp.float32)
-
-            self._obs = obs
-            self._var = var
+            if obs is not None:
+                self._obs = obs
+            else:
+                self._obs = pd.DataFrame(index=range(self.shape[0]))
+            if var is not None:
+                self._var = var
+            else:
+                self._var = pd.DataFrame(index=range(self.shape[1]))
             if uns:
                 self._uns = uns
             else:
                 self._uns = OrderedDict()
             self._layers = Layer_Mapping(self.shape)
             self._obsm = obsm_Mapping(self.shape[0])
             self._varm = varm_Mapping(self.shape[1])
             self.raw = None
 
             if layers:
                 for key, matrix in layers.items():
-                    if issparse_gpu(matrix):
-                        inter = matrix
-                    elif isinstance(matrix, cp.ndarray):
-                        inter = matrix
-                    elif not issparse_cpu(X):
-                        inter = sparse.csr_matrix(matrix)
-                        inter = cp.sparse.csr_matrix(inter, dtype=cp.float32)
-                    else:
-                        inter = cp.sparse.csr_matrix(matrix, dtype=cp.float32)
-                    self.layers[key] = inter
+                    self.layers[key] = matrix
             if obsm:
                 for key, matrix in obsm.items():
                     self.obsm[key] = matrix.copy()
             if varm:
                 for key, matrix in adata.varm.items():
                     self.varm[key] = matrix
         if issparse_gpu(self._X):
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_hvg.py` & `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_hvg.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,26 @@
     theta: int = 100,
     clip: bool = None,
     chunksize: int = 1000,
     n_samples: int = 10000,
     batch_key: str = None,
 ) -> None:
     """\
-    Annotate highly variable genes. 
+    Annotate highly variable genes.
     Expects logarithmized data, except when `flavor='seurat_v3','pearson_residuals','poisson_gene_selection'`, in which count data is expected.
-    
-    Reimplentation of scanpy's function. 
+
+    Reimplentation of scanpy's function.
     Depending on flavor, this reproduces the R-implementations of Seurat, Cell Ranger, Seurat v3 and Pearson Residuals.
     Flavor `poisson_gene_selection` is an implementation of scvi, which is based on M3Drop. It requiers gpu accelerated pytorch to be installed.
-    
-    For these dispersion-based methods, the normalized dispersion is obtained by scaling 
-    with the mean and standard deviation of the dispersions for genes falling into a given 
-    bin for mean expression of genes. This means that for each bin of mean expression, 
+
+    For these dispersion-based methods, the normalized dispersion is obtained by scaling
+    with the mean and standard deviation of the dispersions for genes falling into a given
+    bin for mean expression of genes. This means that for each bin of mean expression,
     highly variable genes are selected.
-    
+
     For Seurat v3, a normalized variance for each gene is computed. First, the data
     are standardized (i.e., z-score normalization per feature) with a regularized
     standard deviation. Next, the normalized variance is computed as the variance
     of each gene after the transformation. Genes are ranked by the normalized variance.
 
     Parameters
     ----------
@@ -59,40 +59,40 @@
         min_disp
             If n_top_genes unequals None, this and all other cutoffs for the means and the normalized dispersions are ignored.
         max_disp
             If n_top_genes unequals None, this and all other cutoffs for the means and the normalized dispersions are ignored.
         n_top_genes
             Number of highly-variable genes to keep.
         flavor :
-            Choose the flavor (`seurat`, `cell_ranger`, `seurat_v3`, `pearson_residuals`, `poisson_gene_selection`) for identifying highly variable genes. For the dispersion based methods 
+            Choose the flavor (`seurat`, `cell_ranger`, `seurat_v3`, `pearson_residuals`, `poisson_gene_selection`) for identifying highly variable genes. For the dispersion based methods
             in their default workflows, Seurat passes the cutoffs whereas Cell Ranger passes n_top_genes.
         n_bins
             Number of bins for binning the mean gene expression. Normalization is done with respect to each bin. If just a single gene falls into a bin, the normalized dispersion is artificially set to 1.
         span
             The fraction of the data (cells) used when estimating the variance in the loess
             model fit if `flavor='seurat_v3'`.
         check_values
             Check if counts in selected layer are integers. A Warning is returned if set to True.
             Only used if `flavor='seurat_v3'` or `'pearson_residuals'`.
         theta
-            The negative binomial overdispersion parameter `theta` for Pearson residuals. 
+            The negative binomial overdispersion parameter `theta` for Pearson residuals.
             Higher values correspond to less overdispersion (`var = mean + mean^2/theta`), and `theta=np.Inf` corresponds to a Poisson model.
         clip
             Only used if `flavor='pearson_residuals'`. Determines if and how residuals are clipped:
                 * If `None`, residuals are clipped to the interval `[-sqrt(n_obs), sqrt(n_obs)]`, where `n_obs` is the number of cells in the dataset (default behavior).
                 * If any scalar `c`, residuals are clipped to the interval `[-c, c]`. Set `clip=np.Inf` for no clipping.
         chunksize
             If `'poisson_gene_selection'`, this dertermines how many genes are processed at
             once. Choosing a smaller value will reduce the required memory.
         n_samples
             The number of Binomial samples to use to estimate posterior probability
             of enrichment of zeros for each gene (only for `flavor='poisson_gene_selection'`).
         batch_key
             If specified, highly-variable genes are selected within each batch separately and merged.
-            
+
     Returns
     -------
         upates `cudata.var` with the following fields:
 
             `highly_variable` : bool
                 boolean indicator of highly-variable genes
             `means`: float
@@ -160,18 +160,17 @@
                 flavor=flavor,
             )
         else:
             cudata.obs[batch_key] = cudata.obs[batch_key].astype("category")
             batches = cudata.obs[batch_key].cat.categories
             df = []
             genes = cudata.var.index.to_numpy()
+            X = cudata.layers[layer] if layer is not None else cudata.X
             for batch in batches:
-                inter_matrix = cudata.X[
-                    np.where(cudata.obs[batch_key] == batch)[0],
-                ].tocsc()
+                inter_matrix = X[np.where(cudata.obs[batch_key] == batch)[0],].tocsc()
                 thr_org = cp.diff(inter_matrix.indptr).ravel()
                 thr = cp.where(thr_org >= 1)[0]
                 thr_2 = cp.where(thr_org < 1)[0]
                 inter_matrix = inter_matrix[:, thr].tocsr()
                 thr = thr.get()
                 thr_2 = thr_2.get()
                 inter_genes = genes[thr]
@@ -273,15 +272,15 @@
         Returns
         -------
         A DataFrame that contains the columns
         `highly_variable`, `means`, `dispersions`, and `dispersions_norm`.
         """
     if flavor == "seurat":
         X = X.expm1()
-    mean, var = _get_mean_var(X)
+    mean, var = _get_mean_var(X, axis=1)
     mean[mean == 0] = 1e-12
     disp = var / mean
     if flavor == "seurat":  # logarithmized mean as in Seurat
         disp[disp == 0] = np.nan
         disp = cp.log(disp)
         mean = cp.log1p(mean)
     df = pd.DataFrame()
@@ -332,14 +331,20 @@
     if n_top_genes is not None:
         dispersion_norm = dispersion_norm[~np.isnan(dispersion_norm)]
         dispersion_norm[
             ::-1
         ].sort()  # interestingly, np.argpartition is slightly slower
         if n_top_genes > X.shape[1]:
             n_top_genes = X.shape[1]
+        if n_top_genes > dispersion_norm.size:
+            warnings.warn(
+                "`n_top_genes` > number of normalized dispersions, returning all genes with normalized dispersions.",
+                UserWarning,
+            )
+            n_top_genes = dispersion_norm.size
         disp_cut_off = dispersion_norm[n_top_genes - 1]
         gene_subset = np.nan_to_num(df["dispersions_norm"].values) >= disp_cut_off
     else:
         dispersion_norm[np.isnan(dispersion_norm)] = 0  # similar to Seurat
         gene_subset = np.logical_and.reduce(
             (
                 mean > min_mean,
@@ -396,34 +401,35 @@
     X = cudata.layers[layer] if layer is not None else cudata.X
     if check_values and not _check_nonnegative_integers(X):
         warnings.warn(
             "`flavor='seurat_v3'` expects raw count data, but non-integers were found.",
             UserWarning,
         )
 
-    mean, var = _get_mean_var(X)
+    mean, var = _get_mean_var(X, axis=1)
     df["means"], df["variances"] = mean.get(), var.get()
     if batch_key is None:
         batch_info = pd.Categorical(np.zeros(cudata.shape[0], dtype=int))
     else:
         batch_info = cudata.obs[batch_key].values
 
     norm_gene_vars = []
     for b in np.unique(batch_info):
         X_batch = X[batch_info == b]
-        mean, var = _get_mean_var(X_batch)
+        mean, var = _get_mean_var(X_batch, axis=1)
         not_const = var > 0
         estimat_var = cp.zeros(X_batch.shape[1], dtype=np.float64)
 
         y = cp.log10(var[not_const])
         x = cp.log10(mean[not_const])
         model = loess(x.get(), y.get(), span=span, degree=2)
         model.fit()
         estimat_var[not_const] = model.outputs.fitted_values
         reg_std = cp.sqrt(10**estimat_var)
+        X_batch.data = X_batch.data.astype(cp.float64)
         batch_counts = X_batch
         N = X_batch.shape[0]
         vmax = cp.sqrt(N)
         clip_val = reg_std * vmax + mean
         mask = batch_counts.data > clip_val[batch_counts.indices]
         batch_counts.data[mask] = clip_val[batch_counts.indices[mask]]
         squared_batch_counts_sum = cp.array(batch_counts.power(2).sum(axis=0))
@@ -443,14 +449,15 @@
     num_batches_high_var = cp.sum(
         (ranked_norm_gene_vars < n_top_genes).astype(int), axis=0
     )
     ranked_norm_gene_vars[ranked_norm_gene_vars >= n_top_genes] = np.nan
     ranked_norm_gene_vars = ranked_norm_gene_vars.get()
     ma_ranked = np.ma.masked_invalid(ranked_norm_gene_vars)
     median_ranked = np.ma.median(ma_ranked, axis=0).filled(np.nan)
+
     df["highly_variable_nbatches"] = num_batches_high_var.get()
     df["highly_variable_rank"] = median_ranked
     df["variances_norm"] = cp.mean(norm_gene_vars, axis=0).get()
     sorted_index = (
         df[["highly_variable_rank", "highly_variable_nbatches"]]
         .sort_values(
             ["highly_variable_rank", "highly_variable_nbatches"],
@@ -464,15 +471,16 @@
     cudata.var["highly_variable"] = df["highly_variable"].values
     cudata.var["highly_variable_rank"] = df["highly_variable_rank"].values
     cudata.var["means"] = df["means"].values
     cudata.var["variances"] = df["variances"].values
     cudata.var["variances_norm"] = df["variances_norm"].values.astype(
         "float64", copy=False
     )
-    cudata.var["highly_variable_nbatches"] = df["highly_variable_nbatches"].values
+    if batch_key:
+        cudata.var["highly_variable_nbatches"] = df["highly_variable_nbatches"].values
     cudata.uns["hvg"] = {"flavor": "seurat_v3"}
 
 
 def _highly_variable_pearson_residuals(
     cudata: cunnData,
     theta: float = 100,
     clip: Optional[float] = None,
@@ -509,15 +517,15 @@
         batch_info = cudata.obs[batch_key].values
 
     n_batches = len(np.unique(batch_info))
     residual_gene_vars = []
     sparse_kernel = cp.RawKernel(
         r"""
     extern "C" __global__
-    void calculate_sum_cg(const int *indptr,const int *index,const float *data, 
+    void calculate_sum_cg(const int *indptr,const int *index,const float *data,
                                         float* sums_genes, float* sums_cells,
                                         int n_genes) {
         int gene = blockDim.x * blockIdx.x + threadIdx.x;
         if(gene >= n_genes){
             return;
         }
         int start_idx = indptr[gene];
@@ -533,15 +541,15 @@
     }
     """,
         "calculate_sum_cg",
     )
     sparse_kernel_res = cp.RawKernel(
         r"""
     extern "C" __global__
-    void calculate_res(const int *indptr,const int *index,const float *data, 
+    void calculate_res(const int *indptr,const int *index,const float *data,
                             const float* sums_genes,const float* sums_cells,
                             float* residuals ,float* sum_total,float* clip,float* theta,int n_genes, int n_cells) {
         int gene = blockDim.x * blockIdx.x + threadIdx.x;
         if(gene >= n_genes){
             return;
         }
         int start_idx = indptr[gene];
@@ -592,14 +600,15 @@
         X_batch = X_batch[:, nonzero_genes]
         if clip is None:
             n = X_batch.shape[0]
             clip = cp.sqrt(n, dtype=cp.float32)
         if clip < 0:
             raise ValueError("Pearson residuals require `clip>=0` or `clip=None`.")
 
+        clip = cp.array([clip], dtype=cp.float32)
         theta = cp.array([theta], dtype=cp.float32)
         sums_genes = cp.zeros(X_batch.shape[1], dtype=cp.float32)
         sums_cells = cp.zeros(X_batch.shape[0], dtype=cp.float32)
         block = (32,)
         grid = (int(math.ceil(X_batch.shape[1] / block[0])),)
         sparse_kernel(
             grid,
@@ -647,15 +656,15 @@
         (ranks_residual_var < n_top_genes).astype(int), axis=0
     ).get()
     ranks_residual_var[ranks_residual_var >= n_top_genes] = np.nan
     ranks_residual_var = ranks_residual_var.get()
     ranks_masked_array = np.ma.masked_invalid(ranks_residual_var)
     # Median rank across batches, ignoring batches in which gene was not selected
     medianrank_residual_var = np.ma.median(ranks_masked_array, axis=0).filled(np.nan)
-    means, variances = _get_mean_var(X)
+    means, variances = _get_mean_var(X, axis=1)
     means, variances = means.get(), variances.get()
     df = pd.DataFrame.from_dict(
         dict(
             means=means,
             variances=variances,
             residual_variances=cp.mean(residual_gene_vars, axis=0).get(),
             highly_variable_rank=medianrank_residual_var,
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_normalize.py` & `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,42 +12,42 @@
     cudata: cunnData, target_sum: int, layer: Optional[str] = None, inplace: bool = True
 ) -> Optional[cpx.scipy.sparse.csr_matrix]:
     """
     Normalizes rows in matrix so they sum to `target_sum`
 
     Parameters
     ----------
-        cudata: 
+        cudata:
             cunnData object
 
-        target_sum : 
+        target_sum :
             Each row will be normalized to sum to this value
-        
+
         layer
             Layer to normalize instead of `X`. If `None`, `X` is normalized.
 
         inplace
             Whether to update `cudata` or return the normalized matrix.
-        
-    
+
+
     Returns
     -------
     Returns a normalized copy or  updates `cudata` with a normalized version of \
     the original `cudata.X` and `cudata.layers['layer']`, depending on `inplace`.
-    
+
     """
     csr_arr = cudata.layers[layer] if layer is not None else cudata.X
 
     if not inplace:
         csr_arr = csr_arr.copy()
 
     mul_kernel = cp.RawKernel(
         r"""
         extern "C" __global__
-        void mul_kernel(const int *indptr, float *data, 
+        void mul_kernel(const int *indptr, float *data,
                         int nrows, int tsum) {
             int row = blockDim.x * blockIdx.x + threadIdx.x;
 
             if(row >= nrows)
                 return;
 
             float scale = 0.0;
@@ -117,15 +117,15 @@
     else:
         return X
 
 
 _sparse_kernel_sum_csc = cp.RawKernel(
     r"""
     extern "C" __global__
-    void calculate_sum_cg_csc(const int *indptr,const int *index,const float *data, 
+    void calculate_sum_cg_csc(const int *indptr,const int *index,const float *data,
                                         float* sums_genes, float* sums_cells,
                                         int n_genes) {
         int gene = blockDim.x * blockIdx.x + threadIdx.x;
         if(gene >= n_genes){
             return;
         }
         int start_idx = indptr[gene];
@@ -142,15 +142,15 @@
     """,
     "calculate_sum_cg_csc",
 )
 
 _sparse_kernel_norm_res_csc = cp.RawKernel(
     r"""
     extern "C" __global__
-    void calculate_res_csc(const int *indptr,const int *index,const float *data, 
+    void calculate_res_csc(const int *indptr,const int *index,const float *data,
                             const float* sums_cells,const float* sums_genes,
                             float* residuals ,const float* sum_total, const float* clip,
                             const float* theta,const int n_cells,const int n_genes) {
         int gene = blockDim.x * blockIdx.x + threadIdx.x;
         if(gene >= n_genes){
             return;
         }
@@ -174,15 +174,15 @@
     "calculate_res_csc",
 )
 
 
 _sparse_kernel_sum_csr = cp.RawKernel(
     r"""
     extern "C" __global__
-    void calculate_sum_cg_csr(const int *indptr,const int *index,const float *data, 
+    void calculate_sum_cg_csr(const int *indptr,const int *index,const float *data,
                                         float* sums_genes, float* sums_cells,
                                         int n_cells) {
         int cell = blockDim.x * blockIdx.x + threadIdx.x;
         if(cell >= n_cells){
             return;
         }
         int start_idx = indptr[cell];
@@ -290,27 +290,27 @@
     `theta` shared across genes. By default, residuals are clipped to `sqrt(n_obs)`
     and overdispersion `theta=100` is used.
 
     Parameters
     ----------
         cudata
             cunnData object
-        theta 
-            The negative binomial overdispersion parameter theta for Pearson residuals. 
+        theta
+            The negative binomial overdispersion parameter theta for Pearson residuals.
             Higher values correspond to less overdispersion (var = mean + mean^2/theta), and theta=np.Inf corresponds to a Poisson model.
-        clip 
+        clip
             Determines if and how residuals are clipped:
             If None, residuals are clipped to the interval [-sqrt(n_obs), sqrt(n_obs)], where n_obs is the number of cells in the dataset (default behavior).
             If any scalar c, residuals are clipped to the interval [-c, c]. Set clip=np.Inf for no clipping.
-        check_values 
-            If True, checks if counts in selected layer are integers as expected by this function, 
+        check_values
+            If True, checks if counts in selected layer are integers as expected by this function,
             and return a warning if non-integers are found. Otherwise, proceed without checking. Setting this to False can speed up code for large datasets.
         layer
             Layer to use as input instead of X. If None, X is used.
-        inplace 
+        inplace
             If True, update cunnData with results. Otherwise, return results. See below for details of what is returned.
 
     Returns
     ----------
         If `inplace=True`, `cudata.X` or the selected layer in `cudata.layers` is updated with the normalized values. \
         If `inplace=False` the normalized matrix is returned.
 
@@ -319,22 +319,25 @@
     X = cudata.layers[layer] if layer is not None else cudata.X
 
     if check_values and not _check_nonnegative_integers(X):
         warnings.warn(
             "`flavor='pearson_residuals'` expects raw count data, but non-integers were found.",
             UserWarning,
         )
+    computed_on = layer if layer else "cudata.X"
+    settings_dict = dict(theta=theta, clip=clip, computed_on=computed_on)
     if theta <= 0:
         raise ValueError("Pearson residuals require theta > 0")
     if clip is None:
         n = X.shape[0]
         clip = cp.sqrt(n, dtype=cp.float32)
     if clip < 0:
         raise ValueError("Pearson residuals require `clip>=0` or `clip=None`.")
     theta = cp.array([1 / theta], dtype=cp.float32)
+    clip = cp.array([clip], dtype=cp.float32)
     sums_cells = cp.zeros(X.shape[0], dtype=cp.float32)
     sums_genes = cp.zeros(X.shape[1], dtype=cp.float32)
 
     if cp.sparse.issparse(X):
         residuals = cp.zeros(X.shape, dtype=cp.float32)
         if cpx.scipy.sparse.isspmatrix_csc(X):
             block = (8,)
@@ -416,14 +419,16 @@
                 sum_total,
                 clip,
                 theta,
                 residuals.shape[0],
                 residuals.shape[1],
             ),
         )
+
     if inplace == True:
+        cudata.uns["pearson_residuals_normalization"] = settings_dict
         if layer:
             cudata.layers[layer] = residuals
         else:
             cudata.X = residuals
     else:
         return residuals
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_plotting.py` & `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_plotting.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_regress_out.py` & `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_regress_out.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,39 +13,39 @@
     layer: Optional[str] = None,
     inplace: bool = True,
     batchsize: Union[int, Literal["all"], None] = 100,
     verbose: bool = False,
 ) -> Optional[cp.ndarray]:
     """
     Use linear regression to adjust for the effects of unwanted noise
-    and variation. 
-    
+    and variation.
+
     Parameters
     ----------
         cudata
             cunnData object
 
         keys
             Keys for numerical observation annotation on which to regress on.
-        
+
         layer
             Layer to regress instead of `X`. If `None`, `X` is regressed.
 
         inplace
             Whether to update `cudata` or return the corrected matrix of `cudata.X` and `cudata.layers`.
 
         batchsize
             Number of genes that should be processed together. \
             If `'all'` all genes will be processed together if `.n_obs` <100000. \
             If `None` each gene will be analysed seperatly. \
-            Will be ignored if cuML version < 22.12 
-            
-        verbose 
+            Will be ignored if cuML version < 22.12
+
+        verbose
             Print debugging information
-        
+
     Returns
     -------
     Returns a corrected copy or  updates `cudata` with a corrected version of the \
     original `cudata.X` and `cudata.layers['layer']`, depending on `inplace`.
     """
 
     if batchsize != "all" and type(batchsize) not in [int, type(None)]:
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_scale.py` & `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_scale.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import cupy as cp
 from ..cunnData import cunnData
 from typing import Optional
 
 
 def scale(
     cudata: cunnData,
-    max_value: int = 10,
+    max_value: Optional[int] = None,
     layer: Optional[str] = None,
     inplace: bool = True,
 ) -> Optional[cp.ndarray]:
     """
     Scales matrix to unit variance and clips values
-    
+
     Parameters
     ----------
         cudata
             cunnData object
 
         max_value
             After scaling matrix to unit variance, values will be clipped to this number of std deviations.
 
-        layer 
+        layer
             Layer to use as input instead of X. If None, X is used.
 
         inplace
             If True, update cunnData with results. Otherwise, return results. See below for details of what is returned.
-        
+
     Returns
     -------
     Returns a sacled copy or updates `cudata` with a scaled version of the original `cudata.X` and `cudata.layers['layer']`, \
     depending on `inplace`.
 
     """
     X = cudata.layers[layer] if layer is not None else cudata.X
@@ -41,15 +41,16 @@
         X = X.copy()
     mean = X.sum(axis=0).flatten() / X.shape[0]
     X -= mean
     del mean
     stddev = cp.sqrt(X.var(axis=0))
     X /= stddev
     del stddev
-    X = cp.clip(X, a_max=max_value)
+    if max_value:
+        X = cp.clip(X, a_max=max_value)
     if inplace:
         if layer:
             cudata.layers[layer] = X
         else:
             cudata.X = X
     else:
         return X
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_simple.py` & `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import math
 from ..cunnData import cunnData
 from typing import Union
 
 _sparse_qc_kernel_csc = cp.RawKernel(
     r"""
     extern "C" __global__
-    void caluclate_qc_csc(const int *indptr,const int *index,const float *data, 
+    void caluclate_qc_csc(const int *indptr,const int *index,const float *data,
                                         float* sums_cells, float* sums_genes,
                                         int* cell_ex, int* gene_ex,
                                         int n_genes) {
         int gene = blockDim.x * blockIdx.x + threadIdx.x;
         if(gene >= n_genes){
             return;
         }
@@ -34,15 +34,15 @@
     """,
     "caluclate_qc_csc",
 )
 
 _sparse_qc_kernel_csr = cp.RawKernel(
     r"""
     extern "C" __global__
-    void caluclate_qc_csr(const int *indptr,const int *index,const float *data, 
+    void caluclate_qc_csr(const int *indptr,const int *index,const float *data,
                         float* sums_cells, float* sums_genes,
                         int* cell_ex, int* gene_ex,
                         int n_cells) {
         int cell = blockDim.x * blockIdx.x + threadIdx.x;
         if(cell >= n_cells){
             return;
         }
@@ -62,42 +62,42 @@
     """,
     "caluclate_qc_csr",
 )
 
 _sparse_qc_kernel_dense = cp.RawKernel(
     r"""
     extern "C" __global__
-    void caluclate_qc_dense(const float *data, 
+    void caluclate_qc_dense(const float *data,
                         float* sums_cells, float* sums_genes,
                         int* cell_ex, int* gene_ex,
                         int n_cells,int n_genes) {
         int cell = blockDim.x * blockIdx.x + threadIdx.x;
         int gene = blockDim.y * blockIdx.y + threadIdx.y;
         if(cell >= n_cells || gene >=n_genes){
             return;
         }
-    
+
 
         long long int index = static_cast<long long int>(cell) * n_genes + gene;
         float value = data[index];
-        if (value>0.0){ 
+        if (value>0.0){
             atomicAdd(&sums_genes[gene], value);
             atomicAdd(&sums_cells[cell], value);
             atomicAdd(&gene_ex[gene], 1);
             atomicAdd(&cell_ex[cell], 1);
         }
     }
     """,
     "caluclate_qc_dense",
 )
 
 _sparse_qc_kernel_csc_sub = cp.RawKernel(
     r"""
     extern "C" __global__
-    void caluclate_qc_csc_sub(const int *indptr,const int *index,const float *data, 
+    void caluclate_qc_csc_sub(const int *indptr,const int *index,const float *data,
                                         float* sums_cells, bool* mask,
                                         int n_genes) {
         int gene = blockDim.x * blockIdx.x + threadIdx.x;
         if(gene >= n_genes){
             return;
         }
         if(mask[gene] == false){
@@ -114,15 +114,15 @@
     """,
     "caluclate_qc_csc_sub",
 )
 
 _sparse_qc_kernel_csr_sub = cp.RawKernel(
     r"""
     extern "C" __global__
-    void caluclate_qc_csr_sub(const int *indptr,const int *index,const float *data, 
+    void caluclate_qc_csr_sub(const int *indptr,const int *index,const float *data,
                         float* sums_cells, bool* mask,
                         int n_cells) {
         int cell = blockDim.x * blockIdx.x + threadIdx.x;
         if(cell >= n_cells){
             return;
         }
         int start_idx = indptr[cell];
@@ -139,26 +139,26 @@
     """,
     "caluclate_qc_csr_sub",
 )
 
 _sparse_qc_kernel_dense_sub = cp.RawKernel(
     r"""
     extern "C" __global__
-    void caluclate_qc_dense_sub(const float *data, 
+    void caluclate_qc_dense_sub(const float *data,
                         float* sums_cells, bool *mask,
                         int n_cells, int n_genes) {
         int cell = blockDim.x * blockIdx.x + threadIdx.x;
         int gene = blockDim.y * blockIdx.y + threadIdx.y;
         if(cell >= n_cells || gene >=n_genes){
             return;
         }
         if(mask[gene] == false){
             return;
         }
-        
+
         long long int index = static_cast<long long int>(cell) * n_genes + gene;
         atomicAdd(&sums_cells[cell], data[index]);
 
     }
     """,
     "caluclate_qc_dense_sub",
 )
@@ -170,52 +170,52 @@
     var_type: str = "genes",
     qc_vars: Union[str, list] = None,
     log1p: bool = True,
 ) -> None:
     """\
     Calculates basic qc Parameters. Calculates number of genes per cell (n_genes) and number of counts per cell (n_counts).
     Loosly based on calculate_qc_metrics from scanpy [Wolf et al. 2018]. Updates :attr:`.obs` and :attr:`.var`  with columns with qc data.
-    
+
     Parameters
     ----------
-        cudata 
+        cudata
             cunnData object
         expr_type
             Name of kind of values in X.
         var_type
             The kind of thing the variables are.
         qc_vars
             Keys for boolean columns of :attr:`.var` which identify variables you could want to control for (e.g. Mito).
             Run flag_gene_family first
         log1p
             Set to `False` to skip computing `log1p` transformed annotations.
-            
+
     Returns
     -------
         adds the following columns in :attr:`.obs` :
             `total_{var_type}_by_{expr_type}`
                 E.g. 'total_genes_by_counts'. Number of genes with positive counts in a cell.
             `total_{expr_type}`
                 E.g. 'total_counts'. Total number of counts for a cell.
             for `qc_var` in `qc_vars`
                 `total_{expr_type}_{qc_var}`
                     number of counts per qc_var (e.g total counts mitochondrial genes)
                 `pct_{expr_type}_{qc_var}`
                     Proportion of counts of qc_var (percent of counts mitochondrial genes)
-        
+
         adds the following columns in :attr:`.var` :
             `total_{expr_type}`
                 E.g. 'total_counts'. Sum of counts for a gene.
             `n_genes_by_{expr_type}`
                 E.g. 'n_cells_by_counts'. Number of cells this expression is measured in.
             `mean_{expr_type}`
                 E.g. "mean_counts". Mean expression over all cells.
             `pct_dropout_by_{expr_type}`
                 E.g. 'pct_dropout_by_counts'. Percentage of cells this feature does not appear in.
-        
+
     """
 
     X = cudata.X
     sums_cells = cp.zeros(X.shape[0], dtype=cp.float32)
     sums_genes = cp.zeros(X.shape[1], dtype=cp.float32)
     cell_ex = cp.zeros(X.shape[0], dtype=cp.int32)
     gene_ex = cp.zeros(X.shape[1], dtype=cp.int32)
@@ -287,15 +287,15 @@
         cudata.obs[f"log1p_total_{expr_type}"] = cp.asnumpy(cp.log1p(sums_cells))
 
     if qc_vars:
         if type(qc_vars) is str:
             qc_vars = [qc_vars]
         for qc_var in qc_vars:
             sums_cells_sub = cp.zeros(X.shape[0], dtype=cp.float32)
-            mask = cp.array(cudata.var["MT"], dtype=cp.bool_)
+            mask = cp.array(cudata.var[qc_var], dtype=cp.bool_)
             if cp.sparse.issparse(X):
                 if cpx.scipy.sparse.isspmatrix_csr(X):
                     block = (32,)
                     grid = (int(math.ceil(X.shape[0] / block[0])),)
                     _sparse_qc_kernel_csr_sub(
                         grid,
                         block,
@@ -377,36 +377,36 @@
 ) -> None:
     """
     Filter genes based on number of cells or counts.
 
     Filters genes, that have greater than a max number of genes or less than
     a minimum number of a feature in a given :attr:`.var` columns. Can so far only be used for numerical columns.
     You can run this function on 'n_cells' or 'n_counts' with a previous columns in :attr:`.var`.
-    
+
     Parameters
     ----------
-        cudata: 
+        cudata:
             cunnData object
 
         qc_var
             column in :attr:`.var` with numerical entries to filter against
 
         min_count
             Lower bound on number of a given feature to keep gene
 
         max_count
             Upper bound on number of a given feature to keep gene
 
         verbose
             Print number of discarded genes
-    
+
     Returns
     -------
         a filtered :class:`~rapids_singlecell.cunnData.cunnData` object inplace
-    
+
     """
 
     if qc_var in cudata.var.keys():
         if min_count is not None and max_count is not None:
             thr = np.where(
                 (cudata.var[qc_var] <= max_count) & (min_count <= cudata.var[qc_var])
             )[0]
@@ -480,28 +480,28 @@
     verbose: bool = True,
 ) -> None:
     """\
     Filter cell outliers based on counts and numbers of genes expressed.
 
     Filter cells based on numerical columns in the :attr:`.obs` by selecting those with a feature count greater than a specified maximum or less than a specified minimum.
     It is recommended to run :func:`calculate_qc_metrics` before using this function. You can run this function on n_genes or n_counts before running :func:`calculate_qc_metrics`.
-    
+
     Parameters
     ----------
-        cudata: 
+        cudata:
             cunnData object
         qc_var
             column in .obs with numerical entries to filter against
         min_count
             Lower bound on number of a given feature to keep cell
         max_count
             Upper bound on number of a given feature to keep cell
         verbose
             Print number of discarded cells
-    
+
     Returns
     -------
        a filtered :class:`~rapids_singlecell.cunnData.cunnData` object inplace
 
     """
     if qc_var in cudata.obs.keys():
         inter = np.array
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.6.3/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_clustering.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_clustering.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_diffmap.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_diffmap.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_draw_graph.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_draw_graph.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_embedding_density.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_embedding_density.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     categorical cell annotation. The cell density can be plotted using the
     `pl.embedding_density` function.
     Note that density values are scaled to be between 0 and 1. Thus, the
     density value at each cell is only comparable to densities in
     the same category.
     This function was written by Sophie Tritschler and implemented into
     Scanpy by Malte Luecken.
-    This function uses cuML's KernelDensity. It returns log Likelihood as does 
+    This function uses cuML's KernelDensity. It returns log Likelihood as does
     sklearn's implementation. scipy.stats implementation, used
     in scanpy, returns PDF.
 
     Parameters
     ----------
         adata
             The annotated data matrix.
@@ -43,15 +43,15 @@
             This is limited to two components.
     Returns
     -------
     Updates `adata.obs` with an additional field specified by the `key_added` \
     parameter. This parameter defaults to `[basis]_density_[groupby]`, where \
     `[basis]` is one of `umap`, `diffmap`, `pca`, `tsne`, or `draw_graph_fa` \
     and `[groupby]` denotes the parameter input.
-    
+
     Updates `adata.uns` with an additional field `[key_added]_params`.
     """
     # to ensure that newly created covariates are categorical
     # to test for category numbers
     adata._sanitize()
     # Test user inputs
     basis = basis.lower()
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_harmony_integrate.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_harmony_integrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         adjusted_basis
             The name of the field in ``adata.obsm`` where the adjusted PCA
             table will be stored after running this function. Defaults to
             ``X_pca_harmony``.
         kwargs
             Any additional arguments will be passed to
             ``harmonpy_gpu.run_harmony()``.
-            
+
     Returns
     -------
         Updates adata with the field ``adata.obsm[adjusted_basis]``, \
         containing principal components adjusted by Harmony such that \
         different experiments are integrated.
-    
+
     """
     from . import _harmonpy_gpu
 
     harmony_out = _harmonpy_gpu.run_harmony(adata.obsm[basis], adata.obs, key, **kwargs)
 
     adata.obsm[adjusted_basis] = harmony_out.Z_corr.T.get()
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_pca.py` & `rapids_singlecell-0.6.3/rapids_singlecell/cunnData_funcs/_pca.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-from cuml.decomposition import PCA, TruncatedSVD
+from ..cunnData import cunnData
 from anndata import AnnData
-from typing import Optional
 
-from scipy.sparse import issparse
-import warnings
+from cuml.decomposition import PCA, TruncatedSVD
+from typing import Optional, Union
+
+from cupy.sparse import issparse
 import math
 import numpy as np
 
 
 def pca(
-    adata: AnnData,
+    cudata: Union[cunnData, AnnData],
     layer: str = None,
-    n_comps: int = 50,
+    n_comps: Optional[int] = None,
     zero_center: bool = True,
+    random_state: Union[int, None] = 0,
     use_highly_variable: Optional[bool] = None,
     chunked: bool = False,
     chunk_size: int = None,
 ) -> None:
     """
-    Performs PCA using the cuML decomposition function for the :class:`~anndata.AnnData` object.
+    Performs PCA using the cuML decomposition function for the :class:`~rapids_singlecell.cunnData.cunnData` object.
 
     Parameters
     ----------
-        adata
-            annData object
+        cudata :
+            cunnData, AnnData object
 
         layer
-            If provided, use `adata.layers[layer]` for expression values instead of `adata.X`.
+            If provided, use `cudata.layers[layer]` for expression values instead of `cudata.X`.
 
         n_comps
-            Number of principal components to compute. Defaults to 50
+            Number of principal components to compute. Defaults to 50, or 1 - minimum
+            dimension size of selected representation
 
         zero_center
             If `True`, compute standard PCA from covariance matrix.
             If `False`, omit zero-centering variables
 
+        random_state
+            Change to use different initial states for the optimization.
+
         use_highly_variable
             Whether to use highly variable genes only, stored in
             `.var['highly_variable']`.
             By default uses them if they have been determined beforehand.
 
         chunked
             If `True`, perform an incremental PCA on segments of `chunk_size`.
@@ -46,48 +52,48 @@
             `random_seed` and `svd_solver`. If `False`, perform a full PCA.
 
         chunk_size
             Number of observations to include in each chunk.
             Required if `chunked=True` was passed.
 
     Returns
-    --------
-        adds fields to `adata`:
-
+    -------
+        adds fields to `cudata` :
             `.obsm['X_pca']`
-                    PCA representation of data.
+                PCA representation of data.
             `.varm['PCs']`
-                    The principal components containing the loadings.
+                The principal components containing the loadings.
             `.uns['pca']['variance_ratio']`
-                    Ratio of explained variance.
+                Ratio of explained variance.
             `.uns['pca']['variance']`
-                    Explained variance, equivalent to the eigenvalues of the
-                    covariance matrix.
+                Explained variance, equivalent to the eigenvalues of the
+                covariance matrix.
     """
 
-    if use_highly_variable is True and "highly_variable" not in adata.var.keys():
+    if use_highly_variable is True and "highly_variable" not in cudata.var.keys():
         raise ValueError(
-            "Did not find adata.var['highly_variable']. "
+            "Did not find cudata.var['highly_variable']. "
             "Either your data already only consists of highly-variable genes "
             "or consider running `highly_variable_genes` first."
         )
 
-    X = adata.layers[layer] if layer is not None else adata.X
+    X = cudata.layers[layer] if layer is not None else cudata.X
 
     if use_highly_variable is None:
-        use_highly_variable = True if "highly_variable" in adata.var.keys() else False
+        use_highly_variable = True if "highly_variable" in cudata.var.keys() else False
 
     if use_highly_variable:
-        X = X[:, adata.var["highly_variable"]]
+        X = X[:, cudata.var["highly_variable"]]
 
-    if issparse(X) and zero_center:
-        warnings.warn(
-            "Your Countmatrix seems to be sparse, this can lead to a massive performance penalty.",
-            UserWarning,
-        )
+    if n_comps is None:
+        min_dim = min(X.shape[0], X.shape[1])
+        if 50 >= min_dim:
+            n_comps = min_dim - 1
+        else:
+            n_comps = 50
 
     if chunked:
         from cuml.decomposition import IncrementalPCA
 
         X_pca = np.zeros((X.shape[0], n_comps), X.dtype)
 
         pca_func = IncrementalPCA(
@@ -98,24 +104,30 @@
         n_batches = math.ceil(X.shape[0] / chunk_size)
         for batch in range(n_batches):
             start_idx = batch * chunk_size
             stop_idx = min(batch * chunk_size + chunk_size, X.shape[0])
             chunk = X[start_idx:stop_idx, :]
             chunk = chunk.toarray() if issparse(chunk) else chunk
             X_pca[start_idx:stop_idx] = pca_func.transform(chunk)
-    elif zero_center:
-        pca_func = PCA(n_components=n_comps, output_type="numpy")
-        X_pca = pca_func.fit_transform(X)
-
-    elif not zero_center:
-        pca_func = TruncatedSVD(n_components=n_comps, output_type="numpy")
-        X_pca = pca_func.fit_transform(X)
-    adata.obsm["X_pca"] = X_pca
-    adata.uns["pca"] = {
+    else:
+        if zero_center:
+            pca_func = PCA(
+                n_components=n_comps, random_state=random_state, output_type="numpy"
+            )
+            X_pca = pca_func.fit_transform(X)
+
+        elif not zero_center:
+            pca_func = TruncatedSVD(
+                n_components=n_comps, random_state=random_state, output_type="numpy"
+            )
+            X_pca = pca_func.fit_transform(X)
+
+    cudata.obsm["X_pca"] = X_pca
+    cudata.uns["pca"] = {
         "variance": pca_func.explained_variance_,
         "variance_ratio": pca_func.explained_variance_ratio_,
     }
     if use_highly_variable:
-        adata.varm["PCs"] = np.zeros(shape=(adata.n_vars, n_comps))
-        adata.varm["PCs"][adata.var["highly_variable"]] = pca_func.components_.T
+        cudata.varm["PCs"] = np.zeros(shape=(cudata.n_vars, n_comps))
+        cudata.varm["PCs"][cudata.var["highly_variable"]] = pca_func.components_.T
     else:
-        adata.varm["PCs"] = pca_func.components_.T
+        cudata.varm["PCs"] = pca_func.components_.T
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_pymde.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_pymde.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_tsne.py` & `rapids_singlecell-0.6.3/rapids_singlecell/scanpy_gpu/_tsne.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_autocorr.py` & `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_autocorr.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     use_raw: bool = False,
     use_sparse: bool = False,
     copy: bool = False,
 ) -> Optional[pd.DataFrame]:
     """
     Calculate spatial autocorrelation for genes in an AnnData object.
 
-    This function computes spatial autocorrelation scores (Moran's I or Geary's C) for each gene in an AnnData object. 
+    This function computes spatial autocorrelation scores (Moran's I or Geary's C) for each gene in an AnnData object.
     The function also calculates p-values and corrected p-values for multiple testing.
 
     Note:
-        This implementation uses single-precision (float32) for calculations, which may result in decreased accuracy for weak 
-        correlations when compared to double-precision (float64) calculations. For strongly correlated data, the difference in p-values 
-        should be minimal. However, for weakly correlated data with I or C values close to their expected values, the lack of precision 
+        This implementation uses single-precision (float32) for calculations, which may result in decreased accuracy for weak
+        correlations when compared to double-precision (float64) calculations. For strongly correlated data, the difference in p-values
+        should be minimal. However, for weakly correlated data with I or C values close to their expected values, the lack of precision
         may lead to larger discrepancies in p-values.
 
 
     Parameters
     ----------
         adata
             Annotated data matrix.
@@ -106,19 +106,19 @@
         adj_matrix_cupy = adj_matrix_cupy.multiply(cp.sparse.csr_matrix(row_sums))
 
     params = {"two_tailed": two_tailed}
 
     # check sparse:
     if use_sparse:
         vals = sparse.csr_matrix(vals)
-        data = cp.sparse.csr_matrix(vals)
+        data = cp.sparse.csr_matrix(vals, dtype=cp.float32)
     else:
         if sparse.issparse(vals):
             vals = vals.toarray()
-        data = cp.array(vals)
+        data = cp.array(vals, dtype=cp.float32)
     # Run Spartial Autocorr
     if mode == "moran":
         score, score_perms = _morans_I_cupy(
             data, adj_matrix_cupy, n_permutations=n_perms
         )
         params["stat"] = "I"
         params["expected"] = -1.0 / (adata.shape[0] - 1)  # expected score
@@ -132,15 +132,16 @@
         params["expected"] = 1.0
         params["ascending"] = True
         params["mode"] = "gearyC"
     else:
         raise NotImplementedError(f"Mode `{mode}` is not yet implemented.")
     g = sparse.csr_matrix(adj_matrix_cupy.get())
     score = score.get()
-    score_perms = score_perms.get()
+    if n_perms is not None:
+        score_perms = score_perms.get()
     with np.errstate(divide="ignore"):
         pval_results = _p_value_calc(score, score_perms, g, params)
 
     df = pd.DataFrame({params["stat"]: score, **pval_results}, index=genes)
 
     if corr_method is not None:
         for pv in filter(lambda x: "pval" in x, df.columns):
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_gearysc.py` & `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_gearysc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import cupy as cp
 import math
 
 
 kernel_gearys_C_num_dense = r"""
-extern "C" __global__ void gearys_C_num_dense(const float* data, 
-const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, const float* adj_matrix_data, 
+extern "C" __global__ void gearys_C_num_dense(const float* data,
+const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, const float* adj_matrix_data,
 float* num, int n_samples, int n_features) {
     int f = blockIdx.x * blockDim.x + threadIdx.x;
     int i = blockIdx.y * blockDim.y + threadIdx.y;
 
     if (i >= n_samples || f >= n_features) {
         return;
     }
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_ligrec.py` & `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_ligrec.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Union,
     Literal,
     Optional,
     Sequence,
     Mapping,
     Iterable,
 )
-from ._utils import _create_sparse_df
+from ._utils import _create_sparse_df, _assert_categorical_obs
 
 
 SOURCE = "source"
 TARGET = "target"
 
 
 def _get_interactions(
@@ -241,16 +241,14 @@
 
     """
     # Get and Check interactions
     if interactions is None:
         interactions = _get_interactions(
             interactions_params, transmitter_params, receiver_params
         )
-    else:
-        interactions = interactions.copy()
 
     if isinstance(interactions, Mapping):
         interactions = pd.DataFrame(interactions)
 
     if isinstance(interactions, pd.DataFrame):
         if SOURCE not in interactions.columns:
             raise KeyError(f"Column `{SOURCE!r}` is not in `interactions`.")
@@ -273,14 +271,21 @@
     else:
         raise TypeError(
             f"Expected either a `pandas.DataFrame`, `dict` or `iterable`, found `{type(interactions).__name__}`"
         )
 
     assert isinstance(interactions, pd.DataFrame)
 
+    if corr_axis:
+        if corr_axis not in {"clusters", "interactions"}:
+            raise ValueError(f"Invalid option `{corr_axis}` for `CorrAxis`.")
+
+    if n_perms <= 0:
+        raise ValueError(f"Expected `n_perms` to be positive, found `{n_perms}`.")
+
     if interactions.empty:
         raise ValueError("The interactions are empty")
     # Prepare adata
     if not isinstance(adata, AnnData):
         raise TypeError(
             f"Expected `adata` to be of type `anndata.AnnData`, found `{type(adata).__name__}`."
         )
@@ -351,26 +356,31 @@
         interactions = pd.merge(
             interactions, src, how="left", left_index=True, right_index=True
         )
         interactions = pd.merge(
             interactions, tgt, how="left", left_index=True, right_index=True
         )
     else:
-        raise NotImplementedError(
-            f"Complex policy {complex_policy!r} is not implemented."
-        )
+        raise ValueError(f"Invalid option `{complex_policy!r}` for `ComplexPolicy`.")
 
     interactions = interactions[
         interactions[SOURCE].isin(data.columns)
         & interactions[TARGET].isin(data.columns)
     ]
 
+    _assert_categorical_obs(adata, key=cluster_key)
+    if interactions.empty:
+        raise ValueError("After filtering by genes, no interactions remain.")
     filtered_data = data.loc[
         :, list(set(interactions[SOURCE]) | set(interactions[TARGET]))
     ]
+    if len(adata.obs[cluster_key].cat.categories) <= 1:
+        raise ValueError(
+            f"Expected at least `2` clusters, found `{len(adata.obs[cluster_key].cat.categories)}`."
+        )
     filtered_data["clusters"] = (
         adata.obs.copy()[cluster_key].astype("string").astype("category").values
     )
     interactions.drop_duplicates(subset=(SOURCE, TARGET), inplace=True, keep="first")
     if clusters is None:
         clusters = list(map(str, adata.obs[cluster_key].cat.categories))
     if all(isinstance(c, str) for c in clusters):
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_moransi.py` & `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_moransi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import cupy as cp
 import math
 
 kernel_morans_I_num_dense = r"""
 extern "C" __global__
-void morans_I_num_dense(const float* data_centered, const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, 
+void morans_I_num_dense(const float* data_centered, const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind,
 const float* adj_matrix_data, float* num, int n_samples, int n_features) {
     int f = blockIdx.x * blockDim.x + threadIdx.x;
     int i = blockIdx.y * blockDim.y + threadIdx.y;
 
     if (i >= n_samples || f >= n_features) {
         return;
     }
```

### Comparing `rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_utils.py` & `rapids_singlecell-0.6.3/rapids_singlecell/squidpy_gpu/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Any,
     Dict,
     Union,
 )
 from scipy import stats
 from scipy.sparse import spmatrix, issparse
 import pandas as pd
+from pandas.api.types import infer_dtype, is_categorical_dtype
 
 
 ### Taken from squidpy: https://github.com/scverse/squidpy/blob/main/squidpy/gr/_ppatterns.py
 def _p_value_calc(
     score: np.ndarray,
     sims: Union[np.ndarray, None],
     weights: Union[spmatrix, np.ndarray],
@@ -198,7 +199,17 @@
         idx = IntIndex(n_rows, indices[sl], check_integrity=False)
         arr = SparseArray._simple_new(array_data[sl], idx, dtype)
         arrays.append(arr)
 
     return pd.DataFrame._from_arrays(
         arrays, columns=columns, index=index, verify_integrity=False
     )
+
+
+def _assert_categorical_obs(adata, key):
+    if key not in adata.obs:
+        raise KeyError(f"Cluster key `{key}` not found in `adata.obs`.")
+
+    if not is_categorical_dtype(adata.obs[key]):
+        raise TypeError(
+            f"Expected `adata.obs[{key!r}]` to be `categorical`, found `{infer_dtype(adata.obs[key])}`."
+        )
```

### Comparing `rapids_singlecell-0.6.2/PKG-INFO` & `rapids_singlecell-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids_singlecell
-Version: 0.6.2
+Version: 0.6.3
 Summary: running single cell analysis on Nvidia GPUs
 Author: Severin Dicks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: decoupler>=1.3.2
@@ -27,15 +27,15 @@
 [![PyPI](https://img.shields.io/pypi/v/rapids-singlecell?logo=PyPI)](https://pypi.org/project/rapids-singlecell)
 [![PyPIDownloads](https://pepy.tech/badge/rapids-singlecell)](https://pepy.tech/project/rapids-singlecell)
 [![Documentation Status](https://readthedocs.org/projects/rapids-singlecell/badge/?version=latest)](https://rapids-singlecell.readthedocs.io/en/latest/?badge=latest)
 
 # rapids-singlecell
 
 ## Background
-This repository offers some tools to make analyses of single cell datasets faster by running them on the GPU. 
+This repository offers some tools to make analyses of single cell datasets faster by running them on the GPU.
 The functions are analogous versions of functions that can be found within [scanpy](https://github.com/scverse/scanpy) from the Theis lab or functions from [rapids-single-cell-examples](https://github.com/clara-parabricks/rapids-single-cell-examples) created by the Nvidia RAPIDS team. Most functions are kept close to the original code to ensure compatibility. My aim with this repository was to use the speedup that GPU computing offers and combine it with the ease of use from scanpy.
 
 ## Installation
 ### Conda
 The easiest way to install *rapids-singlecell* is to use one of the *yaml* file provided in the [conda](https://github.com/Intron7/rapids_singlecell/tree/main/conda) folder. These *yaml* files install everything needed to run the example notbooks and get you started.
 ```
 conda env create -f conda/rsc_rapids_23.04.yml
@@ -73,15 +73,15 @@
 If you use the accelerated decoupler functions please cite [decoupler](https://doi.org/10.1093/bioadv/vbac016)
 
 ## Notebooks
 To show the capability of these functions, I created two example notebooks evaluating the same workflow running on the CPU and GPU. These notebooks should run in the environment, that is described in Requirements. First, run the `data_downloader` notebook to create the AnnData object for the analysis. If you run both `demo_cpu` and `demo_gpu` you should see a big speedup when running the analyses on the GPU.
 
 ## Benchmarks
 
-Here are some benchmarks. I ran the notebook on the CPU with as many cores as were available where possible. 
+Here are some benchmarks. I ran the notebook on the CPU with as many cores as were available where possible.
 
 |Step                          |CPU (Ryzen 5950x, 32 Cores, 64GB RAM)|GPU (RTX 3090)|CPU (AMD Eypc Rome, 30 Cores, 500GB RAM)| GPU (Quadro RTX 6000)|GPU (A100 80GB)|
 |------------------------------|---------------------------|--------------|----------|--------------|----------------|
 |whole Notebook                | 728 s                     | 43 s         | 917 s    | 67 s         | 57 s           |
 |Preprocessing                 | 75 s                      | 21 s         | 40 s     | 34 s         | 30 s           |
 |Clustering and Visulatization | 423 s                     | 18 s         | 524 s    | 27 s         | 21 s           |
 |Normalize_total               | 252 ms                    | > 1ms        | 425 ms   | 1 ms         | 1 ms           |
```

