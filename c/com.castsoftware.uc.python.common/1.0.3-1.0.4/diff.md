# Comparing `tmp/com.castsoftware.uc.python.common-1.0.3.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-1.0.3.tar", last modified: Tue May 16 19:13:49 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.0.4.tar", last modified: Thu May 18 17:41:39 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-1.0.3.tar` & `com.castsoftware.uc.python.common-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:13:49.416673 com.castsoftware.uc.python.common-1.0.3/
--rw-rw-rw-   0        0        0    35823 2021-04-05 17:40:19.000000 com.castsoftware.uc.python.common-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      712 2023-05-16 19:13:49.408530 com.castsoftware.uc.python.common-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      103 2021-06-01 15:37:40.000000 com.castsoftware.uc.python.common-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 19:13:49.334258 com.castsoftware.uc.python.common-1.0.3/cast_common/
--rw-rw-rw-   0        0        0        0 2023-05-16 12:52:23.000000 com.castsoftware.uc.python.common-1.0.3/cast_common/__init__.py
--rw-rw-rw-   0        0        0     2036 2023-05-16 12:52:23.000000 com.castsoftware.uc.python.common-1.0.3/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    11962 2023-05-16 12:52:23.000000 com.castsoftware.uc.python.common-1.0.3/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0     3386 2023-05-16 19:11:27.000000 com.castsoftware.uc.python.common-1.0.3/cast_common/highlight.py
--rw-rw-rw-   0        0        0     5563 2023-05-16 12:57:24.000000 com.castsoftware.uc.python.common-1.0.3/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1688 2023-05-16 12:58:08.000000 com.castsoftware.uc.python.common-1.0.3/cast_common/logger.py
--rw-rw-rw-   0        0        0     5930 2023-05-16 12:52:23.000000 com.castsoftware.uc.python.common-1.0.3/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     6054 2023-05-16 12:59:39.000000 com.castsoftware.uc.python.common-1.0.3/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:13:49.392586 com.castsoftware.uc.python.common-1.0.3/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      712 2023-05-16 19:13:49.000000 com.castsoftware.uc.python.common-1.0.3/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-16 19:13:49.000000 com.castsoftware.uc.python.common-1.0.3/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:13:49.000000 com.castsoftware.uc.python.common-1.0.3/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 19:13:49.000000 com.castsoftware.uc.python.common-1.0.3/com.castsoftware.uc.python.common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 19:13:49.000000 com.castsoftware.uc.python.common-1.0.3/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      628 2023-05-16 19:13:28.000000 com.castsoftware.uc.python.common-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 19:13:49.416673 com.castsoftware.uc.python.common-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-18 17:41:39.118391 com.castsoftware.uc.python.common-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      714 2023-05-18 17:41:39.109952 com.castsoftware.uc.python.common-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 17:41:39.037442 com.castsoftware.uc.python.common-1.0.4/cast_common/
+-rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    11811 2023-05-18 15:27:04.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0     4069 2023-05-18 15:21:32.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/highlight.py
+-rw-rw-rw-   0        0        0     5478 2023-05-18 15:25:57.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1688 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/logger.py
+-rw-rw-rw-   0        0        0     3823 2023-05-18 15:32:24.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     6930 2023-05-18 15:27:50.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2023-05-18 17:41:39.096689 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      630 2023-05-18 17:34:18.000000 com.castsoftware.uc.python.common-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-18 17:41:39.118391 com.castsoftware.uc.python.common-1.0.4/setup.cfg
```

### Comparing `com.castsoftware.uc.python.common-1.0.3/LICENSE` & `com.castsoftware.uc.python.common-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.3/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.3
+Version: 1.0.4
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # com.castsoftware.uc.python.common
 A set of common classes and methods for use with python projects
```

### Comparing `com.castsoftware.uc.python.common-1.0.3/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-1.0.4/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.3/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-1.0.4/cast_common/aipRestCall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from cast_common.restAPI import RestCall
 from requests import codes
 
 from pandas import DataFrame
 from pandas import merge
 from pandas import json_normalize
 
-__author__ = "Nevin Kaplan"
-__email__ = "n.kaplan@castsoftware.com"
-__copyright__ = "Copyright 2022, CAST Software"
-
 class AipRestCall(RestCall):
     _measures = {
         '60017':'TQI',
         '60013':'Robustness',
         '60014':'Efficiency',
         '60016':'Security',
-        '60012':'Changeability',
         '60011':'Transferability',
+        '60012':'Changeability',
 #        '60015':'SEI Maintainability',
         '66033':'Documentation',
         '1061000':"ISO",
         '1061003':"ISO_REL",
         '1061001':"ISO_MAINT",
         '1061002':"ISO_EFF",
         '1061004':"ISO_SEC"
@@ -30,20 +26,20 @@
         '67011':'Violation Count',
         '67012':' per file',
         '67013':' per kLoC'
     }
 
     def get_domain(self, schema_name):
         self.debug(f'retrieving domain for {schema_name}')
