# Comparing `tmp/codat-sync-for-expenses-0.15.3.tar.gz` & `tmp/codat-sync-for-expenses-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.15.3.tar", last modified: Thu May 11 20:35:54 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.19.0.tar", last modified: Thu May 18 08:35:01 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.15.3.tar` & `codat-sync-for-expenses-0.19.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.909308 codat-sync-for-expenses-0.15.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.913308 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:35:54.000000 codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.917308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4384 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2400 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4451 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2329 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.917308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.921308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/integrationtype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2142 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6597 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3978 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:35:54.925308 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25963 2023-05-11 20:35:45.000000 codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.503766 codat-sync-for-expenses-0.19.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.507766 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 08:35:01.000000 codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.507766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4616 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4645 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2464 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.507766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.507766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1833 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      360 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnectionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/integrationtype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2142 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2921 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7137 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:35:01.511766 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-05-18 08:34:50.000000 codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.15.3/PKG-INFO` & `codat-sync-for-expenses-0.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.15.3
+Version: 0.19.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.15.3/README.md` & `codat-sync-for-expenses-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/setup.py` & `codat-sync-for-expenses-0.19.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.15.3",
+    version="0.19.0",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.15.3
+Version: 0.19.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.19.0/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,26 +26,27 @@
     def get_company_configuration(self, request: operations.GetCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyConfigurationResponse:
         r"""Get company configuration
         Gets a companies expense sync configuration
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
-        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -63,19 +64,19 @@
     def save_company_configuration(self, request: operations.SaveCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.SaveCompanyConfigurationResponse:
         r"""Set company configuration
         Sets a companies expense sync configuration
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.SaveCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
-        
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "company_configuration", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/connections.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,26 +26,27 @@
     def create_partner_expense_connection(self, request: operations.CreatePartnerExpenseConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreatePartnerExpenseConnectionResponse:
         r"""Create Partner Expense connection
         Creates a Partner Expense data connection
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreatePartnerExpenseConnectionRequest, base_url, '/companies/{companyId}/sync/expenses/connections/partnerExpense', request)
-        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('POST', url)
+            return client.request('POST', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/expenses.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     def create_expense_dataset(self, request: operations.CreateExpenseDatasetRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateExpenseDatasetResponse:
         r"""Create expense-transactions
         Create an expense transaction
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateExpenseDatasetRequest, base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
-        
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_expense_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
@@ -67,19 +67,19 @@
     def upload_attachment(self, request: operations.UploadAttachmentRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UploadAttachmentResponse:
         r"""Upload attachment
         Creates an attachment in the accounting software against the given transactionId
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.UploadAttachmentRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}/attachments', request)
-        
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/mapping_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,26 +26,27 @@
     def get_mapping_options(self, request: operations.GetMappingOptionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetMappingOptionsResponse:
         r"""Mapping options
         Gets the expense mapping options for a companies accounting software
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetMappingOptionsRequest, base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
-        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/hallink.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/hallink.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     transaction_status: TransactionStatus
     r"""Retrieve the status of transactions within a sync."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.15.3"
-    _gen_version: str = "2.26.3"
+    _sdk_version: str = "0.19.0"
+    _gen_version: str = "2.30.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     def intiate_sync(self, request: operations.IntiateSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.IntiateSyncResponse:
         r"""Initiate sync
         Initiate sync of pending transactions.
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.IntiateSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs', request)
-        
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "post_sync", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/sync_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,26 +26,27 @@
     def get_last_successful_sync(self, request: operations.GetLastSuccessfulSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLastSuccessfulSyncResponse:
         r"""Last successful sync
         Gets the status of the last successfull sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetLastSuccessfulSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/lastSuccessful/status', request)
-        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -63,26 +64,27 @@
     def get_latest_sync(self, request: operations.GetLatestSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLatestSyncResponse:
         r"""Latest sync status
         Gets the latest sync status
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetLatestSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/latest/status', request)
-        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -100,26 +102,27 @@
     def get_sync_by_id(self, request: operations.GetSyncByIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncByIDResponse:
         r"""Get Sync status
         Get the sync status for a specified sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncByIDRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/status', request)
-        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -137,26 +140,27 @@
     def list_syncs(self, request: operations.ListSyncsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncsResponse:
         r"""List sync statuses
         Gets a list of sync statuses
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSyncsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/list/status', request)
-        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/transaction_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,26 +26,27 @@
     def get_sync_transaction(self, request: operations.GetSyncTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncTransactionResponse:
         r"""Get Sync Transaction
         Gets the status of a transaction for a sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
-        
+        headers = {}
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
@@ -63,27 +64,28 @@
     def list_sync_transactions(self, request: operations.ListSyncTransactionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncTransactionsResponse:
         r"""Get Sync transactions
         Get's the transactions and status for a sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSyncTransactionsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
-        
+        headers = {}
         query_params = utils.get_query_params(operations.ListSyncTransactionsRequest, request)
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url, params=query_params)
+            return client.request('GET', url, params=query_params, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
```

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.15.3/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.19.0/src/codatsyncexpenses/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             raise Exception('not supported')
     elif scheme_type == "openIdConnect":
         client.client.headers[header_name] = value
     elif scheme_type == 'oauth2':
         client.client.headers[header_name] = value
     elif scheme_type == 'http':
         if sub_type == 'bearer':
-            client.client.headers[header_name] = value
+            client.client.headers[header_name] = value.lower().startswith('bearer ') and value or f'Bearer {value}'
         else:
             raise Exception('not supported')
     else:
         raise Exception('not supported')
 
 
 def _parse_basic_auth_scheme(client: SecurityClient, scheme: dataclass):
@@ -372,17 +372,17 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, array_delimiter: str) -> dict[
+def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, delimiter: str) -> dict[
     str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, array_delimiter)
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
     'json': 'application/json',
     'form': 'application/x-www-form-urlencoded',
     'multipart': 'multipart/form-data',
     'raw': 'application/octet-stream',
@@ -544,15 +544,15 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, array_delimiter: str) -> \
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, delimiter: str) -> \
         dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
@@ -568,31 +568,31 @@
             if val is None:
                 continue
 
             if explode:
                 params[obj_field_name] = [_val_to_string(val)]
             else:
                 items.append(
-                    f'{obj_field_name},{_val_to_string(val)}')
+                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
 
         if len(items) > 0:
-            params[field_name] = [','.join(items)]
+            params[field_name] = [delimiter.join(items)]
     elif isinstance(obj, dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
                 params[key] = _val_to_string(value)
             else:
-                items.append(f'{key},{_val_to_string(value)}')
+                items.append(f'{key}{delimiter}{_val_to_string(value)}')
 
         if len(items) > 0:
-            params[field_name] = [','.join(items)]
+            params[field_name] = [delimiter.join(items)]
     elif isinstance(obj, list):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
@@ -600,15 +600,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [array_delimiter.join([str(item) for item in items])]
+            params[field_name] = [delimiter.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
```

