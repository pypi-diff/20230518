# Comparing `tmp/ds_caselaw_utils-1.0.0.tar.gz` & `tmp/ds_caselaw_utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_caselaw_utils-1.0.0.tar", max compression
+gzip compressed data, was "ds_caselaw_utils-1.0.1.tar", max compression
```

## Comparing `ds_caselaw_utils-1.0.0.tar` & `ds_caselaw_utils-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1108 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     4132 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/README.md
--rw-r--r--   0        0        0      617 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       12 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/.gitignore
--rw-r--r--   0        0        0       75 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/__init__.py
--rw-r--r--   0        0        0     3062 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/courts.py
--rw-r--r--   0        0        0      709 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/data/README.md
--rw-r--r--   0        0        0    12780 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/data/court_names.yaml
--rw-r--r--   0        0        0      615 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/data/neutral_citation_regex.yaml
--rw-r--r--   0        0        0      656 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/neutral.py
--rw-r--r--   0        0        0     6899 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/test_courts.py
--rw-r--r--   0        0        0     1395 2023-04-12 15:25:13.646979 ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/test_neutral.py
--rw-r--r--   0        0        0     4782 1970-01-01 00:00:00.000000 ds_caselaw_utils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     4132 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/README.md
+-rw-r--r--   0        0        0      617 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/.gitignore
+-rw-r--r--   0        0        0       75 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/__init__.py
+-rw-r--r--   0        0        0     3062 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/courts.py
+-rw-r--r--   0        0        0      709 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/README.md
+-rw-r--r--   0        0        0    15200 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/court_names.yaml
+-rw-r--r--   0        0        0      615 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/neutral_citation_regex.yaml
+-rw-r--r--   0        0        0      656 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/neutral.py
+-rw-r--r--   0        0        0     6899 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/test_courts.py
+-rw-r--r--   0        0        0     1395 2023-05-18 10:46:26.935196 ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/test_neutral.py
+-rw-r--r--   0        0        0     4782 1970-01-01 00:00:00.000000 ds_caselaw_utils-1.0.1/PKG-INFO
```

### Comparing `ds_caselaw_utils-1.0.0/LICENSE.md` & `ds_caselaw_utils-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.0/README.md` & `ds_caselaw_utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.0/pyproject.toml` & `ds_caselaw_utils-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ds_caselaw_utils"
-version = "1.0.0"
+version = "1.0.1"
 description = "Utilities for the National Archives Caselaw project"
 authors = ["Nick Jackson <nick@dxw.com>", "David McKee <dragon@dxw.com>", "Tim Cowlishaw <tim@timcowlishaw.co.uk>", "Laura Porter <laura@dxw.com>"]
 license = "MIT"
 homepage = "https://github.com/nationalarchives/ds-caselaw-utils"
 keywords = ["national archives", "caselaw"]
 readme = "README.md"
```

### Comparing `ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/courts.py` & `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/courts.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/data/README.md` & `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/README.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/data/court_names.yaml` & `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/court_names.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -64,25 +64,47 @@
         ncn: \[(\d{4})\] (EWHC) (\d+) \((Admin)\)
         param: 'ewhc/admin'
         start_year: 2003
         end_year: 2022
         selectable: true
         listable: true
     -
+        code: EWHC-KBD-Admin
+        name: Administrative Court
+        list_name: High Court (Administrative Court)
+        link: https://www.gov.uk/courts-tribunals/administrative-court
+        ncn: \[(\d{4})\] (EWHC) (\d+) \((Admin)\)
+        param: 'ewhc/admin'
+        start_year: 2022
+        end_year: 2022
+        selectable: false
+        listable: false
+    -
         code: EWHC-QBD-Admiralty
         name: Admiralty Court
         list_name: High Court (Admiralty Division)
         link: https://www.gov.uk/courts-tribunals/admiralty-court
         ncn: \[(\d{4})\] (EWHC) (\d+) \((Admlty)\)
         param: 'ewhc/admlty'
         start_year: 2003
         end_year: 2022
         selectable: true
         listable: true
     -
+        code: EWHC-KBD-Admiralty
+        name: Admiralty Court
+        list_name: High Court (Admiralty Division)
+        link: https://www.gov.uk/courts-tribunals/admiralty-court
+        ncn: \[(\d{4})\] (EWHC) (\d+) \((Admlty)\)
+        param: 'ewhc/admlty'
+        start_year: 2022
+        end_year: 2022
+        selectable: false
+        listable: false
+    -
         code: EWHC-Chancery
         name: Chancery Division of the High Court
         list_name: High Court (Chancery Division)
         link: https://www.gov.uk/courts-tribunals/chancery-division-of-the-high-court
         ncn: \[(\d{4})\] (EWHC) (\d+) \((Ch)\)
         param: 'ewhc/ch'
         start_year: 2003
