# Comparing `tmp/hkbot-2.1.2.tar.gz` & `tmp/hkbot-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkbot-2.1.2.tar", last modified: Wed May 17 22:43:48 2023, max compression
+gzip compressed data, was "hkbot-2.1.3.tar", last modified: Wed May 17 23:27:03 2023, max compression
```

## Comparing `hkbot-2.1.2.tar` & `hkbot-2.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 22:43:48.688888 hkbot-2.1.2/
--rw-rw-rw-   0        0        0     2220 2023-05-17 22:43:48.688888 hkbot-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2077 2023-05-15 05:26:42.000000 hkbot-2.1.2/README.md
--rw-rw-rw-   0        0        0  1285403 2023-05-17 22:43:25.000000 hkbot-2.1.2/hkbot.c
-drwxrwxrwx   0        0        0        0 2023-05-17 22:43:48.686890 hkbot-2.1.2/hkbot.egg-info/
--rw-rw-rw-   0        0        0     2220 2023-05-17 22:43:48.000000 hkbot-2.1.2/hkbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-05-17 22:43:48.000000 hkbot-2.1.2/hkbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 22:43:48.000000 hkbot-2.1.2/hkbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-17 22:43:48.000000 hkbot-2.1.2/hkbot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-05-17 22:43:48.000000 hkbot-2.1.2/hkbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-17 22:43:48.000000 hkbot-2.1.2/hkbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 22:43:48.689892 hkbot-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-05-17 22:28:26.000000 hkbot-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 23:27:03.809540 hkbot-2.1.3/
+-rw-rw-rw-   0        0        0     2220 2023-05-17 23:27:03.808543 hkbot-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2077 2023-05-15 05:26:42.000000 hkbot-2.1.3/README.md
+-rw-rw-rw-   0        0        0  1285035 2023-05-17 23:26:43.000000 hkbot-2.1.3/hkbot.c
+drwxrwxrwx   0        0        0        0 2023-05-17 23:27:03.805535 hkbot-2.1.3/hkbot.egg-info/
+-rw-rw-rw-   0        0        0     2220 2023-05-17 23:27:03.000000 hkbot-2.1.3/hkbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-17 23:27:03.000000 hkbot-2.1.3/hkbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 23:27:03.000000 hkbot-2.1.3/hkbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-17 23:27:03.000000 hkbot-2.1.3/hkbot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-05-17 23:27:03.000000 hkbot-2.1.3/hkbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-17 23:27:03.000000 hkbot-2.1.3/hkbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 23:27:03.809540 hkbot-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-05-17 23:26:18.000000 hkbot-2.1.3/setup.py
```

### Comparing `hkbot-2.1.2/PKG-INFO` & `hkbot-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkbot
-Version: 2.1.2
+Version: 2.1.3
 Summary: hkbot automation
 Author: AkasakaID
 Description-Content-Type: text/markdown
 
 # HKBOT Automation
 
 a program created to help complete tasks from hkbot telegram
```

### Comparing `hkbot-2.1.2/README.md` & `hkbot-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hkbot-2.1.2/hkbot.c` & `hkbot-2.1.3/hkbot.c`

 * *Files 0% similar despite different names*

```diff
@@ -22984,26 +22984,18 @@
  
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_5hkbot_3getConfig, 0, __pyx_n_s_getConfig, NULL, __pyx_n_s_hkbot, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_getConfig, __pyx_t_5) < 0) __PYX_ERR(0, 941, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
  
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_main); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 967, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 967, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
- 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
  
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
```

### Comparing `hkbot-2.1.2/hkbot.egg-info/PKG-INFO` & `hkbot-2.1.3/hkbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkbot
-Version: 2.1.2
+Version: 2.1.3
 Summary: hkbot automation
 Author: AkasakaID
 Description-Content-Type: text/markdown
 
 # HKBOT Automation
 
 a program created to help complete tasks from hkbot telegram
```

### Comparing `hkbot-2.1.2/setup.py` & `hkbot-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 0d0a 6672 6f6d 2070 6174 686c 6962 2069  ..from pathlib i
 00000010: 6d70 6f72 7420 5061 7468 0d0a 6672 6f6d  mport Path..from
 00000020: 2073 6574 7570 746f 6f6c 7320 696d 706f   setuptools impo
 00000030: 7274 2073 6574 7570 2c20 4578 7465 6e73  rt setup, Extens
 00000040: 696f 6e0d 0a0d 0a76 6572 7369 6f6e 203d  ion....version =
-00000050: 2022 322e 312e 3222 0d0a 6578 7465 6e73   "2.1.2"..extens
+00000050: 2022 322e 312e 3322 0d0a 6578 7465 6e73   "2.1.3"..extens
 00000060: 696f 6e5f 6e61 6d65 203d 2022 6322 0d0a  ion_name = "c"..
 00000070: 6865 7265 203d 2050 6174 682e 6377 6428  here = Path.cwd(
 00000080: 290d 0a74 6869 735f 6469 7265 6374 6f72  )..this_director
 00000090: 7920 3d20 5061 7468 285f 5f66 696c 655f  y = Path(__file_
 000000a0: 5f29 2e70 6172 656e 740d 0a6c 6f6e 675f  _).parent..long_
 000000b0: 6465 7363 7269 7074 696f 6e20 3d20 2874  description = (t
 000000c0: 6869 735f 6469 7265 6374 6f72 7920 2f20  his_directory /
```

