# Comparing `tmp/pyrle-0.0.8.tar.gz` & `tmp/pyrle-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrle-0.0.8.tar", last modified: Tue Jun  5 11:06:51 2018, max compression
+gzip compressed data, was "dist/pyrle-0.0.9.tar", last modified: Tue Jun  5 13:21:42 2018, max compression
```

## Comparing `pyrle-0.0.8.tar` & `pyrle-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 endrebak   (501) staff       (20)        0 2018-06-05 11:06:51.000000 pyrle-0.0.8/
-drwxr-xr-x   0 endrebak   (501) staff       (20)        0 2018-06-05 11:06:50.000000 pyrle-0.0.8/tests/
--rw-r--r--   0 endrebak   (501) staff       (20)     6188 2018-05-23 12:49:27.000000 pyrle-0.0.8/tests/test_coverage.py
--rw-r--r--   0 endrebak   (501) staff       (20)      819 2018-06-04 11:28:43.000000 pyrle-0.0.8/tests/test_inverse.py
--rw-r--r--   0 endrebak   (501) staff       (20)     1311 2018-05-23 12:49:29.000000 pyrle-0.0.8/tests/test_operations_GRles.py
--rw-r--r--   0 endrebak   (501) staff       (20)     5123 2018-06-04 12:54:11.000000 pyrle-0.0.8/tests/test_div.py
--rw-r--r--   0 endrebak   (501) staff       (20)        0 2018-05-23 12:49:26.000000 pyrle-0.0.8/tests/__init__.py
--rw-r--r--   0 endrebak   (501) staff       (20)     3619 2018-05-23 12:49:29.000000 pyrle-0.0.8/tests/test_subtract.py
--rw-r--r--   0 endrebak   (501) staff       (20)     8765 2018-05-23 12:49:28.000000 pyrle-0.0.8/tests/test_GRles.py
--rw-r--r--   0 endrebak   (501) staff       (20)     2612 2018-06-04 09:58:54.000000 pyrle-0.0.8/tests/test_add.py
--rw-r--r--   0 endrebak   (501) staff       (20)     1025 2018-05-23 12:49:28.000000 pyrle-0.0.8/tests/test_mul.py
--rw-r--r--   0 endrebak   (501) staff       (20)     1087 2018-04-25 12:19:48.000000 pyrle-0.0.8/README.md
-drwxr-xr-x   0 endrebak   (501) staff       (20)        0 2018-06-05 11:06:41.000000 pyrle-0.0.8/pyrle/
--rw-r--r--   0 endrebak   (501) staff       (20)      185 2018-05-23 12:49:24.000000 pyrle-0.0.8/pyrle/__init__.py
--rw-r--r--   0 endrebak   (501) staff       (20)     4502 2018-05-24 10:06:01.000000 pyrle-0.0.8/pyrle/methods.py
-drwxr-xr-x   0 endrebak   (501) staff       (20)        0 2018-06-05 11:06:47.000000 pyrle-0.0.8/pyrle/src/
--rw-r--r--   0 endrebak   (501) staff       (20)   852480 2018-05-23 12:35:08.000000 pyrle-0.0.8/pyrle/src/coverage.c
--rw-r--r--   0 endrebak   (501) staff       (20)     4691 2018-05-23 12:34:51.000000 pyrle-0.0.8/pyrle/src/coverage.pyx
--rw-r--r--   0 endrebak   (501) staff       (20)        0 2018-05-23 12:49:25.000000 pyrle-0.0.8/pyrle/src/__init__.py
--rw-r--r--   0 endrebak   (501) staff       (20)    14552 2018-06-05 10:57:51.000000 pyrle-0.0.8/pyrle/src/rle.pyx
--rw-r--r--   0 endrebak   (501) staff       (20)  1038679 2018-06-05 11:06:04.000000 pyrle-0.0.8/pyrle/src/rle.c
--rw-r--r--   0 endrebak   (501) staff       (20)     8261 2018-05-25 07:27:17.000000 pyrle-0.0.8/pyrle/rledict.py
--rw-r--r--   0 endrebak   (501) staff       (20)     3619 2018-06-05 10:01:03.000000 pyrle-0.0.8/pyrle/rle.py
--rw-r--r--   0 endrebak   (501) staff       (20)      728 2018-06-05 11:06:51.000000 pyrle-0.0.8/PKG-INFO
--rw-r--r--   0 endrebak   (501) staff       (20)     3055 2018-06-05 11:06:31.000000 pyrle-0.0.8/setup.py
-drwxr-xr-x   0 endrebak   (501) staff       (20)        0 2018-06-05 11:06:44.000000 pyrle-0.0.8/pyrle.egg-info/
--rw-r--r--   0 endrebak   (501) staff       (20)       37 2018-06-05 11:06:36.000000 pyrle-0.0.8/pyrle.egg-info/requires.txt
--rw-r--r--   0 endrebak   (501) staff       (20)      518 2018-06-05 11:06:37.000000 pyrle-0.0.8/pyrle.egg-info/SOURCES.txt
--rw-r--r--   0 endrebak   (501) staff       (20)        1 2018-06-05 11:06:36.000000 pyrle-0.0.8/pyrle.egg-info/dependency_links.txt
--rw-r--r--   0 endrebak   (501) staff       (20)       12 2018-06-05 11:06:36.000000 pyrle-0.0.8/pyrle.egg-info/top_level.txt
--rw-r--r--   0 endrebak   (501) staff       (20)      728 2018-06-05 11:06:36.000000 pyrle-0.0.8/pyrle.egg-info/PKG-INFO
--rw-r--r--   0 endrebak   (501) staff       (20)       38 2018-06-05 11:06:51.000000 pyrle-0.0.8/setup.cfg
+drwxr-xr-x   0 endrebak (108065) biocore  (10000)        0 2018-06-05 13:21:41.000000 pyrle-0.0.9/
+drwxr-xr-x   0 endrebak (108065) biocore  (10000)        0 2018-06-05 13:21:41.000000 pyrle-0.0.9/tests/
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     6188 2018-05-23 12:49:27.000000 pyrle-0.0.9/tests/test_coverage.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)      819 2018-06-04 11:28:43.000000 pyrle-0.0.9/tests/test_inverse.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     1311 2018-05-23 12:49:29.000000 pyrle-0.0.9/tests/test_operations_GRles.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     5123 2018-06-04 12:54:11.000000 pyrle-0.0.9/tests/test_div.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)        0 2018-05-23 12:49:26.000000 pyrle-0.0.9/tests/__init__.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     3619 2018-05-23 12:49:29.000000 pyrle-0.0.9/tests/test_subtract.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     8765 2018-05-23 12:49:28.000000 pyrle-0.0.9/tests/test_GRles.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     2612 2018-06-04 09:58:54.000000 pyrle-0.0.9/tests/test_add.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     1025 2018-05-23 12:49:28.000000 pyrle-0.0.9/tests/test_mul.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     1087 2018-04-25 12:19:48.000000 pyrle-0.0.9/README.md
+drwxr-xr-x   0 endrebak (108065) biocore  (10000)        0 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle/
+-rw-r--r--   0 endrebak (108065) biocore  (10000)      185 2018-05-23 12:49:24.000000 pyrle-0.0.9/pyrle/__init__.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     4502 2018-05-24 10:06:01.000000 pyrle-0.0.9/pyrle/methods.py
+drwxr-xr-x   0 endrebak (108065) biocore  (10000)        0 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle/src/
+-rw-r--r--   0 endrebak (108065) biocore  (10000)   852480 2018-05-23 12:35:08.000000 pyrle-0.0.9/pyrle/src/coverage.c
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     4691 2018-05-23 12:34:51.000000 pyrle-0.0.9/pyrle/src/coverage.pyx
+-rw-r--r--   0 endrebak (108065) biocore  (10000)        0 2018-05-23 12:49:25.000000 pyrle-0.0.9/pyrle/src/__init__.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)    14540 2018-06-05 13:21:40.000000 pyrle-0.0.9/pyrle/src/rle.pyx
+-rw-r--r--   0 endrebak (108065) biocore  (10000)  1038703 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle/src/rle.c
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     8261 2018-05-25 07:27:17.000000 pyrle-0.0.9/pyrle/rledict.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     3619 2018-06-05 10:01:03.000000 pyrle-0.0.9/pyrle/rle.py
+-rw-r--r--   0 endrebak (108065) biocore  (10000)      728 2018-06-05 13:21:41.000000 pyrle-0.0.9/PKG-INFO
+-rw-r--r--   0 endrebak (108065) biocore  (10000)     3055 2018-06-05 13:20:38.000000 pyrle-0.0.9/setup.py
+drwxr-xr-x   0 endrebak (108065) biocore  (10000)        0 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle.egg-info/
+-rw-r--r--   0 endrebak (108065) biocore  (10000)       37 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle.egg-info/requires.txt
+-rw-r--r--   0 endrebak (108065) biocore  (10000)      518 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle.egg-info/SOURCES.txt
+-rw-r--r--   0 endrebak (108065) biocore  (10000)        1 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle.egg-info/dependency_links.txt
+-rw-r--r--   0 endrebak (108065) biocore  (10000)       12 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle.egg-info/top_level.txt
+-rw-r--r--   0 endrebak (108065) biocore  (10000)      728 2018-06-05 13:21:41.000000 pyrle-0.0.9/pyrle.egg-info/PKG-INFO
+-rw-r--r--   0 endrebak (108065) biocore  (10000)       38 2018-06-05 13:21:41.000000 pyrle-0.0.9/setup.cfg
```

### Comparing `pyrle-0.0.8/tests/test_coverage.py` & `pyrle-0.0.9/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/tests/test_inverse.py` & `pyrle-0.0.9/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/tests/test_operations_GRles.py` & `pyrle-0.0.9/tests/test_operations_GRles.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/tests/test_div.py` & `pyrle-0.0.9/tests/test_div.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/tests/test_subtract.py` & `pyrle-0.0.9/tests/test_subtract.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/tests/test_GRles.py` & `pyrle-0.0.9/tests/test_GRles.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/tests/test_add.py` & `pyrle-0.0.9/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/tests/test_mul.py` & `pyrle-0.0.9/tests/test_mul.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/README.md` & `pyrle-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/pyrle/methods.py` & `pyrle-0.0.9/pyrle/methods.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/pyrle/src/coverage.c` & `pyrle-0.0.9/pyrle/src/coverage.c`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/pyrle/src/coverage.pyx` & `pyrle-0.0.9/pyrle/src/coverage.pyx`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/pyrle/src/rle.pyx` & `pyrle-0.0.9/pyrle/src/rle.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,14 @@
 
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 cpdef mul_rles(long [::1] runs1, double [::1] values1, long [::1] runs2, double [::1] values2):
-
     cdef int x1 = 0
     cdef int x2 = 0
     cdef int xn = 0
     cdef int nr = 0
     cdef double nv = 0
     cdef double diff = 0
     cdef int l1 = len(runs1)
