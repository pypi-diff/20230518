# Comparing `tmp/volcengine-1.0.90.tar.gz` & `tmp/volcengine-1.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volcengine-1.0.90.tar", last modified: Wed May 17 06:38:59 2023, max compression
+gzip compressed data, was "dist/volcengine-1.0.91.tar", last modified: Thu May 18 15:57:09 2023, max compression
```

## Comparing `volcengine-1.0.90.tar` & `volcengine-1.0.91.tar`

### file list

```diff
@@ -1,723 +1,724 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine.egg-info/
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      293 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    31507 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      590 2023-05-17 06:38:57.000000 volcengine-1.0.90/setup.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-05-17 06:38:59.000000 volcengine-1.0.90/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-17 06:38:59.000000 volcengine-1.0.90/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/iam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/iam/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13316 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/iam/IamService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/image_registry/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/image_registry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9173 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/image_registry/ImageRegistryService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/dcdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/dcdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15998 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/dcdn/DCDNService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/billing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/billing/BillingService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/code_pipeline/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/code_pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13140 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/code_pipeline/CodePipelineService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/cdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24979 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/cdn/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/vedit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vedit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vedit/VEditService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/vod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/vod/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/vod/models/response/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/response/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69254 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/response/response_vod_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/vod/models/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/request/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70979 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/request/request_vod_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/vod/models/business/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16138 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_common_pb2.py
--rw-r--r--   0 root         (0) root         (0)    25019 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_measure_pb2.py
--rw-r--r--   0 root         (0) root         (0)    23323 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_upload_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3416 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_edit_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22584 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_cdn_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28862 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_workflow_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6189 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_play_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_apps_manage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_callback_pb2.py
--rw-r--r--   0 root         (0) root         (0)    33240 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_media_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4332 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_smart_strategy_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4524 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/models/business/vod_space_pb2.py
--rw-r--r--   0 root         (0) root         (0)   106666 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/VodService.py
--rw-r--r--   0 root         (0) root         (0)    10577 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vod/VodServiceConfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/sms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/sms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8664 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/sms/SmsService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/util/Util.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/util/Functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/base/
--rw-r--r--   0 root         (0) root         (0)    10796 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/Service.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/Request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/base/models/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/base/models/base/
--rw-r--r--   0 root         (0) root         (0)     2736 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/base/base_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/base/models/business/
--rw-r--r--   0 root         (0) root         (0)     3671 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/deny_config_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3870 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/pull_to_push_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/record_manage_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/domain_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4484 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/relay_source_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/snapshot_manage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6454 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/stream_manage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5225 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/VQScore_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3922 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/base/models/business/addr_pb2.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/__init__.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/Credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/notify/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/notify/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11061 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/notify/notify.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/adblocker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/adblocker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/adblocker/AdBlockerService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/imagex/
--rw-r--r--   0 root         (0) root         (0)     3494 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imagex/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8973 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imagex/ImageXConfig.py
--rw-r--r--   0 root         (0) root         (0)    41797 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imagex/ImageXService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/imp/
--rw-r--r--   0 root         (0) root         (0)     4260 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/ImpService.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/ImpServiceConfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/imp/models/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/imp/models/base/
--rw-r--r--   0 root         (0) root         (0)     7196 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/base/base_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/imp/models/response/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/response/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9927 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/response/response_imp_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/imp/models/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/request/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7112 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/request/request_imp_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/imp/models/business/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/business/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14236 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/imp/models/business/imp_common_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/const/
--rw-r--r--   0 root         (0) root         (0)     1937 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/const/Const.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/const/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/visual/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/visual/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32492 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/visual/VisualService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/auth/
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/auth/MetaData.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/auth/SignParam.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/auth/SignResult.py
--rw-r--r--   0 root         (0) root         (0)     8531 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/auth/SignerV4.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/nlp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/nlp/NLPService.py
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/ApiInfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/livesaas/
--rw-r--r--   0 root         (0) root         (0)    15125 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/livesaas/LivesaasService.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/livesaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/verender/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/verender/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30090 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/verender/VerenderService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/content_security/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/content_security/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10533 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/content_security/ContentSecurityService.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/Policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/rtc/
--rw-r--r--   0 root         (0) root         (0)     2020 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/rtc/example_start_record.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/rtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/rtc/example_get_record_task.py
--rw-r--r--   0 root         (0) root         (0)      691 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/rtc/example_stop_reocrd.py
--rw-r--r--   0 root         (0) root         (0)     2137 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/rtc/RtcService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/dcdn/
--rw-r--r--   0 root         (0) root         (0)      488 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/stop_domain.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_domain_config.py
--rw-r--r--   0 root         (0) root         (0)      580 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_domain_logs.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/delete_domain.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_dcdn_region_and_isp.py
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      584 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_domain_isp_data.py
--rw-r--r--   0 root         (0) root         (0)      569 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_top_ips.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_top_domains.py
--rw-r--r--   0 root         (0) root         (0)      727 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_origin_statistics_detail.py
--rw-r--r--   0 root         (0) root         (0)      511 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_user_domains.py
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/start_domain.py
--rw-r--r--   0 root         (0) root         (0)      526 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/retry_purge_prefetch_task.py
--rw-r--r--   0 root         (0) root         (0)      469 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/get_purge_prefetch_task_quota.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_realtime_data.py
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_statistics_detail.py
--rw-r--r--   0 root         (0) root         (0)      811 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/update_domain_config.py
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_domain_region_data.py
--rw-r--r--   0 root         (0) root         (0)      570 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_top_urls.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_domain_pv_data.py
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_top_referers.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_domain_uv_data.py
--rw-r--r--   0 root         (0) root         (0)      643 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_origin_statistics.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_statistics.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/create_purge_prefetch_task.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/check_purge_prefetch_task.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/create_domain.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/dcdn/describe_origin_realtime_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/cdn/
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/add_cdn_certificate.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/list_resource_tags.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_district_isp_data.py
--rw-r--r--   0 root         (0) root         (0)      570 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_accounting_data.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/update_cdn_config.py
--rw-r--r--   0 root         (0) root         (0)      448 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/submit_unblock_task.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/list_cert_info.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_ip_list_info.py
--rw-r--r--   0 root         (0) root         (0)      400 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_ip_info.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cdn_region_and_isp.py
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      448 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/submit_preload_task.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/update_resource_tags.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/batch_deploy_cert.py
--rw-r--r--   0 root         (0) root         (0)      909 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/add_cdn_domain.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/list_cdn_cert_info.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/delete_cdn_domain.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_content_block_tasks.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_edge_top_status_code.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_origin_top_nrt_data.py
--rw-r--r--   0 root         (0) root         (0)      625 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_edge_top_statistical_data.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_content_quota.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cert_config.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_edge_nrt_data_summary.py
--rw-r--r--   0 root         (0) root         (0)      533 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_origin_top_status_code.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/stop_cdn_domain.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_accounting_summary.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_edge_statistical_data.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cdn_access_log.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cdn_data_detail.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_content_tasks.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/delete_resource_tags.py
--rw-r--r--   0 root         (0) root         (0)      414 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cdn_upper_ip.py
--rw-r--r--   0 root         (0) root         (0)      446 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/submit_block_task.py
--rw-r--r--   0 root         (0) root         (0)      717 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cdn_data.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/start_cdn_domain.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cdn_origin_data.py
--rw-r--r--   0 root         (0) root         (0)      356 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cdn_service.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_origin_nrt_data_summary.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_cdn_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/submit_refresh_task.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/describe_edge_top_nrt_data.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/add_resource_tags.py
--rw-r--r--   0 root         (0) root         (0)      452 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/cdn/list_cdn_domains.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vedit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vedit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vedit/example_edit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/cdn/
--rw-r--r--   0 root         (0) root         (0)      711 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/CreateCdnRefreshTaskExample.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/DescribeCdnIpExample.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnPvDataExample.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/DescribeVodDomainTrafficDataExample.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnStatusDataExample.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnUsageDataExample.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnTopAccessUrlExample.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnTasksExample.py
--rw-r--r--   0 root         (0) root         (0)      691 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/ListDomainExample.py
--rw-r--r--   0 root         (0) root         (0)      724 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/CreateCdnPreloadTaskExample.py
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnAccessLogExample.py
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/cdn/DescribeVodDomainBandwidthDataExample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/space/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/space/__init__.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/space/CreateSpaceExample.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/space/UpdateSpaceExample.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/space/ListSpaceExample.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/space/DescribeVodSpaceStorageDataExample.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/space/UpdateSpaceUploadConfigExample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/vedit/
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/vedit/GetDirectEditProgress.py
--rw-r--r--   0 root         (0) root         (0)      625 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/vedit/GetDirectEditResult.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/vedit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/vedit/SubmitDirectEditTaskAsync.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/workflow/
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/workflow/RetrieveTranscodeResultExample.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/workflow/WorkflowExample.py
--rw-r--r--   0 root         (0) root         (0)      747 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/workflow/GetWorkflowExecutionResultExample.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/workflow/GetWorkflowExecutionExample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/callback/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/callback/__init__.py
--rw-r--r--   0 root         (0) root         (0)      805 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/callback/AddCallbackSubscriptionExample.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/callback/SetCallbackEvent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/measure/
--rw-r--r--   0 root         (0) root         (0)      980 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSnapshotData.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/measure/__init__.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceEditDetailData.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceDetectStatisData.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceTranscodeData.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceSubtitleStatisData.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceWorkflowDetailData.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceAIStatisData.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/upload/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/upload/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/upload/UploadUrl.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/upload/CommitUploadInfoExample.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/upload/UploadMedia.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/upload/QueryUploadTaskInfo.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/upload/ApplyUploadInfoExample.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/upload/UploadMaterial.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/upload/UploadSts2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/subtitle/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/subtitle/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/subtitle/SubtitleExample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/play/
--rw-r--r--   0 root         (0) root         (0)      839 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/play/GetPlayInfoExample.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/play/GetHlsDrmAuthTokenExample.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/play/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/play/GetAllPlayInfoExample.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/play/GetPlayAuthTokenExample.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/play/GetPrivateDrmPlayAuthExample.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/play/GetPlayInfoWithLiveTimeShiftSceneExample.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/play/GetPrivateDrmPlayAuthTokenExample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vod/media/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/media/__init__.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/media/GetSubtitleAuthToken.py
--rw-r--r--   0 root         (0) root         (0)     7520 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/media/MediaExample.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vod/media/GetSubtitleToken.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/sms/
--rw-r--r--   0 root         (0) root         (0)      790 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_apply_sms_signature.py
--rw-r--r--   0 root         (0) root         (0)      870 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_send_batch_sms.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_vms_template_query.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      713 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_get_sub_account_list.py
--rw-r--r--   0 root         (0) root         (0)      716 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_delete_sms_template.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_get_sms_template_and_order_list.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_get_signature_and_order_list.py
--rw-r--r--   0 root         (0) root         (0)     1216 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_apply_sms_template.py
--rw-r--r--   0 root         (0) root         (0)      605 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_conversion.py
--rw-r--r--   0 root         (0) root         (0)     1403 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_apply_vms_template.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_get_sub_account_detail.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_insert_sms_sub_account.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_delete_signature.py
--rw-r--r--   0 root         (0) root         (0)     1324 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_send_sms.py
--rw-r--r--   0 root         (0) root         (0)      819 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sms/example_send_vms.py
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/notify/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_remuse_task.py
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_single_info.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_create_tts.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_batch_append_task.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_create_task.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/__init__.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/examplae_sigle_batch_append.py
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_pause_task.py
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_get_reource_upload_url.py
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_open_update_resource.py
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_delete_resource.py
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_single_cancle.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_query_usable_resource.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_stop_task.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_query_open_get_resource.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_fetch_resource.py
--rw-r--r--   0 root         (0) root         (0)      342 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_commit_resource_upload.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/notify/example_update_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/imagex/
--rw-r--r--   0 root         (0) root         (0)      501 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_common.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_upload_sts2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/__init__.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_upload_image.py
--rw-r--r--   0 root         (0) root         (0)      660 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_fetch_url.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_content_block_list.py
--rw-r--r--   0 root         (0) root         (0)      591 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_enhance_result_with_data.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_create_image_content_task.py
--rw-r--r--   0 root         (0) root         (0)      539 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_content_task_detail.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_erase_result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/imagex/data/
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/edge_request.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/mirror_request_bandwidth.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/domain_bandwidth_data.py
--rw-r--r--   0 root         (0) root         (0)      554 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/edge_request_traffic.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/imagex_summary.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/edge_request_region.py
--rw-r--r--   0 root         (0) root         (0)      548 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/compress_usage.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/hit_rate_request_data.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/request_cnt_usage.py
--rw-r--r--   0 root         (0) root         (0)      546 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/bucket_usage.py
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/cdn_top_request_data.py
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/mirror_request_http_code_by_time.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/edge_request_bandwidth.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/domain_traffic_data.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/mirror_request_http_code_overview.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/mirror_request_traffic.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/hit_rate_traffic_data.py
--rw-r--r--   0 root         (0) root         (0)      547 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/data/bucket_base_op_usage.py
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_update_storage_ttl.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_super_resolution_result.py
--rw-r--r--   0 root         (0) root         (0)      533 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_bg_fill_result.py
--rw-r--r--   0 root         (0) root         (0)      570 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_enhance_result.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_style_result.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_delete_image.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_describe_imagex_volc_cdn_access_log.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_license_plate_detection.py
--rw-r--r--   0 root         (0) root         (0)      477 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_comic_result.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/examle_get_image_erase_models.py
--rw-r--r--   0 root         (0) root         (0)      406 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_info.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_upload_image_token.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_segment.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imagex/example_get_image_ocr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/imp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imp/RetrieveJob.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imp/SubmitJob.py
--rw-r--r--   0 root         (0) root         (0)      771 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/imp/KillJob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/visual/
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_summarization_query_task.py
--rw-r--r--   0 root         (0) root         (0)      504 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_over_resolution_submit_task.py
--rw-r--r--   0 root         (0) root         (0)     4340 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_common.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_image_search_image_delete.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_scene_detect.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/__init__.py
--rw-r--r--   0 root         (0) root         (0)      471 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_product_search_delete_image.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_inpaint_query_task.py
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_image_search_image_search.py
--rw-r--r--   0 root         (0) root         (0)      474 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_image_outpaint.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_image_search_image_add.py
--rw-r--r--   0 root         (0) root         (0)      540 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_retargeting_submit_task.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_ocr_demo.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_product_search_search_image.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_over_resolution_query_task.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_cover_selection.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_over_resolution.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_product_search_add_image.py
--rw-r--r--   0 root         (0) root         (0)      488 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_inpaint_submit_task.py
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_goods_detect.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_highlight_extraction_submit_task.py
--rw-r--r--   0 root         (0) root         (0)      506 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_highlight_extraction_query_task.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_summarization_submit_task.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_entity_detect.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_goods_segment.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_image_inpaint.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_video_retargeting_query_task.py
--rw-r--r--   0 root         (0) root         (0)      469 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_image_cut.py
--rw-r--r--   0 root         (0) root         (0)     2647 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/visual/example_cert_verify.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/nlp/
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/nlp/example_text_correction_zh_correct.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/nlp/example_keyphrase_extraction_extract.py
--rw-r--r--   0 root         (0) root         (0)      440 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/nlp/example_sentiment_analysis.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/nlp/example_essay_auto_grade.py
--rw-r--r--   0 root         (0) root         (0)      468 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/nlp/example_text_correction_en_correct.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/nlp/example_text_summarization.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/nlp/example_novel_correction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/livesaas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/livesaas/example_comment/
--rw-r--r--   0 root         (0) root         (0)      477 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_comment/example_presenter_chat_api.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_comment/__init__.py
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_comment/example_delete_chat_api.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/livesaas/example_replay_admin/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_replay_admin/example_list_medias_api.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_replay_admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_replay_admin/example_update_media_online_status_api.py
--rw-r--r--   0 root         (0) root         (0)      528 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_replay_admin/example_upload_replay_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_admin/
--rw-r--r--   0 root         (0) root         (0)      607 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_admin/example_list_activity_api.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_admin/example_create_activity_api.py
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_admin/example_delete_activity_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/
--rw-r--r--   0 root         (0) root         (0)      522 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_loop_video_status_api.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_get_activity_api.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_get_streams_api.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_activity_status_api.py
--rw-r--r--   0 root         (0) root         (0)     3115 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_activity_basic_config_api.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_pull_to_push_api.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_get_activity_basic_config_api.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_loop_video_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/livesaas/example_client_sdk/
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_client_sdk/example_get_sdk_token_api.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/livesaas/example_client_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/bioos/
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_create_workflow.py
--rw-r--r--   0 root         (0) root         (0)      570 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_delete_submission.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_create_cluster.py
--rw-r--r--   0 root         (0) root         (0)      495 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_workspaces.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_create_workspace.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_create_submission.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_delete_cluster.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_runs.py
--rw-r--r--   0 root         (0) root         (0)      539 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_data_models.py
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_submissions.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_clusters.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_delete_workspace.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_update_workspace.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_create_data_model.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_delete_data_model_rows_and_headers.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_workflows.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_bind_cluster_to_workspace.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_data_model_rows.py
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_unbind_cluster_and_workspace.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_delete_workflow.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_cancel_submission.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_cancel_run.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_clusters_of_workspace.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_list_tasks.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/bioos/example_update_workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/veen/
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/stop_instances.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/start_instances.py
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/delete_cloudserver.py
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/get_cloudserver.py
--rw-r--r--   0 root         (0) root         (0)      446 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/get_instance.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/list_instance_types.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/create_instance.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/list_cloudservers.py
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/stop_cloudserver.py
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/start_cloudserver.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/create_cloudserver.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/set_instance_name.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/reboot_cloudserver.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/reset_login_credential.py
--rw-r--r--   0 root         (0) root         (0)      609 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/list_instances.py
--rw-r--r--   0 root         (0) root         (0)      467 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/reboot_instances.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/get_instance_cloud_disk_info.py
--rw-r--r--   0 root         (0) root         (0)      656 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/scale_instance_cloud_disk_capacity.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/list_available_resource_info.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/veen/offline_instances.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/sts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      390 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/sts/example_assume_role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/rdspostgresql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/rdspostgresql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/rdspostgresql/example_create_instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/tls/
--rw-r--r--   0 root         (0) root         (0)     3913 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/tls/example_alarm.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/tls/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5626 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/tls/example_rule.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/tls/example_host_group.py
--rw-r--r--   0 root         (0) root         (0)     3723 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/tls/example_log.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/tls/example_topic.py
--rw-r--r--   0 root         (0) root         (0)     2572 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/tls/example_index.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/tls/example_project.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/DemoSignOnly.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/vms/
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vms/example_enable_or_disable_number.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vms/example_number_pool_list.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vms/example_select_number.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vms/example_number_list.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vms/example_query_can_call.py
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vms/example_update_number_pool.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/vms/example_create_number_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/secretnumber/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_unbind_axn.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_select_number_and_bind_axn.py
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_unbind_axyb.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axne.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/__init__.py
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_unbind_axne.py
--rw-r--r--   0 root         (0) root         (0)      525 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_query_subscription_for_list.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_query_subscription.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axb.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_click2_call_lite.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_bind_yb_for_axyb.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_upgrade_ax_to_axb.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_update_axne.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axyb.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_update_axyb.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axn.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axb_for_axne.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_unbind_axb.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_update_axn.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_select_number_and_bind_axb_form.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_update_axb.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/secretnumber/example_click2_call.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_vqs_task/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_vqs_task/__init__.py
--rw-r--r--   0 root         (0) root         (0)      528 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_vqs_task/example_create_v_q_score_task.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_vqs_task/example_list_v_q_score_task.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_vqs_task/example_describe_v_q_score_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_auth/example_describe_auth.py
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_auth/example_update_auth_key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_transcode/
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_transcode/example_list_vhost_transcode_preset.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_transcode/__init__.py
--rw-r--r--   0 root         (0) root         (0)      372 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_transcode/example_delete_transcode_preset.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_transcode/example_create_transcode_preset.py
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_transcode/example_list_common_trans_preset_detail.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_transcode/example_update_transcode_preset.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_cert/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_cert/example_update_cert.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_cert/example_bind_cert.py
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_cert/example_delete_cert.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_cert/__init__.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_cert/example_create_cert.py
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_cert/example_un_bind_cert.py
--rw-r--r--   0 root         (0) root         (0)      372 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_cert/example_list_cert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_generate_url/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_generate_url/__init__.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_generate_url/example_generate_play_u_r_l.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_generate_url/example_generate_push_u_r_l.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_audit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_audit/__init__.py
--rw-r--r--   0 root         (0) root         (0)      395 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_audit/example_delete_snapshot_audit_preset.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_audit/example_list_vhost_snapshot_audit_preset.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_audit/example_update_snapshot_audit_preset.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_audit/example_create_snapshot_audit_preset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_index_m3u8/
--rw-r--r--   0 root         (0) root         (0)      519 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_index_m3u8/example_create_live_stream_record_index_file.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_index_m3u8/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_usage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_usage/__init__.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_usage/describe_live_batch_push_stream_metrics.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_usage/describe_live_batch_source_stream_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_describe_info/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_describe_info/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_describe_info/example_describe_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_relay_source/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_relay_source/__init__.py
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_relay_source/example_update_relay_source_v2.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_relay_source/example_delete_relay_source_v2.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_relay_source/example_describe_relay_source_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_referer/
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_referer/example_update_referer.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_referer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      341 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_referer/example_delete_referer.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_referer/example_describe_referer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_callback/
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_callback/example_update_callback.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_callback/__init__.py
--rw-r--r--   0 root         (0) root         (0)      361 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_callback/example_delete_callback.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_callback/example_describe_callback.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_domain/example_create_domain.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_domain/example_disable_domain.py
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_domain/example_describe_domain.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_domain/example_list_domain_detail.py
--rw-r--r--   0 root         (0) root         (0)      328 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_domain/example_delete_domain.py
--rw-r--r--   0 root         (0) root         (0)      328 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_domain/example_enable_domain.py
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_domain/example_manager_pull_push_domain_bind.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_stream/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_stream/example_describe_forbidden_stream_info_by_page.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_stream/example_describe_closed_stream_info_by_page.py
--rw-r--r--   0 root         (0) root         (0)      446 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_stream/example_kill_stream.py
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_stream/example_describe_live_stream_state.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_stream/example_resume_stream.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_stream/example_forbid_stream.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_stream/example_describe_live_stream_info_by_page.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_record/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_record/example_create_record_preset.py
--rw-r--r--   0 root         (0) root         (0)      375 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_record/example_delete_record_preset.py
--rw-r--r--   0 root         (0) root         (0)      637 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_record/example_describe_record_task_file_history.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_record/__init__.py
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_record/example_list_vhost_record_preset.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_record/example_update_record_preset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_snapshot/
--rw-r--r--   0 root         (0) root         (0)      535 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_snapshot/example_update_snapshot_preset.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_snapshot/__init__.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_snapshot/example_delete_snapshot_preset.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_snapshot/example_create_snapshot_preset.py
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_snapshot/example_list_vhost_snapshot_preset.py
--rw-r--r--   0 root         (0) root         (0)      655 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_snapshot/example_describe_c_d_n_snapshot_history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/live/example_pull_to_push/
--rw-r--r--   0 root         (0) root         (0)      429 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_pull_to_push/example_stop_pull_to_push_task.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_pull_to_push/example_list_pull_to_push_task.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_pull_to_push/__init__.py
--rw-r--r--   0 root         (0) root         (0)      437 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_pull_to_push/example_delete_pull_to_push_task.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_pull_to_push/example_create_pull_to_push_task.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_pull_to_push/example_restart_pull_to_push_task.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/live/example_pull_to_push/example_update_pull_to_push_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/example/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/emr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/emr/example_list_clusters.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/example/emr/example_list_instance_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/bioos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/bioos/doc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/bioos/doc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/bioos/doc/source/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/bioos/doc/source/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/bioos/doc/source/conf.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/bioos/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46611 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/bioos/BioOsService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/veen/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/veen/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11746 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/veen/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/business_security/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/business_security/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5260 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/business_security/RiskDetectionService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/sts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/sts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1424 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/sts/StsService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/rdspostgresql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/rdspostgresql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/rdspostgresql/rdspostgresql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/tls/
--rw-r--r--   0 root         (0) root         (0)    15196 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/tls/tls_responses.py
--rw-r--r--   0 root         (0) root         (0)    35427 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/tls/TLSService.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/tls/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21704 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/tls/data.py
--rw-r--r--   0 root         (0) root         (0)    31907 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/tls/tls_requests.py
--rw-r--r--   0 root         (0) root         (0)     3099 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/tls/log_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6534 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/tls/const.py
--rw-r--r--   0 root         (0) root         (0)     1407 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/tls/tls_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/vms/
--rw-r--r--   0 root         (0) root         (0)     2298 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vms/risk.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/vms/NumberPoolService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/secretnumber/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/secretnumber/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3136 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/secretnumber/DatacenterService.py
--rw-r--r--   0 root         (0) root         (0)     9226 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/secretnumber/SecretNumberService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/live/
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/live/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/live/models/response/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/response/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27896 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/response/response_live_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/live/models/request/
--rw-r--r--   0 root         (0) root         (0)     1230 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/request/live_requests.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/request/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28008 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/request/request_live_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/live/models/business/
--rw-r--r--   0 root         (0) root         (0)     3682 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/deny_config_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3870 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/pull_to_push_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/record_manage_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/domain_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4488 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/relay_source_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/snapshot_manage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6407 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/stream_manage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2552 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/index_m3u8_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5225 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/VQScore_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3922 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/models/business/addr_pb2.py
--rw-r--r--   0 root         (0) root         (0)    52984 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/live/LiveService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/emr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5045 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/emr/EMRService.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:38:59.000000 volcengine-1.0.90/volcengine/game_protect/
--rw-r--r--   0 root         (0) root         (0)     1738 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/game_protect/GameProtectService.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/game_protect/__init__.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-05-17 06:38:57.000000 volcengine-1.0.90/volcengine/ServiceInfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-18 15:57:09.000000 volcengine-1.0.91/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      590 2023-05-18 15:57:06.000000 volcengine-1.0.91/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    31538 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/tls/
+-rw-r--r--   0 root         (0) root         (0)    35427 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/tls/TLSService.py
+-rw-r--r--   0 root         (0) root         (0)    15196 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/tls/tls_responses.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/tls/tls_exception.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/tls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21704 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/tls/data.py
+-rw-r--r--   0 root         (0) root         (0)    31907 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/tls/tls_requests.py
+-rw-r--r--   0 root         (0) root         (0)     6534 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/tls/const.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/tls/log_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/ServiceInfoHttps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/cdn/
+-rw-r--r--   0 root         (0) root         (0)    24979 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/cdn/service.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/cdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/Policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/billing/
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/billing/BillingService.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/vms/
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vms/NumberPoolService.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vms/risk.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/content_security/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/content_security/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10915 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/content_security/ContentSecurityService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/verender/
+-rw-r--r--   0 root         (0) root         (0)    30090 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/verender/VerenderService.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/verender/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/vedit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vedit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vedit/VEditService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/nlp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/nlp/NLPService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/veen/
+-rw-r--r--   0 root         (0) root         (0)    11746 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/veen/service.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/veen/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/adblocker/
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/adblocker/AdBlockerService.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/adblocker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/live/
+-rw-r--r--   0 root         (0) root         (0)    52984 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/LiveService.py
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/live/models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/live/models/response/
+-rw-r--r--   0 root         (0) root         (0)    27896 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/response/response_live_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/response/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/live/models/business/
+-rw-r--r--   0 root         (0) root         (0)     3922 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/addr_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/record_manage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/deny_config_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/index_m3u8_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/VQScore_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/snapshot_manage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6407 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/stream_manage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/domain_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4488 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/relay_source_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/business/pull_to_push_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/live/models/request/
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/request/live_requests.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/request/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28008 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/live/models/request/request_live_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/imp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/imp/models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/imp/models/response/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/response/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9927 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/response/response_imp_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/imp/models/business/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/business/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14236 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/business/imp_common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/imp/models/base/
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/base/base_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/imp/models/request/
+-rw-r--r--   0 root         (0) root         (0)     7112 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/request/request_imp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/models/request/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/ImpServiceConfig.py
+-rw-r--r--   0 root         (0) root         (0)     4260 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imp/ImpService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/auth/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/auth/SignParam.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/auth/SignResult.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8531 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/auth/SignerV4.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/auth/MetaData.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/game_protect/
+-rw-r--r--   0 root         (0) root         (0)     1738 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/game_protect/GameProtectService.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/game_protect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/image_registry/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/image_registry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9173 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/image_registry/ImageRegistryService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/code_pipeline/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/code_pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13140 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/code_pipeline/CodePipelineService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/livesaas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/livesaas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15125 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/livesaas/LivesaasService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/bioos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/bioos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/bioos/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/bioos/doc/source/
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/bioos/doc/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/bioos/doc/source/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/bioos/doc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46611 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/bioos/BioOsService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/util/
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/util/Functions.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/util/Util.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/const/
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/const/Const.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/const/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/ServiceInfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/visual/
+-rw-r--r--   0 root         (0) root         (0)    32492 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/visual/VisualService.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/visual/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/Credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/rdspostgresql/
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/rdspostgresql/rdspostgresql.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/rdspostgresql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/business_security/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/business_security/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5260 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/business_security/RiskDetectionService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/sms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/sms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/sms/SmsService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/dcdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/dcdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15998 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/dcdn/DCDNService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/notify/
+-rw-r--r--   0 root         (0) root         (0)    11061 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/notify/notify.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/notify/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/base/
+-rw-r--r--   0 root         (0) root         (0)    10796 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/Service.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/Request.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/base/models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/base/models/business/
+-rw-r--r--   0 root         (0) root         (0)     3922 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/addr_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/record_manage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/deny_config_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/VQScore_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/snapshot_manage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/stream_manage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/domain_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/relay_source_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/business/pull_to_push_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/base/models/base/
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/base/base_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/base/models/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/ApiInfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/secretnumber/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/secretnumber/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9226 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/secretnumber/SecretNumberService.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/secretnumber/DatacenterService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/iam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/iam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13316 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/iam/IamService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/sts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/sts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/sts/StsService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/tls/
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/tls/example_log.py
+-rw-r--r--   0 root         (0) root         (0)     5626 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/tls/example_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/tls/example_project.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/tls/example_index.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/tls/example_host_group.py
+-rw-r--r--   0 root         (0) root         (0)     3913 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/tls/example_alarm.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/tls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/tls/example_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/cdn/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_origin_nrt_data_summary.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_content_quota.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/start_cdn_domain.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/list_cert_info.py
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/submit_refresh_task.py
+-rw-r--r--   0 root         (0) root         (0)      414 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cdn_upper_ip.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/batch_deploy_cert.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_district_isp_data.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_edge_top_status_code.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/submit_block_task.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cdn_region_and_isp.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_origin_top_nrt_data.py
+-rw-r--r--   0 root         (0) root         (0)      521 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/update_resource_tags.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/list_cdn_cert_info.py
+-rw-r--r--   0 root         (0) root         (0)      860 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/update_cdn_config.py
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/list_cdn_domains.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_content_tasks.py
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      570 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_accounting_data.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cdn_config.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/delete_cdn_domain.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cert_config.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/add_cdn_certificate.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cdn_origin_data.py
+-rw-r--r--   0 root         (0) root         (0)      533 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_origin_top_status_code.py
+-rw-r--r--   0 root         (0) root         (0)      625 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_edge_top_statistical_data.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_edge_top_nrt_data.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_edge_nrt_data_summary.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/stop_cdn_domain.py
+-rw-r--r--   0 root         (0) root         (0)      400 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_ip_info.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_content_block_tasks.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_accounting_summary.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/list_resource_tags.py
+-rw-r--r--   0 root         (0) root         (0)      356 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cdn_service.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cdn_data_detail.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_edge_statistical_data.py
+-rw-r--r--   0 root         (0) root         (0)      448 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/submit_unblock_task.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/add_resource_tags.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cdn_access_log.py
+-rw-r--r--   0 root         (0) root         (0)      909 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/add_cdn_domain.py
+-rw-r--r--   0 root         (0) root         (0)      448 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/submit_preload_task.py
+-rw-r--r--   0 root         (0) root         (0)      717 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_cdn_data.py
+-rw-r--r--   0 root         (0) root         (0)      521 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/delete_resource_tags.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/cdn/describe_ip_list_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/rtc/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/rtc/example_get_record_task.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/rtc/example_start_record.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/rtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/rtc/example_stop_reocrd.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/rtc/RtcService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vms/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vms/example_enable_or_disable_number.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vms/example_query_can_call.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vms/example_number_pool_list.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      315 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vms/example_select_number.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vms/example_create_number_pool.py
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vms/example_update_number_pool.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vms/example_number_list.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/DemoSignOnly.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vedit/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vedit/example_edit.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vedit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/nlp/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/nlp/example_novel_correction.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/nlp/example_text_summarization.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/nlp/example_text_correction_zh_correct.py
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/nlp/example_keyphrase_extraction_extract.py
+-rw-r--r--   0 root         (0) root         (0)      440 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/nlp/example_sentiment_analysis.py
+-rw-r--r--   0 root         (0) root         (0)      468 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/nlp/example_text_correction_en_correct.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/nlp/example_essay_auto_grade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/veen/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/get_cloudserver.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/get_instance.py
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/scale_instance_cloud_disk_capacity.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/list_cloudservers.py
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/stop_cloudserver.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/delete_cloudserver.py
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/stop_instances.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/offline_instances.py
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/start_cloudserver.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/list_available_resource_info.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/list_instance_types.py
+-rw-r--r--   0 root         (0) root         (0)      467 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/reboot_instances.py
+-rw-r--r--   0 root         (0) root         (0)      609 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/list_instances.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/start_instances.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/reboot_cloudserver.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/reset_login_credential.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/set_instance_name.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/create_instance.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/create_cloudserver.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/veen/get_instance_cloud_disk_info.py
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_auth/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_auth/example_describe_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_auth/example_update_auth_key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_domain/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_domain/example_disable_domain.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_domain/example_list_domain_detail.py
+-rw-r--r--   0 root         (0) root         (0)      377 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_domain/example_describe_domain.py
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_domain/example_manager_pull_push_domain_bind.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_domain/example_create_domain.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      328 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_domain/example_enable_domain.py
+-rw-r--r--   0 root         (0) root         (0)      328 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_domain/example_delete_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_referer/
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_referer/example_update_referer.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_referer/example_describe_referer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_referer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      341 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_referer/example_delete_referer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_pull_to_push/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_pull_to_push/example_create_pull_to_push_task.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_pull_to_push/example_stop_pull_to_push_task.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_pull_to_push/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_pull_to_push/example_restart_pull_to_push_task.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_pull_to_push/example_list_pull_to_push_task.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_pull_to_push/example_update_pull_to_push_task.py
+-rw-r--r--   0 root         (0) root         (0)      437 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_pull_to_push/example_delete_pull_to_push_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_snapshot/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_snapshot/example_list_vhost_snapshot_preset.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_snapshot/example_update_snapshot_preset.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_snapshot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      655 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_snapshot/example_describe_c_d_n_snapshot_history.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_snapshot/example_delete_snapshot_preset.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_snapshot/example_create_snapshot_preset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_cert/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_cert/example_update_cert.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_cert/example_un_bind_cert.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_cert/example_bind_cert.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_cert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      372 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_cert/example_list_cert.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_cert/example_delete_cert.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_cert/example_create_cert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_record/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_record/example_describe_record_task_file_history.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_record/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_record/example_list_vhost_record_preset.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_record/example_create_record_preset.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_record/example_update_record_preset.py
+-rw-r--r--   0 root         (0) root         (0)      375 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_record/example_delete_record_preset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_stream/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_stream/example_describe_live_stream_state.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_stream/example_resume_stream.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_stream/example_describe_forbidden_stream_info_by_page.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_stream/example_describe_live_stream_info_by_page.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_stream/example_describe_closed_stream_info_by_page.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_stream/example_forbid_stream.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_stream/example_kill_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_generate_url/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_generate_url/example_generate_play_u_r_l.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_generate_url/example_generate_push_u_r_l.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_generate_url/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_describe_info/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_describe_info/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_describe_info/example_describe_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_usage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_usage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_usage/describe_live_batch_push_stream_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_usage/describe_live_batch_source_stream_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_transcode/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_transcode/example_list_common_trans_preset_detail.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_transcode/example_create_transcode_preset.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_transcode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_transcode/example_list_vhost_transcode_preset.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_transcode/example_update_transcode_preset.py
+-rw-r--r--   0 root         (0) root         (0)      372 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_transcode/example_delete_transcode_preset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_callback/
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_callback/example_update_callback.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_callback/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_callback/example_delete_callback.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_callback/example_describe_callback.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_relay_source/
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_relay_source/example_update_relay_source_v2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_relay_source/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_relay_source/example_describe_relay_source_v2.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_relay_source/example_delete_relay_source_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_vqs_task/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_vqs_task/example_describe_v_q_score_task.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_vqs_task/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_vqs_task/example_list_v_q_score_task.py
+-rw-r--r--   0 root         (0) root         (0)      528 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_vqs_task/example_create_v_q_score_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_index_m3u8/
+-rw-r--r--   0 root         (0) root         (0)      519 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_index_m3u8/example_create_live_stream_record_index_file.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_index_m3u8/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/live/example_audit/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_audit/example_list_vhost_snapshot_audit_preset.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_audit/example_create_snapshot_audit_preset.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_audit/example_update_snapshot_audit_preset.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_audit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      395 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/live/example_audit/example_delete_snapshot_audit_preset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/imp/
+-rw-r--r--   0 root         (0) root         (0)      771 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imp/KillJob.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imp/RetrieveJob.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imp/SubmitJob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/livesaas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_admin/
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_admin/example_create_activity_api.py
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_admin/example_delete_activity_api.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_admin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      607 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_admin/example_list_activity_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/livesaas/example_replay_admin/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_replay_admin/example_list_medias_api.py
+-rw-r--r--   0 root         (0) root         (0)      528 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_replay_admin/example_upload_replay_api.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_replay_admin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      523 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_replay_admin/example_update_media_online_status_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/
+-rw-r--r--   0 root         (0) root         (0)      640 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_pull_to_push_api.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_activity_basic_config_api.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_activity_status_api.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_loop_video_api.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_loop_video_status_api.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_get_activity_api.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_get_activity_basic_config_api.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_get_streams_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/livesaas/example_comment/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_comment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_comment/example_delete_chat_api.py
+-rw-r--r--   0 root         (0) root         (0)      477 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_comment/example_presenter_chat_api.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/livesaas/example_client_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_client_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/livesaas/example_client_sdk/example_get_sdk_token_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/bioos/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_tasks.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_delete_workflow.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_delete_workspace.py
+-rw-r--r--   0 root         (0) root         (0)      495 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_workspaces.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_delete_cluster.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_workflows.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_data_model_rows.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_bind_cluster_to_workspace.py
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_submissions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_create_data_model.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_update_workflow.py
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_create_cluster.py
+-rw-r--r--   0 root         (0) root         (0)      604 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_unbind_cluster_and_workspace.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_clusters_of_workspace.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_create_workflow.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_create_submission.py
+-rw-r--r--   0 root         (0) root         (0)      539 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_data_models.py
+-rw-r--r--   0 root         (0) root         (0)      570 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_delete_submission.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_runs.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_update_workspace.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_delete_data_model_rows_and_headers.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_list_clusters.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_create_workspace.py
+-rw-r--r--   0 root         (0) root         (0)      571 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_cancel_submission.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/bioos/example_cancel_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/visual/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_summarization_query_task.py
+-rw-r--r--   0 root         (0) root         (0)      471 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_product_search_delete_image.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_image_inpaint.py
+-rw-r--r--   0 root         (0) root         (0)      469 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_image_cut.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_image_outpaint.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_ocr_demo.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_common.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_over_resolution.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_goods_segment.py
+-rw-r--r--   0 root         (0) root         (0)      488 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_inpaint_submit_task.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_entity_detect.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_product_search_add_image.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_cert_verify.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_image_search_image_add.py
+-rw-r--r--   0 root         (0) root         (0)      506 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_highlight_extraction_query_task.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_highlight_extraction_submit_task.py
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_goods_detect.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_inpaint_query_task.py
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_over_resolution_submit_task.py
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_retargeting_submit_task.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_image_search_image_delete.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_product_search_search_image.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_over_resolution_query_task.py
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_image_search_image_search.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_retargeting_query_task.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_cover_selection.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_summarization_submit_task.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/visual/example_video_scene_detect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/rdspostgresql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/rdspostgresql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/rdspostgresql/example_create_instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/sms/
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_send_batch_sms.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_apply_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_delete_signature.py
+-rw-r--r--   0 root         (0) root         (0)      762 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_vms_template_query.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_send_vms.py
+-rw-r--r--   0 root         (0) root         (0)      639 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_delete_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_send_sms.py
+-rw-r--r--   0 root         (0) root         (0)      599 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_get_sms_template_and_order_list.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_apply_vms_template.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_get_sub_account_list.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_conversion.py
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_insert_sms_sub_account.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_apply_sms_signature.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_get_signature_and_order_list.py
+-rw-r--r--   0 root         (0) root         (0)      532 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sms/example_get_sub_account_detail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/dcdn/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_origin_realtime_data.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_domain_region_data.py
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_statistics_detail.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/delete_domain.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/create_domain.py
+-rw-r--r--   0 root         (0) root         (0)      580 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_domain_logs.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_dcdn_region_and_isp.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_domain_uv_data.py
+-rw-r--r--   0 root         (0) root         (0)      584 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_domain_isp_data.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_top_domains.py
+-rw-r--r--   0 root         (0) root         (0)      469 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/get_purge_prefetch_task_quota.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_statistics.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_realtime_data.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/create_purge_prefetch_task.py
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_domain_pv_data.py
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_user_domains.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/retry_purge_prefetch_task.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/check_purge_prefetch_task.py
+-rw-r--r--   0 root         (0) root         (0)      643 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_origin_statistics.py
+-rw-r--r--   0 root         (0) root         (0)      488 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/stop_domain.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_domain_config.py
+-rw-r--r--   0 root         (0) root         (0)      727 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_origin_statistics_detail.py
+-rw-r--r--   0 root         (0) root         (0)      570 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_top_urls.py
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/start_domain.py
+-rw-r--r--   0 root         (0) root         (0)      811 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/update_domain_config.py
+-rw-r--r--   0 root         (0) root         (0)      569 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_top_ips.py
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/dcdn/describe_top_referers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/notify/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_pause_task.py
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_remuse_task.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_query_open_get_resource.py
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_get_reource_upload_url.py
+-rw-r--r--   0 root         (0) root         (0)      342 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_commit_resource_upload.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_create_task.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_create_tts.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_fetch_resource.py
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_single_info.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/examplae_sigle_batch_append.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_batch_append_task.py
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_delete_resource.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_update_task.py
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_open_update_resource.py
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_single_cancle.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_stop_task.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/notify/example_query_usable_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/secretnumber/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axne.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axn.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_update_axne.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_click2_call_lite.py
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_unbind_axyb.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_query_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_update_axn.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axb_for_axne.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_unbind_axn.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_update_axyb.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_unbind_axb.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_select_number_and_bind_axn.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_click2_call.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_select_number_and_bind_axb_form.py
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_unbind_axne.py
+-rw-r--r--   0 root         (0) root         (0)      525 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_query_subscription_for_list.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_update_axb.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_upgrade_ax_to_axb.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_bind_yb_for_axyb.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axyb.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/sts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      390 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/sts/example_assume_role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/emr/example_list_instance_group.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/emr/example_list_clusters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/cdn/
+-rw-r--r--   0 root         (0) root         (0)      691 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/ListDomainExample.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/DescribeVodDomainTrafficDataExample.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnPvDataExample.py
+-rw-r--r--   0 root         (0) root         (0)      711 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/CreateCdnRefreshTaskExample.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnStatusDataExample.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/DescribeVodDomainBandwidthDataExample.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnUsageDataExample.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnTasksExample.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/DescribeCdnIpExample.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnTopAccessUrlExample.py
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnAccessLogExample.py
+-rw-r--r--   0 root         (0) root         (0)      724 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/cdn/CreateCdnPreloadTaskExample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/workflow/
+-rw-r--r--   0 root         (0) root         (0)      959 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/workflow/WorkflowExample.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/workflow/GetWorkflowExecutionExample.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/workflow/GetWorkflowExecutionResultExample.py
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/workflow/RetrieveTranscodeResultExample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/upload/
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/upload/UploadUrl.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/upload/UploadSts2.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/upload/QueryUploadTaskInfo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/upload/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/upload/CommitUploadInfoExample.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/upload/ApplyUploadInfoExample.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/upload/UploadMedia.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/upload/UploadMaterial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/subtitle/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/subtitle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/subtitle/SubtitleExample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/vedit/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/vedit/GetDirectEditResult.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/vedit/SubmitDirectEditTaskAsync.py
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/vedit/GetDirectEditProgress.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/vedit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/measure/
+-rw-r--r--   0 root         (0) root         (0)      902 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceEditDetailData.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSnapshotData.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceDetectStatisData.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceAIStatisData.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceTranscodeData.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/measure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceSubtitleStatisData.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceWorkflowDetailData.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/play/
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/play/GetPrivateDrmPlayAuthExample.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/play/GetPlayInfoWithLiveTimeShiftSceneExample.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/play/GetHlsDrmAuthTokenExample.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/play/GetPlayInfoExample.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/play/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/play/GetAllPlayInfoExample.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/play/GetPlayAuthTokenExample.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/play/GetPrivateDrmPlayAuthTokenExample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/space/
+-rw-r--r--   0 root         (0) root         (0)      732 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/space/UpdateSpaceExample.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/space/DescribeVodSpaceStorageDataExample.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/space/CreateSpaceExample.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/space/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/space/ListSpaceExample.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/space/UpdateSpaceUploadConfigExample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/callback/
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/callback/SetCallbackEvent.py
+-rw-r--r--   0 root         (0) root         (0)      805 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/callback/AddCallbackSubscriptionExample.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/callback/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/vod/media/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/media/GetSubtitleToken.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/media/GetSubtitleAuthToken.py
+-rw-r--r--   0 root         (0) root         (0)     7520 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/vod/media/MediaExample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/imagex/
+-rw-r--r--   0 root         (0) root         (0)      502 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_erase_result.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/examle_get_image_erase_models.py
+-rw-r--r--   0 root         (0) root         (0)      533 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_bg_fill_result.py
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_license_plate_detection.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_common.py
+-rw-r--r--   0 root         (0) root         (0)      539 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_content_task_detail.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_upload_image_token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/example/imagex/data/
+-rw-r--r--   0 root         (0) root         (0)      546 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/bucket_usage.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/hit_rate_traffic_data.py
+-rw-r--r--   0 root         (0) root         (0)      547 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/bucket_base_op_usage.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/domain_traffic_data.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/mirror_request_http_code_overview.py
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/mirror_request_http_code_by_time.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/hit_rate_request_data.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/edge_request_bandwidth.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/request_cnt_usage.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/cdn_top_request_data.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/mirror_request_bandwidth.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/imagex_summary.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/domain_bandwidth_data.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/edge_request_region.py
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/compress_usage.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/edge_request.py
+-rw-r--r--   0 root         (0) root         (0)      554 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/edge_request_traffic.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/data/mirror_request_traffic.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_delete_image.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_content_block_list.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_upload_sts2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      477 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_comic_result.py
+-rw-r--r--   0 root         (0) root         (0)      570 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_enhance_result.py
+-rw-r--r--   0 root         (0) root         (0)      660 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_fetch_url.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_segment.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_create_image_content_task.py
+-rw-r--r--   0 root         (0) root         (0)      591 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_enhance_result_with_data.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_upload_image.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_describe_imagex_volc_cdn_access_log.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_style_result.py
+-rw-r--r--   0 root         (0) root         (0)      406 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_info.py
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_update_storage_ttl.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_ocr.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/example/imagex/example_get_image_super_resolution_result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/emr/EMRService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/vod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10577 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/VodServiceConfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/vod/models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/vod/models/response/
+-rw-r--r--   0 root         (0) root         (0)    70194 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/response/response_vod_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/response/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/vod/models/business/
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_space_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_smart_strategy_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    26767 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_measure_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22701 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_cdn_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_apps_manage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6189 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_play_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    33240 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_media_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_callback_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    23323 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_upload_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28862 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_workflow_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3416 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_edit_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16138 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/business/vod_common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/vod/models/request/
+-rw-r--r--   0 root         (0) root         (0)    71933 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/request/request_vod_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/models/request/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   106666 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/vod/VodService.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:57:09.000000 volcengine-1.0.91/volcengine/imagex/
+-rw-r--r--   0 root         (0) root         (0)     3494 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imagex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8973 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imagex/ImageXConfig.py
+-rw-r--r--   0 root         (0) root         (0)    41797 2023-05-18 15:57:06.000000 volcengine-1.0.91/volcengine/imagex/ImageXService.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-18 15:57:09.000000 volcengine-1.0.91/PKG-INFO
```

### Comparing `volcengine-1.0.90/volcengine.egg-info/SOURCES.txt` & `volcengine-1.0.91/volcengine.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 setup.py
 volcengine/ApiInfo.py
 volcengine/Credentials.py
 volcengine/Policy.py
 volcengine/ServiceInfo.py
