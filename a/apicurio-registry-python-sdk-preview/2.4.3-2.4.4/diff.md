# Comparing `tmp/apicurio_registry_python_sdk_preview-2.4.3.tar.gz` & `tmp/apicurio_registry_python_sdk_preview-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicurio_registry_python_sdk_preview-2.4.3.tar", max compression
+gzip compressed data, was "apicurio_registry_python_sdk_preview-2.4.4.tar", max compression
```

## Comparing `apicurio_registry_python_sdk_preview-2.4.3.tar` & `apicurio_registry_python_sdk_preview-2.4.4.tar`

### file list

```diff
@@ -1,86 +1,97 @@
--rw-r--r--   0        0        0      368 2023-05-17 11:57:07.580710 apicurio_registry_python_sdk_preview-2.4.3/README.md
--rw-r--r--   0        0        0     2224 2023-05-17 11:57:07.580853 apicurio_registry_python_sdk_preview-2.4.3/kiota-gen.py
--rw-r--r--   0        0        0     1133 2023-05-17 11:59:12.179901 apicurio_registry_python_sdk_preview-2.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 11:57:07.581617 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/__init__.py
--rw-r--r--   0        0        0     6316 2023-05-17 11:58:03.965323 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/admin_request_builder.py
--rw-r--r--   0        0        0     4141 2023-05-17 11:58:03.988283 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/artifact_types/artifact_types_request_builder.py
--rw-r--r--   0        0        0     2509 2023-05-17 11:58:03.969731 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/config_request_builder.py
--rw-r--r--   0        0        0     9895 2023-05-17 11:58:03.973749 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/properties/item/with_property_name_item_request_builder.py
--rw-r--r--   0        0        0     4230 2023-05-17 11:58:03.971418 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/properties/properties_request_builder.py
--rw-r--r--   0        0        0     4497 2023-05-17 11:58:03.991072 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/export/export_request_builder.py
--rw-r--r--   0        0        0     4016 2023-05-17 11:58:03.989723 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/import_/import_request_builder.py
--rw-r--r--   0        0        0     9210 2023-05-17 11:58:03.986822 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/loggers/item/with_logger_item_request_builder.py
--rw-r--r--   0        0        0     3970 2023-05-17 11:58:03.984865 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/loggers/loggers_request_builder.py
--rw-r--r--   0        0        0     9490 2023-05-17 11:58:03.983360 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/role_mappings/item/with_principal_item_request_builder.py
--rw-r--r--   0        0        0     6823 2023-05-17 11:58:03.975845 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/role_mappings/role_mappings_request_builder.py
--rw-r--r--   0        0        0     9847 2023-05-17 11:58:03.968546 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/rules/item/with_rule_item_request_builder.py
--rw-r--r--   0        0        0     9029 2023-05-17 11:58:03.966798 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/rules/rules_request_builder.py
--rw-r--r--   0        0        0     7675 2023-05-17 11:58:03.895749 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/groups_request_builder.py
--rw-r--r--   0        0        0    17933 2023-05-17 11:58:03.893278 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/artifacts_request_builder.py
--rw-r--r--   0        0        0    12567 2023-05-17 11:58:03.886788 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/meta/meta_request_builder.py
--rw-r--r--   0        0        0     6977 2023-05-17 11:58:03.878777 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/owner/owner_request_builder.py
--rw-r--r--   0        0        0    11150 2023-05-17 11:58:03.890714 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py
--rw-r--r--   0        0        0    10297 2023-05-17 11:58:03.889210 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/rules/rules_request_builder.py
--rw-r--r--   0        0        0     4942 2023-05-17 11:58:03.887760 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/state/state_request_builder.py
--rw-r--r--   0        0        0     6104 2023-05-17 11:58:03.891646 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/test/test_request_builder.py
--rw-r--r--   0        0        0    10548 2023-05-17 11:58:03.881391 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py
--rw-r--r--   0        0        0     6008 2023-05-17 11:58:03.879938 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4767 2023-05-17 11:58:03.883765 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py
--rw-r--r--   0        0        0    10171 2023-05-17 11:58:03.882732 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py
--rw-r--r--   0        0        0     9632 2023-05-17 11:58:03.885032 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/versions_request_builder.py
--rw-r--r--   0        0        0    16487 2023-05-17 11:58:03.877530 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py
--rw-r--r--   0        0        0     7662 2023-05-17 11:58:03.894579 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/with_group_item_request_builder.py
--rw-r--r--   0        0        0     1299 2023-05-17 11:58:03.961423 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/content_hashes_request_builder.py
--rw-r--r--   0        0        0     4122 2023-05-17 11:58:03.960005 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4828 2023-05-17 11:58:03.960895 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py
--rw-r--r--   0        0        0     1287 2023-05-17 11:58:03.957929 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/content_ids_request_builder.py
--rw-r--r--   0        0        0     4108 2023-05-17 11:58:03.956443 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4820 2023-05-17 11:58:03.957362 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/item/with_content_item_request_builder.py
--rw-r--r--   0        0        0     1283 2023-05-17 11:58:03.962038 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/global_ids_request_builder.py
--rw-r--r--   0        0        0     4807 2023-05-17 11:58:03.963054 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/item/references/references_request_builder.py
--rw-r--r--   0        0        0     5362 2023-05-17 11:58:03.964005 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/item/with_global_item_request_builder.py
--rw-r--r--   0        0        0     4913 2023-05-17 11:58:03.958932 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/ids_request_builder.py
--rw-r--r--   0        0        0     1160 2023-05-17 11:58:04.053648 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/kiota-lock.json
--rw-r--r--   0        0        0     4573 2023-05-17 11:58:03.943710 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_content.py
--rw-r--r--   0        0        0    15041 2023-05-17 11:58:03.908896 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_meta_data.py
--rw-r--r--   0        0        0     3253 2023-05-17 11:58:03.939926 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_owner.py
--rw-r--r--   0        0        0     5461 2023-05-17 11:58:03.903898 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_reference.py
--rw-r--r--   0        0        0     4781 2023-05-17 11:58:03.950660 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_search_results.py
--rw-r--r--   0        0        0      134 2023-05-17 11:58:03.918704 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_state.py
--rw-r--r--   0        0        0     3192 2023-05-17 11:58:03.919539 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_type_info.py
--rw-r--r--   0        0        0     5921 2023-05-17 11:58:03.953433 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/configuration_property.py
--rw-r--r--   0        0        0     4961 2023-05-17 11:58:03.905804 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/create_group_meta_data.py
--rw-r--r--   0        0        0     3989 2023-05-17 11:58:03.912876 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/download_ref.py
--rw-r--r--   0        0        0     5719 2023-05-17 11:58:03.928803 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/editable_meta_data.py
--rw-r--r--   0        0        0     5777 2023-05-17 11:58:03.945068 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/error.py
--rw-r--r--   0        0        0     8023 2023-05-17 11:58:03.948338 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/group_meta_data.py
--rw-r--r--   0        0        0     4661 2023-05-17 11:58:03.902712 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/group_search_results.py
--rw-r--r--   0        0        0    14563 2023-05-17 11:58:03.923761 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/limits.py
--rw-r--r--   0        0        0     2597 2023-05-17 11:58:03.933727 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/log_configuration.py
--rw-r--r--   0        0        0      281 2023-05-17 11:58:03.919936 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/log_level.py
--rw-r--r--   0        0        0     3217 2023-05-17 11:58:03.913704 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/named_log_configuration.py
--rw-r--r--   0        0        0     2605 2023-05-17 11:58:03.909685 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/properties.py
--rw-r--r--   0        0        0     4978 2023-05-17 11:58:03.935563 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/role_mapping.py
--rw-r--r--   0        0        0      125 2023-05-17 11:58:03.910824 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/role_type.py
--rw-r--r--   0        0        0     3964 2023-05-17 11:58:03.936706 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/rule.py
--rw-r--r--   0        0        0      110 2023-05-17 11:58:03.924553 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/rule_type.py
--rw-r--r--   0        0        0     2301 2023-05-17 11:58:03.918175 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/rule_violation_error.py
--rw-r--r--   0        0        0    11035 2023-05-17 11:58:03.932367 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_artifact.py
--rw-r--r--   0        0        0     7087 2023-05-17 11:58:03.938505 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_group.py
--rw-r--r--   0        0        0    12237 2023-05-17 11:58:03.942119 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_version.py
--rw-r--r--   0        0        0     5359 2023-05-17 11:58:03.926428 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/system_info.py
--rw-r--r--   0        0        0     3263 2023-05-17 11:58:03.949597 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_configuration_property.py
--rw-r--r--   0        0        0     3322 2023-05-17 11:58:03.904847 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_role.py
--rw-r--r--   0        0        0     3712 2023-05-17 11:58:03.946103 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_state.py
--rw-r--r--   0        0        0     6096 2023-05-17 11:58:03.951886 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/user_info.py
--rw-r--r--   0        0        0    12512 2023-05-17 11:58:03.917536 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/version_meta_data.py
--rw-r--r--   0        0        0     4748 2023-05-17 11:58:03.911864 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/version_search_results.py
--rw-r--r--   0        0        0     4683 2023-05-17 11:58:03.955217 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/registry_client.py
--rw-r--r--   0        0        0    10097 2023-05-17 11:58:03.871355 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/search/artifacts/artifacts_request_builder.py
--rw-r--r--   0        0        0     1669 2023-05-17 11:58:03.871996 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/search/search_request_builder.py
--rw-r--r--   0        0        0     3945 2023-05-17 11:58:03.868581 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/info/info_request_builder.py
--rw-r--r--   0        0        0     3913 2023-05-17 11:58:03.869805 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/limits/limits_request_builder.py
--rw-r--r--   0        0        0     1973 2023-05-17 11:58:03.858339 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/system_request_builder.py
--rw-r--r--   0        0        0     3793 2023-05-17 11:58:03.873399 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/users/me/me_request_builder.py
--rw-r--r--   0        0        0     1609 2023-05-17 11:58:03.872606 apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/users/users_request_builder.py
--rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 apicurio_registry_python_sdk_preview-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0      368 2023-05-16 11:09:16.401927 apicurio_registry_python_sdk_preview-2.4.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 11:09:16.404377 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/__init__.py
+-rw-r--r--   0        0        0     6488 2023-05-18 14:39:29.615771 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/__pycache__/registry_client.cpython-311.pyc
+-rw-r--r--   0        0        0     6316 2023-05-18 14:39:20.040265 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/admin_request_builder.py
+-rw-r--r--   0        0        0     4141 2023-05-18 14:39:20.027603 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py
+-rw-r--r--   0        0        0     2509 2023-05-18 14:39:20.032365 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/config/config_request_builder.py
+-rw-r--r--   0        0        0     9895 2023-05-18 14:39:20.030372 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py
+-rw-r--r--   0        0        0     4230 2023-05-18 14:39:20.031213 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py
+-rw-r--r--   0        0        0     4497 2023-05-18 14:39:20.028541 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/export/export_request_builder.py
+-rw-r--r--   0        0        0     4016 2023-05-18 14:39:20.026360 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/import_/import_request_builder.py
+-rw-r--r--   0        0        0     9210 2023-05-18 14:39:20.034219 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py
+-rw-r--r--   0        0        0     3970 2023-05-18 14:39:20.033016 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py
+-rw-r--r--   0        0        0     9490 2023-05-18 14:39:20.038332 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py
+-rw-r--r--   0        0        0     6823 2023-05-18 14:39:20.039242 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py
+-rw-r--r--   0        0        0     9847 2023-05-18 14:39:20.035750 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0     9029 2023-05-18 14:39:20.036960 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     7675 2023-05-18 14:39:20.127302 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/groups_request_builder.py
+-rw-r--r--   0        0        0     9509 2023-05-18 14:39:33.963637 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/__pycache__/with_group_item_request_builder.cpython-311.pyc
+-rw-r--r--   0        0        0    19567 2023-05-18 14:39:33.968288 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/__pycache__/artifacts_request_builder.cpython-311.pyc
+-rw-r--r--   0        0        0    17933 2023-05-18 14:39:20.124915 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0    19640 2023-05-18 14:39:34.434927 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/__pycache__/with_artifact_item_request_builder.cpython-311.pyc
+-rw-r--r--   0        0        0    12567 2023-05-18 14:39:20.103819 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6977 2023-05-18 14:39:20.105087 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py
+-rw-r--r--   0        0        0    11150 2023-05-18 14:39:20.110191 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0    10297 2023-05-18 14:39:20.111715 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     4942 2023-05-18 14:39:20.112673 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py
+-rw-r--r--   0        0        0     7642 2023-05-18 14:39:29.352640 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/test/__pycache__/test_request_builder.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     6104 2023-05-18 14:39:20.106124 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py
+-rw-r--r--   0        0        0    10548 2023-05-18 14:39:20.115303 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6008 2023-05-18 14:39:20.116331 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4767 2023-05-18 14:39:20.113882 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py
+-rw-r--r--   0        0        0    10171 2023-05-18 14:39:20.122057 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py
+-rw-r--r--   0        0        0     9632 2023-05-18 14:39:20.123380 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py
+-rw-r--r--   0        0        0    16487 2023-05-18 14:39:20.108609 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py
+-rw-r--r--   0        0        0     7662 2023-05-18 14:39:20.126085 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py
+-rw-r--r--   0        0        0     1299 2023-05-18 14:39:20.096516 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py
+-rw-r--r--   0        0        0     4122 2023-05-18 14:39:20.098289 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4828 2023-05-18 14:39:20.097398 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py
+-rw-r--r--   0        0        0     1287 2023-05-18 14:39:20.094915 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py
+-rw-r--r--   0        0        0     4108 2023-05-18 14:39:20.094390 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4820 2023-05-18 14:39:20.093514 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py
+-rw-r--r--   0        0        0     1283 2023-05-18 14:39:20.101551 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py
+-rw-r--r--   0        0        0     4807 2023-05-18 14:39:20.100799 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     5362 2023-05-18 14:39:20.099517 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py
+-rw-r--r--   0        0        0     4913 2023-05-18 14:39:20.095905 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/ids_request_builder.py
+-rw-r--r--   0        0        0     1159 2023-05-18 14:39:20.187266 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/kiota-lock.json
+-rw-r--r--   0        0        0     6602 2023-05-18 14:39:29.706534 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/__pycache__/artifact_content.cpython-311.pyc
+-rw-r--r--   0        0        0    22102 2023-05-18 14:39:33.976585 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/__pycache__/artifact_meta_data.cpython-311.pyc
+-rw-r--r--   0        0        0     8212 2023-05-18 14:39:34.426302 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/__pycache__/artifact_reference.cpython-311.pyc
+-rw-r--r--   0        0        0      574 2023-05-18 14:39:34.427634 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/__pycache__/artifact_state.cpython-311.pyc
+-rw-r--r--   0        0        0     8327 2023-05-18 14:39:33.973044 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/__pycache__/error.cpython-311.pyc
+-rw-r--r--   0        0        0     3829 2023-05-18 14:39:34.429655 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/__pycache__/properties.cpython-311.pyc
+-rw-r--r--   0        0        0     4573 2023-05-18 14:39:20.076563 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_content.py
+-rw-r--r--   0        0        0    15041 2023-05-18 14:39:20.085020 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_meta_data.py
+-rw-r--r--   0        0        0     3253 2023-05-18 14:39:20.087171 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_owner.py
+-rw-r--r--   0        0        0     5461 2023-05-18 14:39:20.068700 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_reference.py
+-rw-r--r--   0        0        0     4781 2023-05-18 14:39:20.088780 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_search_results.py
+-rw-r--r--   0        0        0      134 2023-05-18 14:39:20.050789 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_state.py
+-rw-r--r--   0        0        0     3192 2023-05-18 14:39:20.060622 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_type_info.py
+-rw-r--r--   0        0        0     5921 2023-05-18 14:39:20.062324 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/configuration_property.py
+-rw-r--r--   0        0        0     4961 2023-05-18 14:39:20.053704 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/create_group_meta_data.py
+-rw-r--r--   0        0        0     3989 2023-05-18 14:39:20.055466 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/download_ref.py
+-rw-r--r--   0        0        0     5719 2023-05-18 14:39:20.065690 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/editable_meta_data.py
+-rw-r--r--   0        0        0     5777 2023-05-18 14:39:20.075631 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/error.py
+-rw-r--r--   0        0        0     8023 2023-05-18 14:39:20.052171 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/group_meta_data.py
+-rw-r--r--   0        0        0     4661 2023-05-18 14:39:20.066794 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/group_search_results.py
+-rw-r--r--   0        0        0    14563 2023-05-18 14:39:20.081969 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/limits.py
+-rw-r--r--   0        0        0     2597 2023-05-18 14:39:20.087888 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/log_configuration.py
+-rw-r--r--   0        0        0      281 2023-05-18 14:39:20.072234 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/log_level.py
+-rw-r--r--   0        0        0     3217 2023-05-18 14:39:20.054885 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/named_log_configuration.py
+-rw-r--r--   0        0        0     2605 2023-05-18 14:39:20.067486 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/properties.py
+-rw-r--r--   0        0        0     4978 2023-05-18 14:39:20.089912 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/role_mapping.py
+-rw-r--r--   0        0        0      125 2023-05-18 14:39:20.059647 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/role_type.py
+-rw-r--r--   0        0        0     3964 2023-05-18 14:39:20.071805 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/rule.py
+-rw-r--r--   0        0        0      110 2023-05-18 14:39:20.052793 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/rule_type.py
+-rw-r--r--   0        0        0     2301 2023-05-18 14:39:20.079846 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/rule_violation_error.py
+-rw-r--r--   0        0        0    11035 2023-05-18 14:39:20.049914 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/searched_artifact.py
+-rw-r--r--   0        0        0     7087 2023-05-18 14:39:20.073495 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/searched_group.py
+-rw-r--r--   0        0        0    12237 2023-05-18 14:39:20.078873 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/searched_version.py
+-rw-r--r--   0        0        0     5359 2023-05-18 14:39:20.086152 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/system_info.py
+-rw-r--r--   0        0        0     3263 2023-05-18 14:39:20.054288 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/update_configuration_property.py
+-rw-r--r--   0        0        0     3322 2023-05-18 14:39:20.059261 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/update_role.py
+-rw-r--r--   0        0        0     3712 2023-05-18 14:39:20.074537 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/update_state.py
+-rw-r--r--   0        0        0     6096 2023-05-18 14:39:20.064268 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/user_info.py
+-rw-r--r--   0        0        0    12512 2023-05-18 14:39:20.057121 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/version_meta_data.py
+-rw-r--r--   0        0        0     4748 2023-05-18 14:39:20.058098 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/version_search_results.py
+-rw-r--r--   0        0        0     4683 2023-05-18 14:39:20.042004 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/registry_client.py
+-rw-r--r--   0        0        0    10097 2023-05-18 14:39:20.025389 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0     1669 2023-05-18 14:39:20.016926 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/search/search_request_builder.py
+-rw-r--r--   0        0        0     3945 2023-05-18 14:39:20.091571 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/system/info/info_request_builder.py
+-rw-r--r--   0        0        0     3913 2023-05-18 14:39:20.092383 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/system/limits/limits_request_builder.py
+-rw-r--r--   0        0        0     1973 2023-05-18 14:39:20.090664 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/system/system_request_builder.py
+-rw-r--r--   0        0        0     3793 2023-05-18 14:39:20.042844 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/users/me/me_request_builder.py
+-rw-r--r--   0        0        0     1609 2023-05-18 14:39:20.043308 apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/users/users_request_builder.py
+-rw-r--r--   0        0        0     2233 2023-05-18 14:39:08.122837 apicurio_registry_python_sdk_preview-2.4.4/kiota-gen.py
+-rw-r--r--   0        0        0     1168 2023-05-18 14:42:17.232270 apicurio_registry_python_sdk_preview-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 apicurio_registry_python_sdk_preview-2.4.4/PKG-INFO
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/kiota-gen.py` & `apicurio_registry_python_sdk_preview-2.4.4/kiota-gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         "common",
         "src",
         "main",
         "resources",
         "META-INF",
         "openapi.json",
     )
