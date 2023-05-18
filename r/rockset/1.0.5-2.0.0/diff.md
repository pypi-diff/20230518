# Comparing `tmp/rockset-1.0.5.tar.gz` & `tmp/rockset-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockset-1.0.5.tar", max compression
+gzip compressed data, was "rockset-2.0.0.tar", max compression
```

## Comparing `rockset-1.0.5.tar` & `rockset-2.0.0.tar`

### file list

```diff
@@ -1,238 +1,237 @@
--rw-r--r--   0        0        0      357 2022-11-16 22:43:16.448063 rockset-1.0.5/LONG_DESCRIPTION.rst
--rw-r--r--   0        0        0     1662 2023-02-15 19:58:52.921760 rockset-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1338 2023-02-15 19:52:29.686527 rockset-1.0.5/rockset/__init__.py
--rw-r--r--   0        0        0      208 2023-02-15 19:52:29.686527 rockset-1.0.5/rockset/api/__init__.py
--rw-r--r--   0        0        0    34696 2023-02-15 19:52:29.790526 rockset-1.0.5/rockset/api/aliases_api.py
--rw-r--r--   0        0        0    29724 2023-02-15 19:52:29.790526 rockset-1.0.5/rockset/api/api_keys_api.py
--rw-r--r--   0        0        0   130795 2023-02-15 19:52:29.794526 rockset-1.0.5/rockset/api/collections_api.py
--rw-r--r--   0        0        0    28165 2023-02-15 19:52:29.798526 rockset-1.0.5/rockset/api/custom_roles_api.py
--rw-r--r--   0        0        0    21187 2023-02-15 19:52:29.798526 rockset-1.0.5/rockset/api/documents_api.py
--rw-r--r--   0        0        0    73682 2023-02-15 19:52:29.790526 rockset-1.0.5/rockset/api/integrations_api.py
--rw-r--r--   0        0        0     6168 2023-02-15 19:52:29.798526 rockset-1.0.5/rockset/api/organizations_api.py
--rw-r--r--   0        0        0    34734 2023-02-15 19:52:29.798526 rockset-1.0.5/rockset/api/queries_api.py
--rw-r--r--   0        0        0    87549 2023-02-15 19:52:29.794526 rockset-1.0.5/rockset/api/query_lambdas_api.py
--rw-r--r--   0        0        0     7727 2023-02-15 19:52:29.790526 rockset-1.0.5/rockset/api/shared_lambdas_api.py
--rw-r--r--   0        0        0    43268 2023-02-15 19:52:29.790526 rockset-1.0.5/rockset/api/users_api.py
--rw-r--r--   0        0        0    34441 2023-02-15 19:52:29.794526 rockset-1.0.5/rockset/api/views_api.py
--rw-r--r--   0        0        0    76220 2023-02-15 19:52:29.798526 rockset-1.0.5/rockset/api/virtual_instances_api.py
--rw-r--r--   0        0        0    22087 2023-02-15 19:52:29.798526 rockset-1.0.5/rockset/api/workspaces_api.py
--rw-r--r--   0        0        0    36245 2023-02-15 19:52:29.690527 rockset-1.0.5/rockset/api_client.py
--rw-r--r--   0        0        0     1112 2023-02-15 19:52:29.702527 rockset-1.0.5/rockset/apis/__init__.py
--rw-r--r--   0        0        0    15516 2023-02-15 19:52:29.686527 rockset-1.0.5/rockset/configuration.py
--rw-r--r--   0        0        0     3831 2022-11-16 22:43:16.456063 rockset-1.0.5/rockset/document.py
--rw-r--r--   0        0        0     6072 2023-02-15 19:52:29.686527 rockset-1.0.5/rockset/exceptions.py
--rw-r--r--   0        0        0      348 2023-02-15 19:52:29.698527 rockset-1.0.5/rockset/model/__init__.py
--rw-r--r--   0        0        0    11950 2023-02-15 19:52:27.762550 rockset-1.0.5/rockset/model/add_documents_request.py
--rw-r--r--   0        0        0    11922 2023-02-15 19:52:27.782550 rockset-1.0.5/rockset/model/add_documents_response.py
--rw-r--r--   0        0        0    13623 2023-02-15 19:52:27.806550 rockset-1.0.5/rockset/model/alias.py
--rw-r--r--   0        0        0    13945 2023-02-15 19:52:27.822549 rockset-1.0.5/rockset/model/api_key.py
--rw-r--r--   0        0        0    13542 2023-02-15 19:52:27.838549 rockset-1.0.5/rockset/model/async_query_options.py
--rw-r--r--   0        0        0    12229 2023-02-15 19:52:27.850549 rockset-1.0.5/rockset/model/aws_access_key.py
--rw-r--r--   0        0        0    12101 2023-02-15 19:52:27.862549 rockset-1.0.5/rockset/model/aws_role.py
--rw-r--r--   0        0        0    15124 2023-02-15 19:52:27.878549 rockset-1.0.5/rockset/model/azure_blob_storage_collection_creation_request.py
--rw-r--r--   0        0        0    11893 2023-02-15 19:52:27.890549 rockset-1.0.5/rockset/model/azure_blob_storage_integration.py
--rw-r--r--   0        0        0    12616 2023-02-15 19:52:27.898548 rockset-1.0.5/rockset/model/azure_blob_storage_integration_creation_request.py
--rw-r--r--   0        0        0    14449 2023-02-15 19:52:27.910548 rockset-1.0.5/rockset/model/azure_blob_storage_source_wrapper.py
--rw-r--r--   0        0        0    15104 2023-02-15 19:52:27.922548 rockset-1.0.5/rockset/model/azure_event_hubs_collection_creation_request.py
--rw-r--r--   0        0        0    11787 2023-02-15 19:52:27.938548 rockset-1.0.5/rockset/model/azure_event_hubs_integration.py
--rw-r--r--   0        0        0    12586 2023-02-15 19:52:27.946548 rockset-1.0.5/rockset/model/azure_event_hubs_integration_creation_request.py
--rw-r--r--   0        0        0    13452 2023-02-15 19:52:27.958548 rockset-1.0.5/rockset/model/azure_event_hubs_source_wrapper.py
--rw-r--r--   0        0        0    15114 2023-02-15 19:52:27.970548 rockset-1.0.5/rockset/model/azure_service_bus_collection_creation_request.py
--rw-r--r--   0        0        0    11888 2023-02-15 19:52:27.982548 rockset-1.0.5/rockset/model/azure_service_bus_integration.py
--rw-r--r--   0        0        0    13333 2023-02-15 19:52:27.990548 rockset-1.0.5/rockset/model/azure_service_bus_source_wrapper.py
--rw-r--r--   0        0        0    18743 2023-02-15 19:52:27.998547 rockset-1.0.5/rockset/model/bulk_stats.py
--rw-r--r--   0        0        0    11798 2023-02-15 19:52:28.010547 rockset-1.0.5/rockset/model/cancel_query_response.py
--rw-r--r--   0        0        0    13225 2023-02-15 19:52:28.018547 rockset-1.0.5/rockset/model/cluster.py
--rw-r--r--   0        0        0    17684 2023-02-15 19:52:28.030547 rockset-1.0.5/rockset/model/collection.py
--rw-r--r--   0        0        0    14579 2023-02-15 19:52:28.038547 rockset-1.0.5/rockset/model/collection_mount.py
--rw-r--r--   0        0        0    11852 2023-02-15 19:52:28.046547 rockset-1.0.5/rockset/model/collection_mount_response.py
--rw-r--r--   0        0        0    11772 2023-02-15 19:52:28.054547 rockset-1.0.5/rockset/model/collection_mount_stats.py
--rw-r--r--   0        0        0    16965 2023-02-15 19:52:28.062547 rockset-1.0.5/rockset/model/collection_stats.py
--rw-r--r--   0        0        0    12333 2023-02-15 19:52:28.074546 rockset-1.0.5/rockset/model/create_alias_request.py
--rw-r--r--   0        0        0    11769 2023-02-15 19:52:28.082546 rockset-1.0.5/rockset/model/create_alias_response.py
--rw-r--r--   0        0        0    12098 2023-02-15 19:52:28.090546 rockset-1.0.5/rockset/model/create_api_key_request.py
--rw-r--r--   0        0        0    11780 2023-02-15 19:52:28.098546 rockset-1.0.5/rockset/model/create_api_key_response.py
--rw-r--r--   0        0        0    12071 2023-02-15 19:52:28.106546 rockset-1.0.5/rockset/model/create_collection_mount_request.py
--rw-r--r--   0        0        0    11913 2023-02-15 19:52:28.114546 rockset-1.0.5/rockset/model/create_collection_mounts_response.py
--rw-r--r--   0        0        0    14506 2023-02-15 19:52:28.122546 rockset-1.0.5/rockset/model/create_collection_request.py
--rw-r--r--   0        0        0    11819 2023-02-15 19:52:28.130546 rockset-1.0.5/rockset/model/create_collection_response.py
--rw-r--r--   0        0        0    16037 2023-02-15 19:52:28.138546 rockset-1.0.5/rockset/model/create_integration_request.py
--rw-r--r--   0        0        0    11829 2023-02-15 19:52:28.146546 rockset-1.0.5/rockset/model/create_integration_response.py
--rw-r--r--   0        0        0    12571 2023-02-15 19:52:28.154545 rockset-1.0.5/rockset/model/create_query_lambda_request.py
--rw-r--r--   0        0        0    12063 2023-02-15 19:52:28.166545 rockset-1.0.5/rockset/model/create_query_lambda_tag_request.py
--rw-r--r--   0        0        0    12501 2023-02-15 19:52:28.174545 rockset-1.0.5/rockset/model/create_role_request.py
--rw-r--r--   0        0        0    12479 2023-02-15 19:52:28.182545 rockset-1.0.5/rockset/model/create_user_request.py
--rw-r--r--   0        0        0    11759 2023-02-15 19:52:28.190545 rockset-1.0.5/rockset/model/create_user_response.py
--rw-r--r--   0        0        0    12170 2023-02-15 19:52:28.198545 rockset-1.0.5/rockset/model/create_view_request.py
--rw-r--r--   0        0        0    11759 2023-02-15 19:52:28.206545 rockset-1.0.5/rockset/model/create_view_response.py
--rw-r--r--   0        0        0    13224 2023-02-15 19:52:28.210545 rockset-1.0.5/rockset/model/create_virtual_instance_request.py
--rw-r--r--   0        0        0    11870 2023-02-15 19:52:28.218545 rockset-1.0.5/rockset/model/create_virtual_instance_response.py
--rw-r--r--   0        0        0    12038 2023-02-15 19:52:28.226545 rockset-1.0.5/rockset/model/create_workspace_request.py
--rw-r--r--   0        0        0    11809 2023-02-15 19:52:28.234545 rockset-1.0.5/rockset/model/create_workspace_response.py
--rw-r--r--   0        0        0    14179 2023-02-15 19:52:28.242545 rockset-1.0.5/rockset/model/csv_params.py
--rw-r--r--   0        0        0    11769 2023-02-15 19:52:28.250544 rockset-1.0.5/rockset/model/delete_alias_response.py
--rw-r--r--   0        0        0    11780 2023-02-15 19:52:28.258544 rockset-1.0.5/rockset/model/delete_api_key_response.py
--rw-r--r--   0        0        0    11819 2023-02-15 19:52:28.266544 rockset-1.0.5/rockset/model/delete_collection_response.py
--rw-r--r--   0        0        0    12036 2023-02-15 19:52:28.270544 rockset-1.0.5/rockset/model/delete_documents_request.py
--rw-r--r--   0        0        0    11686 2023-02-15 19:52:28.278544 rockset-1.0.5/rockset/model/delete_documents_request_data.py
--rw-r--r--   0        0        0    11927 2023-02-15 19:52:28.286544 rockset-1.0.5/rockset/model/delete_documents_response.py
--rw-r--r--   0        0        0    11829 2023-02-15 19:52:28.294544 rockset-1.0.5/rockset/model/delete_integration_response.py
--rw-r--r--   0        0        0    11830 2023-02-15 19:52:28.302544 rockset-1.0.5/rockset/model/delete_query_lambda_response.py
--rw-r--r--   0        0        0    11759 2023-02-15 19:52:28.310544 rockset-1.0.5/rockset/model/delete_user_response.py
--rw-r--r--   0        0        0    11759 2023-02-15 19:52:28.318544 rockset-1.0.5/rockset/model/delete_view_response.py
--rw-r--r--   0        0        0    11870 2023-02-15 19:52:28.322543 rockset-1.0.5/rockset/model/delete_virtual_instance_response.py
--rw-r--r--   0        0        0    11809 2023-02-15 19:52:28.330543 rockset-1.0.5/rockset/model/delete_workspace_response.py
--rw-r--r--   0        0        0    13023 2023-02-15 19:52:28.338543 rockset-1.0.5/rockset/model/document_status.py
--rw-r--r--   0        0        0    15042 2023-02-15 19:52:28.346543 rockset-1.0.5/rockset/model/dynamodb_collection_creation_request.py
--rw-r--r--   0        0        0    12563 2023-02-15 19:52:28.354543 rockset-1.0.5/rockset/model/dynamodb_integration.py
--rw-r--r--   0        0        0    12484 2023-02-15 19:52:28.362543 rockset-1.0.5/rockset/model/dynamodb_integration_creation_request.py
--rw-r--r--   0        0        0    14440 2023-02-15 19:52:28.370543 rockset-1.0.5/rockset/model/dynamodb_source_wrapper.py
--rw-r--r--   0        0        0    14520 2023-02-15 19:52:28.378543 rockset-1.0.5/rockset/model/error_model.py
--rw-r--r--   0        0        0    12392 2023-02-15 19:52:28.386543 rockset-1.0.5/rockset/model/event_time_info.py
--rw-r--r--   0        0        0    12656 2023-02-15 19:52:28.394543 rockset-1.0.5/rockset/model/execute_public_query_lambda_request.py
--rw-r--r--   0        0        0    14367 2023-02-15 19:52:28.398543 rockset-1.0.5/rockset/model/execute_query_lambda_request.py
--rw-r--r--   0        0        0    11743 2023-02-15 19:52:28.406542 rockset-1.0.5/rockset/model/field_mapping_query.py
--rw-r--r--   0        0        0    13075 2023-02-15 19:52:28.414542 rockset-1.0.5/rockset/model/field_mapping_v2.py
--rw-r--r--   0        0        0    12543 2023-02-15 19:52:28.418542 rockset-1.0.5/rockset/model/field_partition.py
--rw-r--r--   0        0        0    15063 2023-02-15 19:52:28.426542 rockset-1.0.5/rockset/model/file_upload_collection_creation_request.py
--rw-r--r--   0        0        0    13611 2023-02-15 19:52:28.434542 rockset-1.0.5/rockset/model/file_upload_source_wrapper.py
--rw-r--r--   0        0        0    13202 2023-02-15 19:52:28.442542 rockset-1.0.5/rockset/model/format_params.py
--rw-r--r--   0        0        0    12001 2023-02-15 19:52:28.446542 rockset-1.0.5/rockset/model/gcp_service_account.py
--rw-r--r--   0        0        0    14992 2023-02-15 19:52:28.454542 rockset-1.0.5/rockset/model/gcs_collection_creation_request.py
--rw-r--r--   0        0        0    11915 2023-02-15 19:52:28.462542 rockset-1.0.5/rockset/model/gcs_integration.py
--rw-r--r--   0        0        0    12409 2023-02-15 19:52:28.470542 rockset-1.0.5/rockset/model/gcs_integration_creation_request.py
--rw-r--r--   0        0        0    14666 2023-02-15 19:52:28.474542 rockset-1.0.5/rockset/model/gcs_source_wrapper.py
--rw-r--r--   0        0        0    11760 2023-02-15 19:52:28.482542 rockset-1.0.5/rockset/model/get_alias_response.py
--rw-r--r--   0        0        0    11771 2023-02-15 19:52:28.490542 rockset-1.0.5/rockset/model/get_api_key_response.py
--rw-r--r--   0        0        0    11810 2023-02-15 19:52:28.498541 rockset-1.0.5/rockset/model/get_collection_response.py
--rw-r--r--   0        0        0    11820 2023-02-15 19:52:28.502541 rockset-1.0.5/rockset/model/get_integration_response.py
--rw-r--r--   0        0        0    11789 2023-02-15 19:52:28.510541 rockset-1.0.5/rockset/model/get_query_response.py
--rw-r--r--   0        0        0    11750 2023-02-15 19:52:28.514541 rockset-1.0.5/rockset/model/get_view_response.py
--rw-r--r--   0        0        0    11861 2023-02-15 19:52:28.522541 rockset-1.0.5/rockset/model/get_virtual_instance_response.py
--rw-r--r--   0        0        0    11800 2023-02-15 19:52:28.530541 rockset-1.0.5/rockset/model/get_workspace_response.py
--rw-r--r--   0        0        0    12704 2023-02-15 19:52:28.534541 rockset-1.0.5/rockset/model/input_field.py
--rw-r--r--   0        0        0    17362 2023-02-15 19:52:28.542541 rockset-1.0.5/rockset/model/integration.py
--rw-r--r--   0        0        0    15012 2023-02-15 19:52:28.550541 rockset-1.0.5/rockset/model/kafka_collection_creation_request.py
--rw-r--r--   0        0        0    14826 2023-02-15 19:52:28.558541 rockset-1.0.5/rockset/model/kafka_integration.py
--rw-r--r--   0        0        0    12439 2023-02-15 19:52:28.562541 rockset-1.0.5/rockset/model/kafka_integration_creation_request.py
--rw-r--r--   0        0        0    14027 2023-02-15 19:52:28.570541 rockset-1.0.5/rockset/model/kafka_source_wrapper.py
--rw-r--r--   0        0        0    11845 2023-02-15 19:52:28.578540 rockset-1.0.5/rockset/model/kafka_v3_security_config.py
--rw-r--r--   0        0        0    15032 2023-02-15 19:52:28.582540 rockset-1.0.5/rockset/model/kinesis_collection_creation_request.py
--rw-r--r--   0        0        0    12169 2023-02-15 19:52:28.590540 rockset-1.0.5/rockset/model/kinesis_integration.py
--rw-r--r--   0        0        0    12469 2023-02-15 19:52:28.598540 rockset-1.0.5/rockset/model/kinesis_integration_creation_request.py
--rw-r--r--   0        0        0    14265 2023-02-15 19:52:28.602540 rockset-1.0.5/rockset/model/kinesis_source_wrapper.py
--rw-r--r--   0        0        0    11819 2023-02-15 19:52:28.610540 rockset-1.0.5/rockset/model/list_aliases_response.py
--rw-r--r--   0        0        0    11835 2023-02-15 19:52:28.618540 rockset-1.0.5/rockset/model/list_api_keys_response.py
--rw-r--r--   0        0        0    11937 2023-02-15 19:52:28.622540 rockset-1.0.5/rockset/model/list_collection_mounts_response.py
--rw-r--r--   0        0        0    11874 2023-02-15 19:52:28.630540 rockset-1.0.5/rockset/model/list_collections_response.py
--rw-r--r--   0        0        0    11892 2023-02-15 19:52:28.634540 rockset-1.0.5/rockset/model/list_integrations_response.py
--rw-r--r--   0        0        0    11804 2023-02-15 19:52:28.642540 rockset-1.0.5/rockset/model/list_queries_response.py
--rw-r--r--   0        0        0    11964 2023-02-15 19:52:28.646540 rockset-1.0.5/rockset/model/list_query_lambda_tags_response.py
--rw-r--r--   0        0        0    12010 2023-02-15 19:52:28.654539 rockset-1.0.5/rockset/model/list_query_lambda_versions_response.py
--rw-r--r--   0        0        0    11889 2023-02-15 19:52:28.658539 rockset-1.0.5/rockset/model/list_query_lambdas_response.py
--rw-r--r--   0        0        0    11802 2023-02-15 19:52:28.662539 rockset-1.0.5/rockset/model/list_roles_response.py
--rw-r--r--   0        0        0    12003 2023-02-15 19:52:28.670539 rockset-1.0.5/rockset/model/list_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    11794 2023-02-15 19:52:28.674539 rockset-1.0.5/rockset/model/list_users_response.py
--rw-r--r--   0        0        0    11802 2023-02-15 19:52:28.682539 rockset-1.0.5/rockset/model/list_views_response.py
--rw-r--r--   0        0        0    11937 2023-02-15 19:52:28.686539 rockset-1.0.5/rockset/model/list_virtual_instances_response.py
--rw-r--r--   0        0        0    11854 2023-02-15 19:52:28.694539 rockset-1.0.5/rockset/model/list_workspaces_response.py
--rw-r--r--   0        0        0    11815 2023-02-15 19:52:28.698539 rockset-1.0.5/rockset/model/mongo_db_integration.py
--rw-r--r--   0        0        0    15032 2023-02-15 19:52:28.706539 rockset-1.0.5/rockset/model/mongodb_collection_creation_request.py
--rw-r--r--   0        0        0    12470 2023-02-15 19:52:28.710539 rockset-1.0.5/rockset/model/mongodb_integration_creation_request.py
--rw-r--r--   0        0        0    13434 2023-02-15 19:52:28.718539 rockset-1.0.5/rockset/model/mongodb_source_wrapper.py
--rw-r--r--   0        0        0    13277 2023-02-15 19:52:28.722539 rockset-1.0.5/rockset/model/organization.py
--rw-r--r--   0        0        0    11821 2023-02-15 19:52:28.730538 rockset-1.0.5/rockset/model/organization_response.py
--rw-r--r--   0        0        0    12527 2023-02-15 19:52:28.734538 rockset-1.0.5/rockset/model/output_field.py
--rw-r--r--   0        0        0    11775 2023-02-15 19:52:28.738538 rockset-1.0.5/rockset/model/pagination.py
--rw-r--r--   0        0        0    13055 2023-02-15 19:52:28.746538 rockset-1.0.5/rockset/model/pagination_info.py
--rw-r--r--   0        0        0    12155 2023-02-15 19:52:28.750538 rockset-1.0.5/rockset/model/patch_document.py
--rw-r--r--   0        0        0    11920 2023-02-15 19:52:28.758538 rockset-1.0.5/rockset/model/patch_documents_request.py
--rw-r--r--   0        0        0    11868 2023-02-15 19:52:28.762538 rockset-1.0.5/rockset/model/patch_documents_response.py
--rw-r--r--   0        0        0    13672 2023-02-15 19:52:28.770538 rockset-1.0.5/rockset/model/patch_operation.py
--rw-r--r--   0        0        0    15362 2023-02-15 19:52:28.774538 rockset-1.0.5/rockset/model/privilege.py
--rw-r--r--   0        0        0    12407 2023-02-15 19:52:28.778538 rockset-1.0.5/rockset/model/query_error.py
--rw-r--r--   0        0        0    11907 2023-02-15 19:52:28.786538 rockset-1.0.5/rockset/model/query_field_type.py
--rw-r--r--   0        0        0    14725 2023-02-15 19:52:28.790538 rockset-1.0.5/rockset/model/query_info.py
--rw-r--r--   0        0        0    13688 2023-02-15 19:52:28.798538 rockset-1.0.5/rockset/model/query_lambda.py
--rw-r--r--   0        0        0    12219 2023-02-15 19:52:28.802538 rockset-1.0.5/rockset/model/query_lambda_sql.py
--rw-r--r--   0        0        0    12786 2023-02-15 19:52:28.806538 rockset-1.0.5/rockset/model/query_lambda_stats.py
--rw-r--r--   0        0        0    12124 2023-02-15 19:52:28.814538 rockset-1.0.5/rockset/model/query_lambda_tag.py
--rw-r--r--   0        0        0    11843 2023-02-15 19:52:28.818538 rockset-1.0.5/rockset/model/query_lambda_tag_response.py
--rw-r--r--   0        0        0    14841 2023-02-15 19:52:28.826537 rockset-1.0.5/rockset/model/query_lambda_version.py
--rw-r--r--   0        0        0    11883 2023-02-15 19:52:28.830537 rockset-1.0.5/rockset/model/query_lambda_version_response.py
--rw-r--r--   0        0        0    12729 2023-02-15 19:52:28.834537 rockset-1.0.5/rockset/model/query_pagination_response.py
--rw-r--r--   0        0        0    12164 2023-02-15 19:52:28.842537 rockset-1.0.5/rockset/model/query_parameter.py
--rw-r--r--   0        0        0    12227 2023-02-15 19:52:28.846537 rockset-1.0.5/rockset/model/query_request.py
--rw-r--r--   0        0        0    14009 2023-02-15 19:52:28.850537 rockset-1.0.5/rockset/model/query_request_sql.py
--rw-r--r--   0        0        0    16189 2022-11-16 22:43:16.476063 rockset-1.0.5/rockset/model/query_response.py
--rw-r--r--   0        0        0    12105 2023-02-15 19:52:28.858537 rockset-1.0.5/rockset/model/query_response_stats.py
--rw-r--r--   0        0        0    11870 2023-02-15 19:52:28.866537 rockset-1.0.5/rockset/model/resume_virtual_instance_response.py
--rw-r--r--   0        0        0    13363 2023-02-15 19:52:28.870537 rockset-1.0.5/rockset/model/role.py
--rw-r--r--   0        0        0    11741 2023-02-15 19:52:28.874537 rockset-1.0.5/rockset/model/role_response.py
--rw-r--r--   0        0        0    14982 2023-02-15 19:52:28.882537 rockset-1.0.5/rockset/model/s3_collection_creation_request.py
--rw-r--r--   0        0        0    12154 2023-02-15 19:52:28.886537 rockset-1.0.5/rockset/model/s3_integration.py
--rw-r--r--   0        0        0    12394 2023-02-15 19:52:28.894537 rockset-1.0.5/rockset/model/s3_integration_creation_request.py
--rw-r--r--   0        0        0    15239 2023-02-15 19:52:28.898537 rockset-1.0.5/rockset/model/s3_source_wrapper.py
--rw-r--r--   0        0        0    12201 2023-02-15 19:52:28.902536 rockset-1.0.5/rockset/model/schema_registry_config.py
--rw-r--r--   0        0        0    11696 2022-11-16 22:43:16.480063 rockset-1.0.5/rockset/model/segment_integration.py
--rw-r--r--   0        0        0    12465 2022-11-16 22:43:16.480063 rockset-1.0.5/rockset/model/segment_integration_creation_request.py
--rw-r--r--   0        0        0    15052 2023-02-15 19:52:28.910536 rockset-1.0.5/rockset/model/snowflake_collection_creation_request.py
--rw-r--r--   0        0        0    14450 2023-02-15 19:52:28.914536 rockset-1.0.5/rockset/model/snowflake_integration.py
--rw-r--r--   0        0        0    12499 2023-02-15 19:52:28.922536 rockset-1.0.5/rockset/model/snowflake_integration_creation_request.py
--rw-r--r--   0        0        0    13907 2023-02-15 19:52:28.926536 rockset-1.0.5/rockset/model/snowflake_source_wrapper.py
--rw-r--r--   0        0        0    12501 2023-02-15 19:52:28.934536 rockset-1.0.5/rockset/model/source.py
--rw-r--r--   0        0        0    13169 2023-02-15 19:52:28.938536 rockset-1.0.5/rockset/model/source_azure_blob_storage.py
--rw-r--r--   0        0        0    12664 2023-02-15 19:52:28.942536 rockset-1.0.5/rockset/model/source_azure_event_hubs.py
--rw-r--r--   0        0        0    12552 2023-02-15 19:52:28.950536 rockset-1.0.5/rockset/model/source_azure_service_bus.py
--rw-r--r--   0        0        0    13624 2023-02-15 19:52:28.954536 rockset-1.0.5/rockset/model/source_dynamo_db.py
--rw-r--r--   0        0        0    12391 2023-02-15 19:52:28.958536 rockset-1.0.5/rockset/model/source_file_upload.py
--rw-r--r--   0        0        0    13371 2023-02-15 19:52:28.966536 rockset-1.0.5/rockset/model/source_gcs.py
--rw-r--r--   0        0        0    13209 2023-02-15 19:52:28.970536 rockset-1.0.5/rockset/model/source_kafka.py
--rw-r--r--   0        0        0    13024 2023-02-15 19:52:28.974536 rockset-1.0.5/rockset/model/source_kinesis.py
--rw-r--r--   0        0        0    12652 2023-02-15 19:52:28.982535 rockset-1.0.5/rockset/model/source_mongo_db.py
--rw-r--r--   0        0        0    13923 2023-02-15 19:52:28.986535 rockset-1.0.5/rockset/model/source_s3.py
--rw-r--r--   0        0        0    13110 2023-02-15 19:52:28.990535 rockset-1.0.5/rockset/model/source_snowflake.py
--rw-r--r--   0        0        0    11661 2023-02-15 19:52:28.998535 rockset-1.0.5/rockset/model/sql_expression.py
--rw-r--r--   0        0        0    13116 2023-02-15 19:52:29.002535 rockset-1.0.5/rockset/model/stats.py
--rw-r--r--   0        0        0    13658 2023-02-15 19:52:29.006535 rockset-1.0.5/rockset/model/status.py
--rw-r--r--   0        0        0    13111 2023-02-15 19:52:29.014535 rockset-1.0.5/rockset/model/status_azure_event_hubs.py
--rw-r--r--   0        0        0    12364 2023-02-15 19:52:29.018535 rockset-1.0.5/rockset/model/status_azure_event_hubs_partition.py
--rw-r--r--   0        0        0    12727 2023-02-15 19:52:29.026535 rockset-1.0.5/rockset/model/status_azure_service_bus.py
--rw-r--r--   0        0        0    12210 2023-02-15 19:52:29.030535 rockset-1.0.5/rockset/model/status_azure_service_bus_session.py
--rw-r--r--   0        0        0    13563 2023-02-15 19:52:29.034535 rockset-1.0.5/rockset/model/status_dynamo_db.py
--rw-r--r--   0        0        0    12705 2023-02-15 19:52:29.042535 rockset-1.0.5/rockset/model/status_dynamo_db_v2.py
--rw-r--r--   0        0        0    13123 2023-02-15 19:52:29.046535 rockset-1.0.5/rockset/model/status_kafka.py
--rw-r--r--   0        0        0    12337 2023-02-15 19:52:29.050535 rockset-1.0.5/rockset/model/status_kafka_partition.py
--rw-r--r--   0        0        0    15614 2023-02-15 19:52:29.054535 rockset-1.0.5/rockset/model/status_mongo_db.py
--rw-r--r--   0        0        0    11924 2023-02-15 19:52:29.062535 rockset-1.0.5/rockset/model/status_snowflake.py
--rw-r--r--   0        0        0    11873 2023-02-15 19:52:29.066535 rockset-1.0.5/rockset/model/suspend_virtual_instance_response.py
--rw-r--r--   0        0        0    11894 2023-02-15 19:52:29.070535 rockset-1.0.5/rockset/model/unsubscribe_preference.py
--rw-r--r--   0        0        0    12119 2023-02-15 19:52:29.078534 rockset-1.0.5/rockset/model/update_alias_request.py
--rw-r--r--   0        0        0    11818 2023-02-15 19:52:29.082534 rockset-1.0.5/rockset/model/update_api_key_request.py
--rw-r--r--   0        0        0    11780 2023-02-15 19:52:29.086534 rockset-1.0.5/rockset/model/update_api_key_response.py
--rw-r--r--   0        0        0    11867 2022-11-16 22:43:16.484063 rockset-1.0.5/rockset/model/update_integration_request.py
--rw-r--r--   0        0        0    11829 2022-11-16 22:43:16.488063 rockset-1.0.5/rockset/model/update_integration_response.py
--rw-r--r--   0        0        0    12329 2023-02-15 19:52:29.094534 rockset-1.0.5/rockset/model/update_query_lambda_request.py
--rw-r--r--   0        0        0    12222 2023-02-15 19:52:29.098534 rockset-1.0.5/rockset/model/update_role_request.py
--rw-r--r--   0        0        0    12006 2023-02-15 19:52:29.102534 rockset-1.0.5/rockset/model/update_unsubscribe_preferences_request.py
--rw-r--r--   0        0        0    12009 2023-02-15 19:52:29.110534 rockset-1.0.5/rockset/model/update_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    12206 2023-02-15 19:52:29.114534 rockset-1.0.5/rockset/model/update_user_request.py
--rw-r--r--   0        0        0    11958 2023-02-15 19:52:29.118534 rockset-1.0.5/rockset/model/update_view_request.py
--rw-r--r--   0        0        0    11759 2023-02-15 19:52:29.122534 rockset-1.0.5/rockset/model/update_view_response.py
--rw-r--r--   0        0        0    13762 2023-02-15 19:52:29.130534 rockset-1.0.5/rockset/model/update_virtual_instance_request.py
--rw-r--r--   0        0        0    11870 2023-02-15 19:52:29.134534 rockset-1.0.5/rockset/model/update_virtual_instance_response.py
--rw-r--r--   0        0        0    12907 2023-02-15 19:52:29.138534 rockset-1.0.5/rockset/model/user.py
--rw-r--r--   0        0        0    12155 2023-02-15 19:52:29.146534 rockset-1.0.5/rockset/model/validate_query_response.py
--rw-r--r--   0        0        0    14473 2023-02-15 19:52:29.150534 rockset-1.0.5/rockset/model/view.py
--rw-r--r--   0        0        0    17180 2023-02-15 19:52:29.154533 rockset-1.0.5/rockset/model/virtual_instance.py
--rw-r--r--   0        0        0    11772 2023-02-15 19:52:29.162533 rockset-1.0.5/rockset/model/virtual_instance_stats.py
--rw-r--r--   0        0        0    12971 2023-02-15 19:52:29.166533 rockset-1.0.5/rockset/model/workspace.py
--rw-r--r--   0        0        0    12998 2023-02-15 19:52:29.170533 rockset-1.0.5/rockset/model/xml_params.py
--rw-r--r--   0        0        0    84037 2023-02-15 19:52:29.698527 rockset-1.0.5/rockset/model_utils.py
--rw-r--r--   0        0        0    14505 2023-02-15 19:52:29.698527 rockset-1.0.5/rockset/models/__init__.py
--rw-r--r--   0        0        0     1819 2022-11-16 22:43:16.492063 rockset-1.0.5/rockset/query_paginator.py
--rw-r--r--   0        0        0    14645 2023-02-15 19:52:29.690527 rockset-1.0.5/rockset/rest.py
--rw-r--r--   0        0        0     8491 2022-11-28 23:26:32.961780 rockset-1.0.5/rockset/rockset_client.py
--rw-r--r--   0        0        0     3644 2022-11-16 22:43:16.492063 rockset-1.0.5/rockset/value.py
--rw-r--r--   0        0        0     1165 2023-02-15 20:13:45.152222 rockset-1.0.5/setup.py
--rw-r--r--   0        0        0     2156 2023-02-15 20:13:45.152761 rockset-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      357 2022-12-13 01:58:51.206007 rockset-2.0.0/LONG_DESCRIPTION.rst
+-rw-r--r--   0        0        0     1615 2023-05-17 23:59:17.562975 rockset-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1338 2022-12-13 01:58:51.321191 rockset-2.0.0/rockset/__init__.py
+-rw-r--r--   0        0        0      208 2022-12-13 01:58:42.690343 rockset-2.0.0/rockset/api/__init__.py
+-rw-r--r--   0        0        0    34696 2022-12-13 01:58:51.322358 rockset-2.0.0/rockset/api/aliases_api.py
+-rw-r--r--   0        0        0    29724 2022-12-13 01:58:51.323252 rockset-2.0.0/rockset/api/api_keys_api.py
+-rw-r--r--   0        0        0   130795 2022-12-13 01:58:51.324989 rockset-2.0.0/rockset/api/collections_api.py
+-rw-r--r--   0        0        0    28165 2022-12-13 01:58:42.693877 rockset-2.0.0/rockset/api/custom_roles_api.py
+-rw-r--r--   0        0        0    21187 2022-12-13 01:58:51.325994 rockset-2.0.0/rockset/api/documents_api.py
+-rw-r--r--   0        0        0    73682 2022-12-13 01:58:51.327346 rockset-2.0.0/rockset/api/integrations_api.py
+-rw-r--r--   0        0        0     6168 2022-12-13 01:58:42.696525 rockset-2.0.0/rockset/api/organizations_api.py
+-rw-r--r--   0        0        0    34734 2023-05-12 17:22:20.907117 rockset-2.0.0/rockset/api/queries_api.py
+-rw-r--r--   0        0        0    87549 2022-12-13 01:58:51.329493 rockset-2.0.0/rockset/api/query_lambdas_api.py
+-rw-r--r--   0        0        0     7727 2023-05-12 17:22:20.910399 rockset-2.0.0/rockset/api/shared_lambdas_api.py
+-rw-r--r--   0        0        0    43268 2023-05-12 17:22:20.918078 rockset-2.0.0/rockset/api/users_api.py
+-rw-r--r--   0        0        0    34441 2022-12-13 01:58:51.332337 rockset-2.0.0/rockset/api/views_api.py
+-rw-r--r--   0        0        0    76220 2023-05-12 17:22:20.924296 rockset-2.0.0/rockset/api/virtual_instances_api.py
+-rw-r--r--   0        0        0    22087 2022-12-13 01:58:51.335148 rockset-2.0.0/rockset/api/workspaces_api.py
+-rw-r--r--   0        0        0    36245 2022-12-13 01:58:51.336141 rockset-2.0.0/rockset/api_client.py
+-rw-r--r--   0        0        0     1112 2022-12-13 01:58:51.337188 rockset-2.0.0/rockset/apis/__init__.py
+-rw-r--r--   0        0        0    15516 2022-12-13 01:58:51.338079 rockset-2.0.0/rockset/configuration.py
+-rw-r--r--   0        0        0     3831 2022-12-13 01:58:42.708412 rockset-2.0.0/rockset/document.py
+-rw-r--r--   0        0        0     6072 2022-12-13 01:58:51.338930 rockset-2.0.0/rockset/exceptions.py
+-rw-r--r--   0        0        0      348 2022-12-13 01:58:42.709463 rockset-2.0.0/rockset/model/__init__.py
+-rw-r--r--   0        0        0    11950 2022-12-13 01:58:51.340059 rockset-2.0.0/rockset/model/add_documents_request.py
+-rw-r--r--   0        0        0    11922 2022-12-13 01:58:51.341043 rockset-2.0.0/rockset/model/add_documents_response.py
+-rw-r--r--   0        0        0    13623 2022-12-13 01:58:51.342438 rockset-2.0.0/rockset/model/alias.py
+-rw-r--r--   0        0        0    13945 2022-12-13 01:58:51.343654 rockset-2.0.0/rockset/model/api_key.py
+-rw-r--r--   0        0        0    13542 2022-12-13 01:58:51.344826 rockset-2.0.0/rockset/model/async_query_options.py
+-rw-r--r--   0        0        0    12229 2022-12-13 01:58:51.346082 rockset-2.0.0/rockset/model/aws_access_key.py
+-rw-r--r--   0        0        0    12101 2022-12-13 01:58:51.347099 rockset-2.0.0/rockset/model/aws_role.py
+-rw-r--r--   0        0        0    15124 2022-12-13 01:58:51.347977 rockset-2.0.0/rockset/model/azure_blob_storage_collection_creation_request.py
+-rw-r--r--   0        0        0    11893 2022-12-13 01:58:51.348793 rockset-2.0.0/rockset/model/azure_blob_storage_integration.py
+-rw-r--r--   0        0        0    12616 2022-12-13 01:58:51.349789 rockset-2.0.0/rockset/model/azure_blob_storage_integration_creation_request.py
+-rw-r--r--   0        0        0    14449 2022-12-13 01:58:51.350910 rockset-2.0.0/rockset/model/azure_blob_storage_source_wrapper.py
+-rw-r--r--   0        0        0    15104 2022-12-13 01:58:51.355455 rockset-2.0.0/rockset/model/azure_event_hubs_collection_creation_request.py
+-rw-r--r--   0        0        0    11787 2022-12-13 01:58:51.356462 rockset-2.0.0/rockset/model/azure_event_hubs_integration.py
+-rw-r--r--   0        0        0    12586 2022-12-13 01:58:51.357448 rockset-2.0.0/rockset/model/azure_event_hubs_integration_creation_request.py
+-rw-r--r--   0        0        0    13452 2022-12-13 01:58:51.358672 rockset-2.0.0/rockset/model/azure_event_hubs_source_wrapper.py
+-rw-r--r--   0        0        0    15114 2022-12-13 01:58:51.359647 rockset-2.0.0/rockset/model/azure_service_bus_collection_creation_request.py
+-rw-r--r--   0        0        0    11888 2022-12-13 01:58:51.361464 rockset-2.0.0/rockset/model/azure_service_bus_integration.py
+-rw-r--r--   0        0        0    13333 2022-12-13 01:58:51.363034 rockset-2.0.0/rockset/model/azure_service_bus_source_wrapper.py
+-rw-r--r--   0        0        0    18743 2023-05-12 17:22:20.928164 rockset-2.0.0/rockset/model/bulk_stats.py
+-rw-r--r--   0        0        0    11798 2022-12-13 01:58:51.364718 rockset-2.0.0/rockset/model/cancel_query_response.py
+-rw-r--r--   0        0        0    13225 2022-12-13 01:58:51.365908 rockset-2.0.0/rockset/model/cluster.py
+-rw-r--r--   0        0        0    17684 2022-12-13 01:58:51.367440 rockset-2.0.0/rockset/model/collection.py
+-rw-r--r--   0        0        0    14579 2023-05-12 17:22:20.935169 rockset-2.0.0/rockset/model/collection_mount.py
+-rw-r--r--   0        0        0    11852 2022-12-13 01:58:51.369480 rockset-2.0.0/rockset/model/collection_mount_response.py
+-rw-r--r--   0        0        0    11772 2023-05-12 17:22:20.942953 rockset-2.0.0/rockset/model/collection_mount_stats.py
+-rw-r--r--   0        0        0    16965 2022-12-13 01:58:51.370768 rockset-2.0.0/rockset/model/collection_stats.py
+-rw-r--r--   0        0        0    12333 2022-12-13 01:58:51.371874 rockset-2.0.0/rockset/model/create_alias_request.py
+-rw-r--r--   0        0        0    11769 2022-12-13 01:58:51.373053 rockset-2.0.0/rockset/model/create_alias_response.py
+-rw-r--r--   0        0        0    12098 2022-12-13 01:58:51.373927 rockset-2.0.0/rockset/model/create_api_key_request.py
+-rw-r--r--   0        0        0    11780 2022-12-13 01:58:51.374901 rockset-2.0.0/rockset/model/create_api_key_response.py
+-rw-r--r--   0        0        0    12071 2022-12-13 01:58:51.375498 rockset-2.0.0/rockset/model/create_collection_mount_request.py
+-rw-r--r--   0        0        0    11913 2023-05-12 17:22:20.945604 rockset-2.0.0/rockset/model/create_collection_mounts_response.py
+-rw-r--r--   0        0        0    14506 2022-12-13 01:58:51.376828 rockset-2.0.0/rockset/model/create_collection_request.py
+-rw-r--r--   0        0        0    11819 2022-12-13 01:58:51.377747 rockset-2.0.0/rockset/model/create_collection_response.py
+-rw-r--r--   0        0        0    16037 2022-12-13 01:58:51.378736 rockset-2.0.0/rockset/model/create_integration_request.py
+-rw-r--r--   0        0        0    11829 2022-12-13 01:58:51.379675 rockset-2.0.0/rockset/model/create_integration_response.py
+-rw-r--r--   0        0        0    12571 2022-12-13 01:58:51.381735 rockset-2.0.0/rockset/model/create_query_lambda_request.py
+-rw-r--r--   0        0        0    12063 2022-12-13 01:58:51.382700 rockset-2.0.0/rockset/model/create_query_lambda_tag_request.py
+-rw-r--r--   0        0        0    12501 2022-12-13 01:58:51.383928 rockset-2.0.0/rockset/model/create_role_request.py
+-rw-r--r--   0        0        0    12479 2023-05-12 17:22:20.953879 rockset-2.0.0/rockset/model/create_user_request.py
+-rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.387934 rockset-2.0.0/rockset/model/create_user_response.py
+-rw-r--r--   0        0        0    12170 2022-12-13 01:58:51.388848 rockset-2.0.0/rockset/model/create_view_request.py
+-rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.389749 rockset-2.0.0/rockset/model/create_view_response.py
+-rw-r--r--   0        0        0    13224 2022-12-13 01:58:51.390403 rockset-2.0.0/rockset/model/create_virtual_instance_request.py
+-rw-r--r--   0        0        0    11870 2022-12-13 01:58:51.391137 rockset-2.0.0/rockset/model/create_virtual_instance_response.py
+-rw-r--r--   0        0        0    12038 2022-12-13 01:58:51.391990 rockset-2.0.0/rockset/model/create_workspace_request.py
+-rw-r--r--   0        0        0    11809 2022-12-13 01:58:51.392971 rockset-2.0.0/rockset/model/create_workspace_response.py
+-rw-r--r--   0        0        0    14179 2022-12-13 01:58:51.394177 rockset-2.0.0/rockset/model/csv_params.py
+-rw-r--r--   0        0        0    11769 2022-12-13 01:58:51.395065 rockset-2.0.0/rockset/model/delete_alias_response.py
+-rw-r--r--   0        0        0    11780 2022-12-13 01:58:51.395871 rockset-2.0.0/rockset/model/delete_api_key_response.py
+-rw-r--r--   0        0        0    11819 2022-12-13 01:58:51.397342 rockset-2.0.0/rockset/model/delete_collection_response.py
+-rw-r--r--   0        0        0    12036 2022-12-13 01:58:51.398103 rockset-2.0.0/rockset/model/delete_documents_request.py
+-rw-r--r--   0        0        0    11686 2022-12-13 01:58:51.398891 rockset-2.0.0/rockset/model/delete_documents_request_data.py
+-rw-r--r--   0        0        0    11927 2022-12-13 01:58:51.399594 rockset-2.0.0/rockset/model/delete_documents_response.py
+-rw-r--r--   0        0        0    11829 2022-12-13 01:58:51.400868 rockset-2.0.0/rockset/model/delete_integration_response.py
+-rw-r--r--   0        0        0    11830 2022-12-13 01:58:51.401717 rockset-2.0.0/rockset/model/delete_query_lambda_response.py
+-rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.405750 rockset-2.0.0/rockset/model/delete_user_response.py
+-rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.406881 rockset-2.0.0/rockset/model/delete_view_response.py
+-rw-r--r--   0        0        0    11870 2022-12-13 01:58:51.407738 rockset-2.0.0/rockset/model/delete_virtual_instance_response.py
+-rw-r--r--   0        0        0    11809 2022-12-13 01:58:51.408605 rockset-2.0.0/rockset/model/delete_workspace_response.py
+-rw-r--r--   0        0        0    13023 2022-12-13 01:58:51.409506 rockset-2.0.0/rockset/model/document_status.py
+-rw-r--r--   0        0        0    15042 2022-12-13 01:58:51.410273 rockset-2.0.0/rockset/model/dynamodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12563 2022-12-13 01:58:51.411173 rockset-2.0.0/rockset/model/dynamodb_integration.py
+-rw-r--r--   0        0        0    12484 2022-12-13 01:58:51.411877 rockset-2.0.0/rockset/model/dynamodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14440 2022-12-13 01:58:51.412536 rockset-2.0.0/rockset/model/dynamodb_source_wrapper.py
+-rw-r--r--   0        0        0    14520 2023-05-12 17:22:20.957148 rockset-2.0.0/rockset/model/error_model.py
+-rw-r--r--   0        0        0    12392 2022-12-13 01:58:51.414156 rockset-2.0.0/rockset/model/event_time_info.py
+-rw-r--r--   0        0        0    12656 2023-05-12 17:22:20.961849 rockset-2.0.0/rockset/model/execute_public_query_lambda_request.py
+-rw-r--r--   0        0        0    14367 2022-12-13 01:58:51.414854 rockset-2.0.0/rockset/model/execute_query_lambda_request.py
+-rw-r--r--   0        0        0    11743 2022-12-13 01:58:51.415485 rockset-2.0.0/rockset/model/field_mapping_query.py
+-rw-r--r--   0        0        0    13075 2022-12-13 01:58:51.416534 rockset-2.0.0/rockset/model/field_mapping_v2.py
+-rw-r--r--   0        0        0    12543 2022-12-13 01:58:51.417789 rockset-2.0.0/rockset/model/field_partition.py
+-rw-r--r--   0        0        0    15063 2022-12-13 01:58:51.418937 rockset-2.0.0/rockset/model/file_upload_collection_creation_request.py
+-rw-r--r--   0        0        0    13611 2022-12-13 01:58:51.419752 rockset-2.0.0/rockset/model/file_upload_source_wrapper.py
+-rw-r--r--   0        0        0    13202 2022-12-13 01:58:51.420839 rockset-2.0.0/rockset/model/format_params.py
+-rw-r--r--   0        0        0    12001 2022-12-13 01:58:51.421612 rockset-2.0.0/rockset/model/gcp_service_account.py
+-rw-r--r--   0        0        0    14992 2022-12-13 01:58:51.422369 rockset-2.0.0/rockset/model/gcs_collection_creation_request.py
+-rw-r--r--   0        0        0    11915 2022-12-13 01:58:51.423092 rockset-2.0.0/rockset/model/gcs_integration.py
+-rw-r--r--   0        0        0    12409 2022-12-13 01:58:51.423760 rockset-2.0.0/rockset/model/gcs_integration_creation_request.py
+-rw-r--r--   0        0        0    14666 2022-12-13 01:58:51.424461 rockset-2.0.0/rockset/model/gcs_source_wrapper.py
+-rw-r--r--   0        0        0    11760 2022-12-13 01:58:51.425075 rockset-2.0.0/rockset/model/get_alias_response.py
+-rw-r--r--   0        0        0    11771 2022-12-13 01:58:51.425773 rockset-2.0.0/rockset/model/get_api_key_response.py
+-rw-r--r--   0        0        0    11810 2022-12-13 01:58:51.426421 rockset-2.0.0/rockset/model/get_collection_response.py
+-rw-r--r--   0        0        0    11820 2022-12-13 01:58:51.427289 rockset-2.0.0/rockset/model/get_integration_response.py
+-rw-r--r--   0        0        0    11789 2022-12-13 01:58:51.428017 rockset-2.0.0/rockset/model/get_query_response.py
+-rw-r--r--   0        0        0    11750 2022-12-13 01:58:51.428894 rockset-2.0.0/rockset/model/get_view_response.py
+-rw-r--r--   0        0        0    11861 2022-12-13 01:58:51.429731 rockset-2.0.0/rockset/model/get_virtual_instance_response.py
+-rw-r--r--   0        0        0    11800 2022-12-13 01:58:51.430619 rockset-2.0.0/rockset/model/get_workspace_response.py
+-rw-r--r--   0        0        0    12704 2022-12-13 01:58:51.431409 rockset-2.0.0/rockset/model/input_field.py
+-rw-r--r--   0        0        0    17362 2022-12-13 01:58:51.432299 rockset-2.0.0/rockset/model/integration.py
+-rw-r--r--   0        0        0    15012 2022-12-13 01:58:51.433257 rockset-2.0.0/rockset/model/kafka_collection_creation_request.py
+-rw-r--r--   0        0        0    14826 2022-12-13 01:58:51.433924 rockset-2.0.0/rockset/model/kafka_integration.py
+-rw-r--r--   0        0        0    12439 2022-12-13 01:58:51.434725 rockset-2.0.0/rockset/model/kafka_integration_creation_request.py
+-rw-r--r--   0        0        0    14027 2022-12-13 01:58:51.435418 rockset-2.0.0/rockset/model/kafka_source_wrapper.py
+-rw-r--r--   0        0        0    11845 2022-12-13 01:58:51.436134 rockset-2.0.0/rockset/model/kafka_v3_security_config.py
+-rw-r--r--   0        0        0    15032 2022-12-13 01:58:51.436744 rockset-2.0.0/rockset/model/kinesis_collection_creation_request.py
+-rw-r--r--   0        0        0    12169 2022-12-13 01:58:51.438159 rockset-2.0.0/rockset/model/kinesis_integration.py
+-rw-r--r--   0        0        0    12469 2022-12-13 01:58:51.438947 rockset-2.0.0/rockset/model/kinesis_integration_creation_request.py
+-rw-r--r--   0        0        0    14265 2022-12-13 01:58:51.439735 rockset-2.0.0/rockset/model/kinesis_source_wrapper.py
+-rw-r--r--   0        0        0    11819 2022-12-13 01:58:51.440610 rockset-2.0.0/rockset/model/list_aliases_response.py
+-rw-r--r--   0        0        0    11835 2022-12-13 01:58:51.441850 rockset-2.0.0/rockset/model/list_api_keys_response.py
+-rw-r--r--   0        0        0    11937 2022-12-13 01:58:51.442402 rockset-2.0.0/rockset/model/list_collection_mounts_response.py
+-rw-r--r--   0        0        0    11874 2022-12-13 01:58:51.443359 rockset-2.0.0/rockset/model/list_collections_response.py
+-rw-r--r--   0        0        0    11892 2022-12-13 01:58:51.444428 rockset-2.0.0/rockset/model/list_integrations_response.py
+-rw-r--r--   0        0        0    11804 2022-12-13 01:58:51.445389 rockset-2.0.0/rockset/model/list_queries_response.py
+-rw-r--r--   0        0        0    11964 2022-12-13 01:58:51.446199 rockset-2.0.0/rockset/model/list_query_lambda_tags_response.py
+-rw-r--r--   0        0        0    12010 2022-12-13 01:58:51.447037 rockset-2.0.0/rockset/model/list_query_lambda_versions_response.py
+-rw-r--r--   0        0        0    11889 2022-12-13 01:58:51.448465 rockset-2.0.0/rockset/model/list_query_lambdas_response.py
+-rw-r--r--   0        0        0    11802 2022-12-13 01:58:51.449343 rockset-2.0.0/rockset/model/list_roles_response.py
+-rw-r--r--   0        0        0    12003 2022-12-13 01:58:51.450548 rockset-2.0.0/rockset/model/list_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    11794 2022-12-13 01:58:51.451885 rockset-2.0.0/rockset/model/list_users_response.py
+-rw-r--r--   0        0        0    11802 2022-12-13 01:58:51.455878 rockset-2.0.0/rockset/model/list_views_response.py
+-rw-r--r--   0        0        0    11937 2022-12-13 01:58:51.456878 rockset-2.0.0/rockset/model/list_virtual_instances_response.py
+-rw-r--r--   0        0        0    11854 2022-12-13 01:58:51.457814 rockset-2.0.0/rockset/model/list_workspaces_response.py
+-rw-r--r--   0        0        0    11815 2022-12-13 01:58:51.458840 rockset-2.0.0/rockset/model/mongo_db_integration.py
+-rw-r--r--   0        0        0    15032 2022-12-13 01:58:51.459596 rockset-2.0.0/rockset/model/mongodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12470 2022-12-13 01:58:51.460283 rockset-2.0.0/rockset/model/mongodb_integration_creation_request.py
+-rw-r--r--   0        0        0    13434 2022-12-13 01:58:51.460926 rockset-2.0.0/rockset/model/mongodb_source_wrapper.py
+-rw-r--r--   0        0        0    13277 2022-12-13 01:58:51.461621 rockset-2.0.0/rockset/model/organization.py
+-rw-r--r--   0        0        0    11821 2022-12-13 01:58:51.462439 rockset-2.0.0/rockset/model/organization_response.py
+-rw-r--r--   0        0        0    12527 2022-12-13 01:58:51.463085 rockset-2.0.0/rockset/model/output_field.py
+-rw-r--r--   0        0        0    11775 2022-12-13 01:58:51.463873 rockset-2.0.0/rockset/model/pagination.py
+-rw-r--r--   0        0        0    13055 2022-12-13 01:58:51.464710 rockset-2.0.0/rockset/model/pagination_info.py
+-rw-r--r--   0        0        0    12155 2022-12-13 01:58:51.465583 rockset-2.0.0/rockset/model/patch_document.py
+-rw-r--r--   0        0        0    11920 2022-12-13 01:58:51.466714 rockset-2.0.0/rockset/model/patch_documents_request.py
+-rw-r--r--   0        0        0    11868 2022-12-13 01:58:51.468318 rockset-2.0.0/rockset/model/patch_documents_response.py
+-rw-r--r--   0        0        0    13672 2022-12-13 01:58:51.469338 rockset-2.0.0/rockset/model/patch_operation.py
+-rw-r--r--   0        0        0    15362 2023-05-12 17:22:20.967106 rockset-2.0.0/rockset/model/privilege.py
+-rw-r--r--   0        0        0    12407 2022-12-13 01:58:51.471138 rockset-2.0.0/rockset/model/query_error.py
+-rw-r--r--   0        0        0    11907 2022-12-13 01:58:51.472036 rockset-2.0.0/rockset/model/query_field_type.py
+-rw-r--r--   0        0        0    14725 2022-12-13 01:58:51.472774 rockset-2.0.0/rockset/model/query_info.py
+-rw-r--r--   0        0        0    13688 2022-12-13 01:58:51.473624 rockset-2.0.0/rockset/model/query_lambda.py
+-rw-r--r--   0        0        0    12219 2022-12-13 01:58:51.474716 rockset-2.0.0/rockset/model/query_lambda_sql.py
+-rw-r--r--   0        0        0    12786 2022-12-13 01:58:51.475873 rockset-2.0.0/rockset/model/query_lambda_stats.py
+-rw-r--r--   0        0        0    12124 2022-12-13 01:58:51.477013 rockset-2.0.0/rockset/model/query_lambda_tag.py
+-rw-r--r--   0        0        0    11843 2022-12-13 01:58:51.477906 rockset-2.0.0/rockset/model/query_lambda_tag_response.py
+-rw-r--r--   0        0        0    14841 2022-12-13 01:58:51.478799 rockset-2.0.0/rockset/model/query_lambda_version.py
+-rw-r--r--   0        0        0    11883 2022-12-13 01:58:51.479680 rockset-2.0.0/rockset/model/query_lambda_version_response.py
+-rw-r--r--   0        0        0    13051 2023-05-18 17:55:09.709562 rockset-2.0.0/rockset/model/query_pagination_response.py
+-rw-r--r--   0        0        0    12164 2022-12-13 01:58:51.481278 rockset-2.0.0/rockset/model/query_parameter.py
+-rw-r--r--   0        0        0    12227 2022-12-13 01:58:51.481934 rockset-2.0.0/rockset/model/query_request.py
+-rw-r--r--   0        0        0    14009 2023-05-12 17:22:20.984866 rockset-2.0.0/rockset/model/query_request_sql.py
+-rw-r--r--   0        0        0    16189 2023-05-17 23:55:16.173168 rockset-2.0.0/rockset/model/query_response.py
+-rw-r--r--   0        0        0    12105 2022-12-13 01:58:51.483887 rockset-2.0.0/rockset/model/query_response_stats.py
+-rw-r--r--   0        0        0    11870 2022-12-13 01:58:51.484388 rockset-2.0.0/rockset/model/resume_virtual_instance_response.py
+-rw-r--r--   0        0        0    13363 2022-12-13 01:58:51.485738 rockset-2.0.0/rockset/model/role.py
+-rw-r--r--   0        0        0    11741 2022-12-13 01:58:51.487202 rockset-2.0.0/rockset/model/role_response.py
+-rw-r--r--   0        0        0    14982 2022-12-13 01:58:51.488257 rockset-2.0.0/rockset/model/s3_collection_creation_request.py
+-rw-r--r--   0        0        0    12154 2022-12-13 01:58:51.489532 rockset-2.0.0/rockset/model/s3_integration.py
+-rw-r--r--   0        0        0    12394 2022-12-13 01:58:51.491627 rockset-2.0.0/rockset/model/s3_integration_creation_request.py
+-rw-r--r--   0        0        0    15239 2022-12-13 01:58:51.492470 rockset-2.0.0/rockset/model/s3_source_wrapper.py
+-rw-r--r--   0        0        0    12201 2022-12-13 01:58:51.493440 rockset-2.0.0/rockset/model/schema_registry_config.py
+-rw-r--r--   0        0        0    11696 2022-12-13 01:58:51.494236 rockset-2.0.0/rockset/model/segment_integration.py
+-rw-r--r--   0        0        0    12465 2022-12-13 01:58:51.495198 rockset-2.0.0/rockset/model/segment_integration_creation_request.py
+-rw-r--r--   0        0        0    15052 2022-12-13 01:58:51.495692 rockset-2.0.0/rockset/model/snowflake_collection_creation_request.py
+-rw-r--r--   0        0        0    14450 2022-12-13 01:58:51.496199 rockset-2.0.0/rockset/model/snowflake_integration.py
+-rw-r--r--   0        0        0    12499 2022-12-13 01:58:51.496726 rockset-2.0.0/rockset/model/snowflake_integration_creation_request.py
+-rw-r--r--   0        0        0    13907 2022-12-13 01:58:51.497226 rockset-2.0.0/rockset/model/snowflake_source_wrapper.py
+-rw-r--r--   0        0        0    12501 2022-12-13 01:58:51.498002 rockset-2.0.0/rockset/model/source.py
+-rw-r--r--   0        0        0    13169 2022-12-13 01:58:51.498911 rockset-2.0.0/rockset/model/source_azure_blob_storage.py
+-rw-r--r--   0        0        0    12664 2022-12-13 01:58:51.499899 rockset-2.0.0/rockset/model/source_azure_event_hubs.py
+-rw-r--r--   0        0        0    12552 2022-12-13 01:58:51.500742 rockset-2.0.0/rockset/model/source_azure_service_bus.py
+-rw-r--r--   0        0        0    13624 2022-12-13 01:58:51.502104 rockset-2.0.0/rockset/model/source_dynamo_db.py
+-rw-r--r--   0        0        0    12391 2022-12-13 01:58:51.506381 rockset-2.0.0/rockset/model/source_file_upload.py
+-rw-r--r--   0        0        0    13371 2022-12-13 01:58:51.507531 rockset-2.0.0/rockset/model/source_gcs.py
+-rw-r--r--   0        0        0    13209 2022-12-13 01:58:51.509226 rockset-2.0.0/rockset/model/source_kafka.py
+-rw-r--r--   0        0        0    13024 2022-12-13 01:58:51.510021 rockset-2.0.0/rockset/model/source_kinesis.py
+-rw-r--r--   0        0        0    12652 2022-12-13 01:58:51.510772 rockset-2.0.0/rockset/model/source_mongo_db.py
+-rw-r--r--   0        0        0    13923 2022-12-13 01:58:51.511460 rockset-2.0.0/rockset/model/source_s3.py
+-rw-r--r--   0        0        0    13110 2022-12-13 01:58:51.511957 rockset-2.0.0/rockset/model/source_snowflake.py
+-rw-r--r--   0        0        0    11661 2022-12-13 01:58:51.512868 rockset-2.0.0/rockset/model/sql_expression.py
+-rw-r--r--   0        0        0    13116 2022-12-13 01:58:51.513635 rockset-2.0.0/rockset/model/stats.py
+-rw-r--r--   0        0        0    13658 2023-05-12 17:22:21.008906 rockset-2.0.0/rockset/model/status.py
+-rw-r--r--   0        0        0    13111 2022-12-13 01:58:51.515374 rockset-2.0.0/rockset/model/status_azure_event_hubs.py
+-rw-r--r--   0        0        0    12364 2022-12-13 01:58:51.516105 rockset-2.0.0/rockset/model/status_azure_event_hubs_partition.py
+-rw-r--r--   0        0        0    12727 2022-12-13 01:58:51.516913 rockset-2.0.0/rockset/model/status_azure_service_bus.py
+-rw-r--r--   0        0        0    12210 2022-12-13 01:58:51.517709 rockset-2.0.0/rockset/model/status_azure_service_bus_session.py
+-rw-r--r--   0        0        0    13563 2022-12-13 01:58:51.518336 rockset-2.0.0/rockset/model/status_dynamo_db.py
+-rw-r--r--   0        0        0    12705 2022-12-13 01:58:51.519331 rockset-2.0.0/rockset/model/status_dynamo_db_v2.py
+-rw-r--r--   0        0        0    13123 2022-12-13 01:58:51.520073 rockset-2.0.0/rockset/model/status_kafka.py
+-rw-r--r--   0        0        0    12337 2022-12-13 01:58:51.520751 rockset-2.0.0/rockset/model/status_kafka_partition.py
+-rw-r--r--   0        0        0    15614 2022-12-13 01:58:51.521466 rockset-2.0.0/rockset/model/status_mongo_db.py
+-rw-r--r--   0        0        0    11924 2022-12-13 01:58:51.521971 rockset-2.0.0/rockset/model/status_snowflake.py
+-rw-r--r--   0        0        0    11873 2022-12-13 01:58:51.522386 rockset-2.0.0/rockset/model/suspend_virtual_instance_response.py
+-rw-r--r--   0        0        0    11894 2022-12-13 01:58:51.523204 rockset-2.0.0/rockset/model/unsubscribe_preference.py
+-rw-r--r--   0        0        0    12119 2022-12-13 01:58:51.523819 rockset-2.0.0/rockset/model/update_alias_request.py
+-rw-r--r--   0        0        0    11818 2022-12-13 01:58:51.524650 rockset-2.0.0/rockset/model/update_api_key_request.py
+-rw-r--r--   0        0        0    11780 2022-12-13 01:58:51.525248 rockset-2.0.0/rockset/model/update_api_key_response.py
+-rw-r--r--   0        0        0    11867 2022-12-13 01:58:51.525826 rockset-2.0.0/rockset/model/update_integration_request.py
+-rw-r--r--   0        0        0    11829 2022-12-13 01:58:51.526397 rockset-2.0.0/rockset/model/update_integration_response.py
+-rw-r--r--   0        0        0    12329 2022-12-13 01:58:51.526916 rockset-2.0.0/rockset/model/update_query_lambda_request.py
+-rw-r--r--   0        0        0    12222 2022-12-13 01:58:51.527531 rockset-2.0.0/rockset/model/update_role_request.py
+-rw-r--r--   0        0        0    12006 2022-12-13 01:58:51.528227 rockset-2.0.0/rockset/model/update_unsubscribe_preferences_request.py
+-rw-r--r--   0        0        0    12009 2022-12-13 01:58:51.528766 rockset-2.0.0/rockset/model/update_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    12206 2022-12-13 01:58:51.529107 rockset-2.0.0/rockset/model/update_user_request.py
+-rw-r--r--   0        0        0    11958 2022-12-13 01:58:51.529732 rockset-2.0.0/rockset/model/update_view_request.py
+-rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.530315 rockset-2.0.0/rockset/model/update_view_response.py
+-rw-r--r--   0        0        0    13762 2022-12-13 01:58:51.531030 rockset-2.0.0/rockset/model/update_virtual_instance_request.py
+-rw-r--r--   0        0        0    11870 2022-12-13 01:58:51.531710 rockset-2.0.0/rockset/model/update_virtual_instance_response.py
+-rw-r--r--   0        0        0    12907 2022-12-13 01:58:51.532928 rockset-2.0.0/rockset/model/user.py
+-rw-r--r--   0        0        0    12155 2022-12-13 01:58:51.533563 rockset-2.0.0/rockset/model/validate_query_response.py
+-rw-r--r--   0        0        0    14473 2022-12-13 01:58:51.534222 rockset-2.0.0/rockset/model/view.py
+-rw-r--r--   0        0        0    17180 2022-12-13 01:58:51.535531 rockset-2.0.0/rockset/model/virtual_instance.py
+-rw-r--r--   0        0        0    11772 2022-12-13 01:58:51.536198 rockset-2.0.0/rockset/model/virtual_instance_stats.py
+-rw-r--r--   0        0        0    12971 2022-12-13 01:58:51.537165 rockset-2.0.0/rockset/model/workspace.py
+-rw-r--r--   0        0        0    12998 2022-12-13 01:58:51.537919 rockset-2.0.0/rockset/model/xml_params.py
+-rw-r--r--   0        0        0    84037 2022-12-13 01:58:51.539401 rockset-2.0.0/rockset/model_utils.py
+-rw-r--r--   0        0        0    14505 2023-05-12 17:22:21.013772 rockset-2.0.0/rockset/models/__init__.py
+-rw-r--r--   0        0        0     1819 2022-12-13 01:58:42.845037 rockset-2.0.0/rockset/query_paginator.py
+-rw-r--r--   0        0        0    14645 2022-12-13 01:58:51.541699 rockset-2.0.0/rockset/rest.py
+-rw-r--r--   0        0        0     8491 2022-12-13 01:58:51.542775 rockset-2.0.0/rockset/rockset_client.py
+-rw-r--r--   0        0        0     3644 2022-12-13 01:58:42.847883 rockset-2.0.0/rockset/value.py
+-rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 rockset-2.0.0/PKG-INFO
```

### Comparing `rockset-1.0.5/pyproject.toml` & `rockset-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "rockset"
-version = "1.0.5"
+version = "2.0.0"
 description = "The python client for the Rockset API."
 authors = ["Rockset <support@rockset.com>"]
 packages = [
     {include = "rockset"}
 ]
 documentation = "https://github.com/rockset/rockset-python-client"
 repository = "https://github.com/rockset/rockset-python-client"
 readme = "LONG_DESCRIPTION.rst"