-        schema_name = schema_name.replace('-','_').replace('.','_').lower() + '_central'
+        schema_name = schema_name.replace('-','_')
         domain_id = None
         (status,json) = self.get()
         if status == codes.ok:
             try: 
-                domain_id = list(filter(lambda x:x["schema"].lower()==schema_name,json))[0]['name']
+                domain_id = list(filter(lambda x:x["schema"].lower()==schema_name.lower(),json))[0]['name']
             except IndexError:
                 self.error(f'Domain not found for schema {schema_name}')
         if status == 0:
             domain_id = -1        
         return domain_id
 
     def get_quality_indicators(self,domain_id,snapshot_id, key):
```

### Comparing `com.castsoftware.uc.python.common-1.0.3/cast_common/highlight.py` & `com.castsoftware.uc.python.common-1.0.4/cast_common/highlight.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from requests import codes
 from pandas import ExcelWriter,DataFrame
 
 
 class Highlight(RestCall):
 
-    _data = []
+    _data = {}
     _apps = []
     _tags = []
     _cloud = []
     _oss = []
     _elegance = []
     _instance_id = None
 
@@ -35,19 +35,36 @@
         self.info(f'Found {len(self._apps)} applications')
         self._apps.dropna(subset=['metrics'],inplace=True)
         self.info(f'Found {len(self._apps)} analyzed applications')
         if len(hl_apps) > 0:
             self._apps = self._apps[self._apps['name'].isin(hl_apps)]
         self.info(f'{len(self._apps)} applications selected')
 
-        for app in hl_apps:
+        app_data = {}
+        for app in self._apps.loc():
             try:
-                self._data[app]=self._get_application_data(app)
+                app_name = app['name']
+                app_data[app_name]={}
+                self.info(f'Loading Highlight data for {app_name}')
+                data = self._get_application_data(app_name)
+
+
+                # domains = data['domains']
+                # metrics = data['metrics'][0]
+                # green_detail = metrics['greenDetail'][0]
+                # cloud_detail = metrics['cloudReadyDetail'][0]
+                # technology_detail = metrics['technologies'][0]
+                # vulnerability_detail = metrics['vulnerabilities'][0]
+                # components_detail = metrics['components'][0]
+
+                # app_data[app]={'domains':domains}
+
+                pass
             except KeyError as ke:
-                
+                pass
                 
         pass
 
 
         # file_name = r'e:/work/wellsfargo/tags.xlsx'
         # writer = ExcelWriter(file_name, engine='xlsxwriter')
         # summary_tab = format_table(writer,DataFrame(self._tags),'Tags')
```

### Comparing `com.castsoftware.uc.python.common-1.0.3/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-1.0.4/cast_common/hlRestCall.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from cast_common.restAPI import RestCall
-from cast_common.logger import INFO
 from requests import codes, post
-from pandas import DataFrame,json_normalize,concat
+from pandas import DataFrame
+from pandas import json_normalize
+from pandas import concat
+from logging import DEBUG, INFO, ERROR, warning
 
-__author__ = "Nevin Kaplan"
-__email__ = "n.kaplan@castsoftware.com"
-__copyright__ = "Copyright 2022, CAST Software"
 
 class HLRestCall(RestCall):
     """
     Class to handle HL REST API calls.
     """
     def __init__(self, hl_base_url, hl_user, hl_pswd, hl_instance, timer_on=False,log_level=INFO):
-        super().__init__(hl_base_url, hl_user, hl_pswd, timer_on,log_level,accept_json=False)
+        super().__init__(hl_base_url, hl_user, hl_pswd, timer_on,log_level)
 
         self._hl_instance = hl_instance
         self._hl_data_retrieved = False
     
     def _get_app_ids(self, instance_id):
         # Retrieve the HL app id for the application.
```

### Comparing `com.castsoftware.uc.python.common-1.0.3/cast_common/logger.py` & `com.castsoftware.uc.python.common-1.0.4/cast_common/logger.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.3/cast_common/util.py` & `com.castsoftware.uc.python.common-1.0.4/cast_common/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from pandas import DataFrame,json_normalize,concat,ExcelWriter
 from os import mkdir
 from os.path import exists,abspath,join
 from subprocess import Popen,PIPE,STDOUT
-from cast_common.logger import Logger
-from pandas.api.types import is_numeric_dtype
 import sys
 