@@ -480,57 +479,56 @@
             if x2 < l2:
                 r2 = runs2[x2]
 
         # if the new value is the same as the old, merge the runs
         if xn > 0 and np.isclose(nv, nvs[xn - 1]):
             nrs[xn - 1] += nr
         else:
-                nrs[xn] = nr
-                nvs[xn] = nv
-                xn += 1
-
+            nrs[xn] = nr
+            nvs[xn] = nv
+            xn += 1
     # Here we unwind the rest of the values that were not added because one Rle was longer than the other.
     # (If other had largest sum of lengths.)
     if x1 == l1 and not x2 == l2:
-
         # Have some values left in one rl from the previous comparison
         # which must be added before we move on
+
+
         if diff < 0:
             nrs[xn] = r2
             nv = 0 if np.isfinite(values2[x2]) else np.nan
             nvs[xn] = nv
             x2 += 1
 
-
         for i in range(x2, l2):
             nv = 0 if np.isfinite(values2[i]) else values2[i]
 
             if np.isclose(nv, nvs[xn - 1]):
                 nrs[xn - 1] += runs2[i]
             else:
-                nrs[xn] = runs2[i]
+                nrs[xn] += runs2[i]
                 nvs[xn] = nv
                 xn += 1
 
     # (If self had largest sum of lengths)
     elif x2 == l2 and not x1 == l1:
+
         if diff > 0:
             nrs[xn] = r1
             nv = 0 if np.isfinite(values1[x1]) else values1[x1] * 0
             nvs[xn] = nv
             x1 += 1
 
-
         for i in range(x1, l1):
             nv = 0 if np.isfinite(values1[i]) else np.nan
 
             if np.isclose(nv, nvs[xn - 1]):
                 nrs[xn - 1] += runs1[i]
             else:
-                nrs[xn] = runs1[i]
+                nrs[xn] += runs1[i]
                 nvs[xn] = nv
                 xn += 1
 
     # Must use resize because initial guess for array was likely way too large
     nrs_arr.resize(xn, refcheck=False)
     nvs_arr.resize(xn, refcheck=False)
```

### Comparing `pyrle-0.0.8/pyrle/src/rle.c` & `pyrle-0.0.9/pyrle/src/rle.c`

 * *Files 0% similar despite different names*

```diff
@@ -7993,16 +7993,16 @@
   return __pyx_r;
 }
 
 /* "pyrle/src/rle.pyx":437
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef mul_rles(long [::1] runs1, double [::1] values1, long [::1] runs2, double [::1] values2):             # <<<<<<<<<<<<<<
- * 
  *     cdef int x1 = 0
+ *     cdef int x2 = 0
  */
 
 static PyObject *__pyx_pw_5pyrle_3src_3rle_9mul_rles(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_5pyrle_3src_3rle_mul_rles(__Pyx_memviewslice __pyx_v_runs1, __Pyx_memviewslice __pyx_v_values1, __Pyx_memviewslice __pyx_v_runs2, __Pyx_memviewslice __pyx_v_values2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_x1;
   int __pyx_v_x2;
   int __pyx_v_xn;
@@ -8070,209 +8070,209 @@
   Py_ssize_t __pyx_t_48;
   Py_ssize_t __pyx_t_49;
   Py_ssize_t __pyx_t_50;
   Py_ssize_t __pyx_t_51;
   Py_ssize_t __pyx_t_52;
   __Pyx_RefNannySetupContext("mul_rles", 0);
 
-  /* "pyrle/src/rle.pyx":439
+  /* "pyrle/src/rle.pyx":438
+ * @cython.wraparound(False)
  * cpdef mul_rles(long [::1] runs1, double [::1] values1, long [::1] runs2, double [::1] values2):
- * 
  *     cdef int x1 = 0             # <<<<<<<<<<<<<<
  *     cdef int x2 = 0
  *     cdef int xn = 0
  */
   __pyx_v_x1 = 0;
 
-  /* "pyrle/src/rle.pyx":440
- * 
+  /* "pyrle/src/rle.pyx":439
+ * cpdef mul_rles(long [::1] runs1, double [::1] values1, long [::1] runs2, double [::1] values2):
  *     cdef int x1 = 0
  *     cdef int x2 = 0             # <<<<<<<<<<<<<<
  *     cdef int xn = 0
  *     cdef int nr = 0
  */
   __pyx_v_x2 = 0;
 
-  /* "pyrle/src/rle.pyx":441
+  /* "pyrle/src/rle.pyx":440
  *     cdef int x1 = 0
  *     cdef int x2 = 0
  *     cdef int xn = 0             # <<<<<<<<<<<<<<
  *     cdef int nr = 0
  *     cdef double nv = 0
  */
   __pyx_v_xn = 0;
 
-  /* "pyrle/src/rle.pyx":442
+  /* "pyrle/src/rle.pyx":441
  *     cdef int x2 = 0
  *     cdef int xn = 0
  *     cdef int nr = 0             # <<<<<<<<<<<<<<
  *     cdef double nv = 0
  *     cdef double diff = 0
  */
   __pyx_v_nr = 0;
 
-  /* "pyrle/src/rle.pyx":443
+  /* "pyrle/src/rle.pyx":442
  *     cdef int xn = 0
  *     cdef int nr = 0
  *     cdef double nv = 0             # <<<<<<<<<<<<<<
  *     cdef double diff = 0
  *     cdef int l1 = len(runs1)
  */
   __pyx_v_nv = 0.0;
 
-  /* "pyrle/src/rle.pyx":444
+  /* "pyrle/src/rle.pyx":443
  *     cdef int nr = 0
  *     cdef double nv = 0
  *     cdef double diff = 0             # <<<<<<<<<<<<<<
  *     cdef int l1 = len(runs1)
  *     cdef int l2 = len(runs2)
  */
   __pyx_v_diff = 0.0;
 
-  /* "pyrle/src/rle.pyx":445
+  /* "pyrle/src/rle.pyx":444
  *     cdef double nv = 0
  *     cdef double diff = 0
  *     cdef int l1 = len(runs1)             # <<<<<<<<<<<<<<
  *     cdef int l2 = len(runs2)
  *     cdef long r1 = runs1[x1]
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_runs1); 
   __pyx_v_l1 = __pyx_t_1;
 
-  /* "pyrle/src/rle.pyx":446
+  /* "pyrle/src/rle.pyx":445
  *     cdef double diff = 0
  *     cdef int l1 = len(runs1)
  *     cdef int l2 = len(runs2)             # <<<<<<<<<<<<<<
  *     cdef long r1 = runs1[x1]
  *     cdef long r2 = runs2[x2]
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_runs2); 
   __pyx_v_l2 = __pyx_t_1;
 
-  /* "pyrle/src/rle.pyx":447
+  /* "pyrle/src/rle.pyx":446
  *     cdef int l1 = len(runs1)
  *     cdef int l2 = len(runs2)
  *     cdef long r1 = runs1[x1]             # <<<<<<<<<<<<<<
  *     cdef long r2 = runs2[x2]
  *     nrs_arr = np.zeros(len(runs1) + len(runs2), dtype=np.long)
  */
   __pyx_t_2 = __pyx_v_x1;
   __pyx_v_r1 = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs1.data) + __pyx_t_2)) )));
 
