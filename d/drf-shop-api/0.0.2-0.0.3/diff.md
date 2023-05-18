# Comparing `tmp/drf_shop_api-0.0.2.tar.gz` & `tmp/drf_shop_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_shop_api-0.0.2.tar", max compression
+gzip compressed data, was "drf_shop_api-0.0.3.tar", max compression
```

## Comparing `drf_shop_api-0.0.2.tar` & `drf_shop_api-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     3060 2023-05-16 08:05:31.955824 drf_shop_api-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-18 12:58:19.167199 drf_shop_api-0.0.2/drf_shop_api/__init__.py
--rw-r--r--   0        0        0     2003 2023-05-16 07:14:02.635612 drf_shop_api-0.0.2/drf_shop_api/abstract_models.py
--rw-r--r--   0        0        0     4476 2023-05-17 13:30:50.707985 drf_shop_api-0.0.2/drf_shop_api/admin.py
--rw-r--r--   0        0        0      151 2023-05-02 06:11:20.327034 drf_shop_api-0.0.2/drf_shop_api/apps.py
--rw-r--r--   0        0        0        0 2023-04-21 05:04:18.787953 drf_shop_api-0.0.2/drf_shop_api/customers/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-02 06:09:39.859540 drf_shop_api-0.0.2/drf_shop_api/customers/filters.py
--rw-r--r--   0        0        0     1919 2023-05-17 13:31:21.619254 drf_shop_api-0.0.2/drf_shop_api/customers/models.py
--rw-r--r--   0        0        0     4586 2023-05-17 13:32:46.291563 drf_shop_api-0.0.2/drf_shop_api/customers/serializers.py
--rw-r--r--   0        0        0    11443 2023-05-17 13:29:55.510681 drf_shop_api-0.0.2/drf_shop_api/customers/tests.py
--rw-r--r--   0        0        0      742 2023-05-17 13:23:30.248336 drf_shop_api-0.0.2/drf_shop_api/customers/urls.py
--rw-r--r--   0        0        0     6595 2023-05-17 13:21:18.774078 drf_shop_api-0.0.2/drf_shop_api/customers/views.py
--rw-r--r--   0        0        0      537 2023-05-16 05:52:21.374090 drf_shop_api-0.0.2/drf_shop_api/decorators.py
--rw-r--r--   0        0        0        0 2023-05-17 13:43:27.864812 drf_shop_api-0.0.2/drf_shop_api/migrations/.gitignore
--rw-r--r--   0        0        0        0 2023-04-18 12:58:19.170967 drf_shop_api-0.0.2/drf_shop_api/migrations/__init__.py
--rw-r--r--   0        0        0     1800 2023-05-16 11:42:24.294850 drf_shop_api-0.0.2/drf_shop_api/models.py
--rw-r--r--   0        0        0        0 2023-04-21 07:03:32.137480 drf_shop_api-0.0.2/drf_shop_api/orders/__init__.py
--rw-r--r--   0        0        0      328 2023-05-16 08:12:07.125840 drf_shop_api-0.0.2/drf_shop_api/orders/constants.py
--rw-r--r--   0        0        0        0 2023-05-02 05:45:04.690248 drf_shop_api-0.0.2/drf_shop_api/orders/filters.py
--rw-r--r--   0        0        0     2119 2023-05-16 11:44:39.145565 drf_shop_api-0.0.2/drf_shop_api/orders/models.py
--rw-r--r--   0        0        0     4212 2023-05-16 13:22:57.000875 drf_shop_api-0.0.2/drf_shop_api/orders/serializers.py
--rw-r--r--   0        0        0     3365 2023-05-16 09:33:08.141979 drf_shop_api-0.0.2/drf_shop_api/orders/tests.py
--rw-r--r--   0        0        0      236 2023-05-02 06:09:55.984725 drf_shop_api-0.0.2/drf_shop_api/orders/urls.py
--rw-r--r--   0        0        0      142 2023-05-16 09:41:43.338239 drf_shop_api-0.0.2/drf_shop_api/orders/utils.py
--rw-r--r--   0        0        0     2227 2023-05-16 12:44:19.399851 drf_shop_api-0.0.2/drf_shop_api/orders/views.py
--rw-r--r--   0        0        0      692 2023-04-28 08:02:54.619717 drf_shop_api-0.0.2/drf_shop_api/paginators.py
--rw-r--r--   0        0        0     2271 2023-04-28 09:57:02.058215 drf_shop_api-0.0.2/drf_shop_api/permissions.py
--rw-r--r--   0        0        0        0 2023-04-19 12:14:02.155874 drf_shop_api-0.0.2/drf_shop_api/products/__init__.py
--rw-r--r--   0        0        0      208 2023-05-01 14:26:40.198927 drf_shop_api-0.0.2/drf_shop_api/products/constants.py
--rw-r--r--   0        0        0     1155 2023-05-02 06:09:55.334922 drf_shop_api-0.0.2/drf_shop_api/products/filters.py
--rw-r--r--   0        0        0     2839 2023-05-16 11:55:54.791725 drf_shop_api-0.0.2/drf_shop_api/products/models.py
--rw-r--r--   0        0        0     2637 2023-05-17 11:45:51.736626 drf_shop_api-0.0.2/drf_shop_api/products/serializers.py
--rw-r--r--   0        0        0     7877 2023-05-16 11:59:24.701138 drf_shop_api-0.0.2/drf_shop_api/products/tests.py
--rw-r--r--   0        0        0      435 2023-05-16 05:40:10.692883 drf_shop_api-0.0.2/drf_shop_api/products/urls.py
--rw-r--r--   0        0        0        0 2023-04-21 09:52:46.128283 drf_shop_api-0.0.2/drf_shop_api/products/utils.py
--rw-r--r--   0        0        0     3491 2023-05-02 06:09:28.026351 drf_shop_api-0.0.2/drf_shop_api/products/views.py
--rw-r--r--   0        0        0     2397 2023-05-08 05:14:56.407108 drf_shop_api-0.0.2/drf_shop_api/serializers.py
--rw-r--r--   0        0        0        0 2023-04-19 12:27:36.021705 drf_shop_api-0.0.2/drf_shop_api/tasks.py
--rw-r--r--   0        0        0     1055 2023-05-02 08:30:25.003346 drf_shop_api-0.0.2/drf_shop_api/tests.py
--rw-r--r--   0        0        0      305 2023-05-02 06:12:22.345106 drf_shop_api-0.0.2/drf_shop_api/urls.py
--rw-r--r--   0        0        0     3629 2023-05-17 13:12:43.981890 drf_shop_api-0.0.2/drf_shop_api/utils.py
--rw-r--r--   0        0        0       27 2023-04-19 12:27:10.142562 drf_shop_api-0.0.2/drf_shop_api/views.py
--rw-r--r--   0        0        0      598 2023-05-17 13:44:55.819900 drf_shop_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 drf_shop_api-0.0.2/setup.py
--rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 drf_shop_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2044 2023-05-18 04:36:26.946153 drf_shop_api-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 12:58:19.167199 drf_shop_api-0.0.3/drf_shop_api/__init__.py
+-rw-r--r--   0        0        0     2003 2023-05-16 07:14:02.635612 drf_shop_api-0.0.3/drf_shop_api/abstract_models.py
+-rw-r--r--   0        0        0     4476 2023-05-17 13:30:50.707985 drf_shop_api-0.0.3/drf_shop_api/admin.py
+-rw-r--r--   0        0        0      151 2023-05-02 06:11:20.327034 drf_shop_api-0.0.3/drf_shop_api/apps.py
+-rw-r--r--   0        0        0        0 2023-04-21 05:04:18.787953 drf_shop_api-0.0.3/drf_shop_api/customers/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-02 06:09:39.859540 drf_shop_api-0.0.3/drf_shop_api/customers/filters.py
+-rw-r--r--   0        0        0     1919 2023-05-17 13:31:21.619254 drf_shop_api-0.0.3/drf_shop_api/customers/models.py
+-rw-r--r--   0        0        0     4586 2023-05-17 13:32:46.291563 drf_shop_api-0.0.3/drf_shop_api/customers/serializers.py
+-rw-r--r--   0        0        0    11443 2023-05-17 13:29:55.510681 drf_shop_api-0.0.3/drf_shop_api/customers/tests.py
+-rw-r--r--   0        0        0      742 2023-05-17 13:23:30.248336 drf_shop_api-0.0.3/drf_shop_api/customers/urls.py
+-rw-r--r--   0        0        0     6595 2023-05-17 13:21:18.774078 drf_shop_api-0.0.3/drf_shop_api/customers/views.py
+-rw-r--r--   0        0        0      537 2023-05-16 05:52:21.374090 drf_shop_api-0.0.3/drf_shop_api/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:43:27.864812 drf_shop_api-0.0.3/drf_shop_api/migrations/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-18 12:58:19.170967 drf_shop_api-0.0.3/drf_shop_api/migrations/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-16 11:42:24.294850 drf_shop_api-0.0.3/drf_shop_api/models.py
+-rw-r--r--   0        0        0        0 2023-04-21 07:03:32.137480 drf_shop_api-0.0.3/drf_shop_api/orders/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-16 08:12:07.125840 drf_shop_api-0.0.3/drf_shop_api/orders/constants.py
+-rw-r--r--   0        0        0        0 2023-05-02 05:45:04.690248 drf_shop_api-0.0.3/drf_shop_api/orders/filters.py
+-rw-r--r--   0        0        0     2119 2023-05-16 11:44:39.145565 drf_shop_api-0.0.3/drf_shop_api/orders/models.py
+-rw-r--r--   0        0        0     4212 2023-05-16 13:22:57.000875 drf_shop_api-0.0.3/drf_shop_api/orders/serializers.py
+-rw-r--r--   0        0        0     3365 2023-05-16 09:33:08.141979 drf_shop_api-0.0.3/drf_shop_api/orders/tests.py
+-rw-r--r--   0        0        0      236 2023-05-02 06:09:55.984725 drf_shop_api-0.0.3/drf_shop_api/orders/urls.py
+-rw-r--r--   0        0        0      142 2023-05-16 09:41:43.338239 drf_shop_api-0.0.3/drf_shop_api/orders/utils.py
+-rw-r--r--   0        0        0     2227 2023-05-16 12:44:19.399851 drf_shop_api-0.0.3/drf_shop_api/orders/views.py
+-rw-r--r--   0        0        0      692 2023-04-28 08:02:54.619717 drf_shop_api-0.0.3/drf_shop_api/paginators.py
+-rw-r--r--   0        0        0     2271 2023-04-28 09:57:02.058215 drf_shop_api-0.0.3/drf_shop_api/permissions.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:14:02.155874 drf_shop_api-0.0.3/drf_shop_api/products/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-01 14:26:40.198927 drf_shop_api-0.0.3/drf_shop_api/products/constants.py
+-rw-r--r--   0        0        0     1155 2023-05-02 06:09:55.334922 drf_shop_api-0.0.3/drf_shop_api/products/filters.py
+-rw-r--r--   0        0        0     2839 2023-05-16 11:55:54.791725 drf_shop_api-0.0.3/drf_shop_api/products/models.py
+-rw-r--r--   0        0        0     2637 2023-05-17 11:45:51.736626 drf_shop_api-0.0.3/drf_shop_api/products/serializers.py
+-rw-r--r--   0        0        0     7877 2023-05-16 11:59:24.701138 drf_shop_api-0.0.3/drf_shop_api/products/tests.py
+-rw-r--r--   0        0        0      435 2023-05-16 05:40:10.692883 drf_shop_api-0.0.3/drf_shop_api/products/urls.py
+-rw-r--r--   0        0        0        0 2023-04-21 09:52:46.128283 drf_shop_api-0.0.3/drf_shop_api/products/utils.py
+-rw-r--r--   0        0        0     3491 2023-05-02 06:09:28.026351 drf_shop_api-0.0.3/drf_shop_api/products/views.py
+-rw-r--r--   0        0        0     2397 2023-05-08 05:14:56.407108 drf_shop_api-0.0.3/drf_shop_api/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:27:36.021705 drf_shop_api-0.0.3/drf_shop_api/tasks.py
+-rw-r--r--   0        0        0     1055 2023-05-02 08:30:25.003346 drf_shop_api-0.0.3/drf_shop_api/tests.py
+-rw-r--r--   0        0        0      305 2023-05-02 06:12:22.345106 drf_shop_api-0.0.3/drf_shop_api/urls.py
+-rw-r--r--   0        0        0     3629 2023-05-17 13:12:43.981890 drf_shop_api-0.0.3/drf_shop_api/utils.py
+-rw-r--r--   0        0        0       27 2023-04-19 12:27:10.142562 drf_shop_api-0.0.3/drf_shop_api/views.py
+-rw-r--r--   0        0        0      598 2023-05-18 04:36:32.764260 drf_shop_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 drf_shop_api-0.0.3/setup.py
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 drf_shop_api-0.0.3/PKG-INFO
```

### Comparing `drf_shop_api-0.0.2/README.md` & `drf_shop_api-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-# Features
-
-Features:
+Metadata-Version: 2.1
+Name: drf-shop-api
+Version: 0.0.3
+Summary: Standalone shop app, that you can add to your project
+Author: Oleksandr Korol
+Author-email: oleksandr.korol@coaxsoft.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=4.2.1,<5.0.0)
+Requires-Dist: django-filter (>=23.2,<24.0)
+Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: drf-yasg (>=1.21.5,<2.0.0)
+Requires-Dist: rest-framework-simplejwt (>=0.0.2,<0.0.3)
+Description-Content-Type: text/markdown
 
