# Comparing `tmp/django-plans-1.0.4.tar.gz` & `tmp/django-plans-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plans-1.0.4.tar", last modified: Thu May 18 09:54:09 2023, max compression
+gzip compressed data, was "django-plans-1.0.5.tar", last modified: Thu May 18 09:56:53 2023, max compression
```

## Comparing `django-plans-1.0.4.tar` & `django-plans-1.0.5.tar`

### file list

```diff
@@ -1,285 +1,286 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.378397 django-plans-1.0.4/
--rw-rw-r--   0 petr      (1000) petr      (1000)      653 2023-05-18 09:54:08.000000 django-plans-1.0.4/.coveragerc
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.346397 django-plans-1.0.4/.github/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.354397 django-plans-1.0.4/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4211 2023-05-18 09:54:08.000000 django-plans-1.0.4/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      343 2023-05-18 09:54:08.000000 django-plans-1.0.4/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      616 2023-05-18 09:54:08.000000 django-plans-1.0.4/.travis.yml
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.354397 django-plans-1.0.4/.tx/
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-05-18 09:54:08.000000 django-plans-1.0.4/.tx/config
--rw-rw-r--   0 petr      (1000) petr      (1000)       83 2023-05-18 09:54:08.000000 django-plans-1.0.4/AUTHORS
--rw-rw-r--   0 petr      (1000) petr      (1000)     5365 2023-05-18 09:54:08.000000 django-plans-1.0.4/CHANGELOG
--rw-rw-r--   0 petr      (1000) petr      (1000)     3215 2023-05-18 09:54:08.000000 django-plans-1.0.4/CODE_OF_CONDUCT.md
--rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2023-05-18 09:54:08.000000 django-plans-1.0.4/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-05-18 09:54:08.000000 django-plans-1.0.4/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1709 2023-05-18 09:54:09.378397 django-plans-1.0.4/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     1061 2023-05-18 09:54:08.000000 django-plans-1.0.4/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1617 2023-05-18 09:54:08.000000 django-plans-1.0.4/conftest.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.354397 django-plans-1.0.4/demo/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.354397 django-plans-1.0.4/demo/example/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.354397 django-plans-1.0.4/demo/example/foo/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.354397 django-plans-1.0.4/demo/example/foo/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)     7641 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/fixtures/initial_data.json
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/forms.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/foo/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)      821 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      279 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/foo/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/foo/templates/foo/
--rw-rw-r--   0 petr      (1000) petr      (1000)      591 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/templates/foo/foo_confirm_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/templates/foo/foo_form.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1044 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/templates/foo/foo_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      383 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      402 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      323 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/validators.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1483 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/foo/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/locale/en/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/locale/en/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      378 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      714 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/locale/pl/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      603 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      904 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/locale/pt_BR/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      495 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      804 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/locale/ru/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      549 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      858 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/sample_plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      160 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      233 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      190 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/sample_plans/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      693 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/fixtures/initial_plan.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/fixtures/test_django-plans_auth.json
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/fixtures/test_django-plans_default_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     9864 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/fixtures/test_django-plans_plans.json
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/sample_plans/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/sample_plans/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      119 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/management/commands/autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      117 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/management/commands/create_userplans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      116 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/management/commands/expire_accounts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.358397 django-plans-1.0.4/demo/example/sample_plans/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)    30868 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2041 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/sample_plans/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.362397 django-plans-1.0.4/demo/example/sample_plans/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/change_plan_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/change_plan_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      573 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/expired_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/expired_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/extend_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      145 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/extend_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      511 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/invoice_created_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      225 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/invoice_created_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/remind_expire_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/mail/remind_expire_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.362397 django-plans-1.0.4/demo/example/sample_plans/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      668 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/account_activation.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      305 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      653 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/billing_info_create.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      835 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/billing_info_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      744 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/billing_info_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/create_order.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/current.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/expiration_messages.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/extend.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/fake_payments.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.362397 django-plans-1.0.4/demo/example/sample_plans/templates/plans/invoices/
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/invoices/PL_EN.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/invoices/invoice_base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/order_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/order_detail_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/order_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      846 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/pagination.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     5465 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/plan_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      176 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/pricing.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/templates/plans/upgrade.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2272 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/sample_plans/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5573 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.362397 django-plans-1.0.4/demo/example/static/css/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3961 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/static/css/example.css
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/demo/example/static/img/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.362397 django-plans-1.0.4/demo/example/static/img/messages/
--rw-rw-r--   0 petr      (1000) petr      (1000)      294 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/static/img/messages/icon_alert.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     3668 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/static/img/messages/icon_error.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     3675 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/static/img/messages/icon_success.png
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.362397 django-plans-1.0.4/demo/example/templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)     2746 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/templates/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      823 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/templates/home.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.362397 django-plans-1.0.4/demo/example/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)       25 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      757 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/templates/plans/billing_info_create.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      882 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/templates/plans/billing_info_update.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.362397 django-plans-1.0.4/demo/example/templates/registration/
--rw-rw-r--   0 petr      (1000) petr      (1000)      718 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/templates/registration/login.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      566 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1131 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/example/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      323 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/fabfile.py
--rwxrwxr-x   0 petr      (1000) petr      (1000)      813 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2023-05-18 09:54:08.000000 django-plans-1.0.4/demo/requirements.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.366397 django-plans-1.0.4/django_plans.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1709 2023-05-18 09:54:09.000000 django-plans-1.0.4/django_plans.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     8358 2023-05-18 09:54:09.000000 django-plans-1.0.4/django_plans.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-05-18 09:54:09.000000 django-plans-1.0.4/django_plans.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-05-18 09:54:09.000000 django-plans-1.0.4/django_plans.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-05-18 09:54:09.000000 django-plans-1.0.4/django_plans.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2023-05-18 09:54:09.000000 django-plans-1.0.4/django_plans.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.366397 django-plans-1.0.4/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     5597 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/Makefile
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.366397 django-plans-1.0.4/docs/source/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/docs/source/_static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.366397 django-plans-1.0.4/docs/source/_static/images/
--rw-rw-r--   0 petr      (1000) petr      (1000)   176623 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/_static/images/django-plans-1.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   193693 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/_static/images/django-plans-2.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   146667 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/_static/images/django-plans-3.png
--rw-rw-r--   0 petr      (1000) petr      (1000)      860 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/caveats.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     7913 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1217 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/customize_models.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1668 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2386 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1966 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/integration.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2588 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/invoicing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6661 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/plans.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/plans_change.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      847 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/plans_expiration.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2246 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/plans_recurrence.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     5248 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/quota_validators.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     9824 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/settings.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2388 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/south.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1583 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/taxation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2302 2023-05-18 09:54:08.000000 django-plans-1.0.4/docs/source/templating.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      296 2023-05-18 09:54:08.000000 django-plans-1.0.4/fabfile.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     8399 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      277 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/base/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/base/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    42514 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/base/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      319 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1262 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/context_processors.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2418 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/contrib.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1688 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/enumeration.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      678 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/fixtures/initial_plan.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/fixtures/test_django-plans_auth.json
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/fixtures/test_django-plans_default_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     9479 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/fixtures/test_django-plans_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     2101 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/forms.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/importer.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2284 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/listeners.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/plans/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/plans/locale/en/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/locale/en/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    15215 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/plans/locale/pl/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    10111 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    15132 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/plans/locale/pt_BR/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4374 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    16542 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/plans/locale/ru/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    11843 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    15021 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.370397 django-plans-1.0.4/plans/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      892 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/management/commands/autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      417 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/management/commands/create_userplans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      291 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/management/commands/expire_accounts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.374397 django-plans-1.0.4/plans/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)    13851 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      733 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0002_auto_20180901_1744.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1403 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0003_make_plans_unique.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      503 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0004_create_user_plans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2679 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0005_recurring_payments.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      603 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0006_auto_20200504_1541.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0007_recurringuserplan_card_masked_number.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      563 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0008_recurringuserplan_token_verified.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      457 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0009_auto_20210303_1134.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2561 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0010_auto_20220113_1317.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4916 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0011_auto_20220208_1344.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      469 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/0012_planpricing_visible.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      486 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/mixins.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1985 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3544 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/plan_change.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      307 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/quota.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1721 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/signals.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1995 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.374397 django-plans-1.0.4/plans/taxation/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1266 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/taxation/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     6066 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/taxation/eu.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      529 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/taxation/ru.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.350397 django-plans-1.0.4/plans/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.374397 django-plans-1.0.4/plans/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/change_plan_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/change_plan_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      573 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/expired_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/expired_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/extend_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      145 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/extend_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      511 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/invoice_created_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      225 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/invoice_created_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/remind_expire_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/mail/remind_expire_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.378397 django-plans-1.0.4/plans/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      668 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/account_activation.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      305 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      835 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/billing_info_create_or_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/billing_info_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/create_order.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/current.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/expiration_messages.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/extend.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/fake_payments.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.378397 django-plans-1.0.4/plans/templates/plans/invoices/
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/invoices/PL_EN.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/invoices/PL_EN_layout.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/invoices/invoice_base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/order_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/order_detail_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/order_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      846 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/pagination.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     5599 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/plan_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      176 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/pricing.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/templates/plans/upgrade.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.378397 django-plans-1.0.4/plans/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)       29 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     7224 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    46249 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/tests/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2233 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1296 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5748 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/validators.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    18540 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:09.378397 django-plans-1.0.4/plans_i18n/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1427 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans_i18n/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans_i18n/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      815 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans_i18n/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       65 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans_i18n/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      383 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans_i18n/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      743 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans_i18n/translation.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       26 2023-05-18 09:54:08.000000 django-plans-1.0.4/plans_i18n/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      350 2023-05-18 09:54:09.378397 django-plans-1.0.4/setup.cfg
--rw-rw-r--   0 petr      (1000) petr      (1000)     1330 2023-05-18 09:54:08.000000 django-plans-1.0.4/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      624 2023-05-18 09:54:08.000000 django-plans-1.0.4/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.733781 django-plans-1.0.5/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      653 2023-05-18 09:56:53.000000 django-plans-1.0.5/.coveragerc
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.701782 django-plans-1.0.5/.github/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4394 2023-05-18 09:56:53.000000 django-plans-1.0.5/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      343 2023-05-18 09:56:53.000000 django-plans-1.0.5/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      616 2023-05-18 09:56:53.000000 django-plans-1.0.5/.travis.yml
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/.tx/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-05-18 09:56:53.000000 django-plans-1.0.5/.tx/config
+-rw-rw-r--   0 petr      (1000) petr      (1000)       83 2023-05-18 09:56:53.000000 django-plans-1.0.5/AUTHORS
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5364 2023-05-18 09:56:53.000000 django-plans-1.0.5/CHANGELOG
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3215 2023-05-18 09:56:53.000000 django-plans-1.0.5/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2023-05-18 09:56:53.000000 django-plans-1.0.5/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-05-18 09:56:53.000000 django-plans-1.0.5/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1709 2023-05-18 09:56:53.733781 django-plans-1.0.5/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1061 2023-05-18 09:56:53.000000 django-plans-1.0.5/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1617 2023-05-18 09:56:53.000000 django-plans-1.0.5/conftest.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/demo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/demo/example/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/demo/example/foo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/demo/example/foo/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7641 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/fixtures/initial_data.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/forms.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/demo/example/foo/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1128 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      279 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.701782 django-plans-1.0.5/demo/example/foo/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/demo/example/foo/templates/foo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      591 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/templates/foo/foo_confirm_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/templates/foo/foo_form.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1044 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/templates/foo/foo_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      383 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      402 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      323 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/validators.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1530 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/foo/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/demo/example/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.701782 django-plans-1.0.5/demo/example/locale/en/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/demo/example/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      378 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      714 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.701782 django-plans-1.0.5/demo/example/locale/pl/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.709782 django-plans-1.0.5/demo/example/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      603 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      904 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/demo/example/locale/pt_BR/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.713781 django-plans-1.0.5/demo/example/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      495 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      804 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/demo/example/locale/ru/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.713781 django-plans-1.0.5/demo/example/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      549 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      858 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.713781 django-plans-1.0.5/demo/example/sample_plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      160 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      190 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.713781 django-plans-1.0.5/demo/example/sample_plans/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      693 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/fixtures/initial_plan.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/fixtures/test_django-plans_auth.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/fixtures/test_django-plans_default_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9864 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/fixtures/test_django-plans_plans.json
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.713781 django-plans-1.0.5/demo/example/sample_plans/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.713781 django-plans-1.0.5/demo/example/sample_plans/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      119 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/management/commands/autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      117 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/management/commands/create_userplans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      116 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/management/commands/expire_accounts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.713781 django-plans-1.0.5/demo/example/sample_plans/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    30867 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1960 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/demo/example/sample_plans/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.713781 django-plans-1.0.5/demo/example/sample_plans/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/change_plan_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/change_plan_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      573 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/expired_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/expired_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/extend_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      145 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/extend_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      511 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/invoice_created_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      225 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/invoice_created_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/remind_expire_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/mail/remind_expire_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/demo/example/sample_plans/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      668 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/account_activation.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      305 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      653 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/billing_info_create.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      835 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      429 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/billing_info_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      744 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/billing_info_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/create_order.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/current.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/expiration_messages.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/extend.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/fake_payments.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/demo/example/sample_plans/templates/plans/invoices/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/invoices/PL_EN.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/invoices/invoice_base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/order_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/order_detail_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/order_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      846 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/pagination.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5465 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/plan_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      176 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/pricing.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/templates/plans/upgrade.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2239 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/sample_plans/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5544 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/demo/example/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/demo/example/static/css/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3961 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/static/css/example.css
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/demo/example/static/img/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/demo/example/static/img/messages/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      294 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/static/img/messages/icon_alert.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3668 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/static/img/messages/icon_error.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3675 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/static/img/messages/icon_success.png
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/demo/example/templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2746 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/templates/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      823 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/templates/home.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/demo/example/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      757 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/templates/plans/billing_info_create.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      882 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/templates/plans/billing_info_update.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/demo/example/templates/registration/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      718 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/templates/registration/login.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      605 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1131 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/example/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      323 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/fabfile.py
+-rwxrwxr-x   0 petr      (1000) petr      (1000)      813 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2023-05-18 09:56:53.000000 django-plans-1.0.5/demo/requirements.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/django_plans.egg-info/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1709 2023-05-18 09:56:53.000000 django-plans-1.0.5/django_plans.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8397 2023-05-18 09:56:53.000000 django-plans-1.0.5/django_plans.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-05-18 09:56:53.000000 django-plans-1.0.5/django_plans.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-05-18 09:56:53.000000 django-plans-1.0.5/django_plans.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-05-18 09:56:53.000000 django-plans-1.0.5/django_plans.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2023-05-18 09:56:53.000000 django-plans-1.0.5/django_plans.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.717782 django-plans-1.0.5/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5597 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/Makefile
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.721782 django-plans-1.0.5/docs/source/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/docs/source/_static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.721782 django-plans-1.0.5/docs/source/_static/images/
+-rw-rw-r--   0 petr      (1000) petr      (1000)   176623 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/_static/images/django-plans-1.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   193693 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/_static/images/django-plans-2.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   146667 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/_static/images/django-plans-3.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)      860 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/caveats.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8032 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1217 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/customize_models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1668 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2316 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1966 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/integration.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2588 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/invoicing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6661 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/plans.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/plans_change.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      847 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/plans_expiration.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2246 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/plans_recurrence.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5248 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/quota_validators.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9824 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/settings.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2388 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/south.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1583 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/taxation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2302 2023-05-18 09:56:53.000000 django-plans-1.0.5/docs/source/templating.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      296 2023-05-18 09:56:53.000000 django-plans-1.0.5/fabfile.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8840 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      277 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/base/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/base/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    44890 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/base/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      273 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1299 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/context_processors.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2488 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/contrib.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1686 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/enumeration.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      678 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/fixtures/initial_plan.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/fixtures/test_django-plans_auth.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/fixtures/test_django-plans_default_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9479 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/fixtures/test_django-plans_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2127 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/forms.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      351 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/importer.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2273 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/listeners.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/plans/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/plans/locale/en/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15215 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/plans/locale/pl/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    10111 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15132 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/plans/locale/pt_BR/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4374 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    16542 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/plans/locale/ru/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    11843 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15021 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.725782 django-plans-1.0.5/plans/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      930 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/management/commands/autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      417 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/management/commands/create_userplans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      291 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/management/commands/expire_accounts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.729781 django-plans-1.0.5/plans/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    22268 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      890 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0002_auto_20180901_1744.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1481 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0003_make_plans_unique.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      480 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0004_create_user_plans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4417 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0005_recurring_payments.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      665 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0006_auto_20200504_1541.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0007_recurringuserplan_card_masked_number.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      625 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0008_recurringuserplan_token_verified.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      456 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0009_auto_20210303_1134.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2715 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0010_auto_20220113_1317.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5735 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0011_auto_20220208_1344.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      531 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/0012_planpricing_visible.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/mixins.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1903 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3643 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/plan_change.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      308 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/quota.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1721 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/signals.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2079 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.729781 django-plans-1.0.5/plans/taxation/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1266 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/taxation/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6207 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/taxation/eu.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/taxation/ru.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.705782 django-plans-1.0.5/plans/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.729781 django-plans-1.0.5/plans/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/change_plan_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/change_plan_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      573 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/expired_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/expired_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/extend_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      145 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/extend_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      511 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/invoice_created_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      225 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/invoice_created_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/remind_expire_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/mail/remind_expire_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.729781 django-plans-1.0.5/plans/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      668 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/account_activation.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      305 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      835 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/billing_info_create_or_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      429 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/billing_info_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/create_order.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/current.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/expiration_messages.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/extend.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/fake_payments.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.729781 django-plans-1.0.5/plans/templates/plans/invoices/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/invoices/PL_EN.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/invoices/PL_EN_layout.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/invoices/invoice_base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/order_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/order_detail_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/order_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      846 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/pagination.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5599 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/plan_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      176 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/pricing.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/templates/plans/upgrade.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.733781 django-plans-1.0.5/plans/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       29 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2213 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/tests/test_autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7224 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    49156 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/tests/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2375 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1316 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/utils.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5946 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/validators.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    19429 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.733781 django-plans-1.0.5/plans_i18n/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1427 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans_i18n/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans_i18n/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      815 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans_i18n/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       65 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans_i18n/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      383 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans_i18n/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      764 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans_i18n/translation.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       26 2023-05-18 09:56:53.000000 django-plans-1.0.5/plans_i18n/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      371 2023-05-18 09:56:53.733781 django-plans-1.0.5/setup.cfg
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1329 2023-05-18 09:56:53.000000 django-plans-1.0.5/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      624 2023-05-18 09:56:53.000000 django-plans-1.0.5/tox.ini
```

### Comparing `django-plans-1.0.4/.coveragerc` & `django-plans-1.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/.github/workflows/main.yml` & `django-plans-1.0.5/.github/workflows/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,19 @@
   # This workflow contains a single job called "build"
   tests:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        DJANGO_VERSION: [ '2.2.*', '3.0.*', '3.1.*', '3.2.*', '4.0.*', '4.1.*' ]
+        DJANGO_VERSION: [ '2.2.*', '3.0.*', '3.1.*', '3.2.*', '4.0.*', '4.1.*', '4.2.*' ]
         python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
         exclude:
+          - DJANGO_VERSION: '4.2.*'
+            python-version: '3.7'
           - DJANGO_VERSION: '4.1.*'
             python-version: '3.7'
           - DJANGO_VERSION: '4.0.*'
             python-version: '3.7'
           - DJANGO_VERSION: '3.1.*'
             python-version: '3.10'
           - DJANGO_VERSION: '3.0.*'
@@ -94,15 +96,15 @@
               }
 
       - name: Testing
         run: |
           # Run tests for sample app used for testing extensibility
           PYTHONPATH="." MANAGE_PY_PATH="demo/manage.py" SAMPLE_APP=1 demo/manage.py test example
           case "${{ matrix.DJANGO_VERSION }},${{ matrix.python-version }}" in
-            2.2.*,3.7|3.0.*,3.7|3.1.*,3.7)  # Django runs with warnings in this python version
+            2.2.*,3.7|3.0.*,3.7|3.1.*,3.7|3.2.*,3.7|4.0.*,3.8|4.0.*,3.9|4.0.*,3.10)  # Django runs with warnings in this python version
               PYTHONPATH="." MANAGE_PY_PATH="demo/manage.py" coverage run demo/manage.py test plans
               ;;
             *)
               PYTHONPATH="." MANAGE_PY_PATH="demo/manage.py" PYTHONWARNINGS="error::DeprecationWarning" coverage run demo/manage.py test plans
               ;;
           esac
           coverage xml && codecov
@@ -110,12 +112,14 @@
           POSTGRES_HOST: postgres
           POSTGRES_PORT: 5432
   lint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Install
-        run: pip install flake8 isort
+        run: pip install flake8 isort black
       - name: Running Flake8
         run: flake8
       - name: Running isort
         run: isort
+      - name: Running black
+        run: black --check .
```

### Comparing `django-plans-1.0.4/.travis.yml` & `django-plans-1.0.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/CHANGELOG` & `django-plans-1.0.5/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 django-plans changelog
 ======================
 
-1.0.4
+1.0.5
 -----
 * Re-use old RecurringUserPlan in set_plan_renewal() to retain ID and history
 * `autorenew_accounts` management command: better output, --providers option
 * Blackify whole source
 
-
 1.0.3
 -----
 * Prevent duplicated invoice creation when concurrent Order.complete_order() are callled
 * Test in Python 3.11
 
 1.0.2
 -----
@@ -41,15 +40,15 @@
 * UserPlans are now automatically created with initial migration or with `create_userplans` adminaction.
 * Added possibility to define `PLANS_APP_VERBOSE_NAME` to personalize plans' `verbose_name`
 * Return back to order after setting up billing info
 
 0.8.13
 ------
 * Supporting Django 2.0.6.
-1.0.4 (unreleased)
+1.0.5 (unreleased)
 * New VAT standard rates 2017
 * Remove dependency on `django.contrib.sites`.
 * Feature #53: Cleaner and more explicit exception handling on `Plan.get_default_plan `.
 * Feature #59: Adding code coverage to code base.
 * Support customised user models by using `django.contrib.auth.get_user_model()`.
 * Add Database migrations.
```

### Comparing `django-plans-1.0.4/CODE_OF_CONDUCT.md` & `django-plans-1.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/LICENSE` & `django-plans-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/PKG-INFO` & `django-plans-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans
-Version: 1.0.4
+Version: 1.0.5
 Summary: Pluggable django app for managing pricing plans with quotas and accounts expiration
 Home-page: https://github.com/cypreess/django-plans
 Author: Krzysztof Dorosz
 Author-email: cypreess@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
```

### Comparing `django-plans-1.0.4/README.rst` & `django-plans-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/conftest.py` & `django-plans-1.0.5/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import os
 import sys
 from decimal import Decimal
 
 from django.conf import settings
 
