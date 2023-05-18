# Comparing `tmp/bert_schemas-1.17.0.tar.gz` & `tmp/bert_schemas-1.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_schemas-1.17.0.tar", max compression
+gzip compressed data, was "bert_schemas-1.18.0.tar", max compression
```

## Comparing `bert_schemas-1.17.0.tar` & `bert_schemas-1.18.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0      481 2023-05-08 17:00:22.488612 bert_schemas-1.17.0/README.md
--rw-r--r--   0        0        0       72 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/__init__.py
--rw-r--r--   0        0        0      302 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/group.py
--rw-r--r--   0        0        0    45398 2023-05-08 16:25:47.915204 bert_schemas-1.17.0/bert_schemas/job.py
--rw-r--r--   0        0        0      770 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/message.py
--rw-r--r--   0        0        0     1967 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/questionnaire.py
--rw-r--r--   0        0        0      175 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/report.py
--rw-r--r--   0        0        0       51 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/factories/__init__.py
--rw-r--r--   0        0        0      492 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/factories/helpers.py
--rw-r--r--   0        0        0        0 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/factories/job/__init__.py
--rw-r--r--   0        0        0     2713 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/factories/job/barrier.py
--rw-r--r--   0        0        0     2509 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/factories/job/bec.py
--rw-r--r--   0        0        0     2611 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/factories/job/bragg.py
--rw-r--r--   0        0        0     2715 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/factories/job/paint_1d.py
--rw-r--r--   0        0        0     2866 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/factories/job/transistor.py
--rw-r--r--   0        0        0        0 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/fixtures/__init__.py
--rw-r--r--   0        0        0     9136 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/__init__.py
--rw-r--r--   0        0        0     6071 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/barrier.py
--rw-r--r--   0        0        0     5811 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/bec.py
--rw-r--r--   0        0        0     5945 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/bragg.py
--rw-r--r--   0        0        0     6113 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/paint_1d.py
--rw-r--r--   0        0        0     6248 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/transistor.py
--rw-r--r--   0        0        0        0 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/schemas/__init__.py
--rw-r--r--   0        0        0     1568 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/schemas/job/__init__.py
--rw-r--r--   0        0        0     2275 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/schemas/job/barrier.py
--rw-r--r--   0        0        0     2180 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/schemas/job/bec.py
--rw-r--r--   0        0        0     2197 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/schemas/job/bragg.py
--rw-r--r--   0        0        0     2368 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/schemas/job/paint_1d.py
--rw-r--r--   0        0        0     2340 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/schemas/job/shared.py
--rw-r--r--   0        0        0     2465 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/testing/schemas/job/transistor.py
--rw-r--r--   0        0        0     1950 2023-05-02 21:54:37.676186 bert_schemas-1.17.0/bert_schemas/user.py
--rw-r--r--   0        0        0     1329 2023-05-08 18:02:42.367134 bert_schemas-1.17.0/pyproject.toml
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 bert_schemas-1.17.0/PKG-INFO
+-rw-r--r--   0        0        0      481 2023-05-15 14:27:01.954881 bert_schemas-1.18.0/README.md
+-rw-r--r--   0        0        0       80 2023-05-15 14:27:01.954881 bert_schemas-1.18.0/bert_schemas/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-15 14:27:01.954881 bert_schemas-1.18.0/bert_schemas/access.py
+-rw-r--r--   0        0        0      357 2023-05-15 14:27:01.954881 bert_schemas-1.18.0/bert_schemas/group.py
+-rw-r--r--   0        0        0    45200 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/job.py
+-rw-r--r--   0        0        0      770 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/message.py
+-rw-r--r--   0        0        0     1967 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/questionnaire.py
+-rw-r--r--   0        0        0      175 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/report.py
+-rw-r--r--   0        0        0       51 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/factories/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/factories/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/factories/job/__init__.py
+-rw-r--r--   0        0        0     2713 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/barrier.py
+-rw-r--r--   0        0        0     2509 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/bec.py
+-rw-r--r--   0        0        0     2611 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/bragg.py
+-rw-r--r--   0        0        0     2715 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/paint_1d.py
+-rw-r--r--   0        0        0     2866 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/transistor.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/fixtures/__init__.py
+-rw-r--r--   0        0        0     9136 2023-04-26 21:05:16.851464 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/__init__.py
+-rw-r--r--   0        0        0     6071 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/barrier.py
+-rw-r--r--   0        0        0     5811 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/bec.py
+-rw-r--r--   0        0        0     5945 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/bragg.py
+-rw-r--r--   0        0        0     6113 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/paint_1d.py
+-rw-r--r--   0        0        0     6248 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/transistor.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/schemas/__init__.py
+-rw-r--r--   0        0        0     1568 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/__init__.py
+-rw-r--r--   0        0        0     2275 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/barrier.py
+-rw-r--r--   0        0        0     2180 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/bec.py
+-rw-r--r--   0        0        0     2197 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/bragg.py
+-rw-r--r--   0        0        0     2368 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/paint_1d.py
+-rw-r--r--   0        0        0     2340 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/shared.py
+-rw-r--r--   0        0        0     2465 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/transistor.py
+-rw-r--r--   0        0        0     1950 2023-05-18 13:19:14.771500 bert_schemas-1.18.0/bert_schemas/user.py
+-rw-r--r--   0        0        0     1329 2023-05-18 17:48:19.987547 bert_schemas-1.18.0/pyproject.toml
+-rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 bert_schemas-1.18.0/setup.py
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 bert_schemas-1.18.0/PKG-INFO
```

### Comparing `bert_schemas-1.17.0/bert_schemas/job.py` & `bert_schemas-1.18.0/bert_schemas/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,14 @@
     ONLINE = "ONLINE"
     OFFLINE = "OFFLINE"
 
     def __str__(self):
         return str(self.value)
 
 