-  /* "pyrle/src/rle.pyx":448
+  /* "pyrle/src/rle.pyx":447
  *     cdef int l2 = len(runs2)
  *     cdef long r1 = runs1[x1]
  *     cdef long r2 = runs2[x2]             # <<<<<<<<<<<<<<
  *     nrs_arr = np.zeros(len(runs1) + len(runs2), dtype=np.long)
  *     nvs_arr = np.zeros(len(runs1) + len(runs2), dtype=np.double)
  */
   __pyx_t_3 = __pyx_v_x2;
   __pyx_v_r2 = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs2.data) + __pyx_t_3)) )));
 
-  /* "pyrle/src/rle.pyx":449
+  /* "pyrle/src/rle.pyx":448
  *     cdef long r1 = runs1[x1]
  *     cdef long r2 = runs2[x2]
  *     nrs_arr = np.zeros(len(runs1) + len(runs2), dtype=np.long)             # <<<<<<<<<<<<<<
  *     nvs_arr = np.zeros(len(runs1) + len(runs2), dtype=np.double)
  * 
  */
-  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_runs1); 
   __pyx_t_6 = __Pyx_MemoryView_Len(__pyx_v_runs2); 
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_1 + __pyx_t_6)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_1 + __pyx_t_6)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_long); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_long); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_nrs_arr = __pyx_t_9;
   __pyx_t_9 = 0;
 
-  /* "pyrle/src/rle.pyx":450
+  /* "pyrle/src/rle.pyx":449
  *     cdef long r2 = runs2[x2]
  *     nrs_arr = np.zeros(len(runs1) + len(runs2), dtype=np.long)
  *     nvs_arr = np.zeros(len(runs1) + len(runs2), dtype=np.double)             # <<<<<<<<<<<<<<
  * 
  *     cdef long[::1] nrs
  */
-  __pyx_t_9 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_6 = __Pyx_MemoryView_Len(__pyx_v_runs1); 
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_runs2); 
-  __pyx_t_9 = PyInt_FromSsize_t((__pyx_t_6 + __pyx_t_1)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_9 = PyInt_FromSsize_t((__pyx_t_6 + __pyx_t_1)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_9);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_9);
   __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 450, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_v_nvs_arr = __pyx_t_8;
   __pyx_t_8 = 0;
 
-  /* "pyrle/src/rle.pyx":455
+  /* "pyrle/src/rle.pyx":454
  *     cdef double[::1] nvs
  * 
  *     nrs = nrs_arr             # <<<<<<<<<<<<<<
  *     nvs = nvs_arr
  * 
  */
-  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_nrs_arr, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_long(__pyx_v_nrs_arr, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 454, __pyx_L1_error)
   __pyx_v_nrs = __pyx_t_10;
   __pyx_t_10.memview = NULL;
   __pyx_t_10.data = NULL;
 
-  /* "pyrle/src/rle.pyx":456
+  /* "pyrle/src/rle.pyx":455
  * 
  *     nrs = nrs_arr
  *     nvs = nvs_arr             # <<<<<<<<<<<<<<
  * 
  *     while(x1 < l1 and x2 < l2):
  */
-  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_v_nvs_arr, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 456, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_v_nvs_arr, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 455, __pyx_L1_error)
   __pyx_v_nvs = __pyx_t_11;
   __pyx_t_11.memview = NULL;
   __pyx_t_11.data = NULL;
 
-  /* "pyrle/src/rle.pyx":458
+  /* "pyrle/src/rle.pyx":457
  *     nvs = nvs_arr
  * 
  *     while(x1 < l1 and x2 < l2):             # <<<<<<<<<<<<<<
  * 
  *         diff = r1 - r2
  */
   while (1) {
@@ -8283,296 +8283,296 @@
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_13 = ((__pyx_v_x2 < __pyx_v_l2) != 0);
     __pyx_t_12 = __pyx_t_13;
     __pyx_L5_bool_binop_done:;
     if (!__pyx_t_12) break;
 
-    /* "pyrle/src/rle.pyx":460
+    /* "pyrle/src/rle.pyx":459
  *     while(x1 < l1 and x2 < l2):
  * 
  *         diff = r1 - r2             # <<<<<<<<<<<<<<
  *         nv = values1[x1] * values2[x2]
  *         if diff < 0:
  */
     __pyx_v_diff = (__pyx_v_r1 - __pyx_v_r2);
 
-    /* "pyrle/src/rle.pyx":461
+    /* "pyrle/src/rle.pyx":460
  * 
  *         diff = r1 - r2
  *         nv = values1[x1] * values2[x2]             # <<<<<<<<<<<<<<
  *         if diff < 0:
  *             nr = r1
  */
     __pyx_t_14 = __pyx_v_x1;
     __pyx_t_15 = __pyx_v_x2;
     __pyx_v_nv = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values1.data) + __pyx_t_14)) ))) * (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values2.data) + __pyx_t_15)) ))));
 
-    /* "pyrle/src/rle.pyx":462
+    /* "pyrle/src/rle.pyx":461
  *         diff = r1 - r2
  *         nv = values1[x1] * values2[x2]
  *         if diff < 0:             # <<<<<<<<<<<<<<
  *             nr = r1
  *             r2 = r2 - r1
  */
     __pyx_t_12 = ((__pyx_v_diff < 0.0) != 0);
     if (__pyx_t_12) {
 
-      /* "pyrle/src/rle.pyx":463
+      /* "pyrle/src/rle.pyx":462
  *         nv = values1[x1] * values2[x2]
  *         if diff < 0:
  *             nr = r1             # <<<<<<<<<<<<<<
  *             r2 = r2 - r1
  *             x1 += 1
  */
       __pyx_v_nr = __pyx_v_r1;
 
-      /* "pyrle/src/rle.pyx":464
+      /* "pyrle/src/rle.pyx":463
  *         if diff < 0:
  *             nr = r1
  *             r2 = r2 - r1             # <<<<<<<<<<<<<<
  *             x1 += 1
  *             if x1 < l1:
  */
       __pyx_v_r2 = (__pyx_v_r2 - __pyx_v_r1);
 
-      /* "pyrle/src/rle.pyx":465
+      /* "pyrle/src/rle.pyx":464
  *             nr = r1
  *             r2 = r2 - r1
  *             x1 += 1             # <<<<<<<<<<<<<<
  *             if x1 < l1:
  *                 r1 = runs1[x1]
  */
       __pyx_v_x1 = (__pyx_v_x1 + 1);
 
-      /* "pyrle/src/rle.pyx":466
+      /* "pyrle/src/rle.pyx":465
  *             r2 = r2 - r1
  *             x1 += 1
  *             if x1 < l1:             # <<<<<<<<<<<<<<
  *                 r1 = runs1[x1]
  *         elif diff > 0:
  */
       __pyx_t_12 = ((__pyx_v_x1 < __pyx_v_l1) != 0);
       if (__pyx_t_12) {
 
-        /* "pyrle/src/rle.pyx":467
+        /* "pyrle/src/rle.pyx":466
  *             x1 += 1
  *             if x1 < l1:
  *                 r1 = runs1[x1]             # <<<<<<<<<<<<<<
  *         elif diff > 0:
  *             nr = r2
  */
         __pyx_t_16 = __pyx_v_x1;
         __pyx_v_r1 = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs1.data) + __pyx_t_16)) )));
 