-sys.path[:0] = [os.path.join(os.getcwd(), 'demo')]
+sys.path[:0] = [os.path.join(os.getcwd(), "demo")]
 
 
 def pytest_configure(config):
     settings.configure(
-        DATABASE_ENGINE='sqlite3',
+        DATABASE_ENGINE="sqlite3",
         DATABASES={
-            'default': {
-                'NAME': ':memory:',
-                'ENGINE': 'django.db.backends.sqlite3',
-                'TEST_NAME': ':memory:',
+            "default": {
+                "NAME": ":memory:",
+                "ENGINE": "django.db.backends.sqlite3",
+                "TEST_NAME": ":memory:",
             },
         },
-        DATABASE_NAME=':memory:',
-        TEST_DATABASE_NAME=':memory:',
+        DATABASE_NAME=":memory:",
+        TEST_DATABASE_NAME=":memory:",
         INSTALLED_APPS=[
-            'django.contrib.auth',
-            'django.contrib.contenttypes',
-            'django.contrib.admin',
-            'django.contrib.sessions',
-            'django.contrib.sites',
-            'ordered_model',
-            'example.foo',
-            'plans',
+            "django.contrib.auth",
+            "django.contrib.contenttypes",
+            "django.contrib.admin",
+            "django.contrib.sessions",
+            "django.contrib.sites",
+            "ordered_model",
+            "example.foo",
+            "plans",
         ],
-        ROOT_URLCONF='example.urls',
+        ROOT_URLCONF="example.urls",
         DEBUG=False,
         SITE_ID=1,
         TEMPLATE_DEBUG=True,
         USE_TZ=True,
-        ALLOWED_HOSTS=['*'],
+        ALLOWED_HOSTS=["*"],
         PLANS_INVOICE_ISSUER={
             "issuer_name": "My Company Ltd",
             "issuer_street": "48th Suny street",
             "issuer_zipcode": "111-456",
             "issuer_city": "Django City",
             "issuer_country": "PL",
             "issuer_tax_number": "PL123456789",
         },
         PLANS_TAX=Decimal(23.0),
-        PLANS_TAXATION_POLICY='plans.taxation.eu.EUTaxationPolicy',
-        PLANS_TAX_COUNTRY='PL',
-        PLANS_CURRENCY='PLN',
+        PLANS_TAXATION_POLICY="plans.taxation.eu.EUTaxationPolicy",
+        PLANS_TAX_COUNTRY="PL",
+        PLANS_CURRENCY="PLN",
         PLANS_VALIDATORS={
-            'MAX_FOO_COUNT': 'example.foo.validators.max_foos_validator',
+            "MAX_FOO_COUNT": "example.foo.validators.max_foos_validator",
         },
-        EMAIL_BACKEND='django.core.mail.backends.console.EmailBackend',
+        EMAIL_BACKEND="django.core.mail.backends.console.EmailBackend",
     )
```

### Comparing `django-plans-1.0.4/demo/example/foo/fixtures/initial_data.json` & `django-plans-1.0.5/demo/example/foo/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/foo/templates/foo/foo_confirm_delete.html` & `django-plans-1.0.5/demo/example/foo/templates/foo/foo_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/foo/templates/foo/foo_form.html` & `django-plans-1.0.5/demo/example/foo/templates/foo/foo_form.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/foo/templates/foo/foo_list.html` & `django-plans-1.0.5/demo/example/foo/templates/foo/foo_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/foo/views.py` & `django-plans-1.0.5/demo/example/foo/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,32 +19,35 @@
 
 class FooCreateView(CreateView):
     model = Foo
     form_class = FooForm
 
     def get_initial(self):
         initial = super(FooCreateView, self).get_initial()
-        initial['user'] = self.request.user
+        initial["user"] = self.request.user
         return initial
 
     def get_success_url(self):
-        return reverse('foo_list')
+        return reverse("foo_list")
 
     def get_queryset(self):
         return super(FooCreateView, self).get_queryset().filter(user=self.request.user)
 
 
 class FooDeleteView(DeleteView):
     model = Foo
 
     def get_queryset(self):
         return super(FooDeleteView, self).get_queryset().filter(user=self.request.user)
 
     def get_success_url(self):
-        return reverse('foo_list')
+        return reverse("foo_list")
 
     def delete(self, request, *args, **kwargs):
-        if not get_user_quota(request.user).get('CAN_DELETE_FOO', True):
-            messages.error(request, 'Sorry, your plan does not allow to deletes Foo. Please upgrade!')
-            return redirect('foo_del', pk=self.get_object().pk)
+        if not get_user_quota(request.user).get("CAN_DELETE_FOO", True):
+            messages.error(
+                request,
+                "Sorry, your plan does not allow to deletes Foo. Please upgrade!",
+            )
+            return redirect("foo_del", pk=self.get_object().pk)
         else:
             return super(FooDeleteView, self).delete(request, *args, **kwargs)
```

### Comparing `django-plans-1.0.4/demo/example/locale/en/LC_MESSAGES/django.po` & `django-plans-1.0.5/demo/example/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/locale/pl/LC_MESSAGES/django.mo` & `django-plans-1.0.5/demo/example/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/locale/pl/LC_MESSAGES/django.po` & `django-plans-1.0.5/demo/example/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/locale/pt_BR/LC_MESSAGES/django.po` & `django-plans-1.0.5/demo/example/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/locale/ru/LC_MESSAGES/django.mo` & `django-plans-1.0.5/demo/example/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/locale/ru/LC_MESSAGES/django.po` & `django-plans-1.0.5/demo/example/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/fixtures/initial_plan.json` & `django-plans-1.0.5/demo/example/sample_plans/fixtures/initial_plan.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/fixtures/test_django-plans_auth.json` & `django-plans-1.0.5/demo/example/sample_plans/fixtures/test_django-plans_auth.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/fixtures/test_django-plans_plans.json` & `django-plans-1.0.5/demo/example/sample_plans/fixtures/test_django-plans_plans.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/migrations/0001_initial.py` & `django-plans-1.0.5/demo/example/sample_plans/migrations/0001_initial.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,851 +8,850 @@
 from django.conf import settings
 from django.db import migrations, models
 
 import plans.base.models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='Plan',
+            name="Plan",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
                 (
-                    'order',
+                    "order",
                     models.PositiveIntegerField(
-                        db_index=True, editable=False, verbose_name='order'
+                        db_index=True, editable=False, verbose_name="order"
                     ),
                 ),
-                ('name', models.CharField(max_length=100, verbose_name='name')),
+                ("name", models.CharField(max_length=100, verbose_name="name")),
                 (
-                    'description',
-                    models.TextField(blank=True, verbose_name='description'),
+                    "description",
+                    models.TextField(blank=True, verbose_name="description"),
                 ),
                 (
-                    'available',
+                    "available",
                     models.BooleanField(
                         db_index=True,
                         default=False,
-                        help_text='Is still available for purchase',
-                        verbose_name='available',
+                        help_text="Is still available for purchase",
+                        verbose_name="available",
                     ),
                 ),
                 (
-                    'visible',
+                    "visible",
                     models.BooleanField(
                         db_index=True,
                         default=True,
-                        help_text='Is visible in current offer',
-                        verbose_name='visible',
+                        help_text="Is visible in current offer",
+                        verbose_name="visible",
                     ),
                 ),
                 (
-                    'created',
-                    models.DateTimeField(db_index=True, verbose_name='created'),
+                    "created",
+                    models.DateTimeField(db_index=True, verbose_name="created"),
                 ),
                 (
-                    'url',
+                    "url",
                     models.URLField(
                         blank=True,
-                        help_text='Optional link to page with more information (for clickable pricing table headers)',
+                        help_text="Optional link to page with more information (for clickable pricing table headers)",
                     ),
                 ),
                 (
-                    'default',
+                    "default",
                     models.BooleanField(
                         blank=True,
                         default=None,
                         help_text='Both "Unknown" and "No" means that the plan is not default',
                         null=True,
                     ),
                 ),
                 (
-                    'customized',
+                    "customized",
                     models.ForeignKey(
                         blank=True,
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         to=settings.AUTH_USER_MODEL,
-                        verbose_name='customized',
+                        verbose_name="customized",
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'Plan',
-                'verbose_name_plural': 'Plans',
-                'ordering': ('order',),
-                'abstract': False,
+                "verbose_name": "Plan",
+                "verbose_name_plural": "Plans",
+                "ordering": ("order",),
+                "abstract": False,
             },
             bases=(plans.base.models.BaseMixin, models.Model),
         ),
         migrations.CreateModel(
-            name='Pricing',
+            name="Pricing",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
-                ('name', models.CharField(max_length=100, verbose_name='name')),
+                ("name", models.CharField(max_length=100, verbose_name="name")),
                 (
-                    'period',
+                    "period",
                     models.PositiveIntegerField(
                         blank=True,
                         db_index=True,
                         default=30,
                         null=True,
-                        verbose_name='period',
+                        verbose_name="period",
                     ),
                 ),
                 (
-                    'url',
+                    "url",
                     models.URLField(
                         blank=True,
-                        help_text='Optional link to page with more information (for clickable pricing table headers)',
+                        help_text="Optional link to page with more information (for clickable pricing table headers)",
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'Pricing',
-                'verbose_name_plural': 'Pricings',
-                'ordering': ('period',),
-                'abstract': False,
+                "verbose_name": "Pricing",
+                "verbose_name_plural": "Pricings",
+                "ordering": ("period",),
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
         migrations.CreateModel(
-            name='Quota',
+            name="Quota",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
                 (
-                    'order',
+                    "order",
                     models.PositiveIntegerField(
-                        db_index=True, editable=False, verbose_name='order'
+                        db_index=True, editable=False, verbose_name="order"
                     ),
                 ),
                 (
-                    'codename',
+                    "codename",
                     models.CharField(
                         db_index=True,
                         max_length=50,
                         unique=True,
-                        verbose_name='codename',
+                        verbose_name="codename",
                     ),
                 ),
-                ('name', models.CharField(max_length=100, verbose_name='name')),
+                ("name", models.CharField(max_length=100, verbose_name="name")),
                 (
-                    'unit',
-                    models.CharField(blank=True, max_length=100, verbose_name='unit'),
+                    "unit",
+                    models.CharField(blank=True, max_length=100, verbose_name="unit"),
                 ),
                 (
-                    'description',
-                    models.TextField(blank=True, verbose_name='description'),
+                    "description",
+                    models.TextField(blank=True, verbose_name="description"),
                 ),
                 (
-                    'is_boolean',
-                    models.BooleanField(default=False, verbose_name='is boolean'),
+                    "is_boolean",
+                    models.BooleanField(default=False, verbose_name="is boolean"),
                 ),
                 (
-                    'url',
+                    "url",
                     models.CharField(
                         blank=True,
-                        help_text='Optional link to page with more information (for clickable pricing table headers)',
+                        help_text="Optional link to page with more information (for clickable pricing table headers)",
                         max_length=200,
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'Quota',
-                'verbose_name_plural': 'Quotas',
-                'ordering': ('order',),
-                'abstract': False,
+                "verbose_name": "Quota",
+                "verbose_name_plural": "Quotas",
+                "ordering": ("order",),
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
         migrations.CreateModel(
-            name='TestApp',
+            name="TestApp",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
             ],
             options={
-                'abstract': False,
+                "abstract": False,
             },
             bases=(example.sample_plans.models.DetailFieldMixin, models.Model),
         ),
         migrations.CreateModel(
-            name='UserPlan',
+            name="UserPlan",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
                 (
-                    'expire',
+                    "expire",
                     models.DateField(
                         blank=True,
                         db_index=True,
                         default=None,
                         null=True,
-                        verbose_name='expire',
+                        verbose_name="expire",
                     ),
                 ),
                 (
-                    'active',
+                    "active",
                     models.BooleanField(
-                        db_index=True, default=True, verbose_name='active'
+                        db_index=True, default=True, verbose_name="active"
                     ),
                 ),
                 (
-                    'plan',
+                    "plan",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
-                        to='sample_plans.plan',
-                        verbose_name='plan',
+                        to="sample_plans.plan",
+                        verbose_name="plan",
                     ),
                 ),
                 (
-                    'user',
+                    "user",
                     models.OneToOneField(
                         on_delete=django.db.models.deletion.CASCADE,
                         to=settings.AUTH_USER_MODEL,
-                        verbose_name='user',
+                        verbose_name="user",
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'User plan',
-                'verbose_name_plural': 'Users plans',
-                'abstract': False,
+                "verbose_name": "User plan",
+                "verbose_name_plural": "Users plans",
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
         migrations.CreateModel(
-            name='RecurringUserPlan',
+            name="RecurringUserPlan",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
                 (
-                    'token',
+                    "token",
                     models.CharField(
                         blank=True,
                         default=None,
-                        help_text='Token, that will be used for payment renewal. Depends on used payment provider',
+                        help_text="Token, that will be used for payment renewal. Depends on used payment provider",
                         max_length=255,
                         null=True,
-                        verbose_name='recurring token',
+                        verbose_name="recurring token",
                     ),
                 ),
                 (
-                    'payment_provider',
+                    "payment_provider",
                     models.CharField(
                         blank=True,
                         default=None,
-                        help_text='Provider, that will be used for payment renewal',
+                        help_text="Provider, that will be used for payment renewal",
                         max_length=255,
                         null=True,
-                        verbose_name='payment provider',
+                        verbose_name="payment provider",
                     ),
                 ),
                 (
-                    'amount',
+                    "amount",
                     models.DecimalField(
                         blank=True,
                         db_index=True,
                         decimal_places=2,
                         max_digits=7,
                         null=True,
-                        verbose_name='amount',
+                        verbose_name="amount",
                     ),
                 ),
                 (
-                    'tax',
+                    "tax",
                     models.DecimalField(
                         blank=True,
                         db_index=True,
                         decimal_places=2,
                         max_digits=4,
                         null=True,
-                        verbose_name='tax',
+                        verbose_name="tax",
                     ),
                 ),
-                ('currency', models.CharField(max_length=3, verbose_name='currency')),
+                ("currency", models.CharField(max_length=3, verbose_name="currency")),
                 (
-                    'has_automatic_renewal',
+                    "has_automatic_renewal",
                     models.BooleanField(
                         default=False,
-                        help_text='Automatic renewal is enabled for associated plan. If False, the plan renewal can be still initiated by user.',
-                        verbose_name='has automatic plan renewal',
+                        help_text="Automatic renewal is enabled for associated plan. If False, the plan renewal can be still initiated by user.",
+                        verbose_name="has automatic plan renewal",
                     ),
                 ),
                 (
-                    'token_verified',
+                    "token_verified",
                     models.BooleanField(
                         default=False,
-                        help_text='The recurring token has been verified by at least one payment to be working.',
-                        verbose_name='token has been verified by payment',
+                        help_text="The recurring token has been verified by at least one payment to be working.",
+                        verbose_name="token has been verified by payment",
                     ),
                 ),
-                ('card_expire_year', models.IntegerField(blank=True, null=True)),
-                ('card_expire_month', models.IntegerField(blank=True, null=True)),
+                ("card_expire_year", models.IntegerField(blank=True, null=True)),
+                ("card_expire_month", models.IntegerField(blank=True, null=True)),
                 (
-                    'card_masked_number',
+                    "card_masked_number",
                     models.CharField(blank=True, max_length=255, null=True),
                 ),
                 (
-                    'pricing',
+                    "pricing",
                     models.ForeignKey(
                         blank=True,
                         default=None,
-                        help_text='Recurring pricing',
+                        help_text="Recurring pricing",
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
-                        to='sample_plans.pricing',
+                        to="sample_plans.pricing",
                     ),
                 ),
                 (
-                    'user_plan',
+                    "user_plan",
                     models.OneToOneField(
                         on_delete=django.db.models.deletion.CASCADE,
-                        related_name='recurring',
-                        to='sample_plans.userplan',
+                        related_name="recurring",
+                        to="sample_plans.userplan",
                     ),
                 ),
             ],
             options={
-                'abstract': False,
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
         migrations.CreateModel(
-            name='PlanQuota',
+            name="PlanQuota",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
-                ('value', models.IntegerField(blank=True, default=1, null=True)),
+                ("value", models.IntegerField(blank=True, default=1, null=True)),
                 (
-                    'plan',
+                    "plan",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
-                        to='sample_plans.plan',
+                        to="sample_plans.plan",
                     ),
                 ),
                 (
-                    'quota',
+                    "quota",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
-                        to='sample_plans.quota',
+                        to="sample_plans.quota",
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'Plan quota',
-                'verbose_name_plural': 'Plans quotas',
-                'abstract': False,
+                "verbose_name": "Plan quota",
+                "verbose_name_plural": "Plans quotas",
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
         migrations.CreateModel(
-            name='PlanPricing',
+            name="PlanPricing",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
                 (
-                    'price',
+                    "price",
                     models.DecimalField(db_index=True, decimal_places=2, max_digits=7),
                 ),
-                ('order', models.IntegerField(default=0)),
+                ("order", models.IntegerField(default=0)),
                 (
-                    'has_automatic_renewal',
+                    "has_automatic_renewal",
                     models.BooleanField(
                         default=False,
-                        help_text='Use automatic renewal if possible?',
-                        verbose_name='has automatic renewal',
+                        help_text="Use automatic renewal if possible?",
+                        verbose_name="has automatic renewal",
                     ),
                 ),
                 (
-                    'plan',
+                    "plan",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
-                        to='sample_plans.plan',
+                        to="sample_plans.plan",
                     ),
                 ),
                 (
-                    'pricing',
+                    "pricing",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
-                        to='sample_plans.pricing',
+                        to="sample_plans.pricing",
                     ),
                 ),
                 (
-                    'visible',
+                    "visible",
                     models.BooleanField(
                         default=True,
-                        help_text='Is visible in current offer',
-                        verbose_name='is visible by default',
+                        help_text="Is visible in current offer",
+                        verbose_name="is visible by default",
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'Plan pricing',
-                'verbose_name_plural': 'Plans pricings',
-                'ordering': ('order', 'pricing__period'),
-                'abstract': False,
+                "verbose_name": "Plan pricing",
+                "verbose_name_plural": "Plans pricings",
+                "ordering": ("order", "pricing__period"),
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
         migrations.AddField(
-            model_name='plan',
-            name='quotas',
+            model_name="plan",
+            name="quotas",
             field=models.ManyToManyField(
-                through='sample_plans.PlanQuota', to='sample_plans.Quota'
+                through="sample_plans.PlanQuota", to="sample_plans.Quota"
             ),
         ),
         migrations.CreateModel(
-            name='Order',
+            name="Order",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
-                ('flat_name', models.CharField(blank=True, max_length=200, null=True)),
+                ("flat_name", models.CharField(blank=True, max_length=200, null=True)),
                 (
-                    'created',
-                    models.DateTimeField(db_index=True, verbose_name='created'),
+                    "created",
+                    models.DateTimeField(db_index=True, verbose_name="created"),
                 ),
                 (
-                    'completed',
+                    "completed",
                     models.DateTimeField(
-                        blank=True, db_index=True, null=True, verbose_name='completed'
+                        blank=True, db_index=True, null=True, verbose_name="completed"
                     ),
                 ),
                 (
-                    'plan_extended_from',
+                    "plan_extended_from",
                     models.DateField(
                         blank=True,
-                        help_text='The plan was extended from this date',
+                        help_text="The plan was extended from this date",
                         null=True,
-                        verbose_name='plan extended from',
+                        verbose_name="plan extended from",
                     ),
                 ),
                 (
-                    'plan_extended_until',
+                    "plan_extended_until",
                     models.DateField(
                         blank=True,
-                        help_text='The plan was extended until this date',
+                        help_text="The plan was extended until this date",
                         null=True,
-                        verbose_name='plan extended until',
+                        verbose_name="plan extended until",
                     ),
                 ),
                 (
-                    'amount',
+                    "amount",
                     models.DecimalField(
                         db_index=True,
                         decimal_places=2,
                         max_digits=7,
-                        verbose_name='amount',
+                        verbose_name="amount",
                     ),
                 ),
                 (
-                    'tax',
+                    "tax",
                     models.DecimalField(
                         blank=True,
                         db_index=True,
                         decimal_places=2,
                         max_digits=4,
                         null=True,
-                        verbose_name='tax',
+                        verbose_name="tax",
                     ),
                 ),
                 (
-                    'currency',
+                    "currency",
                     models.CharField(
-                        default='EUR', max_length=3, verbose_name='currency'
+                        default="EUR", max_length=3, verbose_name="currency"
                     ),
                 ),
                 (
-                    'status',
+                    "status",
                     models.IntegerField(
                         choices=[
-                            (1, 'new'),
-                            (2, 'completed'),
-                            (3, 'not valid'),
-                            (4, 'canceled'),
-                            (5, 'returned'),
+                            (1, "new"),
+                            (2, "completed"),
+                            (3, "not valid"),
+                            (4, "canceled"),
+                            (5, "returned"),
                         ],
                         default=1,
-                        verbose_name='status',
+                        verbose_name="status",
                     ),
                 ),
                 (
-                    'plan',
+                    "plan",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
-                        related_name='plan_order',
-                        to='sample_plans.plan',
-                        verbose_name='plan',
+                        related_name="plan_order",
+                        to="sample_plans.plan",
+                        verbose_name="plan",
                     ),
                 ),
                 (
-                    'pricing',
+                    "pricing",
                     models.ForeignKey(
                         blank=True,
                         null=True,
                         on_delete=django.db.models.deletion.CASCADE,
-                        to='sample_plans.pricing',
-                        verbose_name='pricing',
+                        to="sample_plans.pricing",
+                        verbose_name="pricing",
                     ),
                 ),
                 (
-                    'user',
+                    "user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         to=settings.AUTH_USER_MODEL,
-                        verbose_name='user',
+                        verbose_name="user",
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'Order',
-                'verbose_name_plural': 'Orders',
-                'ordering': ('-created',),
-                'abstract': False,
+                "verbose_name": "Order",
+                "verbose_name_plural": "Orders",
+                "ordering": ("-created",),
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
         migrations.CreateModel(
-            name='Invoice',
+            name="Invoice",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
-                ('number', models.IntegerField(db_index=True)),
-                ('full_number', models.CharField(max_length=200)),
+                ("number", models.IntegerField(db_index=True)),
+                ("full_number", models.CharField(max_length=200)),
                 (
-                    'type',
+                    "type",
                     models.IntegerField(
                         choices=[
-                            (1, 'Invoice'),
-                            (2, 'Invoice Duplicate'),
-                            (3, 'Order confirmation'),
+                            (1, "Invoice"),
+                            (2, "Invoice Duplicate"),
+                            (3, "Order confirmation"),
                         ],
                         db_index=True,
                         default=1,
                     ),
                 ),
-                ('issued', models.DateField(db_index=True)),
+                ("issued", models.DateField(db_index=True)),
                 (
-                    'issued_duplicate',
+                    "issued_duplicate",
                     models.DateField(blank=True, db_index=True, null=True),
                 ),
                 (
-                    'selling_date',
+                    "selling_date",
                     models.DateField(blank=True, db_index=True, null=True),
                 ),
-                ('payment_date', models.DateField(db_index=True)),
-                ('unit_price_net', models.DecimalField(decimal_places=2, max_digits=7)),
-                ('quantity', models.IntegerField(default=1)),
-                ('total_net', models.DecimalField(decimal_places=2, max_digits=7)),
-                ('total', models.DecimalField(decimal_places=2, max_digits=7)),
-                ('tax_total', models.DecimalField(decimal_places=2, max_digits=7)),
+                ("payment_date", models.DateField(db_index=True)),
+                ("unit_price_net", models.DecimalField(decimal_places=2, max_digits=7)),
+                ("quantity", models.IntegerField(default=1)),
+                ("total_net", models.DecimalField(decimal_places=2, max_digits=7)),
+                ("total", models.DecimalField(decimal_places=2, max_digits=7)),
+                ("tax_total", models.DecimalField(decimal_places=2, max_digits=7)),
                 (
-                    'tax',
+                    "tax",
                     models.DecimalField(
                         blank=True,
                         db_index=True,
                         decimal_places=2,
                         max_digits=4,
                         null=True,
                     ),
                 ),
                 (
-                    'rebate',
+                    "rebate",
                     models.DecimalField(
-                        decimal_places=2, default=Decimal('0'), max_digits=4
+                        decimal_places=2, default=Decimal("0"), max_digits=4
                     ),
                 ),
-                ('currency', models.CharField(default='EUR', max_length=3)),
-                ('item_description', models.CharField(max_length=200)),
-                ('buyer_name', models.CharField(max_length=200, verbose_name='Name')),
+                ("currency", models.CharField(default="EUR", max_length=3)),
+                ("item_description", models.CharField(max_length=200)),
+                ("buyer_name", models.CharField(max_length=200, verbose_name="Name")),
                 (
-                    'buyer_street',
-                    models.CharField(max_length=200, verbose_name='Street'),
+                    "buyer_street",
+                    models.CharField(max_length=200, verbose_name="Street"),
                 ),
                 (
-                    'buyer_zipcode',
-                    models.CharField(max_length=200, verbose_name='Zip code'),
+                    "buyer_zipcode",
+                    models.CharField(max_length=200, verbose_name="Zip code"),
                 ),
-                ('buyer_city', models.CharField(max_length=200, verbose_name='City')),
+                ("buyer_city", models.CharField(max_length=200, verbose_name="City")),
                 (
-                    'buyer_country',
+                    "buyer_country",
                     django_countries.fields.CountryField(
-                        default='PL', max_length=2, verbose_name='Country'
+                        default="PL", max_length=2, verbose_name="Country"
                     ),
                 ),
                 (
-                    'buyer_tax_number',
+                    "buyer_tax_number",
                     models.CharField(
-                        blank=True, max_length=200, verbose_name='TAX/VAT number'
+                        blank=True, max_length=200, verbose_name="TAX/VAT number"
                     ),
                 ),
                 (
-                    'shipping_name',
-                    models.CharField(max_length=200, verbose_name='Name'),
+                    "shipping_name",
+                    models.CharField(max_length=200, verbose_name="Name"),
                 ),
                 (
-                    'shipping_street',
-                    models.CharField(max_length=200, verbose_name='Street'),
+                    "shipping_street",
+                    models.CharField(max_length=200, verbose_name="Street"),
                 ),
                 (
-                    'shipping_zipcode',
-                    models.CharField(max_length=200, verbose_name='Zip code'),
+                    "shipping_zipcode",
+                    models.CharField(max_length=200, verbose_name="Zip code"),
                 ),
                 (
-                    'shipping_city',
-                    models.CharField(max_length=200, verbose_name='City'),
+                    "shipping_city",
+                    models.CharField(max_length=200, verbose_name="City"),
                 ),
                 (
-                    'shipping_country',
+                    "shipping_country",
                     django_countries.fields.CountryField(
-                        default='PL', max_length=2, verbose_name='Country'
+                        default="PL", max_length=2, verbose_name="Country"
                     ),
                 ),
-                ('require_shipment', models.BooleanField(db_index=True, default=False)),
-                ('issuer_name', models.CharField(max_length=200, verbose_name='Name')),
+                ("require_shipment", models.BooleanField(db_index=True, default=False)),
+                ("issuer_name", models.CharField(max_length=200, verbose_name="Name")),
                 (
-                    'issuer_street',
-                    models.CharField(max_length=200, verbose_name='Street'),
+                    "issuer_street",
+                    models.CharField(max_length=200, verbose_name="Street"),
                 ),
                 (
-                    'issuer_zipcode',
-                    models.CharField(max_length=200, verbose_name='Zip code'),
+                    "issuer_zipcode",
+                    models.CharField(max_length=200, verbose_name="Zip code"),
                 ),
-                ('issuer_city', models.CharField(max_length=200, verbose_name='City')),
+                ("issuer_city", models.CharField(max_length=200, verbose_name="City")),
                 (
-                    'issuer_country',
+                    "issuer_country",
                     django_countries.fields.CountryField(
-                        default='PL', max_length=2, verbose_name='Country'
+                        default="PL", max_length=2, verbose_name="Country"
                     ),
                 ),
                 (
-                    'issuer_tax_number',
+                    "issuer_tax_number",
                     models.CharField(
-                        blank=True, max_length=200, verbose_name='TAX/VAT number'
+                        blank=True, max_length=200, verbose_name="TAX/VAT number"
                     ),
                 ),
                 (
-                    'order',
+                    "order",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
-                        to='sample_plans.order',
-                        verbose_name='order',
+                        to="sample_plans.order",
+                        verbose_name="order",
                     ),
                 ),
                 (
-                    'user',
+                    "user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
                         to=settings.AUTH_USER_MODEL,
-                        verbose_name='user',
+                        verbose_name="user",
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'Invoice',
-                'verbose_name_plural': 'Invoices',
-                'abstract': False,
+                "verbose_name": "Invoice",
+                "verbose_name_plural": "Invoices",
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
         migrations.CreateModel(
-            name='BillingInfo',
+            name="BillingInfo",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
                 (
-                    'tax_number',
+                    "tax_number",
                     models.CharField(
-                        blank=True, db_index=True, max_length=200, verbose_name='VAT ID'
+                        blank=True, db_index=True, max_length=200, verbose_name="VAT ID"
                     ),
                 ),
                 (
-                    'name',
+                    "name",
                     models.CharField(
-                        db_index=True, max_length=200, verbose_name='name'
+                        db_index=True, max_length=200, verbose_name="name"
                     ),
                 ),
-                ('street', models.CharField(max_length=200, verbose_name='street')),
-                ('zipcode', models.CharField(max_length=200, verbose_name='zip code')),
-                ('city', models.CharField(max_length=200, verbose_name='city')),
+                ("street", models.CharField(max_length=200, verbose_name="street")),
+                ("zipcode", models.CharField(max_length=200, verbose_name="zip code")),
+                ("city", models.CharField(max_length=200, verbose_name="city")),
                 (
-                    'country',
+                    "country",
                     django_countries.fields.CountryField(
-                        max_length=2, verbose_name='country'
+                        max_length=2, verbose_name="country"
                     ),
                 ),
                 (
-                    'shipping_name',
+                    "shipping_name",
                     models.CharField(
                         blank=True,
-                        help_text='optional',
+                        help_text="optional",
                         max_length=200,
-                        verbose_name='name (shipping)',
+                        verbose_name="name (shipping)",
                     ),
                 ),
                 (
-                    'shipping_street',
+                    "shipping_street",
                     models.CharField(
                         blank=True,
-                        help_text='optional',
+                        help_text="optional",
                         max_length=200,
-                        verbose_name='street (shipping)',
+                        verbose_name="street (shipping)",
                     ),
                 ),
                 (
-                    'shipping_zipcode',
+                    "shipping_zipcode",
                     models.CharField(
                         blank=True,
-                        help_text='optional',
+                        help_text="optional",
                         max_length=200,
-                        verbose_name='zip code (shipping)',
+                        verbose_name="zip code (shipping)",
                     ),
                 ),
                 (
-                    'shipping_city',
+                    "shipping_city",
                     models.CharField(
                         blank=True,
-                        help_text='optional',
+                        help_text="optional",
                         max_length=200,
-                        verbose_name='city (shipping)',
+                        verbose_name="city (shipping)",
                     ),
                 ),
                 (
-                    'user',
+                    "user",
                     models.OneToOneField(
                         on_delete=django.db.models.deletion.CASCADE,
                         to=settings.AUTH_USER_MODEL,
-                        verbose_name='user',
+                        verbose_name="user",
                     ),
                 ),
             ],
             options={
-                'verbose_name': 'Billing info',
-                'verbose_name_plural': 'Billing infos',
-                'abstract': False,
+                "verbose_name": "Billing info",
+                "verbose_name_plural": "Billing infos",
+                "abstract": False,
             },
             bases=(
                 example.sample_plans.models.DetailFieldMixin,
                 plans.base.models.BaseMixin,
                 models.Model,
             ),
         ),
```

### Comparing `django-plans-1.0.4/demo/example/sample_plans/models.py` & `django-plans-1.0.5/demo/example/sample_plans/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from django.db import models
 
-from plans.base.models import (AbstractBillingInfo, AbstractInvoice,
-                               AbstractOrder, AbstractPlan,
-                               AbstractPlanPricing, AbstractPlanQuota,
-                               AbstractPricing, AbstractQuota,
-                               AbstractRecurringUserPlan, AbstractUserPlan)
+from plans.base.models import (
+    AbstractBillingInfo,
+    AbstractInvoice,
+    AbstractOrder,
+    AbstractPlan,
+    AbstractPlanPricing,
+    AbstractPlanQuota,
+    AbstractPricing,
+    AbstractQuota,
+    AbstractRecurringUserPlan,
+    AbstractUserPlan,
+)
 
 
 class DetailFieldMixin:
     # Tests additional field can be added to the models
     detail = models.CharField(max_length=50, null=True, blank=True)
 
 
@@ -26,16 +33,16 @@
     class Meta(AbstractOrder.Meta):
         abstract = False
 
 
 class Plan(AbstractPlan):
     # Test existing fields can be modified
     default = models.BooleanField(
-        help_text=AbstractPlan._meta.get_field('default').help_text,
-        default=AbstractPlan._meta.get_field('default').default,
+        help_text=AbstractPlan._meta.get_field("default").help_text,
+        default=AbstractPlan._meta.get_field("default").default,
         null=True,
         blank=True,
     )
 
     class Meta(AbstractPlan.Meta):
         abstract = False
```

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/mail/change_plan_body.txt` & `django-plans-1.0.5/demo/example/sample_plans/templates/mail/change_plan_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/mail/expired_account_body.txt` & `django-plans-1.0.5/demo/example/sample_plans/templates/mail/expired_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/mail/extend_account_body.txt` & `django-plans-1.0.5/demo/example/sample_plans/templates/mail/extend_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/mail/remind_expire_body.txt` & `django-plans-1.0.5/demo/example/sample_plans/templates/mail/remind_expire_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/account_activation.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/account_activation.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/billing_info_create.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/billing_info_create.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/billing_info_update.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/billing_info_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/create_order.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/create_order.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/current.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/current.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/expiration_messages.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/expiration_messages.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/extend.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/extend.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/invoices/invoice_base.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/invoices/invoice_base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/order_detail.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/order_detail_table.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/order_detail_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/order_list.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/order_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/pagination.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/pagination.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/templates/plans/plan_table.html` & `django-plans-1.0.5/demo/example/sample_plans/templates/plans/plan_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/sample_plans/tests.py` & `django-plans-1.0.5/demo/example/sample_plans/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 from plans.tests.tests import BillingInfoTestCase as BaseBillingInfoTestCase
-from plans.tests.tests import \
-    BillingInfoViewTestCase as BaseBillingInfoViewTestCase
-from plans.tests.tests import \
-    ConcurrentTestInvoice as BaseConcurrentTestInvoice
-from plans.tests.tests import \
-    CreateOrderViewTestCase as BaseCreateOrderViewTestCase
-from plans.tests.tests import \
-    EUTaxationPolicyTestCase as BaseEUTaxationPolicyTestCase
+from plans.tests.tests import BillingInfoViewTestCase as BaseBillingInfoViewTestCase
+from plans.tests.tests import ConcurrentTestInvoice as BaseConcurrentTestInvoice
+from plans.tests.tests import CreateOrderViewTestCase as BaseCreateOrderViewTestCase
+from plans.tests.tests import EUTaxationPolicyTestCase as BaseEUTaxationPolicyTestCase
 from plans.tests.tests import OrderTestCase as BaseOrderTestCase
-from plans.tests.tests import \
-    PlanChangePolicyTestCase as BasePlanChangePolicyTestCase
+from plans.tests.tests import PlanChangePolicyTestCase as BasePlanChangePolicyTestCase
 from plans.tests.tests import PlansTestCase as BasePlansTestCase
-from plans.tests.tests import \
-    RecurringPlansTestCase as BaseRecurringPlansTestCase
-from plans.tests.tests import \
-    StandardPlanChangePolicyTestCase as BaseStandardPlanChangePolicyTestCase
+from plans.tests.tests import RecurringPlansTestCase as BaseRecurringPlansTestCase
+from plans.tests.tests import (
+    StandardPlanChangePolicyTestCase as BaseStandardPlanChangePolicyTestCase,
+)
 from plans.tests.tests import TasksTestCase as BaseTasksTestCase
 from plans.tests.tests import TestInvoice as BaseTestInvoice
 from plans.tests.tests import ValidatorsTestCase as BaseValidatorsTestCase
 
 
 class PlanTestCase(BasePlansTestCase):
     pass
```

### Comparing `django-plans-1.0.4/demo/example/settings.py` & `django-plans-1.0.5/demo/example/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,187 +14,178 @@
 
 DEBUG = True
 
 ADMINS = (
     # ('Your Name', 'your_email@example.com'),
 )
 
-ALLOWED_HOSTS = ['*']
+ALLOWED_HOSTS = ["*"]
 
 MANAGERS = ADMINS
 
 DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.postgresql',
+    "default": {
+        "ENGINE": "django.db.backends.postgresql",
         # Add 'postgresql_psycopg2', 'postgresql', 'mysql', 'sqlite3' or 'oracle'.
-        'NAME': 'postgres',  # Or path to database file if using sqlite3.
-        'USER': 'postgres',  # Not used with sqlite3.
-        'PASSWORD': 'postgres',  # Not used with sqlite3.
-        'HOST': 'localhost',  # Set to empty string for localhost. Not used with sqlite3.
-        'PORT': '5432',  # Set to empty string for default. Not used with sqlite3.
+        "NAME": "postgres",  # Or path to database file if using sqlite3.
+        "USER": "postgres",  # Not used with sqlite3.
+        "PASSWORD": "postgres",  # Not used with sqlite3.
+        "HOST": "localhost",  # Set to empty string for localhost. Not used with sqlite3.
+        "PORT": "5432",  # Set to empty string for default. Not used with sqlite3.
     }
 }
 
 CACHES = {
-    'default': {
-        'BACKEND': 'django.core.cache.backends.locmem.LocMemCache',
+    "default": {
+        "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
     }
 }
 
-TIME_ZONE = 'America/Chicago'
+TIME_ZONE = "America/Chicago"
 USE_TZ = True
-LANGUAGE_CODE = 'en'
+LANGUAGE_CODE = "en"
 SITE_ID = 1
 USE_I18N = True
-USE_L10N = True
 
-LANGUAGES = (
-    ('en', 'English'),
-)
+LANGUAGES = (("en", "English"),)
 
-MEDIA_ROOT = ''
-MEDIA_URL = ''
-STATIC_ROOT = ''
-STATIC_URL = '/static/'
-ADMIN_MEDIA_PREFIX = '/static/admin/'
-STATICFILES_DIRS = (
-    os.path.join(SITE_ROOT, 'static'),
-)
+MEDIA_ROOT = ""
+MEDIA_URL = ""
+STATIC_ROOT = ""
+STATIC_URL = "/static/"
+ADMIN_MEDIA_PREFIX = "/static/admin/"
+STATICFILES_DIRS = (os.path.join(SITE_ROOT, "static"),)
 
 STATICFILES_FINDERS = (
-    'django.contrib.staticfiles.finders.FileSystemFinder',
-    'django.contrib.staticfiles.finders.AppDirectoriesFinder',
+    "django.contrib.staticfiles.finders.FileSystemFinder",
+    "django.contrib.staticfiles.finders.AppDirectoriesFinder",
     #    'django.contrib.staticfiles.finders.DefaultStorageFinder',
 )
 
-SECRET_KEY = 'l#^#iad$8$4=dlh74$!xs=3g4jb(&j+y6*ozy&8k1-&d+vruzy'
+SECRET_KEY = "l#^#iad$8$4=dlh74$!xs=3g4jb(&j+y6*ozy&8k1-&d+vruzy"
 
 MIDDLEWARE = [
-    'django.middleware.security.SecurityMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
+    "django.middleware.security.SecurityMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
 ]
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [
-            os.path.join(SITE_ROOT, 'templates'),
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [
+            os.path.join(SITE_ROOT, "templates"),
         ],
-        'APP_DIRS': False,
-        'OPTIONS': {
-            'debug': True,
-            'context_processors': [
-                'django.contrib.auth.context_processors.auth',
-                'django.template.context_processors.debug',
-                'django.template.context_processors.i18n',
-                'django.template.context_processors.media',
-                'django.template.context_processors.static',
-                'django.template.context_processors.tz',
-                'django.template.context_processors.request',
-                'django.contrib.messages.context_processors.messages',
-                'plans.context_processors.account_status',
+        "APP_DIRS": False,
+        "OPTIONS": {
+            "debug": True,
+            "context_processors": [
+                "django.contrib.auth.context_processors.auth",
+                "django.template.context_processors.debug",
+                "django.template.context_processors.i18n",
+                "django.template.context_processors.media",
+                "django.template.context_processors.static",
+                "django.template.context_processors.tz",
+                "django.template.context_processors.request",
+                "django.contrib.messages.context_processors.messages",
+                "plans.context_processors.account_status",
+            ],
+            "loaders": [
+                "django.template.loaders.filesystem.Loader",
+                "django.template.loaders.app_directories.Loader",
             ],
-            'loaders': [
-                'django.template.loaders.filesystem.Loader',
-                'django.template.loaders.app_directories.Loader',
-            ]
         },
     },
 ]
 
 
-ROOT_URLCONF = 'example.urls'
-WSGI_APPLICATION = 'example.wsgi.application'
+ROOT_URLCONF = "example.urls"
+WSGI_APPLICATION = "example.wsgi.application"
 
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
 
 INSTALLED_APPS = [
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'django.contrib.sites',
-
-    'ordered_model',
-    'bootstrap3',
-    'django_concurrent_tests',
-
-    'plans',
-    'example.foo',
-    'django_extensions',
-    'sequences.apps.SequencesConfig',
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+    "django.contrib.sites",
+    "ordered_model",
+    "bootstrap3",
+    "django_concurrent_tests",
+    "plans",
+    "example.foo",
+    "django_extensions",
+    "sequences.apps.SequencesConfig",
 ]
 
 LOGGING = {
-    'version': 1,
-    'disable_existing_loggers': False,
-    'handlers': {
-        'mail_admins': {
-            'level': 'ERROR',
-            'class': 'django.utils.log.AdminEmailHandler'
+    "version": 1,
+    "disable_existing_loggers": False,
+    "handlers": {
+        "mail_admins": {
+            "level": "ERROR",
+            "class": "django.utils.log.AdminEmailHandler",
         },
-
     },
-    'loggers': {
-        'django.request': {
-            'handlers': ['mail_admins'],
-            'level': 'ERROR',
-            'propagate': True,
+    "loggers": {
+        "django.request": {
+            "handlers": ["mail_admins"],
+            "level": "ERROR",
+            "propagate": True,
         },
-
-    }
+    },
 }
 
 
 # This is required for django-plans
 
 PLANS_INVOICE_ISSUER = {
     "issuer_name": "My Company Ltd",
     "issuer_street": "48th Suny street",
     "issuer_zipcode": "111-456",
     "issuer_city": "Django City",
     "issuer_country": "PL",
     "issuer_tax_number": "PL123456789",
 }
 
-PLANS_TAX = Decimal('23.0')
-PLANS_TAXATION_POLICY = 'plans.taxation.eu.EUTaxationPolicy'
-PLANS_TAX_COUNTRY = 'PL'
+PLANS_TAX = Decimal("23.0")
+PLANS_TAXATION_POLICY = "plans.taxation.eu.EUTaxationPolicy"
+PLANS_TAX_COUNTRY = "PL"
 
 PLANS_VALIDATORS = {
-    'MAX_FOO_COUNT': 'example.foo.validators.max_foos_validator',
+    "MAX_FOO_COUNT": "example.foo.validators.max_foos_validator",
 }
 
-MANAGE_PY_PATH = os.environ.get("MANAGE_PY_PATH", './manage.py')
+MANAGE_PY_PATH = os.environ.get("MANAGE_PY_PATH", "./manage.py")
 
-PLANS_CURRENCY = 'EUR'
+PLANS_CURRENCY = "EUR"
 
-EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
+EMAIL_BACKEND = "django.core.mail.backends.console.EmailBackend"
 
-LOGIN_REDIRECT_URL = '/foo/list/'
+LOGIN_REDIRECT_URL = "/foo/list/"
 
 ENABLE_FAKE_PAYMENTS = True
 
-if os.environ.get('SAMPLE_APP', False):
-    INSTALLED_APPS.remove('plans')
-    INSTALLED_APPS.append('example.sample_plans')
-
-    PLANS_PLAN_MODEL = 'sample_plans.Plan'
-    PLANS_BILLINGINFO_MODEL = 'sample_plans.BillingInfo'
-    PLANS_USERPLAN_MODEL = 'sample_plans.UserPlan'
-    PLANS_PRICING_MODEL = 'sample_plans.Pricing'
-    PLANS_PLANPRICING_MODEL = 'sample_plans.PlanPricing'
-    PLANS_QUOTA_MODEL = 'sample_plans.Quota'
-    PLANS_PLANQUOTA_MODEL = 'sample_plans.PlanQuota'
-    PLANS_ORDER_MODEL = 'sample_plans.Order'
-    PLANS_INVOICE_MODEL = 'sample_plans.Invoice'
-    PLANS_RECURRINGUSERPLAN_MODEL = 'sample_plans.RecurringUserPlan'
+if os.environ.get("SAMPLE_APP", False):
+    INSTALLED_APPS.remove("plans")
+    INSTALLED_APPS.append("example.sample_plans")
+
+    PLANS_PLAN_MODEL = "sample_plans.Plan"
+    PLANS_BILLINGINFO_MODEL = "sample_plans.BillingInfo"
+    PLANS_USERPLAN_MODEL = "sample_plans.UserPlan"
+    PLANS_PRICING_MODEL = "sample_plans.Pricing"
+    PLANS_PLANPRICING_MODEL = "sample_plans.PlanPricing"
+    PLANS_QUOTA_MODEL = "sample_plans.Quota"
+    PLANS_PLANQUOTA_MODEL = "sample_plans.PlanQuota"
+    PLANS_ORDER_MODEL = "sample_plans.Order"
+    PLANS_INVOICE_MODEL = "sample_plans.Invoice"
+    PLANS_RECURRINGUSERPLAN_MODEL = "sample_plans.RecurringUserPlan"
 
     # Celery auto detects tasks only from INSTALLED_APPS
-    CELERY_IMPORTS = ('openwisp_notifications.tasks',)
+    CELERY_IMPORTS = ("openwisp_notifications.tasks",)
```

### Comparing `django-plans-1.0.4/demo/example/static/css/example.css` & `django-plans-1.0.5/demo/example/static/css/example.css`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/static/img/messages/icon_error.png` & `django-plans-1.0.5/demo/example/static/img/messages/icon_error.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/static/img/messages/icon_success.png` & `django-plans-1.0.5/demo/example/static/img/messages/icon_success.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/templates/base.html` & `django-plans-1.0.5/demo/example/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/templates/home.html` & `django-plans-1.0.5/demo/example/templates/home.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/templates/plans/billing_info_create.html` & `django-plans-1.0.5/demo/example/templates/plans/billing_info_create.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/templates/plans/billing_info_update.html` & `django-plans-1.0.5/demo/example/templates/plans/billing_info_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/templates/registration/login.html` & `django-plans-1.0.5/demo/example/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/example/wsgi.py` & `django-plans-1.0.5/demo/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/demo/manage.py` & `django-plans-1.0.5/demo/manage.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/django_plans.egg-info/PKG-INFO` & `django-plans-1.0.5/django_plans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans
-Version: 1.0.4
+Version: 1.0.5
 Summary: Pluggable django app for managing pricing plans with quotas and accounts expiration
 Home-page: https://github.com/cypreess/django-plans
 Author: Krzysztof Dorosz
 Author-email: cypreess@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
```

### Comparing `django-plans-1.0.4/django_plans.egg-info/SOURCES.txt` & `django-plans-1.0.5/django_plans.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,15 @@
 plans/templates/plans/plan_table.html
 plans/templates/plans/pricing.html
 plans/templates/plans/upgrade.html
 plans/templates/plans/invoices/PL_EN.html
 plans/templates/plans/invoices/PL_EN_layout.html
 plans/templates/plans/invoices/invoice_base.html
 plans/tests/__init__.py
+plans/tests/test_autorenew_accounts.py
 plans/tests/test_views.py
 plans/tests/tests.py
 plans_i18n/README.rst
 plans_i18n/__init__.py
 plans_i18n/admin.py
 plans_i18n/models.py
 plans_i18n/tests.py
```

### Comparing `django-plans-1.0.4/docs/Makefile` & `django-plans-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/_static/images/django-plans-1.png` & `django-plans-1.0.5/docs/source/_static/images/django-plans-1.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/_static/images/django-plans-2.png` & `django-plans-1.0.5/docs/source/_static/images/django-plans-2.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/_static/images/django-plans-3.png` & `django-plans-1.0.5/docs/source/_static/images/django-plans-3.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/caveats.rst` & `django-plans-1.0.5/docs/source/caveats.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/conf.py` & `django-plans-1.0.5/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,231 +15,239 @@
 
 settings.configure()
 
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'django-plans'
-copyright = u'2012, Krzysztof Dorosz'
+project = "django-plans"
+copyright = "2012, Krzysztof Dorosz"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.7-alpha'
+version = "0.7-alpha"
 # The full version, including alpha/beta/rc tags.
-release = '0.7-alpha'
+release = "0.7-alpha"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "default"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'django-plansdoc'
+htmlhelp_basename = "django-plansdoc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ('index', 'django-plans.tex', u'django-plans Documentation',
-     u'Krzysztof Dorosz', 'manual'),
+    (
+        "index",
+        "django-plans.tex",
+        "django-plans Documentation",
+        "Krzysztof Dorosz",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'django-plans', u'django-plans Documentation',
-     [u'Krzysztof Dorosz'], 1)
+    ("index", "django-plans", "django-plans Documentation", ["Krzysztof Dorosz"], 1)
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output ------------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    ('index', 'django-plans', u'django-plans Documentation',
-     u'Krzysztof Dorosz', 'django-plans', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        "index",
+        "django-plans",
+        "django-plans Documentation",
+        "Krzysztof Dorosz",
+        "django-plans",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
```

### Comparing `django-plans-1.0.4/docs/source/customize_models.rst` & `django-plans-1.0.5/docs/source/customize_models.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/index.rst` & `django-plans-1.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/installation.rst` & `django-plans-1.0.5/docs/source/installation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -61,18 +61,15 @@
 
 
 Initialize example project database:
 
 .. code-block:: bash
 
     $ cd ..
-    $ python manage.py syncdb
-    [...]
-    Would you like to create one now? (yes/no): no
-    [...]
+    $ python manage.py migrate
 
 
 Initial example data will be loaded automatically.
 
 
 Create `UserPlan` objects for all `User` objects:
 This is done automatically during migrations, but any UserPlan is missing for whatever reason,
```

### Comparing `django-plans-1.0.4/docs/source/integration.rst` & `django-plans-1.0.5/docs/source/integration.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/invoicing.rst` & `django-plans-1.0.5/docs/source/invoicing.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/plans.rst` & `django-plans-1.0.5/docs/source/plans.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/plans_change.rst` & `django-plans-1.0.5/docs/source/plans_change.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/plans_expiration.rst` & `django-plans-1.0.5/docs/source/plans_expiration.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/plans_recurrence.rst` & `django-plans-1.0.5/docs/source/plans_recurrence.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/quota_validators.rst` & `django-plans-1.0.5/docs/source/quota_validators.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/settings.rst` & `django-plans-1.0.5/docs/source/settings.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/south.rst` & `django-plans-1.0.5/docs/source/south.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/taxation.rst` & `django-plans-1.0.5/docs/source/taxation.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/docs/source/templating.rst` & `django-plans-1.0.5/docs/source/templating.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/admin.py` & `django-plans-1.0.5/plans/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,19 +3,26 @@
 from django.contrib import admin
 from django.contrib.auth import get_user_model
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
 from ordered_model.admin import OrderedModelAdmin
 
-from plans.base.models import (AbstractBillingInfo, AbstractInvoice,
-                               AbstractOrder, AbstractPlan,
-                               AbstractPlanPricing, AbstractPlanQuota,
-                               AbstractPricing, AbstractQuota,
-                               AbstractRecurringUserPlan, AbstractUserPlan)
+from plans.base.models import (
+    AbstractBillingInfo,
+    AbstractInvoice,
+    AbstractOrder,
+    AbstractPlan,
+    AbstractPlanPricing,
+    AbstractPlanQuota,
+    AbstractPricing,
+    AbstractQuota,
+    AbstractRecurringUserPlan,
+    AbstractUserPlan,
+)
 
 from .signals import account_automatic_renewal
 
 Invoice = AbstractInvoice.get_concrete_model()
 UserPlan = AbstractUserPlan.get_concrete_model()
 Plan = AbstractPlan.get_concrete_model()
 PlanQuota = AbstractPlanQuota.get_concrete_model()
@@ -28,33 +35,39 @@
 
 
 class UserLinkMixin(object):
     def user_link(self, obj):
         user_model = get_user_model()
         app_label = user_model._meta.app_label
         model_name = user_model._meta.model_name
-        change_url = reverse('admin:%s_%s_change' % (app_label, model_name), args=(obj.user.id,))
+        change_url = reverse(
+            "admin:%s_%s_change" % (app_label, model_name), args=(obj.user.id,)
+        )
         return format_html('<a href="{}">{}</a>', change_url, obj.user.username)
 
-    user_link.short_description = 'User'
+    user_link.short_description = "User"
     user_link.allow_tags = True
 
 
 class PlanQuotaInline(admin.TabularInline):
     model = PlanQuota
 
 
 class PlanPricingInline(admin.TabularInline):
     model = PlanPricing
 
 
 class QuotaAdmin(OrderedModelAdmin):
     list_display = [
-        'codename', 'name', 'description', 'unit',
-        'is_boolean', 'move_up_down_links',
+        "codename",
+        "name",
+        "description",
+        "unit",
+        "is_boolean",
+        "move_up_down_links",
     ]
 
     readonly_fields = ("created", "updated_at")
     list_display_links = list_display
 
 
 def copy_plan(modeladmin, request, queryset):
@@ -76,111 +89,148 @@
 
         for quota in plan.planquota_set.all():
             quota.id = None
             quota.plan = plan_copy
             quota.save(force_insert=True)
 
 
-copy_plan.short_description = _('Make a plan copy')
+copy_plan.short_description = _("Make a plan copy")
 
 
 class PlanAdmin(OrderedModelAdmin):
-    search_fields = ('name', 'customized__username', 'customized__email', )
-    list_filter = ('available', 'visible')
+    search_fields = (
+        "name",
+        "customized__username",
+        "customized__email",
+    )
+    list_filter = ("available", "visible")
     list_display = [
-        'name', 'description', 'customized', 'default', 'available', 'is_free',
-        'created', 'move_up_down_links'
+        "name",
+        "description",
+        "customized",
+        "default",
+        "available",
+        "is_free",
+        "created",
+        "move_up_down_links",
     ]
     list_display_links = list_display
     inlines = (PlanPricingInline, PlanQuotaInline)
     list_select_related = True
-    raw_id_fields = ('customized',)
+    raw_id_fields = ("customized",)
     readonly_fields = ("created", "updated_at")
-    actions = [copy_plan, ]
+    actions = [
+        copy_plan,
+    ]
 
     def queryset(self, request):
-        return super(PlanAdmin, self).queryset(request).select_related(
-            'customized'
-        )
+        return super(PlanAdmin, self).queryset(request).select_related("customized")
 
 
 class BillingInfoAdmin(UserLinkMixin, admin.ModelAdmin):
-    search_fields = ('user__username', 'user__email', 'tax_number', 'name')
-    list_display = ('user', 'tax_number', 'name', 'street', 'zipcode', 'city', 'country')
+    search_fields = ("user__username", "user__email", "tax_number", "name")
+    list_display = (
+        "user",
+        "tax_number",
+        "name",
+        "street",
+        "zipcode",
+        "city",
+        "country",
+    )
     list_display_links = list_display
     list_select_related = True
-    readonly_fields = ('user_link', "created", "updated_at")
-    exclude = ('user',)
+    readonly_fields = ("user_link", "created", "updated_at")
+    exclude = ("user",)
 
 
 def make_order_completed(modeladmin, request, queryset):
     for order in queryset:
         order.complete_order()
 
 
-make_order_completed.short_description = _('Make selected orders completed')
+make_order_completed.short_description = _("Make selected orders completed")
 
 
 def make_order_invoice(modeladmin, request, queryset):
     for order in queryset:
-        if Invoice.objects.filter(type=Invoice.INVOICE_TYPES['INVOICE'], order=order).count() == 0:
-            Invoice.create(order, Invoice.INVOICE_TYPES['INVOICE'])
+        if (
+            Invoice.objects.filter(
+                type=Invoice.INVOICE_TYPES["INVOICE"], order=order
+            ).count()
+            == 0
+        ):
+            Invoice.create(order, Invoice.INVOICE_TYPES["INVOICE"])
 
 
-make_order_invoice.short_description = _('Make invoices for orders')
+make_order_invoice.short_description = _("Make invoices for orders")
 
 
 class InvoiceInline(admin.TabularInline):
     model = Invoice
     extra = 0
-    raw_id_fields = (
-        'user',
-    )
+    raw_id_fields = ("user",)
 
 
 class OrderAdmin(admin.ModelAdmin):
-    list_filter = ('status', 'created', 'completed', 'plan__name', 'pricing')
-    raw_id_fields = ('user',)
-    search_fields = (
-        'id', 'user__username', 'user__email', 'invoice__full_number'
-    )
+    list_filter = ("status", "created", "completed", "plan__name", "pricing")
+    raw_id_fields = ("user",)
+    search_fields = ("id", "user__username", "user__email", "invoice__full_number")
     list_display = (
-        'id', 'name', 'created', 'user', 'status', 'completed',
-        'tax', 'amount', 'currency', 'plan', 'pricing',
-        'plan_extended_from', 'plan_extended_until',
+        "id",
+        "name",
+        "created",
+        "user",
+        "status",
+        "completed",
+        "tax",
+        "amount",
+        "currency",
+        "plan",
+        "pricing",
+        "plan_extended_from",
+        "plan_extended_until",
     )
     readonly_fields = ("created", "updated_at")
     list_display_links = list_display
     actions = [make_order_completed, make_order_invoice]
-    inlines = (InvoiceInline, )
+    inlines = (InvoiceInline,)
 
     def queryset(self, request):
-        return super(OrderAdmin, self).queryset(request).select_related('plan', 'pricing', 'user')
+        return (
+            super(OrderAdmin, self)
+            .queryset(request)
+            .select_related("plan", "pricing", "user")
+        )
 
 
 class InvoiceAdmin(admin.ModelAdmin):
-    search_fields = (
-        'full_number', 'buyer_tax_number',
-        'user__username', 'user__email'
-    )
+    search_fields = ("full_number", "buyer_tax_number", "user__username", "user__email")
     list_filter = (
-        'type',
-        'issued',
-        'tax',
-        'currency',
-        'buyer_country',
+        "type",
+        "issued",
+        "tax",
+        "currency",
+        "buyer_country",
     )
     list_display = (
-        'full_number', 'issued', 'total_net', 'currency', 'user',
-        'tax', 'buyer_name', 'buyer_city', 'buyer_tax_number'
+        "full_number",
+        "issued",
+        "total_net",
+        "currency",
+        "user",
+        "tax",
+        "buyer_name",
+        "buyer_city",
+        "buyer_tax_number",
     )
     readonly_fields = ("created", "updated_at")
     list_display_links = list_display
     list_select_related = True
-    raw_id_fields = ('user', 'order')
+    raw_id_fields = ("user", "order")
 
 
 class RecurringPlanInline(admin.StackedInline):
     model = RecurringUserPlan
     readonly_fields = ("created", "updated_at")
     extra = 0
 
@@ -189,56 +239,77 @@
     """
     Automatically renew payment for this plan
     """
     for user_plan in queryset:
         account_automatic_renewal.send(sender=None, user=user_plan.user)
 
 
-autorenew_payment.short_description = _('Autorenew plan')
+autorenew_payment.short_description = _("Autorenew plan")
 
 
 class UserPlanAdmin(UserLinkMixin, admin.ModelAdmin):
     list_filter = (
-        'active', 'expire', 'plan__name', 'plan__available', 'plan__visible',
-        'recurring__has_automatic_renewal', 'recurring__payment_provider',
-        'recurring__token_verified', 'recurring__pricing',
+        "active",
+        "expire",
+        "plan__name",
+        "plan__available",
+        "plan__visible",
+        "recurring__has_automatic_renewal",
+        "recurring__payment_provider",
+        "recurring__token_verified",
+        "recurring__pricing",
     )
-    search_fields = ('user__username', 'user__email', 'plan__name', 'recurring__token')
+    search_fields = ("user__username", "user__email", "plan__name", "recurring__token")
     list_display = (
-        'user', 'plan', 'expire', 'active', 'recurring__automatic_renewal',
-        'recurring__token_verified', 'recurring__payment_provider', 'recurring__pricing',
+        "user",
+        "plan",
+        "expire",
+        "active",
+        "recurring__automatic_renewal",
+        "recurring__token_verified",
+        "recurring__payment_provider",
+        "recurring__pricing",
     )
     list_display_links = list_display
     list_select_related = True
-    readonly_fields = ('user_link', "created", "updated_at")
+    readonly_fields = ("user_link", "created", "updated_at")
     inlines = (RecurringPlanInline,)
-    actions = [autorenew_payment, ]
-    fields = ('user', 'user_link', 'plan', 'expire', 'active', "created", "updated_at")
-    raw_id_fields = ['user', 'plan', ]
+    actions = [
+        autorenew_payment,
+    ]
+    fields = ("user", "user_link", "plan", "expire", "active", "created", "updated_at")
+    raw_id_fields = [
+        "user",
+        "plan",
+    ]
 
     def recurring__automatic_renewal(self, obj):
         return obj.recurring.has_automatic_renewal
-    recurring__automatic_renewal.admin_order_field = 'recurring__has_automatic_renewal'
+
+    recurring__automatic_renewal.admin_order_field = "recurring__has_automatic_renewal"
     recurring__automatic_renewal.boolean = True
     recurring__automatic_renewal.short_description = "Automatic renewal"
 
     def recurring__token_verified(self, obj):
         return obj.recurring.token_verified
-    recurring__token_verified.admin_order_field = 'recurring__token_verified'
+
+    recurring__token_verified.admin_order_field = "recurring__token_verified"
     recurring__token_verified.boolean = True
     recurring__token_verified.short_description = "Renewal token verified"
 
     def recurring__payment_provider(self, obj):
         return obj.recurring.payment_provider
-    recurring__payment_provider.admin_order_field = 'recurring__payment_provider'
+
+    recurring__payment_provider.admin_order_field = "recurring__payment_provider"
     recurring__payment_provider.short_description = "Renewal payment_provider"
 
     def recurring__pricing(self, obj):
         return obj.recurring.pricing
-    recurring__automatic_renewal.admin_order_field = 'recurring__pricing'
+
+    recurring__automatic_renewal.admin_order_field = "recurring__pricing"
 
 
 admin.site.register(Quota, QuotaAdmin)
 admin.site.register(Plan, PlanAdmin)
 admin.site.register(UserPlan, UserPlanAdmin)
 admin.site.register(Pricing)
 admin.site.register(Order, OrderAdmin)
```

### Comparing `django-plans-1.0.4/plans/base/models.py` & `django-plans-1.0.5/plans/base/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,182 +26,216 @@
 from ordered_model.models import OrderedModel
 from sequences import get_next_value
 from swapper import load_model
 
 from plans.contrib import get_user_language, send_template_email
 from plans.enumeration import Enumeration
 from plans.importer import import_name
-from plans.signals import (account_activated, account_change_plan,
-                           account_deactivated, account_expired,
-                           order_completed)
+from plans.signals import (
+    account_activated,
+    account_change_plan,
+    account_deactivated,
+    account_expired,
+    order_completed,
+)
 from plans.taxation.eu import EUTaxationPolicy
 from plans.utils import country_code_transform, get_country_code, get_currency
 from plans.validators import plan_validation
 
-accounts_logger = logging.getLogger('accounts')
+accounts_logger = logging.getLogger("accounts")
 
 
 class BaseMixin(models.Model):
-    created = models.DateTimeField(_('created'), db_index=True, auto_now_add=True, null=True)
+    created = models.DateTimeField(
+        _("created"), db_index=True, auto_now_add=True, null=True
+    )
     updated_at = models.DateTimeField(auto_now=True, null=True)
 
     class Meta:
         abstract = True
 
     @classmethod
     def get_concrete_model(cls):
-        return load_model('plans', cls.__name__.replace('Abstract', ''))
+        return load_model("plans", cls.__name__.replace("Abstract", ""))
 
 
 class AbstractPlan(BaseMixin, OrderedModel):
     """
     Single plan defined in the system. A plan can customized (referred to user) which means
     that only this user can purchase this plan and have it selected.
 
     Plan also can be visible and available. Plan is displayed on the list of currently available plans
     for user if it is visible. User cannot change plan to a plan that is not visible. Available means
     that user can buy a plan. If plan is not visible but still available it means that user which
     is using this plan already will be able to extend this plan again. If plan is not visible and not
     available, he will be forced then to change plan next time he extends an account.
     """
-    name = models.CharField(_('name'), max_length=100)
-    description = models.TextField(_('description'), blank=True)
+
+    name = models.CharField(_("name"), max_length=100)
+    description = models.TextField(_("description"), blank=True)
     default = models.BooleanField(
         help_text=_('Both "Unknown" and "No" means that the plan is not default'),
         default=None,
         db_index=True,
         unique=True,
         null=True,
     )
     available = models.BooleanField(
-        _('available'), default=False, db_index=True,
-        help_text=_('Is still available for purchase')
+        _("available"),
+        default=False,
+        db_index=True,
+        help_text=_("Is still available for purchase"),
     )
     visible = models.BooleanField(
-        _('visible'), default=True, db_index=True,
-        help_text=_('Is visible in current offer')
+        _("visible"),
+        default=True,
+        db_index=True,
+        help_text=_("Is visible in current offer"),
     )
     customized = models.ForeignKey(
-        settings.AUTH_USER_MODEL, null=True, blank=True,
-        verbose_name=_('customized'),
-        on_delete=models.CASCADE
+        settings.AUTH_USER_MODEL,
+        null=True,
+        blank=True,
+        verbose_name=_("customized"),
+        on_delete=models.CASCADE,
+    )
+    quotas = models.ManyToManyField("Quota", through="PlanQuota")
+    url = models.URLField(
+        max_length=200,
+        blank=True,
+        help_text=_(
+            "Optional link to page with more information (for clickable pricing table headers)"
+        ),
     )
-    quotas = models.ManyToManyField('Quota', through='PlanQuota')
-    url = models.URLField(max_length=200, blank=True, help_text=_(
-        'Optional link to page with more information (for clickable pricing table headers)'))
 
     class Meta:
         abstract = True
-        ordering = ('order',)
+        ordering = ("order",)
         verbose_name = _("Plan")
         verbose_name_plural = _("Plans")
 
     @classmethod
     def get_default_plan(cls):
         try:
             return_value = cls.objects.get(default=True)
         except cls.DoesNotExist:
             return_value = None
         return return_value
 
     @classmethod
     def get_current_plan(cls, user):
-        """ Get current plan for user. If userplan is expired, get default plan """
-        if not user or user.is_anonymous or not hasattr(user, 'userplan') or user.userplan.is_expired():
+        """Get current plan for user. If userplan is expired, get default plan"""
+        if (
+            not user
+            or user.is_anonymous
+            or not hasattr(user, "userplan")
+            or user.userplan.is_expired()
+        ):
             default_plan = cls.get_default_plan()
             if default_plan is None or not default_plan.is_free():
-                raise ValidationError(_('User plan has expired'))
+                raise ValidationError(_("User plan has expired"))
             return default_plan
         return user.userplan.plan
 
     def __str__(self):
         return self.name
 
     def get_quota_dict(self):
-        return dict(self.planquota_set.values_list('quota__codename', 'value'))
+        return dict(self.planquota_set.values_list("quota__codename", "value"))
 
     def is_free(self):
         return self.planpricing_set.count() == 0
+
     is_free.boolean = True
 
 
 class AbstractBillingInfo(BaseMixin, models.Model):
     """
     Stores customer billing data needed to issue an invoice
     """
+
     user = models.OneToOneField(
-        settings.AUTH_USER_MODEL, verbose_name=_('user'),
-        on_delete=models.CASCADE
+        settings.AUTH_USER_MODEL, verbose_name=_("user"), on_delete=models.CASCADE
     )
     tax_number = models.CharField(
-        _('VAT ID'), max_length=200, blank=True, db_index=True
+        _("VAT ID"), max_length=200, blank=True, db_index=True
     )
-    name = models.CharField(_('name'), max_length=200, db_index=True)
-    street = models.CharField(_('street'), max_length=200)
-    zipcode = models.CharField(_('zip code'), max_length=200)
-    city = models.CharField(_('city'), max_length=200)
+    name = models.CharField(_("name"), max_length=200, db_index=True)
+    street = models.CharField(_("street"), max_length=200)
+    zipcode = models.CharField(_("zip code"), max_length=200)
+    city = models.CharField(_("city"), max_length=200)
     country = CountryField(_("country"))
     shipping_name = models.CharField(
-        _('name (shipping)'), max_length=200, blank=True, help_text=_('optional'))
+        _("name (shipping)"), max_length=200, blank=True, help_text=_("optional")
+    )
     shipping_street = models.CharField(
-        _('street (shipping)'), max_length=200, blank=True, help_text=_('optional'))
+        _("street (shipping)"), max_length=200, blank=True, help_text=_("optional")
+    )
     shipping_zipcode = models.CharField(
-        _('zip code (shipping)'), max_length=200, blank=True, help_text=_('optional'))
+        _("zip code (shipping)"), max_length=200, blank=True, help_text=_("optional")
+    )
     shipping_city = models.CharField(
-        _('city (shipping)'), max_length=200, blank=True, help_text=_('optional'))
+        _("city (shipping)"), max_length=200, blank=True, help_text=_("optional")
+    )
 
     class Meta:
         abstract = True
         verbose_name = _("Billing info")
         verbose_name_plural = _("Billing infos")
 
     @staticmethod
     def get_full_tax_number(tax_number, country):
         number = tax_number
         if tax_number.startswith(country):
-            number = tax_number[len(country):]
+            number = tax_number[len(country) :]
         return country_code_transform(country) + number
 
     @staticmethod
     def clean_tax_number(tax_number, country):
-        tax_number = re.sub(r'[^A-Z0-9]', '', tax_number.upper())
+        tax_number = re.sub(r"[^A-Z0-9]", "", tax_number.upper())
 
-        country_str = tax_number[:len(country)]
+        country_str = tax_number[: len(country)]
         if country_str == country_code_transform(country):
             country = country_code_transform(country)
 
         if country_str.isalpha() and country_str != country:
-            raise ValidationError(_('VAT ID country code doesn\'t corespond with country'))
+            raise ValidationError(
+                _("VAT ID country code doesn't corespond with country")
+            )
 
         if tax_number and country:
-
             if country.lower() in stdnum.eu.vat.MEMBER_STATES:
-                full_number = AbstractBillingInfo.get_concrete_model().get_full_tax_number(tax_number, country)
+                full_number = (
+                    AbstractBillingInfo.get_concrete_model().get_full_tax_number(
+                        tax_number, country
+                    )
+                )
                 try:
                     return stdnum.eu.vat.validate(full_number)
                 except stdnum.exceptions.ValidationError as e:
-                    raise ValidationError(_(f'VAT ID is not correct: {e.message}'))
+                    raise ValidationError(_(f"VAT ID is not correct: {e.message}"))
 
             return tax_number
         else:
-            return ''
+            return ""
 
 
 class AbstractUserPlan(BaseMixin, models.Model):
     """
     Currently selected plan for user account.
     """
+
     user = models.OneToOneField(
-        settings.AUTH_USER_MODEL, verbose_name=_('user'),
-        on_delete=models.CASCADE
+        settings.AUTH_USER_MODEL, verbose_name=_("user"), on_delete=models.CASCADE
     )
-    plan = models.ForeignKey('Plan', verbose_name=_('plan'), on_delete=models.CASCADE)
+    plan = models.ForeignKey("Plan", verbose_name=_("plan"), on_delete=models.CASCADE)
     expire = models.DateField(
-        _('expire'), default=None, blank=True, null=True, db_index=True)
-    active = models.BooleanField(_('active'), default=True, db_index=True)
+        _("expire"), default=None, blank=True, null=True, db_index=True
+    )
+    active = models.BooleanField(_("active"), default=True, db_index=True)
 
     class Meta:
         abstract = True
         verbose_name = _("User plan")
         verbose_name_plural = _("Users plans")
 
     def __str__(self):
@@ -220,15 +254,15 @@
         if self.expire is None:
             return None
         else:
             return (self.expire - date.today()).days
 
     def clean_activation(self):
         errors = plan_validation(self.user)
-        if not errors['required_to_activate']:
+        if not errors["required_to_activate"]:
             plan_validation(self.user, on_activation=True)
             self.activate()
         else:
             self.deactivate()
         return errors
 
     def activate(self):
@@ -247,61 +281,76 @@
         """
         Set up user plan for first use
         """
         if not self.is_active():
             # Plans without pricings don't need to expire
             if self.expire is None and self.plan.planpricing_set.count():
                 self.expire = now() + timedelta(
-                    days=getattr(settings, 'PLANS_DEFAULT_GRACE_PERIOD', 30))
+                    days=getattr(settings, "PLANS_DEFAULT_GRACE_PERIOD", 30)
+                )
             self.activate()  # this will call self.save()
 
     def get_plan_extended_from(self, plan):
         if plan.is_free():
             return None
         if not self.is_expired() and self.expire is not None and self.plan == plan:
             return self.expire
         return date.today()
 
     def has_automatic_renewal(self):
-        return hasattr(self, 'recurring') and self.recurring.has_automatic_renewal and self.recurring.token_verified
+        return (
+            hasattr(self, "recurring")
+            and self.recurring.has_automatic_renewal
+            and self.recurring.token_verified
+        )
 
     def get_plan_extended_until(self, plan, pricing):
         if plan.is_free():
             return None
         if pricing is None:
             return self.expire
         return self.get_plan_extended_from(plan) + timedelta(days=pricing.period)
 
     def plan_autorenew_at(self):
         """
         Helper function which calculates when the plan autorenewal will occur
         """
         if self.expire:
-            plans_autorenew_before_days = getattr(settings, 'PLANS_AUTORENEW_BEFORE_DAYS', 0)
-            plans_autorenew_before_hours = getattr(settings, 'PLANS_AUTORENEW_BEFORE_HOURS', 0)
-            return self.expire - timedelta(days=plans_autorenew_before_days, hours=plans_autorenew_before_hours)
+            plans_autorenew_before_days = getattr(
+                settings, "PLANS_AUTORENEW_BEFORE_DAYS", 0
+            )
+            plans_autorenew_before_hours = getattr(
+                settings, "PLANS_AUTORENEW_BEFORE_HOURS", 0
+            )
+            return self.expire - timedelta(
+                days=plans_autorenew_before_days, hours=plans_autorenew_before_hours
+            )
 
     def set_plan_renewal(self, order, has_automatic_renewal=True, **kwargs):
         """
         Creates or updates plan renewal information for this userplan with given order
         """
-        if hasattr(self, 'recurring'):
-            # Delete the plan to populate with default values
-            # We don't want to mix the old and new values
-            self.recurring.delete()
-        recurring = AbstractRecurringUserPlan.get_concrete_model().objects.create(
-            user_plan=self,
-            pricing=order.pricing,
-            amount=order.amount,
-            tax=order.tax,
-            currency=order.currency,
-            has_automatic_renewal=has_automatic_renewal,
-            **kwargs,
-        )
-        return recurring
+        if not hasattr(self, "recurring"):
+            self.recurring = AbstractRecurringUserPlan.get_concrete_model()()
+
+        # Erase values of all fields
+        # We don't want to mix the old and new values
+        self.recurring.set_all_fields_default()
+
+        # Set new values
+        self.recurring.user_plan = self
+        self.recurring.pricing = order.pricing
+        self.recurring.amount = order.amount
+        self.recurring.tax = order.tax
+        self.recurring.currency = order.currency
+        self.recurring.has_automatic_renewal = has_automatic_renewal
+        for k, v in kwargs.items():
+            setattr(self.recurring, k, v)
+        self.recurring.save()
+        return self.recurring
 
     def extend_account(self, plan, pricing):
         """
         Manages extending account after plan or pricing order
         :param plan:
         :param pricing: if pricing is None then account will be only upgraded
         :return:
@@ -316,87 +365,110 @@
 
             if self.expire is not None and not plan.planpricing_set.count():
                 # Assume no expiry date for plans without pricing.
                 self.expire = None
 
             self.save()
             account_change_plan.send(sender=self, user=self.user)
-            if getattr(settings, 'PLANS_SEND_EMAILS_PLAN_CHANGED', True):
-                mail_context = {'user': self.user, 'userplan': self, 'plan': plan}
-                send_template_email([self.user.email], 'mail/change_plan_title.txt', 'mail/change_plan_body.txt',
-                                    mail_context, get_user_language(self.user))
+            if getattr(settings, "PLANS_SEND_EMAILS_PLAN_CHANGED", True):
+                mail_context = {"user": self.user, "userplan": self, "plan": plan}
+                send_template_email(
+                    [self.user.email],
+                    "mail/change_plan_title.txt",
+                    "mail/change_plan_body.txt",
+                    mail_context,
+                    get_user_language(self.user),
+                )
             accounts_logger.info(
-                "Account '%s' [id=%d] plan changed to '%s' [id=%d]" % (self.user, self.user.pk, plan, plan.pk))
+                "Account '%s' [id=%d] plan changed to '%s' [id=%d]"
+                % (self.user, self.user.pk, plan, plan.pk)
+            )
             status = True
         else:
             # Processing standard account extending procedure
             if self.plan == plan:
                 status = True
             else:
                 # This should not ever happen (as this case should be managed by plan change request)
                 # but just in case we consider a case when user has a different plan
                 if not self.plan.is_free() and self.expire is None:
                     status = True
                 elif not self.plan.is_free() and self.expire > date.today():
                     status = False
-                    accounts_logger.warning("Account '%s' [id=%d] plan NOT changed to '%s' [id=%d]" % (
-                        self.user, self.user.pk, plan, plan.pk))
+                    accounts_logger.warning(
+                        "Account '%s' [id=%d] plan NOT changed to '%s' [id=%d]"
+                        % (self.user, self.user.pk, plan, plan.pk)
+                    )
                 else:
                     status = True
                     account_change_plan.send(sender=self, user=self.user)
                     self.plan = plan
 
             if status:
                 self.expire = expire
                 self.save()
-                accounts_logger.info("Account '%s' [id=%d] has been extended by %d days using plan '%s' [id=%d]" % (
-                    self.user, self.user.pk, pricing.period, plan, plan.pk))
-                if getattr(settings, 'PLANS_SEND_EMAILS_PLAN_EXTENDED', True):
-                    mail_context = {'user': self.user,
-                                    'userplan': self,
-                                    'plan': plan,
-                                    'pricing': pricing}
-                    send_template_email([self.user.email], 'mail/extend_account_title.txt',
-                                        'mail/extend_account_body.txt',
-                                        mail_context, get_user_language(self.user))
+                accounts_logger.info(
+                    "Account '%s' [id=%d] has been extended by %d days using plan '%s' [id=%d]"
+                    % (self.user, self.user.pk, pricing.period, plan, plan.pk)
+                )
+                if getattr(settings, "PLANS_SEND_EMAILS_PLAN_EXTENDED", True):
+                    mail_context = {
+                        "user": self.user,
+                        "userplan": self,
+                        "plan": plan,
+                        "pricing": pricing,
+                    }
+                    send_template_email(
+                        [self.user.email],
+                        "mail/extend_account_title.txt",
+                        "mail/extend_account_body.txt",
+                        mail_context,
+                        get_user_language(self.user),
+                    )
 
         if status:
             self.clean_activation()
 
         return status
 
     def expire_account(self):
         """manages account expiration"""
 
         self.deactivate()
 
         accounts_logger.info(
-            "Account '%s' [id=%d] has expired" % (self.user, self.user.pk))
+            "Account '%s' [id=%d] has expired" % (self.user, self.user.pk)
+        )
 
-        mail_context = {'user': self.user, 'userplan': self}
-        send_template_email([self.user.email], 'mail/expired_account_title.txt', 'mail/expired_account_body.txt',
-                            mail_context, get_user_language(self.user))
+        mail_context = {"user": self.user, "userplan": self}
+        send_template_email(
+            [self.user.email],
+            "mail/expired_account_title.txt",
+            "mail/expired_account_body.txt",
+            mail_context,
+            get_user_language(self.user),
+        )
 
         account_expired.send(sender=self, user=self.user)
 
     def remind_expire_soon(self):
         """reminds about soon account expiration"""
 
-        mail_context = {
-            'user': self.user,
-            'userplan': self,
-            'days': self.days_left()
-        }
-        send_template_email([self.user.email], 'mail/remind_expire_title.txt', 'mail/remind_expire_body.txt',
-                            mail_context, get_user_language(self.user))
+        mail_context = {"user": self.user, "userplan": self, "days": self.days_left()}
+        send_template_email(
+            [self.user.email],
+            "mail/remind_expire_title.txt",
+            "mail/remind_expire_body.txt",
+            mail_context,
+            get_user_language(self.user),
+        )
 
     @classmethod
     def create_for_user(cls, user):
-        default_plan = AbstractPlan.get_concrete_model() \
-                                   .get_default_plan()
+        default_plan = AbstractPlan.get_concrete_model().get_default_plan()
         if default_plan is not None:
             UserPlan = AbstractUserPlan.get_concrete_model()
             return UserPlan.objects.create(
                 user=user,
                 plan=default_plan,
                 active=False,
                 expire=None,
@@ -406,59 +478,77 @@
     def create_for_users_without_plan(cls):
         userplans = get_user_model().objects.filter(userplan=None)
         for user in userplans:
             AbstractUserPlan.get_concrete_model().create_for_user(user)
         return userplans
 
     def get_current_plan(self):
-        """ Tiny helper, very usefull in templates """
+        """Tiny helper, very usefull in templates"""
         return AbstractPlan.get_concrete_model().get_current_plan(self.user)
 
 
 class AbstractRecurringUserPlan(BaseMixin, models.Model):
     """
     OneToOne model associated with UserPlan that stores information about the plan recurrence.
     More about recurring payments in docs.
     """
-    user_plan = models.OneToOneField('UserPlan', on_delete=models.CASCADE, related_name='recurring')
+
+    user_plan = models.OneToOneField(
+        "UserPlan", on_delete=models.CASCADE, related_name="recurring"
+    )
     token = models.CharField(
-        _('recurring token'),
-        help_text=_('Token, that will be used for payment renewal. Depends on used payment provider'),
+        _("recurring token"),
+        help_text=_(
+            "Token, that will be used for payment renewal. Depends on used payment provider"
+        ),
         max_length=255,
         default=None,
         null=True,
         blank=True,
     )
     payment_provider = models.CharField(
-        _('payment provider'),
-        help_text=_('Provider, that will be used for payment renewal'),
+        _("payment provider"),
+        help_text=_("Provider, that will be used for payment renewal"),
         max_length=255,
         default=None,
         null=True,
         blank=True,
     )
-    pricing = models.ForeignKey('Pricing', help_text=_('Recurring pricing'), default=None,
-                                null=True, blank=True, on_delete=models.CASCADE)
+    pricing = models.ForeignKey(
+        "Pricing",
+        help_text=_("Recurring pricing"),
+        default=None,
+        null=True,
+        blank=True,
+        on_delete=models.CASCADE,
+    )
     amount = models.DecimalField(
-        _('amount'), max_digits=7, decimal_places=2, db_index=True, null=True, blank=True)
-    tax = models.DecimalField(_('tax'), max_digits=4, decimal_places=2, db_index=True, null=True,
-                              blank=True)  # Tax=None is when tax is not applicable
-    currency = models.CharField(_('currency'), max_length=3)
+        _("amount"),
+        max_digits=7,
+        decimal_places=2,
+        db_index=True,
+        null=True,
+        blank=True,
+    )
+    tax = models.DecimalField(
+        _("tax"), max_digits=4, decimal_places=2, db_index=True, null=True, blank=True
+    )  # Tax=None is when tax is not applicable
+    currency = models.CharField(_("currency"), max_length=3)
     has_automatic_renewal = models.BooleanField(
-        _('has automatic plan renewal'),
+        _("has automatic plan renewal"),
         help_text=_(
-            'Automatic renewal is enabled for associated plan. '
-            'If False, the plan renewal can be still initiated by user.',
+            "Automatic renewal is enabled for associated plan. "
+            "If False, the plan renewal can be still initiated by user.",
         ),
         default=False,
     )
     token_verified = models.BooleanField(
-        _('token has been verified by payment'),
+        _("token has been verified by payment"),
         help_text=_(
-            'The recurring token has been verified by at least one payment to be working.',
+            "The recurring token has been verified by at least one payment to be working.",
         ),
         default=False,
     )
     card_expire_year = models.IntegerField(null=True, blank=True)
     card_expire_month = models.IntegerField(null=True, blank=True)
     card_masked_number = models.CharField(null=True, blank=True, max_length=255)
 
@@ -474,107 +564,148 @@
             user=userplan.user,
             plan=userplan.plan,
             pricing=userplan.recurring.pricing,
             amount=userplan.recurring.amount,
             tax=userplan.recurring.tax,  # Fallback value in case of VIES fault
             currency=userplan.recurring.currency,
         )
-        order.recalculate(userplan.recurring.amount, userplan.user.billinginfo, use_default=False)
+        order.recalculate(
+            userplan.recurring.amount, userplan.user.billinginfo, use_default=False
+        )
         order.save()
 
         # Save new value of tax
         userplan.recurring.tax = order.tax
         userplan.recurring.save()
         return order
 
+    def set_all_fields_default(self):
+        """
+        Set all fields to default values
+        """
+        self.token = None
+        self.payment_provider = None
+        self.pricing = None
+        self.amount = None
+        self.tax = None
+        self.currency = None
+        self.has_automatic_renewal = False
+        self.token_verified = False
+        self.card_expire_year = None
+        self.card_expire_month = None
+        self.card_masked_number = None
+
 
 class AbstractPricing(BaseMixin, models.Model):
     """
     Type of plan period that could be purchased (e.g. 10 days, month, year, etc)
     """
-    name = models.CharField(_('name'), max_length=100)
+
+    name = models.CharField(_("name"), max_length=100)
     period = models.PositiveIntegerField(
-        _('period'), default=30, null=True, blank=True, db_index=True)
-    url = models.URLField(max_length=200, blank=True, help_text=_(
-        'Optional link to page with more information (for clickable pricing table headers)'))
+        _("period"), default=30, null=True, blank=True, db_index=True
+    )
+    url = models.URLField(
+        max_length=200,
+        blank=True,
+        help_text=_(
+            "Optional link to page with more information (for clickable pricing table headers)"
+        ),
+    )
 
     class Meta:
         abstract = True
-        ordering = ('period',)
+        ordering = ("period",)
         verbose_name = _("Pricing")
         verbose_name_plural = _("Pricings")
 
     def __str__(self):
         return "%s (%d " % (self.name, self.period) + "%s)" % _("days")
 
 
 class AbstractQuota(BaseMixin, OrderedModel):
     """
     Single countable or boolean property of system (limitation).
     """
+
     codename = models.CharField(
-        _('codename'), max_length=50, unique=True, db_index=True)
-    name = models.CharField(_('name'), max_length=100)
-    unit = models.CharField(_('unit'), max_length=100, blank=True)
-    description = models.TextField(_('description'), blank=True)
-    is_boolean = models.BooleanField(_('is boolean'), default=False)
-    url = models.CharField(max_length=200, blank=True, help_text=_(
-        'Optional link to page with more information (for clickable pricing table headers)'))
+        _("codename"), max_length=50, unique=True, db_index=True
+    )
+    name = models.CharField(_("name"), max_length=100)
+    unit = models.CharField(_("unit"), max_length=100, blank=True)
+    description = models.TextField(_("description"), blank=True)
+    is_boolean = models.BooleanField(_("is boolean"), default=False)
+    url = models.CharField(
+        max_length=200,
+        blank=True,
+        help_text=_(
+            "Optional link to page with more information (for clickable pricing table headers)"
+        ),
+    )
 
     class Meta:
         abstract = True
-        ordering = ('order',)
+        ordering = ("order",)
         verbose_name = _("Quota")
         verbose_name_plural = _("Quotas")
 
     def __str__(self):
-        return "%s" % (self.codename, )
+        return "%s" % (self.codename,)
 
 
 class PlanPricingManager(models.Manager):
     def get_queryset(self):
-        return super(PlanPricingManager, self).get_queryset().select_related('plan', 'pricing')
+        return (
+            super(PlanPricingManager, self)
+            .get_queryset()
+            .select_related("plan", "pricing")
+        )
 
 
 class AbstractPlanPricing(BaseMixin, models.Model):
-    plan = models.ForeignKey('Plan', on_delete=models.CASCADE)
-    pricing = models.ForeignKey('Pricing', on_delete=models.CASCADE)
+    plan = models.ForeignKey("Plan", on_delete=models.CASCADE)
+    pricing = models.ForeignKey("Pricing", on_delete=models.CASCADE)
     price = models.DecimalField(max_digits=7, decimal_places=2, db_index=True)
     order = models.IntegerField(default=0, null=False, blank=False)
     has_automatic_renewal = models.BooleanField(
-        _('has automatic renewal'),
-        help_text=_('Use automatic renewal if possible?'),
+        _("has automatic renewal"),
+        help_text=_("Use automatic renewal if possible?"),
         default=False,
     )
     visible = models.BooleanField(
-        _('is visible by default'),
-        help_text=_('Is visible in current offer'),
+        _("is visible by default"),
+        help_text=_("Is visible in current offer"),
         default=True,
     )
 
     objects = PlanPricingManager()
 
     class Meta:
         abstract = True
-        ordering = ('order', 'pricing__period', )
+        ordering = (
+            "order",
+            "pricing__period",
+        )
         verbose_name = _("Plan pricing")
         verbose_name_plural = _("Plans pricings")
 
     def __str__(self):
         return f"{self.plan.name} {self.pricing} {'recurring' if self.has_automatic_renewal else ''}"
 
 
 class PlanQuotaManager(models.Manager):
     def get_queryset(self):
-        return super(PlanQuotaManager, self).get_queryset().select_related('plan', 'quota')
+        return (
+            super(PlanQuotaManager, self).get_queryset().select_related("plan", "quota")
+        )
 
 
 class AbstractPlanQuota(BaseMixin, models.Model):
-    plan = models.ForeignKey('Plan', on_delete=models.CASCADE)
-    quota = models.ForeignKey('Quota', on_delete=models.CASCADE)
+    plan = models.ForeignKey("Plan", on_delete=models.CASCADE)
+    quota = models.ForeignKey("Quota", on_delete=models.CASCADE)
     value = models.BigIntegerField(default=1, null=True, blank=True)
 
     objects = PlanQuotaManager()
 
     class Meta:
         abstract = True
         verbose_name = _("Plan quota")
@@ -586,53 +717,68 @@
     Order in this app supports only one item per order. This item is defined by
     plan and pricing attributes. If both are defined the order represents buying
     an account extension.
 
     If only plan is provided (with pricing set to None) this means that user purchased
     a plan upgrade.
     """
-    STATUS = Enumeration([
-        (1, 'NEW', pgettext_lazy('Order status', 'new')),
-        (2, 'COMPLETED', pgettext_lazy('Order status', 'completed')),
-        (3, 'NOT_VALID', pgettext_lazy('Order status', 'not valid')),
-        (4, 'CANCELED', pgettext_lazy('Order status', 'canceled')),
-        (5, 'RETURNED', pgettext_lazy('Order status', 'returned')),
 
-    ])
+    STATUS = Enumeration(
+        [
+            (1, "NEW", pgettext_lazy("Order status", "new")),
+            (2, "COMPLETED", pgettext_lazy("Order status", "completed")),
+            (3, "NOT_VALID", pgettext_lazy("Order status", "not valid")),
+            (4, "CANCELED", pgettext_lazy("Order status", "canceled")),
+            (5, "RETURNED", pgettext_lazy("Order status", "returned")),
+        ]
+    )
 
-    user = models.ForeignKey(settings.AUTH_USER_MODEL, verbose_name=_('user'), on_delete=models.CASCADE)
+    user = models.ForeignKey(
+        settings.AUTH_USER_MODEL, verbose_name=_("user"), on_delete=models.CASCADE
+    )
     flat_name = models.CharField(max_length=200, blank=True, null=True)
-    plan = models.ForeignKey('Plan', verbose_name=_(
-        'plan'), related_name="plan_order", on_delete=models.CASCADE)
-    pricing = models.ForeignKey('Pricing', blank=True, null=True, verbose_name=_(
-        'pricing'), on_delete=models.CASCADE)  # if pricing is None the order is upgrade plan, not buy new pricing
+    plan = models.ForeignKey(
+        "Plan",
+        verbose_name=_("plan"),
+        related_name="plan_order",
+        on_delete=models.CASCADE,
+    )
+    pricing = models.ForeignKey(
+        "Pricing",
+        blank=True,
+        null=True,
+        verbose_name=_("pricing"),
+        on_delete=models.CASCADE,
+    )  # if pricing is None the order is upgrade plan, not buy new pricing
     completed = models.DateTimeField(
-        _('completed'), null=True, blank=True, db_index=True)
+        _("completed"), null=True, blank=True, db_index=True
+    )
     plan_extended_from = models.DateField(
-        _('plan extended from'),
-        help_text=_('The plan was extended from this date'),
+        _("plan extended from"),
+        help_text=_("The plan was extended from this date"),
         null=True,
         blank=True,
     )
     plan_extended_until = models.DateField(
-        _('plan extended until'),
-        help_text=('The plan was extended until this date'),
+        _("plan extended until"),
+        help_text=("The plan was extended until this date"),
         null=True,
         blank=True,
     )
     amount = models.DecimalField(
-        _('amount'), max_digits=7, decimal_places=2, db_index=True)
-    tax = models.DecimalField(_('tax'), max_digits=4, decimal_places=2, db_index=True, null=True,
-                              blank=True)  # Tax=None is when tax is not applicable
-    currency = models.CharField(_('currency'), max_length=3, default='EUR')
-    status = models.IntegerField(
-        _('status'), choices=STATUS, default=STATUS.NEW)
+        _("amount"), max_digits=7, decimal_places=2, db_index=True
+    )
+    tax = models.DecimalField(
+        _("tax"), max_digits=4, decimal_places=2, db_index=True, null=True, blank=True
+    )  # Tax=None is when tax is not applicable
+    currency = models.CharField(_("currency"), max_length=3, default="EUR")
+    status = models.IntegerField(_("status"), choices=STATUS, default=STATUS.NEW)
 
     def __str__(self):
-        return _("Order #%(id)d") % {'id': self.id}
+        return _("Order #%(id)d") % {"id": self.id}
 
     @property
     def name(self):
         """
         Support for two kind of Order names:
         * (preferred) dynamically generated from Plan and Pricing (if flatname is not provided) (translatable)
         * (legacy) just return flat name, which is any text (not translatable)
@@ -640,30 +786,39 @@
         Flat names are only introduced for legacy system support, when you need to migrate old orders into
         django-plans and you cannot match Plan&Pricings convention.
         """
         if self.flat_name:
             return self.flat_name
         else:
             return "%s %s %s " % (
-                _('Plan'), self.plan.name, "(upgrade)" if self.pricing is None else '- %s' % self.pricing)
+                _("Plan"),
+                self.plan.name,
+                "(upgrade)" if self.pricing is None else "- %s" % self.pricing,
+            )
 
     def is_ready_for_payment(self):
         return self.status == self.STATUS.NEW and (now() - self.created).days < getattr(
-            settings, 'PLANS_ORDER_EXPIRATION', 14)
+            settings, "PLANS_ORDER_EXPIRATION", 14
+        )
 
     def get_plan_extended_from(self):
         return self.user.userplan.get_plan_extended_from(self.plan)
 
     def get_plan_extended_until(self):
         return self.user.userplan.get_plan_extended_until(self.plan, self.pricing)
 
     @transaction.atomic()
     def complete_order(self):
         # Get locked order to ensure only one completed order is processed at a time
-        order = AbstractOrder.get_concrete_model().objects.filter(id=self.id).select_for_update().get()
+        order = (
+            AbstractOrder.get_concrete_model()
+            .objects.filter(id=self.id)
+            .select_for_update()
+            .get()
+        )
 
         if order.completed is None:
             self.plan_extended_from = self.get_plan_extended_from()
             status = self.user.userplan.extend_account(self.plan, self.pricing)
             self.plan_extended_until = self.user.userplan.expire
             order.completed = self.completed = now()
             if status:
@@ -679,223 +834,262 @@
     def get_invoices_proforma(self):
         return AbstractInvoice.get_concrete_model().proforma.filter(order=self)
 
     def get_invoices(self):
         return AbstractInvoice.get_concrete_model().invoices.filter(order=self)
 
     def get_all_invoices(self):
-        return self.invoice_set.order_by('issued', 'issued_duplicate', 'pk')
+        return self.invoice_set.order_by("issued", "issued_duplicate", "pk")
 
     def get_plan_pricing(self):
-        return AbstractPlanPricing.get_concrete_model().objects.get(plan=self.plan, pricing=self.pricing)
+        return AbstractPlanPricing.get_concrete_model().objects.get(
+            plan=self.plan, pricing=self.pricing
+        )
 
     def tax_total(self):
         if self.tax is None:
-            return Decimal('0.00')
+            return Decimal("0.00")
         else:
             return self.total() - self.amount
 
     def total(self):
         if self.tax is not None:
-            return (Decimal(self.amount) * (Decimal(self.tax) + 100) / 100).quantize(Decimal('1.00'))
+            return (Decimal(self.amount) * (Decimal(self.tax) + 100) / 100).quantize(
+                Decimal("1.00")
+            )
         else:
             return self.amount
 
     def get_absolute_url(self):
-        return reverse('order', kwargs={'pk': self.pk})
+        return reverse("order", kwargs={"pk": self.pk})
 
     def recalculate(self, amount, billing_info, request=None, use_default=True):
         """
         Calculates and return pre-filled Order
         """
         self.amount = amount
         self.currency = get_currency()
-        country = getattr(billing_info, 'country', None)
+        country = getattr(billing_info, "country", None)
         if country is None:
             country = get_country_code(request)
         else:
             country = country.code
-        if hasattr(billing_info, 'tax_number') and billing_info.tax_number:
-            tax_number = AbstractBillingInfo.get_full_tax_number(billing_info.tax_number, country)
+        if hasattr(billing_info, "tax_number") and billing_info.tax_number:
+            tax_number = AbstractBillingInfo.get_full_tax_number(
+                billing_info.tax_number, country
+            )
         else:
             tax_number = None
         # Calculating tax can be complex task (e.g. VIES webservice call)
         # To ensure that tax calculated on order preview will be the same on final order
         # tax rate is cached for a given billing data (as this value only depends on it)
         tax_session_key = "tax_%s_%s" % (tax_number, country)
         request_successful = True
         if request:
             tax = request.session.get(tax_session_key)
         else:
             tax = None
         if tax is None:
-            taxation_policy = getattr(settings, 'PLANS_TAXATION_POLICY', None)
+            taxation_policy = getattr(settings, "PLANS_TAXATION_POLICY", None)
             if not taxation_policy:
-                raise ImproperlyConfigured('PLANS_TAXATION_POLICY is not set')
+                raise ImproperlyConfigured("PLANS_TAXATION_POLICY is not set")
             taxation_policy = import_name(taxation_policy)
-            tax, request_successful = taxation_policy.get_tax_rate(tax_number, country, request)
+            tax, request_successful = taxation_policy.get_tax_rate(
+                tax_number, country, request
+            )
             tax = str(tax)
             # Because taxation policy could return None which clutters with saving this value
             # into cache, we use str() representation of this value
             if request and request_successful:
                 request.session[tax_session_key] = tax
-        if use_default or request_successful:  # Don't change the tax, if the request was not successful
-            self.tax = Decimal(tax) if tax != 'None' else None
+        if (
+            use_default or request_successful
+        ):  # Don't change the tax, if the request was not successful
+            self.tax = Decimal(tax) if tax != "None" else None
 
     class Meta:
-        ordering = ('-created', )
+        ordering = ("-created",)
         abstract = True
         verbose_name = _("Order")
         verbose_name_plural = _("Orders")
 
 
 class InvoiceManager(models.Manager):
     def get_queryset(self):
-        return super(InvoiceManager, self).get_queryset().filter(type=AbstractInvoice.INVOICE_TYPES['INVOICE'])
+        return (
+            super(InvoiceManager, self)
+            .get_queryset()
+            .filter(type=AbstractInvoice.INVOICE_TYPES["INVOICE"])
+        )
 
 
 class InvoiceProformaManager(models.Manager):
     def get_queryset(self):
-        return super(InvoiceProformaManager, self).get_queryset().filter(type=AbstractInvoice.INVOICE_TYPES['PROFORMA'])
+        return (
+            super(InvoiceProformaManager, self)
+            .get_queryset()
+            .filter(type=AbstractInvoice.INVOICE_TYPES["PROFORMA"])
+        )
 
 
 class InvoiceDuplicateManager(models.Manager):
     def get_queryset(self):
-        return super(InvoiceDuplicateManager, self).get_queryset().filter(
-            type=AbstractInvoice.INVOICE_TYPES['DUPLICATE']
+        return (
+            super(InvoiceDuplicateManager, self)
+            .get_queryset()
+            .filter(type=AbstractInvoice.INVOICE_TYPES["DUPLICATE"])
         )
 
 
 def get_initial_number(older_invoices):
-    return getattr(older_invoices.order_by("number").last(), 'number', 0) + 1
+    return getattr(older_invoices.order_by("number").last(), "number", 0) + 1
 
 
 class AbstractInvoice(BaseMixin, models.Model):
     """
     Single invoice document.
     """
 
-    INVOICE_TYPES = Enumeration([
-        (1, 'INVOICE', _('Invoice')),
-        (2, 'DUPLICATE', _('Invoice Duplicate')),
-        (3, 'PROFORMA', pgettext_lazy('proforma', 'Order confirmation')),
-    ])
+    INVOICE_TYPES = Enumeration(
+        [
+            (1, "INVOICE", _("Invoice")),
+            (2, "DUPLICATE", _("Invoice Duplicate")),
+            (3, "PROFORMA", pgettext_lazy("proforma", "Order confirmation")),
+        ]
+    )
 
     objects = models.Manager()
     invoices = InvoiceManager()
     proforma = InvoiceProformaManager()
     duplicates = InvoiceDuplicateManager()
 
     class NUMBERING:
         """Used as a choices for settings.PLANS_INVOICE_COUNTER_RESET"""
 
         DAILY = 1
         MONTHLY = 2
         ANNUALLY = 3
 
-    user = models.ForeignKey(settings.AUTH_USER_MODEL, verbose_name=_('user'), on_delete=models.CASCADE)
-    order = models.ForeignKey('Order', verbose_name=_('order'), on_delete=models.CASCADE)
+    user = models.ForeignKey(
+        settings.AUTH_USER_MODEL, verbose_name=_("user"), on_delete=models.CASCADE
+    )
+    order = models.ForeignKey(
+        "Order", verbose_name=_("order"), on_delete=models.CASCADE
+    )
     number = models.IntegerField(db_index=True)
     full_number = models.CharField(max_length=200)
     type = models.IntegerField(
-        choices=INVOICE_TYPES, default=INVOICE_TYPES.INVOICE, db_index=True)
+        choices=INVOICE_TYPES, default=INVOICE_TYPES.INVOICE, db_index=True
+    )
     issued = models.DateField(db_index=True)
     issued_duplicate = models.DateField(db_index=True, null=True, blank=True)
     selling_date = models.DateField(db_index=True, null=True, blank=True)
     payment_date = models.DateField(db_index=True)
     unit_price_net = models.DecimalField(max_digits=7, decimal_places=2)
     quantity = models.IntegerField(default=1)
     total_net = models.DecimalField(max_digits=7, decimal_places=2)
     total = models.DecimalField(max_digits=7, decimal_places=2)
     tax_total = models.DecimalField(max_digits=7, decimal_places=2)
-    tax = models.DecimalField(max_digits=4, decimal_places=2, db_index=True, null=True,
-                              blank=True)  # Tax=None is whet tax is not applicable
-    rebate = models.DecimalField(
-        max_digits=4, decimal_places=2, default=Decimal(0))
-    currency = models.CharField(max_length=3, default='EUR')
+    tax = models.DecimalField(
+        max_digits=4, decimal_places=2, db_index=True, null=True, blank=True
+    )  # Tax=None is whet tax is not applicable
+    rebate = models.DecimalField(max_digits=4, decimal_places=2, default=Decimal(0))
+    currency = models.CharField(max_length=3, default="EUR")
     item_description = models.CharField(max_length=200)
     buyer_name = models.CharField(max_length=200, verbose_name=_("Name"), blank=True)
-    buyer_street = models.CharField(max_length=200, verbose_name=_("Street"), blank=True)
+    buyer_street = models.CharField(
+        max_length=200, verbose_name=_("Street"), blank=True
+    )
     buyer_zipcode = models.CharField(
-        max_length=200, verbose_name=_("Zip code"), blank=True)
+        max_length=200, verbose_name=_("Zip code"), blank=True
+    )
     buyer_city = models.CharField(max_length=200, verbose_name=_("City"), blank=True)
-    buyer_country = CountryField(verbose_name=_("Country"), default='PL', blank=True)
+    buyer_country = CountryField(verbose_name=_("Country"), default="PL", blank=True)
     buyer_tax_number = models.CharField(
-        max_length=200, blank=True, verbose_name=_("TAX/VAT number"))
+        max_length=200, blank=True, verbose_name=_("TAX/VAT number")
+    )
     shipping_name = models.CharField(max_length=200, verbose_name=_("Name"), blank=True)
     shipping_street = models.CharField(
-        max_length=200, verbose_name=_("Street"), blank=True)
+        max_length=200, verbose_name=_("Street"), blank=True
+    )
     shipping_zipcode = models.CharField(
-        max_length=200, verbose_name=_("Zip code"), blank=True)
+        max_length=200, verbose_name=_("Zip code"), blank=True
+    )
     shipping_city = models.CharField(max_length=200, verbose_name=_("City"), blank=True)
-    shipping_country = CountryField(verbose_name=_("Country"), default='PL', blank=True)
+    shipping_country = CountryField(verbose_name=_("Country"), default="PL", blank=True)
     require_shipment = models.BooleanField(default=False, db_index=True)
     issuer_name = models.CharField(max_length=200, verbose_name=_("Name"))
     issuer_street = models.CharField(max_length=200, verbose_name=_("Street"))
-    issuer_zipcode = models.CharField(
-        max_length=200, verbose_name=_("Zip code"))
+    issuer_zipcode = models.CharField(max_length=200, verbose_name=_("Zip code"))
     issuer_city = models.CharField(max_length=200, verbose_name=_("City"))
-    issuer_country = CountryField(verbose_name=_("Country"), default='PL')
+    issuer_country = CountryField(verbose_name=_("Country"), default="PL")
     issuer_tax_number = models.CharField(
-        max_length=200, blank=True, verbose_name=_("TAX/VAT number"))
+        max_length=200, blank=True, verbose_name=_("TAX/VAT number")
+    )
 
     class Meta:
         abstract = True
         verbose_name = _("Invoice")
         verbose_name_plural = _("Invoices")
 
     def __str__(self):
         return self.full_number
 
     def get_absolute_url(self):
-        return reverse('invoice_preview_html', kwargs={'pk': self.pk})
+        return reverse("invoice_preview_html", kwargs={"pk": self.pk})
 
     def clean(self):
         if self.number is None:
             Invoice = self.get_concrete_model()
             invoice_counter_reset = getattr(
-                settings, 'PLANS_INVOICE_COUNTER_RESET', Invoice.NUMBERING.MONTHLY)
+                settings, "PLANS_INVOICE_COUNTER_RESET", Invoice.NUMBERING.MONTHLY
+            )
             invoice_counter_reset_name = invoice_counter_reset
 
             # To avoid duplicates as well as gaps in the sequence, we are using django-sequences
             # to generate sequence number for each invoice
             # We keep the old sequence generating mechanism to get lower initial value,
             # so that the sequence will continue backward compatibly
             older_invoices = Invoice.objects.filter(type=self.type)
             initial_number = None
             if invoice_counter_reset == Invoice.NUMBERING.DAILY:
-                invoice_counter_value = f"{self.issued.year}_{self.issued.month}_{self.issued.day}"
+                invoice_counter_value = (
+                    f"{self.issued.year}_{self.issued.month}_{self.issued.day}"
+                )
                 older_invoices = older_invoices.filter(issued=self.issued)
             elif invoice_counter_reset == Invoice.NUMBERING.MONTHLY:
                 invoice_counter_value = f"{self.issued.year}_{self.issued.month}"
                 older_invoices = older_invoices.filter(
                     issued__year=self.issued.year,
                     issued__month=self.issued.month,
                 )
             elif invoice_counter_reset == Invoice.NUMBERING.ANNUALLY:
                 invoice_counter_value = f"{self.issued.year}"
                 older_invoices = older_invoices.filter(issued__year=self.issued.year)
             elif callable(invoice_counter_reset):
                 invoice_counter_value, initial_number = invoice_counter_reset(self)
-                invoice_counter_reset_name = 'call'
+                invoice_counter_reset_name = "call"
             else:
                 raise ImproperlyConfigured(
-                    "PLANS_INVOICE_COUNTER_RESET can be set only to these values: daily, monthly, yearly.")
+                    "PLANS_INVOICE_COUNTER_RESET can be set only to these values: daily, monthly, yearly."
+                )
 
             # get initial value for backward compatibility
             if initial_number:
                 self.initial_number = initial_number
             else:
                 self.initial_number = get_initial_number(older_invoices)
             self.sequence_name = f"invoice_numbers_{self.type}_{invoice_counter_reset_name}_{invoice_counter_value}"
 
     def save(self, *args, **kwargs):
         with transaction.atomic():
             if self.number is None:
-                self.number = get_next_value(self.sequence_name, initial_value=self.initial_number)
+                self.number = get_next_value(
+                    self.sequence_name, initial_value=self.initial_number
+                )
             super(AbstractInvoice, self).save(*args, **kwargs)
 
         # We need to generate full number based on what invoice sequence number actually ended up in DB
         self.refresh_from_db()
         if self.full_number == "":
             self.full_number = self.get_full_number()
         super(AbstractInvoice, self).save(update_fields=["full_number"])
@@ -924,33 +1118,34 @@
         format = getattr(
             settings,
             "PLANS_INVOICE_NUMBER_FORMAT",
             "{{ invoice.number }}/"
             "{% if invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV{% endif %}"
             "/{{ invoice.issued|date:'m/Y' }}",
         )
-        return Template(format).render(Context({'invoice': self}))
+        return Template(format).render(Context({"invoice": self}))
 
     def set_issuer_invoice_data(self):
         """
         Fills models object with issuer data copied from ``settings.PLANS_INVOICE_ISSUER``
 
         :raise: ImproperlyConfigured
         """
         try:
-            issuer = getattr(settings, 'PLANS_INVOICE_ISSUER')
+            issuer = getattr(settings, "PLANS_INVOICE_ISSUER")
         except Exception:
             raise ImproperlyConfigured(
-                "Please set PLANS_INVOICE_ISSUER in order to make an invoice.")
-        self.issuer_name = issuer['issuer_name']
-        self.issuer_street = issuer['issuer_street']
-        self.issuer_zipcode = issuer['issuer_zipcode']
-        self.issuer_city = issuer['issuer_city']
-        self.issuer_country = issuer['issuer_country']
-        self.issuer_tax_number = issuer['issuer_tax_number']
+                "Please set PLANS_INVOICE_ISSUER in order to make an invoice."
+            )
+        self.issuer_name = issuer["issuer_name"]
+        self.issuer_street = issuer["issuer_street"]
+        self.issuer_zipcode = issuer["issuer_zipcode"]
+        self.issuer_city = issuer["issuer_city"]
+        self.issuer_country = issuer["issuer_country"]
+        self.issuer_tax_number = issuer["issuer_tax_number"]
 
     def set_buyer_invoice_data(self, billing_info):
         """
         Fill buyer invoice billing and shipping data by copy them from provided user's ``BillingInfo`` object.
 
         :param billing_info: BillingInfo object
         :type billing_info: BillingInfo
@@ -982,15 +1177,17 @@
         self.total_net = order.amount
         self.total = order.total()
         self.tax_total = order.total() - order.amount
         self.tax = order.tax
         self.currency = order.currency
         if Site is not None:
             self.item_description = "%s - %s" % (
-                Site.objects.get_current().name, order.name)
+                Site.objects.get_current().name,
+                order.name,
+            )
         else:
             self.item_description = order.name
 
     @classmethod
     def create(cls, order, invoice_type):
         language_code = get_user_language(order.user)
 
@@ -1001,42 +1198,52 @@
         try:
             billing_info = BillingInfo.objects.get(user=order.user)
         except BillingInfo.DoesNotExist:
             return
 
         day = date.today()
         pday = order.completed
-        if invoice_type == cls.INVOICE_TYPES['PROFORMA']:
+        if invoice_type == cls.INVOICE_TYPES["PROFORMA"]:
             pday = day + timedelta(days=14)
 
-        invoice = cls(issued=day, selling_date=order.completed,
-                      payment_date=pday)  # FIXME: 14 - this should set accordingly to ORDER_TIMEOUT in days
+        invoice = cls(
+            issued=day, selling_date=order.completed, payment_date=pday
+        )  # FIXME: 14 - this should set accordingly to ORDER_TIMEOUT in days
         invoice.type = invoice_type
         invoice.copy_from_order(order)
         invoice.set_issuer_invoice_data()
         invoice.set_buyer_invoice_data(billing_info)
         invoice.clean()
         invoice.save()
         if language_code is not None:
             translation.deactivate()
 
     def send_invoice_by_email(self):
-        if self.type in getattr(settings, 'PLANS_SEND_EMAILS_DISABLED_INVOICE_TYPES', []):
+        if self.type in getattr(
+            settings, "PLANS_SEND_EMAILS_DISABLED_INVOICE_TYPES", []
+        ):
             return
 
         language_code = get_user_language(self.user)
 
         if language_code is not None:
             translation.activate(language_code)
-        mail_context = {'user': self.user,
-                        'invoice_type': self.get_type_display(),
-                        'invoice_number': self.get_full_number(),
-                        'order': self.order.id,
-                        'order_object': self.order,
-                        'url': self.get_absolute_url(), }
+        mail_context = {
+            "user": self.user,
+            "invoice_type": self.get_type_display(),
+            "invoice_number": self.get_full_number(),
+            "order": self.order.id,
+            "order_object": self.order,
+            "url": self.get_absolute_url(),
+        }
         if language_code is not None:
             translation.deactivate()
-        send_template_email([self.user.email], 'mail/invoice_created_title.txt', 'mail/invoice_created_body.txt',
-                            mail_context, language_code)
+        send_template_email(
+            [self.user.email],
+            "mail/invoice_created_title.txt",
+            "mail/invoice_created_body.txt",
+            mail_context,
+            language_code,
+        )
 
     def is_UE_customer(self):
         return EUTaxationPolicy.is_in_EU(self.buyer_country.code)
```

### Comparing `django-plans-1.0.4/plans/context_processors.py` & `django-plans-1.0.5/plans/context_processors.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,20 +14,22 @@
                                         not active
      * ``EXPIRE_IN_DAYS = integer``, number of days to account expiration,
      * ``EXTEND_URL = string``, URL to account extend page.
      * ``ACTIVATE_URL = string``, URL to account activation needed if  account is not active
 
     """
 
