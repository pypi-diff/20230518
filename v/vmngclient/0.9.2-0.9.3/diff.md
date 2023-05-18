# Comparing `tmp/vmngclient-0.9.2.tar.gz` & `tmp/vmngclient-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmngclient-0.9.2.tar", max compression
+gzip compressed data, was "vmngclient-0.9.3.tar", max compression
```

## Comparing `vmngclient-0.9.2.tar` & `vmngclient-0.9.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0     3612 2023-05-16 12:58:27.914339 vmngclient-0.9.2/README.md
--rw-r--r--   0        0        0      827 2023-05-16 12:58:27.914339 vmngclient-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2259 2023-05-16 12:58:27.914339 vmngclient-0.9.2/vmngclient/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 12:58:27.914339 vmngclient-0.9.2/vmngclient/api/__init__.py
--rw-r--r--   0        0        0     6090 2023-05-16 12:58:27.914339 vmngclient-0.9.2/vmngclient/api/admin_tech_api.py
--rw-r--r--   0        0        0     8709 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/administration.py
--rw-r--r--   0        0        0     6253 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/alarms_api.py
--rw-r--r--   0        0        0     1919 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/api_containter.py
--rw-r--r--   0        0        0    11322 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/basic_api.py
--rw-r--r--   0        0        0     7051 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/dashboard_api.py
--rw-r--r--   0        0        0     6508 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/device_action_api.py
--rw-r--r--   0        0        0     1651 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/logs_api.py
--rw-r--r--   0        0        0     5971 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4040 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/omp_api.py
--rw-r--r--   0        0        0     5631 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/packet_capture_api.py
--rw-r--r--   0        0        0     4945 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/partition_manager_api.py
--rw-r--r--   0        0        0     2041 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/resource_pool_api.py
--rw-r--r--   0        0        0     7330 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/software_action_api.py
--rw-r--r--   0        0        0     5412 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/speedtest_api.py
--rw-r--r--   0        0        0     8577 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/task_status_api.py
--rw-r--r--   0        0        0    24650 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/template_api.py
--rw-r--r--   0        0        0     3194 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/README.md
--rw-r--r--   0        0        0     1476 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/__init__.py
--rw-r--r--   0        0        0     7232 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/cli_template.py
--rw-r--r--   0        0        0     2093 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      476 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0     1306 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/feature_template.py
--rw-r--r--   0        0        0     3101 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      599 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     2425 2023-05-16 12:58:27.918340 vmngclient-0.9.2/vmngclient/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0     1159 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      656 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     2199 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0      476 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_system/cisco_system_model.py
--rw-r--r--   0        0        0     6752 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2
--rw-r--r--   0        0        0     2465 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4529 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2123 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      627 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     2745 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py
--rw-r--r--   0        0        0     8179 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2
--rw-r--r--   0        0        0     9926 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2
--rw-r--r--   0        0        0     7057 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1730 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     1119 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/tenant_api.py
--rw-r--r--   0        0        0     4953 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0    10790 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/api/versions_utils.py
--rw-r--r--   0        0        0    20283 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/dataclasses.py
--rw-r--r--   0        0        0     2974 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/exceptions.py
--rw-r--r--   0        0        0      672 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/logging.conf
--rw-r--r--   0        0        0     5727 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/primitives/__init__.py
--rw-r--r--   0        0        0     2299 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/primitives/client.py
--rw-r--r--   0        0        0      780 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/primitives/primitive_container.py
--rw-r--r--   0        0        0      832 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/primitives/tenant_backup_restore.py
--rw-r--r--   0        0        0     6568 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/primitives/tenant_management.py
--rw-r--r--   0        0        0      669 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/primitives/tenant_migration.py
--rw-r--r--   0        0        0     6987 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/response.py
--rw-r--r--   0        0        0    14290 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/session.py
--rw-r--r--   0        0        0     7877 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    11881 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_administration.py
--rw-r--r--   0        0        0    11034 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8053 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_cli_template.py
--rw-r--r--   0        0        0     4460 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3878 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_device_action_api.py
--rw-r--r--   0        0        0    25969 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_devices_api.py
--rw-r--r--   0        0        0      836 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1485 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_logs_api.py
--rw-r--r--   0        0        0    10911 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16398 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_omp_api.py
--rw-r--r--   0        0        0     5153 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_packet_capture.py
--rw-r--r--   0        0        0     4967 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7454 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_primitives.py
--rw-r--r--   0        0        0     5724 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_response.py
--rw-r--r--   0        0        0     4753 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_session.py
--rw-r--r--   0        0        0     3774 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6005 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_speed_test_api.py
--rw-r--r--   0        0        0     3862 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_task_status_api.py
--rw-r--r--   0        0        0     8686 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_templates.py
--rw-r--r--   0        0        0     3625 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     8432 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_typed_list.py
--rw-r--r--   0        0        0     5170 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_version_utils.py
--rw-r--r--   0        0        0     3132 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     7341 2023-05-16 12:58:27.922340 vmngclient-0.9.2/vmngclient/typed_list.py
--rw-r--r--   0        0        0        0 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/__init__.py
--rw-r--r--   0        0        0      190 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/alarm_status.py
--rw-r--r--   0        0        0      196 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/certificate_status.py
--rw-r--r--   0        0        0       97 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/config_status.py
--rw-r--r--   0        0        0     4677 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/creation_tools.py
--rw-r--r--   0        0        0     7219 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/dashboard.py
--rw-r--r--   0        0        0     2369 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/device_model.py
--rw-r--r--   0        0        0      472 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/operation_status.py
--rw-r--r--   0        0        0      139 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/personality.py
--rw-r--r--   0        0        0      115 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/reachability.py
--rw-r--r--   0        0        0      278 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/session_type.py
--rw-r--r--   0        0        0       92 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/template_type.py
--rw-r--r--   0        0        0     1944 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/upgrades_helper.py
--rw-r--r--   0        0        0      102 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/utils/validate_status.py
--rw-r--r--   0        0        0     5302 2023-05-16 12:58:27.926340 vmngclient-0.9.2/vmngclient/vmanage_auth.py
--rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 vmngclient-0.9.2/setup.py
--rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 vmngclient-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     3612 2023-05-18 08:05:34.916999 vmngclient-0.9.3/README.md
+-rw-r--r--   0        0        0      827 2023-05-18 08:05:34.916999 vmngclient-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2259 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/__init__.py
+-rw-r--r--   0        0        0     6090 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/admin_tech_api.py
+-rw-r--r--   0        0        0     8709 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/administration.py
+-rw-r--r--   0        0        0     6253 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/alarms_api.py
+-rw-r--r--   0        0        0     1919 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/api_containter.py
+-rw-r--r--   0        0        0    11322 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/basic_api.py
+-rw-r--r--   0        0        0     7051 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/dashboard_api.py
+-rw-r--r--   0        0        0     6508 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/device_action_api.py
+-rw-r--r--   0        0        0     1651 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/logs_api.py
+-rw-r--r--   0        0        0     5971 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4040 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/omp_api.py
+-rw-r--r--   0        0        0     5631 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/packet_capture_api.py
+-rw-r--r--   0        0        0     4945 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/partition_manager_api.py
+-rw-r--r--   0        0        0     2041 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/resource_pool_api.py
+-rw-r--r--   0        0        0     7330 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/software_action_api.py
+-rw-r--r--   0        0        0     5412 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/speedtest_api.py
+-rw-r--r--   0        0        0     8577 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/task_status_api.py
+-rw-r--r--   0        0        0    24704 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/template_api.py
+-rw-r--r--   0        0        0     3194 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/README.md
+-rw-r--r--   0        0        0     1476 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/__init__.py
+-rw-r--r--   0        0        0     7232 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/cli_template.py
+-rw-r--r--   0        0        0     2093 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      476 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0     1306 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/feature_template.py
+-rw-r--r--   0        0        0     3101 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      599 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     2430 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0     1159 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      656 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     2199 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0      476 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_system/cisco_system_model.py
+-rw-r--r--   0        0        0     6752 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2
+-rw-r--r--   0        0        0     2465 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4529 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2123 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      627 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     2745 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py
+-rw-r--r--   0        0        0     8179 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2
+-rw-r--r--   0        0        0     9926 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2
+-rw-r--r--   0        0        0     7057 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1730 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     1119 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/tenant_api.py
+-rw-r--r--   0        0        0     4953 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0    10808 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/versions_utils.py
+-rw-r--r--   0        0        0    20283 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/dataclasses.py
+-rw-r--r--   0        0        0     2974 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/exceptions.py
+-rw-r--r--   0        0        0      672 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/logging.conf
+-rw-r--r--   0        0        0     5727 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/__init__.py
+-rw-r--r--   0        0        0     2299 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/client.py
+-rw-r--r--   0        0        0      780 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/primitive_container.py
+-rw-r--r--   0        0        0      832 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/tenant_backup_restore.py
+-rw-r--r--   0        0        0     6568 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/tenant_management.py
+-rw-r--r--   0        0        0      669 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/tenant_migration.py
+-rw-r--r--   0        0        0     6987 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/response.py
+-rw-r--r--   0        0        0    14290 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/session.py
+-rw-r--r--   0        0        0     7877 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    11881 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_administration.py
+-rw-r--r--   0        0        0    11034 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8053 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_cli_template.py
+-rw-r--r--   0        0        0     4460 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3878 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    25969 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_devices_api.py
+-rw-r--r--   0        0        0      836 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1485 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_logs_api.py
+-rw-r--r--   0        0        0    10911 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16398 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5153 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     4967 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7454 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_primitives.py
+-rw-r--r--   0        0        0     5724 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_response.py
+-rw-r--r--   0        0        0     4753 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_session.py
+-rw-r--r--   0        0        0     3774 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6005 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0     3862 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_task_status_api.py
+-rw-r--r--   0        0        0     8686 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_templates.py
+-rw-r--r--   0        0        0     3625 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     8432 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_typed_list.py
+-rw-r--r--   0        0        0     5170 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3132 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     7341 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/typed_list.py
+-rw-r--r--   0        0        0        0 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/alarm_status.py
+-rw-r--r--   0        0        0      196 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/certificate_status.py
+-rw-r--r--   0        0        0       97 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/config_status.py
+-rw-r--r--   0        0        0     4677 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/creation_tools.py
+-rw-r--r--   0        0        0     7219 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/dashboard.py
+-rw-r--r--   0        0        0     2369 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/device_model.py
+-rw-r--r--   0        0        0      472 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/operation_status.py
+-rw-r--r--   0        0        0      139 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/personality.py
+-rw-r--r--   0        0        0      115 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/reachability.py
+-rw-r--r--   0        0        0      278 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/session_type.py
+-rw-r--r--   0        0        0       92 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/template_type.py
+-rw-r--r--   0        0        0     1944 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      102 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/validate_status.py
+-rw-r--r--   0        0        0     5302 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/vmanage_auth.py
+-rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 vmngclient-0.9.3/setup.py
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 vmngclient-0.9.3/PKG-INFO
```

### Comparing `vmngclient-0.9.2/README.md` & `vmngclient-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/pyproject.toml` & `vmngclient-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vmngclient"
-version = "0.9.2"
+version = "0.9.3"
 description = "Universal vManage API"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/CiscoDevNet/vManage-client"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `vmngclient-0.9.2/vmngclient/__init__.py` & `vmngclient-0.9.3/vmngclient/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/admin_tech_api.py` & `vmngclient-0.9.3/vmngclient/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/administration.py` & `vmngclient-0.9.3/vmngclient/api/administration.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/alarms_api.py` & `vmngclient-0.9.3/vmngclient/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/api_containter.py` & `vmngclient-0.9.3/vmngclient/api/api_containter.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/basic_api.py` & `vmngclient-0.9.3/vmngclient/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/dashboard_api.py` & `vmngclient-0.9.3/vmngclient/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/device_action_api.py` & `vmngclient-0.9.3/vmngclient/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/logs_api.py` & `vmngclient-0.9.3/vmngclient/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/mtt_aaa_api.py` & `vmngclient-0.9.3/vmngclient/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/omp_api.py` & `vmngclient-0.9.3/vmngclient/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/packet_capture_api.py` & `vmngclient-0.9.3/vmngclient/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/partition_manager_api.py` & `vmngclient-0.9.3/vmngclient/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/resource_pool_api.py` & `vmngclient-0.9.3/vmngclient/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/software_action_api.py` & `vmngclient-0.9.3/vmngclient/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/speedtest_api.py` & `vmngclient-0.9.3/vmngclient/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/task_status_api.py` & `vmngclient-0.9.3/vmngclient/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/template_api.py` & `vmngclient-0.9.3/vmngclient/api/template_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         else:
             payload = json.loads(template.generate_payload(self.session))
 
         response = self.session.put(f"/dataservice/template/feature/{data.id}", json=payload)
         return response
 
     @overload