-        /* "pyrle/src/rle.pyx":466
+        /* "pyrle/src/rle.pyx":465
  *             r2 = r2 - r1
  *             x1 += 1
  *             if x1 < l1:             # <<<<<<<<<<<<<<
  *                 r1 = runs1[x1]
  *         elif diff > 0:
  */
       }
 
-      /* "pyrle/src/rle.pyx":462
+      /* "pyrle/src/rle.pyx":461
  *         diff = r1 - r2
  *         nv = values1[x1] * values2[x2]
  *         if diff < 0:             # <<<<<<<<<<<<<<
  *             nr = r1
  *             r2 = r2 - r1
  */
       goto __pyx_L7;
     }
 
-    /* "pyrle/src/rle.pyx":468
+    /* "pyrle/src/rle.pyx":467
  *             if x1 < l1:
  *                 r1 = runs1[x1]
  *         elif diff > 0:             # <<<<<<<<<<<<<<
  *             nr = r2
  *             r1 = r1 - r2
  */
     __pyx_t_12 = ((__pyx_v_diff > 0.0) != 0);
     if (__pyx_t_12) {
 
-      /* "pyrle/src/rle.pyx":469
+      /* "pyrle/src/rle.pyx":468
  *                 r1 = runs1[x1]
  *         elif diff > 0:
  *             nr = r2             # <<<<<<<<<<<<<<
  *             r1 = r1 - r2
  *             x2 += 1
  */
       __pyx_v_nr = __pyx_v_r2;
 
-      /* "pyrle/src/rle.pyx":470
+      /* "pyrle/src/rle.pyx":469
  *         elif diff > 0:
  *             nr = r2
  *             r1 = r1 - r2             # <<<<<<<<<<<<<<
  *             x2 += 1
  *             if x2 < l2:
  */
       __pyx_v_r1 = (__pyx_v_r1 - __pyx_v_r2);
 
-      /* "pyrle/src/rle.pyx":471
+      /* "pyrle/src/rle.pyx":470
  *             nr = r2
  *             r1 = r1 - r2
  *             x2 += 1             # <<<<<<<<<<<<<<
  *             if x2 < l2:
  *                 r2 = runs2[x2]
  */
       __pyx_v_x2 = (__pyx_v_x2 + 1);
 
-      /* "pyrle/src/rle.pyx":472
+      /* "pyrle/src/rle.pyx":471
  *             r1 = r1 - r2
  *             x2 += 1
  *             if x2 < l2:             # <<<<<<<<<<<<<<
  *                 r2 = runs2[x2]
  *         else:
  */
       __pyx_t_12 = ((__pyx_v_x2 < __pyx_v_l2) != 0);
       if (__pyx_t_12) {
 
-        /* "pyrle/src/rle.pyx":473
+        /* "pyrle/src/rle.pyx":472
  *             x2 += 1
  *             if x2 < l2:
  *                 r2 = runs2[x2]             # <<<<<<<<<<<<<<
  *         else:
  *             nr = r2
  */
         __pyx_t_17 = __pyx_v_x2;
         __pyx_v_r2 = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs2.data) + __pyx_t_17)) )));
 
-        /* "pyrle/src/rle.pyx":472
+        /* "pyrle/src/rle.pyx":471
  *             r1 = r1 - r2
  *             x2 += 1
  *             if x2 < l2:             # <<<<<<<<<<<<<<
  *                 r2 = runs2[x2]
  *         else:
  */
       }
 
-      /* "pyrle/src/rle.pyx":468
+      /* "pyrle/src/rle.pyx":467
  *             if x1 < l1:
  *                 r1 = runs1[x1]
  *         elif diff > 0:             # <<<<<<<<<<<<<<
  *             nr = r2
  *             r1 = r1 - r2
  */
       goto __pyx_L7;
     }
 
-    /* "pyrle/src/rle.pyx":475
+    /* "pyrle/src/rle.pyx":474
  *                 r2 = runs2[x2]
  *         else:
  *             nr = r2             # <<<<<<<<<<<<<<
  *             x1 += 1
  *             x2 += 1
  */
     /*else*/ {
       __pyx_v_nr = __pyx_v_r2;
 
-      /* "pyrle/src/rle.pyx":476
+      /* "pyrle/src/rle.pyx":475
  *         else:
  *             nr = r2
  *             x1 += 1             # <<<<<<<<<<<<<<
  *             x2 += 1
  *             if x1 < l1:
  */
       __pyx_v_x1 = (__pyx_v_x1 + 1);
 
-      /* "pyrle/src/rle.pyx":477
+      /* "pyrle/src/rle.pyx":476
  *             nr = r2
  *             x1 += 1
  *             x2 += 1             # <<<<<<<<<<<<<<
  *             if x1 < l1:
  *                 r1 = runs1[x1]
  */
       __pyx_v_x2 = (__pyx_v_x2 + 1);
 
-      /* "pyrle/src/rle.pyx":478
+      /* "pyrle/src/rle.pyx":477
  *             x1 += 1
  *             x2 += 1
  *             if x1 < l1:             # <<<<<<<<<<<<<<
  *                 r1 = runs1[x1]
  *             if x2 < l2:
  */
       __pyx_t_12 = ((__pyx_v_x1 < __pyx_v_l1) != 0);
       if (__pyx_t_12) {
 
-        /* "pyrle/src/rle.pyx":479
+        /* "pyrle/src/rle.pyx":478
  *             x2 += 1
  *             if x1 < l1:
  *                 r1 = runs1[x1]             # <<<<<<<<<<<<<<
  *             if x2 < l2:
  *                 r2 = runs2[x2]
  */
         __pyx_t_18 = __pyx_v_x1;
         __pyx_v_r1 = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs1.data) + __pyx_t_18)) )));
 
-        /* "pyrle/src/rle.pyx":478
+        /* "pyrle/src/rle.pyx":477
  *             x1 += 1
  *             x2 += 1
  *             if x1 < l1:             # <<<<<<<<<<<<<<
  *                 r1 = runs1[x1]
  *             if x2 < l2:
  */
       }
 
-      /* "pyrle/src/rle.pyx":480
+      /* "pyrle/src/rle.pyx":479
  *             if x1 < l1:
  *                 r1 = runs1[x1]
  *             if x2 < l2:             # <<<<<<<<<<<<<<
  *                 r2 = runs2[x2]
  * 
  */
       __pyx_t_12 = ((__pyx_v_x2 < __pyx_v_l2) != 0);
       if (__pyx_t_12) {
 
-        /* "pyrle/src/rle.pyx":481
+        /* "pyrle/src/rle.pyx":480
  *                 r1 = runs1[x1]
  *             if x2 < l2:
  *                 r2 = runs2[x2]             # <<<<<<<<<<<<<<
  * 
  *         # if the new value is the same as the old, merge the runs
  */
         __pyx_t_19 = __pyx_v_x2;
         __pyx_v_r2 = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs2.data) + __pyx_t_19)) )));
 
-        /* "pyrle/src/rle.pyx":480
+        /* "pyrle/src/rle.pyx":479
  *             if x1 < l1:
  *                 r1 = runs1[x1]
  *             if x2 < l2:             # <<<<<<<<<<<<<<
  *                 r2 = runs2[x2]
  * 
  */
       }
     }
     __pyx_L7:;
 
-    /* "pyrle/src/rle.pyx":484
+    /* "pyrle/src/rle.pyx":483
  * 
  *         # if the new value is the same as the old, merge the runs
  *         if xn > 0 and np.isclose(nv, nvs[xn - 1]):             # <<<<<<<<<<<<<<
  *             nrs[xn - 1] += nr
  *         else:
  */
     __pyx_t_13 = ((__pyx_v_xn > 0) != 0);
     if (__pyx_t_13) {
     } else {
       __pyx_t_12 = __pyx_t_13;
       goto __pyx_L13_bool_binop_done;
     }
