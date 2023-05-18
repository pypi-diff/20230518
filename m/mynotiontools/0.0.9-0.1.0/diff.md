# Comparing `tmp/mynotiontools-0.0.9.tar.gz` & `tmp/mynotiontools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mynotiontools-0.0.9.tar", last modified: Thu Dec  1 08:41:34 2022, max compression
+gzip compressed data, was "dist/mynotiontools-0.1.0.tar", last modified: Thu May 18 03:17:32 2023, max compression
```

## Comparing `mynotiontools-0.0.9.tar` & `mynotiontools-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       38 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/setup.cfg
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     3767 2022-12-01 08:41:27.000000 mynotiontools-0.0.9/setup.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      608 2022-11-28 10:27:36.000000 mynotiontools-0.0.9/README.md
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1049 2022-11-27 17:38:00.000000 mynotiontools-0.0.9/LICENSE
-drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)        1 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/dependency_links.txt
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       14 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/top_level.txt
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)        9 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/requires.txt
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      321 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/SOURCES.txt
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1264 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/PKG-INFO
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       26 2022-11-27 17:34:02.000000 mynotiontools-0.0.9/MANIFEST.in
-drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools/
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)    11452 2022-12-01 08:41:08.000000 mynotiontools-0.0.9/mynotiontools/__init__.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      352 2022-11-28 03:39:39.000000 mynotiontools-0.0.9/mynotiontools/__version__.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       40 2022-11-28 06:39:58.000000 mynotiontools-0.0.9/mynotiontools/main.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       26 2022-11-27 17:34:02.000000 mynotiontools-0.0.9/mynotiontools/core.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1264 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/PKG-INFO
+drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       38 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/setup.cfg
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     3767 2023-05-18 03:16:54.000000 mynotiontools-0.1.0/setup.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      608 2022-11-28 10:27:36.000000 mynotiontools-0.1.0/README.md
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1049 2022-11-27 17:38:00.000000 mynotiontools-0.1.0/LICENSE
+drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/mynotiontools.egg-info/
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)        1 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/mynotiontools.egg-info/dependency_links.txt
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       14 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/mynotiontools.egg-info/top_level.txt
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)        9 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/mynotiontools.egg-info/requires.txt
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      321 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/mynotiontools.egg-info/SOURCES.txt
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1264 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/mynotiontools.egg-info/PKG-INFO
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       26 2022-11-27 17:34:02.000000 mynotiontools-0.1.0/MANIFEST.in
+drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/mynotiontools/
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)    14112 2023-05-18 03:16:30.000000 mynotiontools-0.1.0/mynotiontools/__init__.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      352 2022-11-28 03:39:39.000000 mynotiontools-0.1.0/mynotiontools/__version__.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       40 2022-11-28 06:39:58.000000 mynotiontools-0.1.0/mynotiontools/main.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       26 2022-11-27 17:34:02.000000 mynotiontools-0.1.0/mynotiontools/core.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1264 2023-05-18 03:17:32.000000 mynotiontools-0.1.0/PKG-INFO
```

### Comparing `mynotiontools-0.0.9/setup.py` & `mynotiontools-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'mynotiontools'
 DESCRIPTION = 'Some tools for notion, Just for fun.'
 URL = 'https://github.com/suyelu/mynotion'
 EMAIL = 'suyelu@hotmail.com'
 AUTHOR = 'Vincent Su'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests'
 ]
 
 # What packages are optional?
```

### Comparing `mynotiontools-0.0.9/README.md` & `mynotiontools-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mynotiontools-0.0.9/LICENSE` & `mynotiontools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mynotiontools-0.0.9/mynotiontools.egg-info/PKG-INFO` & `mynotiontools-0.1.0/mynotiontools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mynotiontools
-Version: 0.0.9
+Version: 0.1.0
 Summary: Some tools for notion, Just for fun.
 Home-page: https://github.com/suyelu/mynotion
 Author: Vincent Su
 Author-email: suyelu@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mynotiontools-0.0.9/mynotiontools/__init__.py` & `mynotiontools-0.1.0/mynotiontools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,91 @@
 #!/usr/bin/env python
 # coding=utf-8
 import secrets
 import requests
 import copy
 import json
 import os
+import datetime
+import time
+import sys
+
+
 
 
 class NotionHelper:
     def __init__(self, secrets = None):
         if secrets == None:
             self.secrets = os.environ.get('NOTION_SECRETS')
         else:
             self.secrets = secrets
         if self.secrets == None:
             print('NOTION_SECRETS not set')
