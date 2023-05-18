# Comparing `tmp/hrcl_jobs-1.0.1.tar.gz` & `tmp/hrcl_jobs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrcl_jobs-1.0.1.tar", last modified: Mon May  1 14:12:13 2023, max compression
+gzip compressed data, was "hrcl_jobs-1.1.0.tar", last modified: Thu May 18 20:02:07 2023, max compression
```

## Comparing `hrcl_jobs-1.0.1.tar` & `hrcl_jobs-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.529474 hrcl_jobs-1.0.1/
--rw-r--r--   0 austinwallace   (501) staff       (20)     1803 2023-02-02 20:22:41.000000 hrcl_jobs-1.0.1/.gitignore
--rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-02-02 20:22:41.000000 hrcl_jobs-1.0.1/LICENSE
--rw-r--r--   0 austinwallace   (501) staff       (20)      962 2023-05-01 14:12:13.529631 hrcl_jobs-1.0.1/PKG-INFO
--rw-r--r--   0 austinwallace   (501) staff       (20)      342 2023-02-03 23:39:01.000000 hrcl_jobs-1.0.1/README.md
--rw-r--r--   0 austinwallace   (501) staff       (20)      116 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/main.py
--rw-r--r--   0 austinwallace   (501) staff       (20)      665 2023-05-01 14:11:50.000000 hrcl_jobs-1.0.1/pyproject.toml
--rw-r--r--   0 austinwallace   (501) staff       (20)      295 2023-05-01 14:12:13.530125 hrcl_jobs-1.0.1/setup.cfg
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.518910 hrcl_jobs-1.0.1/src/
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.526480 hrcl_jobs-1.0.1/src/hrcl_jobs/
--rw-r--r--   0 austinwallace   (501) staff       (20)      105 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/__init__.py
--rw-r--r--   0 austinwallace   (501) staff       (20)    14404 2023-02-02 20:22:41.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/data.py
--rw-r--r--   0 austinwallace   (501) staff       (20)      892 2023-05-01 14:11:35.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/jobspec.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     5818 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/parallel.py
--rw-r--r--   0 austinwallace   (501) staff       (20)    19831 2023-02-02 20:22:41.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/s22.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     2093 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/serial.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     9082 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/setup.py
--rw-r--r--   0 austinwallace   (501) staff       (20)    17798 2023-05-01 14:11:35.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/sqlt.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     2929 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs/tools_og.py
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.528047 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/
--rw-r--r--   0 austinwallace   (501) staff       (20)      962 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/PKG-INFO
--rw-r--r--   0 austinwallace   (501) staff       (20)      554 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)       69 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/requires.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)       10 2023-05-01 14:12:13.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/top_level.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-02-02 20:26:18.000000 hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/zip-safe
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-01 14:12:13.529103 hrcl_jobs-1.0.1/src/hrcl_jobs_psi4/
--rw-r--r--   0 austinwallace   (501) staff       (20)      842 2023-03-27 20:06:21.000000 hrcl_jobs-1.0.1/src/hrcl_jobs_psi4/jobspec.py
--rw-r--r--   0 austinwallace   (501) staff       (20)    22675 2023-03-30 13:05:54.000000 hrcl_jobs-1.0.1/src/hrcl_jobs_psi4/psi4_inps.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.095466 hrcl_jobs-1.1.0/
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1803 2023-02-02 20:22:41.000000 hrcl_jobs-1.1.0/.gitignore
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-02-02 20:22:41.000000 hrcl_jobs-1.1.0/LICENSE
+-rw-r--r--   0 austinwallace   (501) staff       (20)      962 2023-05-18 20:02:07.095976 hrcl_jobs-1.1.0/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      342 2023-02-03 23:39:01.000000 hrcl_jobs-1.1.0/README.md
+-rw-r--r--   0 austinwallace   (501) staff       (20)      116 2023-03-27 20:06:21.000000 hrcl_jobs-1.1.0/main.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      665 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/pyproject.toml
+-rw-r--r--   0 austinwallace   (501) staff       (20)      295 2023-05-18 20:02:07.097950 hrcl_jobs-1.1.0/setup.cfg
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.081689 hrcl_jobs-1.1.0/src/
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.088929 hrcl_jobs-1.1.0/src/hrcl_jobs/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      128 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    14403 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/data.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      968 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/examples.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      893 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     5861 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/parallel.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    20138 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/s22.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     2093 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/serial.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     9082 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/setup.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    19958 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/sqlt.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     2929 2023-03-27 20:06:21.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/tools_og.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.091304 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      962 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      704 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       69 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/requires.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       40 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/top_level.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-02-02 20:26:18.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/zip-safe
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.093088 hrcl_jobs-1.1.0/src/hrcl_jobs_orca/
+-rw-r--r--   0 austinwallace   (501) staff       (20)       24 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_orca/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      629 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_orca/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     2463 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_orca/orca_inps.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.094719 hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/
+-rw-r--r--   0 austinwallace   (501) staff       (20)       24 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      842 2023-03-27 20:06:21.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    24621 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/psi4_inps.py
```

### Comparing `hrcl_jobs-1.0.1/.gitignore` & `hrcl_jobs-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.1/LICENSE` & `hrcl_jobs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.1/PKG-INFO` & `hrcl_jobs-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrcl_jobs
-Version: 1.0.1
+Version: 1.1.0
 Summary: Runs python functions on worker threads with main thread communicating with sql db
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/hierarchical_python_jobs
 Project-URL: Bug Tracker, https://github.com/Awallace3/hierarchical_python_jobs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hrcl_jobs-1.0.1/pyproject.toml` & `hrcl_jobs-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hrcl_jobs"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Austin M. Wallace", email="awallace43@gatech.edu" },
 ]
 description = "Runs python functions on worker threads with main thread communicating with sql db"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs/data.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,18 +368,17 @@
     ind_neutralA_set = set(ind_neutralA)
     ind_neutralB_set = set(ind_neutralB)
     charge_neutral1 = ind_chargeA_set.intersection(ind_neutralB_set)
     charge_neutral2 = ind_chargeB_set.intersection(ind_neutralA_set)
     ind_charge_neutral = list(charge_neutral1.union(charge_neutral2))
 
     df["charge_diff"] = (df["TQA"] - df["TQB"]).abs()