+volcengine/ServiceInfoHttps.py
 volcengine/__init__.py
 volcengine.egg-info/PKG-INFO
 volcengine.egg-info/SOURCES.txt
 volcengine.egg-info/dependency_links.txt
 volcengine.egg-info/requires.txt
 volcengine.egg-info/top_level.txt
 volcengine/adblocker/AdBlockerService.py
```

### Comparing `volcengine-1.0.90/setup.py` & `volcengine-1.0.91/setup.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/iam/IamService.py` & `volcengine-1.0.91/volcengine/iam/IamService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/image_registry/ImageRegistryService.py` & `volcengine-1.0.91/volcengine/image_registry/ImageRegistryService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/dcdn/DCDNService.py` & `volcengine-1.0.91/volcengine/dcdn/DCDNService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/billing/BillingService.py` & `volcengine-1.0.91/volcengine/billing/BillingService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/code_pipeline/CodePipelineService.py` & `volcengine-1.0.91/volcengine/code_pipeline/CodePipelineService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/cdn/service.py` & `volcengine-1.0.91/volcengine/cdn/service.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vedit/VEditService.py` & `volcengine-1.0.91/volcengine/vedit/VEditService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/response/response_vod_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/response/response_vod_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from volcengine.vod.models.business import vod_cdn_pb2 as vod_dot_business_dot_vod__cdn__pb2
 from volcengine.vod.models.business import vod_common_pb2 as vod_dot_business_dot_vod__common__pb2
 from volcengine.vod.models.business import vod_smart_strategy_pb2 as vod_dot_business_dot_vod__smart__strategy__pb2
 from volcengine.vod.models.business import vod_apps_manage_pb2 as vod_dot_business_dot_vod__apps__manage__pb2
 from volcengine.vod.models.business import vod_measure_pb2 as vod_dot_business_dot_vod__measure__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fvod/response/response_vod.proto\x12\x1eVolcengine.Vod.Models.Response\x1a\x0f\x62\x61se/base.proto\x1a\x1bvod/business/vod_play.proto\x1a\x1cvod/business/vod_media.proto\x1a\x1dvod/business/vod_upload.proto\x1a\x1fvod/business/vod_workflow.proto\x1a\x1bvod/business/vod_edit.proto\x1a\x1cvod/business/vod_space.proto\x1a\x1avod/business/vod_cdn.proto\x1a\x1dvod/business/vod_common.proto\x1a%vod/business/vod_smart_strategy.proto\x1a\"vod/business/vod_apps_manage.proto\x1a\x1evod/business/vod_measure.proto\"\xaa\x01\n\x19VodGetAllPlayInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x44\n\x06Result\x18\x02 \x01(\x0b\x32\x34.Volcengine.Vod.Models.Business.VodAllPlayInfoResult\"\xa3\x01\n\x16VodGetPlayInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12@\n\x06Result\x18\x02 \x01(\x0b\x32\x30.Volcengine.Vod.Models.Business.VodPlayInfoModel\"\xb7\x01\n\x1eVodGetOriginalPlayInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12L\n\x06Result\x18\x02 \x01(\x0b\x32<.Volcengine.Vod.Models.Business.VodGetOriginalPlayInfoResult\"\xbb\x01\n VodGetPrivateDrmPlayAuthResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12N\n\x06Result\x18\x02 \x01(\x0b\x32>.Volcengine.Vod.Models.Business.VodGetPrivateDrmPlayAuthResult\"\xb7\x01\n\x1eVodGetHlsDecryptionKeyResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12L\n\x06Result\x18\x02 \x01(\x0b\x32<.Volcengine.Vod.Models.Business.VodGetHlsDecryptionKeyResult\"\xd3\x01\n,VodGetPlayInfoWithLiveTimeShiftSceneResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12Z\n\x06Result\x18\x02 \x01(\x0b\x32J.Volcengine.Vod.Models.Business.VodGetPlayInfoWithLiveTimeShiftSceneResult\"\xa0\x01\n\x16VodUploadMediaResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12=\n\x06Result\x18\x02 \x01(\x0b\x32-.Volcengine.Vod.Models.Business.VodCommitData\"\xa7\x01\n\x1eVodQueryUploadTaskInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12<\n\x06Result\x18\x02 \x01(\x0b\x32,.Volcengine.Vod.Models.Business.VodQueryData\"\xa3\x01\n\x14VodUrlUploadResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x42\n\x06Result\x18\x02 \x01(\x0b\x32\x32.Volcengine.Vod.Models.Business.VodUrlResponseData\"\xaf\x01\n\x1aVodApplyUploadInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12H\n\x06Result\x18\x02 \x01(\x0b\x32\x38.Volcengine.Vod.Models.Business.VodApplyUploadInfoResult\"\xb1\x01\n\x1bVodCommitUploadInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12I\n\x06Result\x18\x02 \x01(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodCommitUploadInfoResult\"\xa9\x01\n\x18VodGetMediaInfosResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x44\n\x06Result\x18\x02 \x01(\x0b\x32\x34.Volcengine.Vod.Models.Business.VodGetMediaInfosData\"e\n\x1aVodUpdateMediaInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xaf\x01\n\x1fVodGetRecommendedPosterResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x01(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodGetRecPosterData\"n\n#VodUpdateMediaPublishStatusResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xbd\x01\n\"VodUpdateMediaStorageClassResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12N\n\x06Result\x18\x02 \x01(\x0b\x32>.Volcengine.Vod.Models.Business.VodUpdateMediaStorageClassData\"\xa5\x01\n\x16VodDeleteMediaResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x42\n\x06Result\x18\x02 \x01(\x0b\x32\x32.Volcengine.Vod.Models.Business.VodDeleteMediaData\"\xaf\x01\n\x1bVodDeleteTranscodesResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12G\n\x06Result\x18\x02 \x01(\x0b\x32\x37.Volcengine.Vod.Models.Business.VodDeleteTranscodesData\"\xa7\x01\n\x17VodGetMediaListResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x01(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodGetMediaListData\"\xb5\x01\n\x1eVodGetSubtitleInfoListResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12J\n\x06Result\x18\x02 \x01(\x0b\x32:.Volcengine.Vod.Models.Business.VodGetSubtitleInfoListData\"\xb7\x01\n\x1fVodUpdateSubtitleStatusResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12K\n\x06Result\x18\x02 \x01(\x0b\x32;.Volcengine.Vod.Models.Business.VodUpdateSubtitleStatusData\"h\n\x1dVodUpdateSubtitleInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xb8\x01\n!VodGetAuditFramesForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12J\n\x06Result\x18\x02 \x01(\x0b\x32:.Volcengine.Vod.Models.Business.VodGetFramesForAuditResult\"\xb5\x01\n\x1eVodGetMLFramesForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12J\n\x06Result\x18\x02 \x01(\x0b\x32:.Volcengine.Vod.Models.Business.VodGetFramesForAuditResult\"\xbf\x01\n\"VodGetBetterFramesForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12P\n\x06Result\x18\x02 \x01(\x0b\x32@.Volcengine.Vod.Models.Business.VodGetBetterFramesForAuditResult\"\xb9\x01\n\x1fVodGetAudioInfoForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12M\n\x06Result\x18\x02 \x01(\x0b\x32=.Volcengine.Vod.Models.Business.VodGetAudioInfoForAuditResult\"\xdb\x01\n0VodGetAutomaticSpeechRecognitionForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12^\n\x06Result\x18\x02 \x01(\x0b\x32N.Volcengine.Vod.Models.Business.VodGetAutomaticSpeechRecognitionForAuditResult\"\xcd\x01\n)VodGetAudioEventDetectionForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12W\n\x06Result\x18\x02 \x01(\x0b\x32G.Volcengine.Vod.Models.Business.VodGetAudioEventDetectionForAuditResult\"\xc1\x01\n$VodCreateVideoClassificationResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12P\n\x06Result\x18\x02 \x01(\x0b\x32@.Volcengine.Vod.Models.Business.VodCreateVideoClassificationData\"o\n$VodUpdateVideoClassificationResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"o\n$VodDeleteVideoClassificationResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xbb\x01\n#VodListVideoClassificationsResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12K\n\x06Result\x18\x02 \x01(\x0b\x32;.Volcengine.Vod.Models.Business.VodVideoClassificationsData\"\xa4\x01\n\x18VodListSnapshotsResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12?\n\x06Result\x18\x02 \x01(\x0b\x32/.Volcengine.Vod.Models.Business.VodSnapshotData\"\xa7\x01\n\x16VodGetFileListResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x44\n\x06Result\x18\x02 \x01(\x0b\x32\x34.Volcengine.Vod.Models.Business.VodGetMediaInfosData\"j\n\x1fVodExtractMediaMetaTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xab\x01\n\x18VodStartWorkflowResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x46\n\x06Result\x18\x02 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodStartWorkflowResult\"\xae\x01\n\"VodRetrieveTranscodeResultResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12?\n\x06Result\x18\x02 \x01(\x0b\x32/.Volcengine.Vod.Models.Business.TranscodeResult\"\xbb\x01\n VodListWorkflowExecutionResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12N\n\x06Result\x18\x02 \x01(\x0b\x32>.Volcengine.Vod.Models.Business.VodListWorkflowExecutionResult\"\xc5\x01\n%VodGetWorkflowExecutionDetailResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12S\n\x06Result\x18\x02 \x01(\x0b\x32\x43.Volcengine.Vod.Models.Business.VodGetWorkflowExecutionDetailResult\"\xb3\x01\n%VodGetWorkflowExecutionStatusResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x41\n\x06Result\x18\x02 \x01(\x0b\x32\x31.Volcengine.Vod.Models.Business.WorkflowExecution\"\xaa\x01\n\x1cVodGetWorkflowResultResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x41\n\x06Result\x18\x02 \x01(\x0b\x32\x31.Volcengine.Vod.Models.Business.VodWorkflowResult\"\xc0\x01\n$VodSubmitDirectEditTaskAsyncResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12O\n\x06Result\x18\x02 \x01(\x0b\x32?.Volcengine.Vod.Models.Business.SubmitDirectEditTaskAsyncResult\"\xb2\x01\n VodGetDirectEditProgressResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x45\n\x06Result\x18\x02 \x01(\x0b\x32\x35.Volcengine.Vod.Models.Business.GetDirectEditProgress\"\xae\x01\n\x1eVodGetDirectEditResultResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x03(\x0b\x32\x33.Volcengine.Vod.Models.Business.GetDirectEditResult\"a\n\x16VodCreateSpaceResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\x9d\x01\n\x14VodListSpaceResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12<\n\x06Result\x18\x02 \x03(\x0b\x32,.Volcengine.Vod.Models.Business.VodSpaceInfo\"\xa2\x01\n\x19VodGetSpaceDetailResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12<\n\x06Result\x18\x02 \x01(\x0b\x32,.Volcengine.Vod.Models.Business.VodSpaceInfo\"a\n\x16VodUpdateSpaceResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"m\n\"VodUpdateSpaceUploadConfigResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xc7\x01\n&VodDescribeVodSpaceStorageDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12T\n\x06Result\x18\x02 \x01(\x0b\x32\x44.Volcengine.Vod.Models.Business.VodDescribeVodSpaceStorageDataResult\"\xa5\x01\n\x15VodListDomainResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x01(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodDomainConfigInfo\"\xb2\x01\n\x1fVodCreateCdnRefreshTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x46\n\x06Result\x18\x02 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodCreateCdnTaskResult\"\xb2\x01\n\x1fVodCreateCdnPreloadTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x46\n\x06Result\x18\x02 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodCreateCdnTaskResult\"\xa4\x01\n\x17VodListCdnTasksResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12@\n\x06Result\x18\x02 \x01(\x0b\x32\x30.Volcengine.Vod.Models.Business.VodCdnTaskResult\"\xb1\x01\n\x1bVodListCdnAccessLogResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12I\n\x06Result\x18\x02 \x01(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodListCdnAccessLogResult\"\xb7\x01\n\x1eVodListCdnTopAccessUrlResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12L\n\x06Result\x18\x02 \x01(\x0b\x32<.Volcengine.Vod.Models.Business.VodListCdnTopAccessUrlResult\"\xcd\x01\n)VodDescribeVodDomainBandwidthDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12W\n\x06Result\x18\x02 \x01(\x0b\x32G.Volcengine.Vod.Models.Business.VodDescribeVodDomainBandwidthDataResult\"\xb7\x01\n\x1eVodCdnStatisticsCommonResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12L\n\x06Result\x18\x02 \x01(\x0b\x32<.Volcengine.Vod.Models.Business.VodCdnStatisticsCommonResult\"\xa2\x01\n\x19VodDescribeIPInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12<\n\x06Result\x18\x02 \x03(\x0b\x32,.Volcengine.Vod.Models.Business.VodCdnIpInfo\"\xc9\x01\n\'VodDescribeVodDomainTrafficDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12U\n\x06Result\x18\x02 \x01(\x0b\x32\x45.Volcengine.Vod.Models.Business.VodDescribeVodDomainTrafficDataResult\"\xb1\x01\n\x1bVodSubmitBlockTasksResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12I\n\x06Result\x18\x02 \x01(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodSubmitBlockTasksResult\"\xb9\x01\n\x1fVodGetContentBlockTasksResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12M\n\x06Result\x18\x02 \x01(\x0b\x32=.Volcengine.Vod.Models.Business.VodGetContentBlockTasksResult\"d\n\x19VodCreateDomainV2Response\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"j\n\x1fVodUpdateDomainExpireV2Response\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"n\n#VodUpdateDomainAuthConfigV2Response\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"m\n\"VodAddCallbackSubscriptionResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"f\n\x1bVodSetCallbackEventResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xc9\x01\n\'VodGetSmartStrategyLitePlayInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12U\n\x06Result\x18\x02 \x01(\x0b\x32\x45.Volcengine.Vod.Models.Business.VodGetSmartStrategyLitePlayInfoResult\"\xa5\x01\n\x15VodGetAppInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x01(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodGetAppInfoResult\"\xc5\x01\n%DescribeVodSpaceTranscodeDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12S\n\x06Result\x18\x02 \x01(\x0b\x32\x43.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeDataResult\"\xc3\x01\n$DescribeVodSpaceAIStatisDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12R\n\x06Result\x18\x02 \x01(\x0b\x32\x42.Volcengine.Vod.Models.Business.DescribeVodSpaceAIStatisDataResult\"\xcf\x01\n*DescribeVodSpaceSubtitleStatisDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12X\n\x06Result\x18\x02 \x01(\x0b\x32H.Volcengine.Vod.Models.Business.DescribeVodSpaceSubtitleStatisDataResult\"\xcb\x01\n(DescribeVodSpaceDetectStatisDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12V\n\x06Result\x18\x02 \x01(\x0b\x32\x46.Volcengine.Vod.Models.Business.DescribeVodSpaceDetectStatisDataResult\"\xb9\x01\n\x1f\x44\x65scribeVodSnapshotDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12M\n\x06Result\x18\x02 \x01(\x0b\x32=.Volcengine.Vod.Models.Business.DescribeVodSnapshotDataResult\"\xcf\x01\n*DescribeVodSpaceWorkflowDetailDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12X\n\x06Result\x18\x02 \x01(\x0b\x32H.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowDetailDataResult\"\xc7\x01\n&DescribeVodSpaceEditDetailDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12T\n\x06Result\x18\x02 \x01(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodSpaceEditDetailDataResult\"\xb9\x01\n\x1fVodSubmitBlockMediaTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12M\n\x06Result\x18\x02 \x01(\x0b\x32=.Volcengine.Vod.Models.Business.VodSubmitBlockMediaTaskResult\"\xbd\x01\n!VodSubmitUnblockMediaTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12O\n\x06Result\x18\x02 \x01(\x0b\x32?.Volcengine.Vod.Models.Business.VodSubmitUnblockMediaTaskResult\"\xbb\x01\n VodQueryMediaBlockStatusResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12N\n\x06Result\x18\x02 \x01(\x0b\x32>.Volcengine.Vod.Models.Business.VodQueryMediaBlockStatusResultB\xcc\x01\n)com.volcengine.service.vod.model.responseB\x0bVodResponseP\x01ZAgithub.com/volcengine/volc-sdk-golang/service/vod/models/response\xa0\x01\x01\xd8\x01\x01\xca\x02 Volc\\Service\\Vod\\Models\\Response\xe2\x02#Volc\\Service\\Vod\\Models\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fvod/response/response_vod.proto\x12\x1eVolcengine.Vod.Models.Response\x1a\x0f\x62\x61se/base.proto\x1a\x1bvod/business/vod_play.proto\x1a\x1cvod/business/vod_media.proto\x1a\x1dvod/business/vod_upload.proto\x1a\x1fvod/business/vod_workflow.proto\x1a\x1bvod/business/vod_edit.proto\x1a\x1cvod/business/vod_space.proto\x1a\x1avod/business/vod_cdn.proto\x1a\x1dvod/business/vod_common.proto\x1a%vod/business/vod_smart_strategy.proto\x1a\"vod/business/vod_apps_manage.proto\x1a\x1evod/business/vod_measure.proto\"\xaa\x01\n\x19VodGetAllPlayInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x44\n\x06Result\x18\x02 \x01(\x0b\x32\x34.Volcengine.Vod.Models.Business.VodAllPlayInfoResult\"\xa3\x01\n\x16VodGetPlayInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12@\n\x06Result\x18\x02 \x01(\x0b\x32\x30.Volcengine.Vod.Models.Business.VodPlayInfoModel\"\xb7\x01\n\x1eVodGetOriginalPlayInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12L\n\x06Result\x18\x02 \x01(\x0b\x32<.Volcengine.Vod.Models.Business.VodGetOriginalPlayInfoResult\"\xbb\x01\n VodGetPrivateDrmPlayAuthResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12N\n\x06Result\x18\x02 \x01(\x0b\x32>.Volcengine.Vod.Models.Business.VodGetPrivateDrmPlayAuthResult\"\xb7\x01\n\x1eVodGetHlsDecryptionKeyResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12L\n\x06Result\x18\x02 \x01(\x0b\x32<.Volcengine.Vod.Models.Business.VodGetHlsDecryptionKeyResult\"\xd3\x01\n,VodGetPlayInfoWithLiveTimeShiftSceneResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12Z\n\x06Result\x18\x02 \x01(\x0b\x32J.Volcengine.Vod.Models.Business.VodGetPlayInfoWithLiveTimeShiftSceneResult\"\xa0\x01\n\x16VodUploadMediaResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12=\n\x06Result\x18\x02 \x01(\x0b\x32-.Volcengine.Vod.Models.Business.VodCommitData\"\xa7\x01\n\x1eVodQueryUploadTaskInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12<\n\x06Result\x18\x02 \x01(\x0b\x32,.Volcengine.Vod.Models.Business.VodQueryData\"\xa3\x01\n\x14VodUrlUploadResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x42\n\x06Result\x18\x02 \x01(\x0b\x32\x32.Volcengine.Vod.Models.Business.VodUrlResponseData\"\xaf\x01\n\x1aVodApplyUploadInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12H\n\x06Result\x18\x02 \x01(\x0b\x32\x38.Volcengine.Vod.Models.Business.VodApplyUploadInfoResult\"\xb1\x01\n\x1bVodCommitUploadInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12I\n\x06Result\x18\x02 \x01(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodCommitUploadInfoResult\"\xa9\x01\n\x18VodGetMediaInfosResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x44\n\x06Result\x18\x02 \x01(\x0b\x32\x34.Volcengine.Vod.Models.Business.VodGetMediaInfosData\"e\n\x1aVodUpdateMediaInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xaf\x01\n\x1fVodGetRecommendedPosterResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x01(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodGetRecPosterData\"n\n#VodUpdateMediaPublishStatusResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xbd\x01\n\"VodUpdateMediaStorageClassResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12N\n\x06Result\x18\x02 \x01(\x0b\x32>.Volcengine.Vod.Models.Business.VodUpdateMediaStorageClassData\"\xa5\x01\n\x16VodDeleteMediaResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x42\n\x06Result\x18\x02 \x01(\x0b\x32\x32.Volcengine.Vod.Models.Business.VodDeleteMediaData\"\xaf\x01\n\x1bVodDeleteTranscodesResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12G\n\x06Result\x18\x02 \x01(\x0b\x32\x37.Volcengine.Vod.Models.Business.VodDeleteTranscodesData\"\xa7\x01\n\x17VodGetMediaListResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x01(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodGetMediaListData\"\xb5\x01\n\x1eVodGetSubtitleInfoListResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12J\n\x06Result\x18\x02 \x01(\x0b\x32:.Volcengine.Vod.Models.Business.VodGetSubtitleInfoListData\"\xb7\x01\n\x1fVodUpdateSubtitleStatusResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12K\n\x06Result\x18\x02 \x01(\x0b\x32;.Volcengine.Vod.Models.Business.VodUpdateSubtitleStatusData\"h\n\x1dVodUpdateSubtitleInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xb8\x01\n!VodGetAuditFramesForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12J\n\x06Result\x18\x02 \x01(\x0b\x32:.Volcengine.Vod.Models.Business.VodGetFramesForAuditResult\"\xb5\x01\n\x1eVodGetMLFramesForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12J\n\x06Result\x18\x02 \x01(\x0b\x32:.Volcengine.Vod.Models.Business.VodGetFramesForAuditResult\"\xbf\x01\n\"VodGetBetterFramesForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12P\n\x06Result\x18\x02 \x01(\x0b\x32@.Volcengine.Vod.Models.Business.VodGetBetterFramesForAuditResult\"\xb9\x01\n\x1fVodGetAudioInfoForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12M\n\x06Result\x18\x02 \x01(\x0b\x32=.Volcengine.Vod.Models.Business.VodGetAudioInfoForAuditResult\"\xdb\x01\n0VodGetAutomaticSpeechRecognitionForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12^\n\x06Result\x18\x02 \x01(\x0b\x32N.Volcengine.Vod.Models.Business.VodGetAutomaticSpeechRecognitionForAuditResult\"\xcd\x01\n)VodGetAudioEventDetectionForAuditResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12W\n\x06Result\x18\x02 \x01(\x0b\x32G.Volcengine.Vod.Models.Business.VodGetAudioEventDetectionForAuditResult\"\xc1\x01\n$VodCreateVideoClassificationResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12P\n\x06Result\x18\x02 \x01(\x0b\x32@.Volcengine.Vod.Models.Business.VodCreateVideoClassificationData\"o\n$VodUpdateVideoClassificationResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"o\n$VodDeleteVideoClassificationResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xbb\x01\n#VodListVideoClassificationsResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12K\n\x06Result\x18\x02 \x01(\x0b\x32;.Volcengine.Vod.Models.Business.VodVideoClassificationsData\"\xa4\x01\n\x18VodListSnapshotsResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12?\n\x06Result\x18\x02 \x01(\x0b\x32/.Volcengine.Vod.Models.Business.VodSnapshotData\"\xa7\x01\n\x16VodGetFileListResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x44\n\x06Result\x18\x02 \x01(\x0b\x32\x34.Volcengine.Vod.Models.Business.VodGetMediaInfosData\"j\n\x1fVodExtractMediaMetaTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xab\x01\n\x18VodStartWorkflowResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x46\n\x06Result\x18\x02 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodStartWorkflowResult\"\xae\x01\n\"VodRetrieveTranscodeResultResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12?\n\x06Result\x18\x02 \x01(\x0b\x32/.Volcengine.Vod.Models.Business.TranscodeResult\"\xbb\x01\n VodListWorkflowExecutionResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12N\n\x06Result\x18\x02 \x01(\x0b\x32>.Volcengine.Vod.Models.Business.VodListWorkflowExecutionResult\"\xc5\x01\n%VodGetWorkflowExecutionDetailResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12S\n\x06Result\x18\x02 \x01(\x0b\x32\x43.Volcengine.Vod.Models.Business.VodGetWorkflowExecutionDetailResult\"\xb3\x01\n%VodGetWorkflowExecutionStatusResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x41\n\x06Result\x18\x02 \x01(\x0b\x32\x31.Volcengine.Vod.Models.Business.WorkflowExecution\"\xaa\x01\n\x1cVodGetWorkflowResultResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x41\n\x06Result\x18\x02 \x01(\x0b\x32\x31.Volcengine.Vod.Models.Business.VodWorkflowResult\"\xc0\x01\n$VodSubmitDirectEditTaskAsyncResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12O\n\x06Result\x18\x02 \x01(\x0b\x32?.Volcengine.Vod.Models.Business.SubmitDirectEditTaskAsyncResult\"\xb2\x01\n VodGetDirectEditProgressResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x45\n\x06Result\x18\x02 \x01(\x0b\x32\x35.Volcengine.Vod.Models.Business.GetDirectEditProgress\"\xae\x01\n\x1eVodGetDirectEditResultResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x03(\x0b\x32\x33.Volcengine.Vod.Models.Business.GetDirectEditResult\"a\n\x16VodCreateSpaceResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\x9d\x01\n\x14VodListSpaceResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12<\n\x06Result\x18\x02 \x03(\x0b\x32,.Volcengine.Vod.Models.Business.VodSpaceInfo\"\xa2\x01\n\x19VodGetSpaceDetailResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12<\n\x06Result\x18\x02 \x01(\x0b\x32,.Volcengine.Vod.Models.Business.VodSpaceInfo\"a\n\x16VodUpdateSpaceResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"m\n\"VodUpdateSpaceUploadConfigResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xc7\x01\n&VodDescribeVodSpaceStorageDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12T\n\x06Result\x18\x02 \x01(\x0b\x32\x44.Volcengine.Vod.Models.Business.VodDescribeVodSpaceStorageDataResult\"\xa5\x01\n\x15VodListDomainResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x01(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodDomainConfigInfo\"\xb2\x01\n\x1fVodCreateCdnRefreshTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x46\n\x06Result\x18\x02 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodCreateCdnTaskResult\"\xb2\x01\n\x1fVodCreateCdnPreloadTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x46\n\x06Result\x18\x02 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodCreateCdnTaskResult\"\xa4\x01\n\x17VodListCdnTasksResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12@\n\x06Result\x18\x02 \x01(\x0b\x32\x30.Volcengine.Vod.Models.Business.VodCdnTaskResult\"\xb1\x01\n\x1bVodListCdnAccessLogResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12I\n\x06Result\x18\x02 \x01(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodListCdnAccessLogResult\"\xb7\x01\n\x1eVodListCdnTopAccessUrlResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12L\n\x06Result\x18\x02 \x01(\x0b\x32<.Volcengine.Vod.Models.Business.VodListCdnTopAccessUrlResult\"\xcd\x01\n)VodDescribeVodDomainBandwidthDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12W\n\x06Result\x18\x02 \x01(\x0b\x32G.Volcengine.Vod.Models.Business.VodDescribeVodDomainBandwidthDataResult\"\xb7\x01\n\x1eVodCdnStatisticsCommonResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12L\n\x06Result\x18\x02 \x01(\x0b\x32<.Volcengine.Vod.Models.Business.VodCdnStatisticsCommonResult\"\xa2\x01\n\x19VodDescribeIPInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12<\n\x06Result\x18\x02 \x03(\x0b\x32,.Volcengine.Vod.Models.Business.VodCdnIpInfo\"\xc9\x01\n\'VodDescribeVodDomainTrafficDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12U\n\x06Result\x18\x02 \x01(\x0b\x32\x45.Volcengine.Vod.Models.Business.VodDescribeVodDomainTrafficDataResult\"\xb1\x01\n\x1bVodSubmitBlockTasksResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12I\n\x06Result\x18\x02 \x01(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodSubmitBlockTasksResult\"\xb9\x01\n\x1fVodGetContentBlockTasksResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12M\n\x06Result\x18\x02 \x01(\x0b\x32=.Volcengine.Vod.Models.Business.VodGetContentBlockTasksResult\"d\n\x19VodCreateDomainV2Response\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"j\n\x1fVodUpdateDomainExpireV2Response\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"n\n#VodUpdateDomainAuthConfigV2Response\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"m\n\"VodAddCallbackSubscriptionResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"f\n\x1bVodSetCallbackEventResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\"\xc9\x01\n\'VodGetSmartStrategyLitePlayInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12U\n\x06Result\x18\x02 \x01(\x0b\x32\x45.Volcengine.Vod.Models.Business.VodGetSmartStrategyLitePlayInfoResult\"\xa5\x01\n\x15VodGetAppInfoResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12\x43\n\x06Result\x18\x02 \x01(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodGetAppInfoResult\"\xc5\x01\n%DescribeVodSpaceTranscodeDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12S\n\x06Result\x18\x02 \x01(\x0b\x32\x43.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeDataResult\"\xc3\x01\n$DescribeVodSpaceAIStatisDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12R\n\x06Result\x18\x02 \x01(\x0b\x32\x42.Volcengine.Vod.Models.Business.DescribeVodSpaceAIStatisDataResult\"\xcf\x01\n*DescribeVodSpaceSubtitleStatisDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12X\n\x06Result\x18\x02 \x01(\x0b\x32H.Volcengine.Vod.Models.Business.DescribeVodSpaceSubtitleStatisDataResult\"\xcb\x01\n(DescribeVodSpaceDetectStatisDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12V\n\x06Result\x18\x02 \x01(\x0b\x32\x46.Volcengine.Vod.Models.Business.DescribeVodSpaceDetectStatisDataResult\"\xb9\x01\n\x1f\x44\x65scribeVodSnapshotDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12M\n\x06Result\x18\x02 \x01(\x0b\x32=.Volcengine.Vod.Models.Business.DescribeVodSnapshotDataResult\"\xcf\x01\n*DescribeVodSpaceWorkflowDetailDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12X\n\x06Result\x18\x02 \x01(\x0b\x32H.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowDetailDataResult\"\xc7\x01\n&DescribeVodSpaceEditDetailDataResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12T\n\x06Result\x18\x02 \x01(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodSpaceEditDetailDataResult\"\xc7\x01\n&DescribeVodPlayFileLogByDomainResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12T\n\x06Result\x18\x02 \x01(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodPlayFileLogByDomainResult\"\xb9\x01\n\x1fVodSubmitBlockMediaTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12M\n\x06Result\x18\x02 \x01(\x0b\x32=.Volcengine.Vod.Models.Business.VodSubmitBlockMediaTaskResult\"\xbd\x01\n!VodSubmitUnblockMediaTaskResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12O\n\x06Result\x18\x02 \x01(\x0b\x32?.Volcengine.Vod.Models.Business.VodSubmitUnblockMediaTaskResult\"\xbb\x01\n VodQueryMediaBlockStatusResponse\x12G\n\x10ResponseMetadata\x18\x01 \x01(\x0b\x32-.Volcengine.Base.Models.Base.ResponseMetadata\x12N\n\x06Result\x18\x02 \x01(\x0b\x32>.Volcengine.Vod.Models.Business.VodQueryMediaBlockStatusResultB\xcc\x01\n)com.volcengine.service.vod.model.responseB\x0bVodResponseP\x01ZAgithub.com/volcengine/volc-sdk-golang/service/vod/models/response\xa0\x01\x01\xd8\x01\x01\xca\x02 Volc\\Service\\Vod\\Models\\Response\xe2\x02#Volc\\Service\\Vod\\Models\\GPBMetadatab\x06proto3')
 
 
 
 _VODGETALLPLAYINFORESPONSE = DESCRIPTOR.message_types_by_name['VodGetAllPlayInfoResponse']
 _VODGETPLAYINFORESPONSE = DESCRIPTOR.message_types_by_name['VodGetPlayInfoResponse']
 _VODGETORIGINALPLAYINFORESPONSE = DESCRIPTOR.message_types_by_name['VodGetOriginalPlayInfoResponse']
 _VODGETPRIVATEDRMPLAYAUTHRESPONSE = DESCRIPTOR.message_types_by_name['VodGetPrivateDrmPlayAuthResponse']
