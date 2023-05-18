# Comparing `tmp/prodiapy-2.5.tar.gz` & `tmp/prodiapy-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-2.5.tar", last modified: Wed May 17 08:02:23 2023, max compression
+gzip compressed data, was "prodiapy-2.6.tar", last modified: Thu May 18 10:11:04 2023, max compression
```

## Comparing `prodiapy-2.5.tar` & `prodiapy-2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 08:02:23.230169 prodiapy-2.5/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-2.5/LICENSE
--rw-rw-rw-   0        0        0     1039 2023-05-17 08:02:23.229170 prodiapy-2.5/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-05-17 08:01:08.000000 prodiapy-2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 08:02:23.209890 prodiapy-2.5/prodia/
--rw-rw-rw-   0        0        0      132 2023-05-17 08:01:33.000000 prodiapy-2.5/prodia/__init__.py
--rw-rw-rw-   0        0        0     2290 2023-05-16 11:51:42.000000 prodiapy-2.5/prodia/data.py
--rw-rw-rw-   0        0        0    15010 2023-05-17 07:59:57.000000 prodiapy-2.5/prodia/main.py
-drwxrwxrwx   0        0        0        0 2023-05-17 08:02:23.228170 prodiapy-2.5/prodiapy.egg-info/
--rw-rw-rw-   0        0        0     1039 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 08:02:23.230169 prodiapy-2.5/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-05-16 11:04:01.000000 prodiapy-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:11:04.680724 prodiapy-2.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-2.6/LICENSE
+-rw-rw-rw-   0        0        0     1039 2023-05-18 10:11:04.679238 prodiapy-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-05-17 08:01:08.000000 prodiapy-2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 10:11:04.666673 prodiapy-2.6/prodia/
+-rw-rw-rw-   0        0        0      132 2023-05-17 08:01:33.000000 prodiapy-2.6/prodia/__init__.py
+-rw-rw-rw-   0        0        0     2290 2023-05-16 11:51:42.000000 prodiapy-2.6/prodia/data.py
+-rw-rw-rw-   0        0        0    15009 2023-05-17 08:47:07.000000 prodiapy-2.6/prodia/main.py
+drwxrwxrwx   0        0        0        0 2023-05-18 10:11:04.679238 prodiapy-2.6/prodiapy.egg-info/
+-rw-rw-rw-   0        0        0     1039 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 10:11:04.681228 prodiapy-2.6/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-05-17 08:45:42.000000 prodiapy-2.6/setup.py
```

### Comparing `prodiapy-2.5/LICENSE` & `prodiapy-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-2.5/PKG-INFO` & `prodiapy-2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 2.5
+Version: 2.6
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `prodiapy-2.5/README.md` & `prodiapy-2.6/README.md`

 * *Files identical despite different names*

### Comparing `prodiapy-2.5/prodia/data.py` & `prodiapy-2.6/prodia/data.py`

 * *Files identical despite different names*

### Comparing `prodiapy-2.5/prodia/main.py` & `prodiapy-2.6/prodia/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         response = requests.post(url, json=payload, headers=headers)
         job_id = response.json()['job']
         time.sleep(3)
 
         retrieve_url = f'https://api.prodia.com/v1/job/{job_id}'
         stt = True
         while stt is True:
-            rec = requests.get(retrieve_url, headers=headersr2)
+            rec = requests.get(retrieve_url, headers=headers2)
             status = rec.json()['status']
             if status == "succeeded":
                 print(f"Image {job_id} generated!")
                 image_url = rec.json()['imageUrl']
                 stt = False
                 return image_url
             elif status == "queued":
```

### Comparing `prodiapy-2.5/prodiapy.egg-info/PKG-INFO` & `prodiapy-2.6/prodiapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 2.5
+Version: 2.6
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