-    df['sizeA'] = df.apply(lambda r: len(r['RA']), axis=1)
-    df['sizeB'] = df.apply(lambda r: len(r['RB']), axis=1)
-    df['sizeColor'] = df.apply(lambda r: size_shrink(r['sizeA'], r['sizeB']), axis=1)
-
+    df["sizeA"] = df.apply(lambda r: len(r["RA"]), axis=1)
+    df["sizeB"] = df.apply(lambda r: len(r["RB"]), axis=1)
+    df["sizeColor"] = df.apply(lambda r: size_shrink(r["sizeA"], r["sizeB"]), axis=1)
 
     neutral = df.copy(deep=True).loc[ind_neutral]
     charges_neutral = df.copy(deep=True).loc[ind_charge_neutral]
     charges = df.copy(deep=True).loc[ind_charge]
     anion = df.copy(deep=True).loc[ind_anion]
     df["ClassicalInd"] = df["static_q"] - df["static_q_vac"]
     # df.plot(x="Ind_aug", y="ClassicalInd", style="o", ms=0.5, use_index=True, label="")
@@ -423,18 +422,18 @@
     # )
     # anion["ClassicalInd"] = anion["static_q"] - anion["static_q_vac"]
     # anion.plot(
     #     x="Ind_aug", y="ClassicalInd", style="o", ms=0.5, use_index=True, label="anion"
     # )
 
     cmap = cm.get_cmap("Spectral")
-    x = df['Ind_aug'].tolist()
-    y = df['ClassicalInd'].tolist()
-    c = df['charge_diff'].tolist()
-    c = df['sizeColor'].tolist()
+    x = df["Ind_aug"].tolist()
+    y = df["ClassicalInd"].tolist()
+    c = df["charge_diff"].tolist()
+    c = df["sizeColor"].tolist()
     fig, ax = plt.subplots(1)
     scat = ax.scatter(x, y, c=c, cmap=cmap, s=0.5)
     plt.colorbar(scat)
     plt.ylabel("Ind_aug E (kcal/mol)")
     plt.xlabel("ClassicalInd (kcal/mol)")
     plt.savefig("size.png")
     # df.plot(
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs/jobspec.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs/jobspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 All dataclass_js should have id_label for ms_sl() usage to update sql db
 correctly
 
 TODO: make own repo to consume in both hrcl submodules
 """
 
+
 @dataclass
 class example_js:
     id_label: int
     val: float
 
 
 @dataclass
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs/parallel.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,17 @@
     """
     example_run_js_job
     """
     v1 = js.val + 1
     v2 = js.val + 2
     return [v1, v2]
 
-
+# READS n_procs from comm now
 def ms_sl(
     id_list=[0, 50],
-    n_procs=50,
     db_path="db/dimers_all.db",
     collect_ids_into_js_ls=collect_ids_into_js_ls,
     collect_id_into_js=collect_id_into_js,
     run_js_job=example_run_js_job,
     update_func=update_by_id,
     headers_sql=["main_id", "id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
     level_theory=["hf/aug-cc-pV(D+d)Z"],
@@ -59,14 +58,15 @@
     ```bash
     mpiexec -n 2 python3 -u main.py
     ```
     """
 
     comm = MPI.COMM_WORLD
     rank = comm.Get_rank()
+    n_procs = comm.Get_size()
     print("rank", rank)
     if rank == 0:
         jobs = len(id_list)
         start = time.time()
         first = True
         con, cur = establish_connection(db_p=db_path)
         cur_rows = []
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs/s22.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs/s22.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,73 @@
 def s22_testing() -> {}:
     """
     s22_testing
     """
     geoms = []