-    __pyx_t_9 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 483, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_isclose); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_isclose); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 483, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = PyFloat_FromDouble(__pyx_v_nv); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_9 = PyFloat_FromDouble(__pyx_v_nv); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 483, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_20 = (__pyx_v_xn - 1);
-    __pyx_t_4 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_20)) )))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_4 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_20)) )))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 483, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_21 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -8581,349 +8581,349 @@
         __Pyx_DECREF_SET(__pyx_t_7, function);
         __pyx_t_21 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_7)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_9, __pyx_t_4};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_21, 2+__pyx_t_21); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 484, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_21, 2+__pyx_t_21); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 483, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_9, __pyx_t_4};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_21, 2+__pyx_t_21); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 484, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_21, 2+__pyx_t_21); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 483, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_22 = PyTuple_New(2+__pyx_t_21); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 484, __pyx_L1_error)
+      __pyx_t_22 = PyTuple_New(2+__pyx_t_21); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 483, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_22, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_9);
       PyTuple_SET_ITEM(__pyx_t_22, 0+__pyx_t_21, __pyx_t_9);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_22, 1+__pyx_t_21, __pyx_t_4);
       __pyx_t_9 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_22, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 484, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_22, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 483, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
     }
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(0, 483, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_12 = __pyx_t_13;
     __pyx_L13_bool_binop_done:;
     if (__pyx_t_12) {
 
-      /* "pyrle/src/rle.pyx":485
+      /* "pyrle/src/rle.pyx":484
  *         # if the new value is the same as the old, merge the runs
  *         if xn > 0 and np.isclose(nv, nvs[xn - 1]):
  *             nrs[xn - 1] += nr             # <<<<<<<<<<<<<<
  *         else:
- *                 nrs[xn] = nr
+ *             nrs[xn] = nr
  */
       __pyx_t_23 = (__pyx_v_xn - 1);
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_23)) )) += __pyx_v_nr;
 
-      /* "pyrle/src/rle.pyx":484
+      /* "pyrle/src/rle.pyx":483
  * 
  *         # if the new value is the same as the old, merge the runs
  *         if xn > 0 and np.isclose(nv, nvs[xn - 1]):             # <<<<<<<<<<<<<<
  *             nrs[xn - 1] += nr
  *         else:
  */
       goto __pyx_L12;
     }
 
-    /* "pyrle/src/rle.pyx":487
+    /* "pyrle/src/rle.pyx":486
  *             nrs[xn - 1] += nr
  *         else:
- *                 nrs[xn] = nr             # <<<<<<<<<<<<<<
- *                 nvs[xn] = nv
- *                 xn += 1
+ *             nrs[xn] = nr             # <<<<<<<<<<<<<<
+ *             nvs[xn] = nv
+ *             xn += 1
  */
     /*else*/ {
       __pyx_t_24 = __pyx_v_xn;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_24)) )) = __pyx_v_nr;
 
-      /* "pyrle/src/rle.pyx":488
+      /* "pyrle/src/rle.pyx":487
  *         else:
- *                 nrs[xn] = nr
- *                 nvs[xn] = nv             # <<<<<<<<<<<<<<
- *                 xn += 1
- * 
+ *             nrs[xn] = nr
+ *             nvs[xn] = nv             # <<<<<<<<<<<<<<
+ *             xn += 1
+ *     # Here we unwind the rest of the values that were not added because one Rle was longer than the other.
  */
       __pyx_t_25 = __pyx_v_xn;
       *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_25)) )) = __pyx_v_nv;
 
-      /* "pyrle/src/rle.pyx":489
- *                 nrs[xn] = nr
- *                 nvs[xn] = nv
- *                 xn += 1             # <<<<<<<<<<<<<<
- * 
+      /* "pyrle/src/rle.pyx":488
+ *             nrs[xn] = nr
+ *             nvs[xn] = nv
+ *             xn += 1             # <<<<<<<<<<<<<<
  *     # Here we unwind the rest of the values that were not added because one Rle was longer than the other.
+ *     # (If other had largest sum of lengths.)
  */
       __pyx_v_xn = (__pyx_v_xn + 1);
     }
     __pyx_L12:;
   }
 
-  /* "pyrle/src/rle.pyx":493
+  /* "pyrle/src/rle.pyx":491
  *     # Here we unwind the rest of the values that were not added because one Rle was longer than the other.
  *     # (If other had largest sum of lengths.)
  *     if x1 == l1 and not x2 == l2:             # <<<<<<<<<<<<<<
- * 
  *         # Have some values left in one rl from the previous comparison
+ *         # which must be added before we move on
  */
   __pyx_t_13 = ((__pyx_v_x1 == __pyx_v_l1) != 0);
   if (__pyx_t_13) {
   } else {
     __pyx_t_12 = __pyx_t_13;
     goto __pyx_L16_bool_binop_done;
   }
   __pyx_t_13 = ((!((__pyx_v_x2 == __pyx_v_l2) != 0)) != 0);
   __pyx_t_12 = __pyx_t_13;
   __pyx_L16_bool_binop_done:;
   if (__pyx_t_12) {
 
-    /* "pyrle/src/rle.pyx":497
- *         # Have some values left in one rl from the previous comparison
- *         # which must be added before we move on
+    /* "pyrle/src/rle.pyx":496
+ * 
+ * 
  *         if diff < 0:             # <<<<<<<<<<<<<<
  *             nrs[xn] = r2
  *             nv = 0 if np.isfinite(values2[x2]) else np.nan
  */
     __pyx_t_12 = ((__pyx_v_diff < 0.0) != 0);
     if (__pyx_t_12) {
 
-      /* "pyrle/src/rle.pyx":498
- *         # which must be added before we move on
+      /* "pyrle/src/rle.pyx":497
+ * 
  *         if diff < 0:
  *             nrs[xn] = r2             # <<<<<<<<<<<<<<
  *             nv = 0 if np.isfinite(values2[x2]) else np.nan
  *             nvs[xn] = nv
  */
       __pyx_t_26 = __pyx_v_xn;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_26)) )) = __pyx_v_r2;
 
-      /* "pyrle/src/rle.pyx":499
+      /* "pyrle/src/rle.pyx":498
  *         if diff < 0:
  *             nrs[xn] = r2
  *             nv = 0 if np.isfinite(values2[x2]) else np.nan             # <<<<<<<<<<<<<<
  *             nvs[xn] = nv
  *             x2 += 1
  */
-      __pyx_t_7 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 499, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 498, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 499, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 498, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_28 = __pyx_v_x2;
-      __pyx_t_7 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values2.data) + __pyx_t_28)) )))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 499, __pyx_L1_error)
+      __pyx_t_7 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values2.data) + __pyx_t_28)) )))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 498, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_22))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_22);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_22);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_22, function);
         }
       }
       if (!__pyx_t_4) {
-        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_t_22, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 499, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_t_22, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_8);
       } else {
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_22)) {
           PyObject *__pyx_temp[2] = {__pyx_t_4, __pyx_t_7};
-          __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_22, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 499, __pyx_L1_error)
+          __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_22, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 498, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_22)) {
           PyObject *__pyx_temp[2] = {__pyx_t_4, __pyx_t_7};
-          __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_22, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 499, __pyx_L1_error)
+          __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_22, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 498, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         } else
         #endif
         {
-          __pyx_t_9 = PyTuple_New(1+1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 499, __pyx_L1_error)
+          __pyx_t_9 = PyTuple_New(1+1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 498, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_4); __pyx_t_4 = NULL;
           __Pyx_GIVEREF(__pyx_t_7);
           PyTuple_SET_ITEM(__pyx_t_9, 0+1, __pyx_t_7);
           __pyx_t_7 = 0;
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_22, __pyx_t_9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 499, __pyx_L1_error)
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_22, __pyx_t_9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 498, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
       }
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 499, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 498, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       if (__pyx_t_12) {
         __pyx_t_27 = 0.0;
       } else {
-        __pyx_t_8 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 499, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_nan); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 499, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_nan); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_29 = __pyx_PyFloat_AsDouble(__pyx_t_22); if (unlikely((__pyx_t_29 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 499, __pyx_L1_error)
+        __pyx_t_29 = __pyx_PyFloat_AsDouble(__pyx_t_22); if (unlikely((__pyx_t_29 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         __pyx_t_27 = __pyx_t_29;
       }
       __pyx_v_nv = __pyx_t_27;
 
-      /* "pyrle/src/rle.pyx":500
+      /* "pyrle/src/rle.pyx":499
  *             nrs[xn] = r2
  *             nv = 0 if np.isfinite(values2[x2]) else np.nan
  *             nvs[xn] = nv             # <<<<<<<<<<<<<<
  *             x2 += 1
  * 
  */
       __pyx_t_30 = __pyx_v_xn;
       *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_30)) )) = __pyx_v_nv;
 