@@ -102,14 +102,15 @@
 _DESCRIBEVODSPACETRANSCODEDATARESPONSE = DESCRIPTOR.message_types_by_name['DescribeVodSpaceTranscodeDataResponse']
 _DESCRIBEVODSPACEAISTATISDATARESPONSE = DESCRIPTOR.message_types_by_name['DescribeVodSpaceAIStatisDataResponse']
 _DESCRIBEVODSPACESUBTITLESTATISDATARESPONSE = DESCRIPTOR.message_types_by_name['DescribeVodSpaceSubtitleStatisDataResponse']
 _DESCRIBEVODSPACEDETECTSTATISDATARESPONSE = DESCRIPTOR.message_types_by_name['DescribeVodSpaceDetectStatisDataResponse']
 _DESCRIBEVODSNAPSHOTDATARESPONSE = DESCRIPTOR.message_types_by_name['DescribeVodSnapshotDataResponse']
 _DESCRIBEVODSPACEWORKFLOWDETAILDATARESPONSE = DESCRIPTOR.message_types_by_name['DescribeVodSpaceWorkflowDetailDataResponse']
 _DESCRIBEVODSPACEEDITDETAILDATARESPONSE = DESCRIPTOR.message_types_by_name['DescribeVodSpaceEditDetailDataResponse']
