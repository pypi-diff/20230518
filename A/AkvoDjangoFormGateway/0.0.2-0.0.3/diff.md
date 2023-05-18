# Comparing `tmp/AkvoDjangoFormGateway-0.0.2.tar.gz` & `tmp/AkvoDjangoFormGateway-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoDjangoFormGateway-0.0.2.tar", last modified: Mon May 15 15:53:00 2023, max compression
+gzip compressed data, was "AkvoDjangoFormGateway-0.0.3.tar", last modified: Thu May 18 09:56:17 2023, max compression
```

## Comparing `AkvoDjangoFormGateway-0.0.2.tar` & `AkvoDjangoFormGateway-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 15:53:00.158035 AkvoDjangoFormGateway-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/management/commands/fake_data_seeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/management/commands/form_seeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-15 15:52:49.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:53:00.154035 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-15 15:53:00.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-15 15:53:00.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:53:00.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:53:00.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 15:53:00.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 15:53:00.000000 AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.742553 AkvoDjangoFormGateway-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-18 09:56:17.746553 AkvoDjangoFormGateway-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-18 09:56:17.746553 AkvoDjangoFormGateway-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.730553 AkvoDjangoFormGateway-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.738553 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.738553 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.738553 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/management/commands/fake_data_seeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/management/commands/form_seeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.742553 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.742553 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.742553 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-18 09:56:08.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:56:17.738553 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-18 09:56:17.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-18 09:56:17.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:56:17.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:56:17.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 09:56:17.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 09:56:17.000000 AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/top_level.txt
```

### Comparing `AkvoDjangoFormGateway-0.0.2/LICENSE` & `AkvoDjangoFormGateway-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.2/PKG-INFO` & `AkvoDjangoFormGateway-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.2/README.md` & `AkvoDjangoFormGateway-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.2/setup.py` & `AkvoDjangoFormGateway-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 # -*- coding: utf-8 -*-
 import sys
 import setuptools
 
 
-
 INSTALL_PYTHON_REQUIRES = []
 # We are intending to keep up to date with the supported Django versions.
 # For the official support, please visit:
 # https://docs.djangoproject.com/en/4.0/faq/install/#what-python-version-can-i-use-with-django
 if sys.version_info[1] in [8, 9, 10, 11]:
     django_python_version_install = "Django>=4.0.4"
     INSTALL_PYTHON_REQUIRES.append(django_python_version_install)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name='AkvoDjangoFormGateway',
+    name="AkvoDjangoFormGateway",
     author="Akvo",
     author_email="tech.consultancy@akvo.org",
     maintainer="Deden Bangkit",
     maintainer_email="deden@akvo.org",
-    description="A Django library that enables seamless integration of messenger services",
-    keywords='akvo, twilio, whatsapp, ssid, sms, django',
+    description=(
+        "A Django library that enables seamless integration of messenger"
+        " services"
+    ),
+    keywords="akvo, twilio, whatsapp, ssid, sms, django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     zip_safe=False,
     include_package_data=True,
-    url='https://github.com/akvo/Akvo-DjangoFormGateway',
+    url="https://github.com/akvo/Akvo-DjangoFormGateway",
     project_urls={
         "Documentation": "https://github.com/akvo/Akvo-DjangoFormGateway",
         "Bug Reports": "https://github.com/akvo/Akvo-DjangoFormGateway/issues",
         "Source Code": "https://github.com/akvo/Akvo-DjangoFormGateway",
     },
     classifiers=[
         # https://pypi.org/classifiers/
         "Development Status :: 4 - Beta",
-        'Intended Audience :: Developers',
-        'License :: Public Domain',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy',
-        'Framework :: Django',
-        'Framework :: Django :: 4.0',
-        'Framework :: Django :: 4.1',
+        "Intended Audience :: Developers",
+        "License :: Public Domain",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Framework :: Django",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
         "Operating System :: OS Independent",
-        'Topic :: Internet :: WWW/HTTP',
+        "Topic :: Internet :: WWW/HTTP",
     ],
     python_requires=">=3.8.5",
     install_requires=[
-        'setuptools>=36.2',
-        'twilio>=8.2.0',
-        'djangorestframework>=3.12.4',
-    ] + INSTALL_PYTHON_REQUIRES,
+        "setuptools>=36.2",
+        "twilio>=8.2.0",
+        "djangorestframework>=3.12.4",
+    ]
+    + INSTALL_PYTHON_REQUIRES,
     extras_require={
         "dev": ["check-manifest"],
     },
-
 )
```

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/management/commands/fake_data_seeder.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/management/commands/fake_data_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/management/commands/form_seeder.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/management/commands/form_seeder.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,18 @@
                 form=form,
                 order=qi + 1,
                 text=q["question"],
                 type=getattr(QuestionTypes, q["type"]),
                 required=q.get("required"),
             )
         else:
-            question.order = q.get("order")
+            if "order" in q:
+                question.order = q["order"]
+            else:
+                question.order = qi + 1
             question.text = q["question"]
             question.type = getattr(QuestionTypes, q["type"])
             question.required = q.get("required")
             question.save()
         if q.get("options"):
             QO.objects.filter(question=question).all().delete()
             QO.objects.bulk_create(
```

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/migrations/0001_initial.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/models.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/models.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,31 +59,29 @@
         fd = self.data.first()
         self.answer = Answers.objects.filter(data=fd.id).first()
         self.answer_serializer = ListDataAnswerSerializer(instance=self.answer)
 
     def test_expected_fields_in_data(self):
         data = self.data_serializer.data
         self.assertCountEqual(
-            set(data.keys()),
-            set(
-                [
-                    "id",
-                    "name",
-                    "form",
-                    "geo",
-                    "phone",
-                    "status",
-                    "created",
-                    "updated",
-                ]
-            ),
+            list(data),
+            [
+                "id",
+                "name",
+                "form",
+                "geo",
+                "phone",
+                "status",
+                "created",
+                "updated",
+            ],
         )
 
     def test_expected_fields_in_answer(self):
         data = self.answer_serializer.data