-      /* "pyrle/src/rle.pyx":501
+      /* "pyrle/src/rle.pyx":500
  *             nv = 0 if np.isfinite(values2[x2]) else np.nan
  *             nvs[xn] = nv
  *             x2 += 1             # <<<<<<<<<<<<<<
  * 
- * 
+ *         for i in range(x2, l2):
  */
       __pyx_v_x2 = (__pyx_v_x2 + 1);
 
-      /* "pyrle/src/rle.pyx":497
- *         # Have some values left in one rl from the previous comparison
- *         # which must be added before we move on
+      /* "pyrle/src/rle.pyx":496
+ * 
+ * 
  *         if diff < 0:             # <<<<<<<<<<<<<<
  *             nrs[xn] = r2
  *             nv = 0 if np.isfinite(values2[x2]) else np.nan
  */
     }
 
-    /* "pyrle/src/rle.pyx":504
- * 
+    /* "pyrle/src/rle.pyx":502
+ *             x2 += 1
  * 
  *         for i in range(x2, l2):             # <<<<<<<<<<<<<<
  *             nv = 0 if np.isfinite(values2[i]) else values2[i]
  * 
  */
     __pyx_t_21 = __pyx_v_l2;
     __pyx_t_31 = __pyx_t_21;
     for (__pyx_t_32 = __pyx_v_x2; __pyx_t_32 < __pyx_t_31; __pyx_t_32+=1) {
       __pyx_v_i = __pyx_t_32;
 
-      /* "pyrle/src/rle.pyx":505
+      /* "pyrle/src/rle.pyx":503
  * 
  *         for i in range(x2, l2):
  *             nv = 0 if np.isfinite(values2[i]) else values2[i]             # <<<<<<<<<<<<<<
  * 
  *             if np.isclose(nv, nvs[xn - 1]):
  */
-      __pyx_t_8 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 503, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 505, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 503, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_33 = __pyx_v_i;
-      __pyx_t_8 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values2.data) + __pyx_t_33)) )))); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
+      __pyx_t_8 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values2.data) + __pyx_t_33)) )))); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 503, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       if (!__pyx_t_7) {
-        __pyx_t_22 = __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_8); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 505, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_8); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 503, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_22);
       } else {
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_9)) {
           PyObject *__pyx_temp[2] = {__pyx_t_7, __pyx_t_8};
-          __pyx_t_22 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 505, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 503, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
           PyObject *__pyx_temp[2] = {__pyx_t_7, __pyx_t_8};
-          __pyx_t_22 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 505, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 503, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_4 = PyTuple_New(1+1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 505, __pyx_L1_error)
+          __pyx_t_4 = PyTuple_New(1+1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 503, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
           __Pyx_GIVEREF(__pyx_t_8);
           PyTuple_SET_ITEM(__pyx_t_4, 0+1, __pyx_t_8);
           __pyx_t_8 = 0;
-          __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_4, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 505, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_4, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 503, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         }
       }
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 505, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 503, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       if (__pyx_t_12) {
         __pyx_t_27 = 0.0;
       } else {
         __pyx_t_34 = __pyx_v_i;
         __pyx_t_27 = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values2.data) + __pyx_t_34)) )));
       }
       __pyx_v_nv = __pyx_t_27;
 
-      /* "pyrle/src/rle.pyx":507
+      /* "pyrle/src/rle.pyx":505
  *             nv = 0 if np.isfinite(values2[i]) else values2[i]
  * 
  *             if np.isclose(nv, nvs[xn - 1]):             # <<<<<<<<<<<<<<
  *                 nrs[xn - 1] += runs2[i]
  *             else:
  */
-      __pyx_t_9 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 507, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 505, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_isclose); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_isclose); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 505, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_9 = PyFloat_FromDouble(__pyx_v_nv); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 507, __pyx_L1_error)
+      __pyx_t_9 = PyFloat_FromDouble(__pyx_v_nv); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 505, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_35 = (__pyx_v_xn - 1);
-      __pyx_t_8 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_35)) )))); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 507, __pyx_L1_error)
+      __pyx_t_8 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_35)) )))); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_7 = NULL;
       __pyx_t_36 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -8932,359 +8932,359 @@
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_36 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_9, __pyx_t_8};
-        __pyx_t_22 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_36, 2+__pyx_t_36); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 507, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_36, 2+__pyx_t_36); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 505, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_9, __pyx_t_8};
-        __pyx_t_22 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_36, 2+__pyx_t_36); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 507, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_36, 2+__pyx_t_36); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 505, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       } else
       #endif
       {
-        __pyx_t_5 = PyTuple_New(2+__pyx_t_36); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 507, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_New(2+__pyx_t_36); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 505, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         if (__pyx_t_7) {
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7); __pyx_t_7 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_9);
         PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_36, __pyx_t_9);
         __Pyx_GIVEREF(__pyx_t_8);
         PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_36, __pyx_t_8);
         __pyx_t_9 = 0;
         __pyx_t_8 = 0;
-        __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 507, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 505, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 507, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 505, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       if (__pyx_t_12) {
 
-        /* "pyrle/src/rle.pyx":508
+        /* "pyrle/src/rle.pyx":506
  * 
  *             if np.isclose(nv, nvs[xn - 1]):
  *                 nrs[xn - 1] += runs2[i]             # <<<<<<<<<<<<<<
  *             else:
- *                 nrs[xn] = runs2[i]
+ *                 nrs[xn] += runs2[i]
  */
         __pyx_t_37 = __pyx_v_i;
         __pyx_t_38 = (__pyx_v_xn - 1);
         *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_38)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs2.data) + __pyx_t_37)) )));
 
-        /* "pyrle/src/rle.pyx":507
+        /* "pyrle/src/rle.pyx":505
  *             nv = 0 if np.isfinite(values2[i]) else values2[i]
  * 
  *             if np.isclose(nv, nvs[xn - 1]):             # <<<<<<<<<<<<<<
  *                 nrs[xn - 1] += runs2[i]
  *             else:
  */
         goto __pyx_L21;
       }
 
-      /* "pyrle/src/rle.pyx":510
+      /* "pyrle/src/rle.pyx":508
  *                 nrs[xn - 1] += runs2[i]
  *             else:
- *                 nrs[xn] = runs2[i]             # <<<<<<<<<<<<<<
+ *                 nrs[xn] += runs2[i]             # <<<<<<<<<<<<<<
  *                 nvs[xn] = nv
  *                 xn += 1
  */
       /*else*/ {
         __pyx_t_39 = __pyx_v_i;
         __pyx_t_40 = __pyx_v_xn;
-        *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_40)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs2.data) + __pyx_t_39)) )));
+        *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_40)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs2.data) + __pyx_t_39)) )));
 
-        /* "pyrle/src/rle.pyx":511
+        /* "pyrle/src/rle.pyx":509
  *             else:
- *                 nrs[xn] = runs2[i]
+ *                 nrs[xn] += runs2[i]
  *                 nvs[xn] = nv             # <<<<<<<<<<<<<<
  *                 xn += 1
  * 
  */
         __pyx_t_41 = __pyx_v_xn;
         *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_41)) )) = __pyx_v_nv;
 
-        /* "pyrle/src/rle.pyx":512
- *                 nrs[xn] = runs2[i]
+        /* "pyrle/src/rle.pyx":510
+ *                 nrs[xn] += runs2[i]
  *                 nvs[xn] = nv
  *                 xn += 1             # <<<<<<<<<<<<<<
  * 
  *     # (If self had largest sum of lengths)
  */
         __pyx_v_xn = (__pyx_v_xn + 1);
       }
       __pyx_L21:;
     }
 
