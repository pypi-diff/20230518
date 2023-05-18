# Comparing `tmp/django_gcp-0.9.1.tar.gz` & `tmp/django_gcp-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gcp-0.9.1.tar", max compression
+gzip compressed data, was "django_gcp-0.9.2.tar", max compression
```

## Comparing `django_gcp-0.9.1.tar` & `django_gcp-0.9.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1080 2023-05-04 12:22:25.483580 django_gcp-0.9.1/LICENSE
--rw-r--r--   0        0        0     3746 2023-05-04 12:22:25.483580 django_gcp-0.9.1/README.md
--rw-r--r--   0        0        0       58 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/__init__.py
--rw-r--r--   0        0        0      627 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/apps.py
--rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/events/__init__.py
--rw-r--r--   0        0        0       63 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/events/signals.py
--rw-r--r--   0        0        0     7279 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/events/utils.py
--rw-r--r--   0        0        0     1703 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/events/views.py
--rw-r--r--   0        0        0     1342 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/exceptions.py
--rw-r--r--   0        0        0      189 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/logging/__init__.py
--rw-r--r--   0        0        0     2212 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/logging/error_reporting.py
--rw-r--r--   0        0        0     1765 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/logging/structured_logs.py
--rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/commands/__init__.py
--rw-r--r--   0        0        0      816 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/commands/_base.py
--rw-r--r--   0        0        0     1637 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/commands/cleanup_tmp_files.py
--rw-r--r--   0        0        0     1760 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/management/commands/task_manager.py
--rw-r--r--   0        0        0       96 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/metadata/__init__.py
--rw-r--r--   0        0        0     3410 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/metadata/metadata.py
--rw-r--r--   0        0        0      170 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/signals.py
--rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/static/.gitignore
--rw-r--r--   0        0        0     2630 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/static/django_gcp/cloud_object_widget.css
--rw-r--r--   0        0        0     7686 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/static/django_gcp/cloud_object_widget.js
--rw-r--r--   0        0        0      328 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/compress.py
--rw-r--r--   0        0        0    22857 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/fields.py
--rw-r--r--   0        0        0     2595 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/forms.py
--rw-r--r--   0        0        0    14266 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/gcloud.py
--rw-r--r--   0        0        0     6373 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/operations.py
--rw-r--r--   0        0        0     4427 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/settings.py
--rw-r--r--   0        0        0     3202 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/utils.py
--rw-r--r--   0        0        0     1942 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/storage/widgets.py
--rw-r--r--   0        0        0      192 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/__init__.py
--rw-r--r--   0        0        0     1124 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/_patch_cloud_scheduler.py
--rw-r--r--   0        0        0     1106 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/_patch_cloud_tasks.py
--rw-r--r--   0        0        0      350 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/helpers.py
--rw-r--r--   0        0        0     8669 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/manager.py
--rw-r--r--   0        0        0     1307 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/serializers.py
--rw-r--r--   0        0        0    11229 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/tasks.py
--rw-r--r--   0        0        0     1836 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/tasks/views.py
--rw-r--r--   0        0        0        0 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/templates/django_gcp/.gitignore
--rw-r--r--   0        0        0     2571 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/templates/django_gcp/cloud_object_widget.html
--rw-r--r--   0        0        0      491 2023-05-04 12:22:25.483580 django_gcp-0.9.1/django_gcp/urls.py
--rw-r--r--   0        0        0     1651 2023-05-04 12:22:25.487580 django_gcp-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 django_gcp-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-18 07:55:48.665574 django_gcp-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3746 2023-05-18 07:55:48.665574 django_gcp-0.9.2/README.md
+-rw-r--r--   0        0        0       58 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/apps.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/events/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/events/signals.py
+-rw-r--r--   0        0        0     7279 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/events/utils.py
+-rw-r--r--   0        0        0     1703 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/events/views.py
+-rw-r--r--   0        0        0     1450 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/exceptions.py
+-rw-r--r--   0        0        0      189 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/logging/__init__.py
+-rw-r--r--   0        0        0     2212 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/logging/error_reporting.py
+-rw-r--r--   0        0        0     1765 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/logging/structured_logs.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/commands/__init__.py
+-rw-r--r--   0        0        0      816 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/commands/_base.py
+-rw-r--r--   0        0        0     1637 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/commands/cleanup_tmp_files.py
+-rw-r--r--   0        0        0     1760 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/commands/task_manager.py
+-rw-r--r--   0        0        0       96 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/metadata/__init__.py
+-rw-r--r--   0        0        0     3410 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/metadata/metadata.py
+-rw-r--r--   0        0        0      170 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/signals.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/static/.gitignore
+-rw-r--r--   0        0        0     2630 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/static/django_gcp/cloud_object_widget.css
+-rw-r--r--   0        0        0     7686 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/static/django_gcp/cloud_object_widget.js
+-rw-r--r--   0        0        0      328 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/compress.py
+-rw-r--r--   0        0        0    22857 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/fields.py
+-rw-r--r--   0        0        0     2595 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/forms.py
+-rw-r--r--   0        0        0    14266 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/gcloud.py
+-rw-r--r--   0        0        0     6373 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/operations.py
+-rw-r--r--   0        0        0     4427 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/settings.py
+-rw-r--r--   0        0        0     3202 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/utils.py
+-rw-r--r--   0        0        0     1942 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/widgets.py
+-rw-r--r--   0        0        0      192 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/__init__.py
+-rw-r--r--   0        0        0     1124 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/_patch_cloud_scheduler.py
+-rw-r--r--   0        0        0     1106 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/_patch_cloud_tasks.py
+-rw-r--r--   0        0        0      350 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/helpers.py
+-rw-r--r--   0        0        0     8860 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/manager.py
+-rw-r--r--   0        0        0     1307 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/serializers.py
+-rw-r--r--   0        0        0    11797 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/tasks.py
+-rw-r--r--   0        0        0     1836 2023-05-18 07:55:48.669574 django_gcp-0.9.2/django_gcp/tasks/views.py
+-rw-r--r--   0        0        0        0 2023-05-18 07:55:48.669574 django_gcp-0.9.2/django_gcp/templates/django_gcp/.gitignore
+-rw-r--r--   0        0        0     2571 2023-05-18 07:55:48.669574 django_gcp-0.9.2/django_gcp/templates/django_gcp/cloud_object_widget.html
+-rw-r--r--   0        0        0      491 2023-05-18 07:55:48.669574 django_gcp-0.9.2/django_gcp/urls.py
+-rw-r--r--   0        0        0     1651 2023-05-18 07:55:48.677574 django_gcp-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 django_gcp-0.9.2/PKG-INFO
```

### Comparing `django_gcp-0.9.1/LICENSE` & `django_gcp-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/README.md` & `django_gcp-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/apps.py` & `django_gcp-0.9.2/django_gcp/apps.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/events/utils.py` & `django_gcp-0.9.2/django_gcp/events/utils.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/events/views.py` & `django_gcp-0.9.2/django_gcp/events/views.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/exceptions.py` & `django_gcp-0.9.2/django_gcp/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,7 +32,11 @@
 
 class AttemptedOverwriteError(Exception):
     """Raised when attempting to overwrite an existing object in GCS with another object"""
 
 
 class MissingBlobError(Exception):
     """Raised when attempting to access or copy a blob that is not present in GCS"""