-   #  geoms.append("""
-   #  0 1
-   #  7  -1.578718  -0.046611   0.000000
-   #  1  -2.158621   0.136396  -0.809565
-   #  1  -2.158621   0.136396   0.809565
-   #  1  -0.849471   0.658193   0.000000
-   #  --
-   #  0 1
-   #  7   1.578718   0.046611   0.000000
-   #  1   2.158621  -0.136396  -0.809565
-   #  1   0.849471  -0.658193   0.000000
-   #  1   2.158621  -0.136396   0.809565    """
-   # )
-    geoms.append("""
+    #  geoms.append("""
+    #  0 1
+    #  7  -1.578718  -0.046611   0.000000
+    #  1  -2.158621   0.136396  -0.809565
+    #  1  -2.158621   0.136396   0.809565
+    #  1  -0.849471   0.658193   0.000000
+    #  --
+    #  0 1
+    #  7   1.578718   0.046611   0.000000
+    #  1   2.158621  -0.136396  -0.809565
+    #  1   0.849471  -0.658193   0.000000
+    #  1   2.158621  -0.136396   0.809565    """
+    # )
+    geoms.append(
+        """
     0 1
     8  -1.551007  -0.114520   0.000000
     1  -1.934259   0.762503   0.000000
     1  -0.599677   0.040712   0.000000
     --
     0 1
     8   1.350625   0.111469   0.000000
     1   1.680398  -0.373741  -0.758561
-    1   1.680398  -0.373741   0.758561    """)
-    geoms.append("""
+    1   1.680398  -0.373741   0.758561    """
+    )
+    geoms.append(
+        """
     0 1
     6  -1.888896  -0.179692   0.000000
     8  -1.493280   1.073689   0.000000
     8  -1.170435  -1.166590   0.000000
     1  -2.979488  -0.258829   0.000000
     1  -0.498833   1.107195   0.000000
     --
     0 1
     6   1.888896   0.179692   0.000000
     8   1.493280  -1.073689   0.000000
     8   1.170435   1.166590   0.000000
     1   2.979488   0.258829   0.000000
-    1   0.498833  -1.107195   0.000000    """)
-    geoms.append("""
+    1   0.498833  -1.107195   0.000000    """
+    )
+    geoms.append(
+        """
     0 1
     6  -2.018649   0.052883   0.000000
     8  -1.452200   1.143634   0.000000
     7  -1.407770  -1.142484   0.000000
     1  -1.964596  -1.977036   0.000000
     1  -0.387244  -1.207782   0.000000
     1  -3.117061  -0.013701   0.000000
     --
     0 1
     6   2.018649  -0.052883   0.000000
     8   1.452200  -1.143634   0.000000
     7   1.407770   1.142484   0.000000
     1   1.964596   1.977036   0.000000
     1   0.387244   1.207782   0.000000
-    1   3.117061   0.013701   0.000000    """)
-    geoms.append("""
+    1   3.117061   0.013701   0.000000    """
+    )
+    geoms.append(
+        """
     0 1
     8    -1.4663316    1.0121693    0.0000000
     6    -0.6281464    1.9142678    0.0000000
     7     0.7205093    1.6882688    0.0000000
     6     1.6367290    2.7052764    0.0000000
     6     1.2769036    4.0061763    0.0000000
     6    -0.1286005    4.3621549    0.0000000
@@ -79,16 +86,18 @@
     6    -1.2769036   -4.0061763    0.0000000
     6     0.1286005   -4.3621549    0.0000000
     7     0.9777230   -3.2396433    0.0000000
     8     0.5972229   -5.4864066    0.0000000
     1    -2.0103504   -4.7938642    0.0000000
     1    -1.0232515   -0.7061820    0.0000000
     1     1.9700268   -3.4323850    0.0000000
-    1    -2.6690620   -2.3883417    0.0000000    """)
-    geoms.append("""
+    1    -2.6690620   -2.3883417    0.0000000    """
+    )
+    geoms.append(
+        """
     0 1
     8    -1.3976213   -1.8858368   -0.3673061
     7    -1.4642550    0.3641828    0.0192301
     6    -4.1857398    0.3696669    0.0360960
     6    -3.4832598    1.5783111    0.2500752
     6    -2.1179502    1.5307048    0.2338383
     6    -2.0773833   -0.8637492   -0.1899414
@@ -108,16 +117,18 @@
     6     2.1280138    1.4953324   -0.2175374
     1     4.0459206   -1.7361356    0.3076883
     1     5.2999426    0.3666009   -0.0663349
     1     4.0110923    2.5024313   -0.4130052
     1     1.5339878    2.3893837   -0.3670565
     7     1.3883123   -1.9083038    0.4198149
     1     1.8694714   -2.7812773    0.2940385
-    1     0.4089067   -1.9079942    0.1300860    """)
-    geoms.append("""
+    1     0.4089067   -1.9079942    0.1300860    """
+    )
+    geoms.append(
+        """
     0 1
     7     0.9350155   -0.0279801   -0.3788916
     6     1.6739638   -0.0357766    0.7424316
     6     3.0747955   -0.0094480    0.5994562
     6     3.5646109    0.0195446   -0.7059872
     7     2.8531510    0.0258031   -1.8409596
     6     1.5490760    0.0012569   -1.5808009
@@ -142,46 +153,52 @@
     8    -1.8674730    0.0112093    1.9120833
     8    -1.9416783   -0.0291878   -2.6573783
     1    -4.4017172   -0.0036078   -2.4004924
     1    -0.8838255   -0.0216168   -0.3784269
     1    -5.6909220    0.0269347   -0.4227183
     1    -4.4439282   -0.8302573    2.7695655
     1    -4.4267056    0.9186178    2.7530256
-    1    -5.7883971    0.0505530    2.0247280    """)
-    geoms.append("""
+    1    -5.7883971    0.0505530    2.0247280    """
+    )
+    geoms.append(
+        """
     0 1
     6   0.000000  -0.000140   1.859161
     1  -0.888551   0.513060   1.494685
     1   0.888551   0.513060   1.494685
     1   0.000000  -1.026339   1.494868
     1   0.000000   0.000089   2.948284
     --
     0 1
     6   0.000000   0.000140  -1.859161
     1   0.000000  -0.000089  -2.948284
     1  -0.888551  -0.513060  -1.494685
     1   0.888551  -0.513060  -1.494685
-    1   0.000000   1.026339  -1.494868    """)
-    geoms.append("""
+    1   0.000000   1.026339  -1.494868    """
+    )
+    geoms.append(
+        """
     0 1
     6  -0.471925  -0.471925  -1.859111
     6   0.471925   0.471925  -1.859111
     1  -0.872422  -0.872422  -0.936125
     1   0.872422   0.872422  -0.936125
     1  -0.870464  -0.870464  -2.783308
     1   0.870464   0.870464  -2.783308
     --
     0 1
     6  -0.471925   0.471925   1.859111
     6   0.471925  -0.471925   1.859111
     1  -0.872422   0.872422   0.936125
     1   0.872422  -0.872422   0.936125
     1  -0.870464   0.870464   2.783308
-    1   0.870464  -0.870464   2.783308    """)
-    geoms.append("""
+    1   0.870464  -0.870464   2.783308    """
+    )
+    geoms.append(
+        """
     0 1
     6     1.3932178    0.0362913   -0.6332803
     6     0.7280364   -1.1884015   -0.6333017
     6    -0.6651797   -1.2247077   -0.6332803
     6    -1.3932041   -0.0362972   -0.6333017
     6    -0.7280381    1.1884163   -0.6332803
     6     0.6651677    1.2246987   -0.6333017
@@ -193,16 +210,18 @@
     1     1.1813026    2.1750056   -0.6317401
     --
     0 1
     6     0.0000000    0.0000000    3.0826195
     1     0.5868776    0.8381742    3.4463772
     1    -1.0193189    0.0891638    3.4463772
     1     0.0000000    0.0000000    1.9966697
-    1     0.4324413   -0.9273380    3.4463772    """)
-    geoms.append("""
+    1     0.4324413   -0.9273380    3.4463772    """
+    )
+    geoms.append(
+        """
     0 1
     6    -1.0478252   -1.4216736    0.0000000
     6    -1.4545034   -0.8554459    1.2062048
     6    -1.4545034   -0.8554459   -1.2062048
     6    -2.2667970    0.2771610    1.2069539
     6    -2.6714781    0.8450211    0.0000000
     6    -2.2667970    0.2771610   -1.2069539
@@ -221,16 +240,18 @@
     6     2.6714781   -0.8450211    0.0000000
     6     2.2667970   -0.2771610    1.2069539
     1     0.4060253    2.2919049    0.0000000
     1     1.1338534    1.2920593    2.1423150
     1     2.5824943   -0.7163066    2.1437977
     1     3.3030422   -1.7232700    0.0000000
     1     2.5824943   -0.7163066   -2.1437977
-    1     1.1338534    1.2920593   -2.1423150    """)
-    geoms.append("""
+    1     1.1338534    1.2920593   -2.1423150    """
+    )
+    geoms.append(
+        """
     0 1
     6    -1.2471894   -1.1718212   -0.6961388
     6    -1.2471894   -1.1718212    0.6961388
     7    -0.2589510   -1.7235771    1.4144796
     6     0.7315327   -2.2652221    0.6967288
     6     0.7315327   -2.2652221   -0.6967288
     7    -0.2589510   -1.7235771   -1.4144796
@@ -245,16 +266,18 @@
     7     1.4701787    0.9907598    0.0000000
     6     0.8540254    1.3593471   -1.1306308
     6    -0.3380031    2.0800608   -1.1300452
     7    -0.9523059    2.4528836    0.0000000
     1    -0.8103758    2.3643033    2.0618643
     1     1.3208583    1.0670610    2.0623986
     1     1.3208583    1.0670610   -2.0623986
-    1    -0.8103758    2.3643033   -2.0618643    """)
-    geoms.append("""
+    1    -0.8103758    2.3643033   -2.0618643    """
+    )
+    geoms.append(
+        """
     0 1
     7     2.0113587   -1.2132073   -0.0980673
     6     2.0257076   -0.6971797   -1.3644029
     1     2.2975208   -1.3910592   -2.1456459
     6     1.7145226    0.5919651   -1.6124892
     1     1.7272873    0.9908466   -2.6120050
     6     1.3089605    1.4575340   -0.5205890
@@ -273,16 +296,18 @@
     1    -1.7272873   -0.9908466   -2.6120050
     6    -1.3089605   -1.4575340   -0.5205890
     8    -0.9205926   -2.6110864   -0.6260457
     7    -1.3768885   -0.8397454    0.7346356
     1    -1.0518040   -1.3862229    1.5233710
     6    -1.6459909    0.4852113    1.0187267
     8    -1.5611090    0.9718061    2.1298059
-    1    -2.1294635    2.2015046    0.0568134    """)
-    geoms.append("""
+    1    -2.1294635    2.2015046    0.0568134    """
+    )
+    geoms.append(
+        """
     0 1
     6    -0.0210742    1.5318615   -1.3639345
     6    -1.2746794    0.9741030   -1.6074097
     6    -1.3783055   -0.2256981   -2.3084154
     6    -0.2289426   -0.8664053   -2.7687944
     6     1.0247882   -0.3035171   -2.5312410
     6     1.1289996    0.8966787   -1.8299830
@@ -305,16 +330,18 @@
     7     1.5646462   -1.2137812    0.7555384
     6     0.2861214   -0.8269486    1.0618752
     6    -0.9284667   -1.4853121    0.8606937
     1    -0.9729200   -2.4554847    0.3834013
     6    -2.0792848   -0.8417668    1.2876443
     1    -3.0389974   -1.3203846    1.1468400
     1     1.8075741   -2.0366963    0.2333038
-    1     3.5028794   -0.3485344    0.9695233    """)
-    geoms.append("""
+    1     3.5028794   -0.3485344    0.9695233    """
+    )
+    geoms.append(
+        """
     0 1
     7     0.2793014    2.4068393   -0.6057517
     6    -1.0848570    2.4457461   -0.5511608
     1    -1.6594403    3.0230294   -1.2560905
     7    -1.5977117    1.7179877    0.4287543
     6    -0.4897255    1.1714358    1.0301910
     6    -0.3461366    0.2914710    2.1172343
@@ -339,30 +366,34 @@
     1     1.5112443   -3.3572767    0.9513659
     6    -0.9684711   -1.5298112   -0.5939792
     8    -2.0029280   -1.8396957   -0.0199453
     7    -0.9956916   -0.6383870   -1.6720420
     1    -1.9014057   -0.2501720   -1.8985760
     6     0.0684702   -0.1191762   -2.3763759
     8    -0.0397875    0.7227006   -3.2531083
-    1     2.0853289   -0.2760176   -2.4454577    """)
-    geoms.append("""
+    1     2.0853289   -0.2760176   -2.4454577    """
+    )
+    geoms.append(
+        """
     0 1
     6   0.000000  -0.667578  -2.124659
     6   0.000000   0.667578  -2.124659
     1   0.923621  -1.232253  -2.126185
     1  -0.923621  -1.232253  -2.126185
     1  -0.923621   1.232253  -2.126185
     1   0.923621   1.232253  -2.126185
     --
     0 1
     6   0.000000   0.000000   2.900503
     6   0.000000   0.000000   1.693240
     1   0.000000   0.000000   0.627352
-    1   0.000000   0.000000   3.963929    """)
-    geoms.append("""
+    1   0.000000   0.000000   3.963929    """
+    )
+    geoms.append(
+        """
     0 1
     6     0.7806117   -0.6098875   -1.2075426
     6     0.4784039    0.7510406   -1.2079040
     6     0.3276592    1.4318573    0.0000000
     6     0.4784039    0.7510406    1.2079040
     6     0.7806117   -0.6098875    1.2075426
     6     0.9321510   -1.2899614    0.0000000
@@ -372,16 +403,18 @@
     1     0.3573895    1.2782091    2.1440546
     1     0.8966688   -1.1376051    2.1441482
     1     1.1690064   -2.3451668    0.0000000
     --
     0 1
     8    -2.7885270   -0.2744854    0.0000000
     1    -2.6229114   -1.2190831    0.0000000
-    1    -1.9015103    0.0979110    0.0000000    """)
-    geoms.append("""
+    1    -1.9015103    0.0979110    0.0000000    """
+    )
+    geoms.append(
+        """
     0 1
     6    -0.7392810    0.5158785   -1.2071079
     6    -1.4261442    0.3965455    0.0000000
     6    -0.7392810    0.5158785    1.2071079
     6     0.6342269    0.7546398    1.2070735
     6     1.3210434    0.8737566    0.0000000
     6     0.6342269    0.7546398   -1.2070735
@@ -392,16 +425,18 @@
     1     2.3863585    1.0596312    0.0000000
     1     1.1668005    0.8474885   -2.1436950
     --
     0 1
     7     0.1803930   -2.9491231    0.0000000
     1     0.7595495   -3.1459477   -0.8060729
     1     0.7595495   -3.1459477    0.8060729
-    1     0.0444167   -1.9449399    0.0000000    """)
-    geoms.append("""
+    1     0.0444167   -1.9449399    0.0000000    """
+    )
+    geoms.append(
+        """
     0 1
     6    -0.7097741   -0.9904230    1.2077018
     6    -1.4065340   -0.9653529    0.0000000
     6    -0.7097741   -0.9904230   -1.2077018
     6     0.6839651   -1.0405105   -1.2078652
     6     1.3809779   -1.0655522    0.0000000
     6     0.6839651   -1.0405105    1.2078652
@@ -411,16 +446,18 @@
     1     1.2242882   -1.0580753   -2.1442563
     1     2.4615886   -1.1029818    0.0000000
     1     1.2242882   -1.0580753    2.1442563
     --
     0 1
     7    -0.0034118    3.5353926    0.0000000
     6     0.0751963    2.3707040    0.0000000
-    1     0.1476295    1.3052847    0.0000000    """)
-    geoms.append("""
+    1     0.1476295    1.3052847    0.0000000    """
+    )
+    geoms.append(
+        """
     0 1
     6     0.0000000    0.0000000    1.0590353
     6     0.0000000   -1.2060084    1.7576742
     6     0.0000000   -1.2071767    3.1515905
     6     0.0000000    0.0000000    3.8485751
     6     0.0000000    1.2071767    3.1515905
     6     0.0000000    1.2060084    1.7576742
@@ -439,16 +476,18 @@
     6     0.6970468   -1.2072378   -2.4546277
     6    -0.6970468   -1.2072378   -2.4546277
     1    -2.4753995    0.0000000   -2.4503221
     1    -1.2382321    2.1435655   -2.4536764
     1     1.2382321    2.1435655   -2.4536764
     1     2.4753995    0.0000000   -2.4503221
     1     1.2382321   -2.1435655   -2.4536764
-    1    -1.2382321   -2.1435655   -2.4536764    """)
-    geoms.append("""
+    1    -1.2382321   -2.1435655   -2.4536764    """
+    )
+    geoms.append(
+        """
     0 1
     6     2.5118997    1.6250148    0.0000000
     6     2.7130094    0.9578537   -1.2082918
     6     3.1177821   -0.3767436   -1.2083647
     6     3.3213848   -1.0437307    0.0000000
     6     3.1177821   -0.3767436    1.2083647
     6     2.7130094    0.9578537    1.2082918
@@ -471,16 +510,18 @@
     6    -3.8054511    1.0974790    0.0000000
     6    -3.6798167   -0.2817209    0.0000000
     1     0.2310024   -2.8653173    0.0000000
     1    -2.4585759   -3.0956052    0.0000000
     1    -0.5188733    2.0539520    0.0000000
     1    -2.8077570    3.0097859    0.0000000
     1    -4.7905991    1.5439372    0.0000000
-    1    -4.5580187   -0.9142916    0.0000000    """)
-    geoms.append("""
+    1    -4.5580187   -0.9142916    0.0000000    """
+    )
+    geoms.append(
+        """
     0 1
     6    -2.0071056    0.7638459   -0.1083509
     8    -1.3885044    1.9298523   -0.4431206
     1    -0.5238121    1.9646519   -0.0064609
     6    -1.4630807   -0.1519120    0.7949930
     6    -2.1475789   -1.3295094    1.0883677
     6    -3.3743208   -1.6031427    0.4895864
@@ -501,9 +542,10 @@
     6     3.3315674   -1.5665603   -0.5748636
     6     3.7696838   -0.8396901    0.5286439
     6     3.1224836    0.3383498    0.8960491
     1     0.7445512    0.4367983   -1.5218583
     1     1.8921463   -1.6649726   -2.1701843
     1     3.8330227   -2.4811537   -0.8566666
     1     4.6137632   -1.1850101    1.1092635
-    1     3.4598854    0.9030376    1.7569489    """)
+    1     3.4598854    0.9030376    1.7569489    """
+    )
     return geoms
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs/serial.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs/serial.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,30 @@
     update_mp_rows,
     update_rows,
     collect_rows_into_js_ls_mp,
     collect_row_specific_into_js_mp,
     read_example_output,
     collect_id_into_js,
     update_by_id,
-
 )
 import os
 from glob import glob
 import time
 from .jobspec import example_js
 
+
 def example_run_js_job(js: example_js) -> float:
     """
     example_run_js_job
     """
     v1 = js.val + 1
     v2 = js.val + 2
     return [v1, v2]
 
+
 def ms_sl_serial(
     id_list=[0, 50],
     db_path="db/dimers_all.db",
     collect_id_into_js=collect_id_into_js,
     run_js_job=example_run_js_job,
     update_func=update_by_id,
     headers_sql=["main_id", "id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
@@ -75,8 +76,7 @@
             id_value=active_ind,
             table=table,
             output_columns=output_columns,
         )
     print((time.time() - start) / 60, "Minutes")
     print("COMPLETED MAIN")
     return
-
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs/setup.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,14 @@
         db_p=db_p,
         input_columns=input_columns,
         output_columns=output_columns,
     )
     return
 
 
-
 def test_db(db_p="db/test.db") -> None:
     """
     test_db for saptdft
     """
     input_columns = {
         "monAs": "array",
         "monBs": "array",
@@ -196,31 +195,32 @@
         df_p="data/test.pkl",
         db_p=db_p,
         input_columns=input_columns,
         output_columns=output_columns,
     )
     return
 
+
 def test_db_2(db_p="db/test2.db") -> None:
     """
     test_db for saptdft
     """
     geos = s22_testing()
     geoms = [string_carts_to_np(i) for i in geos]
     d = {
         "monAs": [],
         "monBs": [],
         "Geometry": [],
         "charges": [],
     }
     for i in geoms:
-        d['Geometry'].append(i[0])
-        d['charges'].append(i[1])
-        d['monAs'].append(i[2])
-        d['monBs'].append(i[3])
+        d["Geometry"].append(i[0])
+        d["charges"].append(i[1])
+        d["monAs"].append(i[2])
+        d["monBs"].append(i[3])
     df = pd.DataFrame(d)
     df.to_pickle("data/test2.pkl")
 
     input_columns = {
         "monAs": "array",
         "monBs": "array",
         "Geometry": "array",
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs/sqlt.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs/sqlt.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,35 +57,34 @@
         "out": "array",
     },
 ):
     conn, cur = establish_connection(db_path)
     headers = ",\n".join([f"{k} {v}" for k, v in table.items()])
     if not conn:
         return
-    table_format = f""" CREATE TABLE IF NOT EXISTS {table_name} (
+    table_format = f""" CREATE TABLE {table_name} (
             {headers}
             );"""
-    # print(table_format)
-    create_table(conn, table_format)
-    return
+    return create_table(conn, table_format)
 
 
 def create_table(conn, create_table_sql):
     """create a table from the create_table_sql statement
     :param conn: Connection object
     :param create_table_sql: a CREATE TABLE statement
     :return:
     """
     try:
         c = conn.cursor()
         c.execute(create_table_sql)
-    except Error as e:
-        # print("\nTable already exists. Skipping generation\n")
+    except sql.OperationalError as e:
+        # print("TABLE ALREADY EXISTS. SKIPPING GENERATION\n")
         print(e)
-    return
+        return False
+    return True
 
 
 def create_new_db(
     db_name="db/main.db",
     table_name="main",
     table={
         "Dimer": "TEXT",
@@ -124,15 +123,17 @@
     """
     convert_df_into_sql
     """
     con = sql.connect("db/dimers.db", detect_types=sql.PARSE_DECLTYPES)
     cur = con.cursor()
     x = np.arange(18).reshape(3, 6)
     cur.execute("DROP TABLE IF EXISTS test2")
-    cur.execute("create table test2 (id INTEGER PRIMARY KEY AUTOINCREMENT, arr array)")
+    cur.execute(
+        "create table test2 (id INTEGER PRIMARY KEY AUTOINCREMENT, arr array)"
+    )
     cur.execute("insert into test2 (arr) values (?)", (x,))
     cur.execute("select arr from test2")
     data = cur.fetchone()[0]
     return data
 
 
 def insert_new_row(
@@ -342,16 +343,16 @@
     cmd = f"""
         UPDATE {table}
         SET
             {headers}
         WHERE
             {id_label}=?;
     """
-    print(cmd)
-    print("OUTPUT:", (*tuple(output), id_value))
+    # print(cmd)
+    # print("OUTPUT:", (*tuple(output), id_value))
     cursor.execute(
         cmd,
         (*tuple(output), id_value),
     )
     conn.commit()
     return
 
@@ -477,33 +478,71 @@
     return js
 
 
 def return_id_list(cur, column, table_name, id_name="id", values=[0]) -> [int]:
     """
     return_id_list queries db for matches with column and returns id
     """
+    op = "="
     if len(values) == 1:
-        sql_cmd = (
-            f"""SELECT {id_name} FROM {table_name} WHERE {column}=={values[0]};"""
-        )
+        if values[0] == "NULL":
+            op = " IS "
+        sql_cmd = f"""SELECT {id_name} FROM {table_name} WHERE {column}{op}{values[0]};"""
     else:
-        sql_cmd = (
-            f"""SELECT {id_name} FROM {table_name} WHERE {column} IN {tuple(values)};"""
-        )
+        sql_cmd = f"""SELECT {id_name} FROM {table_name} WHERE {column} IN {tuple(values)};"""
     cur.execute(sql_cmd)
     id_list = [i for i, *_ in cur.fetchall()]
     return id_list
 
+def query_clean_match(m):
+    """
+    query_clean_match
+    """
+    if type(m[0]) == str:
+        m = [f'"{i}"' for i in m]
+    return m
+
+
+def query_columns_for_values(cur, table_name, id_names=["id"], matches={
+    "id": [0],
+    }) -> [int]:
+    """
+    return_id_list queries db for matches with column and returns id
+    """
+    if type(id_names) == str:
+        id_name = id_names
+    else:
+        id_name = ", ".join(id_names)
+    if len(matches) > 0:
+        where_match = []
+        for k, v in matches.items():
+            v = query_clean_match(v)
+            if len(v) == 1:
+                m = f'{k}=={v[0]}'
+            else:
+                m = f"{k} IN {tuple(v)}"
+            where_match.append(m)
+        wm = " AND ".join(where_match)
+        sql_cmd = f"""SELECT {id_name} FROM {table_name} WHERE {wm};"""
+    else:
+        sql_cmd = f"""SELECT {id_name} FROM {table_name};"""
+    print(sql_cmd)
+    cur.execute(sql_cmd)
+    val_list = [i for i in cur.fetchall()]
+    for i in range(len(val_list)):
+        if len(val_list[i]) == 1:
+            val_list[i] = val_list[i][0]
+    return val_list
+
+
 def return_id_list_full_table(cur, table_name, id_name="id") -> [int]:
     """
     return_id_list queries db for matches with column and returns id
     """
-    sql_cmd = (
-        f"""SELECT {id_name} FROM {table_name};"""
-    )
+    sql_cmd = f"""SELECT {id_name} FROM {table_name};"""
     cur.execute(sql_cmd)
     id_list = [i for i, *_ in cur.fetchall()]
     return id_list
 
 
 def collect_ids_into_ls(
     cursor: object,
@@ -532,56 +571,73 @@
     table="main",
 ) -> []:
     """
     collect_rows collects a range of rows for a table with requested headers.
     The headers list must match the dataclass_obj's fields.
     """
     cols = ", ".join(headers)
-    sql_cmd = (
-        f"""SELECT {cols} FROM {table} WHERE {table}.{id_label} IN {tuple(id_list)};"""
-    )
+    sql_cmd = f"""SELECT {cols} FROM {table} WHERE {table}.{id_label} IN {tuple(id_list)};"""
     cursor.execute(sql_cmd)
     js_ls = [
         dataclass_obj(
             *i,
             extra_info,
             mem=mem,
         )
         for i in cursor.fetchall()
     ]
     return js_ls
 
+
+def collect_all_table_values_into_ls(
+    cursor: object,
+    headers: [] = ["id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
+    id_list: [] = [0, 1],
+    id_label: str = "id",
+    table="tcase",
+    process_func=None,
+) -> []:
+    """
+    collect_rows collects a range of rows for a table with requested headers.
+    The headers list must match the dataclass_obj's fields.
+    """
+    cols = ", ".join(headers)
+    sql_cmd = f"""SELECT {cols} FROM {table};"""
+    cursor.execute(sql_cmd)
+    if process_func:
+        ls = [process_func(i) for i in cursor.fetchall()]
+    else:
+        ls = [i for i in cursor.fetchall()]
+    return ls
+
+
 def collect_ids_into_ls(
     cursor: object,
     headers: [] = ["id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
     id_list: [] = [0, 1],
     id_label: str = "id",
     table="tcase",
     process_func=None,
 ) -> []:
     """
     collect_rows collects a range of rows for a table with requested headers.
     The headers list must match the dataclass_obj's fields.
     """
     cols = ", ".join(headers)
     sql_cmd = (
-        f"""SELECT {cols} FROM {table} WHERE {table}.{id_label} IN {tuple(id_list)};"""
+        f"""SELECT {cols} FROM {table} WHERE {id_label} IN {tuple(id_list)};"""
     )
     cursor.execute(sql_cmd)
     if process_func:
-        ls = [
-            process_func(i)
-            for i in cursor.fetchall()
-        ]
+        ls = [process_func(i) for i in cursor.fetchall()]
     else:
-        ls = [
-                i for i in cursor.fetchall()
-        ]
+        ls = [i for i in cursor.fetchall()]
     return ls
 
+
 def collect_rows_into_js_ls_mp(
     cursor: object,
     headers: [] = ["main_id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
     mem: str = "4gb",
     extra_info: [] = ["hf/aug-cc-pV(D+d)Z"],
     dataclass_obj: mp_js = mp_js,
     v_range: [] = [0, 2],
@@ -625,15 +681,17 @@
 def select_table_by_column_match(
     cursor: object,
     selection="*",
     column="id",
     value="'CCCxNXdO-1_acc-carbonyl_CCxdOXNc1nccynHY1_H-Narom_37_0.73_175_29_132_25_93'",
     table="main",
 ):
-    sql_cmd = f"""SELECT {selection} FROM {table} WHERE {table}.{column}={value};"""
+    sql_cmd = (
+        f"""SELECT {selection} FROM {table} WHERE {table}.{column}={value};"""
+    )
     cursor.execute(sql_cmd)
     return cursor.fetchall()
 
 
 def table_to_df_pkl(
     db_p="db/dimers_all.db",
     table="main",
@@ -647,15 +705,15 @@
     con, cur = establish_connection(db_p)
     if id_list:
         cmd = f"""SELECT * FROM {table} WHERE {table}.{id_label} IN {tuple(id_list)};"""
         print(cmd)
         df = pd.read_sql_query(cmd, con)
     else:
         df = pd.read_sql_query(f"SELECT * from {table};", con)
-    print(df.head())
+    print(df)
     df.to_pickle(df_p)
     print(df.columns)
     return
 
 
 def read_example_output(db_path="db/dimers.db", row_range=[0, 1]) -> None:
     """
@@ -681,7 +739,29 @@
     con, cur = establish_connection(db_path)
     r = collect_ids_into_ls(
         cur, id_list=id_list, id_label=id_label, table=table, outputs=outputs
     )
     for n, i in enumerate(r):
         print(f"main_id: {id_list[n]}, \t{list(i)[-5:-1]}")
     return
+
+
+def delete_rows_by_search(
+    con,
+    table_name: str,
+    column: str,
+    values: [],
+) -> None:
+    """
+    delete_rows_by_id
+    """
+    cur = con.cursor()
+    if len(values) == 1:
+        sql_cmd = f"""DELETE FROM {table_name} WHERE {column}=={values[0]};"""
+        print(sql_cmd)
+    else:
+        sql_cmd = (
+            f"""DELETE FROM {table_name} WHERE {column} IN {tuple(values)};"""
+        )
+    cur.execute(sql_cmd)
+    con.commit()
+    return
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs/tools_og.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs/tools_og.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/PKG-INFO` & `hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrcl-jobs
-Version: 1.0.1
+Version: 1.1.0
 Summary: Runs python functions on worker threads with main thread communicating with sql db
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/hierarchical_python_jobs
 Project-URL: Bug Tracker, https://github.com/Awallace3/hierarchical_python_jobs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs.egg-info/SOURCES.txt` & `hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 LICENSE
 README.md
 main.py
 pyproject.toml
 setup.cfg
 src/hrcl_jobs/__init__.py
 src/hrcl_jobs/data.py
+src/hrcl_jobs/examples.py
 src/hrcl_jobs/jobspec.py
 src/hrcl_jobs/parallel.py
 src/hrcl_jobs/s22.py
 src/hrcl_jobs/serial.py
 src/hrcl_jobs/setup.py
 src/hrcl_jobs/sqlt.py
 src/hrcl_jobs/tools_og.py
 src/hrcl_jobs.egg-info/PKG-INFO
 src/hrcl_jobs.egg-info/SOURCES.txt
 src/hrcl_jobs.egg-info/dependency_links.txt
 src/hrcl_jobs.egg-info/requires.txt
 src/hrcl_jobs.egg-info/top_level.txt
 src/hrcl_jobs.egg-info/zip-safe
+src/hrcl_jobs_orca/__init__.py
+src/hrcl_jobs_orca/jobspec.py
+src/hrcl_jobs_orca/orca_inps.py
+src/hrcl_jobs_psi4/__init__.py
 src/hrcl_jobs_psi4/jobspec.py
 src/hrcl_jobs_psi4/psi4_inps.py
```

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs_psi4/jobspec.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/jobspec.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.0.1/src/hrcl_jobs_psi4/psi4_inps.py` & `hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/psi4_inps.py`

 * *Files 3% similar despite different names*

```diff
@@ -736,7 +736,70 @@
             DISP = psi4.core.variable("SAPT DISP ENERGY")
             out_energies = np.array([e, ELST, EXCH, IND, DISP]) * mult
             es.append(out_energies)
         else:
             es.append(np.array([e * mult]))
         psi4.core.clean()
     return es
+
+def run_mp_js_grimme_components(js: grimme_js) -> np.array:
+    """
+    create_mp_js_grimme turns mp_js object into a psi4 job and runs it
+    """
+    ma, mb = [], []
+    for i in js.monAs:
+        ma.append(js.geometry[i, :])
+    for i in js.monBs:
+        mb.append(js.geometry[i, :])
+    ma = np_carts_to_string(ma)
+    mb = np_carts_to_string(mb)
+    ies = run_psi4_sapt0_components(
+        ma,
+        mb,
+        ppm=js.mem,
+        level_theory=js.level_theory,
+    )
+    return ies
+
+def run_psi4_sapt0_components(
+    A: str,
+    B: str,
+    ppm: str = "4 gb",
+    level_theory: [] = ["hf/cc-pvdz"],
+    charge_mult: np.array = np.array([[0, 1], [0, 1], [0, 1]]),
+    d_convergence: int = 4,
+    scf_type="df",
+) -> []:
+    A_cm = charge_mult[1, :]
+    B_cm = charge_mult[2, :]
+    geom = f"{A_cm[0]} {A_cm[1]}\n{A}--\n{A_cm[0]} {A_cm[1]}\n{B}"
+    es = []
+    for l in level_theory:
+        mol = psi4.geometry(geom)
+        psi4.set_memory(ppm)
+        psi4.set_options(
+            {
+                "d_convergence": d_convergence,
+                "freeze_core": "True",
+                "guess": "sad",
+                "scf_type": scf_type,
+                # "cholesky_tolerance": 1e-6 # default about 1e-4
+                # check psi4/src/read_options
+            }
+        )
+        psi4.core.be_quiet()
+        e = psi4.energy(f"{l}")
+
+        e *= constants.conversion_factor("hartree", "kcal / mol")
+        # print(psi4.core.variables())
+
+        ELST = psi4.core.variable("SAPT ELST ENERGY")
+        EXCH = psi4.core.variable("SAPT EXCH ENERGY")
+        IND = psi4.core.variable("SAPT IND ENERGY")
+        DISP = psi4.core.variable("SAPT DISP ENERGY")
+        ie = sum([ELST, EXCH, IND, DISP])
+        mult = constants.conversion_factor("hartree", "kcal / mol")
+        out_energies = np.array([ie, ELST, EXCH, IND, DISP]) * mult
+        # es.append(ie)
+        es.append(out_energies)
+        psi4.core.clean()
+    return es
```