-    /* "pyrle/src/rle.pyx":493
+    /* "pyrle/src/rle.pyx":491
  *     # Here we unwind the rest of the values that were not added because one Rle was longer than the other.
  *     # (If other had largest sum of lengths.)
  *     if x1 == l1 and not x2 == l2:             # <<<<<<<<<<<<<<
- * 
  *         # Have some values left in one rl from the previous comparison
+ *         # which must be added before we move on
  */
     goto __pyx_L15;
   }
 
-  /* "pyrle/src/rle.pyx":515
+  /* "pyrle/src/rle.pyx":513
  * 
  *     # (If self had largest sum of lengths)
  *     elif x2 == l2 and not x1 == l1:             # <<<<<<<<<<<<<<
+ * 
  *         if diff > 0:
- *             nrs[xn] = r1
  */
   __pyx_t_13 = ((__pyx_v_x2 == __pyx_v_l2) != 0);
   if (__pyx_t_13) {
   } else {
     __pyx_t_12 = __pyx_t_13;
     goto __pyx_L22_bool_binop_done;
   }
   __pyx_t_13 = ((!((__pyx_v_x1 == __pyx_v_l1) != 0)) != 0);
   __pyx_t_12 = __pyx_t_13;
   __pyx_L22_bool_binop_done:;
   if (__pyx_t_12) {
 
-    /* "pyrle/src/rle.pyx":516
- *     # (If self had largest sum of lengths)
+    /* "pyrle/src/rle.pyx":515
  *     elif x2 == l2 and not x1 == l1:
+ * 
  *         if diff > 0:             # <<<<<<<<<<<<<<
  *             nrs[xn] = r1
  *             nv = 0 if np.isfinite(values1[x1]) else values1[x1] * 0
  */
     __pyx_t_12 = ((__pyx_v_diff > 0.0) != 0);
     if (__pyx_t_12) {
 
-      /* "pyrle/src/rle.pyx":517
- *     elif x2 == l2 and not x1 == l1:
+      /* "pyrle/src/rle.pyx":516
+ * 
  *         if diff > 0:
  *             nrs[xn] = r1             # <<<<<<<<<<<<<<
  *             nv = 0 if np.isfinite(values1[x1]) else values1[x1] * 0
  *             nvs[xn] = nv
  */
       __pyx_t_42 = __pyx_v_xn;
       *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_42)) )) = __pyx_v_r1;
 
-      /* "pyrle/src/rle.pyx":518
+      /* "pyrle/src/rle.pyx":517
  *         if diff > 0:
  *             nrs[xn] = r1
  *             nv = 0 if np.isfinite(values1[x1]) else values1[x1] * 0             # <<<<<<<<<<<<<<
  *             nvs[xn] = nv
  *             x1 += 1
  */
-      __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 517, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 518, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 517, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_43 = __pyx_v_x1;
-      __pyx_t_4 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values1.data) + __pyx_t_43)) )))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
+      __pyx_t_4 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values1.data) + __pyx_t_43)) )))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 517, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       if (!__pyx_t_8) {
-        __pyx_t_22 = __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 518, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 517, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_GOTREF(__pyx_t_22);
       } else {
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[2] = {__pyx_t_8, __pyx_t_4};
-          __pyx_t_22 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 518, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 517, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[2] = {__pyx_t_8, __pyx_t_4};
-          __pyx_t_22 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 518, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 517, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_9 = PyTuple_New(1+1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 518, __pyx_L1_error)
+          __pyx_t_9 = PyTuple_New(1+1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 517, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_8); __pyx_t_8 = NULL;
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_9, 0+1, __pyx_t_4);
           __pyx_t_4 = 0;
-          __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 518, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 517, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 518, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 517, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       if (__pyx_t_12) {
         __pyx_t_27 = 0.0;
       } else {
         __pyx_t_44 = __pyx_v_x1;
         __pyx_t_27 = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values1.data) + __pyx_t_44)) ))) * 0.0);
       }
       __pyx_v_nv = __pyx_t_27;
 
-      /* "pyrle/src/rle.pyx":519
+      /* "pyrle/src/rle.pyx":518
  *             nrs[xn] = r1
  *             nv = 0 if np.isfinite(values1[x1]) else values1[x1] * 0
  *             nvs[xn] = nv             # <<<<<<<<<<<<<<
  *             x1 += 1
  * 
  */
       __pyx_t_45 = __pyx_v_xn;
       *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_45)) )) = __pyx_v_nv;
 
-      /* "pyrle/src/rle.pyx":520
+      /* "pyrle/src/rle.pyx":519
  *             nv = 0 if np.isfinite(values1[x1]) else values1[x1] * 0
  *             nvs[xn] = nv
  *             x1 += 1             # <<<<<<<<<<<<<<
  * 
- * 
+ *         for i in range(x1, l1):
  */
       __pyx_v_x1 = (__pyx_v_x1 + 1);
 
-      /* "pyrle/src/rle.pyx":516
- *     # (If self had largest sum of lengths)
+      /* "pyrle/src/rle.pyx":515
  *     elif x2 == l2 and not x1 == l1:
+ * 
  *         if diff > 0:             # <<<<<<<<<<<<<<
  *             nrs[xn] = r1
  *             nv = 0 if np.isfinite(values1[x1]) else values1[x1] * 0
  */
     }
 
-    /* "pyrle/src/rle.pyx":523
- * 
+    /* "pyrle/src/rle.pyx":521
+ *             x1 += 1
  * 
  *         for i in range(x1, l1):             # <<<<<<<<<<<<<<
  *             nv = 0 if np.isfinite(values1[i]) else np.nan
  * 
  */
     __pyx_t_21 = __pyx_v_l1;
     __pyx_t_31 = __pyx_t_21;
     for (__pyx_t_32 = __pyx_v_x1; __pyx_t_32 < __pyx_t_31; __pyx_t_32+=1) {
       __pyx_v_i = __pyx_t_32;
 
-      /* "pyrle/src/rle.pyx":524
+      /* "pyrle/src/rle.pyx":522
  * 
  *         for i in range(x1, l1):
  *             nv = 0 if np.isfinite(values1[i]) else np.nan             # <<<<<<<<<<<<<<
  * 
  *             if np.isclose(nv, nvs[xn - 1]):
  */
-      __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 522, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 522, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_46 = __pyx_v_i;
-      __pyx_t_5 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values1.data) + __pyx_t_46)) )))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_5 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_values1.data) + __pyx_t_46)) )))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 522, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       if (!__pyx_t_4) {
-        __pyx_t_22 = __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_5); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 524, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_5); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 522, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_22);
       } else {
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_9)) {
           PyObject *__pyx_temp[2] = {__pyx_t_4, __pyx_t_5};
-          __pyx_t_22 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 524, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 522, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
           PyObject *__pyx_temp[2] = {__pyx_t_4, __pyx_t_5};
-          __pyx_t_22 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 524, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-1, 1+1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 522, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(1+1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 524, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(1+1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 522, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4); __pyx_t_4 = NULL;
           __Pyx_GIVEREF(__pyx_t_5);
           PyTuple_SET_ITEM(__pyx_t_8, 0+1, __pyx_t_5);
           __pyx_t_5 = 0;
-          __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_8, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 524, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_8, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 522, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
       }
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 522, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       if (__pyx_t_12) {
         __pyx_t_27 = 0.0;
       } else {
-        __pyx_t_22 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 524, __pyx_L1_error)
+        __pyx_t_22 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 522, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
-        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_nan); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 524, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_nan); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 522, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-        __pyx_t_29 = __pyx_PyFloat_AsDouble(__pyx_t_9); if (unlikely((__pyx_t_29 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 524, __pyx_L1_error)
+        __pyx_t_29 = __pyx_PyFloat_AsDouble(__pyx_t_9); if (unlikely((__pyx_t_29 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 522, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __pyx_t_27 = __pyx_t_29;
       }
       __pyx_v_nv = __pyx_t_27;
 
-      /* "pyrle/src/rle.pyx":526
+      /* "pyrle/src/rle.pyx":524
  *             nv = 0 if np.isfinite(values1[i]) else np.nan
  * 
  *             if np.isclose(nv, nvs[xn - 1]):             # <<<<<<<<<<<<<<
  *                 nrs[xn - 1] += runs1[i]
  *             else:
  */
-      __pyx_t_22 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_GetModuleGlobalName(__pyx_n_s_np); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_isclose); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_isclose); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-      __pyx_t_22 = PyFloat_FromDouble(__pyx_v_nv); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_22 = PyFloat_FromDouble(__pyx_v_nv); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
       __pyx_t_47 = (__pyx_v_xn - 1);
-      __pyx_t_5 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_47)) )))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_5 = PyFloat_FromDouble((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_47)) )))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_4 = NULL;
       __pyx_t_36 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -9293,176 +9293,176 @@
           __Pyx_DECREF_SET(__pyx_t_8, function);
           __pyx_t_36 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_8)) {
         PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_22, __pyx_t_5};