-class DayOfWeek(StrEnum):
-    MONDAY = "MONDAY"
-    TUESDAY = "TUESDAY"
-    WEDNESDAY = "WEDNESDAY"
-    THURSDAY = "THURSDAY"
-    FRIDAY = "FRIDAY"
-    SATURDAY = "SATURDAY"
-    SUNDAY = "SUNDAY"
-
-
 class JobOrigin(StrEnum):
     WEB = auto()
     OQTANT = auto()
 
 
 class JobType(StrEnum):
     BEC = "BEC"
```

### Comparing `bert_schemas-1.17.0/bert_schemas/message.py` & `bert_schemas-1.18.0/bert_schemas/message.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/questionnaire.py` & `bert_schemas-1.18.0/bert_schemas/questionnaire.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/factories/job/barrier.py` & `bert_schemas-1.18.0/bert_schemas/testing/factories/job/barrier.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/factories/job/bec.py` & `bert_schemas-1.18.0/bert_schemas/testing/factories/job/bec.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/factories/job/bragg.py` & `bert_schemas-1.18.0/bert_schemas/testing/factories/job/bragg.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/factories/job/paint_1d.py` & `bert_schemas-1.18.0/bert_schemas/testing/factories/job/paint_1d.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/factories/job/transistor.py` & `bert_schemas-1.18.0/bert_schemas/testing/factories/job/transistor.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/__init__.py` & `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/barrier.py` & `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/barrier.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/bec.py` & `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/bec.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/bragg.py` & `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/bragg.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/paint_1d.py` & `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/paint_1d.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/fixtures/job/transistor.py` & `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/transistor.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/schemas/job/__init__.py` & `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/schemas/job/barrier.py` & `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/barrier.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/schemas/job/bec.py` & `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/bec.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/schemas/job/bragg.py` & `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/bragg.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/schemas/job/paint_1d.py` & `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/paint_1d.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/schemas/job/shared.py` & `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/shared.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/testing/schemas/job/transistor.py` & `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/transistor.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/bert_schemas/user.py` & `bert_schemas-1.18.0/bert_schemas/user.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.17.0/pyproject.toml` & `bert_schemas-1.18.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bert-schemas"
-version = "1.17.0"
+version = "1.18.0"
 description = "Bert service schemas"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
 exclude = ["**/.pytest_cache/**/*", "**/__pycache__", ".gitignore"]
```

### Comparing `bert_schemas-1.17.0/PKG-INFO` & `bert_schemas-1.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-schemas
-Version: 1.17.0
+Version: 1.18.0
 Summary: Bert service schemas
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