-__author__ = "Nevin Kaplan"
-__email__ = "n.kaplan@castsoftware.com"
-__copyright__ = "Copyright 2022, CAST Software"
 
 def get_between(txt,tag_start,tag_end,start_at=0):
     text = txt[start_at:]
     
     start = text[start_at:].find(f"{tag_start}")+len(f"{tag_start}")
     end = text[start:].find(f"{tag_end}")
     between = text[start:start+end].strip()
@@ -72,14 +67,48 @@
 
         ppt.replace_text(f'{{app{app_no}_risk_detail}}','')
         ppt.replace_text(f'{{end_app{app_no}_risk_detail}}','')
 
     ppt.remove_empty_placeholders()
     return risk_grades
 
+def format_table(writer, data, sheet_name,width=None):
+    
+    data.to_excel(writer, index=False, sheet_name=sheet_name, startrow=1,header=False)
+
+    workbook = writer.book
+    worksheet = writer.sheets[sheet_name]
+    rows = len(data)
+    cols = len(data.columns)-1
+    columns=[]
+    for col_num, value in enumerate(data.columns.values):
+        columns.append({'header': value})
+
+    table_options={
+                'columns':columns,
+                'header_row':True,
+                'autofilter':True,
+                'banded_rows':True
+                }
+    worksheet.add_table(0, 0, rows, cols,table_options)
+    
+    header_format = workbook.add_format({'text_wrap':True,
+                                        'align': 'center'})
+
+    col_width = 10
+    if width == None:
+        width = []
+        for i in range(1,len(data.columns)+1):
+           width.append(col_width)
+    for col_num, value in enumerate(data.columns.values):
+        worksheet.write(0, col_num, value, header_format)
+        w=width[col_num]
+        worksheet.set_column(col_num, col_num, w)
+    return worksheet
+
 def find_nth(string, substring, n):
    if (n == 1):
        return string.find(substring)
    else:
        return string.find(substring, find_nth(string, substring, n - 1) + 1)
 
 def no_dups(string, separator,add_count=False):
@@ -140,57 +169,50 @@
     ret = []
     while process.poll() is None:
         line = process.stdout.readline()
         line = line.lstrip("b'").rstrip('\n')
         if output == True and len(line.strip(' ')) > 0:
             print(line)
         ret.append(line)
-    try:
-        stdout, stderr = process.communicate()
-    except: 
-        return process.returncode,ret
+    stdout, stderr = process.communicate()
     return process.returncode,ret
-     
+    
+
 def format_table(writer, data, sheet_name,width=None):
     
     data.to_excel(writer, index=False, sheet_name=sheet_name, startrow=1,header=False)
 
     workbook = writer.book
     worksheet = writer.sheets[sheet_name]
-    rows = len(data)+1
+    rows = len(data)
     cols = len(data.columns)-1
-
     columns=[]
-    first=True
     for col_num, value in enumerate(data.columns.values):
-        json = {'header': value}
-        if first:
-            first=False
-            json['total_string']='Totals'
-        else: 
-            if is_numeric_dtype(data[value]) and data[value].dtype != 'bool':
-                json['total_function']='sum'
-
-        columns.append(json)
+        columns.append({'header': value})
 
     table_options={
-                'total_row':True,
                 'columns':columns,
                 'header_row':True,
                 'autofilter':True,
                 'banded_rows':True
                 }
     worksheet.add_table(0, 0, rows, cols,table_options)
+    
+    header_format = workbook.add_format({'text_wrap':True,
+                                        'align': 'center'})
 
     col_width = 10
     if width == None:
         width = []
         for i in range(1,len(data.columns)+1):
            width.append(col_width)
-
+    for col_num, value in enumerate(data.columns.values):
+        worksheet.write(0, col_num, value, header_format)
+        w=width[col_num]
+        worksheet.set_column(col_num, col_num, w)
     return worksheet
 
 def convert_LOC(total:int):
     unit = ''
     if 1000 <= total <= 1000000:
         unit = 'KLoc'
         total = int(total/1000)
```

### Comparing `com.castsoftware.uc.python.common-1.0.3/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.3
+Version: 1.0.4
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # com.castsoftware.uc.python.common
 A set of common classes and methods for use with python projects
```

### Comparing `com.castsoftware.uc.python.common-1.0.3/pyproject.toml` & `com.castsoftware.uc.python.common-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='1.0.3' #prod version
+version='1.0.4' #prod version
 
 dependencies = ['pandas','requests']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.10.6"
 readme = "README.md"
 [project.urls]
 "Homepage" = "https://github.com/CAST-Extend/com.castsoftware.uc.python.common"
 "Bug Tracker" = "https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues"
```

