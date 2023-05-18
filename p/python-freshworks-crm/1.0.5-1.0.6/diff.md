# Comparing `tmp/python-freshworks-crm-1.0.5.tar.gz` & `tmp/python-freshworks-crm-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-freshworks-crm-1.0.5.tar", last modified: Thu May 18 16:22:37 2023, max compression
+gzip compressed data, was "dist\python-freshworks-crm-1.0.6.tar", last modified: Thu May 18 19:28:51 2023, max compression
```

## Comparing `python-freshworks-crm-1.0.5.tar` & `python-freshworks-crm-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/freshsales/
--rw-rw-rw-   0        0        0    36055 2023-05-18 15:47:25.000000 python-freshworks-crm-1.0.5/freshsales/api.py
--rw-rw-rw-   0        0        0      672 2023-05-06 14:43:54.000000 python-freshworks-crm-1.0.5/freshsales/errors.py
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:26.000000 python-freshworks-crm-1.0.5/freshsales/exceptions.py
--rw-rw-rw-   0        0        0     6751 2023-05-16 19:48:06.000000 python-freshworks-crm-1.0.5/freshsales/models.py
-drwxrwxrwx   0        0        0        0 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/freshsales/tests/
--rw-rw-rw-   0        0        0     7911 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/conftest.py
--rw-rw-rw-   0        0        0     3546 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_accounts.py
--rw-rw-rw-   0        0        0     2700 2023-05-18 15:40:21.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_appointments.py
--rw-rw-rw-   0        0        0     3564 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_contacts.py
--rw-rw-rw-   0        0        0     3365 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_deals.py
--rw-rw-rw-   0        0        0     3341 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_documents.py
--rw-rw-rw-   0        0        0     2419 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_lists.py
--rw-rw-rw-   0        0        0     1724 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_notes.py
--rw-rw-rw-   0        0        0     4029 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_products.py
--rw-rw-rw-   0        0        0     2788 2023-05-18 15:47:50.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_sales_activities.py
--rw-rw-rw-   0        0        0     6558 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_selectors.py
--rw-rw-rw-   0        0        0     3230 2023-05-18 15:42:59.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_tasks.py
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:43.000000 python-freshworks-crm-1.0.5/freshsales/tests/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-18 10:54:29.000000 python-freshworks-crm-1.0.5/freshsales/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-16 20:08:52.000000 python-freshworks-crm-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      878 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      878 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/requires.txt
--rw-rw-rw-   0        0        0      792 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    25929 2023-05-18 16:19:29.000000 python-freshworks-crm-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1156 2023-05-18 03:21:39.000000 python-freshworks-crm-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:28:51.000000 python-freshworks-crm-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-18 19:28:51.000000 python-freshworks-crm-1.0.6/freshsales/
+-rw-rw-rw-   0        0        0    37001 2023-05-18 19:20:56.000000 python-freshworks-crm-1.0.6/freshsales/api.py
+-rw-rw-rw-   0        0        0      672 2023-05-06 14:43:54.000000 python-freshworks-crm-1.0.6/freshsales/errors.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:26.000000 python-freshworks-crm-1.0.6/freshsales/exceptions.py
+-rw-rw-rw-   0        0        0     6751 2023-05-16 19:48:06.000000 python-freshworks-crm-1.0.6/freshsales/models.py
+drwxrwxrwx   0        0        0        0 2023-05-18 19:28:51.000000 python-freshworks-crm-1.0.6/freshsales/tests/
+-rw-rw-rw-   0        0        0     7911 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.6/freshsales/tests/conftest.py
+-rw-rw-rw-   0        0        0     3546 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_accounts.py
+-rw-rw-rw-   0        0        0     2700 2023-05-18 15:40:21.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_appointments.py
+-rw-rw-rw-   0        0        0     3832 2023-05-18 19:18:37.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_contacts.py
+-rw-rw-rw-   0        0        0     3365 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_deals.py
+-rw-rw-rw-   0        0        0     3341 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_documents.py
+-rw-rw-rw-   0        0        0     2419 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_lists.py
+-rw-rw-rw-   0        0        0     1724 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_notes.py
+-rw-rw-rw-   0        0        0     4029 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_products.py
+-rw-rw-rw-   0        0        0     2788 2023-05-18 15:47:50.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_sales_activities.py
+-rw-rw-rw-   0        0        0     6558 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_selectors.py
+-rw-rw-rw-   0        0        0     3230 2023-05-18 15:42:59.000000 python-freshworks-crm-1.0.6/freshsales/tests/test_tasks.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:43.000000 python-freshworks-crm-1.0.6/freshsales/tests/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-18 19:26:21.000000 python-freshworks-crm-1.0.6/freshsales/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 20:08:52.000000 python-freshworks-crm-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      878 2023-05-18 19:28:51.000000 python-freshworks-crm-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 19:28:51.000000 python-freshworks-crm-1.0.6/python_freshworks_crm.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-18 19:28:50.000000 python-freshworks-crm-1.0.6/python_freshworks_crm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      878 2023-05-18 19:28:50.000000 python-freshworks-crm-1.0.6/python_freshworks_crm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-05-18 19:28:50.000000 python-freshworks-crm-1.0.6/python_freshworks_crm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      792 2023-05-18 19:28:51.000000 python-freshworks-crm-1.0.6/python_freshworks_crm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 19:28:50.000000 python-freshworks-crm-1.0.6/python_freshworks_crm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25825 2023-05-18 19:22:03.000000 python-freshworks-crm-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 19:28:51.000000 python-freshworks-crm-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2023-05-18 03:21:39.000000 python-freshworks-crm-1.0.6/setup.py
```

### Comparing `python-freshworks-crm-1.0.5/freshsales/api.py` & `python-freshworks-crm-1.0.6/freshsales/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 class ContactAPI(object):
     def __init__(self, api):
         self._api = api
 
     def create_contact(self, **kwargs):
         url = f'/contacts'
         data = kwargs.copy()