@@ -97,14 +119,25 @@
         ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
         param: 'ewhc/comm'
         start_year: 2003
         end_year: 2022
         selectable: true
         listable: true
     -
+        code: EWHC-KBD-Commercial
+        name: Commercial Court
+        list_name: High Court (Commercial Court)
+        link: https://www.gov.uk/courts-tribunals/commercial-court
+        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+        param: 'ewhc/comm'
+        start_year: 2022
+        end_year: 2022
+        selectable: false
+        listable: false
+    -
         code: EWHC-SeniorCourtsCosts
         name: Senior Courts Costs Office
         list_name: High Court (Senior Court Costs Office)
         link: https://www.gov.uk/courts-tribunals/senior-courts-costs-office
         ncn: \[(\d{4})\] (EWHC) (\d+) \((SCCO)\)
         param: 'ewhc/scco'
         extra_params: ['ewhc/costs']
@@ -194,14 +227,25 @@
         ncn: \[(\d{4})\] (EWHC) (\d+) \((TCC)\)
         param: 'ewhc/tcc'
         start_year: 2003
         end_year: 2022
         selectable: true
         listable: true
     -
+        code: EWHC-KBD-TCC
+        name: Technology and Construction Court
+        list_name: High Court (Technology and Construction Court)
+        link: https://www.gov.uk/courts-tribunals/technology-and-construction-court
+        ncn: \[(\d{4})\] (EWHC) (\d+) \((TCC)\)
+        param: 'ewhc/tcc'
+        start_year: 2022
+        end_year: 2022
+        selectable: false
+        listable: false
+    -
         code: EWCOP
         name: Court of Protection
         link: https://www.gov.uk/courts-tribunals/court-of-protection
         ncn: \[(\d{4})\] (EWCOP) (\d+)
         param: 'ewcop'
         start_year: 2009
         end_year: 2022
@@ -220,35 +264,60 @@
     -
         code: EWHC-QBD-Planning
         name: Planning Court
         link: https://www.gov.uk/courts-tribunals/planning-court
         selectable: false
         listable: false
     -
+        code: EWHC-KBD-Planning
+        name: Planning Court
+        link: https://www.gov.uk/courts-tribunals/planning-court
+        selectable: false
+        listable: false
+    -
         code: EWHC-QBD-BusinessAndProperty
         name: The Business and Property Courts
         link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
         selectable: false
         listable: false
-
+    -
+        code: EWHC-KBD-BusinessAndProperty
+        name: The Business and Property Courts
+        link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
+        selectable: false
+        listable: false
     -
         code: EWHC-QBD-Commercial-Financial
         name: The Financial List
         link: https://www.gov.uk/courts-tribunals/the-financial-list
         ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
         selectable: false
         listable: false
     -
+        code: EWHC-KBD-Commercial-Financial
+        name: The Financial List
+        link: https://www.gov.uk/courts-tribunals/the-financial-list
+        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+        selectable: false
+        listable: false
+    -
         code: EWHC-QBD-Commercial-Circuit
         name: Circuit Commercial Court
         link: https://www.gov.uk/courts-tribunals/commercial-circuit-court
         ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
         selectable: false
         listable: false
     -
+        code: EWHC-KBD-Commercial-Circuit
+        name: Circuit Commercial Court
+        link: https://www.gov.uk/courts-tribunals/commercial-circuit-court
+        ncn: \[(\d{4})\] (EWHC) (\d+) \((Comm)\)
+        selectable: false
+        listable: false
+    -
         code: EWHC-Chancery-BusinessAndProperty
         name: The Business and Property Courts
         link: https://www.gov.uk/courts-tribunals/the-business-and-property-courts
         selectable: false
         listable: false
     -
         code: EWHC-Chancery-Business
```

### Comparing `ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/data/neutral_citation_regex.yaml` & `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/data/neutral_citation_regex.yaml`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/neutral.py` & `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/neutral.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/test_courts.py` & `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/test_courts.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.0/src/ds_caselaw_utils/test_neutral.py` & `ds_caselaw_utils-1.0.1/src/ds_caselaw_utils/test_neutral.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_utils-1.0.0/PKG-INFO` & `ds_caselaw_utils-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds-caselaw-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utilities for the National Archives Caselaw project
 Home-page: https://github.com/nationalarchives/ds-caselaw-utils
 License: MIT
 Keywords: national archives,caselaw
 Author: Nick Jackson
 Author-email: nick@dxw.com
 Requires-Python: >=3.9,<4.0
```