-    output = Path(__file__).parent.joinpath("python_sdk", "client")
+    output = Path(__file__).parent.joinpath("apicurioregistrysdk", "client")
 
     command = f'{kiota_bin} generate --language=python --openapi="{openapi_doc}" --output="{output}" --class-name=RegistryClient --namespace-name=client --clean-output --clear-cache'
     print(f"Executing kiota command: {command}")
 
     os.system(command)
     print("Kiota client generation has been successful")
     return setup_kwargs
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/admin_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/admin_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/artifact_types/artifact_types_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/config_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/config/config_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/properties/item/with_property_name_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/config/properties/properties_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/export/export_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/export/export_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/import_/import_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/import_/import_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/loggers/item/with_logger_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/loggers/loggers_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/role_mappings/item/with_principal_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/role_mappings/role_mappings_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/rules/item/with_rule_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/admin/rules/rules_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/admin/rules/rules_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/groups_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/groups_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/artifacts_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/meta/meta_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/owner/owner_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/rules/rules_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/state/state_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/test/test_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/versions/versions_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/groups/item/with_group_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/content_hashes_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/item/references/references_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/content_ids_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/item/references/references_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/content_ids/item/with_content_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/global_ids_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/item/references/references_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/global_ids/item/with_global_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/ids/ids_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/ids/ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/kiota-lock.json` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/kiota-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'descriptionLocation'": "'/Users/aperuffo/workspace/apicurio-registry/python-sdk/../common/src/main/resources/META-INF/openapi.json'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "clientClassName": "RegistryClient",
     "clientNamespaceName": "client",
     "descriptionHash": "82E94440E9EBA79EE0B70D22913243F7B674081B9D7A032753497AC6179FD7D29BA4F101D46CA67D3898BD6F094986D2789B9A596941496B7C674EAF03456F11",
-    "descriptionLocation": "/Users/aperuffo/workspace/apicurio-registry2/python-sdk/../common/src/main/resources/META-INF/openapi.json",
+    "descriptionLocation": "/Users/aperuffo/workspace/apicurio-registry/python-sdk/../common/src/main/resources/META-INF/openapi.json",
     "deserializers": [
         "Microsoft.Kiota.Serialization.Json.JsonParseNodeFactory",
         "Microsoft.Kiota.Serialization.Text.TextParseNodeFactory",
         "Microsoft.Kiota.Serialization.Form.FormParseNodeFactory"
     ],
     "disabledValidationRules": [],
     "excludePatterns": [],
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_content.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_content.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_owner.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_owner.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_reference.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_reference.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_search_results.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/artifact_type_info.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/artifact_type_info.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/configuration_property.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/configuration_property.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/create_group_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/create_group_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/download_ref.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/download_ref.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/editable_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/editable_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/error.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/error.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/group_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/group_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/group_search_results.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/group_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/limits.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/limits.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/log_configuration.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/log_configuration.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/named_log_configuration.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/named_log_configuration.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/properties.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/properties.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/role_mapping.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/role_mapping.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/rule.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/rule.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/rule_violation_error.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/rule_violation_error.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_artifact.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/searched_artifact.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_group.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/searched_group.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/searched_version.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/searched_version.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/system_info.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_configuration_property.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/update_configuration_property.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_role.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/update_role.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/update_state.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/update_state.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/user_info.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/user_info.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/version_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/version_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/models/version_search_results.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/models/version_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/registry_client.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/registry_client.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/search/artifacts/artifacts_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/search/search_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/search/search_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/info/info_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/system/info/info_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/limits/limits_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/system/limits/limits_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/system/system_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/system/system_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/users/me/me_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/users/me/me_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/python_sdk/client/users/users_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.4/apicurioregistrysdk/client/users/users_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.3/PKG-INFO` & `apicurio_registry_python_sdk_preview-2.4.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: apicurio-registry-python-sdk-preview
-Version: 2.4.3
+Version: 2.4.4
 Summary: 
 Home-page: https://github.com/apicurio/apicurio-registry
 License: Apache 2.0
 Keywords: apicurio,registry
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: microsoft-kiota-abstractions (>=0.5.1,<0.6.0)
 Requires-Dist: microsoft-kiota-http (>=0.4.1,<0.5.0)
 Requires-Dist: microsoft-kiota-serialization-json (>=0.3.2,<0.4.0)
 Requires-Dist: microsoft-kiota-serialization-text (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/apicurio/apicurio-registry
 Description-Content-Type: text/markdown
```