-        __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_36, 2+__pyx_t_36); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 526, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_36, 2+__pyx_t_36); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 524, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
         PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_22, __pyx_t_5};
-        __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_36, 2+__pyx_t_36); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 526, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_36, 2+__pyx_t_36); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 524, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       } else
       #endif
       {
-        __pyx_t_7 = PyTuple_New(2+__pyx_t_36); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 526, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_New(2+__pyx_t_36); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 524, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         if (__pyx_t_4) {
           __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_22);
         PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_36, __pyx_t_22);
         __Pyx_GIVEREF(__pyx_t_5);
         PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_36, __pyx_t_5);
         __pyx_t_22 = 0;
         __pyx_t_5 = 0;
-        __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_7, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 526, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_7, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 524, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 526, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       if (__pyx_t_12) {
 
-        /* "pyrle/src/rle.pyx":527
+        /* "pyrle/src/rle.pyx":525
  * 
  *             if np.isclose(nv, nvs[xn - 1]):
  *                 nrs[xn - 1] += runs1[i]             # <<<<<<<<<<<<<<
  *             else:
- *                 nrs[xn] = runs1[i]
+ *                 nrs[xn] += runs1[i]
  */
         __pyx_t_48 = __pyx_v_i;
         __pyx_t_49 = (__pyx_v_xn - 1);
         *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_49)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs1.data) + __pyx_t_48)) )));
 
-        /* "pyrle/src/rle.pyx":526
+        /* "pyrle/src/rle.pyx":524
  *             nv = 0 if np.isfinite(values1[i]) else np.nan
  * 
  *             if np.isclose(nv, nvs[xn - 1]):             # <<<<<<<<<<<<<<
  *                 nrs[xn - 1] += runs1[i]
  *             else:
  */
         goto __pyx_L27;
       }
 
-      /* "pyrle/src/rle.pyx":529
+      /* "pyrle/src/rle.pyx":527
  *                 nrs[xn - 1] += runs1[i]
  *             else:
- *                 nrs[xn] = runs1[i]             # <<<<<<<<<<<<<<
+ *                 nrs[xn] += runs1[i]             # <<<<<<<<<<<<<<
  *                 nvs[xn] = nv
  *                 xn += 1
  */
       /*else*/ {
         __pyx_t_50 = __pyx_v_i;
         __pyx_t_51 = __pyx_v_xn;
-        *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_51)) )) = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs1.data) + __pyx_t_50)) )));
+        *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_nrs.data) + __pyx_t_51)) )) += (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_runs1.data) + __pyx_t_50)) )));
 
-        /* "pyrle/src/rle.pyx":530
+        /* "pyrle/src/rle.pyx":528
  *             else:
- *                 nrs[xn] = runs1[i]
+ *                 nrs[xn] += runs1[i]
  *                 nvs[xn] = nv             # <<<<<<<<<<<<<<
  *                 xn += 1
  * 
  */
         __pyx_t_52 = __pyx_v_xn;
         *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_nvs.data) + __pyx_t_52)) )) = __pyx_v_nv;
 
-        /* "pyrle/src/rle.pyx":531
- *                 nrs[xn] = runs1[i]
+        /* "pyrle/src/rle.pyx":529
+ *                 nrs[xn] += runs1[i]
  *                 nvs[xn] = nv
  *                 xn += 1             # <<<<<<<<<<<<<<
  * 
  *     # Must use resize because initial guess for array was likely way too large
  */
         __pyx_v_xn = (__pyx_v_xn + 1);
       }
       __pyx_L27:;
     }
 
-    /* "pyrle/src/rle.pyx":515
+    /* "pyrle/src/rle.pyx":513
  * 
  *     # (If self had largest sum of lengths)
  *     elif x2 == l2 and not x1 == l1:             # <<<<<<<<<<<<<<
+ * 
  *         if diff > 0:
- *             nrs[xn] = r1
  */
   }
   __pyx_L15:;
 
-  /* "pyrle/src/rle.pyx":534
+  /* "pyrle/src/rle.pyx":532
  * 
  *     # Must use resize because initial guess for array was likely way too large
  *     nrs_arr.resize(xn, refcheck=False)             # <<<<<<<<<<<<<<
  *     nvs_arr.resize(xn, refcheck=False)
  * 
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_nrs_arr, __pyx_n_s_resize); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_nrs_arr, __pyx_n_s_resize); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 532, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_xn); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_xn); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 532, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 532, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 532, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_refcheck, Py_False) < 0) __PYX_ERR(0, 534, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 534, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_refcheck, Py_False) < 0) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 532, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyrle/src/rle.pyx":535
+  /* "pyrle/src/rle.pyx":533
  *     # Must use resize because initial guess for array was likely way too large
  *     nrs_arr.resize(xn, refcheck=False)
  *     nvs_arr.resize(xn, refcheck=False)             # <<<<<<<<<<<<<<
  * 
  *     return nrs_arr, nvs_arr
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_nvs_arr, __pyx_n_s_resize); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_nvs_arr, __pyx_n_s_resize); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_xn); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_xn); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_refcheck, Py_False) < 0) __PYX_ERR(0, 535, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 535, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_refcheck, Py_False) < 0) __PYX_ERR(0, 533, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "pyrle/src/rle.pyx":537
+  /* "pyrle/src/rle.pyx":535
  *     nvs_arr.resize(xn, refcheck=False)
  * 
  *     return nrs_arr, nvs_arr             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 537, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_INCREF(__pyx_v_nrs_arr);
   __Pyx_GIVEREF(__pyx_v_nrs_arr);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_nrs_arr);
   __Pyx_INCREF(__pyx_v_nvs_arr);
   __Pyx_GIVEREF(__pyx_v_nvs_arr);
   PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_nvs_arr);
@@ -9470,16 +9470,16 @@
   __pyx_t_9 = 0;
   goto __pyx_L0;
 
   /* "pyrle/src/rle.pyx":437
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef mul_rles(long [::1] runs1, double [::1] values1, long [::1] runs2, double [::1] values2):             # <<<<<<<<<<<<<<
- * 
  *     cdef int x1 = 0
+ *     cdef int x2 = 0
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
```

### Comparing `pyrle-0.0.8/pyrle/rledict.py` & `pyrle-0.0.9/pyrle/rledict.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/pyrle/rle.py` & `pyrle-0.0.9/pyrle/rle.py`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/PKG-INFO` & `pyrle-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyrle
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/endrebak/pyrle
 Author: Endre Bakken Stovner
 Author-email: endrebak85@gmail.com
 License: ['MIT']
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyrle-0.0.8/setup.py` & `pyrle-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 e2 = Extension("pyrle.src.coverage", ["pyrle/src/coverage.pyx"], define_macros = macros)
 
 extensions = [e1, e2]
 
 install_requires = ["cython", "pandas", "tabulate", "numpy", "natsort"]
 
 setup(name='pyrle',
-      version="0.0.8",
+      version="0.0.9",
       packages=find_packages(),
       ext_modules=cythonize(extensions),
       install_requires=install_requires,
       author="Endre Bakken Stovner",
       author_email="endrebak85@gmail.com",
       url="https://github.com/endrebak/pyrle",
       license=["MIT"],
```

### Comparing `pyrle-0.0.8/pyrle.egg-info/SOURCES.txt` & `pyrle-0.0.9/pyrle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrle-0.0.8/pyrle.egg-info/PKG-INFO` & `pyrle-0.0.9/pyrle.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyrle
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/endrebak/pyrle
 Author: Endre Bakken Stovner
 Author-email: endrebak85@gmail.com
 License: ['MIT']
 Description: UNKNOWN
 Platform: UNKNOWN
```

