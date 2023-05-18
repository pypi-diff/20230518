# Comparing `tmp/python-freshworks-crm-1.0.4.tar.gz` & `tmp/python-freshworks-crm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-freshworks-crm-1.0.4.tar", last modified: Wed May 17 17:51:13 2023, max compression
+gzip compressed data, was "dist\python-freshworks-crm-1.0.5.tar", last modified: Thu May 18 16:22:37 2023, max compression
```

## Comparing `python-freshworks-crm-1.0.4.tar` & `python-freshworks-crm-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/freshsales/
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:26.000000 python-freshworks-crm-1.0.4/freshsales/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/freshsales/v2/
--rw-rw-rw-   0        0        0    36122 2023-05-17 17:15:40.000000 python-freshworks-crm-1.0.4/freshsales/v2/api.py
--rw-rw-rw-   0        0        0      672 2023-05-06 14:43:54.000000 python-freshworks-crm-1.0.4/freshsales/v2/errors.py
--rw-rw-rw-   0        0        0     6751 2023-05-16 19:48:06.000000 python-freshworks-crm-1.0.4/freshsales/v2/models.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/
--rw-rw-rw-   0        0        0     7914 2023-05-16 19:03:28.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/conftest.py
--rw-rw-rw-   0        0        0     3549 2023-05-13 23:26:20.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_accounts.py
--rw-rw-rw-   0        0        0     2711 2023-05-16 11:24:32.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_appointments.py
--rw-rw-rw-   0        0        0     3567 2023-05-13 23:26:09.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_contacts.py
--rw-rw-rw-   0        0        0     3368 2023-05-16 15:02:47.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_deals.py
--rw-rw-rw-   0        0        0     3344 2023-05-16 19:06:03.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_documents.py
--rw-rw-rw-   0        0        0     2422 2023-05-14 12:53:28.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_lists.py
--rw-rw-rw-   0        0        0     1727 2023-05-14 13:16:40.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_notes.py
--rw-rw-rw-   0        0        0     4032 2023-05-16 15:03:28.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_products.py
--rw-rw-rw-   0        0        0     2907 2023-05-16 19:05:03.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_sales_activities.py
--rw-rw-rw-   0        0        0     6561 2023-05-14 20:08:32.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_selectors.py
--rw-rw-rw-   0        0        0     3241 2023-05-15 01:49:25.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/test_tasks.py
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:43.000000 python-freshworks-crm-1.0.4/freshsales/v2/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-06 00:00:11.000000 python-freshworks-crm-1.0.4/freshsales/v2/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-17 17:50:50.000000 python-freshworks-crm-1.0.4/freshsales/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-16 20:08:52.000000 python-freshworks-crm-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      878 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      878 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/requires.txt
--rw-rw-rw-   0        0        0      866 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-05-17 17:51:12.000000 python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      443 2023-05-16 19:56:20.000000 python-freshworks-crm-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 17:51:13.000000 python-freshworks-crm-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-05-16 22:04:30.000000 python-freshworks-crm-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/freshsales/
+-rw-rw-rw-   0        0        0    36055 2023-05-18 15:47:25.000000 python-freshworks-crm-1.0.5/freshsales/api.py
+-rw-rw-rw-   0        0        0      672 2023-05-06 14:43:54.000000 python-freshworks-crm-1.0.5/freshsales/errors.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:26.000000 python-freshworks-crm-1.0.5/freshsales/exceptions.py
+-rw-rw-rw-   0        0        0     6751 2023-05-16 19:48:06.000000 python-freshworks-crm-1.0.5/freshsales/models.py
+drwxrwxrwx   0        0        0        0 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/freshsales/tests/
+-rw-rw-rw-   0        0        0     7911 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/conftest.py
+-rw-rw-rw-   0        0        0     3546 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_accounts.py
+-rw-rw-rw-   0        0        0     2700 2023-05-18 15:40:21.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_appointments.py
+-rw-rw-rw-   0        0        0     3564 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_contacts.py
+-rw-rw-rw-   0        0        0     3365 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_deals.py
+-rw-rw-rw-   0        0        0     3341 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_documents.py
+-rw-rw-rw-   0        0        0     2419 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_lists.py
+-rw-rw-rw-   0        0        0     1724 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_notes.py
+-rw-rw-rw-   0        0        0     4029 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_products.py
+-rw-rw-rw-   0        0        0     2788 2023-05-18 15:47:50.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_sales_activities.py
+-rw-rw-rw-   0        0        0     6558 2023-05-18 10:33:56.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_selectors.py
+-rw-rw-rw-   0        0        0     3230 2023-05-18 15:42:59.000000 python-freshworks-crm-1.0.5/freshsales/tests/test_tasks.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 00:00:43.000000 python-freshworks-crm-1.0.5/freshsales/tests/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-18 10:54:29.000000 python-freshworks-crm-1.0.5/freshsales/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 20:08:52.000000 python-freshworks-crm-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      878 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      878 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      792 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2023-05-18 16:22:36.000000 python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25929 2023-05-18 16:19:29.000000 python-freshworks-crm-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 16:22:37.000000 python-freshworks-crm-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2023-05-18 03:21:39.000000 python-freshworks-crm-1.0.5/setup.py
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/api.py` & `python-freshworks-crm-1.0.5/freshsales/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 import requests
 from requests import HTTPError
 
