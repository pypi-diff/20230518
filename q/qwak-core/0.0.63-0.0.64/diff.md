# Comparing `tmp/qwak_core-0.0.63.tar.gz` & `tmp/qwak_core-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.63.tar", max compression
+gzip compressed data, was "qwak_core-0.0.64.tar", max compression
```

## Comparing `qwak_core-0.0.63.tar` & `qwak_core-0.0.64.tar`

### file list

```diff
@@ -1,573 +1,573 @@
--rw-r--r--   0        0        0      264 2023-05-18 10:05:55.938010 qwak_core-0.0.63/README.md
--rw-r--r--   0        0        0        0 2023-05-18 10:07:39.918544 qwak_core-0.0.63/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-18 10:07:39.942544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-18 10:07:18.842436 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.946544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-18 10:07:39.938544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-18 10:07:18.462434 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.942544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-18 10:07:39.942544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-18 10:07:18.650435 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.942544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-18 10:07:39.934544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-18 10:07:17.890431 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-18 10:07:39.934544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-18 10:07:39.934544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-18 10:07:18.082432 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.938544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-18 10:07:39.938544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-18 10:07:18.270433 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.938544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-18 10:07:39.918544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-18 10:07:17.702430 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-18 10:07:39.922544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-18 10:07:39.922544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-18 10:07:19.030437 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.922544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-18 10:07:39.926544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-18 10:07:19.406439 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.926544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-18 10:07:39.930544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-18 10:07:19.598440 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-18 10:07:39.930544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-18 10:07:39.926544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-18 10:07:19.218438 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.926544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-18 10:07:39.930544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-18 10:07:19.786440 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.930544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-18 10:07:39.974544 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-18 10:07:22.458454 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.974544 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-18 10:07:39.978544 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-18 10:07:22.650455 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-18 10:07:39.978544 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-18 10:07:40.122545 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-18 10:07:28.118483 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.122545 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-18 10:07:40.122545 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-18 10:07:28.310484 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-18 10:07:40.126545 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-18 10:07:40.126545 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-18 10:07:29.270489 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-18 10:07:40.130545 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-18 10:07:40.126545 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-18 10:07:29.078488 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.126545 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-18 10:07:40.130545 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-18 10:07:29.462490 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.130545 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-18 10:07:40.134545 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-18 10:07:29.650491 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-18 10:07:40.134545 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-18 10:07:40.222545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-18 10:07:37.418531 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.222545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-18 10:07:40.214545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-18 10:07:37.030529 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.218545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-18 10:07:40.218545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-18 10:07:37.222530 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.218545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-18 10:07:40.210545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-18 10:07:36.642527 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-18 10:07:40.214545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-18 10:07:40.214545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-18 10:07:36.838528 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.214545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-18 10:07:40.226545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-18 10:07:37.978534 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.226545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-18 10:07:40.226545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-18 10:07:37.794533 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.226545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-18 10:07:40.222545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-18 10:07:37.606532 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.222545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-18 10:07:40.210545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-18 10:07:36.442526 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.210545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-18 10:07:40.206545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-18 10:07:36.046524 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.206545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-18 10:07:40.206545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-18 10:07:36.250525 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-18 10:07:40.210545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-18 10:07:40.158545 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-18 10:07:31.598501 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-18 10:07:40.158545 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-18 10:07:40.158545 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-18 10:07:31.406500 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.158545 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-18 10:07:40.146545 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-18 10:07:31.018498 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.150545 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-18 10:07:40.150545 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-18 10:07:31.210499 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.150545 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-18 10:07:40.150545 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-18 10:07:31.790502 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-18 10:07:40.154545 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-18 10:07:40.154545 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-18 10:07:32.206504 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-18 10:07:40.154545 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-18 10:07:40.166545 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-18 10:07:32.598506 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.166545 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-18 10:07:40.166545 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-18 10:07:32.786507 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-18 10:07:40.170545 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-18 10:07:40.142545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-18 10:07:30.438495 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.142545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-18 10:07:40.142545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-18 10:07:30.634496 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-18 10:07:40.146545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-18 10:07:40.138545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-18 10:07:30.050493 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.138545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-18 10:07:40.134545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-18 10:07:29.858492 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.134545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-18 10:07:40.138545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-18 10:07:30.250494 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-18 10:07:40.138545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-18 10:07:39.962544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-18 10:07:21.502449 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.966544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-18 10:07:39.966544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-18 10:07:21.694450 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.966544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-18 10:07:39.966544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-18 10:07:21.886451 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-18 10:07:39.970544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-18 10:07:40.102545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-18 10:07:26.966477 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.102545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-18 10:07:40.098545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-18 10:07:26.774476 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-18 10:07:40.102545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-18 10:07:40.078545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-18 10:07:25.038468 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.082545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-18 10:07:40.078545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-18 10:07:24.842466 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.078545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-18 10:07:40.070545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-18 10:07:24.246463 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.070545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-18 10:07:40.074545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-18 10:07:24.650466 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-18 10:07:40.074545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-18 10:07:40.082545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-18 10:07:25.230469 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.082545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-18 10:07:40.082545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-18 10:07:25.422469 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-18 10:07:40.086545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-18 10:07:40.074545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-18 10:07:24.446464 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.074545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-18 10:07:40.086545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-18 10:07:25.610470 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.086545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     7216 2023-05-18 10:07:40.086545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0     8200 2023-05-18 10:07:25.802471 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.090545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-18 10:07:40.102545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-18 10:07:39.342541 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.106545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-18 10:07:40.106545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-18 10:07:39.566542 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-18 10:07:40.106545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-18 10:07:40.106545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-18 10:07:27.538480 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.110545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-18 10:07:40.110545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-18 10:07:27.734481 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-18 10:07:40.110545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-18 10:07:40.114545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-18 10:07:27.926482 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.114545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-18 10:07:40.118545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-18 10:07:28.698486 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.118545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-18 10:07:40.114545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-18 10:07:28.502485 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-18 10:07:40.114545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-18 10:07:40.118545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-18 10:07:28.886487 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.122545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-18 10:07:40.090545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-18 10:07:25.998473 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.090545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-18 10:07:40.094545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-18 10:07:26.190473 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.094545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-18 10:07:40.094545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-18 10:07:26.386474 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-18 10:07:40.094545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-18 10:07:40.098545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-18 10:07:26.582476 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.098545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-18 10:07:40.230545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-18 10:07:38.170535 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.230545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-18 10:07:40.230545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-18 10:07:38.354536 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-18 10:07:40.230545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-18 10:07:40.234546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-18 10:07:38.542537 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.234546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-18 10:07:40.234546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-18 10:07:38.742538 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-18 10:07:40.238546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-18 10:07:40.238546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-18 10:07:38.942539 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-18 10:07:40.238546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-18 10:07:40.238546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-18 10:07:39.130540 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.242545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-18 10:07:40.170545 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-18 10:07:32.970508 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.170545 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-18 10:07:40.174545 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-18 10:07:33.158509 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-18 10:07:40.174545 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-18 10:07:39.994544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-18 10:07:23.478459 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.002544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-18 10:07:40.014544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-18 10:07:23.670461 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.026544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-18 10:07:40.038545 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-18 10:07:23.858461 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-18 10:07:40.050545 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-18 10:07:40.058544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-18 10:07:24.050462 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.070545 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-18 10:07:40.146545 qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-18 10:07:30.826497 qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-18 10:07:40.146545 qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-18 10:07:40.186545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-18 10:07:34.294515 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.186545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-18 10:07:40.186545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-18 10:07:34.486516 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.190545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-18 10:07:40.190545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-18 10:07:34.678517 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.190545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-18 10:07:40.190545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-18 10:07:34.870518 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.194545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-18 10:07:40.194545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-18 10:07:35.070519 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.194545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-18 10:07:40.198545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-18 10:07:35.282520 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-18 10:07:40.198545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-18 10:07:40.198545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-18 10:07:35.474521 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.198545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-18 10:07:40.178545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-18 10:07:33.534511 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.178545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-18 10:07:40.182545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-18 10:07:34.106514 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.182545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-18 10:07:40.178545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-18 10:07:33.722512 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-18 10:07:40.178545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-18 10:07:40.182545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-18 10:07:33.918513 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.182545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-18 10:07:40.162545 qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-18 10:07:32.410505 qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-18 10:07:40.166545 qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-18 10:07:39.958544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-18 10:07:23.094457 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-18 10:07:39.962544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-18 10:07:39.958544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-18 10:07:22.862456 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.958544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-18 10:07:39.962544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-18 10:07:23.290459 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-18 10:07:39.962544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-18 10:07:40.162545 qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-18 10:07:31.994503 qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-18 10:07:40.162545 qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-18 10:07:40.174545 qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-18 10:07:33.346510 qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-18 10:07:40.174545 qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-18 10:07:39.954544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-18 10:07:20.734445 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.954544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-18 10:07:39.954544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-18 10:07:20.542445 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-18 10:07:39.954544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-18 10:07:39.946544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-18 10:07:19.978442 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.946544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-18 10:07:39.950544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-18 10:07:20.166442 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.950544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-18 10:07:39.950544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-18 10:07:20.354443 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-18 10:07:39.950544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-18 10:07:40.202545 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-18 10:07:35.858523 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-18 10:07:40.202545 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-18 10:07:40.202545 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-18 10:07:35.666522 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:40.202545 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-18 10:07:39.970544 qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-18 10:07:22.078452 qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.970544 qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-18 10:07:39.974544 qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-18 10:07:22.266453 qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 10:07:39.974544 qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-18 10:07:45.046570 qwak_core-0.0.63/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-18 10:07:45.046570 qwak_core-0.0.63/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    18744 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.63/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.63/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-18 11:16:11.358401 qwak_core-0.0.64/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 11:17:57.911086 qwak_core-0.0.64/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-18 11:17:57.935086 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-18 11:17:35.586946 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.939086 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-18 11:17:57.931086 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-18 11:17:35.186945 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.935086 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-18 11:17:57.935086 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-18 11:17:35.386946 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.935086 qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-18 11:17:57.927086 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-18 11:17:34.574943 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-18 11:17:57.927086 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-18 11:17:57.927086 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-18 11:17:34.794944 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.927086 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-18 11:17:57.931086 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-18 11:17:34.990944 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.931086 qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-18 11:17:57.911086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-18 11:17:34.378943 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-18 11:17:57.915086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-18 11:17:57.915086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-18 11:17:35.790947 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.915086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-18 11:17:57.919086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-18 11:17:36.206948 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.919086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-18 11:17:57.923086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-18 11:17:36.426948 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-18 11:17:57.923086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-18 11:17:57.915086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-18 11:17:35.994947 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.919086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-18 11:17:57.923086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-18 11:17:36.626949 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.923086 qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-18 11:17:57.975086 qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-18 11:17:39.390964 qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.979086 qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-18 11:17:57.979086 qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-18 11:17:39.578966 qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-18 11:17:57.979086 qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-18 11:17:58.123087 qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-18 11:17:45.319003 qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.123087 qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-18 11:17:58.123087 qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-18 11:17:45.539005 qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-18 11:17:58.127087 qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-18 11:17:58.127087 qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-18 11:17:46.559012 qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-18 11:17:58.131087 qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-18 11:17:58.127087 qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-18 11:17:46.359010 qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.127087 qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-18 11:17:58.131087 qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-18 11:17:46.759013 qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.131087 qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-18 11:17:58.135087 qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-18 11:17:46.955014 qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-18 11:17:58.135087 qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-18 11:17:58.227088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-18 11:17:55.259068 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.227088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-18 11:17:58.223088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-18 11:17:54.847066 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.223088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-18 11:17:58.223088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-18 11:17:55.047067 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.227088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-18 11:17:58.219088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-18 11:17:54.443063 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-18 11:17:58.219088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-18 11:17:58.219088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-18 11:17:54.647064 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.223088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-18 11:17:58.231088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-18 11:17:55.871072 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.235088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-18 11:17:58.231088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-18 11:17:55.651071 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.231088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-18 11:17:58.227088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-18 11:17:55.455070 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.231088 qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-18 11:17:58.215088 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-18 11:17:54.235062 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.215088 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-18 11:17:58.211088 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-18 11:17:53.799059 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.211088 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-18 11:17:58.215088 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-18 11:17:54.019060 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-18 11:17:58.215088 qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-18 11:17:58.159087 qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-18 11:17:49.003028 qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-18 11:17:58.159087 qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-18 11:17:58.159087 qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-18 11:17:48.799026 qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.159087 qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-18 11:17:58.147087 qwak_core-0.0.64/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-18 11:17:48.399024 qwak_core-0.0.64/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.151087 qwak_core-0.0.64/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-18 11:17:58.151087 qwak_core-0.0.64/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-18 11:17:48.595025 qwak_core-0.0.64/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.151087 qwak_core-0.0.64/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-18 11:17:58.151087 qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-18 11:17:49.211029 qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-18 11:17:58.155087 qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-18 11:17:58.155087 qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-18 11:17:49.635032 qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-18 11:17:58.155087 qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-18 11:17:58.167087 qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-18 11:17:50.043034 qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.167087 qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-18 11:17:58.171087 qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-18 11:17:50.255036 qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-18 11:17:58.171087 qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-18 11:17:58.143087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-18 11:17:47.791020 qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.143087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-18 11:17:58.143087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-18 11:17:47.999021 qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-18 11:17:58.147087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-18 11:17:58.139087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-18 11:17:47.367017 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.139087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-18 11:17:58.135087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-18 11:17:47.163015 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.135087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-18 11:17:58.139087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-18 11:17:47.583018 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-18 11:17:58.139087 qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-18 11:17:57.955086 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-18 11:17:38.418958 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.959086 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-18 11:17:57.959086 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-18 11:17:38.630960 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.959086 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-18 11:17:57.959086 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-18 11:17:38.826961 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-18 11:17:57.963086 qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-18 11:17:58.103087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-18 11:17:44.034995 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.103087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-18 11:17:58.099087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-18 11:17:43.826994 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-18 11:17:58.103087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-18 11:17:58.079087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-18 11:17:42.010982 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.083087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-18 11:17:58.079087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-18 11:17:41.810980 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.079087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-18 11:17:58.067087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-18 11:17:41.194976 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.071087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-18 11:17:58.075087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-18 11:17:41.614979 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-18 11:17:58.075087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-18 11:17:58.083087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-18 11:17:42.210983 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.083087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-18 11:17:58.087087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-18 11:17:42.414984 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-18 11:17:58.087087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25222 2023-05-18 11:17:58.071087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37429 2023-05-18 11:17:41.402978 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.071087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-18 11:17:58.087087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-18 11:17:42.618986 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.087087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     7284 2023-05-18 11:17:58.091087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0     8518 2023-05-18 11:17:42.818987 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.091087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-18 11:17:58.107087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-18 11:17:57.283082 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.107087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-18 11:17:58.107087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-18 11:17:57.495083 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-18 11:17:58.107087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-18 11:17:58.111087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-18 11:17:44.650999 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.111087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-18 11:17:58.111087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-18 11:17:44.855000 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-18 11:17:58.111087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-18 11:17:58.115087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-18 11:17:45.087002 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.115087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-18 11:17:58.119087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-18 11:17:45.959008 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.119087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-18 11:17:58.115087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-18 11:17:45.743006 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-18 11:17:58.119087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-18 11:17:58.119087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-18 11:17:46.155009 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.123087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-18 11:17:58.091087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-18 11:17:43.022988 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.095087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-18 11:17:58.095087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-18 11:17:43.222990 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.095087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-18 11:17:58.095087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-18 11:17:43.418991 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-18 11:17:58.099087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-18 11:17:58.099087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-18 11:17:43.622992 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.099087 qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-18 11:17:58.235088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-18 11:17:56.063073 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.235088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-18 11:17:58.239088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-18 11:17:56.259075 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-18 11:17:58.239088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-18 11:17:58.239088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-18 11:17:56.463076 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.239088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-18 11:17:58.243088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-18 11:17:56.663077 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-18 11:17:58.243088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-18 11:17:58.243088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-18 11:17:56.863079 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-18 11:17:58.243088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-18 11:17:58.247088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-18 11:17:57.059080 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.247088 qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-18 11:17:58.175087 qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-18 11:17:50.455037 qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.175087 qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-18 11:17:58.175087 qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-18 11:17:50.655038 qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-18 11:17:58.179087 qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-18 11:17:57.983086 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-18 11:17:40.394971 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.003086 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-18 11:17:58.011086 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-18 11:17:40.578972 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.023086 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-18 11:17:58.035086 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-18 11:17:40.790974 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-18 11:17:58.047087 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-18 11:17:58.055086 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-18 11:17:40.986975 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.067087 qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-18 11:17:58.147087 qwak_core-0.0.64/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-18 11:17:48.199022 qwak_core-0.0.64/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-18 11:17:58.147087 qwak_core-0.0.64/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-18 11:17:58.191087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-18 11:17:51.911047 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.191087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-18 11:17:58.195088 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-18 11:17:52.111048 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.195088 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-18 11:17:58.195088 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-18 11:17:52.343049 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.195088 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-18 11:17:58.199087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-18 11:17:52.567051 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.199087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-18 11:17:58.199087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-18 11:17:52.779052 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.199087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-18 11:17:58.203087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-18 11:17:53.003054 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-18 11:17:58.203087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-18 11:17:58.203087 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-18 11:17:53.199055 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.207088 qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-18 11:17:58.183087 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-18 11:17:51.103041 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.183087 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-18 11:17:58.187087 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-18 11:17:51.719045 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.191087 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-18 11:17:58.183087 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-18 11:17:51.323043 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-18 11:17:58.187087 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-18 11:17:58.187087 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-18 11:17:51.519044 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.187087 qwak_core-0.0.64/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-18 11:17:58.163087 qwak_core-0.0.64/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-18 11:17:49.855033 qwak_core-0.0.64/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-18 11:17:58.167087 qwak_core-0.0.64/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-18 11:17:57.951086 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-18 11:17:40.002968 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-18 11:17:57.955086 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-18 11:17:57.951086 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-18 11:17:39.786967 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.951086 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-18 11:17:57.955086 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-18 11:17:40.202970 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-18 11:17:57.955086 qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-18 11:17:58.163087 qwak_core-0.0.64/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-18 11:17:49.419030 qwak_core-0.0.64/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-18 11:17:58.163087 qwak_core-0.0.64/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-18 11:17:58.179087 qwak_core-0.0.64/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-18 11:17:50.887040 qwak_core-0.0.64/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-18 11:17:58.179087 qwak_core-0.0.64/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-18 11:17:57.947086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-18 11:17:37.622953 qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.947086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-18 11:17:57.947086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-18 11:17:37.422952 qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-18 11:17:57.947086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-18 11:17:57.939086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-18 11:17:36.842949 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.939086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-18 11:17:57.939086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-18 11:17:37.042950 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.943086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-18 11:17:57.943086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-18 11:17:37.234951 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-18 11:17:57.943086 qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-18 11:17:58.207088 qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-18 11:17:53.599058 qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-18 11:17:58.211088 qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-18 11:17:58.207088 qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-18 11:17:53.395056 qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:58.207088 qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-18 11:17:57.963086 qwak_core-0.0.64/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15881 2023-05-18 11:17:39.014962 qwak_core-0.0.64/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.963086 qwak_core-0.0.64/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-18 11:17:57.967086 qwak_core-0.0.64/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-18 11:17:39.198963 qwak_core-0.0.64/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 11:17:57.975086 qwak_core-0.0.64/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-18 11:17:59.419095 qwak_core-0.0.64/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-18 11:17:59.419095 qwak_core-0.0.64/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    18744 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.358401 qwak_core-0.0.64/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.362401 qwak_core-0.0.64/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-18 11:16:11.366401 qwak_core-0.0.64/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.64/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.64/PKG-INFO
```

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.feature_store.features import execution_pb2 as qwak_dot_feature__store_dot_features_dot_execution__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=qwak/feature_store/features/real_time_feature_extractor.proto\x12\x1bqwak.feature.store.features\x1a+qwak/feature_store/features/execution.proto\"\x97\x02\n\x18RealTimeFeatureExtractor\x12K\n\x12real_time_artifact\x18\x01 \x01(\x0b\x32/.qwak.feature.store.features.ExtractionArtifact\x12P\n\x12\x64\x65pendency_manager\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.features.PythonDependencyManager\x12\\\n\x1c\x63lient_pod_compute_resources\x18\x03 \x01(\x0b\x32\x36.qwak.feature.store.features.ExtractorComputeResources\"U\n\x12\x45xtractionArtifact\x12\x34\n\x06\x61ws_s3\x18\x01 \x01(\x0b\x32\".qwak.feature.store.features.AwsS3H\x00\x42\t\n\x07\x66s_type\"\x1e\n\x05\x41wsS3\x12\x15\n\rartifact_path\x18\x01 \x01(\t\"\x98\x02\n\x17PythonDependencyManager\x12\x42\n\x0epython_version\x18\x01 \x01(\x0e\x32*.qwak.feature.store.features.PythonVersion\x12\x45\n\nvirtualenv\x18\x02 \x01(\x0b\x32/.qwak.feature.store.features.VirtualEnvironmentH\x00\x12\x33\n\x05\x63onda\x18\x03 \x01(\x0b\x32\".qwak.feature.store.features.CondaH\x00\x12\x35\n\x06poetry\x18\x04 \x01(\x0b\x32#.qwak.feature.store.features.PoetryH\x00\x42\x06\n\x04type\"#\n\x05\x43onda\x12\x1a\n\x12\x65ncoded_conda_file\x18\x01 \x01(\t\"#\n\x06Poetry\x12\x19\n\x11\x65ncoded_lock_file\x18\x01 \x01(\t\"6\n\x12VirtualEnvironment\x12 \n\x18\x65ncoded_requirements_txt\x18\x01 \x01(\t\"\x85\x01\n\x19\x45xtractorComputeResources\x12[\n\x19\x63ompute_resource_template\x18\x01 \x01(\x0e\x32\x36.qwak.feature.store.features.execution.ClusterTemplateH\x00\x42\x0b\n\tresources*s\n\rPythonVersion\x12\x1a\n\x16PYTHON_VERSION_INVALID\x10\x00\x12\x16\n\x12PYTHON_VERSION_3_7\x10\x01\x12\x16\n\x12PYTHON_VERSION_3_8\x10\x02\x12\x16\n\x12PYTHON_VERSION_3_9\x10\x03\x42[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=qwak/feature_store/features/real_time_feature_extractor.proto\x12\x1bqwak.feature.store.features\x1a+qwak/feature_store/features/execution.proto\"\x97\x02\n\x18RealTimeFeatureExtractor\x12K\n\x12real_time_artifact\x18\x01 \x01(\x0b\x32/.qwak.feature.store.features.ExtractionArtifact\x12P\n\x12\x64\x65pendency_manager\x18\x02 \x01(\x0b\x32\x34.qwak.feature.store.features.PythonDependencyManager\x12\\\n\x1c\x63lient_pod_compute_resources\x18\x03 \x01(\x0b\x32\x36.qwak.feature.store.features.ExtractorComputeResources\"U\n\x12\x45xtractionArtifact\x12\x34\n\x06\x61ws_s3\x18\x01 \x01(\x0b\x32\".qwak.feature.store.features.AwsS3H\x00\x42\t\n\x07\x66s_type\"\x1e\n\x05\x41wsS3\x12\x15\n\rartifact_path\x18\x01 \x01(\t\"\x98\x02\n\x17PythonDependencyManager\x12\x42\n\x0epython_version\x18\x01 \x01(\x0e\x32*.qwak.feature.store.features.PythonVersion\x12\x45\n\nvirtualenv\x18\x02 \x01(\x0b\x32/.qwak.feature.store.features.VirtualEnvironmentH\x00\x12\x33\n\x05\x63onda\x18\x03 \x01(\x0b\x32\".qwak.feature.store.features.CondaH\x00\x12\x35\n\x06poetry\x18\x04 \x01(\x0b\x32#.qwak.feature.store.features.PoetryH\x00\x42\x06\n\x04type\"*\n\x05\x43onda\x12!\n\x19\x62\x61se64_encoded_conda_file\x18\x01 \x01(\t\"*\n\x06Poetry\x12 \n\x18\x62\x61se64_encoded_lock_file\x18\x01 \x01(\t\"=\n\x12VirtualEnvironment\x12\'\n\x1f\x62\x61se64_encoded_requirements_txt\x18\x01 \x01(\t\"\x9a\x01\n\x19\x45xtractorComputeResources\x12[\n\x19\x63ompute_resource_template\x18\x01 \x01(\x0e\x32\x36.qwak.feature.store.features.execution.ClusterTemplateH\x00\x12\x13\n\x0bparallelism\x18\x02 \x01(\x05\x42\x0b\n\tresources*s\n\rPythonVersion\x12\x1a\n\x16PYTHON_VERSION_INVALID\x10\x00\x12\x16\n\x12PYTHON_VERSION_3_7\x10\x01\x12\x16\n\x12PYTHON_VERSION_3_8\x10\x02\x12\x16\n\x12PYTHON_VERSION_3_9\x10\x03\x42[\n&com.qwak.ai.feature.store.features.apiP\x01Z/qwak/featurestore/features;featurestorefeaturesb\x06proto3')
 
 _PYTHONVERSION = DESCRIPTOR.enum_types_by_name['PythonVersion']
 PythonVersion = enum_type_wrapper.EnumTypeWrapper(_PYTHONVERSION)
 PYTHON_VERSION_INVALID = 0
 PYTHON_VERSION_3_7 = 1
 PYTHON_VERSION_3_8 = 2
 PYTHON_VERSION_3_9 = 3
@@ -90,26 +90,26 @@
   })
 _sym_db.RegisterMessage(ExtractorComputeResources)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n&com.qwak.ai.feature.store.features.apiP\001Z/qwak/featurestore/features;featurestorefeatures'
-  _PYTHONVERSION._serialized_start=1089
-  _PYTHONVERSION._serialized_end=1204
+  _PYTHONVERSION._serialized_start=1131
+  _PYTHONVERSION._serialized_end=1246
   _REALTIMEFEATUREEXTRACTOR._serialized_start=140
   _REALTIMEFEATUREEXTRACTOR._serialized_end=419
   _EXTRACTIONARTIFACT._serialized_start=421
   _EXTRACTIONARTIFACT._serialized_end=506
   _AWSS3._serialized_start=508
   _AWSS3._serialized_end=538
   _PYTHONDEPENDENCYMANAGER._serialized_start=541
   _PYTHONDEPENDENCYMANAGER._serialized_end=821
   _CONDA._serialized_start=823
-  _CONDA._serialized_end=858
-  _POETRY._serialized_start=860
-  _POETRY._serialized_end=895
-  _VIRTUALENVIRONMENT._serialized_start=897
-  _VIRTUALENVIRONMENT._serialized_end=951
-  _EXTRACTORCOMPUTERESOURCES._serialized_start=954
-  _EXTRACTORCOMPUTERESOURCES._serialized_end=1087
+  _CONDA._serialized_end=865
+  _POETRY._serialized_start=867
+  _POETRY._serialized_end=909
+  _VIRTUALENVIRONMENT._serialized_start=911
+  _VIRTUALENVIRONMENT._serialized_end=972
+  _EXTRACTORCOMPUTERESOURCES._serialized_start=975
+  _EXTRACTORCOMPUTERESOURCES._serialized_end=1129
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -127,64 +127,68 @@
     def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["virtualenv", "conda", "poetry"] | None: ...
 
 global___PythonDependencyManager = PythonDependencyManager
 
 class Conda(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ENCODED_CONDA_FILE_FIELD_NUMBER: builtins.int
-    encoded_conda_file: builtins.str
-    """Encoded contents of a conda file"""
+    BASE64_ENCODED_CONDA_FILE_FIELD_NUMBER: builtins.int
+    base64_encoded_conda_file: builtins.str
+    """Base64 utf-8 encoded contents of a conda file"""
     def __init__(
         self,
         *,
-        encoded_conda_file: builtins.str = ...,
+        base64_encoded_conda_file: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["encoded_conda_file", b"encoded_conda_file"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["base64_encoded_conda_file", b"base64_encoded_conda_file"]) -> None: ...
 
 global___Conda = Conda
 
 class Poetry(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ENCODED_LOCK_FILE_FIELD_NUMBER: builtins.int
-    encoded_lock_file: builtins.str
-    """Encoded contents of a poetry lock file"""
+    BASE64_ENCODED_LOCK_FILE_FIELD_NUMBER: builtins.int
+    base64_encoded_lock_file: builtins.str
+    """Base64 utf-8 encoded contents of a poetry lock file"""
     def __init__(
         self,
         *,
-        encoded_lock_file: builtins.str = ...,
+        base64_encoded_lock_file: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["encoded_lock_file", b"encoded_lock_file"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["base64_encoded_lock_file", b"base64_encoded_lock_file"]) -> None: ...
 
 global___Poetry = Poetry
 
 class VirtualEnvironment(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ENCODED_REQUIREMENTS_TXT_FIELD_NUMBER: builtins.int
-    encoded_requirements_txt: builtins.str
-    """Encoded contents of a requirements file"""
+    BASE64_ENCODED_REQUIREMENTS_TXT_FIELD_NUMBER: builtins.int
+    base64_encoded_requirements_txt: builtins.str
+    """Base64 utf-8 encoded contents of a requirements file,"""
     def __init__(
         self,
         *,
-        encoded_requirements_txt: builtins.str = ...,
+        base64_encoded_requirements_txt: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["encoded_requirements_txt", b"encoded_requirements_txt"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["base64_encoded_requirements_txt", b"base64_encoded_requirements_txt"]) -> None: ...
 
 global___VirtualEnvironment = VirtualEnvironment
 
 class ExtractorComputeResources(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COMPUTE_RESOURCE_TEMPLATE_FIELD_NUMBER: builtins.int
+    PARALLELISM_FIELD_NUMBER: builtins.int
     compute_resource_template: qwak.feature_store.features.execution_pb2.ClusterTemplate.ValueType
+    parallelism: builtins.int
+    """Webserver workers"""
     def __init__(
         self,
         *,
         compute_resource_template: qwak.feature_store.features.execution_pb2.ClusterTemplate.ValueType = ...,
+        parallelism: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["compute_resource_template", b"compute_resource_template", "resources", b"resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["compute_resource_template", b"compute_resource_template", "resources", b"resources"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["compute_resource_template", b"compute_resource_template", "parallelism", b"parallelism", "resources", b"resources"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["resources", b"resources"]) -> typing_extensions.Literal["compute_resource_template"] | None: ...
 
 global___ExtractorComputeResources = ExtractorComputeResources
```

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.64/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.64/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/pyproject.toml` & `qwak_core-0.0.64/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.63"
+version = "0.0.64"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.63/qwak/automations/__init__.py` & `qwak_core-0.0.64/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/automations/automation_executions.py` & `qwak_core-0.0.64/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/automations/automations.py` & `qwak_core-0.0.64/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.64/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.64/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/automations/common.py` & `qwak_core-0.0.64/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.64/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.64/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.64/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.64/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.64/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/alert_management/client.py` & `qwak_core-0.0.64/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/analytics/client.py` & `qwak_core-0.0.64/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/audience/client.py` & `qwak_core-0.0.64/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/automation_management/client.py` & `qwak_core-0.0.64/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.64/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.64/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.64/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.64/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/build_management/client.py` & `qwak_core-0.0.64/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.64/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.64/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/deployment/client.py` & `qwak_core-0.0.64/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.64/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.64/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.64/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.64/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.64/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/logging_client/client.py` & `qwak_core-0.0.64/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/model_management/client.py` & `qwak_core-0.0.64/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/project/client.py` & `qwak_core-0.0.64/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/secret_service/client.py` & `qwak_core-0.0.64/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.64/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.64/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.64/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.64/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.64/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.64/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.64/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.64/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.64/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.64/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.64/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.64/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.64/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.64/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.64/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/offline/client.py` & `qwak_core-0.0.64/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/feature_store/online/client.py` & `qwak_core-0.0.64/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/const.py` & `qwak_core-0.0.64/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.64/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.64/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.64/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.64/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/singleton_meta.py` & `qwak_core-0.0.64/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/tool/auth.py` & `qwak_core-0.0.64/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.64/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.64/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.64/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.64/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/adapters/__init__.py` & `qwak_core-0.0.64/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.64/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.64/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.64/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.64/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.64/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/base.py` & `qwak_core-0.0.64/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/decorators/api.py` & `qwak_core-0.0.64/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.64/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/experiment_tracking.py` & `qwak_core-0.0.64/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/schema.py` & `qwak_core-0.0.64/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/schema_entities.py` & `qwak_core-0.0.64/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.64/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.64/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.64/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.64/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.64/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.64/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.64/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.64/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/qwak_client/client.py` & `qwak_core-0.0.64/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.64/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/qwak_client/models/model.py` & `qwak_core-0.0.64/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.64/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.64/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/tools/logger/logger.py` & `qwak_core-0.0.64/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak/tools/logger/logging.yml` & `qwak_core-0.0.64/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.64/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/qwak_services_mock/services_mock.py` & `qwak_core-0.0.64/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.63/setup.py` & `qwak_core-0.0.64/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.63',
+    'version': '0.0.64',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.63/PKG-INFO` & `qwak_core-0.0.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.63
+Version: 0.0.64
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