-    if hasattr(request, 'user') and request.user.is_authenticated:
+    if hasattr(request, "user") and request.user.is_authenticated:
         try:
             return {
-                'ACCOUNT_EXPIRED': request.user.userplan.is_expired(),
-                'ACCOUNT_NOT_ACTIVE': (
-                    not request.user.userplan.is_active() and not request.user.userplan.is_expired()),
-                'EXPIRE_IN_DAYS': request.user.userplan.days_left(),
-                'EXTEND_URL': reverse('current_plan'),
-                'ACTIVATE_URL': reverse('account_activation'),
+                "ACCOUNT_EXPIRED": request.user.userplan.is_expired(),
+                "ACCOUNT_NOT_ACTIVE": (
+                    not request.user.userplan.is_active()
+                    and not request.user.userplan.is_expired()
+                ),
+                "EXPIRE_IN_DAYS": request.user.userplan.days_left(),
+                "EXTEND_URL": reverse("current_plan"),
+                "ACTIVATE_URL": reverse("account_activation"),
             }
         except UserPlan.DoesNotExist:
             pass
     return {}
```

### Comparing `django-plans-1.0.4/plans/contrib.py` & `django-plans-1.0.5/plans/contrib.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,66 +6,74 @@
 from django.core.exceptions import ImproperlyConfigured
 from django.template import loader
 from django.template.exceptions import TemplateDoesNotExist
 from django.utils import translation
 
 from plans.signals import user_language
 
-email_logger = logging.getLogger('emails')
+email_logger = logging.getLogger("emails")
 
 
 def send_template_email(recipients, title_template, body_template, context, language):
     """Sends e-mail using templating system"""
 
-    send_emails = getattr(settings, 'SEND_PLANS_EMAILS', True)
+    send_emails = getattr(settings, "SEND_PLANS_EMAILS", True)
     if not send_emails:
         return
 
-    site_name = getattr(settings, 'SITE_NAME', 'Please define settings.SITE_NAME')
-    domain = getattr(settings, 'SITE_URL', None)
+    site_name = getattr(settings, "SITE_NAME", "Please define settings.SITE_NAME")
+    domain = getattr(settings, "SITE_URL", None)
 
     if domain is None:
         try:
-            Site = apps.get_model('sites', 'Site')
+            Site = apps.get_model("sites", "Site")
             current_site = Site.objects.get_current()
             site_name = current_site.name
             domain = current_site.domain
         except LookupError:
             pass
 
-    context.update({'site_name': site_name, 'site_domain': domain, 'site': current_site})
+    context.update(
+        {"site_name": site_name, "site_domain": domain, "site": current_site}
+    )
 
     if language is not None:
         translation.activate(language)
 
     mail_title_template = loader.get_template(title_template)
     mail_body_template = loader.get_template(body_template)
     title = mail_title_template.render(context).strip()
     body = mail_body_template.render(context)
     try:
-        mail_body_template_html = loader.get_template(body_template.replace('.txt', '.html'))
+        mail_body_template_html = loader.get_template(
+            body_template.replace(".txt", ".html")
+        )
         html_body = mail_body_template_html.render(context)
     except TemplateDoesNotExist:
         html_body = None
 
     try:
-        email_from = getattr(settings, 'DEFAULT_FROM_EMAIL')
+        email_from = getattr(settings, "DEFAULT_FROM_EMAIL")
     except AttributeError:
-        raise ImproperlyConfigured('DEFAULT_FROM_EMAIL setting needed for sending e-mails')
+        raise ImproperlyConfigured(
+            "DEFAULT_FROM_EMAIL setting needed for sending e-mails"
+        )
 
     mail.send_mail(title, body, email_from, recipients, html_message=html_body)
 
     if language is not None:
         translation.deactivate()
 
-    email_logger.info(u"Email (%s) sent to %s\nTitle: %s\n%s\n\n" % (language, recipients, title, body))
+    email_logger.info(
+        "Email (%s) sent to %s\nTitle: %s\n%s\n\n" % (language, recipients, title, body)
+    )
 
 
 def get_user_language(user):
-    """ Simple helper that will fire django signal in order
+    """Simple helper that will fire django signal in order
     to get User language possibly given by other part of application.
     :param user:
     :return: string or None
     """
     return_value = {}
     user_language.send(sender=user, user=user, return_value=return_value)
-    return return_value.get('language')
+    return return_value.get("language")
```

### Comparing `django-plans-1.0.4/plans/enumeration.py` & `django-plans-1.0.5/plans/enumeration.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.enum_display = {}
         for item in enum_list:
             self.enum_dict[item[1]] = item[0]
             self.enum_display[item[0]] = item[2]
             self.enum_code[item[0]] = item[1]
 
     def __contains__(self, v):
-        return (v in self.enum_list)
+        return v in self.enum_list
 
     def __len__(self):
         return len(self.enum_list)
 
     def __getitem__(self, v):
         if isinstance(v, six.string_types):
             return self.enum_dict[v]
@@ -46,14 +46,14 @@
         except KeyError:
             raise AttributeError
 
     def __iter__(self):
         return self.enum_list.__iter__()
 
     def __repr__(self):
-        return 'Enum(%s)' % self.enum_list_full.__repr__()
+        return "Enum(%s)" % self.enum_list_full.__repr__()
 
     def get_display_name(self, v):
         return self.enum_display[v]
 
     def get_display_code(self, v):
         return self.enum_code[v]
```

### Comparing `django-plans-1.0.4/plans/fixtures/initial_plan.json` & `django-plans-1.0.5/plans/fixtures/initial_plan.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/fixtures/test_django-plans_auth.json` & `django-plans-1.0.5/plans/fixtures/test_django-plans_auth.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/fixtures/test_django-plans_plans.json` & `django-plans-1.0.5/plans/fixtures/test_django-plans_plans.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/forms.py` & `django-plans-1.0.5/plans/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from django import forms
 from django.core.exceptions import ValidationError
 from django.forms.widgets import HiddenInput
 from django.utils.translation import gettext
 
-from plans.base.models import (AbstractBillingInfo, AbstractOrder,
-                               AbstractPlanPricing)
+from plans.base.models import AbstractBillingInfo, AbstractOrder, AbstractPlanPricing
 
 from .utils import get_country_code
 
 Order = AbstractOrder.get_concrete_model()
 PlanPricing = AbstractPlanPricing.get_concrete_model()
 BillingInfo = AbstractBillingInfo.get_concrete_model()
 
 
 class OrderForm(forms.Form):
-    plan_pricing = forms.ModelChoiceField(queryset=PlanPricing.objects.all(), widget=HiddenInput, required=True)
+    plan_pricing = forms.ModelChoiceField(
+        queryset=PlanPricing.objects.all(), widget=HiddenInput, required=True
+    )
 
 
 class CreateOrderForm(forms.ModelForm):
     """
     This form is intentionally empty as all values for Order object creation need to be computed inside view
 
     Therefore, when implementing for example a rabat coupons, you can add some fields here
@@ -29,35 +30,44 @@
         model = Order
         fields = tuple()
 
 
 class BillingInfoForm(forms.ModelForm):
     class Meta:
         model = BillingInfo
-        exclude = ('user',)
+        exclude = ("user",)
 
     def __init__(self, *args, request=None, **kwargs):
         ret_val = super().__init__(*args, **kwargs)
         if not self.instance.country:
-            self.fields['country'].initial = get_country_code(request)
+            self.fields["country"].initial = get_country_code(request)
         return ret_val
 
     def clean(self):
         cleaned_data = super(BillingInfoForm, self).clean()
 
         try:
-            cleaned_data['tax_number'] = BillingInfo.clean_tax_number(cleaned_data['tax_number'],
-                                                                      cleaned_data.get('country', None))
+            cleaned_data["tax_number"] = BillingInfo.clean_tax_number(
+                cleaned_data["tax_number"], cleaned_data.get("country", None)
+            )
         except ValidationError as e:
-            self._errors['tax_number'] = e.messages
+            self._errors["tax_number"] = e.messages
 
         return cleaned_data
 
 
 class BillingInfoWithoutShippingForm(BillingInfoForm):
     class Meta:
         model = BillingInfo
-        exclude = ('user', 'shipping_name', 'shipping_street', 'shipping_zipcode', 'shipping_city')
+        exclude = (
+            "user",
+            "shipping_name",
+            "shipping_street",
+            "shipping_zipcode",
+            "shipping_city",
+        )
 
 
 class FakePaymentsForm(forms.Form):
-    status = forms.ChoiceField(choices=Order.STATUS, required=True, label=gettext('Change order status to'))
+    status = forms.ChoiceField(
+        choices=Order.STATUS, required=True, label=gettext("Change order status to")
+    )
```

### Comparing `django-plans-1.0.4/plans/listeners.py` & `django-plans-1.0.5/plans/listeners.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from django.contrib.auth import get_user_model
 from django.db.models.signals import post_save
 from django.dispatch.dispatcher import receiver
 
-from plans.base.models import (AbstractInvoice, AbstractOrder, AbstractPlan,
-                               AbstractUserPlan)
+from plans.base.models import (
+    AbstractInvoice,
+    AbstractOrder,
+    AbstractPlan,
+    AbstractUserPlan,
+)
 from plans.signals import activate_user_plan, order_completed
 
 User = get_user_model()
 Order = AbstractOrder.get_concrete_model()
 Invoice = AbstractInvoice.get_concrete_model()
 UserPlan = AbstractUserPlan.get_concrete_model()
 Plan = AbstractPlan.get_concrete_model()
@@ -16,20 +20,20 @@
 @receiver(post_save, sender=Order)
 def create_proforma_invoice(sender, instance, created, **kwargs):
     """
     For every Order if there are defined billing_data creates invoice proforma,
     which is an order confirmation document
     """
     if created:
-        Invoice.create(instance, Invoice.INVOICE_TYPES['PROFORMA'])
+        Invoice.create(instance, Invoice.INVOICE_TYPES["PROFORMA"])
 
 
 @receiver(order_completed)
 def create_invoice(sender, **kwargs):
-    Invoice.create(sender, Invoice.INVOICE_TYPES['INVOICE'])
+    Invoice.create(sender, Invoice.INVOICE_TYPES["INVOICE"])
 
 
 @receiver(post_save, sender=Invoice)
 def send_invoice_by_email(sender, instance, created, **kwargs):
     if created:
         instance.send_invoice_by_email()
 
@@ -42,14 +46,15 @@
 
     if created:
         UserPlan.create_for_user(instance)
 
 
 # Hook to django-registration to initialize plan automatically after user has confirm account
 
+
 @receiver(activate_user_plan)
 def initialize_plan_generic(sender, user, **kwargs):
     try:
         user.userplan.initialize()
     except UserPlan.DoesNotExist:
         return
 
@@ -60,21 +65,21 @@
     @receiver(user_activated)
     def initialize_plan_django_registration(sender, user, request, **kwargs):
         try:
             user.userplan.initialize()
         except UserPlan.DoesNotExist:
             return
 
-
 except ImportError:
     pass
 
 
 # Hook to django-getpaid if it is installed
 try:
     from getpaid.signals import user_data_query
 
     @receiver(user_data_query)
     def set_user_email_for_getpaid(sender, order, user_data, **kwargs):
-        user_data['email'] = order.user.email
+        user_data["email"] = order.user.email
+
 except ImportError:
     pass
```

### Comparing `django-plans-1.0.4/plans/locale/en/LC_MESSAGES/django.po` & `django-plans-1.0.5/plans/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/locale/pl/LC_MESSAGES/django.mo` & `django-plans-1.0.5/plans/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/locale/pl/LC_MESSAGES/django.po` & `django-plans-1.0.5/plans/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/locale/pt_BR/LC_MESSAGES/django.mo` & `django-plans-1.0.5/plans/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/locale/pt_BR/LC_MESSAGES/django.po` & `django-plans-1.0.5/plans/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/locale/ru/LC_MESSAGES/django.mo` & `django-plans-1.0.5/plans/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/locale/ru/LC_MESSAGES/django.po` & `django-plans-1.0.5/plans/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/migrations/0002_auto_20180901_1744.py` & `django-plans-1.0.5/plans/migrations/0002_auto_20180901_1744.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # Generated by Django 2.0.8 on 2018-09-01 15:44
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('plans', '0001_initial'),
+        ("plans", "0001_initial"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='order',
-            name='plan_extended_from',
-            field=models.DateField(blank=True, null=True, verbose_name='plan extended from', help_text='The plan was extended from this date'),
+            model_name="order",
+            name="plan_extended_from",
+            field=models.DateField(
+                blank=True,
+                null=True,
+                verbose_name="plan extended from",
+                help_text="The plan was extended from this date",
+            ),
         ),
         migrations.AddField(
-            model_name='order',
-            name='plan_extended_until',
-            field=models.DateField(blank=True, null=True, verbose_name='plan extended until', help_text='The plan was extended until this date'),
+            model_name="order",
+            name="plan_extended_until",
+            field=models.DateField(
+                blank=True,
+                null=True,
+                verbose_name="plan extended until",
+                help_text="The plan was extended until this date",
+            ),
         ),
     ]
```

### Comparing `django-plans-1.0.4/plans/migrations/0003_make_plans_unique.py` & `django-plans-1.0.5/plans/migrations/0003_make_plans_unique.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,25 +17,29 @@
 
 def set_default_false(apps, schema_editor):
     Plan = apps.get_model("plans", "Plan")
     Plan.objects.filter(default=None).update(default=False)
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('plans', '0002_auto_20180901_1744'),
+        ("plans", "0002_auto_20180901_1744"),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='plan',
-            name='default',
+            model_name="plan",
+            name="default",
             field=models.NullBooleanField(db_index=True, default=None),
         ),
         migrations.RunPython(set_default_null, reverse_code=set_default_false),
         migrations.AlterField(
-            model_name='plan',
-            name='default',
-            field=models.NullBooleanField(db_index=True, default=None, help_text='Both "Unknown" and "No" means that the plan is not default', unique=True),
+            model_name="plan",
+            name="default",
+            field=models.NullBooleanField(
+                db_index=True,
+                default=None,
+                help_text='Both "Unknown" and "No" means that the plan is not default',
+                unique=True,
+            ),
         ),
     ]
```

### Comparing `django-plans-1.0.4/plans/migrations/0010_auto_20220113_1317.py` & `django-plans-1.0.5/plans/migrations/0010_auto_20220113_1317.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,78 @@
 # Generated by Django 3.2.11 on 2022-01-13 19:17
 
 import django_countries.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('plans', '0009_auto_20210303_1134'),
+        ("plans", "0009_auto_20210303_1134"),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='invoice',
-            name='buyer_city',
-            field=models.CharField(blank=True, max_length=200, verbose_name='City'),
+            model_name="invoice",
+            name="buyer_city",
+            field=models.CharField(blank=True, max_length=200, verbose_name="City"),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='buyer_country',
-            field=django_countries.fields.CountryField(blank=True, default='PL', max_length=2, verbose_name='Country'),
+            model_name="invoice",
+            name="buyer_country",
+            field=django_countries.fields.CountryField(
+                blank=True, default="PL", max_length=2, verbose_name="Country"
+            ),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='buyer_name',
-            field=models.CharField(blank=True, max_length=200, verbose_name='Name'),
+            model_name="invoice",
+            name="buyer_name",
+            field=models.CharField(blank=True, max_length=200, verbose_name="Name"),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='buyer_street',
-            field=models.CharField(blank=True, max_length=200, verbose_name='Street'),
+            model_name="invoice",
+            name="buyer_street",
+            field=models.CharField(blank=True, max_length=200, verbose_name="Street"),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='buyer_zipcode',
-            field=models.CharField(blank=True, max_length=200, verbose_name='Zip code'),
+            model_name="invoice",
+            name="buyer_zipcode",
+            field=models.CharField(blank=True, max_length=200, verbose_name="Zip code"),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='shipping_city',
-            field=models.CharField(blank=True, max_length=200, verbose_name='City'),
+            model_name="invoice",
+            name="shipping_city",
+            field=models.CharField(blank=True, max_length=200, verbose_name="City"),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='shipping_country',
-            field=django_countries.fields.CountryField(blank=True, default='PL', max_length=2, verbose_name='Country'),
+            model_name="invoice",
+            name="shipping_country",
+            field=django_countries.fields.CountryField(
+                blank=True, default="PL", max_length=2, verbose_name="Country"
+            ),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='shipping_name',
-            field=models.CharField(blank=True, max_length=200, verbose_name='Name'),
+            model_name="invoice",
+            name="shipping_name",
+            field=models.CharField(blank=True, max_length=200, verbose_name="Name"),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='shipping_street',
-            field=models.CharField(blank=True, max_length=200, verbose_name='Street'),
+            model_name="invoice",
+            name="shipping_street",
+            field=models.CharField(blank=True, max_length=200, verbose_name="Street"),
         ),
         migrations.AlterField(
-            model_name='invoice',
-            name='shipping_zipcode',
-            field=models.CharField(blank=True, max_length=200, verbose_name='Zip code'),
+            model_name="invoice",
+            name="shipping_zipcode",
+            field=models.CharField(blank=True, max_length=200, verbose_name="Zip code"),
         ),
         migrations.AlterField(
-            model_name='plan',
-            name='default',
-            field=models.BooleanField(db_index=True, default=None, help_text='Both "Unknown" and "No" means that the plan is not default', null=True, unique=True),
+            model_name="plan",
+            name="default",
+            field=models.BooleanField(
+                db_index=True,
+                default=None,
+                help_text='Both "Unknown" and "No" means that the plan is not default',
+                null=True,
+                unique=True,
+            ),
         ),
     ]
```

### Comparing `django-plans-1.0.4/plans/models.py` & `django-plans-1.0.5/plans/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 from swapper import swappable_setting
 
-from plans.base.models import (AbstractBillingInfo, AbstractInvoice,
-                               AbstractOrder, AbstractPlan,
-                               AbstractPlanPricing, AbstractPlanQuota,
-                               AbstractPricing, AbstractQuota,
-                               AbstractRecurringUserPlan, AbstractUserPlan)
+from plans.base.models import (
+    AbstractBillingInfo,
+    AbstractInvoice,
+    AbstractOrder,
+    AbstractPlan,
+    AbstractPlanPricing,
+    AbstractPlanQuota,
+    AbstractPricing,
+    AbstractQuota,
+    AbstractRecurringUserPlan,
+    AbstractUserPlan,
+)
 
 
 class Plan(AbstractPlan):
     class Meta(AbstractPlan.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'Plan')
+        swappable = swappable_setting("plans", "Plan")
 
 
 class BillingInfo(AbstractBillingInfo):
     class Meta(AbstractBillingInfo.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'BillingInfo')
+        swappable = swappable_setting("plans", "BillingInfo")
 
 
 class UserPlan(AbstractUserPlan):
     class Meta(AbstractUserPlan.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'UserPlan')
+        swappable = swappable_setting("plans", "UserPlan")
 
 
 class Pricing(AbstractPricing):
     class Meta(AbstractPricing.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'Pricing')
+        swappable = swappable_setting("plans", "Pricing")
 
 
 class PlanPricing(AbstractPlanPricing):
     class Meta(AbstractPlanPricing.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'PlanPricing')
+        swappable = swappable_setting("plans", "PlanPricing")
 
 
 class Quota(AbstractQuota):
     class Meta(AbstractQuota.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'Quota')
+        swappable = swappable_setting("plans", "Quota")
 
 
 class PlanQuota(AbstractPlanQuota):
     class Meta(AbstractPlanQuota.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'PlanQuota')
+        swappable = swappable_setting("plans", "PlanQuota")
 
 
 class Order(AbstractOrder):
     class Meta(AbstractOrder.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'Order')
+        swappable = swappable_setting("plans", "Order")
 
 
 class Invoice(AbstractInvoice):
     class Meta(AbstractInvoice.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'Invoice')
+        swappable = swappable_setting("plans", "Invoice")
 
 
 class RecurringUserPlan(AbstractRecurringUserPlan):
-
     class Meta(AbstractRecurringUserPlan.Meta):
         abstract = False
-        swappable = swappable_setting('plans', 'RecurringUserPlan')
+        swappable = swappable_setting("plans", "RecurringUserPlan")
```

### Comparing `django-plans-1.0.4/plans/plan_change.py` & `django-plans-1.0.5/plans/plan_change.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # coding=utf-8
 from decimal import Decimal
 
 
 class PlanChangePolicy(object):
-
     def _calculate_day_cost(self, plan, period):
         """
         Finds most fitted plan pricing for a given period, and calculate day cost
         """
         if plan.is_free():
             # If plan is free then cost is always 0
             return 0
 
-        plan_pricings = plan.planpricing_set.order_by('-pricing__period').select_related('pricing')
+        plan_pricings = plan.planpricing_set.order_by(
+            "-pricing__period"
+        ).select_related("pricing")
         selected_pricing = None
         for plan_pricing in plan_pricings:
             selected_pricing = plan_pricing
             if plan_pricing.pricing.period <= period:
                 break
 
         if selected_pricing:
-            return (selected_pricing.price / selected_pricing.pricing.period).quantize(Decimal('1.00'))
+            return (selected_pricing.price / selected_pricing.pricing.period).quantize(
+                Decimal("1.00")
+            )
 
-        raise ValueError('Plan %s has no pricings.' % plan)
+        raise ValueError("Plan %s has no pricings." % plan)
 
     def _calculate_final_price(self, period, day_cost_diff):
         if day_cost_diff is None:
             return None
         else:
             return period * day_cost_diff
 
@@ -39,15 +42,17 @@
 
         plan_old_day_cost = self._calculate_day_cost(plan_old, period)
         plan_new_day_cost = self._calculate_day_cost(plan_new, period)
 
         if plan_new_day_cost <= plan_old_day_cost:
             return self._calculate_final_price(period, None)
         else:
-            return self._calculate_final_price(period, plan_new_day_cost - plan_old_day_cost)
+            return self._calculate_final_price(
+                period, plan_new_day_cost - plan_old_day_cost
+            )
 
 
 class StandardPlanChangePolicy(PlanChangePolicy):
     """
     This plan switch policy follows the rules:
         * user can downgrade a plan for free if the plan is
           cheaper or have exact the same price (additional constant charge can be applied)
@@ -71,21 +76,23 @@
             Upgrade percent rate is 10%
             Constant upgrade charge is 0 €
             Switch cost is:
                        23 *            1.00 € *                  10% +                     0 € = 25.30 €
                 days_left * cost_diff_per_day * upgrade_percent_rate + constant_upgrade_charge
     """
 
-    UPGRADE_PERCENT_RATE = Decimal('10.0')
-    UPGRADE_CHARGE = Decimal('0.0')
+    UPGRADE_PERCENT_RATE = Decimal("10.0")
+    UPGRADE_CHARGE = Decimal("0.0")
     DOWNGRADE_CHARGE = None
-    FREE_UPGRADE = Decimal('0.0')
+    FREE_UPGRADE = Decimal("0.0")
 
     def _calculate_final_price(self, period, day_cost_diff):
         if day_cost_diff is None:
             return self.DOWNGRADE_CHARGE
-        cost = (period * day_cost_diff * (self.UPGRADE_PERCENT_RATE / 100 + 1) +
-                self.UPGRADE_CHARGE).quantize(Decimal('1.00'))
+        cost = (
+            period * day_cost_diff * (self.UPGRADE_PERCENT_RATE / 100 + 1)
+            + self.UPGRADE_CHARGE
+        ).quantize(Decimal("1.00"))
         if cost is None or cost < self.FREE_UPGRADE:
             return None
         else:
             return cost
```

### Comparing `django-plans-1.0.4/plans/signals.py` & `django-plans-1.0.5/plans/signals.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/taxation/__init__.py` & `django-plans-1.0.5/plans/taxation/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     @classmethod
     def get_default_tax(cls):
         """
         Gets default tax rate. Simply returns ``settings.PLANS_TAX``
 
         :return: Decimal()
         """
-        return getattr(settings, 'PLANS_TAX', None)
+        return getattr(settings, "PLANS_TAX", None)
 
     @classmethod
     def get_issuer_country_code(cls):
         """
         Gets issuers country. Simply returns ``settings.PLANS_TAX_COUNTRY``
 
         :return: unicode
         """
-        return getattr(settings, 'PLANS_TAX_COUNTRY', None)
+        return getattr(settings, "PLANS_TAX_COUNTRY", None)
 
     @classmethod
     def get_tax_rate(cls, tax_id, country_code):
         """
         Methods
 
         :param tax_id: customer tax id
         :param country_code:  customer country in ISO 2-letters format
         :return: Decimal()
         """
-        raise NotImplementedError('Method get_tax_rate should be implemented.')
+        raise NotImplementedError("Method get_tax_rate should be implemented.")
```

### Comparing `django-plans-1.0.4/plans/taxation/eu.py` & `django-plans-1.0.5/plans/taxation/eu.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from requests.exceptions import ConnectionError
 from suds import WebFault
 from suds.transport import TransportError
 
 from plans.taxation import TaxationPolicy
 from plans.utils import country_code_transform
 
-logger = logging.getLogger('plans.taxation.eu.vies')
+logger = logging.getLogger("plans.taxation.eu.vies")
 
 
 class EUTaxationPolicy(TaxationPolicy):
     """
     This taxation policy should be correct for all EU countries. It uses following rules:
         * if issuer country is not in EU - assert error,
         * for buyer of the same country as issuer - return issuer tax,
@@ -31,66 +31,70 @@
     """
 
     # Standard VAT rates according to
     # http://ec.europa.eu/taxation_customs/resources/documents/taxation/vat/how_vat_works/rates/vat_rates_en.pdf
     # Situation at 1 Jan 2017
 
     EU_COUNTRIES_VAT = {
-        'BE': Decimal('21'),  # Belgium
-        'BG': Decimal('20'),  # Bulgaria
-        'CZ': Decimal('21'),  # Czech Republic
-        'DK': Decimal('25'),  # Denmark
-        'DE': Decimal('19'),  # Germany
-        'EE': Decimal('20'),  # Estonia
-        'EL': Decimal('24'),  # Greece
-        'ES': Decimal('21'),  # Spain
-        'FR': Decimal('20'),  # France
-        'HR': Decimal('25'),  # Croatia
-        'IE': Decimal('23'),  # Ireland
-        'IT': Decimal('22'),  # Italy
-        'CY': Decimal('19'),  # Cyprus
-        'LV': Decimal('21'),  # Latvia
-        'LT': Decimal('21'),  # Lithuania
-        'LU': Decimal('17'),  # Luxembourg
-        'HU': Decimal('27'),  # Hungary
-        'MT': Decimal('18'),  # Malta
-        'NL': Decimal('21'),  # Netherlands
-        'AT': Decimal('20'),  # Austria
-        'PL': Decimal('23'),  # Poland
-        'PT': Decimal('23'),  # Portugal
-        'RO': Decimal('19'),  # Romania
-        'SI': Decimal('22'),  # Slovenia
-        'SK': Decimal('20'),  # Slovakia
-        'FI': Decimal('24'),  # Finland
-        'SE': Decimal('25'),  # Sweden
+        "BE": Decimal("21"),  # Belgium
+        "BG": Decimal("20"),  # Bulgaria
+        "CZ": Decimal("21"),  # Czech Republic
+        "DK": Decimal("25"),  # Denmark
+        "DE": Decimal("19"),  # Germany
+        "EE": Decimal("20"),  # Estonia
+        "EL": Decimal("24"),  # Greece
+        "ES": Decimal("21"),  # Spain
+        "FR": Decimal("20"),  # France
+        "HR": Decimal("25"),  # Croatia
+        "IE": Decimal("23"),  # Ireland
+        "IT": Decimal("22"),  # Italy
+        "CY": Decimal("19"),  # Cyprus
+        "LV": Decimal("21"),  # Latvia
+        "LT": Decimal("21"),  # Lithuania
+        "LU": Decimal("17"),  # Luxembourg
+        "HU": Decimal("27"),  # Hungary
+        "MT": Decimal("18"),  # Malta
+        "NL": Decimal("21"),  # Netherlands
+        "AT": Decimal("20"),  # Austria
+        "PL": Decimal("23"),  # Poland
+        "PT": Decimal("23"),  # Portugal
+        "RO": Decimal("19"),  # Romania
+        "SI": Decimal("22"),  # Slovenia
+        "SK": Decimal("20"),  # Slovakia
+        "FI": Decimal("24"),  # Finland
+        "SE": Decimal("25"),  # Sweden
         # 'GB': Decimal('20'),  # United Kingdom (Great Britain)
     }
 
     @classmethod
     def is_in_EU(cls, country_code):
         return country_code_transform(country_code).upper() in cls.EU_COUNTRIES_VAT
 
     @classmethod
     def get_default_tax(cls):
         issuer_country_code = cls.get_issuer_country_code()
         issuer_country_code = country_code_transform(issuer_country_code)
         try:
             return cls.EU_COUNTRIES_VAT[issuer_country_code]
         except KeyError:
-            raise ImproperlyConfigured("EUTaxationPolicy requires that issuer country is in EU")
+            raise ImproperlyConfigured(
+                "EUTaxationPolicy requires that issuer country is in EU"
+            )
 
     @classmethod
     def get_tax_rate(cls, tax_id, country_code, request=None):
         """
         returns tax rate and if the request was successful.
         """
         country_code = country_code_transform(country_code)
         issuer_country_code = cls.get_issuer_country_code()
         if not cls.is_in_EU(issuer_country_code):
-            raise ImproperlyConfigured("EUTaxationPolicy requires that issuer country is in EU")
+            raise ImproperlyConfigured(
+                "EUTaxationPolicy requires that issuer country is in EU"
+            )
 
         if not tax_id and not country_code:
             # No vat id, no country
             return cls.get_default_tax(), True
 
         elif not tax_id and country_code:
             # Customer is not a company, we know his country
@@ -111,38 +115,42 @@
                 # Company is from the same country as issuer
                 # Normal tax
                 return cls.get_default_tax(), True
 
             if cls.is_in_EU(country_code):
                 # Company is from other EU country
                 try:
-                    vies_result = bool(stdnum.eu.vat.check_vies(tax_id)['valid'])
+                    vies_result = bool(stdnum.eu.vat.check_vies(tax_id)["valid"])
                     logger.info("TAX_ID=%s RESULT=%s" % (tax_id, vies_result))
                     if tax_id and vies_result:
                         # Company is registered in VIES
                         # Charge back
                         return None, True
                     else:
                         return cls.EU_COUNTRIES_VAT[country_code], True
                 except (
-                    WebFault, TransportError, stdnum.exceptions.InvalidComponent, ConnectionError, URLError,
+                    WebFault,
+                    TransportError,
+                    stdnum.exceptions.InvalidComponent,
+                    ConnectionError,
+                    URLError,
                     SAXParseException,
                 ) as e:
                     # If we could not connect to VIES or the VAT ID is incorrect
                     if request:
                         messages.warning(
                             request,
                             format_html(
-                                'There was an error during determining validity of your VAT ID.<br/>'
-                                'If you think, you have european VAT ID and should not be taxed, '
-                                'please try resaving billing info later.<br/>'
-                                '<br/>'
-                                'European VAT Information Exchange System throw following error: {}',
+                                "There was an error during determining validity of your VAT ID.<br/>"
+                                "If you think, you have european VAT ID and should not be taxed, "
+                                "please try resaving billing info later.<br/>"
+                                "<br/>"
+                                "European VAT Information Exchange System throw following error: {}",
                                 e,
-                            )
+                            ),
                         )
                     logger.exception("TAX_ID=%s" % (tax_id))
                     return cls.EU_COUNTRIES_VAT[country_code], False
             else:
                 # Company is not from EU
                 # VAT n/a
                 return None, True
```

### Comparing `django-plans-1.0.4/plans/taxation/ru.py` & `django-plans-1.0.5/plans/taxation/ru.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 class RussianTaxationPolicy(TaxationPolicy):
     """
     FIXME: description needed
 
     """
 
-#   This could be inherited unless there is a reason to be custom
-#    def get_default_tax(self):
-#        return getattr(settings, 'PLANS_TAX', None)
-#
-#    def get_issuer_country_code(self):
-#        return getattr(settings, 'PLANS_TAX_COUNTRY', None)
+    #   This could be inherited unless there is a reason to be custom
+    #    def get_default_tax(self):
+    #        return getattr(settings, 'PLANS_TAX', None)
+    #
+    #    def get_issuer_country_code(self):
+    #        return getattr(settings, 'PLANS_TAX_COUNTRY', None)
 
     def get_tax_rate(self, tax_id, country_code, request=None):
         # TODO
         return 0, True
```

### Comparing `django-plans-1.0.4/plans/templates/mail/change_plan_body.txt` & `django-plans-1.0.5/plans/templates/mail/change_plan_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/mail/expired_account_body.txt` & `django-plans-1.0.5/plans/templates/mail/expired_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/mail/extend_account_body.txt` & `django-plans-1.0.5/plans/templates/mail/extend_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/mail/remind_expire_body.txt` & `django-plans-1.0.5/plans/templates/mail/remind_expire_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/account_activation.html` & `django-plans-1.0.5/plans/templates/plans/account_activation.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/billing_info_create_or_update.html` & `django-plans-1.0.5/plans/templates/plans/billing_info_create_or_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/create_order.html` & `django-plans-1.0.5/plans/templates/plans/create_order.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/current.html` & `django-plans-1.0.5/plans/templates/plans/current.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/expiration_messages.html` & `django-plans-1.0.5/plans/templates/plans/expiration_messages.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/extend.html` & `django-plans-1.0.5/plans/templates/plans/extend.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/invoices/PL_EN_layout.html` & `django-plans-1.0.5/plans/templates/plans/invoices/PL_EN_layout.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/invoices/invoice_base.html` & `django-plans-1.0.5/plans/templates/plans/invoices/invoice_base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/order_detail.html` & `django-plans-1.0.5/plans/templates/plans/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/order_detail_table.html` & `django-plans-1.0.5/plans/templates/plans/order_detail_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/order_list.html` & `django-plans-1.0.5/plans/templates/plans/order_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/pagination.html` & `django-plans-1.0.5/plans/templates/plans/pagination.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/templates/plans/plan_table.html` & `django-plans-1.0.5/plans/templates/plans/plan_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/tests/test_views.py` & `django-plans-1.0.5/plans/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans/tests/tests.py` & `django-plans-1.0.5/plans/tests/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 from django.contrib.messages.storage.fallback import FallbackStorage
 from django.contrib.sessions.middleware import SessionMiddleware
 from django.core import mail
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.core.management import call_command
 from django.db import transaction
 from django.db.models import Q
-from django.test import (RequestFactory, TestCase, TransactionTestCase,
-                         override_settings)
+from django.test import RequestFactory, TestCase, TransactionTestCase, override_settings
 from django.urls import reverse
 from django_concurrent_tests.helpers import call_concurrently
 from freezegun import freeze_time
 from internet_sabotage import no_connection
 from model_bakery import baker
 
 from plans import tasks
-from plans.base.models import (AbstractBillingInfo, AbstractInvoice,
-                               AbstractOrder, AbstractPlan,
-                               AbstractPlanPricing, AbstractUserPlan)
+from plans.base.models import (
+    AbstractBillingInfo,
+    AbstractInvoice,
+    AbstractOrder,
+    AbstractPlan,
+    AbstractPlanPricing,
+    AbstractUserPlan,
+)
 from plans.plan_change import PlanChangePolicy, StandardPlanChangePolicy
 from plans.quota import get_user_quota
 from plans.taxation.eu import EUTaxationPolicy
 from plans.validators import ModelCountValidator
 from plans.views import CreateOrderView
 
 User = get_user_model()
@@ -39,187 +43,215 @@
 Invoice = AbstractInvoice.get_concrete_model()
 Order = AbstractOrder.get_concrete_model()
 Plan = AbstractPlan.get_concrete_model()
 UserPlan = AbstractUserPlan.get_concrete_model()
 
 
 class PlansTestCase(TestCase):
-    fixtures = ['initial_plan', 'test_django-plans_auth', 'test_django-plans_plans']
+    fixtures = ["initial_plan", "test_django-plans_auth", "test_django-plans_plans"]
 
     def setUp(self):
         mail.outbox = []
 
     def test_create_userplans_command(self):
-        """ Test that create_userplans command creates userplan for users that doesn't have it """
-        u = User.objects.get(username='test1')
+        """Test that create_userplans command creates userplan for users that doesn't have it"""
+        u = User.objects.get(username="test1")
         UserPlan.objects.all().delete()
         with self.assertRaises(UserPlan.DoesNotExist):
             u.userplan
         u.refresh_from_db()
         out = StringIO()
-        call_command('create_userplans', stdout=out)
-        self.assertIn('2 user plans was created', out.getvalue())
+        call_command("create_userplans", stdout=out)
+        self.assertIn("2 user plans was created", out.getvalue())
         default_plan = Plan.objects.get(pk=1)
         self.assertEqual(u.userplan.plan, default_plan)
 
     def test_create_userplans(self):
-        """ Test that create_for_users_without_plan method """
-        u = User.objects.get(username='test1')
+        """Test that create_for_users_without_plan method"""
+        u = User.objects.get(username="test1")
         UserPlan.objects.all().delete()
         with self.assertRaises(UserPlan.DoesNotExist):
             u.userplan
         u.refresh_from_db()
         created_plans = UserPlan.create_for_users_without_plan()
         self.assertEqual(created_plans.count(), 2)
         default_plan = Plan.objects.get(pk=1)
         self.assertEqual(u.userplan.plan, default_plan)
 
     def test_get_user_quota(self):
-        u = User.objects.get(username='test1')
-        self.assertEqual(get_user_quota(u),
-                         {u'CUSTOM_WATERMARK': 1, u'MAX_GALLERIES_COUNT': 3, u'MAX_PHOTOS_PER_GALLERY': None})
+        u = User.objects.get(username="test1")
+        self.assertEqual(
+            get_user_quota(u),
+            {
+                "CUSTOM_WATERMARK": 1,
+                "MAX_GALLERIES_COUNT": 3,
+                "MAX_PHOTOS_PER_GALLERY": None,
+            },
+        )
 
     def test_get_user_quota_expired_no_default(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() - timedelta(days=5)
         Plan.get_default_plan().delete()
         with self.assertRaises(ValidationError):
             get_user_quota(u)
 
     def test_get_user_quota_expired_free_plan(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() - timedelta(days=5)
         with self.assertRaises(ValidationError):
             get_user_quota(u)
 
     def test_get_plan_quota(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         p = u.userplan.plan
-        self.assertEqual(p.get_quota_dict(),
-                         {u'CUSTOM_WATERMARK': 1, u'MAX_GALLERIES_COUNT': 3, u'MAX_PHOTOS_PER_GALLERY': None})
+        self.assertEqual(
+            p.get_quota_dict(),
+            {
+                "CUSTOM_WATERMARK": 1,
+                "MAX_GALLERIES_COUNT": 3,
+                "MAX_PHOTOS_PER_GALLERY": None,
+            },
+        )
 
     def test_extend_account_same_plan_future(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=50)
         u.userplan.active = False
         u.userplan.save()
         plan_pricing = PlanPricing.objects.get(plan=u.userplan.plan, pricing__period=30)
         u.userplan.extend_account(plan_pricing.plan, plan_pricing.pricing)
-        self.assertEqual(u.userplan.expire,
-                         date.today() + timedelta(days=50) + timedelta(days=plan_pricing.pricing.period))
+        self.assertEqual(
+            u.userplan.expire,
+            date.today()
+            + timedelta(days=50)
+            + timedelta(days=plan_pricing.pricing.period),
+        )
         self.assertEqual(u.userplan.plan, plan_pricing.plan)
         self.assertEqual(u.userplan.active, True)
         self.assertEqual(len(mail.outbox), 1)
 
     def test_extend_account_same_plan_before(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() - timedelta(days=50)
         u.userplan.active = False
         u.userplan.save()
         plan_pricing = PlanPricing.objects.get(plan=u.userplan.plan, pricing__period=30)
         u.userplan.extend_account(plan_pricing.plan, plan_pricing.pricing)
-        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=plan_pricing.pricing.period))
+        self.assertEqual(
+            u.userplan.expire,
+            date.today() + timedelta(days=plan_pricing.pricing.period),
+        )
         self.assertEqual(u.userplan.plan, plan_pricing.plan)
         self.assertEqual(u.userplan.active, True)
         self.assertEqual(len(mail.outbox), 1)
 
     def test_extend_account_other(self):
         """
         Tests extending expired account with other Plan that user had before:
         Tests if expire date is set correctly
         Tests if mail has been send
         Tests if account has been activated
         """
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() - timedelta(days=50)
         u.userplan.active = False
         u.userplan.save()
-        plan_pricing = PlanPricing.objects.filter(~Q(plan=u.userplan.plan) & Q(pricing__period=30))[0]
+        plan_pricing = PlanPricing.objects.filter(
+            ~Q(plan=u.userplan.plan) & Q(pricing__period=30)
+        )[0]
         u.userplan.extend_account(plan_pricing.plan, plan_pricing.pricing)
-        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=plan_pricing.pricing.period))
+        self.assertEqual(
+            u.userplan.expire,
+            date.today() + timedelta(days=plan_pricing.pricing.period),
+        )
         self.assertEqual(u.userplan.plan, plan_pricing.plan)
         self.assertEqual(u.userplan.active, True)
         self.assertEqual(len(mail.outbox), 1)
 
     @freeze_time("2012-01-14")
     def test_extend_account_other_expire_none(self):
         """
         Tests extending expired=None account with other Plan that user had before and is expired:
         Tests if expire stays None
         Tests if mail has been send
         Tests if account stays activated
         """
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = None
         u.userplan.active = False
         u.userplan.save()
-        plan_pricing = PlanPricing.objects.filter(~Q(plan=u.userplan.plan) & Q(pricing__period=30))[0]
+        plan_pricing = PlanPricing.objects.filter(
+            ~Q(plan=u.userplan.plan) & Q(pricing__period=30)
+        )[0]
         default_plan = Plan.objects.get(pk=1)
         u.userplan.extend_account(plan_pricing.plan, plan_pricing.pricing)
         self.assertEqual(u.userplan.expire, date(2012, 2, 13))
         self.assertEqual(u.userplan.plan, default_plan)
         self.assertEqual(u.userplan.active, True)
         self.assertEqual(len(mail.outbox), 1)
 
     def test_extend_account_other_expire_future(self):
         """
         Tests extending active account with other Plan that user had before:
         Tests if expire date stays the same
         Tests if mail has not been send
         Tests if account has not been activated
         """
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=5)
         u.userplan.active = False
         u.userplan.save()
-        plan_pricing = PlanPricing.objects.filter(~Q(plan=u.userplan.plan) & Q(pricing__period=30))[0]
+        plan_pricing = PlanPricing.objects.filter(
+            ~Q(plan=u.userplan.plan) & Q(pricing__period=30)
+        )[0]
         default_plan = Plan.objects.get(pk=1)
         u.userplan.extend_account(plan_pricing.plan, plan_pricing.pricing)
         self.assertEqual(u.userplan.expire, date.today() + timedelta(days=5))
         self.assertEqual(u.userplan.plan, default_plan)
         self.assertEqual(u.userplan.active, False)
         self.assertEqual(len(mail.outbox), 0)
 
     def test_expire_account(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=50)
         u.userplan.active = True
         u.userplan.save()
         u.userplan.expire_account()
         self.assertEqual(u.userplan.active, False)
         self.assertEqual(len(mail.outbox), 1)
 
     def test_remind_expire(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=14)
         u.userplan.active = True
         u.userplan.save()
         u.userplan.remind_expire_soon()
         self.assertEqual(u.userplan.active, True)
         self.assertEqual(len(mail.outbox), 1)
 
     def test_disable_emails(self):
         with self.settings(SEND_PLANS_EMAILS=False):
             # Re-run the remind_expire test, but look for 0 emails sent
-            u = User.objects.get(username='test1')
+            u = User.objects.get(username="test1")
             u.userplan.expire = date.today() + timedelta(days=14)
             u.userplan.active = True
             u.userplan.save()
             u.userplan.remind_expire_soon()
             self.assertEqual(u.userplan.active, True)
             self.assertEqual(len(mail.outbox), 0)
 
     def test_switch_to_free_no_expiry(self):
         """
         Tests switching to a free Plan and checks that their expiry is cleared
         Tests if expire date is set correctly
         Tests if mail has been send
         Tests if account has been activated
         """
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=14)
         self.assertIsNotNone(u.userplan.expire)
 
         plan = Plan.objects.get(name="Free")
         self.assertTrue(plan.is_free())
         self.assertNotEqual(u.userplan.plan, plan)
 
@@ -232,35 +264,37 @@
     def test_switch_from_free_set_expiry(self):
         """
         Tests switching from a free Plan and should set the expiry date
         Tests if expire date is set correctly
         Tests if mail has been send
         Tests if account has been activated
         """
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = None
         u.userplan.plan = Plan.objects.get(name="Free")
         u.userplan.save()
         self.assertIsNone(u.userplan.expire)
         self.assertTrue(u.userplan.plan.is_free())
 
         plan = Plan.objects.get(name="Standard")
         self.assertFalse(plan.is_free())
         self.assertNotEqual(u.userplan.plan, plan)
-        plan_pricing = PlanPricing.objects.filter(Q(plan=plan) & Q(pricing__period=30))[0]
+        plan_pricing = PlanPricing.objects.filter(Q(plan=plan) & Q(pricing__period=30))[
+            0
+        ]
 
         # Switch to Standard Plan
         u.userplan.extend_account(plan, plan_pricing.pricing)
         self.assertEqual(u.userplan.plan, plan)
         self.assertIsNotNone(u.userplan.expire)
         self.assertEqual(u.userplan.active, True)
 
 
 class TestInvoice(TestCase):
-    fixtures = ['initial_plan', 'test_django-plans_auth', 'test_django-plans_plans']
+    fixtures = ["initial_plan", "test_django-plans_auth", "test_django-plans_plans"]
 
     def test_get_full_number(self):
         i = Invoice()
         i.number = 123
         i.issued = date(2010, 5, 30)
         self.assertEqual(i.get_full_number(), "123/FV/05/2010")
 
@@ -282,16 +316,18 @@
         i = Invoice()
         i.type = Invoice.INVOICE_TYPES.PROFORMA
         i.number = 123
         i.issued = date(2010, 5, 30)
         self.assertEqual(i.get_full_number(), "123/PF/05/2010")
 
     def test_get_full_number_with_settings(self):
-        settings.PLANS_INVOICE_NUMBER_FORMAT = "{{ invoice.issued|date:'Y' }}." \
+        settings.PLANS_INVOICE_NUMBER_FORMAT = (
+            "{{ invoice.issued|date:'Y' }}."
             "{{ invoice.number }}.{{ invoice.issued|date:'m' }}"
+        )
         i = Invoice()
         i.number = 123
         i.issued = date(2010, 5, 30)
         self.assertEqual(i.get_full_number(), "2010.123.05")
 
     def test_set_issuer_invoice_data_raise(self):
         issdata = settings.PLANS_INVOICE_ISSUER
@@ -299,76 +335,103 @@
         i = Invoice()
         self.assertRaises(ImproperlyConfigured, i.set_issuer_invoice_data)
         settings.PLANS_INVOICE_ISSUER = issdata
 
     def test_set_issuer_invoice_data(self):
         i = Invoice()
         i.set_issuer_invoice_data()
-        self.assertEqual(i.issuer_name, settings.PLANS_INVOICE_ISSUER['issuer_name'])
-        self.assertEqual(i.issuer_street, settings.PLANS_INVOICE_ISSUER['issuer_street'])
-        self.assertEqual(i.issuer_zipcode, settings.PLANS_INVOICE_ISSUER['issuer_zipcode'])
-        self.assertEqual(i.issuer_city, settings.PLANS_INVOICE_ISSUER['issuer_city'])
-        self.assertEqual(i.issuer_country, settings.PLANS_INVOICE_ISSUER['issuer_country'])
-        self.assertEqual(i.issuer_tax_number, settings.PLANS_INVOICE_ISSUER['issuer_tax_number'])
+        self.assertEqual(i.issuer_name, settings.PLANS_INVOICE_ISSUER["issuer_name"])
+        self.assertEqual(
+            i.issuer_street, settings.PLANS_INVOICE_ISSUER["issuer_street"]
+        )
+        self.assertEqual(
+            i.issuer_zipcode, settings.PLANS_INVOICE_ISSUER["issuer_zipcode"]
+        )
+        self.assertEqual(i.issuer_city, settings.PLANS_INVOICE_ISSUER["issuer_city"])
+        self.assertEqual(
+            i.issuer_country, settings.PLANS_INVOICE_ISSUER["issuer_country"]
+        )
+        self.assertEqual(
+            i.issuer_tax_number, settings.PLANS_INVOICE_ISSUER["issuer_tax_number"]
+        )
 
     def set_buyer_invoice_data(self):
         i = Invoice()
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         i.set_buyer_invoice_data(u.billinginfo)
         self.assertEqual(i.buyer_name, u.billinginfo.name)
         self.assertEqual(i.buyer_street, u.billinginfo.street)
         self.assertEqual(i.buyer_zipcode, u.billinginfo.zipcode)
         self.assertEqual(i.buyer_city, u.billinginfo.city)
         self.assertEqual(i.buyer_country, u.billinginfo.country)
         self.assertEqual(i.buyer_tax_number, u.billinginfo.tax_number)
         self.assertEqual(i.buyer_name, u.billinginfo.shipping_name)
         self.assertEqual(i.buyer_street, u.billinginfo.shipping_street)
         self.assertEqual(i.buyer_zipcode, u.billinginfo.shipping_zipcode)
         self.assertEqual(i.buyer_city, u.billinginfo.shipping_city)
         self.assertEqual(i.buyer_country, u.billinginfo.shipping_country)
 
     def test_invoice_number(self):
-        settings.PLANS_INVOICE_NUMBER_FORMAT = "{{ invoice.number }}/{% if " \
-            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV" \
+        settings.PLANS_INVOICE_NUMBER_FORMAT = (
+            "{{ invoice.number }}/{% if "
+            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV"
             "{% endif %}/{{ invoice.issued|date:'m/Y' }}"
+        )
         o = Order.objects.all()[0]
         day = date(2010, 5, 3)
         i = Invoice(issued=day, selling_date=day, payment_date=day)
         i.copy_from_order(o)
         i.set_issuer_invoice_data()
         i.set_buyer_invoice_data(o.user.billinginfo)
         i.clean()
         i.save()
 
         self.assertEqual(i.number, 1)
-        self.assertEqual(i.full_number, '1/FV/05/2010')
+        self.assertEqual(i.full_number, "1/FV/05/2010")
 
     def test_invoice_number_daily(self):
-        settings.PLANS_INVOICE_NUMBER_FORMAT = "{{ invoice.number }}/{% if " \
-            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV" \
+        settings.PLANS_INVOICE_NUMBER_FORMAT = (
+            "{{ invoice.number }}/{% if "
+            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV"
             "{% endif %}/{{ invoice.issued|date:'d/m/Y' }}"
+        )
         settings.PLANS_INVOICE_COUNTER_RESET = Invoice.NUMBERING.DAILY
 
-        user = User.objects.get(username='test1')
+        user = User.objects.get(username="test1")
         plan_pricing = PlanPricing.objects.all()[0]
         tax = getattr(settings, "PLANS_TAX")
         currency = getattr(settings, "PLANS_CURRENCY")
-        o1 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o1 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o1.save()
 
-        o2 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o2 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o2.save()
 
-        o3 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o3 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o3.save()
 
         day = date(2001, 5, 3)
         i1 = Invoice(issued=day, selling_date=day, payment_date=day)
         i1.copy_from_order(o1)
         i1.set_issuer_invoice_data()
         i1.set_buyer_invoice_data(o1.user.billinginfo)
@@ -391,36 +454,53 @@
         i3.save()
 
         self.assertEqual(i1.full_number, "1/FV/03/05/2001")
         self.assertEqual(i2.full_number, "2/FV/03/05/2001")
         self.assertEqual(i3.full_number, "1/FV/04/05/2001")
 
     def test_invoice_number_monthly(self):
-        settings.PLANS_INVOICE_NUMBER_FORMAT = "{{ invoice.number }}/{% if " \
-            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV" \
+        settings.PLANS_INVOICE_NUMBER_FORMAT = (
+            "{{ invoice.number }}/{% if "
+            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV"
             "{% endif %}/{{ invoice.issued|date:'m/Y' }}"
+        )
         settings.PLANS_INVOICE_COUNTER_RESET = Invoice.NUMBERING.MONTHLY
 
-        user = User.objects.get(username='test1')
+        user = User.objects.get(username="test1")
         plan_pricing = PlanPricing.objects.all()[0]
         tax = getattr(settings, "PLANS_TAX")
         currency = getattr(settings, "PLANS_CURRENCY")
-        o1 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o1 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o1.save()
 
-        o2 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o2 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o2.save()
 
-        o3 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o3 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o3.save()
 
         day = date(2002, 5, 3)
         i1 = Invoice(issued=day, selling_date=day, payment_date=day)
         i1.copy_from_order(o1)
         i1.set_issuer_invoice_data()
         i1.set_buyer_invoice_data(o1.user.billinginfo)
@@ -444,36 +524,53 @@
         i3.save()
 
         self.assertEqual(i1.full_number, "1/FV/05/2002")
         self.assertEqual(i2.full_number, "2/FV/05/2002")
         self.assertEqual(i3.full_number, "1/FV/06/2002")
 
     def test_invoice_number_annually(self):
-        settings.PLANS_INVOICE_NUMBER_FORMAT = "{{ invoice.number }}/{% if " \
-            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV" \
+        settings.PLANS_INVOICE_NUMBER_FORMAT = (
+            "{{ invoice.number }}/{% if "
+            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV"
             "{% endif %}/{{ invoice.issued|date:'Y' }}"
+        )
         settings.PLANS_INVOICE_COUNTER_RESET = Invoice.NUMBERING.ANNUALLY
 
-        user = User.objects.get(username='test1')
+        user = User.objects.get(username="test1")
         plan_pricing = PlanPricing.objects.all()[0]
         tax = getattr(settings, "PLANS_TAX")
         currency = getattr(settings, "PLANS_CURRENCY")
-        o1 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o1 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o1.save()
 
-        o2 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o2 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o2.save()
 
-        o3 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o3 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o3.save()
 
         day = date(1991, 5, 3)
         i1 = Invoice(issued=day, selling_date=day, payment_date=day)
         i1.copy_from_order(o1)
         i1.set_issuer_invoice_data()
         i1.set_buyer_invoice_data(o1.user.billinginfo)
@@ -497,50 +594,69 @@
         i3.save()
 
         self.assertEqual(i1.full_number, "1/FV/1991")
         self.assertEqual(i2.full_number, "2/FV/1991")
         self.assertEqual(i3.full_number, "1/FV/1992")
 
     def test_invoice_number_custom(self):
-        settings.PLANS_INVOICE_NUMBER_FORMAT = "{{ invoice.number }}/{% if " \
-            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV" \
+        settings.PLANS_INVOICE_NUMBER_FORMAT = (
+            "{{ invoice.number }}/{% if "
+            "invoice.type == invoice.INVOICE_TYPES.PROFORMA %}PF{% else %}FV"
             "{% endif %}/{{ invoice.issued|date:'Y' }}"
+        )
 
         def plans_invoice_counter_reset_function(invoice):
             from plans.base.models import get_initial_number
 
             older_invoices = Invoice.objects.filter(
                 type=invoice.type,
                 issued__year=invoice.issued.year,
                 issued__month=invoice.issued.month,
                 currency=invoice.currency,
             )
-            sequence_name = f"{invoice.issued.year}_{invoice.issued.month}_{invoice.currency}"
+            sequence_name = (
+                f"{invoice.issued.year}_{invoice.issued.month}_{invoice.currency}"
+            )
             return sequence_name, get_initial_number(older_invoices)
 
         settings.PLANS_INVOICE_COUNTER_RESET = plans_invoice_counter_reset_function
 
-        user = User.objects.get(username='test1')
+        user = User.objects.get(username="test1")
         plan_pricing = PlanPricing.objects.all()[0]
         tax = getattr(settings, "PLANS_TAX")
         currency = getattr(settings, "PLANS_CURRENCY")
-        currency1 = 'CZK'
-        o1 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        currency1 = "CZK"
+        o1 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o1.save()
 
-        o2 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency1)
+        o2 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency1,
+        )
         o2.save()
 
-        o3 = Order(user=user, plan=plan_pricing.plan,
-                   pricing=plan_pricing.pricing, amount=plan_pricing.price,
-                   tax=tax, currency=currency)
+        o3 = Order(
+            user=user,
+            plan=plan_pricing.plan,
+            pricing=plan_pricing.pricing,
+            amount=plan_pricing.price,
+            tax=tax,
+            currency=currency,
+        )
         o3.save()
 
         day = date(1991, 7, 13)
         i1 = Invoice(issued=day, selling_date=day, payment_date=day)
         i1.copy_from_order(o1)
         i1.set_issuer_invoice_data()
         i1.set_buyer_invoice_data(o1.user.billinginfo)
@@ -581,109 +697,124 @@
         self.assertEqual(i.tax, o.tax)
         self.assertEqual(i.tax_total, o.total() - o.amount)
         self.assertEqual(i.currency, o.currency)
 
 
 @transaction.atomic
 def complete_order():
-    user = User.objects.get(username='test1')
+    user = User.objects.get(username="test1")
 
     plan_pricing = PlanPricing.objects.all()[0]
-    o1 = Order(user=user, plan=plan_pricing.plan,
-               pricing=plan_pricing.pricing, amount=plan_pricing.price,
-               )
+    o1 = Order(
+        user=user,
+        plan=plan_pricing.plan,
+        pricing=plan_pricing.pricing,
+        amount=plan_pricing.price,
+    )
     o1.save()
     with freeze_time(random.choice(["2012-01-14", "2012-02-14"])):
         o1.complete_order()
 
 
 def complete_concrete_order(order_id):
     order = Order.objects.get(id=order_id)
     order.complete_order()
 
 
 class ConcurrentTestInvoice(TransactionTestCase):
-    fixtures = ['initial_plan', 'test_django-plans_auth', 'test_django-plans_plans']
+    fixtures = ["initial_plan", "test_django-plans_auth", "test_django-plans_plans"]
 
     def test_invoice_number_monthly_duplicity(self):
         """
         Test for problem where two simultaneously created invoices had duplicate number
         """
         call_concurrently(15, complete_order)
-        invoices = Invoice.objects.filter(type=Invoice.INVOICE_TYPES.INVOICE).order_by("issued", "number")
+        invoices = Invoice.objects.filter(type=Invoice.INVOICE_TYPES.INVOICE).order_by(
+            "issued", "number"
+        )
 
         first_december_number = 0
         for i in range(1, 15):
             invoice = invoices[i - 1]
             if invoice.issued.month == 2 and first_december_number == 0:
                 first_december_number = i - 1
             invoice_number = i - first_december_number
             self.assertEqual(invoice.number, invoice_number)
-            self.assertEqual(invoice.full_number, f"{invoice_number}/FV/0{1 if first_december_number == 0 else 2}/2012")
+            self.assertEqual(
+                invoice.full_number,
+                f"{invoice_number}/FV/0{1 if first_december_number == 0 else 2}/2012",
+            )
 
     def test_duplicate_invoices(self):
         """
         Order.complete_order should not create duplicate invoice if called concurrently
         """
         biling_info = baker.make(BillingInfo)
         for i in range(20):  # Try this more times to increase chance of failure
             order = baker.make(Order, user=biling_info.user)
             Invoice.objects.all().delete()
             call_concurrently(3, complete_concrete_order, order_id=order.id)
             self.assertEqual(Invoice.objects.count(), 1)
 
 
 class OrderTestCase(TestCase):
-    fixtures = ['initial_plan', 'test_django-plans_auth', 'test_django-plans_plans']
+    fixtures = ["initial_plan", "test_django-plans_auth", "test_django-plans_plans"]
 
     def test_order_complete_order(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=50)
         u.userplan.active = False
         u.userplan.save()
         plan_pricing = PlanPricing.objects.get(plan=u.userplan.plan, pricing__period=30)
         order = Order.objects.create(
             user=u,
             pricing=plan_pricing.pricing,
             amount=100,
             plan=plan_pricing.plan,
         )
         self.assertTrue(order.complete_order())
-        self.assertEqual(u.userplan.expire,
-                         date.today() + timedelta(days=50) + timedelta(days=plan_pricing.pricing.period))
+        self.assertEqual(
+            u.userplan.expire,
+            date.today()
+            + timedelta(days=50)
+            + timedelta(days=plan_pricing.pricing.period),
+        )
         self.assertEqual(u.userplan.plan, plan_pricing.plan)
         self.assertEqual(u.userplan.active, True)
         self.assertEqual(order.status, 2)  # completed
         self.assertEqual(order.plan_extended_from, date.today() + timedelta(days=50))
-        self.assertEqual(order.plan_extended_until, date.today() + timedelta(days=50) +
-                         timedelta(days=plan_pricing.pricing.period))
+        self.assertEqual(
+            order.plan_extended_until,
+            date.today()
+            + timedelta(days=50)
+            + timedelta(days=plan_pricing.pricing.period),
+        )
         self.assertEqual(len(mail.outbox), 3)
 
     def test_order_complete_order_invalid(self):
-        u = User.objects.get(username='test1')
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=5)
         u.userplan.active = False
         u.userplan.save()
         plan_pricing = PlanPricing.objects.get(plan=u.userplan.plan, pricing__period=30)
         order = Order.objects.create(
             user=u,
             pricing=plan_pricing.pricing,
             amount=100,
             plan=PlanPricing.objects.all()[0].plan,
         )
         self.assertTrue(order.complete_order())
-        self.assertEqual(u.userplan.expire,
-                         date.today() + timedelta(days=5))
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=5))
         self.assertEqual(u.userplan.plan, plan_pricing.plan)
         self.assertEqual(u.userplan.active, False)
         self.assertEqual(order.status, 3)  # not valid
 
     def test_order_complete_order_completed(self):
-        """ Completed order doesn't get completed any more """
-        u = User.objects.get(username='test1')
+        """Completed order doesn't get completed any more"""
+        u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=50)
         u.userplan.active = False
         u.userplan.save()
         plan_pricing = PlanPricing.objects.get(plan=u.userplan.plan, pricing__period=30)
         order = Order.objects.create(
             user=u,
             pricing=plan_pricing.pricing,
@@ -693,230 +824,254 @@
         )
         self.assertFalse(order.complete_order())
 
     def test_amount_taxed_none(self):
         o = Order()
         o.amount = Decimal(123)
         o.tax = None