-from freshsales.v2.errors import *
+from freshsales.errors import *
 
-from freshsales.v2.models import *
+from freshsales.models import *
 
 
 class ContactAPI(object):
     def __init__(self, api):
         self._api = api
 
     def create_contact(self, **kwargs):
@@ -373,15 +373,15 @@
         if response.get('sales_accounts'):
             response['sales_accounts'] = [Account(**account)
                                           for account in response['sales_accounts']]
         if response.get('deals'):
             response['deals'] = Deal(**response['deal'])
         return response
 
-    def list_all_tasks(self, filter_param, *include, page=None, per_page=100):
+    def list_tasks(self, filter_param, *include, page=None, per_page=100):
         url = f'/tasks?filter={filter_param}'
         url += f'&include={",".join(include)}' if include else ''
 
         tasks = self._api._get(url)
 
         if not tasks.get("tasks"):
             return tasks
@@ -447,15 +447,15 @@
     def view_appointment(self, appointment_id):
         url = f'/appointments/{appointment_id}'
         response = self._api._get(url)
         response['appointment'] = Appointment(**response['appointment'])
         response['notes'] = [Note(**note) for note in response['notes']]
         return response
 
-    def list_all_appointments(self, filter_param, *include, page=None, per_page=100):
+    def list_appointments(self, filter_param, *include, page=None, per_page=100):
         url = f'/appointments?filter={filter_param}'
         url += f'&include={",".join(include)}' if include else ''
 
         response = self._api._get(url)
         total_pages = response.get('meta', {}).get('total_pages', 1)
         appointments = response.get('appointments', [])
 
@@ -491,26 +491,26 @@
         return self._api._delete(url).get('success') == "200"
 
 
 class SalesActivityAPI(object):
     def __init__(self, api):
         self._api = api
 
-    def create_sales_activity(self, **kwargs):
+    def create_activity(self, **kwargs):
         url = '/sales_activities'
         data = {'sales_activity': kwargs}
         response = self._api._post(url, data=json.dumps(data))
         return SalesActivity(**response.get('sales_activity', {}))
 
-    def view_sales_activity(self, sales_activity_id):
+    def view_activity(self, sales_activity_id):
         url = f'/sales_activities/{sales_activity_id}'
         response = self._api._get(url)
         return SalesActivity(**response.get('sales_activity', {}))
 
-    def list_all_sales_activities(self, page=None, per_page=10):
+    def list_activities(self, page=None, per_page=10):
         url = '/sales_activities'
         response = self._api._get(url)
 
         sales_activities = response.get('sales_activities', [])
         total_pages = response.get('meta', {}).get('total_pages', 1)
 
         # In case pagination is required
@@ -528,26 +528,26 @@
             page_sales_activities = self._api._get(
                 url + f"?page={page}&per_page={per_page}").get('sales_activities', [])
             sales_activities = [SalesActivity(
                 **activity) for activity in page_sales_activities]
 
         return sales_activities
 
-    def list_all_sales_activity_fields(self):
+    def list_fields(self):
         url = '/settings/sales_activities/fields'
         response = self._api._get(url)
         return [Field(**field) for field in response.get('fields', [])]
 
-    def update_sales_activity(self, sales_activity_id, **kwargs):
+    def update_activity(self, sales_activity_id, **kwargs):
         url = f'/sales_activities/{sales_activity_id}'
         data = {'sales_activity': kwargs}
         response = self._api._put(url, data=json.dumps(data))
         return SalesActivity(**response.get('sales_activity', {}))
 