-    def create(self, template: FeatureTemplate) -> str:
+    def create(self, template: FeatureTemplate, debug=False) -> str:
         ...
 
     @overload
     def create(self, template: DeviceTemplate) -> str:
         ...
 
     @overload
@@ -488,15 +488,15 @@
     def generate_feature_template_payload(
         self, template: FeatureTemplate, schema: Any, debug: bool = False
     ) -> FeatureTemplatePayload:
         payload = FeatureTemplatePayload(
             name=template.name,
             description=template.description,
             template_type=template.type,
-            device_types=["omp-vsmart"],  # TODO
+            device_types=[device_model.value for device_model in template.device_models],
             definition={},
         )  # type: ignore
 
         fr_template_fields = [FeatureTemplateField(**field) for field in schema["fields"]]  # TODO
         payload.definition.update(get_path_dict([field.dataPath for field in fr_template_fields]))
 
         for field in fr_template_fields:
```

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/README.md` & `vmngclient-0.9.3/vmngclient/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/__init__.py` & `vmngclient-0.9.3/vmngclient/api/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/cli_template.py` & `vmngclient-0.9.3/vmngclient/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/device_template/device_template.py` & `vmngclient-0.9.3/vmngclient/api/templates/device_template/device_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/feature_template.py` & `vmngclient-0.9.3/vmngclient/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/feature_template_field.py` & `vmngclient-0.9.3/vmngclient/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/feature_template_payload.py` & `vmngclient-0.9.3/vmngclient/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/models/cisco_aaa_model.py` & `vmngclient-0.9.3/vmngclient/api/templates/models/cisco_aaa_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     group_name: str = Field(alias="group-name")
     vpn: Optional[int]
     source_interface: Optional[str] = Field(alias="source-interface")
     server: List[RadiusServer] = []
 
 
-class DomainStripping(Enum):
+class DomainStripping(str, Enum):
     YES = "yes"
     NO = "no"
     RIGHT_TO_LEFT = "right-to-left"
 
 
 class TacacsServer(BaseModel):
     class Config:
```

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/models/omp_vsmart_model.py` & `vmngclient-0.9.3/vmngclient/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/models/security_vsmart_model.py` & `vmngclient-0.9.3/vmngclient/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/aaa_model.py` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/aaa/feature/user.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/tenant/tenant.json.j2` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/templates/payloads/tenant/tenant_model.py` & `vmngclient-0.9.3/vmngclient/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/tenant_api.py` & `vmngclient-0.9.3/vmngclient/api/tenant_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/tenant_backup_restore_api.py` & `vmngclient-0.9.3/vmngclient/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/api/versions_utils.py` & `vmngclient-0.9.3/vmngclient/api/versions_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from pathlib import PurePath
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
-from attr import define, field  # type: ignore
+from attr import Factory, define, field  # type: ignore
 from clint.textui.progress import Bar as ProgressBar  # type: ignore
 from requests_toolbelt.multipart.encoder import MultipartEncoder, MultipartEncoderMonitor  # type: ignore
 
 from vmngclient.dataclasses import DataclassBase, Device
 from vmngclient.exceptions import ImageNotInRepositoryError
 from vmngclient.typed_list import DataSequence
 from vmngclient.utils.creation_tools import FIELD_NAME, create_dataclass