-        response = self._api._post(url, data=json.dumps(data))
-        return Contact(**response.get('contact', {}))
+        response = self._api._post(url, data=json.dumps(data)).get('contact', {})
+        if response.get('sales_accounts'):
+            response['sales_accounts'] = [Account(**account)
+                                    for account in response['sales_accounts']]
+        return Contact(**response)
 
     def view_contact(self, contact_id, *include):
         url = f'/contacts/{contact_id}'
         url += f'?include={",".join(include)}' if include else ''
         contact = self._api._get(url)
         response = contact.get("contact", {})
+        if response.get('sales_accounts'):
+            response['sales_accounts'] = [Account(**account)
+                                    for account in response['sales_accounts']]
         return Contact(**response)
 
     def list_views(self):
         url = '/contacts/filters'
         response = self._api._get(url)
         return [View(**view) for view in response.get('filters', [])]
 
@@ -58,33 +64,42 @@
                 url + f"?page={page}&per_page={per_page}").get('contacts', [])
             contacts = [Contact(**contact) for contact in page_contacts]
 
         return contacts
 
     def update_contact(self, contact_id, **data):
         url = f'/contacts/{contact_id}'
-        response = self._api._put(url, data=json.dumps(data))
-        return Contact(**response.get('contact', {}))
+        response = self._api._put(url, data=json.dumps(data)).get('contact', {})
+        if response.get('sales_accounts'):
+            response['sales_accounts'] = [Account(**account)
+                                    for account in response['sales_accounts']]        
+        return Contact(**response)
 
     def upsert_contact(self, unique_identifier, **contact_properties):
         url = '/contacts/upsert'
         unique_field_name, unique_field_value = unique_identifier
         unique_identifier = {unique_field_name: unique_field_value}
         data = {
             'unique_identifier': unique_identifier,
             'contact': contact_properties
         }
-        response = self._api._post(url, data=json.dumps(data))
-        return Contact(**response.get('contact', {}))
+        response = self._api._post(url, data=json.dumps(data)).get('contact', {})
+        if response.get('sales_accounts'):
+            response['sales_accounts'] = [Account(**account)
+                                    for account in response['sales_accounts']]           
+        return Contact(**response)
 
     def clone_contact(self, contact_id, **data):
         url = f'/contacts/{contact_id}/clone'
         payload = {'contact': data} if data else {}
         contact = self._api._post(
             url, data=json.dumps(payload)).get('contact', {})
+        if contact.get('sales_accounts'):
+            contact['sales_accounts'] = [Account(**account)
+                                    for account in contact['sales_accounts']]
         return Contact(**contact)
 
     def delete_contact(self, contact_id):
         url = f'/contacts/{contact_id}'
         return self._api._delete(url)
 
     def forget_contact(self, contact_id):
```

### Comparing `python-freshworks-crm-1.0.5/freshsales/errors.py` & `python-freshworks-crm-1.0.6/freshsales/errors.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/models.py` & `python-freshworks-crm-1.0.6/freshsales/models.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/conftest.py` & `python-freshworks-crm-1.0.6/freshsales/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_accounts.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_appointments.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_appointments.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_contacts.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_contacts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import datetime
 
 import pytest
 
-from freshsales.models import Contact, Field, View
+from freshsales.models import (
+    Contact,
+    Field,
+    View,
+    Account
+)
 
 
 @pytest.fixture
 def contact(api):
     return api.contacts.view_contact(31016358306)
 
 
@@ -26,14 +31,15 @@
 
 def test_view_contact(contact):
     assert isinstance(contact, Contact)
     assert contact.first_name == "Jane"
     assert contact.last_name == "Sampleton"
     assert contact.emails[0]['value'] == "janesampleton@gmail.com"
     assert contact.id == 31016358306
+    assert isinstance(contact.sales_accounts[0], Account)
 
 
 def test_list_views(api):
     views = api.contacts.list_views()
     assert isinstance(views, list)
     assert len(views) > 0
     assert isinstance(views[0], View)
@@ -55,39 +61,41 @@
 
 
 def test_update_contact(api):
     contact = api.contacts.update_contact(
         31016358306, first_name="New", last_name="Name", display_name="New Name")
     assert isinstance(contact, Contact)
     assert contact.display_name == "New Name"
