# Comparing `tmp/indiek-core-0.1.3.tar.gz` & `tmp/indiek-core-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-n6x9td7w/indiek-core-0.1.3.tar", last modified: Tue May  9 22:16:55 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-dyo32cgb/indiek-core-0.1.4.tar", last modified: Thu May 18 00:48:14 2023, max compression
```

## Comparing `indiek-core-0.1.3.tar` & `indiek-core-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.678692 indiek-core-0.1.3/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.3/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1165 2023-05-09 22:16:55.678692 indiek-core-0.1.3/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      714 2023-05-09 22:12:17.000000 indiek-core-0.1.3/README.rst
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.674692 indiek-core-0.1.3/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.674692 indiek-core-0.1.3/indiek/core/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-05-07 17:29:44.000000 indiek-core-0.1.3/indiek/core/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3310 2023-05-07 18:01:42.000000 indiek-core-0.1.3/indiek/core/items.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3488 2023-05-08 22:13:30.000000 indiek-core-0.1.3/indiek/core/search.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.678692 indiek-core-0.1.3/indiek_core.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1165 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      319 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       58 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-09 22:16:55.678692 indiek-core-0.1.3/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      924 2023-05-07 14:33:34.000000 indiek-core-0.1.3/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.678692 indiek-core-0.1.3/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1503 2023-05-07 17:43:18.000000 indiek-core-0.1.3/tests/test_items.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3031 2023-05-08 22:21:51.000000 indiek-core-0.1.3/tests/test_search.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.639869 indiek-core-0.1.4/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.4/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1165 2023-05-18 00:48:14.639869 indiek-core-0.1.4/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      714 2023-05-09 22:12:17.000000 indiek-core-0.1.4/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.619868 indiek-core-0.1.4/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.639869 indiek-core-0.1.4/indiek/core/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-05-07 17:29:44.000000 indiek-core-0.1.4/indiek/core/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3588 2023-05-13 11:39:09.000000 indiek-core-0.1.4/indiek/core/items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3488 2023-05-08 22:13:30.000000 indiek-core-0.1.4/indiek/core/search.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.639869 indiek-core-0.1.4/indiek_core.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1165 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      319 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       58 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-18 00:48:14.000000 indiek-core-0.1.4/indiek_core.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-18 00:48:14.639869 indiek-core-0.1.4/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      924 2023-05-18 00:01:49.000000 indiek-core-0.1.4/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-18 00:48:14.639869 indiek-core-0.1.4/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1528 2023-05-10 02:20:52.000000 indiek-core-0.1.4/tests/test_items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3031 2023-05-08 22:21:51.000000 indiek-core-0.1.4/tests/test_search.py
```

### Comparing `indiek-core-0.1.3/LICENSE` & `indiek-core-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-core-0.1.3/PKG-INFO` & `indiek-core-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: core logic for indiek
 Home-page: https://pypi.org/project/indiek-core/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek.core
 Project-URL: Documentation, https://indiekcore.readthedocs.io/en/latest/
