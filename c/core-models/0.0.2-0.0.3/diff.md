# Comparing `tmp/core_models-0.0.2.tar.gz` & `tmp/core_models-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_models-0.0.2.tar", last modified: Wed May 17 06:55:23 2023, max compression
+gzip compressed data, was "core_models-0.0.3.tar", last modified: Thu May 18 15:50:45 2023, max compression
```

## Comparing `core_models-0.0.2.tar` & `core_models-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.698734 core_models-0.0.2/
--rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.0.2/LICENSE
--rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-17 06:55:23.698529 core_models-0.0.2/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     6234 2023-04-18 09:31:52.000000 core_models-0.0.2/README.md
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.688338 core_models-0.0.2/core_models/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.0.2/core_models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.0.2/core_models/api_response.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.690275 core_models-0.0.2/core_models/app/
--rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.0.2/core_models/app/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     9301 2023-05-12 19:47:36.000000 core_models-0.0.2/core_models/app/admin.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.0.2/core_models/app/apps.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.0.2/core_models/app/context_processors.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.690726 core_models-0.0.2/core_models/app/managers/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.0.2/core_models/app/managers/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2844 2023-05-01 17:47:00.000000 core_models-0.0.2/core_models/app/managers/notification_manager.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.693442 core_models-0.0.2/core_models/app/migrations/
--rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.0.2/core_models/app/migrations/0001_initial.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.0.2/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.0.2/core_models/app/migrations/0003_alter_user_onboarding_stage.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.0.2/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.0.2/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.0.2/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.0.2/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.0.2/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.0.2/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.0.2/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.0.2/core_models/app/migrations/__init__.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.696984 core_models-0.0.2/core_models/app/models/
--rw-r--r--   0 macbookpro   (501) staff       (20)      365 2023-04-28 12:03:37.000000 core_models-0.0.2/core_models/app/models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-04-26 06:22:29.000000 core_models-0.0.2/core_models/app/models/bank_account.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1189 2023-05-01 18:18:35.000000 core_models-0.0.2/core_models/app/models/base.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2046 2023-04-28 12:37:27.000000 core_models-0.0.2/core_models/app/models/company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      514 2023-04-28 11:34:04.000000 core_models-0.0.2/core_models/app/models/configuration.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2727 2023-05-01 17:53:25.000000 core_models-0.0.2/core_models/app/models/contract.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.0.2/core_models/app/models/currency.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     3280 2023-05-13 01:34:48.000000 core_models-0.0.2/core_models/app/models/invoice.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      464 2023-04-26 12:59:06.000000 core_models-0.0.2/core_models/app/models/notification.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      867 2023-04-26 23:25:11.000000 core_models-0.0.2/core_models/app/models/transaction.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1654 2023-04-30 21:58:23.000000 core_models-0.0.2/core_models/app/models/user.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.697587 core_models-0.0.2/core_models/app/templates/
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.698191 core_models-0.0.2/core_models/app/templates/core_models/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    15388 2023-05-12 10:38:46.000000 core_models-0.0.2/core_models/app/templates/core_models/mail-base.html
--rw-r--r--   0 macbookpro   (501) staff       (20)      696 2023-04-29 21:56:01.000000 core_models-0.0.2/core_models/app/templates/core_models/mail-base.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)    15204 2023-04-29 13:48:29.000000 core_models-0.0.2/core_models/app/templates/invoice.html
--rw-r--r--   0 macbookpro   (501) staff       (20)    12372 2023-04-29 13:43:51.000000 core_models-0.0.2/core_models/app/templates/reset.html
--rw-r--r--   0 macbookpro   (501) staff       (20)     3022 2023-05-11 22:07:09.000000 core_models-0.0.2/core_models/base_views.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2062 2023-05-12 21:33:33.000000 core_models-0.0.2/core_models/constants.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.0.2/core_models/settings.example.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     7013 2023-05-12 10:38:46.000000 core_models-0.0.2/core_models/settings.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 core_models-0.0.2/core_models/utils.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-17 06:55:23.689280 core_models-0.0.2/core_models.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-17 06:55:23.000000 core_models-0.0.2/core_models.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     1979 2023-05-17 06:55:23.000000 core_models-0.0.2/core_models.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-05-17 06:55:23.000000 core_models-0.0.2/core_models.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      145 2023-05-17 06:55:23.000000 core_models-0.0.2/core_models.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       12 2023-05-17 06:55:23.000000 core_models-0.0.2/core_models.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.0.2/pyproject.toml
--rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-05-17 06:55:23.698801 core_models-0.0.2/setup.cfg
--rw-r--r--   0 macbookpro   (501) staff       (20)     1176 2023-05-17 06:55:16.000000 core_models-0.0.2/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.135768 core_models-0.0.3/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.0.3/LICENSE
+-rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-18 15:50:45.135490 core_models-0.0.3/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6234 2023-04-18 09:31:52.000000 core_models-0.0.3/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.121894 core_models-0.0.3/core_models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.0.3/core_models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.0.3/core_models/api_response.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.124780 core_models-0.0.3/core_models/app/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.0.3/core_models/app/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     9301 2023-05-12 19:47:36.000000 core_models-0.0.3/core_models/app/admin.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.0.3/core_models/app/apps.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.0.3/core_models/app/context_processors.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.125495 core_models-0.0.3/core_models/app/managers/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.0.3/core_models/app/managers/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2844 2023-05-01 17:47:00.000000 core_models-0.0.3/core_models/app/managers/notification_manager.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.129037 core_models-0.0.3/core_models/app/migrations/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.0.3/core_models/app/migrations/0001_initial.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.0.3/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.0.3/core_models/app/migrations/0003_alter_user_onboarding_stage.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.0.3/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.0.3/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.0.3/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.0.3/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.0.3/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.0.3/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.0.3/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.0.3/core_models/app/migrations/__init__.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.133415 core_models-0.0.3/core_models/app/models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      365 2023-04-28 12:03:37.000000 core_models-0.0.3/core_models/app/models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-04-26 06:22:29.000000 core_models-0.0.3/core_models/app/models/bank_account.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1189 2023-05-01 18:18:35.000000 core_models-0.0.3/core_models/app/models/base.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2046 2023-04-28 12:37:27.000000 core_models-0.0.3/core_models/app/models/company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      514 2023-04-28 11:34:04.000000 core_models-0.0.3/core_models/app/models/configuration.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2727 2023-05-01 17:53:25.000000 core_models-0.0.3/core_models/app/models/contract.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.0.3/core_models/app/models/currency.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3280 2023-05-13 01:34:48.000000 core_models-0.0.3/core_models/app/models/invoice.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      464 2023-04-26 12:59:06.000000 core_models-0.0.3/core_models/app/models/notification.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      867 2023-04-26 23:25:11.000000 core_models-0.0.3/core_models/app/models/transaction.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1654 2023-04-30 21:58:23.000000 core_models-0.0.3/core_models/app/models/user.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.134278 core_models-0.0.3/core_models/app/templates/
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.134925 core_models-0.0.3/core_models/app/templates/core_models/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    15388 2023-05-12 10:38:46.000000 core_models-0.0.3/core_models/app/templates/core_models/mail-base.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)      696 2023-04-29 21:56:01.000000 core_models-0.0.3/core_models/app/templates/core_models/mail-base.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)    15204 2023-04-29 13:48:29.000000 core_models-0.0.3/core_models/app/templates/invoice.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)    12372 2023-04-29 13:43:51.000000 core_models-0.0.3/core_models/app/templates/reset.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3022 2023-05-11 22:07:09.000000 core_models-0.0.3/core_models/base_views.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2062 2023-05-12 21:33:33.000000 core_models-0.0.3/core_models/constants.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.0.3/core_models/settings.example.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     7460 2023-05-18 14:06:25.000000 core_models-0.0.3/core_models/settings.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 core_models-0.0.3/core_models/utils.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 15:50:45.123273 core_models-0.0.3/core_models.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-18 15:50:45.000000 core_models-0.0.3/core_models.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1979 2023-05-18 15:50:45.000000 core_models-0.0.3/core_models.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-05-18 15:50:45.000000 core_models-0.0.3/core_models.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      161 2023-05-18 15:50:45.000000 core_models-0.0.3/core_models.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       12 2023-05-18 15:50:45.000000 core_models-0.0.3/core_models.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.0.3/pyproject.toml
+-rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-05-18 15:50:45.135825 core_models-0.0.3/setup.cfg
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1195 2023-05-18 15:50:29.000000 core_models-0.0.3/setup.py
```

### Comparing `core_models-0.0.2/LICENSE` & `core_models-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/README.md` & `core_models-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/api_response.py` & `core_models-0.0.3/core_models/api_response.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/admin.py` & `core_models-0.0.3/core_models/app/admin.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/managers/notification_manager.py` & `core_models-0.0.3/core_models/app/managers/notification_manager.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0001_initial.py` & `core_models-0.0.3/core_models/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py` & `core_models-0.0.3/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py` & `core_models-0.0.3/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py` & `core_models-0.0.3/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py` & `core_models-0.0.3/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py` & `core_models-0.0.3/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py` & `core_models-0.0.3/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py` & `core_models-0.0.3/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py` & `core_models-0.0.3/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/models/base.py` & `core_models-0.0.3/core_models/app/models/base.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/models/company.py` & `core_models-0.0.3/core_models/app/models/company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/models/configuration.py` & `core_models-0.0.3/core_models/app/models/configuration.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/models/contract.py` & `core_models-0.0.3/core_models/app/models/contract.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/models/currency.py` & `core_models-0.0.3/core_models/app/models/currency.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/models/invoice.py` & `core_models-0.0.3/core_models/app/models/invoice.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/models/transaction.py` & `core_models-0.0.3/core_models/app/models/transaction.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/models/user.py` & `core_models-0.0.3/core_models/app/models/user.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/templates/core_models/mail-base.html` & `core_models-0.0.3/core_models/app/templates/core_models/mail-base.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/templates/core_models/mail-base.txt` & `core_models-0.0.3/core_models/app/templates/core_models/mail-base.txt`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/templates/invoice.html` & `core_models-0.0.3/core_models/app/templates/invoice.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/app/templates/reset.html` & `core_models-0.0.3/core_models/app/templates/reset.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/base_views.py` & `core_models-0.0.3/core_models/base_views.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/constants.py` & `core_models-0.0.3/core_models/constants.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/settings.example.py` & `core_models-0.0.3/core_models/settings.example.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models/settings.py` & `core_models-0.0.3/core_models/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os, sys
+import dj_database_url
 
 from dotenv import load_dotenv
 from datetime import timedelta
 
 from pathlib import Path
 
 PACKAGE_DIR = Path(__file__).resolve().parent
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 load_dotenv()
 
 AUTH_USER_MODEL = 'app.User'
 
-SECRET_KEY = 'da)(@*#Uhubjindu*(!@#$#@nfoinond-ahp*nen2@=*u)!g8m9pthdg'
+SECRET_KEY = os.getenv("SECRET_KEY")
 
 INSTALLED_APPS = ['daphne']
 
 CORE_APPS = [
     'storages',
     'cities_light',
     'django_slack',
@@ -42,15 +43,19 @@
         'default': {
             'ENGINE': "django.db.backends.sqlite3",
             'NAME': "test.db"
         }
     }
 else:
     DATABASES = {
-        'default': {
+        'default': dj_database_url.config(
+            default=db("DB_URL"),
+            conn_max_age=600,
+            conn_health_checks=True,
+        ) if db("DB_URL") else {
             'ENGINE': db("DB_ENGINE"),
             'NAME': db('POSTGRES_DB'),
             'USER': db('POSTGRES_USER'),
             'PASSWORD': db('POSTGRES_PASSWORD'),
             'HOST': db('DB_HOST'),
             'PORT': db('DB_PORT'),
         }
@@ -242,14 +247,15 @@
 
 if FILE_UPLOAD_STORAGE == "local":
     MEDIA_ROOT_NAME = "media"
     MEDIA_ROOT = os.path.join(BASE_DIR, MEDIA_ROOT_NAME)
     MEDIA_URL = f"/{MEDIA_ROOT_NAME}/"
 
 if FILE_UPLOAD_STORAGE == "s3":
+    STATICFILES_STORAGE = 'storages.backends.s3boto3.S3StaticStorage'
     # Using django-storages
     # https://django-storages.readthedocs.io/en/latest/backends/amazon-S3.html
     DEFAULT_FILE_STORAGE = 'storages.backends.s3boto3.S3Boto3Storage'
 
     AWS_AUTO_CREATE_BUCKET = True
     AWS_S3_ACCESS_KEY_ID = get_env("AWS_S3_ACCESS_KEY_ID")
     AWS_S3_SECRET_ACCESS_KEY = get_env("AWS_S3_SECRET_ACCESS_KEY")
@@ -257,7 +263,13 @@
     AWS_S3_REGION_NAME = get_env("AWS_S3_REGION_NAME")
     AWS_S3_SIGNATURE_VERSION = get_env("AWS_S3_SIGNATURE_VERSION", default="s3v4")
 
     # https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl
     AWS_DEFAULT_ACL = get_env("AWS_DEFAULT_ACL", default="public-read")
 
     AWS_PRESIGNED_EXPIRY = int(get_env("AWS_PRESIGNED_EXPIRY", default='10'))  # seconds
+
+if FILE_UPLOAD_STORAGE == "gcloud":
+    DEFAULT_FILE_STORAGE = 'storages.backends.gcloud.GoogleCloudStorage'
+    GS_BUCKET_NAME = 'YOUR_BUCKET_NAME_GOES_HERE'
+    STATICFILES_STORAGE = 'storages.backends.gcloud.GoogleCloudStorage'
+
```

### Comparing `core_models-0.0.2/core_models/utils.py` & `core_models-0.0.3/core_models/utils.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/core_models.egg-info/SOURCES.txt` & `core_models-0.0.3/core_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_models-0.0.2/setup.py` & `core_models-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Liquify core package'
 LONG_DESCRIPTION = 'Package that holds all models and core ' \
                    'functions/classes of Liquify project'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
@@ -15,15 +15,15 @@
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     package_data={'': ['app/templates/core_models/*']},
     include_package_data=True,
     install_requires=["django", "python-dotenv", "django-safedelete", "redis",
                       "onesignal-sdk", "django-cities-light", 'daphne', 'psycopg2-binary',
-                      "django-slack", "uvicorn", "django-storages", "boto3"],
+                      "django-slack", "uvicorn", "django-storages", "boto3", 'dj-database-url'],
     # add any
     # additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=['python', 'liquify'],
     classifiers=[
         "Programming Language :: Python :: 3",
```