-        self.assertEqual(o.total(), Decimal('123'))
+        self.assertEqual(o.total(), Decimal("123"))
 
     def test_amount_taxed_0(self):
         o = Order()
         o.amount = Decimal(123)
         o.tax = Decimal(0)
-        self.assertEqual(o.total(), Decimal('123'))
+        self.assertEqual(o.total(), Decimal("123"))
 
     def test_amount_taxed_23(self):
         o = Order()
         o.amount = Decimal(123)
         o.tax = Decimal(23)
-        self.assertEqual(o.total(), Decimal('151.29'))
+        self.assertEqual(o.total(), Decimal("151.29"))
 
 
 class PlanChangePolicyTestCase(TestCase):
-    fixtures = ['initial_plan', 'test_django-plans_auth', 'test_django-plans_plans']
+    fixtures = ["initial_plan", "test_django-plans_auth", "test_django-plans_plans"]
 
     def setUp(self):
         self.policy = PlanChangePolicy()
 
     def test_calculate_day_cost(self):
         plan = Plan.objects.get(pk=5)
-        self.assertEqual(self.policy._calculate_day_cost(plan, 13), Decimal('6.67'))
+        self.assertEqual(self.policy._calculate_day_cost(plan, 13), Decimal("6.67"))
 
     def test_get_change_price(self):
         p1 = Plan.objects.get(pk=3)
         p2 = Plan.objects.get(pk=4)
-        self.assertEqual(self.policy.get_change_price(p1, p2, 23), Decimal('7.82'))
+        self.assertEqual(self.policy.get_change_price(p1, p2, 23), Decimal("7.82"))
         self.assertEqual(self.policy.get_change_price(p2, p1, 23), None)
 
     def test_get_change_price1(self):
         p1 = Plan.objects.get(pk=3)
         p2 = Plan.objects.get(pk=4)
-        self.assertEqual(self.policy.get_change_price(p1, p2, 53), Decimal('18.02'))
+        self.assertEqual(self.policy.get_change_price(p1, p2, 53), Decimal("18.02"))
         self.assertEqual(self.policy.get_change_price(p2, p1, 53), None)
 
     def test_get_change_price2(self):
         p1 = Plan.objects.get(pk=3)
         p2 = Plan.objects.get(pk=4)
         self.assertEqual(self.policy.get_change_price(p1, p2, -53), None)
         self.assertEqual(self.policy.get_change_price(p1, p2, 0), None)
 
 
 class StandardPlanChangePolicyTestCase(TestCase):
-    fixtures = ['initial_plan', 'test_django-plans_auth', 'test_django-plans_plans']
+    fixtures = ["initial_plan", "test_django-plans_auth", "test_django-plans_plans"]
 
     def setUp(self):
         self.policy = StandardPlanChangePolicy()
 
     def test_get_change_price(self):
         p1 = Plan.objects.get(pk=3)
         p2 = Plan.objects.get(pk=4)
-        self.assertEqual(self.policy.get_change_price(p1, p2, 23), Decimal('8.60'))
+        self.assertEqual(self.policy.get_change_price(p1, p2, 23), Decimal("8.60"))
         self.assertEqual(self.policy.get_change_price(p2, p1, 23), None)
 
 
 class EUTaxationPolicyTestCase(TestCase):
     def setUp(self):
         self.policy = EUTaxationPolicy()
 
     def test_none(self):
-        with self.settings(PLANS_TAX=Decimal('23.0'), PLANS_TAX_COUNTRY='PL'):
-            self.assertEqual(self.policy.get_tax_rate(None, None), (Decimal('23.0'), True))
+        with self.settings(PLANS_TAX=Decimal("23.0"), PLANS_TAX_COUNTRY="PL"):
+            self.assertEqual(
+                self.policy.get_tax_rate(None, None), (Decimal("23.0"), True)
+            )
 
     def test_private_nonEU(self):
-        with self.settings(PLANS_TAX=Decimal('23.0'), PLANS_TAX_COUNTRY='PL'):
-            self.assertEqual(self.policy.get_tax_rate(None, 'RU'), (None, True))
+        with self.settings(PLANS_TAX=Decimal("23.0"), PLANS_TAX_COUNTRY="PL"):
+            self.assertEqual(self.policy.get_tax_rate(None, "RU"), (None, True))
 
     def test_private_EU_same(self):
-        with self.settings(PLANS_TAX=Decimal('23.0'), PLANS_TAX_COUNTRY='PL'):
-            self.assertEqual(self.policy.get_tax_rate(None, 'PL'), (Decimal('23.0'), True))
+        with self.settings(PLANS_TAX=Decimal("23.0"), PLANS_TAX_COUNTRY="PL"):
+            self.assertEqual(
+                self.policy.get_tax_rate(None, "PL"), (Decimal("23.0"), True)
+            )
 
     def test_private_EU_notsame(self):
-        with self.settings(PLANS_TAX=Decimal('23.0'), PLANS_TAX_COUNTRY='PL'):
-            self.assertEqual(self.policy.get_tax_rate(None, 'AT'), (Decimal('20.0'), True))
+        with self.settings(PLANS_TAX=Decimal("23.0"), PLANS_TAX_COUNTRY="PL"):
+            self.assertEqual(
+                self.policy.get_tax_rate(None, "AT"), (Decimal("20.0"), True)
+            )
 
     def test_company_nonEU(self):
-        with self.settings(PLANS_TAX=Decimal('23.0'), PLANS_TAX_COUNTRY='PL'):
-            self.assertEqual(self.policy.get_tax_rate('123456', 'RU'), (None, True))
+        with self.settings(PLANS_TAX=Decimal("23.0"), PLANS_TAX_COUNTRY="PL"):
+            self.assertEqual(self.policy.get_tax_rate("123456", "RU"), (None, True))
 
     def test_company_EU_same(self):
-        with self.settings(PLANS_TAX=Decimal('23.0'), PLANS_TAX_COUNTRY='PL'):
-            self.assertEqual(self.policy.get_tax_rate('123456', 'PL'), (Decimal('23.0'), True))
+        with self.settings(PLANS_TAX=Decimal("23.0"), PLANS_TAX_COUNTRY="PL"):
+            self.assertEqual(
+                self.policy.get_tax_rate("123456", "PL"), (Decimal("23.0"), True)
+            )
 
     def test_company_EU_GR_vies_tax(self):
         """
         Test, that greece has VAT OK. Greece has code GR in django-countries, but EL in VIES
         Tax ID is not valid VAT ID, so tax is counted
         """
-        self.assertEqual(self.policy.get_tax_rate('123456', 'GR'), (24, False))
+        self.assertEqual(self.policy.get_tax_rate("123456", "GR"), (24, False))
 
     @mock.patch("stdnum.eu.vat.check_vies")
     def test_company_EU_GR_vies_zero(self, mock_check):
         """
         Test, that greece has VAT OK. Greece has code GR in django-countries, but EL in VIES
         Tax ID is valid VAT ID, so no tax is counted
         """
-        mock_check.return_value = {'valid': True}
-        self.assertEqual(self.policy.get_tax_rate('EL090145420', 'GR'), (None, True))
+        mock_check.return_value = {"valid": True}
+        self.assertEqual(self.policy.get_tax_rate("EL090145420", "GR"), (None, True))
 
     @mock.patch("stdnum.eu.vat.check_vies")
     def test_company_EU_notsame_vies_ok(self, mock_check):
-        mock_check.return_value = {'valid': True}
-        with self.settings(PLANS_TAX=Decimal('23.0'), PLANS_TAX_COUNTRY='PL'):
-            self.assertEqual(self.policy.get_tax_rate('123456', 'AT'), (None, True))
+        mock_check.return_value = {"valid": True}
+        with self.settings(PLANS_TAX=Decimal("23.0"), PLANS_TAX_COUNTRY="PL"):
+            self.assertEqual(self.policy.get_tax_rate("123456", "AT"), (None, True))
 
     @mock.patch("stdnum.eu.vat.check_vies")
     def test_company_EU_notsame_vies_not_ok(self, mock_check):
-        mock_check.return_value = {'valid': False}
-        with self.settings(PLANS_TAX=Decimal('23.0'), PLANS_TAX_COUNTRY='PL'):
-            self.assertEqual(self.policy.get_tax_rate('123456', 'AT'), (Decimal('20.0'), True))
+        mock_check.return_value = {"valid": False}
+        with self.settings(PLANS_TAX=Decimal("23.0"), PLANS_TAX_COUNTRY="PL"):
+            self.assertEqual(
+                self.policy.get_tax_rate("123456", "AT"), (Decimal("20.0"), True)
+            )
 
 
 class BillingInfoTestCase(TestCase):
     def test_clean_tax_number(self):
         with self.assertRaises(ValidationError):
-            BillingInfo.clean_tax_number('123456', 'CZ')
+            BillingInfo.clean_tax_number("123456", "CZ")
 
     def test_clean_tax_number_valid(self):
-        self.assertEqual(BillingInfo.clean_tax_number('48136450', 'CZ'), 'CZ48136450')
+        self.assertEqual(BillingInfo.clean_tax_number("48136450", "CZ"), "CZ48136450")
 
     def test_clean_tax_number_valid_space(self):
-        self.assertEqual(BillingInfo.clean_tax_number('48 136 450', 'CZ'), 'CZ48136450')
+        self.assertEqual(BillingInfo.clean_tax_number("48 136 450", "CZ"), "CZ48136450")
 
     def test_clean_tax_number_valid_with_country(self):
-        self.assertEqual(BillingInfo.clean_tax_number('CZ48136450', 'CZ'), 'CZ48136450')
+        self.assertEqual(BillingInfo.clean_tax_number("CZ48136450", "CZ"), "CZ48136450")
 
     def test_clean_tax_number_valid_with_country_GR(self):
-        self.assertEqual(BillingInfo.clean_tax_number('GR104594676', 'GR'), 'EL104594676')
+        self.assertEqual(
+            BillingInfo.clean_tax_number("GR104594676", "GR"), "EL104594676"
+        )
 
     def test_clean_tax_number_valid_with_country_EL(self):
-        self.assertEqual(BillingInfo.clean_tax_number('EL104594676', 'GR'), 'EL104594676')
+        self.assertEqual(
+            BillingInfo.clean_tax_number("EL104594676", "GR"), "EL104594676"
+        )
 
     def test_clean_tax_number_vat_id_is_not_correct(self):
-        with self.assertRaisesRegex(ValidationError, 'VAT ID is not correct'):
-            BillingInfo.clean_tax_number('GR48136450', 'GR')
+        with self.assertRaisesRegex(ValidationError, "VAT ID is not correct"):
+            BillingInfo.clean_tax_number("GR48136450", "GR")
 
     def test_clean_tax_number_country_code_does_not_equal_as_country(self):
-        with self.assertRaisesRegex(ValidationError, 'VAT ID country code doesn\'t corespond with country'):
-            BillingInfo.clean_tax_number('AT48136450', 'CZ')
+        with self.assertRaisesRegex(
+            ValidationError, "VAT ID country code doesn't corespond with country"
+        ):
+            BillingInfo.clean_tax_number("AT48136450", "CZ")
 
 
 def timeout(*args, **kwargs):
     raise requests.Timeout
 
 
 class CreateOrderViewTestCase(TestCase):
     def setUp(self):
         self.factory = RequestFactory()
-        request = self.factory.get('')
+        request = self.factory.get("")
         middleware = SessionMiddleware(lambda x: x)
         middleware.process_request(request)
         messages = FallbackStorage(request)
-        setattr(request, '_messages', messages)
+        setattr(request, "_messages", messages)
         self.create_view = CreateOrderView()
         self.create_view.request = request
 
     def test_recalculate_order_no_connection(self):
         # VAT is right, but with no internet connection
         with no_connection():
-            with patch('plans.taxation.eu.logger') as mock_logger:
-                o = self.create_view.recalculate(10, BillingInfo(tax_number='48136450', country='CZ'))
+            with patch("plans.taxation.eu.logger") as mock_logger:
+                o = self.create_view.recalculate(
+                    10, BillingInfo(tax_number="48136450", country="CZ")
+                )
                 self.assertEqual(o.tax, 21)
                 mock_logger.exception.assert_called_with("TAX_ID=CZ48136450")
         message = self.create_view.request._messages._queued_messages[0].message
         self.assertEqual(
             message,
-            'There was an error during determining validity of your VAT ID.<br/>'
-            'If you think, you have european VAT ID and should not be taxed, '
-            'please try resaving billing info later.<br/><br/>'
-            'European VAT Information Exchange System throw following error: '
-            '&lt;urlopen error Internet is disabled&gt;',
+            "There was an error during determining validity of your VAT ID.<br/>"
+            "If you think, you have european VAT ID and should not be taxed, "
+            "please try resaving billing info later.<br/><br/>"
+            "European VAT Information Exchange System throw following error: "
+            "&lt;urlopen error Internet is disabled&gt;",
         )
 
     @mock.patch("stdnum.eu.vat.check_vies")
     def test_recalculate_order(self, mock_check):
-        mock_check.return_value = {'valid': True}
+        mock_check.return_value = {"valid": True}
         # BE 0203.201.340 is VAT ID of Belgium national bank.
         # It is used, because national provider for VIES seems to be stable enough
         c = self.create_view
-        o = c.recalculate(10, BillingInfo(tax_number='BE 0203 201 340', country='BE'))
+        o = c.recalculate(10, BillingInfo(tax_number="BE 0203 201 340", country="BE"))
         self.assertEqual(o.tax, None)
 
-        o = c.recalculate(10, BillingInfo(tax_number='0203 201 340', country='BE'))
+        o = c.recalculate(10, BillingInfo(tax_number="0203 201 340", country="BE"))
         self.assertEqual(o.tax, None)
 
-        mock_check.return_value = {'valid': False}
-        o = c.recalculate(10, BillingInfo(tax_number='1234565', country='BE'))
+        mock_check.return_value = {"valid": False}
+        o = c.recalculate(10, BillingInfo(tax_number="1234565", country="BE"))
         self.assertEqual(o.tax, 21)
 
-        o = c.recalculate(10, BillingInfo(tax_number='1234567', country='GR'))
+        o = c.recalculate(10, BillingInfo(tax_number="1234567", country="GR"))
         self.assertEqual(o.tax, 24)
 
-        mock_check.return_value = {'valid': True}
-        o = c.recalculate(10, BillingInfo(tax_number='090145420', country='GR'))
+        mock_check.return_value = {"valid": True}
+        o = c.recalculate(10, BillingInfo(tax_number="090145420", country="GR"))
         self.assertEqual(o.tax, None)
 
 
 class ValidatorsTestCase(TestCase):
-    fixtures = ['test_django-plans_auth']
+    fixtures = ["test_django-plans_auth"]
 
     def test_model_count_validator(self):
         """
         We create a test model validator for User. It will raise ValidationError when QUOTA_NAME value
         will be lower than number of elements of model User.
         """
 
         class TestValidator(ModelCountValidator):
-            code = 'QUOTA_NAME'
+            code = "QUOTA_NAME"
             model = User
 
         validator_object = TestValidator()
-        self.assertRaises(ValidationError, validator_object, user=None, quota_dict={'QUOTA_NAME': 1})
-        self.assertEqual(validator_object(user=None, quota_dict={'QUOTA_NAME': 2}), None)
-        self.assertEqual(validator_object(user=None, quota_dict={'QUOTA_NAME': 3}), None)
+        self.assertRaises(
+            ValidationError, validator_object, user=None, quota_dict={"QUOTA_NAME": 1}
+        )
+        self.assertEqual(
+            validator_object(user=None, quota_dict={"QUOTA_NAME": 2}), None
+        )
+        self.assertEqual(
+            validator_object(user=None, quota_dict={"QUOTA_NAME": 3}), None
+        )
 
         #   TODO: FIX this test not to use Pricing for testing  ModelAttributeValidator
         # def test_model_attribute_validator(self):
         #     """
         #     We create a test attribute validator which will validate if Pricing objects has a specific value set.
         #     """
         #
@@ -927,194 +1082,255 @@
         #
         #     validator_object = TestValidator()
         #     self.assertRaises(ValidationError, validator_object, user=None, quota_dict={'QUOTA_NAME': 360})
         #     self.assertEqual(validator_object(user=None, quota_dict={'QUOTA_NAME': 365}), None)
 
 
 class BillingInfoViewTestCase(TestCase):
-    fixtures = ['test_django-plans_auth']
+    fixtures = ["test_django-plans_auth"]
 
     def setUp(self):
-        self.user = User.objects.create_user('foo', 'myemail@test.com', 'bar')
-        self.client.login(username='foo', password='bar')
+        self.user = User.objects.create_user("foo", "myemail@test.com", "bar")
+        self.client.login(username="foo", password="bar")
 
     @override_settings(
         PLANS_GET_COUNTRY_FROM_IP=True,
-        PLANS_DEFAULT_COUNTRY='PL',
+        PLANS_DEFAULT_COUNTRY="PL",
     )
     def test_default_country_set(self):
         """
         Test, that default country is PL
         """
-        response = self.client.get(reverse('billing_info'))
+        response = self.client.get(reverse("billing_info"))
         self.assertEqual(response.status_code, 200)
-        self.assertContains(response, '<option value="PL" selected>Poland</option>', html=True)
+        self.assertContains(
+            response, '<option value="PL" selected>Poland</option>', html=True
+        )
 
     @override_settings(
-        PLANS_DEFAULT_COUNTRY='PL',
+        PLANS_DEFAULT_COUNTRY="PL",
     )
     def test_default_country_set_no_ip(self):
         """
         Test, that default country is PL
         """
-        response = self.client.get(reverse('billing_info'))
+        response = self.client.get(reverse("billing_info"))
         self.assertEqual(response.status_code, 200)
-        self.assertContains(response, '<option value="PL" selected>Poland</option>', html=True)
+        self.assertContains(
+            response, '<option value="PL" selected>Poland</option>', html=True
+        )
 
     @override_settings(PLANS_GET_COUNTRY_FROM_IP=True)
     def test_default_country_unset(self):
         """
         Test, that default country is None
         """
-        response = self.client.get(reverse('billing_info'))
+        response = self.client.get(reverse("billing_info"))
         self.assertEqual(response.status_code, 200)
-        self.assertContains(response, '<option value="" selected>---------</option>', html=True)
+        self.assertContains(
+            response, '<option value="" selected>---------</option>', html=True
+        )
 
     @override_settings(PLANS_GET_COUNTRY_FROM_IP=True)
     def test_default_country_by_ip(self):
         """
         Test, that default country is determined by German IP
         """
 
-        response = self.client.get(reverse('billing_info'), HTTP_X_FORWARDED_FOR='85.214.132.117')
+        response = self.client.get(
+            reverse("billing_info"), HTTP_X_FORWARDED_FOR="85.214.132.117"
+        )
         self.assertEqual(response.status_code, 200)
-        self.assertContains(response, '<option value="DE" selected>Germany</option>', html=True)
+        self.assertContains(
+            response, '<option value="DE" selected>Germany</option>', html=True
+        )
 
-        response = self.client.get(reverse('billing_info'), REMOTE_ADDR='85.214.132.117')
+        response = self.client.get(
+            reverse("billing_info"), REMOTE_ADDR="85.214.132.117"
+        )
         self.assertEqual(response.status_code, 200)
-        self.assertContains(response, '<option value="DE" selected>Germany</option>', html=True)
+        self.assertContains(
+            response, '<option value="DE" selected>Germany</option>', html=True
+        )
 
     def test_default_country_by_ip_no_settings(self):
         """
         Test, that default country is not determined
         """
 
-        response = self.client.get(reverse('billing_info'), HTTP_X_FORWARDED_FOR='85.214.132.117')
+        response = self.client.get(
+            reverse("billing_info"), HTTP_X_FORWARDED_FOR="85.214.132.117"
+        )
         self.assertEqual(response.status_code, 200)
-        self.assertContains(response, '<option value="" selected>---------</option>', html=True)
+        self.assertContains(
+            response, '<option value="" selected>---------</option>', html=True
+        )
 
     def test_billing_info(self):
         """
         Test, BillingInfoCreateOrUpdateView and BillingInfoDeleteView views
         """
         # Test get does not contain delete button
-        response = self.client.get(reverse('billing_info'))
-        self.assertNotContains(response, '<a class="btn btn-danger" href="/plan/billing/delete/">Delete</a>', html=True)
+        response = self.client.get(reverse("billing_info"))
+        self.assertNotContains(
+            response,
+            '<a class="btn btn-danger" href="/plan/billing/delete/">Delete</a>',
+            html=True,
+        )
 
         # Test create
         parameters = {
             "country": "GR",
             "tax_number": "GR104594676",
             "name": "bar",
             "street": "baz",
             "city": "bay",
             "zipcode": "bax",
         }
-        response = self.client.post(reverse('billing_info') + "?next=/plan/pricing/", parameters)
+        response = self.client.post(
+            reverse("billing_info") + "?next=/plan/pricing/", parameters
+        )
         self.assertRedirects(
-            response, '/plan/pricing/', status_code=302,
-            target_status_code=200, fetch_redirect_response=True,
+            response,
+            "/plan/pricing/",
+            status_code=302,
+            target_status_code=200,
+            fetch_redirect_response=True,
         )
         self.assertEqual(self.user.billinginfo.tax_number, "EL104594676")
 
         # Test get contains delete button
-        response = self.client.get(reverse('billing_info'))
-        self.assertContains(response, '<a class="btn btn-danger" href="/plan/billing/delete/">Delete</a>', html=True)
+        response = self.client.get(reverse("billing_info"))
+        self.assertContains(
+            response,
+            '<a class="btn btn-danger" href="/plan/billing/delete/">Delete</a>',
+            html=True,
+        )
 
         # Test update
         del parameters["tax_number"]
         parameters["name"] = "foo"
-        response = self.client.post(reverse('billing_info') + "?next=/plan/pricing/", parameters)
+        response = self.client.post(
+            reverse("billing_info") + "?next=/plan/pricing/", parameters
+        )
         self.user.billinginfo.refresh_from_db()
         self.assertEqual(self.user.billinginfo.name, "foo")
         self.assertEqual(self.user.billinginfo.tax_number, "")
 
         # Test delete
-        response = self.client.post(reverse('billing_info_delete'))
+        response = self.client.post(reverse("billing_info_delete"))
         with self.assertRaises(BillingInfo.DoesNotExist):
             self.user.billinginfo.refresh_from_db()
 
 
 class RecurringPlansTestCase(TestCase):
-
     def test_set_plan_renewal(self):
-        """ Test that UserPlan.set_plan_renewal() method """
-        up = baker.make('UserPlan')
-        o = baker.make('Order', amount=10)
+        """Test that UserPlan.set_plan_renewal() method"""
+        up = baker.make("UserPlan")
+        o = baker.make("Order", amount=10)
         up.set_plan_renewal(order=o, card_masked_number="1234")
         self.assertEqual(up.recurring.amount, 10)
         self.assertEqual(up.recurring.card_masked_number, "1234")
+        old_id = up.recurring.id
 
         # test setting new values
         up.set_plan_renewal(order=o)
         self.assertEqual(up.recurring.amount, 10)
         self.assertEqual(up.recurring.card_masked_number, None)
+        self.assertEqual(up.recurring.id, old_id)
 
     def test_plan_autorenew_at(self):
-        """ Test that UserPlan.plan_autorenew_at() method """
-        up = baker.make('UserPlan')
+        """Test that UserPlan.plan_autorenew_at() method"""
+        up = baker.make("UserPlan")
         self.assertEqual(up.plan_autorenew_at(), None)
 
     def test_plan_autorenew_at_expire(self):
-        """ Test that UserPlan.plan_autorenew_at() method """
-        up = baker.make('UserPlan', expire=date(2020, 1, 1))
+        """Test that UserPlan.plan_autorenew_at() method"""
+        up = baker.make("UserPlan", expire=date(2020, 1, 1))
         self.assertEqual(up.plan_autorenew_at(), date(2020, 1, 1))
 
     @override_settings(
         PLANS_AUTORENEW_BEFORE_DAYS=3,
         PLANS_AUTORENEW_BEFORE_HOURS=24,
     )
     def test_plan_autorenew_at_settings(self):
-        """ Test that UserPlan.plan_autorenew_at() method """
-        up = baker.make('UserPlan', expire=date(2020, 1, 5))
+        """Test that UserPlan.plan_autorenew_at() method"""
+        up = baker.make("UserPlan", expire=date(2020, 1, 5))
         self.assertEqual(up.plan_autorenew_at(), date(2020, 1, 1))
 
     def test_has_automatic_renewal(self):
-        """ Test UserPlan.has_automatic_renewal() method """
-        user_plan = baker.make('UserPlan')
-        order = baker.make('Order', amount=10)
+        """Test UserPlan.has_automatic_renewal() method"""
+        user_plan = baker.make("UserPlan")
+        order = baker.make("Order", amount=10)
         user_plan.set_plan_renewal(order=order, card_masked_number="1234")
         self.assertEqual(user_plan.has_automatic_renewal(), False)
 
         user_plan.recurring.token_verified = True
         self.assertEqual(user_plan.has_automatic_renewal(), True)
 
     def test_create_new_order(self):
         rup = baker.make(
-            'RecurringUserPlan',
-            user_plan__user__billinginfo__country='CZ',
+            "RecurringUserPlan",
+            user_plan__user__billinginfo__country="CZ",
             amount=10,
         )
         order = rup.create_renew_order()
         self.assertEqual(order.tax, 21)
         self.assertEqual(rup.tax, 21)
 
     def test_create_new_order_VIES_fault(self):
-        """ If VIES fails, we use last available TAX value """
+        """If VIES fails, we use last available TAX value"""
         rup = baker.make(
-            'RecurringUserPlan',
-            user_plan__user__billinginfo__country='CZ',
+            "RecurringUserPlan",
+            user_plan__user__billinginfo__country="CZ",
             user_plan__user__billinginfo__tax_number="CZ0123",
             amount=10,
             tax=11,
         )
         with no_connection():
             order = rup.create_renew_order()
         self.assertEqual(order.tax, 11)
 
 
 class TasksTestCase(TestCase):
+    def setUp(self):
+        self.user = baker.make("User", email="foo@bar.cz", username="foo bar")
+
     def test_expire_account_task(self):
-        order = baker.make('Order', amount=10)
-        userplan = baker.make('UserPlan', user=baker.make('User'))
+        order = baker.make("Order", amount=10)
+        userplan = baker.make("UserPlan", user=self.user)
         userplan.expire = date.today() - timedelta(days=1)
         userplan.active = True
 
         # If the automatic renewal didn't go through, even automatic renewal plans has to go
         userplan.set_plan_renewal(order=order, card_masked_number="1234")
 
         userplan.save()
         tasks.expire_account()
 
         userplan.refresh_from_db()
         self.assertEqual(userplan.active, False)
-        # self.assertEqual(len(mail.outbox), 1)
+        self.assertEqual(len(mail.outbox), 1)
+        self.assertEqual(
+            mail.outbox[0].subject, "Your account foo bar has just expired"
+        )
+
+    @override_settings(PLANS_EXPIRATION_REMIND=[3])
+    def test_expire_account_task_notify(self):
+        order = baker.make("Order", amount=10)
+        userplan = baker.make("UserPlan", user=self.user)
+        userplan.expire = date.today() + timedelta(days=3)
+        userplan.active = True
+
+        # If the automatic renewal didn't go through, even automatic renewal plans has to go
+        userplan.set_plan_renewal(order=order, card_masked_number="1234")
+
+        userplan.save()
+        tasks.expire_account()
+
+        userplan.refresh_from_db()
+        self.assertEqual(userplan.active, True)
+        self.assertEqual(len(mail.outbox), 1)
+        self.assertEqual(
+            mail.outbox[0].subject,
+            "Your account foo bar will expire in 3 days",
+        )
```

### Comparing `django-plans-1.0.4/plans/urls.py` & `django-plans-1.0.5/plans/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,74 @@
 from django.conf import settings
 from django.urls import path
 
-from plans.views import (AccountActivationView, BillingInfoCreateOrUpdateView,
-                         BillingInfoDeleteView, ChangePlanView,
-                         CreateOrderPlanChangeView, CreateOrderView,
-                         CurrentPlanView, FakePaymentsView, InvoiceDetailView,
-                         OrderListView, OrderPaymentReturnView, OrderView,
-                         PricingView, RedirectToBilling, UpgradePlanView)
+from plans.views import (
+    AccountActivationView,
+    BillingInfoCreateOrUpdateView,
+    BillingInfoDeleteView,
+    ChangePlanView,
+    CreateOrderPlanChangeView,
+    CreateOrderView,
+    CurrentPlanView,
+    FakePaymentsView,
+    InvoiceDetailView,
+    OrderListView,
+    OrderPaymentReturnView,
+    OrderView,
+    PricingView,
+    RedirectToBilling,
+    UpgradePlanView,
+)
 
 urlpatterns = [
-    path('pricing/', PricingView.as_view(), name='pricing'),
-    path('account/', CurrentPlanView.as_view(), name='current_plan'),
-    path('account/activation/', AccountActivationView.as_view(), name='account_activation'),
-    path('upgrade/', UpgradePlanView.as_view(), name='upgrade_plan'),
-    path('order/extend/new/<int:pk>/', CreateOrderView.as_view(), name='create_order_plan'),
-    path('order/upgrade/new/<int:pk>/', CreateOrderPlanChangeView.as_view(), name='create_order_plan_change'),
-    path('change/<int:pk>/', ChangePlanView.as_view(), name='change_plan'),
-    path('order/', OrderListView.as_view(), name='order_list'),
-    path('order/<int:pk>/', OrderView.as_view(), name='order'),
-    path('order/<int:pk>/payment/success/', OrderPaymentReturnView.as_view(status='success'),
-         name='order_payment_success'),
-    path('order/<int:pk>/payment/failure/', OrderPaymentReturnView.as_view(status='failure'),
-         name='order_payment_failure'),
+    path("pricing/", PricingView.as_view(), name="pricing"),
+    path("account/", CurrentPlanView.as_view(), name="current_plan"),
+    path(
+        "account/activation/",
+        AccountActivationView.as_view(),
+        name="account_activation",
+    ),
+    path("upgrade/", UpgradePlanView.as_view(), name="upgrade_plan"),
+    path(
+        "order/extend/new/<int:pk>/",
+        CreateOrderView.as_view(),
+        name="create_order_plan",
+    ),
+    path(
+        "order/upgrade/new/<int:pk>/",
+        CreateOrderPlanChangeView.as_view(),
+        name="create_order_plan_change",
+    ),
+    path("change/<int:pk>/", ChangePlanView.as_view(), name="change_plan"),
+    path("order/", OrderListView.as_view(), name="order_list"),
+    path("order/<int:pk>/", OrderView.as_view(), name="order"),
+    path(
+        "order/<int:pk>/payment/success/",
+        OrderPaymentReturnView.as_view(status="success"),
+        name="order_payment_success",
+    ),
+    path(
+        "order/<int:pk>/payment/failure/",
+        OrderPaymentReturnView.as_view(status="failure"),
+        name="order_payment_failure",
+    ),
     # Redirect for backward compatibility:
-    path('billing/create/', RedirectToBilling.as_view(), name='billing_info_create'),
+    path("billing/create/", RedirectToBilling.as_view(), name="billing_info_create"),
     # Redirect for backward compatibility:
-    path('billing/update/', RedirectToBilling.as_view(), name='billing_info_update'),
-    path('billing/', BillingInfoCreateOrUpdateView.as_view(), name='billing_info'),
-    path('billing/delete/', BillingInfoDeleteView.as_view(), name='billing_info_delete'),
-    path('invoice/<int:pk>/preview/html/', InvoiceDetailView.as_view(), name='invoice_preview_html'),
+    path("billing/update/", RedirectToBilling.as_view(), name="billing_info_update"),
+    path("billing/", BillingInfoCreateOrUpdateView.as_view(), name="billing_info"),
+    path(
+        "billing/delete/", BillingInfoDeleteView.as_view(), name="billing_info_delete"
+    ),
+    path(
+        "invoice/<int:pk>/preview/html/",
+        InvoiceDetailView.as_view(),
+        name="invoice_preview_html",
+    ),
 ]
 
-if getattr(settings, 'DEBUG', False) or getattr(settings, 'ENABLE_FAKE_PAYMENTS', True):
+if getattr(settings, "DEBUG", False) or getattr(settings, "ENABLE_FAKE_PAYMENTS", True):
     urlpatterns += [
-        path('fakepayments/<int:pk>/', FakePaymentsView.as_view(), name='fake_payments'),
+        path(
+            "fakepayments/<int:pk>/", FakePaymentsView.as_view(), name="fake_payments"
+        ),
     ]
```

### Comparing `django-plans-1.0.4/plans/utils.py` & `django-plans-1.0.5/plans/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 
 
 def get_client_ip(request):
-    x_forwarded_for = request.META.get('HTTP_X_FORWARDED_FOR')
+    x_forwarded_for = request.META.get("HTTP_X_FORWARDED_FOR")
     if x_forwarded_for:
-        ip = x_forwarded_for.split(',')[0]
+        ip = x_forwarded_for.split(",")[0]
     else:
-        ip = request.META.get('REMOTE_ADDR')
+        ip = request.META.get("REMOTE_ADDR")
     return ip
 
 
 def get_country_code(request):
-    if getattr(settings, 'PLANS_GET_COUNTRY_FROM_IP', False):
+    if getattr(settings, "PLANS_GET_COUNTRY_FROM_IP", False):
         try:
             from geolite2 import geolite2
 
             reader = geolite2.reader()
             ip_address = get_client_ip(request)
             ip_info = reader.get(ip_address)
         except ModuleNotFoundError:
             ip_info = None
 