```

### Comparing `indiek-core-0.1.3/README.rst` & `indiek-core-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `indiek-core-0.1.3/indiek/core/items.py` & `indiek-core-0.1.4/indiek/core/items.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,16 @@
     Attributes:
         _ikid (int): a unique identifier.
         name (str): a human-friendly short identifier.
         content (str): some string with data the Item is meant to hold or reference.
         backend (Any): backend port for I/O operations with DB
     """
 
-    BACKEND_CLS = default_driver.Item
-    """Class from backend items module corresponding to present core API class."""
-
+    _attr_defs = ['_ikid', 'content', 'name']
+    
     def __init__(self, *, name: str = '', content: Any = '', _ikid: Optional[int] = None, driver: Any = default_driver):
         self._ikid = _ikid
         self.name = name
         self.content = content
         self.backend = driver
 
     def __repr__(self):
@@ -49,39 +48,52 @@
         return (self._ikid == other._ikid
                 and self.name == other.name
                 and self.content == other.content
                 and type(other) == type(self))
 
     def _to_db(self) -> default_driver.Item:
         """Export core Item to DB Item instance."""
-        return self.BACKEND_CLS.from_core(self)
+        as_dict = self.to_dict()
+        try:
+            return self.BACKEND_CLS(**as_dict)
+        except AttributeError:
+            return self.backend.Item(**as_dict)
+        
+    @property
+    def exists_in_db(self):
+        """This is shallow, it doesn't query the DB at all."""
+        return self._ikid is not None
     
     def save(self) -> int:
         """Save to backend.
         
         This method delegates the save operation to the backend.
         If _ikid is None in self, it will get set to new value
         generated by backend.
         """
         self._ikid = self._to_db().save()
         return self._ikid
+    
+    def delete(self) -> None:
+        self._to_db().delete()
+        self._ikid = None
 
     @classmethod
     def load(cls, ikid) -> Item:
         """Create Core Item from backend using ikid."""
         return cls.from_db(cls.BACKEND_CLS.load(ikid))
 
     @classmethod
     def from_db(cls, db_item: default_driver.Item) -> Item:
         """Instantiate core Item off of backend Item."""
         return cls(**db_item.to_dict())
     
     def to_dict(self):
         """Export core Item content to dict."""
-        return {'name': self.name, 'content': self.content, '_ikid': self._ikid}
+        return {a: getattr(self, a) for a in self._attr_defs}
     
 
 class Definition(Item):
     BACKEND_CLS = default_driver.Definition
     pass
```

### Comparing `indiek-core-0.1.3/indiek/core/search.py` & `indiek-core-0.1.4/indiek/core/search.py`

 * *Files identical despite different names*

### Comparing `indiek-core-0.1.3/indiek_core.egg-info/PKG-INFO` & `indiek-core-0.1.4/indiek_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: core logic for indiek
 Home-page: https://pypi.org/project/indiek-core/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek.core
 Project-URL: Documentation, https://indiekcore.readthedocs.io/en/latest/
```

### Comparing `indiek-core-0.1.3/setup.py` & `indiek-core-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.rst'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='indiek-core',
     python_requires='>=3.8',
-    version='0.1.3',
+    version='0.1.4',
     url='https://pypi.org/project/indiek-core/',
     description='core logic for indiek',
     long_description=long_description,
     author='Adrian Ernesto Radillo',
     author_email='adrian.radillo@gmail.com',
     license='GNU Affero General Public License v3.0',
     packages=['indiek.core'],
-    install_requires=['indiek-mockdb==0.1.3'],
+    install_requires=['indiek-mockdb>=0.1.4'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov'
         ]
     },
```

### Comparing `indiek-core-0.1.3/tests/test_items.py` & `indiek-core-0.1.4/tests/test_items.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from indiek.core.items import Item, Definition, Theorem, Proof
-from indiek.mockdb.items import Item as DBitem
+from indiek.mockdb.items import Definition as DBDefinition
 from indiek import mockdb
 
 CORE_ITEM_TYPES = [Definition, Theorem, Proof]
 
 class TestItemAttr(unittest.TestCase):
     def test_instantiation(self):
         item = Item()
@@ -19,17 +19,17 @@
             self.assertTrue(hasattr(item, attr_name))
 
 
 class TestItemIO(unittest.TestCase):
     db_driver = mockdb.items
 
     def test_to_db(self):
-        pure_item = Item(driver=self.db_driver)
+        pure_item = Definition(driver=self.db_driver)
         db_item = pure_item._to_db()
-        self.assertIsInstance(db_item, DBitem)
+        self.assertIsInstance(db_item, DBDefinition)
 
         for core_cls in CORE_ITEM_TYPES:
             pure_item = core_cls(driver=self.db_driver)
             db_item = pure_item._to_db()
             self.assertIsInstance(db_item, pure_item.BACKEND_CLS)
 
     def test_item_io(self):
@@ -41,12 +41,12 @@
             self.assertEqual(core_item, new_item)
             
 
 class TestComparison(unittest.TestCase):
     def test_core_vs_db(self):
         core = Item()
         db = core._to_db()
-        self.assertFalse(core == db)
+        self.assertNotEqual(core, db)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `indiek-core-0.1.3/tests/test_search.py` & `indiek-core-0.1.4/tests/test_search.py`

 * *Files identical despite different names*