-            return
+            sys.exit(1)
         self.headers = {
             "accept": "application/json",
             "Notion-Version": "2022-06-28",
             "content-type": "application/json",
             "Authorization" : self.secrets
         }
         self.payload = {
             "page_size" : 10000
         }
         self.base_url = "https://api.notion.com/v1/databases/"
         self.keys = []
         self.rela = {}
 
     def get_keys(self, database_id):
+        '''
+            获取数据库的所有属性名
+            database_id - notion database的id
+        '''
         page_size_old = self.payload['page_size']
         self.payload['page_size'] = 1
         response = requests.request("POST", self.base_url + database_id + "/query", json = self.payload, headers = self.headers)
         res = json.loads(response.text)
         print(response, res, self.headers)
         self.keys = list(res['results'][0]['properties'].keys())
         self.payload['page_size'] = page_size_old
         return self.keys
+        
+
+    def find_title_name(self, name, res_t):
+        '''
+            找到关联属性的title
+            name - 关联属性的名字
+            res_t - 关联属性的json
+        '''
+        for key in res_t['properties']:
+            if res_t['properties'][key]['type'] == 'title':
+                self.rela[name]['title'] = key
+                break
+            
 
     def get_rela_name(self, name, rela_id):
-            if rela_id == 0:
-                return "None"
-            if name not in self.rela:
-                self.rela[name] = {}
-            if rela_id in self.rela[name]:
-                #print("命中")
-                return self.rela[name][rela_id]
-            url = "https://api.notion.com/v1/pages/{}".format(rela_id)
-            res = requests.request("GET", url, headers=self.headers)
-            res_t = json.loads(res.text)
-            if 'title' not in self.rela[name]:
-                self.find_title_name(name, res_t)
-                #print("未命中表头")
-            self.rela[name][rela_id] = res_t['properties'][self.rela[name]['title']]['title'][0]['text']['content']
+        '''
+            获取关联属性的名字
+            name - 关联属性的名字
+            rela_id - 关联属性的id
+        '''
+        if rela_id == 0:
+            return "None"
+        if name not in self.rela:
+            self.rela[name] = {}
+        if rela_id in self.rela[name]:
+            #print("命中")
             return self.rela[name][rela_id]
+        url = "https://api.notion.com/v1/pages/{}".format(rela_id)
+        res = requests.request("GET", url, headers=self.headers)
+        res_t = json.loads(res.text)
+        if 'title' not in self.rela[name]:
+            self.find_title_name(name, res_t)
+            #print("未命中表头")
+        self.rela[name][rela_id] = res_t['properties'][self.rela[name]['title']]['title'][0]['text']['content']
+        return self.rela[name][rela_id]
 
     def get_property_value(self, properties, property_name):
         """获取Notion database中一行数据的某个property的值
             properties     - notion page返回的的properties字典
             property_name  - 需要查找的property名字，字符串
         """
         try:
@@ -123,35 +150,46 @@
             try :
                 for each in property[property_type]:
                     rela_id = each[id]
                     rela_name = self.get_rela_name(property_name, rela_id)
                     ans.append({'id' : rela_id, 'name' : rela_name})
             except:
                 ans = None
+        elif property_type == 'status':
+            ans = property[property_type]['name']
         else:
             ans = None
         return ans
 
     def insert_notion_page_into_database(self, parent_id):
+        """
+            在notion database中插入一个新的page
+            parent_id - notion database的id
+        """
         url = "https://api.notion.com/v1/pages"
         parent = {"type":"database_id", "database_id" : parent_id}
         payload = {
             "parent": parent,
             "properties": {"Name" : {'title':[{ 'text' : {'content' : "New"}, 'plain_text' : "New"}]}}
         }
         response = requests.post(url, json=payload, headers=self.headers)
         try:
             ret = json.loads(response.text)
         except:
             return None
-        return ret['id']
-
+        #print(ret)
+        return ret
 
+    #定义一个函数get_timestamp，用于将一个datetime转换为时间戳
+    def get_timestamp(self, dt):
+        return int(time.mktime(dt.timetuple()))
+    
+    
 