-- products (multiple images + main image, title, description, etc.)
-- products categories (parent/child categories)
-- product dynamic stats (for filtering like on Rozetka, ek.ua)
-- product comments
-- wish lists
-- cart
-- compare lists
-- orders
-- order reports (+ ability to generate pdf)
-- history
-- contact online support via web-sockets (or offline via email)
-- connect implemented payment systems
-- shipment
-- taxes
-- bonuses wallet
-- search for products/categories
-- filter for products in the category
-- statuses of buy / payment / shipment
+# Features
 
 Features:
 
 - Products
   - products (multiple images + main image, title, description, etc.)
   - products categories (parent/child categories)
-  - product dynamic stats (for filtering like on Rozetka, ek.ua)
+  - product dynamic stats
   - product comments
   - search for products/categories
   - filter for products in the category
 - Customers
   - wish lists
   - cart
   - compare lists
   - bonuses wallet
+  - customer support request
 - Settings
   - taxes
   - currencies
 - Orders
   - orders
   - order reports (view and generation of pdf)
   - shipping
@@ -89,41 +85,19 @@
         user.save(using=self._db)
         return user
 ```
 
 - Setup `AUTH_USER_MODEL` in settings.py
 
 - Run `python manage.py makemigrations` and `python manage.py migrate` (Due to optional Payment model from root project)
-
-## Features overview
-
-### Customers
-
-This app will hold User related data:
-
-`CustomerCart`
-`CustomerWishList`
-`CustomerBonusWallet`
-`CustomerOrderHistory`
-
-## Settings requirements
-
-- DRF settings
-
-```json
-"DEFAULT_AUTHENTICATION_CLASSES": ("rest_framework_simplejwt.authentication.JWTAuthentication",)
-```
-
-- DRF_SHOP settings:
-  - DRF_SHOP_PAGE_SIZE on will be default 10
-  - DRF_SHOP_PAYMENT_MODEL = "projects.payments.models.Payment"
-  - DRF_SHOP_PAYMENT_STATUS_CHOICES = "project.payments.choices.PaymentStatus"
-  - DRF_SHOP_BONUS_RATE = percentage value for each order that will go to bonus wallet
-
-> Statuses should be aligned as regular flow then cancel followed by refund
+- Optional settings:
+  - `DRF_SHOP_PAGE_SIZE` on will be default 10
+  - `DRF_SHOP_PAYMENT_MODEL` = "projects.payments.models.Payment"
+  - `DRF_SHOP_PAYMENT_STATUS_CHOICES` = "project.payments.choices.PaymentStatus"
+  - `DRF_SHOP_BONUS_RATE` = percentage value for each order that will go to bonus wallet
 
 ## Dependencies
 
     django
     drf
     drf-yasg 1.21.5
     rest_framework_simplejwt
@@ -131,8 +105,8 @@
     django-filter
 
 ### TODO
 
 - Add DB indexes
 - Task for currency rate update
 - Review permissions
-- Add custom migration to create all related model for auth user model
+
```