-    def delete_sales_activity(self, sales_activity_id):
+    def delete_activity(self, sales_activity_id):
         url = f'/sales_activities/{sales_activity_id}'
         return self._api._delete(url).get('success') == "200"
 
 
 class ProductAPI(object):
     def __init__(self, api):
         self._api = api
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/errors.py` & `python-freshworks-crm-1.0.5/freshsales/errors.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/models.py` & `python-freshworks-crm-1.0.5/freshsales/models.py`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/conftest.py` & `python-freshworks-crm-1.0.5/freshsales/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from freshsales.v2.api import API
+from freshsales.api import API
 import pytest
 import json
 import os.path
 import re
 
 DOMAIN = 'apiwrapperinc.myfreshworks.com/crm/sales'
 API_KEY = 'AIaj6VTSzNm0hoNdzTSJUg'
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_accounts.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import (
+from freshsales.models import (
     Account,
     View,
     Field,
 )
 
 
 @pytest.fixture
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_appointments.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_appointments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import Appointment
+from freshsales.models import Appointment
 
 
 @pytest.fixture
 def appointment(api):
     return api.appointments.view_appointment(31001473829).get('appointment')
 
 
@@ -35,16 +35,16 @@
     assert isinstance(appointment, Appointment)
     assert appointment.title == "Sample Appointment"
     assert appointment.description == "This is just a sample Appointment."
     assert isinstance(appointment.from_date, datetime.datetime)
     assert isinstance(appointment.end_date, datetime.datetime)
 
 
-def test_list_all_appointments(api):
-    appointments = api.appointments.list_all_appointments("upcoming")
+def test_list_appointments(api):
+    appointments = api.appointments.list_appointments("upcoming")
 
     if appointments:
         appointment = appointments[1]
         assert isinstance(appointment, Appointment)
         assert appointment.title == "(Sample) Meeting - final discussion about the deal"
         assert isinstance(appointment.from_date, datetime.datetime)
         assert isinstance(appointment.end_date, datetime.datetime)
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_contacts.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_contacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import Contact, Field, View
+from freshsales.models import Contact, Field, View
 
 
 @pytest.fixture
 def contact(api):
     return api.contacts.view_contact(31016358306)
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_deals.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_deals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import (
+from freshsales.models import (
     Deal,
     View,
     Field,
 )
 
 
 @pytest.fixture
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_documents.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import (
+from freshsales.models import (
     Document,
     Product,
 )
 
 
 @pytest.fixture
 def document(api):
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_lists.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from freshsales.v2.models import (
+from freshsales.models import (
     List,
     Contact,
 )
 
 
 def test_create_list(api):
     mlist = api.lists.create_list("Brand Lovers")
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_notes.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import Note
+from freshsales.models import Note
 
 
 @pytest.fixture
 def note(api):
     return api.notes.view_note(31003638276)
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_products.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_products.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import (
+from freshsales.models import (
     Product,
     Deal,
 )
 
 
 @pytest.fixture
 def product(api):
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_sales_activities.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_sales_activities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import (
+from freshsales.models import (
     SalesActivity,
     Field,
 )
 
 
 @pytest.fixture
 def sales_activity(api):
-    return api.sales_activities.view_sales_activity(31000274656)
+    return api.sales_activities.view_activity(31000274656)
 
 
-def test_create_sales_activity(api):
-    sales_activity = api.sales_activities.create_sales_activity(
+def test_create_activity(api):
+    sales_activity = api.sales_activities.create_activity(
         title='ticket',
         notes='sample',
         targetable_id=31016358306,
         targetable_type='Contact',
         start_date='2017-12-04T17:00:00+05:30',
         end_date='2017-12-04T17:30:00+05:30',
         owner_id=31000148397,
@@ -29,54 +29,54 @@
     assert sales_activity.notes == "sample"
     assert sales_activity.targetable_id == 31016358306
     assert isinstance(sales_activity.start_date, datetime.datetime)
     assert isinstance(sales_activity.end_date, datetime.datetime)
     assert isinstance(sales_activity.created_at, datetime.datetime)
 
 
-def test_view_sales_activity(sales_activity):
+def test_view_activity(sales_activity):
     assert isinstance(sales_activity, SalesActivity)
     assert sales_activity.title == "ticket"
     assert sales_activity.notes == "sample"
     assert sales_activity.targetable_id == 31016358306
     assert isinstance(sales_activity.start_date, datetime.datetime)
     assert isinstance(sales_activity.end_date, datetime.datetime)
     assert isinstance(sales_activity.created_at, datetime.datetime)
 
 
-def test_list_all_sales_activities(api):
-    sales_activities = api.sales_activities.list_all_sales_activities()
+def test_listes_activities(api):
+    sales_activities = api.sales_activities.list_activities()
     assert isinstance(sales_activities[0], SalesActivity)
     assert sales_activities[0].title == "ticket"
     assert sales_activities[1].title == "ticket 2"
     assert sales_activities[0].targetable_id == 31016358306
     assert isinstance(sales_activities[0].start_date, datetime.datetime)
     assert isinstance(sales_activities[0].end_date, datetime.datetime)
     assert isinstance(sales_activities[0].created_at, datetime.datetime)
 
 
-def test_list_all_sales_activity_fields(api):
-    fields = api.sales_activities.list_all_sales_activity_fields()
+def test_list_fields(api):
+    fields = api.sales_activities.list_fields()
     assert isinstance(fields, list)
     assert isinstance(fields[0], Field)
     assert fields[1].name == "start_date"
 
 
-def test_update_sales_activity(api):
-    sales_activity = api.sales_activities.update_sales_activity(
+def test_update_activity(api):
+    sales_activity = api.sales_activities.update_activity(
         31000274656, title='ticket Updated')
     assert isinstance(sales_activity, SalesActivity)
     assert sales_activity.title == "ticket Updated"
 
 
-def test_delete_sales_activity(api):
-    assert api.sales_activities.delete_sales_activity(31000274656) == True
+def test_delete_activity(api):
+    assert api.sales_activities.delete_activity(31000274656) == True
 
 
-def test_sales_activity_str(sales_activity):
+def test_activity_str(sales_activity):
     assert str(
         sales_activity) == "ticket"
 
 
-def test_sales_activity_repr(sales_activity):
+def test_activity_repr(sales_activity):
     assert repr(
         sales_activity) == "<SalesActivity 'ticket' #31000274656>"
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_selectors.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_selectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import (
+from freshsales.models import (
     User,
     Territory,
     DealStage,
     Currency,
     DealReason,
     DealType,
     LeadSource,
```

