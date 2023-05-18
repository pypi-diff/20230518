# Comparing `tmp/sayuDB-1.0.0.tar.gz` & `tmp/sayuDB-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayuDB-1.0.0.tar", last modified: Mon May 15 18:53:30 2023, max compression
+gzip compressed data, was "sayuDB-1.1.4.tar", last modified: Thu May 18 13:49:58 2023, max compression
```

## Comparing `sayuDB-1.0.0.tar` & `sayuDB-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 18:53:30.112789 sayuDB-1.0.0/
--rw-rw-rw-   0        0        0     1085 2023-04-23 05:32:47.000000 sayuDB-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     9981 2023-05-15 18:53:30.112789 sayuDB-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10068 2023-05-15 18:43:51.000000 sayuDB-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 18:53:30.079787 sayuDB-1.0.0/sayuDB/
--rw-rw-rw-   0        0        0      635 2023-04-23 05:32:47.000000 sayuDB-1.0.0/sayuDB/__init__.py
--rw-rw-rw-   0        0        0     4847 2023-05-15 18:50:36.000000 sayuDB-1.0.0/sayuDB/__main__.py
--rw-rw-rw-   0        0        0    21637 2023-05-15 18:46:50.000000 sayuDB-1.0.0/sayuDB/processor.py
--rw-rw-rw-   0        0        0     2042 2023-04-23 05:32:47.000000 sayuDB-1.0.0/sayuDB/remote.py
--rw-rw-rw-   0        0        0     3252 2023-04-23 05:32:47.000000 sayuDB-1.0.0/sayuDB/server.py
-drwxrwxrwx   0        0        0        0 2023-05-15 18:53:30.111172 sayuDB-1.0.0/sayuDB.egg-info/
--rw-rw-rw-   0        0        0     9981 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 18:53:29.000000 sayuDB-1.0.0/sayuDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 18:53:30.113792 sayuDB-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0    10344 2023-05-15 18:49:44.000000 sayuDB-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 13:49:58.520741 sayuDB-1.1.4/
+-rw-rw-rw-   0        0        0     1085 2023-04-23 05:32:47.000000 sayuDB-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     9981 2023-05-18 13:49:58.519748 sayuDB-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10068 2023-05-15 18:43:51.000000 sayuDB-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 13:49:58.498263 sayuDB-1.1.4/sayuDB/
+-rw-rw-rw-   0        0        0     2525 2023-05-18 13:08:16.000000 sayuDB-1.1.4/sayuDB/SQLite.py
+-rw-rw-rw-   0        0        0     1551 2023-05-18 13:13:51.000000 sayuDB-1.1.4/sayuDB/__init__.py
+-rw-rw-rw-   0        0        0     4911 2023-05-18 13:20:28.000000 sayuDB-1.1.4/sayuDB/__main__.py
+-rw-rw-rw-   0        0        0    21637 2023-05-18 13:04:44.000000 sayuDB-1.1.4/sayuDB/processor.py
+-rw-rw-rw-   0        0        0     2042 2023-04-23 05:32:47.000000 sayuDB-1.1.4/sayuDB/remote.py
+-rw-rw-rw-   0        0        0     3252 2023-05-18 13:48:02.000000 sayuDB-1.1.4/sayuDB/server.py
+drwxrwxrwx   0        0        0        0 2023-05-18 13:49:58.518565 sayuDB-1.1.4/sayuDB.egg-info/
+-rw-rw-rw-   0        0        0     9981 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 13:49:58.520741 sayuDB-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0    10344 2023-05-18 13:48:28.000000 sayuDB-1.1.4/setup.py
```

### Comparing `sayuDB-1.0.0/LICENSE` & `sayuDB-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sayuDB-1.0.0/PKG-INFO` & `sayuDB-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayuDB
-Version: 1.0.0
+Version: 1.1.4
 Summary: Database management system based on python and JSON.
 Home-page: https://github.com/Arsybai/sayuDB
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: database
 Description-Content-Type: text/markdown
```

### Comparing `sayuDB-1.0.0/README.md` & `sayuDB-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sayuDB-1.0.0/sayuDB/__main__.py` & `sayuDB-1.1.4/sayuDB/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 def save_conf():
     with open(f'{os.path.dirname(__file__)}/users.json', 'w')as wconf:
         json.dump(user, wconf, indent=4)
     with open(f'{os.path.dirname(__file__)}/config.json', 'w')as wconf:
         json.dump(config, wconf, indent=4)
     return
 
+def main():
+    pass
+
 try:
     sys.argv[1]
 except:
     print("Read the doc here : https://github.com/Arsybai/blob/main/README.md")
     print("""Invalid commad. get help by
 --h""")
     exit()
@@ -64,15 +67,16 @@
         sayuDB.create_database(sys.argv[3])
 
 elif sys.argv[1] == 'show':
     if sys.argv[2] == 'users':
         for i in user:
             print(f"> {i}")
     elif sys.argv[2] == 'databases':
-        sayuDB.show_databases()
+        for i in sayuDB.show_databases():
+            print(f'> {i}')
 
 elif sys.argv[1] == 'remove':
     if sys.argv[2] == 'user':
         if sys.argv[3] in user:
             del user[sys.argv[3]]
             print("User deleted")
             save_conf()
```

### Comparing `sayuDB-1.0.0/sayuDB/processor.py` & `sayuDB-1.1.4/sayuDB/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         print("Database already exist")
         
 def show_databases():
     databases = os.listdir(f'{os.path.dirname(__file__)}/datas/')
     lists = []
     for i in databases:
         if '.ezdb' in i:
-            print(f"> {i.replace('.ezdb','')}")
+            # print(f"> {i.replace('.ezdb','')}")
             lists.append(i.replace('.ezdb',''))
     return lists
         
 def drop_database(name: str):
     if os.path.isfile(f'{os.path.dirname(__file__)}/datas/{name}.ezdb'):
         os.remove(f'{os.path.dirname(__file__)}/datas/{name}.ezdb')
         print(f"Database dropped [ {name} ]")
@@ -177,15 +177,14 @@
         Contents Function:
             today()\t\t: Generate today datetime (only work in str typedata)
             index()\t\t: Indexing the number of row. it can be use as id too (only work in int typedata)
             genID()\t\t: Generate random 5 digits ID
             increase()\t: Increase from the last row value (Only work in int typedata)
         """
 
-
         db_ = self.openDB()
         def index():
             return len(db_[table]["datas"]) + 1
         if type(col) == str:
             col = col.split(',')
         column_ = db_[table]["column"]
         for i in col:
```

### Comparing `sayuDB-1.0.0/sayuDB/remote.py` & `sayuDB-1.1.4/sayuDB/remote.py`

 * *Files identical despite different names*

### Comparing `sayuDB-1.0.0/sayuDB/server.py` & `sayuDB-1.1.4/sayuDB/server.py`

 * *Files identical despite different names*

### Comparing `sayuDB-1.0.0/sayuDB.egg-info/PKG-INFO` & `sayuDB-1.1.4/sayuDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayuDB
-Version: 1.0.0
+Version: 1.1.4
 Summary: Database management system based on python and JSON.
 Home-page: https://github.com/Arsybai/sayuDB
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: database
 Description-Content-Type: text/markdown
```

### Comparing `sayuDB-1.0.0/setup.py` & `sayuDB-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="sayuDB",
-    version="1.0.0",
+    version="1.1.4",
     author="Arsybai",
     description="Database management system based on python and JSON.",
     packages=["sayuDB"],
     license="MIT",
     author_email="me@arsybai.com",
     url="https://github.com/Arsybai/sayuDB",
     keywords=[
```

