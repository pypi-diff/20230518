# Comparing `tmp/alibabacloud_dingtalk-2.0.14.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.14.tar", last modified: Wed May 17 02:21:50 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.15.tar", last modified: Thu May 18 06:04:19 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.14.tar` & `alibabacloud_dingtalk-2.0.15.tar`

### file list

```diff
@@ -1,357 +1,361 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/
--rw-r--r--   0 root         (0) root         (0)    19557 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158124 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   299469 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   569113 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138814 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   331545 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220322 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   547684 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45840 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    65285 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312544 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   433417 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   523174 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   756557 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   131349 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   159547 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44880 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81308 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53454 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   118368 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175082 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   370377 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11743 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-17 02:21:50.000000 alibabacloud_dingtalk-2.0.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/
+-rw-r--r--   0 root         (0) root         (0)    19622 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161892 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   317257 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   569113 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138814 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   331545 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10927 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85810 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110530 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   293352 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   387566 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   220322 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   547684 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45840 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    65285 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312544 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   433417 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18281 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   523174 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   756557 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131349 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   159547 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44880 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81308 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377583 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11880 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 06:04:19.000000 alibabacloud_dingtalk-2.0.15/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-18 06:04:18.000000 alibabacloud_dingtalk-2.0.15/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.14/ChangeLog.md` & `alibabacloud_dingtalk-2.0.15/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-17 Version: 2.0.14
+- Update AddOfficialAccountFollower.
+
 2023-05-16 Version: 2.0.13
 - Update AddOfficialAccountFollower.
 
 2023-05-12 Version: 2.0.12
 - Update AddOfficialAccountFollower.
 
 2023-05-09 Version: 2.0.11
```

### Comparing `alibabacloud_dingtalk-2.0.14/LICENSE` & `alibabacloud_dingtalk-2.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/PKG-INFO` & `alibabacloud_dingtalk-2.0.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.14
+Version: 2.0.15
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.14/README-CN.md` & `alibabacloud_dingtalk-2.0.15/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/README.md` & `alibabacloud_dingtalk-2.0.15/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1853,14 +1853,104 @@
         self,
         request: dingtalkattendance__1__0_models.GetOvertimeSettingRequest,
     ) -> dingtalkattendance__1__0_models.GetOvertimeSettingResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkattendance__1__0_models.GetOvertimeSettingHeaders()
         return await self.get_overtime_setting_with_options_async(request, headers, runtime)
 