+    assert isinstance(contact.sales_accounts[0], Account)
 
 
 def test_clone_contact(api):
 
     contact = api.contacts.clone_contact(
         31016358306, first_name="New", last_name="Name", display_name="New Name")
     assert isinstance(contact, Contact)
     assert contact.first_name == "New"
     assert contact.last_name == "Name"
     assert contact.display_name == "New Name"
-
+    assert isinstance(contact.sales_accounts[0], Account)
 
 def test_upsert_contact(api):
     contact_data = {
         "first_name": "Jane",
         "last_name": "Sampleton",
         "display_name": "Jane Sampleton"
     }
     unique_identifier = ('email', 'janesampleton@gmail.com')
     contact = api.contacts.upsert_contact(unique_identifier, **contact_data)
 
     assert isinstance(contact, Contact)
     assert contact.first_name == "Jane"
     assert contact.last_name == "Sampleton"
     assert contact.display_name == "Jane Sampleton"
+    assert isinstance(contact.sales_accounts[0], Account)
 
 
 def test_delete_contact(api):
     assert api.contacts.delete_contact(31016358306) is True
 
 
 def test_forget_contact(api):
```

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_deals.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_deals.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_documents.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_lists.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_notes.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_notes.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_products.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_products.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_sales_activities.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_sales_activities.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_selectors.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/freshsales/tests/test_tasks.py` & `python-freshworks-crm-1.0.6/freshsales/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/LICENSE` & `python-freshworks-crm-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/PKG-INFO` & `python-freshworks-crm-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-freshworks-crm
-Version: 1.0.5
+Version: 1.0.6
 Summary: An API wrapper for the Freshsales CRM
 Home-page: https://github.com/robertvy/python-freshworksCRM
 Author: Robert Van Ysendyck
 Author-email: rvy@vyp-consulting.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/PKG-INFO` & `python-freshworks-crm-1.0.6/python_freshworks_crm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-freshworks-crm
-Version: 1.0.5
+Version: 1.0.6
 Summary: An API wrapper for the Freshsales CRM
 Home-page: https://github.com/robertvy/python-freshworksCRM
 Author: Robert Van Ysendyck
 Author-email: rvy@vyp-consulting.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/SOURCES.txt` & `python-freshworks-crm-1.0.6/python_freshworks_crm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.5/README.md` & `python-freshworks-crm-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Python Wrapper for Freshsales Suite CRM
+# Python API Wrapper for Freshsales Suite CRM
 
 [![PyPI](https://img.shields.io/pypi/v/python-freshworks-crm)](https://pypi.org/project/python-freshworks-crm/)
 ![Stars](https://img.shields.io/github/stars/robertvy/python-freshworksCRM)
 ![Forks](https://img.shields.io/github/forks/robertvy/python-freshworksCRM)
 
 [![Build Status](https://app.travis-ci.com/robertvy/python-freshworksCRM.svg?branch=main)](https://app.travis-ci.com/robertvy/python-freshworksCRM)
 [![codecov](https://codecov.io/github/robertvy/python-freshworksCRM/branch/main/graph/badge.svg?token=M6E8FH72KD)](https://codecov.io/github/robertvy/python-freshworksCRM)
@@ -207,36 +207,30 @@
 Get specific page of contacts:
 
 ```python
 >>> a.contacts.list_contacts(page=2, per_page=5)
 [<Contact 'John Doe'>, <Contact 'Jane Sampleton'>,...]
 ```
 
-[<Contact 'Jane Sampleton'>]
-
-```
-[<Contact 'Jane Sampleton'>]
-```
-
 #### Update
 
 ```python
 >>> a.contacts.update_contact(1,
                               first_name='Jane',
                               last_name='Updated')
-<Contact 'Jane Updated'></Contact>
+<Contact 'Jane Updated'>
 ```
 
 ### Upsert
 
 ```python
 >>> a.contacts.upsert_contact(unique_identifier=('emails', 'janesampleton@gmail.com'),
                               first_name='Jane',
                               last_name='Upserted')
-<Contact 'Jane Upserted'></Contact>
+<Contact 'Jane Upserted'>
 ```
 
 #### Delete
 
 ```python
 >>> a.contacts.delete_contact(1)
 True
@@ -289,15 +283,15 @@
 ```
 
 #### Update
 
 ```python
 >>> a.lists.update_list(1,
                         name='My Updated List')
-<List 'My Updated List'></List>
+<List 'My Updated List'>
 ```
 
 #### Fetch Contacts
 
 ```python
 >>> a.lists.fetch_contacts_from_list(1)
 [<Contact 'John Doe'>, <Contact 'Jane Sampleton'>]
@@ -486,15 +480,15 @@
 
 #### Create
 
 ```python
 >>> a.notes.create_note(description='My Note',
                         targetable_type='Contact',
                         targetable_id=1)
-<Note 'My Note'></Note>
+<Note 'My Note'>
 ```
 
 #### Update
 
 ```python
 >>> a.notes.update_note(1,
                         description='My Updated Note')
```

### Comparing `python-freshworks-crm-1.0.5/setup.py` & `python-freshworks-crm-1.0.6/setup.py`

 * *Files identical despite different names*