+_DESCRIBEVODPLAYFILELOGBYDOMAINRESPONSE = DESCRIPTOR.message_types_by_name['DescribeVodPlayFileLogByDomainResponse']
 _VODSUBMITBLOCKMEDIATASKRESPONSE = DESCRIPTOR.message_types_by_name['VodSubmitBlockMediaTaskResponse']
 _VODSUBMITUNBLOCKMEDIATASKRESPONSE = DESCRIPTOR.message_types_by_name['VodSubmitUnblockMediaTaskResponse']
 _VODQUERYMEDIABLOCKSTATUSRESPONSE = DESCRIPTOR.message_types_by_name['VodQueryMediaBlockStatusResponse']
 VodGetAllPlayInfoResponse = _reflection.GeneratedProtocolMessageType('VodGetAllPlayInfoResponse', (_message.Message,), {
   'DESCRIPTOR' : _VODGETALLPLAYINFORESPONSE,
   '__module__' : 'vod.response.response_vod_pb2'
   # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Response.VodGetAllPlayInfoResponse)
@@ -637,14 +638,21 @@
 DescribeVodSpaceEditDetailDataResponse = _reflection.GeneratedProtocolMessageType('DescribeVodSpaceEditDetailDataResponse', (_message.Message,), {
   'DESCRIPTOR' : _DESCRIBEVODSPACEEDITDETAILDATARESPONSE,
   '__module__' : 'vod.response.response_vod_pb2'
   # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Response.DescribeVodSpaceEditDetailDataResponse)
   })
 _sym_db.RegisterMessage(DescribeVodSpaceEditDetailDataResponse)
 
+DescribeVodPlayFileLogByDomainResponse = _reflection.GeneratedProtocolMessageType('DescribeVodPlayFileLogByDomainResponse', (_message.Message,), {
+  'DESCRIPTOR' : _DESCRIBEVODPLAYFILELOGBYDOMAINRESPONSE,
+  '__module__' : 'vod.response.response_vod_pb2'
+  # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Response.DescribeVodPlayFileLogByDomainResponse)
+  })
+_sym_db.RegisterMessage(DescribeVodPlayFileLogByDomainResponse)
+
 VodSubmitBlockMediaTaskResponse = _reflection.GeneratedProtocolMessageType('VodSubmitBlockMediaTaskResponse', (_message.Message,), {
   'DESCRIPTOR' : _VODSUBMITBLOCKMEDIATASKRESPONSE,
   '__module__' : 'vod.response.response_vod_pb2'
   # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Response.VodSubmitBlockMediaTaskResponse)
   })
 _sym_db.RegisterMessage(VodSubmitBlockMediaTaskResponse)
 
@@ -814,14 +822,16 @@
   _DESCRIBEVODSPACEDETECTSTATISDATARESPONSE._serialized_end=12793
   _DESCRIBEVODSNAPSHOTDATARESPONSE._serialized_start=12796
   _DESCRIBEVODSNAPSHOTDATARESPONSE._serialized_end=12981
   _DESCRIBEVODSPACEWORKFLOWDETAILDATARESPONSE._serialized_start=12984
   _DESCRIBEVODSPACEWORKFLOWDETAILDATARESPONSE._serialized_end=13191
   _DESCRIBEVODSPACEEDITDETAILDATARESPONSE._serialized_start=13194
   _DESCRIBEVODSPACEEDITDETAILDATARESPONSE._serialized_end=13393
-  _VODSUBMITBLOCKMEDIATASKRESPONSE._serialized_start=13396
-  _VODSUBMITBLOCKMEDIATASKRESPONSE._serialized_end=13581
-  _VODSUBMITUNBLOCKMEDIATASKRESPONSE._serialized_start=13584
-  _VODSUBMITUNBLOCKMEDIATASKRESPONSE._serialized_end=13773
-  _VODQUERYMEDIABLOCKSTATUSRESPONSE._serialized_start=13776
-  _VODQUERYMEDIABLOCKSTATUSRESPONSE._serialized_end=13963
+  _DESCRIBEVODPLAYFILELOGBYDOMAINRESPONSE._serialized_start=13396
+  _DESCRIBEVODPLAYFILELOGBYDOMAINRESPONSE._serialized_end=13595
+  _VODSUBMITBLOCKMEDIATASKRESPONSE._serialized_start=13598
+  _VODSUBMITBLOCKMEDIATASKRESPONSE._serialized_end=13783
+  _VODSUBMITUNBLOCKMEDIATASKRESPONSE._serialized_start=13786
+  _VODSUBMITUNBLOCKMEDIATASKRESPONSE._serialized_end=13975
+  _VODQUERYMEDIABLOCKSTATUSRESPONSE._serialized_start=13978
+  _VODQUERYMEDIABLOCKSTATUSRESPONSE._serialized_end=14165
 # @@protoc_insertion_point(module_scope)
```

### Comparing `volcengine-1.0.90/volcengine/vod/models/request/request_vod_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/request/request_vod_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from volcengine.vod.models.business import vod_workflow_pb2 as vod_dot_business_dot_vod__workflow__pb2
 from volcengine.vod.models.business import vod_upload_pb2 as vod_dot_business_dot_vod__upload__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dvod/request/request_vod.proto\x12\x1dVolcengine.Vod.Models.Request\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fvod/business/vod_workflow.proto\x1a\x1dvod/business/vod_upload.proto\"\x84\x03\n\x18VodGetAllPlayInfoRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\x12\x0f\n\x07\x46ormats\x18\x02 \x01(\t\x12\x0e\n\x06\x43odecs\x18\x03 \x01(\t\x12\x13\n\x0b\x44\x65\x66initions\x18\x04 \x01(\t\x12\x11\n\tFileTypes\x18\x05 \x01(\t\x12\x11\n\tLogoTypes\x18\x06 \x01(\t\x12\x19\n\x11NeedEncryptStream\x18\x07 \x01(\t\x12\x0b\n\x03Ssl\x18\x08 \x01(\t\x12\x12\n\nNeedThumbs\x18\t \x01(\t\x12\x17\n\x0fNeedBarrageMask\x18\n \x01(\t\x12\x0f\n\x07\x43\x64nType\x18\x0b \x01(\t\x12\x11\n\tUnionInfo\x18\x0c \x01(\t\x12\x11\n\tPlayScene\x18\r \x01(\t\x12\x1a\n\x12\x44rmExpireTimestamp\x18\x0e \x01(\t\x12\x0f\n\x07HDRType\x18\x0f \x01(\t\x12 \n\x18KeyFrameAlignmentVersion\x18\x10 \x01(\t\x12\x12\n\nUserAction\x18\x11 \x01(\t\x12\x0f\n\x07Quality\x18\x12 \x01(\t\"\xd4\x02\n\x15VodGetPlayInfoRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0e\n\x06\x46ormat\x18\x02 \x01(\t\x12\r\n\x05\x43odec\x18\x03 \x01(\t\x12\x12\n\nDefinition\x18\x04 \x01(\t\x12\x10\n\x08\x46ileType\x18\x05 \x01(\t\x12\x10\n\x08LogoType\x18\x06 \x01(\t\x12\x0e\n\x06\x42\x61se64\x18\x07 \x01(\t\x12\x0b\n\x03Ssl\x18\x08 \x01(\t\x12\x12\n\nNeedThumbs\x18\t \x01(\t\x12\x17\n\x0fNeedBarrageMask\x18\n \x01(\t\x12\x0f\n\x07\x43\x64nType\x18\x0b \x01(\t\x12\x11\n\tUnionInfo\x18\x0c \x01(\t\x12\x15\n\rHDRDefinition\x18\r \x01(\t\x12\x11\n\tPlayScene\x18\x0e \x01(\t\x12\x1a\n\x12\x44rmExpireTimestamp\x18\x0f \x01(\t\x12\x0f\n\x07Quality\x18\x10 \x01(\t\x12\x12\n\nPlayConfig\x18\x11 \x01(\t\"g\n\x1fVodGetPrivateDrmPlayAuthRequest\x12\x0f\n\x07\x44rmType\x18\x01 \x01(\t\x12\x0b\n\x03Vid\x18\x02 \x01(\t\x12\x13\n\x0bPlayAuthIds\x18\x03 \x01(\t\x12\x11\n\tUnionInfo\x18\x04 \x01(\t\"Q\n\x1dVodGetHlsDecryptionKeyRequest\x12\x14\n\x0c\x44rmAuthToken\x18\x01 \x01(\t\x12\n\n\x02\x41k\x18\x02 \x01(\t\x12\x0e\n\x06Source\x18\x03 \x01(\t\"\x98\x01\n+VodGetPlayInfoWithLiveTimeShiftSceneRequest\x12\x11\n\tStoreUris\x18\x01 \x01(\t\x12\x11\n\tSpaceName\x18\x02 \x01(\t\x12\x0b\n\x03Ssl\x18\x03 \x01(\t\x12\x17\n\x0f\x45xpireTimestamp\x18\x04 \x01(\t\x12\x1d\n\x15NeedComposeBucketName\x18\x05 \x01(\t\"m\n\x13VodUrlUploadRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x43\n\x07URLSets\x18\x02 \x03(\x0b\x32\x32.Volcengine.Vod.Models.Business.VodUrlUploadURLSet\"/\n\x1dVodQueryUploadTaskInfoRequest\x12\x0e\n\x06JobIds\x18\x01 \x01(\t\"\xa5\x01\n\x19VodApplyUploadInfoRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nSessionKey\x18\x02 \x01(\t\x12\x10\n\x08\x46ileSize\x18\x03 \x01(\x01\x12\x10\n\x08\x46ileType\x18\x04 \x01(\t\x12\x10\n\x08\x46ileName\x18\x05 \x01(\t\x12\x14\n\x0cStorageClass\x18\x06 \x01(\x05\x12\x15\n\rFileExtension\x18\x07 \x01(\t\"\xbd\x01\n\x15VodUploadMediaRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x10\n\x08\x46ilePath\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\x12\x11\n\tFunctions\x18\x04 \x01(\t\x12\x10\n\x08\x46ileName\x18\x05 \x01(\t\x12\x14\n\x0cStorageClass\x18\x06 \x01(\x05\x12\x15\n\rFileExtension\x18\x07 \x01(\t\x12\x17\n\x0fVodUploadSource\x18\x08 \x01(\t\"\xa3\x01\n\x18VodUploadMaterialRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x10\n\x08\x46ilePath\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\x12\x11\n\tFunctions\x18\x04 \x01(\t\x12\x10\n\x08\x46ileType\x18\x05 \x01(\t\x12\x10\n\x08\x46ileName\x18\x06 \x01(\t\x12\x15\n\rFileExtension\x18\x07 \x01(\t\"\x85\x01\n\x1aVodCommitUploadInfoRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nSessionKey\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\x12\x11\n\tFunctions\x18\x04 \x01(\t\x12\x17\n\x0fVodUploadSource\x18\x05 \x01(\t\"=\n\x17VodUrlUploadJsonRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0f\n\x07URLSets\x18\x02 \x01(\t\".\n\x1eVodGetRecommendedPosterRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\"A\n\"VodUpdateMediaPublishStatusRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0e\n\x06Status\x18\x02 \x01(\t\"n\n!VodUpdateMediaStorageClassRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\x12\x14\n\x0cStorageClass\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\x12\x0f\n\x07\x46ileIds\x18\x04 \x01(\t\"\x9c\x02\n\x19VodUpdateMediaInfoRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12/\n\tPosterUri\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05Title\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x44\x65scription\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04Tags\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x35\n\x10\x43lassificationId\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\"\'\n\x17VodGetMediaInfosRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\";\n\x15VodDeleteMediaRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x02 \x01(\t\"P\n\x1aVodDeleteTranscodesRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0f\n\x07\x46ileIds\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\"\xfb\x01\n\x16VodGetMediaListRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0b\n\x03Vid\x18\x02 \x01(\t\x12\x0e\n\x06Status\x18\x03 \x01(\t\x12\r\n\x05Order\x18\x04 \x01(\t\x12\x0c\n\x04Tags\x18\x05 \x01(\t\x12\x11\n\tStartTime\x18\x06 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x07 \x01(\t\x12\x0e\n\x06Offset\x18\x08 \x01(\t\x12\x10\n\x08PageSize\x18\t \x01(\t\x12\x19\n\x11\x43lassificationIds\x18\n \x01(\t\x12\x19\n\x11TosStorageClasses\x18\x0b \x01(\t\x12\x18\n\x10VodUploadSources\x18\x0c \x01(\t\"\xe6\x01\n\x1dVodGetSubtitleInfoListRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0f\n\x07\x46ileIds\x18\x02 \x01(\t\x12\x11\n\tLanguages\x18\x03 \x01(\t\x12\x0f\n\x07\x46ormats\x18\x04 \x01(\t\x12\x13\n\x0bLanguageIds\x18\x05 \x01(\t\x12\x13\n\x0bSubtitleIds\x18\x06 \x01(\t\x12\x0e\n\x06Status\x18\x07 \x01(\t\x12\r\n\x05Title\x18\x08 \x01(\t\x12\x0b\n\x03Tag\x18\t \x01(\t\x12\x0e\n\x06Offset\x18\n \x01(\t\x12\x10\n\x08PageSize\x18\x0b \x01(\t\x12\x0b\n\x03Ssl\x18\x0c \x01(\t\"r\n\x1eVodUpdateSubtitleStatusRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0f\n\x07\x46ileIds\x18\x02 \x01(\t\x12\x11\n\tLanguages\x18\x03 \x01(\t\x12\x0f\n\x07\x46ormats\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\"\xb5\x01\n\x1cVodUpdateSubtitleInfoRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0e\n\x06\x46ileId\x18\x02 \x01(\t\x12\x10\n\x08Language\x18\x03 \x01(\t\x12\x0e\n\x06\x46ormat\x18\x04 \x01(\t\x12+\n\x05Title\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03Tag\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"w\n VodGetAuditFramesForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\x12\x19\n\x11MinNumberOfFrames\x18\x03 \x01(\t\x12\x19\n\x11MaxNumberOfFrames\x18\x04 \x01(\t\"\xa1\x02\n\x1dVodGetMLFramesForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\x12\x10\n\x08\x46rameOpt\x18\x03 \x01(\t\x12\x10\n\x08\x46rameFps\x18\x04 \x01(\t\x12\x16\n\x0eNumberOfFrames\x18\x05 \x01(\t\x12\x14\n\x0c\x43utTimeMills\x18\x06 \x01(\t\x12\x16\n\x0eNeedFirstFrame\x18\x07 \x01(\t\x12\x15\n\rNeedLastFrame\x18\x08 \x01(\t\x12\x15\n\rStartTimeMill\x18\t \x01(\t\x12\x13\n\x0b\x45ndTimeMill\x18\n \x01(\t\x12\x19\n\x11MinNumberOfFrames\x18\x0b \x01(\t\x12\x19\n\x11MaxNumberOfFrames\x18\x0c \x01(\t\"U\n!VodGetBetterFramesForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\x12\x11\n\tCoverRate\x18\x03 \x01(\t\"?\n\x1eVodGetAudioInfoForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\"P\n/VodGetAutomaticSpeechRecognitionForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\"I\n(VodGetAudioEventDetectionForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\"q\n#VodCreateVideoClassificationRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\r\n\x05Level\x18\x02 \x01(\x05\x12\x10\n\x08ParentId\x18\x03 \x01(\x03\x12\x16\n\x0e\x43lassification\x18\x04 \x01(\t\"j\n#VodUpdateVideoClassificationRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x18\n\x10\x43lassificationId\x18\x02 \x01(\x03\x12\x16\n\x0e\x43lassification\x18\x03 \x01(\t\"R\n#VodDeleteVideoClassificationRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x18\n\x10\x43lassificationId\x18\x02 \x01(\x03\"Q\n\"VodListVideoClassificationsRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x18\n\x10\x43lassificationId\x18\x02 \x01(\x03\"&\n\x17VodListSnapshotsRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\"Z\n\x15VodGetFileListRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0e\n\x06Prefix\x18\x02 \x01(\t\x12\r\n\x05Limit\x18\x03 \x01(\t\x12\x0f\n\x07Starter\x18\x04 \x01(\t\"-\n\x1eVodExtractMediaMetaTaskRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\"\x8e\x02\n\x17VodStartWorkflowRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x12\n\nTemplateId\x18\x02 \x01(\t\x12=\n\x05Input\x18\x03 \x01(\x0b\x32..Volcengine.Vod.Models.Business.WorkflowParams\x12\x10\n\x08Priority\x18\x04 \x01(\x05\x12\x14\n\x0c\x43\x61llbackArgs\x18\x05 \x01(\t\x12\x19\n\x11\x45nableLowPriority\x18\x06 \x01(\x08\x12<\n\tDirectUrl\x18\x07 \x01(\x0b\x32).Volcengine.Vod.Models.Business.DirectUrl\x12\x12\n\nTaskListId\x18\x08 \x01(\t\"D\n!VodRetrieveTranscodeResultRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x12\n\nResultType\x18\x02 \x01(\t\"\x9f\x02\n\x1fVodListWorkflowExecutionRequest\x12\r\n\x05RunId\x18\x01 \x01(\t\x12\x0b\n\x03Vid\x18\x02 \x01(\t\x12\x11\n\tSpaceName\x18\x03 \x01(\t\x12\x12\n\nTemplateId\x18\x04 \x01(\t\x12\x12\n\nTaskListId\x18\x05 \x01(\t\x12\x19\n\x11\x45nableLowPriority\x18\x06 \x01(\t\x12\x11\n\tJobSource\x18\x07 \x01(\t\x12\x0e\n\x06Status\x18\x08 \x01(\t\x12\x11\n\tStartTime\x18\t \x01(\t\x12\x0f\n\x07\x45ndTime\x18\n \x01(\t\x12\x10\n\x08PageSize\x18\x0b \x01(\t\x12\x0e\n\x06Offset\x18\x0c \x01(\t\x12\x12\n\nOrderByKey\x18\r \x01(\t\x12\r\n\x05Order\x18\x0e \x01(\t\"5\n$VodGetWorkflowExecutionDetailRequest\x12\r\n\x05RunId\x18\x01 \x01(\t\",\n\x1bVodGetWorkflowResultRequest\x12\r\n\x05RunId\x18\x01 \x01(\t\"N\n$VodGetWorkflowExecutionStatusRequest\x12\r\n\x05RunId\x18\x01 \x01(\t\x12\x17\n\x0fNeedTasksDetail\x18\x02 \x01(\t\"\x9c\x01\n#VodSubmitDirectEditTaskAsyncRequest\x12\x10\n\x08Uploader\x18\x01 \x01(\t\x12\x13\n\x0b\x41pplication\x18\x02 \x01(\t\x12\x11\n\tEditParam\x18\x04 \x01(\x0c\x12\x10\n\x08Priority\x18\x05 \x01(\x05\x12\x13\n\x0b\x43\x61llbackUri\x18\x06 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x07 \x01(\t\"/\n\x1dVodGetDirectEditResultRequest\x12\x0e\n\x06ReqIds\x18\x01 \x03(\t\"0\n\x1fVodGetDirectEditProgressRequest\x12\r\n\x05ReqId\x18\x01 \x01(\t\"v\n\x15VodCreateSpaceRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x13\n\x0bProjectName\x18\x02 \x01(\t\x12\x13\n\x0b\x44\x65scription\x18\x03 \x01(\t\x12\x0e\n\x06Region\x18\x04 \x01(\t\x12\x10\n\x08UserName\x18\x05 \x01(\t\"-\n\x18VodGetSpaceDetailRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\"4\n\x13VodListSpaceRequest\x12\x0e\n\x06Offset\x18\x01 \x01(\x01\x12\r\n\x05Limit\x18\x02 \x01(\x01\"u\n\x15VodUpdateSpaceRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x19\n\x11SourceProjectName\x18\x02 \x01(\t\x12\x19\n\x11TargetProjectName\x18\x03 \x01(\t\x12\x13\n\x0b\x44\x65scription\x18\x04 \x01(\t\"^\n!VodUpdateSpaceUploadConfigRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x11\n\tConfigKey\x18\x02 \x01(\t\x12\x13\n\x0b\x43onfigValue\x18\x03 \x01(\t\"\x81\x01\n%VodDescribeVodSpaceStorageDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x0c\n\x04Type\x18\x05 \x01(\t\")\n\x14VodListDomainRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\"O\n\x1eVodCreateCdnRefreshTaskRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Urls\x18\x02 \x01(\t\x12\x0c\n\x04Type\x18\x03 \x01(\t\"A\n\x1eVodCreateCdnPreloadTaskRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Urls\x18\x02 \x01(\t\"\xc2\x01\n\x16VodListCdnTasksRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0e\n\x06TaskId\x18\x02 \x01(\t\x12\x12\n\nDomainName\x18\x03 \x01(\t\x12\x10\n\x08TaskType\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x06 \x01(\x05\x12\x14\n\x0c\x45ndTimestamp\x18\x07 \x01(\x05\x12\x0f\n\x07PageNum\x18\x08 \x01(\x05\x12\x10\n\x08PageSize\x18\t \x01(\x05\"n\n\x1aVodListCdnAccessLogRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x02 \x01(\x05\x12\x14\n\x0c\x45ndTimestamp\x18\x03 \x01(\x05\x12\x11\n\tSpaceName\x18\x04 \x01(\t\"p\n\x1dVodListCdnTopAccessUrlRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x02 \x01(\x05\x12\x14\n\x0c\x45ndTimestamp\x18\x03 \x01(\x05\x12\x10\n\x08SortType\x18\x04 \x01(\t\"\x9c\x01\n(VodDescribeVodDomainBandwidthDataRequest\x12\x12\n\nDomainList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x15\n\rBandwidthType\x18\x05 \x01(\t\x12\x0c\n\x04\x41rea\x18\x06 \x01(\t\"\xa3\x01\n\x1aVodListCdnUsageDataRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x10\n\x08Interval\x18\x02 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x03 \x01(\x03\x12\x14\n\x0c\x45ndTimestamp\x18\x04 \x01(\x03\x12\x10\n\x08\x44\x61taType\x18\x05 \x01(\t\x12\x0e\n\x06Metric\x18\x06 \x01(\t\x12\x12\n\nNeedDetail\x18\x07 \x01(\x08\"\xa4\x01\n\x1bVodListCdnStatusDataRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x10\n\x08Interval\x18\x02 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x03 \x01(\x03\x12\x14\n\x0c\x45ndTimestamp\x18\x04 \x01(\x03\x12\x10\n\x08\x44\x61taType\x18\x05 \x01(\t\x12\x0e\n\x06Metric\x18\x06 \x01(\t\x12\x12\n\nNeedDetail\x18\x07 \x01(\x08\"\'\n\x18VodDescribeIPInfoRequest\x12\x0b\n\x03Ips\x18\x01 \x01(\t\"\x90\x01\n\x17VodListCdnPvDataRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x10\n\x08Interval\x18\x02 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x03 \x01(\x03\x12\x14\n\x0c\x45ndTimestamp\x18\x04 \x01(\x03\x12\x10\n\x08\x44\x61taType\x18\x05 \x01(\t\x12\x12\n\nNeedDetail\x18\x06 \x01(\x08\"\x93\x01\n\x1cVodListCdnHitrateDataRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x10\n\x08Interval\x18\x02 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x03 \x01(\x03\x12\x14\n\x0c\x45ndTimestamp\x18\x04 \x01(\x03\x12\x0e\n\x06Metric\x18\x05 \x01(\t\x12\x12\n\nNeedDetail\x18\x06 \x01(\x08\"\x8a\x01\n&VodDescribeVodDomainTrafficDataRequest\x12\x12\n\nDomainList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x13\n\x0bTrafficType\x18\x05 \x01(\t\"A\n\x1aVodSubmitBlockTasksRequest\x12\x10\n\x08\x46ileUrls\x18\x01 \x01(\t\x12\x11\n\tOperation\x18\x02 \x01(\t\"\xb6\x01\n\x1eVodGetContentBlockTasksRequest\x12\x0b\n\x03Url\x18\x01 \x01(\t\x12\x0e\n\x06\x44omain\x18\x02 \x01(\t\x12\x0e\n\x06TaskID\x18\x03 \x01(\t\x12\x10\n\x08TaskType\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\x12\x11\n\tStartTime\x18\x06 \x01(\x03\x12\x0f\n\x07\x45ndTime\x18\x07 \x01(\x03\x12\x0f\n\x07PageNum\x18\x08 \x01(\x03\x12\x10\n\x08PageSize\x18\t \x01(\x03\"\xc1\x01\n\x18VodCreateDomainV2Request\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nDomainType\x18\x02 \x01(\t\x12\x0e\n\x06\x44omain\x18\x03 \x01(\t\x12\x19\n\x11SourceStationType\x18\x05 \x01(\x05\x12 \n\x18SourceStationAddressType\x18\x06 \x01(\x05\x12\x0f\n\x07Origins\x18\x07 \x01(\t\x12\x0c\n\x04\x41rea\x18\x08 \x01(\t\x12\x12\n\nBucketName\x18\t \x01(\t\"g\n\x1eVodUpdateDomainExpireV2Request\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nDomainType\x18\x02 \x01(\t\x12\x0e\n\x06\x44omain\x18\x03 \x01(\t\x12\x0e\n\x06\x45xpire\x18\x04 \x01(\x05\"\x8f\x01\n\"VodUpdateDomainAuthConfigV2Request\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nDomainType\x18\x02 \x01(\t\x12\x0e\n\x06\x44omain\x18\x03 \x01(\t\x12\x0f\n\x07MainKey\x18\x04 \x01(\t\x12\x11\n\tBackupKey\x18\x05 \x01(\t\x12\x0e\n\x06Status\x18\x06 \x01(\t\"X\n!VodAddCallbackSubscriptionRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0b\n\x03Url\x18\x02 \x01(\t\x12\x13\n\x0b\x43ontentType\x18\x03 \x01(\t\"h\n\x1aVodSetCallbackEventRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0e\n\x06\x45vents\x18\x02 \x01(\t\x12\x13\n\x0b\x41uthEnabled\x18\x03 \x01(\t\x12\x12\n\nPrivateKey\x18\x04 \x01(\t\"\xf4\x01\n&VodGetSmartStrategyLitePlayInfoRequest\x12\x0f\n\x07PlayUrl\x18\x01 \x01(\t\x12\x0e\n\x06\x46ormat\x18\x02 \x01(\t\x12\r\n\x05\x43odec\x18\x03 \x01(\t\x12\x12\n\nDefinition\x18\x04 \x01(\t\x12\x10\n\x08\x46ileType\x18\x05 \x01(\t\x12\x10\n\x08LogoType\x18\x06 \x01(\t\x12\x0b\n\x03Ssl\x18\x07 \x01(\t\x12\x12\n\nNeedThumbs\x18\x08 \x01(\t\x12\x17\n\x0fNeedBarrageMask\x18\t \x01(\t\x12\x11\n\tUnionInfo\x18\n \x01(\t\x12\x15\n\rHDRDefinition\x18\x0b \x01(\t\"%\n\x14VodGetAppInfoRequest\x12\r\n\x05\x41ppId\x18\x01 \x01(\x04\"\xd0\x01\n$DescribeVodSpaceTranscodeDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x15\n\rTranscodeType\x18\x04 \x01(\t\x12\x15\n\rSpecification\x18\x05 \x01(\t\x12\x15\n\rTaskStageList\x18\x06 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x07 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x08 \x01(\t\"\xb6\x01\n#DescribeVodSpaceAIStatisDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0bMediaAiType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x01(\t\"\xbd\x01\n)DescribeVodSpaceSubtitleStatisDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x14\n\x0cSubtitleType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x01(\t\"\xb9\x01\n\'DescribeVodSpaceDetectStatisDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x12\n\nDetectType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x01(\t\"\xb2\x01\n\x1e\x44\x65scribeVodSnapshotDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x14\n\x0cSnapshotType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x01(\t\"\x91\x01\n)DescribeVodSpaceWorkflowDetailDataRequest\x12\x0e\n\x06Region\x18\x01 \x01(\t\x12\r\n\x05Space\x18\x02 \x01(\t\x12\x11\n\tStartTime\x18\x03 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x04 \x01(\t\x12\x10\n\x08PageSize\x18\x05 \x01(\x03\x12\x0f\n\x07PageNum\x18\x06 \x01(\x03\"\x8d\x01\n%DescribeVodSpaceEditDetailDataRequest\x12\x0e\n\x06Region\x18\x01 \x01(\t\x12\r\n\x05Space\x18\x02 \x01(\t\x12\x11\n\tStartTime\x18\x03 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x04 \x01(\t\x12\x10\n\x08PageSize\x18\x05 \x01(\x03\x12\x0f\n\x07PageNum\x18\x06 \x01(\x03\"A\n\x1eVodSubmitBlockMediaTaskRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Vids\x18\x02 \x01(\t\"C\n VodSubmitUnblockMediaTaskRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Vids\x18\x02 \x01(\t\"B\n\x1fVodQueryMediaBlockStatusRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Vids\x18\x02 \x01(\tB\xc8\x01\n(com.volcengine.service.vod.model.requestB\nVodRequestP\x01Z@github.com/volcengine/volc-sdk-golang/service/vod/models/request\xa0\x01\x01\xd8\x01\x01\xca\x02\x1fVolc\\Service\\Vod\\Models\\Request\xe2\x02#Volc\\Service\\Vod\\Models\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dvod/request/request_vod.proto\x12\x1dVolcengine.Vod.Models.Request\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fvod/business/vod_workflow.proto\x1a\x1dvod/business/vod_upload.proto\"\x84\x03\n\x18VodGetAllPlayInfoRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\x12\x0f\n\x07\x46ormats\x18\x02 \x01(\t\x12\x0e\n\x06\x43odecs\x18\x03 \x01(\t\x12\x13\n\x0b\x44\x65\x66initions\x18\x04 \x01(\t\x12\x11\n\tFileTypes\x18\x05 \x01(\t\x12\x11\n\tLogoTypes\x18\x06 \x01(\t\x12\x19\n\x11NeedEncryptStream\x18\x07 \x01(\t\x12\x0b\n\x03Ssl\x18\x08 \x01(\t\x12\x12\n\nNeedThumbs\x18\t \x01(\t\x12\x17\n\x0fNeedBarrageMask\x18\n \x01(\t\x12\x0f\n\x07\x43\x64nType\x18\x0b \x01(\t\x12\x11\n\tUnionInfo\x18\x0c \x01(\t\x12\x11\n\tPlayScene\x18\r \x01(\t\x12\x1a\n\x12\x44rmExpireTimestamp\x18\x0e \x01(\t\x12\x0f\n\x07HDRType\x18\x0f \x01(\t\x12 \n\x18KeyFrameAlignmentVersion\x18\x10 \x01(\t\x12\x12\n\nUserAction\x18\x11 \x01(\t\x12\x0f\n\x07Quality\x18\x12 \x01(\t\"\xd4\x02\n\x15VodGetPlayInfoRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0e\n\x06\x46ormat\x18\x02 \x01(\t\x12\r\n\x05\x43odec\x18\x03 \x01(\t\x12\x12\n\nDefinition\x18\x04 \x01(\t\x12\x10\n\x08\x46ileType\x18\x05 \x01(\t\x12\x10\n\x08LogoType\x18\x06 \x01(\t\x12\x0e\n\x06\x42\x61se64\x18\x07 \x01(\t\x12\x0b\n\x03Ssl\x18\x08 \x01(\t\x12\x12\n\nNeedThumbs\x18\t \x01(\t\x12\x17\n\x0fNeedBarrageMask\x18\n \x01(\t\x12\x0f\n\x07\x43\x64nType\x18\x0b \x01(\t\x12\x11\n\tUnionInfo\x18\x0c \x01(\t\x12\x15\n\rHDRDefinition\x18\r \x01(\t\x12\x11\n\tPlayScene\x18\x0e \x01(\t\x12\x1a\n\x12\x44rmExpireTimestamp\x18\x0f \x01(\t\x12\x0f\n\x07Quality\x18\x10 \x01(\t\x12\x12\n\nPlayConfig\x18\x11 \x01(\t\"g\n\x1fVodGetPrivateDrmPlayAuthRequest\x12\x0f\n\x07\x44rmType\x18\x01 \x01(\t\x12\x0b\n\x03Vid\x18\x02 \x01(\t\x12\x13\n\x0bPlayAuthIds\x18\x03 \x01(\t\x12\x11\n\tUnionInfo\x18\x04 \x01(\t\"Q\n\x1dVodGetHlsDecryptionKeyRequest\x12\x14\n\x0c\x44rmAuthToken\x18\x01 \x01(\t\x12\n\n\x02\x41k\x18\x02 \x01(\t\x12\x0e\n\x06Source\x18\x03 \x01(\t\"\x98\x01\n+VodGetPlayInfoWithLiveTimeShiftSceneRequest\x12\x11\n\tStoreUris\x18\x01 \x01(\t\x12\x11\n\tSpaceName\x18\x02 \x01(\t\x12\x0b\n\x03Ssl\x18\x03 \x01(\t\x12\x17\n\x0f\x45xpireTimestamp\x18\x04 \x01(\t\x12\x1d\n\x15NeedComposeBucketName\x18\x05 \x01(\t\"m\n\x13VodUrlUploadRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x43\n\x07URLSets\x18\x02 \x03(\x0b\x32\x32.Volcengine.Vod.Models.Business.VodUrlUploadURLSet\"/\n\x1dVodQueryUploadTaskInfoRequest\x12\x0e\n\x06JobIds\x18\x01 \x01(\t\"\xa5\x01\n\x19VodApplyUploadInfoRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nSessionKey\x18\x02 \x01(\t\x12\x10\n\x08\x46ileSize\x18\x03 \x01(\x01\x12\x10\n\x08\x46ileType\x18\x04 \x01(\t\x12\x10\n\x08\x46ileName\x18\x05 \x01(\t\x12\x14\n\x0cStorageClass\x18\x06 \x01(\x05\x12\x15\n\rFileExtension\x18\x07 \x01(\t\"\xbd\x01\n\x15VodUploadMediaRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x10\n\x08\x46ilePath\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\x12\x11\n\tFunctions\x18\x04 \x01(\t\x12\x10\n\x08\x46ileName\x18\x05 \x01(\t\x12\x14\n\x0cStorageClass\x18\x06 \x01(\x05\x12\x15\n\rFileExtension\x18\x07 \x01(\t\x12\x17\n\x0fVodUploadSource\x18\x08 \x01(\t\"\xa3\x01\n\x18VodUploadMaterialRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x10\n\x08\x46ilePath\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\x12\x11\n\tFunctions\x18\x04 \x01(\t\x12\x10\n\x08\x46ileType\x18\x05 \x01(\t\x12\x10\n\x08\x46ileName\x18\x06 \x01(\t\x12\x15\n\rFileExtension\x18\x07 \x01(\t\"\x85\x01\n\x1aVodCommitUploadInfoRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nSessionKey\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\x12\x11\n\tFunctions\x18\x04 \x01(\t\x12\x17\n\x0fVodUploadSource\x18\x05 \x01(\t\"=\n\x17VodUrlUploadJsonRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0f\n\x07URLSets\x18\x02 \x01(\t\".\n\x1eVodGetRecommendedPosterRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\"A\n\"VodUpdateMediaPublishStatusRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0e\n\x06Status\x18\x02 \x01(\t\"n\n!VodUpdateMediaStorageClassRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\x12\x14\n\x0cStorageClass\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\x12\x0f\n\x07\x46ileIds\x18\x04 \x01(\t\"\x9c\x02\n\x19VodUpdateMediaInfoRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12/\n\tPosterUri\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05Title\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x44\x65scription\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04Tags\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x35\n\x10\x43lassificationId\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\"\'\n\x17VodGetMediaInfosRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\";\n\x15VodDeleteMediaRequest\x12\x0c\n\x04Vids\x18\x01 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x02 \x01(\t\"P\n\x1aVodDeleteTranscodesRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0f\n\x07\x46ileIds\x18\x02 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x03 \x01(\t\"\xfb\x01\n\x16VodGetMediaListRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0b\n\x03Vid\x18\x02 \x01(\t\x12\x0e\n\x06Status\x18\x03 \x01(\t\x12\r\n\x05Order\x18\x04 \x01(\t\x12\x0c\n\x04Tags\x18\x05 \x01(\t\x12\x11\n\tStartTime\x18\x06 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x07 \x01(\t\x12\x0e\n\x06Offset\x18\x08 \x01(\t\x12\x10\n\x08PageSize\x18\t \x01(\t\x12\x19\n\x11\x43lassificationIds\x18\n \x01(\t\x12\x19\n\x11TosStorageClasses\x18\x0b \x01(\t\x12\x18\n\x10VodUploadSources\x18\x0c \x01(\t\"\xe6\x01\n\x1dVodGetSubtitleInfoListRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0f\n\x07\x46ileIds\x18\x02 \x01(\t\x12\x11\n\tLanguages\x18\x03 \x01(\t\x12\x0f\n\x07\x46ormats\x18\x04 \x01(\t\x12\x13\n\x0bLanguageIds\x18\x05 \x01(\t\x12\x13\n\x0bSubtitleIds\x18\x06 \x01(\t\x12\x0e\n\x06Status\x18\x07 \x01(\t\x12\r\n\x05Title\x18\x08 \x01(\t\x12\x0b\n\x03Tag\x18\t \x01(\t\x12\x0e\n\x06Offset\x18\n \x01(\t\x12\x10\n\x08PageSize\x18\x0b \x01(\t\x12\x0b\n\x03Ssl\x18\x0c \x01(\t\"r\n\x1eVodUpdateSubtitleStatusRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0f\n\x07\x46ileIds\x18\x02 \x01(\t\x12\x11\n\tLanguages\x18\x03 \x01(\t\x12\x0f\n\x07\x46ormats\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\"\xb5\x01\n\x1cVodUpdateSubtitleInfoRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x0e\n\x06\x46ileId\x18\x02 \x01(\t\x12\x10\n\x08Language\x18\x03 \x01(\t\x12\x0e\n\x06\x46ormat\x18\x04 \x01(\t\x12+\n\x05Title\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03Tag\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"w\n VodGetAuditFramesForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\x12\x19\n\x11MinNumberOfFrames\x18\x03 \x01(\t\x12\x19\n\x11MaxNumberOfFrames\x18\x04 \x01(\t\"\xa1\x02\n\x1dVodGetMLFramesForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\x12\x10\n\x08\x46rameOpt\x18\x03 \x01(\t\x12\x10\n\x08\x46rameFps\x18\x04 \x01(\t\x12\x16\n\x0eNumberOfFrames\x18\x05 \x01(\t\x12\x14\n\x0c\x43utTimeMills\x18\x06 \x01(\t\x12\x16\n\x0eNeedFirstFrame\x18\x07 \x01(\t\x12\x15\n\rNeedLastFrame\x18\x08 \x01(\t\x12\x15\n\rStartTimeMill\x18\t \x01(\t\x12\x13\n\x0b\x45ndTimeMill\x18\n \x01(\t\x12\x19\n\x11MinNumberOfFrames\x18\x0b \x01(\t\x12\x19\n\x11MaxNumberOfFrames\x18\x0c \x01(\t\"U\n!VodGetBetterFramesForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\x12\x11\n\tCoverRate\x18\x03 \x01(\t\"?\n\x1eVodGetAudioInfoForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\"P\n/VodGetAutomaticSpeechRecognitionForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\"I\n(VodGetAudioEventDetectionForAuditRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x10\n\x08Strategy\x18\x02 \x01(\t\"q\n#VodCreateVideoClassificationRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\r\n\x05Level\x18\x02 \x01(\x05\x12\x10\n\x08ParentId\x18\x03 \x01(\x03\x12\x16\n\x0e\x43lassification\x18\x04 \x01(\t\"j\n#VodUpdateVideoClassificationRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x18\n\x10\x43lassificationId\x18\x02 \x01(\x03\x12\x16\n\x0e\x43lassification\x18\x03 \x01(\t\"R\n#VodDeleteVideoClassificationRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x18\n\x10\x43lassificationId\x18\x02 \x01(\x03\"Q\n\"VodListVideoClassificationsRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x18\n\x10\x43lassificationId\x18\x02 \x01(\x03\"&\n\x17VodListSnapshotsRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\"Z\n\x15VodGetFileListRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0e\n\x06Prefix\x18\x02 \x01(\t\x12\r\n\x05Limit\x18\x03 \x01(\t\x12\x0f\n\x07Starter\x18\x04 \x01(\t\"-\n\x1eVodExtractMediaMetaTaskRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\"\x8e\x02\n\x17VodStartWorkflowRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x12\n\nTemplateId\x18\x02 \x01(\t\x12=\n\x05Input\x18\x03 \x01(\x0b\x32..Volcengine.Vod.Models.Business.WorkflowParams\x12\x10\n\x08Priority\x18\x04 \x01(\x05\x12\x14\n\x0c\x43\x61llbackArgs\x18\x05 \x01(\t\x12\x19\n\x11\x45nableLowPriority\x18\x06 \x01(\x08\x12<\n\tDirectUrl\x18\x07 \x01(\x0b\x32).Volcengine.Vod.Models.Business.DirectUrl\x12\x12\n\nTaskListId\x18\x08 \x01(\t\"D\n!VodRetrieveTranscodeResultRequest\x12\x0b\n\x03Vid\x18\x01 \x01(\t\x12\x12\n\nResultType\x18\x02 \x01(\t\"\x9f\x02\n\x1fVodListWorkflowExecutionRequest\x12\r\n\x05RunId\x18\x01 \x01(\t\x12\x0b\n\x03Vid\x18\x02 \x01(\t\x12\x11\n\tSpaceName\x18\x03 \x01(\t\x12\x12\n\nTemplateId\x18\x04 \x01(\t\x12\x12\n\nTaskListId\x18\x05 \x01(\t\x12\x19\n\x11\x45nableLowPriority\x18\x06 \x01(\t\x12\x11\n\tJobSource\x18\x07 \x01(\t\x12\x0e\n\x06Status\x18\x08 \x01(\t\x12\x11\n\tStartTime\x18\t \x01(\t\x12\x0f\n\x07\x45ndTime\x18\n \x01(\t\x12\x10\n\x08PageSize\x18\x0b \x01(\t\x12\x0e\n\x06Offset\x18\x0c \x01(\t\x12\x12\n\nOrderByKey\x18\r \x01(\t\x12\r\n\x05Order\x18\x0e \x01(\t\"5\n$VodGetWorkflowExecutionDetailRequest\x12\r\n\x05RunId\x18\x01 \x01(\t\",\n\x1bVodGetWorkflowResultRequest\x12\r\n\x05RunId\x18\x01 \x01(\t\"N\n$VodGetWorkflowExecutionStatusRequest\x12\r\n\x05RunId\x18\x01 \x01(\t\x12\x17\n\x0fNeedTasksDetail\x18\x02 \x01(\t\"\x9c\x01\n#VodSubmitDirectEditTaskAsyncRequest\x12\x10\n\x08Uploader\x18\x01 \x01(\t\x12\x13\n\x0b\x41pplication\x18\x02 \x01(\t\x12\x11\n\tEditParam\x18\x04 \x01(\x0c\x12\x10\n\x08Priority\x18\x05 \x01(\x05\x12\x13\n\x0b\x43\x61llbackUri\x18\x06 \x01(\t\x12\x14\n\x0c\x43\x61llbackArgs\x18\x07 \x01(\t\"/\n\x1dVodGetDirectEditResultRequest\x12\x0e\n\x06ReqIds\x18\x01 \x03(\t\"0\n\x1fVodGetDirectEditProgressRequest\x12\r\n\x05ReqId\x18\x01 \x01(\t\"v\n\x15VodCreateSpaceRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x13\n\x0bProjectName\x18\x02 \x01(\t\x12\x13\n\x0b\x44\x65scription\x18\x03 \x01(\t\x12\x0e\n\x06Region\x18\x04 \x01(\t\x12\x10\n\x08UserName\x18\x05 \x01(\t\"-\n\x18VodGetSpaceDetailRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\"4\n\x13VodListSpaceRequest\x12\x0e\n\x06Offset\x18\x01 \x01(\x01\x12\r\n\x05Limit\x18\x02 \x01(\x01\"u\n\x15VodUpdateSpaceRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x19\n\x11SourceProjectName\x18\x02 \x01(\t\x12\x19\n\x11TargetProjectName\x18\x03 \x01(\t\x12\x13\n\x0b\x44\x65scription\x18\x04 \x01(\t\"^\n!VodUpdateSpaceUploadConfigRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x11\n\tConfigKey\x18\x02 \x01(\t\x12\x13\n\x0b\x43onfigValue\x18\x03 \x01(\t\"\x81\x01\n%VodDescribeVodSpaceStorageDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x0c\n\x04Type\x18\x05 \x01(\t\"h\n\x14VodListDomainRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nDomainType\x18\x02 \x01(\t\x12\x19\n\x11SourceStationType\x18\x03 \x01(\x05\x12\x0e\n\x06Offset\x18\x04 \x01(\x03\"O\n\x1eVodCreateCdnRefreshTaskRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Urls\x18\x02 \x01(\t\x12\x0c\n\x04Type\x18\x03 \x01(\t\"A\n\x1eVodCreateCdnPreloadTaskRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Urls\x18\x02 \x01(\t\"\xc2\x01\n\x16VodListCdnTasksRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0e\n\x06TaskId\x18\x02 \x01(\t\x12\x12\n\nDomainName\x18\x03 \x01(\t\x12\x10\n\x08TaskType\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x06 \x01(\x05\x12\x14\n\x0c\x45ndTimestamp\x18\x07 \x01(\x05\x12\x0f\n\x07PageNum\x18\x08 \x01(\x05\x12\x10\n\x08PageSize\x18\t \x01(\x05\"n\n\x1aVodListCdnAccessLogRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x02 \x01(\x05\x12\x14\n\x0c\x45ndTimestamp\x18\x03 \x01(\x05\x12\x11\n\tSpaceName\x18\x04 \x01(\t\"p\n\x1dVodListCdnTopAccessUrlRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x02 \x01(\x05\x12\x14\n\x0c\x45ndTimestamp\x18\x03 \x01(\x05\x12\x10\n\x08SortType\x18\x04 \x01(\t\"\x9c\x01\n(VodDescribeVodDomainBandwidthDataRequest\x12\x12\n\nDomainList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x15\n\rBandwidthType\x18\x05 \x01(\t\x12\x0c\n\x04\x41rea\x18\x06 \x01(\t\"\xa3\x01\n\x1aVodListCdnUsageDataRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x10\n\x08Interval\x18\x02 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x03 \x01(\x03\x12\x14\n\x0c\x45ndTimestamp\x18\x04 \x01(\x03\x12\x10\n\x08\x44\x61taType\x18\x05 \x01(\t\x12\x0e\n\x06Metric\x18\x06 \x01(\t\x12\x12\n\nNeedDetail\x18\x07 \x01(\x08\"\xa4\x01\n\x1bVodListCdnStatusDataRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x10\n\x08Interval\x18\x02 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x03 \x01(\x03\x12\x14\n\x0c\x45ndTimestamp\x18\x04 \x01(\x03\x12\x10\n\x08\x44\x61taType\x18\x05 \x01(\t\x12\x0e\n\x06Metric\x18\x06 \x01(\t\x12\x12\n\nNeedDetail\x18\x07 \x01(\x08\"\'\n\x18VodDescribeIPInfoRequest\x12\x0b\n\x03Ips\x18\x01 \x01(\t\"\x90\x01\n\x17VodListCdnPvDataRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x10\n\x08Interval\x18\x02 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x03 \x01(\x03\x12\x14\n\x0c\x45ndTimestamp\x18\x04 \x01(\x03\x12\x10\n\x08\x44\x61taType\x18\x05 \x01(\t\x12\x12\n\nNeedDetail\x18\x06 \x01(\x08\"\x93\x01\n\x1cVodListCdnHitrateDataRequest\x12\x0f\n\x07\x44omains\x18\x01 \x01(\t\x12\x10\n\x08Interval\x18\x02 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x03 \x01(\x03\x12\x14\n\x0c\x45ndTimestamp\x18\x04 \x01(\x03\x12\x0e\n\x06Metric\x18\x05 \x01(\t\x12\x12\n\nNeedDetail\x18\x06 \x01(\x08\"\x8a\x01\n&VodDescribeVodDomainTrafficDataRequest\x12\x12\n\nDomainList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x13\n\x0bTrafficType\x18\x05 \x01(\t\"A\n\x1aVodSubmitBlockTasksRequest\x12\x10\n\x08\x46ileUrls\x18\x01 \x01(\t\x12\x11\n\tOperation\x18\x02 \x01(\t\"\xb6\x01\n\x1eVodGetContentBlockTasksRequest\x12\x0b\n\x03Url\x18\x01 \x01(\t\x12\x0e\n\x06\x44omain\x18\x02 \x01(\t\x12\x0e\n\x06TaskID\x18\x03 \x01(\t\x12\x10\n\x08TaskType\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\x12\x11\n\tStartTime\x18\x06 \x01(\x03\x12\x0f\n\x07\x45ndTime\x18\x07 \x01(\x03\x12\x0f\n\x07PageNum\x18\x08 \x01(\x03\x12\x10\n\x08PageSize\x18\t \x01(\x03\"\xc1\x01\n\x18VodCreateDomainV2Request\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nDomainType\x18\x02 \x01(\t\x12\x0e\n\x06\x44omain\x18\x03 \x01(\t\x12\x19\n\x11SourceStationType\x18\x05 \x01(\x05\x12 \n\x18SourceStationAddressType\x18\x06 \x01(\x05\x12\x0f\n\x07Origins\x18\x07 \x01(\t\x12\x0c\n\x04\x41rea\x18\x08 \x01(\t\x12\x12\n\nBucketName\x18\t \x01(\t\"g\n\x1eVodUpdateDomainExpireV2Request\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nDomainType\x18\x02 \x01(\t\x12\x0e\n\x06\x44omain\x18\x03 \x01(\t\x12\x0e\n\x06\x45xpire\x18\x04 \x01(\x05\"\x8f\x01\n\"VodUpdateDomainAuthConfigV2Request\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x12\n\nDomainType\x18\x02 \x01(\t\x12\x0e\n\x06\x44omain\x18\x03 \x01(\t\x12\x0f\n\x07MainKey\x18\x04 \x01(\t\x12\x11\n\tBackupKey\x18\x05 \x01(\t\x12\x0e\n\x06Status\x18\x06 \x01(\t\"X\n!VodAddCallbackSubscriptionRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0b\n\x03Url\x18\x02 \x01(\t\x12\x13\n\x0b\x43ontentType\x18\x03 \x01(\t\"h\n\x1aVodSetCallbackEventRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0e\n\x06\x45vents\x18\x02 \x01(\t\x12\x13\n\x0b\x41uthEnabled\x18\x03 \x01(\t\x12\x12\n\nPrivateKey\x18\x04 \x01(\t\"\xf4\x01\n&VodGetSmartStrategyLitePlayInfoRequest\x12\x0f\n\x07PlayUrl\x18\x01 \x01(\t\x12\x0e\n\x06\x46ormat\x18\x02 \x01(\t\x12\r\n\x05\x43odec\x18\x03 \x01(\t\x12\x12\n\nDefinition\x18\x04 \x01(\t\x12\x10\n\x08\x46ileType\x18\x05 \x01(\t\x12\x10\n\x08LogoType\x18\x06 \x01(\t\x12\x0b\n\x03Ssl\x18\x07 \x01(\t\x12\x12\n\nNeedThumbs\x18\x08 \x01(\t\x12\x17\n\x0fNeedBarrageMask\x18\t \x01(\t\x12\x11\n\tUnionInfo\x18\n \x01(\t\x12\x15\n\rHDRDefinition\x18\x0b \x01(\t\"%\n\x14VodGetAppInfoRequest\x12\r\n\x05\x41ppId\x18\x01 \x01(\x04\"\xd0\x01\n$DescribeVodSpaceTranscodeDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x15\n\rTranscodeType\x18\x04 \x01(\t\x12\x15\n\rSpecification\x18\x05 \x01(\t\x12\x15\n\rTaskStageList\x18\x06 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x07 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x08 \x01(\t\"\xb6\x01\n#DescribeVodSpaceAIStatisDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0bMediaAiType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x01(\t\"\xbd\x01\n)DescribeVodSpaceSubtitleStatisDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x14\n\x0cSubtitleType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x01(\t\"\xb9\x01\n\'DescribeVodSpaceDetectStatisDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x12\n\nDetectType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x01(\t\"\xb2\x01\n\x1e\x44\x65scribeVodSnapshotDataRequest\x12\x11\n\tSpaceList\x18\x01 \x01(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x14\n\x0cSnapshotType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x01(\t\"\x91\x01\n)DescribeVodSpaceWorkflowDetailDataRequest\x12\x0e\n\x06Region\x18\x01 \x01(\t\x12\r\n\x05Space\x18\x02 \x01(\t\x12\x11\n\tStartTime\x18\x03 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x04 \x01(\t\x12\x10\n\x08PageSize\x18\x05 \x01(\x03\x12\x0f\n\x07PageNum\x18\x06 \x01(\x03\"\x8d\x01\n%DescribeVodSpaceEditDetailDataRequest\x12\x0e\n\x06Region\x18\x01 \x01(\t\x12\r\n\x05Space\x18\x02 \x01(\t\x12\x11\n\tStartTime\x18\x03 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x04 \x01(\t\x12\x10\n\x08PageSize\x18\x05 \x01(\x03\x12\x0f\n\x07PageNum\x18\x06 \x01(\x03\"_\n%DescribeVodPlayFileLogByDomainRequest\x12\x11\n\tStartTime\x18\x01 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x02 \x01(\t\x12\x12\n\nDomainList\x18\x03 \x01(\t\"A\n\x1eVodSubmitBlockMediaTaskRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Vids\x18\x02 \x01(\t\"C\n VodSubmitUnblockMediaTaskRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Vids\x18\x02 \x01(\t\"B\n\x1fVodQueryMediaBlockStatusRequest\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12\x0c\n\x04Vids\x18\x02 \x01(\tB\xc8\x01\n(com.volcengine.service.vod.model.requestB\nVodRequestP\x01Z@github.com/volcengine/volc-sdk-golang/service/vod/models/request\xa0\x01\x01\xd8\x01\x01\xca\x02\x1fVolc\\Service\\Vod\\Models\\Request\xe2\x02#Volc\\Service\\Vod\\Models\\GPBMetadatab\x06proto3')
 
 
 
 _VODGETALLPLAYINFOREQUEST = DESCRIPTOR.message_types_by_name['VodGetAllPlayInfoRequest']
 _VODGETPLAYINFOREQUEST = DESCRIPTOR.message_types_by_name['VodGetPlayInfoRequest']
 _VODGETPRIVATEDRMPLAYAUTHREQUEST = DESCRIPTOR.message_types_by_name['VodGetPrivateDrmPlayAuthRequest']
 _VODGETHLSDECRYPTIONKEYREQUEST = DESCRIPTOR.message_types_by_name['VodGetHlsDecryptionKeyRequest']
@@ -97,14 +97,15 @@
 _DESCRIBEVODSPACETRANSCODEDATAREQUEST = DESCRIPTOR.message_types_by_name['DescribeVodSpaceTranscodeDataRequest']
 _DESCRIBEVODSPACEAISTATISDATAREQUEST = DESCRIPTOR.message_types_by_name['DescribeVodSpaceAIStatisDataRequest']
 _DESCRIBEVODSPACESUBTITLESTATISDATAREQUEST = DESCRIPTOR.message_types_by_name['DescribeVodSpaceSubtitleStatisDataRequest']
 _DESCRIBEVODSPACEDETECTSTATISDATAREQUEST = DESCRIPTOR.message_types_by_name['DescribeVodSpaceDetectStatisDataRequest']
 _DESCRIBEVODSNAPSHOTDATAREQUEST = DESCRIPTOR.message_types_by_name['DescribeVodSnapshotDataRequest']
 _DESCRIBEVODSPACEWORKFLOWDETAILDATAREQUEST = DESCRIPTOR.message_types_by_name['DescribeVodSpaceWorkflowDetailDataRequest']
 _DESCRIBEVODSPACEEDITDETAILDATAREQUEST = DESCRIPTOR.message_types_by_name['DescribeVodSpaceEditDetailDataRequest']
+_DESCRIBEVODPLAYFILELOGBYDOMAINREQUEST = DESCRIPTOR.message_types_by_name['DescribeVodPlayFileLogByDomainRequest']
 _VODSUBMITBLOCKMEDIATASKREQUEST = DESCRIPTOR.message_types_by_name['VodSubmitBlockMediaTaskRequest']
 _VODSUBMITUNBLOCKMEDIATASKREQUEST = DESCRIPTOR.message_types_by_name['VodSubmitUnblockMediaTaskRequest']
 _VODQUERYMEDIABLOCKSTATUSREQUEST = DESCRIPTOR.message_types_by_name['VodQueryMediaBlockStatusRequest']
 VodGetAllPlayInfoRequest = _reflection.GeneratedProtocolMessageType('VodGetAllPlayInfoRequest', (_message.Message,), {
   'DESCRIPTOR' : _VODGETALLPLAYINFOREQUEST,
   '__module__' : 'vod.request.request_vod_pb2'
   # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Request.VodGetAllPlayInfoRequest)
@@ -660,14 +661,21 @@
 DescribeVodSpaceEditDetailDataRequest = _reflection.GeneratedProtocolMessageType('DescribeVodSpaceEditDetailDataRequest', (_message.Message,), {
   'DESCRIPTOR' : _DESCRIBEVODSPACEEDITDETAILDATAREQUEST,
   '__module__' : 'vod.request.request_vod_pb2'
   # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Request.DescribeVodSpaceEditDetailDataRequest)
   })
 _sym_db.RegisterMessage(DescribeVodSpaceEditDetailDataRequest)
 
+DescribeVodPlayFileLogByDomainRequest = _reflection.GeneratedProtocolMessageType('DescribeVodPlayFileLogByDomainRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DESCRIBEVODPLAYFILELOGBYDOMAINREQUEST,
+  '__module__' : 'vod.request.request_vod_pb2'
+  # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Request.DescribeVodPlayFileLogByDomainRequest)
+  })
+_sym_db.RegisterMessage(DescribeVodPlayFileLogByDomainRequest)
+
 VodSubmitBlockMediaTaskRequest = _reflection.GeneratedProtocolMessageType('VodSubmitBlockMediaTaskRequest', (_message.Message,), {
   'DESCRIPTOR' : _VODSUBMITBLOCKMEDIATASKREQUEST,
   '__module__' : 'vod.request.request_vod_pb2'
   # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Request.VodSubmitBlockMediaTaskRequest)
   })
 _sym_db.RegisterMessage(VodSubmitBlockMediaTaskRequest)
 
@@ -788,71 +796,73 @@
   _VODUPDATESPACEREQUEST._serialized_start=6191
   _VODUPDATESPACEREQUEST._serialized_end=6308
   _VODUPDATESPACEUPLOADCONFIGREQUEST._serialized_start=6310
   _VODUPDATESPACEUPLOADCONFIGREQUEST._serialized_end=6404
   _VODDESCRIBEVODSPACESTORAGEDATAREQUEST._serialized_start=6407
   _VODDESCRIBEVODSPACESTORAGEDATAREQUEST._serialized_end=6536
   _VODLISTDOMAINREQUEST._serialized_start=6538
-  _VODLISTDOMAINREQUEST._serialized_end=6579
-  _VODCREATECDNREFRESHTASKREQUEST._serialized_start=6581
-  _VODCREATECDNREFRESHTASKREQUEST._serialized_end=6660
-  _VODCREATECDNPRELOADTASKREQUEST._serialized_start=6662
-  _VODCREATECDNPRELOADTASKREQUEST._serialized_end=6727
-  _VODLISTCDNTASKSREQUEST._serialized_start=6730
-  _VODLISTCDNTASKSREQUEST._serialized_end=6924
-  _VODLISTCDNACCESSLOGREQUEST._serialized_start=6926
-  _VODLISTCDNACCESSLOGREQUEST._serialized_end=7036
-  _VODLISTCDNTOPACCESSURLREQUEST._serialized_start=7038
-  _VODLISTCDNTOPACCESSURLREQUEST._serialized_end=7150
-  _VODDESCRIBEVODDOMAINBANDWIDTHDATAREQUEST._serialized_start=7153
-  _VODDESCRIBEVODDOMAINBANDWIDTHDATAREQUEST._serialized_end=7309
-  _VODLISTCDNUSAGEDATAREQUEST._serialized_start=7312
-  _VODLISTCDNUSAGEDATAREQUEST._serialized_end=7475
-  _VODLISTCDNSTATUSDATAREQUEST._serialized_start=7478
-  _VODLISTCDNSTATUSDATAREQUEST._serialized_end=7642
-  _VODDESCRIBEIPINFOREQUEST._serialized_start=7644
-  _VODDESCRIBEIPINFOREQUEST._serialized_end=7683
-  _VODLISTCDNPVDATAREQUEST._serialized_start=7686
-  _VODLISTCDNPVDATAREQUEST._serialized_end=7830
-  _VODLISTCDNHITRATEDATAREQUEST._serialized_start=7833
-  _VODLISTCDNHITRATEDATAREQUEST._serialized_end=7980
-  _VODDESCRIBEVODDOMAINTRAFFICDATAREQUEST._serialized_start=7983
-  _VODDESCRIBEVODDOMAINTRAFFICDATAREQUEST._serialized_end=8121
-  _VODSUBMITBLOCKTASKSREQUEST._serialized_start=8123
-  _VODSUBMITBLOCKTASKSREQUEST._serialized_end=8188
-  _VODGETCONTENTBLOCKTASKSREQUEST._serialized_start=8191
-  _VODGETCONTENTBLOCKTASKSREQUEST._serialized_end=8373
-  _VODCREATEDOMAINV2REQUEST._serialized_start=8376
-  _VODCREATEDOMAINV2REQUEST._serialized_end=8569
-  _VODUPDATEDOMAINEXPIREV2REQUEST._serialized_start=8571
-  _VODUPDATEDOMAINEXPIREV2REQUEST._serialized_end=8674
-  _VODUPDATEDOMAINAUTHCONFIGV2REQUEST._serialized_start=8677
-  _VODUPDATEDOMAINAUTHCONFIGV2REQUEST._serialized_end=8820
-  _VODADDCALLBACKSUBSCRIPTIONREQUEST._serialized_start=8822
-  _VODADDCALLBACKSUBSCRIPTIONREQUEST._serialized_end=8910
-  _VODSETCALLBACKEVENTREQUEST._serialized_start=8912
-  _VODSETCALLBACKEVENTREQUEST._serialized_end=9016
-  _VODGETSMARTSTRATEGYLITEPLAYINFOREQUEST._serialized_start=9019
-  _VODGETSMARTSTRATEGYLITEPLAYINFOREQUEST._serialized_end=9263
-  _VODGETAPPINFOREQUEST._serialized_start=9265
-  _VODGETAPPINFOREQUEST._serialized_end=9302
-  _DESCRIBEVODSPACETRANSCODEDATAREQUEST._serialized_start=9305
-  _DESCRIBEVODSPACETRANSCODEDATAREQUEST._serialized_end=9513
-  _DESCRIBEVODSPACEAISTATISDATAREQUEST._serialized_start=9516
-  _DESCRIBEVODSPACEAISTATISDATAREQUEST._serialized_end=9698
-  _DESCRIBEVODSPACESUBTITLESTATISDATAREQUEST._serialized_start=9701
-  _DESCRIBEVODSPACESUBTITLESTATISDATAREQUEST._serialized_end=9890
-  _DESCRIBEVODSPACEDETECTSTATISDATAREQUEST._serialized_start=9893
-  _DESCRIBEVODSPACEDETECTSTATISDATAREQUEST._serialized_end=10078
-  _DESCRIBEVODSNAPSHOTDATAREQUEST._serialized_start=10081
-  _DESCRIBEVODSNAPSHOTDATAREQUEST._serialized_end=10259
-  _DESCRIBEVODSPACEWORKFLOWDETAILDATAREQUEST._serialized_start=10262
-  _DESCRIBEVODSPACEWORKFLOWDETAILDATAREQUEST._serialized_end=10407
-  _DESCRIBEVODSPACEEDITDETAILDATAREQUEST._serialized_start=10410
-  _DESCRIBEVODSPACEEDITDETAILDATAREQUEST._serialized_end=10551
-  _VODSUBMITBLOCKMEDIATASKREQUEST._serialized_start=10553
-  _VODSUBMITBLOCKMEDIATASKREQUEST._serialized_end=10618
-  _VODSUBMITUNBLOCKMEDIATASKREQUEST._serialized_start=10620
-  _VODSUBMITUNBLOCKMEDIATASKREQUEST._serialized_end=10687
-  _VODQUERYMEDIABLOCKSTATUSREQUEST._serialized_start=10689
-  _VODQUERYMEDIABLOCKSTATUSREQUEST._serialized_end=10755
+  _VODLISTDOMAINREQUEST._serialized_end=6642
+  _VODCREATECDNREFRESHTASKREQUEST._serialized_start=6644
+  _VODCREATECDNREFRESHTASKREQUEST._serialized_end=6723
+  _VODCREATECDNPRELOADTASKREQUEST._serialized_start=6725
+  _VODCREATECDNPRELOADTASKREQUEST._serialized_end=6790
+  _VODLISTCDNTASKSREQUEST._serialized_start=6793
+  _VODLISTCDNTASKSREQUEST._serialized_end=6987
+  _VODLISTCDNACCESSLOGREQUEST._serialized_start=6989
+  _VODLISTCDNACCESSLOGREQUEST._serialized_end=7099
+  _VODLISTCDNTOPACCESSURLREQUEST._serialized_start=7101
+  _VODLISTCDNTOPACCESSURLREQUEST._serialized_end=7213
+  _VODDESCRIBEVODDOMAINBANDWIDTHDATAREQUEST._serialized_start=7216
+  _VODDESCRIBEVODDOMAINBANDWIDTHDATAREQUEST._serialized_end=7372
+  _VODLISTCDNUSAGEDATAREQUEST._serialized_start=7375
+  _VODLISTCDNUSAGEDATAREQUEST._serialized_end=7538
+  _VODLISTCDNSTATUSDATAREQUEST._serialized_start=7541
+  _VODLISTCDNSTATUSDATAREQUEST._serialized_end=7705
+  _VODDESCRIBEIPINFOREQUEST._serialized_start=7707
+  _VODDESCRIBEIPINFOREQUEST._serialized_end=7746
+  _VODLISTCDNPVDATAREQUEST._serialized_start=7749
+  _VODLISTCDNPVDATAREQUEST._serialized_end=7893
+  _VODLISTCDNHITRATEDATAREQUEST._serialized_start=7896
+  _VODLISTCDNHITRATEDATAREQUEST._serialized_end=8043
+  _VODDESCRIBEVODDOMAINTRAFFICDATAREQUEST._serialized_start=8046
+  _VODDESCRIBEVODDOMAINTRAFFICDATAREQUEST._serialized_end=8184
+  _VODSUBMITBLOCKTASKSREQUEST._serialized_start=8186
+  _VODSUBMITBLOCKTASKSREQUEST._serialized_end=8251
+  _VODGETCONTENTBLOCKTASKSREQUEST._serialized_start=8254
+  _VODGETCONTENTBLOCKTASKSREQUEST._serialized_end=8436
+  _VODCREATEDOMAINV2REQUEST._serialized_start=8439
+  _VODCREATEDOMAINV2REQUEST._serialized_end=8632
+  _VODUPDATEDOMAINEXPIREV2REQUEST._serialized_start=8634
+  _VODUPDATEDOMAINEXPIREV2REQUEST._serialized_end=8737
+  _VODUPDATEDOMAINAUTHCONFIGV2REQUEST._serialized_start=8740
+  _VODUPDATEDOMAINAUTHCONFIGV2REQUEST._serialized_end=8883
+  _VODADDCALLBACKSUBSCRIPTIONREQUEST._serialized_start=8885
+  _VODADDCALLBACKSUBSCRIPTIONREQUEST._serialized_end=8973
+  _VODSETCALLBACKEVENTREQUEST._serialized_start=8975
+  _VODSETCALLBACKEVENTREQUEST._serialized_end=9079
+  _VODGETSMARTSTRATEGYLITEPLAYINFOREQUEST._serialized_start=9082
+  _VODGETSMARTSTRATEGYLITEPLAYINFOREQUEST._serialized_end=9326
+  _VODGETAPPINFOREQUEST._serialized_start=9328
+  _VODGETAPPINFOREQUEST._serialized_end=9365
+  _DESCRIBEVODSPACETRANSCODEDATAREQUEST._serialized_start=9368
+  _DESCRIBEVODSPACETRANSCODEDATAREQUEST._serialized_end=9576
+  _DESCRIBEVODSPACEAISTATISDATAREQUEST._serialized_start=9579
+  _DESCRIBEVODSPACEAISTATISDATAREQUEST._serialized_end=9761
+  _DESCRIBEVODSPACESUBTITLESTATISDATAREQUEST._serialized_start=9764
+  _DESCRIBEVODSPACESUBTITLESTATISDATAREQUEST._serialized_end=9953
+  _DESCRIBEVODSPACEDETECTSTATISDATAREQUEST._serialized_start=9956
+  _DESCRIBEVODSPACEDETECTSTATISDATAREQUEST._serialized_end=10141
+  _DESCRIBEVODSNAPSHOTDATAREQUEST._serialized_start=10144
+  _DESCRIBEVODSNAPSHOTDATAREQUEST._serialized_end=10322
+  _DESCRIBEVODSPACEWORKFLOWDETAILDATAREQUEST._serialized_start=10325
+  _DESCRIBEVODSPACEWORKFLOWDETAILDATAREQUEST._serialized_end=10470
+  _DESCRIBEVODSPACEEDITDETAILDATAREQUEST._serialized_start=10473
+  _DESCRIBEVODSPACEEDITDETAILDATAREQUEST._serialized_end=10614
+  _DESCRIBEVODPLAYFILELOGBYDOMAINREQUEST._serialized_start=10616
+  _DESCRIBEVODPLAYFILELOGBYDOMAINREQUEST._serialized_end=10711
+  _VODSUBMITBLOCKMEDIATASKREQUEST._serialized_start=10713
+  _VODSUBMITBLOCKMEDIATASKREQUEST._serialized_end=10778
+  _VODSUBMITUNBLOCKMEDIATASKREQUEST._serialized_start=10780
+  _VODSUBMITUNBLOCKMEDIATASKREQUEST._serialized_end=10847
+  _VODQUERYMEDIABLOCKSTATUSREQUEST._serialized_start=10849
+  _VODQUERYMEDIABLOCKSTATUSREQUEST._serialized_end=10915
 # @@protoc_insertion_point(module_scope)
```

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_common_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_common_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_measure_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_measure_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1evod/business/vod_measure.proto\x12\x1eVolcengine.Vod.Models.Business\"<\n\x1d\x44\x65scribeVodSpaceTranscodeItem\x12\x0c\n\x04Name\x18\x01 \x01(\t\x12\r\n\x05Value\x18\x02 \x01(\x03\"\x8f\x01\n%DescribeVodSpaceTranscodeDetailTVUnit\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12X\n\x11TranscodeItemList\x18\x02 \x03(\x0b\x32=.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeItem\"\xb5\x01\n\x1f\x44\x65scribeVodSpaceTranscodeDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12\r\n\x05Total\x18\x03 \x01(\x03\x12\x61\n\x12TranscodeUsageList\x18\x04 \x03(\x0b\x32\x45.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeDetailTVUnit\"\xac\x03\n#DescribeVodSpaceTranscodeDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x15\n\rTranscodeType\x18\x04 \x01(\t\x12\x15\n\rSpecification\x18\x05 \x01(\t\x12\x15\n\rTaskStageList\x18\x06 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x07 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x08 \x03(\t\x12\x1a\n\x12TotalTranscodeData\x18\t \x01(\x03\x12]\n\x16TotalTranscodeDataList\x18\n \x03(\x0b\x32=.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeItem\x12`\n\x17TranscodeDataDetailList\x18\x0b \x03(\x0b\x32?.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeDetail\"B\n DescribeVodSpaceAIStatisDataItem\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\x10\n\x08\x44uration\x18\x02 \x01(\x03\"\xa1\x01\n\"DescribeVodSpaceAIStatisDataDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12Y\n\x0f\x41iUsageDataList\x18\x03 \x03(\x0b\x32@.Volcengine.Vod.Models.Business.DescribeVodSpaceAIStatisDataItem\"\x8d\x03\n\"DescribeVodSpaceAIStatisDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0bMediaAiType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x03(\t\x12\x18\n\x10TotalAiUsageData\x18\x08 \x01(\x03\x12Y\n\x0f\x41iUsageDataList\x18\t \x03(\x0b\x32@.Volcengine.Vod.Models.Business.DescribeVodSpaceAIStatisDataItem\x12\x61\n\x15\x41iUsageDataDetailList\x18\n \x03(\x0b\x32\x42.Volcengine.Vod.Models.Business.DescribeVodSpaceAIStatisDataDetail\"E\n&DescribeVodSpaceSubtitleStatisDataItem\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\r\n\x05Usage\x18\x02 \x01(\x03\"\xb3\x01\n(DescribeVodSpaceSubtitleStatisDataDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12\x65\n\x15SubtitleUsageDataList\x18\x03 \x03(\x0b\x32\x46.Volcengine.Vod.Models.Business.DescribeVodSpaceSubtitleStatisDataItem\"\xb2\x03\n(DescribeVodSpaceSubtitleStatisDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x14\n\x0cSubtitleType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x03(\t\x12\x1e\n\x16TotalSubtitleUsageData\x18\x08 \x01(\x03\x12\x65\n\x15SubtitleUsageDataList\x18\t \x03(\x0b\x32\x46.Volcengine.Vod.Models.Business.DescribeVodSpaceSubtitleStatisDataItem\x12m\n\x1bSubtitleUsageDataDetailList\x18\n \x03(\x0b\x32H.Volcengine.Vod.Models.Business.DescribeVodSpaceSubtitleStatisDataDetail\"C\n$DescribeVodSpaceDetectStatisDataItem\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\r\n\x05Usage\x18\x02 \x01(\x03\"\xad\x01\n&DescribeVodSpaceDetectStatisDataDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12\x61\n\x13\x44\x65tectUsageDataList\x18\x03 \x03(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodSpaceDetectStatisDataItem\"\xa4\x03\n&DescribeVodSpaceDetectStatisDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x12\n\nDetectType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x03(\t\x12\x1c\n\x14TotalDetectUsageData\x18\x08 \x01(\x03\x12\x61\n\x13\x44\x65tectUsageDataList\x18\t \x03(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodSpaceDetectStatisDataItem\x12i\n\x19\x44\x65tectUsageDataDetailList\x18\n \x03(\x0b\x32\x46.Volcengine.Vod.Models.Business.DescribeVodSpaceDetectStatisDataDetail\":\n\x1b\x44\x65scribeVodSnapshotDataItem\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\r\n\x05\x43ount\x18\x02 \x01(\x03\"\xa7\x01\n\x1d\x44\x65scribeVodSnapshotDataDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12\r\n\x05Total\x18\x03 \x01(\t\x12U\n\x10SnapshotDataList\x18\x04 \x03(\x0b\x32;.Volcengine.Vod.Models.Business.DescribeVodSnapshotDataItem\"\x82\x03\n\x1d\x44\x65scribeVodSnapshotDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x14\n\x0cSnapshotType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x03(\t\x12\x19\n\x11TotalSnapshotData\x18\x08 \x01(\x03\x12U\n\x10SnapshotDataList\x18\t \x03(\x0b\x32;.Volcengine.Vod.Models.Business.DescribeVodSnapshotDataItem\x12]\n\x16SnapshotDetailDataList\x18\n \x03(\x0b\x32=.Volcengine.Vod.Models.Business.DescribeVodSnapshotDataDetail\"\xd8\x01\n%DescribeVodSpaceWorkflowTranscodeInfo\x12\x14\n\x0cTemplateType\x18\x01 \x01(\t\x12\x10\n\x08\x46ileType\x18\x02 \x01(\t\x12\x10\n\x08\x44uration\x18\x03 \x01(\x03\x12\r\n\x05\x43odec\x18\x04 \x01(\t\x12\r\n\x05Remux\x18\x05 \x01(\x08\x12\x12\n\nDefinition\x18\x06 \x01(\t\x12\r\n\x05Width\x18\x07 \x01(\x03\x12\x0e\n\x06Height\x18\x08 \x01(\x03\x12\r\n\x05Slice\x18\t \x01(\x08\x12\x15\n\rIsLowPriority\x18\n \x01(\x08\"c\n$DescribeVodSpaceWorkflowSnapshotInfo\x12\x14\n\x0cTemplateType\x18\x01 \x01(\t\x12\x0e\n\x06Number\x18\x02 \x01(\x03\x12\x15\n\rIsLowPriority\x18\x03 \x01(\x08\"h\n\'DescribeVodSpaceWorkflowEnhanceExecInfo\x12\x14\n\x0cTemplateType\x18\x01 \x01(\t\x12\x10\n\x08\x44uration\x18\x02 \x01(\x03\x12\x15\n\rIsLowPriority\x18\x03 \x01(\x08\"t\n#DescribeVodSpaceWorkflowVideoAIInfo\x12\x14\n\x0cTemplateType\x18\x01 \x01(\t\x12\x10\n\x08\x44uration\x18\x02 \x01(\x03\x12\x0e\n\x06Number\x18\x03 \x01(\x03\x12\x15\n\rIsLowPriority\x18\x04 \x01(\x08\"\x8d\x04\n\x1e\x44\x65scribeVodSpaceWorkflowDetail\x12\r\n\x05RunId\x18\x01 \x01(\t\x12\x0b\n\x03Vid\x18\x02 \x01(\t\x12\x12\n\nTemplateId\x18\x03 \x01(\t\x12\x11\n\tSpaceName\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\x12\x11\n\tStartTime\x18\x06 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x07 \x01(\t\x12\\\n\rTranscodeInfo\x18\x08 \x01(\x0b\x32\x45.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowTranscodeInfo\x12Z\n\x0cSnapshotInfo\x18\t \x01(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowSnapshotInfo\x12`\n\x0f\x45nhanceExecInfo\x18\n \x01(\x0b\x32G.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowEnhanceExecInfo\x12X\n\x0bVideoAIInfo\x18\x0b \x01(\x0b\x32\x43.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowVideoAIInfo\"\xfb\x01\n(DescribeVodSpaceWorkflowDetailDataResult\x12\x0e\n\x06Region\x18\x01 \x01(\t\x12\r\n\x05Space\x18\x02 \x01(\t\x12\x11\n\tStartTime\x18\x03 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x04 \x01(\t\x12\x10\n\x08PageSize\x18\x05 \x01(\x03\x12\x0f\n\x07PageNum\x18\x06 \x01(\x03\x12\r\n\x05Total\x18\x07 \x01(\x03\x12Z\n\x12WorkflowDetailData\x18\x08 \x03(\x0b\x32>.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowDetail\"\x81\x01\n\x1a\x44\x65scribeVodSpaceEditDetail\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\x11\n\tOutputVid\x18\x02 \x01(\t\x12\r\n\x05Space\x18\x03 \x01(\t\x12\r\n\x05\x43odec\x18\x04 \x01(\t\x12\x12\n\nDefinition\x18\x05 \x01(\t\x12\x10\n\x08\x44uration\x18\x06 \x01(\x03\"\xef\x01\n$DescribeVodSpaceEditDetailDataResult\x12\x0e\n\x06Region\x18\x01 \x01(\t\x12\r\n\x05Space\x18\x02 \x01(\t\x12\x11\n\tStartTime\x18\x03 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x04 \x01(\t\x12\x10\n\x08PageSize\x18\x05 \x01(\x03\x12\x0f\n\x07PageNum\x18\x06 \x01(\x03\x12\r\n\x05Total\x18\x07 \x01(\x03\x12R\n\x0e\x45\x64itDetailData\x18\x08 \x03(\x0b\x32:.Volcengine.Vod.Models.Business.DescribeVodSpaceEditDetailB\xcb\x01\n)com.volcengine.service.vod.model.businessB\nVodMeasureP\x01ZAgithub.com/volcengine/volc-sdk-golang/service/vod/models/business\xa0\x01\x01\xd8\x01\x01\xca\x02 Volc\\Service\\Vod\\Models\\Business\xe2\x02#Volc\\Service\\Vod\\Models\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1evod/business/vod_measure.proto\x12\x1eVolcengine.Vod.Models.Business\"<\n\x1d\x44\x65scribeVodSpaceTranscodeItem\x12\x0c\n\x04Name\x18\x01 \x01(\t\x12\r\n\x05Value\x18\x02 \x01(\x03\"\x8f\x01\n%DescribeVodSpaceTranscodeDetailTVUnit\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12X\n\x11TranscodeItemList\x18\x02 \x03(\x0b\x32=.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeItem\"\xb5\x01\n\x1f\x44\x65scribeVodSpaceTranscodeDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12\r\n\x05Total\x18\x03 \x01(\x03\x12\x61\n\x12TranscodeUsageList\x18\x04 \x03(\x0b\x32\x45.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeDetailTVUnit\"\xac\x03\n#DescribeVodSpaceTranscodeDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x15\n\rTranscodeType\x18\x04 \x01(\t\x12\x15\n\rSpecification\x18\x05 \x01(\t\x12\x15\n\rTaskStageList\x18\x06 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x07 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x08 \x03(\t\x12\x1a\n\x12TotalTranscodeData\x18\t \x01(\x03\x12]\n\x16TotalTranscodeDataList\x18\n \x03(\x0b\x32=.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeItem\x12`\n\x17TranscodeDataDetailList\x18\x0b \x03(\x0b\x32?.Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeDetail\"B\n DescribeVodSpaceAIStatisDataItem\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\x10\n\x08\x44uration\x18\x02 \x01(\x03\"\xa1\x01\n\"DescribeVodSpaceAIStatisDataDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12Y\n\x0f\x41iUsageDataList\x18\x03 \x03(\x0b\x32@.Volcengine.Vod.Models.Business.DescribeVodSpaceAIStatisDataItem\"\x8d\x03\n\"DescribeVodSpaceAIStatisDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0bMediaAiType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x03(\t\x12\x18\n\x10TotalAiUsageData\x18\x08 \x01(\x03\x12Y\n\x0f\x41iUsageDataList\x18\t \x03(\x0b\x32@.Volcengine.Vod.Models.Business.DescribeVodSpaceAIStatisDataItem\x12\x61\n\x15\x41iUsageDataDetailList\x18\n \x03(\x0b\x32\x42.Volcengine.Vod.Models.Business.DescribeVodSpaceAIStatisDataDetail\"E\n&DescribeVodSpaceSubtitleStatisDataItem\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\r\n\x05Usage\x18\x02 \x01(\x03\"\xb3\x01\n(DescribeVodSpaceSubtitleStatisDataDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12\x65\n\x15SubtitleUsageDataList\x18\x03 \x03(\x0b\x32\x46.Volcengine.Vod.Models.Business.DescribeVodSpaceSubtitleStatisDataItem\"\xb2\x03\n(DescribeVodSpaceSubtitleStatisDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x14\n\x0cSubtitleType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x03(\t\x12\x1e\n\x16TotalSubtitleUsageData\x18\x08 \x01(\x03\x12\x65\n\x15SubtitleUsageDataList\x18\t \x03(\x0b\x32\x46.Volcengine.Vod.Models.Business.DescribeVodSpaceSubtitleStatisDataItem\x12m\n\x1bSubtitleUsageDataDetailList\x18\n \x03(\x0b\x32H.Volcengine.Vod.Models.Business.DescribeVodSpaceSubtitleStatisDataDetail\"C\n$DescribeVodSpaceDetectStatisDataItem\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\r\n\x05Usage\x18\x02 \x01(\x03\"\xad\x01\n&DescribeVodSpaceDetectStatisDataDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12\x61\n\x13\x44\x65tectUsageDataList\x18\x03 \x03(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodSpaceDetectStatisDataItem\"\xa4\x03\n&DescribeVodSpaceDetectStatisDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x12\n\nDetectType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x03(\t\x12\x1c\n\x14TotalDetectUsageData\x18\x08 \x01(\x03\x12\x61\n\x13\x44\x65tectUsageDataList\x18\t \x03(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodSpaceDetectStatisDataItem\x12i\n\x19\x44\x65tectUsageDataDetailList\x18\n \x03(\x0b\x32\x46.Volcengine.Vod.Models.Business.DescribeVodSpaceDetectStatisDataDetail\":\n\x1b\x44\x65scribeVodSnapshotDataItem\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\r\n\x05\x43ount\x18\x02 \x01(\x03\"\xa7\x01\n\x1d\x44\x65scribeVodSnapshotDataDetail\x12\r\n\x05Space\x18\x01 \x01(\t\x12\x11\n\tTaskStage\x18\x02 \x01(\t\x12\r\n\x05Total\x18\x03 \x01(\t\x12U\n\x10SnapshotDataList\x18\x04 \x03(\x0b\x32;.Volcengine.Vod.Models.Business.DescribeVodSnapshotDataItem\"\x82\x03\n\x1d\x44\x65scribeVodSnapshotDataResult\x12\x11\n\tSpaceList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x14\n\x0cSnapshotType\x18\x04 \x01(\t\x12\x15\n\rTaskStageList\x18\x05 \x03(\t\x12\x13\n\x0b\x41ggregation\x18\x06 \x01(\x03\x12\x17\n\x0f\x44\x65tailFieldList\x18\x07 \x03(\t\x12\x19\n\x11TotalSnapshotData\x18\x08 \x01(\x03\x12U\n\x10SnapshotDataList\x18\t \x03(\x0b\x32;.Volcengine.Vod.Models.Business.DescribeVodSnapshotDataItem\x12]\n\x16SnapshotDetailDataList\x18\n \x03(\x0b\x32=.Volcengine.Vod.Models.Business.DescribeVodSnapshotDataDetail\"\xd8\x01\n%DescribeVodSpaceWorkflowTranscodeInfo\x12\x14\n\x0cTemplateType\x18\x01 \x01(\t\x12\x10\n\x08\x46ileType\x18\x02 \x01(\t\x12\x10\n\x08\x44uration\x18\x03 \x01(\x03\x12\r\n\x05\x43odec\x18\x04 \x01(\t\x12\r\n\x05Remux\x18\x05 \x01(\x08\x12\x12\n\nDefinition\x18\x06 \x01(\t\x12\r\n\x05Width\x18\x07 \x01(\x03\x12\x0e\n\x06Height\x18\x08 \x01(\x03\x12\r\n\x05Slice\x18\t \x01(\x08\x12\x15\n\rIsLowPriority\x18\n \x01(\x08\"c\n$DescribeVodSpaceWorkflowSnapshotInfo\x12\x14\n\x0cTemplateType\x18\x01 \x01(\t\x12\x0e\n\x06Number\x18\x02 \x01(\x03\x12\x15\n\rIsLowPriority\x18\x03 \x01(\x08\"h\n\'DescribeVodSpaceWorkflowEnhanceExecInfo\x12\x14\n\x0cTemplateType\x18\x01 \x01(\t\x12\x10\n\x08\x44uration\x18\x02 \x01(\x03\x12\x15\n\rIsLowPriority\x18\x03 \x01(\x08\"t\n#DescribeVodSpaceWorkflowVideoAIInfo\x12\x14\n\x0cTemplateType\x18\x01 \x01(\t\x12\x10\n\x08\x44uration\x18\x02 \x01(\x03\x12\x0e\n\x06Number\x18\x03 \x01(\x03\x12\x15\n\rIsLowPriority\x18\x04 \x01(\x08\"\x8d\x04\n\x1e\x44\x65scribeVodSpaceWorkflowDetail\x12\r\n\x05RunId\x18\x01 \x01(\t\x12\x0b\n\x03Vid\x18\x02 \x01(\t\x12\x12\n\nTemplateId\x18\x03 \x01(\t\x12\x11\n\tSpaceName\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\x12\x11\n\tStartTime\x18\x06 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x07 \x01(\t\x12\\\n\rTranscodeInfo\x18\x08 \x01(\x0b\x32\x45.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowTranscodeInfo\x12Z\n\x0cSnapshotInfo\x18\t \x01(\x0b\x32\x44.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowSnapshotInfo\x12`\n\x0f\x45nhanceExecInfo\x18\n \x01(\x0b\x32G.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowEnhanceExecInfo\x12X\n\x0bVideoAIInfo\x18\x0b \x01(\x0b\x32\x43.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowVideoAIInfo\"\xfb\x01\n(DescribeVodSpaceWorkflowDetailDataResult\x12\x0e\n\x06Region\x18\x01 \x01(\t\x12\r\n\x05Space\x18\x02 \x01(\t\x12\x11\n\tStartTime\x18\x03 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x04 \x01(\t\x12\x10\n\x08PageSize\x18\x05 \x01(\x03\x12\x0f\n\x07PageNum\x18\x06 \x01(\x03\x12\r\n\x05Total\x18\x07 \x01(\x03\x12Z\n\x12WorkflowDetailData\x18\x08 \x03(\x0b\x32>.Volcengine.Vod.Models.Business.DescribeVodSpaceWorkflowDetail\"\x81\x01\n\x1a\x44\x65scribeVodSpaceEditDetail\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\x11\n\tOutputVid\x18\x02 \x01(\t\x12\r\n\x05Space\x18\x03 \x01(\t\x12\r\n\x05\x43odec\x18\x04 \x01(\t\x12\x12\n\nDefinition\x18\x05 \x01(\t\x12\x10\n\x08\x44uration\x18\x06 \x01(\x03\"\xef\x01\n$DescribeVodSpaceEditDetailDataResult\x12\x0e\n\x06Region\x18\x01 \x01(\t\x12\r\n\x05Space\x18\x02 \x01(\t\x12\x11\n\tStartTime\x18\x03 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x04 \x01(\t\x12\x10\n\x08PageSize\x18\x05 \x01(\x03\x12\x0f\n\x07PageNum\x18\x06 \x01(\x03\x12\r\n\x05Total\x18\x07 \x01(\x03\x12R\n\x0e\x45\x64itDetailData\x18\x08 \x03(\x0b\x32:.Volcengine.Vod.Models.Business.DescribeVodSpaceEditDetail\"W\n\"DescribeVodPlayFileLogByDomainItem\x12\x0c\n\x04\x44\x61te\x18\x01 \x01(\t\x12\x0e\n\x06\x44omain\x18\x02 \x01(\t\x12\x13\n\x0b\x44ownloadUrl\x18\x03 \x01(\t\"\xb4\x01\n$DescribeVodPlayFileLogByDomainResult\x12\x11\n\tStartTime\x18\x01 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x02 \x01(\t\x12\x12\n\nDomainList\x18\x03 \x03(\t\x12T\n\x08\x46ileList\x18\x04 \x03(\x0b\x32\x42.Volcengine.Vod.Models.Business.DescribeVodPlayFileLogByDomainItemB\xcb\x01\n)com.volcengine.service.vod.model.businessB\nVodMeasureP\x01ZAgithub.com/volcengine/volc-sdk-golang/service/vod/models/business\xa0\x01\x01\xd8\x01\x01\xca\x02 Volc\\Service\\Vod\\Models\\Business\xe2\x02#Volc\\Service\\Vod\\Models\\GPBMetadatab\x06proto3')
 
 
 
 _DESCRIBEVODSPACETRANSCODEITEM = DESCRIPTOR.message_types_by_name['DescribeVodSpaceTranscodeItem']
 _DESCRIBEVODSPACETRANSCODEDETAILTVUNIT = DESCRIPTOR.message_types_by_name['DescribeVodSpaceTranscodeDetailTVUnit']
 _DESCRIBEVODSPACETRANSCODEDETAIL = DESCRIPTOR.message_types_by_name['DescribeVodSpaceTranscodeDetail']
 _DESCRIBEVODSPACETRANSCODEDATARESULT = DESCRIPTOR.message_types_by_name['DescribeVodSpaceTranscodeDataResult']
@@ -38,14 +38,16 @@
 _DESCRIBEVODSPACEWORKFLOWSNAPSHOTINFO = DESCRIPTOR.message_types_by_name['DescribeVodSpaceWorkflowSnapshotInfo']
 _DESCRIBEVODSPACEWORKFLOWENHANCEEXECINFO = DESCRIPTOR.message_types_by_name['DescribeVodSpaceWorkflowEnhanceExecInfo']
 _DESCRIBEVODSPACEWORKFLOWVIDEOAIINFO = DESCRIPTOR.message_types_by_name['DescribeVodSpaceWorkflowVideoAIInfo']
 _DESCRIBEVODSPACEWORKFLOWDETAIL = DESCRIPTOR.message_types_by_name['DescribeVodSpaceWorkflowDetail']
 _DESCRIBEVODSPACEWORKFLOWDETAILDATARESULT = DESCRIPTOR.message_types_by_name['DescribeVodSpaceWorkflowDetailDataResult']
 _DESCRIBEVODSPACEEDITDETAIL = DESCRIPTOR.message_types_by_name['DescribeVodSpaceEditDetail']
 _DESCRIBEVODSPACEEDITDETAILDATARESULT = DESCRIPTOR.message_types_by_name['DescribeVodSpaceEditDetailDataResult']
+_DESCRIBEVODPLAYFILELOGBYDOMAINITEM = DESCRIPTOR.message_types_by_name['DescribeVodPlayFileLogByDomainItem']
+_DESCRIBEVODPLAYFILELOGBYDOMAINRESULT = DESCRIPTOR.message_types_by_name['DescribeVodPlayFileLogByDomainResult']
 DescribeVodSpaceTranscodeItem = _reflection.GeneratedProtocolMessageType('DescribeVodSpaceTranscodeItem', (_message.Message,), {
   'DESCRIPTOR' : _DESCRIBEVODSPACETRANSCODEITEM,
   '__module__' : 'vod.business.vod_measure_pb2'
   # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Business.DescribeVodSpaceTranscodeItem)
   })
 _sym_db.RegisterMessage(DescribeVodSpaceTranscodeItem)
 
@@ -206,14 +208,28 @@
 DescribeVodSpaceEditDetailDataResult = _reflection.GeneratedProtocolMessageType('DescribeVodSpaceEditDetailDataResult', (_message.Message,), {
   'DESCRIPTOR' : _DESCRIBEVODSPACEEDITDETAILDATARESULT,
   '__module__' : 'vod.business.vod_measure_pb2'
   # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Business.DescribeVodSpaceEditDetailDataResult)
   })
 _sym_db.RegisterMessage(DescribeVodSpaceEditDetailDataResult)
 
+DescribeVodPlayFileLogByDomainItem = _reflection.GeneratedProtocolMessageType('DescribeVodPlayFileLogByDomainItem', (_message.Message,), {
+  'DESCRIPTOR' : _DESCRIBEVODPLAYFILELOGBYDOMAINITEM,
+  '__module__' : 'vod.business.vod_measure_pb2'
+  # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Business.DescribeVodPlayFileLogByDomainItem)
+  })
+_sym_db.RegisterMessage(DescribeVodPlayFileLogByDomainItem)
+
+DescribeVodPlayFileLogByDomainResult = _reflection.GeneratedProtocolMessageType('DescribeVodPlayFileLogByDomainResult', (_message.Message,), {
+  'DESCRIPTOR' : _DESCRIBEVODPLAYFILELOGBYDOMAINRESULT,
+  '__module__' : 'vod.business.vod_measure_pb2'
+  # @@protoc_insertion_point(class_scope:Volcengine.Vod.Models.Business.DescribeVodPlayFileLogByDomainResult)
+  })
+_sym_db.RegisterMessage(DescribeVodPlayFileLogByDomainResult)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n)com.volcengine.service.vod.model.businessB\nVodMeasureP\001ZAgithub.com/volcengine/volc-sdk-golang/service/vod/models/business\240\001\001\330\001\001\312\002 Volc\\Service\\Vod\\Models\\Business\342\002#Volc\\Service\\Vod\\Models\\GPBMetadata'
   _DESCRIBEVODSPACETRANSCODEITEM._serialized_start=66
   _DESCRIBEVODSPACETRANSCODEITEM._serialized_end=126
   _DESCRIBEVODSPACETRANSCODEDETAILTVUNIT._serialized_start=129
@@ -258,8 +274,12 @@
   _DESCRIBEVODSPACEWORKFLOWDETAIL._serialized_end=4568
   _DESCRIBEVODSPACEWORKFLOWDETAILDATARESULT._serialized_start=4571
   _DESCRIBEVODSPACEWORKFLOWDETAILDATARESULT._serialized_end=4822
   _DESCRIBEVODSPACEEDITDETAIL._serialized_start=4825
   _DESCRIBEVODSPACEEDITDETAIL._serialized_end=4954
   _DESCRIBEVODSPACEEDITDETAILDATARESULT._serialized_start=4957
   _DESCRIBEVODSPACEEDITDETAILDATARESULT._serialized_end=5196
+  _DESCRIBEVODPLAYFILELOGBYDOMAINITEM._serialized_start=5198
+  _DESCRIBEVODPLAYFILELOGBYDOMAINITEM._serialized_end=5285
+  _DESCRIBEVODPLAYFILELOGBYDOMAINRESULT._serialized_start=5288
+  _DESCRIBEVODPLAYFILELOGBYDOMAINRESULT._serialized_end=5468
 # @@protoc_insertion_point(module_scope)
```

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_upload_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_upload_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_edit_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_edit_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_cdn_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_cdn_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from volcengine.vod.models.business import vod_common_pb2 as vod_dot_business_dot_vod__common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1avod/business/vod_cdn.proto\x12\x1eVolcengine.Vod.Models.Business\x1a\x1dvod/business/vod_common.proto\"\xe8\x01\n\x13VodDomainConfigInfo\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12P\n\x10PlayInstanceInfo\x18\x02 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodDomainInstanceInfos\x12Q\n\x11ImageInstanceInfo\x18\x03 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodDomainInstanceInfos\x12\x19\n\x11\x44\x65\x66\x61ultPlayDomain\x18\x04 \x01(\t\"\xb5\x01\n\x16VodDomainInstanceInfos\x12L\n\rByteInstances\x18\x01 \x03(\x0b\x32\x35.Volcengine.Vod.Models.Business.VodDomainInstanceInfo\x12M\n\x0eOtherInstances\x18\x02 \x03(\x0b\x32\x35.Volcengine.Vod.Models.Business.VodDomainInstanceInfo\"\x9a\x01\n\x15VodDomainInstanceInfo\x12\x12\n\nInstanceId\x18\x01 \x01(\t\x12?\n\x07\x44omains\x18\x02 \x03(\x0b\x32..Volcengine.Vod.Models.Business.VodDomainoInfo\x12\x16\n\x0e\x43\x61nSelfEditing\x18\x03 \x01(\x08\x12\x14\n\x0c\x43onfigStatus\x18\x04 \x01(\t\"\xcb\x02\n\x0eVodDomainoInfo\x12\x0e\n\x06\x44omain\x18\x01 \x01(\t\x12\r\n\x05\x43name\x18\x02 \x01(\t\x12\x14\n\x0c\x43onfigStatus\x18\x03 \x01(\t\x12\x13\n\x0b\x43nameStatus\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\x12M\n\x0b\x43\x65rtificate\x18\x06 \x01(\x0b\x32\x38.Volcengine.Vod.Models.Business.VodDomainCertificateInfo\x12\x12\n\nCreateTime\x18\x07 \x01(\t\x12\x12\n\nUpdateTime\x18\x08 \x01(\t\x12\x0e\n\x06Region\x18\t \x01(\t\x12\x44\n\x07Sources\x18\n \x03(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodDomainSourceInfo\x12\x12\n\nLockStatus\x18\x0b \x01(\t\"\xa2\x01\n\x18VodDomainCertificateInfo\x12\x15\n\rCertificateId\x18\x01 \x01(\t\x12\x17\n\x0f\x43\x65rtificateName\x18\x02 \x01(\t\x12\x16\n\x0e\x43\x65rtificatePub\x18\x03 \x01(\t\x12\x16\n\x0e\x43\x65rtificatePri\x18\x04 \x01(\t\x12\x13\n\x0bHttpsStatus\x18\x05 \x01(\t\x12\x11\n\tExpiredAt\x18\x06 \x01(\t\"(\n\x16VodCreateCdnTaskResult\x12\x0e\n\x06TaskId\x18\x01 \x01(\t\"x\n\x0eVodContentInfo\x12\x0e\n\x06ItemId\x18\x01 \x01(\t\x12\x0b\n\x03Url\x18\x02 \x01(\t\x12\x0e\n\x06Status\x18\x03 \x01(\t\x12\x10\n\x08TaskType\x18\x04 \x01(\t\x12\x17\n\x0f\x43reateTimestamp\x18\x05 \x01(\x05\x12\x0e\n\x06TaskId\x18\x06 \x01(\t\"\x8f\x01\n\x10VodCdnTaskResult\x12\x12\n\nTotalCount\x18\x01 \x01(\x05\x12\x0f\n\x07PageNum\x18\x02 \x01(\x05\x12\x10\n\x08PageSize\x18\x03 \x01(\x05\x12\x44\n\x0c\x43ontentInfos\x18\x04 \x03(\x0b\x32..Volcengine.Vod.Models.Business.VodContentInfo\"\x7f\n\x16VodCdnAccessLogElement\x12\x13\n\x0b\x44ownloadUrl\x18\x01 \x01(\t\x12\x10\n\x08\x46ileSize\x18\x02 \x01(\x03\x12\x10\n\x08\x46ileName\x18\x03 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x04 \x01(\x05\x12\x14\n\x0c\x45ndTimestamp\x18\x05 \x01(\x05\"n\n\x13VodCdnAccessLogInfo\x12\x0e\n\x06\x44omain\x18\x01 \x01(\t\x12G\n\x07LogList\x18\x02 \x03(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodCdnAccessLogElement\"^\n\x19VodListCdnAccessLogResult\x12\x41\n\x04Logs\x18\x01 \x03(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodCdnAccessLogInfo\"B\n\x19VodCdnTopAccessUrlElement\x12\x0b\n\x03Url\x18\x01 \x01(\t\x12\n\n\x02Pv\x18\x02 \x01(\x03\x12\x0c\n\x04\x46lux\x18\x03 \x01(\x03\"k\n\x1cVodListCdnTopAccessUrlResult\x12K\n\x08UrlInfos\x18\x01 \x03(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodCdnTopAccessUrlElement\"3\n\x10VodBandwidthData\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\x11\n\tBandwidth\x18\x02 \x01(\x01\"\x8c\x02\n\'VodDescribeVodDomainBandwidthDataResult\x12\x12\n\nDomainList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x15\n\rBandwidthType\x18\x05 \x01(\t\x12\x15\n\rPeakBandwidth\x18\x06 \x01(\x01\x12\x19\n\x11PeakBandwidthTime\x18\x07 \x01(\t\x12K\n\x11\x42\x61ndwidthDataList\x18\x08 \x03(\x0b\x32\x30.Volcengine.Vod.Models.Business.VodBandwidthData\"\x80\x01\n\x14VodCdnStatisticsData\x12\x0c\n\x04Name\x18\x01 \x01(\t\x12\x0e\n\x06Metric\x18\x02 \x01(\t\x12\x10\n\x08\x44\x61taType\x18\x03 \x01(\t\x12\x38\n\x06Points\x18\x04 \x03(\x0b\x32(.Volcengine.Vod.Models.Business.VodPoint\"\x80\x01\n\x1cVodCdnStatisticsCommonResult\x12\x43\n\x05\x44\x61tas\x18\x01 \x03(\x0b\x32\x34.Volcengine.Vod.Models.Business.VodCdnStatisticsData\x12\x1b\n\x13NoPermissionDomains\x18\x02 \x03(\t\"H\n\x0cVodCdnIpInfo\x12\n\n\x02Ip\x18\x01 \x01(\t\x12\r\n\x05\x43\x64nIp\x18\x02 \x01(\x08\x12\x10\n\x08Location\x18\x03 \x01(\t\x12\x0b\n\x03Isp\x18\x04 \x01(\t\"V\n\x17VodDescribeIpInfoResult\x12;\n\x05Infos\x18\x01 \x03(\x0b\x32,.Volcengine.Vod.Models.Business.VodCdnIpInfo\"/\n\x0eVodTrafficData\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\x0f\n\x07Traffic\x18\x02 \x01(\x01\"\xe8\x01\n%VodDescribeVodDomainTrafficDataResult\x12\x12\n\nDomainList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x13\n\x0bTrafficType\x18\x05 \x01(\t\x12\x14\n\x0cTotalTraffic\x18\x06 \x01(\x01\x12G\n\x0fTrafficDataList\x18\x07 \x03(\x0b\x32..Volcengine.Vod.Models.Business.VodTrafficData\"\xac\x02\n\x13VodDomainSourceInfo\x12U\n\x11SourceStationType\x18\x01 \x01(\x0e\x32:.Volcengine.Vod.Models.Business.VodDomainSourceStationType\x12\x63\n\x18SourceStationAddressType\x18\x02 \x01(\x0e\x32\x41.Volcengine.Vod.Models.Business.VodDomainSourceStationAddressType\x12\x0e\n\x06Origin\x18\x03 \x01(\t\x12I\n\x06\x42ucket\x18\x04 \x01(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodDomainOriginBucketInfo\"_\n\x19VodDomainOriginBucketInfo\x12\x12\n\nBucketName\x18\x01 \x01(\t\x12\x18\n\x10\x42ucketSourceType\x18\x02 \x01(\t\x12\x14\n\x0c\x42ucketRegion\x18\x03 \x01(\t\"+\n\x19VodSubmitBlockTasksResult\x12\x0e\n\x06TaskID\x18\x01 \x01(\t\"\x8c\x01\n\x1dVodGetContentBlockTasksResult\x12\r\n\x05Total\x18\x01 \x01(\x03\x12\x0f\n\x07PageNum\x18\x02 \x01(\x03\x12\x10\n\x08PageSize\x18\x03 \x01(\x03\x12\x39\n\x04\x44\x61ta\x18\x04 \x03(\x0b\x32+.Volcengine.Vod.Models.Business.ContentTask\"`\n\x0b\x43ontentTask\x12\x0b\n\x03Url\x18\x01 \x01(\t\x12\x0e\n\x06Status\x18\x02 \x01(\t\x12\x10\n\x08TaskType\x18\x03 \x01(\t\x12\x12\n\nCreateTime\x18\x04 \x01(\x03\x12\x0e\n\x06TaskID\x18\x05 \x01(\t*\x92\x01\n\x1aVodDomainSourceStationType\x12\'\n#UndefinedVodDomainSourceStationType\x10\x00\x12!\n\x1dVodVodDomainSourceStationType\x10\x01\x12(\n$ThirdPartyVodDomainSourceStationType\x10\x02*\xa9\x01\n!VodDomainSourceStationAddressType\x12.\n*UndefinedVodDomainSourceStationAddressType\x10\x00\x12+\n\'DomainVodDomainSourceStationAddressType\x10\x01\x12\'\n#IPVodDomainSourceStationAddressType\x10\x02\x42\xca\x01\n)com.volcengine.service.vod.model.businessB\x06VodCdnP\x01ZAgithub.com/volcengine/volc-sdk-golang/service/vod/models/business\xa0\x01\x01\xd8\x01\x01\xc2\x02\x00\xca\x02 Volc\\Service\\Vod\\Models\\Business\xe2\x02#Volc\\Service\\Vod\\Models\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1avod/business/vod_cdn.proto\x12\x1eVolcengine.Vod.Models.Business\x1a\x1dvod/business/vod_common.proto\"\x87\x02\n\x13VodDomainConfigInfo\x12\x11\n\tSpaceName\x18\x01 \x01(\t\x12P\n\x10PlayInstanceInfo\x18\x02 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodDomainInstanceInfos\x12Q\n\x11ImageInstanceInfo\x18\x03 \x01(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodDomainInstanceInfos\x12\x19\n\x11\x44\x65\x66\x61ultPlayDomain\x18\x04 \x01(\t\x12\r\n\x05Total\x18\x05 \x01(\x03\x12\x0e\n\x06Offset\x18\x06 \x01(\x03\"\xb5\x01\n\x16VodDomainInstanceInfos\x12L\n\rByteInstances\x18\x01 \x03(\x0b\x32\x35.Volcengine.Vod.Models.Business.VodDomainInstanceInfo\x12M\n\x0eOtherInstances\x18\x02 \x03(\x0b\x32\x35.Volcengine.Vod.Models.Business.VodDomainInstanceInfo\"\x9a\x01\n\x15VodDomainInstanceInfo\x12\x12\n\nInstanceId\x18\x01 \x01(\t\x12?\n\x07\x44omains\x18\x02 \x03(\x0b\x32..Volcengine.Vod.Models.Business.VodDomainoInfo\x12\x16\n\x0e\x43\x61nSelfEditing\x18\x03 \x01(\x08\x12\x14\n\x0c\x43onfigStatus\x18\x04 \x01(\t\"\xcb\x02\n\x0eVodDomainoInfo\x12\x0e\n\x06\x44omain\x18\x01 \x01(\t\x12\r\n\x05\x43name\x18\x02 \x01(\t\x12\x14\n\x0c\x43onfigStatus\x18\x03 \x01(\t\x12\x13\n\x0b\x43nameStatus\x18\x04 \x01(\t\x12\x0e\n\x06Status\x18\x05 \x01(\t\x12M\n\x0b\x43\x65rtificate\x18\x06 \x01(\x0b\x32\x38.Volcengine.Vod.Models.Business.VodDomainCertificateInfo\x12\x12\n\nCreateTime\x18\x07 \x01(\t\x12\x12\n\nUpdateTime\x18\x08 \x01(\t\x12\x0e\n\x06Region\x18\t \x01(\t\x12\x44\n\x07Sources\x18\n \x03(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodDomainSourceInfo\x12\x12\n\nLockStatus\x18\x0b \x01(\t\"\xa2\x01\n\x18VodDomainCertificateInfo\x12\x15\n\rCertificateId\x18\x01 \x01(\t\x12\x17\n\x0f\x43\x65rtificateName\x18\x02 \x01(\t\x12\x16\n\x0e\x43\x65rtificatePub\x18\x03 \x01(\t\x12\x16\n\x0e\x43\x65rtificatePri\x18\x04 \x01(\t\x12\x13\n\x0bHttpsStatus\x18\x05 \x01(\t\x12\x11\n\tExpiredAt\x18\x06 \x01(\t\"(\n\x16VodCreateCdnTaskResult\x12\x0e\n\x06TaskId\x18\x01 \x01(\t\"\x89\x01\n\x0eVodContentInfo\x12\x0e\n\x06ItemId\x18\x01 \x01(\t\x12\x0b\n\x03Url\x18\x02 \x01(\t\x12\x0e\n\x06Status\x18\x03 \x01(\t\x12\x10\n\x08TaskType\x18\x04 \x01(\t\x12\x17\n\x0f\x43reateTimestamp\x18\x05 \x01(\x05\x12\x0e\n\x06TaskId\x18\x06 \x01(\t\x12\x0f\n\x07Message\x18\x07 \x01(\t\"\x8f\x01\n\x10VodCdnTaskResult\x12\x12\n\nTotalCount\x18\x01 \x01(\x05\x12\x0f\n\x07PageNum\x18\x02 \x01(\x05\x12\x10\n\x08PageSize\x18\x03 \x01(\x05\x12\x44\n\x0c\x43ontentInfos\x18\x04 \x03(\x0b\x32..Volcengine.Vod.Models.Business.VodContentInfo\"\x7f\n\x16VodCdnAccessLogElement\x12\x13\n\x0b\x44ownloadUrl\x18\x01 \x01(\t\x12\x10\n\x08\x46ileSize\x18\x02 \x01(\x03\x12\x10\n\x08\x46ileName\x18\x03 \x01(\t\x12\x16\n\x0eStartTimestamp\x18\x04 \x01(\x05\x12\x14\n\x0c\x45ndTimestamp\x18\x05 \x01(\x05\"n\n\x13VodCdnAccessLogInfo\x12\x0e\n\x06\x44omain\x18\x01 \x01(\t\x12G\n\x07LogList\x18\x02 \x03(\x0b\x32\x36.Volcengine.Vod.Models.Business.VodCdnAccessLogElement\"^\n\x19VodListCdnAccessLogResult\x12\x41\n\x04Logs\x18\x01 \x03(\x0b\x32\x33.Volcengine.Vod.Models.Business.VodCdnAccessLogInfo\"B\n\x19VodCdnTopAccessUrlElement\x12\x0b\n\x03Url\x18\x01 \x01(\t\x12\n\n\x02Pv\x18\x02 \x01(\x03\x12\x0c\n\x04\x46lux\x18\x03 \x01(\x03\"k\n\x1cVodListCdnTopAccessUrlResult\x12K\n\x08UrlInfos\x18\x01 \x03(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodCdnTopAccessUrlElement\"3\n\x10VodBandwidthData\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\x11\n\tBandwidth\x18\x02 \x01(\x01\"\x8c\x02\n\'VodDescribeVodDomainBandwidthDataResult\x12\x12\n\nDomainList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x15\n\rBandwidthType\x18\x05 \x01(\t\x12\x15\n\rPeakBandwidth\x18\x06 \x01(\x01\x12\x19\n\x11PeakBandwidthTime\x18\x07 \x01(\t\x12K\n\x11\x42\x61ndwidthDataList\x18\x08 \x03(\x0b\x32\x30.Volcengine.Vod.Models.Business.VodBandwidthData\"\x80\x01\n\x14VodCdnStatisticsData\x12\x0c\n\x04Name\x18\x01 \x01(\t\x12\x0e\n\x06Metric\x18\x02 \x01(\t\x12\x10\n\x08\x44\x61taType\x18\x03 \x01(\t\x12\x38\n\x06Points\x18\x04 \x03(\x0b\x32(.Volcengine.Vod.Models.Business.VodPoint\"\x80\x01\n\x1cVodCdnStatisticsCommonResult\x12\x43\n\x05\x44\x61tas\x18\x01 \x03(\x0b\x32\x34.Volcengine.Vod.Models.Business.VodCdnStatisticsData\x12\x1b\n\x13NoPermissionDomains\x18\x02 \x03(\t\"H\n\x0cVodCdnIpInfo\x12\n\n\x02Ip\x18\x01 \x01(\t\x12\r\n\x05\x43\x64nIp\x18\x02 \x01(\x08\x12\x10\n\x08Location\x18\x03 \x01(\t\x12\x0b\n\x03Isp\x18\x04 \x01(\t\"V\n\x17VodDescribeIpInfoResult\x12;\n\x05Infos\x18\x01 \x03(\x0b\x32,.Volcengine.Vod.Models.Business.VodCdnIpInfo\"/\n\x0eVodTrafficData\x12\x0c\n\x04Time\x18\x01 \x01(\t\x12\x0f\n\x07Traffic\x18\x02 \x01(\x01\"\xe8\x01\n%VodDescribeVodDomainTrafficDataResult\x12\x12\n\nDomainList\x18\x01 \x03(\t\x12\x11\n\tStartTime\x18\x02 \x01(\t\x12\x0f\n\x07\x45ndTime\x18\x03 \x01(\t\x12\x13\n\x0b\x41ggregation\x18\x04 \x01(\x05\x12\x13\n\x0bTrafficType\x18\x05 \x01(\t\x12\x14\n\x0cTotalTraffic\x18\x06 \x01(\x01\x12G\n\x0fTrafficDataList\x18\x07 \x03(\x0b\x32..Volcengine.Vod.Models.Business.VodTrafficData\"\xac\x02\n\x13VodDomainSourceInfo\x12U\n\x11SourceStationType\x18\x01 \x01(\x0e\x32:.Volcengine.Vod.Models.Business.VodDomainSourceStationType\x12\x63\n\x18SourceStationAddressType\x18\x02 \x01(\x0e\x32\x41.Volcengine.Vod.Models.Business.VodDomainSourceStationAddressType\x12\x0e\n\x06Origin\x18\x03 \x01(\t\x12I\n\x06\x42ucket\x18\x04 \x01(\x0b\x32\x39.Volcengine.Vod.Models.Business.VodDomainOriginBucketInfo\"_\n\x19VodDomainOriginBucketInfo\x12\x12\n\nBucketName\x18\x01 \x01(\t\x12\x18\n\x10\x42ucketSourceType\x18\x02 \x01(\t\x12\x14\n\x0c\x42ucketRegion\x18\x03 \x01(\t\"+\n\x19VodSubmitBlockTasksResult\x12\x0e\n\x06TaskID\x18\x01 \x01(\t\"\x8c\x01\n\x1dVodGetContentBlockTasksResult\x12\r\n\x05Total\x18\x01 \x01(\x03\x12\x0f\n\x07PageNum\x18\x02 \x01(\x03\x12\x10\n\x08PageSize\x18\x03 \x01(\x03\x12\x39\n\x04\x44\x61ta\x18\x04 \x03(\x0b\x32+.Volcengine.Vod.Models.Business.ContentTask\"`\n\x0b\x43ontentTask\x12\x0b\n\x03Url\x18\x01 \x01(\t\x12\x0e\n\x06Status\x18\x02 \x01(\t\x12\x10\n\x08TaskType\x18\x03 \x01(\t\x12\x12\n\nCreateTime\x18\x04 \x01(\x03\x12\x0e\n\x06TaskID\x18\x05 \x01(\t*\x92\x01\n\x1aVodDomainSourceStationType\x12\'\n#UndefinedVodDomainSourceStationType\x10\x00\x12!\n\x1dVodVodDomainSourceStationType\x10\x01\x12(\n$ThirdPartyVodDomainSourceStationType\x10\x02*\xa9\x01\n!VodDomainSourceStationAddressType\x12.\n*UndefinedVodDomainSourceStationAddressType\x10\x00\x12+\n\'DomainVodDomainSourceStationAddressType\x10\x01\x12\'\n#IPVodDomainSourceStationAddressType\x10\x02\x42\xca\x01\n)com.volcengine.service.vod.model.businessB\x06VodCdnP\x01ZAgithub.com/volcengine/volc-sdk-golang/service/vod/models/business\xa0\x01\x01\xd8\x01\x01\xc2\x02\x00\xca\x02 Volc\\Service\\Vod\\Models\\Business\xe2\x02#Volc\\Service\\Vod\\Models\\GPBMetadatab\x06proto3')
 
 _VODDOMAINSOURCESTATIONTYPE = DESCRIPTOR.enum_types_by_name['VodDomainSourceStationType']
 VodDomainSourceStationType = enum_type_wrapper.EnumTypeWrapper(_VODDOMAINSOURCESTATIONTYPE)
 _VODDOMAINSOURCESTATIONADDRESSTYPE = DESCRIPTOR.enum_types_by_name['VodDomainSourceStationAddressType']
 VodDomainSourceStationAddressType = enum_type_wrapper.EnumTypeWrapper(_VODDOMAINSOURCESTATIONADDRESSTYPE)
 UndefinedVodDomainSourceStationType = 0
 VodVodDomainSourceStationType = 1
@@ -238,64 +238,64 @@
   })
 _sym_db.RegisterMessage(ContentTask)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n)com.volcengine.service.vod.model.businessB\006VodCdnP\001ZAgithub.com/volcengine/volc-sdk-golang/service/vod/models/business\240\001\001\330\001\001\302\002\000\312\002 Volc\\Service\\Vod\\Models\\Business\342\002#Volc\\Service\\Vod\\Models\\GPBMetadata'
-  _VODDOMAINSOURCESTATIONTYPE._serialized_start=3711
-  _VODDOMAINSOURCESTATIONTYPE._serialized_end=3857
-  _VODDOMAINSOURCESTATIONADDRESSTYPE._serialized_start=3860
-  _VODDOMAINSOURCESTATIONADDRESSTYPE._serialized_end=4029
+  _VODDOMAINSOURCESTATIONTYPE._serialized_start=3760
+  _VODDOMAINSOURCESTATIONTYPE._serialized_end=3906
+  _VODDOMAINSOURCESTATIONADDRESSTYPE._serialized_start=3909
+  _VODDOMAINSOURCESTATIONADDRESSTYPE._serialized_end=4078
   _VODDOMAINCONFIGINFO._serialized_start=94
-  _VODDOMAINCONFIGINFO._serialized_end=326
-  _VODDOMAININSTANCEINFOS._serialized_start=329
-  _VODDOMAININSTANCEINFOS._serialized_end=510
-  _VODDOMAININSTANCEINFO._serialized_start=513
-  _VODDOMAININSTANCEINFO._serialized_end=667
-  _VODDOMAINOINFO._serialized_start=670
-  _VODDOMAINOINFO._serialized_end=1001
-  _VODDOMAINCERTIFICATEINFO._serialized_start=1004
-  _VODDOMAINCERTIFICATEINFO._serialized_end=1166
-  _VODCREATECDNTASKRESULT._serialized_start=1168
-  _VODCREATECDNTASKRESULT._serialized_end=1208
-  _VODCONTENTINFO._serialized_start=1210
-  _VODCONTENTINFO._serialized_end=1330
-  _VODCDNTASKRESULT._serialized_start=1333
-  _VODCDNTASKRESULT._serialized_end=1476
-  _VODCDNACCESSLOGELEMENT._serialized_start=1478
-  _VODCDNACCESSLOGELEMENT._serialized_end=1605
-  _VODCDNACCESSLOGINFO._serialized_start=1607
-  _VODCDNACCESSLOGINFO._serialized_end=1717
-  _VODLISTCDNACCESSLOGRESULT._serialized_start=1719
-  _VODLISTCDNACCESSLOGRESULT._serialized_end=1813
-  _VODCDNTOPACCESSURLELEMENT._serialized_start=1815
-  _VODCDNTOPACCESSURLELEMENT._serialized_end=1881
-  _VODLISTCDNTOPACCESSURLRESULT._serialized_start=1883
-  _VODLISTCDNTOPACCESSURLRESULT._serialized_end=1990
-  _VODBANDWIDTHDATA._serialized_start=1992
-  _VODBANDWIDTHDATA._serialized_end=2043
-  _VODDESCRIBEVODDOMAINBANDWIDTHDATARESULT._serialized_start=2046
-  _VODDESCRIBEVODDOMAINBANDWIDTHDATARESULT._serialized_end=2314
-  _VODCDNSTATISTICSDATA._serialized_start=2317
-  _VODCDNSTATISTICSDATA._serialized_end=2445
-  _VODCDNSTATISTICSCOMMONRESULT._serialized_start=2448
-  _VODCDNSTATISTICSCOMMONRESULT._serialized_end=2576
-  _VODCDNIPINFO._serialized_start=2578
-  _VODCDNIPINFO._serialized_end=2650
-  _VODDESCRIBEIPINFORESULT._serialized_start=2652
-  _VODDESCRIBEIPINFORESULT._serialized_end=2738
-  _VODTRAFFICDATA._serialized_start=2740
-  _VODTRAFFICDATA._serialized_end=2787
-  _VODDESCRIBEVODDOMAINTRAFFICDATARESULT._serialized_start=2790
-  _VODDESCRIBEVODDOMAINTRAFFICDATARESULT._serialized_end=3022
-  _VODDOMAINSOURCEINFO._serialized_start=3025
-  _VODDOMAINSOURCEINFO._serialized_end=3325
-  _VODDOMAINORIGINBUCKETINFO._serialized_start=3327
-  _VODDOMAINORIGINBUCKETINFO._serialized_end=3422
-  _VODSUBMITBLOCKTASKSRESULT._serialized_start=3424
-  _VODSUBMITBLOCKTASKSRESULT._serialized_end=3467
-  _VODGETCONTENTBLOCKTASKSRESULT._serialized_start=3470
-  _VODGETCONTENTBLOCKTASKSRESULT._serialized_end=3610
-  _CONTENTTASK._serialized_start=3612
-  _CONTENTTASK._serialized_end=3708
+  _VODDOMAINCONFIGINFO._serialized_end=357
+  _VODDOMAININSTANCEINFOS._serialized_start=360
+  _VODDOMAININSTANCEINFOS._serialized_end=541
+  _VODDOMAININSTANCEINFO._serialized_start=544
+  _VODDOMAININSTANCEINFO._serialized_end=698
+  _VODDOMAINOINFO._serialized_start=701
+  _VODDOMAINOINFO._serialized_end=1032
+  _VODDOMAINCERTIFICATEINFO._serialized_start=1035
+  _VODDOMAINCERTIFICATEINFO._serialized_end=1197
+  _VODCREATECDNTASKRESULT._serialized_start=1199
+  _VODCREATECDNTASKRESULT._serialized_end=1239
+  _VODCONTENTINFO._serialized_start=1242
+  _VODCONTENTINFO._serialized_end=1379
+  _VODCDNTASKRESULT._serialized_start=1382
+  _VODCDNTASKRESULT._serialized_end=1525
+  _VODCDNACCESSLOGELEMENT._serialized_start=1527
+  _VODCDNACCESSLOGELEMENT._serialized_end=1654
+  _VODCDNACCESSLOGINFO._serialized_start=1656
+  _VODCDNACCESSLOGINFO._serialized_end=1766
+  _VODLISTCDNACCESSLOGRESULT._serialized_start=1768
+  _VODLISTCDNACCESSLOGRESULT._serialized_end=1862
+  _VODCDNTOPACCESSURLELEMENT._serialized_start=1864
+  _VODCDNTOPACCESSURLELEMENT._serialized_end=1930
+  _VODLISTCDNTOPACCESSURLRESULT._serialized_start=1932
+  _VODLISTCDNTOPACCESSURLRESULT._serialized_end=2039
+  _VODBANDWIDTHDATA._serialized_start=2041
+  _VODBANDWIDTHDATA._serialized_end=2092
+  _VODDESCRIBEVODDOMAINBANDWIDTHDATARESULT._serialized_start=2095
+  _VODDESCRIBEVODDOMAINBANDWIDTHDATARESULT._serialized_end=2363
+  _VODCDNSTATISTICSDATA._serialized_start=2366
+  _VODCDNSTATISTICSDATA._serialized_end=2494
+  _VODCDNSTATISTICSCOMMONRESULT._serialized_start=2497
+  _VODCDNSTATISTICSCOMMONRESULT._serialized_end=2625
+  _VODCDNIPINFO._serialized_start=2627
+  _VODCDNIPINFO._serialized_end=2699
+  _VODDESCRIBEIPINFORESULT._serialized_start=2701
+  _VODDESCRIBEIPINFORESULT._serialized_end=2787
+  _VODTRAFFICDATA._serialized_start=2789
+  _VODTRAFFICDATA._serialized_end=2836
+  _VODDESCRIBEVODDOMAINTRAFFICDATARESULT._serialized_start=2839
+  _VODDESCRIBEVODDOMAINTRAFFICDATARESULT._serialized_end=3071
+  _VODDOMAINSOURCEINFO._serialized_start=3074
+  _VODDOMAINSOURCEINFO._serialized_end=3374
+  _VODDOMAINORIGINBUCKETINFO._serialized_start=3376
+  _VODDOMAINORIGINBUCKETINFO._serialized_end=3471
+  _VODSUBMITBLOCKTASKSRESULT._serialized_start=3473
+  _VODSUBMITBLOCKTASKSRESULT._serialized_end=3516
+  _VODGETCONTENTBLOCKTASKSRESULT._serialized_start=3519
+  _VODGETCONTENTBLOCKTASKSRESULT._serialized_end=3659
+  _CONTENTTASK._serialized_start=3661
+  _CONTENTTASK._serialized_end=3757
 # @@protoc_insertion_point(module_scope)
```

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_workflow_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_workflow_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_play_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_play_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_apps_manage_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_apps_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_callback_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_callback_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_media_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_media_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_smart_strategy_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_smart_strategy_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/models/business/vod_space_pb2.py` & `volcengine-1.0.91/volcengine/vod/models/business/vod_space_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/VodService.py` & `volcengine-1.0.91/volcengine/vod/VodService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vod/VodServiceConfig.py` & `volcengine-1.0.91/volcengine/vod/VodServiceConfig.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/sms/SmsService.py` & `volcengine-1.0.91/volcengine/sms/SmsService.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # coding:utf-8
 import json
 import threading
 
 from volcengine.ApiInfo import ApiInfo
 from volcengine.Credentials import Credentials
 from volcengine.base.Service import Service
-from volcengine.ServiceInfo import ServiceInfo
+from volcengine.ServiceInfoHttps import ServiceInfoSms
 from volcengine.const.Const import *
 from retry import retry
 
 
 class SmsService(Service):
     _instance_lock = threading.Lock()
 
     def __new__(cls, *args, **kwargs):
         if not hasattr(SmsService, "_instance"):
             with SmsService._instance_lock:
                 if not hasattr(SmsService, "_instance"):
                     SmsService._instance = object.__new__(cls)
         return SmsService._instance
 
-    def __init__(self, region=REGION_CN_NORTH1):
-        self.service_info = SmsService.get_service_info(self, region)
+    def __init__(self):
+        self.service_info = SmsService.get_service_info(self, REGION_CN_NORTH1)
         self.api_info = SmsService.get_api_info()
         super(SmsService, self).__init__(self.service_info, self.api_info)
 
     @staticmethod
     def get_service_info(self, region):
-        if region == REGION_AP_SINGAPORE1:
-            service_info = ServiceInfo("sms.byteplusapi.com", {'Accept': 'application/json'},
-                                       Credentials('', '', 'volcSMS', region), 5, 5)
-        else:
-            service_info = ServiceInfo("sms.volcengineapi.com", {'Accept': 'application/json'},
-                                       Credentials('', '', 'volcSMS', region), 5, 5)
+        service_info = ServiceInfoSms("sms.volcengineapi.com", {'Accept': 'application/json'},
+                                      Credentials('', '', 'volcSMS', region), 5, 5)
         return service_info
 
     @staticmethod
     def get_api_info():
         api_info = {
             "SendSms": ApiInfo("POST", "/", {"Action": "SendSms", "Version": "2020-01-01"}, {}, {}),
             "SendSmsVerifyCode": ApiInfo("POST", "/", {"Action": "SendSmsVerifyCode", "Version": "2020-01-01"}, {}, {}),
@@ -60,16 +56,16 @@
                                        {}),
             "ApplyVmsTemplate": ApiInfo("POST", "/", {"Action": "ApplyVmsTemplate", "Version": "2021-01-11"}, {},
                                         {}),
             "GetVmsTemplateStatus": ApiInfo("POST", "/", {"Action": "GetVmsTemplateStatus", "Version": "2021-01-11"},
                                             {},
                                             {}),
             "InsertSubAccount": ApiInfo("POST", "/", {"Action": "InsertSubAccount", "Version": "2021-01-11"},
-                                            {},
-                                            {}),
+                                        {},
+                                        {}),
         }
         return api_info
 
     @retry(tries=2, delay=0)
     def send_sms(self, body):
         res = self.json('SendSms', {}, body)
         if res == '':
```

### Comparing `volcengine-1.0.90/volcengine/util/Util.py` & `volcengine-1.0.91/volcengine/util/Util.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/util/Functions.py` & `volcengine-1.0.91/volcengine/util/Functions.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/Service.py` & `volcengine-1.0.91/volcengine/base/Service.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/Request.py` & `volcengine-1.0.91/volcengine/base/Request.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/base/base_pb2.py` & `volcengine-1.0.91/volcengine/base/models/base/base_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/deny_config_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/deny_config_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/pull_to_push_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/pull_to_push_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/record_manage_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/record_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/domain_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/domain_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/relay_source_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/relay_source_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/snapshot_manage_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/snapshot_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/stream_manage_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/stream_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/VQScore_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/VQScore_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/base/models/business/addr_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/addr_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/notify/notify.py` & `volcengine-1.0.91/volcengine/notify/notify.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/adblocker/AdBlockerService.py` & `volcengine-1.0.91/volcengine/adblocker/AdBlockerService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imagex/__init__.py` & `volcengine-1.0.91/volcengine/imagex/__init__.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imagex/ImageXConfig.py` & `volcengine-1.0.91/volcengine/imagex/ImageXConfig.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imagex/ImageXService.py` & `volcengine-1.0.91/volcengine/imagex/ImageXService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imp/ImpService.py` & `volcengine-1.0.91/volcengine/imp/ImpService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imp/ImpServiceConfig.py` & `volcengine-1.0.91/volcengine/imp/ImpServiceConfig.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imp/models/base/base_pb2.py` & `volcengine-1.0.91/volcengine/imp/models/base/base_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imp/models/response/response_imp_pb2.py` & `volcengine-1.0.91/volcengine/imp/models/response/response_imp_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imp/models/request/request_imp_pb2.py` & `volcengine-1.0.91/volcengine/imp/models/request/request_imp_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/imp/models/business/imp_common_pb2.py` & `volcengine-1.0.91/volcengine/imp/models/business/imp_common_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/const/Const.py` & `volcengine-1.0.91/volcengine/const/Const.py`

 * *Files 19% similar despite different names*

```diff
@@ -64,16 +64,28 @@
 AREA_CN = "cn"
 AREA_OVERSEAS = "overseas"
 AREA_ALL = "all"
 
 SOURCE_TYPE_TEXT = "text/string"
 SOURCE_TYPE_VIDEO = "video/mp4"
 SOURCE_TYPE_IMAGE_JPG = "image/jpg"
-Source_TYPE_IMAGE_PNG = "image/png "
-Source_TYPE_IMAGE_GIF = "image/gif"
-Source_TYPE_MP3 = "audio/mp3"
+SOURCE_TYPE_IMAGE_PNG = "image/png "
+SOURCE_TYPE_IMAGE_GIF = "image/gif"
+SOURCE_TYPE_MP3 = "audio/mp3"
 
-SourceTypeImageJPG = "image/jpg"
-SourceTypeImagePNG = "image/png "
-SourceTypeImageGIF = "image/gif"
-SourceTypeAudio = "audio/mp3"
+DOC_TYPE_THREE_IN_ONE = 0  # 三证合一
+DOC_TYPE_BUSINESS_LICENSE = 1  # 企业营业执照
+DOC_TYPE_ORGANIZATION_CODE_CERTIFICATE = 2  # 组织机构代码证
+DOC_TYPE_TAX_REGISTRATION_CERTIFICATE = 3  # 税务登记证
+DOC_TYPE_SOCIAL_CREDIT_CODE_CERTIFICATE = 4  # 社会信用代码证书
+DOC_TYPE_POWER_OF_ATTORNEY = 5  # 授权委托书
+DOC_TYPE_OTHERS = 6  # 其他 / 更多
 
+SIGN_SOURCE_TYPE_COMPANY = "公司全称/简称"
+SIGN_SOURCE_TYPE_SITE = "工信部备案网站全称/简称"
+SIGN_SOURCE_TYPE_APP = "APP全称/简称"
+SIGN_SOURCE_TYPE_OFFICIAL_ACCOUNTS = "公众号、小程序全称/简称"
+SIGN_SOURCE_TYPE_BRAND = "商标全称/简称"
+SIGN_SOURCE_TYPE_STORE = "电商平台店铺名的全称/简称"
+
+SIGN_PURPOSE_FOR_OWN = 1
+SIGN_PURPOSE_FOR_OTHER = 2
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `volcengine-1.0.90/volcengine/visual/VisualService.py` & `volcengine-1.0.91/volcengine/visual/VisualService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/auth/MetaData.py` & `volcengine-1.0.91/volcengine/auth/MetaData.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/auth/SignParam.py` & `volcengine-1.0.91/volcengine/auth/SignParam.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/auth/SignerV4.py` & `volcengine-1.0.91/volcengine/auth/SignerV4.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/nlp/NLPService.py` & `volcengine-1.0.91/volcengine/nlp/NLPService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/livesaas/LivesaasService.py` & `volcengine-1.0.91/volcengine/livesaas/LivesaasService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/verender/VerenderService.py` & `volcengine-1.0.91/volcengine/verender/VerenderService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/content_security/ContentSecurityService.py` & `volcengine-1.0.91/volcengine/content_security/ContentSecurityService.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         return service_info
 
     @staticmethod
     def get_api_info():
         api_info = {"AsyncVideoRisk": ApiInfo("POST", "/", {"Action": "AsyncVideoRisk", "Version": "2021-11-29"}, {}, {}),
                     "VideoResult": ApiInfo("GET", "/", {"Action": "VideoResult", "Version": "2021-11-29"}, {}, {}),
                     "ImageContentRisk": ApiInfo("POST", "/", {"Action": "ImageContentRisk", "Version": "2021-11-29"}, {}, {}),
+                    "ImageContentRiskV2": ApiInfo("POST", "/", {"Action": "ImageContentRiskV2", "Version": "2021-11-29"}, {}, {}),
                     "AsyncImageRisk": ApiInfo("POST", "/", {"Action": "AsyncImageRisk", "Version": "2021-11-29"}, {}, {}),
                     "ImageResult": ApiInfo("GET", "/", {"Action": "GetImageResult", "Version": "2021-11-29"}, {}, {}),
                     "TextRisk": ApiInfo("POST", "/", {"Action": "TextRisk", "Version": "2022-01-26"}, {}, {}),
                     "CreateCustomContents": ApiInfo("POST", "/", {"Action": "CreateCustomContents", "Version": "2022-01-22"}, {}, {}),
                     "UploadCustomContents": ApiInfo("POST", "/", {"Action": "UploadCustomContents", "Version": "2022-02-07"}, {}, {}),
                     "EnableCustomContents": ApiInfo("PUT", "/", {"Action": "EnableCustomContents", "Version": "2022-04-28"}, {}, {}),
                     "DisableCustomContents": ApiInfo("PUT", "/", {"Action": "DisableCustomContents", "Version": "2022-04-28"}, {}, {}),
@@ -79,14 +80,21 @@
     def image_content_risk(self, params, body):
         res = self.json("ImageContentRisk", params, json.dumps(body))
         if res == '':
             raise Exception("empty response")
         res_json = json.loads(res)
         return res_json
 
+    def image_content_risk_v2(self, params, body):
+        res = self.json("ImageContentRiskV2", params, json.dumps(body))
+        if res == '':
+            raise Exception("empty response")
+        res_json = json.loads(res)
+        return res_json
+
     @redo.retriable(sleeptime=0.1, jitter=0.01, attempts=2,
                     retry_exceptions=(exceptions.ConnectionError, exceptions.ConnectTimeout))
     def async_image_risk(self, params, body):
         res = self.json("AsyncImageRisk", params, json.dumps(body))
         if res == '':
             raise Exception("empty response")
         res_json = json.loads(res)
```

### Comparing `volcengine-1.0.90/volcengine/Policy.py` & `volcengine-1.0.91/volcengine/Policy.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/rtc/example_start_record.py` & `volcengine-1.0.91/volcengine/example/rtc/example_start_record.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/rtc/example_get_record_task.py` & `volcengine-1.0.91/volcengine/example/rtc/example_get_record_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/rtc/example_stop_reocrd.py` & `volcengine-1.0.91/volcengine/example/rtc/example_stop_reocrd.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/rtc/RtcService.py` & `volcengine-1.0.91/volcengine/example/rtc/RtcService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_domain_logs.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_domain_logs.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_domain_isp_data.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_domain_isp_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_top_ips.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_top_ips.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_top_domains.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_top_domains.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_origin_statistics_detail.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_origin_statistics_detail.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/retry_purge_prefetch_task.py` & `volcengine-1.0.91/volcengine/example/dcdn/retry_purge_prefetch_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_realtime_data.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_realtime_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_statistics_detail.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_statistics_detail.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/update_domain_config.py` & `volcengine-1.0.91/volcengine/example/dcdn/update_domain_config.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_domain_region_data.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_domain_region_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_top_urls.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_top_urls.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_domain_pv_data.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_domain_pv_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_top_referers.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_top_referers.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_domain_uv_data.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_domain_uv_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_origin_statistics.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_origin_statistics.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_statistics.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_statistics.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/create_purge_prefetch_task.py` & `volcengine-1.0.91/volcengine/example/dcdn/create_purge_prefetch_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/check_purge_prefetch_task.py` & `volcengine-1.0.91/volcengine/example/dcdn/check_purge_prefetch_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/create_domain.py` & `volcengine-1.0.91/volcengine/example/dcdn/create_domain.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/dcdn/describe_origin_realtime_data.py` & `volcengine-1.0.91/volcengine/example/dcdn/describe_origin_realtime_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/add_cdn_certificate.py` & `volcengine-1.0.91/volcengine/example/cdn/add_cdn_certificate.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_district_isp_data.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_district_isp_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_accounting_data.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_accounting_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/update_cdn_config.py` & `volcengine-1.0.91/volcengine/example/cdn/update_cdn_config.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/update_resource_tags.py` & `volcengine-1.0.91/volcengine/example/cdn/update_resource_tags.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/add_cdn_domain.py` & `volcengine-1.0.91/volcengine/example/cdn/add_cdn_domain.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_content_block_tasks.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_content_block_tasks.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_edge_top_status_code.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_edge_top_status_code.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_origin_top_nrt_data.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_origin_top_nrt_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_edge_top_statistical_data.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_edge_top_statistical_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_edge_nrt_data_summary.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_edge_nrt_data_summary.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_origin_top_status_code.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_origin_top_status_code.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_accounting_summary.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_accounting_summary.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_edge_statistical_data.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_edge_statistical_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_cdn_access_log.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_cdn_access_log.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_cdn_data_detail.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_cdn_data_detail.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/delete_resource_tags.py` & `volcengine-1.0.91/volcengine/example/cdn/delete_resource_tags.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_cdn_data.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_cdn_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_cdn_origin_data.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_cdn_origin_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_origin_nrt_data_summary.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_origin_nrt_data_summary.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/describe_edge_top_nrt_data.py` & `volcengine-1.0.91/volcengine/example/cdn/describe_edge_top_nrt_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/cdn/add_resource_tags.py` & `volcengine-1.0.91/volcengine/example/cdn/add_resource_tags.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vedit/example_edit.py` & `volcengine-1.0.91/volcengine/example/vedit/example_edit.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/CreateCdnRefreshTaskExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/CreateCdnRefreshTaskExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/DescribeCdnIpExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/DescribeCdnIpExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnPvDataExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnPvDataExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/DescribeVodDomainTrafficDataExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/DescribeVodDomainTrafficDataExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnStatusDataExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnStatusDataExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnUsageDataExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnUsageDataExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnTopAccessUrlExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnTopAccessUrlExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnTasksExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnTasksExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/ListDomainExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/ListDomainExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/CreateCdnPreloadTaskExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/CreateCdnPreloadTaskExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/ListCdnAccessLogExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/ListCdnAccessLogExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/cdn/DescribeVodDomainBandwidthDataExample.py` & `volcengine-1.0.91/volcengine/example/vod/cdn/DescribeVodDomainBandwidthDataExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/space/CreateSpaceExample.py` & `volcengine-1.0.91/volcengine/example/vod/space/CreateSpaceExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/space/UpdateSpaceExample.py` & `volcengine-1.0.91/volcengine/example/vod/space/UpdateSpaceExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/space/ListSpaceExample.py` & `volcengine-1.0.91/volcengine/example/vod/space/ListSpaceExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/space/DescribeVodSpaceStorageDataExample.py` & `volcengine-1.0.91/volcengine/example/vod/space/DescribeVodSpaceStorageDataExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/space/UpdateSpaceUploadConfigExample.py` & `volcengine-1.0.91/volcengine/example/vod/space/UpdateSpaceUploadConfigExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/vedit/GetDirectEditProgress.py` & `volcengine-1.0.91/volcengine/example/vod/vedit/GetDirectEditProgress.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/vedit/GetDirectEditResult.py` & `volcengine-1.0.91/volcengine/example/vod/vedit/GetDirectEditResult.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/vedit/SubmitDirectEditTaskAsync.py` & `volcengine-1.0.91/volcengine/example/vod/vedit/SubmitDirectEditTaskAsync.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/workflow/RetrieveTranscodeResultExample.py` & `volcengine-1.0.91/volcengine/example/vod/workflow/RetrieveTranscodeResultExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/workflow/WorkflowExample.py` & `volcengine-1.0.91/volcengine/example/vod/workflow/WorkflowExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/workflow/GetWorkflowExecutionResultExample.py` & `volcengine-1.0.91/volcengine/example/vod/workflow/GetWorkflowExecutionResultExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/workflow/GetWorkflowExecutionExample.py` & `volcengine-1.0.91/volcengine/example/vod/workflow/GetWorkflowExecutionExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/callback/AddCallbackSubscriptionExample.py` & `volcengine-1.0.91/volcengine/example/vod/callback/AddCallbackSubscriptionExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/callback/SetCallbackEvent.py` & `volcengine-1.0.91/volcengine/example/vod/callback/SetCallbackEvent.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSnapshotData.py` & `volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSnapshotData.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceEditDetailData.py` & `volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceEditDetailData.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceDetectStatisData.py` & `volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceDetectStatisData.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceTranscodeData.py` & `volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceTranscodeData.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceSubtitleStatisData.py` & `volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceSubtitleStatisData.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceWorkflowDetailData.py` & `volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceWorkflowDetailData.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/measure/DescribeVodSpaceAIStatisData.py` & `volcengine-1.0.91/volcengine/example/vod/measure/DescribeVodSpaceAIStatisData.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/upload/UploadUrl.py` & `volcengine-1.0.91/volcengine/example/vod/upload/UploadUrl.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/upload/CommitUploadInfoExample.py` & `volcengine-1.0.91/volcengine/example/vod/upload/CommitUploadInfoExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/upload/UploadMedia.py` & `volcengine-1.0.91/volcengine/example/vod/upload/UploadMedia.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/upload/QueryUploadTaskInfo.py` & `volcengine-1.0.91/volcengine/example/vod/upload/QueryUploadTaskInfo.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/upload/ApplyUploadInfoExample.py` & `volcengine-1.0.91/volcengine/example/vod/upload/ApplyUploadInfoExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/upload/UploadMaterial.py` & `volcengine-1.0.91/volcengine/example/vod/upload/UploadMaterial.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/subtitle/SubtitleExample.py` & `volcengine-1.0.91/volcengine/example/vod/subtitle/SubtitleExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/play/GetPlayInfoExample.py` & `volcengine-1.0.91/volcengine/example/vod/play/GetPlayInfoExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/play/GetAllPlayInfoExample.py` & `volcengine-1.0.91/volcengine/example/vod/play/GetAllPlayInfoExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/play/GetPlayAuthTokenExample.py` & `volcengine-1.0.91/volcengine/example/vod/play/GetPlayAuthTokenExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/play/GetPrivateDrmPlayAuthExample.py` & `volcengine-1.0.91/volcengine/example/vod/play/GetPrivateDrmPlayAuthExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/play/GetPlayInfoWithLiveTimeShiftSceneExample.py` & `volcengine-1.0.91/volcengine/example/vod/play/GetPlayInfoWithLiveTimeShiftSceneExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/play/GetPrivateDrmPlayAuthTokenExample.py` & `volcengine-1.0.91/volcengine/example/vod/play/GetPrivateDrmPlayAuthTokenExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/media/GetSubtitleAuthToken.py` & `volcengine-1.0.91/volcengine/example/vod/media/GetSubtitleAuthToken.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/vod/media/MediaExample.py` & `volcengine-1.0.91/volcengine/example/vod/media/MediaExample.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_apply_sms_signature.py` & `volcengine-1.0.91/volcengine/example/sms/example_insert_sms_sub_account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 # coding:utf-8
 from __future__ import print_function
 
 import json
 
-from volcengine.const.Const import *
 from volcengine.sms.SmsService import SmsService
+from volcengine.const.Const import *
 
 if __name__ == '__main__':
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
     # cn
     sms_service = SmsService()
 
     # call below method if you dont set ak and sk in $HOME/.volc/config
     sms_service.set_ak('ak')
     sms_service.set_sk('sk')
-    # sms_service.set_scheme("http")
-    sms_service.set_scheme("https")
     # sms_service.set_host('host')
 
     body = {
-        "SubAccount": "subAccount",
-        "Content": "content",
-        "Desc": "description",
-        "Source": "公司名称/公司缩写",
-        "Domain": "网站域名"
+        "subAccountName": "smsAccount",
+        "desc": "desc",
     }
 
-    resp = sms_service.apply_sms_signature(body)
+    resp = sms_service.insert_sms_sub_account(body)
     print(resp)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_send_batch_sms.py` & `volcengine-1.0.91/volcengine/example/sms/example_send_batch_sms.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,20 @@
 
 import json
 
 from volcengine.const.Const import REGION_AP_SINGAPORE1
 from volcengine.sms.SmsService import SmsService
 
 if __name__ == '__main__':
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
     # cn
     sms_service = SmsService()
 
     # call below method if you dont set ak and sk in $HOME/.volc/config
     sms_service.set_ak('ak')
     sms_service.set_sk('sk')
-    # sms_service.set_scheme("http")
-    # sms_service.set_scheme("https")
     # sms_service.set_host('host')
 
     body = {
         "SmsAccount": "subAccount",
         "Sign": "signature",
         "From": "BytePlus",
         "TemplateID": "ST_xxx",
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_vms_template_query.py` & `volcengine-1.0.91/volcengine/example/sms/example_vms_template_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,20 @@
 if __name__ == '__main__':
     # base64 encode func
     def to_base64_str(file):
         with open(file, 'rb') as fileObj:
             image_data = fileObj.read()
             return base64.b64encode(image_data).decode('utf-8')
 
-
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
     # cn
     sms_service = SmsService()
 
     # call below method if you dont set ak and sk in $HOME/.volc/config
     sms_service.set_ak('ak')
     sms_service.set_sk('sk')
-    # sms_service.set_scheme("http")
-    # sms_service.set_scheme("https")
     # sms_service.set_host('host')
     body = {
         "SubAccount": "subAccount",
         "TemplateId": "templateId"
     }
 
     resp = sms_service.get_vms_template_status(body)
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_get_sub_account_list.py` & `volcengine-1.0.91/volcengine/example/sms/example_get_sms_template_and_order_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # coding:utf-8
 from __future__ import print_function
 
 import json
 
-from volcengine.const.Const import REGION_AP_SINGAPORE1
+from volcengine.const.Const import AREA_CN
 from volcengine.sms.SmsService import SmsService
 
 if __name__ == '__main__':
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
     # cn
     sms_service = SmsService()
-
     # call below method if you dont set ak and sk in $HOME/.volc/config
     sms_service.set_ak('ak')
     sms_service.set_sk('sk')
-    # sms_service.set_scheme("http")
-    # sms_service.set_scheme("https")
     # sms_service.set_host('host')
 
     param = {
-        "subAccountName": "",
+        "subAccount": "subAccount",
+        "area": AREA_CN,
         "pageIndex": 1,
-        "pageSize": 1
+        "pageSize": 10
     }
-
-    resp = sms_service.get_sub_account_list(param)
+    resp = sms_service.get_sms_template_and_order_list(param)
     print(resp)
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_delete_sms_template.py` & `volcengine-1.0.91/volcengine/example/sms/example_get_sub_account_detail.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,27 +3,21 @@
 
 import json
 
 from volcengine.const.Const import REGION_AP_SINGAPORE1
 from volcengine.sms.SmsService import SmsService
 
 if __name__ == '__main__':
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
     # cn
     sms_service = SmsService()
 
     # call below method if you dont set ak and sk in $HOME/.volc/config
-    sms_service.set_ak('ak')
-    sms_service.set_sk('sk')
-    # sms_service.set_scheme("http")
-    # sms_service.set_scheme("https")
-    # sms_service.set_host('host')¬
-
-    body = {
-        "subAccount": "subAccount",
-        "id": "id",
-        "isOrder": True
+    sms_service.set_ak("ak")
+    sms_service.set_sk("sk")
+    # sms_service.set_host('host')
+
+    param = {
+        "subAccount": "subAccount"
     }
 
-    resp = sms_service.delete_sms_template(body)
+    resp = sms_service.get_sub_account_detail(param)
     print(resp)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_get_sms_template_and_order_list.py` & `volcengine-1.0.91/volcengine/example/sms/example_delete_sms_template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # coding:utf-8
 from __future__ import print_function
 
 import json
 
-from volcengine.const.Const import AREA_CN
+from volcengine.const.Const import REGION_AP_SINGAPORE1
 from volcengine.sms.SmsService import SmsService
 
 if __name__ == '__main__':
     # oversea
     # sms_service = SmsService(REGION_AP_SINGAPORE1)
     # cn
     sms_service = SmsService()
 
     # call below method if you dont set ak and sk in $HOME/.volc/config
     sms_service.set_ak('ak')
     sms_service.set_sk('sk')
-    # sms_service.set_scheme("http")
-    # sms_service.set_scheme("https")
     # sms_service.set_host('host')
 
-    param = {
+    body = {
         "subAccount": "subAccount",
-        "area": AREA_CN,
-        "pageIndex": 1,
-        "pageSize": 10
+        "id": "id",
+        "isOrder": True
     }
-    resp = sms_service.get_sms_template_and_order_list(param)
+
+    resp = sms_service.delete_sms_template(body)
     print(resp)
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_conversion.py` & `volcengine-1.0.91/volcengine/example/bioos/example_list_clusters.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # coding:utf-8
 from __future__ import print_function
 
-import json
-
-from volcengine.sms.SmsService import SmsService
+from volcengine.bioos.BioOsService import BioOsService
 
 if __name__ == '__main__':
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
-    # cn
-    sms_service = SmsService()
-
-    # call below method if you dont set ak and sk in $HOME/.volc/config
-    sms_service.set_ak('ak')
-    sms_service.set_sk('sk')
-    # sms_service.set_scheme("http")
-    # sms_service.set_scheme("https")
-    # sms_service.set_host('host')
+    # set endpoint/region here if the default value is unsatisfied
+    bioos_service = BioOsService(endpoint='endpoint', region='region')
 
-    body = {
-        "MessageIDs": ["testMsgId"]
+    # call below method if you don't set ak and sk in $HOME/.volc/config
+    bioos_service.set_ak('ak')
+    bioos_service.set_sk('sk')
+
+    params = {
+        'PageNumber': 1,
+        'PageSize': 10,
+        'Filter': {
+            'IDs': ['test-workflow'],
+            'Status': ['Running'],
+            'Type': ['shared'],
+            'Public': True,
+        },
     }
 
-    resp = sms_service.conversion(body)
+    resp = bioos_service.list_clusters(params)
     print(resp)
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_apply_vms_template.py` & `volcengine-1.0.91/volcengine/example/sms/example_apply_sms_signature.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,41 +10,31 @@
 if __name__ == '__main__':
     # base64 encode func
     def to_base64_str(file):
         with open(file, 'rb') as fileObj:
             image_data = fileObj.read()
             return base64.b64encode(image_data).decode('utf-8')
 
-
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
     # cn
     sms_service = SmsService()
 
     # call below method if you dont set ak and sk in $HOME/.volc/config
     sms_service.set_ak('ak')
     sms_service.set_sk('sk')
-    # sms_service.set_scheme("http")
-    # sms_service.set_scheme("https")
     # sms_service.set_host('host')
-    file_base64_string = to_base64_str("媒体文件路径")
+
     body = {
-        "subAccount": "subAccount",
-        "name": "SDK测试",
-        "theme": "SDK测试视频短信",
-        "signature": "签名",
-        "channelType": "CN_VMS",
-        "contents": [
-            {
-                "sourceType": SOURCE_TYPE_TEXT,
-                "content": "火山引擎，做企业好的伙伴"
-            },
-            {
-                # choose the midea type
-                "sourceType": Source_TYPE_IMAGE_GIF,
-                "content": file_base64_string
-            }
-        ]
+        "SubAccount": "subAccount",
+        "Content": "content",
+        "Desc": "description",
+        "Source": "公司名称/公司缩写",
+        "Domain": "网站域名",
+        "UploadFileList": [{
+            "FileType": DOC_TYPE_THREE_IN_ONE,
+            "FileContent": to_base64_str("图片.jpg"),
+            "FileSuffix": "jpg"
+        }],
+        "Purpose": SIGN_PURPOSE_FOR_OWN
     }
 
-    resp = sms_service.apply_vms_template(body)
+    resp = sms_service.apply_sms_signature(body)
     print(resp)
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_insert_sms_sub_account.py` & `volcengine-1.0.91/volcengine/example/visual/example_video_retargeting_submit_task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # coding:utf-8
 from __future__ import print_function
 
-import json
+import time
 
-from volcengine.sms.SmsService import SmsService
-from volcengine.const.Const import *
+from volcengine.visual.VisualService import VisualService
 
 if __name__ == '__main__':
-    sms_service = SmsService()
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
+    visual_service = VisualService()
 
     # call below method if you dont set ak and sk in $HOME/.volc/config
-    sms_service.set_ak('ak')
-    sms_service.set_sk('sk')
-    # sms_service.set_host('host')
-
-    body = {
-        "subAccountName": "smsAccount",
-        "desc": "desc",
+    visual_service.set_ak('ak')
+    visual_service.set_sk('sk')
+
+    form = {
+        "strategy": "STATIC_CROPPING",
+        "aspect_ratio": 1,
+        "crop_size": 1,
+        "video_url": ""
     }
 
-    resp = sms_service.insert_sms_sub_account(body)
+    resp = visual_service.video_retargeting_submit_task(form)
     print(resp)
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_send_sms.py` & `volcengine-1.0.91/volcengine/example/sms/example_send_sms.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 import json
 
 from volcengine.sms.SmsService import SmsService
 from volcengine.const.Const import *
 
 if __name__ == '__main__':
     sms_service = SmsService()
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
-
     # call below method if you dont set ak and sk in $HOME/.volc/config
     sms_service.set_ak('ak')
     sms_service.set_sk('sk')
     # sms_service.set_host('host')
 
     body = {
         "SmsAccount": "smsAccount",
```

### Comparing `volcengine-1.0.90/volcengine/example/sms/example_send_vms.py` & `volcengine-1.0.91/volcengine/example/sms/example_send_vms.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import json
 
 from volcengine.sms.SmsService import SmsService
 from volcengine.const.Const import *
 
 if __name__ == '__main__':
     sms_service = SmsService()
-    # oversea
-    # sms_service = SmsService(REGION_AP_SINGAPORE1)
 
     # call below method if you dont set ak and sk in $HOME/.volc/config
     sms_service.set_ak('ak')
     sms_service.set_sk('sk')
     # sms_service.set_host('host')
 
     body = {
```

### Comparing `volcengine-1.0.90/volcengine/example/notify/example_create_tts.py` & `volcengine-1.0.91/volcengine/example/notify/example_create_tts.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/notify/example_create_task.py` & `volcengine-1.0.91/volcengine/example/notify/example_create_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/notify/examplae_sigle_batch_append.py` & `volcengine-1.0.91/volcengine/example/notify/examplae_sigle_batch_append.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_upload_image.py` & `volcengine-1.0.91/volcengine/example/imagex/example_upload_image.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_fetch_url.py` & `volcengine-1.0.91/volcengine/example/imagex/example_fetch_url.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_get_image_enhance_result_with_data.py` & `volcengine-1.0.91/volcengine/example/imagex/example_get_image_enhance_result_with_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_get_image_content_task_detail.py` & `volcengine-1.0.91/volcengine/example/imagex/example_get_image_content_task_detail.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/edge_request.py` & `volcengine-1.0.91/volcengine/example/imagex/data/edge_request.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/mirror_request_bandwidth.py` & `volcengine-1.0.91/volcengine/example/imagex/data/mirror_request_bandwidth.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/domain_bandwidth_data.py` & `volcengine-1.0.91/volcengine/example/imagex/data/domain_bandwidth_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/edge_request_traffic.py` & `volcengine-1.0.91/volcengine/example/imagex/data/edge_request_traffic.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/edge_request_region.py` & `volcengine-1.0.91/volcengine/example/imagex/data/edge_request_region.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/compress_usage.py` & `volcengine-1.0.91/volcengine/example/imagex/data/compress_usage.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/hit_rate_request_data.py` & `volcengine-1.0.91/volcengine/example/imagex/data/hit_rate_request_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/request_cnt_usage.py` & `volcengine-1.0.91/volcengine/example/imagex/data/request_cnt_usage.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/bucket_usage.py` & `volcengine-1.0.91/volcengine/example/imagex/data/bucket_usage.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/cdn_top_request_data.py` & `volcengine-1.0.91/volcengine/example/imagex/data/cdn_top_request_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/mirror_request_http_code_by_time.py` & `volcengine-1.0.91/volcengine/example/imagex/data/mirror_request_http_code_by_time.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/edge_request_bandwidth.py` & `volcengine-1.0.91/volcengine/example/imagex/data/edge_request_bandwidth.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/domain_traffic_data.py` & `volcengine-1.0.91/volcengine/example/imagex/data/domain_traffic_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/mirror_request_http_code_overview.py` & `volcengine-1.0.91/volcengine/example/imagex/data/mirror_request_http_code_overview.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/mirror_request_traffic.py` & `volcengine-1.0.91/volcengine/example/imagex/data/mirror_request_traffic.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/hit_rate_traffic_data.py` & `volcengine-1.0.91/volcengine/example/imagex/data/hit_rate_traffic_data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/data/bucket_base_op_usage.py` & `volcengine-1.0.91/volcengine/example/imagex/data/bucket_base_op_usage.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_get_image_super_resolution_result.py` & `volcengine-1.0.91/volcengine/example/imagex/example_get_image_super_resolution_result.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_get_image_bg_fill_result.py` & `volcengine-1.0.91/volcengine/example/imagex/example_get_image_bg_fill_result.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_get_image_enhance_result.py` & `volcengine-1.0.91/volcengine/example/imagex/example_get_image_enhance_result.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_get_image_style_result.py` & `volcengine-1.0.91/volcengine/example/imagex/example_get_image_style_result.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_describe_imagex_volc_cdn_access_log.py` & `volcengine-1.0.91/volcengine/example/imagex/example_describe_imagex_volc_cdn_access_log.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imagex/example_get_image_segment.py` & `volcengine-1.0.91/volcengine/example/imagex/example_get_image_segment.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imp/RetrieveJob.py` & `volcengine-1.0.91/volcengine/example/imp/RetrieveJob.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imp/SubmitJob.py` & `volcengine-1.0.91/volcengine/example/imp/SubmitJob.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/imp/KillJob.py` & `volcengine-1.0.91/volcengine/example/imp/KillJob.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/visual/example_common.py` & `volcengine-1.0.91/volcengine/example/visual/example_common.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/visual/example_ocr_demo.py` & `volcengine-1.0.91/volcengine/example/visual/example_ocr_demo.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/visual/example_product_search_search_image.py` & `volcengine-1.0.91/volcengine/example/visual/example_product_search_search_image.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/visual/example_product_search_add_image.py` & `volcengine-1.0.91/volcengine/example/visual/example_product_search_add_image.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/visual/example_video_summarization_submit_task.py` & `volcengine-1.0.91/volcengine/example/visual/example_video_summarization_submit_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/visual/example_cert_verify.py` & `volcengine-1.0.91/volcengine/example/visual/example_cert_verify.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/nlp/example_keyphrase_extraction_extract.py` & `volcengine-1.0.91/volcengine/example/nlp/example_keyphrase_extraction_extract.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/nlp/example_essay_auto_grade.py` & `volcengine-1.0.91/volcengine/example/nlp/example_essay_auto_grade.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/nlp/example_text_summarization.py` & `volcengine-1.0.91/volcengine/example/nlp/example_text_summarization.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_replay_admin/example_list_medias_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_replay_admin/example_list_medias_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_replay_admin/example_update_media_online_status_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_replay_admin/example_update_media_online_status_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_replay_admin/example_upload_replay_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_replay_admin/example_upload_replay_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_live_admin/example_list_activity_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_live_admin/example_list_activity_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_live_admin/example_create_activity_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_live_admin/example_create_activity_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_loop_video_status_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_loop_video_status_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_activity_basic_config_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_activity_basic_config_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_pull_to_push_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_pull_to_push_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_live_control/example_update_loop_video_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_live_control/example_update_loop_video_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/livesaas/example_client_sdk/example_get_sdk_token_api.py` & `volcengine-1.0.91/volcengine/example/livesaas/example_client_sdk/example_get_sdk_token_api.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_create_workflow.py` & `volcengine-1.0.91/volcengine/example/bioos/example_create_workflow.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_delete_submission.py` & `volcengine-1.0.91/volcengine/example/bioos/example_delete_submission.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_create_cluster.py` & `volcengine-1.0.91/volcengine/example/bioos/example_create_cluster.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_create_workspace.py` & `volcengine-1.0.91/volcengine/example/bioos/example_create_workspace.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_create_submission.py` & `volcengine-1.0.91/volcengine/example/bioos/example_create_submission.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_list_runs.py` & `volcengine-1.0.91/volcengine/example/bioos/example_list_runs.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_list_data_models.py` & `volcengine-1.0.91/volcengine/example/bioos/example_list_data_models.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_list_submissions.py` & `volcengine-1.0.91/volcengine/example/bioos/example_list_submissions.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_list_clusters.py` & `volcengine-1.0.91/volcengine/example/bioos/example_list_data_model_rows.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,17 @@
     bioos_service = BioOsService(endpoint='endpoint', region='region')
 
     # call below method if you don't set ak and sk in $HOME/.volc/config
     bioos_service.set_ak('ak')
     bioos_service.set_sk('sk')
 
     params = {
+        'WorkspaceID': 'workspace_id',
+        'ID': 'data_model_id',
         'PageNumber': 1,
-        'PageSize': 10,
-        'Filter': {
-            'IDs': ['test-workflow'],
-            'Status': ['Running'],
-            'Type': ['shared'],
-            'Public': True,
-        },
+        'PageSize': 0,
+        'SortBy': 'id',
+        'SortOrder': 'DESC'
     }
 
-    resp = bioos_service.list_clusters(params)
+    resp = bioos_service.list_data_model_rows(params)
     print(resp)
```

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_update_workspace.py` & `volcengine-1.0.91/volcengine/example/bioos/example_update_workspace.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_create_data_model.py` & `volcengine-1.0.91/volcengine/example/bioos/example_create_data_model.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_delete_data_model_rows_and_headers.py` & `volcengine-1.0.91/volcengine/example/bioos/example_delete_data_model_rows_and_headers.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_list_workflows.py` & `volcengine-1.0.91/volcengine/example/bioos/example_list_workflows.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_bind_cluster_to_workspace.py` & `volcengine-1.0.91/volcengine/example/bioos/example_bind_cluster_to_workspace.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_list_data_model_rows.py` & `volcengine-1.0.91/volcengine/example/bioos/example_list_tasks.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,17 +8,13 @@
     bioos_service = BioOsService(endpoint='endpoint', region='region')
 
     # call below method if you don't set ak and sk in $HOME/.volc/config
     bioos_service.set_ak('ak')
     bioos_service.set_sk('sk')
 
     params = {
-        'WorkspaceID': 'workspace_id',
-        'ID': 'data_model_id',
-        'PageNumber': 1,
-        'PageSize': 0,
-        'SortBy': 'id',
-        'SortOrder': 'DESC'
+        'RunID': 'run_id',
+        'WorkspaceID': 'workspace_id'
     }
 
-    resp = bioos_service.list_data_model_rows(params)
+    resp = bioos_service.list_tasks(params)
     print(resp)
```

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_unbind_cluster_and_workspace.py` & `volcengine-1.0.91/volcengine/example/bioos/example_unbind_cluster_and_workspace.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_delete_workflow.py` & `volcengine-1.0.91/volcengine/example/bioos/example_delete_workflow.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_cancel_submission.py` & `volcengine-1.0.91/volcengine/example/bioos/example_cancel_submission.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_cancel_run.py` & `volcengine-1.0.91/volcengine/example/bioos/example_cancel_run.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_list_clusters_of_workspace.py` & `volcengine-1.0.91/volcengine/example/bioos/example_list_clusters_of_workspace.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/bioos/example_list_tasks.py` & `volcengine-1.0.91/volcengine/example/bioos/example_update_workflow.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,13 +8,19 @@
     bioos_service = BioOsService(endpoint='endpoint', region='region')
 
     # call below method if you don't set ak and sk in $HOME/.volc/config
     bioos_service.set_ak('ak')
     bioos_service.set_sk('sk')
 
     params = {
-        'RunID': 'run_id',
-        'WorkspaceID': 'workspace_id'
+        'WorkspaceID': 'workflow_id',
+        'ID': 'workflow_id',
+        'Name': 'workflow_name',
+        'Description': 'workflow_description',
+        'Source': 'https://foo/wdl.git',
+        'Tag': 'git_tag',
+        'Token': 'git_token',
+        'MainWorkflowPath': 'hello.wdl'
     }
 
-    resp = bioos_service.list_tasks(params)
+    resp = bioos_service.update_workflow(params)
     print(resp)
```

### Comparing `volcengine-1.0.90/volcengine/example/veen/create_instance.py` & `volcengine-1.0.91/volcengine/example/veen/create_instance.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/veen/create_cloudserver.py` & `volcengine-1.0.91/volcengine/example/veen/create_cloudserver.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/veen/list_instances.py` & `volcengine-1.0.91/volcengine/example/veen/list_instances.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/veen/scale_instance_cloud_disk_capacity.py` & `volcengine-1.0.91/volcengine/example/veen/scale_instance_cloud_disk_capacity.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/veen/offline_instances.py` & `volcengine-1.0.91/volcengine/example/veen/offline_instances.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/rdspostgresql/example_create_instance.py` & `volcengine-1.0.91/volcengine/example/rdspostgresql/example_create_instance.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/tls/example_alarm.py` & `volcengine-1.0.91/volcengine/example/tls/example_alarm.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/tls/example_rule.py` & `volcengine-1.0.91/volcengine/example/tls/example_rule.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/tls/example_host_group.py` & `volcengine-1.0.91/volcengine/example/tls/example_host_group.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/tls/example_log.py` & `volcengine-1.0.91/volcengine/example/tls/example_log.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/tls/example_topic.py` & `volcengine-1.0.91/volcengine/example/tls/example_topic.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/tls/example_index.py` & `volcengine-1.0.91/volcengine/example/tls/example_index.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/tls/example_project.py` & `volcengine-1.0.91/volcengine/example/tls/example_project.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/DemoSignOnly.py` & `volcengine-1.0.91/volcengine/example/DemoSignOnly.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_select_number_and_bind_axn.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_select_number_and_bind_axn.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axne.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axne.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_query_subscription_for_list.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_query_subscription_for_list.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axb.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axb.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_upgrade_ax_to_axb.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_upgrade_ax_to_axb.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axyb.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axyb.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axn.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axn.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_bind_axb_for_axne.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_bind_axb_for_axne.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/secretnumber/example_select_number_and_bind_axb_form.py` & `volcengine-1.0.91/volcengine/example/secretnumber/example_select_number_and_bind_axb_form.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_vqs_task/example_create_v_q_score_task.py` & `volcengine-1.0.91/volcengine/example/live/example_vqs_task/example_create_v_q_score_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_generate_url/example_generate_play_u_r_l.py` & `volcengine-1.0.91/volcengine/example/live/example_generate_url/example_generate_play_u_r_l.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_audit/example_create_snapshot_audit_preset.py` & `volcengine-1.0.91/volcengine/example/live/example_audit/example_create_snapshot_audit_preset.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_index_m3u8/example_create_live_stream_record_index_file.py` & `volcengine-1.0.91/volcengine/example/live/example_index_m3u8/example_create_live_stream_record_index_file.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_usage/describe_live_batch_push_stream_metrics.py` & `volcengine-1.0.91/volcengine/example/live/example_usage/describe_live_batch_push_stream_metrics.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_usage/describe_live_batch_source_stream_metrics.py` & `volcengine-1.0.91/volcengine/example/live/example_usage/describe_live_batch_source_stream_metrics.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_describe_info/example_describe_info.py` & `volcengine-1.0.91/volcengine/example/live/example_describe_info/example_describe_info.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_relay_source/example_update_relay_source_v2.py` & `volcengine-1.0.91/volcengine/example/live/example_relay_source/example_update_relay_source_v2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_referer/example_update_referer.py` & `volcengine-1.0.91/volcengine/example/live/example_referer/example_update_referer.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_callback/example_update_callback.py` & `volcengine-1.0.91/volcengine/example/live/example_callback/example_update_callback.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_stream/example_describe_forbidden_stream_info_by_page.py` & `volcengine-1.0.91/volcengine/example/live/example_stream/example_describe_forbidden_stream_info_by_page.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_record/example_create_record_preset.py` & `volcengine-1.0.91/volcengine/example/live/example_record/example_create_record_preset.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_record/example_describe_record_task_file_history.py` & `volcengine-1.0.91/volcengine/example/live/example_record/example_describe_record_task_file_history.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_record/example_update_record_preset.py` & `volcengine-1.0.91/volcengine/example/live/example_record/example_update_record_preset.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_snapshot/example_update_snapshot_preset.py` & `volcengine-1.0.91/volcengine/example/live/example_snapshot/example_update_snapshot_preset.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_snapshot/example_create_snapshot_preset.py` & `volcengine-1.0.91/volcengine/example/live/example_snapshot/example_create_snapshot_preset.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_snapshot/example_describe_c_d_n_snapshot_history.py` & `volcengine-1.0.91/volcengine/example/live/example_snapshot/example_describe_c_d_n_snapshot_history.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_pull_to_push/example_create_pull_to_push_task.py` & `volcengine-1.0.91/volcengine/example/live/example_pull_to_push/example_create_pull_to_push_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/live/example_pull_to_push/example_update_pull_to_push_task.py` & `volcengine-1.0.91/volcengine/example/live/example_pull_to_push/example_update_pull_to_push_task.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/emr/example_list_clusters.py` & `volcengine-1.0.91/volcengine/example/emr/example_list_clusters.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/example/emr/example_list_instance_group.py` & `volcengine-1.0.91/volcengine/example/emr/example_list_instance_group.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/bioos/doc/source/conf.py` & `volcengine-1.0.91/volcengine/bioos/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/bioos/BioOsService.py` & `volcengine-1.0.91/volcengine/bioos/BioOsService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/veen/service.py` & `volcengine-1.0.91/volcengine/veen/service.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/business_security/RiskDetectionService.py` & `volcengine-1.0.91/volcengine/business_security/RiskDetectionService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/sts/StsService.py` & `volcengine-1.0.91/volcengine/sts/StsService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/rdspostgresql/rdspostgresql.py` & `volcengine-1.0.91/volcengine/rdspostgresql/rdspostgresql.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/tls/tls_responses.py` & `volcengine-1.0.91/volcengine/tls/tls_responses.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/tls/TLSService.py` & `volcengine-1.0.91/volcengine/tls/TLSService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/tls/data.py` & `volcengine-1.0.91/volcengine/tls/data.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/tls/tls_requests.py` & `volcengine-1.0.91/volcengine/tls/tls_requests.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/tls/log_pb2.py` & `volcengine-1.0.91/volcengine/tls/log_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/tls/const.py` & `volcengine-1.0.91/volcengine/tls/const.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/tls/tls_exception.py` & `volcengine-1.0.91/volcengine/tls/tls_exception.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vms/risk.py` & `volcengine-1.0.91/volcengine/vms/risk.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/vms/NumberPoolService.py` & `volcengine-1.0.91/volcengine/vms/NumberPoolService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/secretnumber/DatacenterService.py` & `volcengine-1.0.91/volcengine/secretnumber/DatacenterService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/secretnumber/SecretNumberService.py` & `volcengine-1.0.91/volcengine/secretnumber/SecretNumberService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/response/response_live_pb2.py` & `volcengine-1.0.91/volcengine/live/models/response/response_live_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/request/live_requests.py` & `volcengine-1.0.91/volcengine/live/models/request/live_requests.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/request/request_live_pb2.py` & `volcengine-1.0.91/volcengine/live/models/request/request_live_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/deny_config_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/deny_config_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/pull_to_push_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/pull_to_push_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/record_manage_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/record_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/domain_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/domain_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/relay_source_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/relay_source_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/snapshot_manage_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/snapshot_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/stream_manage_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/stream_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/index_m3u8_pb2.py` & `volcengine-1.0.91/volcengine/live/models/business/index_m3u8_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/VQScore_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/VQScore_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/models/business/addr_pb2.py` & `volcengine-1.0.91/volcengine/base/models/business/addr_pb2.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/live/LiveService.py` & `volcengine-1.0.91/volcengine/live/LiveService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/emr/EMRService.py` & `volcengine-1.0.91/volcengine/emr/EMRService.py`

 * *Files identical despite different names*

### Comparing `volcengine-1.0.90/volcengine/game_protect/GameProtectService.py` & `volcengine-1.0.91/volcengine/game_protect/GameProtectService.py`

 * *Files identical despite different names*

