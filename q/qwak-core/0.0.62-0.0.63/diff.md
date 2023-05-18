# Comparing `tmp/qwak_core-0.0.62.tar.gz` & `tmp/qwak_core-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.62.tar", max compression
+gzip compressed data, was "qwak_core-0.0.63.tar", max compression
```

## Comparing `qwak_core-0.0.62.tar` & `qwak_core-0.0.63.tar`

### file list

```diff
@@ -1,573 +1,573 @@
--rw-r--r--   0        0        0      264 2023-05-17 12:08:36.805546 qwak_core-0.0.62/README.md
--rw-r--r--   0        0        0        0 2023-05-17 12:10:24.106831 qwak_core-0.0.62/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-17 12:10:24.130831 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-17 12:10:03.882588 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.134831 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-17 12:10:24.126831 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-17 12:10:03.518584 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.126831 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-17 12:10:24.130831 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-17 12:10:03.702586 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.130831 qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-17 12:10:24.122831 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-17 12:10:02.906576 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-17 12:10:24.122831 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-17 12:10:24.122831 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-17 12:10:03.110579 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.122831 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-17 12:10:24.126831 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-17 12:10:03.334581 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.126831 qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-17 12:10:24.106831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-17 12:10:02.702574 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-17 12:10:24.110831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-17 12:10:24.110831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-17 12:10:04.066590 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.110831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-17 12:10:24.114831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-17 12:10:04.430595 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.114831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-17 12:10:24.118831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-17 12:10:04.610597 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-17 12:10:24.118831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-17 12:10:24.110831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-17 12:10:04.246592 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.114831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-17 12:10:24.118831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-17 12:10:04.794599 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.118831 qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-17 12:10:24.162831 qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-17 12:10:07.402630 qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.162831 qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-17 12:10:24.162831 qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-17 12:10:07.594633 qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-17 12:10:24.162831 qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-17 12:10:24.230832 qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-17 12:10:12.758695 qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.230832 qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-17 12:10:24.230832 qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-17 12:10:12.942697 qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-17 12:10:24.234832 qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-17 12:10:24.234832 qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-17 12:10:13.870708 qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-17 12:10:24.238832 qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-17 12:10:24.234832 qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-17 12:10:13.682706 qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.234832 qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-17 12:10:24.238832 qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-17 12:10:14.054710 qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.238832 qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-17 12:10:24.242832 qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-17 12:10:14.234712 qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-17 12:10:24.242832 qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-17 12:10:24.326833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-17 12:10:21.782803 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.326833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-17 12:10:24.322833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-17 12:10:21.410798 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.322833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-17 12:10:24.326833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-17 12:10:21.594801 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.326833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-17 12:10:24.318833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-17 12:10:21.038794 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-17 12:10:24.318833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-17 12:10:24.322833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-17 12:10:21.226796 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.322833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-17 12:10:24.334833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-17 12:10:22.330809 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.334833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-17 12:10:24.330833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-17 12:10:22.146807 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.330833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-17 12:10:24.330833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-17 12:10:21.966805 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.330833 qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-17 12:10:24.314833 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-17 12:10:20.846792 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.318833 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-17 12:10:24.310833 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-17 12:10:20.466787 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.314833 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-17 12:10:24.314833 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-17 12:10:20.662789 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-17 12:10:24.314833 qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-17 12:10:24.266833 qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-17 12:10:16.142735 qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-17 12:10:24.266833 qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-17 12:10:24.262832 qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-17 12:10:15.926733 qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.266833 qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-17 12:10:24.254832 qwak_core-0.0.62/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-17 12:10:15.554728 qwak_core-0.0.62/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.258833 qwak_core-0.0.62/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-17 12:10:24.258833 qwak_core-0.0.62/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-17 12:10:15.738731 qwak_core-0.0.62/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.258833 qwak_core-0.0.62/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-17 12:10:24.258833 qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-17 12:10:16.326737 qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-17 12:10:24.262832 qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-17 12:10:24.262832 qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-17 12:10:16.722742 qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-17 12:10:24.262832 qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-17 12:10:24.274833 qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-17 12:10:17.102747 qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.274833 qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-17 12:10:24.274833 qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-17 12:10:17.286749 qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-17 12:10:24.274833 qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-17 12:10:24.250832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-17 12:10:15.002722 qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.250832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-17 12:10:24.250832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-17 12:10:15.182724 qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-17 12:10:24.254832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-17 12:10:24.246832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-17 12:10:14.622717 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.246832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-17 12:10:24.242832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-17 12:10:14.434715 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.242832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-17 12:10:24.246832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-17 12:10:14.814719 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-17 12:10:24.246832 qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-17 12:10:24.150831 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-17 12:10:06.442619 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.150831 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-17 12:10:24.154831 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-17 12:10:06.634621 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.154831 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-17 12:10:24.154831 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-17 12:10:06.830623 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-17 12:10:24.154831 qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-17 12:10:24.210832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-17 12:10:11.662682 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.210832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-17 12:10:24.210832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-17 12:10:11.482679 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-17 12:10:24.210832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-17 12:10:24.190832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-17 12:10:09.826660 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.190832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-17 12:10:24.186832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-17 12:10:09.642657 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.186832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-17 12:10:24.178832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-17 12:10:09.074650 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.182832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-17 12:10:24.182832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-17 12:10:09.462655 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-17 12:10:24.186832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-17 12:10:24.190832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-17 12:10:10.010662 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.190832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-17 12:10:24.194832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-17 12:10:10.190664 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-17 12:10:24.194832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-17 12:10:24.182832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-17 12:10:09.266653 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.182832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-17 12:10:24.194832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-17 12:10:10.374666 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.198832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     7216 2023-05-17 12:10:24.198832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0     8200 2023-05-17 12:10:10.558668 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.198832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-17 12:10:24.214832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-17 12:10:23.662825 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.214832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-17 12:10:24.214832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-17 12:10:23.846828 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-17 12:10:24.214832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-17 12:10:24.218832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-17 12:10:12.210688 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.218832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-17 12:10:24.218832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-17 12:10:12.394690 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-17 12:10:24.218832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-17 12:10:24.222832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-17 12:10:12.574693 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.222832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-17 12:10:24.226832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-17 12:10:13.318701 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.226832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-17 12:10:24.222832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-17 12:10:13.130699 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-17 12:10:24.226832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-17 12:10:24.226832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-17 12:10:13.498704 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.230832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-17 12:10:24.198832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-17 12:10:10.742671 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.202832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-17 12:10:24.202832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-17 12:10:10.926673 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.202832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-17 12:10:24.202832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-17 12:10:11.114675 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-17 12:10:24.206832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-17 12:10:24.206832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-17 12:10:11.298677 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.206832 qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-17 12:10:24.334833 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-17 12:10:22.522812 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.334833 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-17 12:10:24.338833 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-17 12:10:22.714814 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-17 12:10:24.338833 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-17 12:10:24.338833 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-17 12:10:22.906816 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.338833 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-17 12:10:24.342834 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-17 12:10:23.102819 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-17 12:10:24.342834 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-17 12:10:24.342834 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-17 12:10:23.294821 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-17 12:10:24.346834 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-17 12:10:24.346834 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-17 12:10:23.478823 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.346834 qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-17 12:10:24.278833 qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-17 12:10:17.466751 qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.278833 qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-17 12:10:24.278833 qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-17 12:10:17.646753 qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-17 12:10:24.282833 qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-17 12:10:24.166831 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-17 12:10:08.338642 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.166831 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-17 12:10:24.170832 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-17 12:10:08.518644 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.170832 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-17 12:10:24.174831 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-17 12:10:08.702646 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-17 12:10:24.174831 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-17 12:10:24.178832 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-17 12:10:08.886648 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.178832 qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-17 12:10:24.254832 qwak_core-0.0.62/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-17 12:10:15.366726 qwak_core-0.0.62/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-17 12:10:24.254832 qwak_core-0.0.62/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-17 12:10:24.290833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-17 12:10:18.782767 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.294833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-17 12:10:24.294833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-17 12:10:18.966769 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.294833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-17 12:10:24.294833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-17 12:10:19.162772 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.298833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-17 12:10:24.298833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-17 12:10:19.350774 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.298833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-17 12:10:24.302833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-17 12:10:19.538776 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.302833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-17 12:10:24.302833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-17 12:10:19.742778 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-17 12:10:24.302833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-17 12:10:24.306833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-17 12:10:19.922781 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.306833 qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-17 12:10:24.282833 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-17 12:10:18.018758 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.286833 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-17 12:10:24.290833 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-17 12:10:18.594765 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.290833 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-17 12:10:24.286833 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-17 12:10:18.210760 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-17 12:10:24.286833 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-17 12:10:24.286833 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-17 12:10:18.406762 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.290833 qwak_core-0.0.62/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-17 12:10:24.270833 qwak_core-0.0.62/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-17 12:10:16.918745 qwak_core-0.0.62/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-17 12:10:24.270833 qwak_core-0.0.62/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-17 12:10:24.146831 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-17 12:10:07.970637 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-17 12:10:24.146831 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-17 12:10:24.142831 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-17 12:10:07.786635 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.146831 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-17 12:10:24.146831 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-17 12:10:08.158640 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-17 12:10:24.150831 qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-17 12:10:24.270833 qwak_core-0.0.62/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-17 12:10:16.518740 qwak_core-0.0.62/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-17 12:10:24.270833 qwak_core-0.0.62/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-17 12:10:24.282833 qwak_core-0.0.62/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-17 12:10:17.830756 qwak_core-0.0.62/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-17 12:10:24.282833 qwak_core-0.0.62/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-17 12:10:24.142831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-17 12:10:05.706610 qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.142831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-17 12:10:24.138831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-17 12:10:05.522608 qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-17 12:10:24.142831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-17 12:10:24.134831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-17 12:10:04.974601 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.134831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-17 12:10:24.134831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-17 12:10:05.154603 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.138831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-17 12:10:24.138831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-17 12:10:05.338605 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-17 12:10:24.138831 qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-17 12:10:24.310833 qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-17 12:10:20.286785 qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-17 12:10:24.310833 qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-17 12:10:24.306833 qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-17 12:10:20.106783 qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.310833 qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-17 12:10:24.158831 qwak_core-0.0.62/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-17 12:10:07.018626 qwak_core-0.0.62/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.158831 qwak_core-0.0.62/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-17 12:10:24.158831 qwak_core-0.0.62/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-17 12:10:07.198628 qwak_core-0.0.62/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-17 12:10:24.158831 qwak_core-0.0.62/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-17 12:10:26.426859 qwak_core-0.0.62/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-17 12:10:26.426859 qwak_core-0.0.62/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    18744 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-17 12:08:36.809546 qwak_core-0.0.62/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-17 12:08:36.813546 qwak_core-0.0.62/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.62/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.62/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-18 10:05:55.938010 qwak_core-0.0.63/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 10:07:39.918544 qwak_core-0.0.63/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-18 10:07:39.942544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-18 10:07:18.842436 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.946544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-18 10:07:39.938544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-18 10:07:18.462434 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.942544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-18 10:07:39.942544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-18 10:07:18.650435 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.942544 qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-18 10:07:39.934544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-18 10:07:17.890431 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-18 10:07:39.934544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-18 10:07:39.934544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-18 10:07:18.082432 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.938544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-18 10:07:39.938544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-18 10:07:18.270433 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.938544 qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-18 10:07:39.918544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-18 10:07:17.702430 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-18 10:07:39.922544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-18 10:07:39.922544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-18 10:07:19.030437 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.922544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-18 10:07:39.926544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-18 10:07:19.406439 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.926544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-18 10:07:39.930544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-18 10:07:19.598440 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-18 10:07:39.930544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-18 10:07:39.926544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-18 10:07:19.218438 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.926544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-18 10:07:39.930544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-18 10:07:19.786440 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.930544 qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-18 10:07:39.974544 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-18 10:07:22.458454 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.974544 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-18 10:07:39.978544 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-18 10:07:22.650455 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-18 10:07:39.978544 qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-18 10:07:40.122545 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-18 10:07:28.118483 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.122545 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-18 10:07:40.122545 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-18 10:07:28.310484 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-18 10:07:40.126545 qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-18 10:07:40.126545 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-18 10:07:29.270489 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-18 10:07:40.130545 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-18 10:07:40.126545 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-18 10:07:29.078488 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.126545 qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-18 10:07:40.130545 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-18 10:07:29.462490 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.130545 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-18 10:07:40.134545 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-18 10:07:29.650491 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-18 10:07:40.134545 qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-18 10:07:40.222545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-18 10:07:37.418531 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.222545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-18 10:07:40.214545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-18 10:07:37.030529 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.218545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-18 10:07:40.218545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-18 10:07:37.222530 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.218545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-18 10:07:40.210545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-18 10:07:36.642527 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-18 10:07:40.214545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-18 10:07:40.214545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-18 10:07:36.838528 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.214545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-18 10:07:40.226545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-18 10:07:37.978534 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.226545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-18 10:07:40.226545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-18 10:07:37.794533 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.226545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-18 10:07:40.222545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-18 10:07:37.606532 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.222545 qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-18 10:07:40.210545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-18 10:07:36.442526 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.210545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-18 10:07:40.206545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-18 10:07:36.046524 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.206545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-18 10:07:40.206545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-18 10:07:36.250525 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-18 10:07:40.210545 qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-18 10:07:40.158545 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-18 10:07:31.598501 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-18 10:07:40.158545 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-18 10:07:40.158545 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-18 10:07:31.406500 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.158545 qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-18 10:07:40.146545 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-18 10:07:31.018498 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.150545 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-18 10:07:40.150545 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-18 10:07:31.210499 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.150545 qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-18 10:07:40.150545 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-18 10:07:31.790502 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-18 10:07:40.154545 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-18 10:07:40.154545 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-18 10:07:32.206504 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-18 10:07:40.154545 qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-18 10:07:40.166545 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-18 10:07:32.598506 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.166545 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-18 10:07:40.166545 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-18 10:07:32.786507 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-18 10:07:40.170545 qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-18 10:07:40.142545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-18 10:07:30.438495 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.142545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-18 10:07:40.142545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-18 10:07:30.634496 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-18 10:07:40.146545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-18 10:07:40.138545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-18 10:07:30.050493 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.138545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-18 10:07:40.134545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-18 10:07:29.858492 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.134545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-18 10:07:40.138545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-18 10:07:30.250494 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-18 10:07:40.138545 qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-18 10:07:39.962544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-18 10:07:21.502449 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.966544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-18 10:07:39.966544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-18 10:07:21.694450 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.966544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-18 10:07:39.966544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-18 10:07:21.886451 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-18 10:07:39.970544 qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-18 10:07:40.102545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-18 10:07:26.966477 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.102545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-18 10:07:40.098545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-18 10:07:26.774476 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-18 10:07:40.102545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-18 10:07:40.078545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-18 10:07:25.038468 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.082545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-18 10:07:40.078545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-18 10:07:24.842466 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.078545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-18 10:07:40.070545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-18 10:07:24.246463 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.070545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-18 10:07:40.074545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-18 10:07:24.650466 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-18 10:07:40.074545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-18 10:07:40.082545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-18 10:07:25.230469 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.082545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-18 10:07:40.082545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-18 10:07:25.422469 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-18 10:07:40.086545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25222 2023-05-18 10:07:40.074545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37429 2023-05-18 10:07:24.446464 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.074545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-18 10:07:40.086545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-18 10:07:25.610470 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.086545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     7216 2023-05-18 10:07:40.086545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0     8200 2023-05-18 10:07:25.802471 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.090545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-18 10:07:40.102545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-18 10:07:39.342541 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.106545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-18 10:07:40.106545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-18 10:07:39.566542 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-18 10:07:40.106545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-18 10:07:40.106545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-18 10:07:27.538480 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.110545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-18 10:07:40.110545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-18 10:07:27.734481 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-18 10:07:40.110545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-18 10:07:40.114545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-18 10:07:27.926482 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.114545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-18 10:07:40.118545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-18 10:07:28.698486 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.118545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-18 10:07:40.114545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-18 10:07:28.502485 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-18 10:07:40.114545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-18 10:07:40.118545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-18 10:07:28.886487 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.122545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-18 10:07:40.090545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-18 10:07:25.998473 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.090545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-18 10:07:40.094545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-18 10:07:26.190473 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.094545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-18 10:07:40.094545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-18 10:07:26.386474 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-18 10:07:40.094545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-18 10:07:40.098545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-18 10:07:26.582476 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.098545 qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-18 10:07:40.230545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-18 10:07:38.170535 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.230545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-18 10:07:40.230545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-18 10:07:38.354536 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-18 10:07:40.230545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-18 10:07:40.234546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-18 10:07:38.542537 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.234546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-18 10:07:40.234546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-18 10:07:38.742538 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-18 10:07:40.238546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-18 10:07:40.238546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-18 10:07:38.942539 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-18 10:07:40.238546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-18 10:07:40.238546 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-18 10:07:39.130540 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.242545 qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-18 10:07:40.170545 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-18 10:07:32.970508 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.170545 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-18 10:07:40.174545 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-18 10:07:33.158509 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-18 10:07:40.174545 qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-18 10:07:39.994544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-18 10:07:23.478459 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.002544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-18 10:07:40.014544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-18 10:07:23.670461 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.026544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-18 10:07:40.038545 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-18 10:07:23.858461 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-18 10:07:40.050545 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-18 10:07:40.058544 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-18 10:07:24.050462 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.070545 qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-18 10:07:40.146545 qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-18 10:07:30.826497 qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-18 10:07:40.146545 qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-18 10:07:40.186545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-18 10:07:34.294515 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.186545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-18 10:07:40.186545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-18 10:07:34.486516 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.190545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-18 10:07:40.190545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-18 10:07:34.678517 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.190545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-18 10:07:40.190545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-18 10:07:34.870518 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.194545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-18 10:07:40.194545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-18 10:07:35.070519 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.194545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-18 10:07:40.198545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-18 10:07:35.282520 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-18 10:07:40.198545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-18 10:07:40.198545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-18 10:07:35.474521 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.198545 qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-18 10:07:40.178545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-18 10:07:33.534511 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.178545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-18 10:07:40.182545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-18 10:07:34.106514 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.182545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-18 10:07:40.178545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-18 10:07:33.722512 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-18 10:07:40.178545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-18 10:07:40.182545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-18 10:07:33.918513 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.182545 qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-18 10:07:40.162545 qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-18 10:07:32.410505 qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-18 10:07:40.166545 qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-18 10:07:39.958544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-18 10:07:23.094457 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-18 10:07:39.962544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-18 10:07:39.958544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-18 10:07:22.862456 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.958544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-18 10:07:39.962544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-18 10:07:23.290459 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-18 10:07:39.962544 qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-18 10:07:40.162545 qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-18 10:07:31.994503 qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-18 10:07:40.162545 qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-18 10:07:40.174545 qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-18 10:07:33.346510 qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-18 10:07:40.174545 qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-18 10:07:39.954544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-18 10:07:20.734445 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.954544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-18 10:07:39.954544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-18 10:07:20.542445 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-18 10:07:39.954544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-18 10:07:39.946544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-18 10:07:19.978442 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.946544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-18 10:07:39.950544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-18 10:07:20.166442 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.950544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-18 10:07:39.950544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-18 10:07:20.354443 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-18 10:07:39.950544 qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-18 10:07:40.202545 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-18 10:07:35.858523 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-18 10:07:40.202545 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-18 10:07:40.202545 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-18 10:07:35.666522 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:40.202545 qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-18 10:07:39.970544 qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15881 2023-05-18 10:07:22.078452 qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.970544 qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-18 10:07:39.974544 qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-18 10:07:22.266453 qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-18 10:07:39.974544 qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-18 10:07:45.046570 qwak_core-0.0.63/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-18 10:07:45.046570 qwak_core-0.0.63/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    18744 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-18 10:05:55.942010 qwak_core-0.0.63/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-18 10:05:55.946010 qwak_core-0.0.63/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.63/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.63/PKG-INFO
```

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.63/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/pyproject.toml` & `qwak_core-0.0.63/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.62"
+version = "0.0.63"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.62/qwak/automations/__init__.py` & `qwak_core-0.0.63/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/automations/automation_executions.py` & `qwak_core-0.0.63/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/automations/automations.py` & `qwak_core-0.0.63/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.63/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.63/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/automations/common.py` & `qwak_core-0.0.63/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.63/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.63/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.63/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.63/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.63/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/alert_management/client.py` & `qwak_core-0.0.63/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/analytics/client.py` & `qwak_core-0.0.63/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/audience/client.py` & `qwak_core-0.0.63/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/automation_management/client.py` & `qwak_core-0.0.63/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.63/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.63/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.63/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.63/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/build_management/client.py` & `qwak_core-0.0.63/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.63/qwak/clients/build_orchestrator/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,14 @@
                         no_cache=not build_conf.build_env.docker.cache,
                         env_vars=build_conf.build_env.docker.env_vars,
                     ),
                     python_env=PythonEnv(
                         git_credentials=build_conf.build_properties.model_uri.git_credentials,
                         git_credentials_secret=build_conf.build_properties.model_uri.git_credentials_secret,
                         qwak_sdk_version=sdk_version,
-                        qwak_sdk_extra_index=build_conf.build_env.python_env.qwak_sdk_extra_index_url,
                     ),
                 ),
                 verbose=verbose,
                 build_code_path=build_code_path,
                 build_config=json.dumps(
                     yaml.load(build_conf.to_yaml(), Loader=Loader)  # nosec B506
                 ),
```