-    def update_notion_databse_item(self, id, db_properties, update_properties):
+    def update_notion_database_item(self, id, db_properties, update_properties):
         """修改notion database中一个page的属性值
             id      - notion page的id
             db_properties -
             update_properties - 需要更新的property和值的字典列表
                         {
                             "property_name" : "name",
                             "property_value" : value
@@ -177,27 +215,45 @@
                     value[value_type].pop('id')
                 except:
                     pass
                 try:
                     value[value_type].pop('color')
                 except:
                     pass
+            elif value_type == 'title' or value_type == 'rich_text':
+                value[value_type] = [{"text" : {"content" : each['property_value']}}]
+            elif value_type == 'multi_select':
+                if  each['property_value'] == None:
+                    value[value_type] = []
+                else:
+                    for every in each['property_value']:
+                        value[value_type].append({'name' : every})
+            elif value_type == 'date':
+                value[value_type] = {'start' : each['property_value']}
+            elif value_type == 'url':
+                try:
+                    if len(each['property_value']) == 0:
+                        value[value_type] = None
+                except:
+                    pass
+                else:
+                    value[value_type] = each['property_value']
             else:
                 value[value_type] = []
                 #value[value_type].append(each['property_value'])
                 value[value_type] = each['property_value']
             payload['properties'][name] = value
         payload['archived'] = False
         #print(payload)
         response = requests.patch(url, json=payload, headers=headers)
         return response
 
 
 
-    def update_notion_databse_item_easy(self, id, db_properties, update_properties):
+    def update_notion_database_item_easy(self, id, db_properties, update_properties):
         """修改notion database中一个page的属性值
             id      - notion page的id
             db_properties -
             update_properties - 需要更新的property和值的字典列表
                         {
                             "property_name" : "name",
                             "property_value" : value
@@ -229,28 +285,35 @@
                     pass
             elif value_type == 'title' or value_type == 'rich_text':
                 value[value_type] = [{"text" : {"content" : each['property_value']}}]
             elif value_type == 'multi_select':
                 if  each['property_value'] == None:
                     value[value_type] = []
                 else:
-                    value[value_type] = [{'name' : each['property_value']}]
+                    for every in each['property_value']:
+                        value[value_type].append({'name' : every})
             elif value_type == 'date':
                 value[value_type] = {'start' : each['property_value']}
             else:
                 value[value_type] = []
                 #value[value_type].append(each['property_value'])
                 value[value_type] = each['property_value']
             payload['properties'][name] = value
         payload['archived'] = False
         #print(payload)
         response = requests.patch(url, json=payload, headers=headers)
         return response
 
     def add_to_relation(self, id, db_properties, name, add_id):
+        """修改notion database中一个page的属性值
+            id      - notion page的id
+            db_properties - 数据库的属性
+            name - relation的名字
+            add_id - 需要添加的id
+        """
         url = "https://api.notion.com/v1/pages/{}".format(id)
         headers = self.headers
         payload = {}
         payload['properties'] = {}
         in_property = copy.deepcopy(db_properties)
 
         value = in_property[name]
@@ -259,14 +322,18 @@
         payload['archived'] = False
         #print(payload)
         response = requests.patch(url, json=payload, headers=headers)
         return response
 
 
     def get_id_of_page(self, parent, filter):
+        """根据filter获取page的id
+            parent - 数据库的id
+            filter - 过滤条件
+        """
         url = "https://api.notion.com/v1/databases/{}".format(parent)
         headers = self.headers
         payload = {
             "page_size" : 1,
             "filter" : filter,
             "sorts" : []
 
@@ -279,21 +346,30 @@
         try:
             id = res['results'][0]['id']
         except:
             id = None
         return id
 
     def add_to_multi_select(self, id, db_properties, name, add_value):
+        """修改notion database中一个page的属性值
+            id      - notion page的id
+            db_properties - 数据库的属性
+            name - multi_select的名字
+            add_value - 需要添加的值
+        """
         url = "https://api.notion.com/v1/pages/{}".format(id)
         headers = self.headers
         payload = {}
         payload['properties'] = {}
         in_property = copy.deepcopy(db_properties)
 
         value = in_property[name]
         value['multi_select'].append({'name' : add_value})
         payload['properties'][name] = value
         payload['archived'] = False
         #print(payload)
         response = requests.patch(url, json=payload, headers=headers)
         #print(response, response.text)
         return response
+    def utc_to_local(self, utc_dt):
+        """UTC时间转本地时间（+8:00）"""
+        return utc_dt + datetime.timedelta(hours=8)
```

### Comparing `mynotiontools-0.0.9/PKG-INFO` & `mynotiontools-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mynotiontools
-Version: 0.0.9
+Version: 0.1.0
 Summary: Some tools for notion, Just for fun.
 Home-page: https://github.com/suyelu/mynotion
 Author: Vincent Su
 Author-email: suyelu@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