### Comparing `python-freshworks-crm-1.0.4/freshsales/v2/tests/test_tasks.py` & `python-freshworks-crm-1.0.5/freshsales/tests/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 
 import pytest
 
-from freshsales.v2.models import (
+from freshsales.models import (
     Task,
     Contact,
     User,
     Account,
     Deal,
 )
 
@@ -45,16 +45,16 @@
         assert isinstance(contacts[0], Contact)
 
     if users:
         assert isinstance(users, list)
         assert isinstance(users[0], User)
 
 
-def test_list_all_tasks(api):
-    response = api.tasks.list_all_tasks("open")
+def test_list_tasks(api):
+    response = api.tasks.list_tasks("open")
     contacts = response.get('contacts')
     users = response.get('users')
     tasks = response.get('tasks')
     accounts = response.get('accounts')
     deals = response.get('deals')
 
     if tasks:
```

### Comparing `python-freshworks-crm-1.0.4/LICENSE` & `python-freshworks-crm-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-freshworks-crm-1.0.4/PKG-INFO` & `python-freshworks-crm-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-freshworks-crm
-Version: 1.0.4
+Version: 1.0.5
 Summary: An API wrapper for the Freshsales CRM
 Home-page: https://github.com/robertvy/python-freshworksCRM
 Author: Robert Van Ysendyck
 Author-email: rvy@vyp-consulting.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-freshworks-crm-1.0.4/python_freshworks_crm.egg-info/PKG-INFO` & `python-freshworks-crm-1.0.5/python_freshworks_crm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-freshworks-crm
-Version: 1.0.4
+Version: 1.0.5
 Summary: An API wrapper for the Freshsales CRM
 Home-page: https://github.com/robertvy/python-freshworksCRM
 Author: Robert Van Ysendyck
 Author-email: rvy@vyp-consulting.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `python-freshworks-crm-1.0.4/setup.py` & `python-freshworks-crm-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires=[
         "requests",
         "python-dateutil",
     ],
     extras_require={
         'test': [
             'pytest',
-            'pytest-mock'
+            'pytest-mock',
         ],
     },
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
```