@@ -18,15 +18,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 @define
 class DeviceSoftwareRepository(DataclassBase):
     installed_versions: List[str] = field(default=None)
-    available_versions: List[str] = field(default=None, metadata={FIELD_NAME: "availableVersions"})
+    available_versions: List[str] = field(default=Factory(list), metadata={FIELD_NAME: "availableVersions"})
     current_version: str = field(default=None, metadata={FIELD_NAME: "version"})
     default_version: str = field(default=None, metadata={FIELD_NAME: "defaultVersion"})
     device_id: str = field(default=None, metadata={FIELD_NAME: "uuid"})
 
 
 @define
 class DeviceVersionPayload(DataclassBase):
```

### Comparing `vmngclient-0.9.2/vmngclient/dataclasses.py` & `vmngclient-0.9.3/vmngclient/dataclasses.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/exceptions.py` & `vmngclient-0.9.3/vmngclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/logging.conf` & `vmngclient-0.9.3/vmngclient/logging.conf`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/primitives/__init__.py` & `vmngclient-0.9.3/vmngclient/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/primitives/client.py` & `vmngclient-0.9.3/vmngclient/primitives/client.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/primitives/primitive_container.py` & `vmngclient-0.9.3/vmngclient/primitives/primitive_container.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/primitives/tenant_backup_restore.py` & `vmngclient-0.9.3/vmngclient/primitives/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/primitives/tenant_management.py` & `vmngclient-0.9.3/vmngclient/primitives/tenant_management.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/primitives/tenant_migration.py` & `vmngclient-0.9.3/vmngclient/primitives/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/response.py` & `vmngclient-0.9.3/vmngclient/response.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/session.py` & `vmngclient-0.9.3/vmngclient/session.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_admin_tech_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_administration.py` & `vmngclient-0.9.3/vmngclient/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_alarms_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_cli_template.py` & `vmngclient-0.9.3/vmngclient/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_creation_tools.py` & `vmngclient-0.9.3/vmngclient/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_device_action_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_devices_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_feature_template_field.py` & `vmngclient-0.9.3/vmngclient/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_logs_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_mtt_aaa_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_omp_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_packet_capture.py` & `vmngclient-0.9.3/vmngclient/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_partition_manager_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_primitives.py` & `vmngclient-0.9.3/vmngclient/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_response.py` & `vmngclient-0.9.3/vmngclient/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_session.py` & `vmngclient-0.9.3/vmngclient/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_software_action_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_speed_test_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_task_status_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_templates.py` & `vmngclient-0.9.3/vmngclient/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_tenant_backup_restore_api.py` & `vmngclient-0.9.3/vmngclient/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_typed_list.py` & `vmngclient-0.9.3/vmngclient/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_version_utils.py` & `vmngclient-0.9.3/vmngclient/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/tests/test_vmanage_auth.py` & `vmngclient-0.9.3/vmngclient/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/typed_list.py` & `vmngclient-0.9.3/vmngclient/typed_list.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/utils/creation_tools.py` & `vmngclient-0.9.3/vmngclient/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/utils/dashboard.py` & `vmngclient-0.9.3/vmngclient/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/utils/device_model.py` & `vmngclient-0.9.3/vmngclient/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/utils/upgrades_helper.py` & `vmngclient-0.9.3/vmngclient/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/vmngclient/vmanage_auth.py` & `vmngclient-0.9.3/vmngclient/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.2/setup.py` & `vmngclient-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'requests-toolbelt>=0.10.1,<0.11.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'vmngclient',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Universal vManage API',
     'long_description': '# vManage-client\n[![Python3.8](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8)](https://www.python.org/)\n\nvManage client is a package for creating simple and parallel automatic requests via official vManageAPI. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any vManage.\n\n## Installation\n```console\npip install vmngclient\n```\n\n## Session usage example\nOur session is an extension to `requests.Session` designed to make it easier to communicate via API calls with vManage. We provide ready to use authenticetion, you have to simply provide the vmanage url, username and password as as if you were doing it through a GUI. \n```python\nfrom vmngclient.session import create_vManageSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\nsession = create_vManageSession(url=url, username=username, password=password)\n\nsession.get("/dataservice/device")\n```\n\n## API usage examples\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\nvsmarts = session.api.devices.get().filter(personality = Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(software_image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices = vsmarts,\n    image= image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\n\n```python\nalarms = session.api.alarms.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>User operations</b> <i>(click to expand)</i></summary>\n\n```python\nfrom vmngclient.api.administration import User, UsersAPI\n\n# Get all users\nall_users = UsersAPI(session).get_all_users()\n\n# Create a user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nstatus = UsersAPI(session).create_user(new_user)\n\n# Delete a user\nstatus = UsersAPI(session).delete_user(username="new_user")\n```\n\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `VMNGCLIENT_DEVEL` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n\tsession.api.users.delete_user("XYZ")\nexcept vManageBadRequestError as error:\n\t# Process an error.\n\tlogger.error(error.info.details)\n\n# message = \'Delete users request failed\' \n# details = \'No user with name XYZ was found\' \n# code = \'USER0006\'\n```\n\n## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CiscoDevNet/vManage-client',
```

### Comparing `vmngclient-0.9.2/PKG-INFO` & `vmngclient-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmngclient
-Version: 0.9.2
+Version: 0.9.3
 Summary: Universal vManage API
 Home-page: https://github.com/CiscoDevNet/vManage-client
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