+    def get_shift_with_options(
+        self,
+        request: dingtalkattendance__1__0_models.GetShiftRequest,
+        headers: dingtalkattendance__1__0_models.GetShiftHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.GetShiftResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.op_user_id):
+            query['opUserId'] = request.op_user_id
+        if not UtilClient.is_unset(request.shift_id):
+            query['shiftId'] = request.shift_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetShift',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/shifts',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.GetShiftResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_shift_with_options_async(
+        self,
+        request: dingtalkattendance__1__0_models.GetShiftRequest,
+        headers: dingtalkattendance__1__0_models.GetShiftHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.GetShiftResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.op_user_id):
+            query['opUserId'] = request.op_user_id
+        if not UtilClient.is_unset(request.shift_id):
+            query['shiftId'] = request.shift_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetShift',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/shifts',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.GetShiftResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_shift(
+        self,
+        request: dingtalkattendance__1__0_models.GetShiftRequest,
+    ) -> dingtalkattendance__1__0_models.GetShiftResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.GetShiftHeaders()
+        return self.get_shift_with_options(request, headers, runtime)
+
+    async def get_shift_async(
+        self,
+        request: dingtalkattendance__1__0_models.GetShiftRequest,
+    ) -> dingtalkattendance__1__0_models.GetShiftResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.GetShiftHeaders()
+        return await self.get_shift_with_options_async(request, headers, runtime)
+
     def get_simple_overtime_setting_with_options(
         self,
         request: dingtalkattendance__1__0_models.GetSimpleOvertimeSettingRequest,
         headers: dingtalkattendance__1__0_models.GetSimpleOvertimeSettingHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkattendance__1__0_models.GetSimpleOvertimeSettingResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5137,14 +5137,554 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetOvertimeSettingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetShiftHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetShiftRequest(TeaModel):
+    def __init__(
+        self,
+        op_user_id: str = None,
+        shift_id: int = None,
+    ):
+        self.op_user_id = op_user_id
+        self.shift_id = shift_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.op_user_id is not None:
+            result['opUserId'] = self.op_user_id
+        if self.shift_id is not None:
+            result['shiftId'] = self.shift_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('opUserId') is not None:
+            self.op_user_id = m.get('opUserId')
+        if m.get('shiftId') is not None:
+            self.shift_id = m.get('shiftId')
+        return self
+
+
+class GetShiftResponseBodyResultSectionsPunchesLateBackSettingLateBackPairs(TeaModel):
+    def __init__(
+        self,
+        extra: int = None,
+        late: int = None,
+    ):
+        self.extra = extra
+        self.late = late
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extra is not None:
+            result['extra'] = self.extra
+        if self.late is not None:
+            result['late'] = self.late
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('extra') is not None:
+            self.extra = m.get('extra')
+        if m.get('late') is not None:
+            self.late = m.get('late')
+        return self
+
+
+class GetShiftResponseBodyResultSectionsPunchesLateBackSetting(TeaModel):
+    def __init__(
+        self,
+        late_back_pairs: List[GetShiftResponseBodyResultSectionsPunchesLateBackSettingLateBackPairs] = None,
+    ):
+        self.late_back_pairs = late_back_pairs
+
+    def validate(self):
+        if self.late_back_pairs:
+            for k in self.late_back_pairs:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['lateBackPairs'] = []
+        if self.late_back_pairs is not None:
+            for k in self.late_back_pairs:
+                result['lateBackPairs'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.late_back_pairs = []
+        if m.get('lateBackPairs') is not None:
+            for k in m.get('lateBackPairs'):
+                temp_model = GetShiftResponseBodyResultSectionsPunchesLateBackSettingLateBackPairs()
+                self.late_back_pairs.append(temp_model.from_map(k))
+        return self
+
+
+class GetShiftResponseBodyResultSectionsPunches(TeaModel):
+    def __init__(
+        self,
+        absenteeism_late_minutes: int = None,
+        across: int = None,
+        begin_min: int = None,
+        check_time: str = None,
+        check_type: str = None,
+        end_min: int = None,
+        free_check: bool = None,
+        late_back_setting: GetShiftResponseBodyResultSectionsPunchesLateBackSetting = None,
+        permit_minutes: int = None,
+        punche_id: int = None,
+        serious_late_minutes: int = None,
+    ):
+        self.absenteeism_late_minutes = absenteeism_late_minutes
+        self.across = across
+        self.begin_min = begin_min
+        self.check_time = check_time
+        self.check_type = check_type
+        self.end_min = end_min
+        self.free_check = free_check
+        self.late_back_setting = late_back_setting
+        self.permit_minutes = permit_minutes
+        self.punche_id = punche_id
+        self.serious_late_minutes = serious_late_minutes
+
+    def validate(self):
+        if self.late_back_setting:
+            self.late_back_setting.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.absenteeism_late_minutes is not None:
+            result['absenteeismLateMinutes'] = self.absenteeism_late_minutes
+        if self.across is not None:
+            result['across'] = self.across
+        if self.begin_min is not None:
+            result['beginMin'] = self.begin_min
+        if self.check_time is not None:
+            result['checkTime'] = self.check_time
+        if self.check_type is not None:
+            result['checkType'] = self.check_type
+        if self.end_min is not None:
+            result['end_min'] = self.end_min
+        if self.free_check is not None:
+            result['freeCheck'] = self.free_check
+        if self.late_back_setting is not None:
+            result['lateBackSetting'] = self.late_back_setting.to_map()
+        if self.permit_minutes is not None:
+            result['permitMinutes'] = self.permit_minutes
+        if self.punche_id is not None:
+            result['puncheId'] = self.punche_id
+        if self.serious_late_minutes is not None:
+            result['seriousLateMinutes'] = self.serious_late_minutes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('absenteeismLateMinutes') is not None:
+            self.absenteeism_late_minutes = m.get('absenteeismLateMinutes')
+        if m.get('across') is not None:
+            self.across = m.get('across')
+        if m.get('beginMin') is not None:
+            self.begin_min = m.get('beginMin')
+        if m.get('checkTime') is not None:
+            self.check_time = m.get('checkTime')
+        if m.get('checkType') is not None:
+            self.check_type = m.get('checkType')
+        if m.get('end_min') is not None:
+            self.end_min = m.get('end_min')
+        if m.get('freeCheck') is not None:
+            self.free_check = m.get('freeCheck')
+        if m.get('lateBackSetting') is not None:
+            temp_model = GetShiftResponseBodyResultSectionsPunchesLateBackSetting()
+            self.late_back_setting = temp_model.from_map(m['lateBackSetting'])
+        if m.get('permitMinutes') is not None:
+            self.permit_minutes = m.get('permitMinutes')
+        if m.get('puncheId') is not None:
+            self.punche_id = m.get('puncheId')
+        if m.get('seriousLateMinutes') is not None:
+            self.serious_late_minutes = m.get('seriousLateMinutes')
+        return self
+
+
+class GetShiftResponseBodyResultSectionsRests(TeaModel):
+    def __init__(
+        self,
+        across: int = None,
+        check_time: str = None,
+        check_type: str = None,
+        rest_id: int = None,
+    ):
+        self.across = across
+        self.check_time = check_time
+        self.check_type = check_type
+        self.rest_id = rest_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.across is not None:
+            result['across'] = self.across
+        if self.check_time is not None:
+            result['checkTime'] = self.check_time
+        if self.check_type is not None:
+            result['check_type'] = self.check_type
+        if self.rest_id is not None:
+            result['restId'] = self.rest_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('across') is not None:
+            self.across = m.get('across')
+        if m.get('checkTime') is not None:
+            self.check_time = m.get('checkTime')
+        if m.get('check_type') is not None:
+            self.check_type = m.get('check_type')
+        if m.get('restId') is not None:
+            self.rest_id = m.get('restId')
+        return self
+
+
+class GetShiftResponseBodyResultSections(TeaModel):
+    def __init__(
+        self,
+        punches: List[GetShiftResponseBodyResultSectionsPunches] = None,
+        rests: List[GetShiftResponseBodyResultSectionsRests] = None,
+        section_id: int = None,
+    ):
+        self.punches = punches
+        self.rests = rests
+        self.section_id = section_id
+
+    def validate(self):
+        if self.punches:
+            for k in self.punches:
+                if k:
+                    k.validate()
+        if self.rests:
+            for k in self.rests:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['punches'] = []
+        if self.punches is not None:
+            for k in self.punches:
+                result['punches'].append(k.to_map() if k else None)
+        result['rests'] = []
+        if self.rests is not None:
+            for k in self.rests:
+                result['rests'].append(k.to_map() if k else None)
+        if self.section_id is not None:
+            result['sectionId'] = self.section_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.punches = []
+        if m.get('punches') is not None:
+            for k in m.get('punches'):
+                temp_model = GetShiftResponseBodyResultSectionsPunches()
+                self.punches.append(temp_model.from_map(k))
+        self.rests = []
+        if m.get('rests') is not None:
+            for k in m.get('rests'):
+                temp_model = GetShiftResponseBodyResultSectionsRests()
+                self.rests.append(temp_model.from_map(k))
+        if m.get('sectionId') is not None:
+            self.section_id = m.get('sectionId')
+        return self
+
+
+class GetShiftResponseBodyResultShiftSetting(TeaModel):
+    def __init__(
+        self,
+        attend_days: str = None,
+        corp_id: str = None,
+        gmt_create: str = None,
+        gmt_modified: str = None,
+        shift_id: int = None,
+        shift_setting_id: int = None,
+        work_time_minutes: int = None,
+    ):
+        self.attend_days = attend_days
+        self.corp_id = corp_id
+        self.gmt_create = gmt_create
+        self.gmt_modified = gmt_modified
+        self.shift_id = shift_id
+        self.shift_setting_id = shift_setting_id
+        self.work_time_minutes = work_time_minutes
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.attend_days is not None:
+            result['attendDays'] = self.attend_days
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.gmt_create is not None:
+            result['gmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['gmtModified'] = self.gmt_modified
+        if self.shift_id is not None:
+            result['shiftId'] = self.shift_id
+        if self.shift_setting_id is not None:
+            result['shiftSettingId'] = self.shift_setting_id
+        if self.work_time_minutes is not None:
+            result['workTimeMinutes'] = self.work_time_minutes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('attendDays') is not None:
+            self.attend_days = m.get('attendDays')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('gmtCreate') is not None:
+            self.gmt_create = m.get('gmtCreate')
+        if m.get('gmtModified') is not None:
+            self.gmt_modified = m.get('gmtModified')
+        if m.get('shiftId') is not None:
+            self.shift_id = m.get('shiftId')
+        if m.get('shiftSettingId') is not None:
+            self.shift_setting_id = m.get('shiftSettingId')
+        if m.get('workTimeMinutes') is not None:
+            self.work_time_minutes = m.get('workTimeMinutes')
+        return self
+
+
+class GetShiftResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        id: int = None,
+        name: str = None,
+        owner: str = None,
+        sections: List[GetShiftResponseBodyResultSections] = None,
+        shift_group_id: int = None,
+        shift_group_name: str = None,
+        shift_setting: GetShiftResponseBodyResultShiftSetting = None,
+    ):
+        self.corp_id = corp_id
+        self.id = id
+        self.name = name
+        self.owner = owner
+        self.sections = sections
+        self.shift_group_id = shift_group_id
+        self.shift_group_name = shift_group_name
+        self.shift_setting = shift_setting
+
+    def validate(self):
+        if self.sections:
+            for k in self.sections:
+                if k:
+                    k.validate()
+        if self.shift_setting:
+            self.shift_setting.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.owner is not None:
+            result['owner'] = self.owner
+        result['sections'] = []
+        if self.sections is not None:
+            for k in self.sections:
+                result['sections'].append(k.to_map() if k else None)
+        if self.shift_group_id is not None:
+            result['shiftGroupId'] = self.shift_group_id
+        if self.shift_group_name is not None:
+            result['shiftGroupName'] = self.shift_group_name
+        if self.shift_setting is not None:
+            result['shiftSetting'] = self.shift_setting.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('owner') is not None:
+            self.owner = m.get('owner')
+        self.sections = []
+        if m.get('sections') is not None:
+            for k in m.get('sections'):
+                temp_model = GetShiftResponseBodyResultSections()
+                self.sections.append(temp_model.from_map(k))
+        if m.get('shiftGroupId') is not None:
+            self.shift_group_id = m.get('shiftGroupId')
+        if m.get('shiftGroupName') is not None:
+            self.shift_group_name = m.get('shiftGroupName')
+        if m.get('shiftSetting') is not None:
+            temp_model = GetShiftResponseBodyResultShiftSetting()
+            self.shift_setting = temp_model.from_map(m['shiftSetting'])
+        return self
+
+
+class GetShiftResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: GetShiftResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = GetShiftResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class GetShiftResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetShiftResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetShiftResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetSimpleOvertimeSettingHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -311,14 +311,100 @@
         team_id: str,
         request: dingtalkwiki__2__0_models.DeleteTeamRequest,
     ) -> dingtalkwiki__2__0_models.DeleteTeamResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkwiki__2__0_models.DeleteTeamHeaders()
         return await self.delete_team_with_options_async(team_id, request, headers, runtime)
 
+    def get_default_hand_over_user_with_options(
+        self,
+        request: dingtalkwiki__2__0_models.GetDefaultHandOverUserRequest,
+        headers: dingtalkwiki__2__0_models.GetDefaultHandOverUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkwiki__2__0_models.GetDefaultHandOverUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDefaultHandOverUser',
+            version='wiki_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/wiki/managementSettings/defaultHandOverUsers',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkwiki__2__0_models.GetDefaultHandOverUserResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_default_hand_over_user_with_options_async(
+        self,
+        request: dingtalkwiki__2__0_models.GetDefaultHandOverUserRequest,
+        headers: dingtalkwiki__2__0_models.GetDefaultHandOverUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkwiki__2__0_models.GetDefaultHandOverUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDefaultHandOverUser',
+            version='wiki_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/wiki/managementSettings/defaultHandOverUsers',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkwiki__2__0_models.GetDefaultHandOverUserResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_default_hand_over_user(
+        self,
+        request: dingtalkwiki__2__0_models.GetDefaultHandOverUserRequest,
+    ) -> dingtalkwiki__2__0_models.GetDefaultHandOverUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkwiki__2__0_models.GetDefaultHandOverUserHeaders()
+        return self.get_default_hand_over_user_with_options(request, headers, runtime)
+
+    async def get_default_hand_over_user_async(
+        self,
+        request: dingtalkwiki__2__0_models.GetDefaultHandOverUserRequest,
+    ) -> dingtalkwiki__2__0_models.GetDefaultHandOverUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkwiki__2__0_models.GetDefaultHandOverUserHeaders()
+        return await self.get_default_hand_over_user_with_options_async(request, headers, runtime)
+
     def get_mine_workspace_with_options(
         self,
         request: dingtalkwiki__2__0_models.GetMineWorkspaceRequest,
         headers: dingtalkwiki__2__0_models.GetMineWorkspaceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkwiki__2__0_models.GetMineWorkspaceResponse:
         UtilClient.validate_model(request)
@@ -973,14 +1059,116 @@
         self,
         request: dingtalkwiki__2__0_models.GetWorkspacesRequest,
     ) -> dingtalkwiki__2__0_models.GetWorkspacesResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkwiki__2__0_models.GetWorkspacesHeaders()
         return await self.get_workspaces_with_options_async(request, headers, runtime)
 
+    def hand_over_workspace_with_options(
+        self,
+        request: dingtalkwiki__2__0_models.HandOverWorkspaceRequest,
+        headers: dingtalkwiki__2__0_models.HandOverWorkspaceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkwiki__2__0_models.HandOverWorkspaceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.source_owner_id):
+            body['sourceOwnerId'] = request.source_owner_id
+        if not UtilClient.is_unset(request.target_owner_id):
+            body['targetOwnerId'] = request.target_owner_id
+        if not UtilClient.is_unset(request.workspace_id):
+            body['workspaceId'] = request.workspace_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='HandOverWorkspace',
+            version='wiki_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/wiki/managementOperations/workspaces/handOver',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkwiki__2__0_models.HandOverWorkspaceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def hand_over_workspace_with_options_async(
+        self,
+        request: dingtalkwiki__2__0_models.HandOverWorkspaceRequest,
+        headers: dingtalkwiki__2__0_models.HandOverWorkspaceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkwiki__2__0_models.HandOverWorkspaceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.source_owner_id):
+            body['sourceOwnerId'] = request.source_owner_id
+        if not UtilClient.is_unset(request.target_owner_id):
+            body['targetOwnerId'] = request.target_owner_id
+        if not UtilClient.is_unset(request.workspace_id):
+            body['workspaceId'] = request.workspace_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='HandOverWorkspace',
+            version='wiki_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/wiki/managementOperations/workspaces/handOver',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkwiki__2__0_models.HandOverWorkspaceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def hand_over_workspace(
+        self,
+        request: dingtalkwiki__2__0_models.HandOverWorkspaceRequest,
+    ) -> dingtalkwiki__2__0_models.HandOverWorkspaceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkwiki__2__0_models.HandOverWorkspaceHeaders()
+        return self.hand_over_workspace_with_options(request, headers, runtime)
+
+    async def hand_over_workspace_async(
+        self,
+        request: dingtalkwiki__2__0_models.HandOverWorkspaceRequest,
+    ) -> dingtalkwiki__2__0_models.HandOverWorkspaceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkwiki__2__0_models.HandOverWorkspaceHeaders()
+        return await self.hand_over_workspace_with_options_async(request, headers, runtime)
+
     def list_nodes_with_options(
         self,
         request: dingtalkwiki__2__0_models.ListNodesRequest,
         headers: dingtalkwiki__2__0_models.ListNodesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkwiki__2__0_models.ListNodesResponse:
         UtilClient.validate_model(request)
@@ -1274,7 +1462,101 @@
     async def list_workspaces_async(
         self,
         request: dingtalkwiki__2__0_models.ListWorkspacesRequest,
     ) -> dingtalkwiki__2__0_models.ListWorkspacesResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkwiki__2__0_models.ListWorkspacesHeaders()
         return await self.list_workspaces_with_options_async(request, headers, runtime)
+
+    def set_default_hand_over_user_with_options(
+        self,
+        request: dingtalkwiki__2__0_models.SetDefaultHandOverUserRequest,
+        headers: dingtalkwiki__2__0_models.SetDefaultHandOverUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkwiki__2__0_models.SetDefaultHandOverUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.default_handover_user_id):
+            body['defaultHandoverUserId'] = request.default_handover_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SetDefaultHandOverUser',
+            version='wiki_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/wiki/managementSettings/defaultHandOverUsers/set',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkwiki__2__0_models.SetDefaultHandOverUserResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def set_default_hand_over_user_with_options_async(
+        self,
+        request: dingtalkwiki__2__0_models.SetDefaultHandOverUserRequest,
+        headers: dingtalkwiki__2__0_models.SetDefaultHandOverUserHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkwiki__2__0_models.SetDefaultHandOverUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.default_handover_user_id):
+            body['defaultHandoverUserId'] = request.default_handover_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SetDefaultHandOverUser',
+            version='wiki_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/wiki/managementSettings/defaultHandOverUsers/set',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkwiki__2__0_models.SetDefaultHandOverUserResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def set_default_hand_over_user(
+        self,
+        request: dingtalkwiki__2__0_models.SetDefaultHandOverUserRequest,
+    ) -> dingtalkwiki__2__0_models.SetDefaultHandOverUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkwiki__2__0_models.SetDefaultHandOverUserHeaders()
+        return self.set_default_hand_over_user_with_options(request, headers, runtime)
+
+    async def set_default_hand_over_user_async(
+        self,
+        request: dingtalkwiki__2__0_models.SetDefaultHandOverUserRequest,
+    ) -> dingtalkwiki__2__0_models.SetDefaultHandOverUserResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkwiki__2__0_models.SetDefaultHandOverUserHeaders()
+        return await self.set_default_hand_over_user_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -794,14 +794,145 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteTeamResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetDefaultHandOverUserHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetDefaultHandOverUserRequest(TeaModel):
+    def __init__(
+        self,
+        operator_id: str = None,
+    ):
+        self.operator_id = operator_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
+class GetDefaultHandOverUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        default_handover_user_id: str = None,
+    ):
+        self.default_handover_user_id = default_handover_user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.default_handover_user_id is not None:
+            result['defaultHandoverUserId'] = self.default_handover_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('defaultHandoverUserId') is not None:
+            self.default_handover_user_id = m.get('defaultHandoverUserId')
+        return self
+
+
+class GetDefaultHandOverUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDefaultHandOverUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDefaultHandOverUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetMineWorkspaceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -2864,14 +2995,163 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetWorkspacesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class HandOverWorkspaceHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class HandOverWorkspaceRequest(TeaModel):
+    def __init__(
+        self,
+        source_owner_id: str = None,
+        target_owner_id: str = None,
+        workspace_id: str = None,
+        operator_id: str = None,
+    ):
+        self.source_owner_id = source_owner_id
+        self.target_owner_id = target_owner_id
+        self.workspace_id = workspace_id
+        self.operator_id = operator_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.source_owner_id is not None:
+            result['sourceOwnerId'] = self.source_owner_id
+        if self.target_owner_id is not None:
+            result['targetOwnerId'] = self.target_owner_id
+        if self.workspace_id is not None:
+            result['workspaceId'] = self.workspace_id
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('sourceOwnerId') is not None:
+            self.source_owner_id = m.get('sourceOwnerId')
+        if m.get('targetOwnerId') is not None:
+            self.target_owner_id = m.get('targetOwnerId')
+        if m.get('workspaceId') is not None:
+            self.workspace_id = m.get('workspaceId')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
+class HandOverWorkspaceResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class HandOverWorkspaceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: HandOverWorkspaceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = HandOverWorkspaceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListNodesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -3767,7 +4047,144 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListWorkspacesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SetDefaultHandOverUserHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SetDefaultHandOverUserRequest(TeaModel):
+    def __init__(
+        self,
+        default_handover_user_id: str = None,
+        operator_id: str = None,
+    ):
+        self.default_handover_user_id = default_handover_user_id
+        self.operator_id = operator_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.default_handover_user_id is not None:
+            result['defaultHandoverUserId'] = self.default_handover_user_id
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('defaultHandoverUserId') is not None:
+            self.default_handover_user_id = m.get('defaultHandoverUserId')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
+class SetDefaultHandOverUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+    ):
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class SetDefaultHandOverUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetDefaultHandOverUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetDefaultHandOverUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,112 @@
         self,
         request: dingtalkworkflow__1__0_models.AddProcessInstanceCommentRequest,
     ) -> dingtalkworkflow__1__0_models.AddProcessInstanceCommentResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkworkflow__1__0_models.AddProcessInstanceCommentHeaders()
         return await self.add_process_instance_comment_with_options_async(request, headers, runtime)
 
+    def batch_execute_process_instances_with_options(
+        self,
+        request: dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesRequest,
+        headers: dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.actioner_user_id):
+            body['actionerUserId'] = request.actioner_user_id
+        if not UtilClient.is_unset(request.remark):
+            body['remark'] = request.remark
+        if not UtilClient.is_unset(request.result):
+            body['result'] = request.result
+        if not UtilClient.is_unset(request.task_info_list):
+            body['taskInfoList'] = request.task_info_list
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchExecuteProcessInstances',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/processInstances/batchExecute',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def batch_execute_process_instances_with_options_async(
+        self,
+        request: dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesRequest,
+        headers: dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.actioner_user_id):
+            body['actionerUserId'] = request.actioner_user_id
+        if not UtilClient.is_unset(request.remark):
+            body['remark'] = request.remark
+        if not UtilClient.is_unset(request.result):
+            body['result'] = request.result
+        if not UtilClient.is_unset(request.task_info_list):
+            body['taskInfoList'] = request.task_info_list
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchExecuteProcessInstances',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/processInstances/batchExecute',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def batch_execute_process_instances(
+        self,
+        request: dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesRequest,
+    ) -> dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesHeaders()
+        return self.batch_execute_process_instances_with_options(request, headers, runtime)
+
+    async def batch_execute_process_instances_async(
+        self,
+        request: dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesRequest,
+    ) -> dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesHeaders()
+        return await self.batch_execute_process_instances_with_options_async(request, headers, runtime)
+
     def batch_update_process_instance_with_options(
         self,
         request: dingtalkworkflow__1__0_models.BatchUpdateProcessInstanceRequest,
         headers: dingtalkworkflow__1__0_models.BatchUpdateProcessInstanceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkworkflow__1__0_models.BatchUpdateProcessInstanceResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,14 +483,47 @@
             self.component_type = m.get('componentType')
         if m.get('props') is not None:
             temp_model = FormComponentProps()
             self.props = temp_model.from_map(m['props'])
         return self
 
 
+class ResultValue(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+        message: str = None,
+    ):
+        self.result = result
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        if self.message is not None:
+            result['message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        return self
+
+
 class AddApproveDentryAuthHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -916,14 +949,218 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddProcessInstanceCommentResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchExecuteProcessInstancesHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class BatchExecuteProcessInstancesRequestTaskInfoList(TeaModel):
+    def __init__(
+        self,
+        process_instance_id: str = None,
+        task_id: int = None,
+    ):
+        self.process_instance_id = process_instance_id
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.process_instance_id is not None:
+            result['processInstanceId'] = self.process_instance_id
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('processInstanceId') is not None:
+            self.process_instance_id = m.get('processInstanceId')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        return self
+
+
+class BatchExecuteProcessInstancesRequest(TeaModel):
+    def __init__(
+        self,
+        actioner_user_id: str = None,
+        remark: str = None,
+        result: str = None,
+        task_info_list: List[BatchExecuteProcessInstancesRequestTaskInfoList] = None,
+    ):
+        self.actioner_user_id = actioner_user_id
+        self.remark = remark
+        self.result = result
+        self.task_info_list = task_info_list
+
+    def validate(self):
+        if self.task_info_list:
+            for k in self.task_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.actioner_user_id is not None:
+            result['actionerUserId'] = self.actioner_user_id
+        if self.remark is not None:
+            result['remark'] = self.remark
+        if self.result is not None:
+            result['result'] = self.result
+        result['taskInfoList'] = []
+        if self.task_info_list is not None:
+            for k in self.task_info_list:
+                result['taskInfoList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('actionerUserId') is not None:
+            self.actioner_user_id = m.get('actionerUserId')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        self.task_info_list = []
+        if m.get('taskInfoList') is not None:
+            for k in m.get('taskInfoList'):
+                temp_model = BatchExecuteProcessInstancesRequestTaskInfoList()
+                self.task_info_list.append(temp_model.from_map(k))
+        return self
+
+
+class BatchExecuteProcessInstancesResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: Dict[str, ResultValue] = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            for v in self.result.values():
+                if v:
+                    v.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = {}
+        if self.result is not None:
+            for k, v in self.result.items():
+                result['result'][k] = v.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = {}
+        if m.get('result') is not None:
+            for k, v in m.get('result').items():
+                temp_model = ResultValue()
+                self.result[k] = temp_model.from_map(v)
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class BatchExecuteProcessInstancesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchExecuteProcessInstancesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BatchExecuteProcessInstancesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BatchUpdateProcessInstanceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.14
+Version: 2.0.15
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.14/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.15/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 alibabacloud_dingtalk/calendar_1_0/models.py
 alibabacloud_dingtalk/carbon_1_0/__init__.py
 alibabacloud_dingtalk/carbon_1_0/client.py
 alibabacloud_dingtalk/carbon_1_0/models.py
 alibabacloud_dingtalk/card_1_0/__init__.py
 alibabacloud_dingtalk/card_1_0/client.py
 alibabacloud_dingtalk/card_1_0/models.py
+alibabacloud_dingtalk/check_in_1_0/__init__.py
+alibabacloud_dingtalk/check_in_1_0/client.py
+alibabacloud_dingtalk/check_in_1_0/models.py
 alibabacloud_dingtalk/chengfeng_1_0/__init__.py
 alibabacloud_dingtalk/chengfeng_1_0/client.py
 alibabacloud_dingtalk/chengfeng_1_0/models.py
 alibabacloud_dingtalk/conference_1_0/__init__.py
 alibabacloud_dingtalk/conference_1_0/client.py
 alibabacloud_dingtalk/conference_1_0/models.py
 alibabacloud_dingtalk/connector_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.14/setup.py` & `alibabacloud_dingtalk-2.0.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 17/05/2023
+Created on 18/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