+
+
+class IncompatibleSettingsError(ValueError):
+    """Raised when settings values are mutually exclusive"""
```

### Comparing `django_gcp-0.9.1/django_gcp/logging/error_reporting.py` & `django_gcp-0.9.2/django_gcp/logging/error_reporting.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/logging/structured_logs.py` & `django_gcp-0.9.2/django_gcp/logging/structured_logs.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/management/commands/_base.py` & `django_gcp-0.9.2/django_gcp/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/management/commands/cleanup_tmp_files.py` & `django_gcp-0.9.2/django_gcp/management/commands/cleanup_tmp_files.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/management/commands/task_manager.py` & `django_gcp-0.9.2/django_gcp/management/commands/task_manager.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/metadata/metadata.py` & `django_gcp-0.9.2/django_gcp/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/static/django_gcp/cloud_object_widget.css` & `django_gcp-0.9.2/django_gcp/static/django_gcp/cloud_object_widget.css`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/static/django_gcp/cloud_object_widget.js` & `django_gcp-0.9.2/django_gcp/static/django_gcp/cloud_object_widget.js`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/storage/compress.py` & `django_gcp-0.9.2/django_gcp/storage/compress.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/storage/fields.py` & `django_gcp-0.9.2/django_gcp/storage/fields.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/storage/forms.py` & `django_gcp-0.9.2/django_gcp/storage/forms.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/storage/gcloud.py` & `django_gcp-0.9.2/django_gcp/storage/gcloud.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/storage/operations.py` & `django_gcp-0.9.2/django_gcp/storage/operations.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/storage/settings.py` & `django_gcp-0.9.2/django_gcp/storage/settings.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/storage/utils.py` & `django_gcp-0.9.2/django_gcp/storage/utils.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/storage/widgets.py` & `django_gcp-0.9.2/django_gcp/storage/widgets.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/tasks/_patch_cloud_scheduler.py` & `django_gcp-0.9.2/django_gcp/tasks/_patch_cloud_scheduler.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/tasks/_patch_cloud_tasks.py` & `django_gcp-0.9.2/django_gcp/tasks/_patch_cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/tasks/manager.py` & `django_gcp-0.9.2/django_gcp/tasks/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 
     @property
     def delimiter(self):
         """Return the GCP_TASKS_DELIMITER setting or a default"""
         return getattr(settings, "GCP_TASKS_DELIMITER", "--")
 
     @property
