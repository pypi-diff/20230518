# Comparing `tmp/apicurio_registry_python_sdk_preview-2.4.5.tar.gz` & `tmp/apicurio_registry_python_sdk_preview-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicurio_registry_python_sdk_preview-2.4.5.tar", max compression
+gzip compressed data, was "apicurio_registry_python_sdk_preview-2.4.6.tar", max compression
```

## Comparing `apicurio_registry_python_sdk_preview-2.4.5.tar` & `apicurio_registry_python_sdk_preview-2.4.6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      368 2023-05-16 11:09:16.401927 apicurio_registry_python_sdk_preview-2.4.5/README.md
--rw-r--r--   0        0        0        0 2023-05-16 11:09:16.404377 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/__init__.py
--rw-r--r--   0        0        0     6316 2023-05-18 14:42:35.461976 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/admin_request_builder.py
--rw-r--r--   0        0        0     4141 2023-05-18 14:42:35.472031 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py
--rw-r--r--   0        0        0     2509 2023-05-18 14:42:35.481045 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/config/config_request_builder.py
--rw-r--r--   0        0        0     9895 2023-05-18 14:42:35.482384 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py
--rw-r--r--   0        0        0     4230 2023-05-18 14:42:35.483127 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py
--rw-r--r--   0        0        0     4497 2023-05-18 14:42:35.483981 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/export/export_request_builder.py
--rw-r--r--   0        0        0     4016 2023-05-18 14:42:35.484876 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/import_/import_request_builder.py
--rw-r--r--   0        0        0     9210 2023-05-18 14:42:35.477101 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py
--rw-r--r--   0        0        0     3970 2023-05-18 14:42:35.475767 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py
--rw-r--r--   0        0        0     9490 2023-05-18 14:42:35.473933 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py
--rw-r--r--   0        0        0     6823 2023-05-18 14:42:35.475036 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py
--rw-r--r--   0        0        0     9847 2023-05-18 14:42:35.480328 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py
--rw-r--r--   0        0        0     9029 2023-05-18 14:42:35.478591 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/rules/rules_request_builder.py
--rw-r--r--   0        0        0     7675 2023-05-18 14:42:35.547169 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/groups_request_builder.py
--rw-r--r--   0        0        0    17933 2023-05-18 14:42:35.578990 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py
--rw-r--r--   0        0        0    12567 2023-05-18 14:42:35.575660 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py
--rw-r--r--   0        0        0     6977 2023-05-18 14:42:35.577071 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py
--rw-r--r--   0        0        0    11150 2023-05-18 14:42:35.557956 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py
--rw-r--r--   0        0        0    10297 2023-05-18 14:42:35.554921 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py
--rw-r--r--   0        0        0     4942 2023-05-18 14:42:35.552361 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py
--rw-r--r--   0        0        0     6104 2023-05-18 14:42:35.559413 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py
--rw-r--r--   0        0        0    10548 2023-05-18 14:42:35.564020 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py
--rw-r--r--   0        0        0     6008 2023-05-18 14:42:35.561349 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4767 2023-05-18 14:42:35.565506 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py
--rw-r--r--   0        0        0    10171 2023-05-18 14:42:35.567770 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py
--rw-r--r--   0        0        0     9632 2023-05-18 14:42:35.569863 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py
--rw-r--r--   0        0        0    16487 2023-05-18 14:42:35.573412 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py
--rw-r--r--   0        0        0     7662 2023-05-18 14:42:35.549519 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py
--rw-r--r--   0        0        0     1299 2023-05-18 14:42:35.581858 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py
--rw-r--r--   0        0        0     4122 2023-05-18 14:42:35.581301 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4828 2023-05-18 14:42:35.580312 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py
--rw-r--r--   0        0        0     1287 2023-05-18 14:42:35.593628 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py
--rw-r--r--   0        0        0     4108 2023-05-18 14:42:35.592951 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py
--rw-r--r--   0        0        0     4820 2023-05-18 14:42:35.591982 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py
--rw-r--r--   0        0        0     1283 2023-05-18 14:42:35.583430 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py
--rw-r--r--   0        0        0     4807 2023-05-18 14:42:35.585542 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py
--rw-r--r--   0        0        0     5362 2023-05-18 14:42:35.584491 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py
--rw-r--r--   0        0        0     4913 2023-05-18 14:42:35.582826 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/ids_request_builder.py
--rw-r--r--   0        0        0     1159 2023-05-18 14:42:35.693676 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/kiota-lock.json
--rw-r--r--   0        0        0     4573 2023-05-18 14:42:35.501188 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_content.py
--rw-r--r--   0        0        0    15041 2023-05-18 14:42:35.511381 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_meta_data.py
--rw-r--r--   0        0        0     3253 2023-05-18 14:42:35.504295 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_owner.py
--rw-r--r--   0        0        0     5461 2023-05-18 14:42:35.544433 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_reference.py
--rw-r--r--   0        0        0     4781 2023-05-18 14:42:35.534210 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_search_results.py
--rw-r--r--   0        0        0      134 2023-05-18 14:42:35.518870 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_state.py
--rw-r--r--   0        0        0     3192 2023-05-18 14:42:35.513022 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_type_info.py
--rw-r--r--   0        0        0     5921 2023-05-18 14:42:35.540434 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/configuration_property.py
--rw-r--r--   0        0        0     4961 2023-05-18 14:42:35.530319 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/create_group_meta_data.py
--rw-r--r--   0        0        0     3989 2023-05-18 14:42:35.536018 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/download_ref.py
--rw-r--r--   0        0        0     5719 2023-05-18 14:42:35.502509 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/editable_meta_data.py
--rw-r--r--   0        0        0     5777 2023-05-18 14:42:35.496456 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/error.py
--rw-r--r--   0        0        0     8023 2023-05-18 14:42:35.497896 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/group_meta_data.py
--rw-r--r--   0        0        0     4661 2023-05-18 14:42:35.541645 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/group_search_results.py
--rw-r--r--   0        0        0    14563 2023-05-18 14:42:35.532983 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/limits.py
--rw-r--r--   0        0        0     2597 2023-05-18 14:42:35.542781 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/log_configuration.py
--rw-r--r--   0        0        0      281 2023-05-18 14:42:35.515792 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/log_level.py
--rw-r--r--   0        0        0     3217 2023-05-18 14:42:35.517088 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/named_log_configuration.py
--rw-r--r--   0        0        0     2605 2023-05-18 14:42:35.518445 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/properties.py
--rw-r--r--   0        0        0     4978 2023-05-18 14:42:35.503485 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/role_mapping.py
--rw-r--r--   0        0        0      125 2023-05-18 14:42:35.527897 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/role_type.py
--rw-r--r--   0        0        0     3964 2023-05-18 14:42:35.495082 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/rule.py
--rw-r--r--   0        0        0      110 2023-05-18 14:42:35.515024 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/rule_type.py
--rw-r--r--   0        0        0     2301 2023-05-18 14:42:35.494119 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/rule_violation_error.py
--rw-r--r--   0        0        0    11035 2023-05-18 14:42:35.527399 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/searched_artifact.py
--rw-r--r--   0        0        0     7087 2023-05-18 14:42:35.522466 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/searched_group.py
--rw-r--r--   0        0        0    12237 2023-05-18 14:42:35.493406 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/searched_version.py
--rw-r--r--   0        0        0     5359 2023-05-18 14:42:35.537602 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/system_info.py
--rw-r--r--   0        0        0     3263 2023-05-18 14:42:35.528921 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/update_configuration_property.py
--rw-r--r--   0        0        0     3322 2023-05-18 14:42:35.538947 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/update_role.py
--rw-r--r--   0        0        0     3712 2023-05-18 14:42:35.506421 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/update_state.py
--rw-r--r--   0        0        0     6096 2023-05-18 14:42:35.520486 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/user_info.py
--rw-r--r--   0        0        0    12512 2023-05-18 14:42:35.500132 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/version_meta_data.py
--rw-r--r--   0        0        0     4748 2023-05-18 14:42:35.505226 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/version_search_results.py
--rw-r--r--   0        0        0     4683 2023-05-18 14:42:35.601668 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/registry_client.py
--rw-r--r--   0        0        0    10097 2023-05-18 14:42:35.599810 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py
--rw-r--r--   0        0        0     1669 2023-05-18 14:42:35.598478 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/search/search_request_builder.py
--rw-r--r--   0        0        0     3945 2023-05-18 14:42:35.596431 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/system/info/info_request_builder.py
--rw-r--r--   0        0        0     3913 2023-05-18 14:42:35.594829 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/system/limits/limits_request_builder.py
--rw-r--r--   0        0        0     1973 2023-05-18 14:42:35.595560 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/system/system_request_builder.py
--rw-r--r--   0        0        0     3793 2023-05-18 14:42:35.597348 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/users/me/me_request_builder.py
--rw-r--r--   0        0        0     1609 2023-05-18 14:42:35.597873 apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/users/users_request_builder.py
--rw-r--r--   0        0        0     2233 2023-05-18 14:39:08.122837 apicurio_registry_python_sdk_preview-2.4.5/kiota-gen.py
--rw-r--r--   0        0        0     1121 2023-05-18 15:16:08.247032 apicurio_registry_python_sdk_preview-2.4.5/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 apicurio_registry_python_sdk_preview-2.4.5/PKG-INFO
+-rw-r--r--   0        0        0      368 2023-05-16 11:09:16.401927 apicurio_registry_python_sdk_preview-2.4.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 11:09:16.404377 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/__init__.py
+-rw-r--r--   0        0        0     6316 2023-05-18 15:16:41.445520 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/admin_request_builder.py
+-rw-r--r--   0        0        0     4141 2023-05-18 15:16:41.456905 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py
+-rw-r--r--   0        0        0     2509 2023-05-18 15:16:41.451335 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/config/config_request_builder.py
+-rw-r--r--   0        0        0     9895 2023-05-18 15:16:41.452585 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py
+-rw-r--r--   0        0        0     4230 2023-05-18 15:16:41.453460 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py
+-rw-r--r--   0        0        0     4497 2023-05-18 15:16:41.457622 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/export/export_request_builder.py
+-rw-r--r--   0        0        0     4016 2023-05-18 15:16:41.456234 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/import_/import_request_builder.py
+-rw-r--r--   0        0        0     9210 2023-05-18 15:16:41.448388 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py
+-rw-r--r--   0        0        0     3970 2023-05-18 15:16:41.446398 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py
+-rw-r--r--   0        0        0     9490 2023-05-18 15:16:41.454757 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py
+-rw-r--r--   0        0        0     6823 2023-05-18 15:16:41.455577 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py
+-rw-r--r--   0        0        0     9847 2023-05-18 15:16:41.449649 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0     9029 2023-05-18 15:16:41.450744 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     7675 2023-05-18 15:16:41.482390 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/groups_request_builder.py
+-rw-r--r--   0        0        0    17933 2023-05-18 15:16:41.480515 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0    12567 2023-05-18 15:16:41.467592 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6977 2023-05-18 15:16:41.479276 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py
+-rw-r--r--   0        0        0    11150 2023-05-18 15:16:41.477124 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py
+-rw-r--r--   0        0        0    10297 2023-05-18 15:16:41.478307 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py
+-rw-r--r--   0        0        0     4942 2023-05-18 15:16:41.464789 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py
+-rw-r--r--   0        0        0     6104 2023-05-18 15:16:41.474382 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py
+-rw-r--r--   0        0        0    10548 2023-05-18 15:16:41.468941 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py
+-rw-r--r--   0        0        0     6008 2023-05-18 15:16:41.470067 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4767 2023-05-18 15:16:41.472298 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py
+-rw-r--r--   0        0        0    10171 2023-05-18 15:16:41.471446 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py
+-rw-r--r--   0        0        0     9632 2023-05-18 15:16:41.473529 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py
+-rw-r--r--   0        0        0    16487 2023-05-18 15:16:41.466364 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py
+-rw-r--r--   0        0        0     7662 2023-05-18 15:16:41.481479 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py
+-rw-r--r--   0        0        0     1299 2023-05-18 15:16:41.461310 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py
+-rw-r--r--   0        0        0     4122 2023-05-18 15:16:41.460900 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4828 2023-05-18 15:16:41.460257 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py
+-rw-r--r--   0        0        0     1287 2023-05-18 15:16:41.459522 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py
+-rw-r--r--   0        0        0     4108 2023-05-18 15:16:41.458495 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     4820 2023-05-18 15:16:41.459115 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py
+-rw-r--r--   0        0        0     1283 2023-05-18 15:16:41.461712 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py
+-rw-r--r--   0        0        0     4807 2023-05-18 15:16:41.463051 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py
+-rw-r--r--   0        0        0     5362 2023-05-18 15:16:41.462383 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py
+-rw-r--r--   0        0        0     4913 2023-05-18 15:16:41.463806 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/ids_request_builder.py
+-rw-r--r--   0        0        0     1159 2023-05-18 15:16:41.593738 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/kiota-lock.json
+-rw-r--r--   0        0        0     4573 2023-05-18 15:16:41.509845 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_content.py
+-rw-r--r--   0        0        0    15041 2023-05-18 15:16:41.519558 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_meta_data.py
+-rw-r--r--   0        0        0     3253 2023-05-18 15:16:41.513405 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_owner.py
+-rw-r--r--   0        0        0     5461 2023-05-18 15:16:41.515483 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_reference.py
+-rw-r--r--   0        0        0     4781 2023-05-18 15:16:41.491379 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_search_results.py
+-rw-r--r--   0        0        0      134 2023-05-18 15:16:41.514510 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_state.py
+-rw-r--r--   0        0        0     3192 2023-05-18 15:16:41.496884 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_type_info.py
+-rw-r--r--   0        0        0     5921 2023-05-18 15:16:41.494126 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/configuration_property.py
+-rw-r--r--   0        0        0     4961 2023-05-18 15:16:41.495274 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/create_group_meta_data.py
+-rw-r--r--   0        0        0     3989 2023-05-18 15:16:41.530888 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/download_ref.py
+-rw-r--r--   0        0        0     5719 2023-05-18 15:16:41.534144 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/editable_meta_data.py
+-rw-r--r--   0        0        0     5777 2023-05-18 15:16:41.508861 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/error.py
+-rw-r--r--   0        0        0     8023 2023-05-18 15:16:41.521112 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/group_meta_data.py
+-rw-r--r--   0        0        0     4661 2023-05-18 15:16:41.497813 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/group_search_results.py
+-rw-r--r--   0        0        0    14563 2023-05-18 15:16:41.505669 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/limits.py
+-rw-r--r--   0        0        0     2597 2023-05-18 15:16:41.516491 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/log_configuration.py
+-rw-r--r--   0        0        0      281 2023-05-18 15:16:41.515858 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/log_level.py
+-rw-r--r--   0        0        0     3217 2023-05-18 15:16:41.496101 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/named_log_configuration.py
+-rw-r--r--   0        0        0     2605 2023-05-18 15:16:41.492488 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/properties.py
+-rw-r--r--   0        0        0     4978 2023-05-18 15:16:41.526081 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/role_mapping.py
+-rw-r--r--   0        0        0      125 2023-05-18 15:16:41.503568 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/role_type.py
+-rw-r--r--   0        0        0     3964 2023-05-18 15:16:41.502346 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/rule.py
+-rw-r--r--   0        0        0      110 2023-05-18 15:16:41.512656 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/rule_type.py
+-rw-r--r--   0        0        0     2301 2023-05-18 15:16:41.522607 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/rule_violation_error.py
+-rw-r--r--   0        0        0    11035 2023-05-18 15:16:41.507685 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/searched_artifact.py
+-rw-r--r--   0        0        0     7087 2023-05-18 15:16:41.525009 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/searched_group.py
+-rw-r--r--   0        0        0    12237 2023-05-18 15:16:41.511852 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/searched_version.py
+-rw-r--r--   0        0        0     5359 2023-05-18 15:16:41.533019 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/system_info.py
+-rw-r--r--   0        0        0     3263 2023-05-18 15:16:41.521962 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/update_configuration_property.py
+-rw-r--r--   0        0        0     3322 2023-05-18 15:16:41.498782 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/update_role.py
+-rw-r--r--   0        0        0     3712 2023-05-18 15:16:41.514177 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/update_state.py
+-rw-r--r--   0        0        0     6096 2023-05-18 15:16:41.532009 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/user_info.py
+-rw-r--r--   0        0        0    12512 2023-05-18 15:16:41.501029 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/version_meta_data.py
+-rw-r--r--   0        0        0     4748 2023-05-18 15:16:41.523649 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/version_search_results.py
+-rw-r--r--   0        0        0     4683 2023-05-18 15:16:41.484118 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/registry_client.py
+-rw-r--r--   0        0        0    10097 2023-05-18 15:16:41.537958 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py
+-rw-r--r--   0        0        0     1669 2023-05-18 15:16:41.538587 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/search/search_request_builder.py
+-rw-r--r--   0        0        0     3945 2023-05-18 15:16:41.535200 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/system/info/info_request_builder.py
+-rw-r--r--   0        0        0     3913 2023-05-18 15:16:41.536656 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/system/limits/limits_request_builder.py
+-rw-r--r--   0        0        0     1973 2023-05-18 15:16:41.535845 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/system/system_request_builder.py
+-rw-r--r--   0        0        0     3793 2023-05-18 15:16:41.443676 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/users/me/me_request_builder.py
+-rw-r--r--   0        0        0     1609 2023-05-18 15:16:41.435511 apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/users/users_request_builder.py
+-rw-r--r--   0        0        0     2233 2023-05-18 14:39:08.122837 apicurio_registry_python_sdk_preview-2.4.6/kiota-gen.py
+-rw-r--r--   0        0        0     1146 2023-05-18 15:21:28.538756 apicurio_registry_python_sdk_preview-2.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 apicurio_registry_python_sdk_preview-2.4.6/PKG-INFO
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/admin_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/admin_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/artifact_types/artifact_types_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/config/config_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/config/config_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/config/properties/item/with_property_name_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/config/properties/properties_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/export/export_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/export/export_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/import_/import_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/import_/import_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/loggers/item/with_logger_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/loggers/loggers_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/role_mappings/item/with_principal_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/role_mappings/role_mappings_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/rules/item/with_rule_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/admin/rules/rules_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/admin/rules/rules_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/groups_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/groups_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/artifacts_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/meta/meta_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/owner/owner_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/rules/item/with_rule_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/rules/rules_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/state/state_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/test/test_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/meta/meta_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/state/state_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/item/with_version_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/versions/versions_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/artifacts/item/with_artifact_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/groups/item/with_group_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_hashes/content_hashes_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_hashes/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_hashes/item/with_content_hash_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_ids/content_ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_ids/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/content_ids/item/with_content_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/global_ids/global_ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/global_ids/item/references/references_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/global_ids/item/with_global_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/ids/ids_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/ids/ids_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/kiota-lock.json` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/kiota-lock.json`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_content.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_content.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_owner.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_owner.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_reference.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_reference.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_search_results.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/artifact_type_info.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/artifact_type_info.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/configuration_property.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/configuration_property.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/create_group_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/create_group_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/download_ref.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/download_ref.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/editable_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/editable_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/error.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/error.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/group_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/group_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/group_search_results.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/group_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/limits.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/limits.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/log_configuration.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/log_configuration.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/named_log_configuration.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/named_log_configuration.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/properties.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/properties.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/role_mapping.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/role_mapping.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/rule.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/rule.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/rule_violation_error.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/rule_violation_error.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/searched_artifact.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/searched_artifact.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/searched_group.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/searched_group.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/searched_version.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/searched_version.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/system_info.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/system_info.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/update_configuration_property.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/update_configuration_property.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/update_role.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/update_role.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/update_state.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/update_state.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/user_info.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/user_info.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/version_meta_data.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/version_meta_data.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/models/version_search_results.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/models/version_search_results.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/registry_client.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/registry_client.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/search/artifacts/artifacts_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/search/search_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/search/search_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/system/info/info_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/system/info/info_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/system/limits/limits_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/system/limits/limits_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/system/system_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/system/system_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/users/me/me_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/users/me/me_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/apicurioregistrysdk/client/users/users_request_builder.py` & `apicurio_registry_python_sdk_preview-2.4.6/apicurioregistrysdk/client/users/users_request_builder.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/kiota-gen.py` & `apicurio_registry_python_sdk_preview-2.4.6/kiota-gen.py`

 * *Files identical despite different names*

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/pyproject.toml` & `apicurio_registry_python_sdk_preview-2.4.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "apicurio-registry-python-sdk-preview"
-version = "2.4.5"
+version = "2.4.6"
 description = ""
 authors = ["Andrea Peruffo <andrea.peruffo1982@gmail.com>"]
 readme = "README.md"
 packages = [{include = "apicurioregistrysdk"}]
 include = [
-    { path = "apicurioregistrysdk/client/**/*" }
+    "apicurioregistrysdk/client/*",
+    "apicurioregistrysdk/client/**/*"
 ]
 license = "Apache 2.0"
 homepage = "https://github.com/apicurio/apicurio-registry"
 repository = "https://github.com/apicurio/apicurio-registry"
 keywords = ["apicurio", "registry"]
 
 [tool.poetry.dependencies]
```

### Comparing `apicurio_registry_python_sdk_preview-2.4.5/PKG-INFO` & `apicurio_registry_python_sdk_preview-2.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apicurio-registry-python-sdk-preview
-Version: 2.4.5
+Version: 2.4.6
 Summary: 
 Home-page: https://github.com/apicurio/apicurio-registry
 License: Apache 2.0
 Keywords: apicurio,registry
 Author: Andrea Peruffo
 Author-email: andrea.peruffo1982@gmail.com
 Requires-Python: >=3.9,<4.0
```

