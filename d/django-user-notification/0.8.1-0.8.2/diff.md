# Comparing `tmp/django_user_notification-0.8.1.tar.gz` & `tmp/django_user_notification-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_user_notification-0.8.1.tar", max compression
+gzip compressed data, was "django_user_notification-0.8.2.tar", max compression
```

## Comparing `django_user_notification-0.8.1.tar` & `django_user_notification-0.8.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11347 2022-08-01 06:35:17.000000 django_user_notification-0.8.1/LICENSE
--rw-r--r--   0        0        0     4648 2023-04-13 02:57:49.997974 django_user_notification-0.8.1/README.md
--rw-r--r--   0        0        0       22 2023-04-18 07:02:27.476163 django_user_notification-0.8.1/notification/__init__.py
--rw-r--r--   0        0        0     3805 2023-04-12 10:58:28.320016 django_user_notification-0.8.1/notification/admin.py
--rw-r--r--   0        0        0      156 2023-03-06 01:45:02.889012 django_user_notification-0.8.1/notification/apps.py
--rw-r--r--   0        0        0     1301 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/backends/__init__.py
--rw-r--r--   0        0        0     4088 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/backends/aliyunsms.py
--rw-r--r--   0        0        0     3967 2023-04-12 11:07:43.899930 django_user_notification-0.8.1/notification/backends/dingchatbot.py
--rw-r--r--   0        0        0     4170 2022-08-08 06:38:56.158235 django_user_notification-0.8.1/notification/backends/dingtodotask.py
--rw-r--r--   0        0        0     4599 2023-04-18 06:59:20.038967 django_user_notification-0.8.1/notification/backends/dingworkmessage.py
--rw-r--r--   0        0        0     1193 2022-08-08 08:42:41.480190 django_user_notification-0.8.1/notification/backends/dummy.py
--rw-r--r--   0        0        0     2417 2023-04-12 11:08:12.028162 django_user_notification-0.8.1/notification/backends/email.py
--rw-r--r--   0        0        0     2216 2023-04-12 11:08:29.622794 django_user_notification-0.8.1/notification/backends/websocket.py
--rw-r--r--   0        0        0     6710 2023-04-12 11:12:05.725862 django_user_notification-0.8.1/notification/base.py
--rw-r--r--   0        0        0     1208 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/consumers.py
--rw-r--r--   0        0        0     3989 2023-04-12 11:09:49.072702 django_user_notification-0.8.1/notification/migrations/0001_initial.py
--rw-r--r--   0        0        0      630 2022-08-08 07:36:05.355986 django_user_notification-0.8.1/notification/migrations/0002_auto_20220808_0736.py
--rw-r--r--   0        0        0      885 2022-08-10 09:10:18.668000 django_user_notification-0.8.1/notification/migrations/0003_auto_20220810_1710.py
--rw-r--r--   0        0        0     1093 2022-08-12 07:05:54.107684 django_user_notification-0.8.1/notification/migrations/0004_auto_20220812_0705.py
--rw-r--r--   0        0        0      884 2023-01-29 05:37:49.837884 django_user_notification-0.8.1/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py
--rw-r--r--   0        0        0        0 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/migrations/__init__.py
--rw-r--r--   0        0        0     5188 2023-04-12 11:05:18.719018 django_user_notification-0.8.1/notification/models.py
--rw-r--r--   0        0        0      109 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/static/css/hide_admin_original.css
--rw-r--r--   0        0        0      174 2023-04-12 10:53:45.477657 django_user_notification-0.8.1/notification/urls.py
--rw-r--r--   0        0        0      785 2022-08-04 10:27:11.874598 django_user_notification-0.8.1/notification/utils.py
--rw-r--r--   0        0        0     1685 2023-04-18 07:02:27.482911 django_user_notification-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     5884 1970-01-01 00:00:00.000000 django_user_notification-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-08-01 06:35:17.000000 django_user_notification-0.8.2/LICENSE
+-rw-r--r--   0        0        0     4648 2023-04-13 02:57:49.997974 django_user_notification-0.8.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-18 07:43:41.803887 django_user_notification-0.8.2/notification/__init__.py
+-rw-r--r--   0        0        0     3805 2023-04-12 10:58:28.320016 django_user_notification-0.8.2/notification/admin.py
+-rw-r--r--   0        0        0      156 2023-03-06 01:45:02.889012 django_user_notification-0.8.2/notification/apps.py
+-rw-r--r--   0        0        0     1301 2022-08-01 03:08:17.000000 django_user_notification-0.8.2/notification/backends/__init__.py
+-rw-r--r--   0        0        0     4135 2023-05-18 07:43:18.299901 django_user_notification-0.8.2/notification/backends/aliyunsms.py
+-rw-r--r--   0        0        0     3967 2023-04-12 11:07:43.899930 django_user_notification-0.8.2/notification/backends/dingchatbot.py
+-rw-r--r--   0        0        0     4170 2022-08-08 06:38:56.158235 django_user_notification-0.8.2/notification/backends/dingtodotask.py
+-rw-r--r--   0        0        0     4599 2023-04-18 06:59:20.038967 django_user_notification-0.8.2/notification/backends/dingworkmessage.py
+-rw-r--r--   0        0        0     1193 2022-08-08 08:42:41.480190 django_user_notification-0.8.2/notification/backends/dummy.py
+-rw-r--r--   0        0        0     2417 2023-04-12 11:08:12.028162 django_user_notification-0.8.2/notification/backends/email.py
+-rw-r--r--   0        0        0     2216 2023-04-12 11:08:29.622794 django_user_notification-0.8.2/notification/backends/websocket.py
+-rw-r--r--   0        0        0     6710 2023-04-12 11:12:05.725862 django_user_notification-0.8.2/notification/base.py
+-rw-r--r--   0        0        0     1208 2022-08-01 03:08:17.000000 django_user_notification-0.8.2/notification/consumers.py
+-rw-r--r--   0        0        0     3989 2023-04-12 11:09:49.072702 django_user_notification-0.8.2/notification/migrations/0001_initial.py
+-rw-r--r--   0        0        0      630 2022-08-08 07:36:05.355986 django_user_notification-0.8.2/notification/migrations/0002_auto_20220808_0736.py
+-rw-r--r--   0        0        0      885 2022-08-10 09:10:18.668000 django_user_notification-0.8.2/notification/migrations/0003_auto_20220810_1710.py
+-rw-r--r--   0        0        0     1093 2022-08-12 07:05:54.107684 django_user_notification-0.8.2/notification/migrations/0004_auto_20220812_0705.py
+-rw-r--r--   0        0        0      884 2023-01-29 05:37:49.837884 django_user_notification-0.8.2/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:08:17.000000 django_user_notification-0.8.2/notification/migrations/__init__.py
+-rw-r--r--   0        0        0     5188 2023-04-12 11:05:18.719018 django_user_notification-0.8.2/notification/models.py
+-rw-r--r--   0        0        0      109 2022-08-01 03:08:17.000000 django_user_notification-0.8.2/notification/static/css/hide_admin_original.css
+-rw-r--r--   0        0        0      174 2023-04-12 10:53:45.477657 django_user_notification-0.8.2/notification/urls.py
+-rw-r--r--   0        0        0      785 2022-08-04 10:27:11.874598 django_user_notification-0.8.2/notification/utils.py
+-rw-r--r--   0        0        0     1685 2023-05-18 07:43:41.810364 django_user_notification-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     5884 1970-01-01 00:00:00.000000 django_user_notification-0.8.2/PKG-INFO
```

### Comparing `django_user_notification-0.8.1/LICENSE` & `django_user_notification-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/README.md` & `django_user_notification-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/admin.py` & `django_user_notification-0.8.2/notification/admin.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/backends/__init__.py` & `django_user_notification-0.8.2/notification/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/backends/aliyunsms.py` & `django_user_notification-0.8.2/notification/backends/aliyunsms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import json
 import typing
 