-        if ip_info and 'country' in ip_info:
-            country_code = ip_info['country']['iso_code']
+        if ip_info and "country" in ip_info:
+            country_code = ip_info["country"]["iso_code"]
             return country_code
-    return getattr(settings, 'PLANS_DEFAULT_COUNTRY', None)
+    return getattr(settings, "PLANS_DEFAULT_COUNTRY", None)
 
 
 def get_currency():
-    CURRENCY = getattr(settings, 'PLANS_CURRENCY', '')
+    CURRENCY = getattr(settings, "PLANS_CURRENCY", "")
     if len(CURRENCY) != 3:
-        raise ImproperlyConfigured('PLANS_CURRENCY should be configured as 3-letter currency code.')
+        raise ImproperlyConfigured(
+            "PLANS_CURRENCY should be configured as 3-letter currency code."
+        )
     return CURRENCY
 
 
 def country_code_transform(country_code):
-    """ Transform country code to the code used by VIES """
+    """Transform country code to the code used by VIES"""
     transform_dict = {
         "GR": "EL",
     }
     return transform_dict.get(country_code, country_code)
```

### Comparing `django-plans-1.0.4/plans/validators.py` & `django-plans-1.0.5/plans/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,39 +13,39 @@
     """
 
     required_to_activate = True
     default_quota_value = None
 
     @property
     def code(self):
-        raise ImproperlyConfigured('Quota code name is not provided for validator')
+        raise ImproperlyConfigured("Quota code name is not provided for validator")
 
     def get_quota_value(self, user, quota_dict=None):
         """
         Returns quota value for a given user
         """
         if quota_dict is None:
             quota_dict = get_user_quota(user)
 
         return quota_dict.get(self.code, self.default_quota_value)
 
     def get_error_message(self, quota_value, **kwargs):
-        return u'Plan validation error'
+        return "Plan validation error"
 
     def get_error_params(self, quota_value, **kwargs):
         return {
-            'quota': quota_value,
-            'validator_codename': self.code,
+            "quota": quota_value,
+            "validator_codename": self.code,
         }
 
     def __call__(self, user, quota_dict=None, **kwargs):
         """
         Performs validation of quota limit for a user account
         """
-        raise NotImplementedError('Please implement specific QuotaValidator')
+        raise NotImplementedError("Please implement specific QuotaValidator")
 
     def on_activation(self, user, quota_dict=None, **kwargs):
         """
         Hook for any action that validator needs to do while successful activation of the plan
         Most useful for validators not required to activate, e.g. some "option" is turned ON for user
         but when user downgrade plan this option should be turned OFF automatically rather than
         stops account activation
@@ -56,77 +56,91 @@
 class ModelCountValidator(QuotaValidator):
     """
     Validator that checks if there is no more than quota number of objects given model
     """
 
     @property
     def model(self):
-        raise ImproperlyConfigured('ModelCountValidator requires model name')
+        raise ImproperlyConfigured("ModelCountValidator requires model name")
 
     def get_queryset(self, user):
         return self.model.objects.all()
 
     def get_error_message(self, quota_value, **kwargs):
-        return _('Limit of %(model_name_plural)s exceeded. The limit is %(quota)s items.')
+        return _(
+            "Limit of %(model_name_plural)s exceeded. The limit is %(quota)s items."
+        )
 
     def get_error_params(self, quota_value, total_count, **kwargs):
         return {
-            'quota': quota_value,
-            'model_name_plural': self.model._meta.verbose_name_plural.title().lower(),
-            'validator_codename': self.code,
-            'total_count': total_count,
+            "quota": quota_value,
+            "model_name_plural": self.model._meta.verbose_name_plural.title().lower(),
+            "validator_codename": self.code,
+            "total_count": total_count,
         }
 
     def __call__(self, user, quota_dict=None, **kwargs):
         quota = self.get_quota_value(user, quota_dict)
-        total_count = self.get_queryset(user).count() + kwargs.get('add', 0)
+        total_count = self.get_queryset(user).count() + kwargs.get("add", 0)
         if quota is not None and total_count > quota:
-            raise ValidationError(message=self.get_error_message(
-                quota), params=self.get_error_params(quota, total_count))
+            raise ValidationError(
+                message=self.get_error_message(quota),
+                params=self.get_error_params(quota, total_count),
+            )
 
 
 class ModelAttributeValidator(ModelCountValidator):
     """
     Validator checks if every obj.attribute value for a given model satisfy condition
     provided in check_attribute_value() method.
 
     .. warning::
         ModelAttributeValidator requires `get_absolute_url()` method on provided model.
     """
 
     @property
     def attribute(self):
-        raise ImproperlyConfigured('ModelAttributeValidator requires defining attribute name')
+        raise ImproperlyConfigured(
+            "ModelAttributeValidator requires defining attribute name"
+        )
 
     def check_attribute_value(self, attribute_value, quota_value):
         # default is to value is <= limit
         return attribute_value <= quota_value
 
     def get_error_message(self, quota_value, **kwargs):
-        return _('Following %(model_name_plural)s are not in limits: %(objects)s')
+        return _("Following %(model_name_plural)s are not in limits: %(objects)s")
 
     def get_error_params(self, quota_value, total_count, **kwargs):
         return {
-            'quota': quota_value,
-            'validator_codename': self.code,
-            'model_name_plural': self.model._meta.verbose_name_plural.title().lower(),
-            'objects': u', '.join(map(lambda o: u'<a href="%s">%s</a>' % (o.get_absolute_url(), six.u(o)),
-                                      kwargs['not_valid_objects'])),
+            "quota": quota_value,
+            "validator_codename": self.code,
+            "model_name_plural": self.model._meta.verbose_name_plural.title().lower(),
+            "objects": ", ".join(
+                map(
+                    lambda o: '<a href="%s">%s</a>' % (o.get_absolute_url(), six.u(o)),
+                    kwargs["not_valid_objects"],
+                )
+            ),
         }
 
     def __call__(self, user, quota_dict=None, **kwargs):
         quota_value = self.get_quota_value(user, quota_dict)
         not_valid_objects = []
         if quota_value is not None:
             for obj in self.get_queryset(user):
-                if not self.check_attribute_value(getattr(obj, self.attribute), quota_value):
+                if not self.check_attribute_value(
+                    getattr(obj, self.attribute), quota_value
+                ):
                     not_valid_objects.append(obj)
         if not_valid_objects:
             raise ValidationError(
-                self.get_error_message(quota_value, not_valid_objects=not_valid_objects),
+                self.get_error_message(
+                    quota_value, not_valid_objects=not_valid_objects
+                ),
                 self.get_error_params(quota_value, not_valid_objects=not_valid_objects),
             )
 
 
 def plan_validation(user, plan=None, on_activation=False):
     """
     Validates validator that represents quotas in a given system
@@ -134,28 +148,28 @@
     :param plan:
     :return:
     """
     if plan is None:
         # if plan is not given, the default is to use current plan of the user
         plan = user.userplan.plan
     quota_dict = plan.get_quota_dict()
-    validators = getattr(settings, 'PLANS_VALIDATORS', {})
+    validators = getattr(settings, "PLANS_VALIDATORS", {})
     validators = import_name(validators)
     errors = {
-        'required_to_activate': [],
-        'other': [],
+        "required_to_activate": [],
+        "other": [],
     }
 
     for quota in validators:
         validator = import_name(validators[quota])
 
         if on_activation:
             validator.on_activation(user, quota_dict)
         else:
             try:
                 validator(user, quota_dict)
             except ValidationError as e:
                 if validator.required_to_activate:
-                    errors['required_to_activate'].extend(e.messages)
+                    errors["required_to_activate"].extend(e.messages)
                 else:
-                    errors['other'].extend(e.messages)
+                    errors["other"].extend(e.messages)
     return errors
```

### Comparing `django-plans-1.0.4/plans/views.py` & `django-plans-1.0.5/plans/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,37 @@
 from django.core.exceptions import ImproperlyConfigured
 from django.db.models import Q
 from django.http import Http404, HttpResponseForbidden, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.urls import reverse, reverse_lazy
 from django.utils.translation import gettext_lazy as _
 from django.views.generic import CreateView, RedirectView, TemplateView, View
-from django.views.generic.detail import (DetailView, SingleObjectMixin,
-                                         SingleObjectTemplateResponseMixin)
-from django.views.generic.edit import (DeleteView, FormView, ModelFormMixin,
-                                       ProcessFormView)
+from django.views.generic.detail import (
+    DetailView,
+    SingleObjectMixin,
+    SingleObjectTemplateResponseMixin,
+)
+from django.views.generic.edit import (
+    DeleteView,
+    FormView,
+    ModelFormMixin,
+    ProcessFormView,
+)
 from django.views.generic.list import ListView
 from next_url_mixin.mixin import NextUrlMixin
 
-from plans.base.models import (AbstractBillingInfo, AbstractInvoice,
-                               AbstractOrder, AbstractPlan,
-                               AbstractPlanPricing, AbstractQuota,
-                               AbstractUserPlan)
+from plans.base.models import (
+    AbstractBillingInfo,
+    AbstractInvoice,
+    AbstractOrder,
+    AbstractPlan,
+    AbstractPlanPricing,
+    AbstractQuota,
+    AbstractUserPlan,
+)
 from plans.forms import BillingInfoForm, CreateOrderForm, FakePaymentsForm
 from plans.importer import import_name
 from plans.mixins import LoginRequired
 from plans.signals import order_started
 from plans.utils import get_currency
 from plans.validators import plan_validation
 
@@ -35,32 +47,35 @@
 Order = AbstractOrder.get_concrete_model()
 BillingInfo = AbstractBillingInfo.get_concrete_model()
 Quota = AbstractQuota.get_concrete_model()
 Invoice = AbstractInvoice.get_concrete_model()
 
 
 class AccountActivationView(LoginRequired, TemplateView):
-    template_name = 'plans/account_activation.html'
+    template_name = "plans/account_activation.html"
 
     def get_context_data(self, **kwargs):
-        if self.request.user.userplan.active is True or self.request.user.userplan.is_expired():
+        if (
+            self.request.user.userplan.active is True
+            or self.request.user.userplan.is_expired()
+        ):
             raise Http404()
 
         context = super(AccountActivationView, self).get_context_data(**kwargs)
         errors = self.request.user.userplan.clean_activation()
 
-        if errors['required_to_activate']:
-            context['SUCCESSFUL'] = False
+        if errors["required_to_activate"]:
+            context["SUCCESSFUL"] = False
         else:
-            context['SUCCESSFUL'] = True
+            context["SUCCESSFUL"] = True
             messages.success(self.request, _("Your account is now active"))
 
-        for error in errors['required_to_activate']:
+        for error in errors["required_to_activate"]:
             messages.error(self.request, error)
-        for error in errors['other']:
+        for error in errors["other"]:
             messages.warning(self.request, error)
 
         return context
 
 
 class PlanTableMixin(object):
     def get_plan_table(self, plan_list):
@@ -78,76 +93,90 @@
         Quotas are calculated based on ``plan_list``. These are all available quotas that are
         used by given plans. If any ``Plan`` does not have any of ``PlanQuota`` then value ``None``
         will be propagated to the data structure.
 
         """
 
         # Retrieve all quotas that are used by any ``Plan`` in ``plan_list``
-        quota_list = Quota.objects.all().filter(planquota__plan__in=plan_list).distinct()
+        quota_list = (
+            Quota.objects.all().filter(planquota__plan__in=plan_list).distinct()
+        )
 
         # Create random access dict that for every ``Plan`` map ``Quota`` -> ``PlanQuota``
         plan_quotas_dic = {}
         for plan in plan_list:
             plan_quotas_dic[plan] = {}
             for plan_quota in plan.planquota_set.all():
                 plan_quotas_dic[plan][plan_quota.quota] = plan_quota
 
         # Generate data structure described in method docstring, propagate ``None`` whenever
         # ``PlanQuota`` is not available for given ``Plan`` and ``Quota``
-        return map(lambda quota: (quota,
-                                  map(lambda plan: plan_quotas_dic[plan].get(quota, None), plan_list)
-
-                                  ), quota_list)
+        return map(
+            lambda quota: (
+                quota,
+                map(lambda plan: plan_quotas_dic[plan].get(quota, None), plan_list),
+            ),
+            quota_list,
+        )
 
 
 class PlanTableViewBase(PlanTableMixin, ListView):
     model = Plan
     context_object_name = "plan_list"
 
     def get_queryset(self):
-        queryset = super(PlanTableViewBase, self).get_queryset().prefetch_related('planpricing_set__pricing',
-                                                                                  'planquota_set__quota')
+        queryset = (
+            super(PlanTableViewBase, self)
+            .get_queryset()
+            .prefetch_related("planpricing_set__pricing", "planquota_set__quota")
+        )
         if self.request.user.is_authenticated:
             queryset = queryset.filter(
-                Q(available=True, visible=True) & (
-                    Q(customized=self.request.user) | Q(customized__isnull=True)
-                )
+                Q(available=True, visible=True)
+                & (Q(customized=self.request.user) | Q(customized__isnull=True))
             )
         else:
-            queryset = queryset.filter(Q(available=True, visible=True) & Q(customized__isnull=True))
+            queryset = queryset.filter(
+                Q(available=True, visible=True) & Q(customized__isnull=True)
+            )
         return queryset
 
     def get_context_data(self, **kwargs):
         context = super(PlanTableViewBase, self).get_context_data(**kwargs)
 
         if self.request.user.is_authenticated:
             try:
-                self.userplan = UserPlan.objects.select_related('plan').get(user=self.request.user)
+                self.userplan = UserPlan.objects.select_related("plan").get(
+                    user=self.request.user
+                )
             except UserPlan.DoesNotExist:
                 self.userplan = None
 
-            context['userplan'] = self.userplan
+            context["userplan"] = self.userplan
 
             try:
-                context['current_userplan_index'] = list(self.object_list).index(self.userplan.plan)
+                context["current_userplan_index"] = list(self.object_list).index(
+                    self.userplan.plan
+                )
             except (ValueError, AttributeError):
                 pass
 
-        context['plan_table'] = self.get_plan_table(self.object_list)
-        context['CURRENCY'] = settings.PLANS_CURRENCY
+        context["plan_table"] = self.get_plan_table(self.object_list)
+        context["CURRENCY"] = settings.PLANS_CURRENCY
 
         return context
 
 
 class CurrentPlanView(LoginRequired, PlanTableViewBase):
     template_name = "plans/current.html"
 
     def get_queryset(self):
-        return Plan.objects.filter(userplan__user=self.request.user).prefetch_related('planpricing_set__pricing',
-                                                                                      'planquota_set__quota')
+        return Plan.objects.filter(userplan__user=self.request.user).prefetch_related(
+            "planpricing_set__pricing", "planquota_set__quota"
+        )
 
 
 class UpgradePlanView(LoginRequired, PlanTableViewBase):
     template_name = "plans/upgrade.html"
 
 
 class PricingView(PlanTableViewBase):
@@ -163,32 +192,41 @@
     * within current change plan policy this does not require any additional payment (None)
 
     It always redirects to ``upgrade_plan`` url as this is a potential only one place from
     where change plan could be invoked.
     """
 
     def get(self, request, *args, **kwargs):
-        return HttpResponseRedirect(reverse('upgrade_plan'))
+        return HttpResponseRedirect(reverse("upgrade_plan"))
 
     def post(self, request, *args, **kwargs):
-        plan = get_object_or_404(Plan, Q(pk=kwargs['pk']) & Q(available=True, visible=True) & (
-            Q(customized=request.user) | Q(customized__isnull=True)))
+        plan = get_object_or_404(
+            Plan,
+            Q(pk=kwargs["pk"])
+            & Q(available=True, visible=True)
+            & (Q(customized=request.user) | Q(customized__isnull=True)),
+        )
         if request.user.userplan.plan != plan:
             policy = import_name(
-                getattr(settings, 'PLANS_CHANGE_POLICY', 'plans.plan_change.StandardPlanChangePolicy'))()
+                getattr(
+                    settings,
+                    "PLANS_CHANGE_POLICY",
+                    "plans.plan_change.StandardPlanChangePolicy",
+                )
+            )()
 
             period = request.user.userplan.days_left()
             price = policy.get_change_price(request.user.userplan.plan, plan, period)
 
             if price is None:
                 request.user.userplan.extend_account(plan, None)
                 messages.success(request, _("Your plan has been successfully changed"))
             else:
                 return HttpResponseForbidden()
-        return HttpResponseRedirect(reverse('upgrade_plan'))
+        return HttpResponseRedirect(reverse("upgrade_plan"))
 
 
 class CreateOrderView(LoginRequired, CreateView):
     template_name = "plans/create_order.html"
     form_class = CreateOrderForm
 
     def recalculate(self, amount, billing_info):
@@ -197,38 +235,53 @@
         """
         order = Order(pk=-1)
         order.recalculate(amount, billing_info, self.request)
         return order
 
     def validate_plan(self, plan):
         validation_errors = plan_validation(self.request.user, plan)
-        if validation_errors['required_to_activate'] or validation_errors['other']:
-            messages.error(self.request, _(
-                "The selected plan is insufficient for your account. "
-                "Your account will not be activated or will not work fully after completing this order."
-                "<br><br>Following limits will be exceeded: <ul><li>%(reasons)s</ul>") % {
-                'reasons': '<li>'.join(chain(validation_errors['required_to_activate'],
-                                             validation_errors['other'])),
-            })
+        if validation_errors["required_to_activate"] or validation_errors["other"]:
+            messages.error(
+                self.request,
+                _(
+                    "The selected plan is insufficient for your account. "
+                    "Your account will not be activated or will not work fully after completing this order."
+                    "<br><br>Following limits will be exceeded: <ul><li>%(reasons)s</ul>"
+                )
+                % {
+                    "reasons": "<li>".join(
+                        chain(
+                            validation_errors["required_to_activate"],
+                            validation_errors["other"],
+                        )
+                    ),
+                },
+            )
 
     def get_all_context(self):
         """
         Retrieves Plan and Pricing for current order creation
         """
-        self.plan_pricing = get_object_or_404(PlanPricing.objects.all().select_related('plan', 'pricing'),
-                                              Q(pk=self.kwargs['pk']) & Q(plan__available=True) & (
-                                                  Q(plan__customized=self.request.user) | Q(
-                                                      plan__customized__isnull=True)))
+        self.plan_pricing = get_object_or_404(
+            PlanPricing.objects.all().select_related("plan", "pricing"),
+            Q(pk=self.kwargs["pk"])
+            & Q(plan__available=True)
+            & (
+                Q(plan__customized=self.request.user) | Q(plan__customized__isnull=True)
+            ),
+        )
 
         # User is not allowed to create new order for Plan when he has different Plan
         # unless it's a free plan. Otherwise, the should use Plan Change View for this
         # kind of action
-        if not self.request.user.userplan.is_expired() \
-                and not self.request.user.userplan.plan.is_free() \
-                and self.request.user.userplan.plan != self.plan_pricing.plan:
+        if (
+            not self.request.user.userplan.is_expired()
+            and not self.request.user.userplan.plan.is_free()
+            and self.request.user.userplan.plan != self.plan_pricing.plan
+        ):
             raise Http404
 
         self.plan = self.plan_pricing.plan
         self.pricing = self.plan_pricing.pricing
 
     def get_billing_info(self):
         try:
@@ -238,29 +291,33 @@
 
     def get_price(self):
         return self.plan_pricing.price
 
     def get_context_data(self, **kwargs):
         context = super(CreateOrderView, self).get_context_data(**kwargs)
         self.get_all_context()
-        context['billing_info'] = self.get_billing_info()
+        context["billing_info"] = self.get_billing_info()
 
-        order = self.recalculate(self.get_price() or Decimal('0.0'), context['billing_info'])
+        order = self.recalculate(
+            self.get_price() or Decimal("0.0"), context["billing_info"]
+        )
         order.plan = self.plan_pricing.plan
         order.pricing = self.plan_pricing.pricing
         order.currency = get_currency()
         order.user = self.request.user
-        context['object'] = order
+        context["object"] = order
 
         self.validate_plan(order.plan)
         return context
 
     def form_valid(self, form):
         self.get_all_context()
-        order = self.recalculate(self.get_price() or Decimal('0.0'), self.get_billing_info())
+        order = self.recalculate(
+            self.get_price() or Decimal("0.0"), self.get_billing_info()
+        )
 
         self.object = form.save(commit=False)
         self.object.user = self.request.user
         self.object.plan = self.plan
         self.object.pricing = self.pricing
         self.object.amount = order.amount
         self.object.tax = order.tax
@@ -271,120 +328,163 @@
 
 
 class CreateOrderPlanChangeView(CreateOrderView):
     template_name = "plans/create_order.html"
     form_class = CreateOrderForm
 
     def get_all_context(self):
-        self.plan = get_object_or_404(Plan, Q(pk=self.kwargs['pk']) & Q(available=True, visible=True) & (
-            Q(customized=self.request.user) | Q(customized__isnull=True)))
+        self.plan = get_object_or_404(
+            Plan,
+            Q(pk=self.kwargs["pk"])
+            & Q(available=True, visible=True)
+            & (Q(customized=self.request.user) | Q(customized__isnull=True)),
+        )
         self.pricing = None
 
     def get_policy(self):
-        policy_class = getattr(settings, 'PLANS_CHANGE_POLICY', 'plans.plan_change.StandardPlanChangePolicy')
+        policy_class = getattr(
+            settings,
+            "PLANS_CHANGE_POLICY",
+            "plans.plan_change.StandardPlanChangePolicy",
+        )
         return import_name(policy_class)()
 
     def get_price(self):
         policy = self.get_policy()
         userplan = self.request.user.userplan
 
         if userplan.expire is not None:
             period = self.request.user.userplan.days_left()
         else:
             # Use the default period of the new plan
             period = 30
 
-        return policy.get_change_price(self.request.user.userplan.plan, self.plan, period)
+        return policy.get_change_price(
+            self.request.user.userplan.plan, self.plan, period
+        )
 
     def get_context_data(self, **kwargs):
         context = super(CreateOrderView, self).get_context_data(**kwargs)
         self.get_all_context()
 
         price = self.get_price()
-        context['plan'] = self.plan
-        context['billing_info'] = self.get_billing_info()
+        context["plan"] = self.plan
+        context["billing_info"] = self.get_billing_info()
         if price is None:
-            context['FREE_ORDER'] = True
+            context["FREE_ORDER"] = True
             price = 0
-        order = self.recalculate(price, context['billing_info'])
+        order = self.recalculate(price, context["billing_info"])
         order.pricing = None
         order.plan = self.plan
         order.user = self.request.user
-        context['billing_info'] = context['billing_info']
-        context['object'] = order
+        context["billing_info"] = context["billing_info"]
+        context["object"] = order
         self.validate_plan(order.plan)
         return context
 
 
 class OrderView(LoginRequired, DetailView):
     model = Order
 
     def get_queryset(self):
-        return super(OrderView, self).get_queryset().filter(user=self.request.user).select_related('plan', 'pricing', )
+        return (
+            super(OrderView, self)
+            .get_queryset()
+            .filter(user=self.request.user)
+            .select_related(
+                "plan",
+                "pricing",
+            )
+        )
 
 
 class OrderListView(LoginRequired, ListView):
     model = Order
     paginate_by = 10
 
     def get_context_data(self, **kwargs):
         context = super(OrderListView, self).get_context_data(**kwargs)
-        self.CURRENCY = getattr(settings, 'PLANS_CURRENCY', None)
+        self.CURRENCY = getattr(settings, "PLANS_CURRENCY", None)
         if len(self.CURRENCY) != 3:
-            raise ImproperlyConfigured('PLANS_CURRENCY should be configured as 3-letter currency code.')
-        context['CURRENCY'] = self.CURRENCY
+            raise ImproperlyConfigured(
+                "PLANS_CURRENCY should be configured as 3-letter currency code."
+            )
+        context["CURRENCY"] = self.CURRENCY
         return context
 
     def get_queryset(self):
-        return super(OrderListView, self).get_queryset().filter(user=self.request.user).select_related('plan',
-                                                                                                       'pricing', )
+        return (
+            super(OrderListView, self)
+            .get_queryset()
+            .filter(user=self.request.user)
+            .select_related(
+                "plan",
+                "pricing",
+            )
+        )
 
 
 class OrderPaymentReturnView(LoginRequired, DetailView):
     """
     This view is a fallback from any payments processor. It allows just to set additional message
     context and redirect to Order view itself.
     """
+
     model = Order
     status = None
 
     def render_to_response(self, context, **response_kwargs):
-        if self.status == 'success':
-            messages.success(self.request,
-                             _('Thank you for placing a payment. It will be processed as soon as possible.'))
-        elif self.status == 'failure':
-            messages.error(self.request, _('Payment was not completed correctly. Please repeat payment process.'))
+        if self.status == "success":
+            messages.success(
+                self.request,
+                _(
+                    "Thank you for placing a payment. It will be processed as soon as possible."
+                ),
+            )
+        elif self.status == "failure":
+            messages.error(
+                self.request,
+                _(
+                    "Payment was not completed correctly. Please repeat payment process."
+                ),
+            )
 
         return HttpResponseRedirect(self.object.get_absolute_url())
 
     def get_queryset(self):
-        return super(OrderPaymentReturnView, self).get_queryset().filter(user=self.request.user)
+        return (
+            super(OrderPaymentReturnView, self)
+            .get_queryset()
+            .filter(user=self.request.user)
+        )
 
 
-class SuccessUrlMixin():
+class SuccessUrlMixin:
     def get_success_url(self):
-        messages.success(self.request, _('Billing info has been updated successfuly.'))
-        return reverse('billing_info')
+        messages.success(self.request, _("Billing info has been updated successfuly."))
+        return reverse("billing_info")
 
 
 class CreateOrUpdateView(
     SingleObjectTemplateResponseMixin, ModelFormMixin, ProcessFormView
 ):
     def get(self, request, *args, **kwargs):
         self.object = self.get_object()
         return super().get(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
         self.object = self.get_object()
         return super().post(request, *args, **kwargs)
 
 
-class BillingInfoCreateOrUpdateView(NextUrlMixin, SuccessUrlMixin, LoginRequired, CreateOrUpdateView):
+class BillingInfoCreateOrUpdateView(
+    NextUrlMixin, SuccessUrlMixin, LoginRequired, CreateOrUpdateView
+):
     form_class = BillingInfoForm
-    template_name = 'plans/billing_info_create_or_update.html'
+    template_name = "plans/billing_info_create_or_update.html"
 
     def get_object(self):
         try:
             return self.request.user.billinginfo
         except (AttributeError, BillingInfo.DoesNotExist):
             return None
 
@@ -395,15 +495,15 @@
     def get_form_kwargs(self):
         kwargs = super().get_form_kwargs()
         kwargs.update(request=self.request)
         return kwargs
 
 
 class RedirectToBilling(RedirectView):
-    url = reverse_lazy('billing_info')
+    url = reverse_lazy("billing_info")
     permanent = False
     query_string = True
 
     def get_redirect_url(self, *args, **kwargs):
         warnings.warn(
             "This view URL is deprecated. Use plain billing_info instead.",
             DeprecationWarning,
@@ -411,64 +511,76 @@
         return super().get_redirect_url(*args, **kwargs)
 
 
 class BillingInfoDeleteView(LoginRequired, DeleteView):
     """
     Deletes billing data for user
     """
-    template_name = 'plans/billing_info_delete.html'
+
+    template_name = "plans/billing_info_delete.html"
 
     def get_object(self):
         try:
             return self.request.user.billinginfo
         except BillingInfo.DoesNotExist:
             raise Http404
 
     def get_success_url(self):
-        messages.success(self.request, _('Billing info has been deleted.'))
-        return reverse('billing_info')
+        messages.success(self.request, _("Billing info has been deleted."))
+        return reverse("billing_info")
 
 
 class InvoiceDetailView(LoginRequired, DetailView):
     model = Invoice
 
     def get_template_names(self):
-        return getattr(settings, 'PLANS_INVOICE_TEMPLATE', 'plans/invoices/PL_EN.html')
+        return getattr(settings, "PLANS_INVOICE_TEMPLATE", "plans/invoices/PL_EN.html")
 
     def get_context_data(self, **kwargs):
         context = super(InvoiceDetailView, self).get_context_data(**kwargs)
-        context['logo_url'] = getattr(settings, 'PLANS_INVOICE_LOGO_URL', None)
-        context['auto_print'] = True
+        context["logo_url"] = getattr(settings, "PLANS_INVOICE_LOGO_URL", None)
+        context["auto_print"] = True
         return context
 
     def get_queryset(self):
         if self.request.user.is_superuser:
-            return super(InvoiceDetailView, self).get_queryset().select_related('order')
+            return super(InvoiceDetailView, self).get_queryset().select_related("order")
         else:
-            return super(InvoiceDetailView, self).get_queryset().filter(user=self.request.user).select_related('order')
+            return (
+                super(InvoiceDetailView, self)
+                .get_queryset()
+                .filter(user=self.request.user)
+                .select_related("order")
+            )
 
 
 class FakePaymentsView(LoginRequired, SingleObjectMixin, FormView):
     form_class = FakePaymentsForm
     model = Order
-    template_name = 'plans/fake_payments.html'
+    template_name = "plans/fake_payments.html"
 
     def get_success_url(self):
         return self.object.get_absolute_url()
 
     def get_queryset(self):
-        return super(FakePaymentsView, self).get_queryset().filter(user=self.request.user)
+        return (
+            super(FakePaymentsView, self).get_queryset().filter(user=self.request.user)
+        )
 
     def dispatch(self, *args, **kwargs):
-        if not getattr(settings, 'DEBUG', False):
-            return HttpResponseForbidden('This view is accessible only in debug mode.')
+        if not getattr(settings, "DEBUG", False):
+            return HttpResponseForbidden("This view is accessible only in debug mode.")
         self.object = self.get_object()
         return super(FakePaymentsView, self).dispatch(*args, **kwargs)
 
     def form_valid(self, form):
-        if int(form['status'].value()) == Order.STATUS.COMPLETED:
+        if int(form["status"].value()) == Order.STATUS.COMPLETED:
             self.object.complete_order()
-            return HttpResponseRedirect(reverse('order_payment_success', kwargs={'pk': self.object.pk}))
+            return HttpResponseRedirect(
+                reverse("order_payment_success", kwargs={"pk": self.object.pk})
+            )
         else:
-            self.object.status = form['status'].value()
+            self.object.status = form["status"].value()
             self.object.save()
-            return HttpResponseRedirect(reverse('order_payment_failure', kwargs={'pk': self.object.pk}))
+            return HttpResponseRedirect(
+                reverse("order_payment_failure", kwargs={"pk": self.object.pk})
+            )
```

### Comparing `django-plans-1.0.4/plans_i18n/README.rst` & `django-plans-1.0.5/plans_i18n/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans_i18n/admin.py` & `django-plans-1.0.5/plans_i18n/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.4/plans_i18n/translation.py` & `django-plans-1.0.5/plans_i18n/translation.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 Pricing = AbstractPricing.get_concrete_model()
 Quota = AbstractQuota.get_concrete_model()
 
 # Translations for django-plans
 
 
 class PlanTranslationOptions(TranslationOptions):
-    fields = ('name', 'description', )
+    fields = (
+        "name",
+        "description",
+    )
 
 
 translator.register(Plan, PlanTranslationOptions)
 
 
 class PricingTranslationOptions(TranslationOptions):
-    fields = ('name',)
+    fields = ("name",)
 
 
 translator.register(Pricing, PricingTranslationOptions)
 
 
 class QuotaTranslationOptions(TranslationOptions):
-    fields = ('name', 'description', 'unit')
+    fields = ("name", "description", "unit")
 
 
 translator.register(Quota, QuotaTranslationOptions)
```

### Comparing `django-plans-1.0.4/setup.py` & `django-plans-1.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import find_packages, setup
 
 from plans import __version__ as VERSION
 
-with open('README.rst') as file:
+with open("README.rst") as file:
     long_description = file.read()
 
 setup(
-    name='django-plans',
+    name="django-plans",
     version=VERSION,
-    description='Pluggable django app for managing pricing plans with quotas and accounts expiration',
+    description="Pluggable django app for managing pricing plans with quotas and accounts expiration",
     long_description=long_description,
-    author='Krzysztof Dorosz',
-    author_email='cypreess@gmail.com',
-    url='https://github.com/cypreess/django-plans',
-    license='MIT',
-
+    author="Krzysztof Dorosz",
+    author_email="cypreess@gmail.com",
+    url="https://github.com/cypreess/django-plans",
+    license="MIT",
     packages=find_packages(),
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Framework :: Django',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
+        "Development Status :: 4 - Beta",
+        "Framework :: Django",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.6",
     ],
     install_requires=[
-        'django-countries>=4.5',
-        'pytz>=2017.2',
-        'django-ordered-model>=1.4.1',
-        'python-stdnum',
-        'django-next-url-mixin>=0.1.0',
-        'suds',
-        'django-sequences',
-        'swapper~=1.3.0',
-        'six',
+        "django-countries>=4.5",
+        "pytz>=2017.2",
+        "django-ordered-model>=1.4.1",
+        "python-stdnum",
+        "django-next-url-mixin>=0.1.0",
+        "suds",
+        "django-sequences",
+        "swapper~=1.3.0",
+        "six",
     ],
     extras_require={
-        'i18n': [
-            'django-modeltranslation>=0.5b1',
+        "i18n": [
+            "django-modeltranslation>=0.5b1",
         ],
     },
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `django-plans-1.0.4/tox.ini` & `django-plans-1.0.5/tox.ini`

 * *Files identical despite different names*