### Comparing `drf_shop_api-0.0.2/drf_shop_api/abstract_models.py` & `drf_shop_api-0.0.3/drf_shop_api/abstract_models.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/admin.py` & `drf_shop_api-0.0.3/drf_shop_api/admin.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/customers/filters.py` & `drf_shop_api-0.0.3/drf_shop_api/customers/filters.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/customers/models.py` & `drf_shop_api-0.0.3/drf_shop_api/customers/models.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/customers/serializers.py` & `drf_shop_api-0.0.3/drf_shop_api/customers/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/customers/tests.py` & `drf_shop_api-0.0.3/drf_shop_api/customers/tests.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/customers/urls.py` & `drf_shop_api-0.0.3/drf_shop_api/customers/urls.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/customers/views.py` & `drf_shop_api-0.0.3/drf_shop_api/customers/views.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/decorators.py` & `drf_shop_api-0.0.3/drf_shop_api/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/models.py` & `drf_shop_api-0.0.3/drf_shop_api/models.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/orders/models.py` & `drf_shop_api-0.0.3/drf_shop_api/orders/models.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/orders/serializers.py` & `drf_shop_api-0.0.3/drf_shop_api/orders/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/orders/tests.py` & `drf_shop_api-0.0.3/drf_shop_api/orders/tests.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/orders/views.py` & `drf_shop_api-0.0.3/drf_shop_api/orders/views.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/paginators.py` & `drf_shop_api-0.0.3/drf_shop_api/paginators.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/permissions.py` & `drf_shop_api-0.0.3/drf_shop_api/permissions.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/products/filters.py` & `drf_shop_api-0.0.3/drf_shop_api/products/filters.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/products/models.py` & `drf_shop_api-0.0.3/drf_shop_api/products/models.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/products/serializers.py` & `drf_shop_api-0.0.3/drf_shop_api/products/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/products/tests.py` & `drf_shop_api-0.0.3/drf_shop_api/products/tests.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/products/views.py` & `drf_shop_api-0.0.3/drf_shop_api/products/views.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/serializers.py` & `drf_shop_api-0.0.3/drf_shop_api/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/tests.py` & `drf_shop_api-0.0.3/drf_shop_api/tests.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/drf_shop_api/utils.py` & `drf_shop_api-0.0.3/drf_shop_api/utils.py`

 * *Files identical despite different names*

### Comparing `drf_shop_api-0.0.2/pyproject.toml` & `drf_shop_api-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-shop-api"
-version = "0.0.2"
+version = "0.0.3"
 description = "Standalone shop app, that you can add to your project"
 authors = ["Oleksandr Korol <oleksandr.korol@coaxsoft.com>"]
 readme = "README.md"
 packages = [{include = "drf_shop_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