-        self.assertCountEqual(set(data.keys()), set(["question", "value"]))
+        self.assertEqual(list(data), ["question", "value"])
         self.assertEqual(str(self.data.first()), self.data.first().name)
 
     def test_value_content_in_answer(self):
         data = self.answer_serializer.data
         self.assertEqual(data["value"], self.answer.name)
         self.assertEqual(str(self.answer), self.answer.data.name)
```

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 from AkvoDjangoFormGateway.models import AkvoGatewayForm as Forms
 from AkvoDjangoFormGateway.serializers import ListFormSerializer
 
 
 class ListFormSerializerTestCase(TestCase):
     def setUp(self):
         self.form_attributes = {
-            'id': 1,
-            'name': 'Form #1',
-            'description': 'Form #1 description',
+            "id": 1,
+            "name": "Form #1",
+            "description": "Form #1 description",
         }
         self.form = Forms.objects.create(**self.form_attributes)
         self.serializers = ListFormSerializer(instance=self.form)
 
     def test_contains_expected_fields(self):
         data = self.serializers.data
         self.assertCountEqual(
-            set(data.keys()), set(['id', 'name', 'description', 'version'])
+            set(data.keys()), set(["id", "name", "description", "version"])
         )
 
     def test_version_content(self):
         data = self.serializers.data
-        self.assertEqual(data['version'], self.form.version)
+        self.assertEqual(data["version"], self.form.version)
         self.assertEqual(str(self.form), self.form.name)
 
     def test_forms_api(self):
         res = self.client.get("/api/gateway/forms/1/?format=json")
         res = res.json()
-        self.assertEqual(res["name"], "Form #1")
+        self.assertEqual(
+            res,
+            {
+                "id": 1,
+                "name": "Form #1",
+                "description": "Form #1 description",
+                "version": 1,
+            },
+        )
```

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_init.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_init.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,14 +59,39 @@
                     f"Form Updated | {form.name} V{form.version}", output
                 )
         # RUN FAKE DATA SEEDER
         output = self.call_fake_data_seeder_command("-t", True)
         form = Forms.objects.get(name="Form Complaint")
         self.assertIn(output, form.name)
 
+    def test_updating_form(self):
+        out = StringIO()
+        err = StringIO()
+        first_version = "./backend/source/forms/1.json"
+        call_command(
+            "form_seeder",
+            "--file",
+            first_version,
+            stdout=out,
+            stderr=err,
+        )
+        self.assertEqual(out.getvalue(), "Form Created | Form Complaint V1\n")
+
+        out = StringIO()
+        err = StringIO()
+        second_version = "./backend/source/forms/1-update-test.json"
+        call_command(
+            "form_seeder",
+            "--file",
+            second_version,
+            stdout=out,
+            stderr=err,
+        )
+        self.assertEqual(out.getvalue(), "Form Updated | Form Complaint V2\n")
+
     def test_seeder_raises_command_error(self):
         invalid_json_file = "./backend/source/forms/invalid.json"
 
         # Redirect stdout and stderr to StringIO to capture the output
         out = StringIO()
         err = StringIO()
```

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway/utils/functions.py` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway/utils/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,20 @@
 )
 from AkvoDjangoFormGateway.constants import QuestionTypes, StatusTypes
 
 
 fake = Faker()
 
 
-def get_answer_value(answer: Answers, toString: bool = False):
+def get_answer_value(answer: Answers):
     if answer.question.type in [
         QuestionTypes.geo,
         QuestionTypes.option,
         QuestionTypes.multiple_option,
     ]:
-        # TODO: Remove if unecessary
-        # if toString:
-        #     if answer.options:
-        #         return "|".join([str(a) for a in answer.options])
-        #     return None
         return answer.options
     elif answer.question.type == QuestionTypes.number:
         return answer.value
     else:
         return answer.name
```

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/PKG-INFO` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.2/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt` & `AkvoDjangoFormGateway-0.0.3/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/AkvoDjangoFormGateway/__init__.py
 src/AkvoDjangoFormGateway/admin.py
 src/AkvoDjangoFormGateway/apps.py
 src/AkvoDjangoFormGateway/constants.py
+src/AkvoDjangoFormGateway/feed.py
 src/AkvoDjangoFormGateway/models.py
 src/AkvoDjangoFormGateway/serializers.py
 src/AkvoDjangoFormGateway/urls.py
 src/AkvoDjangoFormGateway/views.py
 src/AkvoDjangoFormGateway.egg-info/PKG-INFO
 src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
 src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
@@ -22,13 +23,17 @@
 src/AkvoDjangoFormGateway/management/commands/__init__.py
 src/AkvoDjangoFormGateway/management/commands/fake_data_seeder.py
 src/AkvoDjangoFormGateway/management/commands/form_seeder.py
 src/AkvoDjangoFormGateway/migrations/0001_initial.py
 src/AkvoDjangoFormGateway/migrations/__init__.py
 src/AkvoDjangoFormGateway/tests/__init__.py
 src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
+src/AkvoDjangoFormGateway/tests/tests_env.py
 src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
 src/AkvoDjangoFormGateway/tests/tests_init.py
 src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
 src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
+src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
+src/AkvoDjangoFormGateway/tests/tests_validation.py
 src/AkvoDjangoFormGateway/utils/__init__.py
-src/AkvoDjangoFormGateway/utils/functions.py
+src/AkvoDjangoFormGateway/utils/functions.py
+src/AkvoDjangoFormGateway/utils/validation.py
```