-license = "BSD License"
+license = "Apache-2.0"
 classifiers = [
-    "License :: OSI Approved :: BSD License",
     "Environment :: Console",
     "Environment :: Other Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.6",
```

### Comparing `rockset-1.0.5/rockset/__init__.py` & `rockset-2.0.0/rockset/__init__.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/aliases_api.py` & `rockset-2.0.0/rockset/api/aliases_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/api_keys_api.py` & `rockset-2.0.0/rockset/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/collections_api.py` & `rockset-2.0.0/rockset/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/custom_roles_api.py` & `rockset-2.0.0/rockset/api/custom_roles_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/documents_api.py` & `rockset-2.0.0/rockset/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/integrations_api.py` & `rockset-2.0.0/rockset/api/integrations_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/organizations_api.py` & `rockset-2.0.0/rockset/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/queries_api.py` & `rockset-2.0.0/rockset/api/queries_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/query_lambdas_api.py` & `rockset-2.0.0/rockset/api/query_lambdas_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/shared_lambdas_api.py` & `rockset-2.0.0/rockset/api/shared_lambdas_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/users_api.py` & `rockset-2.0.0/rockset/api/users_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/views_api.py` & `rockset-2.0.0/rockset/api/views_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/virtual_instances_api.py` & `rockset-2.0.0/rockset/api/virtual_instances_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api/workspaces_api.py` & `rockset-2.0.0/rockset/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/api_client.py` & `rockset-2.0.0/rockset/api_client.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/apis/__init__.py` & `rockset-2.0.0/rockset/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/configuration.py` & `rockset-2.0.0/rockset/configuration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/document.py` & `rockset-2.0.0/rockset/document.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/exceptions.py` & `rockset-2.0.0/rockset/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/add_documents_request.py` & `rockset-2.0.0/rockset/model/add_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/add_documents_response.py` & `rockset-2.0.0/rockset/model/add_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/alias.py` & `rockset-2.0.0/rockset/model/alias.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/api_key.py` & `rockset-2.0.0/rockset/model/api_key.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/async_query_options.py` & `rockset-2.0.0/rockset/model/async_query_options.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/aws_access_key.py` & `rockset-2.0.0/rockset/model/aws_access_key.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/aws_role.py` & `rockset-2.0.0/rockset/model/aws_role.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_blob_storage_collection_creation_request.py` & `rockset-2.0.0/rockset/model/azure_blob_storage_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_blob_storage_integration.py` & `rockset-2.0.0/rockset/model/azure_blob_storage_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_blob_storage_integration_creation_request.py` & `rockset-2.0.0/rockset/model/azure_blob_storage_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_blob_storage_source_wrapper.py` & `rockset-2.0.0/rockset/model/azure_blob_storage_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_event_hubs_collection_creation_request.py` & `rockset-2.0.0/rockset/model/azure_event_hubs_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_event_hubs_integration.py` & `rockset-2.0.0/rockset/model/azure_event_hubs_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_event_hubs_integration_creation_request.py` & `rockset-2.0.0/rockset/model/azure_event_hubs_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_event_hubs_source_wrapper.py` & `rockset-2.0.0/rockset/model/azure_event_hubs_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_service_bus_collection_creation_request.py` & `rockset-2.0.0/rockset/model/azure_service_bus_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_service_bus_integration.py` & `rockset-2.0.0/rockset/model/azure_service_bus_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/azure_service_bus_source_wrapper.py` & `rockset-2.0.0/rockset/model/azure_service_bus_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/bulk_stats.py` & `rockset-2.0.0/rockset/model/bulk_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/cancel_query_response.py` & `rockset-2.0.0/rockset/model/cancel_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/cluster.py` & `rockset-2.0.0/rockset/model/cluster.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/collection.py` & `rockset-2.0.0/rockset/model/collection.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/collection_mount.py` & `rockset-2.0.0/rockset/model/collection_mount.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/collection_mount_response.py` & `rockset-2.0.0/rockset/model/collection_mount_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/collection_mount_stats.py` & `rockset-2.0.0/rockset/model/collection_mount_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/collection_stats.py` & `rockset-2.0.0/rockset/model/collection_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_alias_request.py` & `rockset-2.0.0/rockset/model/create_alias_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_alias_response.py` & `rockset-2.0.0/rockset/model/create_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_api_key_request.py` & `rockset-2.0.0/rockset/model/create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_api_key_response.py` & `rockset-2.0.0/rockset/model/create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_collection_mount_request.py` & `rockset-2.0.0/rockset/model/create_collection_mount_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_collection_mounts_response.py` & `rockset-2.0.0/rockset/model/create_collection_mounts_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_collection_request.py` & `rockset-2.0.0/rockset/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_collection_response.py` & `rockset-2.0.0/rockset/model/create_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_integration_request.py` & `rockset-2.0.0/rockset/model/create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_integration_response.py` & `rockset-2.0.0/rockset/model/create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_query_lambda_request.py` & `rockset-2.0.0/rockset/model/create_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_query_lambda_tag_request.py` & `rockset-2.0.0/rockset/model/create_query_lambda_tag_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_role_request.py` & `rockset-2.0.0/rockset/model/create_role_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_user_request.py` & `rockset-2.0.0/rockset/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_user_response.py` & `rockset-2.0.0/rockset/model/create_user_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_view_request.py` & `rockset-2.0.0/rockset/model/create_view_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_view_response.py` & `rockset-2.0.0/rockset/model/create_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_virtual_instance_request.py` & `rockset-2.0.0/rockset/model/create_virtual_instance_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_virtual_instance_response.py` & `rockset-2.0.0/rockset/model/create_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_workspace_request.py` & `rockset-2.0.0/rockset/model/create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/create_workspace_response.py` & `rockset-2.0.0/rockset/model/create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/csv_params.py` & `rockset-2.0.0/rockset/model/csv_params.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_alias_response.py` & `rockset-2.0.0/rockset/model/delete_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_api_key_response.py` & `rockset-2.0.0/rockset/model/delete_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_collection_response.py` & `rockset-2.0.0/rockset/model/delete_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_documents_request.py` & `rockset-2.0.0/rockset/model/delete_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_documents_request_data.py` & `rockset-2.0.0/rockset/model/delete_documents_request_data.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_documents_response.py` & `rockset-2.0.0/rockset/model/delete_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_integration_response.py` & `rockset-2.0.0/rockset/model/delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_query_lambda_response.py` & `rockset-2.0.0/rockset/model/delete_query_lambda_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_user_response.py` & `rockset-2.0.0/rockset/model/delete_user_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_view_response.py` & `rockset-2.0.0/rockset/model/delete_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_virtual_instance_response.py` & `rockset-2.0.0/rockset/model/delete_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/delete_workspace_response.py` & `rockset-2.0.0/rockset/model/delete_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/document_status.py` & `rockset-2.0.0/rockset/model/document_status.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/dynamodb_collection_creation_request.py` & `rockset-2.0.0/rockset/model/dynamodb_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/dynamodb_integration.py` & `rockset-2.0.0/rockset/model/dynamodb_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/dynamodb_integration_creation_request.py` & `rockset-2.0.0/rockset/model/dynamodb_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/dynamodb_source_wrapper.py` & `rockset-2.0.0/rockset/model/dynamodb_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/error_model.py` & `rockset-2.0.0/rockset/model/error_model.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/event_time_info.py` & `rockset-2.0.0/rockset/model/event_time_info.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/execute_public_query_lambda_request.py` & `rockset-2.0.0/rockset/model/execute_public_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/execute_query_lambda_request.py` & `rockset-2.0.0/rockset/model/execute_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/field_mapping_query.py` & `rockset-2.0.0/rockset/model/field_mapping_query.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/field_mapping_v2.py` & `rockset-2.0.0/rockset/model/field_mapping_v2.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/field_partition.py` & `rockset-2.0.0/rockset/model/field_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/file_upload_collection_creation_request.py` & `rockset-2.0.0/rockset/model/file_upload_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/file_upload_source_wrapper.py` & `rockset-2.0.0/rockset/model/file_upload_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/format_params.py` & `rockset-2.0.0/rockset/model/format_params.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/gcp_service_account.py` & `rockset-2.0.0/rockset/model/gcp_service_account.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/gcs_collection_creation_request.py` & `rockset-2.0.0/rockset/model/gcs_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/gcs_integration.py` & `rockset-2.0.0/rockset/model/gcs_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/gcs_integration_creation_request.py` & `rockset-2.0.0/rockset/model/gcs_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/gcs_source_wrapper.py` & `rockset-2.0.0/rockset/model/gcs_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/get_alias_response.py` & `rockset-2.0.0/rockset/model/get_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/get_api_key_response.py` & `rockset-2.0.0/rockset/model/get_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/get_collection_response.py` & `rockset-2.0.0/rockset/model/get_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/get_integration_response.py` & `rockset-2.0.0/rockset/model/get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/get_query_response.py` & `rockset-2.0.0/rockset/model/get_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/get_view_response.py` & `rockset-2.0.0/rockset/model/get_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/get_virtual_instance_response.py` & `rockset-2.0.0/rockset/model/get_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/get_workspace_response.py` & `rockset-2.0.0/rockset/model/get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/input_field.py` & `rockset-2.0.0/rockset/model/input_field.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/integration.py` & `rockset-2.0.0/rockset/model/integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kafka_collection_creation_request.py` & `rockset-2.0.0/rockset/model/kafka_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kafka_integration.py` & `rockset-2.0.0/rockset/model/kafka_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kafka_integration_creation_request.py` & `rockset-2.0.0/rockset/model/kafka_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kafka_source_wrapper.py` & `rockset-2.0.0/rockset/model/kafka_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kafka_v3_security_config.py` & `rockset-2.0.0/rockset/model/kafka_v3_security_config.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kinesis_collection_creation_request.py` & `rockset-2.0.0/rockset/model/kinesis_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kinesis_integration.py` & `rockset-2.0.0/rockset/model/kinesis_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kinesis_integration_creation_request.py` & `rockset-2.0.0/rockset/model/kinesis_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/kinesis_source_wrapper.py` & `rockset-2.0.0/rockset/model/kinesis_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_aliases_response.py` & `rockset-2.0.0/rockset/model/list_aliases_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_api_keys_response.py` & `rockset-2.0.0/rockset/model/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_collection_mounts_response.py` & `rockset-2.0.0/rockset/model/list_collection_mounts_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_collections_response.py` & `rockset-2.0.0/rockset/model/list_collections_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_integrations_response.py` & `rockset-2.0.0/rockset/model/list_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_queries_response.py` & `rockset-2.0.0/rockset/model/list_queries_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_query_lambda_tags_response.py` & `rockset-2.0.0/rockset/model/list_query_lambda_tags_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_query_lambda_versions_response.py` & `rockset-2.0.0/rockset/model/list_query_lambda_versions_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_query_lambdas_response.py` & `rockset-2.0.0/rockset/model/list_query_lambdas_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_roles_response.py` & `rockset-2.0.0/rockset/model/list_roles_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_unsubscribe_preferences_response.py` & `rockset-2.0.0/rockset/model/list_unsubscribe_preferences_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_users_response.py` & `rockset-2.0.0/rockset/model/list_users_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_views_response.py` & `rockset-2.0.0/rockset/model/list_views_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_virtual_instances_response.py` & `rockset-2.0.0/rockset/model/list_virtual_instances_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/list_workspaces_response.py` & `rockset-2.0.0/rockset/model/list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/mongo_db_integration.py` & `rockset-2.0.0/rockset/model/mongo_db_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/mongodb_collection_creation_request.py` & `rockset-2.0.0/rockset/model/mongodb_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/mongodb_integration_creation_request.py` & `rockset-2.0.0/rockset/model/mongodb_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/mongodb_source_wrapper.py` & `rockset-2.0.0/rockset/model/mongodb_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/organization.py` & `rockset-2.0.0/rockset/model/organization.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/organization_response.py` & `rockset-2.0.0/rockset/model/organization_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/output_field.py` & `rockset-2.0.0/rockset/model/output_field.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/pagination.py` & `rockset-2.0.0/rockset/model/pagination.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/pagination_info.py` & `rockset-2.0.0/rockset/model/pagination_info.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/patch_document.py` & `rockset-2.0.0/rockset/model/patch_document.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/patch_documents_request.py` & `rockset-2.0.0/rockset/model/patch_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/patch_documents_response.py` & `rockset-2.0.0/rockset/model/patch_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/patch_operation.py` & `rockset-2.0.0/rockset/model/patch_operation.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/privilege.py` & `rockset-2.0.0/rockset/model/privilege.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_error.py` & `rockset-2.0.0/rockset/model/query_error.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_field_type.py` & `rockset-2.0.0/rockset/model/query_field_type.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_info.py` & `rockset-2.0.0/rockset/model/query_info.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_lambda.py` & `rockset-2.0.0/rockset/model/query_lambda.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_lambda_sql.py` & `rockset-2.0.0/rockset/model/query_lambda_sql.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_lambda_stats.py` & `rockset-2.0.0/rockset/model/query_lambda_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_lambda_tag.py` & `rockset-2.0.0/rockset/model/query_lambda_tag.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_lambda_tag_response.py` & `rockset-2.0.0/rockset/model/query_lambda_tag_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_lambda_version.py` & `rockset-2.0.0/rockset/model/query_lambda_version.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_lambda_version_response.py` & `rockset-2.0.0/rockset/model/query_lambda_version_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_pagination_response.py` & `rockset-2.0.0/rockset/model/query_pagination_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
+from rockset.document import Document
 
 
 def lazy_import():
     from rockset.model.pagination_info import PaginationInfo
     globals()['PaginationInfo'] = PaginationInfo
 
 
@@ -177,14 +178,17 @@
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
+            if var_name == "results":
+                setattr(self, "results", [Document(doc) for doc in var_value])
+                continue
             setattr(self, var_name, var_value)
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
@@ -260,12 +264,15 @@
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
+            if var_name == "results":
+                setattr(self, "results", [Document(doc) for doc in var_value])
+                continue
             setattr(self, var_name, var_value)
             # todo: remove these comments - this stops the user from setting read only vars but we need this now to address a bug
             # if var_name in self.read_only_vars:
             #     raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
             #                          f"class with read only attributes.")
```

### Comparing `rockset-1.0.5/rockset/model/query_parameter.py` & `rockset-2.0.0/rockset/model/query_parameter.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_request.py` & `rockset-2.0.0/rockset/model/query_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_request_sql.py` & `rockset-2.0.0/rockset/model/query_request_sql.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_response.py` & `rockset-2.0.0/rockset/model/query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/query_response_stats.py` & `rockset-2.0.0/rockset/model/query_response_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/resume_virtual_instance_response.py` & `rockset-2.0.0/rockset/model/resume_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/role.py` & `rockset-2.0.0/rockset/model/role.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/role_response.py` & `rockset-2.0.0/rockset/model/role_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/s3_collection_creation_request.py` & `rockset-2.0.0/rockset/model/s3_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/s3_integration.py` & `rockset-2.0.0/rockset/model/s3_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/s3_integration_creation_request.py` & `rockset-2.0.0/rockset/model/s3_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/s3_source_wrapper.py` & `rockset-2.0.0/rockset/model/s3_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/schema_registry_config.py` & `rockset-2.0.0/rockset/model/schema_registry_config.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/segment_integration.py` & `rockset-2.0.0/rockset/model/segment_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/segment_integration_creation_request.py` & `rockset-2.0.0/rockset/model/segment_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/snowflake_collection_creation_request.py` & `rockset-2.0.0/rockset/model/snowflake_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/snowflake_integration.py` & `rockset-2.0.0/rockset/model/snowflake_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/snowflake_integration_creation_request.py` & `rockset-2.0.0/rockset/model/snowflake_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/snowflake_source_wrapper.py` & `rockset-2.0.0/rockset/model/snowflake_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source.py` & `rockset-2.0.0/rockset/model/source.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_azure_blob_storage.py` & `rockset-2.0.0/rockset/model/source_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_azure_event_hubs.py` & `rockset-2.0.0/rockset/model/source_azure_event_hubs.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_azure_service_bus.py` & `rockset-2.0.0/rockset/model/source_azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_dynamo_db.py` & `rockset-2.0.0/rockset/model/source_dynamo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_file_upload.py` & `rockset-2.0.0/rockset/model/source_file_upload.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_gcs.py` & `rockset-2.0.0/rockset/model/source_gcs.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_kafka.py` & `rockset-2.0.0/rockset/model/source_kafka.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_kinesis.py` & `rockset-2.0.0/rockset/model/source_kinesis.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_mongo_db.py` & `rockset-2.0.0/rockset/model/source_mongo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_s3.py` & `rockset-2.0.0/rockset/model/source_s3.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/source_snowflake.py` & `rockset-2.0.0/rockset/model/source_snowflake.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/sql_expression.py` & `rockset-2.0.0/rockset/model/sql_expression.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/stats.py` & `rockset-2.0.0/rockset/model/stats.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status.py` & `rockset-2.0.0/rockset/model/status.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_azure_event_hubs.py` & `rockset-2.0.0/rockset/model/status_azure_event_hubs.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_azure_event_hubs_partition.py` & `rockset-2.0.0/rockset/model/status_azure_event_hubs_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_azure_service_bus.py` & `rockset-2.0.0/rockset/model/status_azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_azure_service_bus_session.py` & `rockset-2.0.0/rockset/model/status_azure_service_bus_session.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_dynamo_db.py` & `rockset-2.0.0/rockset/model/status_dynamo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_dynamo_db_v2.py` & `rockset-2.0.0/rockset/model/status_dynamo_db_v2.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_kafka.py` & `rockset-2.0.0/rockset/model/status_kafka.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_kafka_partition.py` & `rockset-2.0.0/rockset/model/status_kafka_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_mongo_db.py` & `rockset-2.0.0/rockset/model/status_mongo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/status_snowflake.py` & `rockset-2.0.0/rockset/model/status_snowflake.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/suspend_virtual_instance_response.py` & `rockset-2.0.0/rockset/model/suspend_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/unsubscribe_preference.py` & `rockset-2.0.0/rockset/model/unsubscribe_preference.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_alias_request.py` & `rockset-2.0.0/rockset/model/update_alias_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_api_key_request.py` & `rockset-2.0.0/rockset/model/update_api_key_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_api_key_response.py` & `rockset-2.0.0/rockset/model/update_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_integration_request.py` & `rockset-2.0.0/rockset/model/update_integration_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_integration_response.py` & `rockset-2.0.0/rockset/model/update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_query_lambda_request.py` & `rockset-2.0.0/rockset/model/update_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_role_request.py` & `rockset-2.0.0/rockset/model/update_role_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_unsubscribe_preferences_request.py` & `rockset-2.0.0/rockset/model/update_unsubscribe_preferences_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_unsubscribe_preferences_response.py` & `rockset-2.0.0/rockset/model/update_unsubscribe_preferences_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_user_request.py` & `rockset-2.0.0/rockset/model/update_user_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_view_request.py` & `rockset-2.0.0/rockset/model/update_view_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_view_response.py` & `rockset-2.0.0/rockset/model/update_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_virtual_instance_request.py` & `rockset-2.0.0/rockset/model/update_virtual_instance_request.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/update_virtual_instance_response.py` & `rockset-2.0.0/rockset/model/update_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/user.py` & `rockset-2.0.0/rockset/model/user.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/validate_query_response.py` & `rockset-2.0.0/rockset/model/validate_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/view.py` & `rockset-2.0.0/rockset/model/view.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/virtual_instance.py` & `rockset-2.0.0/rockset/model/virtual_instance.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/virtual_instance_stats.py` & `rockset-2.0.0/rockset/model/virtual_instance_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/workspace.py` & `rockset-2.0.0/rockset/model/workspace.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model/xml_params.py` & `rockset-2.0.0/rockset/model/xml_params.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/model_utils.py` & `rockset-2.0.0/rockset/model_utils.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/models/__init__.py` & `rockset-2.0.0/rockset/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/query_paginator.py` & `rockset-2.0.0/rockset/query_paginator.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/rest.py` & `rockset-2.0.0/rockset/rest.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/rockset_client.py` & `rockset-2.0.0/rockset/rockset_client.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/rockset/value.py` & `rockset-2.0.0/rockset/value.py`

 * *Files identical despite different names*

### Comparing `rockset-1.0.5/PKG-INFO` & `rockset-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: rockset
-Version: 1.0.5
+Version: 2.0.0
 Summary: The python client for the Rockset API.
 Home-page: https://github.com/rockset/rockset-python-client
-License: BSD License
+License: Apache-2.0
 Author: Rockset
 Author-email: support@rockset.com
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
```