-from alibabacloud_dysmsapi20170525.client import Client as Dysmsapi20170525Client
-from alibabacloud_dysmsapi20170525.models import SendSmsRequest
-from alibabacloud_tea_openapi import models as open_api_models
 from django.conf import settings
 from django.contrib.auth.models import User
 from django.core.exceptions import ImproperlyConfigured
 
+try:
+    from alibabacloud_dysmsapi20170525.client import Client as Dysmsapi20170525Client
+    from alibabacloud_dysmsapi20170525.models import SendSmsRequest
+    from alibabacloud_tea_openapi import models as open_api_models
+except ImportError:
+    pass
+
 from notification.base import BaseNotificationBackend, notify
 
 
 class AliyunSMSNotificationBackend(BaseNotificationBackend):
     """
     A backend handle aliyun sms message.
     For details, see: https://help.aliyun.com/document_detail/419273.htm?spm=a2c4g.11186623.0.0.34375695hoVPSt
```

### Comparing `django_user_notification-0.8.1/notification/backends/dingchatbot.py` & `django_user_notification-0.8.2/notification/backends/dingchatbot.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/backends/dingtodotask.py` & `django_user_notification-0.8.2/notification/backends/dingtodotask.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/backends/dingworkmessage.py` & `django_user_notification-0.8.2/notification/backends/dingworkmessage.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/backends/dummy.py` & `django_user_notification-0.8.2/notification/backends/dummy.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/backends/email.py` & `django_user_notification-0.8.2/notification/backends/email.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/backends/websocket.py` & `django_user_notification-0.8.2/notification/backends/websocket.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/base.py` & `django_user_notification-0.8.2/notification/base.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/consumers.py` & `django_user_notification-0.8.2/notification/consumers.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/migrations/0001_initial.py` & `django_user_notification-0.8.2/notification/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/migrations/0002_auto_20220808_0736.py` & `django_user_notification-0.8.2/notification/migrations/0002_auto_20220808_0736.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/migrations/0003_auto_20220810_1710.py` & `django_user_notification-0.8.2/notification/migrations/0003_auto_20220810_1710.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/migrations/0004_auto_20220812_0705.py` & `django_user_notification-0.8.2/notification/migrations/0004_auto_20220812_0705.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py` & `django_user_notification-0.8.2/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/models.py` & `django_user_notification-0.8.2/notification/models.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/notification/utils.py` & `django_user_notification-0.8.2/notification/utils.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.1/pyproject.toml` & `django_user_notification-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.commitizen]
-version = "0.8.1"
+version = "0.8.2"
 changelog_start_rev = "0.7.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = ["pyproject.toml:version", "notification/__init__.py"]
 
 [tool.poetry]
 name = "django-user-notification"
-version = "0.8.1"
+version = "0.8.2"
 description = "Django message notification package"
 authors = ["Aiden Lu <allaher@icloud.com>"]
 readme = "README.md"
 keywords = ["notification", "django"]
 packages = [{ include = "notification" }]
 homepage = "https://github.com/aiden520/django-user-notification"
 repository = "https://github.com/aiden520/django-user-notification"
```

### Comparing `django_user_notification-0.8.1/PKG-INFO` & `django_user_notification-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-user-notification
-Version: 0.8.1
+Version: 0.8.2
 Summary: Django message notification package
 Home-page: https://github.com/aiden520/django-user-notification
 License: Apache-2.0
 Keywords: notification,django
 Author: Aiden Lu
 Author-email: allaher@icloud.com
 Requires-Python: >=3.8
```