+    def disable_execute(self):
+        """Return the GCP_TASKS_DISABLE_EXECUTE setting or default False"""
+        return getattr(settings, "GCP_TASKS_DISABLE_EXECUTE", False)
+
+    @property
     def domain(self):
         """Return the GCP_TASKS_DOMAIN setting or a default"""
         _domain = getattr(settings, "GCP_TASKS_DOMAIN")
         if not _domain.startswith("https://"):
             message = f"The GCP_TASKS_DOMAIN setting is invalid for use with a GCP PubSub push subscription. Endpoints need to be valid and secure (setting is: {_domain})."
             raise exceptions.InvalidEndpointError(message)
         return _domain
```

### Comparing `django_gcp-0.9.1/django_gcp/tasks/serializers.py` & `django_gcp-0.9.2/django_gcp/tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/tasks/tasks.py` & `django_gcp-0.9.2/django_gcp/tasks/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from abc import abstractmethod
 from datetime import datetime, timedelta
 from django.apps import apps
 from django.template.defaultfilters import slugify
 from django.urls import reverse
 from django.utils.timezone import now
 from django_gcp.events.utils import decode_pubsub_message
-from django_gcp.exceptions import DuplicateTaskError, IncorrectTaskUsageError
+from django_gcp.exceptions import DuplicateTaskError, IncompatibleSettingsError, IncorrectTaskUsageError
 from gcp_pilot.pubsub import CloudPublisher, CloudSubscriber
 from google.api_core.exceptions import AlreadyExists
 from google.cloud import pubsub_v1
 
 from ._patch_cloud_scheduler import CloudScheduler
 from ._patch_cloud_tasks import CloudTasks
 from .helpers import run_coroutine
@@ -79,21 +79,27 @@
 class Task(metaclass=TaskMeta):
     """Task base class"""
 
     _url_name = "gcp-tasks"
     deduplicate = False
 
     def enqueue(self, **kwargs):
-        """Invoke a task (place it onto a queue for processing)"""
+        """Invoke a task (place it onto a queue for processing)
+
+        Some settings affect the behaviour of this method, allowing bypass or immediate execution. See settings documentation for more.
+        """
         return self._send(
             task_kwargs=kwargs,
         )
 
     def enqueue_later(self, when, **kwargs):
-        """Invoke a task (place it onto a queue for processing after some time delay)"""
+        """Invoke a task (place it onto a queue for processing after some time delay)
+
+        Some settings affect the behaviour of this method, allowing bypass or immediate execution. See settings documentation for more.
+        """
         if isinstance(when, int):
             delay_in_seconds = when
         elif isinstance(when, timedelta):
             delay_in_seconds = when.total_seconds()
         elif isinstance(when, datetime):
             delay_in_seconds = (when - now()).total_seconds()
         else:
@@ -159,14 +165,20 @@
     # mechanisms (e.g. Cloud Scheduler and Pub/Sub).
     # The Task class is thus treated only partly as an ABC.
     # We should refactor Task to split it into two; a true ABC containing only
     # common functionality, and an OnDemandTask class which implements the detail of
     # interacting with Cloud Tasks, like the following _send method
 
     def _send(self, task_kwargs, api_kwargs=None):
+        if self.manager.disable_execute and self.manager.eager_execute:
+            raise IncompatibleSettingsError("disable_execute and eager_execute should be mutually exclusive")
+
+        if self.manager.disable_execute:
+            return None
+
         payload = serialize(task_kwargs)
         if self.manager.eager_execute:
             return self.run(**deserialize(payload))
 
         api_kwargs = api_kwargs or {}
         api_kwargs.update(
             dict(
```

### Comparing `django_gcp-0.9.1/django_gcp/tasks/views.py` & `django_gcp-0.9.2/django_gcp/tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/django_gcp/templates/django_gcp/cloud_object_widget.html` & `django_gcp-0.9.2/django_gcp/templates/django_gcp/cloud_object_widget.html`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.1/pyproject.toml` & `django_gcp-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-gcp"
-version = "0.9.1"
+version = "0.9.2"
 description = "Utilities to run Django on Google Cloud Platform"
 authors = ["Tom Clark"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `django_gcp-0.9.1/PKG-INFO` & `django_gcp-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gcp
-Version: 0.9.1
+Version: 0.9.2
 Summary: Utilities to run Django on Google Cloud Platform
 Home-page: https://github.com/octue/django-gcp
 License: MIT
 Keywords: django,google,cloud,gcloud,gcp
 Author: Tom Clark
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
```