### Comparing `qwak_core-0.0.62/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.63/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/deployment/client.py` & `qwak_core-0.0.63/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.63/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.63/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.63/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.63/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.63/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/logging_client/client.py` & `qwak_core-0.0.63/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/model_management/client.py` & `qwak_core-0.0.63/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/project/client.py` & `qwak_core-0.0.63/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/secret_service/client.py` & `qwak_core-0.0.63/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.63/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.63/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.63/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.63/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.63/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.63/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.63/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.63/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.63/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.63/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.63/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.63/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.63/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.63/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.63/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/offline/client.py` & `qwak_core-0.0.63/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/feature_store/online/client.py` & `qwak_core-0.0.63/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/const.py` & `qwak_core-0.0.63/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.63/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.63/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.63/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.63/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/singleton_meta.py` & `qwak_core-0.0.63/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/tool/auth.py` & `qwak_core-0.0.63/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.63/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.63/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.63/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/adapters/__init__.py` & `qwak_core-0.0.63/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.63/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.63/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.63/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.63/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.63/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/base.py` & `qwak_core-0.0.63/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/decorators/api.py` & `qwak_core-0.0.63/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.63/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/experiment_tracking.py` & `qwak_core-0.0.63/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/schema.py` & `qwak_core-0.0.63/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/schema_entities.py` & `qwak_core-0.0.63/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.63/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.63/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.63/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.63/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.63/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.63/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.63/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.63/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/qwak_client/client.py` & `qwak_core-0.0.63/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.63/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/qwak_client/models/model.py` & `qwak_core-0.0.63/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.63/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.63/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/tools/logger/logger.py` & `qwak_core-0.0.63/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak/tools/logger/logging.yml` & `qwak_core-0.0.63/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.63/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/qwak_services_mock/services_mock.py` & `qwak_core-0.0.63/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.62/setup.py` & `qwak_core-0.0.63/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.62',
+    'version': '0.0.63',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.62/PKG-INFO` & `qwak_core-0.0.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.62
+Version: 0.0.63
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

